# Comparing `tmp/overwatch_client-0.1.3.tar.gz` & `tmp/overwatch_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overwatch_client-0.1.3.tar", max compression
+gzip compressed data, was "overwatch_client-0.1.4.tar", max compression
```

## Comparing `overwatch_client-0.1.3.tar` & `overwatch_client-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1209 2023-05-16 18:44:30.690073 overwatch_client-0.1.3/README.md
--rw-r--r--   0        0        0       32 2023-05-09 14:55:50.728909 overwatch_client-0.1.3/overwatch_client/__init__.py
--rw-r--r--   0        0        0    12657 2023-05-26 14:59:05.617457 overwatch_client-0.1.3/overwatch_client/client.py
--rw-r--r--   0        0        0      378 2023-05-26 14:59:05.621457 overwatch_client-0.1.3/overwatch_client/utils.py
--rw-r--r--   0        0        0     1044 2023-05-26 14:59:05.621457 overwatch_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 overwatch_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1209 2023-05-16 18:56:32.882104 overwatch_client-0.1.4/README.md
+-rw-r--r--   0        0        0       32 2023-05-02 14:37:02.200028 overwatch_client-0.1.4/overwatch_client/__init__.py
+-rw-r--r--   0        0        0    15570 2023-05-29 15:58:51.403165 overwatch_client-0.1.4/overwatch_client/client.py
+-rw-r--r--   0        0        0      378 2023-05-29 15:58:51.403165 overwatch_client-0.1.4/overwatch_client/utils.py
+-rw-r--r--   0        0        0     1044 2023-05-29 18:01:27.109472 overwatch_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 overwatch_client-0.1.4/PKG-INFO
```

### Comparing `overwatch_client-0.1.3/README.md` & `overwatch_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `overwatch_client-0.1.3/overwatch_client/client.py` & `overwatch_client-0.1.4/overwatch_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os, sys
 import requests
 import time
 from typing import Optional, Sequence, Dict, Union
 from .utils import generate_uuid
+import asyncio
 
 
 class HTTPClient:
     """The base client for communicating with an overwatch server and it's model registry.
 
     The client is used to register, patch, delete and infer on models with the overwatch server.
 
@@ -315,14 +316,98 @@
 
         Args:
             inputs(Sequence[bytes]): A list of inputs in byte format.
             model_name(str): The model name we will be inferencing on.
             slice_batch(int): The number of inputs to run per slice.
             inference_id(Optional[str]): A special ID for this inference instance (Optional).
             compute_group_info(Optional[str]): Compute group information in the form of "<joinKey>/<joinSecret>".
+
+        Returns:
+            Dict: The inference results as a dictionary.
+        """
+        inference_id = (
+            inference_id
+            if inference_id is not None
+            else f"{model_name}_{generate_uuid()}"
+        )
+        url = f"{self.ow_server_url}/Prediction/{inference_id}/detect/iterations/{model_name}/{slice_batch}"
+        if compute_group_info is not None:
+            url = f"{url}/{compute_group_info}"
+        
+        files = {}
+        if type(inputs) is dict:
+            files = inputs
+            for key in files:
+                assert type(files[key]) is bytes, f"Inputs must be bytes but got {type(files[key])} for key {key}"
+        elif type(inputs) is list:
+            for ind, elem in enumerate(inputs):
+                assert type(elem) is bytes, f"Inputs must be bytes but got {type(elem)} for index {ind}"
+                files[f"{ind}"] = elem
+        else:
+            raise TypeError("inputs must be a list or dict")
+
+        start_time = time.time()
+        
+        if self._password is None and self._email is None:
+            response = self.request_session.post(
+                url,
+                files=files,
+            )
+        else:
+            response = self.request_session.post(
+                url,
+                data={
+                    "email": self._email,
+                    "password": self._password
+                },
+                files = files,
+            )
+
+
+        response.raise_for_status()
+
+        end_time = time.time()
+
+        self.inference_timer.append(end_time - start_time)
+        self.inference_counter.append(len(inputs))
+
+        return response.json()
+
+    async def infer_async(
+        self,
+        inputs: Union[Dict, Sequence[bytes]],
+        model_name: str,
+        slice_batch: int = 1,
+        inference_id: Optional[str] = None,
+        compute_group_info: Optional[str] = None,
+    ) -> Dict:
+        """
+        Performs an asynchronous inference on the provided inputs using the model specified. Returns 
+        the inference results as a dictionary.
+
+        To use asynchronous API, please make sure to use asyncio to create task:
+            ```python
+            import asyncio
+
+
+            def callback(task):
+                results = task.result()
+
+            loop = asyncio.get_event_loop()               
+            task = loop.create_task(client.infer_async(...))
+            task.add_done_callback(callback)
+
+            ``` 
+
+        Args:
+            inputs(Sequence[bytes]): A list of inputs in byte format.
+            model_name(str): The model name we will be inferencing on.
+            slice_batch(int): The number of inputs to run per slice.
+            inference_id(Optional[str]): A special ID for this inference instance (Optional).
+            compute_group_info(Optional[str]): Compute group information in the form of "<joinKey>/<joinSecret>".
 
         Returns:
             Dict: The inference results as a dictionary.
         """
         inference_id = (
             inference_id
             if inference_id is not None
```

### Comparing `overwatch_client-0.1.3/pyproject.toml` & `overwatch_client-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overwatch-client"
-version = "0.1.3"
+version = "0.1.4"
 description = "A python based Overwatch Client for interacting with the overwatch server with higher level apis."
 authors = ["Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [{include = "overwatch_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `overwatch_client-0.1.3/PKG-INFO` & `overwatch_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overwatch-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python based Overwatch Client for interacting with the overwatch server with higher level apis.
 Author: Hamada Gasmallah
 Author-email: hamada@distributive.network
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

