# Comparing `tmp/numerbay-0.2.3.tar.gz` & `tmp/numerbay-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerbay-0.2.3.tar", last modified: Tue Sep 20 14:20:35 2022, max compression
+gzip compressed data, was "numerbay-0.2.4.tar", last modified: Mon May 29 15:37:41 2023, max compression
```

## Comparing `numerbay-0.2.3.tar` & `numerbay-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-20 14:20:35.543091 numerbay-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2022-09-20 14:20:30.000000 numerbay-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3294 2022-09-20 14:20:35.539091 numerbay-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2019 2022-09-20 14:20:30.000000 numerbay-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-20 14:20:35.539091 numerbay-0.2.3/numerbay/
--rw-r--r--   0 runner    (1001) docker     (116)      332 2022-09-20 14:20:30.000000 numerbay-0.2.3/numerbay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3822 2022-09-20 14:20:30.000000 numerbay-0.2.3/numerbay/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    32160 2022-09-20 14:20:30.000000 numerbay-0.2.3/numerbay/numerbay.py
--rw-r--r--   0 runner    (1001) docker     (116)     6891 2022-09-20 14:20:30.000000 numerbay-0.2.3/numerbay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-20 14:20:35.539091 numerbay-0.2.3/numerbay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3294 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      296 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-09-20 14:20:35.000000 numerbay-0.2.3/numerbay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-20 14:20:35.543091 numerbay-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1530 2022-09-20 14:20:30.000000 numerbay-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:37:41.731531 numerbay-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-29 15:37:38.000000 numerbay-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-29 15:37:41.731531 numerbay-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-29 15:37:38.000000 numerbay-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:37:41.731531 numerbay-0.2.4/numerbay/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-29 15:37:38.000000 numerbay-0.2.4/numerbay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-29 15:37:38.000000 numerbay-0.2.4/numerbay/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-05-29 15:37:38.000000 numerbay-0.2.4/numerbay/numerbay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-29 15:37:38.000000 numerbay-0.2.4/numerbay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:37:41.731531 numerbay-0.2.4/numerbay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 15:37:41.000000 numerbay-0.2.4/numerbay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:37:41.731531 numerbay-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-29 15:37:38.000000 numerbay-0.2.4/setup.py
```

### Comparing `numerbay-0.2.3/LICENSE` & `numerbay-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `numerbay-0.2.3/PKG-INFO` & `numerbay-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerbay
-Version: 0.2.3
+Version: 0.2.4
 Summary: Programmatic interaction with numerbay.ai - the Numerai community marketplace
 Home-page: https://github.com/councilofelders/numerbay-api
 Maintainer: numerbay
 Maintainer-email: admin@numerbay.ai
 License: MIT License
 Project-URL: Documentation, https://docs.numerbay.ai/
 Description:
```

### Comparing `numerbay-0.2.3/README.md` & `numerbay-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `numerbay-0.2.3/numerbay/cli.py` & `numerbay-0.2.4/numerbay/cli.py`

 * *Files identical despite different names*

### Comparing `numerbay-0.2.3/numerbay/numerbay.py` & `numerbay-0.2.4/numerbay/numerbay.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         elif isinstance(errors, dict):
             if "detail" in errors:
                 msg = errors["detail"]
                 self.logger.error(msg)
         elif isinstance(errors, str):
             msg = errors
             self.logger.error(errors)
+        else:
+            msg = "Unknown error"
+            self.logger.error(msg)
         return msg
 
     def get_account(self) -> Dict:
         """Get all information about your account!
 
         Returns:
             dict: user information including the following fields:
@@ -868,7 +871,48 @@
             # fail!
             raise ValueError(err)
 
         utils.download_file(file_url, dest_path, self.show_progress_bars)
 
         if isinstance(artifact_id, str):
             utils.decrypt_file(dest_path, key_path=key_path, key_base64=key_base64)
+
+    def lock_product(
+        self,
+        product_id: int = None,
+        product_full_name: str = None,
+        round_number: int = None,
+    ) -> Dict:
+        """Lock product.
+        Args:
+            product_id (int, optional): NumerBay product ID
+            product_full_name (str, optional): NumerBay product full name
+                (e.g. numerai-predictions-numerbay),
+                used for resolving product_id if product_id is not provided
+            round_number (int, optional): round number to lock, defaults to current selling round
+        Example:
+            ```python
+            api = NumerBay(username="..", password="..")
+            api.lock_product(product_id=2)
+            ```
+        """
+        product = self._resolve_product(
+            product_id=product_id, product_full_name=product_full_name
+        )
+        if product is None:
+            raise ValueError(
+                "Failed to resolve product: "
+                "make sure you have an active product with provided product_id or product_full_name"
+            )
+        product_id = product["id"]
+
+        data = utils.post_with_err_handling(
+            f"{API_ENDPOINT_URL}/products/{product_id}/lock",
+            json={"round_number": round_number},
+            headers={"Authorization": f"Bearer {self.token}"},
+        )
+
+        if data and "detail" in data:
+            err = self._handle_call_error(data["detail"])
+            # fail!
+            raise ValueError(err)
+        return data
```

### Comparing `numerbay-0.2.3/numerbay/utils.py` & `numerbay-0.2.4/numerbay/utils.py`

 * *Files identical despite different names*

### Comparing `numerbay-0.2.3/numerbay.egg-info/PKG-INFO` & `numerbay-0.2.4/numerbay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerbay
-Version: 0.2.3
+Version: 0.2.4
 Summary: Programmatic interaction with numerbay.ai - the Numerai community marketplace
 Home-page: https://github.com/councilofelders/numerbay-api
 Maintainer: numerbay
 Maintainer-email: admin@numerbay.ai
 License: MIT License
 Project-URL: Documentation, https://docs.numerbay.ai/
 Description:
```

### Comparing `numerbay-0.2.3/setup.py` & `numerbay-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 
 def load(path):
     return open(path, "r").read()
 
 
-numerbay_version = "0.2.3"
+numerbay_version = "0.2.4"
 
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
```

