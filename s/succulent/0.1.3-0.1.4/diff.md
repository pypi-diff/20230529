# Comparing `tmp/succulent-0.1.3.tar.gz` & `tmp/succulent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.1.3.tar", max compression
+gzip compressed data, was "succulent-0.1.4.tar", max compression
```

## Comparing `succulent-0.1.3.tar` & `succulent-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.1.3/LICENSE
--rw-r--r--   0        0        0      708 2023-05-23 08:21:11.992508 succulent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3312 2023-05-22 11:55:26.967092 succulent-0.1.3/README.md
--rw-r--r--   0        0        0      113 2023-05-23 08:21:18.000152 succulent-0.1.3/succulent/__init__.py
--rw-r--r--   0        0        0     1763 2023-05-22 07:54:07.348467 succulent-0.1.3/succulent/api.py
--rw-r--r--   0        0        0      362 2023-05-23 08:16:56.463862 succulent-0.1.3/succulent/configuration.py
--rw-r--r--   0        0        0      140 2023-05-22 07:35:30.619588 succulent-0.1.3/succulent/main.py
--rw-r--r--   0        0        0     2606 2023-05-23 08:15:58.780537 succulent-0.1.3/succulent/processing.py
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 succulent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-04-18 11:02:21.268343 succulent-0.1.4/LICENSE
+-rw-r--r--   0        0        0      708 2023-05-29 13:22:43.505543 succulent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5841 2023-05-29 13:24:59.974193 succulent-0.1.4/README.md
+-rw-r--r--   0        0        0      113 2023-05-29 13:22:52.395173 succulent-0.1.4/succulent/__init__.py
+-rw-r--r--   0        0        0     1710 2023-05-28 20:27:47.551677 succulent-0.1.4/succulent/api.py
+-rw-r--r--   0        0        0      362 2023-05-24 09:55:47.296058 succulent-0.1.4/succulent/configuration.py
+-rw-r--r--   0        0        0     3717 2023-05-29 10:37:54.556319 succulent-0.1.4/succulent/processing.py
+-rw-r--r--   0        0        0     6570 1970-01-01 00:00:00.000000 succulent-0.1.4/PKG-INFO
```

### Comparing `succulent-0.1.3/LICENSE` & `succulent-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `succulent-0.1.3/pyproject.toml` & `succulent-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "succulent"
-version = "0.1.3"
+version = "0.1.4"
 description = "Collect POST requests easily"
 license = "MIT"
 authors = ["Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Tadej Lahovnik <lahovnik.tadej@gmail.com>"]
 keywords = ['data collection', 'data science', 'sensor measurements']
 homepage = "https://github.com/firefly-cpp/succulent"
 repository = "https://github.com/firefly-cpp/succulent"
 readme = "README.md"
```

### Comparing `succulent-0.1.3/succulent/api.py` & `succulent-0.1.4/succulent/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,16 @@
             # Process request
             self.processing.process(request)
             
             # Collect and store timestamp
             timestamp = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             # You can store the timestamp in a database, file, or any other desired storage mechanism.
             # Example: database.insert_timestamp(timestamp)
-        except ValueError:
+        except ValueError as err:
             # Invalid file type
-            return jsonify({'message': f'Invalid file type: {self.format}. Supported file types: csv, json'}), 400
+            return jsonify({'message': str(err)}), 400
 
         # Send response
         return jsonify({'message': 'Data stored', 'timestamp': timestamp}), 200
 
     def start(self):
         self.app.run(host=self.host, port=self.port)
```

### Comparing `succulent-0.1.3/succulent/processing.py` & `succulent-0.1.4/succulent/processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 import os
 import sqlite3
 import inspect
 import pandas as pd
 
 class Processing:
     def __init__(self, config, format):
+        # Validate format
+        if format not in ['csv', 'json', 'sqlite']:
+            raise ValueError(f'Invalid format: {format}')
+        
+        # Initialise attributes
         self.directory = os.path.join(os.path.dirname(os.path.abspath(inspect.stack()[2].filename)), 'data')
         self.format = format
         self.columns = [configuration['name'] for configuration in config]
+        self.boundaries = [{ 
+            configuration['name']: {
+                key: configuration[key]
+                for key in ['min', 'max']
+                if key in configuration
+            }
+        } for configuration in config if configuration.get('min') is not None or configuration.get('max') is not None]
         self.df = None  # Initialize df attribute
     
     def parameters(self):
         parameters = [f'{column}=' for column in self.columns]
         parameters = '&'.join(parameters)
         return parameters
+    
+    def boundary(self, value, boundary, column):
+        if 'min' in boundary and float(value) < float(boundary['min']):
+            raise ValueError(f'{column} ({value}) is lower than the specified minimum ({boundary["min"]}).')
+        if 'max' in boundary and float(value) > float(boundary['max']):
+            raise ValueError(f'{column} ({value}) is greater than the specified maximum ({boundary["max"]}).')
+        return value
         
     def process(self, req):
         # Directory preparation
         if not os.path.exists(self.directory):
             os.makedirs(self.directory)
 
         # Define paths
@@ -39,35 +58,36 @@
                 raise ValueError(f'Invalid file type: {self.format}')
         # Initialise new data
         else:
             self.df = pd.DataFrame(columns=self.columns)
 
         # Parse data from request
         data = {}
-        if req.is_json:
-            for column in self.columns:
-                try:
-                    data[column] = req.json[column]
-                except:
-                    data[column] = None
-        else:
-            for column in self.columns:
-                try: 
-                    data[column] = str(req.args.get(column, default=''))
-                except:
-                    data[column] = ''
+        for column in self.columns:
+            # Request type
+            if req.is_json:
+                value = req.json[column] if column in req.json else None
+            else:
+                value = req.args.get(column, default=None)
+
+            # Boundary check
+            if column in [list(boundaries.keys())[0] for boundaries in self.boundaries]:
+                index = [list(boundaries.keys())[0] for boundaries in self.boundaries].index(column)
+                data[column] = self.boundary(value, self.boundaries[index][column], column)
+            else:
+                data[column] = value
+
+        # Convert data to Series
         data = pd.Series(data, index=self.columns)
 
         # Merge data
         self.df = pd.concat([self.df, data.to_frame().T], ignore_index=True)
 
         # Store data to device
         if self.format == 'csv':
             self.df.to_csv(path, sep=',', index=False)
         elif self.format == 'json':
             self.df.to_json(path, orient='records', indent=4)
         elif self.format == 'sqlite':
             conn = sqlite3.connect(path)
             self.df.to_sql('data', conn, if_exists='replace', index=False)
-            conn.close()
-        else:
-            raise ValueError(f'Invalid format: {self.format}')
+            conn.close()
```

