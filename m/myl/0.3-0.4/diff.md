# Comparing `tmp/myl-0.3.tar.gz` & `tmp/myl-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.3.tar", last modified: Mon May 29 09:47:20 2023, max compression
+gzip compressed data, was "myl-0.4.tar", last modified: Mon May 29 10:18:06 2023, max compression
```

## Comparing `myl-0.3.tar` & `myl-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:47:20.312457 myl-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:47:20.312457 myl-0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 09:47:08.000000 myl-0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:47:20.312457 myl-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 09:47:08.000000 myl-0.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 09:47:08.000000 myl-0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 09:47:08.000000 myl-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 09:47:08.000000 myl-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 09:47:20.312457 myl-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 09:47:08.000000 myl-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:47:20.312457 myl-0.3/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 09:47:20.000000 myl-0.3/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-29 09:47:08.000000 myl-0.3/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 09:47:08.000000 myl-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:47:20.312457 myl-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:18:06.880405 myl-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:18:06.880405 myl-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 10:17:52.000000 myl-0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:18:06.880405 myl-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 10:17:52.000000 myl-0.4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 10:17:52.000000 myl-0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 10:17:52.000000 myl-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 10:17:52.000000 myl-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:18:06.880405 myl-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 10:17:52.000000 myl-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:18:06.880405 myl-0.4/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 10:18:06.000000 myl-0.4/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-29 10:17:52.000000 myl-0.4/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 10:17:52.000000 myl-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:18:06.880405 myl-0.4/setup.cfg
```

### Comparing `myl-0.3/.github/workflows/release.yaml` & `myl-0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.3/LICENSE` & `myl-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.3/PKG-INFO` & `myl-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.3
+Version: 0.4
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.3/myl.egg-info/PKG-INFO` & `myl-0.4/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.3
+Version: 0.4
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.3/myl.py` & `myl-0.4/myl.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,20 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-s", "--server", help="IMAP server address", required=True
     )
     parser.add_argument("-P", "--port", help="IMAP server port", default=143)
     parser.add_argument("--starttls", help="Start TLS", action="store_true")
     parser.add_argument(
+        "-c", "--count", help="Number of messages to fetch", default=10, type=int
+    )
+    parser.add_argument(
+        "-m", "--mark-seen", help="Mark seen", action="store_true"
+    )
+    parser.add_argument(
         "-u", "--username", help="IMAP username", required=True
     )
     parser.add_argument(
         "-p", "--password", help="IMAP password", required=True
     )
     parser.add_argument(
         "-t", "--no-title", help="Do not show title", action="store_true"
@@ -52,25 +58,37 @@
     try:
         mb = imap_tools.MailBoxTls if args.starttls else imap_tools.MailBox
 
         with mb(args.server, port=args.port).login(
             args.username, args.password, args.folder
         ) as mailbox:
             if args.MAILID:
-                msg = [x for x in mailbox.fetch(f"UID {args.MAILID}")][0]
+                msg = [
+                    x
+                    for x in mailbox.fetch(
+                        f"UID {args.MAILID}", mark_seen=args.mark_seen
+                    )
+                ][0]
                 print(msg.text if not args.html else msg.html)
                 return 0
 
-            for msg in mailbox.fetch():
+            for msg in mailbox.fetch(
+                reverse=True,
+                bulk=True,
+                limit=args.count,
+                mark_seen=args.mark_seen,
+            ):
                 table.add_row(
-                    msg.uid,
-                    msg.subject,
+                    msg.uid if msg.uid else "???",
+                    msg.subject if msg.subject else "<no-subject>",
                     msg.from_,
-                    msg.date.strftime("%d/%m/%Y %H:%M"),
+                    msg.date.strftime("%H:%M %d/%m/%Y") if msg.date else "???",
                 )
+                if len(table.rows) >= args.count:
+                    break
 
         console = Console()
         console.print(table)
         return 0
     except Exception as e:
         LOGGER.error(e)
         return 1
```

### Comparing `myl-0.3/pyproject.toml` & `myl-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap_tools",
   "rich"
 ]
-version = "0.3"
+version = "0.4"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

