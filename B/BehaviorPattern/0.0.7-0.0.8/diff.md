# Comparing `tmp/BehaviorPattern-0.0.7.tar.gz` & `tmp/BehaviorPattern-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.7.tar", last modified: Mon May 29 11:18:00 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.8.tar", last modified: Mon May 29 11:34:54 2023, max compression
```

## Comparing `BehaviorPattern-0.0.7.tar` & `BehaviorPattern-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3122 2023-05-29 11:17:25.000000 BehaviorPattern-0.0.7/BehaviorPattern/CombinePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     6893 2023-05-29 11:17:28.000000 BehaviorPattern-0.0.7/BehaviorPattern/ContinuePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2759 2023-05-29 11:17:30.000000 BehaviorPattern-0.0.7/BehaviorPattern/DataClass.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3387 2023-05-29 11:17:32.000000 BehaviorPattern-0.0.7/BehaviorPattern/SequencePattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:17:23.000000 BehaviorPattern-0.0.7/BehaviorPattern/__init__.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      373 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 11:17:44.000000 BehaviorPattern-0.0.7/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 11:18:00.000000 BehaviorPattern-0.0.7/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 11:17:47.000000 BehaviorPattern-0.0.7/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3116 2023-05-29 11:32:44.000000 BehaviorPattern-0.0.8/BehaviorPattern/CombinePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6886 2023-05-29 11:32:48.000000 BehaviorPattern-0.0.8/BehaviorPattern/ContinuePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2759 2023-05-29 11:32:53.000000 BehaviorPattern-0.0.8/BehaviorPattern/DataClass.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3380 2023-05-29 11:32:55.000000 BehaviorPattern-0.0.8/BehaviorPattern/SequencePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:32:41.000000 BehaviorPattern-0.0.8/BehaviorPattern/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3206 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      373 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3206 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2883 2023-05-29 11:34:42.000000 BehaviorPattern-0.0.8/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 11:34:54.000000 BehaviorPattern-0.0.8/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 11:34:43.000000 BehaviorPattern-0.0.8/setup.py
```

### Comparing `BehaviorPattern-0.0.7/BehaviorPattern/CombinePattern.py` & `BehaviorPattern-0.0.8/BehaviorPattern/CombinePattern.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from efficient_apriori import apriori 
 from tqdm import tqdm 
 import warnings 
 from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
-class CombinePattern(DataClass):
+class Generate(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior = [], min_support=0.2, min_confidence=0.5, min_length=3, max_length=6, sep = '@'):
         self.min_support = min_support
         self.min_confidence = min_confidence
         self.min_length = min_length
         self.max_length = max_length
         self.behavior_set = set()
         self.black_behavior, self.white_behavior = self.data_preprocess(data, use_behavior, del_behavior, sep)
```

### Comparing `BehaviorPattern-0.0.7/BehaviorPattern/ContinuePattern.py` & `BehaviorPattern-0.0.8/BehaviorPattern/ContinuePattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd 
 from tqdm import tqdm 
 import warnings 
 from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
-class ContinuePattern(DataClass):
+class Generate(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior=[], min_support=0.1, min_length=3, max_length=6, sep = '@'):
         """
         data: DataFrame, 包含用户行为序列和标签的数据集
         use_behavior: list, 需要使用的行为列表，默认为空
         min_support: float, 最小支持度，默认为0.05
         """
         self.min_support = min_support
```

### Comparing `BehaviorPattern-0.0.7/BehaviorPattern/DataClass.py` & `BehaviorPattern-0.0.8/BehaviorPattern/DataClass.py`

 * *Files identical despite different names*

### Comparing `BehaviorPattern-0.0.7/BehaviorPattern/SequencePattern.py` & `BehaviorPattern-0.0.8/BehaviorPattern/SequencePattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from prefixspan import PrefixSpan 
 from tqdm import tqdm 
 import warnings 
 from .DataClass import DataClass
 warnings.filterwarnings('ignore') 
 tqdm.pandas() 
 
-class SequencePattern(DataClass):
+class Generate(DataClass):
     def __init__(self, data, use_behavior=[], del_behavior = [], min_support=0.2, min_length=3, max_length=6, sep='@'):
         self.min_support = min_support
         self.min_length = min_length
         self.max_length = max_length
         self.behavior_set = set()
         self.black_behavior, self.white_behavior = self.data_preprocess(data, use_behavior, del_behavior, sep)
```

### Comparing `BehaviorPattern-0.0.7/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.8/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.7
+Version: 0.0.8
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -20,62 +20,62 @@
 ```
 
 ## 使用
 
 在你的Python代码中引入类，例如：
 
 ```python
-from BehaviorPattern import CombinePattern, ContinuePattern, SequencePattern
+from BehaviorPattern. import CombinePattern, ContinuePattern, SequencePattern
 
 #--------------------------------- 组合行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = CombinePattern(data=data, 
-                          use_behavior=use_behavior, 
-                          del_behavior=del_behavior, 
-                          min_support=0.1, 
-                          min_confidence=0.5, 
-                          min_length=3, 
-                          max_length=7, 
-                          sep='@') 
+behavior = CombinePattern.Generate(data=data, 
+                                   use_behavior=use_behavior, 
+                                   del_behavior=del_behavior, 
+                                   min_support=0.1, 
+                                   min_confidence=0.5, 
+                                   min_length=3, 
+                                   max_length=7, 
+                                   sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 combine, combine_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 combine_result = combine[combine['lift'] > 6] 
 
 
 #--------------------------------- 连续行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = ContinuePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1, 
-                           min_length=3, 
-                           max_length=6, 
-                           sep='@') 
+behavior = ContinuePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1, 
+                                    min_length=3, 
+                                    max_length=6, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 continues, continue_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 continues_result = continues[continues['lift'] > 6] 
 
 
 #--------------------------------- 序列行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = SequencePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1,
-                           min_length=3, 
-                           max_length=7, 
-                           sep='@') 
+behavior = SequencePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1,
+                                    min_length=3, 
+                                    max_length=7, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 sequence, seq_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 sequence_result = sequence[sequence['lift'] > 6] 
 ```
 
 ## 依赖
@@ -93,19 +93,7 @@
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
 BehaviorPattern由Chen Chen编写和维护。
-
-## 致谢
-
-感谢以下Python包的开发者：
-
-- numpy
-- pandas
-- efficient_apriori
-- tqdm
-- prefixspan
-
-这些开发者对该项目发展做出了重要贡献。
```

### Comparing `BehaviorPattern-0.0.7/PKG-INFO` & `BehaviorPattern-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.7
+Version: 0.0.8
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -20,62 +20,62 @@
 ```
 
 ## 使用
 
 在你的Python代码中引入类，例如：
 
 ```python
-from BehaviorPattern import CombinePattern, ContinuePattern, SequencePattern
+from BehaviorPattern. import CombinePattern, ContinuePattern, SequencePattern
 
 #--------------------------------- 组合行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = CombinePattern(data=data, 
-                          use_behavior=use_behavior, 
-                          del_behavior=del_behavior, 
-                          min_support=0.1, 
-                          min_confidence=0.5, 
-                          min_length=3, 
-                          max_length=7, 
-                          sep='@') 
+behavior = CombinePattern.Generate(data=data, 
+                                   use_behavior=use_behavior, 
+                                   del_behavior=del_behavior, 
+                                   min_support=0.1, 
+                                   min_confidence=0.5, 
+                                   min_length=3, 
+                                   max_length=7, 
+                                   sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 combine, combine_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 combine_result = combine[combine['lift'] > 6] 
 
 
 #--------------------------------- 连续行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = ContinuePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1, 
-                           min_length=3, 
-                           max_length=6, 
-                           sep='@') 
+behavior = ContinuePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1, 
+                                    min_length=3, 
+                                    max_length=6, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 continues, continue_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 continues_result = continues[continues['lift'] > 6] 
 
 
 #--------------------------------- 序列行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = SequencePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1,
-                           min_length=3, 
-                           max_length=7, 
-                           sep='@') 
+behavior = SequencePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1,
+                                    min_length=3, 
+                                    max_length=7, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 sequence, seq_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 sequence_result = sequence[sequence['lift'] > 6] 
 ```
 
 ## 依赖
@@ -93,19 +93,7 @@
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
 BehaviorPattern由Chen Chen编写和维护。
-
-## 致谢
-
-感谢以下Python包的开发者：
-
-- numpy
-- pandas
-- efficient_apriori
-- tqdm
-- prefixspan
-
-这些开发者对该项目发展做出了重要贡献。
```

### Comparing `BehaviorPattern-0.0.7/README.md` & `BehaviorPattern-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,62 +9,62 @@
 ```
 
 ## 使用
 
 在你的Python代码中引入类，例如：
 
 ```python
-from BehaviorPattern import CombinePattern, ContinuePattern, SequencePattern
+from BehaviorPattern. import CombinePattern, ContinuePattern, SequencePattern
 
 #--------------------------------- 组合行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = CombinePattern(data=data, 
-                          use_behavior=use_behavior, 
-                          del_behavior=del_behavior, 
-                          min_support=0.1, 
-                          min_confidence=0.5, 
-                          min_length=3, 
-                          max_length=7, 
-                          sep='@') 
+behavior = CombinePattern.Generate(data=data, 
+                                   use_behavior=use_behavior, 
+                                   del_behavior=del_behavior, 
+                                   min_support=0.1, 
+                                   min_confidence=0.5, 
+                                   min_length=3, 
+                                   max_length=7, 
+                                   sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 combine, combine_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 combine_result = combine[combine['lift'] > 6] 
 
 
 #--------------------------------- 连续行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = ContinuePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1, 
-                           min_length=3, 
-                           max_length=6, 
-                           sep='@') 
+behavior = ContinuePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1, 
+                                    min_length=3, 
+                                    max_length=6, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 continues, continue_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 continues_result = continues[continues['lift'] > 6] 
 
 
 #--------------------------------- 序列行为模式挖掘 ---------------------------------#
 use_behavior = []
 del_behavior = []
 # 创建实例
-behavior = SequencePattern(data=data, 
-                           use_behavior=use_behavior, 
-                           del_behavior=del_behavior, 
-                           min_support=0.1,
-                           min_length=3, 
-                           max_length=7, 
-                           sep='@') 
+behavior = SequencePattern.Generate(data=data, 
+                                    use_behavior=use_behavior, 
+                                    del_behavior=del_behavior, 
+                                    min_support=0.1,
+                                    min_length=3, 
+                                    max_length=7, 
+                                    sep='@') 
 # 运行模型，返回pattern结果和使用的行为列表
 sequence, seq_use_behavior = behavior.run() 
 # 筛选lift符合要求的pattern
 sequence_result = sequence[sequence['lift'] > 6] 
 ```
 
 ## 依赖
@@ -81,20 +81,8 @@
 
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
-BehaviorPattern由Chen Chen编写和维护。
-
-## 致谢
-
-感谢以下Python包的开发者：
-
-- numpy
-- pandas
-- efficient_apriori
-- tqdm
-- prefixspan
-
-这些开发者对该项目发展做出了重要贡献。
+BehaviorPattern由Chen Chen编写和维护。
```

### Comparing `BehaviorPattern-0.0.7/setup.py` & `BehaviorPattern-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return [dependency for dependency in dependencies if dependency not in installed]
 
 # 如果存在未安装的依赖库，安装未安装的依赖库
 missing = get_missing_dependencies()
 if missing:
     setuptools.setup(
         name='BehaviorPattern',
-        version='0.0.7',
+        version='0.0.8',
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
-        version='0.0.7',
+        version='0.0.8',
         author='Chen Chen',
         author_email='cchen56@163.com',
         description='The tool is designed to mine behavior patterns',
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=setuptools.find_packages(),
         classifiers=[
```

