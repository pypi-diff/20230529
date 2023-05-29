# Comparing `tmp/python_pulsechain-0.1.1.tar.gz` & `tmp/python_pulsechain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_pulsechain-0.1.1.tar", max compression
+gzip compressed data, was "python_pulsechain-0.1.2.tar", max compression
```

## Comparing `python_pulsechain-0.1.1.tar` & `python_pulsechain-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-05-28 17:32:44.886854 python_pulsechain-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-28 17:32:44.887853 python_pulsechain-0.1.1/pulsechain/__init__.py
--rw-r--r--   0        0        0     6795 2023-05-28 18:49:51.868263 python_pulsechain-0.1.1/pulsechain/pulsechain.py
--rw-r--r--   0        0        0      555 2023-05-28 17:40:48.504476 python_pulsechain-0.1.1/pulsechain/utils.py
--rw-r--r--   0        0        0      647 2023-05-28 18:46:11.374229 python_pulsechain-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-28 17:33:46.774257 python_pulsechain-0.1.1/README.md
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 python_pulsechain-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-28 17:32:44.886854 python_pulsechain-0.1.2/LICENSE
+-rw-r--r--   0        0        0       96 2023-05-29 20:24:55.522194 python_pulsechain-0.1.2/pulsechain/__init__.py
+-rw-r--r--   0        0        0     4322 2023-05-29 20:22:41.619811 python_pulsechain-0.1.2/pulsechain/account.py
+-rw-r--r--   0        0        0     1675 2023-05-29 20:22:33.161714 python_pulsechain-0.1.2/pulsechain/token.py
+-rw-r--r--   0        0        0     1533 2023-05-29 20:21:56.386910 python_pulsechain-0.1.2/pulsechain/transaction.py
+-rw-r--r--   0        0        0      555 2023-05-28 17:40:48.504476 python_pulsechain-0.1.2/pulsechain/utils.py
+-rw-r--r--   0        0        0      647 2023-05-29 20:17:16.864734 python_pulsechain-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1827 2023-05-29 20:15:37.545898 python_pulsechain-0.1.2/README.md
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_pulsechain-0.1.2/PKG-INFO
```

### Comparing `python_pulsechain-0.1.1/LICENSE` & `python_pulsechain-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_pulsechain-0.1.1/pulsechain/utils.py` & `python_pulsechain-0.1.2/pulsechain/utils.py`

 * *Files identical despite different names*

### Comparing `python_pulsechain-0.1.1/pyproject.toml` & `python_pulsechain-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-pulsechain"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python implementation for PulseChain API"
 license = "MIT"
 repository = "https://github.com/crypto-ralph/python-pulsechain"
 authors = ["CryptoRalph <doxter@protonmail.com>"]
 readme = "README.md"
 include = [
     "LICENSE",
```

