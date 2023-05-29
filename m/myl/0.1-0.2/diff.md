# Comparing `tmp/myl-0.1.tar.gz` & `tmp/myl-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.1.tar", last modified: Sun May 28 14:45:39 2023, max compression
+gzip compressed data, was "myl-0.2.tar", last modified: Sun May 28 16:01:35 2023, max compression
```

## Comparing `myl-0.1.tar` & `myl-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:39.406999 myl-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:39.402999 myl-0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-28 14:45:27.000000 myl-0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:39.406999 myl-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-28 14:45:27.000000 myl-0.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-28 14:45:27.000000 myl-0.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 14:45:27.000000 myl-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 14:45:27.000000 myl-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-28 14:45:39.406999 myl-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 14:45:27.000000 myl-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:45:39.406999 myl-0.1/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 14:45:39.000000 myl-0.1/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-28 14:45:27.000000 myl-0.1/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-28 14:45:27.000000 myl-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:45:39.406999 myl-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:01:35.481800 myl-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:01:35.481800 myl-0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-28 16:01:24.000000 myl-0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:01:35.481800 myl-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-28 16:01:24.000000 myl-0.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-28 16:01:24.000000 myl-0.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 16:01:24.000000 myl-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 16:01:24.000000 myl-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-28 16:01:35.481800 myl-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-28 16:01:24.000000 myl-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:01:35.481800 myl-0.2/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 16:01:35.000000 myl-0.2/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-28 16:01:24.000000 myl-0.2/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-28 16:01:24.000000 myl-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 16:01:35.481800 myl-0.2/setup.cfg
```

### Comparing `myl-0.1/.github/workflows/release.yaml` & `myl-0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.1/LICENSE` & `myl-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.1/PKG-INFO` & `myl-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.1
+Version: 0.2
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.1/myl.egg-info/PKG-INFO` & `myl-0.2/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.1
+Version: 0.2
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.1/myl.py` & `myl-0.2/myl.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,24 @@
     )
     parser.add_argument(
         "-p", "--password", help="IMAP password", required=True
     )
     parser.add_argument(
         "-t", "--no-title", help="Do not show title", action="store_true"
     )
+    parser.add_argument("-f", "--folder", help="IMAP folder", default="INBOX")
     parser.add_argument("-w", "--wrap", help="Wrap text", action="store_true")
+    parser.add_argument("-H", "--html", help="Show HTML", action="store_true")
+    parser.add_argument("MAILID", help="Mail ID to fetch", nargs="?")
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
+
     table = Table(
         expand=True,
         show_header=not args.no_title,
         header_style="bold",
         show_lines=False,
         box=None,
     )
@@ -42,16 +46,21 @@
         "Subject", style="green", no_wrap=not args.wrap, max_width=30
     )
     table.add_column("From", style="blue", no_wrap=not args.wrap, max_width=30)
     table.add_column("Date", style="cyan", no_wrap=not args.wrap)
 
     try:
         with imap_tools.MailBoxTls(args.server, port=args.port).login(
-            args.username, args.password
+            args.username, args.password, args.folder
         ) as mailbox:
+            if args.MAILID:
+                msg = [x for x in mailbox.fetch(f"UID {args.MAILID}")][0]
+                print(msg.text if not args.html else msg.html)
+                return 0
+
             for msg in mailbox.fetch():
                 table.add_row(
                     msg.uid,
                     msg.subject,
                     msg.from_,
                     msg.date.strftime("%d/%m/%Y %H:%M"),
                 )
```

### Comparing `myl-0.1/pyproject.toml` & `myl-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap_tools",
   "rich"
 ]
-version = "0.1"
+version = "0.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

