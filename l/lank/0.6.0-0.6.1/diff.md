# Comparing `tmp/lank-0.6.0.tar.gz` & `tmp/lank-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lank-0.6.0.tar", last modified: Mon Mar 20 16:29:49 2023, max compression
+gzip compressed data, was "lank-0.6.1.tar", last modified: Sun May 28 23:42:08 2023, max compression
```

## Comparing `lank-0.6.0.tar` & `lank-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.899573 lank-0.6.0/
--rw-r--r--   0 shawn     (1000) shawn     (1000)       82 2023-03-18 00:58:16.000000 lank-0.6.0/.gitignore
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2296 2023-03-20 16:24:48.000000 lank-0.6.0/CHANGELOG
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1102 2022-07-10 22:31:07.000000 lank-0.6.0/LICENSE
--rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-03-20 16:29:49.899573 lank-0.6.0/PKG-INFO
--rw-r--r--   0 shawn     (1000) shawn     (1000)      352 2022-07-10 22:32:02.000000 lank-0.6.0/README.md
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.893573 lank-0.6.0/lank/
--rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2022-06-14 19:59:08.000000 lank-0.6.0/lank/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:26.000000 lank-0.6.0/lank/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)       23 2023-03-20 02:50:40.000000 lank-0.6.0/lank/__version__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1397 2023-03-20 09:45:57.000000 lank-0.6.0/lank/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      295 2022-07-01 02:40:05.000000 lank-0.6.0/lank/config.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.894573 lank-0.6.0/lank/crypto/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1285 2022-07-06 23:02:05.000000 lank-0.6.0/lank/crypto/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5119 2022-07-09 03:16:52.000000 lank-0.6.0/lank/crypto/v1.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.895573 lank-0.6.0/lank/gateway/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2763 2023-03-20 13:06:52.000000 lank-0.6.0/lank/gateway/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2023-03-18 00:54:57.000000 lank-0.6.0/lank/gateway/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      846 2023-03-20 11:36:36.000000 lank-0.6.0/lank/gateway/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)    10426 2023-03-20 15:02:03.000000 lank-0.6.0/lank/gateway/node.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)       27 2022-07-09 17:02:10.000000 lank-0.6.0/lank/name.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.895573 lank-0.6.0/lank/node/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     9200 2023-03-20 12:16:37.000000 lank-0.6.0/lank/node/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:11:43.000000 lank-0.6.0/lank/node/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1836 2023-03-20 09:47:34.000000 lank-0.6.0/lank/node/cmd.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7216 2022-07-10 18:21:31.000000 lank-0.6.0/lank/node/db.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.896573 lank-0.6.0/lank/node/patch/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2035 2022-06-16 19:44:28.000000 lank-0.6.0/lank/node/patch/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1305 2022-06-17 06:07:47.000000 lank-0.6.0/lank/node/patch/v2.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1217 2022-07-01 03:06:08.000000 lank-0.6.0/lank/node/patch/v3.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      220 2022-07-07 20:36:15.000000 lank-0.6.0/lank/node/patch/v4.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.897573 lank-0.6.0/lank/node/protocol/
--rw-r--r--   0 shawn     (1000) shawn     (1000)    24013 2023-03-20 13:10:58.000000 lank-0.6.0/lank/node/protocol/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      175 2023-03-20 06:28:41.000000 lank-0.6.0/lank/node/protocol/ack.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     5577 2023-03-20 07:54:45.000000 lank-0.6.0/lank/node/protocol/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      356 2023-03-20 07:56:21.000000 lank-0.6.0/lank/node/protocol/deny.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     7600 2023-03-20 09:10:36.000000 lank-0.6.0/lank/node/protocol/peer.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     4671 2023-03-20 09:08:41.000000 lank-0.6.0/lank/node/protocol/register.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     6406 2023-03-20 08:40:23.000000 lank-0.6.0/lank/node/protocol/sync.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.898573 lank-0.6.0/lank/peer/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2294 2022-07-07 04:19:27.000000 lank-0.6.0/lank/peer/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:11.000000 lank-0.6.0/lank/peer/__main__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     2345 2022-07-14 23:13:40.000000 lank-0.6.0/lank/peer/cmd.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.898573 lank-0.6.0/lank/peer/protocol/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1750 2022-07-05 21:39:16.000000 lank-0.6.0/lank/peer/protocol/__init__.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.898573 lank-0.6.0/lank/peer/protocol/v1/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1668 2022-07-09 18:16:51.000000 lank-0.6.0/lank/peer/protocol/v1/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1041 2022-06-25 20:59:09.000000 lank-0.6.0/lank/peer/protocol/v1/message.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.899573 lank-0.6.0/lank/peer/protocol/v2/
--rw-r--r--   0 shawn     (1000) shawn     (1000)     3383 2022-07-24 05:05:22.000000 lank-0.6.0/lank/peer/protocol/v2/__init__.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1228 2022-06-25 21:42:27.000000 lank-0.6.0/lank/peer/protocol/v2/ack.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1108 2022-06-25 21:08:40.000000 lank-0.6.0/lank/peer/protocol/v2/base.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      416 2022-06-25 21:45:25.000000 lank-0.6.0/lank/peer/protocol/v2/media.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)     3122 2022-06-26 01:34:59.000000 lank-0.6.0/lank/peer/test.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)    12550 2023-03-20 16:08:13.000000 lank-0.6.0/lank/registration.py
--rw-r--r--   0 shawn     (1000) shawn     (1000)      106 2023-03-20 09:47:19.000000 lank-0.6.0/lank/util.py
-drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-03-20 16:29:49.894573 lank-0.6.0/lank.egg-info/
--rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/PKG-INFO
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1163 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/SOURCES.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)        1 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/dependency_links.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)      119 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/entry_points.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       81 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/requires.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)        5 2023-03-20 16:29:49.000000 lank-0.6.0/lank.egg-info/top_level.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       63 2022-06-14 21:35:01.000000 lank-0.6.0/requirements.txt
--rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2023-03-20 16:29:49.899573 lank-0.6.0/setup.cfg
--rw-r--r--   0 shawn     (1000) shawn     (1000)     1735 2023-03-20 09:31:14.000000 lank-0.6.0/setup.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.783802 lank-0.6.1/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       82 2023-03-18 00:58:16.000000 lank-0.6.1/.gitignore
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2486 2023-03-28 20:57:22.000000 lank-0.6.1/CHANGELOG
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1102 2022-07-10 22:31:07.000000 lank-0.6.1/LICENSE
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-05-28 23:42:08.783802 lank-0.6.1/PKG-INFO
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      352 2022-07-10 22:32:02.000000 lank-0.6.1/README.md
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.750801 lank-0.6.1/lank/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2022-06-14 19:59:08.000000 lank-0.6.1/lank/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:26.000000 lank-0.6.1/lank/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       23 2023-03-20 20:11:21.000000 lank-0.6.1/lank/__version__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1397 2023-03-20 09:45:57.000000 lank-0.6.1/lank/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      295 2022-07-01 02:40:05.000000 lank-0.6.1/lank/config.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.761801 lank-0.6.1/lank/crypto/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1285 2023-03-23 13:33:21.000000 lank-0.6.1/lank/crypto/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5119 2023-03-28 20:53:35.000000 lank-0.6.1/lank/crypto/v1.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      321 2023-03-23 15:20:04.000000 lank-0.6.1/lank/crypto/v2.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.767801 lank-0.6.1/lank/gateway/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7594 2023-05-28 23:41:18.000000 lank-0.6.1/lank/gateway/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2023-03-18 00:54:57.000000 lank-0.6.1/lank/gateway/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      846 2023-03-20 11:36:36.000000 lank-0.6.1/lank/gateway/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5715 2023-03-23 12:35:35.000000 lank-0.6.1/lank/gateway/node.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5399 2023-03-28 20:46:20.000000 lank-0.6.1/lank/gateway/peer.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       27 2022-07-09 17:02:10.000000 lank-0.6.1/lank/name.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.769801 lank-0.6.1/lank/node/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9199 2023-03-23 15:09:01.000000 lank-0.6.1/lank/node/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:11:43.000000 lank-0.6.1/lank/node/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1836 2023-03-20 09:47:34.000000 lank-0.6.1/lank/node/cmd.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7216 2022-07-10 18:21:31.000000 lank-0.6.1/lank/node/db.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.771802 lank-0.6.1/lank/node/patch/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2035 2022-06-16 19:44:28.000000 lank-0.6.1/lank/node/patch/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1305 2022-06-17 06:07:47.000000 lank-0.6.1/lank/node/patch/v2.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1217 2022-07-01 03:06:08.000000 lank-0.6.1/lank/node/patch/v3.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      220 2022-07-07 20:36:15.000000 lank-0.6.1/lank/node/patch/v4.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.777802 lank-0.6.1/lank/node/protocol/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)    24186 2023-03-28 08:23:56.000000 lank-0.6.1/lank/node/protocol/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      175 2023-03-20 06:28:41.000000 lank-0.6.1/lank/node/protocol/ack.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     6283 2023-03-28 12:30:29.000000 lank-0.6.1/lank/node/protocol/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      356 2023-03-20 07:56:21.000000 lank-0.6.1/lank/node/protocol/deny.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9134 2023-03-22 03:33:44.000000 lank-0.6.1/lank/node/protocol/peer.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     4671 2023-03-20 09:08:41.000000 lank-0.6.1/lank/node/protocol/register.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     6406 2023-03-20 08:40:23.000000 lank-0.6.1/lank/node/protocol/sync.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.780802 lank-0.6.1/lank/peer/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2310 2023-03-28 11:33:24.000000 lank-0.6.1/lank/peer/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      167 2022-06-27 03:07:11.000000 lank-0.6.1/lank/peer/__main__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2345 2022-07-14 23:13:40.000000 lank-0.6.1/lank/peer/cmd.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.782802 lank-0.6.1/lank/peer/protocol/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3527 2023-03-28 12:57:14.000000 lank-0.6.1/lank/peer/protocol/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2080 2023-03-28 20:50:42.000000 lank-0.6.1/lank/peer/protocol/ack.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5590 2023-03-28 13:03:53.000000 lank-0.6.1/lank/peer/protocol/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1167 2023-03-28 13:07:57.000000 lank-0.6.1/lank/peer/protocol/media.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1393 2023-03-28 11:24:26.000000 lank-0.6.1/lank/peer/protocol/wrap.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3122 2022-06-26 01:34:59.000000 lank-0.6.1/lank/peer/test.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)    12542 2023-05-28 23:41:18.000000 lank-0.6.1/lank/registration.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      106 2023-03-20 09:47:19.000000 lank-0.6.1/lank/util.py
+drwxr-xr-x   0 shawn     (1000) shawn     (1000)        0 2023-05-28 23:42:08.753801 lank-0.6.1/lank.egg-info/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      756 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/PKG-INFO
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1119 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        1 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      119 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/entry_points.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       81 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/requires.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        5 2023-05-28 23:42:08.000000 lank-0.6.1/lank.egg-info/top_level.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       63 2022-06-14 21:35:01.000000 lank-0.6.1/requirements.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       38 2023-05-28 23:42:08.783802 lank-0.6.1/setup.cfg
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1735 2023-03-20 09:31:14.000000 lank-0.6.1/setup.py
```

### Comparing `lank-0.6.0/CHANGELOG` & `lank-0.6.1/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Copyright (C) 2022-2023 LANNOCC (Shawn A. Wilson [lannocc@yahoo.com])
 @%@~LICENSE:MIT~@%@
 
+saw_032823_1 - Lots of work on gateway/peer. Begin some crypto upgrades.
+
+saw_032123_2 - Fixes for the last commit.
+
+saw_032123_1 - Upate GetHistory message to allow for filtering by name.
+
 saw_032023_5 - Registration upgraded. Note that peer stuff is still broken.
 
 saw_032023_4 - Gateway now converted from threading to asyncio.
 
 saw_032023_3 - Node client properly plays ping-pong again.
 
 saw_032023_2 - Flush output while printing by default. Handle incomplete reads.
```

### Comparing `lank-0.6.0/LICENSE` & `lank-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/PKG-INFO` & `lank-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lank
-Version: 0.6.0
+Version: 0.6.1
 Summary: Listening Anchor Nodes for K
 Home-page: https://github.com/lannocc/lank
 Author: LANNOCC (Shawn A. Wilson)
 Author-email: lannocc@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lank-0.6.0/lank/cmd.py` & `lank-0.6.1/lank/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/crypto/__init__.py` & `lank-0.6.1/lank/crypto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 
-VERSION = 1
+VERSION = 2
 
 cache = { }
 
 
 def get_handler(version=None):
     if not version:
         version = VERSION
```

### Comparing `lank-0.6.0/lank/crypto/v1.py` & `lank-0.6.1/lank/crypto/v1.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/gateway/cmd.py` & `lank-0.6.1/lank/gateway/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/gateway/node.py` & `lank-0.6.1/lank/registration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,258 @@
-from ..node import get_nodes
-from ..node.protocol import *
-
-from requests import get
+from .crypto import get_handler as get_crypto
+from .node import get_nodes
+from .node.protocol import *
 
 import asyncio
-#from threading import Thread, current_thread
-#from queue import Queue, Empty
-#import socket
+from concurrent.futures import ThreadPoolExecutor
+from getpass import getpass
+from uuid import uuid4
 
 
-class Client():
+class Interactive:
     def __init__(self, printer=print):
-        #def __init__(self, port, label, pwd, alias,
-        #    on_error, on_connect, verbose=True):
         self.print = printer
+        self.client = Client(printer)
+        self.crypto = get_crypto()
+
+    def run(self):
+        def exception(loop, context):
+            func = context.get('future').get_coro().__name__
+            msg = context.get('exception', context['message'])
+            name = type(msg).__name__
+            if name == 'KeyboardInterrupt': return
+            self.print(f'!!EE!! ({func}) {name} !! {msg}')
+
+        async def main():
+            asyncio.get_running_loop().set_exception_handler(exception)
+            await self.main()
+
+        asyncio.run(main())
+
+    async def main(self):
+        # TODO?: python 3.11
+        #async with asyncio.TaskGroup() as group:
+        #    group.create_task(self.client.main())
+        #    group.create_task(self.console())
+
+        #await asyncio.gather(
+        #        self.client.main(),
+        #        self.console())
+
+        node = asyncio.create_task(self.client.main())
+        try:
+            await self.console()
+
+        except BrokenPipeError:
+            self.print('ABORTED: lost connection to node')
+            await self.client.close()
+
+        node.cancel()
+
+    async def console(self):
+        await self.client.ready.wait()
+        if not self.client.node:
+            self.print('ABORTED: unable to connect to node')
+            return
+
+        self.print()
+        self.print('Ready to create/update a label with a new key pair.')
+        self.print()
+
+        label = await self.input('Label: ')
+        if label: label = label.strip()
+        if not label or not await self.client.online():
+            self.print('ABORTED')
+            return
+
+        uuid = uuid4()
+        exists = await self.client.check_label(uuid, label)
+        exists_priv_key = None
+
+        if exists is None:
+            self.print('ABORTED')
+            return
+
+        elif not exists:
+            password = await self.getpass('Password: ')
+
+        else:
+            self.print('   A label with that name already exists.')
+            uuid = exists.uuid
+
+            try:
+                priv_key = self.crypto.load_private_key(exists.key_pair_pem)
+
+                self.print('   ' \
+                    + 'ERROR: The existing key is OPEN and must remain so.')
+                self.print('ABORTED')
+                return
+
+            except TypeError: # (needs a password)
+                pass # this is expected
+
+            exists_password = await self.getpass('Existing Password: ')
+            if not exists_password:
+                self.print('ABORTED')
+                return
+
+            try:
+                priv_key = self.crypto.load_private_key(exists.key_pair_pem,
+                    password=exists_password)
+
+            except ValueError as e:
+                if e.args: e = ' | '.join(e.args)
+                self.print(f'   ERROR: {e}')
+                self.print('ABORTED')
+                return
+
+            exists_priv_key = priv_key
+            password = await self.getpass('New Password: ')
+
+            if password == exists_password:
+                self.print('   ' \
+                    + 'WARNING: New password is same as the old password.')
+
+        if password:
+            results = self.crypto.PASS_POLICY.test(password)
+            if label.lower() in password.lower():
+                results.append('Contains Label Name')
+            if results:
+                self.print('   WARNING: You have entered a WEAK PASSWORD.')
+                self.print('      ' \
+                    + 'This makes it VERY LIKELY somebody will STEAL it.')
+                self.print('      The following tests FAILED:')
+                for result in results:
+                    self.print(f'         - {result}')
+                self.print('      Proceed with CAUTION!')
+
+            confirm = await self.getpass('Confirm Password: ')
+            if confirm != password:
+                self.print('ABORTED (passwords do not match)')
+                return
+
+        else:
+            self.print('   ' \
+                + 'WARNING: Empty password creates an OPEN key pair.')
+            self.print('      ' \
+                + 'This means EVERYBODY is allowed to control the label')
+            self.print('      ' \
+                + 'FOREVER and CANNOT BE UNDONE. Proceed with CAUTION!')
+
+            agree = await self.input('Type AGREE to continue: ')
+            if agree != 'AGREE':
+                self.print('ABORTED')
+                return
+
+        self.print()
+        self.print('Generating key pair...', end='')
+        keys = self.crypto.make_keys(password)
+        self.print(' [done]')
+
+        priv_key = keys[0]
+        priv_key_pem = keys[1]
+        pub_key_pem = keys[2]
+
+        self.print('Creating signature...', end='')
+        if not exists:
+            time_nonce = self.crypto.make_time_nonce()
+            msg = self.crypto.get_register_message(label, time_nonce)
+            signature = self.crypto.sign(priv_key, msg)
+        else:
+            time_nonce = None
+            msg = self.crypto.get_reregister_message(
+                exists.time_nonce,
+                exists.uuid,
+                priv_key_pem + pub_key_pem)
+            signature = self.crypto.sign(exists_priv_key, msg)
+        self.print(' [done]')
+
+        self.print('Sanity check...', end='')
+        if not exists:
+            assert self.crypto.verify(priv_key.public_key(), msg, signature)
+        else:
+            assert self.crypto.verify(exists_priv_key.public_key(), msg,
+                                      signature)
+        self.print(' [done]')
+
+        self.print('Transmitting...')
+        if await self.client.register_label(uuid, label, priv_key_pem,
+                pub_key_pem, signature, self.crypto.VERSION, time_nonce):
+            self.print(' [SUCCESS]')
+
+        else:
+            self.print(' [FAIL]')
+
+        await self.client.close()
+
+    async def input(self, prompt=''):
+        with ThreadPoolExecutor(1, "Interactive") as exe:
+            loop = asyncio.get_event_loop()
+            return await loop.run_in_executor(exe, input, prompt)
+
+    async def getpass(self, prompt=''):
+        with ThreadPoolExecutor(1, "Interactive") as exe:
+            loop = asyncio.get_event_loop()
+            return await loop.run_in_executor(exe, getpass, prompt)
+
+
+
 
-        self.host = self.get_public_ip()
-        #self.port = port
-        #self.label = label
-        #self.pwd = pwd or None
-        #self.alias = alias or None
-        #self.on_error = on_error
-        #self.on_connect = on_connect
 
-        self.node = None
-        #self.input = Queue()
-        #self.output = Queue()
 
-        #self.ping = None
-        #self.sign_on = False
-        #self.labels_callback = None
-        #self.history_callback = None
-        #self.register_callback = None
-
-        #self.sender_thread = Thread(
-        #    name='node-sender', target=self.sender)
-        #self.receiver_thread = Thread(
-        #    name='node-return', target=self.receiver)
+
+
+
+class Client():
+    def __init__(self, printer=print):
+        self.print = printer
+        self.node = None
+        self.ready = asyncio.Event()
+        self.closing = False
 
     def __str__(self):
         if not self.node:
             return 'no connection'
 
-        #if not self.node.sock:
-        #    return 'no connection (sock)'
-
         return f'{self.node.reader._transport.get_extra_info("peername")}'
 
     def run(self):
         def exception(loop, context):
             func = context.get('future').get_coro().__name__
             msg = context.get('exception', context['message'])
             name = type(msg).__name__
+            if name == 'KeyboardInterrupt': return
             self.print(f'!!EE!! ({func}) {name} !! {msg}')
 
         async def main():
             asyncio.get_running_loop().set_exception_handler(exception)
             await self.main()
 
         asyncio.run(main())
 
     async def main(self):
-        # FIXME: this needs to be smarter (keep a pool of active nodes?)
-
         for addr in get_nodes():
+            if self.closing: break
+
             try:
                 self.print(f'N+ connecting to {addr}')
                 host, port = addr
 
                 reader, writer = await asyncio.wait_for(
                         asyncio.open_connection(host, port),
                         timeout=HELLO_TIMEOUT)
 
                 try:
                     handler = Handler(addr, reader, writer, printer=self.print)
                     await handler.hello()
 
                     try:
                         self.node = handler
+                        self.ready.set()
+                        self.print('N  ready')
 
                         while True:
                             await asyncio.sleep(KEEPALIVE)
 
                             ping = Ping()
                             await self.send(ping)
                             pong = await self.recv()
@@ -95,24 +266,23 @@
                             if pong.nonce != ping.nonce:
                                 raise ValueError('nonce mismatch')
 
                         self.print(f'N- finished {addr}')
 
                     except KeyError as e:
                         self.print(f'N- terminated {addr} [DENIED: {e}]')
-                        #if 'NodeIsSelf' in str(e):
-                        #    self.nodes_client[addr] = False
 
                     except ValueError as e:
                         self.print(f'N- terminated {addr} [BAD MESSAGE: {e}]')
 
                     except asyncio.TimeoutError:
                         self.print(f'N- terminated {addr} [GENERAL TIMEOUT]')
 
                     finally:
+                        self.ready.clear()
                         self.node = None
 
                 except BrokenPipeError:
                     self.print(f'N- closed {addr} [BROKEN PIPE]')
 
                 except ConnectionResetError:
                     self.print(f'N- closed {addr} [CONNECTION RESET]')
@@ -135,199 +305,88 @@
                 self.print(f'N- closed {addr} [CONNECTION REFUSED]')
 
             except asyncio.TimeoutError:
                 self.print(f'N- terminated {addr} [CONNECT TIMEOUT]')
 
             except Exception as e:
                 name = type(e).__name__
-                self.print(f'N- terminated {addr} [ERROR: {name}] !! {e}')
+                self._error_(f'N- terminated {addr} [ERROR: {name}] !! {e}')
                 raise e
 
-        if not self.node: return
-
-        '''
-        self.input.put_nowait(GetRegistration(self.label))
-        msg = self.output.get(timeout=GENERAL_TIMEOUT)
-        if not msg: return
-        if not isinstance(msg, Registration):
-            return self.error(f'failed to get label info: {msg}')
-
-        try:
-            crypto = get_crypto(msg.version)
-            priv_key = crypto.load_private_key(msg.key_pair_pem, self.pwd)
-
-            self.app.server.crypto = crypto
-            self.app.server.priv_key = priv_key
-
-        except TypeError as e:
-            return self.error(f'failed to unlock private key: {e}')
-        except ValueError as e:
-            return self.error(f'failed to unlock private key: {e}')
-
-        msg = PeerOn(crypto.VERSION, self.label, self.host, self.port,
-                     self.alias if self.alias else None)
-        msg.signature = crypto.sign(priv_key, msg.to_sign(crypto))
-
-        self.sign_on = True
-        self.input.put_nowait(msg)
-        msg = self.output.get(timeout=GENERAL_TIMEOUT)
-        if not msg: return
-        if not isinstance(msg, Signed):
-            return self.error(f'failed to sign on: {msg}')
-        self.sign_on = False
-
-        config.save_connect_label(self.label)
-        config.save_connect_alias(self.alias)
-
-        self.input.put_nowait(ListLabels())
-        msg = self.output.get(timeout=GENERAL_TIMEOUT)
-        if not msg: return
-        if not isinstance(msg, LabelsList):
-            return self.error(f'failed to get labels list: {msg}')
-
-        for label in msg.labels:
-            if label in self.app.interests:
-                self.input.put(LabelInterest(label))
+        self.ready.set()
 
-        self.on_connect(msg.labels)
-        '''
+    async def _error_(self, txt):
+        if self.closing: return
+        self.print()
+        self.print(f'** ERROR ** [{txt}]')
+        await self.close()
 
     async def send(self, msg):
-        if not self.node: return
+        if not await self.online(): return
         self.print(f'N    {self.node.addr} <- {msg}')
         await self.node.send(msg)
 
     async def recv(self):
-        if not self.node: return None
+        if not await self.online(): return
         msg = await self.node.recv()
+        if not msg: raise BrokenPipeError()
         self.print(f'N    {self.node.addr} -> {msg}')
         return msg
 
-    async def list_labels(self):
-        await self.send(ListLabels())
-        return await self.recv()
-
-    async def get_registration(self, label):
-        await self.send(GetRegistration(label))
-        return await self.recv()
-
-    async def get_history(self, label):
-        await self.send(GetHistory(label))
-        return await self.recv()
-
-    '''
-    def interest(self, label, notify=True):
-        self.input.put_nowait(
-            LabelInterest(label) if notify else LabelIgnore(label))
-
-    def get_labels(self, callback):
-        if self.labels_callback:
-            return self.error(f'never received last labels request')
-
-        self.labels_callback = callback
-        self.input.put_nowait(ListLabels())
-
-    def get_registration(self, label, callback):
-        if self.register_callback:
-            return self.error(f'never received last registration request')
-
-        self.register_callback = callback
-        self.input.put_nowait(GetRegistration(label))
-
-    def get_history(self, label, callback):
-        if self.history_callback:
-            return self.error(f'never received last history request')
-
-        self.history_callback = callback
-        self.register_callback = self._get_history_
-
-        self.input.put_nowait(GetRegistration(label))
-
-    def _get_history_(self, registration):
-        callback = self.history_callback
-        def history_callback(history):
-            callback(registration, history)
-        self.history_callback = history_callback
-        self.input.put_nowait(GetHistory(registration.label))
-
-    def stop(self):
-        if not self.node: return
-        self.print('stopping')
-        node = self.node
-        self.node = None
-
-        node.sock.shutdown(socket.SHUT_RDWR)
-        node.sock.close()
-        self.output.put_nowait(None)
-        self.input.put_nowait(None)
-
-    def join(self):
-        self.receiver_thread.join()
-        self.sender_thread.join()
-        super().join()
-
-    def sender(self):
-        try:
-            while self.node:
-                try:
-                    #while msg := self.input.get(timeout=KEEPALIVE):
-                    msg = self.input.get(timeout=KEEPALIVE)
-                    if msg:
-                        if not self.node: break
-                        self.send(msg)
-
-                except Empty:
-                    if self.ping:
-                        return self.error('ping sent but no pong received')
-
-                    if self.node:
-                        self.ping = Ping()
-                        self.send(self.ping)
-
-        finally:
-            self.stop()
-
-    def receiver(self):
-        try:
-            #while msg := self.recv():
-            msg = self.recv()
-            while msg:
-                if isinstance(msg, Pong):
-                    if not self.ping:
-                        return self.error(f'received pong without ping: {msg}')
-
-                    if msg.nonce != self.ping.nonce:
-                        return self.error(f'ping-pong nonce mismatch')
-
-                    self.ping = None
-
-                elif isinstance(msg, Signed):
-                    self.app.notify(msg)
-
-                    if self.sign_on:
-                        self.output.put(msg)
-
-                else:
-                    self.output.put(msg)
+    async def online(self):
+        if not self.node:
+            await self.ready.wait()
 
-                msg = self.recv()
+        return self.node
 
-            self.error('lost connection')
+    async def close(self):
+        self.closing = True
+        if self.node:
+            self.node.writer.close()
+            await self.node.writer.wait_closed()
+        self.node = None
+        self.ready.set()
 
-        except OSError as e:
-            self.error(e)
+    async def check_label(self, uuid, label):
+        await self.send(Reservation(label, uuid))
+        resp = await self.recv()
+
+        if isinstance(resp, Reservation):
+            return False
+
+        elif isinstance(resp, ReservationCancel):
+            #return False if resp.exists else None
+            # FIXME: if exists, transmit request to get the key
+
+            if not resp.exists:
+                self._error_('LABEL RESERVATION CONFLICT')
+                return None
+
+            await self.send(GetRegistration(label))
+            resp = await self.recv()
+
+            assert isinstance(resp, Registration)
+            return resp
+
+        else:
+            return None
+
+    async def register_label(self, uuid, label, priv_key_pem, pub_key_pem,
+                       signature, version, time_nonce=None):
+        if time_nonce:
+            req = Registration(uuid, label, version, time_nonce,
+                               priv_key_pem + pub_key_pem,
+                               signature)
+        else:
+            req = ReRegistration(uuid4(), label, version, str(uuid),
+                                 priv_key_pem + pub_key_pem,
+                                 signature)
 
-        finally:
-            self.stop()
+        await self.send(req)
+        resp = await self.recv()
 
-    def error(self, e):
-        if not self.node: return
-        self.print(f'** ERROR ** {e}')
-        #self.on_error(e)
-        self.stop()
-    '''
+        if isinstance(resp, RegistrationSuccess):
+            return True
 
-    def get_public_ip(self):
-        ip = get('http://api.ipify.org').content.decode('utf-8')
-        self.print(f' - our public IP address: {ip}')
-        return ip
+        else:
+            return False
```

### Comparing `lank-0.6.0/lank/node/__init__.py` & `lank-0.6.1/lank/node/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         async def main():
             asyncio.get_running_loop().set_exception_handler(exception)
             await self.main()
 
         asyncio.run(main())
 
     async def main(self):
-
         for label in self.ldb.list_labels():
             self.labels_by_id[label['id']] = label['name']
 
         self.print(f'   getting time from {NTP}...')
         ntp = NTPClient().request(NTP, version=3)
         self.offset = ntp.offset
         self.print(f'      our clock is {abs(self.offset)} seconds ', end='')
```

### Comparing `lank-0.6.0/lank/node/cmd.py` & `lank-0.6.1/lank/node/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/db.py` & `lank-0.6.1/lank/node/db.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/patch/__init__.py` & `lank-0.6.1/lank/node/patch/__init__.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/patch/v2.py` & `lank-0.6.1/lank/node/patch/v2.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/patch/v3.py` & `lank-0.6.1/lank/node/patch/v3.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/protocol/__init__.py` & `lank-0.6.1/lank/node/protocol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from bidict import bidict
 
 import asyncio
 from datetime import datetime, timedelta
 from uuid import UUID
 
 
-VERSION = 3
+VERSION = 4
 HELLO = b'\x04\x02\x00HOLANK\x00\x02\x04'
 HELLO_SIZE = len(HELLO) # bytes
 HELLO_TIMEOUT = 3 # seconds
 MAX_TIME_SKEW = 9 # seconds
 KEEPALIVE = 99 # seconds
-GENERAL_TIMEOUT = KEEPALIVE * 2 # seconds
+GENERAL_TIMEOUT = 2*KEEPALIVE # seconds
 
 
 class VersionMismatch(BaseException):
     def __init__(self, want, got):
         super().__init__(f'want {want} but got {got}')
 
 
@@ -720,16 +720,21 @@
 
         try:
             label_id = master.labels_by_id.inverse[msg.label]
 
         except KeyError:
             return LabelNotFound(msg.label)
 
-        signed_list = master.ldb.find_signed_by_label(
-            label_id, msg.start + msg.count)
+        if msg.name:
+            signed_list = master.ldb.find_signed_by_label_name(
+                label_id, msg.name, limit=msg.start+msg.count)
+
+        else:
+            signed_list = master.ldb.find_signed_by_label(
+                label_id, limit=msg.start+msg.count)
 
         items = [ ]
         idx = 0
         end = msg.start + msg.count - 1
 
         for signed in signed_list:
             if idx >= msg.start:
```

### Comparing `lank-0.6.0/lank/node/protocol/base.py` & `lank-0.6.1/lank/peer/protocol/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 import random
-from datetime import datetime, timezone, timedelta
-from uuid import UUID
+from datetime import datetime, timezone
+from json import JSONEncoder
+from base64 import b64encode
 
 
 class Message(ABC):
     def __str__(self):
         txt = self._str_()
         return self.__repr__() + (f'[{txt}]' if txt else '')
 
@@ -16,14 +17,36 @@
         return None
 
     @classmethod
     async def recv(cls, handler):
         return cls()
 
 
+class MessageEncoder(JSONEncoder):
+        def __init__(self, sort_keys=False):
+            super().__init__(sort_keys=sort_keys)
+
+        def default(self, obj):
+            if isinstance(obj, Message):
+                data = vars(obj)
+                #if hasattr(obj, 'to_sign'):
+                #    data = data.copy()
+                #    data['to_sign'] = obj.to_sign(self.crypto)
+                return { type(obj).__name__: data }
+
+            elif isinstance(obj, bytes):
+                return b64encode(obj).decode()
+
+            elif isinstance(obj, UUID):
+                return str(obj)
+
+            else:
+                return json.JSONEncoder.default(self, obj)
+
+
 class Nonced(Message, ABC):
     NONCE_SIZE = 8 # bytes
 
     def __init__(self, nonce=None):
         if nonce is None:
             nonce = random.randrange(256**self.NONCE_SIZE)
         self.nonce = nonce
@@ -55,18 +78,18 @@
     def __init__(self, timestamp):
         self.timestamp = self._from_datetime_(timestamp)
 
     def _str_(self):
         time = self._to_datetime_(self.timestamp).isoformat()
         return f'timestamp={time}'
 
-    def check_time_skew(self, now, max_skew):
-        now = self._from_datetime_(now)
-        skew = abs(now / self.TS_PRECISION - self.timestamp / self.TS_PRECISION)
-        return skew <= max_skew
+    #def check_time_skew(self, now, max_skew):
+    #    now = self._from_datetime_(now)
+    #    skew = abs(now / self.TS_PRECISION - self.timestamp / self.TS_PRECISION)
+    #    return skew <= max_skew
 
     def to_bytes(self, handler):
         return self._timestamp_bytes_(handler, self.timestamp)
 
     @classmethod
     def _timestamp_bytes_(cls, handler, ts):
         return ts.to_bytes(cls.TIMESTAMP_SIZE, handler.BYTE_ORDER)
@@ -81,51 +104,22 @@
     async def _timestamp_(cls, handler):
         timestamp = await handler.recv_bytes(cls.TIMESTAMP_SIZE)
         if timestamp is None: return None
         return int.from_bytes(timestamp, handler.BYTE_ORDER)
 
     @classmethod
     def _from_datetime_(cls, dt):
+        print(f'XXXXX {dt}')
         return int(dt.timestamp() * cls.TS_PRECISION)
 
     @classmethod
     def _to_datetime_(cls, ts):
         return datetime.fromtimestamp(ts / cls.TS_PRECISION, timezone.utc)
 
 
-class Identified(Message, ABC):
-    UUID_SIZE = 16 # bytes
-
-    def __init__(self, uuid):
-        assert isinstance(uuid, UUID)
-        self.uuid = uuid
-
-    def _str_(self):
-        return f'uuid={self.uuid}'
-
-    def to_bytes(self, handler):
-        return self._uuid_bytes_(handler, self.uuid)
-
-    @classmethod
-    def _uuid_bytes_(cls, handler, uuid):
-        return uuid.bytes
-
-    @classmethod
-    async def recv(cls, handler):
-        uuid = await cls._uuid_(handler)
-        if uuid is None: return None
-        return cls(uuid)
-
-    @classmethod
-    async def _uuid_(cls, handler):
-        uuid = await handler.recv_bytes(cls.UUID_SIZE)
-        if uuid is None: return None
-        return UUID(bytes=bytes(uuid))
-
-
 class Labeled(Message, ABC):
     LABEL_SIZE_SIZE = 1 # bytes
 
     def __init__(self, label):
         assert label
         self.label = label
```

### Comparing `lank-0.6.0/lank/node/protocol/peer.py` & `lank-0.6.1/lank/node/protocol/peer.py`

 * *Files 11% similar despite different names*

```diff
@@ -154,81 +154,118 @@
 class LabelIgnore(Labeled):
     pass
 
 
 class GetHistory(Labeled):
     START_SIZE = 1 # bytes
     COUNT_SIZE = 1 # bytes
+    NAME_SIZE = 1 # bytes
 
-    def __init__(self, label, start=0, count=5):
+    def __init__(self, label, start=0, count=5, name=0):
         Labeled.__init__(self, label)
         self.start = start
         self.count = count
+        self.name = name
 
     def _str_(self):
         return ', '.join([
             Labeled._str_(self),
             f'start={self.start}',
             f'count={self.count}',
+            f'name={self.name}',
         ])
 
     def to_bytes(self, handler):
         label = Labeled.to_bytes(self, handler)
 
         start = self.start
         assert start >= 0 and start < 256**self.START_SIZE
         start = start.to_bytes(self.START_SIZE, handler.BYTE_ORDER)
 
         count = self.count
         assert count > 0 and count < 256**self.COUNT_SIZE
         count = count.to_bytes(self.COUNT_SIZE, handler.BYTE_ORDER)
 
-        return label + start + count
+        name = self.name
+        assert name >= 0 and name < 256**self.NAME_SIZE
+        name = name.to_bytes(self.NAME_SIZE, handler.BYTE_ORDER)
+
+        return label + start + count + name
 
     @classmethod
     async def recv(cls, handler):
         label = await cls._label_(handler)
         if label is None: return None
 
         start = await cls._start_(handler)
         if start is None: return None
 
         count = await cls._count_(handler)
         if count is None: return None
 
-        return cls(label, start, count)
+        name = await cls._name_(handler)
+        if name is None: return None
+
+        return cls(label, start, count, name)
 
     @classmethod
     async def _start_(cls, handler):
         start = await handler.recv_bytes(cls.START_SIZE)
         if start is None: return None
         return int.from_bytes(start, handler.BYTE_ORDER)
 
     @classmethod
     async def _count_(cls, handler):
         count = await handler.recv_bytes(cls.COUNT_SIZE)
         if count is None: return None
         return int.from_bytes(count, handler.BYTE_ORDER)
 
+    @classmethod
+    async def _name_(cls, handler):
+        name = await handler.recv_bytes(cls.NAME_SIZE)
+        if name is None: return None
+        return int.from_bytes(name, handler.BYTE_ORDER)
+
+
+class History(Labeled):
+    START_SIZE = 1 # bytes
+    COUNT_SIZE = 1 # bytes
 
-class History(GetHistory):
     def __init__(self, label, start, items):
-        GetHistory.__init__(self, label, start, len(items))
+        Labeled.__init__(self, label)
+        self.start = start
+        self.count = len(items)
         self.items = items
 
+    def _str_(self):
+        return ', '.join([
+            Labeled._str_(self),
+            f'start={self.start}',
+            f'count={self.count}',
+            #f'items={self.items}',
+        ])
+
     def to_bytes(self, handler):
-        label_start_count = GetHistory.to_bytes(self, handler)
+        label = Labeled.to_bytes(self, handler)
+
+        start = self.start
+        assert start >= 0 and start < 256**self.START_SIZE
+        start = start.to_bytes(self.START_SIZE, handler.BYTE_ORDER)
+
         assert self.count == len(self.items)
+        count = self.count
+        assert count >= 0 and count < 256**self.COUNT_SIZE
+        count = count.to_bytes(self.COUNT_SIZE, handler.BYTE_ORDER)
 
         items = b''
         for signed in self.items:
             assert isinstance(signed, Signed)
             items += signed.to_bytes(handler)
 
-        return label_start_count + items
+        return label + start + count + items
 
     @classmethod
     async def recv(cls, handler):
         label = await cls._label_(handler)
         if label is None: return None
 
         start = await cls._start_(handler)
@@ -241,7 +278,19 @@
         for i in range(count):
             item = await Signed.recv(handler)
             if item is None: return None
             items.append(item)
 
         return cls(label, start, items)
 
+    @classmethod
+    async def _start_(cls, handler):
+        start = await handler.recv_bytes(cls.START_SIZE)
+        if start is None: return None
+        return int.from_bytes(start, handler.BYTE_ORDER)
+
+    @classmethod
+    async def _count_(cls, handler):
+        count = await handler.recv_bytes(cls.COUNT_SIZE)
+        if count is None: return None
+        return int.from_bytes(count, handler.BYTE_ORDER)
+
```

### Comparing `lank-0.6.0/lank/node/protocol/register.py` & `lank-0.6.1/lank/node/protocol/register.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/node/protocol/sync.py` & `lank-0.6.1/lank/node/protocol/sync.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/peer/__init__.py` & `lank-0.6.1/lank/peer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# FIXME
+'''
 from .protocol import get_handler, HELLO
 
 from gevent.pool import Pool
 from gevent.server import StreamServer
 
 from socket import timeout
 
@@ -75,8 +77,9 @@
                 print(f' - terminated {addr} [BAD HELLO]')
 
             else:
                 print(f' - closed {addr} [CLIENT ABORT]')
 
         except timeout:
             print(f' - terminated {addr} [HELLO TIMEOUT]')
+'''
```

### Comparing `lank-0.6.0/lank/peer/cmd.py` & `lank-0.6.1/lank/peer/cmd.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank/peer/protocol/v2/__init__.py` & `lank-0.6.1/lank/peer/protocol/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,124 @@
-from ..v1 import Handler as Base
 from .ack import *
+from .wrap import *
 from .media import *
 
 from bidict import bidict
 
+import asyncio
 
-class Handler(Base):
-    VERSION = 2
 
+VERSION = 3
+HELLO = b'\x04\x02\x00peerHOLANK\x00\x02\x04'
+HELLO_SIZE = len(HELLO) # bytes
+HELLO_TIMEOUT = 3 # seconds
+#MAX_TIME_SKEW = 9 # seconds
+KEEPALIVE = 90 # seconds
+GENERAL_TIMEOUT = 2*KEEPALIVE # seconds
+
+
+class VersionMismatch(BaseException):
+    def __init__(self, want, got):
+        super().__init__(f'want {want} but got {got}')
+
+
+class Handler:
+    #BUFFER_SIZE = 128 # bytes
+    BYTE_ORDER = 'big'
+    ID_SIZE = 1 # bytes
     ENCODING = 'utf-8'
-    BUFFER_SIZE = 2048 # bytes
-    CRYPTO_SIG_SIZE = 512 # bytes
-    CRYPTO_SIZE_SIZE = 3 # bytes
 
     MSG_BY_ID = bidict({
         1: Ping,
         2: Pong,
-        3: Text,
+        3: Signed,
+        4: Text,
     })
 
-    def __init__(self, sock, addr, crypto, priv_key, pub_key=None):
-        super().__init__(sock, addr)
-
-        self.crypto = crypto
-        self.priv_key = priv_key
-        self.pub_key = pub_key
-        self.label = None
-
-    def server(self, master):
-        #self.print('here we go')
-        #while msg := self.recv():
-        msg = self.recv(master)
-        while msg:
-            self.print(f'S    {self.addr} -> {msg}')
-            reply = None
-
-            if isinstance(msg, Ping):
-                reply = Pong(msg.nonce)
-
-            elif isinstance(msg, Text):
-                #reply = Text('got your message')
-                master.on_text(msg, self)
-
-            else:
-                raise ValueError(f'unhandled message: {msg}')
-
-            if reply:
-                self.print(f'S    {self.addr} <- {reply}')
-                self.send(reply)
+    def __init__(self, addr, reader, writer, printer=print):
+        self.addr = addr
+        self.reader = reader
+        self.writer = writer
+        self.print = printer
+
+    async def hello(self):
+        assert VERSION > 0 and VERSION < 256
+        self.writer.write(HELLO + VERSION.to_bytes(1, 'big'))
+        return await asyncio.wait_for(
+                self.writer.drain(), timeout=HELLO_TIMEOUT)
+
+    async def ack(self):
+        hello = await asyncio.wait_for(
+                self.reader.readexactly(HELLO_SIZE+1), timeout=HELLO_TIMEOUT)
+        if hello[:-1] != HELLO:
+            return False
+
+        version = hello[-1]
+        if version != VERSION:
+            # FIXME: more sophisticated version negotiation?
+            raise VersionMismatch(VERSION, version)
+
+        return True
+
+    async def s_send(self, msg):
+        self.print(f'S    {self.addr} <- {msg}')
+        await self.send(msg)
+
+    async def c_send(self, msg):
+        self.print(f'C    {self.addr} <- {msg}')
+        await self.send(msg)
+
+    async def s_recv(self):
+        msg = await self.recv()
+        self.print(f'S    {self.addr} -> {msg}')
+        return msg
 
-            msg = self.recv(master)
+    async def c_recv(self):
+        msg = await asyncio.wait_for(
+                self.recv(), timeout=KEEPALIVE)
+        self.print(f'C    {self.addr} -> {msg}')
+        return msg
 
-    def send(self, msg):
+    async def send(self, msg):
         id_bytes = self.get_id_bytes(msg)
         data = msg.to_bytes(self)
+        self.writer.write(id_bytes + (data if data else b''))
+        return await asyncio.wait_for(
+                self.writer.drain(), timeout=GENERAL_TIMEOUT)
+
+    async def recv(self):
+        id_bytes = await self.recv_bytes(self.ID_SIZE)
+        if id_bytes is None: return None
+        msg = self.get_msg_type(id_bytes)
+        return await msg.recv(self)
+
+    async def recv_bytes(self, size, timeout=GENERAL_TIMEOUT):
+        #FIXME
+        #if size > self.BUFFER_SIZE:
+        #    raise ValueError(f'request to read more than buffer allows: {size}')
+        try:
+            return await asyncio.wait_for(
+                    self.reader.readexactly(size), timeout=timeout)
 
-        data = self.crypto.encrypt(self.pub_key,
-            id_bytes + (data if data else b''))
-
-        sig = self.crypto.sign(self.priv_key, data)
-        assert len(sig) == self.CRYPTO_SIG_SIZE
-
-        size_bytes = len(data).to_bytes(self.CRYPTO_SIZE_SIZE, self.BYTE_ORDER)
-
-        self.sock.sendall(sig + size_bytes + data)
-
-    def recv(self, master):
-        #self.print('receiving')
-        sig = self.recv_bytes(self.CRYPTO_SIG_SIZE)
-        if not sig:
-            #self.print('recv: no sig')
+        except asyncio.IncompleteReadError:
             return None
-        sig = bytes(sig)
-
-        crypto_size = self.recv_bytes(self.CRYPTO_SIZE_SIZE)
-        if not crypto_size: return None
-        crypto_size = int.from_bytes(crypto_size, self.BYTE_ORDER)
-        if not crypto_size: return None
 
-        data = self.recv_bytes(crypto_size)
-        if not data: return None
-        data = bytes(data)
-
-        verify = (data, sig)
-        data = self.crypto.decrypt(self.priv_key, data)
-
-        msg = self.get_msg_type(data[:self.ID_SIZE])
-        data = data[self.ID_SIZE:]
-
-        if not issubclass(msg, Ping):
-            if not self.pub_key:
-                raise ValueError(f'have signed message but no key to check')
-
-            if not self.crypto.verify(self.pub_key, verify[0], verify[1]):
-                raise ValueError(f'signature verification failed')
-
-        msg = msg.from_bytes(self, data)
-
-        if isinstance(msg, Ping):
-            #self.print('got ping')
-            if msg.label != self.label:
-                self.pub_key = master.get_public_key(self.crypto, msg.label)
-
-                if not self.pub_key:
-                    raise ValueError(f'no key on file for label: {msg.label}')
-
-                self.label = msg.label
-                self.print(f'S    {self.addr} is {self.label}')
-                master.on_peered(self)
-
-            if not self.crypto.verify(self.pub_key, verify[0], verify[1]):
-                raise ValueError(f'signature verification failed')
-
-        return msg
+    def get_id_bytes(self, msg):
+        try:
+            mid = self.MSG_BY_ID.inverse[type(msg)]
+            try:
+                return mid.to_bytes(self.ID_SIZE, self.BYTE_ORDER)
+
+            except OverflowError as e:
+                raise ValueError(f'msg type id too big: {mid}') from e
+
+        except KeyError as e:
+            raise ValueError(f'unsupported message type: {type(msg)}') from e
+
+    def get_msg_type(self, id_bytes):
+        mid = int.from_bytes(id_bytes, self.BYTE_ORDER)
+        try:
+            return self.MSG_BY_ID[mid]
 
-    def print(self, txt):
-        print(txt)
+        except KeyError as e:
+            raise ValueError(f'unsupported message type id: {mid}') from e
```

### Comparing `lank-0.6.0/lank/peer/protocol/v2/ack.py` & `lank-0.6.1/lank/peer/protocol/ack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,82 @@
-from .base import Nonced
+from .base import Nonced #, Autographed, Labeled, Timestamped
 
 
 class Ping(Nonced):
-    #LABEL_SIZE_SIZE = 1 # bytes
+    pass
 
-    def __init__(self, label, nonce=None):
-        assert label
-        self.label = label
+
+class Pong(Nonced):
+    def __init__(self, nonce):
+        assert nonce is not None
         super().__init__(nonce)
 
+
+'''
+class Signed(Autographed):
+    PAYLOAD_SIZE_SIZE = 3 # bytes
+
+    def __init__(self, version, signature, data):
+        Autographed.__init__(self, version, signature)
+        self.data = data
+
     def _str_(self):
-        return super()._str_() + ', ' + f'label={self.label}'
+        return ', '.join([
+            Autographed._str_(self),
+            f'size={len(self.data)}',
+        ])
 
     def to_bytes(self, handler):
-        label = self.label.encode(handler.ENCODING)
-        #size = len(label)
-        #assert size > 0 and size < 256**self.LABEL_SIZE_SIZE
-
-        #return super().to_bytes(handler) \
-        #    + size.to_bytes(self.LABEL_SIZE_SIZE, handler.BYTE_ORDER) \
-        #    + label
-        return super().to_bytes(handler) + label
+        autograph = Autographed.to_bytes(self, handler)
+
+        size = len(self.data)
+        assert size > 0 and size < 256**self.PAYLOAD_SIZE_SIZE
+        size = size.to_bytes(self.PAYLOAD_SIZE_SIZE, handler.BYTE_ORDER)
+
+        return autograph + size + self.data
 
     @classmethod
-    def from_bytes(cls, handler, data):
+    async def recv(cls, handler):
+        ver = await cls._version_(handler)
+        if ver is None: return None
+
+        sig = await cls._signature_(handler)
+        if sig is None: return None
+
+        size = await handler.recv_bytes(cls.PAYLOAD_SIZE_SIZE)
+        if size is None: return None
+        size = int.from_bytes(size, handler.BYTE_ORDER)
+
+        data = await handler.recv_bytes(size)
         if data is None: return None
-        nonce, data = cls._from_bytes_(handler, data)
-        #assert len(data) > cls.LABEL_SIZE_SIZE
 
-        #size = int.from_bytes(data[:cls.LABEL_SIZE_SIZE], handler.BYTE_ORDER)
-        #assert size > 0
+        return cls(ver, sig, data)
+
 
-        #data = data[cls.LABEL_SIZE_SIZE:]
-        #assert len(data) == size
-        label = str(data, handler.ENCODING)
+class Identification(Labeled, Timestamped):
+    def __init__(self, label, timestamp):
+        Labeled.__init__(self, label)
+        Timestamped.__init__(self, timestamp)
 
-        return cls(label, nonce)
+    def _str_(self):
+        return ', '.join([
+            Labeled._str_(self),
+            Timestamped._str_(self),
+        ])
 
+    def to_bytes(self, handler):
+        label = Labeled.to_bytes(self, handler)
+        timestamp = Timestamped.to_bytes(self, handler)
 
-class Pong(Nonced):
-    def __init__(self, nonce):
-        assert nonce is not None
-        super().__init__(nonce)
+        return label + timestamp
+
+    @classmethod
+    async def recv(cls, handler):
+        label = await cls._label_(handler)
+        if label is None: return None
+
+        timestamp = await cls._timestamp_(handler)
+        if timestamp is None: return None
+
+        return cls(label, timestamp)
+'''
```

### Comparing `lank-0.6.0/lank/peer/test.py` & `lank-0.6.1/lank/peer/test.py`

 * *Files identical despite different names*

### Comparing `lank-0.6.0/lank.egg-info/PKG-INFO` & `lank-0.6.1/lank.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lank
-Version: 0.6.0
+Version: 0.6.1
 Summary: Listening Anchor Nodes for K
 Home-page: https://github.com/lannocc/lank
 Author: LANNOCC (Shawn A. Wilson)
 Author-email: lannocc@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lank-0.6.0/setup.py` & `lank-0.6.1/setup.py`

 * *Files identical despite different names*

