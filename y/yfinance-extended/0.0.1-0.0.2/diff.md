# Comparing `tmp/yfinance-extended-0.0.1.tar.gz` & `tmp/yfinance-extended-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance-extended-0.0.1.tar", last modified: Mon May 29 00:54:18 2023, max compression
+gzip compressed data, was "yfinance-extended-0.0.2.tar", last modified: Mon May 29 01:04:54 2023, max compression
```

## Comparing `yfinance-extended-0.0.1.tar` & `yfinance-extended-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 zhaohan_dong   (501) staff       (20)        0 2023-05-29 00:54:18.259817 yfinance-extended-0.0.1/
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)     1499 2023-05-29 00:43:27.000000 yfinance-extended-0.0.1/LICENSE
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)     3220 2023-05-29 00:54:18.259866 yfinance-extended-0.0.1/PKG-INFO
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)     2034 2023-05-29 00:39:34.000000 yfinance-extended-0.0.1/README.md
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)      102 2023-05-29 00:54:18.260988 yfinance-extended-0.0.1/setup.cfg
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)     1929 2023-05-29 00:54:09.000000 yfinance-extended-0.0.1/setup.py
-drwxr-xr-x   0 zhaohan_dong   (501) staff       (20)        0 2023-05-29 00:54:18.259673 yfinance-extended-0.0.1/yfinance_extended.egg-info/
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)     3220 2023-05-29 00:54:18.000000 yfinance-extended-0.0.1/yfinance_extended.egg-info/PKG-INFO
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)      240 2023-05-29 00:54:18.000000 yfinance-extended-0.0.1/yfinance_extended.egg-info/SOURCES.txt
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)        1 2023-05-29 00:54:18.000000 yfinance-extended-0.0.1/yfinance_extended.egg-info/dependency_links.txt
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)       33 2023-05-29 00:54:18.000000 yfinance-extended-0.0.1/yfinance_extended.egg-info/requires.txt
--rw-r--r--   0 zhaohan_dong   (501) staff       (20)        1 2023-05-29 00:54:18.000000 yfinance-extended-0.0.1/yfinance_extended.egg-info/top_level.txt
+drwxr-xr-x   0 zhaohan_dong   (501) staff       (20)        0 2023-05-29 01:04:54.340987 yfinance-extended-0.0.2/
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)     1499 2023-05-29 00:43:27.000000 yfinance-extended-0.0.2/LICENSE
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)     3220 2023-05-29 01:04:54.341037 yfinance-extended-0.0.2/PKG-INFO
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)     2034 2023-05-29 00:39:34.000000 yfinance-extended-0.0.2/README.md
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)      102 2023-05-29 01:04:54.342505 yfinance-extended-0.0.2/setup.cfg
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)     1935 2023-05-29 01:04:40.000000 yfinance-extended-0.0.2/setup.py
+drwxr-xr-x   0 zhaohan_dong   (501) staff       (20)        0 2023-05-29 01:04:54.340859 yfinance-extended-0.0.2/yfinance_extended.egg-info/
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)     3220 2023-05-29 01:04:54.000000 yfinance-extended-0.0.2/yfinance_extended.egg-info/PKG-INFO
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)      240 2023-05-29 01:04:54.000000 yfinance-extended-0.0.2/yfinance_extended.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)        1 2023-05-29 01:04:54.000000 yfinance-extended-0.0.2/yfinance_extended.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)       33 2023-05-29 01:04:54.000000 yfinance-extended-0.0.2/yfinance_extended.egg-info/requires.txt
+-rw-r--r--   0 zhaohan_dong   (501) staff       (20)        1 2023-05-29 01:04:54.000000 yfinance-extended-0.0.2/yfinance_extended.egg-info/top_level.txt
```

### Comparing `yfinance-extended-0.0.1/LICENSE` & `yfinance-extended-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yfinance-extended-0.0.1/PKG-INFO` & `yfinance-extended-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-extended
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension of yfinance package to download wide-form stock data from Yahoo! Finance
 Home-page: https://github.com/zhaohan-dong/yfinance-extended
 Author: Zhaohan Dong
 Author-email: zhaohan_dong@yahoo.com
 License: bsd-3-clause
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `yfinance-extended-0.0.1/README.md` & `yfinance-extended-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yfinance-extended-0.0.1/setup.py` & `yfinance-extended-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 # https://github.com/zhaohan-dong/yfinance-extended
 
 """yfinance-extended"""
 
 from setuptools import setup
 
 # --- get version ---
-with open("yfinance-extended/version.py") as f:
-    line = f.read().strip()
-    version = line.replace("version = ", "").replace('"', '')
+# with open("yfinance-extended/version.py") as f:
+#     line = f.read().strip()
+#     version = line.replace("version = ", "").replace('"', '')
 # --- /get version ---
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yfinance-extended',
-    version=version,
+    version="0.0.2",
     description='Extension of yfinance package to download wide-form stock data from Yahoo! Finance',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zhaohan-dong/yfinance-extended',
     author='Zhaohan Dong',
     author_email='zhaohan_dong@yahoo.com',
     license='bsd-3-clause',
```

### Comparing `yfinance-extended-0.0.1/yfinance_extended.egg-info/PKG-INFO` & `yfinance-extended-0.0.2/yfinance_extended.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-extended
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extension of yfinance package to download wide-form stock data from Yahoo! Finance
 Home-page: https://github.com/zhaohan-dong/yfinance-extended
 Author: Zhaohan Dong
 Author-email: zhaohan_dong@yahoo.com
 License: bsd-3-clause
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
```

