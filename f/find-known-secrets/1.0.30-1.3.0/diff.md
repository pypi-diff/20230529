# Comparing `tmp/find_known_secrets-1.0.30.tar.gz` & `tmp/find_known_secrets-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/find_known_secrets-1.0.30.tar", last modified: Fri Aug 10 18:27:15 2018, max compression
+gzip compressed data, was "find_known_secrets-1.3.0.tar", max compression
```

## Comparing `find_known_secrets-1.0.30.tar` & `find_known_secrets-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,10 @@
-drwxr-xr-x   0 martinmat (2121737075) NA\Domain Users (1645605201)        0 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/
-drwxr-xr-x   0 martinmat (2121737075) NA\Domain Users (1645605201)        0 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets/
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       78 2018-08-10 18:27:14.000000 find_known_secrets-1.0.30/find_known_secrets/__init__.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)      174 2018-07-26 20:23:45.000000 find_known_secrets-1.0.30/find_known_secrets/__main__.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       97 2018-08-10 18:27:14.000000 find_known_secrets-1.0.30/find_known_secrets/__version__.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       33 2018-07-24 19:08:12.000000 find_known_secrets-1.0.30/find_known_secrets/_secrets.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     1497 2018-07-26 15:40:16.000000 find_known_secrets-1.0.30/find_known_secrets/main.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     5125 2018-07-26 17:43:15.000000 find_known_secrets-1.0.30/find_known_secrets/searcher.py
-drwxr-xr-x   0 martinmat (2121737075) NA\Domain Users (1645605201)        0 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)        1 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       80 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/entry_points.txt
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     2414 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/PKG-INFO
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       16 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/requires.txt
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)      512 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       19 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/find_known_secrets.egg-info/top_level.txt
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     2414 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/PKG-INFO
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     1447 2018-08-10 18:27:14.000000 find_known_secrets-1.0.30/README.rst
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)       93 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/setup.cfg
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     3072 2018-08-10 18:26:42.000000 find_known_secrets-1.0.30/setup.py
-drwxr-xr-x   0 martinmat (2121737075) NA\Domain Users (1645605201)        0 2018-08-10 18:27:15.000000 find_known_secrets-1.0.30/test/
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)     1670 2018-07-24 19:08:03.000000 find_known_secrets-1.0.30/test/test_command_line.py
--rw-r--r--   0 martinmat (2121737075) NA\Domain Users (1645605201)      553 2018-07-24 14:33:34.000000 find_known_secrets-1.0.30/test/test_main.py
+-rw-r--r--   0        0        0     1071 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/README.md
+-rw-r--r--   0        0        0       64 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/__main__.py
+-rw-r--r--   0        0        0       83 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/__version__.py
+-rw-r--r--   0        0        0       78 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/_secrets.py
+-rw-r--r--   0        0        0     1322 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/main.py
+-rw-r--r--   0        0        0     4349 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/find_known_secrets/searcher.py
+-rw-r--r--   0        0        0     3917 2023-05-29 13:48:39.716246 find_known_secrets-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 find_known_secrets-1.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `find_known_secrets-1.0.30/find_known_secrets/searcher.py` & `find_known_secrets-1.3.0/find_known_secrets/searcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,107 @@
-# coding=utf-8
 """
 3 ways to find secrets I know of:
 
 - grep for THING = "xyzzy" and the like. dodgy and pylint does this.
 - search for high entropy strings. detect-secrets does this.
 - look up known secrets, e.g. values from an known .ini file, or values
   currently set in the environment
 
 """
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
-import tabulate
+import glob
 import os
-from typing import List, Tuple, Optional, Set, Dict
-
-
-from colorama import init, Fore, Back, Style
-
-_ = List
-
-try:
-    import configparser
-except ImportError:
-    # Python 2.x fallback
-    import ConfigParser as configparser
-
 import sys
+from typing import Optional
 
-if sys.version_info.major == 3:
-    unicode = str
-
+import tabulate
+from colorama import Back, Fore, Style, init
 
 init(autoreset=True)  # cross plat now
 
 
-class Searcher(object):
-    def __init__(self, source, files=None):  # type: (str,Optional[str]) -> None
+class Searcher:
+    """Look for possible secrets from common ini, config files"""
+
+    def __init__(self, source: str, files: Optional[str] = None) -> None:
+        """Set up initial state"""
         self.source = source
 
         self.files = ["~/.aws/credentials"]
         if files:
             for file in files.split(","):
                 self.files.append(file)
 
         # TODO: merge in more .ini files
 
         self.false_positives = ["localhost", "admin", "0.0.0.0"]
 
-        self.skip_files = []  # type: List[str]
+        self.skip_files: list[str] = []
         # TODO: merge in an ignore file
 
-        self.secrets = []  # type: List[str]
+        self.secrets: list[str] = []
 
-        self.found = {}  # type: Dict[str, List[Tuple[str,str]]]
+        self.found: dict[str, list[tuple[str, str]]] = {}
 
-    def append_known_secrets(self):  # type: () -> None
+    def append_known_secrets(self) -> None:
         """
         Read key-value pair files with secrets. For example, .conf and .ini files.
-        :return:
         """
         for file_name in self.files:
             if "~" in file_name:
                 file_name = os.path.expanduser(file_name)
             if not os.path.isfile(file_name):
-                print(
-                    "Don't have "
-                    + Back.BLACK
-                    + Fore.YELLOW
-                    + file_name
-                    + ", won't use."
-                )
+                print("Don't have " + Back.BLACK + Fore.YELLOW + file_name + ", won't use.")
                 continue
-            with open(os.path.expanduser(file_name), "r") as file:
+            with open(os.path.expanduser(file_name), encoding="utf-8") as file:
                 for line in file:
                     if line and "=" in line:
                         possible = line.split("=")[1].strip(" \"'\n")
                         if len(possible) > 4 and possible not in self.false_positives:
                             self.secrets.append(possible)
 
-    def search_known_secrets(self):  # type: () -> None
+    def search_known_secrets(self) -> None:
         """
-        Search a path for known secrets, outputing text and file when found
-        :return:
+        Search a path for known secrets, outputting text and file when found
         """
         count = 0
         here = os.path.abspath(self.source)
-        # python 3 only!
-        # for file in glob.glob(here + "/" + "**/*.*", recursive=True):
-
-        # py 2
-        matches = []
-        for root, dirnames, filenames in os.walk(here + "/"):
-            for filename in filenames:
-                matches.append(os.path.join(root, filename))
 
-        for file in matches:
+        for file in glob.glob(here + "/" + "**/*.*", recursive=True):
             if os.path.isdir(file):
                 continue
-            with open(file) as f:
+            with open(file, encoding="utf-8") as file_handle:
                 try:
-                    contents = f.read()
+                    contents = file_handle.read()
                 except UnicodeDecodeError:
                     continue
-                except Exception as e:
-                    print(e)
+                except Exception as exception:
+                    print(exception)
                     print(file)
                     raise
             for secret in self.secrets:
                 if secret in contents:
                     for line in contents.split("\n"):
                         if secret in line:
                             self.found.setdefault(file, []).append(
                                 (
                                     secret,
                                     line.replace(
                                         secret,
-                                        Fore.RED
-                                        + Back.YELLOW
-                                        + secret
-                                        + Style.RESET_ALL,
+                                        Fore.RED + Back.YELLOW + secret + Style.RESET_ALL,
                                     ),
                                 )
                             )
                             count += 1
 
-    def report(self):  # type: ()-> None
+    def report(self) -> None:
+        """Summarize findings"""
         current_directory = os.getcwd()
         count = len(self.found)
         if count > 0:
-            print(Fore.RED + "Found {0} secrets. Failing this run.".format(count))
+            print(Fore.RED + f"Found {count} secrets. Failing this run.")
 
             data = [
                 (
                     key.replace(current_directory, ""),
                     tabulate.tabulate(tabular_data=value, tablefmt="plain"),
                 )
                 for key, value in self.found.items()
@@ -141,26 +109,23 @@
             result = tabulate.tabulate(
                 tabular_data=data,
                 headers=("File", "Secret Found - Secret Text"),
                 tablefmt="grid",
             )
             print(result)
 
-            exit(-1)
+            sys.exit(-1)
         else:
-            print(
-                "No known secrets found. Consider trying out detect-secrets and git-secrets, too."
-            )
+            print("No known secrets found. Consider trying out detect-secrets and git-secrets, too.")
 
-    def go(self):  # type: () -> None
+    def run(self) -> None:
         """
         Entry point method
-        :return:
         """
         self.append_known_secrets()
         self.search_known_secrets()
         self.report()
 
 
 if __name__ == "__main__":
     searcher = Searcher("")
-    searcher.go()
+    searcher.run()
```

