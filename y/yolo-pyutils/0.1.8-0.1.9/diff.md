# Comparing `tmp/yolo-pyutils-0.1.8.tar.gz` & `tmp/yolo-pyutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yolo-pyutils-0.1.8.tar", last modified: Fri Aug 26 06:58:41 2022, max compression
+gzip compressed data, was "dist/yolo-pyutils-0.1.9.tar", last modified: Fri Aug 26 07:34:26 2022, max compression
```

## Comparing `yolo-pyutils-0.1.8.tar` & `yolo-pyutils-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/
--rw-r--r--   0 boyuan     (501) staff       (20)    11357 2022-04-06 23:42:21.000000 yolo-pyutils-0.1.8/LICENSE
--rw-r--r--   0 boyuan     (501) staff       (20)      777 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/PKG-INFO
--rw-r--r--   0 boyuan     (501) staff       (20)      206 2022-08-16 06:33:13.000000 yolo-pyutils-0.1.8/README.md
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/
--rw-r--r--   0 boyuan     (501) staff       (20)       67 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.8/pyutils/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)      379 2022-08-16 06:41:52.000000 yolo-pyutils-0.1.8/pyutils/gen_test_report.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/hadoop/
--rw-r--r--   0 boyuan     (501) staff       (20)       32 2022-08-16 02:36:39.000000 yolo-pyutils-0.1.8/pyutils/hadoop/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)      996 2022-08-16 02:35:42.000000 yolo-pyutils-0.1.8/pyutils/hadoop/conf.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/io/
--rw-r--r--   0 boyuan     (501) staff       (20)       62 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.8/pyutils/io/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)      952 2022-08-16 02:33:21.000000 yolo-pyutils-0.1.8/pyutils/io/file.py
--rw-r--r--   0 boyuan     (501) staff       (20)     1246 2022-08-26 06:56:40.000000 yolo-pyutils-0.1.8/pyutils/io/mail_reader.py
--rw-r--r--   0 boyuan     (501) staff       (20)      815 2022-04-07 09:08:10.000000 yolo-pyutils-0.1.8/pyutils/io/pandas.py
--rw-r--r--   0 boyuan     (501) staff       (20)      761 2022-04-07 00:52:33.000000 yolo-pyutils-0.1.8/pyutils/io/process_bar.py
--rw-r--r--   0 boyuan     (501) staff       (20)     5240 2022-08-16 01:13:22.000000 yolo-pyutils-0.1.8/pyutils/io/rest.py
--rw-r--r--   0 boyuan     (501) staff       (20)     2593 2022-08-16 01:07:16.000000 yolo-pyutils-0.1.8/pyutils/io/table.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/processing/
--rw-r--r--   0 boyuan     (501) staff       (20)       53 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.8/pyutils/processing/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)     1011 2022-04-07 00:54:47.000000 yolo-pyutils-0.1.8/pyutils/processing/qps_calculator.py
--rw-r--r--   0 boyuan     (501) staff       (20)      473 2022-04-07 00:51:48.000000 yolo-pyutils-0.1.8/pyutils/processing/timer.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/scheduling/
--rw-r--r--   0 boyuan     (501) staff       (20)       54 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.8/pyutils/scheduling/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)     3624 2022-08-24 04:02:34.000000 yolo-pyutils-0.1.8/pyutils/scheduling/event_driven.py
--rw-r--r--   0 boyuan     (501) staff       (20)     2303 2022-08-16 03:23:56.000000 yolo-pyutils-0.1.8/pyutils/scheduling/event_driven_test.py
--rw-r--r--   0 boyuan     (501) staff       (20)     1189 2022-04-07 09:42:09.000000 yolo-pyutils-0.1.8/pyutils/scheduling/scheduler.py
--rw-r--r--   0 boyuan     (501) staff       (20)     1097 2022-08-16 06:43:35.000000 yolo-pyutils-0.1.8/pyutils/scheduling/scheduler_test.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/pyutils/structures/
--rw-r--r--   0 boyuan     (501) staff       (20)       91 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.8/pyutils/structures/__init__.py
--rw-r--r--   0 boyuan     (501) staff       (20)      275 2022-04-07 09:00:37.000000 yolo-pyutils-0.1.8/pyutils/structures/convert.py
--rw-r--r--   0 boyuan     (501) staff       (20)     3337 2022-04-07 00:47:55.000000 yolo-pyutils-0.1.8/pyutils/structures/dict.py
--rw-r--r--   0 boyuan     (501) staff       (20)      386 2022-08-16 01:29:32.000000 yolo-pyutils-0.1.8/pyutils/structures/iterable.py
--rw-r--r--   0 boyuan     (501) staff       (20)     1281 2022-08-16 03:21:03.000000 yolo-pyutils-0.1.8/pyutils/structures/iterable_test.py
--rw-r--r--   0 boyuan     (501) staff       (20)      720 2022-04-07 00:20:51.000000 yolo-pyutils-0.1.8/pyutils/structures/list.py
--rw-r--r--   0 boyuan     (501) staff       (20)      590 2022-08-22 10:12:27.000000 yolo-pyutils-0.1.8/pyutils/structures/reflect.py
--rw-r--r--   0 boyuan     (501) staff       (20)      986 2022-04-07 00:45:02.000000 yolo-pyutils-0.1.8/pyutils/structures/string.py
--rw-r--r--   0 boyuan     (501) staff       (20)      883 2022-04-07 00:54:10.000000 yolo-pyutils-0.1.8/pyutils/structures/time.py
--rw-r--r--   0 boyuan     (501) staff       (20)      440 2022-04-18 09:36:07.000000 yolo-pyutils-0.1.8/pyutils/structures/tuple.py
--rw-r--r--   0 boyuan     (501) staff       (20)       38 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/setup.cfg
--rw-r--r--   0 boyuan     (501) staff       (20)      835 2022-08-26 06:58:39.000000 yolo-pyutils-0.1.8/setup.py
-drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/yolo_pyutils.egg-info/
--rw-r--r--   0 boyuan     (501) staff       (20)      777 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/yolo_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 boyuan     (501) staff       (20)      988 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/yolo_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 boyuan     (501) staff       (20)        1 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/yolo_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 boyuan     (501) staff       (20)        8 2022-08-26 06:58:41.000000 yolo-pyutils-0.1.8/yolo_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/
+-rw-r--r--   0 boyuan     (501) staff       (20)    11357 2022-04-06 23:42:21.000000 yolo-pyutils-0.1.9/LICENSE
+-rw-r--r--   0 boyuan     (501) staff       (20)      777 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/PKG-INFO
+-rw-r--r--   0 boyuan     (501) staff       (20)      206 2022-08-16 06:33:13.000000 yolo-pyutils-0.1.9/README.md
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/
+-rw-r--r--   0 boyuan     (501) staff       (20)       67 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.9/pyutils/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      379 2022-08-16 06:41:52.000000 yolo-pyutils-0.1.9/pyutils/gen_test_report.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/hadoop/
+-rw-r--r--   0 boyuan     (501) staff       (20)       32 2022-08-16 02:36:39.000000 yolo-pyutils-0.1.9/pyutils/hadoop/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      996 2022-08-16 02:35:42.000000 yolo-pyutils-0.1.9/pyutils/hadoop/conf.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/io/
+-rw-r--r--   0 boyuan     (501) staff       (20)       62 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.9/pyutils/io/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      952 2022-08-16 02:33:21.000000 yolo-pyutils-0.1.9/pyutils/io/file.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1319 2022-08-26 07:32:57.000000 yolo-pyutils-0.1.9/pyutils/io/mail_reader.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1054 2022-08-26 07:32:07.000000 yolo-pyutils-0.1.9/pyutils/io/mail_sender.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      815 2022-04-07 09:08:10.000000 yolo-pyutils-0.1.9/pyutils/io/pandas.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      761 2022-04-07 00:52:33.000000 yolo-pyutils-0.1.9/pyutils/io/process_bar.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     5240 2022-08-16 01:13:22.000000 yolo-pyutils-0.1.9/pyutils/io/rest.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     2593 2022-08-16 01:07:16.000000 yolo-pyutils-0.1.9/pyutils/io/table.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/processing/
+-rw-r--r--   0 boyuan     (501) staff       (20)       53 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.9/pyutils/processing/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1011 2022-04-07 00:54:47.000000 yolo-pyutils-0.1.9/pyutils/processing/qps_calculator.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      473 2022-04-07 00:51:48.000000 yolo-pyutils-0.1.9/pyutils/processing/timer.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/scheduling/
+-rw-r--r--   0 boyuan     (501) staff       (20)       54 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.9/pyutils/scheduling/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     3624 2022-08-24 04:02:34.000000 yolo-pyutils-0.1.9/pyutils/scheduling/event_driven.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     2303 2022-08-16 03:23:56.000000 yolo-pyutils-0.1.9/pyutils/scheduling/event_driven_test.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1189 2022-04-07 09:42:09.000000 yolo-pyutils-0.1.9/pyutils/scheduling/scheduler.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1097 2022-08-16 06:43:35.000000 yolo-pyutils-0.1.9/pyutils/scheduling/scheduler_test.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/pyutils/structures/
+-rw-r--r--   0 boyuan     (501) staff       (20)       91 2022-08-22 10:12:18.000000 yolo-pyutils-0.1.9/pyutils/structures/__init__.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      275 2022-04-07 09:00:37.000000 yolo-pyutils-0.1.9/pyutils/structures/convert.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     3337 2022-04-07 00:47:55.000000 yolo-pyutils-0.1.9/pyutils/structures/dict.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      386 2022-08-16 01:29:32.000000 yolo-pyutils-0.1.9/pyutils/structures/iterable.py
+-rw-r--r--   0 boyuan     (501) staff       (20)     1281 2022-08-16 03:21:03.000000 yolo-pyutils-0.1.9/pyutils/structures/iterable_test.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      720 2022-04-07 00:20:51.000000 yolo-pyutils-0.1.9/pyutils/structures/list.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      590 2022-08-22 10:12:27.000000 yolo-pyutils-0.1.9/pyutils/structures/reflect.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      986 2022-04-07 00:45:02.000000 yolo-pyutils-0.1.9/pyutils/structures/string.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      883 2022-04-07 00:54:10.000000 yolo-pyutils-0.1.9/pyutils/structures/time.py
+-rw-r--r--   0 boyuan     (501) staff       (20)      440 2022-04-18 09:36:07.000000 yolo-pyutils-0.1.9/pyutils/structures/tuple.py
+-rw-r--r--   0 boyuan     (501) staff       (20)       38 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/setup.cfg
+-rw-r--r--   0 boyuan     (501) staff       (20)      835 2022-08-26 07:33:10.000000 yolo-pyutils-0.1.9/setup.py
+drwxr-xr-x   0 boyuan     (501) staff       (20)        0 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/yolo_pyutils.egg-info/
+-rw-r--r--   0 boyuan     (501) staff       (20)      777 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/yolo_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 boyuan     (501) staff       (20)     1014 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/yolo_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 boyuan     (501) staff       (20)        1 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/yolo_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 boyuan     (501) staff       (20)        8 2022-08-26 07:34:26.000000 yolo-pyutils-0.1.9/yolo_pyutils.egg-info/top_level.txt
```

### Comparing `yolo-pyutils-0.1.8/LICENSE` & `yolo-pyutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/PKG-INFO` & `yolo-pyutils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo-pyutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: yolo-pyutils provides utility functions for IO, data-processing, scheduling, common structures etc.
 Home-page: https://github.com/TaoYang526/yolo-pyutils
 Author: Tao Yang
 Author-email: ytaofighting@gmail.com
 License: Apache License 2.0
 Keywords: utils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yolo-pyutils-0.1.8/pyutils/hadoop/conf.py` & `yolo-pyutils-0.1.9/pyutils/hadoop/conf.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/io/file.py` & `yolo-pyutils-0.1.9/pyutils/io/file.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/io/mail_reader.py` & `yolo-pyutils-0.1.9/pyutils/io/mail_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-import logging
 from imapclient import IMAPClient
 
 
 class MailReader:
 
     def __init__(self, imap_host, imap_port, user, pwd, charset='UTF-8', ssl=True):
         self.__imap_host = imap_host
         self.__imap_port = imap_port
         self.__user = user
         self.__pwd = pwd
-        self.__client = None
         self.__charset = charset
         self.__ssl = ssl
+        self.__client = None
 
     def start(self):
         self.__client = IMAPClient(self.__imap_host, ssl=self.__ssl, port=self.__imap_port)
         self.__client.login(self.__user, self.__pwd)
 
     def stop(self):
         self.__client.logout()
 
-    def search_inbox(self, criteria, search_key_alias):
-        self.__client.select_folder('INBOX')
-        messages = self.__client.search(criteria=criteria, charset=self.__charset)
-        logging.info("%d messages found by criteria={}".format(len(messages), criteria))
+    # return mails and error if exception occurred
+    def get_mails(self, folder, criteria, search_key_alias):
         mails = list()
-        if len(messages) > 0:
-            for mail_id, data in self.__client.fetch(messages, search_key_alias.keys()).items():
-                mail = dict()
-                for key, alias in search_key_alias.items():
-                    mail[alias] = data[bytes(key, self.__charset)].decode(self.__charset)
-                mails.append(mail)
-        return mails
+        err = None
+        try:
+            self.__client.select_folder(folder)
+            messages = self.__client.search(criteria=criteria, charset=self.__charset)
+            if len(messages) > 0:
+                for mail_id, data in self.__client.fetch(messages, search_key_alias.keys()).items():
+                    mail = dict()
+                    for key, alias in search_key_alias.items():
+                        mail[alias] = data[bytes(key, self.__charset)].decode(self.__charset)
+                    mails.append(mail)
+        except Exception as ex:
+            err = ex
+        return mails, err
```

### Comparing `yolo-pyutils-0.1.8/pyutils/io/pandas.py` & `yolo-pyutils-0.1.9/pyutils/io/pandas.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/io/process_bar.py` & `yolo-pyutils-0.1.9/pyutils/io/process_bar.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/io/rest.py` & `yolo-pyutils-0.1.9/pyutils/io/rest.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/io/table.py` & `yolo-pyutils-0.1.9/pyutils/io/table.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/processing/qps_calculator.py` & `yolo-pyutils-0.1.9/pyutils/processing/qps_calculator.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/scheduling/event_driven.py` & `yolo-pyutils-0.1.9/pyutils/scheduling/event_driven.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/scheduling/event_driven_test.py` & `yolo-pyutils-0.1.9/pyutils/scheduling/event_driven_test.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/scheduling/scheduler.py` & `yolo-pyutils-0.1.9/pyutils/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/scheduling/scheduler_test.py` & `yolo-pyutils-0.1.9/pyutils/scheduling/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/dict.py` & `yolo-pyutils-0.1.9/pyutils/structures/dict.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/iterable_test.py` & `yolo-pyutils-0.1.9/pyutils/structures/iterable_test.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/list.py` & `yolo-pyutils-0.1.9/pyutils/structures/list.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/reflect.py` & `yolo-pyutils-0.1.9/pyutils/structures/reflect.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/string.py` & `yolo-pyutils-0.1.9/pyutils/structures/string.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/pyutils/structures/time.py` & `yolo-pyutils-0.1.9/pyutils/structures/time.py`

 * *Files identical despite different names*

### Comparing `yolo-pyutils-0.1.8/setup.py` & `yolo-pyutils-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name="yolo-pyutils",
-    version="0.1.8",
+    version="0.1.9",
     author="Tao Yang",
     author_email="ytaofighting@gmail.com",
     description="yolo-pyutils provides utility functions for IO, data-processing, scheduling, common structures etc.",
     license="Apache License 2.0",
     keywords="utils",
     url="https://github.com/TaoYang526/yolo-pyutils",
     packages=find_packages(),
```

### Comparing `yolo-pyutils-0.1.8/yolo_pyutils.egg-info/PKG-INFO` & `yolo-pyutils-0.1.9/yolo_pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolo-pyutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: yolo-pyutils provides utility functions for IO, data-processing, scheduling, common structures etc.
 Home-page: https://github.com/TaoYang526/yolo-pyutils
 Author: Tao Yang
 Author-email: ytaofighting@gmail.com
 License: Apache License 2.0
 Keywords: utils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yolo-pyutils-0.1.8/yolo_pyutils.egg-info/SOURCES.txt` & `yolo-pyutils-0.1.9/yolo_pyutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyutils/__init__.py
 pyutils/gen_test_report.py
 pyutils/hadoop/__init__.py
 pyutils/hadoop/conf.py
 pyutils/io/__init__.py
 pyutils/io/file.py
 pyutils/io/mail_reader.py
+pyutils/io/mail_sender.py
 pyutils/io/pandas.py
 pyutils/io/process_bar.py
 pyutils/io/rest.py
 pyutils/io/table.py
 pyutils/processing/__init__.py
 pyutils/processing/qps_calculator.py
 pyutils/processing/timer.py
```

