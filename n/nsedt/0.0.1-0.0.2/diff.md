# Comparing `tmp/nsedt-0.0.1.tar.gz` & `tmp/nsedt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsedt-0.0.1.tar", last modified: Fri May 26 11:59:26 2023, max compression
+gzip compressed data, was "nsedt-0.0.2.tar", last modified: Mon May 29 14:52:13 2023, max compression
```

## Comparing `nsedt-0.0.1.tar` & `nsedt-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:26.796768 nsedt-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 11:59:13.000000 nsedt-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-26 11:59:26.796768 nsedt-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-26 11:59:13.000000 nsedt-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:26.796768 nsedt-0.0.1/nsedt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/equity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:26.796768 nsedt-0.0.1/nsedt/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/resources/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:26.796768 nsedt-0.0.1/nsedt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-26 11:59:13.000000 nsedt-0.0.1/nsedt/utils/data_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:26.796768 nsedt-0.0.1/nsedt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-26 11:59:26.000000 nsedt-0.0.1/nsedt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 11:59:26.000000 nsedt-0.0.1/nsedt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:59:26.000000 nsedt-0.0.1/nsedt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 11:59:26.000000 nsedt-0.0.1/nsedt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 11:59:26.000000 nsedt-0.0.1/nsedt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 11:59:26.796768 nsedt-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 11:59:13.000000 nsedt-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:51:56.000000 nsedt-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 14:52:13.856552 nsedt-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-29 14:51:56.000000 nsedt-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/equity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/resources/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-29 14:51:56.000000 nsedt-0.0.2/nsedt/utils/data_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:52:13.856552 nsedt-0.0.2/nsedt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 14:52:13.000000 nsedt-0.0.2/nsedt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 14:52:13.856552 nsedt-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 14:51:56.000000 nsedt-0.0.2/setup.py
```

### Comparing `nsedt-0.0.1/LICENSE` & `nsedt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.1/PKG-INFO` & `nsedt-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# nsedt
+# nse data
 
 ---
 ## Run 
 ```py
 from nsedt import equity as eq
 from datetime import date
 
@@ -28,16 +28,17 @@
 print(eq.get_price(start_date, end_date, symbol="TCS"))
 start_date = "01-03-2022"
 end_date = "03-05-2023"
 print(eq.get_corpinfo(start_date, end_date, symbol="TCS"))
 
 ```
 ---
-## O/P
+## Output
 ```sh
+# get_price
         Date  Open Price  High Price  Low Price  Close Price  ...  52 Week High Price  52 Week Low Price     VWAP  Deliverable Volume  Deliverable Percent
 0   2022-01-03      3750.0     3830.00    3745.00      3817.75  ...              3989.9             2880.0  3807.43             1433211                61.09
 ..         ...         ...         ...        ...          ...  ...                 ...                ...      ...                 ...                  ...
 104 2023-01-04      3306.7     3327.35    3286.20      3314.65  ...              4043.0             2926.1  3306.45              778260                63.19
 
 # get_corpinfo
 symbol series ind faceVal                                            subject  ... ndStartDate                               comp          isin ndEndDate caBroadcastDate
```

### Comparing `nsedt-0.0.1/README.md` & `nsedt-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# nsedt
+# nse data
 
 ---
 ## Run 
 ```py
 from nsedt import equity as eq
 from datetime import date
 
@@ -11,16 +11,17 @@
 print(eq.get_price(start_date, end_date, symbol="TCS"))
 start_date = "01-03-2022"
 end_date = "03-05-2023"
 print(eq.get_corpinfo(start_date, end_date, symbol="TCS"))
 
 ```
 ---
-## O/P
+## Output
 ```sh
+# get_price
         Date  Open Price  High Price  Low Price  Close Price  ...  52 Week High Price  52 Week Low Price     VWAP  Deliverable Volume  Deliverable Percent
 0   2022-01-03      3750.0     3830.00    3745.00      3817.75  ...              3989.9             2880.0  3807.43             1433211                61.09
 ..         ...         ...         ...        ...          ...  ...                 ...                ...      ...                 ...                  ...
 104 2023-01-04      3306.7     3327.35    3286.20      3314.65  ...              4043.0             2926.1  3306.45              778260                63.19
 
 # get_corpinfo
 symbol series ind faceVal                                            subject  ... ndStartDate                               comp          isin ndEndDate caBroadcastDate
```

### Comparing `nsedt-0.0.1/nsedt/equity.py` & `nsedt-0.0.2/nsedt/equity.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         if input_type == "stock":
             params = {
                 "symbol": symbol,
                 "from": st,
                 "to": et,
                 "dataType": "priceVolumeDeliverable",
-                "series": "ALL",
+                "series": "EQ",
             }
             url = base_url + price_api + urllib.parse.urlencode(params)
             url_list.append(url)
 
         # move the window start to the next day after the current window end
         current_window_start = current_window_end + datetime.timedelta(days=1)
```

### Comparing `nsedt-0.0.1/nsedt/utils/__init__.py` & `nsedt-0.0.2/nsedt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.1/nsedt/utils/data_format.py` & `nsedt-0.0.2/nsedt/utils/data_format.py`

 * *Files identical despite different names*

### Comparing `nsedt-0.0.1/nsedt.egg-info/PKG-INFO` & `nsedt-0.0.2/nsedt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nsedt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to collect NSE data in pandas dataframe
 Home-page: https://github.com/pratik141/nsedt
 Author: Pratik Anand
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# nsedt
+# nse data
 
 ---
 ## Run 
 ```py
 from nsedt import equity as eq
 from datetime import date
 
@@ -28,16 +28,17 @@
 print(eq.get_price(start_date, end_date, symbol="TCS"))
 start_date = "01-03-2022"
 end_date = "03-05-2023"
 print(eq.get_corpinfo(start_date, end_date, symbol="TCS"))
 
 ```
 ---
-## O/P
+## Output
 ```sh
+# get_price
         Date  Open Price  High Price  Low Price  Close Price  ...  52 Week High Price  52 Week Low Price     VWAP  Deliverable Volume  Deliverable Percent
 0   2022-01-03      3750.0     3830.00    3745.00      3817.75  ...              3989.9             2880.0  3807.43             1433211                61.09
 ..         ...         ...         ...        ...          ...  ...                 ...                ...      ...                 ...                  ...
 104 2023-01-04      3306.7     3327.35    3286.20      3314.65  ...              4043.0             2926.1  3306.45              778260                63.19
 
 # get_corpinfo
 symbol series ind faceVal                                            subject  ... ndStartDate                               comp          isin ndEndDate caBroadcastDate
```

### Comparing `nsedt-0.0.1/setup.py` & `nsedt-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name="nsedt",
-    version="0.0.1",
+    version="0.0.2",
     author="Pratik Anand",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Library to collect NSE data in pandas dataframe",
     packages=find_packages(),
     url="https://github.com/pratik141/nsedt",
     install_requires=[
```

