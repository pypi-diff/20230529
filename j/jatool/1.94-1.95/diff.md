# Comparing `tmp/jatool-1.94.tar.gz` & `tmp/jatool-1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jatool-1.94.tar", last modified: Sun May 28 18:01:09 2023, max compression
+gzip compressed data, was "jatool-1.95.tar", last modified: Mon May 29 02:26:55 2023, max compression
```

## Comparing `jatool-1.94.tar` & `jatool-1.95.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 slv        (501) staff       (20)        0 2023-05-28 18:01:09.192973 jatool-1.94/
--rw-r--r--   0 slv        (501) staff       (20)     2583 2023-05-28 18:01:09.192540 jatool-1.94/PKG-INFO
--rw-r--r--   0 slv        (501) staff       (20)     2211 2023-05-28 17:55:31.000000 jatool-1.94/README.md
-drwxr-xr-x   0 slv        (501) staff       (20)        0 2023-05-28 18:01:09.189550 jatool-1.94/jatool/
--rw-r--r--   0 slv        (501) staff       (20)        0 2023-05-27 07:49:55.000000 jatool-1.94/jatool/__init__.py
--rw-r--r--   0 slv        (501) staff       (20)    25288 2023-05-28 17:33:43.000000 jatool-1.94/jatool/function.py
-drwxr-xr-x   0 slv        (501) staff       (20)        0 2023-05-28 18:01:09.191884 jatool-1.94/jatool.egg-info/
--rw-r--r--   0 slv        (501) staff       (20)     2583 2023-05-28 18:01:09.000000 jatool-1.94/jatool.egg-info/PKG-INFO
--rw-r--r--   0 slv        (501) staff       (20)      205 2023-05-28 18:01:09.000000 jatool-1.94/jatool.egg-info/SOURCES.txt
--rw-r--r--   0 slv        (501) staff       (20)        1 2023-05-28 18:01:09.000000 jatool-1.94/jatool.egg-info/dependency_links.txt
--rw-r--r--   0 slv        (501) staff       (20)      132 2023-05-28 18:01:09.000000 jatool-1.94/jatool.egg-info/requires.txt
--rw-r--r--   0 slv        (501) staff       (20)        7 2023-05-28 18:01:09.000000 jatool-1.94/jatool.egg-info/top_level.txt
--rw-r--r--   0 slv        (501) staff       (20)       38 2023-05-28 18:01:09.193105 jatool-1.94/setup.cfg
--rw-r--r--   0 slv        (501) staff       (20)      939 2023-05-28 17:53:42.000000 jatool-1.94/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:26:55.733267 jatool-1.95/
+-rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 02:26:55.731849 jatool-1.95/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2391 2023-05-29 02:05:05.000000 jatool-1.95/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:26:55.723056 jatool-1.95/jatool/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-29 02:05:06.000000 jatool-1.95/jatool/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    25575 2023-05-29 02:22:00.000000 jatool-1.95/jatool/function.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:26:55.730113 jatool-1.95/jatool.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 02:26:55.000000 jatool-1.95/jatool.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      205 2023-05-29 02:26:55.000000 jatool-1.95/jatool.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-29 02:26:55.000000 jatool-1.95/jatool.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      132 2023-05-29 02:26:55.000000 jatool-1.95/jatool.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2023-05-29 02:26:55.000000 jatool-1.95/jatool.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-29 02:26:55.733368 jatool-1.95/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      939 2023-05-29 02:22:43.000000 jatool-1.95/setup.py
```

### Comparing `jatool-1.94/PKG-INFO` & `jatool-1.95/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.94
+Version: 1.95
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,22 @@
 
 A Python package to download and downstream-analysis the Japanese literatures.
 
 ## Install 
 
 ``` python
 pip install jatool
+
+#You need to install Rust to install depandency 'SudachiPy'
+##Linux##   
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+##MacOS##
+brew install rustup
+rustup-init
+
 ```
 
 ## load jatool package
 
 ``` python
 from jatool.function import *
 ```
```

### Comparing `jatool-1.94/README.md` & `jatool-1.95/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 A Python package to download and downstream-analysis the Japanese literatures.
 
 ## Install 
 
 ``` python
 pip install jatool
+
+#You need to install Rust to install depandency 'SudachiPy'
+##Linux##   
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+##MacOS##
+brew install rustup
+rustup-init
+
 ```
 
 ## load jatool package
 
 ``` python
 from jatool.function import *
 ```
```

### Comparing `jatool-1.94/jatool/function.py` & `jatool-1.95/jatool/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,19 @@
 
 import json
 from hashlib import md5
 
 
 
 ##################青空文库下载链接文本处理#######################
-fiction_database_file = 'fiction_info_new.txt'
+#fiction_database_file = 'fiction_info_new.txt'
+
+package_path = pkgutil.get_loader('jatool').get_filename()
+fiction_database_file = package_path.replace('__init__.py', 'fiction_info_new.txt')
+
 fiction_df = pd.read_csv(fiction_database_file, delimiter='\t') # 读取txt
 fiction_df['副題'] = fiction_df['副題'].str.replace('\u3000', ' ') # 去除全角空格 
 fiction_df['author_fiction'] = fiction_df['author'] + '_' +fiction_df['作品名']  # 添加 author_fiction
 fiction_df['author_fiction_subname'] = fiction_df['author'] + '_' + fiction_df['作品名'] + '_' + fiction_df['副題']# 添加 author_fiction_subname
 fiction_df.columns
 author_list = fiction_df['author'] # 添加作者
 fiction_df['url'] = fiction_df['テキストファイルURL'] # 添加url下载链接
@@ -351,15 +355,18 @@
         content = read_aozora_file(txt)
         text_token = segment_tokenize(content)
         content_tokenize_list.append(text_token)
     #return(content_tokenize_list)    
     #return([text_list,txt_list])
 
         # 去除停用词
-    with open('stopwords_list_new.txt', 'r', encoding='utf-8') as file:
+    package_path = pkgutil.get_loader('jatool').get_filename()
+    stopwords_file = package_path.replace('__init__.py', 'stopwords_list_new.txt')
+    
+    with open(stopwords_file, 'r', encoding='utf-8') as file:
         stopwords_list = [line.strip() for line in file]
 
     stopwords_list_add = ['\u3000','一','-','み','り','ゝ','ふ','ひ','／','く','＼','す','やう','さま','る','ど','よ','め','ね','ま','人','事','ぬ','やう','さま','る','ど','よ','め','ね','ま','\r\n','樣','ぞ','とて','なれ','たる','わ','とて','ひと','あ','いふ','じ','\r\n\u3000','-','―']
     
     stopwords_list.extend(stopwords_list_add)
     stopwords_list.extend(added_stopwords)
     #去除函数
@@ -592,15 +599,15 @@
     
     # Set your own appid/appkey.
     appid = '20230405001629367'
     appkey = 'SXgLcp_HNY8_nYdsx0uu'
 
     # For list of language codes, please refer to `https://api.fanyi.baidu.com/doc/21`
     from_lang = 'auto'
-    to_lang =  'cn'
+    to_lang =  'zh'
     
     endpoint = 'http://api.fanyi.baidu.com'
     path = '/api/trans/vip/translate'
     url = endpoint + path
     
     query = text
```

### Comparing `jatool-1.94/jatool.egg-info/PKG-INFO` & `jatool-1.95/jatool.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.94
+Version: 1.95
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,22 @@
 
 A Python package to download and downstream-analysis the Japanese literatures.
 
 ## Install 
 
 ``` python
 pip install jatool
+
+#You need to install Rust to install depandency 'SudachiPy'
+##Linux##   
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
+##MacOS##
+brew install rustup
+rustup-init
+
 ```
 
 ## load jatool package
 
 ``` python
 from jatool.function import *
 ```
```

### Comparing `jatool-1.94/setup.py` & `jatool-1.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='jatool',
-    version='1.94',
+    version='1.95',
     author='Pigpig',
     author_email='21310238@tongji.edu.cn',
     description='A Python package for jatools',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bigbrolv/jatool",
     packages=find_packages(),
```

