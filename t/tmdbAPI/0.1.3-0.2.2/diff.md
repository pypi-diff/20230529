# Comparing `tmp/tmdbAPI-0.1.3.tar.gz` & `tmp/tmdbAPI-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmdbAPI-0.1.3.tar", last modified: Mon May 29 06:33:25 2023, max compression
+gzip compressed data, was "tmdbAPI-0.2.2.tar", last modified: Mon May 29 08:31:57 2023, max compression
```

## Comparing `tmdbAPI-0.1.3.tar` & `tmdbAPI-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:33:24.999816 tmdbAPI-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-29 06:33:11.000000 tmdbAPI-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 06:33:24.999816 tmdbAPI-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 06:33:11.000000 tmdbAPI-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:33:24.999816 tmdbAPI-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-29 06:33:11.000000 tmdbAPI-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:33:24.999816 tmdbAPI-0.1.3/tmdbAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 06:33:24.000000 tmdbAPI-0.1.3/tmdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 06:33:24.000000 tmdbAPI-0.1.3/tmdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:33:24.000000 tmdbAPI-0.1.3/tmdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 06:33:24.000000 tmdbAPI-0.1.3/tmdbAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 06:33:24.000000 tmdbAPI-0.1.3/tmdbAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-29 06:33:11.000000 tmdbAPI-0.1.3/tmdbAPI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:31:57.227971 tmdbAPI-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-29 08:31:42.000000 tmdbAPI-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 08:31:57.227971 tmdbAPI-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 08:31:42.000000 tmdbAPI-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:31:57.227971 tmdbAPI-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-29 08:31:42.000000 tmdbAPI-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:31:57.227971 tmdbAPI-0.2.2/tmdbAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 08:31:57.000000 tmdbAPI-0.2.2/tmdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 08:31:57.000000 tmdbAPI-0.2.2/tmdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:31:57.000000 tmdbAPI-0.2.2/tmdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 08:31:57.000000 tmdbAPI-0.2.2/tmdbAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 08:31:57.000000 tmdbAPI-0.2.2/tmdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-29 08:31:42.000000 tmdbAPI-0.2.2/tmdbAPI.py
```

### Comparing `tmdbAPI-0.1.3/LICENSE` & `tmdbAPI-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdbAPI-0.1.3/PKG-INFO` & `tmdbAPI-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmdbAPI
-Version: 0.1.3
+Version: 0.2.2
 Summary: Python Module for accessing the TVDB API
 Home-page: https://github.com/TehRiehlDeal/tmdbAPI
 Author: Kevin Riehl
 Author-email: kevinriehl@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tmdbAPI-0.1.3/setup.py` & `tmdbAPI-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     longDescription = f.read()
 
 # with open(path.join(here, 'requirements.txt')) as f:
 #     requirements = f.read().split('\n')
 
 setup(
     name="tmdbAPI",
-    version="0.1.3",
+    version="0.2.2",
     author="Kevin Riehl",
     author_email="kevinriehl@gmail.com",
     description="Python Module for accessing the TVDB API",
     long_description=longDescription,
     long_description_content_type="text/markdown",
     py_modules=['tmdbAPI'],
     install_requires=['requests >= 2.22.0', 'sanction >= 0.4.1'],
```

### Comparing `tmdbAPI-0.1.3/tmdbAPI.egg-info/PKG-INFO` & `tmdbAPI-0.2.2/tmdbAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmdbAPI
-Version: 0.1.3
+Version: 0.2.2
 Summary: Python Module for accessing the TVDB API
 Home-page: https://github.com/TehRiehlDeal/tmdbAPI
 Author: Kevin Riehl
 Author-email: kevinriehl@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tmdbAPI-0.1.3/tmdbAPI.py` & `tmdbAPI-0.2.2/tmdbAPI.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 import requests
 import sanction
+from classes.search import Search
 from difflib import SequenceMatcher
 
-#Exceptions
+# Exceptions
+
+
 class Error(Exception):
     pass
 
+
 class InvalidCredentials(Error):
     pass
 
+
 class ShowNotFound(Error):
     pass
 
+
 class NoSuchEpisode(Error):
     pass
 
+
 class InvalidShowID(Error):
     pass
 
+
 class InvalidInput(Error):
     pass
 
+
 class NoActorsFound(Error):
     pass
+
+
 class NoImagesFound(Error):
     pass
 
+
 class TMDB:
 
     def __init__(self, apikey='eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI3MjczNzI5MTZmZGM3Y2U3MDQ3YWMwOWYyNWRiYTQ3OSIsInN1YiI6IjYwNDg0N2RiNTQ1MDhkMDA3NzU4MzJhOSIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.YL-Dvu1RPqtnYkwReU5NdtQ-0umRvVkL0GC1zy_1k30'):
         self.headers = {
             'Accept': 'application/json',
             'Accept-Language': 'en-US',
             "Authorization": "Bearer {apikey}".format(apikey=apikey)
@@ -37,59 +49,49 @@
 
         self.config = {}
 
         self.config['apikey'] = apikey
 
         self.config['apiURL'] = "https://api.themoviedb.org/3"
 
-        self.config['tvSearchEndpoint'] = "{baseURL}/search/tv?language=en-US&query={showTitle}"
-
         self.config['episodeEndpoint'] = "{baseURL}/tv/{tv_id}/season/{season_number}/episode/{episode_number}?language=en-US"
 
         self.session = requests.Session()
 
-    def getShow(self, name):
-        if type(name) is not str:
-            raise InvalidInput("You have entered an invalid name. Please try again.")
-        url = self.config['tvSearchEndpoint'].format(baseURL=self.config['apiURL'], apikey=self.config['apikey'], showTitle=name)
-        r = self.session.get(url, headers=self.headers).json()
-        error = r.get('total_results') == 0
-        if error:
-            raise ShowNotFound("Show was not found, please try again")
-        return r
+        self.search = Search(apikey=apikey, session=self.session)
 
-    def getEpisodeName(self, name, seasonNum, epNum, accuracy = 0.8, id = None):
+    def getEpisodeName(self, name, seasonNum, epNum, accuracy=0.8, id=None):
         if type(name) is not str or type(seasonNum) is not int or type(epNum) is not int or seasonNum < 0 or epNum < 1:
             raise InvalidInput(
                 "You have entered an invalid name. Please try again.")
         if (id == None):
-            id = self._getShowID(name,accuracy)
+            id = self._getShowID(name, accuracy)
         else:
             return self._getEpisodeName(id, seasonNum, epNum)
         if id == -1:
             raise InvalidShowID
         return self._getEpisodeName(id, seasonNum, epNum)
 
-
     def _getShowID(self, name, accuracy=0.8):
-        url = self.config['tvSearchEndpoint'].format(baseURL=self.config['apiURL'], apikey=self.config['apikey'], showTitle=name)
-        r = self.session.get(url, headers=self.headers).json()
+        r = self.search.searchTV(name)
         error = r.get('Error')
         if error:
             raise ShowNotFound
         for show in r['results']:
             if SequenceMatcher(None, name.lower(), show['name'].lower()).ratio() >= accuracy:
                 return show['id']
         return -1
 
     def _getEpisodeName(self, id, seasonNum, epNum):
-        url = self.config['episodeEndpoint'].format(baseURL=self.config['apiURL'], tv_id=id, season_number=seasonNum, episode_number=epNum, apikey=self.config['apikey'])
+        url = self.config['episodeEndpoint'].format(
+            baseURL=self.config['apiURL'], tv_id=id, season_number=seasonNum, episode_number=epNum)
         r = self.session.get(url, headers=self.headers).json()
         error = r.get('Error')
         if error:
-            raise NoSuchEpisode("No episode could be found. Please check season or episode number and try again.")
+            raise NoSuchEpisode(
+                "No episode could be found. Please check season or episode number and try again.")
         return self._cleanName(r["name"])
 
     def _cleanName(self, name):
-        newName = name.replace('\\', "").replace("/", "").replace(":", "").replace("*", "").replace("?", "").replace('"', "").replace("<", "").replace(">", "").replace("|", "").replace("\t","")
-        return newName 
-    
+        newName = name.replace('\\', "").replace("/", "").replace(":", "").replace("*", "").replace(
+            "?", "").replace('"', "").replace("<", "").replace(">", "").replace("|", "").replace("\t", "")
+        return newName
```

