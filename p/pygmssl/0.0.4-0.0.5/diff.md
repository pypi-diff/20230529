# Comparing `tmp/pygmssl-0.0.4.tar.gz` & `tmp/pygmssl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmssl-0.0.4.tar", last modified: Sun May 28 05:57:43 2023, max compression
+gzip compressed data, was "pygmssl-0.0.5.tar", last modified: Mon May 29 12:56:14 2023, max compression
```

## Comparing `pygmssl-0.0.4.tar` & `pygmssl-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.410868 pygmssl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 05:57:32.000000 pygmssl-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 05:57:43.410868 pygmssl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-28 05:57:32.000000 pygmssl-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/pygmssl/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/_gm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pygmssl/sm4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/pygmssl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 05:57:43.000000 pygmssl-0.0.4/pygmssl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-28 05:57:32.000000 pygmssl-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 05:57:43.410868 pygmssl-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 05:57:43.406868 pygmssl-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-28 05:57:32.000000 pygmssl-0.0.4/tests/test_sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 12:56:02.000000 pygmssl-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-29 12:56:14.267233 pygmssl-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-29 12:56:02.000000 pygmssl-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/pygmssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/_gm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pygmssl/sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/pygmssl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 12:56:14.000000 pygmssl-0.0.5/pygmssl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 12:56:02.000000 pygmssl-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:56:14.267233 pygmssl-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:56:14.267233 pygmssl-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-29 12:56:02.000000 pygmssl-0.0.5/tests/test_sm4.py
```

### Comparing `pygmssl-0.0.4/LICENSE` & `pygmssl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.4/pygmssl/sm2.py` & `pygmssl-0.0.5/pygmssl/sm2.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from ._gm import _gm
 from .sm3 import _SM3CTX
 
 SM2_DEFAULT_ID = b'1234567812345678'
 SM2_MIN_SIGNATURE_SIZE = 8
 SM2_MAX_SIGNATURE_SIZE = 72
+SM2_MIN_PLAINTEXT_SIZE = 1
+SM2_MAX_PLAINTEXT_SIZE = 255
+SM2_MIN_CIPHERTEXT_SIZE = 45
+SM2_MAX_CIPHERTEXT_SIZE = 366
 
 
 class _SM2_POINT(Structure):
     _fields_ = [
         ('x', c_uint8 * 32),
         ('y', c_uint8 * 32),
     ]
@@ -83,7 +87,27 @@
         buff = (c_uint8 * 4096)()
         for i in range(0, len(data), 4096):
             chunk = data[i:i + 4096]
             buff[:len(chunk)] = chunk
             _gm.sm2_verify_update(byref(_verify_ctx), byref(buff), len(chunk))
         ret = _gm.sm2_verify_finish(byref(_verify_ctx), c_char_p(sig), len(sig))
         return ret == 1
+
+    def encrypt(self, data:bytes) -> bytes:
+        if len(data) > SM2_MAX_PLAINTEXT_SIZE:
+            raise ValueError('to encrypt data\'s length must <= sm2.SM2_MIN_PLAINTEXT_SIZE')
+        buff = (c_uint8 * SM2_MAX_PLAINTEXT_SIZE)()
+        buff[:len(data)] = data
+        out = (c_uint8 * SM2_MAX_CIPHERTEXT_SIZE)()
+        length = c_size_t()
+        _gm.sm2_encrypt(byref(self._sm2_key), byref(buff), len(data), byref(out), byref(length))
+        return bytes(out[:length.value])
+
+    def decrypt(self, data:bytes) -> bytes:
+        if len(data) > SM2_MAX_CIPHERTEXT_SIZE:
+            raise ValueError('to decrypt data\'s length must <= sm2.SM2_MAX_CIPHERTEXT_SIZE')
+        buff = (c_uint8 * SM2_MAX_CIPHERTEXT_SIZE)()
+        buff[:len(data)] = data
+        out = (c_uint8 * SM2_MAX_PLAINTEXT_SIZE)()
+        length = c_size_t()
+        _gm.sm2_decrypt(byref(self._sm2_key), byref(buff), len(data), byref(out), byref(length))
+        return bytes(out[:length.value])
```

### Comparing `pygmssl-0.0.4/pygmssl/sm3.py` & `pygmssl-0.0.5/pygmssl/sm3.py`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.4/pygmssl/sm4.py` & `pygmssl-0.0.5/pygmssl/sm4.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ctypes import byref, c_uint8, c_size_t, c_uint32, Structure, c_char_p
+from enum import Enum
 
 from ._gm import _gm
 
 SM4_KEY_SIZE = 16
 SM4_BLOCK_SIZE = 16
 SM4_NUM_ROUNDS = 32
 
@@ -25,14 +26,15 @@
         assert len(key) == 16
         assert len(iv) == 16
         if encrypt:
             _gm.sm4_cbc_encrypt_init(byref(self), c_char_p(key), c_char_p(iv))
         else:
             _gm.sm4_cbc_decrypt_init(byref(self), c_char_p(key), c_char_p(iv))
         self._result: list[bytes] = []
+        self._encrypt = encrypt
 
     def encrypt_update(self, data: bytes):
         outbuf = (c_uint8 * 4196)()
         out_length = c_size_t(0)
         inbuf = (c_uint8 * 4096)()
         for i in range(0, len(data), 4096):
             chunk = data[i:i + 4096]
@@ -61,24 +63,28 @@
         outbuf = (c_uint8 * 4196)()
         out_length = c_size_t(0)
         _gm.sm4_cbc_decrypt_finish(byref(self), byref(outbuf), byref(out_length))
         self._result.append(bytes(outbuf[:out_length.value]))
         return b''.join(self._result)
 
 
-MOD_CTX_DICT = {
+_MOD_CTX_DICT = {
     'CBC': _SM4_CBC_CTX
 }
 
 
+class MOD(str, Enum):
+    CBC = 'CBC'
+
+
 class SM4:
-    def __init__(self, key: bytes, *, mode: str, iv: bytes):
-        if mode.upper() not in MOD_CTX_DICT:
-            raise ValueError(u'Only support sm4 mod: %s' % MOD_CTX_DICT.keys())
-        self._ctx = MOD_CTX_DICT[mode.upper()]()
+    def __init__(self, key: bytes, *, mode: MOD, iv: bytes):
+        if mode.value.upper() not in _MOD_CTX_DICT:
+            raise ValueError(u'Only support sm4 mod: %s' % _MOD_CTX_DICT.keys())
+        self._ctx = _MOD_CTX_DICT[mode.value.upper()]()
         self.key = key
         self.iv = iv
 
     def encrypt(self, data: bytes) -> bytes:
         self._ctx.init(self.key, self.iv, encrypt=True)
         self._ctx.encrypt_update(data)
         return self._ctx.encrypt_get()
```

### Comparing `pygmssl-0.0.4/pyproject.toml` & `pygmssl-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.4/tests/test_sm2.py` & `pygmssl-0.0.5/tests/test_sm2.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,18 @@
 
     def test_006_sm2_sign_with_id(self):
         data = b'hello, world'
         sig = self.k.sign(data, id=b'123')
         self.assertFalse(self.k.verify(data, sig))
         self.assertTrue(self.k.verify(data, sig=sig, id=b'123'))
         self.assertFalse(self.k.verify(b'\x00' + data, sig=sig, id=b'123'))
+
+    def test_007_sm2_encrypt_and_decrypt(self):
+        data = b'hello, world'
+        self.assertEqual(self.k.decrypt(self.k.encrypt(data)), data)
+
+    def test_008_sm2_encrypt_and_decrypt_check(self):
+        data = b'1' * 1024
+        with self.assertRaises(ValueError):
+            self.k.encrypt(data)
+        with self.assertRaises(ValueError):
+            self.k.decrypt(data)
```

### Comparing `pygmssl-0.0.4/tests/test_sm3.py` & `pygmssl-0.0.5/tests/test_sm3.py`

 * *Files identical despite different names*

### Comparing `pygmssl-0.0.4/tests/test_sm4.py` & `pygmssl-0.0.5/tests/test_sm4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 from unittest import TestCase
 
-from pygmssl.sm4 import SM4
+from pygmssl.sm4 import SM4, MOD
 
 
-class TestSM2(TestCase):
+class TestSM4(TestCase):
     def setUp(self) -> None:
         self._16_key = b"\x97\xfc\xa3\xd7\t;\xf3\xd1'\x9c\x8c\x03\x92\x1c\xf5\xd2"
         self._16_iv = b'p\xce\xb9\x8d\t$x\x9c\x0f]\xea\x92\xae\xa1\x96\x9d'
         self._48_key = b'q\xb4j\xdem\x84|J\xf2\x92u\x14\x8f\x95\x85\x1e\x8fT\x01A' \
                        b'\x19<\xe1\x82t\xf4\x921\x0b\xbb\x9f\xabY8\xf4\xb2\xf2^\x10|\xbf\xf90\xeb\x19\x12,\xd4'
 
     def test_000_valid_mod(self):
         with self.assertRaises(ValueError):
-            SM4(self._16_key, mode='JBC', iv=b'123')
+            SM4(self._16_key, mode=MOD('CDC'), iv=b'123')
 
     def test_001_cbc_encrypt(self):
-        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        k = SM4(self._16_key, mode=MOD.CBC, iv=self._16_iv)
+        k2 = SM4(self._16_key, mode=MOD.CBC, iv=self._16_iv)
         e_data = k.encrypt(b'hello, world')
         self.assertEqual(b'W\x855 su+\x95\xd9@\x0fGL\xacKk', e_data)
         self.assertEqual(b'hello, world', k2.decrypt(e_data))
 
     def test_002_cbc_bulk_encrypt(self):
-        k = SM4(self._16_key, mode='CBC', iv=self._16_iv)
-        k2 = SM4(self._16_key, mode='CBC', iv=self._16_iv)
+        k = SM4(self._16_key, mode=MOD.CBC, iv=self._16_iv)
+        k2 = SM4(self._16_key, mode=MOD.CBC, iv=self._16_iv)
         bulk_data = os.urandom(512) * 2099
         self.assertEqual(bulk_data, k2.decrypt(k.encrypt(bulk_data)))
```

