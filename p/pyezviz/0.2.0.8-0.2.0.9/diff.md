# Comparing `tmp/pyezviz-0.2.0.8.tar.gz` & `tmp/pyezviz-0.2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.0.8.tar", last modified: Wed Apr 27 14:05:38 2022, max compression
+gzip compressed data, was "pyezviz-0.2.0.9.tar", last modified: Fri Jul  8 18:50:33 2022, max compression
```

## Comparing `pyezviz-0.2.0.8.tar` & `pyezviz-0.2.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:05:38.289149 pyezviz-0.2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-04-27 14:05:38.289149 pyezviz-0.2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:05:38.289149 pyezviz-0.2.0.8/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     5386 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (121)    36211 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4901 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:05:38.289149 pyezviz-0.2.0.8/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-27 14:05:38.000000 pyezviz-0.2.0.8/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 14:05:38.289149 pyezviz-0.2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-04-27 14:05:29.000000 pyezviz-0.2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12195 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36211 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7248 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4901 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-08 18:50:33.000000 pyezviz-0.2.0.9/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-08 18:50:33.619938 pyezviz-0.2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-07-08 18:50:26.000000 pyezviz-0.2.0.9/setup.py
```

### Comparing `pyezviz-0.2.0.8/LICENSE.md` & `pyezviz-0.2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/README.md` & `pyezviz-0.2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 Tests are written in the tests directory.
 tests/data folder contains samples of EzvizLife API for tests purposes.
 
 
 ## Side notes
 
 As there is no official documentation on the API, I had to reverse-engineer what is the one used in the Ezviz IOS APP.
-Some Regions might operate on an isolated platform and require a url to be entered. Russia for example:
+Some Regions might operate on an isolated platform and require a url to be entered. US for example:
 
-pyezviz -u username@domain.com -p PASS@123 -r apirus.ezvizru.com devices status
+pyezviz -u username@domain.com -p PASS@123 -r apiius.ezvizlife.com devices status
 
 ## Contributing
 
 Any contribution is welcome, considering the number of features the API provides, there is room for improvement!
 
 ## Versioning
```

### Comparing `pyezviz-0.2.0.8/pyezviz/__init__.py` & `pyezviz-0.2.0.9/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/__main__.py` & `pyezviz-0.2.0.9/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/camera.py` & `pyezviz-0.2.0.9/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/cas.py` & `pyezviz-0.2.0.9/pyezviz/cas.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,15 +53,19 @@
             f"\n\t<Sign>{FEATURE_CODE}</Sign>\n\t"
             f"<DevSerial>{devserial}</DevSerial>"
             f"\n\t<ClientType>0</ClientType>\n</Request>\n"
         ).encode("latin1")
 
         payload_end_padding = rand_hex.encode("latin1")
 
-        context = ssl.SSLContext(cert_reqs=ssl.CERT_NONE)
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+
+        context.set_ciphers(
+            "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
+        )
 
         # Create a TCP/IP socket
         my_socket = socket.create_connection(
             (self._service_urls["sysConf"][15], self._service_urls["sysConf"][16])
         )
         my_socket = context.wrap_socket(
             my_socket, server_hostname=self._service_urls["sysConf"][15]
@@ -121,15 +125,19 @@
             f"<Request>\n"
             f"\t<OperationCode>ABCDEFG</OperationCode>\n"
             f'\t<Defence Type="Global" Status="{enable}" Actor="V" Channel="0" />\n'
             f"</Request>\n"
             f"\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10\x10"
         ).encode("latin1")
 
-        context = ssl.SSLContext(cert_reqs=ssl.CERT_NONE)
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+
+        context.set_ciphers(
+            "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
+        )
 
         # Create a TCP/IP socket
         my_socket = socket.create_connection(
             (self._service_urls["sysConf"][15], self._service_urls["sysConf"][16])
         )
         my_socket = context.wrap_socket(
             my_socket, server_hostname=self._service_urls["sysConf"][15]
```

### Comparing `pyezviz-0.2.0.8/pyezviz/client.py` & `pyezviz-0.2.0.9/pyezviz/client.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/constants.py` & `pyezviz-0.2.0.9/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/exceptions.py` & `pyezviz-0.2.0.9/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/mqtt.py` & `pyezviz-0.2.0.9/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.0.9/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/pyezviz/utils.py` & `pyezviz-0.2.0.9/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.0.8/setup.py` & `pyezviz-0.2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.0.8",
+    version="0.2.0.9",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

