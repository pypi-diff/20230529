# Comparing `tmp/boltz_client-0.1.7.tar.gz` & `tmp/boltz_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boltz_client-0.1.7.tar", max compression
+gzip compressed data, was "boltz_client-0.1.8.tar", max compression
```

## Comparing `boltz_client-0.1.7.tar` & `boltz_client-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      283 2023-05-27 15:07:14.934714 boltz_client-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/__init__.py
--rw-r--r--   0        0        0     7017 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/boltz.py
--rw-r--r--   0        0        0     6547 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/cli.py
--rw-r--r--   0        0        0      375 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/helpers.py
--rw-r--r--   0        0        0     5343 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/mempool.py
--rw-r--r--   0        0        0     3066 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/onchain.py
--rw-r--r--   0        0        0        0 2023-05-27 15:07:14.934714 boltz_client-0.1.7/boltz_client/py.typed
--rw-r--r--   0        0        0     1160 2023-05-27 15:07:14.938714 boltz_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 boltz_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-29 19:24:11.439351 boltz_client-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/__init__.py
+-rw-r--r--   0        0        0     7456 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/boltz.py
+-rw-r--r--   0        0        0     6547 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/cli.py
+-rw-r--r--   0        0        0      375 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/helpers.py
+-rw-r--r--   0        0        0     5036 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/mempool.py
+-rw-r--r--   0        0        0     3066 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/onchain.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:24:11.439351 boltz_client-0.1.8/boltz_client/py.typed
+-rw-r--r--   0        0        0     1160 2023-05-29 19:24:11.443351 boltz_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 boltz_client-0.1.8/PKG-INFO
```

### Comparing `boltz_client-0.1.7/boltz_client/boltz.py` & `boltz_client-0.1.8/boltz_client/boltz.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,21 @@
     def check_version(self):
         return self.request(
             "get",
             f"{self._cfg.api_url}/version",
             headers={"Content-Type": "application/json"},
         )
 
+    def get_fee_estimation(self, feerate: Optional[int]) -> int:
+        # TODO: hardcoded maximum tx size, in the future we try to get the size of the tx via embit
+        # we need a function like Transaction.vsize()
+        tx_size_vbyte = 200
+        mempool_fees = feerate if feerate else self.mempool.get_fees()
+        return mempool_fees * tx_size_vbyte
+
     def set_limits(self) -> None:
         data = self.request(
             "get",
             f"{self._cfg.api_url}/getpairs",
             headers={"Content-Type": "application/json"},
         )
         pair = data["pairs"]["BTC/BTC"]
@@ -131,49 +138,51 @@
         self,
         lockup_address: str,
         receive_address: str,
         privkey_wif: str,
         preimage_hex: str,
         redeem_script_hex: str,
         zeroconf: bool = False,
+        feerate: Optional[int] = None,
     ):
         lockup_tx = await self.mempool.get_tx_from_address(lockup_address)
 
         if not zeroconf and lockup_tx.status != "confirmed":
             await self.mempool.wait_for_tx_confirmed(lockup_tx.txid)
 
         txid, transaction = create_claim_tx(
             lockup_tx=lockup_tx,
             receive_address=receive_address,
             privkey_wif=privkey_wif,
             redeem_script_hex=redeem_script_hex,
             preimage_hex=preimage_hex,
-            fees=self.mempool.get_fee_estimation(),
+            fees=self.get_fee_estimation(feerate),
         )
 
         self.mempool.send_onchain_tx(transaction)
         return txid
 
     async def refund_swap(
         self,
         privkey_wif: str,
         lockup_address: str,
         receive_address: str,
         redeem_script_hex: str,
         timeout_block_height: int,
+        feerate: Optional[int] = None,
     ) -> str:
         self.mempool.check_block_height(timeout_block_height)
         lockup_tx = await self.mempool.get_tx_from_address(lockup_address)
         txid, transaction = create_refund_tx(
             lockup_tx=lockup_tx,
             privkey_wif=privkey_wif,
             receive_address=receive_address,
             redeem_script_hex=redeem_script_hex,
             timeout_block_height=timeout_block_height,
-            fees=self.mempool.get_fee_estimation(),
+            fees=self.get_fee_estimation(feerate),
         )
 
         self.mempool.send_onchain_tx(transaction)
         return txid
 
     def create_swap(self, payment_request: str) -> tuple[str, BoltzSwapResponse]:
         """create swap and return private key and boltz response"""
```

### Comparing `boltz_client-0.1.7/boltz_client/cli.py` & `boltz_client-0.1.8/boltz_client/cli.py`

 * *Files identical despite different names*

### Comparing `boltz_client-0.1.7/boltz_client/mempool.py` & `boltz_client-0.1.8/boltz_client/mempool.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,21 +109,14 @@
         if len(txs) == 0:
             return await self.wait_for_lockup_tx(address)
         lockup_tx = self.find_tx_and_output(txs, address)
         if not lockup_tx:
             return await self.wait_for_lockup_tx(address)
         return lockup_tx
 
-    def get_fee_estimation(self) -> int:
-        # TODO: hardcoded maximum tx size, in the future we try to get the size of the tx via embit
-        # we need a function like Transaction.vsize()
-        tx_size_vbyte = 200
-        mempool_fees = self.get_fees()
-        return mempool_fees * tx_size_vbyte
-
     def get_fees(self) -> int:
         data = self.request(
             "get",
             f"{self._api_url}/v1/fees/recommended",
             headers={"Content-Type": "application/json"},
         )
         return int(data["halfHourFee"])
```

### Comparing `boltz_client-0.1.7/boltz_client/onchain.py` & `boltz_client-0.1.8/boltz_client/onchain.py`

 * *Files identical despite different names*

### Comparing `boltz_client-0.1.7/pyproject.toml` & `boltz_client-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boltz_client"
-version = "0.1.7"
+version = "0.1.8"
 description = "python boltz client"
 license = "MIT"
 authors = ["dni <office@dnilabs.com>"]
 readme = "README.md"
 repository = "https://github.com/dni/boltz-client-python"
 homepage = "https://boltz.exchange"
 packages = [
```

### Comparing `boltz_client-0.1.7/PKG-INFO` & `boltz_client-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boltz-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: python boltz client
 Home-page: https://boltz.exchange
 License: MIT
 Author: dni
 Author-email: office@dnilabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

