# Comparing `tmp/pyanalysis-2.0.8.6.tar.gz` & `tmp/pyanalysis-2.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalysis-2.0.8.6.tar", last modified: Tue Jan 10 12:35:47 2023, max compression
+gzip compressed data, was "pyanalysis-2.1.0.2.tar", last modified: Mon May 29 20:09:11 2023, max compression
```

## Comparing `pyanalysis-2.0.8.6.tar` & `pyanalysis-2.1.0.2.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-01-10 12:35:47.038504 pyanalysis-2.0.8.6/
--rwxrwxrwx   0 user      (1000) user      (1000)     4179 2023-01-10 12:35:47.033488 pyanalysis-2.0.8.6/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     3003 2023-01-10 12:22:22.000000 pyanalysis-2.0.8.6/README.md
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-01-10 12:35:46.564651 pyanalysis-2.0.8.6/pyanalysis/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-29 13:17:16.000000 pyanalysis-2.0.8.6/pyanalysis/__init__.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-01-10 12:35:46.902895 pyanalysis-2.0.8.6/pyanalysis/asyncio/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-29 13:17:26.000000 pyanalysis-2.0.8.6/pyanalysis/asyncio/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     8880 2023-01-10 12:16:14.000000 pyanalysis-2.0.8.6/pyanalysis/asyncio/client.py
--rwxrwxrwx   0 user      (1000) user      (1000)     7949 2023-01-10 12:16:14.000000 pyanalysis-2.0.8.6/pyanalysis/client.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-01-10 12:35:46.786214 pyanalysis-2.0.8.6/pyanalysis.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     4179 2023-01-10 12:35:44.000000 pyanalysis-2.0.8.6/pyanalysis.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      368 2023-01-10 12:35:46.000000 pyanalysis-2.0.8.6/pyanalysis.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-01-10 12:35:44.000000 pyanalysis-2.0.8.6/pyanalysis.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       25 2023-01-10 12:35:44.000000 pyanalysis-2.0.8.6/pyanalysis.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       11 2023-01-10 12:35:44.000000 pyanalysis-2.0.8.6/pyanalysis.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       22 2022-11-16 20:09:24.000000 pyanalysis-2.0.8.6/reqirements-dev.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       26 2022-12-01 15:10:00.000000 pyanalysis-2.0.8.6/requirements.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-01-10 12:35:47.040511 pyanalysis-2.0.8.6/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      728 2023-01-10 12:23:00.000000 pyanalysis-2.0.8.6/setup.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-01-10 12:35:46.991471 pyanalysis-2.0.8.6/tests/
--rwxrwxrwx   0 user      (1000) user      (1000)     7240 2023-01-10 12:16:14.000000 pyanalysis-2.0.8.6/tests/general-async.py
--rwxrwxrwx   0 user      (1000) user      (1000)     6473 2023-01-10 12:16:14.000000 pyanalysis-2.0.8.6/tests/general.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-05-29 20:09:11.166797 pyanalysis-2.1.0.2/
+-rwxrwxrwx   0 user      (1000) user      (1000)     3258 2023-05-29 20:09:11.164707 pyanalysis-2.1.0.2/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     3003 2023-01-10 12:22:22.000000 pyanalysis-2.1.0.2/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-05-29 20:09:11.029781 pyanalysis-2.1.0.2/pyanalysis/
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-29 13:17:16.000000 pyanalysis-2.1.0.2/pyanalysis/__init__.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-05-29 20:09:11.149610 pyanalysis-2.1.0.2/pyanalysis/asyncio/
+-rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-29 13:17:26.000000 pyanalysis-2.1.0.2/pyanalysis/asyncio/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    11521 2023-05-29 20:02:46.000000 pyanalysis-2.1.0.2/pyanalysis/asyncio/client.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    10231 2023-05-29 20:02:46.000000 pyanalysis-2.1.0.2/pyanalysis/client.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-05-29 20:09:11.114470 pyanalysis-2.1.0.2/pyanalysis.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     3258 2023-05-29 20:09:10.000000 pyanalysis-2.1.0.2/pyanalysis.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      291 2023-05-29 20:09:10.000000 pyanalysis-2.1.0.2/pyanalysis.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-05-29 20:09:10.000000 pyanalysis-2.1.0.2/pyanalysis.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       25 2023-05-29 20:09:10.000000 pyanalysis-2.1.0.2/pyanalysis.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       11 2023-05-29 20:09:10.000000 pyanalysis-2.1.0.2/pyanalysis.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-05-29 20:09:11.166797 pyanalysis-2.1.0.2/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      728 2023-05-29 11:14:21.000000 pyanalysis-2.1.0.2/setup.py
```

### Comparing `pyanalysis-2.0.8.6/PKG-INFO` & `pyanalysis-2.1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,122 @@
 Metadata-Version: 2.1
 Name: pyanalysis
-Version: 2.0.8.6
+Version: 2.1.0.2
 Summary: Python Library for pyanalysis.ptsecurity.tech
-Home-page: UNKNOWN
 Author: Stanislav Rakovsky
 Author-email: iam@disasm.me
 License: MIT
-Description: # Python Library for pyanalysis.ptsecurity.tech
-        
-        PT PyAnalysis is an analytic system for AppSec processes to inspect python projects by
-        Positive Technologies.
-        
-        ## Installation
-        
-        Install it by running
-        ```bash
-        pip3 install pyanalysis
-        ```
-        
-        ## Behind the organization's proxy
-        
-        ```python3
-        pa_checker = PaClient(
-            username="username", password="password", proxy="http://your-org-proxy.intranet:81"
-        )
-        ```
-        
-        ## Example usage
-        
-        The full examples in `\tests` folder both for `sync` and `async` code. Use them as
-        a reference.
-        
-        
-        ```python
-        from pyanalysis.client import PaClient
-        import os
-        
-        pa_checker = PaClient(
-            username=os.getenv("pa_login"), password=os.getenv("pa_password")
-        )
-        
-        verdict = pa_checker.find_package("botcity-documents", "0.3.1")
-        print(verdict)
-        ```
-        
-        ```python
-        {'status': 'Suspicious',
-         'why': ['checked by pyanalysis'],
-         'task_id': None,
-         'weights_by_versions': {'0.3.1': 250},
-         'verdicts_by_versions': {'0.3.1': ['anti_analysis::Obfuscation::Packing::Generic',
-           'crypto::base64',
-           'host_interaction::subprocess',
-           'load_code::setup_py',
-           'network::Url']},
-         'files': {'bac168fe9913bde36752ab4600e149fc19bb6903c2a4d9008b840d46e904cf96': {'versions': ['0.3.1'],
-           'verdicts': ['load_code::setup_py', 'network::Url'],
-           'weight': 30},
-        ...,
-          '4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636': {'versions': ['0.3.1'],
-           'verdicts': ['anti_analysis::Obfuscation::Packing::Generic',
-            'crypto::base64'],
-           'weight': 110},
-        ...
-        },
-         'rules_score': {'load_code::setup_py': 10,
-          'network::Url': 20,
-          'host_interaction::subprocess': 10,
-          'anti_analysis::Obfuscation::Packing::Generic': 100,
-          'crypto::base64': 10,
-          'crypto::base64 + load_code::setup_py': 100},
-         'anomalies': {}}
-        ```
-        
-        ```python
-        # Fmm, file 4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636 is packed
-        print(pa_checker.kb_file_bytes("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").decode())
-        ```
-        
-        ```python
-        import zlib, base64
-        exec(zlib.decompress(base64.b64decode('eJytV+tzozYQ/85fQa8fA...jFhc3mH0=')))
-        ```
-        
-        ```python
-        # Do we have an unpacked version?
-        for child in pa_checker.kb_file_meta("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").get("data").get("children"):
-            print("#", child)
-            print(pa_checker.kb_file_bytes(child).decode())
-        ```
-        
-        ```python
-        # bedeb6be112de621869e30b803618a27c89e212411c7ea0222dc42d482b9206f
-        G=' '
-        D=''
-        from typing import List,Optional,Union
-        I=enumerate
-        E=len
-        F=isinstance
-        A=int
-        J=IndexError
-        O=list
-        M=min
-        U=str
-        B=None
-        V=bool
-        N=False
-        W=float
-        from botcity.document_processing.parser.entry import Entry as K
-        from botcity.document_processing.parser.matcher import DataTypeMatcher as P
-        from botcity.document_processing.geometry import Point as C,Polygon as H
-        def clear(HTgBY):HTgBY._entries.clear()
-        def Q(HTgBY):
-            A=HTgBY;A._entries.sort(key=lambda e:(e.p1.y,e.p1.x))
-            for (B,C) in I(A._entries):C.index=B
-        ...
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+# Python Library for pyanalysis.ptsecurity.tech
+
+PT PyAnalysis is an analytic system for AppSec processes to inspect python projects by
+Positive Technologies.
+
+## Installation
+
+Install it by running
+```bash
+pip3 install pyanalysis
+```
+
+## Behind the organization's proxy
+
+```python3
+pa_checker = PaClient(
+    username="username", password="password", proxy="http://your-org-proxy.intranet:81"
+)
+```
+
+## Example usage
+
+The full examples in `\tests` folder both for `sync` and `async` code. Use them as
+a reference.
+
+
+```python
+from pyanalysis.client import PaClient
+import os
+
+pa_checker = PaClient(
+    username=os.getenv("pa_login"), password=os.getenv("pa_password")
+)
+
+verdict = pa_checker.find_package("botcity-documents", "0.3.1")
+print(verdict)
+```
+
+```python
+{'status': 'Suspicious',
+ 'why': ['checked by pyanalysis'],
+ 'task_id': None,
+ 'weights_by_versions': {'0.3.1': 250},
+ 'verdicts_by_versions': {'0.3.1': ['anti_analysis::Obfuscation::Packing::Generic',
+   'crypto::base64',
+   'host_interaction::subprocess',
+   'load_code::setup_py',
+   'network::Url']},
+ 'files': {'bac168fe9913bde36752ab4600e149fc19bb6903c2a4d9008b840d46e904cf96': {'versions': ['0.3.1'],
+   'verdicts': ['load_code::setup_py', 'network::Url'],
+   'weight': 30},
+...,
+  '4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636': {'versions': ['0.3.1'],
+   'verdicts': ['anti_analysis::Obfuscation::Packing::Generic',
+    'crypto::base64'],
+   'weight': 110},
+...
+},
+ 'rules_score': {'load_code::setup_py': 10,
+  'network::Url': 20,
+  'host_interaction::subprocess': 10,
+  'anti_analysis::Obfuscation::Packing::Generic': 100,
+  'crypto::base64': 10,
+  'crypto::base64 + load_code::setup_py': 100},
+ 'anomalies': {}}
+```
+
+```python
+# Fmm, file 4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636 is packed
+print(pa_checker.kb_file_bytes("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").decode())
+```
+
+```python
+import zlib, base64
+exec(zlib.decompress(base64.b64decode('eJytV+tzozYQ/85fQa8fA...jFhc3mH0=')))
+```
+
+```python
+# Do we have an unpacked version?
+for child in pa_checker.kb_file_meta("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").get("data").get("children"):
+    print("#", child)
+    print(pa_checker.kb_file_bytes(child).decode())
+```
+
+```python
+# bedeb6be112de621869e30b803618a27c89e212411c7ea0222dc42d482b9206f
+G=' '
+D=''
+from typing import List,Optional,Union
+I=enumerate
+E=len
+F=isinstance
+A=int
+J=IndexError
+O=list
+M=min
+U=str
+B=None
+V=bool
+N=False
+W=float
+from botcity.document_processing.parser.entry import Entry as K
+from botcity.document_processing.parser.matcher import DataTypeMatcher as P
+from botcity.document_processing.geometry import Point as C,Polygon as H
+def clear(HTgBY):HTgBY._entries.clear()
+def Q(HTgBY):
+    A=HTgBY;A._entries.sort(key=lambda e:(e.p1.y,e.p1.x))
+    for (B,C) in I(A._entries):C.index=B
+...
+```
```

### Comparing `pyanalysis-2.0.8.6/README.md` & `pyanalysis-2.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyanalysis-2.0.8.6/pyanalysis/client.py` & `pyanalysis-2.1.0.2/pyanalysis/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from base64 import b64decode
 
 import logzero
 import requests
 
 
 class PaClient:
-    def request(
-        self, method, path, params: dict = None, _is_token_check_request: bool = False
-    ):
+    def request(self, method, path, params=None, _is_token_check_request: bool = False):
         if not _is_token_check_request:
             self.logger.debug(f"{method} request {self._base + path}: {params}")
             self.check_token()
         else:
             self.logger.debug(
                 f"{method} request {self._base + path} for user {params['username']}"
             )
         if params is None:
             params = dict()
 
+        assert isinstance(params, dict) or isinstance(params, list)
+
         if method == "GET":
             return self._session.get(
                 self._base + path, params=params, proxies=self._proxy
             )
         elif method == "POST":
             return self._session.post(
                 self._base + path, json=params, proxies=self._proxy
@@ -65,15 +65,14 @@
         self,
         username: str = None,
         password: str = None,
         token: str = None,
         proxy: str = None,
         logger_level=logzero.WARNING,
     ):
-
         self._proxy = None
         if proxy:
             if "://" not in proxy:
                 raise Exception(
                     "Invalid proxy schema. Proper one starts with 'https://', 'http://', 'socks4://', 'socks5://', etc"
                 )
             k, v = proxy.split("://", maxsplit=1)
@@ -165,14 +164,28 @@
         #  All the tasks are finished OR no tasks are found
         FINISHED = "Finished"
         #  One of the task in tree is in crashed state
         CRASHED = "Crashed"
         """
         return status
 
+    def current_rules_version(self):
+        resp = self.request("GET", "pyanalysis/current_rules_version").json()
+        return resp
+
+    def package_badges(self, packages: list):
+        resp = self.request("POST", "pyanalysis/package_badges", packages).json()
+        return resp
+
+    def file_rescan(self, file_sha256: str):
+        resp = self.request(
+            "GET", "pyanalysis/file_rescan", {"file_sha256": file_sha256}
+        ).json()
+        return resp
+
     def kb_package(
         self,
         package_name: str,
         package_ver: str = None,
     ):
         data = {"package_name": package_name}
         if package_ver:
@@ -186,26 +199,66 @@
         return resp
 
     def kb_package_history(self, package_name: str):
         data = {"package_name": package_name}
         resp = self.request("GET", "pyanalysis/knowledge/package_history", data).json()
         return resp
 
+    def kb_package_developers_events(self, package_name: str):
+        resp = self.request(
+            "GET",
+            "pyanalysis/knowledge/package_developers_events",
+            {"package_name": package_name},
+        ).json()
+        return resp
+
+    def kb_package_developers_statuses(self, package_name: str):
+        resp = self.request(
+            "GET",
+            "pyanalysis/knowledge/package_developers_statuses",
+            {"package_name": package_name},
+        ).json()
+        return resp
+
+    def kb_developer_packages_events(self, pypi_user: str):
+        resp = self.request(
+            "GET",
+            "pyanalysis/knowledge/developer_packages_events",
+            {"package_name": pypi_user},
+        ).json()
+        return resp
+
+    def kb_developer_packages_statuses(self, pypi_user: str):
+        resp = self.request(
+            "GET",
+            "pyanalysis/knowledge/developer_packages_statuses",
+            {"package_name": pypi_user},
+        ).json()
+        return resp
+
     def kb_file_meta(self, file_sha256: str):
         # simple sanity check
         if len(file_sha256) != 64 or not all(
             i in "0123456789abcdef" for i in file_sha256
         ):
             raise Exception("Invalid hash")
 
         resp = self.request(
             "GET", "pyanalysis/knowledge/file_meta", {"file_sha256": file_sha256}
         ).json()
         return resp
 
+    def kb_package_files_meta(self, package_name: str, package_ver: str, page: int = 0):
+        resp = self.request(
+            "GET",
+            "pyanalysis/knowledge/package_files_meta",
+            {"package_name": package_name, "package_ver": package_ver, "page": page},
+        ).json()
+        return resp
+
     def kb_file_bytes(self, file_sha256: str):
         # simple sanity check
         if len(file_sha256) != 64 or not all(
             i in "0123456789abcdef" for i in file_sha256
         ):
             raise Exception("Invalid hash")
 
@@ -221,7 +274,19 @@
         ):
             raise Exception("Invalid hash")
 
         resp = self.request(
             "GET", "pyanalysis/knowledge/file_releases", {"file_sha256": file_sha256}
         ).json()
         return resp
+
+    def feed_starjacking(self, limit: int = 5):
+        resp = self.request(
+            "GET", "pyanalysis/feed/starjacking", {"limit": limit}
+        ).json()
+        return resp
+
+    def feed_typosquatting(self, limit: int = 5):
+        resp = self.request(
+            "GET", "pyanalysis/feed/typosquatting", {"limit": limit}
+        ).json()
+        return resp
```

### Comparing `pyanalysis-2.0.8.6/pyanalysis.egg-info/PKG-INFO` & `pyanalysis-2.1.0.2/pyanalysis.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,122 @@
 Metadata-Version: 2.1
 Name: pyanalysis
-Version: 2.0.8.6
+Version: 2.1.0.2
 Summary: Python Library for pyanalysis.ptsecurity.tech
-Home-page: UNKNOWN
 Author: Stanislav Rakovsky
 Author-email: iam@disasm.me
 License: MIT
-Description: # Python Library for pyanalysis.ptsecurity.tech
-        
-        PT PyAnalysis is an analytic system for AppSec processes to inspect python projects by
-        Positive Technologies.
-        
-        ## Installation
-        
-        Install it by running
-        ```bash
-        pip3 install pyanalysis
-        ```
-        
-        ## Behind the organization's proxy
-        
-        ```python3
-        pa_checker = PaClient(
-            username="username", password="password", proxy="http://your-org-proxy.intranet:81"
-        )
-        ```
-        
-        ## Example usage
-        
-        The full examples in `\tests` folder both for `sync` and `async` code. Use them as
-        a reference.
-        
-        
-        ```python
-        from pyanalysis.client import PaClient
-        import os
-        
-        pa_checker = PaClient(
-            username=os.getenv("pa_login"), password=os.getenv("pa_password")
-        )
-        
-        verdict = pa_checker.find_package("botcity-documents", "0.3.1")
-        print(verdict)
-        ```
-        
-        ```python
-        {'status': 'Suspicious',
-         'why': ['checked by pyanalysis'],
-         'task_id': None,
-         'weights_by_versions': {'0.3.1': 250},
-         'verdicts_by_versions': {'0.3.1': ['anti_analysis::Obfuscation::Packing::Generic',
-           'crypto::base64',
-           'host_interaction::subprocess',
-           'load_code::setup_py',
-           'network::Url']},
-         'files': {'bac168fe9913bde36752ab4600e149fc19bb6903c2a4d9008b840d46e904cf96': {'versions': ['0.3.1'],
-           'verdicts': ['load_code::setup_py', 'network::Url'],
-           'weight': 30},
-        ...,
-          '4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636': {'versions': ['0.3.1'],
-           'verdicts': ['anti_analysis::Obfuscation::Packing::Generic',
-            'crypto::base64'],
-           'weight': 110},
-        ...
-        },
-         'rules_score': {'load_code::setup_py': 10,
-          'network::Url': 20,
-          'host_interaction::subprocess': 10,
-          'anti_analysis::Obfuscation::Packing::Generic': 100,
-          'crypto::base64': 10,
-          'crypto::base64 + load_code::setup_py': 100},
-         'anomalies': {}}
-        ```
-        
-        ```python
-        # Fmm, file 4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636 is packed
-        print(pa_checker.kb_file_bytes("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").decode())
-        ```
-        
-        ```python
-        import zlib, base64
-        exec(zlib.decompress(base64.b64decode('eJytV+tzozYQ/85fQa8fA...jFhc3mH0=')))
-        ```
-        
-        ```python
-        # Do we have an unpacked version?
-        for child in pa_checker.kb_file_meta("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").get("data").get("children"):
-            print("#", child)
-            print(pa_checker.kb_file_bytes(child).decode())
-        ```
-        
-        ```python
-        # bedeb6be112de621869e30b803618a27c89e212411c7ea0222dc42d482b9206f
-        G=' '
-        D=''
-        from typing import List,Optional,Union
-        I=enumerate
-        E=len
-        F=isinstance
-        A=int
-        J=IndexError
-        O=list
-        M=min
-        U=str
-        B=None
-        V=bool
-        N=False
-        W=float
-        from botcity.document_processing.parser.entry import Entry as K
-        from botcity.document_processing.parser.matcher import DataTypeMatcher as P
-        from botcity.document_processing.geometry import Point as C,Polygon as H
-        def clear(HTgBY):HTgBY._entries.clear()
-        def Q(HTgBY):
-            A=HTgBY;A._entries.sort(key=lambda e:(e.p1.y,e.p1.x))
-            for (B,C) in I(A._entries):C.index=B
-        ...
-        ```
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+# Python Library for pyanalysis.ptsecurity.tech
+
+PT PyAnalysis is an analytic system for AppSec processes to inspect python projects by
+Positive Technologies.
+
+## Installation
+
+Install it by running
+```bash
+pip3 install pyanalysis
+```
+
+## Behind the organization's proxy
+
+```python3
+pa_checker = PaClient(
+    username="username", password="password", proxy="http://your-org-proxy.intranet:81"
+)
+```
+
+## Example usage
+
+The full examples in `\tests` folder both for `sync` and `async` code. Use them as
+a reference.
+
+
+```python
+from pyanalysis.client import PaClient
+import os
+
+pa_checker = PaClient(
+    username=os.getenv("pa_login"), password=os.getenv("pa_password")
+)
+
+verdict = pa_checker.find_package("botcity-documents", "0.3.1")
+print(verdict)
+```
+
+```python
+{'status': 'Suspicious',
+ 'why': ['checked by pyanalysis'],
+ 'task_id': None,
+ 'weights_by_versions': {'0.3.1': 250},
+ 'verdicts_by_versions': {'0.3.1': ['anti_analysis::Obfuscation::Packing::Generic',
+   'crypto::base64',
+   'host_interaction::subprocess',
+   'load_code::setup_py',
+   'network::Url']},
+ 'files': {'bac168fe9913bde36752ab4600e149fc19bb6903c2a4d9008b840d46e904cf96': {'versions': ['0.3.1'],
+   'verdicts': ['load_code::setup_py', 'network::Url'],
+   'weight': 30},
+...,
+  '4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636': {'versions': ['0.3.1'],
+   'verdicts': ['anti_analysis::Obfuscation::Packing::Generic',
+    'crypto::base64'],
+   'weight': 110},
+...
+},
+ 'rules_score': {'load_code::setup_py': 10,
+  'network::Url': 20,
+  'host_interaction::subprocess': 10,
+  'anti_analysis::Obfuscation::Packing::Generic': 100,
+  'crypto::base64': 10,
+  'crypto::base64 + load_code::setup_py': 100},
+ 'anomalies': {}}
+```
+
+```python
+# Fmm, file 4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636 is packed
+print(pa_checker.kb_file_bytes("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").decode())
+```
+
+```python
+import zlib, base64
+exec(zlib.decompress(base64.b64decode('eJytV+tzozYQ/85fQa8fA...jFhc3mH0=')))
+```
+
+```python
+# Do we have an unpacked version?
+for child in pa_checker.kb_file_meta("4712e06e2fa77801f18c28453a710ab64e618885aad98fb488c2b80f59613636").get("data").get("children"):
+    print("#", child)
+    print(pa_checker.kb_file_bytes(child).decode())
+```
+
+```python
+# bedeb6be112de621869e30b803618a27c89e212411c7ea0222dc42d482b9206f
+G=' '
+D=''
+from typing import List,Optional,Union
+I=enumerate
+E=len
+F=isinstance
+A=int
+J=IndexError
+O=list
+M=min
+U=str
+B=None
+V=bool
+N=False
+W=float
+from botcity.document_processing.parser.entry import Entry as K
+from botcity.document_processing.parser.matcher import DataTypeMatcher as P
+from botcity.document_processing.geometry import Point as C,Polygon as H
+def clear(HTgBY):HTgBY._entries.clear()
+def Q(HTgBY):
+    A=HTgBY;A._entries.sort(key=lambda e:(e.p1.y,e.p1.x))
+    for (B,C) in I(A._entries):C.index=B
+...
+```
```

### Comparing `pyanalysis-2.0.8.6/setup.py` & `pyanalysis-2.1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="pyanalysis",
-    version="2.0.8.6",
+    version="2.1.0.2",
     license="MIT",
     description="Python Library for pyanalysis.ptsecurity.tech",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     author="Stanislav Rakovsky",
     author_email="iam@disasm.me",
```

