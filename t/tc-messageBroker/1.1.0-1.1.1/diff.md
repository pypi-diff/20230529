# Comparing `tmp/tc-messageBroker-1.1.0.tar.gz` & `tmp/tc-messageBroker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.1.0.tar", last modified: Thu May 25 12:45:42 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.1.1.tar", last modified: Mon May 29 12:02:49 2023, max compression
```

## Comparing `tc-messageBroker-1.1.0.tar` & `tc-messageBroker-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.178612 tc-messageBroker-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:45:42.178612 tc-messageBroker-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.170612 tc-messageBroker-1.1.0/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.170612 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 12:45:42.000000 tc-messageBroker-1.1.0/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:42.174612 tc-messageBroker-1.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-25 12:45:08.000000 tc-messageBroker-1.1.0/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.189578 tc-messageBroker-1.1.1/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 12:02:49.000000 tc-messageBroker-1.1.1/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.193578 tc-messageBroker-1.1.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:49.197578 tc-messageBroker-1.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-29 12:02:25.000000 tc-messageBroker-1.1.1/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.0/PKG-INFO` & `tc-messageBroker-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.0/README.md` & `tc-messageBroker-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/setup.py` & `tc-messageBroker-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.1.0",
+    version="1.1.1",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.1.1/tc_messageBroker/message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 )
 import jsonschema
 from jsonschema.exceptions import ValidationError
 import logging
 
 
 class MongoDB:
-    def __init__(
-        self, connection_str: str, db_name: str = "RnDAO", collection_name: str = "Saga"
-    ) -> None:
+    def __init__(self, connection_str: str, db_name: str, collection_name: str) -> None:
         """
         initialize the mongodb class
 
         Parameters:
         -------------
         connection_str : str
             the url to connect to mongo_db
```

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,39 @@
     ) -> None:
         self.uuid = sagaId if sagaId is not None else str(uuid.uuid1())
         self.choreography = choreography
         self.status = status
         self.data = data
         self.created_at = created_at
 
+    def start(
+        self,
+        publish_method: callable,
+        mongo_connection: str,
+        test_mode=False,
+    ):
+        """
+        just publish the first transaction
+        """
+        tx_sorted, _ = self._sort_transactions(self.choreography.transactions)
+        current_tx = tx_sorted[0]
+        self.status = Status.IN_PROGRESS
+
+        self._update_save(
+            transactions=tx_sorted,
+            mongo_connection=mongo_connection,
+            test=test_mode,
+        )
+
+        publish_method(
+            queue_name=current_tx.queue,
+            event=current_tx.event,
+            content={"uuid": self.uuid},
+        )
+
     def next(
         self,
         publish_method: callable,
         call_function: callable,
         mongo_connection: str,
         test_mode=False,
     ):
@@ -202,31 +227,37 @@
         data["sagaId"] = self.uuid
         data["createdAt"] = self.created_at
         data["updatedAt"] = datetime.now()
 
         return data
 
 
-def get_saga(guildId, connection_url):
+def get_saga(guildId: str, connection_url: str, db_name: str, collection: str):
     """
     get saga object for a special guild
 
     Parameters:
     ------------
     guildId : str
         the guildId which the saga belongs to
     connection_url : str
         the connection to db which the saga architecture is saved
+    db_name : str
+        the database name to use
+    collection : str
+        the collection which the saga is saved
 
     Returns:
     ----------
     saga_obj : Saga
         the saga object to use
     """
-    mongodb = MongoDB(connection_str=connection_url)
+    mongodb = MongoDB(
+        connection_str=connection_url, db_name=db_name, collection_name=collection
+    )
     mongodb.connect()
 
     data = mongodb.read(query={"data.guildId": guildId}, count=1)
 
     saga_obj = Saga(
         choreography=data["choreography"],
         status=data["status"],
```

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.1.1/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.1.1/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.0/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.1.1/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -31,11 +31,13 @@
 tests/integration/test_mongodb.py
 tests/integration/test_saga.py
 tests/unit/__init__.py
 tests/unit/test_choreagraphy_base.py
 tests/unit/test_enum_status.py
 tests/unit/test_event.py
 tests/unit/test_message_broker.py
+tests/unit/test_predefined_transactions.py
 tests/unit/test_queue.py
 tests/unit/test_saga_base.py
 tests/unit/test_saga_next.py
+tests/unit/test_saga_start.py
 tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.0/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.1.1/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tests/integration/test_mongodb.py` & `tc-messageBroker-1.1.1/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tests/integration/test_saga.py` & `tc-messageBroker-1.1.1/tests/integration/test_saga.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 @pytest.mark.skip(
     reason="Unable to test on GitHub Actions (no available MongoDB instance)"
 )
 def test_inputs():
     connection_url = "mongodb://127.0.0.1:27017/"
 
     ## we should have this data before running this test in db
-    saga = get_saga(guildId="993163081939165234", connection_url=connection_url)
+    saga = get_saga(
+        guildId="993163081939165234",
+        connection_url=connection_url,
+        db_name="Saga",
+        collection="saga",
+    )
 
     assert saga.choreography is not None
     assert saga.status in [
         Status.IN_PROGRESS,
         Status.CANCELLED,
         Status.FAILED,
         Status.NOT_STARTED,
```

### Comparing `tc-messageBroker-1.1.0/tests/unit/test_message_broker.py` & `tc-messageBroker-1.1.1/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tests/unit/test_saga_base.py` & `tc-messageBroker-1.1.1/tests/unit/test_saga_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     )
 
     ## it should sort the NOT_STARTED transactions
     (tx_sorted, not_started_count) = saga._sort_transactions(
         saga.choreography.transactions
     )
 
-    assert not_started_count == 3
+    assert not_started_count == 2
     order_val = 0
     for tx in tx_sorted:
         if tx.status == Status.NOT_STARTED:
             assert order_val < tx.order
             order_val = tx.order
 
 
@@ -41,15 +41,15 @@
     )
 
     ## it should sort the NOT_STARTED transactions
     (tx_sorted, not_started_count) = saga._sort_transactions(
         saga.choreography.transactions
     )
 
-    assert not_started_count == 3
+    assert not_started_count == 2
 
     condition = False
     for tx in tx_sorted:
         if tx.status == Status.NOT_STARTED:
             assert condition is False
         else:
             condition = True
```

### Comparing `tc-messageBroker-1.1.0/tests/unit/test_saga_next.py` & `tc-messageBroker-1.1.1/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.0/tests/unit/test_transactions.py` & `tc-messageBroker-1.1.1/tests/unit/test_transactions.py`

 * *Files identical despite different names*

