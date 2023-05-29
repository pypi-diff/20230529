# Comparing `tmp/acryo-0.4.0.tar.gz` & `tmp/acryo-0.4.1.tar.gz`

## Comparing `acryo-0.4.0.tar` & `acryo-0.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/__init__.py
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_dask.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_reader.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_rotation.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_typed_scipy.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_types.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/_utils.py
--rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/simulator.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/__init__.py
--rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_base.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_bound.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/alignment/_concrete.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/__init__.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_api.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_bandpass.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_missing_wedge.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_pcc.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/backend/_zncc.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/__init__.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/_dask_pca.py
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/classification/pca.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/__init__.py
--rw-r--r--   0        0        0    37929 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_base.py
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_batch.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_cache.py
--rw-r--r--   0        0        0    19585 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_group.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_loader.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_misc.py
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/loader/_mock.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/__init__.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_cut.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_group.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/_rotation.py
--rw-r--r--   0        0        0    33963 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/molecules/core.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/__init__.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/_base.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pick/_concrete.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/__init__.py
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_classes.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_curry.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_imread.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_masking.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/pipe/_transform.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/_templates.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.4.0/acryo/testing/core.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.4.0/.gitignore
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.4.0/LICENSE
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.4.0/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 acryo-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 acryo-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/__init__.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_dask.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_reader.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_rotation.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_typed_scipy.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_types.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/_utils.py
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/simulator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/alignment/__init__.py
+-rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/alignment/_base.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/alignment/_bound.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/alignment/_concrete.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/__init__.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/_api.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/_bandpass.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/_missing_wedge.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/_pcc.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/backend/_zncc.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/classification/__init__.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/classification/_dask_pca.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/classification/pca.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/__init__.py
+-rw-r--r--   0        0        0    37983 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_base.py
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_batch.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_cache.py
+-rw-r--r--   0        0        0    19585 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_group.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_loader.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_misc.py
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/loader/_mock.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/molecules/__init__.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/molecules/_cut.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/molecules/_group.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/molecules/_rotation.py
+-rw-r--r--   0        0        0    33963 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/molecules/core.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pick/__init__.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pick/_base.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pick/_concrete.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/__init__.py
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/_classes.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/_curry.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/_imread.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/_masking.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/pipe/_transform.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/testing/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/testing/_templates.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.4.1/acryo/testing/core.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.4.1/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 acryo-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 acryo-0.4.1/PKG-INFO
```

### Comparing `acryo-0.4.0/acryo/_dask.py` & `acryo-0.4.1/acryo/_dask.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/_reader.py` & `acryo-0.4.1/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/_rotation.py` & `acryo-0.4.1/acryo/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/_typed_scipy.py` & `acryo-0.4.1/acryo/_typed_scipy.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/_utils.py` & `acryo-0.4.1/acryo/_utils.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/simulator.py` & `acryo-0.4.1/acryo/simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/alignment/_base.py` & `acryo-0.4.1/acryo/alignment/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/alignment/_bound.py` & `acryo-0.4.1/acryo/alignment/_bound.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/alignment/_concrete.py` & `acryo-0.4.1/acryo/alignment/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/backend/_api.py` & `acryo-0.4.1/acryo/backend/_api.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/backend/_bandpass.py` & `acryo-0.4.1/acryo/backend/_bandpass.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/backend/_missing_wedge.py` & `acryo-0.4.1/acryo/backend/_missing_wedge.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/backend/_pcc.py` & `acryo-0.4.1/acryo/backend/_pcc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/backend/_zncc.py` & `acryo-0.4.1/acryo/backend/_zncc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/classification/_dask_pca.py` & `acryo-0.4.1/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/classification/pca.py` & `acryo-0.4.1/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_base.py` & `acryo-0.4.1/acryo/loader/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,16 @@
         if model.is_multi_templates:
             task_shape = (model.niter,) + tuple(
                 2 * np.ceil(_max_shifts_px).astype(np.int32) + 1
             )
         else:
             task_shape = tuple(2 * np.ceil(_max_shifts_px).astype(np.int32) + 1)
         task_arrays = (
-            self.iter_mapping_tasks(
+            self.replace(output_shape=model.input_shape)
+            .iter_mapping_tasks(
                 model.landscape,
                 max_shifts=_max_shifts_px,
                 upsample=upsample,
                 var_kwarg=dict(
                     quaternion=self.molecules.quaternion(),
                     pos=self.molecules.pos / self.scale,
                 ),
```

### Comparing `acryo-0.4.0/acryo/loader/_batch.py` & `acryo-0.4.1/acryo/loader/_batch.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_cache.py` & `acryo-0.4.1/acryo/loader/_cache.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_group.py` & `acryo-0.4.1/acryo/loader/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_loader.py` & `acryo-0.4.1/acryo/loader/_loader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_misc.py` & `acryo-0.4.1/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/loader/_mock.py` & `acryo-0.4.1/acryo/loader/_mock.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/molecules/_cut.py` & `acryo-0.4.1/acryo/molecules/_cut.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/molecules/_group.py` & `acryo-0.4.1/acryo/molecules/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/molecules/_rotation.py` & `acryo-0.4.1/acryo/molecules/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/molecules/core.py` & `acryo-0.4.1/acryo/molecules/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pick/_base.py` & `acryo-0.4.1/acryo/pick/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pick/_concrete.py` & `acryo-0.4.1/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/__init__.py` & `acryo-0.4.1/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/_classes.py` & `acryo-0.4.1/acryo/pipe/_classes.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/_curry.py` & `acryo-0.4.1/acryo/pipe/_curry.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/_imread.py` & `acryo-0.4.1/acryo/pipe/_imread.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/_masking.py` & `acryo-0.4.1/acryo/pipe/_masking.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/pipe/_transform.py` & `acryo-0.4.1/acryo/pipe/_transform.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/testing/_templates.py` & `acryo-0.4.1/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/acryo/testing/core.py` & `acryo-0.4.1/acryo/testing/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/.gitignore` & `acryo-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/LICENSE` & `acryo-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/README.md` & `acryo-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `acryo-0.4.0/pyproject.toml` & `acryo-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 [project]
 name = "acryo"
 dynamic = ["version"]
 description = "An extensible cryo-EM/ET toolkit for Python."
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
     { name = "Hanjin Liu", email = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp" },
 ]
 dependencies = [
     "dask>=2021.6.0",
     "numpy>=1.21",
     "polars>=0.17.3",
```

### Comparing `acryo-0.4.0/PKG-INFO` & `acryo-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.4.0
+Version: 0.4.1
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Hanjin Liu
         All rights reserved.
         
@@ -30,19 +30,18 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: dask>=2021.6.0
 Requires-Dist: numpy>=1.21
 Requires-Dist: polars>=0.17.3
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: typing-extensions>=4.1.1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == 'testing'
```

