# Comparing `tmp/prophecy-libs-1.5.3.tar.gz` & `tmp/prophecy-libs-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.3.tar", last modified: Fri May 26 15:20:33 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.4.tar", last modified: Mon May 29 13:41:08 2023, max compression
```

## Comparing `prophecy-libs-1.5.3.tar` & `prophecy-libs-1.5.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.710185 prophecy-libs-1.5.3/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4346 2023-05-25 10:51:46.000000 prophecy-libs-1.5.3/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.3/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.3/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      764 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22812 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1571 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6432 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6368 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/fixed_file_schema.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-26 15:20:33.710185 prophecy-libs-1.5.3/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4346 2023-05-25 10:51:46.000000 prophecy-libs-1.5.4/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.858582 prophecy-libs-1.5.4/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.4/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.4/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1585 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6515 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6393 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/prophecy/transpiler/fixed_file_schema.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.4/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.4/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-29 13:41:08.000000 prophecy-libs-1.5.4/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-29 13:41:08.862583 prophecy-libs-1.5.4/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-29 13:41:07.000000 prophecy-libs-1.5.4/setup.py
```

### Comparing `prophecy-libs-1.5.3/prophecy/config/config_base.py` & `prophecy-libs-1.5.4/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/config/utils.py` & `prophecy-libs-1.5.4/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/libs/utils.py` & `prophecy-libs-1.5.4/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.4/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/random_data_creator.py` & `prophecy-libs-1.5.4/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.4/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.4/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/test/utils.py` & `prophecy-libs-1.5.4/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/transpiler/abi_base.py` & `prophecy-libs-1.5.4/prophecy/transpiler/abi_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
-from pyspark.sql import *
-from prophecy.udfs.scala_udf_wrapper import *
+from prophecy.udfs.scala_udf_wrapper import initializeUDFBase
+from pyspark.sql import SQLContext
 
 
 class ABILib:
     def __init__(self, spark):
         self.spark = spark
         self.sqlContext = SQLContext(spark.sparkContext, sparkSession=spark)
         self.libs = spark.sparkContext._jvm.io.prophecy.libs.package
```

### Comparing `prophecy-libs-1.5.3/prophecy/transpiler/abi_core_fcns.py` & `prophecy-libs-1.5.4/prophecy/transpiler/abi_core_fcns.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def string_split_no_empty(input: str, pattern: str):
         import re
         if input is None:
             return None
         else:
             opt1 = input.split(re.escape(pattern))
             opt2 = input.split(pattern)
-            finalSplit = opt2 if len(opt1) == 1 and opt[0] == input else opt1
+            finalSplit = opt2 if len(opt1) == 1 and opt1[0] == input else opt1
             res = filter(lambda x: x != "", finalSplit)
             return [x for x in res]
 
     @staticmethod
     def string_lrtrim(input: str):
         return None if input is None else input.strip()
 
@@ -179,15 +179,15 @@
         import traceback
         if _filename is None:
             return None
         elif _filename == "":
             return ""
         else:
             try:
-                filepath = searchAndGetFilePathFromBaseDirectory(_filename, baseDirectory)
+                filepath = ABIUtil.searchAndGetFilePathFromBaseDirectory(_filename, baseDirectory)
                 try:
                     with open(filepath, 'r') as file:
                         file_contents = file.read()
                     return file_contents
                 except:
                     with open(filepath, 'r', encoding='ISO-8859-1') as file:
                         file_contents = file.read()
@@ -254,15 +254,15 @@
 
     @staticmethod
     def length(input: str):
         return None if input is None else len(input)
 
     @staticmethod
     def string_length(input: str):
-        return length(input)
+        return ABIUtil.length(input)
 
     @staticmethod
     def string_index(input: str, seek: str, offset: int = 0):
         if input is None or seek is None:
             return -1
         else:
             index = input[offset:].index(seek) + 1
@@ -378,15 +378,15 @@
             return "".join([x for x in res])
 
     @staticmethod
     def random_string_value(length: int):
         import random
         alphaNumericCharArray = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789abcdefghijklmnopqrstuvxyz"
         l = len(alphaNumericCharArray)
-        return "".join([alphaNumericCharArray[random.randint(0, l)] for idx in range(0, length)])
+        return "".join([alphaNumericCharArray[random.randint(0, l - 1)] for idx in range(0, length)])
 
     @staticmethod
     def isnull(input):
         return input is None
 
     @staticmethod
     def encrypt_aes_simple(input1, input2):
@@ -591,15 +591,15 @@
 
     @staticmethod
     def serialise(value, outputFile):
         import pickle
         return pickle.dump(value, outputFile)
 
     @staticmethod
-    def convertInputBytesToStructType(input, typeInfo: list[str], startByte: int = 0):
+    def convertInputBytesToStructType(input, typeInfo: list, startByte: int = 0):
         if isinstance(input, list) and all([isinstance(x, int) for x in input]):
             return Row(*input)
         else:
             curPointer = 0
             byteArray = ABIUtil.getByteArray(input)[startByte:]
             stringVal = byteArray.decode("windows-1252")
             rowValues = []
```

### Comparing `prophecy-libs-1.5.3/prophecy/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.5.4/prophecy/transpiler/abi_fcn_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import io
 
 import pyspark.sql.types
-from pyspark.sql import column
-from pyspark.sql.functions import lit
+from pyspark.sql import Column, DataFrame, SQLContext, SparkSession
 
-from prophecy.transpiler.abi_base import *
-from prophecy.udfs.scala_udf_wrapper import *
+from prophecy.transpiler.abi_base import ScalaUtil
+from prophecy.udfs.scala_udf_wrapper import call_udf
 
 
 def castArgForScala(item):
     # TODO - this seems enough for now, but needs to be enhanced to handle more complex/nested types
     if isinstance(item, Column):
         return item._jc
     elif isinstance(item, SparkSession):
```

### Comparing `prophecy-libs-1.5.3/prophecy/transpiler/dataframe_fcns.py` & `prophecy-libs-1.5.4/prophecy/transpiler/dataframe_fcns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from prophecy.transpiler.abi_base import *
-from prophecy.utils import *
-from prophecy.libs.utils import *
+from pyspark.sql import column, DataFrame
+from prophecy.transpiler.abi_base import ScalaUtil
+from prophecy.utils import ProphecyDataFrame
+from prophecy.libs.utils import createScalaOption
 
 
 def readFixedFile(schema, path):
     spark = ScalaUtil.getAbiLib().spark
     df = spark.sparkContext._jvm.io.prophecy.libs.FixedFileFormatImplicits.readFixedFile(spark._jsparkSession, schema,
                                                                                          path)
     return DataFrame(df, ScalaUtil.getAbiLib().sqlContext)
@@ -47,14 +48,15 @@
         filterSourceDataFrame
 ) -> DataFrame:
     return ProphecyDataFrame(df, spark).collectDataFrameColumnsToApplyFilter(
         columnList,
         filterSourceDataFrame
     )
 
+
 def normalize(
         df,
         spark,
         lengthExpression,
         finishedExpression,
         finishedCondition,
         alias,
```

### Comparing `prophecy-libs-1.5.3/prophecy/transpiler/fixed_file_schema.py` & `prophecy-libs-1.5.4/prophecy/transpiler/fixed_file_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This contains wrappers over various fixed file schema classes implemented in scala
 
-from prophecy.transpiler import *
-from prophecy.transpiler.abi_base import *
-from prophecy.libs.utils import *
+from prophecy.transpiler.abi_base import ScalaUtil
+from prophecy.libs.utils import (createScalaList, createScalaOption, createScalaMap)
 
 
 def FFSchemaRecord(recordType, rows):
     spark = ScalaUtil.getAbiLib().spark
     jvm = spark.sparkContext._jvm
     return jvm.io.prophecy.libs.FFSchemaRecord(recordType, createScalaList(spark, rows))
```

### Comparing `prophecy-libs-1.5.3/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.4/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.4/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy/utils.py` & `prophecy-libs-1.5.4/prophecy/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.3/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.4/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

