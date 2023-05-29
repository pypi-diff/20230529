# Comparing `tmp/myl-0.5.tar.gz` & `tmp/myl-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.5.tar", last modified: Mon May 29 10:26:13 2023, max compression
+gzip compressed data, was "myl-0.6.tar", last modified: Mon May 29 10:35:51 2023, max compression
```

## Comparing `myl-0.5.tar` & `myl-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:26:13.425112 myl-0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:26:13.421112 myl-0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 10:26:00.000000 myl-0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:26:13.421112 myl-0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 10:26:00.000000 myl-0.5/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 10:26:00.000000 myl-0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 10:26:00.000000 myl-0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 10:26:00.000000 myl-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:26:13.425112 myl-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 10:26:00.000000 myl-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:26:13.421112 myl-0.5/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 10:26:13.000000 myl-0.5/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-29 10:26:00.000000 myl-0.5/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 10:26:00.000000 myl-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:26:13.425112 myl-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.999130 myl-0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 10:35:36.000000 myl-0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 10:35:36.000000 myl-0.6/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 10:35:36.000000 myl-0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 10:35:36.000000 myl-0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 10:35:36.000000 myl-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:35:50.999130 myl-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 10:35:36.000000 myl-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-29 10:35:36.000000 myl-0.6/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 10:35:36.000000 myl-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:35:50.999130 myl-0.6/setup.cfg
```

### Comparing `myl-0.5/.github/workflows/release.yaml` & `myl-0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.5/LICENSE` & `myl-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.5/PKG-INFO` & `myl-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.5
+Version: 0.6
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.5/myl.egg-info/PKG-INFO` & `myl-0.6/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.5
+Version: 0.6
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.5/myl.py` & `myl-0.6/myl.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     parser.add_argument(
         "-p", "--password", help="IMAP password", required=True
     )
     parser.add_argument(
         "-t", "--no-title", help="Do not show title", action="store_true"
     )
     parser.add_argument("-f", "--folder", help="IMAP folder", default="INBOX")
+    parser.add_argument("-S", "--search", help="Search string", default="ALL")
     parser.add_argument("-w", "--wrap", help="Wrap text", action="store_true")
     parser.add_argument("-H", "--html", help="Show HTML", action="store_true")
     parser.add_argument("MAILID", help="Mail ID to fetch", nargs="?")
     return parser.parse_args()
 
 
 def main():
@@ -62,24 +63,24 @@
     try:
         mb = imap_tools.MailBoxTls if args.starttls else imap_tools.MailBox
 
         with mb(args.server, port=args.port).login(
             args.username, args.password, args.folder
         ) as mailbox:
             if args.MAILID:
-                msg = [
-                    x
-                    for x in mailbox.fetch(
+                msg = next(
+                    mailbox.fetch(
                         f"UID {args.MAILID}", mark_seen=args.mark_seen
                     )
-                ][0]
+                )
                 print(msg.text if not args.html else msg.html)
                 return 0
 
             for msg in mailbox.fetch(
+                criteria=args.search,
                 reverse=True,
                 bulk=True,
                 limit=args.count,
                 mark_seen=args.mark_seen,
                 headers_only=True,
             ):
                 table.add_row(
```

### Comparing `myl-0.5/pyproject.toml` & `myl-0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap_tools",
   "rich"
 ]
-version = "0.5"
+version = "0.6"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

