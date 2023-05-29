# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230527-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230528-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2397909 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-May-28 04:55 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6818592 b- defN 23-May-28 04:57 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-May-28 04:55 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-May-28 04:55 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-May-28 04:55 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-28 04:57 tflite_runtime_nightly-2.14.0.dev20230527.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-May-28 04:57 tflite_runtime_nightly-2.14.0.dev20230527.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-28 04:57 tflite_runtime_nightly-2.14.0.dev20230527.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-May-28 04:57 tflite_runtime_nightly-2.14.0.dev20230527.dist-info/RECORD
-9 files, 6863481 bytes uncompressed, 2396363 bytes compressed:  65.1%
+Zip file size: 2397911 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-May-29 04:56 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6818592 b- defN 23-May-29 04:58 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-May-29 04:56 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-May-29 04:56 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-May-29 04:56 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-May-29 04:58 tflite_runtime_nightly-2.14.0.dev20230528.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-May-29 04:58 tflite_runtime_nightly-2.14.0.dev20230528.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-29 04:58 tflite_runtime_nightly-2.14.0.dev20230528.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-May-29 04:58 tflite_runtime_nightly-2.14.0.dev20230528.dist-info/RECORD
+9 files, 6863481 bytes uncompressed, 2396365 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230527.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230528.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230527.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230528.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230527.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230528.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230527.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230528.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230527'
-__git_version__ = '0.6.0-148462-g022733ec2b3'
+__version__ = '2.14.0dev20230528'
+__git_version__ = '0.6.0-148466-g727e706af39'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230527.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230528.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230527
+Version: 2.14.0.dev20230528
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230527.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230528.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=ESYS-utY8mrO3RMPBMjD4w3oYUCmD35pweL5yGS3UQE,80
+tflite_runtime/__init__.py,sha256=a6Q2TEg9N-uMDirtAQOtUTd3T-f4LTfLb6Jq920toRw,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=yjmmvsEMedp_BrRo2MWXjZ3uwLUocG-TV-iko0yzhr8,6818592
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230527.dist-info/METADATA,sha256=_CVLCuO0oPQj9wu3vdldevVTbSoI2uqdFQ-c4tvUbls,1440
-tflite_runtime_nightly-2.14.0.dev20230527.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.14.0.dev20230527.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230527.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230528.dist-info/METADATA,sha256=4BFhSZobQsoqtC5p3OyUIg19LIgLcXNXAdt0gQIqqH4,1440
+tflite_runtime_nightly-2.14.0.dev20230528.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.14.0.dev20230528.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230528.dist-info/RECORD,,
```

