# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.900.tar", last modified: Fri May 26 02:23:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.901.tar", last modified: Mon May 29 02:32:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.900.tar` & `tencentcloud-sdk-python-mongodb-3.0.901.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    13571 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46677 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)    36443 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)   149931 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:23:20.000000 tencentcloud-sdk-python-mongodb-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    13571 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46677 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)    36443 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   149746 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:32:14.000000 tencentcloud-sdk-python-mongodb-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/mongodb/v20190725/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,21 +500,19 @@
 - 具体信息，请通过接口 [DescribeSpecInfo](https://cloud.tencent.com/document/product/240/38567) 获取。
 - 该参数为主可用区，如果多可用区部署，Zone必须是AvailabilityZoneList中的一个。
         :type Zone: str
         :param ClusterType: 实例架构类型。
 - REPLSET：副本集。
 - SHARD：分片集群。
         :type ClusterType: str
-        :param VpcId: 私有网络ID，如果不设置该参数，则默认选择基础网络。
+        :param VpcId: 私有网络ID。如果不设置该参数，则默认选择基础网络。
         :type VpcId: str
         :param SubnetId: 私有网络下的子网 ID，如果配置参数 VpcId，则 SubnetId必须配置。
         :type SubnetId: str
-        :param Password: 实例密码。
-- 不设置该参数，则默认密码格式为：实例ID+@+主账户uin。例如：实例 ID 为cmgo-higv73ed，UIN 为100000001，则默认密码为：cmgo-higv73ed@100000001。 
-- 自定义密码长度为8-32个字符，至少包含字母、数字和字符（!@#%^*()_）中的两种。
+        :param Password: 实例密码。自定义密码长度为8-32个字符，至少包含字母、数字和字符（!@#%^*()_）中的两种。
         :type Password: str
         :param ProjectId: 项目ID。若不设置该参数，则为默认项目。
         :type ProjectId: int
         :param Tags: 实例标签信息。
         :type Tags: list of TagInfo
         :param Clone: 实例类型。
 - 1：正式实例。
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.901/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.901/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.900/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.901/setup.py`

 * *Files identical despite different names*

