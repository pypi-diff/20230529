# Comparing `tmp/pylibblkid-0.2.tar.gz` & `tmp/pylibblkid-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibblkid-0.2.tar", last modified: Sun Apr 10 14:24:38 2022, max compression
+gzip compressed data, was "pylibblkid-0.3.tar", last modified: Mon May 29 11:37:11 2023, max compression
```

## Comparing `pylibblkid-0.2.tar` & `pylibblkid-0.3.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxrwxr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2022-04-10 14:24:38.618913 pylibblkid-0.2/
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)    26526 2020-08-28 05:42:04.000000 pylibblkid-0.2/LICENSE
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      118 2022-04-10 14:11:38.000000 pylibblkid-0.2/MANIFEST.in
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1136 2020-10-29 15:39:56.000000 pylibblkid-0.2/Makefile
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      875 2022-04-10 14:24:38.618913 pylibblkid-0.2/PKG-INFO
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      287 2022-04-10 14:21:19.000000 pylibblkid-0.2/README.md
-drwxrwxr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2022-04-10 14:24:38.616913 pylibblkid-0.2/pylibblkid.egg-info/
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      875 2022-04-10 14:24:38.000000 pylibblkid-0.2/pylibblkid.egg-info/PKG-INFO
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      474 2022-04-10 14:24:38.000000 pylibblkid-0.2/pylibblkid.egg-info/SOURCES.txt
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)        1 2022-04-10 14:24:38.000000 pylibblkid-0.2/pylibblkid.egg-info/dependency_links.txt
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)       10 2022-04-10 14:24:38.000000 pylibblkid-0.2/pylibblkid.egg-info/requires.txt
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)        6 2022-04-10 14:24:38.000000 pylibblkid-0.2/pylibblkid.egg-info/top_level.txt
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)       38 2022-04-10 14:24:38.618913 pylibblkid-0.2/setup.cfg
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2393 2022-04-10 14:19:30.000000 pylibblkid-0.2/setup.py
-drwxrwxr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2022-04-10 14:24:38.618913 pylibblkid-0.2/src/
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     9687 2022-04-10 13:54:20.000000 pylibblkid-0.2/src/cache.c
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1243 2021-07-17 15:58:14.000000 pylibblkid-0.2/src/cache.h
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)    17730 2022-04-10 13:54:12.000000 pylibblkid-0.2/src/partitions.c
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2096 2021-07-11 13:09:20.000000 pylibblkid-0.2/src/partitions.h
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)    31108 2022-04-10 13:54:20.000000 pylibblkid-0.2/src/probe.c
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1173 2021-07-11 12:17:56.000000 pylibblkid-0.2/src/probe.h
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)    20661 2022-04-10 13:54:20.000000 pylibblkid-0.2/src/pyblkid.c
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      843 2020-08-28 06:18:14.000000 pylibblkid-0.2/src/pyblkid.h
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     4630 2021-07-31 17:27:22.000000 pylibblkid-0.2/src/topology.c
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1211 2020-10-29 15:39:56.000000 pylibblkid-0.2/src/topology.h
-drwxrwxr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2022-04-10 14:24:38.618913 pylibblkid-0.2/tests/
--rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2020-09-30 17:08:52.000000 pylibblkid-0.2/tests/__init__.py
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     3247 2022-04-10 13:54:20.000000 pylibblkid-0.2/tests/test_blkid.py
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2001 2022-04-10 13:54:20.000000 pylibblkid-0.2/tests/test_cache.py
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     4273 2022-04-10 13:54:12.000000 pylibblkid-0.2/tests/test_partitions.py
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     7294 2022-04-10 13:54:20.000000 pylibblkid-0.2/tests/test_probe.py
--rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1187 2021-07-18 16:02:09.000000 pylibblkid-0.2/tests/utils.py
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.481067 pylibblkid-0.3/
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.478067 pylibblkid-0.3/.github/
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.479067 pylibblkid-0.3/.github/workflows/
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      466 2023-04-12 13:22:07.000000 pylibblkid-0.3/.github/workflows/ci.yml
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     1023 2023-05-29 11:31:52.000000 pylibblkid-0.3/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)       46 2020-10-29 15:39:56.000000 pylibblkid-0.3/.gitignore
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)    26526 2020-08-28 05:42:04.000000 pylibblkid-0.3/LICENSE
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      118 2022-04-10 14:11:38.000000 pylibblkid-0.3/MANIFEST.in
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1136 2020-10-29 15:39:56.000000 pylibblkid-0.3/Makefile
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      974 2023-05-29 11:37:11.480067 pylibblkid-0.3/PKG-INFO
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)      384 2022-04-10 14:26:09.000000 pylibblkid-0.3/README.md
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.479067 pylibblkid-0.3/pylibblkid.egg-info/
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      974 2023-05-29 11:37:11.000000 pylibblkid-0.3/pylibblkid.egg-info/PKG-INFO
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      565 2023-05-29 11:37:11.000000 pylibblkid-0.3/pylibblkid.egg-info/SOURCES.txt
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        1 2023-05-29 11:37:11.000000 pylibblkid-0.3/pylibblkid.egg-info/dependency_links.txt
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        6 2023-05-29 11:37:11.000000 pylibblkid-0.3/pylibblkid.egg-info/top_level.txt
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       94 2023-05-29 11:31:52.000000 pylibblkid-0.3/pyproject.toml
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)       38 2023-05-29 11:37:11.481067 pylibblkid-0.3/setup.cfg
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3083 2023-05-29 11:33:38.000000 pylibblkid-0.3/setup.py
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.480067 pylibblkid-0.3/src/
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     9687 2022-04-10 13:54:20.000000 pylibblkid-0.3/src/cache.c
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1243 2021-07-17 15:58:14.000000 pylibblkid-0.3/src/cache.h
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    17790 2023-05-29 11:31:52.000000 pylibblkid-0.3/src/partitions.c
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2096 2021-07-11 13:09:20.000000 pylibblkid-0.3/src/partitions.h
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    31427 2023-05-29 11:31:52.000000 pylibblkid-0.3/src/probe.c
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1173 2021-07-11 12:17:56.000000 pylibblkid-0.3/src/probe.h
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)    20928 2023-05-29 11:31:52.000000 pylibblkid-0.3/src/pyblkid.c
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)      843 2020-08-28 06:18:14.000000 pylibblkid-0.3/src/pyblkid.h
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4632 2023-05-29 11:31:52.000000 pylibblkid-0.3/src/topology.c
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1211 2020-10-29 15:39:56.000000 pylibblkid-0.3/src/topology.h
+drwxr-xr-x   0 vtrefny   (1001) vtrefny   (1001)        0 2023-05-29 11:37:11.480067 pylibblkid-0.3/tests/
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)        0 2020-09-30 17:08:52.000000 pylibblkid-0.3/tests/__init__.py
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2140 2021-07-11 12:17:56.000000 pylibblkid-0.3/tests/gpt.img.xz
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1612 2020-09-30 17:23:34.000000 pylibblkid-0.3/tests/test.img.xz
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     3301 2023-05-29 11:31:52.000000 pylibblkid-0.3/tests/test_blkid.py
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     2001 2022-04-10 13:54:20.000000 pylibblkid-0.3/tests/test_cache.py
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     4359 2023-05-29 11:31:52.000000 pylibblkid-0.3/tests/test_partitions.py
+-rw-r--r--   0 vtrefny   (1001) vtrefny   (1001)     7574 2023-05-29 11:31:52.000000 pylibblkid-0.3/tests/test_probe.py
+-rw-rw-r--   0 vtrefny   (1001) vtrefny   (1001)     1187 2021-07-18 16:02:09.000000 pylibblkid-0.3/tests/utils.py
```

### Comparing `pylibblkid-0.2/LICENSE` & `pylibblkid-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/Makefile` & `pylibblkid-0.3/Makefile`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/PKG-INFO` & `pylibblkid-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pylibblkid
-Version: 0.2
+Version: 0.3
 Summary: Python interface for the libblkid C library
-Home-page: UNKNOWN
+Home-page: http://github.com/vojtechtrefny/pyblkid
 Author: Vojtech Trefny
 Author-email: vtrefny@redhat.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylibblkid
 
+[![PyPI version](https://badge.fury.io/py/pylibblkid.svg)](https://badge.fury.io/py/pylibblkid)
+
 Python bindings for libblkid library.
 
 ```python
 import blkid
 
 pr = blkid.Probe()
 pr.set_device("/dev/sda1")
@@ -30,9 +30,7 @@
 pr.set_superblocks_flags(blkid.SUBLKS_TYPE | blkid.SUBLKS_USAGE | blkid.SUBLKS_UUID)
 
 pr.do_safeprobe()
 
 # print usage
 pr["USAGE"]
 ```
-
-
```

### Comparing `pylibblkid-0.2/pylibblkid.egg-info/PKG-INFO` & `pylibblkid-0.3/pylibblkid.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pylibblkid
-Version: 0.2
+Version: 0.3
 Summary: Python interface for the libblkid C library
-Home-page: UNKNOWN
+Home-page: http://github.com/vojtechtrefny/pyblkid
 Author: Vojtech Trefny
 Author-email: vtrefny@redhat.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylibblkid
 
+[![PyPI version](https://badge.fury.io/py/pylibblkid.svg)](https://badge.fury.io/py/pylibblkid)
+
 Python bindings for libblkid library.
 
 ```python
 import blkid
 
 pr = blkid.Probe()
 pr.set_device("/dev/sda1")
@@ -30,9 +30,7 @@
 pr.set_superblocks_flags(blkid.SUBLKS_TYPE | blkid.SUBLKS_USAGE | blkid.SUBLKS_UUID)
 
 pr.do_safeprobe()
 
 # print usage
 pr["USAGE"]
 ```
-
-
```

### Comparing `pylibblkid-0.2/setup.py` & `pylibblkid-0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,51 +9,70 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, see <http://www.gnu.org/licenses/>.
 
+import sys
+
 import pkgconfig
+from setuptools import Extension, setup
 
-from setuptools import setup, Extension
+pkgs = pkgconfig.list_all()
+if "blkid" not in pkgs:
+    print("Please install libblkid-dev or libblkid-devel")
+    exit(1)
 
+vers = sys.version_info
+if f"python-{vers.major}.{vers.minor}" not in pkgs:
+    print("Please install python3-dev or python3-devel")
+    exit(1)
 
-macros = []
 
-if pkgconfig.installed("blkid", ">= 2.36"):
-    macros.append(("HAVE_BLKID2360", "1"))
+# define macros for blkid releases
+macros = []
+blkid_releases = ['2.24', '2.25', '2.30', '2.31', '2.36', '2.37', '2.39']
+for blkid_ver in blkid_releases:
+    if pkgconfig.installed("blkid", f">= {blkid_ver}"):
+        ver_list = blkid_ver.split('.')
+        full_release = '_'.join(ver_list)
+        macros.append((f"HAVE_BLKID_{full_release}", "1"))
+        if len(ver_list) > 2:
+            major_minor = '_'.join(ver_list[:2])
+            macros.append((f"HAVE_BLKID_{major_minor}", "1"))
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def main():
     setup(name="pylibblkid",
-          version="0.2",
+          version="0.3",
           description="Python interface for the libblkid C library",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Vojtech Trefny",
           author_email="vtrefny@redhat.com",
+          url="http://github.com/vojtechtrefny/pyblkid",
           ext_modules=[Extension("blkid",
-                                 sources = ["src/pyblkid.c",
-                                            "src/topology.c",
-                                            "src/partitions.c",
-                                            "src/cache.c",
-                                            "src/probe.c",],
-                                 include_dirs = ["/usr/include"],
-                                 libraries = ["blkid"],
-                                 library_dirs = ["/usr/lib"],
+                                 sources=["src/pyblkid.c",
+                                          "src/topology.c",
+                                          "src/partitions.c",
+                                          "src/cache.c",
+                                          "src/probe.c",],
+                                 include_dirs=["/usr/include"],
+                                 libraries=["blkid"],
+                                 library_dirs=["/usr/lib"],
                                  define_macros=macros,
-                                 extra_compile_args = ["-Wall", "-Wextra", "-Werror"])],
-          install_requires=["pkgconfig"],
-          classifiers=["Development Status :: 3 - Alpha",
+                                 extra_compile_args=["-std=c99", "-Wall", "-Wextra", "-Werror"])],
+          classifiers=["Development Status :: 4 - Beta",
                        "Intended Audience :: Developers",
-                       "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
+                       "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
                        "Programming Language :: C",
                        "Programming Language :: Python :: 3",
                        "Operating System :: POSIX :: Linux"])
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `pylibblkid-0.2/src/cache.c` & `pylibblkid-0.3/src/cache.c`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/src/cache.h` & `pylibblkid-0.3/src/cache.h`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/src/partitions.c` & `pylibblkid-0.3/src/partitions.c`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     result->number = partnum;
     result->partition = blkid_part;
     result->Parttable_object = NULL;
 
     return (PyObject *) result;
 }
 
+#ifdef HAVE_BLKID_2_25
 PyDoc_STRVAR(Partlist_get_partition_by_partno__doc__,
 "get_partition_by_partno(number)\n\n"
 "Get partition by partition number.\n\n"
 "This does not assume any order of partitions and correctly handles \"out of order\" "
 "partition tables. partition N is located after partition N+1 on the disk.");
 static PyObject *Partlist_get_partition_by_partno (PartlistObject *self, PyObject *args, PyObject *kwargs) {
     char *kwlist[] = { "number", NULL };
@@ -147,14 +148,15 @@
 
     result->number = partno;
     result->partition = blkid_part;
     result->Parttable_object = NULL;
 
     return (PyObject *) result;
 }
+#endif
 
 static int _Py_Dev_Converter (PyObject *obj, void *p) {
 #ifdef HAVE_LONG_LONG
     *((dev_t *)p) = PyLong_AsUnsignedLongLong (obj);
 #else
     *((dev_t *)p) = PyLong_AsUnsignedLong (obj);
 #endif
@@ -198,15 +200,17 @@
     result->Parttable_object = NULL;
 
     return (PyObject *) result;
 }
 
 static PyMethodDef Partlist_methods[] = {
     {"get_partition", (PyCFunction)(void(*)(void)) Partlist_get_partition, METH_VARARGS|METH_KEYWORDS, Partlist_get_partition__doc__},
+#ifdef HAVE_BLKID_2_25
     {"get_partition_by_partno", (PyCFunction)(void(*)(void)) Partlist_get_partition_by_partno, METH_VARARGS|METH_KEYWORDS, Partlist_get_partition_by_partno__doc__},
+#endif
     {"devno_to_partition", (PyCFunction)(void(*)(void)) Partlist_devno_to_partition, METH_VARARGS|METH_KEYWORDS, Partlist_devno_to_partition__doc__},
     {NULL, NULL, 0, NULL},
 };
 
 static PyObject *Partlist_get_table (PartlistObject *self, PyObject *Py_UNUSED (ignored)) {
     if (self->Parttable_object) {
         Py_INCREF (self->Parttable_object);
```

### Comparing `pylibblkid-0.2/src/partitions.h` & `pylibblkid-0.3/src/partitions.h`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/src/probe.c` & `pylibblkid-0.3/src/probe.c`

 * *Files 2% similar despite different names*

```diff
@@ -548,14 +548,15 @@
         PyErr_SetString (PyExc_RuntimeError, "Failed to step back the probe");
         return NULL;
     }
 
     Py_RETURN_NONE;
 }
 
+#ifdef HAVE_BLKID_2_31
 PyDoc_STRVAR(Probe_reset_buffers__doc__,
 "reset_buffers ()\n\n"
 "libblkid reuse all already read buffers from the device. The buffers may be modified by Probe.hide_range().\n"
 "This function reset and free all cached buffers. The next Probe.do_probe() will read all data from the device.");
 static PyObject *Probe_reset_buffers (ProbeObject *self, PyObject *Py_UNUSED (ignored)) {
     int ret = 0;
 
@@ -563,14 +564,15 @@
     if (ret != 0) {
         PyErr_SetString (PyExc_RuntimeError, "Failed to reset buffers");
         return NULL;
     }
 
     Py_RETURN_NONE;
 }
+#endif
 
 PyDoc_STRVAR(Probe_reset_probe__doc__,
 "reset_probe ()\n\n"
 "Zeroize probing results and resets the current probing (this has impact to do_probe() only).\n"
 "This function does not touch probing filters and keeps assigned device.");
 static PyObject *Probe_reset_probe (ProbeObject *self, PyObject *Py_UNUSED (ignored)) {
     blkid_reset_probe (self->probe);
@@ -584,14 +586,15 @@
         Py_DECREF (self->partlist);
         self->partlist = NULL;
     }
 
     Py_RETURN_NONE;
 }
 
+#ifdef HAVE_BLKID_2_31
 PyDoc_STRVAR(Probe_hide_range__doc__,
 "hide_range (offset, length)\n\n" \
 "This function modifies in-memory cached data from the device. The specified range is zeroized. "
 "This is usable together with Probe.step_back(). The next Probe.do_probe() will not see specified area.\n"
 "Note that this is usable for already (by library) read data, and this function is not a way "
 "how to hide any large areas on your device.\n"
 "The function Probe.reset_buffers() reverts all.");
@@ -609,14 +612,15 @@
     if (ret != 0) {
         PyErr_SetString (PyExc_RuntimeError, "Failed to hide range");
         return NULL;
     }
 
     Py_RETURN_NONE;
 }
+#endif
 
 PyDoc_STRVAR(Probe_do_wipe__doc__,
 "do_wipe (dryrun=False)\n\n"
 "This function erases the current signature detected by the probe. The probe has to be open in "
 "O_RDWR mode, blkid.SUBLKS_MAGIC or/and blkid.PARTS_MAGIC flags has to be enabled (if you want "
 "to erase also superblock with broken check sums then use blkid.SUBLKS_BADCSUM too).\n\n"
 "After successful signature removing the probe prober will be moved one step back and the next "
@@ -725,17 +729,21 @@
 
 static PyMethodDef Probe_methods[] = {
     {"set_device", (PyCFunction)(void(*)(void)) Probe_set_device, METH_VARARGS|METH_KEYWORDS, Probe_set_device__doc__},
     {"do_safeprobe", (PyCFunction) Probe_do_safeprobe, METH_NOARGS, Probe_do_safeprobe__doc__},
     {"do_fullprobe", (PyCFunction) Probe_do_fullprobe, METH_NOARGS, Probe_do_fullprobe__doc__},
     {"do_probe", (PyCFunction) Probe_do_probe, METH_NOARGS, Probe_do_probe__doc__},
     {"step_back", (PyCFunction) Probe_step_back, METH_NOARGS, Probe_step_back__doc__},
+#ifdef HAVE_BLKID_2_31
     {"reset_buffers", (PyCFunction) Probe_reset_buffers, METH_NOARGS, Probe_reset_buffers__doc__},
+#endif
     {"reset_probe", (PyCFunction) Probe_reset_probe, METH_NOARGS, Probe_reset_probe__doc__},
+#ifdef HAVE_BLKID_2_31
     {"hide_range", (PyCFunction)(void(*)(void)) Probe_hide_range, METH_VARARGS|METH_KEYWORDS, Probe_hide_range__doc__},
+#endif
     {"do_wipe", (PyCFunction)(void(*)(void)) Probe_do_wipe, METH_VARARGS|METH_KEYWORDS, Probe_do_wipe__doc__},
     {"enable_partitions", (PyCFunction)(void(*)(void)) Probe_enable_partitions, METH_VARARGS|METH_KEYWORDS, Probe_enable_partitions__doc__},
     {"set_partitions_flags", (PyCFunction)(void(*)(void)) Probe_set_partitions_flags, METH_VARARGS|METH_KEYWORDS, Probe_set_partitions_flags__doc__},
     {"filter_partitions_type", (PyCFunction)(void(*)(void)) Probe_filter_partitions_type, METH_VARARGS|METH_KEYWORDS, Probe_filter_partitions_type__doc__},
     {"invert_partitions_filter", (PyCFunction) Probe_invert_partitions_filter, METH_NOARGS, Probe_invert_partitions_filter__doc__},
     {"reset_partitions_filter", (PyCFunction) Probe_reset_partitions_filter, METH_NOARGS, Probe_reset_partitions_filter__doc__},
     {"enable_topology", (PyCFunction)(void(*)(void)) Probe_enable_topology, METH_VARARGS|METH_KEYWORDS, Probe_enable_topology__doc__},
@@ -782,14 +790,15 @@
 
 static PyObject *Probe_get_sector_size (ProbeObject *self, PyObject *Py_UNUSED (ignored)) {
 	unsigned int sector_size = blkid_probe_get_sectorsize (self->probe);
 
     return PyLong_FromUnsignedLong (sector_size);
 }
 
+#ifdef HAVE_BLKID_2_30
 static int Probe_set_sector_size (ProbeObject *self, PyObject *value, void *closure UNUSED) {
 	unsigned int sector_size = 0;
     int ret = 0;
 
     if (!PyLong_Check (value)) {
 		PyErr_SetString (PyExc_TypeError, "Invalid argument");
 
@@ -802,14 +811,15 @@
     if (ret != 0) {
         PyErr_Format (PyExc_RuntimeError, "Failed to set sector size");
         return -1;
     }
 
     return 0;
 }
+#endif
 
 static PyObject *Probe_get_wholedisk_devno (ProbeObject *self, PyObject *Py_UNUSED (ignored)) {
     dev_t devno = blkid_probe_get_wholedisk_devno (self->probe);
 
     return PyLong_FromUnsignedLong (devno);
 }
 
@@ -843,15 +853,19 @@
 
 static PyGetSetDef Probe_getseters[] = {
     {"devno", (getter) Probe_get_devno, NULL, "block device number, or 0 for regular files", NULL},
     {"fd", (getter) Probe_get_fd, NULL, "file descriptor for assigned device/file or -1 in case of error", NULL},
     {"offset", (getter) Probe_get_offset, NULL, "offset of probing area as defined by Probe.set_device() or -1 in case of error", NULL},
     {"sectors", (getter) Probe_get_sectors, NULL, "512-byte sector count or -1 in case of error", NULL},
     {"size", (getter) Probe_get_size, NULL, "size of probing area as defined by Probe.set_device()", NULL},
+#ifdef HAVE_BLKID_2_30
     {"sector_size", (getter) Probe_get_sector_size, (setter) Probe_set_sector_size, "block device logical sector size (BLKSSZGET ioctl, default 512).", NULL},
+#else
+    {"sector_size", (getter) Probe_get_sector_size, NULL, "block device logical sector size (BLKSSZGET ioctl, default 512).", NULL},
+#endif
     {"wholedisk_devno", (getter) Probe_get_wholedisk_devno, NULL, "device number of the wholedisk, or 0 for regular files", NULL},
     {"is_wholedisk", (getter) Probe_get_is_wholedisk, NULL, "True if the device is whole-disk, False otherwise", NULL},
     {"topology", (getter) Probe_get_topology, NULL, "binary interface for topology values", NULL},
     {"partitions", (getter) Probe_get_partitions, NULL, "binary interface for partitions", NULL},
     {NULL, NULL, NULL, NULL, NULL}
 };
```

### Comparing `pylibblkid-0.2/src/probe.h` & `pylibblkid-0.3/src/probe.h`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/src/pyblkid.c` & `pylibblkid-0.3/src/pyblkid.c`

 * *Files 1% similar despite different names*

```diff
@@ -136,24 +136,32 @@
 PyDoc_STRVAR(Blkid_devno_to_wholedisk__doc__,
 "devno_to_wholedisk (devno)\n\n"
 "This function uses sysfs to convert the devno device number to the name and devno of the whole disk.");
 static PyObject *Blkid_devno_to_wholedisk (PyObject *self UNUSED, PyObject *args, PyObject *kwargs) {
     dev_t devno = 0;
     dev_t diskdevno = 0;
     char *kwlist[] = { "devno", NULL };
+#ifdef HAVE_BLKID_2_28
     char diskname[32];
+#else
+    char diskname[PATH_MAX];
+#endif
     int ret = 0;
     PyObject *tuple = NULL;
     PyObject *py_name = NULL;
     PyObject *py_devno = NULL;
 
     if (!PyArg_ParseTupleAndKeywords (args, kwargs, "O&:devno_to_wholedisk", kwlist, _Py_Dev_Converter, &devno))
         return NULL;
 
+#ifdef HAVE_BLKID_2_28
     ret = blkid_devno_to_wholedisk (devno, diskname, 32, &diskdevno);
+#else
+    ret = blkid_devno_to_wholedisk (devno, diskname, PATH_MAX, &diskdevno);
+#endif
     if (ret != 0) {
         PyErr_SetString (PyExc_RuntimeError, "Failed to get whole disk name");
         return NULL;
     }
 
     tuple = PyTuple_New (2);
 
@@ -358,14 +366,15 @@
 
     py_ret = PyUnicode_FromString (safe_string);
     free (safe_string);
 
     return py_ret;
 }
 
+#ifdef HAVE_BLKID_2_30
 PyDoc_STRVAR(Blkid_partition_types__doc__,
 "partition_types ()\n\n"
 "List of supported partition types.\n");
 static PyObject *Blkid_partition_types (ProbeObject *self UNUSED, PyObject *Py_UNUSED (ignored)) {
     PyObject *ret = NULL;
     PyObject *py_name = NULL;
     size_t idx = 0;
@@ -377,14 +386,15 @@
         py_name = PyUnicode_FromString (name);
         if (py_name != NULL)
             PyList_Append (ret, py_name);
     }
 
     return ret;
 }
+#endif
 
 PyDoc_STRVAR(Blkid_superblocks__doc__,
 "superblocks ()\n\n"
 "List of supported superblocks.\n");
 static PyObject *Blkid_superblocks (ProbeObject *self UNUSED, PyObject *Py_UNUSED (ignored)) {
     PyObject *ret = NULL;
     PyObject *py_name = NULL;
@@ -464,15 +474,17 @@
     {"known_pttype", (PyCFunction)(void(*)(void)) Blkid_known_pttype, METH_VARARGS|METH_KEYWORDS, Blkid_known_pttype__doc__},
     {"parse_version_string", (PyCFunction)(void(*)(void)) Blkid_parse_version_string, METH_VARARGS|METH_KEYWORDS, Blkid_parse_version_string__doc__},
     {"get_library_version", (PyCFunction) Blkid_get_library_version, METH_NOARGS, Blkid_get_library_version__doc__},
     {"parse_tag_string", (PyCFunction)(void(*)(void)) Blkid_parse_tag_string, METH_VARARGS|METH_KEYWORDS, Blkid_parse_tag_string__doc__},
     {"get_dev_size", (PyCFunction)(void(*)(void)) Blkid_get_dev_size, METH_VARARGS|METH_KEYWORDS, Blkid_get_dev_size__doc__},
     {"encode_string", (PyCFunction)(void(*)(void)) Blkid_encode_string, METH_VARARGS|METH_KEYWORDS, Blkid_encode_string__doc__},
     {"safe_string", (PyCFunction)(void(*)(void)) Blkid_safe_string, METH_VARARGS|METH_KEYWORDS, Blkid_safe_string__doc__},
+#ifdef HAVE_BLKID_2_30
     {"partition_types", (PyCFunction) Blkid_partition_types, METH_NOARGS, Blkid_partition_types__doc__},
+#endif
     {"superblocks", (PyCFunction) Blkid_superblocks, METH_NOARGS, Blkid_superblocks__doc__},
     {"evaluate_tag", (PyCFunction)(void(*)(void)) Blkid_evaluate_tag, METH_VARARGS|METH_KEYWORDS, Blkid_evaluate_tag__doc__},
     {"evaluate_spec", (PyCFunction)(void(*)(void)) Blkid_evaluate_spec, METH_VARARGS|METH_KEYWORDS, Blkid_evaluate_spec__doc__},
     {NULL, NULL, 0, NULL}
 };
 
 static struct PyModuleDef blkidmodule = {
@@ -519,15 +531,17 @@
     PyModule_AddIntConstant (module, "DEV_NORMAL", BLKID_DEV_NORMAL);
     PyModule_AddIntConstant (module, "DEV_VERIFY", BLKID_DEV_VERIFY);
 
     PyModule_AddIntConstant (module, "PARTS_ENTRY_DETAILS", BLKID_PARTS_ENTRY_DETAILS);
     PyModule_AddIntConstant (module, "PARTS_FORCE_GPT", BLKID_PARTS_FORCE_GPT);
     PyModule_AddIntConstant (module, "PARTS_MAGIC", BLKID_PARTS_MAGIC);
 
+#ifdef HAVE_BLKID_2_24
     PyModule_AddIntConstant (module, "SUBLKS_BADCSUM", BLKID_SUBLKS_BADCSUM);
+#endif
     PyModule_AddIntConstant (module, "SUBLKS_DEFAULT", BLKID_SUBLKS_DEFAULT);
     PyModule_AddIntConstant (module, "SUBLKS_LABEL", BLKID_SUBLKS_LABEL);
     PyModule_AddIntConstant (module, "SUBLKS_LABELRAW", BLKID_SUBLKS_LABELRAW);
     PyModule_AddIntConstant (module, "SUBLKS_MAGIC", BLKID_SUBLKS_MAGIC);
     PyModule_AddIntConstant (module, "SUBLKS_SECTYPE", BLKID_SUBLKS_SECTYPE);
     PyModule_AddIntConstant (module, "SUBLKS_TYPE", BLKID_SUBLKS_TYPE);
     PyModule_AddIntConstant (module, "SUBLKS_USAGE", BLKID_SUBLKS_USAGE);
```

### Comparing `pylibblkid-0.2/src/pyblkid.h` & `pylibblkid-0.3/src/pyblkid.h`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/src/topology.c` & `pylibblkid-0.3/src/topology.c`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 static PyObject *Topology_get_physical_sector_size (TopologyObject *self, PyObject *Py_UNUSED (ignored)) {
     unsigned long physical_sector_size = blkid_topology_get_physical_sector_size (self->topology);
 
     return PyLong_FromUnsignedLong (physical_sector_size);
 }
 
-#ifdef HAVE_BLKID2360
+#ifdef HAVE_BLKID_2_36
 static PyObject *Topology_get_dax (TopologyObject *self, PyObject *Py_UNUSED (ignored)) {
     int dax = blkid_topology_get_dax (self->topology);
 
     if (dax == 1)
         Py_RETURN_TRUE;
     else
         Py_RETURN_FALSE;
@@ -107,15 +107,15 @@
 
 static PyGetSetDef Topology_getseters[] = {
     {"alignment_offset", (getter) Topology_get_alignment_offset, NULL, "alignment offset in bytes or 0", NULL},
     {"logical_sector_size", (getter) Topology_get_logical_sector_size, NULL, "logical sector size (BLKSSZGET ioctl) in bytes or 0", NULL},
     {"minimum_io_size", (getter) Topology_get_minimum_io_size, NULL, "minimum io size in bytes or 0", NULL},
     {"optimal_io_size", (getter) Topology_get_optimal_io_size, NULL, "optimal io size in bytes or 0", NULL},
     {"physical_sector_size", (getter) Topology_get_physical_sector_size, NULL, "logical sector size (BLKSSZGET ioctl) in bytes or 0", NULL},
-#ifdef HAVE_BLKID2360
+#ifdef HAVE_BLKID_2_36
     {"dax", (getter) Topology_get_dax, NULL, "whether DAX is supported or not", NULL},
 #endif
     {NULL, NULL, NULL, NULL, NULL}
 };
 
 PyTypeObject TopologyType = {
     PyVarObject_HEAD_INIT (NULL, 0)
```

### Comparing `pylibblkid-0.2/src/topology.h` & `pylibblkid-0.3/src/topology.h`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/tests/test_blkid.py` & `pylibblkid-0.3/tests/test_blkid.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
         self.assertEqual(ttype, "NAME")
         self.assertEqual(tvalue, "test")
 
         size = blkid.get_dev_size(self.loop_dev)
         self.assertEqual(size, 2097152)  # test.img is 2 MiB
 
         # dos should be always supported so we can use it here to test
-        types = blkid.partition_types()
-        self.assertIn("dos", types)
+        if hasattr(blkid, "partition_types"):
+            types = blkid.partition_types()
+            self.assertIn("dos", types)
 
         # ext4 should be always supported so we can use it here to test
         supers = blkid.superblocks()
         self.assertIn("ext4", supers)
 
     def test_uevent(self):
         with self.assertRaises(RuntimeError):
```

### Comparing `pylibblkid-0.2/tests/test_cache.py` & `pylibblkid-0.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pylibblkid-0.2/tests/test_partitions.py` & `pylibblkid-0.3/tests/test_partitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,17 @@
         self.assertFalse(part.is_logical)
         self.assertEqual(part.name, "ThisIsName")
         self.assertEqual(part.flags, 0)
         self.assertEqual(part.partno, 1)
         self.assertEqual(part.start, 34)
         self.assertEqual(part.size, 2014)
 
+        if not hasattr(pr.partitions, "get_partition_by_partno"):
+            return
+
         part = pr.partitions.get_partition_by_partno(1)
         self.assertEqual(part.uuid, "1dcf10bc-637e-4c52-8203-087ae10a820b")
 
         # no nested partition table here, just the gpt
         table = part.table
         self.assertEqual(table.type, "gpt")
```

### Comparing `pylibblkid-0.2/tests/test_probe.py` & `pylibblkid-0.3/tests/test_probe.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     loop_dev = None
 
     @classmethod
     def setUpClass(cls):
         test_dir = os.path.abspath(os.path.dirname(__file__))
         cls.loop_dev = utils.loop_setup(os.path.join(test_dir, cls.test_image))
 
+        cls.ver_code, _version, _date = blkid.get_library_version()
+
     @classmethod
     def tearDownClass(cls):
         if cls.loop_dev:
             utils.loop_teardown(cls.loop_dev)
 
     def test_probe(self):
         pr = blkid.Probe()
@@ -33,16 +35,20 @@
 
         self.assertGreater(pr.fd, 0)
         self.assertNotEqual(pr.devno, 0)
         self.assertNotEqual(pr.wholedisk_devno, 0)
 
         self.assertTrue(pr.is_wholedisk)
 
-        pr.sector_size = 4096
-        self.assertEqual(pr.sector_size, 4096)
+        if self.ver_code >= 2300:
+            pr.sector_size = 4096
+            self.assertEqual(pr.sector_size, 4096)
+        else:
+            with self.assertRaises(AttributeError):
+                pr.sector_size = 4096
 
         pr.reset_probe()
 
     def test_probing(self):
         pr = blkid.Probe()
         pr.set_device(self.loop_dev)
 
@@ -58,32 +64,35 @@
         pr.step_back()
         ret = pr.do_probe()
         self.assertTrue(ret)
 
         usage = pr.lookup_value("USAGE")
         self.assertEqual(usage, b"filesystem")
 
-        pr.reset_buffers()
+        if hasattr(pr, "reset_buffers"):
+            pr.reset_buffers()
+
         pr.step_back()
         ret = pr.do_probe()
         self.assertTrue(ret)
 
         usage = pr.lookup_value("USAGE")
         self.assertEqual(usage, b"filesystem")
 
-        offset = pr.lookup_value("SBMAGIC_OFFSET")
-        magic = pr.lookup_value("SBMAGIC")
-        pr.hide_range(int(offset), len(magic))
-
-        pr.step_back()
-        ret = pr.do_probe()
-        self.assertFalse(ret)
+        if hasattr(pr, "hide_range"):
+            offset = pr.lookup_value("SBMAGIC_OFFSET")
+            magic = pr.lookup_value("SBMAGIC")
+            pr.hide_range(int(offset), len(magic))
+
+            pr.step_back()
+            ret = pr.do_probe()
+            self.assertFalse(ret)
 
-        with self.assertRaises(RuntimeError):
-            usage = pr.lookup_value("USAGE")
+            with self.assertRaises(RuntimeError):
+                usage = pr.lookup_value("USAGE")
 
     def test_safe_probing(self):
         pr = blkid.Probe()
         pr.set_device(self.loop_dev)
 
         pr.enable_superblocks(True)
         pr.set_superblocks_flags(blkid.SUBLKS_TYPE | blkid.SUBLKS_USAGE | blkid.SUBLKS_UUID)
@@ -232,16 +241,15 @@
 
         self.assertEqual(pr.topology.alignment_offset, 0)
         self.assertEqual(pr.topology.logical_sector_size, 512)
         self.assertEqual(pr.topology.minimum_io_size, 512)
         self.assertEqual(pr.topology.optimal_io_size, 0)
         self.assertEqual(pr.topology.physical_sector_size, 512)
 
-        code, _version, _date = blkid.get_library_version()
-        if code >= 2360:
+        if self.ver_code >= 2360:
             self.assertFalse(pr.topology.dax)
         else:
             with self.assertRaises(AttributeError):
                 self.assertIsNone(pr.topology.dax)
 
 
 if __name__ == "__main__":
```

### Comparing `pylibblkid-0.2/tests/utils.py` & `pylibblkid-0.3/tests/utils.py`

 * *Files identical despite different names*

