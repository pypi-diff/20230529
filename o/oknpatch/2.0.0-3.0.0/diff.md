# Comparing `tmp/oknpatch-2.0.0.tar.gz` & `tmp/oknpatch-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oknpatch-2.0.0.tar", last modified: Mon May 22 00:04:15 2023, max compression
+gzip compressed data, was "oknpatch-3.0.0.tar", last modified: Sun May 28 23:50:21 2023, max compression
```

## Comparing `oknpatch-2.0.0.tar` & `oknpatch-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.576355 oknpatch-2.0.0/
--rw-rw-rw-   0        0        0    11558 2022-07-06 00:41:01.000000 oknpatch-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      525 2023-05-22 00:04:15.576355 oknpatch-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2344 2023-02-27 04:55:12.000000 oknpatch-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.565384 oknpatch-2.0.0/oknpatch/
--rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknpatch-2.0.0/oknpatch/__init__.py
--rw-rw-rw-   0        0        0     5925 2022-04-19 02:25:13.000000 oknpatch-2.0.0/oknpatch/gazefilters.json
--rw-rw-rw-   0        0        0    26699 2023-05-22 00:00:36.000000 oknpatch-2.0.0/oknpatch/oknpatch.py
-drwxrwxrwx   0        0        0        0 2023-05-22 00:04:15.575358 oknpatch-2.0.0/oknpatch.egg-info/
--rw-rw-rw-   0        0        0      525 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-22 00:03:15.000000 oknpatch-2.0.0/oknpatch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 00:04:15.000000 oknpatch-2.0.0/oknpatch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 00:04:15.576355 oknpatch-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-05-22 00:00:01.000000 oknpatch-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.945933 oknpatch-3.0.0/
+-rw-rw-rw-   0        0        0    11558 2022-07-06 00:41:01.000000 oknpatch-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-05-28 23:50:21.945933 oknpatch-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2344 2023-02-27 04:55:12.000000 oknpatch-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.935196 oknpatch-3.0.0/oknpatch/
+-rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknpatch-3.0.0/oknpatch/__init__.py
+-rw-rw-rw-   0        0        0     6263 2023-05-17 08:39:07.000000 oknpatch-3.0.0/oknpatch/gazefilters.json
+-rw-rw-rw-   0        0        0    13248 2023-02-13 03:27:15.000000 oknpatch-3.0.0/oknpatch/okndetector.gaze.config
+-rw-rw-rw-   0        0        0    36912 2023-05-28 23:34:44.000000 oknpatch-3.0.0/oknpatch/oknpatch.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.944172 oknpatch-3.0.0/oknpatch.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 23:50:08.000000 oknpatch-3.0.0/oknpatch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:50:21.945933 oknpatch-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-05-28 22:12:49.000000 oknpatch-3.0.0/setup.py
```

### Comparing `oknpatch-2.0.0/LICENSE` & `oknpatch-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oknpatch-2.0.0/PKG-INFO` & `oknpatch-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 2.0.0
+Version: 3.0.0
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-2.0.0/README.md` & `oknpatch-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oknpatch-2.0.0/oknpatch/gazefilters.json` & `oknpatch-3.0.0/oknpatch/gazefilters.json`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,20 @@
 
 					{ "Enabled" : false, "input": [ "updated_X_EyeRegion" ],  "output" : "updated_X_EyeRegion",   		"function" : "shiftSignal"  },
 					{ "Enabled" : false, "input": [ "updated_Y_EyeRegion" ],  "output" : "updated_Y_EyeRegion",   		"function" : "shiftSignal"  },
 					
                     // Gradient
 				
 					{ "Enabled" : true, "input": [ "record_timestamp", "updated_x_nom" ],  "output": "updated_dXdt_nom",  "function" : "gradient" },
-					{ "Enabled" : true, "input": [ "record_timestamp", "updated_y_nom" ],  "output": "updated_dYdt_nom",  "function" : "gradient" } ],
+					{ "Enabled" : true, "input": [ "record_timestamp", "updated_y_nom" ],  "output": "updated_dYdt_nom",  "function" : "gradient" },
+
+					// Replace nan by column value
+
+					{ "Enabled" : true, "input": [ "updated_x_nom" ],  "output" : "updated_x_nom",   "function" : "replaceNanBy",  "pointer" : "confidence<=0"  },
+					{ "Enabled" : true, "input": [ "updated_y_nom" ],  "output" : "updated_y_nom",   "function" : "replaceNanBy",  "pointer" : "confidence<=0"  }],
 
 
 	// Graph-It! 
 
 	"Graph"   : {  	"default_profile" 	: "updated_by_nosetip",
 					"time_interval"     : 10,
 					"Profiles" 			: [ { "name" : "raw",  					"overlay" : false, "id": "Id", "t" : "currentTime", "x" : "finalX_NoseTip",		"y" : "finalY_NoseTip",				"dxdt" : "finaldXdt_NoseTip", 	  "scale_factor" : 0.040, "is_tracking" : "isTracked", "is_blinking" : "isBlinking", "filename" : "results.csv" },
```

### Comparing `oknpatch-2.0.0/oknpatch.egg-info/PKG-INFO` & `oknpatch-3.0.0/oknpatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 2.0.0
+Version: 3.0.0
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-2.0.0/setup.py` & `oknpatch-3.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to fix okn and pim related issues.'
 
 setup(
     name='oknpatch',
-    version='2.0.0',
+    version='3.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/oknpatch',
     description='issues fixing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
     packages=find_packages(),
     include_package_data=True,
-    package_data={'': ['gazefilters.json']},
+    package_data={'': ['gazefilters.json', 'okndetector.gaze.config']},
     entry_points={
         'console_scripts': [
             'oknpatch = oknpatch.oknpatch:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

