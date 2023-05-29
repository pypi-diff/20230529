# Comparing `tmp/delta-sharing-0.6.5.tar.gz` & `tmp/delta-sharing-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/delta-sharing-0.6.5.tar", last modified: Sun May 28 09:05:42 2023, max compression
+gzip compressed data, was "dist/delta-sharing-0.6.6.tar", last modified: Mon May 29 17:55:45 2023, max compression
```

## Comparing `delta-sharing-0.6.5.tar` & `delta-sharing-0.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1099 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    11137 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7819 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     7712 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    14850 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-05-28 09:04:20.000000 delta-sharing-0.6.5/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      419 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-05-28 09:05:42.000000 delta-sharing-0.6.5/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-05-12 09:10:25.000000 delta-sharing-0.6.5/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1099 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    11137 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7819 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     7712 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    14850 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-05-29 17:54:26.000000 delta-sharing-0.6.6/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2257 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      419 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-05-29 17:55:45.000000 delta-sharing-0.6.6/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-05-12 09:10:25.000000 delta-sharing-0.6.6/setup.py
```

### Comparing `delta-sharing-0.6.5/PKG-INFO` & `delta-sharing-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.6.5/README.md` & `delta-sharing-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/__init__.py` & `delta-sharing-0.6.6/delta_sharing/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/_yarl_patch.py` & `delta-sharing-0.6.6/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/converter.py` & `delta-sharing-0.6.6/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/delta_sharing.py` & `delta-sharing-0.6.6/delta_sharing/delta_sharing.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/protocol.py` & `delta-sharing-0.6.6/delta_sharing/protocol.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/reader.py` & `delta-sharing-0.6.6/delta_sharing/reader.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/rest_client.py` & `delta-sharing-0.6.6/delta_sharing/rest_client.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-0.6.5/delta_sharing/version.py` & `delta-sharing-0.6.6/delta_sharing/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.6.5"
+__version__ = "0.6.6"
```

### Comparing `delta-sharing-0.6.5/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-0.6.6/delta_sharing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-0.6.5/setup.py` & `delta-sharing-0.6.6/setup.py`

 * *Files identical despite different names*

