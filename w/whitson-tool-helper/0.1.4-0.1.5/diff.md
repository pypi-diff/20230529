# Comparing `tmp/whitson_tool_helper-0.1.4.tar.gz` & `tmp/whitson_tool_helper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.1.4.tar", last modified: Tue May 23 14:40:52 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.1.5.tar", last modified: Mon May 29 07:43:00 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.4.tar` & `whitson_tool_helper-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-05-23 14:40:47.000000 whitson_tool_helper-0.1.4/pyproject.toml
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/setup.cfg
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/__init__.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/logger.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/helper.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-05-02 09:42:15.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/main.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4385 2023-05-23 14:38:25.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/pubsub.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3728 2023-05-23 14:38:30.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/timeout.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper/whitson_exceptions.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-23 14:40:52.899701 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      575 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/requires.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-05-23 14:40:52.000000 whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-05-29 07:42:55.000000 whitson_tool_helper-0.1.5/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/src/whitson_tool_helper/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/logger.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/helper.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2729 2023-05-29 07:32:28.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/main.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3736 2023-05-29 07:22:46.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/pubsub.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3648 2023-05-29 07:34:29.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/timeout.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper/whitson_exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-29 07:43:00.721505 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-05-29 07:43:00.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-05-29 07:43:00.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-05-29 07:43:00.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-05-29 07:43:00.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-05-29 07:43:00.000000 whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.1.4/pyproject.toml` & `whitson_tool_helper-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.1.4"
+version =  "0.1.5"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,9 +68,9 @@
             self._consumer = rabbitmq.RabbitMQPublisher(exchange)
         else:
             raise MessagingSystemNotSupportedError(messaging_system)
 
     def publish(self, topic: str, payload: dict, meta_data: dict = {}, **kwargs: dict):
         self._consumer.publish(topic, payload, meta_data, **kwargs)
 
-    def publish_many(self, payloads: List[dict], meta_data: dict, **kwargs: dict):
-        self._consumer.publish_many(payloads, meta_data, **kwargs)
+    def publish_many(self, topic: str, payloads: List[dict], **kwargs: dict):
+        self._consumer.publish_many(topic, payloads, **kwargs)
```

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os
 from google.cloud import pubsub_v1
 import google.api_core.exceptions
-import logging
 import json
 import traceback
 from typing import List
-import time
-from concurrent import futures
 
 from whitson_tool_helper.messaging.helper import check_environment_variables
 from whitson_tool_helper.logger import LOGGER
 
 
 class PubsubConsumer:
     def __init__(self, process_func, to_dict=False):
@@ -78,47 +75,33 @@
         self.project_id = os.environ["GOOGLE_PROJECT"]
         self.futures = set()
 
     @property
     def topic_name(self):
         return f"projects/{self.project_id}/topics/{self.topic}"
 
-    def get_callback(self, f, data):
-        def callback(f):
-            try:
-                logging.debug(f.result())
-                self.futures.remove(f)
-            except:  # noqa
-                logging.error("Please handle {} for {}.".format(f.exception(), data))
-
-        return callback
+    def callback(future: pubsub_v1.publisher.futures.Future) -> None:
+        future.result()
 
     def publish(
         self,
         topic: str,
         payload: dict,
         meta_data: dict = {},
         encode_json=True,
         **kwargs,
     ):
         LOGGER.debug("Publishing single to pubsub")
         self.topic = topic
         payload = json.dumps(payload).encode("utf8") if encode_json else payload
         future = self.publisher.publish(self.topic_name, payload, **meta_data)
-        self.futures.add(future)
-        # Publish failures shall be handled in the callback function.
-        future.add_done_callback(self.get_callback(future, payload))
-        # Wait for all the publish futures to resolve before exiting.
-        while self.futures:
-            time.sleep(1)
+        future.result()
 
-    def publish_many(self, payloads: List[dict], meta_data: dict = {}):
+    def publish_many(self, topic, payloads: List[dict]):
         LOGGER.debug("Publishing many to pubsub")
-        publish_futures = []
+        self.topic = topic
 
         for payload in payloads:
-            data = json.dumps(payload).encode("utf-8")
-            publish_future = self.publisher.publish(self.topic, data, **meta_data)
-            publish_future.add_done_callback(self.get_callback)
-            publish_futures.append(publish_future)
-
-        futures.wait(publish_futures, return_when=futures.ALL_COMPLETED)
+            data = json.dumps(payload.get("data")).encode("utf-8")
+            meta_data = payload.get("meta_data") or {}
+            future = self.publisher.publish(self.topic_name, data, **meta_data)
+            future.result()
```

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,24 +90,22 @@
                 delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE,
                 priority=priority,
             ),
         )
 
         connection.close()
 
-    def publish_many(self, payloads: List[dict], meta_data: dict, priority: int = 50):
+    def publish_many(self, topic, payloads: List[dict], priority: int = 50):
         connection = pika.BlockingConnection(self.parameters)
         channel = connection.channel()
 
-        for payload in payloads:
-            message = {"data": payload, "meta_data": meta_data}
-
+        for message in payloads:
             channel.basic_publish(
                 exchange="engines",
-                routing_key=self.topic,
+                routing_key=topic,
                 body=json.dumps(message).encode("utf-8"),
                 properties=pika.BasicProperties(
                     delivery_mode=pika.spec.PERSISTENT_DELIVERY_MODE,
                     priority=priority,
                 ),
             )
```

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.4/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.5/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

