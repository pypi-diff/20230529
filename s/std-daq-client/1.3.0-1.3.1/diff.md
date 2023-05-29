# Comparing `tmp/std_daq_client-1.3.0.tar.gz` & `tmp/std_daq_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.3.0.tar", last modified: Mon May 29 21:34:34 2023, max compression
+gzip compressed data, was "std_daq_client-1.3.1.tar", last modified: Mon May 29 21:38:00 2023, max compression
```

## Comparing `std_daq_client-1.3.0.tar` & `std_daq_client-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:34:34.295508 std_daq_client-1.3.0/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:34:34.295326 std_daq_client-1.3.0/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.0/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 21:34:34.295537 std_daq_client-1.3.0/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.0/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1115 2023-05-29 21:33:39.000000 std_daq_client-1.3.0/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:34:34.294568 std_daq_client-1.3.0/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.0/std_daq_client/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)     4879 2023-05-29 21:27:28.000000 std_daq_client-1.3.0/std_daq_client/cli.py
--rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.0/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:34:34.295165 std_daq_client-1.3.0/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      436 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 21:34:34.000000 std_daq_client-1.3.0/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.682895 std_daq_client-1.3.1/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:38:00.682732 std_daq_client-1.3.1/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/README.md
+-rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 21:38:00.682932 std_daq_client-1.3.1/setup.cfg
+-rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/setup.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1115 2023-05-29 21:37:40.000000 std_daq_client-1.3.1/setup_client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.681986 std_daq_client-1.3.1/std_daq_client/
+-rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.1/std_daq_client/__init__.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     4851 2023-05-29 21:36:51.000000 std_daq_client-1.3.1/std_daq_client/cli.py
+-rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.1/std_daq_client/client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 21:38:00.682587 std_daq_client-1.3.1/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)      436 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 21:38:00.000000 std_daq_client-1.3.1/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.3.0/PKG-INFO` & `std_daq_client-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std_daq_client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

### Comparing `std_daq_client-1.3.0/README.md` & `std_daq_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.0/setup.py` & `std_daq_client-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.0/setup_client.py` & `std_daq_client-1.3.1/setup_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.3.0"
+CLIENT_VERSION = "1.3.1"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
```

### Comparing `std_daq_client-1.3.0/std_daq_client/cli.py` & `std_daq_client-1.3.1/std_daq_client/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,25 +52,25 @@
 
 def get_stats():
     parser = argparse.ArgumentParser(description='Get std_daq stats')
     parser.add_argument("-b", type=str, default=os.environ.get('STD_DAQ_API_URL', 'http://127.0.0.1:5000'),
                         help="Base URL of the REST Endpoint. Read also from environment variable STD_DAQ_API_URL")
     args = parser.parse_args()
 
-    client = StdDaqClient(url_base=args.url_base)
+    client = StdDaqClient(url_base=args.b)
     print(json.dumps(client.get_stats(), indent=2))
 
 
 def get_status():
     parser = argparse.ArgumentParser(description='Get std_daq status')
     parser.add_argument("-b", type=str, default=os.environ.get('STD_DAQ_API_URL', 'http://127.0.0.1:5000'),
                         help="Base URL of the REST Endpoint. Read also from environment variable STD_DAQ_API_URL")
     args = parser.parse_args()
 
-    client = StdDaqClient(url_base=args.url_base)
+    client = StdDaqClient(url_base=args.b)
     print(json.dumps(client.get_status(), indent=2))
 
 
 def write_sync():
     parser = argparse.ArgumentParser(description='Start std_daq sync write')
     parser.add_argument("-b", type=str, default=os.environ.get('STD_DAQ_API_URL', 'http://127.0.0.1:5000'),
                         help="Base URL of the REST Endpoint. Read also from environment variable STD_DAQ_API_URL")
@@ -96,14 +96,14 @@
     response = client.start_writer_async({'output_file': args.output_file, 'n_images': args.n_images})
 
     print(json.dumps(response, indent=2))
 
 
 def write_stop():
     parser = argparse.ArgumentParser(description='std_daq stop writer')
-    parser.add_argument("--url_base", type=str, default='http://localhost:5000', help="Base URL of the REST Endpoint")
-    url_base = parser.parse_args().url_base
+    parser.add_argument("-b", type=str, default='http://localhost:5000', help="Base URL of the REST Endpoint")
+    args = parser.parse_args()
 
-    client = StdDaqClient(url_base)
+    client = StdDaqClient(url_base=args.b)
     response = client.stop_writer()
 
     print(json.dumps(response, indent=2))
```

### Comparing `std_daq_client-1.3.0/std_daq_client/client.py` & `std_daq_client-1.3.1/std_daq_client/client.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.0/std_daq_client.egg-info/PKG-INFO` & `std_daq_client-1.3.1/std_daq_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: std-daq-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

