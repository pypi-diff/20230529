# Comparing `tmp/datamarket-0.3.4.tar.gz` & `tmp/datamarket-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.3.4.tar", last modified: Fri May 26 09:46:24 2023, max compression
+gzip compressed data, was "datamarket-0.3.5.tar", last modified: Mon May 29 09:15:25 2023, max compression
```

## Comparing `datamarket-0.3.4.tar` & `datamarket-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.205071 datamarket-0.3.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-26 09:46:24.205071 datamarket-0.3.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.4/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-26 09:46:24.205071 datamarket-0.3.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-26 09:46:08.000000 datamarket-0.3.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.201071 datamarket-0.3.4/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.201071 datamarket-0.3.4/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.4/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.205071 datamarket-0.3.4/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.4/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.4/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.4/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.4/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.4/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.4/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.205071 datamarket-0.3.4/src/datamarket/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.4/src/datamarket/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.4/src/datamarket/utils/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2201 2023-05-26 08:15:10.000000 datamarket-0.3.4/src/datamarket/utils/selenium.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-26 09:46:24.205071 datamarket-0.3.4/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-26 09:46:24.000000 datamarket-0.3.4/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-05-26 09:46:24.000000 datamarket-0.3.4/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-26 09:46:24.000000 datamarket-0.3.4/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-26 09:46:24.000000 datamarket-0.3.4/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-26 09:46:24.000000 datamarket-0.3.4/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.621495 datamarket-0.3.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-29 09:15:25.621495 datamarket-0.3.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.5/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-29 09:15:25.621495 datamarket-0.3.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-29 09:15:06.000000 datamarket-0.3.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.617495 datamarket-0.3.5/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.617495 datamarket-0.3.5/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.5/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.621495 datamarket-0.3.5/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.5/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.5/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.5/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.5/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.5/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.5/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.621495 datamarket-0.3.5/src/datamarket/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-26 09:46:08.000000 datamarket-0.3.5/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.5/src/datamarket/utils/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2207 2023-05-29 09:15:06.000000 datamarket-0.3.5/src/datamarket/utils/selenium.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 09:15:25.617495 datamarket-0.3.5/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-29 09:15:25.000000 datamarket-0.3.5/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-05-29 09:15:25.000000 datamarket-0.3.5/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 09:15:25.000000 datamarket-0.3.5/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-29 09:15:25.000000 datamarket-0.3.5/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-29 09:15:25.000000 datamarket-0.3.5/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.3.4/LICENSE` & `datamarket-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/PKG-INFO` & `datamarket-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.4
+Version: 0.3.5
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.4/README.md` & `datamarket-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/setup.py` & `datamarket-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "stem",
     "pydrive",
     "undetected_chromedriver",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.3.4",
+    version="0.3.5",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.3.4/src/datamarket/interfaces/alchemy.py` & `datamarket-0.3.5/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/interfaces/drive.py` & `datamarket-0.3.5/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/interfaces/ftp.py` & `datamarket-0.3.5/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/interfaces/proxy.py` & `datamarket-0.3.5/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/interfaces/tinybird.py` & `datamarket-0.3.5/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/utils/main.py` & `datamarket-0.3.5/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.4/src/datamarket/utils/selenium.py` & `datamarket-0.3.5/src/datamarket/utils/selenium.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     return uc.Chrome(version_main=get_chromedriver_version(),
                      options=options)
 
 
 def wait(driver, css_selector, timeout=30):
     logger.info(f"waiting for {css_selector}...")
-    return WebDriverWait(driver, timeout).until(EC.element_to_be_clickable(("css selector", css_selector)))
+    return WebDriverWait(driver, timeout).until(EC.visibility_of_element_located(("css selector", css_selector)))
 
 
 def wait_and_click(driver, css_selector, timeout=30):
     logger.info(f"clicking on {css_selector}...")
     wait(driver, css_selector, timeout).click()
```

### Comparing `datamarket-0.3.4/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.3.5/src/datamarket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.4
+Version: 0.3.5
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.4/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.3.5/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

