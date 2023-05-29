# Comparing `tmp/ngscrape-1.0.1.tar.gz` & `tmp/ngscrape-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.0.1.tar", last modified: Sun May 28 19:55:05 2023, max compression
+gzip compressed data, was "ngscrape-1.1.0.tar", last modified: Mon May 29 18:02:23 2023, max compression
```

## Comparing `ngscrape-1.0.1.tar` & `ngscrape-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.935881 ngscrape-1.0.1/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    42296 2023-05-28 19:55:05.933879 ngscrape-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-28 19:54:46.000000 ngscrape-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.0.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-28 19:55:05.936897 ngscrape-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.894883 ngscrape-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.900879 ngscrape-1.0.1/src/ngscrape/
--rw-rw-rw-   0        0        0     3663 2023-05-28 19:51:27.000000 ngscrape-1.0.1/src/ngscrape/ngscrape.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:55:05.931874 ngscrape-1.0.1/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    42296 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 19:55:05.000000 ngscrape-1.0.1/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.513325 ngscrape-1.1.0/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    42296 2023-05-29 18:02:23.511322 ngscrape-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-29 18:01:50.000000 ngscrape-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.1.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 18:02:23.513325 ngscrape-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.479204 ngscrape-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.479204 ngscrape-1.1.0/src/ngscrape/
+-rw-rw-rw-   0        0        0     3764 2023-05-29 18:00:06.000000 ngscrape-1.1.0/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.509323 ngscrape-1.1.0/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    42296 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.0.1/LICENSE` & `ngscrape-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.0.1/PKG-INFO` & `ngscrape-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.0.1
+Version: 1.1.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,15 +666,15 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/aeiea/ngscrape
 Keywords: flash,newgrounds,scraper,games,opensource
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NGScrape
 Newgrounds game scraper made with beautifulsoup4 and requestslib.
 
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
```

### Comparing `ngscrape-1.0.1/pyproject.toml` & `ngscrape-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.0.1"
+version = "1.1.0"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["flash", "newgrounds", "scraper", "games", "opensource"]
 dependencies = ["beautifulsoup4", "requests"]
-requires-python = ">=3.7"
+requires-python = ">=3.0"
 [project.urls]
 Homepage = "https://github.com/aeiea/ngscrape"
```

### Comparing `ngscrape-1.0.1/readme.md` & `ngscrape-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `ngscrape-1.0.1/src/ngscrape/ngscrape.py` & `ngscrape-1.1.0/src/ngscrape/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # NGScrape - Newgrounds game scraper made with beautifulsoup4 and requestslib.
 # NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 # The source code can be found at https://github.com/aeiea/ngscrape. Please star is this was useful, and make a pull request if you find this useful!
 
-import bs4
-import requests
+import bs4, requests, os
 class Scraper:
     '''
     # NGScrape
     Newgrounds game scraper made with beautifulsoup4 and requestslib.
     
     NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
     
@@ -55,18 +54,22 @@
         Example:
         var embed_controller = new embedController([{"url":"https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499","is_published":true, ... );
                             0                          1  2                                     [3]
         '''
         _scripts = _soup.find_all('script')
         for i in _scripts:
             if 'var embed_controller = new embedController([{"url":"' in i.get_text():
-                _gameLink = i.get_text().split('"')[3]
+                _gameLink: str = i.get_text().split('"')[3]
                 if self.debug:
                     print('NGScrape: Found flash game link ' + _gameLink)
-        open(download + '/' + filename, 'wb').write(requests.get(_gameLink, allow_redirects = True).content)
+        try:
+            os.mkdir(download)
+        except:
+            pass
+        open(download + '/' + filename, 'wb').write(requests.get(_gameLink.replace('\\', ''), allow_redirects = True).content)
         if self.debug:
             print('NGScrape: Downloaded swf file to ' + download + '/' + filename)
                 
 if __name__ == '__main__':
     import sys
     scraper = Scraper(debug = True)
     scraper.scrape_game_by_url(sys.argv[1], sys.argv[2], sys.argv[3])
```

### Comparing `ngscrape-1.0.1/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.1.0/src/ngscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.0.1
+Version: 1.1.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,15 +666,15 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/aeiea/ngscrape
 Keywords: flash,newgrounds,scraper,games,opensource
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NGScrape
 Newgrounds game scraper made with beautifulsoup4 and requestslib.
 
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
```

