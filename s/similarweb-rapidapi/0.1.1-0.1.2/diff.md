# Comparing `tmp/similarweb_rapidapi-0.1.1.tar.gz` & `tmp/similarweb_rapidapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarweb_rapidapi-0.1.1.tar", last modified: Mon May 29 18:19:24 2023, max compression
+gzip compressed data, was "similarweb_rapidapi-0.1.2.tar", last modified: Mon May 29 18:22:25 2023, max compression
```

## Comparing `similarweb_rapidapi-0.1.1.tar` & `similarweb_rapidapi-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 18:19:24.682624 similarweb_rapidapi-0.1.1/
--rw-rw-rw-   0        0        0     1836 2023-05-29 18:19:24.683624 similarweb_rapidapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1492 2023-05-28 14:19:30.000000 similarweb_rapidapi-0.1.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-29 18:19:24.685622 similarweb_rapidapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      588 2023-05-29 18:19:21.000000 similarweb_rapidapi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:19:24.653625 similarweb_rapidapi-0.1.1/similarweb_rapidapi/
--rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/__init__.py
--rw-rw-rw-   0        0        0     7700 2023-05-25 19:45:05.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/api.py
--rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/logger_mock.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:19:24.681624 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/
--rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/__init__.py
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/base.py
--rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/basic_domain_data.py
--rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/cancel_task.py
--rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/complete_data_task.py
--rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/my_tasks.py
--rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/task.py
--rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/task_status.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:19:24.671624 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1836 2023-05-29 18:19:24.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-05-29 18:19:24.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 18:19:24.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 14:10:40.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-29 18:19:24.000000 similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.628493 similarweb_rapidapi-0.1.2/
+-rw-rw-rw-   0        0        0     1995 2023-05-29 18:22:25.628493 similarweb_rapidapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2023-05-29 18:22:08.000000 similarweb_rapidapi-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-29 18:22:25.630493 similarweb_rapidapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      579 2023-05-29 18:22:13.000000 similarweb_rapidapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.598492 similarweb_rapidapi-0.1.2/similarweb_rapidapi/
+-rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/__init__.py
+-rw-rw-rw-   0        0        0     7700 2023-05-25 19:45:05.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/api.py
+-rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/logger_mock.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.627493 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/
+-rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/base.py
+-rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/basic_domain_data.py
+-rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/cancel_task.py
+-rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/complete_data_task.py
+-rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/my_tasks.py
+-rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task.py
+-rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task_status.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:22:25.610494 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     1995 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 14:10:40.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-29 18:22:25.000000 similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/top_level.txt
```

### Comparing `similarweb_rapidapi-0.1.1/PKG-INFO` & `similarweb_rapidapi-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: similarweb_rapidapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: SimilarWeb API on RapidAPI
-Home-page: https://github.com/letsscrape/python_similarweb_rapidapi
+Home-page: https://letsscrape.com/scrapers/similarweb-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
 Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
 Description-Content-Type: text/markdown
 
 # SimilarWeb API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/similarweb_rapidapi/)
+## Read more on [main project page](https://letsscrape.com/scrapers/similarweb-api/)
+## See on [RapidAPI](https://rapidapi.com/letsscrape/api/similarweb-working-api)
 
 ## Install
 ### using pip
 ```
 pip install similarweb_rapidapi
 ```
 ### using poetry
```

### Comparing `similarweb_rapidapi-0.1.1/README.md` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+Metadata-Version: 2.1
+Name: similarweb-rapidapi
+Version: 0.1.2
+Summary: SimilarWeb API on RapidAPI
+Home-page: https://letsscrape.com/scrapers/similarweb-api/
+Author: LetsScrape
+Author-email: hello@letsscrape.com
+Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
+Description-Content-Type: text/markdown
+
 # SimilarWeb API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/similarweb_rapidapi/)
+## Read more on [main project page](https://letsscrape.com/scrapers/similarweb-api/)
+## See on [RapidAPI](https://rapidapi.com/letsscrape/api/similarweb-working-api)
 
 ## Install
 ### using pip
 ```
 pip install similarweb_rapidapi
 ```
 ### using poetry
@@ -52,8 +64,8 @@
     r = await api.get_basic_data_from_domain("google.com")
     print(r.status)
     print(r.data.site_name)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
-See the `tests/tests.py` file to see how to use it.
+See the `tests/tests.py` file to see how to use it.
```

### Comparing `similarweb_rapidapi-0.1.1/setup.py` & `similarweb_rapidapi-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='similarweb_rapidapi',
-    version='0.1.1',
+    version='0.1.2',
     description='SimilarWeb API on RapidAPI',
     packages=['similarweb_rapidapi', 'similarweb_rapidapi.schemas'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['rapidapi', 'similarweb', 'similarweb api', 'scraping', 'parsing', 'scraper'],
     classifiers=[],
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url='https://github.com/letsscrape/python_similarweb_rapidapi',
+    url='https://letsscrape.com/scrapers/similarweb-api/',
 )
```

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi/api.py` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi/api.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/basic_domain_data.py` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/basic_domain_data.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/my_tasks.py` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/my_tasks.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi/schemas/task.py` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi/schemas/task.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/PKG-INFO` & `similarweb_rapidapi-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-Metadata-Version: 2.1
-Name: similarweb-rapidapi
-Version: 0.1.1
-Summary: SimilarWeb API on RapidAPI
-Home-page: https://github.com/letsscrape/python_similarweb_rapidapi
-Author: LetsScrape
-Author-email: hello@letsscrape.com
-Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
-Description-Content-Type: text/markdown
-
 # SimilarWeb API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/similarweb_rapidapi/)
+## Read more on [main project page](https://letsscrape.com/scrapers/similarweb-api/)
+## See on [RapidAPI](https://rapidapi.com/letsscrape/api/similarweb-working-api)
 
 ## Install
 ### using pip
 ```
 pip install similarweb_rapidapi
 ```
 ### using poetry
@@ -62,8 +54,8 @@
     r = await api.get_basic_data_from_domain("google.com")
     print(r.status)
     print(r.data.site_name)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
-See the `tests/tests.py` file to see how to use it.
+See the `tests/tests.py` file to see how to use it.
```

### Comparing `similarweb_rapidapi-0.1.1/similarweb_rapidapi.egg-info/SOURCES.txt` & `similarweb_rapidapi-0.1.2/similarweb_rapidapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

