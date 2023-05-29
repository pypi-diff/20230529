# Comparing `tmp/superfluid-0.0.9.tar.gz` & `tmp/superfluid-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.9.tar", last modified: Tue May 23 16:33:53 2023, max compression
+gzip compressed data, was "superfluid-0.1.0.tar", last modified: Mon May 29 13:16:39 2023, max compression
```

## Comparing `superfluid-0.0.9.tar` & `superfluid-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.733557 superfluid-0.0.9/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.9/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:33:53.733386 superfluid-0.0.9/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.9/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.729408 superfluid-0.0.9/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.729958 superfluid-0.0.9/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      118 2023-05-23 16:22:23.000000 superfluid-0.0.9/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.732915 superfluid-0.0.9/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.9/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.9/main/superfluid/src/__types__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9372 2023-05-23 16:28:15.000000 superfluid-0.0.9/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.9/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.9/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1014 2023-05-23 16:28:39.000000 superfluid-0.0.9/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1701 2023-05-23 16:28:48.000000 superfluid-0.0.9/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      760 2023-05-23 16:28:53.000000 superfluid-0.0.9/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:33:53.731001 superfluid-0.0.9/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:33:53.000000 superfluid-0.0.9/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:33:53.733598 superfluid-0.0.9/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-23 16:33:20.000000 superfluid-0.0.9/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.536205 superfluid-0.1.0/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.1.0/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2778 2023-05-29 13:16:39.536013 superfluid-0.1.0/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2289 2023-05-29 13:15:16.000000 superfluid-0.1.0/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.527794 superfluid-0.1.0/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.528425 superfluid-0.1.0/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      166 2023-05-29 13:16:23.000000 superfluid-0.1.0/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.535045 superfluid-0.1.0/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.1.0/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)    21996 2023-05-29 12:34:47.000000 superfluid-0.1.0/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      770 2023-05-29 13:11:06.000000 superfluid-0.1.0/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      335 2023-05-29 08:52:33.000000 superfluid-0.1.0/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1022 2023-05-29 10:12:39.000000 superfluid-0.1.0/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1956 2023-05-29 10:02:53.000000 superfluid-0.1.0/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9946 2023-05-29 11:15:00.000000 superfluid-0.1.0/main/superfluid/src/types.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1513 2023-05-29 10:10:55.000000 superfluid-0.1.0/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.535599 superfluid-0.1.0/main/superfluid/test/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-26 06:50:05.000000 superfluid-0.1.0/main/superfluid/test/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5324 2023-05-29 09:57:23.000000 superfluid-0.1.0/main/superfluid/test/test_utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-29 13:16:39.533238 superfluid-0.1.0/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2778 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      561 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       53 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-29 13:16:39.000000 superfluid-0.1.0/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-29 13:16:39.536251 superfluid-0.1.0/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      848 2023-05-29 13:05:31.000000 superfluid-0.1.0/setup.py
```

### Comparing `superfluid-0.0.9/LICENSE.txt` & `superfluid-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.9/main/superfluid/src/host.py` & `superfluid-0.1.0/main/superfluid/src/host.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 
 from web3 import Web3
 from web3.contract.contract import ContractFunction
 from web3.middleware import geth_poa_middleware
 
 from .constants import HOST_ABI
 from .operation import Operation
-from .__types__ import BatchOperationType
+from .types import BatchOperationType
 
 
 class Host:
 
-    contract = None
-
     def __init__(self, rpc: str, host_address: str) -> None:
+        self.rpc = rpc
         web3 = Web3(Web3.HTTPProvider(rpc))
         web3.middleware_onion.inject(geth_poa_middleware, layer=0)
         self.contract = web3.eth.contract(
             address=host_address, abi=HOST_ABI)
 
     def call_agreement(self, agreement_address: str, calldata: str, user_data: str) -> Operation:
         try:
             agreement_call: ContractFunction = self.contract.functions.callAgreement(
                 agreement_address, calldata, user_data)
-            return Operation(agreement_call, BatchOperationType.SUPERFLUID_CALL_AGREEMENT)
+            return Operation(self.rpc, agreement_call, BatchOperationType.SUPERFLUID_CALL_AGREEMENT)
         except Exception as e:
             raise e
 
     def call_app_action() -> Operation:
         pass
```

### Comparing `superfluid-0.0.9/main/superfluid/src/operation.py` & `superfluid-0.1.0/main/superfluid/src/operation.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,42 +2,50 @@
 
 from web3.types import TxParams
 from web3.contract.contract import ContractFunction
 from web3 import Web3
 from eth_typing import HexStr
 from eth_account import Account
 
-from .__types__ import BatchOperationType
+from .types import BatchOperationType
 
 
 class Operation:
 
-    agreement_call: ContractFunction = None
-    type: BatchOperationType = None
-    forwarder_txn: TxParams = None
-
-    def __init__(self, agreement_call: ContractFunction, type: BatchOperationType, forwarder_txn: Optional[TxParams] = None) -> None:
+    def __init__(self, rpc: str, agreement_call: ContractFunction, type: BatchOperationType, forwarder_call: Optional[ContractFunction] = None) -> None:
+        self.rpc = rpc
         self.agreement_call = agreement_call
         self.type = type
-        self.forwarder_txn = forwarder_txn
+        self.forwarder_call = forwarder_call
 
-    def exec(self, rpc: str, private_key: str) -> HexStr:
+    def exec(self, private_key: str) -> HexStr:
+        """
+            Signs and broadcasts a transaction
+            @param rpc - rpc url
+            @param private_key - private key
+            @returns - HexStr - The transaction hash
+        """
         populated_transaction = self._get_populated_transaction_request(
-            rpc, private_key)
-        web3 = Web3(Web3.HTTPProvider(rpc))
+            self.rpc, private_key)
+        web3 = Web3(Web3.HTTPProvider(self.rpc))
         signed_txn = web3.eth.account.sign_transaction(
             populated_transaction, private_key=private_key)
         transaction_hash = web3.eth.send_raw_transaction(
             signed_txn.rawTransaction)
         return transaction_hash.hex()
 
     def _get_populated_transaction_request(self, rpc: str, private_key: str) -> TxParams:
-        populated_transaction = self.forwarder_txn if self.forwarder_txn is not None else self.agreement_call
+        """
+            Selects and prepares the transaction object to be signed
+            @param rpc - rpc url
+            @param private_key - private key
+            @returns - TxParams - The transaction object
+        """
+        call = self.forwarder_call if self.forwarder_call is not None else self.agreement_call
         address = Account.from_key(private_key).address
-        if populated_transaction == self.agreement_call:
-            populated_transaction = self.agreement_call.build_transaction({
-                "from": address
-            })
+        populated_transaction = call.build_transaction({
+            "from": address
+        })
         web3 = Web3(Web3.HTTPProvider(rpc))
         nonce = web3.eth.get_transaction_count(address)
         populated_transaction["nonce"] = nonce
         return populated_transaction
```

### Comparing `superfluid-0.0.9/setup.py` & `superfluid-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.9",
+    version="0.1.0",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

