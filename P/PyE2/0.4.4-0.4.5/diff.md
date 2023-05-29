# Comparing `tmp/pye2-0.4.4.tar.gz` & `tmp/pye2-0.4.5.tar.gz`

## Comparing `pye2-0.4.4.tar` & `pye2-0.4.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.4/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.4/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.4/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.4/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/__init__.py
--rw-r--r--   0        0        0    22854 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/logger.py
--rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/default/__init__.py
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.4/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/.example_env
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/attach_example.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/ex1.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/hello.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/remote_exec.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.4/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.4/LICENSE
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.4/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.5/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.5/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.5/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.5/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.5/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/.example_env
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/ex1.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/hello.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/remote_exec.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.5/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.4.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.5/LICENSE
+-rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 pye2-0.4.5/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0    12637 2020-02-02 00:00:00.000000 pye2-0.4.5/PKG-INFO
```

### Comparing `pye2-0.4.4/.github/workflows/python-publish.yml` & `pye2-0.4.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/base/__init__.py` & `pye2-0.4.5/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/base/generic_session.py` & `pye2-0.4.5/PyE2/base/generic_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 
 @copyright: Lummetry.AI
 @author: Lummetry\.AI - Stefan Saraev
 @project: 
 @description:
 """
 
+import json
 from time import sleep
 from time import time as tm
 
+from ..utils.code import CodeUtils
+
 from ..const import comms as comm_ct
 from ..io_formatter import IOFormatterManager
 from .logger import Logger
 from .payload import Payload
 from .pipeline import Pipeline
 
 
@@ -175,15 +178,23 @@
   def _track_online_node(self, e2id):
     self._last_seen_boxes[e2id] = tm()
     return
 
   def _on_heartbeat_default(self, dict_msg: dict):
     # extract relevant data from the message
     msg_eeid = dict_msg['EE_ID']
-    msg_active_configs = dict_msg['CONFIG_STREAMS']
+
+    if dict_msg.get("HEARTBEAT_VERSION") == "v2":
+      str_data = CodeUtils().decompress_text(dict_msg["ENCODED_DATA"])
+      data = json.loads(str_data)
+      dict_msg = {**dict_msg, **data}
+
+    msg_active_configs = dict_msg.get('CONFIG_STREAMS')
+    if msg_active_configs is None:
+      return
 
     # default action
     self._track_online_node(msg_eeid)
     self._online_boxes[msg_eeid] = {
         config['NAME']: config for config in msg_active_configs}
 
     if self._maybe_ignore_message(msg_eeid):
```

### Comparing `pye2-0.4.4/PyE2/base/logger.py` & `pye2-0.4.5/PyE2/base/logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/base/pipeline.py` & `pye2-0.4.5/PyE2/base/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @copyright: Lummetry.AI
 @author: Lummetry\.AI - Stefan Saraev
 @project: 
 @description:
 """
 from time import time
 from .payload import Payload
-from ..utils.code_exec import code_to_base64
+from ..utils.code import CodeUtils
 
 
 WAIT_FOR_WORKER = 15
 
 
 class Pipeline(object):
   """
@@ -342,30 +342,30 @@
           self.P(data, color='r')
         exec_error = data['specificValue']['exec_errors']
 
       if exec_error is not None:
         self.P("Error received from <CUSTOM_EXEC_01:{}>: {}".format(
             instance_id, exec_error), color="r")
       if exec_data is not None:
-        on_data(self, Payload(exec_data))
+        on_data(self, exec_data)
       return
 
     if plain_code is None and plain_code_path is None:
       raise Exception(
           "Need to specify at least one of the following: plain_code, plain_code_path")
 
     if plain_code is not None and plain_code_path is not None:
       raise Exception(
           "Need to specify at most one of the following: plain_code, plain_code_path")
 
     if plain_code is None:
       with open(plain_code_path, "r") as fd:
         plain_code = "".join(fd.readlines())
 
-    b64code = code_to_base64(plain_code)
+    b64code = CodeUtils().code_to_base64(plain_code)
     return self.start_plugin_instance(
         signature='CUSTOM_EXEC_01',
         instance_id=instance_id,
         params={
             'CODE': b64code,
             **params
         },
@@ -434,15 +434,15 @@
 
       if 'rest_execution_result' in data['specificValue'] and 'rest_execution_error' in data['specificValue']:
         result = data['specificValue']['rest_execution_result']
         error = data['specificValue']['rest_execution_error']
         finished = True
       return
 
-    b64code = code_to_base64(plain_code)
+    b64code = CodeUtils().code_to_base64(plain_code)
     instance_id = self.name + "_rest_custom_exec_synchronous_0"
     params = {
         'REQUEST': {
             'DATA': {
                 'CODE': b64code,
             },
             'TIMESTAMP': self.log.time_to_str()
```

### Comparing `pye2-0.4.4/PyE2/base/payload/payload.py` & `pye2-0.4.5/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/comm/__init__.py` & `pye2-0.4.5/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/comm/amqp_wrapper.py` & `pye2-0.4.5/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/comm/mqtt_wrapper.py` & `pye2-0.4.5/PyE2/comm/mqtt_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,19 @@
   def _callback_on_publish(self, client, userdata, mid):
     return
 
   def _callback_on_message(self, client, userdata, message):
     if self._custom_on_message is not None:
       self._custom_on_message(client, userdata, message)
     else:
-      msg = message.payload.decode('utf-8')
-      self._recv_buff.append(msg)
+      try:
+        msg = message.payload.decode('utf-8')
+        self._recv_buff.append(msg)
+      except Exception as e:
+        self.P(e)
     # now call the "post-process" callback
     if self._post_default_on_message is not None:
       self._post_default_on_message()
     return
 
   def get_connection_issues(self):
     return self._disconnected_log
@@ -245,15 +248,15 @@
         # TODO: more verbose logging including when there is no actual exception
         self._mqttc.connect(host=self.cfg_host, port=self.cfg_port)
 
         self._mqttc.loop_start()  # start loop in another thread
 
         sleep_time = 0.01
         max_sleep = 2
-        for sleep_iter in range(1, int(max_sleep/sleep_time) + 1):
+        for sleep_iter in range(1, int(max_sleep / sleep_time) + 1):
           sleep(sleep_time)
           if self.connected:
             break
         # endfor
 
         has_connection = self.connected
       except Exception as e:
```

### Comparing `pye2-0.4.4/PyE2/const/__init__.py` & `pye2-0.4.5/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/const/base.py` & `pye2-0.4.5/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/const/comms.py` & `pye2-0.4.5/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/const/heartbeat.py` & `pye2-0.4.5/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/const/misc.py` & `pye2-0.4.5/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/const/payload.py` & `pye2-0.4.5/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/default/mqtt_session.py` & `pye2-0.4.5/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/__init__.py` & `pye2-0.4.5/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/consts.py` & `pye2-0.4.5/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.4.5/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/base/__init__.py` & `pye2-0.4.5/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.4.5/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/default/__init__.py` & `pye2-0.4.5/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.4.5/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/default/cavi2.py` & `pye2-0.4.5/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.4.5/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/PyE2/utils/code.py` & `pye2-0.4.5/PyE2/utils/code_exec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 # -*- coding: utf-8 -*-
 """
-Copyright (C) 2017-2021 Andrei Damian, andrei.damian@me.com,  All rights reserved.
+Copyright 2019-2022 Lummetry.AI (Knowledge Investment Group SRL). All Rights Reserved.
 
-This software and its associated documentation are the exclusive property of the creator. 
-Unauthorized use, copying, or distribution of this software, or any portion thereof, 
-is strictly prohibited.
-
-Parts of this software are licensed and used in software developed by Knowledge Investment Group SRL.
-Any software proprietary to Knowledge Investment Group SRL is covered by Romanian and  Foreign Patents, 
-patents in process, and are protected by trade secret or copyright law.
-
-Dissemination of this information or reproduction of this material is strictly forbidden unless prior 
-written permission from the author.
 
+* NOTICE:  All information contained herein is, and remains
+* the property of Knowledge Investment Group SRL.  
+* The intellectual and technical concepts contained
+* herein are proprietary to Knowledge Investment Group SRL
+* and may be covered by Romanian and Foreign Patents,
+* patents in process, and are protected by trade secret or copyright law.
+* Dissemination of this information or reproduction of this material
+* is strictly forbidden unless prior written permission is obtained
+* from Knowledge Investment Group SRL.
+
+
+@copyright: Lummetry.AI
+@author: Lummetry.AI - AID
+@project: 
+@description:
+Created on Thu Jan 26 16:53:55 2023
 """
 
-import base64
-import sys
 import zlib
+import sys
+import base64
 
 
-class CodeUtils:
-  """
-  This class should be used either as a associated object for code checking or
-  as a mixin for running code
-  """
-
-  def __init__(self):
-    super(CodeUtils, self).__init__()
-    return
-
-  def __msg(self, m, color='d'):
-    if hasattr(self, 'P'):
-      self.P(m, color=color)
-    elif hasattr(self, 'log'):
-      self.log.P(m, color=color)
-    else:
-      print(m)
-    return
-
-  def code_to_base64(self, code, verbose=True, compress=True):
-    if verbose:
-      self.__msg("Processing:\n{}".format(code), color='y')
-    l_i = len(code)
-    l_c = -1
-    b_code = bytes(code, 'utf-8')
-    if compress:
-      b_code = zlib.compress(b_code, level=9)
-      l_c = sys.getsizeof(b_code)
-    b_encoded = base64.b64encode(b_code)
-    str_encoded = b_encoded.decode('utf-8')
-    l_b64 = len(str_encoded)
-    self.__msg("Code checking and serialization suceeded. Initial/Compress/B64: {}/{}/{}".format(
+def code_to_base64(plain_code, verbose=False, compress=True, code_checker_callback=None):
+  if verbose:
+    print("Processing:\n{}".format(plain_code), color='y')
+  errors = None
+  if code_checker_callback is not None:
+    errors = code_checker_callback(plain_code)
+  if errors is not None:
+    print("Cannot serialize code due to: '{}'".format(errors), color='r')
+    return None
+  l_i = len(plain_code)
+  l_c = -1
+  b_code = bytes(plain_code, 'utf-8')
+  if compress:
+    b_code = zlib.compress(b_code, level=9)
+    l_c = sys.getsizeof(b_code)
+  b_encoded = base64.b64encode(b_code)
+  str_encoded = b_encoded.decode('utf-8')
+  l_b64 = len(str_encoded)
+  if verbose:
+    print("Code checking and serialization suceeded. Initial/Compress/B64: {}/{}/{}".format(
         l_i, l_c, l_b64), color='g'
     )
-    return str_encoded
+  return str_encoded
```

### Comparing `pye2-0.4.4/xperimental/attach_example.py` & `pye2-0.4.5/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/ex1.py` & `pye2-0.4.5/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/hello.py` & `pye2-0.4.5/xperimental/hello.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/remote_exec.py` & `pye2-0.4.5/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/save_images.py` & `pye2-0.4.5/xperimental/save_images.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/decentralized/dedist_example.py` & `pye2-0.4.5/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.4.5/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/.gitignore` & `pye2-0.4.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -169,8 +169,10 @@
 *.torchscript
 
 *.pt
 
 *.ths
 
 .vscode
-.pypirc
+.pypirc
+
+personal
```

### Comparing `pye2-0.4.4/LICENSE` & `pye2-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.4.4/README.md` & `pye2-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -335,14 +335,19 @@
   sess.run(wait=60)
 ```
 
 </details>
 
 ## Change log
 
+### v0.4.5
+
+- Feature(heartbeats): support compressed heartbeat
+- Feature(Session): add optional callback for `on_payload` in Session
+
 ### v0.4.1
 
 - Documentation(README): updated this README with examples
 - Refactor(examples): updated all examples to match changes from `v0.3.6`
 
 ### v0.4.0
```

### Comparing `pye2-0.4.4/pyproject.toml` & `pye2-0.4.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt", "Pillow", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

### Comparing `pye2-0.4.4/PKG-INFO` & `pye2-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyE2
-Version: 0.4.4
+Version: 0.4.5
 Summary: PyE2 is an SDK used to communicate with the AiXpand network
 Project-URL: Homepage, https://github.com/AiXpand/PyE2
 Project-URL: Bug Tracker, https://github.com/AiXpand/PyE2/issues
 Author-email: Stefan Saraev <stefan.saraev@global-technical.com>, Cristan Bleotiu <cristan.bleotiu@global-technical.com>, Andrei Ionut Damian <andrei.damian@lummetry.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -349,14 +349,19 @@
   sess.run(wait=60)
 ```
 
 </details>
 
 ## Change log
 
+### v0.4.5
+
+- Feature(heartbeats): support compressed heartbeat
+- Feature(Session): add optional callback for `on_payload` in Session
+
 ### v0.4.1
 
 - Documentation(README): updated this README with examples
 - Refactor(examples): updated all examples to match changes from `v0.3.6`
 
 ### v0.4.0
```

