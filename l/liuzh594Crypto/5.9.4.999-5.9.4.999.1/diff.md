# Comparing `tmp/liuzh594Crypto-5.9.4.999.tar.gz` & `tmp/liuzh594Crypto-5.9.4.999.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liuzh594Crypto-5.9.4.999.tar", last modified: Mon May 29 02:52:27 2023, max compression
+gzip compressed data, was "liuzh594Crypto-5.9.4.999.1.tar", last modified: Mon May 29 07:49:03 2023, max compression
```

## Comparing `liuzh594Crypto-5.9.4.999.tar` & `liuzh594Crypto-5.9.4.999.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.730894 liuzh594Crypto-5.9.4.999/
--rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.999/LICENSE
--rw-r--r--   0 lzh        (501) staff       (20)     6963 2023-05-29 02:52:27.730749 liuzh594Crypto-5.9.4.999/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)     6291 2023-05-28 15:17:55.000000 liuzh594Crypto-5.9.4.999/README.md
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.726584 liuzh594Crypto-5.9.4.999/liuzh594Crypto/
--rw-r--r--   0 lzh        (501) staff       (20)      169 2023-05-29 02:21:01.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.728132 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/
--rw-r--r--   0 lzh        (501) staff       (20)     6250 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/ECC.py
--rw-r--r--   0 lzh        (501) staff       (20)     3550 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/GF.py
--rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-18 08:36:11.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     5630 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/basic.py
--rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-20 12:49:00.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/type.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.728422 liuzh594Crypto-5.9.4.999/liuzh594Crypto/blockCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     9452 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/blockCipher/SM4.py
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:37.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/blockCipher/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.728798 liuzh594Crypto-5.9.4.999/liuzh594Crypto/digitalSignature/
--rw-r--r--   0 lzh        (501) staff       (20)     3221 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/digitalSignature/SM2_SV.py
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/digitalSignature/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.729194 liuzh594Crypto-5.9.4.999/liuzh594Crypto/hash/
--rw-r--r--   0 lzh        (501) staff       (20)     5589 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/hash/SM3.py
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/hash/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.730086 liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/
--rw-r--r--   0 lzh        (501) staff       (20)     3192 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/RSA.py
--rw-r--r--   0 lzh        (501) staff       (20)     3603 2023-05-29 02:50:47.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/SM2.py
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:21:12.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/__init__.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.730560 liuzh594Crypto-5.9.4.999/liuzh594Crypto/tests/
--rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:10:38.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/tests/__init__.py
--rw-r--r--   0 lzh        (501) staff       (20)     9215 2023-05-29 02:51:06.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto/tests/tests.py
-drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 02:52:27.727290 liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/
--rw-r--r--   0 lzh        (501) staff       (20)     6963 2023-05-29 02:52:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/PKG-INFO
--rw-r--r--   0 lzh        (501) staff       (20)      763 2023-05-29 02:52:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/SOURCES.txt
--rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 02:52:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/dependency_links.txt
--rw-r--r--   0 lzh        (501) staff       (20)       15 2023-05-29 02:52:27.000000 liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/top_level.txt
--rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 02:52:27.730935 liuzh594Crypto-5.9.4.999/setup.cfg
--rw-r--r--   0 lzh        (501) staff       (20)     1070 2023-05-29 02:47:54.000000 liuzh594Crypto-5.9.4.999/setup.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.622715 liuzh594Crypto-5.9.4.999.1/
+-rw-r--r--   0 lzh        (501) staff       (20)     1067 2023-05-26 12:17:24.000000 liuzh594Crypto-5.9.4.999.1/LICENSE
+-rw-r--r--   0 lzh        (501) staff       (20)     7441 2023-05-29 07:49:03.622553 liuzh594Crypto-5.9.4.999.1/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)     6767 2023-05-29 03:30:17.000000 liuzh594Crypto-5.9.4.999.1/README.md
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.617934 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/
+-rw-r--r--   0 lzh        (501) staff       (20)      169 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.619745 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/
+-rw-r--r--   0 lzh        (501) staff       (20)     6300 2023-05-29 07:45:53.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/ECC.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3575 2023-05-29 07:46:24.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/GF.py
+-rw-r--r--   0 lzh        (501) staff       (20)      173 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     5655 2023-05-29 07:45:53.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/basic.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3121 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/type.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.620281 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/blockCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     9452 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/blockCipher/SM4.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/blockCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.620725 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/digitalSignature/
+-rw-r--r--   0 lzh        (501) staff       (20)     3221 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/digitalSignature/SM2_SV.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/digitalSignature/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.621077 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/hash/
+-rw-r--r--   0 lzh        (501) staff       (20)     5589 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/hash/SM3.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/hash/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.621629 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/
+-rw-r--r--   0 lzh        (501) staff       (20)     3192 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/RSA.py
+-rw-r--r--   0 lzh        (501) staff       (20)     3603 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/SM2.py
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/__init__.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.621991 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/tests/
+-rw-r--r--   0 lzh        (501) staff       (20)      170 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/tests/__init__.py
+-rw-r--r--   0 lzh        (501) staff       (20)     9215 2023-05-29 02:55:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/tests/tests.py
+drwxr-xr-x   0 lzh        (501) staff       (20)        0 2023-05-29 07:49:03.618633 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/
+-rw-r--r--   0 lzh        (501) staff       (20)     7441 2023-05-29 07:49:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/PKG-INFO
+-rw-r--r--   0 lzh        (501) staff       (20)      763 2023-05-29 07:49:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 lzh        (501) staff       (20)        1 2023-05-29 07:49:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       15 2023-05-29 07:49:03.000000 liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/top_level.txt
+-rw-r--r--   0 lzh        (501) staff       (20)       38 2023-05-29 07:49:03.622766 liuzh594Crypto-5.9.4.999.1/setup.cfg
+-rw-r--r--   0 lzh        (501) staff       (20)     1072 2023-05-29 07:48:54.000000 liuzh594Crypto-5.9.4.999.1/setup.py
```

### Comparing `liuzh594Crypto-5.9.4.999/LICENSE` & `liuzh594Crypto-5.9.4.999.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/PKG-INFO` & `liuzh594Crypto-5.9.4.999.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.999
+Version: 5.9.4.999.1
 Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,100 +34,103 @@
 
 + ### [支持github和PyPI](#写在最后)：latest release请关注Github
 
 ## 项目目录结构
 
 ```bash
 liuzh594Crypto
+├── LICENSE
 ├── README.md
-├── __init__.py
-├── basicMath  # 基础数学库
+├── liuzh594Crypto # 包
 │   ├── __init__.py
-│   ├── ECC.py
-│   ├── GF.py
-│   ├── basic.py
-│   └── type.py
-├── blockCipher # 分组密码学库
-│   ├── __init__.py
-│   ├── SM4.py
-├── pubkeyCipher # 公钥密码学库
-│   └── __init__.py
-│   ├── RSA.py
-│   ├── SM2.py
-├── hash # 哈希算法库
-│   ├── __init__.py
-│   ├── SM3.py
-├── digitalSignature # 数字签名算法库
-│   └── __init__.py
-│   ├── SM2_SV.py
-├── liuzh594Crypto.egg-info
-├── dist
-│   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # liuzh594crypto完整版测试样例
-│   └── tests.py 
+│   ├── basicMath # 基础数学库
+│   │   ├── __init__.py
+│   │   ├── ECC.py
+│   │   ├── GF.py
+│   │   ├── basic.py
+│   │   └── type.py
+│   ├── blockCipher # 分组密码学库
+│   │   ├── __init__.py
+│   │   ├── SM4.py
+│   ├── digitalSignature # 数字签名库
+│   │   ├── __init__.py
+│   │   ├── SM2_SV.py
+│   ├── hash # 哈希算法库
+│   │   ├── __init__.py
+│   │   ├── SM3.py
+│   ├── pubkeyCipher # 公钥密码学库
+│   │   ├── __init__.py
+│   │   ├── RSA.py
+│   │   ├── SM2.py
+│   └── tests # 测试样例库
+│       ├── __init__.py
+│       ├── pic_original.bmp
+│       ├── pic_original_CBC.bmp
+│       ├── pic_original_ECB.bmp
+│       └── tests.py
 └── setup.py
 ```
 
 
 
 ## 项目功能
 
-+ ### [基础数学库](./basicMath):
++ ### [基础数学库](./liuzh594Crypto/basicMath):
 
-    + #### [密码学数学运算](./basicMath/basic.py)
+    + #### [密码学数学运算](./liuzh594Crypto/basicMath/basic.py)
 
         + ##### 支持欧拉算法、模逆运算、快速（模）幂（矩阵）运算、素数生成与检验和中国剩余定理等一系列密码学基础数学运算
 
-    + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
+    + #### [椭圆曲线上的数学运算](./liuzh594Crypto/basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
-    + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
+    + #### [有限域GF(2^8)上的数学运算](./liuzh594Crypto/basicMath/GF.py)
 
         + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
-    + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
+    + #### [本密码学库涉及到的类型转换等操作](./liuzh594Crypto/basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
-+ ### [对称密码学/分组密码学库](./blockCipher)
++ ### [对称密码学/分组密码学库](./liuzh594Crypto/blockCipher)
 
-    + #### [SM4分组密码](./blockCipher/SM4.py)
+    + #### [SM4分组密码](./liuzh594Crypto/blockCipher/SM4.py)
 
         + ##### SM4支持分组长度128比特，密钥长度128比特的分组密码加解密运算
 
         + ##### 支持SM4的ECB和CBC的分组密码工作模式
 
         + ##### 支持基于ECB或CBC工作模式的对文件的加解密处理
 
-+ ### [非对称密码学/公钥密码学库](./pubkeyCipher)
++ ### [非对称密码学/公钥密码学库](./liuzh594Crypto/pubkeyCipher)
 
-    + #### [RSA公钥密码](./pubkeyCipher/RSA.py)
+    + #### [RSA公钥密码](./liuzh594Crypto/pubkeyCipher/RSA.py)
 
         + ##### 支持RSA密钥参数的生成
 
         + ##### 支持RSA的加解密运算
 
-    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./pubkeyCipher/SM2.py)
+    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./liuzh594Crypto/pubkeyCipher/SM2.py)
 
         + ##### 支持杂凑函数为SM3（可替换）的SM2公钥加密算法
 
-+ ### [哈希算法/杂凑函数库](./hash)
++ ### [哈希算法/杂凑函数库](./liuzh594Crypto/hash)
 
-    + #### [SM3密码杂凑算法](./hash/SM3.py)
+    + #### [SM3密码杂凑算法](./liuzh594Crypto/hash/SM3.py)
 
         + ##### 支持输出长度为256比特的消息摘要，消息摘要的输出类型包括十六进制字符串以及字节串两种类型
 
         + ##### 支持对文件的消息摘要生成
 
-+ ### [数字签名算法](./digitalSignature)
++ ### [数字签名算法](./liuzh594Crypto/digitalSignature)
 
-    + #### [SM2椭圆曲线公钥密码：数字签名算法](./digitalSignature/SM2_SV.py)
+    + #### [SM2椭圆曲线公钥密码：数字签名算法](./liuzh594Crypto/digitalSignature/SM2_SV.py)
 
         + ##### 支持基于椭圆曲线的数字签名算法SM2
 
 
 
 ## 项目特色
 
@@ -169,29 +172,29 @@
     python -m pip install liuzh594Crypto
     ```
 
     + ##### 对于 POSIX 用户（包括 macOS 和 Linux 用户）本指南中的示例假定使用了 [virtual environment/pyenv]。对于 Windows 用户，本指南中的示例假定在安装 Python 时选择了修改系统 PATH 环境变量。
 
 ## 项目样例
 
-+ ### 源码详见[完整版测试样例](./tests/tests.py)
++ ### 源码详见[完整版测试样例](./liuzh594Crypto/tests/tests.py)
 
 + ### 在主程序部分可以根据测试者的需求，添加或减少注释函数进行部分测试
 
 ```python
 if __name__ == "__main__":
     """
     可以根据测试需求进行代码注释部分的添加与解除
     """
     """
     basicMath测试样例
     """
     basic_test()
     type_test()
-  	ECC_test()
+    ECC_test()
     GF_test()
 
     """
     blockCipher测试样例
     """
     SM4_test()
 
@@ -232,8 +235,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto)
```

### Comparing `liuzh594Crypto-5.9.4.999/README.md` & `liuzh594Crypto-5.9.4.999.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,100 +16,103 @@
 
 + ### [支持github和PyPI](#写在最后)：latest release请关注Github
 
 ## 项目目录结构
 
 ```bash
 liuzh594Crypto
+├── LICENSE
 ├── README.md
-├── __init__.py
-├── basicMath  # 基础数学库
+├── liuzh594Crypto # 包
 │   ├── __init__.py
-│   ├── ECC.py
-│   ├── GF.py
-│   ├── basic.py
-│   └── type.py
-├── blockCipher # 分组密码学库
-│   ├── __init__.py
-│   ├── SM4.py
-├── pubkeyCipher # 公钥密码学库
-│   └── __init__.py
-│   ├── RSA.py
-│   ├── SM2.py
-├── hash # 哈希算法库
-│   ├── __init__.py
-│   ├── SM3.py
-├── digitalSignature # 数字签名算法库
-│   └── __init__.py
-│   ├── SM2_SV.py
-├── liuzh594Crypto.egg-info
-├── dist
-│   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # liuzh594crypto完整版测试样例
-│   └── tests.py 
+│   ├── basicMath # 基础数学库
+│   │   ├── __init__.py
+│   │   ├── ECC.py
+│   │   ├── GF.py
+│   │   ├── basic.py
+│   │   └── type.py
+│   ├── blockCipher # 分组密码学库
+│   │   ├── __init__.py
+│   │   ├── SM4.py
+│   ├── digitalSignature # 数字签名库
+│   │   ├── __init__.py
+│   │   ├── SM2_SV.py
+│   ├── hash # 哈希算法库
+│   │   ├── __init__.py
+│   │   ├── SM3.py
+│   ├── pubkeyCipher # 公钥密码学库
+│   │   ├── __init__.py
+│   │   ├── RSA.py
+│   │   ├── SM2.py
+│   └── tests # 测试样例库
+│       ├── __init__.py
+│       ├── pic_original.bmp
+│       ├── pic_original_CBC.bmp
+│       ├── pic_original_ECB.bmp
+│       └── tests.py
 └── setup.py
 ```
 
 
 
 ## 项目功能
 
-+ ### [基础数学库](./basicMath):
++ ### [基础数学库](./liuzh594Crypto/basicMath):
 
-    + #### [密码学数学运算](./basicMath/basic.py)
+    + #### [密码学数学运算](./liuzh594Crypto/basicMath/basic.py)
 
         + ##### 支持欧拉算法、模逆运算、快速（模）幂（矩阵）运算、素数生成与检验和中国剩余定理等一系列密码学基础数学运算
 
-    + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
+    + #### [椭圆曲线上的数学运算](./liuzh594Crypto/basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
-    + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
+    + #### [有限域GF(2^8)上的数学运算](./liuzh594Crypto/basicMath/GF.py)
 
         + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
-    + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
+    + #### [本密码学库涉及到的类型转换等操作](./liuzh594Crypto/basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
-+ ### [对称密码学/分组密码学库](./blockCipher)
++ ### [对称密码学/分组密码学库](./liuzh594Crypto/blockCipher)
 
-    + #### [SM4分组密码](./blockCipher/SM4.py)
+    + #### [SM4分组密码](./liuzh594Crypto/blockCipher/SM4.py)
 
         + ##### SM4支持分组长度128比特，密钥长度128比特的分组密码加解密运算
 
         + ##### 支持SM4的ECB和CBC的分组密码工作模式
 
         + ##### 支持基于ECB或CBC工作模式的对文件的加解密处理
 
-+ ### [非对称密码学/公钥密码学库](./pubkeyCipher)
++ ### [非对称密码学/公钥密码学库](./liuzh594Crypto/pubkeyCipher)
 
-    + #### [RSA公钥密码](./pubkeyCipher/RSA.py)
+    + #### [RSA公钥密码](./liuzh594Crypto/pubkeyCipher/RSA.py)
 
         + ##### 支持RSA密钥参数的生成
 
         + ##### 支持RSA的加解密运算
 
-    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./pubkeyCipher/SM2.py)
+    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./liuzh594Crypto/pubkeyCipher/SM2.py)
 
         + ##### 支持杂凑函数为SM3（可替换）的SM2公钥加密算法
 
-+ ### [哈希算法/杂凑函数库](./hash)
++ ### [哈希算法/杂凑函数库](./liuzh594Crypto/hash)
 
-    + #### [SM3密码杂凑算法](./hash/SM3.py)
+    + #### [SM3密码杂凑算法](./liuzh594Crypto/hash/SM3.py)
 
         + ##### 支持输出长度为256比特的消息摘要，消息摘要的输出类型包括十六进制字符串以及字节串两种类型
 
         + ##### 支持对文件的消息摘要生成
 
-+ ### [数字签名算法](./digitalSignature)
++ ### [数字签名算法](./liuzh594Crypto/digitalSignature)
 
-    + #### [SM2椭圆曲线公钥密码：数字签名算法](./digitalSignature/SM2_SV.py)
+    + #### [SM2椭圆曲线公钥密码：数字签名算法](./liuzh594Crypto/digitalSignature/SM2_SV.py)
 
         + ##### 支持基于椭圆曲线的数字签名算法SM2
 
 
 
 ## 项目特色
 
@@ -151,29 +154,29 @@
     python -m pip install liuzh594Crypto
     ```
 
     + ##### 对于 POSIX 用户（包括 macOS 和 Linux 用户）本指南中的示例假定使用了 [virtual environment/pyenv]。对于 Windows 用户，本指南中的示例假定在安装 Python 时选择了修改系统 PATH 环境变量。
 
 ## 项目样例
 
-+ ### 源码详见[完整版测试样例](./tests/tests.py)
++ ### 源码详见[完整版测试样例](./liuzh594Crypto/tests/tests.py)
 
 + ### 在主程序部分可以根据测试者的需求，添加或减少注释函数进行部分测试
 
 ```python
 if __name__ == "__main__":
     """
     可以根据测试需求进行代码注释部分的添加与解除
     """
     """
     basicMath测试样例
     """
     basic_test()
     type_test()
-  	ECC_test()
+    ECC_test()
     GF_test()
 
     """
     blockCipher测试样例
     """
     SM4_test()
 
@@ -214,8 +217,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto)
```

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/ECC.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/ECC.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 Time:     2023/5/18 23:52
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     ECC.py
 Describe: 
 """
-from basic import invmod
-from type import TYPEPOINT, type_check
+from liuzh594Crypto.basicMath.basic import invmod
+from liuzh594Crypto.basicMath.type import TYPEPOINT, type_check
 
 # 无穷远点
 NULL_POINT: TYPEPOINT = (0, 0)
 
 
 class Curve:
     """
```

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/GF.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/GF.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Time:     2023/5/18 16:26
 Author:   刘征昊(£·)
 Version:  V 1.1
 File:     GF.py
 Describe: GF(2^8)有限域上的基础运算
 """
-from type import type_check, TYPEMATRIX
+from liuzh594Crypto.basicMath.type import type_check, TYPEMATRIX
 
 
 def add_minus_GF(a: int, b: int) -> int:
     """
     GF(2^8)上的加减法
     :param a:
     :param b:
```

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/basic.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Version:  V 1.1
 File:     basic.py
 Describe: 基础运算
 """
 from functools import reduce
 from random import randint
 
-from type import type_check, TYPEMATRIX
+from liuzh594Crypto.basicMath.type import type_check, TYPEMATRIX
 
 
 def Egcd(a: int, b: int) -> list:
     """
     扩展欧拉算法:au+bv=g
     :param a:
     :param b:
```

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/basicMath/type.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/basicMath/type.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/blockCipher/SM4.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/blockCipher/SM4.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/digitalSignature/SM2_SV.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/digitalSignature/SM2_SV.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/hash/SM3.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/hash/SM3.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/RSA.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/RSA.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/pubkeyCipher/SM2.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/pubkeyCipher/SM2.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto/tests/tests.py` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto/tests/tests.py`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/PKG-INFO` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liuzh594Crypto
-Version: 5.9.4.999
+Version: 5.9.4.999.1
 Summary: my crypto python package in 2023
 Home-page: https://github.com/lzh594/liuzh594Crypto
 Author: Liuzhenghao
 Author-email: liuzh594@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,100 +34,103 @@
 
 + ### [支持github和PyPI](#写在最后)：latest release请关注Github
 
 ## 项目目录结构
 
 ```bash
 liuzh594Crypto
+├── LICENSE
 ├── README.md
-├── __init__.py
-├── basicMath  # 基础数学库
+├── liuzh594Crypto # 包
 │   ├── __init__.py
-│   ├── ECC.py
-│   ├── GF.py
-│   ├── basic.py
-│   └── type.py
-├── blockCipher # 分组密码学库
-│   ├── __init__.py
-│   ├── SM4.py
-├── pubkeyCipher # 公钥密码学库
-│   └── __init__.py
-│   ├── RSA.py
-│   ├── SM2.py
-├── hash # 哈希算法库
-│   ├── __init__.py
-│   ├── SM3.py
-├── digitalSignature # 数字签名算法库
-│   └── __init__.py
-│   ├── SM2_SV.py
-├── liuzh594Crypto.egg-info
-├── dist
-│   └── liuzh594Crypto-5.9.4.tar.gz
-├── tests # liuzh594crypto完整版测试样例
-│   └── tests.py 
+│   ├── basicMath # 基础数学库
+│   │   ├── __init__.py
+│   │   ├── ECC.py
+│   │   ├── GF.py
+│   │   ├── basic.py
+│   │   └── type.py
+│   ├── blockCipher # 分组密码学库
+│   │   ├── __init__.py
+│   │   ├── SM4.py
+│   ├── digitalSignature # 数字签名库
+│   │   ├── __init__.py
+│   │   ├── SM2_SV.py
+│   ├── hash # 哈希算法库
+│   │   ├── __init__.py
+│   │   ├── SM3.py
+│   ├── pubkeyCipher # 公钥密码学库
+│   │   ├── __init__.py
+│   │   ├── RSA.py
+│   │   ├── SM2.py
+│   └── tests # 测试样例库
+│       ├── __init__.py
+│       ├── pic_original.bmp
+│       ├── pic_original_CBC.bmp
+│       ├── pic_original_ECB.bmp
+│       └── tests.py
 └── setup.py
 ```
 
 
 
 ## 项目功能
 
-+ ### [基础数学库](./basicMath):
++ ### [基础数学库](./liuzh594Crypto/basicMath):
 
-    + #### [密码学数学运算](./basicMath/basic.py)
+    + #### [密码学数学运算](./liuzh594Crypto/basicMath/basic.py)
 
         + ##### 支持欧拉算法、模逆运算、快速（模）幂（矩阵）运算、素数生成与检验和中国剩余定理等一系列密码学基础数学运算
 
-    + #### [椭圆曲线上的数学运算](./basicMath/ECC.py)
+    + #### [椭圆曲线上的数学运算](./liuzh594Crypto/basicMath/ECC.py)
 
         + ##### 支持椭圆曲线密码学所需的常见数学运算，如：椭圆曲线上的点的加减法和倍点运算，其中倍点运算支持double-and-add、NAF以及w-NAF三种方法
 
-    + #### [有限域GF(2^8)上的数学运算](./basicMath/GF.py)
+    + #### [有限域GF(2^8)上的数学运算](./liuzh594Crypto/basicMath/GF.py)
 
         + ##### 支持有限域GF(2^8)上的常见数学运算，如：四则运算、逆元、矩阵运算等
 
-    + #### [本密码学库涉及到的类型转换等操作](./basicMath/type.py)
+    + #### [本密码学库涉及到的类型转换等操作](./liuzh594Crypto/basicMath/type.py)
 
         + ##### 自定义了一系列本项目其他文件所需的变量类型
 
         + ##### 支持十六进制、字节串、字符串、整数、椭圆曲线上的点等变量类型之间的相互转化
 
-+ ### [对称密码学/分组密码学库](./blockCipher)
++ ### [对称密码学/分组密码学库](./liuzh594Crypto/blockCipher)
 
-    + #### [SM4分组密码](./blockCipher/SM4.py)
+    + #### [SM4分组密码](./liuzh594Crypto/blockCipher/SM4.py)
 
         + ##### SM4支持分组长度128比特，密钥长度128比特的分组密码加解密运算
 
         + ##### 支持SM4的ECB和CBC的分组密码工作模式
 
         + ##### 支持基于ECB或CBC工作模式的对文件的加解密处理
 
-+ ### [非对称密码学/公钥密码学库](./pubkeyCipher)
++ ### [非对称密码学/公钥密码学库](./liuzh594Crypto/pubkeyCipher)
 
-    + #### [RSA公钥密码](./pubkeyCipher/RSA.py)
+    + #### [RSA公钥密码](./liuzh594Crypto/pubkeyCipher/RSA.py)
 
         + ##### 支持RSA密钥参数的生成
 
         + ##### 支持RSA的加解密运算
 
-    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./pubkeyCipher/SM2.py)
+    + #### [SM2椭圆曲线公钥密码:公钥加密算法](./liuzh594Crypto/pubkeyCipher/SM2.py)
 
         + ##### 支持杂凑函数为SM3（可替换）的SM2公钥加密算法
 
-+ ### [哈希算法/杂凑函数库](./hash)
++ ### [哈希算法/杂凑函数库](./liuzh594Crypto/hash)
 
-    + #### [SM3密码杂凑算法](./hash/SM3.py)
+    + #### [SM3密码杂凑算法](./liuzh594Crypto/hash/SM3.py)
 
         + ##### 支持输出长度为256比特的消息摘要，消息摘要的输出类型包括十六进制字符串以及字节串两种类型
 
         + ##### 支持对文件的消息摘要生成
 
-+ ### [数字签名算法](./digitalSignature)
++ ### [数字签名算法](./liuzh594Crypto/digitalSignature)
 
-    + #### [SM2椭圆曲线公钥密码：数字签名算法](./digitalSignature/SM2_SV.py)
+    + #### [SM2椭圆曲线公钥密码：数字签名算法](./liuzh594Crypto/digitalSignature/SM2_SV.py)
 
         + ##### 支持基于椭圆曲线的数字签名算法SM2
 
 
 
 ## 项目特色
 
@@ -169,29 +172,29 @@
     python -m pip install liuzh594Crypto
     ```
 
     + ##### 对于 POSIX 用户（包括 macOS 和 Linux 用户）本指南中的示例假定使用了 [virtual environment/pyenv]。对于 Windows 用户，本指南中的示例假定在安装 Python 时选择了修改系统 PATH 环境变量。
 
 ## 项目样例
 
-+ ### 源码详见[完整版测试样例](./tests/tests.py)
++ ### 源码详见[完整版测试样例](./liuzh594Crypto/tests/tests.py)
 
 + ### 在主程序部分可以根据测试者的需求，添加或减少注释函数进行部分测试
 
 ```python
 if __name__ == "__main__":
     """
     可以根据测试需求进行代码注释部分的添加与解除
     """
     """
     basicMath测试样例
     """
     basic_test()
     type_test()
-  	ECC_test()
+    ECC_test()
     GF_test()
 
     """
     blockCipher测试样例
     """
     SM4_test()
 
@@ -232,8 +235,8 @@
 
     + ##### 注释
 
     + ##### ... ...
 
 + ### 本项目已上传至[github](https://github.com/lzh594/liuzh594Crypto)
 
-+ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto/5.9.4/)
++ ### 本项目已上传至[PyPI](https://pypi.org/project/liuzh594Crypto)
```

### Comparing `liuzh594Crypto-5.9.4.999/liuzh594Crypto.egg-info/SOURCES.txt` & `liuzh594Crypto-5.9.4.999.1/liuzh594Crypto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liuzh594Crypto-5.9.4.999/setup.py` & `liuzh594Crypto-5.9.4.999.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="liuzh594Crypto",
-    version="5.9.4.999",
+    version="5.9.4.999.1",
     author="Liuzhenghao",
     author_email="liuzh594@qq.com",
     description="my crypto python package in 2023",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lzh594/liuzh594Crypto",
     packages=setuptools.find_packages(),
```

