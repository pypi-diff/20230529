# Comparing `tmp/file_io_cli_tddschn-1.0.6.tar.gz` & `tmp/file_io_cli_tddschn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_io_cli_tddschn-1.0.6.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.1.0.tar", max compression
```

## Comparing `file_io_cli_tddschn-1.0.6.tar` & `file_io_cli_tddschn-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.0.6/LICENSE
--rw-r--r--   0        0        0     1084 2023-05-03 13:52:47.818681 file_io_cli_tddschn-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2902 2023-05-03 15:23:23.314779 file_io_cli_tddschn-1.0.6/README.md
--rw-r--r--   0        0        0      147 2023-05-03 15:24:22.021634 file_io_cli_tddschn-1.0.6/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0    10179 2023-05-03 15:18:31.333445 file_io_cli_tddschn-1.0.6/file_io_cli_tddschn/cli.py
--rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.0.6/file_io_cli_tddschn/config.py
--rw-r--r--   0        0        0     1064 2023-05-03 15:24:22.021144 file_io_cli_tddschn-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-03 13:52:47.818681 file_io_cli_tddschn-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3191 2023-05-29 10:57:54.277752 file_io_cli_tddschn-1.1.0/README.md
+-rw-r--r--   0        0        0      147 2023-05-29 10:58:24.883572 file_io_cli_tddschn-1.1.0/file_io_cli_tddschn/__init__.py
+-rw-r--r--   0        0        0    11565 2023-05-29 10:56:32.977509 file_io_cli_tddschn-1.1.0/file_io_cli_tddschn/cli.py
+-rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.0/file_io_cli_tddschn/config.py
+-rw-r--r--   0        0        0     1168 2023-05-29 10:58:24.881390 file_io_cli_tddschn-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.0/PKG-INFO
```

### Comparing `file_io_cli_tddschn-1.0.6/LICENSE` & `file_io_cli_tddschn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.0.6/LICENSE.txt` & `file_io_cli_tddschn-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.0.6/README.md` & `file_io_cli_tddschn-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 
 ```
 $ file.io-cli --help
 
 usage: file.io-cli [-h] [--version] [-e E] [-n NAME] [-q] [-c] [-t PATH] [-z]
-                   [-v]
+                   [-v] [-N UPLOAD_TIMES]
                    [file]
 
 Upload a file to file.io and print the download link. Supports stdin.
 
 positional arguments:
   file                  the file to upload
 
@@ -48,14 +48,16 @@
   -q, --quiet           hide the progress bar
   -c, --clip            copy the URL to your clipboard
   -t PATH, --tar PATH   create a TAR archive from the specified file or
                         directory
   -z, --gzip            filter the TAR archive through gzip (only with -t,
                         --tar)
   -v, --verbose         print the server response
+  -N UPLOAD_TIMES, --upload-times UPLOAD_TIMES
+                        upload the file N times
 
 ```
 
 ### Examples
 
 Upload a file and copy the link:
 
@@ -79,14 +81,24 @@
 
 ```
 $ find .. -iname \*.py | file.io -n file-list.txt
 / (312KB)
 https://file.io/uRglUT
 ```
 
+Upload a file 3 times concurrently:
+
+```
+$ file.io -N 3 file_io_cli_tddschn/cli.py
+
+https://file.io/Vv7QtVfMVBr2
+https://file.io/10Y2DgoXDJwQ
+https://file.io/rCoWI2PN58cg
+```
+
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
 
 ```
```

### Comparing `file_io_cli_tddschn-1.0.6/file_io_cli_tddschn/cli.py` & `file_io_cli_tddschn-1.1.0/file_io_cli_tddschn/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 from __future__ import division, print_function
 
+import asyncio
 import argparse
-from typing import Literal
+from io import BufferedReader
+from typing import BinaryIO, Literal
 import json
 import os
 import subprocess
 import sys
 import threading
 import time
 import uuid
@@ -248,69 +250,97 @@
         '--gzip',
         action='store_true',
         help='filter the TAR archive through gzip (only with -t, --tar)',
     )
     parser.add_argument(
         '-v', '--verbose', action='store_true', help='print the server response'
     )
+    parser.add_argument(
+        '-N', '--upload-times', type=int, help='upload the file N times', default=1
+    )
     parser.add_argument('file', nargs='?', help='the file to upload')
     args = parser.parse_args()
 
     if not args.file and not args.tar and sys.stdin.isatty():
         parser.print_usage()
         return 0
     if args.file and args.tar:
         parser.error('conflicting options: file and -t, --tar')
     return args
 
 
-def main(prog=None, argv=None):
+async def main(prog=None, argv=None):
     args = get_args(prog=prog)
     import clipboard
     import requests
 
     if args == 0:
         return
     if not args.name and args.file:
         args.name = os.path.basename(args.file)
     elif not args.name and args.tar:
         args.name = os.path.basename(args.tar) + ('.tgz' if args.gzip else '.tar')
 
-    if args.tar:
-        r, w = os.pipe()
-        flags = '-czf-' if args.gzip else '-cf-'
-        spawn_process(['tar', flags, args.tar], stdout=w, on_exit=lambda: os.close(w))
-        file_size = None
-        fp = os.fdopen(r, 'rb')
-    elif args.file:
-        file_size = os.stat(args.file).st_size
-        fp = open(args.file, 'rb')
-    else:
-        file_size = None
-        fp = sys.stdin if sys.version_info[0] == 2 else sys.stdin.buffer
-
-    if not args.quiet:
-        progress = ProgressDisplay(file_size)
-        fp = FileMonitor(fp, lambda f: progress.update(f.bytes_read))
-
-    encoder = MultipartFileEncoder('file', fp, filename=args.name or 'file')
-    stream = GeneratorFileReader(encoder.iter_encode())
-
-    headers = {'Content-Type': encoder.content_type}
     params = {}
     if args.expires:
         params['expires'] = args.expiry
 
     url = 'http://file.io'
     if params:
         from urllib.parse import urlencode
 
         url += '?' + urlencode(params)
 
+    def get_fp_and_file_size() -> tuple[BufferedReader | BinaryIO, int | None]:
+        assert not isinstance(args, int)
+        if args.tar:
+            r, w = os.pipe()
+            flags = '-czf-' if args.gzip else '-cf-'
+            spawn_process(
+                ['tar', flags, args.tar], stdout=w, on_exit=lambda: os.close(w)
+            )
+            file_size = None
+            fp = os.fdopen(r, 'rb')
+        elif args.file:
+            file_size = os.stat(args.file).st_size
+            fp = open(args.file, 'rb')
+        else:
+            file_size = None
+            fp = sys.stdin if sys.version_info[0] == 2 else sys.stdin.buffer
+        return fp, file_size
+
+    if args.upload_times > 1:
+        # use asyncio.to_thread
+
+        def upload_file() -> dict[str, str]:
+            assert not isinstance(args, int)
+            fp, _ = get_fp_and_file_size()
+            encoder = MultipartFileEncoder('file', fp, filename=args.name or 'file')
+            stream = GeneratorFileReader(encoder.iter_encode())
+            headers = {'Content-Type': encoder.content_type}
+            response = requests.post(
+                url, params=params, data=stream_file(stream), headers=headers
+            )
+            response.raise_for_status()
+            return response.json()
+
+        tasks = [asyncio.to_thread(upload_file) for _ in range(args.upload_times)]
+        responses = await asyncio.gather(*tasks)
+        links = [r['link'] for r in responses]
+        print('\n'.join(links))
+        return
+
+    fp, file_size = get_fp_and_file_size()
+    if not args.quiet and args.upload_times == 1:
+        progress = ProgressDisplay(file_size)
+        fp = FileMonitor(fp, lambda f: progress.update(f.bytes_read))
     try:
+        encoder = MultipartFileEncoder('file', fp, filename=args.name or 'file')
+        stream = GeneratorFileReader(encoder.iter_encode())
+        headers = {'Content-Type': encoder.content_type}
         response = requests.post(
             url, params=params, data=stream_file(stream), headers=headers
         )
         response.raise_for_status()
     except BaseException as exc:
         if not args.quiet:
             progress.finish()  # type: ignore
@@ -330,11 +360,16 @@
     if args.clip:
         print(link, '(copied to clipboard)')
         clipboard.copy(link)
     else:
         print(link)
 
 
-_entry_point = lambda: sys.exit(main())
+# _entry_point = lambda: sys.exit(main())
+def main_sync():
+    asyncio.run(main())
+
 
 if __name__ == '__main__':
-    _entry_point()
+    # _entry_point()
+
+    main_sync()
```

### Comparing `file_io_cli_tddschn-1.0.6/pyproject.toml` & `file_io_cli_tddschn-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file.io-cli-tddschn"
-version = "1.0.6"
+version = "1.1.0"
 description = "Command-line tool to upload files to https://file.io"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 # packages = [{ include = "file_io_cli.py" }]
 packages = [{ include = "file_io_cli_tddschn" }]
 homepage = "https://github.com/tddschn/file.io-cli-tddschn"
@@ -12,16 +12,18 @@
 classifiers = ["Topic :: Utilities"]
 keywords = ["file.io", "utility", "uploader", "CLI"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/file.io-cli-tddschn/issues"
 
 [tool.poetry.scripts]
-"file.io-cli" = "file_io_cli_tddschn.cli:_entry_point"
-"file.io" = "file_io_cli_tddschn.cli:_entry_point"
+# "file.io-cli" = "file_io_cli_tddschn.cli:_entry_point"
+# "file.io" = "file_io_cli_tddschn.cli:_entry_point"
+"file.io-cli" = "file_io_cli_tddschn.cli:main_sync"
+"file.io" = "file_io_cli_tddschn.cli:main_sync"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 clipboard = ">=0.0.4,<1.0.0"
 requests = ">=2.25.1,<3.0.0"
```

### Comparing `file_io_cli_tddschn-1.0.6/PKG-INFO` & `file_io_cli_tddschn-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 1.0.6
+Version: 1.1.0
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
 Keywords: file.io,utility,uploader,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -48,15 +48,15 @@
 
 
 
 ```
 $ file.io-cli --help
 
 usage: file.io-cli [-h] [--version] [-e E] [-n NAME] [-q] [-c] [-t PATH] [-z]
-                   [-v]
+                   [-v] [-N UPLOAD_TIMES]
                    [file]
 
 Upload a file to file.io and print the download link. Supports stdin.
 
 positional arguments:
   file                  the file to upload
 
@@ -68,14 +68,16 @@
   -q, --quiet           hide the progress bar
   -c, --clip            copy the URL to your clipboard
   -t PATH, --tar PATH   create a TAR archive from the specified file or
                         directory
   -z, --gzip            filter the TAR archive through gzip (only with -t,
                         --tar)
   -v, --verbose         print the server response
+  -N UPLOAD_TIMES, --upload-times UPLOAD_TIMES
+                        upload the file N times
 
 ```
 
 ### Examples
 
 Upload a file and copy the link:
 
@@ -99,14 +101,24 @@
 
 ```
 $ find .. -iname \*.py | file.io -n file-list.txt
 / (312KB)
 https://file.io/uRglUT
 ```
 
+Upload a file 3 times concurrently:
+
+```
+$ file.io -N 3 file_io_cli_tddschn/cli.py
+
+https://file.io/Vv7QtVfMVBr2
+https://file.io/10Y2DgoXDJwQ
+https://file.io/rCoWI2PN58cg
+```
+
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
 
 ```
```

