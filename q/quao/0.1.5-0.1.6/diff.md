# Comparing `tmp/quao-0.1.5.tar.gz` & `tmp/quao-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.5.tar", last modified: Wed May 24 09:50:35 2023, max compression
+gzip compressed data, was "quao-0.1.6.tar", last modified: Mon May 29 11:59:45 2023, max compression
```

## Comparing `quao-0.1.5.tar` & `quao-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.352017 quao-0.1.5/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-24 09:50:35.351014 quao-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.5/README.md
--rw-rw-rw-   0        0        0      846 2023-05-24 09:46:35.000000 quao-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 09:50:35.352017 quao-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.311018 quao-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.321024 quao-0.1.5/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.5/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.346016 quao-0.1.5/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.5/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.5/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     2207 2023-05-24 04:52:27.000000 quao-0.1.5/src/quao/backend.py
--rw-rw-rw-   0        0        0      366 2023-04-28 02:04:51.000000 quao-0.1.5/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.347015 quao-0.1.5/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.5/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.350015 quao-0.1.5/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.5/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     4996 2023-05-24 09:49:38.000000 quao-0.1.5/src/quao/sdk/qiskit.py
--rw-rw-rw-   0        0        0     1304 2023-05-24 05:04:40.000000 quao-0.1.5/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:50:35.343014 quao-0.1.5/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-24 09:50:35.000000 quao-0.1.5/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-24 09:50:35.000000 quao-0.1.5/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:50:35.000000 quao-0.1.5/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-24 09:50:35.000000 quao-0.1.5/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-24 09:50:35.000000 quao-0.1.5/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.621852 quao-0.1.6/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-29 11:59:45.620817 quao-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.6/README.md
+-rw-rw-rw-   0        0        0      846 2023-05-29 11:58:45.000000 quao-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:59:45.621852 quao-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.546545 quao-0.1.6/src/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.563876 quao-0.1.6/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.6/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.600693 quao-0.1.6/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.6/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-04-25 02:47:26.000000 quao-0.1.6/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     3523 2023-05-29 11:56:58.000000 quao-0.1.6/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.605694 quao-0.1.6/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.6/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      189 2023-05-29 11:56:58.000000 quao-0.1.6/src/quao/config/loggingConfig.py
+-rw-rw-rw-   0        0        0      175 2023-05-29 11:56:58.000000 quao-0.1.6/src/quao/config/threadConfig.py
+-rw-rw-rw-   0        0        0      529 2023-05-29 11:56:58.000000 quao-0.1.6/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.612908 quao-0.1.6/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-24 01:59:39.000000 quao-0.1.6/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.615843 quao-0.1.6/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.6/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     6402 2023-05-29 11:57:12.000000 quao-0.1.6/src/quao/sdk/qiskit.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.618817 quao-0.1.6/src/quao/status/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.6/src/quao/status/__init__.py
+-rw-rw-rw-   0        0        0     2450 2023-05-29 11:57:12.000000 quao-0.1.6/src/quao/status/qiskit_status.py
+-rw-rw-rw-   0        0        0     1636 2023-05-26 04:51:07.000000 quao-0.1.6/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:45.591699 quao-0.1.6/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-29 11:59:45.000000 quao-0.1.6/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-29 11:59:45.000000 quao-0.1.6/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:59:45.000000 quao-0.1.6/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-29 11:59:45.000000 quao-0.1.6/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-29 11:59:45.000000 quao-0.1.6/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.5/LICENSE` & `quao-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.5/PKG-INFO` & `quao-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.5
+Version: 0.1.6
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.5/README.md` & `quao-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.5/pyproject.toml` & `quao-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.5"
+version = "0.1.6"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.1.5/src/quao/algorithms/shor.py` & `quao-0.1.6/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.5/src/quao/backend.py` & `quao-0.1.6/src/quao/backend.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+"""
+    QuaO Project backend.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
+from .dataUtils import RequestData
+from .utilities import JobResponse
+from .config.threadConfig import pool
+from .config.loggingConfig import logging
 from json import JSONDecodeError, dumps
 
 import requests
-
-from .dataUtils import RequestData
-from .utilities import JobResponse
+import io
 
 
 class Backend:
     def __init__(self, request_data: RequestData, circuit):
+
         self.server_url = request_data.server_url
         self.sdk = request_data.sdk
         self.input = request_data.input
         self.shots = request_data.shots
         self.required_qubit = self.get_qubit_number(circuit)
         self.backend_request = self.generate_backend_request(request_data.device_id)
-        # Get backend data from server
         self.backend_data = self.get_backend_data()
+        self.circuit_export_url = request_data.circuit_export_url
+        pool.apply_async(self.__export_circuit, (circuit,))
 
     def get_qubit_number(self, circuit) -> int:
 
         if self.sdk == "qiskit":
             return int(circuit.num_qubits)
         return 0
 
@@ -42,26 +49,52 @@
                 backend_data = response.json().get("data")
             except JSONDecodeError:
                 return None
             return backend_data
         else:
             return None
 
-    def submit_job(self, circuit, interval: int = 3, timeout: int = 30) -> JobResponse:
+    def submit_job(self, circuit) -> JobResponse:
         job_response = JobResponse()
         shots = self.shots
-        if circuit and self.backend_data and 0 < interval <= timeout:
+        if circuit and self.backend_data:
             if self.sdk == "qiskit":
                 from .sdk.qiskit import QiskitFaaS
 
                 be_instance = QiskitFaaS(self.backend_data)
                 job_response = be_instance.submit_job(circuit, shots=shots)
             else:
                 job_response.job_status = "ERROR"
-                job_response.job_result = dumps({"error": "SDK not supported"})
+                job_response.job_result = {"error": "SDK not supported"}
         elif self.backend_data is None:
             job_response.job_status = "ERROR"
-            job_response.job_result = dumps({"error": "Backend not found"})
+            job_response.job_result = {"error": "Backend not found"}
 
         return job_response
 
+    @staticmethod
+    def __prepare_circuit_export_request(data: bytes) -> dict:
+        return {
+            'circuit': ('circuit_figure', data, 'multipart/form-data')
+        }
 
+    def __export_circuit(self, circuit):
+        """
+            Export circuit to svg file then send to QuaO server for saving
+            Args:
+                circuit: circuit will be exported
+        """
+
+        logging.info("Preparing circuit figure...")
+        circuit_figure = circuit.draw(output='mpl', fold=-1)
+
+        logging.info("Converting circuit figure to svg file...")
+        buffer = io.BytesIO()
+        circuit_figure.savefig(buffer, format='svg')
+
+        logging.info("Sending circuit svg image to [%s] with POST method ...", self.circuit_export_url)
+        response = requests.post(url=self.circuit_export_url,
+                                 files=self.__prepare_circuit_export_request(buffer.getvalue()))
+        if response.ok:
+            logging.info("Sending request successfully!")
+        else:
+            logging.info("Sending request failed with status %s!", response.status_code)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quao-0.1.5/src/quao.egg-info/PKG-INFO` & `quao-0.1.6/src/quao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.5
+Version: 0.1.6
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

