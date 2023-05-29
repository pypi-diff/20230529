# Comparing `tmp/liuzh594Crypto-5.9.4.9.9.9.tar.gz` & `tmp/liuzh594Crypto-5.9.4.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liuzh594Crypto-5.9.4.9.9.9.tar", last modified: Mon May 29 01:55:53 2023, max compression
+gzip compressed data, was "liuzh594Crypto-5.9.4.9.99.tar", last modified: Mon May 29 02:13:17 2023, max compression
```

## Comparing `liuzh594Crypto-5.9.4.9.9.9.tar` & `liuzh594Crypto-5.9.4.9.99.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.208017 liuzh594Crypto-5.9.4.9.9.9/
--rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.9.9.9/LICENSE
--rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 01:55:53.207873 liuzh594Crypto-5.9.4.9.9.9/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.9.9.9/README.md
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.204198 liuzh594Crypto-5.9.4.9.9.9/basicMath/
--rw-r--r--   0 lzh        (501) staff       (20)     6294 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/ECC.py
--rw-r--r--   0 lzh        (501) staff       (20)     3572 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/GF.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     5652 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/basic.py
--rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/type.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.204835 liuzh594Crypto-5.9.4.9.9.9/blockCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     9446 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/blockCipher/SM4.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:58:08.000000 liuzh594Crypto-5.9.4.9.9.9/blockCipher/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.205466 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/
--rw-r--r--   0 lzh        (501) staff       (20)     3209 2023-05-26 09:45:32.000000 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/SM2_SV.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 15:48:59.000000 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.206034 liuzh594Crypto-5.9.4.9.9.9/hash/
--rw-r--r--   0 lzh        (501) staff       (20)     5583 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/hash/SM3.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 16:05:08.000000 liuzh594Crypto-5.9.4.9.9.9/hash/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.206699 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/
--rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)      478 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/SOURCES.txt
--rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/dependency_links.txt
--rw-r--r--   0 lzh        (501) staff       (20)       57 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/top_level.txt
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.207281 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     3186 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/RSA.py
--rw-r--r--   0 lzh        (501) staff       (20)     3638 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/SM2.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 11:46:35.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 01:55:53.208058 liuzh594Crypto-5.9.4.9.9.9/setup.cfg
--rw-r--r--   0 lzh        (501) staff       (20)     1072 2023-05-29 01:54:49.000000 liuzh594Crypto-5.9.4.9.9.9/setup.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.207535 liuzh594Crypto-5.9.4.9.9.9/tests/
--rw-r--r--   0 lzh        (501) staff       (20)     9188 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4.9.9.9/tests/tests.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.603365 liuzh594Crypto-5.9.4.9.99/
+-rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.9.99/LICENSE
+-rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 02:13:17.603202 liuzh594Crypto-5.9.4.9.99/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.9.99/README.md
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.599993 liuzh594Crypto-5.9.4.9.99/basicMath/
+-rw-r--r--   0 lzh        (501) staff       (20)     6294 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/ECC.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3572 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/GF.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.9.99/basicMath/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     5652 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/basic.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.9.99/basicMath/type.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.600465 liuzh594Crypto-5.9.4.9.99/blockCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     9446 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/blockCipher/SM4.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:58:08.000000 liuzh594Crypto-5.9.4.9.99/blockCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.600919 liuzh594Crypto-5.9.4.9.99/digitalSignature/
+-rw-r--r--   0 lzh        (501) staff       (20)     3209 2023-05-26 09:45:32.000000 liuzh594Crypto-5.9.4.9.99/digitalSignature/SM2_SV.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 15:48:59.000000 liuzh594Crypto-5.9.4.9.99/digitalSignature/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.601373 liuzh594Crypto-5.9.4.9.99/hash/
+-rw-r--r--   0 lzh        (501) staff       (20)     5583 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/hash/SM3.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 16:05:08.000000 liuzh594Crypto-5.9.4.9.99/hash/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.601868 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/
+-rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)      496 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       63 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/top_level.txt
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.602535 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     3186 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/RSA.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3638 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/SM2.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 11:46:35.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 02:13:17.603407 liuzh594Crypto-5.9.4.9.99/setup.cfg
+-rw-r--r--   0 lzh        (501) staff       (20)     1072 2023-05-29 02:12:29.000000 liuzh594Crypto-5.9.4.9.99/setup.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.602840 liuzh594Crypto-5.9.4.9.99/tests/
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:10:38.000000 liuzh594Crypto-5.9.4.9.99/tests/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     9188 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4.9.99/tests/tests.py
```

### Comparing `liuzh594Crypto-5.9.4.9.9.9/LICENSE` & `liuzh594Crypto-5.9.4.9.99/LICENSE`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/PKG-INFO` & `liuzh594Crypto-5.9.4.9.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.9.9.9
-Summary: my crypto python package in 2023
+Version: 5.9.4.9.99
+Summary: my hcrypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `liuzh594Crypto-5.9.4.9.9.9/README.md` & `liuzh594Crypto-5.9.4.9.99/README.md`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/basicMath/ECC.py` & `liuzh594Crypto-5.9.4.9.99/basicMath/ECC.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/basicMath/GF.py` & `liuzh594Crypto-5.9.4.9.99/basicMath/GF.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/basicMath/basic.py` & `liuzh594Crypto-5.9.4.9.99/basicMath/basic.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/basicMath/type.py` & `liuzh594Crypto-5.9.4.9.99/basicMath/type.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/blockCipher/SM4.py` & `liuzh594Crypto-5.9.4.9.99/blockCipher/SM4.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/digitalSignature/SM2_SV.py` & `liuzh594Crypto-5.9.4.9.99/digitalSignature/SM2_SV.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/hash/SM3.py` & `liuzh594Crypto-5.9.4.9.99/hash/SM3.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/PKG-INFO` & `liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.9.9.9
-Summary: my crypto python package in 2023
+Version: 5.9.4.9.99
+Summary: my hcrypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/RSA.py` & `liuzh594Crypto-5.9.4.9.99/pubkeyCipher/RSA.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/SM2.py` & `liuzh594Crypto-5.9.4.9.99/pubkeyCipher/SM2.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.9.9/setup.py` & `liuzh594Crypto-5.9.4.9.99/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="liuzh594Crypto",
-    version="5.9.4.9.9.9",
+    version="5.9.4.9.99",
     author="Liuzhenghao",
     author_email="liuzh594@qq.com",
-    description="my crypto python package in 2023",
+    description="my hcrypto python package in 2023",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lzh594/liuzh594Crypto",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `liuzh594Crypto-5.9.4.9.9.9/tests/tests.py` & `liuzh594Crypto-5.9.4.9.99/tests/tests.py`

 * *Files identical despite different names*

