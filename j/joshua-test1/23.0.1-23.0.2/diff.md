# Comparing `tmp/joshua-test1-23.0.1.tar.gz` & `tmp/joshua-test1-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joshua-test1-23.0.1.tar", last modified: Mon May 29 20:11:10 2023, max compression
+gzip compressed data, was "joshua-test1-23.0.2.tar", last modified: Mon May 29 20:25:29 2023, max compression
```

## Comparing `joshua-test1-23.0.1.tar` & `joshua-test1-23.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)    10172 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/LICENSE
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    17322 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/README.md
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/joshua_test1.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      718 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       88 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/requires.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        9 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/top_level.txt
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/pydgraph/
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)      849 2023-05-29 19:21:29.000000 joshua-test1-23.0.1/pydgraph/__init__.py
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)     6648 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/client.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4662 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/pydgraph/client_stub.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2876 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/pydgraph/convert.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1754 2023-05-15 21:41:35.000000 joshua-test1-23.0.1/pydgraph/errors.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      636 2023-05-29 20:09:57.000000 joshua-test1-23.0.1/pydgraph/meta.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/pydgraph/proto/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       79 2023-05-29 20:09:52.000000 joshua-test1-23.0.1/pydgraph/proto/__init__.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7961 2023-05-29 19:48:04.000000 joshua-test1-23.0.1/pydgraph/proto/api_pb2.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7821 2023-05-29 20:09:52.000000 joshua-test1-23.0.1/pydgraph/proto/api_pb2_grpc.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    12606 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/txn.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1952 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/util.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      919 2023-05-29 20:10:55.000000 joshua-test1-23.0.1/pyproject.toml
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/setup.cfg
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/tests/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7787 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_acct_upsert.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5185 2023-05-24 12:24:08.000000 joshua-test1-23.0.1/tests/test_acl.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2154 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_async.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1216 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_client.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2984 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_client_stub.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    16449 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/tests/test_convert.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1946 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_essentials.py
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)     3882 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_queries.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    18545 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_txn.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2980 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_type_system.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5986 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_upsert_block.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1300 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/tests/test_util.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)    10172 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/LICENSE
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    17322 2023-05-24 11:56:21.000000 joshua-test1-23.0.2/README.md
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/joshua_test1.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:25:29.000000 joshua-test1-23.0.2/joshua_test1.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      718 2023-05-29 20:25:29.000000 joshua-test1-23.0.2/joshua_test1.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-05-29 20:25:29.000000 joshua-test1-23.0.2/joshua_test1.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       88 2023-05-29 20:25:29.000000 joshua-test1-23.0.2/joshua_test1.egg-info/requires.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        9 2023-05-29 20:25:29.000000 joshua-test1-23.0.2/joshua_test1.egg-info/top_level.txt
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/pydgraph/
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)      849 2023-05-29 19:21:29.000000 joshua-test1-23.0.2/pydgraph/__init__.py
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)     6648 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/pydgraph/client.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4662 2023-05-23 16:21:12.000000 joshua-test1-23.0.2/pydgraph/client_stub.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2876 2023-05-24 11:56:21.000000 joshua-test1-23.0.2/pydgraph/convert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1754 2023-05-15 21:41:35.000000 joshua-test1-23.0.2/pydgraph/errors.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      636 2023-05-29 20:24:11.000000 joshua-test1-23.0.2/pydgraph/meta.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/pydgraph/proto/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:23:46.000000 joshua-test1-23.0.2/pydgraph/proto/__init__.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7961 2023-05-29 19:48:04.000000 joshua-test1-23.0.2/pydgraph/proto/api_pb2.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7828 2023-05-29 20:23:46.000000 joshua-test1-23.0.2/pydgraph/proto/api_pb2_grpc.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    12606 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/pydgraph/txn.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1952 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/pydgraph/util.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      919 2023-05-29 20:24:38.000000 joshua-test1-23.0.2/pyproject.toml
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/setup.cfg
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:25:29.678418 joshua-test1-23.0.2/tests/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7787 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_acct_upsert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5185 2023-05-24 12:24:08.000000 joshua-test1-23.0.2/tests/test_acl.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2154 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_async.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1216 2023-05-23 16:21:12.000000 joshua-test1-23.0.2/tests/test_client.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2984 2023-05-23 16:21:12.000000 joshua-test1-23.0.2/tests/test_client_stub.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    16449 2023-05-24 11:56:21.000000 joshua-test1-23.0.2/tests/test_convert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1946 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_essentials.py
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)     3882 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_queries.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    18545 2023-05-23 16:21:12.000000 joshua-test1-23.0.2/tests/test_txn.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2980 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_type_system.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5986 2023-05-09 22:49:48.000000 joshua-test1-23.0.2/tests/test_upsert_block.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1300 2023-05-24 11:56:21.000000 joshua-test1-23.0.2/tests/test_util.py
```

### Comparing `joshua-test1-23.0.1/LICENSE` & `joshua-test1-23.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/PKG-INFO` & `joshua-test1-23.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joshua-test1
-Version: 23.0.1
+Version: 23.0.2
 Summary: Official Dgraph client implementation for Python
 Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `joshua-test1-23.0.1/README.md` & `joshua-test1-23.0.2/README.md`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/joshua_test1.egg-info/PKG-INFO` & `joshua-test1-23.0.2/joshua_test1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joshua-test1
-Version: 23.0.1
+Version: 23.0.2
 Summary: Official Dgraph client implementation for Python
 Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `joshua-test1-23.0.1/joshua_test1.egg-info/SOURCES.txt` & `joshua-test1-23.0.2/joshua_test1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/__init__.py` & `joshua-test1-23.0.2/pydgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/client.py` & `joshua-test1-23.0.2/pydgraph/client.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/client_stub.py` & `joshua-test1-23.0.2/pydgraph/client_stub.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/convert.py` & `joshua-test1-23.0.2/pydgraph/convert.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/errors.py` & `joshua-test1-23.0.2/pydgraph/errors.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/meta.py` & `joshua-test1-23.0.2/pydgraph/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata about this package."""
 
-VERSION = '23.0.1'
+VERSION = '23.0.2'
```

### Comparing `joshua-test1-23.0.1/pydgraph/proto/api_pb2.py` & `joshua-test1-23.0.2/pydgraph/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/proto/api_pb2_grpc.py` & `joshua-test1-23.0.2/pydgraph/proto/api_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import api_pb2 as api__pb2
+from . import api_pb2 as api__pb2
 
 
 class DgraphStub(object):
     """Graph response.
     """
 
     def __init__(self, channel):
```

### Comparing `joshua-test1-23.0.1/pydgraph/txn.py` & `joshua-test1-23.0.2/pydgraph/txn.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pydgraph/util.py` & `joshua-test1-23.0.2/pydgraph/util.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/pyproject.toml` & `joshua-test1-23.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_acct_upsert.py` & `joshua-test1-23.0.2/tests/test_acct_upsert.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_acl.py` & `joshua-test1-23.0.2/tests/test_acl.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_async.py` & `joshua-test1-23.0.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_client.py` & `joshua-test1-23.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_client_stub.py` & `joshua-test1-23.0.2/tests/test_client_stub.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_convert.py` & `joshua-test1-23.0.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_essentials.py` & `joshua-test1-23.0.2/tests/test_essentials.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_queries.py` & `joshua-test1-23.0.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_txn.py` & `joshua-test1-23.0.2/tests/test_txn.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_type_system.py` & `joshua-test1-23.0.2/tests/test_type_system.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_upsert_block.py` & `joshua-test1-23.0.2/tests/test_upsert_block.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.1/tests/test_util.py` & `joshua-test1-23.0.2/tests/test_util.py`

 * *Files identical despite different names*

