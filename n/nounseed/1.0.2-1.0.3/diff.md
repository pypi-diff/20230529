# Comparing `tmp/nounseed-1.0.2.tar.gz` & `tmp/nounseed-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nounseed-1.0.2.tar", last modified: Sun May 28 23:45:01 2023, max compression
+gzip compressed data, was "nounseed-1.0.3.tar", last modified: Mon May 29 00:49:40 2023, max compression
```

## Comparing `nounseed-1.0.2.tar` & `nounseed-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.880256 nounseed-1.0.2/
--rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.2/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:45:01.880106 nounseed-1.0.2/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     1710 2023-05-28 23:44:14.000000 nounseed-1.0.2/README.md
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.879126 nounseed-1.0.2/nounseed/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.2/nounseed/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     5056 2023-05-28 23:43:50.000000 nounseed-1.0.2/nounseed/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.879894 nounseed-1.0.2/nounseed.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      277 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/top_level.txt
--rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.2/pyproject.toml
--rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-28 23:45:01.880302 nounseed-1.0.2/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-28 23:44:50.000000 nounseed-1.0.2/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.222531 nounseed-1.0.3/
+-rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.3/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:49:40.222386 nounseed-1.0.3/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     2626 2023-05-29 00:48:40.000000 nounseed-1.0.3/README
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.221650 nounseed-1.0.3/nounseed/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.3/nounseed/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     4970 2023-05-29 00:44:03.000000 nounseed-1.0.3/nounseed/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.222253 nounseed-1.0.3/nounseed.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      274 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/top_level.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.3/pyproject.toml
+-rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-29 00:49:40.222585 nounseed-1.0.3/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-29 00:49:11.000000 nounseed-1.0.3/setup.py
```

### Comparing `nounseed-1.0.2/LICENSE` & `nounseed-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nounseed-1.0.2/nounseed/__main__.py` & `nounseed-1.0.3/nounseed/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
 import random
 from pathlib import Path
 import argparse
 
 
-STORED_NOUNS_FILE = "storednouns.csv"
-CSV_FILE = "nounlist.csv"
+STORED_NOUNS_FILE = "nounseed/storednouns.csv"
+CSV_FILE = "nounseed/nounlist.csv"
 
 
 class NounSeeder:
     def __init__(self, nouns):
         self.nouns = nouns
 
     @classmethod
@@ -71,25 +71,24 @@
         new_ideas = []
         for _ in range(len(original_list) // 2):
             noun1, noun2 = random.sample(original_list, 2)
             new_ideas.append(f"{noun1}{noun2}")
         return new_ideas
 
     def store_ideas(self, choices, writer=print):
-        choices_lower = choices.lower()
-        if choices_lower == 'v':
+        if choices == 'v':
             self.view_stored_ideas(writer)
             return
-        elif choices_lower == 'r':
+        elif choices == 'r':
             self.ideas.extend(self.remix_ideas(self.original_list))
             writer("Remixed Project Ideas:")
             for i, idea in enumerate(self.ideas, start=1):
                 writer(f"{i}. {idea}")
             return
-        elif choices_lower == 'g':
+        elif choices == 'g':
             return 'g'
 
         stored_nouns_file = Path(STORED_NOUNS_FILE)
         with stored_nouns_file.open('a', newline='') as csvfile:
             csv_writer = csv.writer(csvfile)
             for choice in choices:
                 selected_idea = self.ideas[choice - 1]
@@ -131,16 +130,15 @@
             ideas_manager.ideas = ideas_manager.original_ideas
             continue
         elif choices == 'q':
             break
 
         ideas_manager.store_ideas(choices)
 
-        choices_lower = choices.lower()
-        if choices_lower != 'r':
+        if choices != 'r':
             break
 
         ideas_manager.ideas = ideas_manager.original_ideas
 
     print("Exiting the program.")
```

