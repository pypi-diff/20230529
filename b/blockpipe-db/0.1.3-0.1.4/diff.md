# Comparing `tmp/blockpipe_db-0.1.3.tar.gz` & `tmp/blockpipe_db-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.3.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.4.tar", max compression
```

## Comparing `blockpipe_db-0.1.3.tar` & `blockpipe_db-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.3/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.3/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-29 02:55:06.045479 blockpipe_db-0.1.3/blockpipe_db/client.py
--rw-r--r--   0        0        0      393 2023-05-29 02:56:48.820379 blockpipe_db-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.4/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.4/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-29 07:59:30.024936 blockpipe_db-0.1.4/blockpipe_db/client.py
+-rw-r--r--   0        0        0      393 2023-05-29 07:59:42.608662 blockpipe_db-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.4/PKG-INFO
```

### Comparing `blockpipe_db-0.1.3/blockpipe_db/client.py` & `blockpipe_db-0.1.4/blockpipe_db/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, host: str = _DEFAULT_HOST):
         context = zmq.Context()
         self.socket = context.socket(zmq.PAIR)
         self.socket.setsockopt(zmq.SNDHWM, 10000)
         self.socket.setsockopt(zmq.RCVHWM, 10000)
         self.socket.connect(host)
 
-    def load_event_df(self, address: str | bytes, topic0: str | bytes, limit: int = 100):
+    def load_event_df(self, address: str, topic0: str, limit: int = 100):
         query = Query(HexBytes(address), HexBytes(topic0), limit)
         self.socket.send(query.to_bytes())
         data = []
         while True:
             if (e := self.socket.recv()) == b'':
                 break
             data.append(msgpack.unpackb(e))
```

### Comparing `blockpipe_db-0.1.3/PKG-INFO` & `blockpipe_db-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-db
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

