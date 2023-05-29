# Comparing `tmp/SecuriPy-1.0.3.tar.gz` & `tmp/SecuriPy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.3.tar", last modified: Sat May 27 06:05:00 2023, max compression
+gzip compressed data, was "SecuriPy-1.0.5.tar", last modified: Mon May 29 17:32:27 2023, max compression
```

## Comparing `SecuriPy-1.0.3.tar` & `SecuriPy-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 06:05:00.495556 SecuriPy-1.0.3/
--rw-rw-rw-   0        0        0     3594 2023-05-27 06:05:00.494486 SecuriPy-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 06:05:00.492177 SecuriPy-1.0.3/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 06:05:00.000000 SecuriPy-1.0.3/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1663 2023-05-27 06:02:51.000000 SecuriPy-1.0.3/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 06:05:00.496064 SecuriPy-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-27 06:03:32.000000 SecuriPy-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 17:32:27.832889 SecuriPy-1.0.5/
+-rw-rw-rw-   0        0        0     3594 2023-05-29 17:32:27.828902 SecuriPy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 17:32:27.823913 SecuriPy-1.0.5/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 17:32:27.000000 SecuriPy-1.0.5/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1643 2023-05-29 17:28:25.000000 SecuriPy-1.0.5/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 17:32:27.832889 SecuriPy-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-29 17:28:54.000000 SecuriPy-1.0.5/setup.py
```

### Comparing `SecuriPy-1.0.3/PKG-INFO` & `SecuriPy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.3
+Version: 1.0.5
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.3/README.md` & `SecuriPy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.3/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.0.5/SecuriPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.3
+Version: 1.0.5
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.3/SecuriPy.py` & `SecuriPy-1.0.5/SecuriPy.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,23 +23,22 @@
     key = pwd(message, password)
     encrypted_text = []
     for i in range(len(message)):
         x = (ord(message[i]) +ord(key[i]) + 1000)
         encrypted_text.append(chr(x))
     encrypted_text = ("" . join(encrypted_text))
     key = ("".join(key))
-    return encrypted_text+key , key
+    return encrypted_text + " " + key
 
-def decrypt(encrypted_text, password):
+def decrypt(text, password):
     """Figures out the key from the encrypted text and decryptes it with respect to the key"""
     orig_text = []
-    b = int(len(encrypted_text)/2)
-    key = encrypted_text[b:]
-    encrypted_text = encrypted_text[:b-1]
-    if key == password:
+    encrypted_text = text.split(" ")[0]
+    key = pwd(encrypted_text, password)
+    if key == text.split(" ")[1]:
         for i in range(len(encrypted_text)):
             x = (ord(encrypted_text[i]) -ord(key[i]) - 1000)
             orig_text.append(chr(x))
         orig_text = ("" . join(orig_text))
-        return orig_text
+        return orig_text[:-1]
     else:
         return "Message is corrupt or Password is incorrect"
```

### Comparing `SecuriPy-1.0.3/setup.py` & `SecuriPy-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.3",
+    version="1.0.5",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

