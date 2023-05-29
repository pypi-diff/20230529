# Comparing `tmp/liuzh594Crypto-5.9.4.tar.gz` & `tmp/liuzh594Crypto-5.9.4.9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liuzh594Crypto-5.9.4.tar", last modified: Fri May 26 15:59:21 2023, max compression
+gzip compressed data, was "liuzh594Crypto-5.9.4.9.9.9.tar", last modified: Mon May 29 01:55:53 2023, max compression
```

## Comparing `liuzh594Crypto-5.9.4.tar` & `liuzh594Crypto-5.9.4.9.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.160840 liuzh594Crypto-5.9.4/
--rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4/LICENSE
--rw-r--r--   0 lzh        (501) staff       (20)     6926 2023-05-26 15:59:21.160704 liuzh594Crypto-5.9.4/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)     6258 2023-05-26 15:58:27.000000 liuzh594Crypto-5.9.4/README.md
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.157169 liuzh594Crypto-5.9.4/basicMath/
--rw-r--r--   0 lzh        (501) staff       (20)     6294 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/basicMath/ECC.py
--rw-r--r--   0 lzh        (501) staff       (20)     3572 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/basicMath/GF.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4/basicMath/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     5652 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/basicMath/basic.py
--rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4/basicMath/type.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.157800 liuzh594Crypto-5.9.4/blockCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     9446 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/blockCipher/SM4.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:58:08.000000 liuzh594Crypto-5.9.4/blockCipher/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.158267 liuzh594Crypto-5.9.4/digitalSignature/
--rw-r--r--   0 lzh        (501) staff       (20)     3209 2023-05-26 09:45:32.000000 liuzh594Crypto-5.9.4/digitalSignature/SM2_SV.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 15:48:59.000000 liuzh594Crypto-5.9.4/digitalSignature/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.158856 liuzh594Crypto-5.9.4/hash/
--rw-r--r--   0 lzh        (501) staff       (20)     5583 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/hash/SM3.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 16:05:08.000000 liuzh594Crypto-5.9.4/hash/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.159464 liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/
--rw-r--r--   0 lzh        (501) staff       (20)     6926 2023-05-26 15:59:21.000000 liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)      478 2023-05-26 15:59:21.000000 liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/SOURCES.txt
--rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-26 15:59:21.000000 liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/dependency_links.txt
--rw-r--r--   0 lzh        (501) staff       (20)       57 2023-05-26 15:59:21.000000 liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/top_level.txt
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.160138 liuzh594Crypto-5.9.4/pubkeyCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     3186 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/pubkeyCipher/RSA.py
--rw-r--r--   0 lzh        (501) staff       (20)     3638 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4/pubkeyCipher/SM2.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 11:46:35.000000 liuzh594Crypto-5.9.4/pubkeyCipher/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-26 15:59:21.160876 liuzh594Crypto-5.9.4/setup.cfg
--rw-r--r--   0 lzh        (501) staff       (20)     1066 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4/setup.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-26 15:59:21.160418 liuzh594Crypto-5.9.4/tests/
--rw-r--r--   0 lzh        (501) staff       (20)     9188 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4/tests/tests.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.208017 liuzh594Crypto-5.9.4.9.9.9/
+-rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.9.9.9/LICENSE
+-rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 01:55:53.207873 liuzh594Crypto-5.9.4.9.9.9/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.9.9.9/README.md
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.204198 liuzh594Crypto-5.9.4.9.9.9/basicMath/
+-rw-r--r--   0 lzh        (501) staff       (20)     6294 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/ECC.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3572 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/GF.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     5652 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/basic.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.9.9.9/basicMath/type.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.204835 liuzh594Crypto-5.9.4.9.9.9/blockCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     9446 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/blockCipher/SM4.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:58:08.000000 liuzh594Crypto-5.9.4.9.9.9/blockCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.205466 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/
+-rw-r--r--   0 lzh        (501) staff       (20)     3209 2023-05-26 09:45:32.000000 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/SM2_SV.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 15:48:59.000000 liuzh594Crypto-5.9.4.9.9.9/digitalSignature/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.206034 liuzh594Crypto-5.9.4.9.9.9/hash/
+-rw-r--r--   0 lzh        (501) staff       (20)     5583 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/hash/SM3.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 16:05:08.000000 liuzh594Crypto-5.9.4.9.9.9/hash/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.206699 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/
+-rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)      478 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       57 2023-05-29 01:55:53.000000 liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/top_level.txt
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.207281 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     3186 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/RSA.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3638 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/SM2.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 11:46:35.000000 liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 01:55:53.208058 liuzh594Crypto-5.9.4.9.9.9/setup.cfg
+-rw-r--r--   0 lzh        (501) staff       (20)     1072 2023-05-29 01:54:49.000000 liuzh594Crypto-5.9.4.9.9.9/setup.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 01:55:53.207535 liuzh594Crypto-5.9.4.9.9.9/tests/
+-rw-r--r--   0 lzh        (501) staff       (20)     9188 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4.9.9.9/tests/tests.py
```

### Comparing `liuzh594Crypto-5.9.4/LICENSE` & `liuzh594Crypto-5.9.4.9.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/PKG-INFO` & `liuzh594Crypto-5.9.4.9.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4
+Version: 5.9.4.9.9.9
 Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -58,15 +58,15 @@
 │   ├── SM3.py
 ├── digitalSignature # 数字签名算法库
 │   └── __init__.py
 │   ├── SM2_SV.py
 ├── liuzh594Crypto.egg-info
 ├── dist
 │   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # mycrypto完整版测试样例
+├── tests # liuzh594crypto完整版测试样例
 │   └── tests.py 
 └── setup.py
 ```
 
 
 
 ## 项目功能
@@ -79,15 +79,15 @@
 
     + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
     + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
 
-        + ##### 支持有限域$GF(2^8)$上的常见数学运算，如：四则运算、逆元、矩阵运算等
+        + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
     + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
@@ -206,15 +206,14 @@
     """
     SM3_test()
 
     """
     digitalSignature测试样例
     """
     SM2_SV_text()
-
 ```
 
 
 
 ## 写在最后
 
 + ### 本项目的工作量主要来自于
@@ -233,8 +232,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
```

### Comparing `liuzh594Crypto-5.9.4/README.md` & `liuzh594Crypto-5.9.4.9.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 │   ├── SM3.py
 ├── digitalSignature # 数字签名算法库
 │   └── __init__.py
 │   ├── SM2_SV.py
 ├── liuzh594Crypto.egg-info
 ├── dist
 │   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # mycrypto完整版测试样例
+├── tests # liuzh594crypto完整版测试样例
 │   └── tests.py 
 └── setup.py
 ```
 
 
 
 ## 项目功能
@@ -61,15 +61,15 @@
 
     + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
     + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
 
-        + ##### 支持有限域$GF(2^8)$上的常见数学运算，如：四则运算、逆元、矩阵运算等
+        + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
     + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
@@ -188,15 +188,14 @@
     """
     SM3_test()
 
     """
     digitalSignature测试样例
     """
     SM2_SV_text()
-
 ```
 
 
 
 ## 写在最后
 
 + ### 本项目的工作量主要来自于
@@ -215,8 +214,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
```

### Comparing `liuzh594Crypto-5.9.4/basicMath/ECC.py` & `liuzh594Crypto-5.9.4.9.9.9/basicMath/ECC.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/basicMath/GF.py` & `liuzh594Crypto-5.9.4.9.9.9/basicMath/GF.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/basicMath/basic.py` & `liuzh594Crypto-5.9.4.9.9.9/basicMath/basic.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/basicMath/type.py` & `liuzh594Crypto-5.9.4.9.9.9/basicMath/type.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/blockCipher/SM4.py` & `liuzh594Crypto-5.9.4.9.9.9/blockCipher/SM4.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/digitalSignature/SM2_SV.py` & `liuzh594Crypto-5.9.4.9.9.9/digitalSignature/SM2_SV.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/hash/SM3.py` & `liuzh594Crypto-5.9.4.9.9.9/hash/SM3.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/liuzh594Crypto.egg-info/PKG-INFO` & `liuzh594Crypto-5.9.4.9.9.9/liuzh594Crypto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4
+Version: 5.9.4.9.9.9
 Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -58,15 +58,15 @@
 │   ├── SM3.py
 ├── digitalSignature # 数字签名算法库
 │   └── __init__.py
 │   ├── SM2_SV.py
 ├── liuzh594Crypto.egg-info
 ├── dist
 │   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # mycrypto完整版测试样例
+├── tests # liuzh594crypto完整版测试样例
 │   └── tests.py 
 └── setup.py
 ```
 
 
 
 ## 项目功能
@@ -79,15 +79,15 @@
 
     + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
     + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
 
-        + ##### 支持有限域$GF(2^8)$上的常见数学运算，如：四则运算、逆元、矩阵运算等
+        + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
     + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
@@ -206,15 +206,14 @@
     """
     SM3_test()
 
     """
     digitalSignature测试样例
     """
     SM2_SV_text()
-
 ```
 
 
 
 ## 写在最后
 
 + ### 本项目的工作量主要来自于
@@ -233,8 +232,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
```

### Comparing `liuzh594Crypto-5.9.4/pubkeyCipher/RSA.py` & `liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/RSA.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/pubkeyCipher/SM2.py` & `liuzh594Crypto-5.9.4.9.9.9/pubkeyCipher/SM2.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4/setup.py` & `liuzh594Crypto-5.9.4.9.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="liuzh594Crypto",
-    version="5.9.4",
+    version="5.9.4.9.9.9",
     author="Liuzhenghao",
     author_email="liuzh594@qq.com",
     description="my crypto python package in 2023",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lzh594/liuzh594Crypto",
     packages=setuptools.find_packages(),
```

### Comparing `liuzh594Crypto-5.9.4/tests/tests.py` & `liuzh594Crypto-5.9.4.9.9.9/tests/tests.py`

 * *Files identical despite different names*

