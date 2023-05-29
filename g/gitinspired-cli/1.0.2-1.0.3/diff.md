# Comparing `tmp/gitinspired-cli-1.0.2.tar.gz` & `tmp/gitinspired-cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitinspired-cli-1.0.2.tar", last modified: Sun May 21 10:33:28 2023, max compression
+gzip compressed data, was "gitinspired-cli-1.0.3.tar", last modified: Mon May 29 17:41:43 2023, max compression
```

## Comparing `gitinspired-cli-1.0.2.tar` & `gitinspired-cli-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)     1078 2023-05-18 15:12:54.000000 gitinspired-cli-1.0.2/LICENSE
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/PKG-INFO
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      156 2023-05-18 16:04:24.000000 gitinspired-cli-1.0.2/README.md
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      162 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/PKG-INFO
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      319 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        1 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       56 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/entry_points.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        9 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/requires.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        4 2023-05-21 10:33:28.000000 gitinspired-cli-1.0.2/gitinspired_cli.egg-info/top_level.txt
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       38 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/setup.cfg
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      298 2023-05-21 10:33:18.000000 gitinspired-cli-1.0.2/setup.py
-drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-21 10:33:28.862757 gitinspired-cli-1.0.2/src/
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        0 2023-05-18 15:26:18.000000 gitinspired-cli-1.0.2/src/__init__.py
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      861 2023-05-21 10:30:23.000000 gitinspired-cli-1.0.2/src/file_manager.py
--rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      779 2023-05-21 10:31:53.000000 gitinspired-cli-1.0.2/src/greetings_cli.py
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-29 17:41:43.611469 gitinspired-cli-1.0.3/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      189 2023-05-29 17:41:43.611469 gitinspired-cli-1.0.3/PKG-INFO
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      156 2023-05-29 10:01:01.000000 gitinspired-cli-1.0.3/README.md
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-29 17:41:43.607469 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      189 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      325 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        1 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       81 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        9 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/requires.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        4 2023-05-29 17:41:43.000000 gitinspired-cli-1.0.3/gitinspired_cli.egg-info/top_level.txt
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)       38 2023-05-29 17:41:43.611469 gitinspired-cli-1.0.3/setup.cfg
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      338 2023-05-29 17:41:18.000000 gitinspired-cli-1.0.3/setup.py
+drwxrwxr-x   0 jadon6    (1000) jadon6    (1000)        0 2023-05-29 17:41:43.611469 gitinspired-cli-1.0.3/src/
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)        0 2023-05-29 10:01:01.000000 gitinspired-cli-1.0.3/src/__init__.py
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)     2603 2023-05-29 17:21:54.000000 gitinspired-cli-1.0.3/src/file_manager.py
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      960 2023-05-29 10:21:40.000000 gitinspired-cli-1.0.3/src/greetings_cli.py
+-rw-rw-r--   0 jadon6    (1000) jadon6    (1000)      807 2023-05-29 17:27:06.000000 gitinspired-cli-1.0.3/src/subsys.py
```

### Comparing `gitinspired-cli-1.0.2/src/greetings_cli.py` & `gitinspired-cli-1.0.3/src/greetings_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import argparse
-from file_manager import move_to_directory, mark_files, push_files
+from src.file_manager import move_to_directory, mark_files, push_files, config
 
 
 def greet(args):
+    if(args.name) == 'config':
+        return config()
+
     message = f"Hello, {args.name}!"
     print(message)
 
     if args.directory:
         move_to_directory(args.directory)
 
     if args.mark:
         mark_files(args.mark)
 
     if args.push:
         push_files(args.push)
 
+    if args.config:
+        config()
+
 def main():
     parser = argparse.ArgumentParser(description="CLI tool for greeting.")
     parser.add_argument("name", help="Name to greet")
     parser.add_argument("-d", "--directory", help="Move to directory")
     parser.add_argument("-m", "--mark", nargs="+", help="Mark files for capture")
     parser.add_argument("-p", "--push", help="Push marked files to server")
+    parser.add_argument("-config", "--config", help="configure the repo.")
     args = parser.parse_args()
     greet(args)
 
 if __name__ == "__main__":
     main()
```

