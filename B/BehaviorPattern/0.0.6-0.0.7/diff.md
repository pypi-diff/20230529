# Comparing `tmp/BehaviorPattern-0.0.6.tar.gz` & `tmp/BehaviorPattern-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.6.tar", last modified: Mon May 29 10:03:58 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.7.tar", last modified: Mon May 29 11:18:00 2023, max compression
```

## Comparing `BehaviorPattern-0.0.6.tar` & `BehaviorPattern-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/BehaviorPattern/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3121 2023-05-29 10:03:43.000000 BehaviorPattern-0.0.6/BehaviorPattern/CombinePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     6892 2023-05-29 10:03:45.000000 BehaviorPattern-0.0.6/BehaviorPattern/ContinuePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3386 2023-05-29 10:03:50.000000 BehaviorPattern-0.0.6/BehaviorPattern/SequencePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 10:03:40.000000 BehaviorPattern-0.0.6/BehaviorPattern/__init__.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2759 2023-05-29 10:03:48.000000 BehaviorPattern-0.0.6/BehaviorPattern/dataclass.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 10:03:57.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      373 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 10:03:57.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 10:03:57.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 10:03:57.000000 BehaviorPattern-0.0.6/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 10:03:26.000000 BehaviorPattern-0.0.6/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 10:03:58.000000 BehaviorPattern-0.0.6/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 10:03:29.000000 BehaviorPattern-0.0.6/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3122 2023-05-29 11:17:25.000000 BehaviorPattern-0.0.7/BehaviorPattern/CombinePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6893 2023-05-29 11:17:28.000000 BehaviorPattern-0.0.7/BehaviorPattern/ContinuePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2759 2023-05-29 11:17:30.000000 BehaviorPattern-0.0.7/BehaviorPattern/DataClass.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3387 2023-05-29 11:17:32.000000 BehaviorPattern-0.0.7/BehaviorPattern/SequencePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:17:23.000000 BehaviorPattern-0.0.7/BehaviorPattern/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      373 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 11:17:44.000000 BehaviorPattern-0.0.7/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 11:17:47.000000 BehaviorPattern-0.0.7/setup.py
```

### Comparing `BehaviorPattern-0.0.6/BehaviorPattern/CombinePattern.py` & `BehaviorPattern-0.0.7/BehaviorPattern/CombinePattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np 
 import pandas as pd 
 from efficient_apriori import apriori 
 from tqdm import tqdm 
 import warnings 
-from dataclass import DataClass
+from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
 class CombinePattern(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior = [], min_support=0.2, min_confidence=0.5, min_length=3, max_length=6, sep = '@'):
         self.min_support = min_support
         self.min_confidence = min_confidence
```

### Comparing `BehaviorPattern-0.0.6/BehaviorPattern/ContinuePattern.py` & `BehaviorPattern-0.0.7/BehaviorPattern/ContinuePattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np 
 import pandas as pd 
 from tqdm import tqdm 
 import warnings 
-from dataclass import DataClass
+from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
 class ContinuePattern(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior=[], min_support=0.1, min_length=3, max_length=6, sep = '@'):
         """
         data: DataFrame, 包含用户行为序列和标签的数据集
```

### Comparing `BehaviorPattern-0.0.6/BehaviorPattern/SequencePattern.py` & `BehaviorPattern-0.0.7/BehaviorPattern/SequencePattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np 
 import pandas as pd 
 from prefixspan import PrefixSpan 
 from tqdm import tqdm 
 import warnings 
-from dataclass import DataClass
+from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
 class SequencePattern(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior = [], min_support=0.2, min_length=3, max_length=6, sep='@'):
         self.min_support = min_support
         self.min_length = min_length
```

### Comparing `BehaviorPattern-0.0.6/BehaviorPattern/dataclass.py` & `BehaviorPattern-0.0.7/BehaviorPattern/DataClass.py`

 * *Files identical despite different names*

### Comparing `BehaviorPattern-0.0.6/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.7/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.6
+Version: 0.0.7
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.6/PKG-INFO` & `BehaviorPattern-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.6
+Version: 0.0.7
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.6/README.md` & `BehaviorPattern-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `BehaviorPattern-0.0.6/setup.py` & `BehaviorPattern-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return [dependency for dependency in dependencies if dependency not in installed]
 
 # 如果存在未安装的依赖库，安装未安装的依赖库
 missing = get_missing_dependencies()
 if missing:
     setuptools.setup(
         name='BehaviorPattern',
-        version='0.0.6',
+        version='0.0.7',
         author='Chen Chen',
         author_email='cchen56@163.com',
         description='The tool is designed to mine behavior patterns',
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=setuptools.find_packages(),
         classifiers=[
@@ -40,15 +40,15 @@
         ],
         python_requires='>=3.6',
         install_requires=missing,
     )
 else:
     setuptools.setup(
         name='BehaviorPattern',
-        version='0.0.6',
+        version='0.0.7',
         author='Chen Chen',
         author_email='cchen56@163.com',
         description='The tool is designed to mine behavior patterns',
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=setuptools.find_packages(),
         classifiers=[
```

