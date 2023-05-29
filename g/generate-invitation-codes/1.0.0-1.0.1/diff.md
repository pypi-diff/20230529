# Comparing `tmp/generate-invitation-codes-1.0.0.tar.gz` & `tmp/generate-invitation-codes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate-invitation-codes-1.0.0.tar", last modified: Mon May 29 08:45:01 2023, max compression
+gzip compressed data, was "generate-invitation-codes-1.0.1.tar", last modified: Mon May 29 08:47:34 2023, max compression
```

## Comparing `generate-invitation-codes-1.0.0.tar` & `generate-invitation-codes-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 08:45:01.758860 generate-invitation-codes-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1562 2023-05-29 08:45:01.758702 generate-invitation-codes-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1451 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 08:45:01.758467 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1562 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      295 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       77 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       26 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     1260 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/generate_invitation_codes.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-29 08:45:01.758899 generate-invitation-codes-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      564 2023-05-29 08:45:01.000000 generate-invitation-codes-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 08:47:34.853960 generate-invitation-codes-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1569 2023-05-29 08:47:34.853810 generate-invitation-codes-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1458 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-29 08:47:34.853489 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1569 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      295 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       77 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       26 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     1260 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/generate_invitation_codes.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-29 08:47:34.853999 generate-invitation-codes-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      564 2023-05-29 08:47:34.000000 generate-invitation-codes-1.0.1/setup.py
```

### Comparing `generate-invitation-codes-1.0.0/PKG-INFO` & `generate-invitation-codes-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: generate-invitation-codes
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # generate-invitation-codes
-
+```
 🐔動機：為了讓全球試用生成試用碼，所以生成長度任意的數量的試用碼
 💣地雷：一次就 gpt-4 成功，沒有地雷
+```
 
 這是一個 Python 套件，可以用來生成全球試用的邀請碼。您可以通過命令行界面或將其導入到其他 Python 項目中使用。
 
 ## 安裝
 使用以下命令安裝：
 
 ```sh
```

### Comparing `generate-invitation-codes-1.0.0/README.md` & `generate-invitation-codes-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # generate-invitation-codes
-
+```
 🐔動機：為了讓全球試用生成試用碼，所以生成長度任意的數量的試用碼
 💣地雷：一次就 gpt-4 成功，沒有地雷
+```
 
 這是一個 Python 套件，可以用來生成全球試用的邀請碼。您可以通過命令行界面或將其導入到其他 Python 項目中使用。
 
 ## 安裝
 使用以下命令安裝：
 
 ```sh
```

### Comparing `generate-invitation-codes-1.0.0/generate_invitation_codes.egg-info/PKG-INFO` & `generate-invitation-codes-1.0.1/generate_invitation_codes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: generate-invitation-codes
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # generate-invitation-codes
-
+```
 🐔動機：為了讓全球試用生成試用碼，所以生成長度任意的數量的試用碼
 💣地雷：一次就 gpt-4 成功，沒有地雷
+```
 
 這是一個 Python 套件，可以用來生成全球試用的邀請碼。您可以通過命令行界面或將其導入到其他 Python 項目中使用。
 
 ## 安裝
 使用以下命令安裝：
 
 ```sh
```

### Comparing `generate-invitation-codes-1.0.0/generate_invitation_codes.py` & `generate-invitation-codes-1.0.1/generate_invitation_codes.py`

 * *Files identical despite different names*

### Comparing `generate-invitation-codes-1.0.0/setup.py` & `generate-invitation-codes-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="generate-invitation-codes",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['generate_invitation_codes'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'generate_invitation_codes = generate_invitation_codes:main',
         ],
```

