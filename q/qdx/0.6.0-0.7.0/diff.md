# Comparing `tmp/qdx-0.6.0.tar.gz` & `tmp/qdx-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdx-0.6.0.tar", max compression
+gzip compressed data, was "qdx-0.7.0.tar", max compression
```

## Comparing `qdx-0.6.0.tar` & `qdx-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2183 2023-03-14 11:09:05.527233 qdx-0.6.0/README.md
--rw-r--r--   0        0        0     1834 2023-03-20 06:32:02.187932 qdx-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       83 2023-03-06 03:01:11.622918 qdx-0.6.0/qdx/__init__.py
--rw-r--r--   0        0        0     3034 2023-03-14 11:09:05.527233 qdx-0.6.0/qdx/__main__.py
--rw-r--r--   0        0        0    18633 2023-03-17 07:46:55.005859 qdx-0.6.0/qdx/api.py
--rw-r--r--   0        0        0     7340 2023-03-14 11:09:05.527233 qdx-0.6.0/qdx/calcq.py
--rw-r--r--   0        0        0    11129 2023-03-16 02:58:31.259202 qdx-0.6.0/qdx/data.py
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 qdx-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2183 2023-03-14 11:09:05.527233 qdx-0.7.0/README.md
+-rw-r--r--   0        0        0     1834 2023-03-23 11:53:54.374092 qdx-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-03-06 03:01:11.622918 qdx-0.7.0/qdx/__init__.py
+-rw-r--r--   0        0        0     3034 2023-03-14 11:09:05.527233 qdx-0.7.0/qdx/__main__.py
+-rw-r--r--   0        0        0    18604 2023-03-23 07:39:17.135882 qdx-0.7.0/qdx/api.py
+-rw-r--r--   0        0        0     7340 2023-03-14 11:09:05.527233 qdx-0.7.0/qdx/calcq.py
+-rw-r--r--   0        0        0    11176 2023-03-23 11:53:05.430605 qdx-0.7.0/qdx/data.py
+-rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 qdx-0.7.0/PKG-INFO
```

### Comparing `qdx-0.6.0/README.md` & `qdx-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `qdx-0.6.0/pyproject.toml` & `qdx-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 [tool.setuptools.packages]
 [tool.setuptools.packages.find]
 exclude = ["test", "tests"]
 where = [""]
 
 [tool.poetry]
 name = "qdx"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python SDK for interacting with the QDX API"
 authors = ["Ryan Swart <ryan@talosystems.com>"]
 readme = "README.md"
 packages = [{include = "qdx"}]
 
 [tool.poetry.scripts]
 qdx = "qdx.__main__:main"
```

### Comparing `qdx-0.6.0/qdx/__main__.py` & `qdx-0.7.0/qdx/__main__.py`

 * *Files identical despite different names*

### Comparing `qdx-0.6.0/qdx/api.py` & `qdx-0.7.0/qdx/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
         procs: dict[str, Any] | None = response.get("procs")
         if procs:
             procs = procs.get("nodes")
             if procs:
                 deserialized = [Proc.from_dict(proc) for proc in procs]
                 return deserialized
 
-        raise Exception("Failed to find task")
+        return []
 
     def start_ligand_prep(self, complex: Any, prep_for: PrepTypes, tags: list[str] = []):
         response = self.client.execute(
             prepare_ligand_mutation,
             variable_values={"complex": complex, "tags": tags, "prep_for": prep_for.upper()},
         )
```

### Comparing `qdx-0.6.0/qdx/calcq.py` & `qdx-0.7.0/qdx/calcq.py`

 * *Files identical despite different names*

### Comparing `qdx-0.6.0/qdx/data.py` & `qdx-0.7.0/qdx/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 class QCFrag(DataClassJsonMixin):
     """ "keywords.frag" in qc json"""
 
     reference_monomer: Optional[int] = None
     method: str = "MBE"
     level: int = 2
     ngpus_per_group: int = 4
+    new_reference_fragment: Optional[int] = None
     monomers_to_calculate: Optional[list[int]] = None
     monomer_cutoff: int = 40
     dimer_cutoff: int = 40
     dimer_mp2_cutoff: int = 40
     trimer_mp2_cutoff: int = 20
     lattice_energy_calc: bool = False
     trimer_cutoff: int = 30
@@ -330,15 +331,15 @@
     nmer_distances = []
     energy_type = "lattice"
     reference = None
 
     mp_os_total = 0
     mp_ss_total = 0
 
-    for (k, v) in results.nmer_hf_energies.items():
+    for k, v in results.nmer_hf_energies.items():
         mers = list(map(int, k.split(":")))
         if len(mers) > 1:
             if reference:
                 if reference != mers[0]:
                     energy_type = "SPE"
             else:
                 reference = mers[0]
```

### Comparing `qdx-0.6.0/PKG-INFO` & `qdx-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdx
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python SDK for interacting with the QDX API
 Author: Ryan Swart
 Author-email: ryan@talosystems.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

