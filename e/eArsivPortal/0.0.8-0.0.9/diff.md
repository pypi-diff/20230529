# Comparing `tmp/eArsivPortal-0.0.8.tar.gz` & `tmp/eArsivPortal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.8.tar", last modified: Mon May 29 16:00:46 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.9.tar", last modified: Mon May 29 16:22:47 2023, max compression
```

## Comparing `eArsivPortal-0.0.8.tar` & `eArsivPortal-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.276864 eArsivPortal-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:00:46.276864 eArsivPortal-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.288253 eArsivPortal-0.0.9/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:22:47.000000 eArsivPortal-0.0.9/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 16:22:47.000000 eArsivPortal-0.0.9/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:22:47.000000 eArsivPortal-0.0.9/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:22:47.000000 eArsivPortal-0.0.9/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 16:22:47.000000 eArsivPortal-0.0.9/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:22:47.292253 eArsivPortal-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 16:22:21.000000 eArsivPortal-0.0.9/setup.py
```

### Comparing `eArsivPortal-0.0.8/LICENSE` & `eArsivPortal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.8/PKG-INFO` & `eArsivPortal-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.8
+Version: 0.0.9
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.8 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.9 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
```

### Comparing `eArsivPortal-0.0.8/README.md` & `eArsivPortal-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.8/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.9/eArsivPortal/Core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,19 @@
         for tr in secici.xpath("//tr"):
             bos_tdler = tr.xpath(".//td[normalize-space(.)='\xa0']")
 
             if len(bos_tdler) == len(tr.xpath(".//td")):
                 tr_element = tr.root
                 tr_element.getparent().remove(tr_element)
 
+        for td in secici.xpath("//td[@align='right' and @class='lineTableTd']"):
+            if td.xpath("string(.)").get().strip() in ["%0,00", "0,00 TL", "İskonto -"]:
+                td_element = td.root
+                td_element.text = ""
+
         return secici.extract()
 
     def __fatura_ver(self, faturalar) -> list[dict] | Exception:
         if not isinstance(faturalar, list):
             faturalar = [faturalar]
 
         payload = []
```

### Comparing `eArsivPortal-0.0.8/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.9/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.8/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.9/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.8/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.9/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.8/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-0.0.9/eArsivPortal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.8
+Version: 0.0.9
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.8 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.9 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
```

### Comparing `eArsivPortal-0.0.8/setup.py` & `eArsivPortal-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.8",
+    version      = "0.0.9",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

