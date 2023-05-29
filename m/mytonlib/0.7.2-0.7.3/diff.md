# Comparing `tmp/mytonlib-0.7.2.tar.gz` & `tmp/mytonlib-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytonlib-0.7.2.tar", last modified: Sun Feb 26 16:42:56 2023, max compression
+gzip compressed data, was "mytonlib-0.7.3.tar", last modified: Mon May 29 08:58:38 2023, max compression
```

## Comparing `mytonlib-0.7.2.tar` & `mytonlib-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-02-26 16:42:56.812825 mytonlib-0.7.2/
--rw-r--r--   0 ton       (1000) ton       (1000)    35823 2022-08-08 10:10:01.000000 mytonlib-0.7.2/LICENSE
--rw-r--r--   0 ton       (1000) ton       (1000)       62 2023-02-19 09:41:29.000000 mytonlib-0.7.2/MANIFEST.in
--rw-r--r--   0 ton       (1000) ton       (1000)     2992 2023-02-26 16:42:56.812825 mytonlib-0.7.2/PKG-INFO
--rw-r--r--   0 ton       (1000) ton       (1000)     2275 2023-02-26 16:41:38.000000 mytonlib-0.7.2/README.md
-drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-02-26 16:42:56.812825 mytonlib-0.7.2/mytonlib/
--rw-r--r--   0 ton       (1000) ton       (1000)      133 2023-02-18 13:36:34.000000 mytonlib-0.7.2/mytonlib/__init__.py
--rw-r--r--   0 ton       (1000) ton       (1000)    29842 2023-02-26 14:55:30.000000 mytonlib-0.7.2/mytonlib/adnl.py
--rw-r--r--   0 ton       (1000) ton       (1000)     2538 2023-02-15 18:37:11.000000 mytonlib-0.7.2/mytonlib/block.fixes.tlb
--rw-r--r--   0 ton       (1000) ton       (1000)    31584 2023-02-18 13:35:00.000000 mytonlib-0.7.2/mytonlib/boc.py
--rw-r--r--   0 ton       (1000) ton       (1000)     5064 2023-02-26 15:11:56.000000 mytonlib-0.7.2/mytonlib/mytypes.py
--rw-r--r--   0 ton       (1000) ton       (1000)     6690 2023-02-26 15:22:33.000000 mytonlib-0.7.2/mytonlib/tests.py
--rw-r--r--   0 ton       (1000) ton       (1000)    11940 2023-02-15 18:37:11.000000 mytonlib-0.7.2/mytonlib/tl.py
--rw-r--r--   0 ton       (1000) ton       (1000)    25074 2023-02-26 15:22:21.000000 mytonlib-0.7.2/mytonlib/tlb.py
--rw-r--r--   0 ton       (1000) ton       (1000)     2151 2023-02-15 18:37:11.000000 mytonlib-0.7.2/mytonlib/utils.py
-drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-02-26 16:42:56.812825 mytonlib-0.7.2/mytonlib.egg-info/
--rw-r--r--   0 ton       (1000) ton       (1000)     2992 2023-02-26 16:42:56.000000 mytonlib-0.7.2/mytonlib.egg-info/PKG-INFO
--rw-r--r--   0 ton       (1000) ton       (1000)      380 2023-02-26 16:42:56.000000 mytonlib-0.7.2/mytonlib.egg-info/SOURCES.txt
--rw-r--r--   0 ton       (1000) ton       (1000)        1 2023-02-26 16:42:56.000000 mytonlib-0.7.2/mytonlib.egg-info/dependency_links.txt
--rw-r--r--   0 ton       (1000) ton       (1000)      108 2023-02-26 16:42:56.000000 mytonlib-0.7.2/mytonlib.egg-info/requires.txt
--rw-r--r--   0 ton       (1000) ton       (1000)        9 2023-02-26 16:42:56.000000 mytonlib-0.7.2/mytonlib.egg-info/top_level.txt
--rw-r--r--   0 ton       (1000) ton       (1000)      115 2023-02-15 18:37:11.000000 mytonlib-0.7.2/requirements.txt
--rw-r--r--   0 ton       (1000) ton       (1000)       38 2023-02-26 16:42:56.812825 mytonlib-0.7.2/setup.cfg
--rw-r--r--   0 ton       (1000) ton       (1000)      879 2023-02-26 16:42:47.000000 mytonlib-0.7.2/setup.py
+drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-05-29 08:58:38.758081 mytonlib-0.7.3/
+-rw-r--r--   0 ton       (1000) ton       (1000)    35823 2022-08-08 10:10:01.000000 mytonlib-0.7.3/LICENSE
+-rw-r--r--   0 ton       (1000) ton       (1000)       62 2023-02-19 09:41:29.000000 mytonlib-0.7.3/MANIFEST.in
+-rw-r--r--   0 ton       (1000) ton       (1000)     3008 2023-05-29 08:58:38.754081 mytonlib-0.7.3/PKG-INFO
+-rw-r--r--   0 ton       (1000) ton       (1000)     2814 2023-05-27 10:17:55.000000 mytonlib-0.7.3/README.md
+drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-05-29 08:58:38.754081 mytonlib-0.7.3/mytonlib/
+-rw-r--r--   0 ton       (1000) ton       (1000)      209 2023-05-28 06:55:21.000000 mytonlib-0.7.3/mytonlib/__init__.py
+-rw-r--r--   0 ton       (1000) ton       (1000)    31722 2023-05-29 08:57:22.000000 mytonlib-0.7.3/mytonlib/adnl.py
+-rw-r--r--   0 ton       (1000) ton       (1000)    12802 2023-05-27 16:23:07.000000 mytonlib-0.7.3/mytonlib/balancer.py
+-rw-r--r--   0 ton       (1000) ton       (1000)     3822 2023-02-27 18:45:26.000000 mytonlib-0.7.3/mytonlib/block.fixes.tlb
+-rw-r--r--   0 ton       (1000) ton       (1000)     8395 2023-03-17 17:10:29.000000 mytonlib-0.7.3/mytonlib/boc.py
+-rw-r--r--   0 ton       (1000) ton       (1000)     7697 2023-05-18 09:23:48.000000 mytonlib-0.7.3/mytonlib/mytypes.py
+-rw-r--r--   0 ton       (1000) ton       (1000)     8340 2023-04-06 14:47:44.000000 mytonlib-0.7.3/mytonlib/scanner.py
+-rw-r--r--   0 ton       (1000) ton       (1000)    42113 2023-05-18 20:25:32.000000 mytonlib-0.7.3/mytonlib/tests.py
+-rw-r--r--   0 ton       (1000) ton       (1000)    11940 2023-03-12 21:18:50.000000 mytonlib-0.7.3/mytonlib/tl.py
+-rw-r--r--   0 ton       (1000) ton       (1000)    25131 2023-03-09 19:10:23.000000 mytonlib-0.7.3/mytonlib/tlb.py
+-rw-r--r--   0 ton       (1000) ton       (1000)     2657 2023-03-12 18:30:01.000000 mytonlib-0.7.3/mytonlib/utils.py
+drwxr-xr-x   0 ton       (1000) ton       (1000)        0 2023-05-29 08:58:38.754081 mytonlib-0.7.3/mytonlib.egg-info/
+-rw-r--r--   0 ton       (1000) ton       (1000)     3008 2023-05-29 08:58:38.000000 mytonlib-0.7.3/mytonlib.egg-info/PKG-INFO
+-rw-r--r--   0 ton       (1000) ton       (1000)      421 2023-05-29 08:58:38.000000 mytonlib-0.7.3/mytonlib.egg-info/SOURCES.txt
+-rw-r--r--   0 ton       (1000) ton       (1000)        1 2023-05-29 08:58:38.000000 mytonlib-0.7.3/mytonlib.egg-info/dependency_links.txt
+-rw-r--r--   0 ton       (1000) ton       (1000)      108 2023-05-29 08:58:38.000000 mytonlib-0.7.3/mytonlib.egg-info/requires.txt
+-rw-r--r--   0 ton       (1000) ton       (1000)        9 2023-05-29 08:58:38.000000 mytonlib-0.7.3/mytonlib.egg-info/top_level.txt
+-rw-r--r--   0 ton       (1000) ton       (1000)      115 2023-02-15 18:37:11.000000 mytonlib-0.7.3/requirements.txt
+-rw-r--r--   0 ton       (1000) ton       (1000)       38 2023-05-29 08:58:38.758081 mytonlib-0.7.3/setup.cfg
+-rw-r--r--   0 ton       (1000) ton       (1000)      879 2023-05-27 16:02:23.000000 mytonlib-0.7.3/setup.py
```

### Comparing `mytonlib-0.7.2/LICENSE` & `mytonlib-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mytonlib-0.7.2/PKG-INFO` & `mytonlib-0.7.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,87 @@
 Metadata-Version: 2.1
 Name: mytonlib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Native library for working with TON (The Open Network)
 Home-page: https://github.com/igroman787/mytonlib
 Author: Igroman787
-License: UNKNOWN
-Description: ## What is it?
-        This is a native library for working with The Open Network. Without using `libtonlibjson.so`
-        
-        ## Installation
-        ```sh
-        pip3 install mytonlib
-        ```
-        
-        ## How to use
-        ```python
-        from mytonlib import AdnlTcpClient
-        
-        # Take public lite-server from https://ton-blockchain.github.io/global.config.json
-        host = "185.86.79.9"
-        port = 4701
-        pubkey = "G6cNAr6wXBBByWDzddEWP5xMFsAcp6y13fXA8Q7EJlM="
-        
-        # Connect to the lite-server with adnl
-        adnl = AdnlTcpClient()
-        adnl.connect(host, port, pubkey)
-        
-        # Test connection
-        adnl.ping()
-        
-        # Get masterchain info
-        adnl.get_masterchain_info()
-        ```
-        
-        ## List of available functions
-        All available functions are taken from lite-client
-        ```python
-        connect 				# Connect to the lite-server with adnl
-        ping 					# Test connection
-        get_time 				# Get server time
-        get_masterchain_info 	# Get last block and state info from server
-        get_account_state		# Loads the most recent state of specified account
-        run_smc_method			# Runs GET method <method-id> of account <addr> with specified parameters
-        get_all_shards_info		# Shows shard configuration from the most recent masterchain state or from masterchain state corresponding to <block-id-ext>
-        get_config_params		# Shows specified or all configuration parameters from the latest masterchain state
-        get_block_header		# Shows block header for <block-id-ext>
-        get_block				# Downloads block
-        get_last_transactions	# Shows or dumps specified transaction and several preceding ones
-        get_block_transactions	# Lists block transactions, starting immediately after or before the specified one
-        get_one_transaction		# Dumps one transaction of specified account
-        lookup_block			# Looks up a block by workchain, shard and seqno/lt/time, and shows its header
-        ```
-        
-        ## TLB unpacking 
-        A feature of this library is the automatic unpacking of data according to the TLB scheme:
-        ```python
-        data = adnl.run_smc_method("kQBL2_3lMiyywU17g-or8N7v9hDmPCpttzBPE2isF2GTziky", "mult", [5, 4])
-        print(data) # or print(json.dumps(data, indent=4))
-        
-        adnl.tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
-        data = adnl.tlb_schemes.deserialize(data.cell, expected="MyCell")
-        print(data.value)
-        ```
-        
-        ## More examples
-        https://github.com/igroman787/mytonlib/blob/master/mytonlib/tests.py
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## What is it?
+This is a native library for working with The Open Network - without using `libtonlibjson.so`. But for nativeness, we have to pay with speed.
+This library was written based on this documentation: https://github.com/xssnick/ton-deep-doc
+
+## Installation
+```sh
+pip3 install mytonlib
+```
+
+## How to use
+```python
+from mytonlib import AdnlTcpClientWithBalancer
+
+global_config_url = "https://ton-blockchain.github.io/global.config.json"
+adnl = AdnlTcpClientWithBalancer(global_config_url)
+
+# Get masterchain info
+adnl.get_masterchain_info()
+```
+
+## How to use without balancer
+```python
+from mytonlib import AdnlTcpClient
+
+# Take public lite-server from https://ton-blockchain.github.io/global.config.json
+host = "185.86.79.9"
+port = 4701
+pubkey = "G6cNAr6wXBBByWDzddEWP5xMFsAcp6y13fXA8Q7EJlM="
+
+# Connect to the lite-server with adnl
+adnl = AdnlTcpClient()
+adnl.connect(host, port, pubkey)
+
+# Test connection
+adnl.ping()
+
+# Get masterchain info
+adnl.get_masterchain_info()
+```
+
+## List of available functions
+All available functions are taken from lite-client
+```python
+connect 				# Connect to the lite-server with adnl
+ping 					# Test connection
+get_time 				# Get server time
+get_masterchain_info 	# Get last block and state info from server
+get_account_state		# Loads the most recent state of specified account
+run_smc_method			# Runs GET method <method-id> of account <addr> with specified parameters
+get_all_shards_info		# Shows shard configuration from the most recent masterchain state or from masterchain state corresponding to <block-id-ext>
+get_config_params		# Shows specified or all configuration parameters from the latest masterchain state
+get_block_header		# Shows block header for <block-id-ext>
+get_block				# Downloads block
+get_last_transactions	# Shows or dumps specified transaction and several preceding ones
+get_block_transactions	# Lists block transactions, starting immediately after or before the specified one
+get_one_transaction		# Dumps one transaction of specified account
+lookup_block			# Looks up a block by workchain, shard and seqno/lt/time, and shows its header
+```
+
+## TLB unpacking 
+A feature of this library is the automatic unpacking of data according to the TLB scheme:
+```python
+from mytonlib import TlbSchemes
+
+tlb_schemes = TlbSchemes()
+tlb_schemes.load_schemes("/usr/src/ton/tl/generate/scheme/")
+
+data = adnl.run_smc_method("kQBL2_3lMiyywU17g-or8N7v9hDmPCpttzBPE2isF2GTziky", "mult", [5, 4])
+print(data) # or print(json.dumps(data, indent=4))
+
+tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
+data = tlb_schemes.deserialize(data, expected="MyCell")
+print(data.value)
+```
+
+## More examples
+https://github.com/igroman787/mytonlib/blob/master/mytonlib/tests.py
```

### Comparing `mytonlib-0.7.2/README.md` & `mytonlib-0.7.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 ## What is it?
-This is a native library for working with The Open Network. Without using `libtonlibjson.so`
+This is a native library for working with The Open Network - without using `libtonlibjson.so`. But for nativeness, we have to pay with speed.
+This library was written based on this documentation: https://github.com/xssnick/ton-deep-doc
 
 ## Installation
 ```sh
 pip3 install mytonlib
 ```
 
 ## How to use
 ```python
+from mytonlib import AdnlTcpClientWithBalancer
+
+global_config_url = "https://ton-blockchain.github.io/global.config.json"
+adnl = AdnlTcpClientWithBalancer(global_config_url)
+
+# Get masterchain info
+adnl.get_masterchain_info()
+```
+
+## How to use without balancer
+```python
 from mytonlib import AdnlTcpClient
 
 # Take public lite-server from https://ton-blockchain.github.io/global.config.json
 host = "185.86.79.9"
 port = 4701
 pubkey = "G6cNAr6wXBBByWDzddEWP5xMFsAcp6y13fXA8Q7EJlM="
 
@@ -44,17 +56,22 @@
 get_one_transaction		# Dumps one transaction of specified account
 lookup_block			# Looks up a block by workchain, shard and seqno/lt/time, and shows its header
 ```
 
 ## TLB unpacking 
 A feature of this library is the automatic unpacking of data according to the TLB scheme:
 ```python
+from mytonlib import TlbSchemes
+
+tlb_schemes = TlbSchemes()
+tlb_schemes.load_schemes("/usr/src/ton/tl/generate/scheme/")
+
 data = adnl.run_smc_method("kQBL2_3lMiyywU17g-or8N7v9hDmPCpttzBPE2isF2GTziky", "mult", [5, 4])
 print(data) # or print(json.dumps(data, indent=4))
 
-adnl.tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
-data = adnl.tlb_schemes.deserialize(data.cell, expected="MyCell")
+tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
+data = tlb_schemes.deserialize(data, expected="MyCell")
 print(data.value)
 ```
 
 ## More examples
 https://github.com/igroman787/mytonlib/blob/master/mytonlib/tests.py
```

### Comparing `mytonlib-0.7.2/mytonlib/adnl.py` & `mytonlib-0.7.3/mytonlib/adnl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf_8 -*-
 
+import sys
 from os.path import isdir, dirname, join
-from os import listdir
 import time
 import json
+import random
 import base64
 import socket
 import x25519 # pip3 install x25519
 import hashlib
 import secrets
 import fastcrc # pip3 install fastcrc
 #import urllib.request
@@ -19,16 +20,15 @@
 from Crypto.Cipher import AES # pip3 install pycryptodome
 from Crypto.Util import Counter
 
 from .tl import TlSchemes, Int, tl_len
 from .tlb import TlbSchemes
 from .boc import serialize_boc, deserialize_boc
 from .utils import parse_addr, hex2dec
-from .mytypes import Dict
-
+from .mytypes import Dict, Thread
 
 
 class AdnlUdpClient():
 	def __init__(self):
 		self.local = None
 		self.sock = None
 		self.local_private_key = secrets.token_bytes(32)
@@ -71,19 +71,19 @@
 		
 		return mode_bin.uint
 	#end define
 	
 	def connect(self, host, port, peer_public_key_b64):
 		timestamp = int(time.time())
 		peer_public_key = base64.b64decode(peer_public_key_b64)
-		peer_id = self.get_id(peer_public_key)
+		peer_id = self._get_id(peer_public_key)
 		
 		local_public_key = self.get_public_key(self.local_private_key)
 		channel_public_key = self.get_public_key(self.channel_private_key)
-		local_id = self.get_id(local_public_key)
+		local_id = self._get_id(local_public_key)
 		
 		# create PublicKey message
 		public_key_message = Dict(scheme_name="pub.ed25519", key=local_public_key.hex())
 		
 		# create createChannel message
 		create_channel_message = Dict(scheme_name="adnl.message.createChannel", key=channel_public_key.hex(), date=timestamp)
 		
@@ -115,17 +115,17 @@
 		
 		# create PacketContents message with signature
 		packet_contents.flags = self.set_flags("flags.0,3,4,6,7,8,10,11")
 		packet_contents.signature = self.sign_message(self.local_private_key, packet_contents_message)
 		packet_contents_message = scheme.id + scheme.serialize(**packet_contents)
 		#print(f"packet_contents_message: {packet_contents_message.hex()}")
 		
-		checksum = self.sha256(packet_contents_message)
+		checksum = self._sha256(packet_contents_message)
 		secret = self.get_secret(self.local_private_key, peer_public_key)
-		encrypted_message = self.aes_encrypt_with_secret(packet_contents_message, secret, checksum)
+		encrypted_message = self._aes_encrypt_with_secret(packet_contents_message, secret, checksum)
 		send_data = peer_id + local_public_key + checksum + encrypted_message
 		#print(f"send_data: {send_data.hex()}")
 		
 		# send
 		self.sock = socket.socket(family=socket.AF_INET, type=socket.SOCK_DGRAM)
 		self.sock.settimeout(3)
 		self.sock.connect((host, port))
@@ -136,15 +136,15 @@
 		byte_stream = ByteStream(read_data)
 		read_local_id = byte_stream.read(32)
 		read_public_key = byte_stream.read(32)
 		read_checksum = byte_stream.read(32)
 		read_encrypted_message = byte_stream.read()
 		new_secret = self.get_secret(self.local_private_key, read_public_key)
 		read_message = self.aes_decrypt_with_secret(read_encrypted_message, new_secret, read_checksum)
-		checksum = self.sha256(read_message)
+		checksum = self._sha256(read_message)
 		if read_local_id != local_id:
 			raise Exception("connect error: read_local_id != local_id")
 		if read_checksum != checksum:
 			raise Exception("connect error: read_checksum != checksum")
 		#print(f"read_message: {read_message.hex()}")
 		
 		byte_stream = ByteStream(read_message)
@@ -183,28 +183,28 @@
 			flags = self.set_flags("flags.2,6,7"),
 			message = get_signed_address_list_message,
 			seqno = 2,
 			confirm_seqno = 1,
 			rand2 = secrets.token_bytes(15)
 		)
 		packet_contents_message = scheme.id + scheme.serialize(**packet_contents)
-		checksum = self.sha256(packet_contents_message)
-		encrypted_message = self.aes_encrypt_with_secret(packet_contents_message, channel_tx_key, checksum)
+		checksum = self._sha256(packet_contents_message)
+		encrypted_message = self._aes_encrypt_with_secret(packet_contents_message, channel_tx_key, checksum)
 		channel_tx_public_key = self.get_public_key(channel_tx_key)
-		tx_public_key_id = self.get_id(channel_tx_public_key)
+		tx_public_key_id = self._get_id(channel_tx_public_key)
 		send_data = tx_public_key_id + checksum + encrypted_message
 		print(f"send_data: {send_data.hex()}")
 		self.sock.send(send_data)
 		read_data, host_port = self.sock.recvfrom(1024)
 		print(f"read_data: {len(read_data)}, {read_data.hex()}")
 	#end define
 	
 	def get_message_by_name(self, messages, name):
 		for message in messages:
-			message_name = message.get("@name")
+			message_name = message.get("@type")
 			if message_name == name:
 				return message
 	#end define
 	
 	def sign_message(self, private_key, message):
 		signing_key = SigningKey(private_key)
 		signed_message = signing_key.sign(message)[:64]
@@ -224,67 +224,80 @@
 	
 	def get_public_key(self, private_key):
 		signing_key = SigningKey(private_key)
 		public_key = signing_key.verify_key.encode()
 		return public_key
 	#end define
 	
-	def aes_encrypt_with_secret(self, data, secret, checksum):
+	def _aes_encrypt_with_secret(self, data, secret, checksum):
 		key = secret[0:16] + checksum[16:32]
 		nonce = checksum[0:4] + secret[20:32]
-		cipher = self.create_aes_cipher(key, nonce)
+		cipher = self._create_aes_cipher(key, nonce)
 		encrypted_data = cipher.encrypt(data)
 		return encrypted_data
 	#end define
 	
 	def aes_decrypt_with_secret(self, encrypted_data, secret, checksum):
 		key = secret[0:16] + checksum[16:32]
 		nonce = checksum[0:4] + secret[20:32]
-		cipher = self.create_aes_cipher(key, nonce)
+		cipher = self._create_aes_cipher(key, nonce)
 		data = cipher.decrypt(encrypted_data)
 		return data
 	#end define
 	
-	def create_aes_cipher(self, key, nonce):
+	def _create_aes_cipher(self, key, nonce):
 		ctrInitValue = int.from_bytes(nonce, "big")
 		ctr = Counter.new(128, initial_value=ctrInitValue)
 		cipher = AES.new(key, AES.MODE_CTR, counter=ctr)
 		return cipher
 	#end define
 	
-	def get_id(self, pubkey):
+	def _get_id(self, pubkey):
 		magic = bytes.fromhex("c6b41348") # 0x4813b4c6
-		result = self.sha256(magic + pubkey)
+		result = self._sha256(magic + pubkey)
 		return result
 	#end define
 	
-	def sha256(self, data):
+	def _sha256(self, data):
 		return hashlib.sha256(data).digest()
 	#end define
 #end class
 
 class AdnlTcpClient:
 	def __init__(self):
+		self.host = None
+		self.port = None
+		self.ping_result = None
+		self.run_ping_thr = True
+		self.queue = list()
 		self.local = None
 		self.sock = None
 		self.local_priv = None
 		self.local_pub = None
 		self.rx_key = None
 		self.tx_key = None
 		self.rx_nonce = None
 		self.tx_nonce = None
 		self.rx_cipher = None
 		self.tx_cipher = None
-		self.ping_thread = None
 		self.tl_schemes = TlSchemes()
 		self.tlb_schemes = TlbSchemes()
 		self.load_tl_schemes()
 		self.load_tlb_schemes()
 	#end define
 	
+	def __str__(self):
+		return f"<AdnlTcpClient {self.host}:{self.port}, ping={self.ping_result}, rc={sys.getrefcount(self)}>"
+	#end define
+	
+	def __del__(self):
+		self.run_ping_thr = False
+		self.sock.close()
+	#end define
+	
 	def load_tl_schemes(self):
 		dir = "/usr/src/ton/tl/generate/scheme/"
 		if isdir(dir):
 			self.tl_schemes.load_schemes(dir)
 		else:
 			raise Exception("Tl schemes not found. Use command: `cd /usr/src && git clone https://github.com/ton-blockchain/ton`")
 	#end define
@@ -294,62 +307,61 @@
 		if isdir(dir):
 			self.tlb_schemes.load_schemes(dir)
 		else:
 			raise Exception("Tlb schemes not found. Use command: `cd /usr/src && git clone https://github.com/ton-blockchain/ton`")
 		my_dir = dirname(__file__)
 		self.tlb_schemes.load_schemes(join(my_dir, "block.fixes.tlb"))
 	#end define
-	
-	def add_log(self, text, type):
-		if self.local:
-			self.local.AddLog(text, type)
-		else:
-			print(text)
-	#end define
-	
-	def create_channel_keys(self):
-		# create local private key
-		sk = SigningKey.generate() # 32 bytes
-		self.channel_local_priv = sk.encode() # ed25519
-		self.channel_local_pub = sk.verify_key.encode() # ed25519
-	#end define
-	
-	def get_signed_address_list(self):
-		send_scheme = self.tl_schemes.get_scheme_by_name("dht.getSignedAddressList")
-		send_data = send_scheme.id
-	#end define
 
 	def connect(self, host, port, pubkey):
-		handshake = self.create_handshake(pubkey)
+		# save connecting addr
+		self.host = host
+		self.port = port
+		
+		# connect to server
+		self.sock = socket.socket()
+		self.sock.settimeout(3)
+		self.sock.connect((host, port))
+		
+		# create handshake
+		handshake = self._create_handshake(pubkey)
 
 		# create rx, tx cipher
-		self.rx_cipher = self.create_aes_cipher(self.rx_key, self.rx_nonce)
-		self.tx_cipher = self.create_aes_cipher(self.tx_key, self.tx_nonce)
+		self.rx_cipher = self._create_aes_cipher(self.rx_key, self.rx_nonce)
+		self.tx_cipher = self._create_aes_cipher(self.tx_key, self.tx_nonce)
 
 		# send handshake
-		self.sock = socket.socket()
-		self.sock.settimeout(3)
-		self.sock.connect((host, port))
-		self.sock.send(handshake)
+		self.sock.sendall(handshake)
 		
-		self.get_datagram()
+		self._get_datagram()
+		self.ping_result = self.ping()
 		
 		# Start ping thread
-		threading.Thread(target=self.ping_thr, daemon=True).start()
+		self._start_thread(self._ping_thr)
 	#end define
 	
-	def ping_thr(self):
-		while True:
+	def _start_thread(self, func, *args, **kwargs):
+		tnum = random.randint(1, 999999)
+		tname = f"{func.__name__}_{tnum}"
+		thr = Thread(target=func, args=args, name=tname, daemon=True)
+		#setattr(thr, "parent", threading.current_thread())
+		#setattr(thr, "start_time", time.time())
+		thr.start()
+		return thr
+	#end define
+	
+	def _ping_thr(self):
+		while self.run_ping_thr:
+			self.ping_result = self.ping()
 			time.sleep(5)
-			self.ping()
 	#end define
 
-	def create_handshake(self, pubkey_b64):
+	def _create_handshake(self, pubkey_b64):
 		peer_pub = base64.b64decode(pubkey_b64) # 32 bytes, ed25519
-		peer_id = self.get_id(peer_pub) # 32 bytes
+		peer_id = self._get_id(peer_pub) # 32 bytes
 		
 		# create local private key
 		sk = SigningKey.generate() # 32 bytes
 		local_priv = sk.encode() # ed25519
 		local_pub = sk.verify_key.encode() # ed25519
 		private_key = sk.to_curve25519_private_key().encode() # x25519
 
@@ -363,204 +375,251 @@
 		self.tx_key = secrets.token_bytes(32) # 32 bytes
 		self.rx_nonce = secrets.token_bytes(16) # 16 bytes
 		self.tx_nonce = secrets.token_bytes(16) # 16 bytes
 		padding = secrets.token_bytes(64) # 64 bytes
 		aes_params = self.rx_key + self.tx_key + self.rx_nonce + self.tx_nonce + padding # 160 bytes
 
 		#create handshake
-		checksum = self.sha256(aes_params) # 32 bytes
-		encrypted_aes_params = self.aes_encrypt_with_secret(aes_params, secret)
+		checksum = self._sha256(aes_params) # 32 bytes
+		encrypted_aes_params = self._aes_encrypt_with_secret(aes_params, secret)
 		handshake = peer_id + local_pub + checksum + encrypted_aes_params # 256 bytes
 		return handshake
 	#end define
 
-	def get_datagram(self):
-		data = self.receive(4)
+	def _get_datagram(self):
+		data = self._receive(4)
 		dlen = int.from_bytes(data, "little")
-		data = self.receive(dlen)
+		data = self._receive(dlen)
 		nonce = data[0:32]
 		buffer = data[32:-32]
 		checksum = data[-32:]
-		hash = self.sha256(nonce + buffer)
+		hash = self._sha256(nonce + buffer)
 		if hash != checksum:
 			print(f"buffer[{len(buffer)}]: {buffer.hex()}")
 			print("hash:", hash.hex())
 			print("checksum:", checksum.hex())
-			raise Exception("get_datagram error: Checksum does not match")
+			raise Exception("_get_datagram error: Checksum does not match")
 		return buffer
 	#end define
 
-	def send_datagram(self, data):
+	def _send_datagram(self, data):
 		nonce = secrets.token_bytes(32)
-		checksum = self.sha256(nonce + data)
+		checksum = self._sha256(nonce + data)
 		dlen = len(nonce + data + checksum)
 		dlen = dlen.to_bytes(4, byteorder="little")
 		sdata = dlen + nonce + data + checksum
-		self.send(sdata)
+		self._send_data(sdata)
 	#end define
 
-	def send(self, data):
+	def _send_data(self, data):
 		sdata = self.tx_cipher.encrypt(data)
 		self.sock.send(sdata)
 	#end define
 
-	def receive(self, dlen):
+	def _receive(self, dlen):
 		chunks = []
 		bytes_read = 0
 		while bytes_read < dlen:
 			read_len = min(dlen - bytes_read, 1024)
 			chunk = self.sock.recv(read_len)
 			if chunk == b'':
-				raise RuntimeError("receive error: socket connection broken")
+				raise RuntimeError("_receive error: socket connection broken")
 			chunks.append(chunk)
 			bytes_read += len(chunk)
 		rdata = b''.join(chunks)
 		#print(f"dlen: {dlen} -> {len(rdata)}")
 		if len(rdata) == 0:
-			raise Exception("receive error: no data")
+			raise Exception("_receive error: no data")
 		result = self.rx_cipher.decrypt(rdata)
 		return result
 	#end define
 
-	def aes_encrypt_with_secret(self, aes_params, secret):
-		hash = self.sha256(aes_params)
+	def _aes_encrypt_with_secret(self, aes_params, secret):
+		hash = self._sha256(aes_params)
 		key = secret[0:16] + hash[16:32]
 		nonce = hash[0:4] + secret[20:32]
-		cipher = self.create_aes_cipher(key, nonce)
+		cipher = self._create_aes_cipher(key, nonce)
 		result = cipher.encrypt(aes_params)
 		return result
 	#end define
 
-	def create_aes_cipher(self, key, nonce):
+	def _create_aes_cipher(self, key, nonce):
 		ctrInitValue = int.from_bytes(nonce, "big")
 		ctr = Counter.new(128, initial_value=ctrInitValue)
 		cipher = AES.new(key, AES.MODE_CTR, counter=ctr)
 		return cipher
 	#end define
 
-	def sha256(self, data):
+	def _sha256(self, data):
 		return hashlib.sha256(data).digest()
 	#end define
 
-	def get_id(self, pubkey):
+	def _get_id(self, pubkey):
 		magic = bytes.fromhex("c6b41348") # 0x4813b4c6
-		result = self.sha256(magic + pubkey)
+		result = self._sha256(magic + pubkey)
 		return result
 	#end define
 	
 	def get_method_id(self, method_name):
 		# https://github.com/ton-blockchain/ton/blob/24dc184a2ea67f9c47042b4104bbb4d82289fac1/crypto/smc-envelope/SmartContract.h#L75
 		buff = fastcrc.crc16.xmodem(method_name.encode("utf8"))
 		result = (buff & 0xffff) | 0x10000
 		return result
 	#end define
 	
-	def align_bytes(self, data, alen=4):
+	def _align_bytes(self, data, alen=4):
 		dlen = len(data)
 		nlen = 0
 		if dlen % alen != 0:
 			nlen = alen - dlen % alen
 		buff = bytes.fromhex("00")
 		result = data + buff * nlen
 		return result
 	#end define
 	
 	def ping(self):
+		result = None
+		request_id = self._wait()
+		try:
+			result = self._ping_process()
+		except ConnectionError:
+			self.run_ping_thr = False
+		except socket.timeout:
+			self.run_ping_thr = False
+		except OSError:
+			self.run_ping_thr = False
+		except Exception as err:
+			print(f"ping error: {err}, self: {self}")
+			self.run_ping_thr = False
+		self._free(request_id)
+		return result
+	#end define
+	
+	def _ping_process(self):
 		# send
+		start = time.time()
 		send_scheme = self.tl_schemes.get_scheme_by_name("tcp.ping")
 		random_id = secrets.token_bytes(8)
 		send_data = send_scheme.id + random_id
-		self.send_datagram(send_data)
+		self._send_datagram(send_data)
 		
 		# get
-		read_data = self.get_datagram()
+		read_data = self._get_datagram()
 		byte_stream = ByteStream(read_data)
 		read_scheme_id = byte_stream.read(4)
 		read_scheme = self.tl_schemes.get_scheme_by_id(read_scheme_id)
 		data = read_scheme.deserialize(byte_stream)
 		if data.random_id != Int(random_id):
-			raise Exception("Adnl ping error: random_id does not match")
-		return True
+			raise ConnectionError("Adnl ping error: random_id does not match")
+		diff = time.time() - start
+		diff = int(diff * 1000) # milliseconds
+		return diff
+	#end define
+	
+	def _query(self, send_data):
+		request_id = self._wait()
+		read_data = self._query_process(send_data)
+		self._free(request_id)
+		return read_data
 	#end define
 	
-	def query(self, data):
+	def _query_process(self, data):
 		# send
 		send_scheme = self.tl_schemes.get_scheme_by_name("adnl.message.query")
 		query_id = secrets.token_bytes(32)
 		dlen = tl_len(data)
-		data = self.align_bytes(dlen + data)
+		data = self._align_bytes(dlen + data)
 		send_data = send_scheme.id + query_id + data
-		self.send_datagram(send_data)
+		self._send_datagram(send_data)
 		#print(f"send_data: {send_data.hex()}")
 		
 		# get
-		read_data = self.get_datagram()
+		read_data = self._get_datagram()
 		#print(f"read_data[{len(read_data)}]: {read_data.hex()}")
 		byte_stream = ByteStream(read_data)
 		read_scheme_id = byte_stream.read(4)
 		read_scheme = self.tl_schemes.get_scheme_by_id(read_scheme_id)
 		data = read_scheme.deserialize(byte_stream)
 		if query_id.hex() != data.query_id:
 			raise Exception("Adnl query error: query_id does not match")
 		return data.answer
 	#end define
 	
-	def lite_server_query(self, data):
+	def _wait(self):
+		request_id = secrets.token_bytes(4)
+		if request_id not in self.queue:
+			self.queue.append(request_id)
+		else:
+			print("Wow. Recreating the request id")
+			self._wait()
+		while self.queue.index(request_id) > 0:
+			time.sleep(0.01)
+		return request_id
+	#end define
+	
+	def _free(self, request_id):
+		if request_id in self.queue:
+			self.queue.remove(request_id)
+		else:
+			print("Wow. You are faster than me")
+	#end define
+	
+	def _lite_server_query(self, data):
 		# send
 		send_scheme = self.tl_schemes.get_scheme_by_name("liteServer.query")
 		dlen = tl_len(data)
-		data = self.align_bytes(dlen + data)
+		data = self._align_bytes(dlen + data)
 		send_data = send_scheme.id + data
 		
 		# get
-		read_data = self.query(send_data)
+		read_data = self._query(send_data)
 		return read_data
 	#end define
 	
-	def lite_server(self, function_name, **data):
+	def _lite_server(self, function_name, **data):
 		# send
 		send_scheme = self.tl_schemes.get_scheme_by_name(f"liteServer.{function_name}")
 		send_data = send_scheme.id + send_scheme.serialize(**data)
 		
 		# get
-		read_data = self.lite_server_query(send_data)
+		read_data = self._lite_server_query(send_data)
 		#print(f"get: {read_data.hex()}")
 		byte_stream = ByteStream(read_data)
 		read_scheme_id = byte_stream.read(4)
 		read_scheme = self.tl_schemes.get_scheme_by_id(read_scheme_id)
 		result = read_scheme.deserialize(byte_stream, **data)
 		if read_scheme.name == "liteServer.error":
 			raise Exception(f"liteServer.error code: {result.code}, message: {result.message}")
 		return result
 	#end define
 	
 	def get_masterchain_info(self):
 		"""
 		liteServer.getMasterchainInfo = liteServer.MasterchainInfo;
 		"""
-		return self.lite_server("getMasterchainInfo")
+		return self._lite_server("getMasterchainInfo")
 	#end define
 	
 	def get_time(self):
 		"""
 		liteServer.getTime = liteServer.CurrentTime;
 		"""
-		return self.lite_server("getTime")
+		return self._lite_server("getTime")
 	#end define
 	
 	def get_block(self, block_id_ext=None):
 		"""
 		block#11ef55aa global_id:int32 info:^BlockInfo value_flow:^ValueFlow state_update:^(MERKLE_UPDATE ShardState) extra:^BlockExtra = Block;
 		"""
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
-		block_data = self.lite_server("getBlock", id=block_id_ext)
+		block_data = self._lite_server("getBlock", id=block_id_ext)
 		#print(f"get_block block_data: {block_data.data.hex()}")
 		data_cell = deserialize_boc(block_data.data)
 		#print(f"get_block data_cell: {json.dumps(data_cell, indent=4)}")
 		data = self.tlb_schemes.deserialize(data_cell, expected="FBlock")
 		return data
 	#end define
 	
@@ -570,15 +629,15 @@
 		split_state#5f327da5 left:^ShardStateUnsplit right:^ShardStateUnsplit = ShardState;
 		"""
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
-		block_data = self.lite_server("getState", id=block_id_ext)
+		block_data = self._lite_server("getState", id=block_id_ext)
 		data_cell = deserialize_boc(block_data.data)
 		data = self.tlb_schemes.deserialize(data_cell, expected="ShardState")
 		return data
 	#end define
 	
 	def get_block_header(self, block_id_ext=None):
 		"""
@@ -587,15 +646,15 @@
 		"""
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
 		mode = self.set_flags("mode.null")
-		block_header_data = self.lite_server("getBlockHeader", id=block_id_ext, mode=mode)
+		block_header_data = self._lite_server("getBlockHeader", id=block_id_ext, mode=mode)
 		data_cell = deserialize_boc(block_header_data.header_proof)
 		#print(f"get_block_header data_cell: {json.dumps(data_cell, indent=4)}")
 		data = self.tlb_schemes.deserialize(data_cell, expected="BlockHeader")
 		return data.virtual_root
 	#end define
 	
 	def set_flags(self, flags):
@@ -624,53 +683,53 @@
 		
 		mode = self.set_flags("mode.0.2")
 		workchain, addr = parse_addr(input_addr)
 		account_id = {"workchain":workchain, "id":addr}
 		method_id = self.get_method_id(method_name)
 		params_cell = self.tlb_schemes.serialize(required="VmStack", params=params)
 		params_boc = serialize_boc(params_cell)
-		data = self.lite_server("runSmcMethod", mode=mode, id=block_id_ext, account=account_id, method_id=method_id, params=params_boc)
+		data = self._lite_server("runSmcMethod", mode=mode, id=block_id_ext, account=account_id, method_id=method_id, params=params_boc)
+		if data.exit_code != 0:
+			raise Exception(f"run_smc_method error: exit_code={data.exit_code}")
+		#end if
 		
 		# data.proof # TODO
 		# data.shard_proof # TODO
 		data_cell = deserialize_boc(data.result)
 		#print(f"run_smc_method data_cell: {json.dumps(data_cell, indent=4)}")
 		data = self.tlb_schemes.deserialize(data_cell, expected="VmStack")
 		#print(f"run_smc_method data: {json.dumps(data, indent=4)}")
 		result = data.stack
 		if len(result) == 1:
 			result = result.pop()
-		#if "value" in result:
-		#	return result.value
 		return result
 	#end define
 	
 	def get_account_state(self, input_addr, block_id_ext=None):
 		"""
-		TODO: (MERKLE_PROOF ShardStateUnsplit)
 		liteServer.getAccountState id:tonNode.blockIdExt account:liteServer.accountId = liteServer.AccountState;
 		liteServer.accountState id:tonNode.blockIdExt shardblk:tonNode.blockIdExt shard_proof:bytes proof:bytes state:bytes = liteServer.AccountState;
 		"""
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
 		workchain, addr = parse_addr(input_addr)
 		account_id = {"workchain":workchain, "id":addr}
-		account_data = self.lite_server("getAccountState", id=block_id_ext, account=account_id)
+		account_data = self._lite_server("getAccountState", id=block_id_ext, account=account_id)
 		# account_data.proof # TODO
 		# account_data.shard_proof # TODO
 		state_cell = deserialize_boc(account_data.state)
 		proof_cell = deserialize_boc(account_data.proof)
 		#shard_proof_cell = deserialize_boc(account_data.shard_proof)
 		account_state = self.tlb_schemes.deserialize(state_cell, expected="Account")
-		shard_proof_state = self.tlb_schemes.deserialize(proof_cell[0], expected="ShardStateProof")
-		#print(f"shard_proof_state: {json.dumps(shard_proof_state, indent=4)}")
-		account_descr = shard_proof_state.virtual_root.accounts.get(hex2dec(addr))
+		shard_state_proof = self.tlb_schemes.deserialize(proof_cell[0], expected="ShardStateProof")
+		#print(f"shard_state_proof: {json.dumps(shard_state_proof, indent=4)}")
+		account_descr = shard_state_proof.virtual_root.accounts.get(hex2dec(addr))
 		account_state["last_trans_lt"] = account_descr.last_trans_lt
 		account_state["last_trans_hash"] = account_descr.last_trans_hash
 		account_state.to_class()
 		return account_state
 	#end define
 	
 	def get_all_shards_info(self, block_id_ext=None):
@@ -679,39 +738,49 @@
 		liteServer.allShardsInfo id:tonNode.blockIdExt proof:bytes data:bytes = liteServer.AllShardsInfo;
 		"""
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
-		shards_data = self.lite_server("getAllShardsInfo", id=block_id_ext)
+		shards_data = self._lite_server("getAllShardsInfo", id=block_id_ext)
 		# shards_data.proof # TODO
 		data_cell = deserialize_boc(shards_data.data)
 		data = self.tlb_schemes.deserialize(data_cell, expected="ShardHashes")
-		print(f"get_all_shards_info: shards_data.id={shards_data.id}")
-		return data
+		
+		shards = list()
+		for workchain, shards_list in data.items():
+			for shard_descr in shards_list:
+				shard = Dict()
+				shard["workchain"] = workchain
+				shard["shard"] = shard_descr.next_validator_shard
+				shard["seqno"] = shard_descr.seq_no
+				shard["root_hash"] = shard_descr.root_hash
+				shard["file_hash"] = shard_descr.file_hash
+				shard.to_class()
+				shards.append(shard)
+		return shards
 	#end define
 	
 	def get_config_params(self, params, block_id_ext=None):
 		"""
-		TODO: (MERKLE_PROOF ShardStateUnsplit)
 		liteServer.getConfigParams mode:# id:tonNode.blockIdExt param_list:(vector int) = liteServer.ConfigInfo;
 		liteServer.configInfo mode:# id:tonNode.blockIdExt state_proof:bytes config_proof:bytes = liteServer.ConfigInfo;
 		"""
 		if type(params) is int:
 			param_list = [params]
 		elif type(params) is list:
 			param_list = params
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
 		mode = self.set_flags("mode.null")
-		config_params_data = self.lite_server("getConfigParams", id=block_id_ext, mode=mode, param_list=param_list)
+		config_params_data = self._lite_server("getConfigParams", id=block_id_ext, mode=mode, param_list=param_list)
 		# config_params_data.state_proof # TODO
 		#state_proof_cell = deserialize_boc(config_params_data.state_proof)
 		config_proof_cell = deserialize_boc(config_params_data.config_proof)
 		#print(f"get_config_params config_proof_cell: {json.dumps(config_proof_cell, indent=4)}")
 		data = self.tlb_schemes.deserialize(config_proof_cell, expected="ConfigInfo")
 		#print(f"data: {json.dumps(data, indent=4)}")
 		
@@ -732,15 +801,15 @@
 		"""
 		
 		if block_id_ext is None:
 			data = self.get_masterchain_info()
 			block_id_ext = data.last
 		#end if
 		
-		transaction_data = self.lite_server("getOneTransaction", id=block_id_ext, account=account_id, lt=trans_lt)
+		transaction_data = self._lite_server("getOneTransaction", id=block_id_ext, account=account_id, lt=trans_lt)
 		# transaction_data.proof # TODO
 		#print(f"get_one_transaction transaction_data: {transaction_data}")
 		transaction_cell = deserialize_boc(transaction_data.transaction)
 		data = self.tlb_schemes.deserialize(transaction_cell, expected="Transaction")
 		return data
 	#end define
 	
@@ -749,15 +818,15 @@
 		liteServer.getTransactions count:# account:liteServer.accountId lt:long hash:int256 = liteServer.TransactionList;
 		liteServer.transactionList ids:(vector tonNode.blockIdExt) transactions:bytes = liteServer.TransactionList;
 		"""
 		
 		workchain, addr = parse_addr(input_addr)
 		account_id = {"workchain":workchain, "id":addr}
 		account_state = self.get_account_state(input_addr)
-		transactions_data = self.lite_server("getTransactions", count=count, account=account_id, lt=account_state.last_trans_lt, hash=account_state.last_trans_hash)
+		transactions_data = self._lite_server("getTransactions", count=count, account=account_id, lt=account_state.last_trans_lt, hash=account_state.last_trans_hash)
 		# transactions_data.ids # TODO
 		transaction_cells = deserialize_boc(transactions_data.transactions)
 		if type(transaction_cells) != list:
 			transaction_cells = [transaction_cells]
 		#end if
 		
 		result = list()
@@ -771,15 +840,15 @@
 	def get_block_transactions(self, block_id_ext, count=1000):
 		"""
 		liteServer.listBlockTransactions id:tonNode.blockIdExt mode:# count:# after:mode.7?liteServer.transactionId3 reverse_order:mode.6?true want_proof:mode.5?true = liteServer.BlockTransactions;
 		liteServer.blockTransactions id:tonNode.blockIdExt req_count:# incomplete:Bool ids:(vector liteServer.transactionId) proof:bytes = liteServer.BlockTransactions;
 		"""
 		
 		mode = self.set_flags("mode.0.1.2")
-		transactions_data = self.lite_server("listBlockTransactions", id=block_id_ext, mode=mode, count=count)
+		transactions_data = self._lite_server("listBlockTransactions", id=block_id_ext, mode=mode, count=count)
 		#print(f"get_block_transactions: transactions_data={transactions_data}")
 		return transactions_data.ids
 	#end define
 	
 	def lookup_block(self, workchain, shard, seqno=-1, lt=None, utime=None):
 		"""
 		liteServer.lookupBlock mode:# id:tonNode.blockId lt:mode.1?long utime:mode.2?int = liteServer.BlockHeader;
@@ -790,15 +859,15 @@
 			mode_str = "mode.0"
 		elif lt != None:
 			mode_str = "mode.1"
 		elif utime != None:
 			mode_str = "mode.2"
 		mode = self.set_flags(mode_str)
 		block_id = {"workchain": workchain, "shard": shard, "seqno": seqno}
-		block_data = self.lite_server("lookupBlock", mode=mode, id=block_id, lt=lt, utime=utime)
+		block_data = self._lite_server("lookupBlock", mode=mode, id=block_id, lt=lt, utime=utime)
 		block_cell = deserialize_boc(block_data.header_proof)
 		#result = self.tlb_schemes.deserialize(block_cell, expected="BlockHeader")
 		return block_data.id
 	#end define
 	
 	def send_ext_msg_from_filename(self, filename):
 		file = open(filename, 'rb')
@@ -818,11 +887,11 @@
 		byte_stream = ByteStream(body)
 		prefix = byte_stream.read(4)
 		boc_prefix = bytes.fromhex("b5ee9c72")
 		if prefix != boc_prefix:
 			raise Exception("send_ext_msg error: body is not a boc")
 		#end if
 		
-		data = self.lite_server("sendMessage", body=body)
+		data = self._lite_server("sendMessage", body=body)
 		return data
 	#end define
 #end class
```

### Comparing `mytonlib-0.7.2/mytonlib/block.fixes.tlb` & `mytonlib-0.7.3/mytonlib/block.fixes.tlb`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 !root_list$_ {X:Type} = ROOT_LIST X;
 
-
+// fix tl-b schema syntax error - space between type assignment
 block_info#9bc7a987 version:uint32 
   not_master:(## 1) 
   after_merge:(## 1) before_split:(## 1) 
   after_split:(## 1) 
   want_split:Bool want_merge:Bool
   key_block:Bool vert_seqno_incr:(## 1)
   flags:(## 8) { flags <= 1 }
@@ -18,18 +18,19 @@
   prev_key_block_seqno:uint32
   gen_software:flags.0?GlobalVersion
   master_ref:not_master?^BlkMasterInfo 
   prev_ref:^(BlkPrevInfo after_merge)
   prev_vert_ref:vert_seqno_incr?^(BlkPrevInfo 0)
   = BlockInfo;
 
-// issues 001
+// fix tl-b schema syntax error - space between type assignment
 dns_adnl_address#ad01 adnl_addr:bits256 flags:(## 8) { flags <= 1 }
   proto_list:flags.0?ProtoList = DNSRecord;
 
+// fix tl-b schema syntax error - space between type assignment
 dns_smc_address#9fd3 smc_addr:MsgAddressInt flags:(## 8) { flags <= 1 }
   cap_list:flags.0?SmcCapList = DNSRecord;
 
 masterchain_state_extra#cc26
   shard_hashes:ShardHashes
   config:ConfigParams
   ^[ flags:(## 16) { flags <= 1 }
@@ -53,16 +54,16 @@
 
 // issues 004
 block#11ef55aa global_id:int32
   info:^BlockInfo = FFBlock;
 
 
 shard_state_proof$_ (MERKLE_PROOF ShardStateUnsplit) = ShardStateProof;
-shard_block_proof$_ (MERKLE_PROOF Block) = ShardBlockProof;
-state_proof$_ (ROOT_LIST ShardStateProof ShardBlockProof) = StateProof;
+shard_block_proof$_ (MERKLE_PROOF Block) = BlockStateProof;
+state_proof$_ (ROOT_LIST ShardStateProof BlockStateProof) = StateProof;
 
 // issues 005
 shard_state#9023afe2 global_id:int32
   shard_id:ShardIdent 
   seq_no:uint32 vert_seq_no:#
   gen_utime:uint32 gen_lt:uint64
   min_ref_mc_seqno:uint32
@@ -73,11 +74,37 @@
   total_balance:CurrencyCollection
   total_validator_fees:CurrencyCollection
   libraries:(HashmapE 256 LibDescr)
   master_ref:(Maybe BlkMasterInfo) ]
   custom:(Maybe ^McStateExtra)
   = ShardStateUnsplit;
 
+// Add a new type that is already in use
 config_proof$_ (MERKLE_PROOF ShardStateUnsplit) = ConfigInfo;
 
+// Add a new type that is already in use
 vm_stk_bits#0200 value:bits256 = VmStackValue;
 
+// change variable type next_validator_shard from uint64 to int64 (long)
+shard_descr#b seq_no:uint32 reg_mc_seqno:uint32
+  start_lt:uint64 end_lt:uint64
+  root_hash:bits256 file_hash:bits256 
+  before_split:Bool before_merge:Bool
+  want_split:Bool want_merge:Bool
+  nx_cc_updated:Bool flags:(## 3) { flags = 0 }
+  next_catchain_seqno:uint32 next_validator_shard:int64
+  min_ref_mc_seqno:uint32 gen_utime:uint32
+  split_merge_at:FutureSplitMerge
+  fees_collected:CurrencyCollection
+  funds_created:CurrencyCollection = ShardDescr;
+
+shard_descr_new#a seq_no:uint32 reg_mc_seqno:uint32
+  start_lt:uint64 end_lt:uint64
+  root_hash:bits256 file_hash:bits256 
+  before_split:Bool before_merge:Bool
+  want_split:Bool want_merge:Bool
+  nx_cc_updated:Bool flags:(## 3) { flags = 0 }
+  next_catchain_seqno:uint32 next_validator_shard:int64
+  min_ref_mc_seqno:uint32 gen_utime:uint32
+  split_merge_at:FutureSplitMerge
+  ^[ fees_collected:CurrencyCollection
+     funds_created:CurrencyCollection ] = ShardDescr;
```

### Comparing `mytonlib-0.7.2/mytonlib/tl.py` & `mytonlib-0.7.3/mytonlib/tl.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 		#end if
 		
 		result = Dict()
 		self.buff_result = result
 		for var_name, var_type in self.vars.items():
 			result[var_name] = self.deser_types(byte_stream, var_type, send_data)
 		result.to_class()
-		result["@name"] = self.name
+		result["@type"] = self.name
 		return result
 	#end define
 	
 	def deser_types(self, byte_stream, var_type, subvars=None):
 		#p = byte_stream.tell()
 		#buff = byte_stream.read()
 		#byte_stream.seek(p)
```

### Comparing `mytonlib-0.7.2/mytonlib/tlb.py` & `mytonlib-0.7.3/mytonlib/tlb.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 				scheme = TlbScheme(buff)
 				buff = ""
 			else:
 				continue
 			if scheme.class_name == None:
 				continue
 			if scheme in self.schemes:
-				print(f"load_schemes_from_file warning: overwriting an existing tlb schema: {scheme.class_name}")
+				#print(f"load_schemes_from_text warning: overwriting an existing tlb schema: {scheme.class_name}")
 				self.schemes.remove(scheme)
 			self.schemes.append(scheme)
 			#print(f"TlbScheme: {scheme}")
 		#end for
 	#end define
 	
 	def load_schemes_from_dir(self, dir):
@@ -109,15 +109,15 @@
 		scheme = self.get_scheme_using_prefix(slice, expected)
 		#print(f"TlbSchemes deserialize: {scheme}")
 		self.save_class_vars(scheme, old_subvars)
 		if scheme.is_link == True:
 			result = self.deser_types(slice, scheme.link)
 		else:
 			result = self.deser_vars(slice, scheme.vars)
-			result["@name"] = scheme.name
+			result["@type"] = scheme.name
 		return result
 	#end define
 	
 	def save_class_vars(self, scheme, old_subvars):
 		#print(f"save_class_vars: class_vars={scheme.class_vars}, old_subvars={old_subvars}")
 		if old_subvars == None:
 			old_subvars = list()
@@ -289,36 +289,43 @@
 		if buff.bin == '0':
 			var_value = self.deser_types(slice, x_type)
 		else:
 			var_value = self.deser_types(slice, y_type)
 		return var_value
 	#end define
 	
-	def deser_bin_tree(self, slice, x_type):
+	def deser_bin_tree(self, slice, x_type, result=None):
+		if result == None:
+			result = list()
+		#end if
+		
 		buff = slice.read(1)
 		if buff.bin == '0':
-			result = self.deser_types(slice, x_type)
+			# leaf
+			var_value = self.deser_types(slice, x_type)
+			result.append(var_value)
 		elif buff.bin == '1':
-			result = dict()
+			# left
 			left_cell = slice.read_ref()
 			left_slice = Slice(left_cell)
-			result["left"] = self.deser_bin_tree(left_slice, x_type)
+			self.deser_bin_tree(left_slice, x_type, result)
+			
+			# rigth
 			right_cell = slice.read_ref()
 			right_slice = Slice(right_cell)
-			result["right"] = self.deser_bin_tree(right_slice, x_type)
+			self.deser_bin_tree(right_slice, x_type, result)
 		return result
 	#end define
 	
 	def deser_hashmap_e(self, slice, n, x_type):
 		s = ""
 		n = int(n)
 		result = dict()
 		#print(f"deser_hashmap_e: {n} {x_type}")
 		buff = slice.read(1)
-		#print(f"deser_hashmap_e buff: {buff.bin}")
 		if buff.bin == '0':
 			# hme_empty
 			return
 		# hme_root
 		new_cell = slice.read_ref()
 		new_slice = Slice(new_cell)
 		self.deser_hashmap(result, new_slice, n, x_type, s)
@@ -822,15 +829,15 @@
 	def parse_vars(self, vars_buff):
 		vars = dict()
 		for item in vars_buff.copy():
 			if '{' in item or '}' in item:
 				#print(f"Found a logical equation. Skipping: {item}")
 				continue
 			if ':' not in item:
-				print(f"TLB schema syntax error found: {item}")
+				#print(f"TLB schema syntax error found: {item}")
 				continue
 			buff = item.split(':')
 			if item.startswith('^'):
 				var_name = "_"
 				var_type = item
 			else:
 				var_name = buff.pop(0)
```

### Comparing `mytonlib-0.7.2/mytonlib/utils.py` & `mytonlib-0.7.3/mytonlib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf_8 -*-
 
 import base64
 import fastcrc
+import struct
+import socket
 
 
 
+def ip2int(addr):
+	return struct.unpack("!i", socket.inet_aton(addr))[0]
+#end define
+
+def int2ip(dec):
+	return socket.inet_ntoa(struct.pack("!i", dec))
+#end define
+
 def hex2dec(h):
 	return int(h, base=16)
 #end define
 
 def dec2hex_addr(dec):
 	h = dec2hex(dec)
 	h64 = h.rjust(64, '0')
@@ -97,7 +107,21 @@
 def IsAddrFull(addr):
 	try:
 		ParseAddrFull(addr)
 		return True
 	except: pass
 	return False
 #end define
+
+class bcolors:
+	'''This class is designed to display text in color format'''
+	red = "\033[31m"
+	green = "\033[32m"
+	yellow = "\033[33m"
+	blue = "\033[34m"
+	magenta = "\033[35m"
+	cyan = "\033[36m"
+	endc = "\033[0m"
+	bold = "\033[1m"
+	underline = "\033[4m"
+	default = "\033[39m"
+#end class
```

### Comparing `mytonlib-0.7.2/mytonlib.egg-info/PKG-INFO` & `mytonlib-0.7.3/mytonlib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,87 @@
 Metadata-Version: 2.1
 Name: mytonlib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Native library for working with TON (The Open Network)
 Home-page: https://github.com/igroman787/mytonlib
 Author: Igroman787
-License: UNKNOWN
-Description: ## What is it?
-        This is a native library for working with The Open Network. Without using `libtonlibjson.so`
-        
-        ## Installation
-        ```sh
-        pip3 install mytonlib
-        ```
-        
-        ## How to use
-        ```python
-        from mytonlib import AdnlTcpClient
-        
-        # Take public lite-server from https://ton-blockchain.github.io/global.config.json
-        host = "185.86.79.9"
-        port = 4701
-        pubkey = "G6cNAr6wXBBByWDzddEWP5xMFsAcp6y13fXA8Q7EJlM="
-        
-        # Connect to the lite-server with adnl
-        adnl = AdnlTcpClient()
-        adnl.connect(host, port, pubkey)
-        
-        # Test connection
-        adnl.ping()
-        
-        # Get masterchain info
-        adnl.get_masterchain_info()
-        ```
-        
-        ## List of available functions
-        All available functions are taken from lite-client
-        ```python
-        connect 				# Connect to the lite-server with adnl
-        ping 					# Test connection
-        get_time 				# Get server time
-        get_masterchain_info 	# Get last block and state info from server
-        get_account_state		# Loads the most recent state of specified account
-        run_smc_method			# Runs GET method <method-id> of account <addr> with specified parameters
-        get_all_shards_info		# Shows shard configuration from the most recent masterchain state or from masterchain state corresponding to <block-id-ext>
-        get_config_params		# Shows specified or all configuration parameters from the latest masterchain state
-        get_block_header		# Shows block header for <block-id-ext>
-        get_block				# Downloads block
-        get_last_transactions	# Shows or dumps specified transaction and several preceding ones
-        get_block_transactions	# Lists block transactions, starting immediately after or before the specified one
-        get_one_transaction		# Dumps one transaction of specified account
-        lookup_block			# Looks up a block by workchain, shard and seqno/lt/time, and shows its header
-        ```
-        
-        ## TLB unpacking 
-        A feature of this library is the automatic unpacking of data according to the TLB scheme:
-        ```python
-        data = adnl.run_smc_method("kQBL2_3lMiyywU17g-or8N7v9hDmPCpttzBPE2isF2GTziky", "mult", [5, 4])
-        print(data) # or print(json.dumps(data, indent=4))
-        
-        adnl.tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
-        data = adnl.tlb_schemes.deserialize(data.cell, expected="MyCell")
-        print(data.value)
-        ```
-        
-        ## More examples
-        https://github.com/igroman787/mytonlib/blob/master/mytonlib/tests.py
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## What is it?
+This is a native library for working with The Open Network - without using `libtonlibjson.so`. But for nativeness, we have to pay with speed.
+This library was written based on this documentation: https://github.com/xssnick/ton-deep-doc
+
+## Installation
+```sh
+pip3 install mytonlib
+```
+
+## How to use
+```python
+from mytonlib import AdnlTcpClientWithBalancer
+
+global_config_url = "https://ton-blockchain.github.io/global.config.json"
+adnl = AdnlTcpClientWithBalancer(global_config_url)
+
+# Get masterchain info
+adnl.get_masterchain_info()
+```
+
+## How to use without balancer
+```python
+from mytonlib import AdnlTcpClient
+
+# Take public lite-server from https://ton-blockchain.github.io/global.config.json
+host = "185.86.79.9"
+port = 4701
+pubkey = "G6cNAr6wXBBByWDzddEWP5xMFsAcp6y13fXA8Q7EJlM="
+
+# Connect to the lite-server with adnl
+adnl = AdnlTcpClient()
+adnl.connect(host, port, pubkey)
+
+# Test connection
+adnl.ping()
+
+# Get masterchain info
+adnl.get_masterchain_info()
+```
+
+## List of available functions
+All available functions are taken from lite-client
+```python
+connect 				# Connect to the lite-server with adnl
+ping 					# Test connection
+get_time 				# Get server time
+get_masterchain_info 	# Get last block and state info from server
+get_account_state		# Loads the most recent state of specified account
+run_smc_method			# Runs GET method <method-id> of account <addr> with specified parameters
+get_all_shards_info		# Shows shard configuration from the most recent masterchain state or from masterchain state corresponding to <block-id-ext>
+get_config_params		# Shows specified or all configuration parameters from the latest masterchain state
+get_block_header		# Shows block header for <block-id-ext>
+get_block				# Downloads block
+get_last_transactions	# Shows or dumps specified transaction and several preceding ones
+get_block_transactions	# Lists block transactions, starting immediately after or before the specified one
+get_one_transaction		# Dumps one transaction of specified account
+lookup_block			# Looks up a block by workchain, shard and seqno/lt/time, and shows its header
+```
+
+## TLB unpacking 
+A feature of this library is the automatic unpacking of data according to the TLB scheme:
+```python
+from mytonlib import TlbSchemes
+
+tlb_schemes = TlbSchemes()
+tlb_schemes.load_schemes("/usr/src/ton/tl/generate/scheme/")
+
+data = adnl.run_smc_method("kQBL2_3lMiyywU17g-or8N7v9hDmPCpttzBPE2isF2GTziky", "mult", [5, 4])
+print(data) # or print(json.dumps(data, indent=4))
+
+tlb_schemes.load_schemes_from_text("mycell$_ value:uint64 = MyCell;")
+data = tlb_schemes.deserialize(data, expected="MyCell")
+print(data.value)
+```
+
+## More examples
+https://github.com/igroman787/mytonlib/blob/master/mytonlib/tests.py
```

### Comparing `mytonlib-0.7.2/setup.py` & `mytonlib-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open(join(my_dir, "requirements.txt")) as file:
     install_requires = file.read().split('\n')
 with open(join(my_dir, "README.md")) as file:
     long_description = file.read()
 #end with
 
 setup(name = "mytonlib",
-	version = "0.7.2",
+	version = "0.7.3",
 	description = "Native library for working with TON (The Open Network)",
 	author = "Igroman787",
 	url = "https://github.com/igroman787/mytonlib",
 	packages = ["mytonlib"],
 	package_data = {"mytonlib": ["block.fixes.tlb"]},
 	install_requires = install_requires,
     long_description = long_description,
```

