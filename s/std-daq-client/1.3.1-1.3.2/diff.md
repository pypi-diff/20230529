# Comparing `tmp/std_daq_client-1.3.1.tar.gz` & `tmp/std_daq_client-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.3.1.tar", last modified: Mon May 29 21:38:00 2023, max compression
+gzip compressed data, was "std_daq_client-1.3.2.tar", last modified: Mon May 29 21:46:03 2023, max compression
```

## Comparing `std_daq_client-1.3.1.tar` & `std_daq_client-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.682895 std_daq_client-1.3.1/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:38:00.682732 std_daq_client-1.3.1/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 21:38:00.682932 std_daq_client-1.3.1/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1115 2023-05-29 21:37:40.000000 std_daq_client-1.3.1/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.681986 std_daq_client-1.3.1/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.1/std_daq_client/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)     4851 2023-05-29 21:36:51.000000 std_daq_client-1.3.1/std_daq_client/cli.py
--rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.682587 std_daq_client-1.3.1/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      436 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:46:03.284395 std_daq_client-1.3.2/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:46:03.284237 std_daq_client-1.3.2/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.2/README.md
+-rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 21:46:03.284426 std_daq_client-1.3.2/setup.cfg
+-rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.2/setup.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1115 2023-05-29 21:45:14.000000 std_daq_client-1.3.2/setup_client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:46:03.283514 std_daq_client-1.3.2/std_daq_client/
+-rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.2/std_daq_client/__init__.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     4963 2023-05-29 21:44:57.000000 std_daq_client-1.3.2/std_daq_client/cli.py
+-rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.2/std_daq_client/client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:46:03.284099 std_daq_client-1.3.2/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)      436 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 21:46:03.000000 std_daq_client-1.3.2/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.3.1/PKG-INFO` & `std_daq_client-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std_daq_client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

### Comparing `std_daq_client-1.3.1/README.md` & `std_daq_client-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.1/setup.py` & `std_daq_client-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.1/setup_client.py` & `std_daq_client-1.3.2/setup_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.3.1"
+CLIENT_VERSION = "1.3.2"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
```

### Comparing `std_daq_client-1.3.1/std_daq_client/cli.py` & `std_daq_client-1.3.2/std_daq_client/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     response = client.start_writer_async({'output_file': args.output_file, 'n_images': args.n_images})
 
     print(json.dumps(response, indent=2))
 
 
 def write_stop():
     parser = argparse.ArgumentParser(description='std_daq stop writer')
-    parser.add_argument("-b", type=str, default='http://localhost:5000', help="Base URL of the REST Endpoint")
+    parser.add_argument("-b", type=str, default=os.environ.get('STD_DAQ_API_URL', 'http://127.0.0.1:5000'),
+                        help="Base URL of the REST Endpoint. Read also from environment variable STD_DAQ_API_URL")
     args = parser.parse_args()
 
     client = StdDaqClient(url_base=args.b)
     response = client.stop_writer()
 
     print(json.dumps(response, indent=2))
```

### Comparing `std_daq_client-1.3.1/std_daq_client/client.py` & `std_daq_client-1.3.2/std_daq_client/client.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.1/std_daq_client.egg-info/PKG-INFO` & `std_daq_client-1.3.2/std_daq_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std-daq-client
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

