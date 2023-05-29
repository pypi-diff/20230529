# Comparing `tmp/hey-mindsdb-0.1.0.tar.gz` & `tmp/hey_mindsdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hey-mindsdb-0.1.0.tar", last modified: Tue Apr 25 10:28:06 2023, max compression
+gzip compressed data, was "hey_mindsdb-0.1.1.tar", last modified: Mon May 29 09:54:44 2023, max compression
```

## Comparing `hey-mindsdb-0.1.0.tar` & `hey_mindsdb-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.957208 hey-mindsdb-0.1.0/
--rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey-mindsdb-0.1.0/LICENSE
--rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey-mindsdb-0.1.0/MANIFEST.in
--rw-r--r--   0 sadra      (501) staff       (20)     5163 2023-04-25 10:28:06.957273 hey-mindsdb-0.1.0/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)     3964 2023-04-24 08:41:20.000000 hey-mindsdb-0.1.0/README.md
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.952882 hey-mindsdb-0.1.0/hey/
--rw-r--r--   0 sadra      (501) staff       (20)      126 2023-04-25 10:27:53.000000 hey-mindsdb-0.1.0/hey/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2780 2023-04-23 05:58:41.000000 hey-mindsdb-0.1.0/hey/cli.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.953901 hey-mindsdb-0.1.0/hey/constants/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey-mindsdb-0.1.0/hey/constants/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      550 2023-04-23 16:07:39.000000 hey-mindsdb-0.1.0/hey/constants/informations.py
--rw-r--r--   0 sadra      (501) staff       (20)      130 2023-04-22 08:20:35.000000 hey-mindsdb-0.1.0/hey/constants/service.py
--rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey-mindsdb-0.1.0/hey/constants/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.954701 hey-mindsdb-0.1.0/hey/exceptions/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey-mindsdb-0.1.0/hey/exceptions/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey-mindsdb-0.1.0/hey/exceptions/auth.py
--rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey-mindsdb-0.1.0/hey/exceptions/connection.py
--rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey-mindsdb-0.1.0/hey/exceptions/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.955058 hey-mindsdb-0.1.0/hey/middlewares/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey-mindsdb-0.1.0/hey/middlewares/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2607 2023-04-24 16:07:38.000000 hey-mindsdb-0.1.0/hey/middlewares/mindsdb.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.955362 hey-mindsdb-0.1.0/hey/templates/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-24 06:30:05.000000 hey-mindsdb-0.1.0/hey/templates/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      153 2023-04-24 07:25:14.000000 hey-mindsdb-0.1.0/hey/templates/mindsdb_queries.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.956609 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/
--rw-r--r--   0 sadra      (501) staff       (20)     5163 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)      685 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/SOURCES.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/dependency_links.txt
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/entry_points.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/not-zip-safe
--rw-r--r--   0 sadra      (501) staff       (20)       49 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/requires.txt
--rw-r--r--   0 sadra      (501) staff       (20)        4 2023-04-25 10:28:06.000000 hey-mindsdb-0.1.0/hey_mindsdb.egg-info/top_level.txt
--rw-r--r--   0 sadra      (501) staff       (20)     1660 2023-04-25 10:28:06.957593 hey-mindsdb-0.1.0/setup.cfg
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey-mindsdb-0.1.0/setup.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-04-25 10:28:06.956975 hey-mindsdb-0.1.0/tests/
--rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey-mindsdb-0.1.0/tests/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey-mindsdb-0.1.0/tests/test_accounts.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635686 hey_mindsdb-0.1.1/
+-rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey_mindsdb-0.1.1/LICENSE
+-rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey_mindsdb-0.1.1/MANIFEST.in
+-rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-05-29 09:54:44.635776 hey_mindsdb-0.1.1/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)     3969 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/README.md
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.631824 hey_mindsdb-0.1.1/hey/
+-rw-r--r--   0 sadra      (501) staff       (20)      126 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/hey/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2841 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/hey/cli.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632269 hey_mindsdb-0.1.1/hey/constants/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey_mindsdb-0.1.1/hey/constants/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      550 2023-04-23 16:07:39.000000 hey_mindsdb-0.1.1/hey/constants/informations.py
+-rw-r--r--   0 sadra      (501) staff       (20)      130 2023-05-07 16:48:50.000000 hey_mindsdb-0.1.1/hey/constants/service.py
+-rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey_mindsdb-0.1.1/hey/constants/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632703 hey_mindsdb-0.1.1/hey/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey_mindsdb-0.1.1/hey/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey_mindsdb-0.1.1/hey/exceptions/auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey_mindsdb-0.1.1/hey/exceptions/connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey_mindsdb-0.1.1/hey/exceptions/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632919 hey_mindsdb-0.1.1/hey/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey_mindsdb-0.1.1/hey/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2564 2023-05-22 09:08:57.000000 hey_mindsdb-0.1.1/hey/middlewares/mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.633172 hey_mindsdb-0.1.1/hey/templates/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-24 06:30:05.000000 hey_mindsdb-0.1.1/hey/templates/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      153 2023-04-24 07:25:14.000000 hey_mindsdb-0.1.1/hey/templates/mindsdb_queries.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634213 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/
+-rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)      962 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/entry_points.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/not-zip-safe
+-rw-r--r--   0 sadra      (501) staff       (20)       49 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/requires.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        4 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/top_level.txt
+-rw-r--r--   0 sadra      (501) staff       (20)     1440 2023-05-29 09:54:44.636203 hey_mindsdb-0.1.1/setup.cfg
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey_mindsdb-0.1.1/setup.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634555 hey_mindsdb-0.1.1/tests/
+-rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey_mindsdb-0.1.1/tests/__init__.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634958 hey_mindsdb-0.1.1/tests/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      194 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)      178 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      589 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635214 hey_mindsdb-0.1.1/tests/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     1700 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/middlewares/test_mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635575 hey_mindsdb-0.1.1/tests/templates/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/templates/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      542 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/templates/test_mindsdb_queries.py
+-rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey_mindsdb-0.1.1/tests/test_accounts.py
+-rw-r--r--   0 sadra      (501) staff       (20)      249 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/tests/test_cli.py
```

### Comparing `hey-mindsdb-0.1.0/LICENSE` & `hey_mindsdb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.1.0/PKG-INFO` & `hey_mindsdb-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 Metadata-Version: 2.1
-Name: hey-mindsdb
-Version: 0.1.0
+Name: hey_mindsdb
+Version: 0.1.1
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
-License: MIT license
+License: MIT
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Hey! - Your AI-powered Pair Programming Friend
 
 > :basecamp: - Watch this YouTube <a href="https://www.youtube.com/watch?v=fhO34PVa-38&list=LL&index=9">introduction video</a> about Hey!
 
-> :writing_hand: - Read the <a href="https://imsadra/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
+> :writing_hand: - Read the <a href="https://imsadra.me/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
 
 > :package: - Check out <a href="https://pypi.org/project/hey-mindsdb/">Hey on PyPI</a>.
 
 Hey is a CLI-based AI assistant that is powered by the ChatGPT AI model versions supported by [MindsDB](https://mindsdb.com/). This project is designed for [Hashnode X MindsDB](https://hashnode.com/hackathons/mindsdb?source=hncounter-feed) hackathon.
 
 ### Installation
 Make sure you have `pip` and `python>=3.6` installed on your machine and follow the steps.
@@ -76,21 +70,21 @@
 > :bulb:: Read the article for more information about training your MindsDB model.
 
 </details>
 
 <details>
   <summary><h4>3. Set your MindsDB account password</h4></summary>
 
-Now, it's time to set your account's password. Simply run `hey` with `--set-password` followed by your MindsDB account password to set your password.
+Now, it's time to set your account's password. Simply run `hey` with the `--auth` option and enter your MindsDB account password.
 
 ```sh
-hey --set-password <PASSWORD>
+hey --auth
 ```
 
-You're ready to go. :)
+You're all set to go. :)
 
 </details>
 
 ### Usage
 Use `hey` followed by your question and it'll process the phrase and responses back the content in Markdown.
 
 ```
@@ -139,14 +133,14 @@
 - Tools
     - [Python](https://python.org)
 - Infrastructures & Hosting
     - [MindsDB](https://mindsdb.com)
     - [PyPI](https://pypi.org)
 
 ### License
-Hey is being licensed under the [MIT License](LICENSE).
+Hey is being licensed under the [MIT License](https://github.com/lnxpy/hey/blob/main/LICENSE).
 
 ### Special Thanks to
 [MindsDB](https://mindsdb.com) X [Hashnode](https://hashnode.com) for hosting this great hackathon.
 
 <img src="media/badge-dark.svg#gh-dark-mode-only" width=350 height=90>
 <img src="media/badge-light.svg#gh-light-mode-only" width=350 height=90>
```

### Comparing `hey-mindsdb-0.1.0/README.md` & `hey_mindsdb-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Hey! - Your AI-powered Pair Programming Friend
 
 > :basecamp: - Watch this YouTube <a href="https://www.youtube.com/watch?v=fhO34PVa-38&list=LL&index=9">introduction video</a> about Hey!
 
-> :writing_hand: - Read the <a href="https://imsadra/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
+> :writing_hand: - Read the <a href="https://imsadra.me/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
 
 > :package: - Check out <a href="https://pypi.org/project/hey-mindsdb/">Hey on PyPI</a>.
 
 Hey is a CLI-based AI assistant that is powered by the ChatGPT AI model versions supported by [MindsDB](https://mindsdb.com/). This project is designed for [Hashnode X MindsDB](https://hashnode.com/hackathons/mindsdb?source=hncounter-feed) hackathon.
 
 ### Installation
 Make sure you have `pip` and `python>=3.6` installed on your machine and follow the steps.
@@ -45,21 +45,21 @@
 > :bulb:: Read the article for more information about training your MindsDB model.
 
 </details>
 
 <details>
   <summary><h4>3. Set your MindsDB account password</h4></summary>
 
-Now, it's time to set your account's password. Simply run `hey` with `--set-password` followed by your MindsDB account password to set your password.
+Now, it's time to set your account's password. Simply run `hey` with the `--auth` option and enter your MindsDB account password.
 
 ```sh
-hey --set-password <PASSWORD>
+hey --auth
 ```
 
-You're ready to go. :)
+You're all set to go. :)
 
 </details>
 
 ### Usage
 Use `hey` followed by your question and it'll process the phrase and responses back the content in Markdown.
 
 ```
@@ -108,14 +108,14 @@
 - Tools
     - [Python](https://python.org)
 - Infrastructures & Hosting
     - [MindsDB](https://mindsdb.com)
     - [PyPI](https://pypi.org)
 
 ### License
-Hey is being licensed under the [MIT License](LICENSE).
+Hey is being licensed under the [MIT License](https://github.com/lnxpy/hey/blob/main/LICENSE).
 
 ### Special Thanks to
 [MindsDB](https://mindsdb.com) X [Hashnode](https://hashnode.com) for hosting this great hackathon.
 
 <img src="media/badge-dark.svg#gh-dark-mode-only" width=350 height=90>
 <img src="media/badge-light.svg#gh-light-mode-only" width=350 height=90>
```

### Comparing `hey-mindsdb-0.1.0/hey/cli.py` & `hey_mindsdb-0.1.1/hey/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
 import sys
+from getpass import getpass
 
 import keyring
 from rich.console import Console
 
 from hey import __version__
 from hey.constants.informations import APPLICATION_DESCRIPTION, EPILOG_DESCRIPTION, INSTALLATION_GUIDE, VERSION_INFO
 from hey.constants.service import SERVICE_NAME
@@ -27,33 +28,33 @@
 parser.add_argument(
     '--version',
     action='version',
     version=VERSION_INFO.format(__version__),
 )
 
 parser.add_argument(
-    '--set-password',
-    type=str,
+    '--auth',
+    action='store_true',
     help='set your mindsdb account password',
-    metavar='',
 )
 
 
 def main():
     args = parser.parse_args()
     console = Console()
 
-    if args.set_password:
+    if args.auth:
         email_address = os.environ.get(LOCAL_EMAIL_ADDRESS_VARIABLE_NAME)
+        password = getpass(f'Password for ({email_address}):')
         if email_address:
             try:
                 keyring.set_password(
                     service_name=SERVICE_NAME.lower(),
                     username=email_address,
-                    password=args.set_password,
+                    password=password,
                 )
             except Exception as _:
                 raise KeyringIssue(
                     'There is something wrong with your OS keyring system. Make sure you have right access to run hey '
                     'on your system. '
                 )
             console.print(f'Password successfully set for {email_address}!')
```

### Comparing `hey-mindsdb-0.1.0/hey/constants/informations.py` & `hey_mindsdb-0.1.1/hey/constants/informations.py`

 * *Files identical despite different names*

### Comparing `hey-mindsdb-0.1.0/hey/middlewares/mindsdb.py` & `hey_mindsdb-0.1.1/hey/middlewares/mindsdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,14 @@
 
         self.is_authenticated: bool = False
         self.database: Database
 
     def authenticate(self) -> None:
         """
         authorizes the email and password with MindsDB's host
-        Returns:
-            server object
         """
 
         try:
             server = mindsdb_sdk.connect(
                 MINDSDB_HOST,
                 login=self.email,
                 password=self.password,
```

### Comparing `hey-mindsdb-0.1.0/hey_mindsdb.egg-info/PKG-INFO` & `hey_mindsdb-0.1.1/hey_mindsdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 Metadata-Version: 2.1
 Name: hey-mindsdb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
-License: MIT license
+License: MIT
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Hey! - Your AI-powered Pair Programming Friend
 
 > :basecamp: - Watch this YouTube <a href="https://www.youtube.com/watch?v=fhO34PVa-38&list=LL&index=9">introduction video</a> about Hey!
 
-> :writing_hand: - Read the <a href="https://imsadra/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
+> :writing_hand: - Read the <a href="https://imsadra.me/introducing-hey-your-ai-powered-pair-programming-friend">"Introducing Hey! - Your AI-powered Pair Programming Friend"</a> article about the creation process, development phases, and a detailed overview of Hey.
 
 > :package: - Check out <a href="https://pypi.org/project/hey-mindsdb/">Hey on PyPI</a>.
 
 Hey is a CLI-based AI assistant that is powered by the ChatGPT AI model versions supported by [MindsDB](https://mindsdb.com/). This project is designed for [Hashnode X MindsDB](https://hashnode.com/hackathons/mindsdb?source=hncounter-feed) hackathon.
 
 ### Installation
 Make sure you have `pip` and `python>=3.6` installed on your machine and follow the steps.
@@ -76,21 +70,21 @@
 > :bulb:: Read the article for more information about training your MindsDB model.
 
 </details>
 
 <details>
   <summary><h4>3. Set your MindsDB account password</h4></summary>
 
-Now, it's time to set your account's password. Simply run `hey` with `--set-password` followed by your MindsDB account password to set your password.
+Now, it's time to set your account's password. Simply run `hey` with the `--auth` option and enter your MindsDB account password.
 
 ```sh
-hey --set-password <PASSWORD>
+hey --auth
 ```
 
-You're ready to go. :)
+You're all set to go. :)
 
 </details>
 
 ### Usage
 Use `hey` followed by your question and it'll process the phrase and responses back the content in Markdown.
 
 ```
@@ -139,14 +133,14 @@
 - Tools
     - [Python](https://python.org)
 - Infrastructures & Hosting
     - [MindsDB](https://mindsdb.com)
     - [PyPI](https://pypi.org)
 
 ### License
-Hey is being licensed under the [MIT License](LICENSE).
+Hey is being licensed under the [MIT License](https://github.com/lnxpy/hey/blob/main/LICENSE).
 
 ### Special Thanks to
 [MindsDB](https://mindsdb.com) X [Hashnode](https://hashnode.com) for hosting this great hackathon.
 
 <img src="media/badge-dark.svg#gh-dark-mode-only" width=350 height=90>
 <img src="media/badge-light.svg#gh-light-mode-only" width=350 height=90>
```

### Comparing `hey-mindsdb-0.1.0/hey_mindsdb.egg-info/SOURCES.txt` & `hey_mindsdb-0.1.1/hey_mindsdb.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -21,8 +21,17 @@
 hey_mindsdb.egg-info/SOURCES.txt
 hey_mindsdb.egg-info/dependency_links.txt
 hey_mindsdb.egg-info/entry_points.txt
 hey_mindsdb.egg-info/not-zip-safe
 hey_mindsdb.egg-info/requires.txt
 hey_mindsdb.egg-info/top_level.txt
 tests/__init__.py
-tests/test_accounts.py
+tests/test_accounts.py
+tests/test_cli.py
+tests/exceptions/__init__.py
+tests/exceptions/test_auth.py
+tests/exceptions/test_connection.py
+tests/exceptions/test_system.py
+tests/middlewares/__init__.py
+tests/middlewares/test_mindsdb.py
+tests/templates/__init__.py
+tests/templates/test_mindsdb_queries.py
```

