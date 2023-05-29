# Comparing `tmp/torrentp-0.1.5.tar.gz` & `tmp/torrentp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrentp-0.1.5.tar", last modified: Fri Aug 12 16:26:26 2022, max compression
+gzip compressed data, was "torrentp-0.1.6.tar", last modified: Mon May 29 00:03:52 2023, max compression
```

## Comparing `torrentp-0.1.5.tar` & `torrentp-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 16:26:26.919874 torrentp-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)    12179 2022-08-12 16:26:15.000000 torrentp-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-08-12 16:26:26.919874 torrentp-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-08-12 16:26:15.000000 torrentp-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 16:26:26.919874 torrentp-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-08-12 16:26:15.000000 torrentp-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 16:26:26.919874 torrentp-0.1.5/torrentp/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-08-12 16:26:15.000000 torrentp-0.1.5/torrentp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-08-12 16:26:15.000000 torrentp-0.1.5/torrentp/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-12 16:26:15.000000 torrentp-0.1.5/torrentp/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-12 16:26:15.000000 torrentp-0.1.5/torrentp/torrent_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-08-12 16:26:15.000000 torrentp-0.1.5/torrentp/torrent_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 16:26:26.919874 torrentp-0.1.5/torrentp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-08-12 16:26:26.000000 torrentp-0.1.5/torrentp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-08-12 16:26:26.000000 torrentp-0.1.5/torrentp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 16:26:26.000000 torrentp-0.1.5/torrentp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-12 16:26:26.000000 torrentp-0.1.5/torrentp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-12 16:26:26.000000 torrentp-0.1.5/torrentp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:03:52.215801 torrentp-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-05-29 00:03:35.000000 torrentp-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-29 00:03:52.211801 torrentp-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-29 00:03:35.000000 torrentp-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:03:52.215801 torrentp-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-29 00:03:35.000000 torrentp-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:03:52.211801 torrentp-0.1.6/torrentp/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-29 00:03:35.000000 torrentp-0.1.6/torrentp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 00:03:35.000000 torrentp-0.1.6/torrentp/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-29 00:03:35.000000 torrentp-0.1.6/torrentp/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-29 00:03:35.000000 torrentp-0.1.6/torrentp/torrent_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-29 00:03:35.000000 torrentp-0.1.6/torrentp/torrent_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:03:52.211801 torrentp-0.1.6/torrentp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-29 00:03:52.000000 torrentp-0.1.6/torrentp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 00:03:52.000000 torrentp-0.1.6/torrentp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:03:52.000000 torrentp-0.1.6/torrentp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 00:03:52.000000 torrentp-0.1.6/torrentp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 00:03:52.000000 torrentp-0.1.6/torrentp.egg-info/top_level.txt
```

### Comparing `torrentp-0.1.5/LICENSE` & `torrentp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torrentp-0.1.5/PKG-INFO` & `torrentp-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -57,21 +57,39 @@
 Or download with .torrent file:
 ```python
 from torrentp import TorrentDownloader
 torrent_file = TorrentDownloader("test.torrent", '.')
 torrent_file.start_download()
 ```
 
+
+#### How can I limit the upload or download speed?
+
+Download Using 0 (default number) means unlimited speed:
+```python
+torrent_file.start_download(download_speed=0, upload_speed=0)
+```
+Or download with specifc number:
+```python
+torrent_file.start_download(download_speed=2, upload_speed=1)
+```
+
+
 ### To do list
+- [x] Limit upload and download speed
 - [ ] User can change the port
 - [ ] CLI
 - [ ] Pause / Resume
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=iw4p/torrentp&type=Date)](https://star-history.com/#iw4p/torrentp&Date)
+
 ### Issues
-Feel free to submit issues and enhancement requests.
+Feel free to submit issues and enhancement requests or contact me via [vida.page/nima](https://vida.page/nima).
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
 
  1. **Fork** the repo on GitHub
  2. **Clone** the project to your own machine
  3. **Update the Version** inside __init__.py
```

### Comparing `torrentp-0.1.5/README.md` & `torrentp-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,21 +32,39 @@
 Or download with .torrent file:
 ```python
 from torrentp import TorrentDownloader
 torrent_file = TorrentDownloader("test.torrent", '.')
 torrent_file.start_download()
 ```
 
+
+#### How can I limit the upload or download speed?
+
+Download Using 0 (default number) means unlimited speed:
+```python
+torrent_file.start_download(download_speed=0, upload_speed=0)
+```
+Or download with specifc number:
+```python
+torrent_file.start_download(download_speed=2, upload_speed=1)
+```
+
+
 ### To do list
+- [x] Limit upload and download speed
 - [ ] User can change the port
 - [ ] CLI
 - [ ] Pause / Resume
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=iw4p/torrentp&type=Date)](https://star-history.com/#iw4p/torrentp&Date)
+
 ### Issues
-Feel free to submit issues and enhancement requests.
+Feel free to submit issues and enhancement requests or contact me via [vida.page/nima](https://vida.page/nima).
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
 
  1. **Fork** the repo on GitHub
  2. **Clone** the project to your own machine
  3. **Update the Version** inside __init__.py
```

### Comparing `torrentp-0.1.5/setup.py` & `torrentp-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.1.5/torrentp/__init__.py` & `torrentp-0.1.6/torrentp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `torrentp-0.1.5/torrentp/downloader.py` & `torrentp-0.1.6/torrentp/downloader.py`

 * *Files identical despite different names*

### Comparing `torrentp-0.1.5/torrentp/torrent_downloader.py` & `torrentp-0.1.6/torrentp/torrent_downloader.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,25 +11,29 @@
         self._downloader = None
         self._torrent_info = None
         self._lt = lt
         self._file = None
         self._add_torrent_params = None
         self._session = Session(self._lt)
 
-    def start_download(self):
+    def start_download(self, download_speed=0, upload_speed=0):
         if self._file_path.startswith('magnet:'):
             self._add_torrent_params = self._lt.parse_magnet_uri(self._file_path)
             self._add_torrent_params.save_path = self._save_path
             self._downloader = Downloader(session=self._session(), torrent_info=self._add_torrent_params,
                                           save_path=self._save_path, libtorrent=lt, is_magnet=True)
+
         else:
             self._torrent_info = TorrentInfo(self._file_path, self._lt)
             self._downloader = Downloader(session=self._session(), torrent_info=self._torrent_info(),
                                           save_path=self._save_path, libtorrent=None, is_magnet=False)
 
+        self._session.set_download_limit(download_speed)
+        self._session.set_upload_limit(upload_speed)
+
         self._file = self._downloader
         self._file.download()
 
     def __str__(self):
         pass
 
     def __repr__(self):
```

### Comparing `torrentp-0.1.5/torrentp.egg-info/PKG-INFO` & `torrentp-0.1.6/torrentp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrentp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -57,21 +57,39 @@
 Or download with .torrent file:
 ```python
 from torrentp import TorrentDownloader
 torrent_file = TorrentDownloader("test.torrent", '.')
 torrent_file.start_download()
 ```
 
+
+#### How can I limit the upload or download speed?
+
+Download Using 0 (default number) means unlimited speed:
+```python
+torrent_file.start_download(download_speed=0, upload_speed=0)
+```
+Or download with specifc number:
+```python
+torrent_file.start_download(download_speed=2, upload_speed=1)
+```
+
+
 ### To do list
+- [x] Limit upload and download speed
 - [ ] User can change the port
 - [ ] CLI
 - [ ] Pause / Resume
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=iw4p/torrentp&type=Date)](https://star-history.com/#iw4p/torrentp&Date)
+
 ### Issues
-Feel free to submit issues and enhancement requests.
+Feel free to submit issues and enhancement requests or contact me via [vida.page/nima](https://vida.page/nima).
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
 
  1. **Fork** the repo on GitHub
  2. **Clone** the project to your own machine
  3. **Update the Version** inside __init__.py
```

