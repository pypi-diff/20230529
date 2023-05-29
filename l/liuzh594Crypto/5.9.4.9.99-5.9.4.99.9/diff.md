# Comparing `tmp/liuzh594Crypto-5.9.4.9.99.tar.gz` & `tmp/liuzh594Crypto-5.9.4.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liuzh594Crypto-5.9.4.9.99.tar", last modified: Mon May 29 02:13:17 2023, max compression
+gzip compressed data, was "liuzh594Crypto-5.9.4.99.9.tar", last modified: Mon May 29 02:43:27 2023, max compression
```

## Comparing `liuzh594Crypto-5.9.4.9.99.tar` & `liuzh594Crypto-5.9.4.99.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.603365 liuzh594Crypto-5.9.4.9.99/
--rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.9.99/LICENSE
--rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 02:13:17.603202 liuzh594Crypto-5.9.4.9.99/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.9.99/README.md
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.599993 liuzh594Crypto-5.9.4.9.99/basicMath/
--rw-r--r--   0 lzh        (501) staff       (20)     6294 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/ECC.py
--rw-r--r--   0 lzh        (501) staff       (20)     3572 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/GF.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.9.99/basicMath/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     5652 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/basicMath/basic.py
--rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.9.99/basicMath/type.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.600465 liuzh594Crypto-5.9.4.9.99/blockCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     9446 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/blockCipher/SM4.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:58:08.000000 liuzh594Crypto-5.9.4.9.99/blockCipher/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.600919 liuzh594Crypto-5.9.4.9.99/digitalSignature/
--rw-r--r--   0 lzh        (501) staff       (20)     3209 2023-05-26 09:45:32.000000 liuzh594Crypto-5.9.4.9.99/digitalSignature/SM2_SV.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 15:48:59.000000 liuzh594Crypto-5.9.4.9.99/digitalSignature/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.601373 liuzh594Crypto-5.9.4.9.99/hash/
--rw-r--r--   0 lzh        (501) staff       (20)     5583 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/hash/SM3.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 16:05:08.000000 liuzh594Crypto-5.9.4.9.99/hash/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.601868 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/
--rw-r--r--   0 lzh        (501) staff       (20)     6965 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)      496 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/SOURCES.txt
--rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/dependency_links.txt
--rw-r--r--   0 lzh        (501) staff       (20)       63 2023-05-29 02:13:17.000000 liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/top_level.txt
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.602535 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     3186 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/RSA.py
--rw-r--r--   0 lzh        (501) staff       (20)     3638 2023-05-26 09:28:51.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/SM2.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 11:46:35.000000 liuzh594Crypto-5.9.4.9.99/pubkeyCipher/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 02:13:17.603407 liuzh594Crypto-5.9.4.9.99/setup.cfg
--rw-r--r--   0 lzh        (501) staff       (20)     1072 2023-05-29 02:12:29.000000 liuzh594Crypto-5.9.4.9.99/setup.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:13:17.602840 liuzh594Crypto-5.9.4.9.99/tests/
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:10:38.000000 liuzh594Crypto-5.9.4.9.99/tests/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     9188 2023-05-26 15:57:39.000000 liuzh594Crypto-5.9.4.9.99/tests/tests.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.901834 liuzh594Crypto-5.9.4.99.9/
+-rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.99.9/LICENSE
+-rw-r--r--   0 lzh        (501) staff       (20)     6964 2023-05-29 02:43:27.901670 liuzh594Crypto-5.9.4.99.9/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.99.9/README.md
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.896853 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/
+-rw-r--r--   0 lzh        (501) staff       (20)      169 2023-05-29 02:21:01.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.898390 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/
+-rw-r--r--   0 lzh        (501) staff       (20)     6270 2023-05-29 02:24:16.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/ECC.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3560 2023-05-29 02:24:17.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/GF.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     5640 2023-05-29 02:24:17.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/basic.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/type.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.898823 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/blockCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     9422 2023-05-29 02:24:16.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/blockCipher/SM4.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:37.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/blockCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.899252 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/digitalSignature/
+-rw-r--r--   0 lzh        (501) staff       (20)     3161 2023-05-29 02:24:16.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/digitalSignature/SM2_SV.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/digitalSignature/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.900195 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/hash/
+-rw-r--r--   0 lzh        (501) staff       (20)     5559 2023-05-29 02:24:17.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/hash/SM3.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/hash/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.900639 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     3162 2023-05-29 02:24:16.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/RSA.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3558 2023-05-29 02:24:17.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/SM2.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:12.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.901116 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/tests/
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:10:38.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/tests/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     9080 2023-05-29 02:24:41.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/tests/tests.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:43:27.897441 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/
+-rw-r--r--   0 lzh        (501) staff       (20)     6964 2023-05-29 02:43:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)      763 2023-05-29 02:43:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 02:43:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       15 2023-05-29 02:43:27.000000 liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/top_level.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 02:43:27.901874 liuzh594Crypto-5.9.4.99.9/setup.cfg
+-rw-r--r--   0 lzh        (501) staff       (20)     1071 2023-05-29 02:38:27.000000 liuzh594Crypto-5.9.4.99.9/setup.py
```

### Comparing `liuzh594Crypto-5.9.4.9.99/LICENSE` & `liuzh594Crypto-5.9.4.99.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.99/PKG-INFO` & `liuzh594Crypto-5.9.4.99.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.9.99
-Summary: my hcrypto python package in 2023
+Version: 5.9.4.99.9
+Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `liuzh594Crypto-5.9.4.9.99/README.md` & `liuzh594Crypto-5.9.4.99.9/README.md`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.99/basicMath/ECC.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/ECC.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 Time:     2023/5/18 23:52
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     ECC.py
 Describe: 
 """
-from liuzhCrypto.basicMath.basic import invmod
-from liuzhCrypto.basicMath.type import TYPEPOINT, type_check
+from basicMath.basic import invmod
+from basicMath.type import TYPEPOINT, type_check
 
 # 无穷远点
 NULL_POINT: TYPEPOINT = (0, 0)
 
 
 class Curve:
     """
```

### Comparing `liuzh594Crypto-5.9.4.9.99/basicMath/GF.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/GF.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Time:     2023/5/18 16:26
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     GF.py
 Describe: GF(2^8)有限域上的基础运算
 """
-from liuzhCrypto.basicMath.type import type_check, TYPEMATRIX
+from basicMath.type import type_check, TYPEMATRIX
 
 
 def add_minus_GF(a: int, b: int) -> int:
     """
     GF(2^8)上的加减法
     :param a:
     :param b:
```

### Comparing `liuzh594Crypto-5.9.4.9.99/basicMath/basic.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Version:  V 1.1
 File:     basic.py
 Describe: 基础运算
 """
 from functools import reduce
 from random import randint
 
-from liuzhCrypto.basicMath.type import type_check, TYPEMATRIX
+from basicMath.type import type_check, TYPEMATRIX
 
 
 def Egcd(a: int, b: int) -> list:
     """
     扩展欧拉算法:au+bv=g
     :param a:
     :param b:
```

### Comparing `liuzh594Crypto-5.9.4.9.99/basicMath/type.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/basicMath/type.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.9.99/blockCipher/SM4.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/blockCipher/SM4.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     SM4.py
 Describe: 
 """
 import os.path
 
-from liuzhCrypto.basicMath.basic import rot_shift
-from liuzhCrypto.basicMath.type import HEXSTR, byte2hex, hex2byte, byte2int, TYPESM4, type_check
+from basicMath.basic import rot_shift
+from basicMath.type import HEXSTR, byte2hex, hex2byte, byte2int, TYPESM4, type_check
 
 # 工作模式加解密选择
 ENCRYPT: TYPESM4 = 1
 DECRYPT: TYPESM4 = 0
 
 # 文件加密工作模式选择
 MODEECB: TYPESM4 = ord("e")
```

### Comparing `liuzh594Crypto-5.9.4.9.99/digitalSignature/SM2_SV.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/digitalSignature/SM2_SV.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Time:     2023/5/18 23:50
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     SM2_SV.py
 Describe: 
 """
 from math import ceil, log
-from liuzhCrypto.basicMath.ECC import Curve, TYPEPOINT
-from liuzhCrypto.basicMath.basic import invmod
-from liuzhCrypto.basicMath.type import int2byte, type_check, byte2int
-from liuzhCrypto.hash.SM3 import SM3
+from basicMath.ECC import Curve, TYPEPOINT
+from basicMath.basic import invmod
+from basicMath.type import int2byte, type_check, byte2int
+from hash.SM3 import SM3
 
 
 class SM2_SV:
     """
     SM2数字签名类
     """
```

### Comparing `liuzh594Crypto-5.9.4.9.99/hash/SM3.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/hash/SM3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Time:     2023/5/19 00:01
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     SM3.py
 Describe: 
 """
 
-from liuzhCrypto.basicMath.basic import rot_shift
-from liuzhCrypto.basicMath.type import byte2int, int2byte, HEXSTR, BYTESDIGEST, HEXSTRDIGEST, type_check
+from basicMath.basic import rot_shift
+from basicMath.type import byte2int, int2byte, HEXSTR, BYTESDIGEST, HEXSTRDIGEST, type_check
 
 # 初始寄存器向量
 IV: list[int] = [0x7380166f, 0x4914b2b9, 0x172442d7, 0xda8a0600, 0xa96f30bc, 0x163138aa, 0xe38dee4d, 0xb0fb0e4e]
 # T参数
 T = [0x79cc4519, 0x7a879d8a]
```

### Comparing `liuzh594Crypto-5.9.4.9.99/liuzh594Crypto.egg-info/PKG-INFO` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.9.99
-Summary: my hcrypto python package in 2023
+Version: 5.9.4.99.9
+Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `liuzh594Crypto-5.9.4.9.99/pubkeyCipher/RSA.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/RSA.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     RSA.py
 Describe: 
 """
 from math import gcd
 
-from liuzhCrypto.basicMath.basic import get_prime, invmod, fast_power, crt
-from liuzhCrypto.basicMath.type import byte2int, int2byte, len_bytes, type_check
+from basicMath.basic import get_prime, invmod, fast_power, crt
+from basicMath.type import byte2int, int2byte, len_bytes, type_check
 
 
 class RSAkeyParam:
     """
     RSA密钥参数类
     """
```

### Comparing `liuzh594Crypto-5.9.4.9.99/pubkeyCipher/SM2.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/pubkeyCipher/SM2.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 Time:     2023/5/19 20:44
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     SM2.py
 Describe: 
 """
 from math import ceil, floor, log
-
-from libnum import ecc
-
-from liuzhCrypto.basicMath.ECC import Curve
-from liuzhCrypto.basicMath.type import int2byte, byte2int, point2byte, byte2point, TYPEPOINT, type_check, str2byte,byte2hex
-from liuzhCrypto.hash.SM3 import SM3
+from basicMath.ECC import Curve
+from basicMath.type import int2byte, byte2int, point2byte, byte2point, TYPEPOINT, type_check
+from hash.SM3 import SM3
 
 class SM2:
     """
     SM2类
     """
     crv: Curve
```

### Comparing `liuzh594Crypto-5.9.4.9.99/setup.py` & `liuzh594Crypto-5.9.4.99.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="liuzh594Crypto",
-    version="5.9.4.9.99",
+    version="5.9.4.99.9",
     author="Liuzhenghao",
     author_email="liuzh594@qq.com",
-    description="my hcrypto python package in 2023",
+    description="my crypto python package in 2023",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lzh594/liuzh594Crypto",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `liuzh594Crypto-5.9.4.9.99/tests/tests.py` & `liuzh594Crypto-5.9.4.99.9/liuzh594Crypto/tests/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 """
 Time:     2023/5/20 13:14
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     tests.py
 Describe: This is the test samples of liuzh594Crypto!
 """
-from liuzhCrypto.basicMath.ECC import *
-from liuzhCrypto.basicMath.GF import *
-from liuzhCrypto.basicMath.basic import *
-from liuzhCrypto.basicMath.type import *
-from liuzhCrypto.blockCipher.SM4 import *
-from liuzhCrypto.digitalSignature.SM2_SV import *
-from liuzhCrypto.hash.SM3 import *
-from liuzhCrypto.pubkeyCipher.RSA import *
-from liuzhCrypto.pubkeyCipher.SM2 import *
+from basicMath.ECC import *
+from basicMath.GF import *
+from basicMath.basic import *
+from basicMath.type import *
+from blockCipher.SM4 import *
+from digitalSignature.SM2_SV import *
+from hash.SM3 import *
+from pubkeyCipher.RSA import *
+from pubkeyCipher.SM2 import *
 
 
 def basic_test():
     """
     basic.py测试样例
     :return:
     """
```

