# Comparing `tmp/tencentcloud-sdk-python-cii-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-cii-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cii-3.0.900.tar", last modified: Fri May 26 02:13:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cii-3.0.901.tar", last modified: Mon May 29 02:22:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cii-3.0.900.tar` & `tencentcloud-sdk-python-cii-3.0.901.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/
--rw-r--r--   0 root         (0) root         (0)     3879 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/cii_client.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10500 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/
--rw-r--r--   0 root         (0) root         (0)    13637 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/cii_client.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56480 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:13:50.000000 tencentcloud-sdk-python-cii-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/cii_client.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10500 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/
+-rw-r--r--   0 root         (0) root         (0)    13637 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/cii_client.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56480 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:22:40.000000 tencentcloud-sdk-python-cii-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cii-3.0.900/README.rst` & `tencentcloud-sdk-python-cii-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.900'
+__version__ = '3.0.901'
```

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/cii_client.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/cii_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/errorcodes.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20201210/models.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20201210/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/cii_client.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/cii_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/errorcodes.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud/cii/v20210408/models.py` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud/cii/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cii-3.0.900/tencentcloud_sdk_python_cii.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cii-3.0.901/tencentcloud_sdk_python_cii.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cii
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cii SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cii-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-cii-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cii
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cii SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cii-3.0.900/setup.py` & `tencentcloud-sdk-python-cii-3.0.901/setup.py`

 * *Files identical despite different names*

