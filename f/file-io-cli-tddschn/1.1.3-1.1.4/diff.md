# Comparing `tmp/file_io_cli_tddschn-1.1.3.tar.gz` & `tmp/file_io_cli_tddschn-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_io_cli_tddschn-1.1.3.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.1.4.tar", max compression
```

## Comparing `file_io_cli_tddschn-1.1.3.tar` & `file_io_cli_tddschn-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.3/LICENSE
--rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0     3342 2023-05-29 11:18:30.561155 file_io_cli_tddschn-1.1.3/README.md
--rw-r--r--   0        0        0      147 2023-05-29 11:18:43.143047 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0    11741 2023-05-29 11:14:47.400771 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/cli.py
--rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/config.py
--rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/utils.py
--rw-r--r--   0        0        0     1168 2023-05-29 11:18:43.141656 file_io_cli_tddschn-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     3342 2023-05-29 11:18:30.561155 file_io_cli_tddschn-1.1.4/README.md
+-rw-r--r--   0        0        0      147 2023-05-29 16:14:33.520804 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/__init__.py
+-rw-r--r--   0        0        0    11960 2023-05-29 16:12:39.264811 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/cli.py
+-rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/config.py
+-rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/utils.py
+-rw-r--r--   0        0        0     1168 2023-05-29 16:14:33.517821 file_io_cli_tddschn-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.4/PKG-INFO
```

### Comparing `file_io_cli_tddschn-1.1.3/LICENSE` & `file_io_cli_tddschn-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.3/LICENSE.txt` & `file_io_cli_tddschn-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.3/README.md` & `file_io_cli_tddschn-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/cli.py` & `file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     elif not args.name and args.tar:
         args.name = os.path.basename(args.tar) + ('.tgz' if args.gzip else '.tar')
 
     params = {}
     if args.expires:
         params['expires'] = args.expiry
 
-    url = 'http://file.io'
+    url = 'https://file.io'
     if params:
         from urllib.parse import urlencode
 
         url += '?' + urlencode(params)
 
     @cache
     def get_fp_and_file_size() -> tuple[BufferedReader | BinaryIO, int | None]:
@@ -327,15 +327,21 @@
             )
             response.raise_for_status()
             return response.json()
 
         tasks = [asyncio.to_thread(upload_file) for _ in range(args.upload_times)]
         responses = await asyncio.gather(*tasks)
         links = [r['link'] for r in responses]
-        print('\n'.join(links))
+        links_s = '\n'.join(links)
+        if args.verbose:
+            print(json.dumps(responses, indent=2, ensure_ascii=False))
+        else:
+            print(links_s)
+        if args.clip:
+            clipboard.copy(links_s)
         return
 
     fp, file_size = get_fp_and_file_size()
     if not args.quiet and args.upload_times == 1:
         progress = ProgressDisplay(file_size)
         fp = FileMonitor(fp, lambda f: progress.update(f.bytes_read))
     try:
@@ -356,15 +362,15 @@
     else:
         if not args.quiet:
             progress.update(fp.bytes_read, force=True)  # type: ignore
             progress.finish()  # type: ignore
 
     link = (res_d := response.json())['link']
     if args.verbose:
-        print(json.dumps(res_d, indent=2), file=sys.stderr)
+        print(json.dumps(res_d, indent=2, ensure_ascii=False), file=sys.stderr)
 
     if args.clip:
         print(link, '(copied to clipboard)')
         clipboard.copy(link)
     else:
         print(link)
```

### Comparing `file_io_cli_tddschn-1.1.3/pyproject.toml` & `file_io_cli_tddschn-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file.io-cli-tddschn"
-version = "1.1.3"
+version = "1.1.4"
 description = "Command-line tool to upload files to https://file.io"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 # packages = [{ include = "file_io_cli.py" }]
 packages = [{ include = "file_io_cli_tddschn" }]
 homepage = "https://github.com/tddschn/file.io-cli-tddschn"
```

### Comparing `file_io_cli_tddschn-1.1.3/PKG-INFO` & `file_io_cli_tddschn-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 1.1.3
+Version: 1.1.4
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
 Keywords: file.io,utility,uploader,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

