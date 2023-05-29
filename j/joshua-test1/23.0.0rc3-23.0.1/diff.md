# Comparing `tmp/joshua-test1-23.0.0rc3.tar.gz` & `tmp/joshua-test1-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joshua-test1-23.0.0rc3.tar", last modified: Thu May 11 14:46:52 2023, max compression
+gzip compressed data, was "joshua-test1-23.0.1.tar", last modified: Mon May 29 20:11:10 2023, max compression
```

## Comparing `joshua-test1-23.0.0rc3.tar` & `joshua-test1-23.0.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-11 14:46:52.438744 joshua-test1-23.0.0rc3/
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)    10172 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/LICENSE
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    27628 2023-05-11 14:46:52.438744 joshua-test1-23.0.0rc3/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    15503 2023-05-11 05:14:03.000000 joshua-test1-23.0.0rc3/README.md
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-11 14:46:52.434744 joshua-test1-23.0.0rc3/joshua_test1.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    27628 2023-05-11 14:46:52.000000 joshua-test1-23.0.0rc3/joshua_test1.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      676 2023-05-11 14:46:52.000000 joshua-test1-23.0.0rc3/joshua_test1.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-05-11 14:46:52.000000 joshua-test1-23.0.0rc3/joshua_test1.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       32 2023-05-11 14:46:52.000000 joshua-test1-23.0.0rc3/joshua_test1.egg-info/requires.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        9 2023-05-11 14:46:52.000000 joshua-test1-23.0.0rc3/joshua_test1.egg-info/top_level.txt
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-11 14:46:52.434744 joshua-test1-23.0.0rc3/pydgraph/
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)      849 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/__init__.py
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)     6648 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/client.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4640 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/client_stub.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1755 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/errors.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      639 2023-05-10 00:00:12.000000 joshua-test1-23.0.0rc3/pydgraph/meta.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-11 14:46:52.434744 joshua-test1-23.0.0rc3/pydgraph/proto/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        0 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/proto/__init__.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7961 2023-05-09 23:02:16.000000 joshua-test1-23.0.0rc3/pydgraph/proto/api_pb2.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7828 2023-05-09 23:02:36.000000 joshua-test1-23.0.0rc3/pydgraph/proto/api_pb2_grpc.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    12606 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/txn.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1952 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/pydgraph/util.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      816 2023-05-11 14:46:07.000000 joshua-test1-23.0.0rc3/pyproject.toml
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-05-11 14:46:52.438744 joshua-test1-23.0.0rc3/setup.cfg
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-11 14:46:52.438744 joshua-test1-23.0.0rc3/tests/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7787 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_acct_upsert.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5104 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_acl.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2154 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_async.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1220 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_client.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2037 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_client_stub.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1946 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_essentials.py
--rwxrwxr-x   0 joshua    (1000) joshua    (1000)     3882 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_queries.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    18158 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_txn.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2980 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_type_system.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5986 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_upsert_block.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1348 2023-05-09 22:49:48.000000 joshua-test1-23.0.0rc3/tests/test_util.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)    10172 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/LICENSE
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    17322 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/README.md
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/joshua_test1.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    29509 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      718 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       88 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/requires.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        9 2023-05-29 20:11:10.000000 joshua-test1-23.0.1/joshua_test1.egg-info/top_level.txt
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/pydgraph/
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)      849 2023-05-29 19:21:29.000000 joshua-test1-23.0.1/pydgraph/__init__.py
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)     6648 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/client.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4662 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/pydgraph/client_stub.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2876 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/pydgraph/convert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1754 2023-05-15 21:41:35.000000 joshua-test1-23.0.1/pydgraph/errors.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      636 2023-05-29 20:09:57.000000 joshua-test1-23.0.1/pydgraph/meta.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/pydgraph/proto/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       79 2023-05-29 20:09:52.000000 joshua-test1-23.0.1/pydgraph/proto/__init__.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7961 2023-05-29 19:48:04.000000 joshua-test1-23.0.1/pydgraph/proto/api_pb2.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7821 2023-05-29 20:09:52.000000 joshua-test1-23.0.1/pydgraph/proto/api_pb2_grpc.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    12606 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/txn.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1952 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/pydgraph/util.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      919 2023-05-29 20:10:55.000000 joshua-test1-23.0.1/pyproject.toml
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/setup.cfg
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-29 20:11:10.959720 joshua-test1-23.0.1/tests/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7787 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_acct_upsert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5185 2023-05-24 12:24:08.000000 joshua-test1-23.0.1/tests/test_acl.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2154 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_async.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1216 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_client.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2984 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_client_stub.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    16449 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/tests/test_convert.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1946 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_essentials.py
+-rwxrwxr-x   0 joshua    (1000) joshua    (1000)     3882 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_queries.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    18545 2023-05-23 16:21:12.000000 joshua-test1-23.0.1/tests/test_txn.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2980 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_type_system.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5986 2023-05-09 22:49:48.000000 joshua-test1-23.0.1/tests/test_upsert_block.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1300 2023-05-24 11:56:21.000000 joshua-test1-23.0.1/tests/test_util.py
```

### Comparing `joshua-test1-23.0.0rc3/LICENSE` & `joshua-test1-23.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/PKG-INFO` & `joshua-test1-23.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: joshua-test1
-Version: 23.0.0rc3
+Version: 23.0.1
 Summary: Official Dgraph client implementation for Python
+Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -181,54 +182,61 @@
 Project-URL: Homepage, https://github.com/dgraph-io/pydgraph
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pydgraph
 
-This is the official Dgraph database client implementation for Python (Python >= v2.7 and >= v3.5), using [gRPC][grpc].
+This is the official Dgraph database client implementation for Python (Python >= v3.7), using [gRPC][grpc].
 
 [grpc]: https://grpc.io/
 
 This client follows the [Dgraph Go client][goclient] closely.
 
 [goclient]: https://github.com/dgraph-io/dgo
 
-Before using this client, we highly recommend that you read the [Dgraph Python
-Client docs](https://dgraph.io/docs/clients/python/), as well as reviewing
-the product documentation at [docs.dgraph.io].
+Before using this client, we highly recommend that you read the
+the product documentation at [dgraph.io/docs].
 
-[docs.dgraph.io]:https://docs.dgraph.io
+[dgraph.io/docs]:https://dgraph.io/docs
 
 ## Table of contents
-
-- [Install](#install)
-- [Supported Versions](#supported-versions)
-- [Quickstart](#quickstart)
-- [Using a Client](#using-a-client)
-  - [Creating a Client](#creating-a-client)
-  - [Altering the Database](#altering-the-database)
-  - [Creating a Transaction](#creating-a-transaction)
-  - [Running a Mutation](#running-a-mutation)
-  - [Committing a Transaction](#committing-a-transaction)
-  * [Running a Query](#running-a-query)
-  * [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
-  * [Running a Conditional Upsert](#running-a-conditional-upsert)
-  - [Cleaning up Resources](#cleaning-up-resources)
-  - [Setting Metadata Headers](#setting-metadata-headers)
-- [Examples](#examples)
-- [Development](#development)
-  - [Building the source](#building-the-source)
-  - [Running tests](#running-tests)
+- [pydgraph](#pydgraph)
+  - [Table of contents](#table-of-contents)
+  - [Install](#install)
+  - [Supported Versions](#supported-versions)
+  - [Quickstart](#quickstart)
+  - [Using a client](#using-a-client)
+    - [Creating a Client](#creating-a-client)
+    - [Login into a Namespace](#login-into-a-namespace)
+    - [Connecting To Dgraph Cloud](#connecting-to-dgraph-cloud)
+    - [Altering the Database](#altering-the-database)
+    - [Creating a Transaction](#creating-a-transaction)
+    - [Running a Mutation](#running-a-mutation)
+    - [Running a Query](#running-a-query)
+    - [Query with RDF response](#query-with-rdf-response)
+    - [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
+    - [Running a Conditional Upsert](#running-a-conditional-upsert)
+    - [Committing a Transaction](#committing-a-transaction)
+    - [Cleaning Up Resources](#cleaning-up-resources)
+    - [Setting Metadata Headers](#setting-metadata-headers)
+    - [Setting a timeout](#setting-a-timeout)
+    - [Async methods](#async-methods)
+  - [Examples](#examples)
+  - [Development](#development)
+    - [Setting up environment](#setting-up-environment)
+    - [Build from source](#build-from-source)
+    - [Running tests](#running-tests)
 
 ## Install
 
 Install using pip:
 
 ```sh
 pip install pydgraph
@@ -237,18 +245,20 @@
 ## Supported Versions
 
 Depending on the version of Dgraph that you are connecting to, you will have to
 use a different version of this client.
 
 | Dgraph version |   pydgraph version   |
 |:--------------:|:--------------------:|
-|     1.0.X      |      <= *1.2.0*      |
-|     1.1.X      |      >= *2.0.0*      |
-|     1.2.X      |      >= *2.0.0*      |
-|    23.X.Y      |      >= *23.0.0*     |
+|    20.3.X      |      *20.3.0*        |
+|    20.7.X      |      *20.7.0*        |
+|    20.11.X     |      *20.7.0*        |
+|    21.03.X     |      *21.3.0*        |
+|    22.0.X      |      *21.3.0*        |
+|    23.0.X      |      *23.0.0*        |
 
 ## Quickstart
 
 Build and run the [simple project][simple] in the `examples` folder, which
 contains an end-to-end example of using the Dgraph python client. For additional details, follow the
 instructions in the project's [README](./examples/simple/README.md).
 
@@ -260,78 +270,114 @@
 
 You can initialize a `DgraphClient` object by passing it a list of
 `DgraphClientStub` clients as variadic arguments. Connecting to multiple Dgraph
 servers in the same cluster allows for better distribution of workload.
 
 The following code snippet shows just one connection.
 
-```python
+```python3
 import pydgraph
 
 client_stub = pydgraph.DgraphClientStub('localhost:9080')
 client = pydgraph.DgraphClient(client_stub)
 ```
 
+### Login into a Namespace
+
+If your server has Access Control Lists enabled (Dgraph v1.1 or above), the client must be
+logged in for accessing data. Use `login` endpoint:
+
+Calling login will obtain and remember the access and refresh JWT tokens. All subsequent operations
+via the logged in client will send along the stored access token.
+
+```python3
+client.login("groot", "password")
+```
+
+If your server additionally has namespaces (Dgraph v21.03 or above), use the
+`login_into_namespace` API.
+
+```python3
+client.login_into_namespace("groot", "password", "123")
+```
+
+### Connecting To Dgraph Cloud
+
+If you want to connect to Dgraph running on [Dgraph Cloud](https://cloud.dgraph.io) instance, then
+get the gRPC endpoint of your cluster that you can find in the
+[Settings section](https://cloud.dgraph.io/_/settings) of Dgraph Cloud console and obtain a Client
+or Admin API key (created in the [API key tab](https://cloud.dgraph.io/_/settings?tab=api-keys)
+of the Setting section). Create the `client_stub` using the gRPC endpoint and the API key:
+
+```python3
+client_stub = pydgraph.DgraphClientStub.from_cloud(
+    "https://morning-glade.grpc.us-east-1.aws.cloud.dgraph.io:443", "<api-key>")
+client = pydgraph.DgraphClient(client_stub)
+```
+
+The `DgraphClientStub.from_slash_endpoint()` method has been removed v23.0.
+Please use `DgraphClientStub.from_cloud()` instead.
+
 ### Altering the Database
 
 To set the schema, create an `Operation` object, set the schema and pass it to
 `DgraphClient#alter(Operation)` method.
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema)
 client.alter(op)
 ```
 
+`Operation` contains other fields as well, including `DropAttr` and `DropAll`. `DropAll` is
+useful if you wish to discard all the data, and start from a clean slate, without bringing
+the instance down. `DropAttr` is used to drop all the data related to a predicate.
+
+```python3
+# Drop all data including schema from the Dgraph instance. This is a useful
+# for small examples such as this since it puts Dgraph into a clean state.
+op = pydgraph.Operation(drop_all=True)
+client.alter(op)
+```
+
 Indexes can be computed in the background.
 You can set the `run_in_background` field of `pydgraph.Operation` to `True`
 before passing it to the `Alter` function. You can find more details
 [here](https://docs.dgraph.io/master/query-language/#indexes-in-background).
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema, run_in_background=True)
 client.alter(op)
 ```
 
-`Operation` contains other fields as well, including the `drop` predicate and `drop all`.
-Drop all is useful if you wish to discard all the data, and start with a clean
-slate, without bringing the instance down.
-
-```python
-# Drop all data including schema from the Dgraph instance. This is a useful
-# for small examples such as this since it puts Dgraph into a clean state.
-op = pydgraph.Operation(drop_all=True)
-client.alter(op)
-```
-
 ### Creating a Transaction
 
 To create a transaction, call the `DgraphClient#txn()` method, which returns a
 new `Txn` object. This operation incurs no network overhead.
 
 It is good practice to call `Txn#discard()` in a `finally` block after running
 the transaction. Calling `Txn#discard()` after `Txn#commit()` is a no-op
 and you can call `Txn#discard()` multiple times with no additional side-effects.
 
-```python
+```python3
 txn = client.txn()
 try:
   # Do something here
   # ...
 finally:
   txn.discard()
   # ...
 ```
 
 To create a read-only transaction, call `DgraphClient#txn(read_only=True)`.
 Read-only transactions are ideal for transactions which only involve queries.
 Mutations and commits are not allowed.
 
-```python
+```python3
 txn = client.txn(read_only=True)
 try:
   # Do some queries here
   # ...
 finally:
   txn.discard()
   # ...
@@ -351,42 +397,39 @@
 
 `Txn#mutate()` provides convenience keyword arguments `set_obj` and `del_obj`
 for setting JSON values and `set_nquads` and `del_nquads` for setting N-Quad
 values. See examples below for usage.
 
 We define a person object to represent a person and use it in a transaction.
 
-```python
+```python3
 # Create data.
-p = {
-    'name': 'Alice',
-}
+p = { 'name': 'Alice' }
 
 # Run mutation.
 txn.mutate(set_obj=p)
 
 # If you want to use a mutation object, use this instead:
 # mu = pydgraph.Mutation(set_json=json.dumps(p).encode('utf8'))
 # txn.mutate(mu)
 
 # If you want to use N-Quads, use this instead:
 # txn.mutate(set_nquads='_:alice <name> "Alice" .')
 ```
 
-```python
-# Delete data.
+```python3
+# Delete data
 
 query = """query all($a: string)
  {
    all(func: eq(name, $a))
     {
       uid
     }
   }"""
-
 variables = {'$a': 'Bob'}
 
 res = txn.query(query, variables=variables)
 ppl = json.loads(res.json)
 
 # For a mutation to delete a node, use this:
 txn.mutate(del_obj=person)
@@ -397,59 +440,32 @@
 
 Sometimes, you only want to commit a mutation, without querying anything further.
 In such cases, you can set the keyword argument `commit_now=True` to indicate
 that the mutation must be immediately committed.
 
 A mutation can be executed using `txn.do_request` as well.
 
-```python
+```python3
 mutation = txn.create_mutation(set_nquads='_:alice <name> "Alice" .')
 request = txn.create_request(mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
-### Committing a Transaction
-
-A transaction can be committed using the `Txn#commit()` method. If your transaction
-consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
-`Txn#mutate`, then calling `Txn#commit()` is not necessary.
-
-An error is raised if another transaction(s) modify the same data concurrently that was
-modified in the current transaction. It is up to the user to retry transactions
-when they fail.
-
-```python
-txn = client.txn()
-try:
-  # ...
-  # Perform any number of queries and mutations
-  # ...
-  # and finally...
-  txn.commit()
-except pydgraph.AbortedError:
-  # Retry or handle exception.
-finally:
-  # Clean up. Calling this after txn.commit() is a no-op
-  # and hence safe.
-  txn.discard()
-```
-
 ### Running a Query
 
 You can run a query by calling `Txn#query(string)`. You will need to pass in a
-[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass an additional dictionary of any
-variables that you might want to set in the query, call
-`Txn#query(string, variables=d)` with the variables dictionary `d`.
+[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass
+an additional dictionary of any variables that you might want to set in the query,
+call `Txn#query(string, variables=d)` with the variables dictionary `d`.
 
 The query response contains the `json` field, which returns the JSON response.
-
 Let’s run a query with a variable `$a`, deserialize the result from JSON and
 print it out:
 
-```python
+```python3
 # Run query.
 query = """query all($a: string) {
   all(func: eq(name, $a))
   {
     name
   }
 }"""
@@ -473,94 +489,138 @@
 ```console
 Number of people named "Alice": 1
 Alice
 ```
 
 You can also use `txn.do_request` function to run the query.
 
-```python
+```python3
 request = txn.create_request(query=query)
 txn.do_request(request)
 ```
 
+### Query with RDF response
+
+You can get query result as a RDF response by calling `Txn#query(string)` with `resp_format` set
+to `RDF`. The response would contain a `rdf` field, which has the RDF encoded result.
+
+**Note:** If you are querying only for `uid` values, use a JSON format response.
+
+```python3
+res = txn.query(query, variables=variables, resp_format="RDF")
+print(res.rdf)
+```
+
 ### Running an Upsert: Query + Mutation
 
 The `txn.do_request` function allows you to use upsert blocks. An upsert block
 contains one query block and one or more mutation blocks, so it lets you perform
 queries and mutations in a single request. Variables defined in the query block
 can be used in the mutation blocks using the `uid` and `val` functions
 implemented by DQL.
 
 To learn more about upsert blocks, see the
 [Upsert Block documentation](https://dgraph.io/docs/mutations/upsert-block/).
 
-```python
+```python3
 query = """{
   u as var(func: eq(name, "Alice"))
 }"""
+
 nquad = """
   uid(u) <name> "Alice" .
   uid(u) <age> "25" .
 """
+
 mutation = txn.create_mutation(set_nquads=nquad)
 request = txn.create_request(query=query, mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
 ### Running a Conditional Upsert
 
-The upsert block also allows specifying a conditional mutation block using an `@if` directive. The mutation is executed
-only when the specified condition is true. If the condition is false, the mutation is silently ignored.
+The upsert block also allows specifying a conditional mutation block using an `@if` directive.
+The mutation is executed only when the specified condition is true. If the condition is false,
+the mutation is silently ignored.
 
 See more about Conditional Upserts [here](https://docs.dgraph.io/mutations/#conditional-upsert).
 
-```python
+```python3
 query = """
   {
     user as var(func: eq(email, "wrong_email@dgraph.io"))
   }
 """
+
 cond = "@if(eq(len(user), 1))"
 nquads = """
   uid(user) <email> "correct_email@dgraph.io" .
 """
+
 mutation = txn.create_mutation(cond=cond, set_nquads=nquads)
 request = txn.create_request(mutations=[mutation], query=query, commit_now=True)
 txn.do_request(request)
 ```
 
+### Committing a Transaction
+
+A transaction can be committed using the `Txn#commit()` method. If your transaction
+consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
+`Txn#mutate`, then calling `Txn#commit()` is not necessary.
+
+An error is raised if another transaction(s) modify the same data concurrently that was
+modified in the current transaction. It is up to the user to retry transactions
+when they fail.
+
+```python3
+txn = client.txn()
+try:
+  # ...
+  # Perform any number of queries and mutations
+  # ...
+  # and finally...
+  txn.commit()
+except pydgraph.AbortedError:
+  # Retry or handle exception.
+finally:
+  # Clean up. Calling this after txn.commit() is a no-op
+  # and hence safe.
+  txn.discard()
+```
+
 ### Cleaning Up Resources
 
 To clean up resources, you have to call `DgraphClientStub#close()` individually for
 all the instances of `DgraphClientStub`.
 
-```python
-SERVER_ADDR = "localhost:9080"
+```python3
+SERVER_ADDR1 = "localhost:9080"
+SERVER_ADDR2 = "localhost:9080"
 
 # Create instances of DgraphClientStub.
-stub1 = pydgraph.DgraphClientStub(SERVER_ADDR)
-stub2 = pydgraph.DgraphClientStub(SERVER_ADDR)
+stub1 = pydgraph.DgraphClientStub(SERVER_ADDR1)
+stub2 = pydgraph.DgraphClientStub(SERVER_ADDR2)
 
 # Create an instance of DgraphClient.
 client = pydgraph.DgraphClient(stub1, stub2)
 
-# ...
 # Use client
-# ...
+...
 
 # Clean up resources by closing all client stubs.
 stub1.close()
 stub2.close()
 ```
 
 ### Setting Metadata Headers
 
-Metadata headers such as authentication tokens can be set through the metadata of gRPC methods. Below is an example of how to set a header named "auth-token".
+Metadata headers such as authentication tokens can be set through the metadata of gRPC methods.
+Below is an example of how to set a header named "auth-token".
 
-```python
+```python3
 # The following piece of code shows how one can set metadata with
 # auth-token, to allow Alter operation, if the server requires it.
 # metadata is a list of arbitrary key-value pairs.
 metadata = [("auth-token", "the-auth-token-value")]
 dg.alter(op, metadata=metadata)
 ```
 
@@ -568,96 +628,85 @@
 
 A timeout value representing the number of seconds can be passed to the `login`,
 `alter`, `query`, and `mutate` methods using the `timeout` keyword argument.
 
 For example, the following alters the schema with a timeout of ten seconds:
 `dg.alter(op, timeout=10)`
 
-### Passing credentials
-
-A `CallCredentials` object can be passed to the `login`, `alter`, `query`, and
-`mutate` methods using the `credentials` keyword argument.
-
-### Authenticating to a reverse TLS proxy
-
-If the Dgraph instance is behind a reverse TLS proxy, credentials can also be
-passed through the methods available in the gRPC library. Note that in this case
-every request will need to include the credentials. In the example below, we are
-trying to add authentication to a proxy that requires an API key. This value is
-expected to be included in the metadata using the key "authorization".
-
-```python
-creds = grpc.ssl_channel_credentials()
-call_credentials = grpc.metadata_call_credentials(
-    lambda context, callback: callback((("authorization", "<api-key>"),), None))
-composite_credentials = grpc.composite_channel_credentials(creds, call_credentials)
-client_stub = pydgraph.DgraphClientStub(
-    '{host}:{port}'.format(host=GRPC_HOST, port=GRPC_PORT), composite_credentials)
-client = pydgraph.DgraphClient(client_stub)
-```
-
 ### Async methods
 
 The `alter` method in the client has an asynchronous version called
 `async_alter`. The async methods return a future. You can directly call the
 `result` method on the future. However. The DgraphClient class provides a static
 method `handle_alter_future` to handle any possible exception.
 
-```python
+```python3
 alter_future = self.client.async_alter(pydgraph.Operation(
 	schema="name: string @index(term) ."))
 response = pydgraph.DgraphClient.handle_alter_future(alter_future)
 ```
 
 The `query` and `mutate` methods int the `Txn` class also have async versions
 called `async_query` and `async_mutation` respectively. These functions work
 just like `async_alter`.
 
 You can use the `handle_query_future` and `handle_mutate_future` static methods
 in the `Txn` class to retrieve the result. A short example is given below:
 
-```python
+```python3
 txn = client.txn()
 query = "query body here"
 future = txn.async_query()
 response = pydgraph.Txn.handle_query_future(future)
 ```
 
-A working example can be found in the `test_asycn.py` test file.
-
 Keep in mind that due to the nature of async calls, the async functions cannot
 retry the request if the login is invalid. You will have to check for this error
 and retry the login (with the function `retry_login` in both the `Txn` and
 `Client` classes). A short example is given below:
 
-```python
+```python3
 client = DgraphClient(client_stubs) # client_stubs is a list of gRPC stubs.
 alter_future = client.async_alter()
 try:
     response = alter_future.result()
 except Exception as e:
 	# You can use this function in the util package to check for JWT
     # expired errors.
     if pydgraph.util.is_jwt_expired(e):
         # retry your request here.
 ```
 
 ## Examples
 
+[tls]: ./examples/tls
+[parse_datetime]: ./examples/parse_datetime
+
 - [simple][]: Quickstart example of using pydgraph.
+- [tls][]: Quickstart example that uses TLS.
+- [parse_datetime]: Demonstration of converting Dgraph's DateTime strings to native python datetime.
 
 ## Development
 
+### Setting up environment
+
+There are many ways to set up your local Python environment. We suggest some sane defaults here.
+
+- Use [pyenv](https://github.com/pyenv/pyenv) to manage your Python installations.
+- Most recent versions of Python should work, but the version of Python officially supported is located in
+`.python-version`
+- Create a Python virtual environment using `python -m venv .venv`
+- Activate virtual environment via `source .venv/bin/activate`
+
 ### Build from source
 
 To build and install pydgraph locally, run
 
 ```sh
-python -m build
-pip install -e .
+pip install -e ".[dev]"
 ```
 
 If you have made changes to the `pydgraph/proto/api.proto` file, you need need
 to regenerate the source files generated by Protocol Buffer tools. To do that,
 install the [grpcio-tools][grpcio-tools] library and then run the following
 command:
 
@@ -679,15 +728,16 @@
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
 
-This script assumes dgraph is located on your path.  Dgraph release binaries can be found [here](https://github.com/dgraph-io/dgraph/releases).
+This script assumes dgraph is located on your path. Dgraph release binaries can
+be found [here](https://github.com/dgraph-io/dgraph/releases).
 The test script also requires that `docker` and `docker compose` are installed on
 your machine.
 
 The script will take care of bringing up a Dgraph cluster and bringing it down
 after the tests are executed. The script connects to randomly selected ports for
 HTTP and gRPC requests to prevent interference with clusters running on the
 default port. Docker and docker-compose need to be installed before running the
```

### Comparing `joshua-test1-23.0.0rc3/README.md` & `joshua-test1-23.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 # pydgraph
 
-This is the official Dgraph database client implementation for Python (Python >= v2.7 and >= v3.5), using [gRPC][grpc].
+This is the official Dgraph database client implementation for Python (Python >= v3.7), using [gRPC][grpc].
 
 [grpc]: https://grpc.io/
 
 This client follows the [Dgraph Go client][goclient] closely.
 
 [goclient]: https://github.com/dgraph-io/dgo
 
-Before using this client, we highly recommend that you read the [Dgraph Python
-Client docs](https://dgraph.io/docs/clients/python/), as well as reviewing
-the product documentation at [docs.dgraph.io].
+Before using this client, we highly recommend that you read the
+the product documentation at [dgraph.io/docs].
 
-[docs.dgraph.io]:https://docs.dgraph.io
+[dgraph.io/docs]:https://dgraph.io/docs
 
 ## Table of contents
-
-- [Install](#install)
-- [Supported Versions](#supported-versions)
-- [Quickstart](#quickstart)
-- [Using a Client](#using-a-client)
-  - [Creating a Client](#creating-a-client)
-  - [Altering the Database](#altering-the-database)
-  - [Creating a Transaction](#creating-a-transaction)
-  - [Running a Mutation](#running-a-mutation)
-  - [Committing a Transaction](#committing-a-transaction)
-  * [Running a Query](#running-a-query)
-  * [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
-  * [Running a Conditional Upsert](#running-a-conditional-upsert)
-  - [Cleaning up Resources](#cleaning-up-resources)
-  - [Setting Metadata Headers](#setting-metadata-headers)
-- [Examples](#examples)
-- [Development](#development)
-  - [Building the source](#building-the-source)
-  - [Running tests](#running-tests)
+- [pydgraph](#pydgraph)
+  - [Table of contents](#table-of-contents)
+  - [Install](#install)
+  - [Supported Versions](#supported-versions)
+  - [Quickstart](#quickstart)
+  - [Using a client](#using-a-client)
+    - [Creating a Client](#creating-a-client)
+    - [Login into a Namespace](#login-into-a-namespace)
+    - [Connecting To Dgraph Cloud](#connecting-to-dgraph-cloud)
+    - [Altering the Database](#altering-the-database)
+    - [Creating a Transaction](#creating-a-transaction)
+    - [Running a Mutation](#running-a-mutation)
+    - [Running a Query](#running-a-query)
+    - [Query with RDF response](#query-with-rdf-response)
+    - [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
+    - [Running a Conditional Upsert](#running-a-conditional-upsert)
+    - [Committing a Transaction](#committing-a-transaction)
+    - [Cleaning Up Resources](#cleaning-up-resources)
+    - [Setting Metadata Headers](#setting-metadata-headers)
+    - [Setting a timeout](#setting-a-timeout)
+    - [Async methods](#async-methods)
+  - [Examples](#examples)
+  - [Development](#development)
+    - [Setting up environment](#setting-up-environment)
+    - [Build from source](#build-from-source)
+    - [Running tests](#running-tests)
 
 ## Install
 
 Install using pip:
 
 ```sh
 pip install pydgraph
@@ -46,18 +52,20 @@
 ## Supported Versions
 
 Depending on the version of Dgraph that you are connecting to, you will have to
 use a different version of this client.
 
 | Dgraph version |   pydgraph version   |
 |:--------------:|:--------------------:|
-|     1.0.X      |      <= *1.2.0*      |
-|     1.1.X      |      >= *2.0.0*      |
-|     1.2.X      |      >= *2.0.0*      |
-|    23.X.Y      |      >= *23.0.0*     |
+|    20.3.X      |      *20.3.0*        |
+|    20.7.X      |      *20.7.0*        |
+|    20.11.X     |      *20.7.0*        |
+|    21.03.X     |      *21.3.0*        |
+|    22.0.X      |      *21.3.0*        |
+|    23.0.X      |      *23.0.0*        |
 
 ## Quickstart
 
 Build and run the [simple project][simple] in the `examples` folder, which
 contains an end-to-end example of using the Dgraph python client. For additional details, follow the
 instructions in the project's [README](./examples/simple/README.md).
 
@@ -69,78 +77,114 @@
 
 You can initialize a `DgraphClient` object by passing it a list of
 `DgraphClientStub` clients as variadic arguments. Connecting to multiple Dgraph
 servers in the same cluster allows for better distribution of workload.
 
 The following code snippet shows just one connection.
 
-```python
+```python3
 import pydgraph
 
 client_stub = pydgraph.DgraphClientStub('localhost:9080')
 client = pydgraph.DgraphClient(client_stub)
 ```
 
+### Login into a Namespace
+
+If your server has Access Control Lists enabled (Dgraph v1.1 or above), the client must be
+logged in for accessing data. Use `login` endpoint:
+
+Calling login will obtain and remember the access and refresh JWT tokens. All subsequent operations
+via the logged in client will send along the stored access token.
+
+```python3
+client.login("groot", "password")
+```
+
+If your server additionally has namespaces (Dgraph v21.03 or above), use the
+`login_into_namespace` API.
+
+```python3
+client.login_into_namespace("groot", "password", "123")
+```
+
+### Connecting To Dgraph Cloud
+
+If you want to connect to Dgraph running on [Dgraph Cloud](https://cloud.dgraph.io) instance, then
+get the gRPC endpoint of your cluster that you can find in the
+[Settings section](https://cloud.dgraph.io/_/settings) of Dgraph Cloud console and obtain a Client
+or Admin API key (created in the [API key tab](https://cloud.dgraph.io/_/settings?tab=api-keys)
+of the Setting section). Create the `client_stub` using the gRPC endpoint and the API key:
+
+```python3
+client_stub = pydgraph.DgraphClientStub.from_cloud(
+    "https://morning-glade.grpc.us-east-1.aws.cloud.dgraph.io:443", "<api-key>")
+client = pydgraph.DgraphClient(client_stub)
+```
+
+The `DgraphClientStub.from_slash_endpoint()` method has been removed v23.0.
+Please use `DgraphClientStub.from_cloud()` instead.
+
 ### Altering the Database
 
 To set the schema, create an `Operation` object, set the schema and pass it to
 `DgraphClient#alter(Operation)` method.
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema)
 client.alter(op)
 ```
 
+`Operation` contains other fields as well, including `DropAttr` and `DropAll`. `DropAll` is
+useful if you wish to discard all the data, and start from a clean slate, without bringing
+the instance down. `DropAttr` is used to drop all the data related to a predicate.
+
+```python3
+# Drop all data including schema from the Dgraph instance. This is a useful
+# for small examples such as this since it puts Dgraph into a clean state.
+op = pydgraph.Operation(drop_all=True)
+client.alter(op)
+```
+
 Indexes can be computed in the background.
 You can set the `run_in_background` field of `pydgraph.Operation` to `True`
 before passing it to the `Alter` function. You can find more details
 [here](https://docs.dgraph.io/master/query-language/#indexes-in-background).
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema, run_in_background=True)
 client.alter(op)
 ```
 
-`Operation` contains other fields as well, including the `drop` predicate and `drop all`.
-Drop all is useful if you wish to discard all the data, and start with a clean
-slate, without bringing the instance down.
-
-```python
-# Drop all data including schema from the Dgraph instance. This is a useful
-# for small examples such as this since it puts Dgraph into a clean state.
-op = pydgraph.Operation(drop_all=True)
-client.alter(op)
-```
-
 ### Creating a Transaction
 
 To create a transaction, call the `DgraphClient#txn()` method, which returns a
 new `Txn` object. This operation incurs no network overhead.
 
 It is good practice to call `Txn#discard()` in a `finally` block after running
 the transaction. Calling `Txn#discard()` after `Txn#commit()` is a no-op
 and you can call `Txn#discard()` multiple times with no additional side-effects.
 
-```python
+```python3
 txn = client.txn()
 try:
   # Do something here
   # ...
 finally:
   txn.discard()
   # ...
 ```
 
 To create a read-only transaction, call `DgraphClient#txn(read_only=True)`.
 Read-only transactions are ideal for transactions which only involve queries.
 Mutations and commits are not allowed.
 
-```python
+```python3
 txn = client.txn(read_only=True)
 try:
   # Do some queries here
   # ...
 finally:
   txn.discard()
   # ...
@@ -160,42 +204,39 @@
 
 `Txn#mutate()` provides convenience keyword arguments `set_obj` and `del_obj`
 for setting JSON values and `set_nquads` and `del_nquads` for setting N-Quad
 values. See examples below for usage.
 
 We define a person object to represent a person and use it in a transaction.
 
-```python
+```python3
 # Create data.
-p = {
-    'name': 'Alice',
-}
+p = { 'name': 'Alice' }
 
 # Run mutation.
 txn.mutate(set_obj=p)
 
 # If you want to use a mutation object, use this instead:
 # mu = pydgraph.Mutation(set_json=json.dumps(p).encode('utf8'))
 # txn.mutate(mu)
 
 # If you want to use N-Quads, use this instead:
 # txn.mutate(set_nquads='_:alice <name> "Alice" .')
 ```
 
-```python
-# Delete data.
+```python3
+# Delete data
 
 query = """query all($a: string)
  {
    all(func: eq(name, $a))
     {
       uid
     }
   }"""
-
 variables = {'$a': 'Bob'}
 
 res = txn.query(query, variables=variables)
 ppl = json.loads(res.json)
 
 # For a mutation to delete a node, use this:
 txn.mutate(del_obj=person)
@@ -206,59 +247,32 @@
 
 Sometimes, you only want to commit a mutation, without querying anything further.
 In such cases, you can set the keyword argument `commit_now=True` to indicate
 that the mutation must be immediately committed.
 
 A mutation can be executed using `txn.do_request` as well.
 
-```python
+```python3
 mutation = txn.create_mutation(set_nquads='_:alice <name> "Alice" .')
 request = txn.create_request(mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
-### Committing a Transaction
-
-A transaction can be committed using the `Txn#commit()` method. If your transaction
-consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
-`Txn#mutate`, then calling `Txn#commit()` is not necessary.
-
-An error is raised if another transaction(s) modify the same data concurrently that was
-modified in the current transaction. It is up to the user to retry transactions
-when they fail.
-
-```python
-txn = client.txn()
-try:
-  # ...
-  # Perform any number of queries and mutations
-  # ...
-  # and finally...
-  txn.commit()
-except pydgraph.AbortedError:
-  # Retry or handle exception.
-finally:
-  # Clean up. Calling this after txn.commit() is a no-op
-  # and hence safe.
-  txn.discard()
-```
-
 ### Running a Query
 
 You can run a query by calling `Txn#query(string)`. You will need to pass in a
-[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass an additional dictionary of any
-variables that you might want to set in the query, call
-`Txn#query(string, variables=d)` with the variables dictionary `d`.
+[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass
+an additional dictionary of any variables that you might want to set in the query,
+call `Txn#query(string, variables=d)` with the variables dictionary `d`.
 
 The query response contains the `json` field, which returns the JSON response.
-
 Let’s run a query with a variable `$a`, deserialize the result from JSON and
 print it out:
 
-```python
+```python3
 # Run query.
 query = """query all($a: string) {
   all(func: eq(name, $a))
   {
     name
   }
 }"""
@@ -282,94 +296,138 @@
 ```console
 Number of people named "Alice": 1
 Alice
 ```
 
 You can also use `txn.do_request` function to run the query.
 
-```python
+```python3
 request = txn.create_request(query=query)
 txn.do_request(request)
 ```
 
+### Query with RDF response
+
+You can get query result as a RDF response by calling `Txn#query(string)` with `resp_format` set
+to `RDF`. The response would contain a `rdf` field, which has the RDF encoded result.
+
+**Note:** If you are querying only for `uid` values, use a JSON format response.
+
+```python3
+res = txn.query(query, variables=variables, resp_format="RDF")
+print(res.rdf)
+```
+
 ### Running an Upsert: Query + Mutation
 
 The `txn.do_request` function allows you to use upsert blocks. An upsert block
 contains one query block and one or more mutation blocks, so it lets you perform
 queries and mutations in a single request. Variables defined in the query block
 can be used in the mutation blocks using the `uid` and `val` functions
 implemented by DQL.
 
 To learn more about upsert blocks, see the
 [Upsert Block documentation](https://dgraph.io/docs/mutations/upsert-block/).
 
-```python
+```python3
 query = """{
   u as var(func: eq(name, "Alice"))
 }"""
+
 nquad = """
   uid(u) <name> "Alice" .
   uid(u) <age> "25" .
 """
+
 mutation = txn.create_mutation(set_nquads=nquad)
 request = txn.create_request(query=query, mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
 ### Running a Conditional Upsert
 
-The upsert block also allows specifying a conditional mutation block using an `@if` directive. The mutation is executed
-only when the specified condition is true. If the condition is false, the mutation is silently ignored.
+The upsert block also allows specifying a conditional mutation block using an `@if` directive.
+The mutation is executed only when the specified condition is true. If the condition is false,
+the mutation is silently ignored.
 
 See more about Conditional Upserts [here](https://docs.dgraph.io/mutations/#conditional-upsert).
 
-```python
+```python3
 query = """
   {
     user as var(func: eq(email, "wrong_email@dgraph.io"))
   }
 """
+
 cond = "@if(eq(len(user), 1))"
 nquads = """
   uid(user) <email> "correct_email@dgraph.io" .
 """
+
 mutation = txn.create_mutation(cond=cond, set_nquads=nquads)
 request = txn.create_request(mutations=[mutation], query=query, commit_now=True)
 txn.do_request(request)
 ```
 
+### Committing a Transaction
+
+A transaction can be committed using the `Txn#commit()` method. If your transaction
+consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
+`Txn#mutate`, then calling `Txn#commit()` is not necessary.
+
+An error is raised if another transaction(s) modify the same data concurrently that was
+modified in the current transaction. It is up to the user to retry transactions
+when they fail.
+
+```python3
+txn = client.txn()
+try:
+  # ...
+  # Perform any number of queries and mutations
+  # ...
+  # and finally...
+  txn.commit()
+except pydgraph.AbortedError:
+  # Retry or handle exception.
+finally:
+  # Clean up. Calling this after txn.commit() is a no-op
+  # and hence safe.
+  txn.discard()
+```
+
 ### Cleaning Up Resources
 
 To clean up resources, you have to call `DgraphClientStub#close()` individually for
 all the instances of `DgraphClientStub`.
 
-```python
-SERVER_ADDR = "localhost:9080"
+```python3
+SERVER_ADDR1 = "localhost:9080"
+SERVER_ADDR2 = "localhost:9080"
 
 # Create instances of DgraphClientStub.
-stub1 = pydgraph.DgraphClientStub(SERVER_ADDR)
-stub2 = pydgraph.DgraphClientStub(SERVER_ADDR)
+stub1 = pydgraph.DgraphClientStub(SERVER_ADDR1)
+stub2 = pydgraph.DgraphClientStub(SERVER_ADDR2)
 
 # Create an instance of DgraphClient.
 client = pydgraph.DgraphClient(stub1, stub2)
 
-# ...
 # Use client
-# ...
+...
 
 # Clean up resources by closing all client stubs.
 stub1.close()
 stub2.close()
 ```
 
 ### Setting Metadata Headers
 
-Metadata headers such as authentication tokens can be set through the metadata of gRPC methods. Below is an example of how to set a header named "auth-token".
+Metadata headers such as authentication tokens can be set through the metadata of gRPC methods.
+Below is an example of how to set a header named "auth-token".
 
-```python
+```python3
 # The following piece of code shows how one can set metadata with
 # auth-token, to allow Alter operation, if the server requires it.
 # metadata is a list of arbitrary key-value pairs.
 metadata = [("auth-token", "the-auth-token-value")]
 dg.alter(op, metadata=metadata)
 ```
 
@@ -377,96 +435,85 @@
 
 A timeout value representing the number of seconds can be passed to the `login`,
 `alter`, `query`, and `mutate` methods using the `timeout` keyword argument.
 
 For example, the following alters the schema with a timeout of ten seconds:
 `dg.alter(op, timeout=10)`
 
-### Passing credentials
-
-A `CallCredentials` object can be passed to the `login`, `alter`, `query`, and
-`mutate` methods using the `credentials` keyword argument.
-
-### Authenticating to a reverse TLS proxy
-
-If the Dgraph instance is behind a reverse TLS proxy, credentials can also be
-passed through the methods available in the gRPC library. Note that in this case
-every request will need to include the credentials. In the example below, we are
-trying to add authentication to a proxy that requires an API key. This value is
-expected to be included in the metadata using the key "authorization".
-
-```python
-creds = grpc.ssl_channel_credentials()
-call_credentials = grpc.metadata_call_credentials(
-    lambda context, callback: callback((("authorization", "<api-key>"),), None))
-composite_credentials = grpc.composite_channel_credentials(creds, call_credentials)
-client_stub = pydgraph.DgraphClientStub(
-    '{host}:{port}'.format(host=GRPC_HOST, port=GRPC_PORT), composite_credentials)
-client = pydgraph.DgraphClient(client_stub)
-```
-
 ### Async methods
 
 The `alter` method in the client has an asynchronous version called
 `async_alter`. The async methods return a future. You can directly call the
 `result` method on the future. However. The DgraphClient class provides a static
 method `handle_alter_future` to handle any possible exception.
 
-```python
+```python3
 alter_future = self.client.async_alter(pydgraph.Operation(
 	schema="name: string @index(term) ."))
 response = pydgraph.DgraphClient.handle_alter_future(alter_future)
 ```
 
 The `query` and `mutate` methods int the `Txn` class also have async versions
 called `async_query` and `async_mutation` respectively. These functions work
 just like `async_alter`.
 
 You can use the `handle_query_future` and `handle_mutate_future` static methods
 in the `Txn` class to retrieve the result. A short example is given below:
 
-```python
+```python3
 txn = client.txn()
 query = "query body here"
 future = txn.async_query()
 response = pydgraph.Txn.handle_query_future(future)
 ```
 
-A working example can be found in the `test_asycn.py` test file.
-
 Keep in mind that due to the nature of async calls, the async functions cannot
 retry the request if the login is invalid. You will have to check for this error
 and retry the login (with the function `retry_login` in both the `Txn` and
 `Client` classes). A short example is given below:
 
-```python
+```python3
 client = DgraphClient(client_stubs) # client_stubs is a list of gRPC stubs.
 alter_future = client.async_alter()
 try:
     response = alter_future.result()
 except Exception as e:
 	# You can use this function in the util package to check for JWT
     # expired errors.
     if pydgraph.util.is_jwt_expired(e):
         # retry your request here.
 ```
 
 ## Examples
 
+[tls]: ./examples/tls
+[parse_datetime]: ./examples/parse_datetime
+
 - [simple][]: Quickstart example of using pydgraph.
+- [tls][]: Quickstart example that uses TLS.
+- [parse_datetime]: Demonstration of converting Dgraph's DateTime strings to native python datetime.
 
 ## Development
 
+### Setting up environment
+
+There are many ways to set up your local Python environment. We suggest some sane defaults here.
+
+- Use [pyenv](https://github.com/pyenv/pyenv) to manage your Python installations.
+- Most recent versions of Python should work, but the version of Python officially supported is located in
+`.python-version`
+- Create a Python virtual environment using `python -m venv .venv`
+- Activate virtual environment via `source .venv/bin/activate`
+
 ### Build from source
 
 To build and install pydgraph locally, run
 
 ```sh
-python -m build
-pip install -e .
+pip install -e ".[dev]"
 ```
 
 If you have made changes to the `pydgraph/proto/api.proto` file, you need need
 to regenerate the source files generated by Protocol Buffer tools. To do that,
 install the [grpcio-tools][grpcio-tools] library and then run the following
 command:
 
@@ -488,15 +535,16 @@
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
 
-This script assumes dgraph is located on your path.  Dgraph release binaries can be found [here](https://github.com/dgraph-io/dgraph/releases).
+This script assumes dgraph is located on your path. Dgraph release binaries can
+be found [here](https://github.com/dgraph-io/dgraph/releases).
 The test script also requires that `docker` and `docker compose` are installed on
 your machine.
 
 The script will take care of bringing up a Dgraph cluster and bringing it down
 after the tests are executed. The script connects to randomly selected ports for
 HTTP and gRPC requests to prevent interference with clusters running on the
 default port. Docker and docker-compose need to be installed before running the
```

### Comparing `joshua-test1-23.0.0rc3/joshua_test1.egg-info/PKG-INFO` & `joshua-test1-23.0.1/joshua_test1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: joshua-test1
-Version: 23.0.0rc3
+Version: 23.0.1
 Summary: Official Dgraph client implementation for Python
+Author-email: Dgraph Labs <contact@dgraph.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -181,54 +182,61 @@
 Project-URL: Homepage, https://github.com/dgraph-io/pydgraph
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pydgraph
 
-This is the official Dgraph database client implementation for Python (Python >= v2.7 and >= v3.5), using [gRPC][grpc].
+This is the official Dgraph database client implementation for Python (Python >= v3.7), using [gRPC][grpc].
 
 [grpc]: https://grpc.io/
 
 This client follows the [Dgraph Go client][goclient] closely.
 
 [goclient]: https://github.com/dgraph-io/dgo
 
-Before using this client, we highly recommend that you read the [Dgraph Python
-Client docs](https://dgraph.io/docs/clients/python/), as well as reviewing
-the product documentation at [docs.dgraph.io].
+Before using this client, we highly recommend that you read the
+the product documentation at [dgraph.io/docs].
 
-[docs.dgraph.io]:https://docs.dgraph.io
+[dgraph.io/docs]:https://dgraph.io/docs
 
 ## Table of contents
-
-- [Install](#install)
-- [Supported Versions](#supported-versions)
-- [Quickstart](#quickstart)
-- [Using a Client](#using-a-client)
-  - [Creating a Client](#creating-a-client)
-  - [Altering the Database](#altering-the-database)
-  - [Creating a Transaction](#creating-a-transaction)
-  - [Running a Mutation](#running-a-mutation)
-  - [Committing a Transaction](#committing-a-transaction)
-  * [Running a Query](#running-a-query)
-  * [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
-  * [Running a Conditional Upsert](#running-a-conditional-upsert)
-  - [Cleaning up Resources](#cleaning-up-resources)
-  - [Setting Metadata Headers](#setting-metadata-headers)
-- [Examples](#examples)
-- [Development](#development)
-  - [Building the source](#building-the-source)
-  - [Running tests](#running-tests)
+- [pydgraph](#pydgraph)
+  - [Table of contents](#table-of-contents)
+  - [Install](#install)
+  - [Supported Versions](#supported-versions)
+  - [Quickstart](#quickstart)
+  - [Using a client](#using-a-client)
+    - [Creating a Client](#creating-a-client)
+    - [Login into a Namespace](#login-into-a-namespace)
+    - [Connecting To Dgraph Cloud](#connecting-to-dgraph-cloud)
+    - [Altering the Database](#altering-the-database)
+    - [Creating a Transaction](#creating-a-transaction)
+    - [Running a Mutation](#running-a-mutation)
+    - [Running a Query](#running-a-query)
+    - [Query with RDF response](#query-with-rdf-response)
+    - [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
+    - [Running a Conditional Upsert](#running-a-conditional-upsert)
+    - [Committing a Transaction](#committing-a-transaction)
+    - [Cleaning Up Resources](#cleaning-up-resources)
+    - [Setting Metadata Headers](#setting-metadata-headers)
+    - [Setting a timeout](#setting-a-timeout)
+    - [Async methods](#async-methods)
+  - [Examples](#examples)
+  - [Development](#development)
+    - [Setting up environment](#setting-up-environment)
+    - [Build from source](#build-from-source)
+    - [Running tests](#running-tests)
 
 ## Install
 
 Install using pip:
 
 ```sh
 pip install pydgraph
@@ -237,18 +245,20 @@
 ## Supported Versions
 
 Depending on the version of Dgraph that you are connecting to, you will have to
 use a different version of this client.
 
 | Dgraph version |   pydgraph version   |
 |:--------------:|:--------------------:|
-|     1.0.X      |      <= *1.2.0*      |
-|     1.1.X      |      >= *2.0.0*      |
-|     1.2.X      |      >= *2.0.0*      |
-|    23.X.Y      |      >= *23.0.0*     |
+|    20.3.X      |      *20.3.0*        |
+|    20.7.X      |      *20.7.0*        |
+|    20.11.X     |      *20.7.0*        |
+|    21.03.X     |      *21.3.0*        |
+|    22.0.X      |      *21.3.0*        |
+|    23.0.X      |      *23.0.0*        |
 
 ## Quickstart
 
 Build and run the [simple project][simple] in the `examples` folder, which
 contains an end-to-end example of using the Dgraph python client. For additional details, follow the
 instructions in the project's [README](./examples/simple/README.md).
 
@@ -260,78 +270,114 @@
 
 You can initialize a `DgraphClient` object by passing it a list of
 `DgraphClientStub` clients as variadic arguments. Connecting to multiple Dgraph
 servers in the same cluster allows for better distribution of workload.
 
 The following code snippet shows just one connection.
 
-```python
+```python3
 import pydgraph
 
 client_stub = pydgraph.DgraphClientStub('localhost:9080')
 client = pydgraph.DgraphClient(client_stub)
 ```
 
+### Login into a Namespace
+
+If your server has Access Control Lists enabled (Dgraph v1.1 or above), the client must be
+logged in for accessing data. Use `login` endpoint:
+
+Calling login will obtain and remember the access and refresh JWT tokens. All subsequent operations
+via the logged in client will send along the stored access token.
+
+```python3
+client.login("groot", "password")
+```
+
+If your server additionally has namespaces (Dgraph v21.03 or above), use the
+`login_into_namespace` API.
+
+```python3
+client.login_into_namespace("groot", "password", "123")
+```
+
+### Connecting To Dgraph Cloud
+
+If you want to connect to Dgraph running on [Dgraph Cloud](https://cloud.dgraph.io) instance, then
+get the gRPC endpoint of your cluster that you can find in the
+[Settings section](https://cloud.dgraph.io/_/settings) of Dgraph Cloud console and obtain a Client
+or Admin API key (created in the [API key tab](https://cloud.dgraph.io/_/settings?tab=api-keys)
+of the Setting section). Create the `client_stub` using the gRPC endpoint and the API key:
+
+```python3
+client_stub = pydgraph.DgraphClientStub.from_cloud(
+    "https://morning-glade.grpc.us-east-1.aws.cloud.dgraph.io:443", "<api-key>")
+client = pydgraph.DgraphClient(client_stub)
+```
+
+The `DgraphClientStub.from_slash_endpoint()` method has been removed v23.0.
+Please use `DgraphClientStub.from_cloud()` instead.
+
 ### Altering the Database
 
 To set the schema, create an `Operation` object, set the schema and pass it to
 `DgraphClient#alter(Operation)` method.
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema)
 client.alter(op)
 ```
 
+`Operation` contains other fields as well, including `DropAttr` and `DropAll`. `DropAll` is
+useful if you wish to discard all the data, and start from a clean slate, without bringing
+the instance down. `DropAttr` is used to drop all the data related to a predicate.
+
+```python3
+# Drop all data including schema from the Dgraph instance. This is a useful
+# for small examples such as this since it puts Dgraph into a clean state.
+op = pydgraph.Operation(drop_all=True)
+client.alter(op)
+```
+
 Indexes can be computed in the background.
 You can set the `run_in_background` field of `pydgraph.Operation` to `True`
 before passing it to the `Alter` function. You can find more details
 [here](https://docs.dgraph.io/master/query-language/#indexes-in-background).
 
-```python
+```python3
 schema = 'name: string @index(exact) .'
 op = pydgraph.Operation(schema=schema, run_in_background=True)
 client.alter(op)
 ```
 
-`Operation` contains other fields as well, including the `drop` predicate and `drop all`.
-Drop all is useful if you wish to discard all the data, and start with a clean
-slate, without bringing the instance down.
-
-```python
-# Drop all data including schema from the Dgraph instance. This is a useful
-# for small examples such as this since it puts Dgraph into a clean state.
-op = pydgraph.Operation(drop_all=True)
-client.alter(op)
-```
-
 ### Creating a Transaction
 
 To create a transaction, call the `DgraphClient#txn()` method, which returns a
 new `Txn` object. This operation incurs no network overhead.
 
 It is good practice to call `Txn#discard()` in a `finally` block after running
 the transaction. Calling `Txn#discard()` after `Txn#commit()` is a no-op
 and you can call `Txn#discard()` multiple times with no additional side-effects.
 
-```python
+```python3
 txn = client.txn()
 try:
   # Do something here
   # ...
 finally:
   txn.discard()
   # ...
 ```
 
 To create a read-only transaction, call `DgraphClient#txn(read_only=True)`.
 Read-only transactions are ideal for transactions which only involve queries.
 Mutations and commits are not allowed.
 
-```python
+```python3
 txn = client.txn(read_only=True)
 try:
   # Do some queries here
   # ...
 finally:
   txn.discard()
   # ...
@@ -351,42 +397,39 @@
 
 `Txn#mutate()` provides convenience keyword arguments `set_obj` and `del_obj`
 for setting JSON values and `set_nquads` and `del_nquads` for setting N-Quad
 values. See examples below for usage.
 
 We define a person object to represent a person and use it in a transaction.
 
-```python
+```python3
 # Create data.
-p = {
-    'name': 'Alice',
-}
+p = { 'name': 'Alice' }
 
 # Run mutation.
 txn.mutate(set_obj=p)
 
 # If you want to use a mutation object, use this instead:
 # mu = pydgraph.Mutation(set_json=json.dumps(p).encode('utf8'))
 # txn.mutate(mu)
 
 # If you want to use N-Quads, use this instead:
 # txn.mutate(set_nquads='_:alice <name> "Alice" .')
 ```
 
-```python
-# Delete data.
+```python3
+# Delete data
 
 query = """query all($a: string)
  {
    all(func: eq(name, $a))
     {
       uid
     }
   }"""
-
 variables = {'$a': 'Bob'}
 
 res = txn.query(query, variables=variables)
 ppl = json.loads(res.json)
 
 # For a mutation to delete a node, use this:
 txn.mutate(del_obj=person)
@@ -397,59 +440,32 @@
 
 Sometimes, you only want to commit a mutation, without querying anything further.
 In such cases, you can set the keyword argument `commit_now=True` to indicate
 that the mutation must be immediately committed.
 
 A mutation can be executed using `txn.do_request` as well.
 
-```python
+```python3
 mutation = txn.create_mutation(set_nquads='_:alice <name> "Alice" .')
 request = txn.create_request(mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
-### Committing a Transaction
-
-A transaction can be committed using the `Txn#commit()` method. If your transaction
-consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
-`Txn#mutate`, then calling `Txn#commit()` is not necessary.
-
-An error is raised if another transaction(s) modify the same data concurrently that was
-modified in the current transaction. It is up to the user to retry transactions
-when they fail.
-
-```python
-txn = client.txn()
-try:
-  # ...
-  # Perform any number of queries and mutations
-  # ...
-  # and finally...
-  txn.commit()
-except pydgraph.AbortedError:
-  # Retry or handle exception.
-finally:
-  # Clean up. Calling this after txn.commit() is a no-op
-  # and hence safe.
-  txn.discard()
-```
-
 ### Running a Query
 
 You can run a query by calling `Txn#query(string)`. You will need to pass in a
-[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass an additional dictionary of any
-variables that you might want to set in the query, call
-`Txn#query(string, variables=d)` with the variables dictionary `d`.
+[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass
+an additional dictionary of any variables that you might want to set in the query,
+call `Txn#query(string, variables=d)` with the variables dictionary `d`.
 
 The query response contains the `json` field, which returns the JSON response.
-
 Let’s run a query with a variable `$a`, deserialize the result from JSON and
 print it out:
 
-```python
+```python3
 # Run query.
 query = """query all($a: string) {
   all(func: eq(name, $a))
   {
     name
   }
 }"""
@@ -473,94 +489,138 @@
 ```console
 Number of people named "Alice": 1
 Alice
 ```
 
 You can also use `txn.do_request` function to run the query.
 
-```python
+```python3
 request = txn.create_request(query=query)
 txn.do_request(request)
 ```
 
+### Query with RDF response
+
+You can get query result as a RDF response by calling `Txn#query(string)` with `resp_format` set
+to `RDF`. The response would contain a `rdf` field, which has the RDF encoded result.
+
+**Note:** If you are querying only for `uid` values, use a JSON format response.
+
+```python3
+res = txn.query(query, variables=variables, resp_format="RDF")
+print(res.rdf)
+```
+
 ### Running an Upsert: Query + Mutation
 
 The `txn.do_request` function allows you to use upsert blocks. An upsert block
 contains one query block and one or more mutation blocks, so it lets you perform
 queries and mutations in a single request. Variables defined in the query block
 can be used in the mutation blocks using the `uid` and `val` functions
 implemented by DQL.
 
 To learn more about upsert blocks, see the
 [Upsert Block documentation](https://dgraph.io/docs/mutations/upsert-block/).
 
-```python
+```python3
 query = """{
   u as var(func: eq(name, "Alice"))
 }"""
+
 nquad = """
   uid(u) <name> "Alice" .
   uid(u) <age> "25" .
 """
+
 mutation = txn.create_mutation(set_nquads=nquad)
 request = txn.create_request(query=query, mutations=[mutation], commit_now=True)
 txn.do_request(request)
 ```
 
 ### Running a Conditional Upsert
 
-The upsert block also allows specifying a conditional mutation block using an `@if` directive. The mutation is executed
-only when the specified condition is true. If the condition is false, the mutation is silently ignored.
+The upsert block also allows specifying a conditional mutation block using an `@if` directive.
+The mutation is executed only when the specified condition is true. If the condition is false,
+the mutation is silently ignored.
 
 See more about Conditional Upserts [here](https://docs.dgraph.io/mutations/#conditional-upsert).
 
-```python
+```python3
 query = """
   {
     user as var(func: eq(email, "wrong_email@dgraph.io"))
   }
 """
+
 cond = "@if(eq(len(user), 1))"
 nquads = """
   uid(user) <email> "correct_email@dgraph.io" .
 """
+
 mutation = txn.create_mutation(cond=cond, set_nquads=nquads)
 request = txn.create_request(mutations=[mutation], query=query, commit_now=True)
 txn.do_request(request)
 ```
 
+### Committing a Transaction
+
+A transaction can be committed using the `Txn#commit()` method. If your transaction
+consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
+`Txn#mutate`, then calling `Txn#commit()` is not necessary.
+
+An error is raised if another transaction(s) modify the same data concurrently that was
+modified in the current transaction. It is up to the user to retry transactions
+when they fail.
+
+```python3
+txn = client.txn()
+try:
+  # ...
+  # Perform any number of queries and mutations
+  # ...
+  # and finally...
+  txn.commit()
+except pydgraph.AbortedError:
+  # Retry or handle exception.
+finally:
+  # Clean up. Calling this after txn.commit() is a no-op
+  # and hence safe.
+  txn.discard()
+```
+
 ### Cleaning Up Resources
 
 To clean up resources, you have to call `DgraphClientStub#close()` individually for
 all the instances of `DgraphClientStub`.
 
-```python
-SERVER_ADDR = "localhost:9080"
+```python3
+SERVER_ADDR1 = "localhost:9080"
+SERVER_ADDR2 = "localhost:9080"
 
 # Create instances of DgraphClientStub.
-stub1 = pydgraph.DgraphClientStub(SERVER_ADDR)
-stub2 = pydgraph.DgraphClientStub(SERVER_ADDR)
+stub1 = pydgraph.DgraphClientStub(SERVER_ADDR1)
+stub2 = pydgraph.DgraphClientStub(SERVER_ADDR2)
 
 # Create an instance of DgraphClient.
 client = pydgraph.DgraphClient(stub1, stub2)
 
-# ...
 # Use client
-# ...
+...
 
 # Clean up resources by closing all client stubs.
 stub1.close()
 stub2.close()
 ```
 
 ### Setting Metadata Headers
 
-Metadata headers such as authentication tokens can be set through the metadata of gRPC methods. Below is an example of how to set a header named "auth-token".
+Metadata headers such as authentication tokens can be set through the metadata of gRPC methods.
+Below is an example of how to set a header named "auth-token".
 
-```python
+```python3
 # The following piece of code shows how one can set metadata with
 # auth-token, to allow Alter operation, if the server requires it.
 # metadata is a list of arbitrary key-value pairs.
 metadata = [("auth-token", "the-auth-token-value")]
 dg.alter(op, metadata=metadata)
 ```
 
@@ -568,96 +628,85 @@
 
 A timeout value representing the number of seconds can be passed to the `login`,
 `alter`, `query`, and `mutate` methods using the `timeout` keyword argument.
 
 For example, the following alters the schema with a timeout of ten seconds:
 `dg.alter(op, timeout=10)`
 
-### Passing credentials
-
-A `CallCredentials` object can be passed to the `login`, `alter`, `query`, and
-`mutate` methods using the `credentials` keyword argument.
-
-### Authenticating to a reverse TLS proxy
-
-If the Dgraph instance is behind a reverse TLS proxy, credentials can also be
-passed through the methods available in the gRPC library. Note that in this case
-every request will need to include the credentials. In the example below, we are
-trying to add authentication to a proxy that requires an API key. This value is
-expected to be included in the metadata using the key "authorization".
-
-```python
-creds = grpc.ssl_channel_credentials()
-call_credentials = grpc.metadata_call_credentials(
-    lambda context, callback: callback((("authorization", "<api-key>"),), None))
-composite_credentials = grpc.composite_channel_credentials(creds, call_credentials)
-client_stub = pydgraph.DgraphClientStub(
-    '{host}:{port}'.format(host=GRPC_HOST, port=GRPC_PORT), composite_credentials)
-client = pydgraph.DgraphClient(client_stub)
-```
-
 ### Async methods
 
 The `alter` method in the client has an asynchronous version called
 `async_alter`. The async methods return a future. You can directly call the
 `result` method on the future. However. The DgraphClient class provides a static
 method `handle_alter_future` to handle any possible exception.
 
-```python
+```python3
 alter_future = self.client.async_alter(pydgraph.Operation(
 	schema="name: string @index(term) ."))
 response = pydgraph.DgraphClient.handle_alter_future(alter_future)
 ```
 
 The `query` and `mutate` methods int the `Txn` class also have async versions
 called `async_query` and `async_mutation` respectively. These functions work
 just like `async_alter`.
 
 You can use the `handle_query_future` and `handle_mutate_future` static methods
 in the `Txn` class to retrieve the result. A short example is given below:
 
-```python
+```python3
 txn = client.txn()
 query = "query body here"
 future = txn.async_query()
 response = pydgraph.Txn.handle_query_future(future)
 ```
 
-A working example can be found in the `test_asycn.py` test file.
-
 Keep in mind that due to the nature of async calls, the async functions cannot
 retry the request if the login is invalid. You will have to check for this error
 and retry the login (with the function `retry_login` in both the `Txn` and
 `Client` classes). A short example is given below:
 
-```python
+```python3
 client = DgraphClient(client_stubs) # client_stubs is a list of gRPC stubs.
 alter_future = client.async_alter()
 try:
     response = alter_future.result()
 except Exception as e:
 	# You can use this function in the util package to check for JWT
     # expired errors.
     if pydgraph.util.is_jwt_expired(e):
         # retry your request here.
 ```
 
 ## Examples
 
+[tls]: ./examples/tls
+[parse_datetime]: ./examples/parse_datetime
+
 - [simple][]: Quickstart example of using pydgraph.
+- [tls][]: Quickstart example that uses TLS.
+- [parse_datetime]: Demonstration of converting Dgraph's DateTime strings to native python datetime.
 
 ## Development
 
+### Setting up environment
+
+There are many ways to set up your local Python environment. We suggest some sane defaults here.
+
+- Use [pyenv](https://github.com/pyenv/pyenv) to manage your Python installations.
+- Most recent versions of Python should work, but the version of Python officially supported is located in
+`.python-version`
+- Create a Python virtual environment using `python -m venv .venv`
+- Activate virtual environment via `source .venv/bin/activate`
+
 ### Build from source
 
 To build and install pydgraph locally, run
 
 ```sh
-python -m build
-pip install -e .
+pip install -e ".[dev]"
 ```
 
 If you have made changes to the `pydgraph/proto/api.proto` file, you need need
 to regenerate the source files generated by Protocol Buffer tools. To do that,
 install the [grpcio-tools][grpcio-tools] library and then run the following
 command:
 
@@ -679,15 +728,16 @@
 
 To run the tests in your local machine, run:
 
 ```bash
 bash scripts/local-test.sh
 ```
 
-This script assumes dgraph is located on your path.  Dgraph release binaries can be found [here](https://github.com/dgraph-io/dgraph/releases).
+This script assumes dgraph is located on your path. Dgraph release binaries can
+be found [here](https://github.com/dgraph-io/dgraph/releases).
 The test script also requires that `docker` and `docker compose` are installed on
 your machine.
 
 The script will take care of bringing up a Dgraph cluster and bringing it down
 after the tests are executed. The script connects to randomly selected ports for
 HTTP and gRPC requests to prevent interference with clusters running on the
 default port. Docker and docker-compose need to be installed before running the
```

### Comparing `joshua-test1-23.0.0rc3/joshua_test1.egg-info/SOURCES.txt` & `joshua-test1-23.0.1/joshua_test1.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 joshua_test1.egg-info/SOURCES.txt
 joshua_test1.egg-info/dependency_links.txt
 joshua_test1.egg-info/requires.txt
 joshua_test1.egg-info/top_level.txt
 pydgraph/__init__.py
 pydgraph/client.py
 pydgraph/client_stub.py
+pydgraph/convert.py
 pydgraph/errors.py
 pydgraph/meta.py
 pydgraph/txn.py
 pydgraph/util.py
 pydgraph/proto/__init__.py
 pydgraph/proto/api_pb2.py
 pydgraph/proto/api_pb2_grpc.py
 tests/test_acct_upsert.py
 tests/test_acl.py
 tests/test_async.py
 tests/test_client.py
 tests/test_client_stub.py
+tests/test_convert.py
 tests/test_essentials.py
 tests/test_queries.py
 tests/test_txn.py
 tests/test_type_system.py
 tests/test_upsert_block.py
 tests/test_util.py
```

### Comparing `joshua-test1-23.0.0rc3/pydgraph/__init__.py` & `joshua-test1-23.0.1/pydgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/pydgraph/client.py` & `joshua-test1-23.0.1/pydgraph/client.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/pydgraph/client_stub.py` & `joshua-test1-23.0.1/pydgraph/client_stub.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,30 +83,29 @@
         try:
             self.channel.close()
         except:
             pass
         del self.channel
         del self.stub
 
-    # from_slash_endpoint is deprecated and will be removed in v21.07 release.
-    # Use from_cloud method to connect to dgraph cloud backend.
-    @staticmethod
-    def from_slash_endpoint(cloud_endpoint, api_key):
-        return from_cloud(cloud_endpoint, api_key)
-
+    # accepts grpc endpoint as copied in cloud console as well as graphql endpoint
     # Usage:
     # import pydgraph
     # client_stub = pydgraph.DgraphClientStub.from_cloud("cloud_endpoint", "api-key")
     # client = pydgraph.DgraphClient(client_stub)
     @staticmethod
     def from_cloud(cloud_endpoint, api_key):
-        """Returns Dgraph Client stub for the Slash GraphQL endpoint"""
-        url = urlparse(cloud_endpoint)
-        url_parts = url.netloc.split(".", 1)
-        host = url_parts[0] + ".grpc." + url_parts[1]
+        """Returns Dgraph Client stub for the Dgraph Cloud endpoint"""
+        if cloud_endpoint.startswith("http"): # catch http:// and https://
+            host = urlparse(cloud_endpoint).netloc
+        else:
+            host = cloud_endpoint.split(":",1)[0] # remove port if any
+        if not ".grpc." in host:
+            url_parts = host.split(".", 1)
+            host = url_parts[0] + ".grpc." + url_parts[1]
         creds = grpc.ssl_channel_credentials()
         call_credentials = grpc.metadata_call_credentials(
             lambda context, callback: callback((("authorization", api_key),), None))
         composite_credentials = grpc.composite_channel_credentials(
             creds, call_credentials)
         client_stub = DgraphClientStub('{host}:{port}'.format(
             host=host, port="443"), composite_credentials, options=(('grpc.enable_http_proxy', 0),))
```

### Comparing `joshua-test1-23.0.0rc3/pydgraph/errors.py` & `joshua-test1-23.0.1/pydgraph/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,7 @@
     def __str__(self):
         return str(self.exception)
 
 class TransactionError(Exception):
     """Error thrown when the transaction is invalid (e.g trying to mutate in read-only mode)."""
     def __init__(self, msg):
         super(TransactionError, self).__init__(msg)
-
```

### Comparing `joshua-test1-23.0.0rc3/pydgraph/meta.py` & `joshua-test1-23.0.1/pydgraph/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata about this package."""
 
-VERSION = '23.0.0rc3'
+VERSION = '23.0.1'
```

### Comparing `joshua-test1-23.0.0rc3/pydgraph/proto/api_pb2.py` & `joshua-test1-23.0.1/pydgraph/proto/api_pb2.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/pydgraph/proto/api_pb2_grpc.py` & `joshua-test1-23.0.1/pydgraph/proto/api_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import api_pb2 as api__pb2
+import api_pb2 as api__pb2
 
 
 class DgraphStub(object):
     """Graph response.
     """
 
     def __init__(self, channel):
```

### Comparing `joshua-test1-23.0.0rc3/pydgraph/txn.py` & `joshua-test1-23.0.1/pydgraph/txn.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/pydgraph/util.py` & `joshua-test1-23.0.1/pydgraph/util.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/pyproject.toml` & `joshua-test1-23.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 [build-system]
 requires = ["setuptools==67.7.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joshua-test1"
-#authors = [
-#  { name="Dgraph Labs", email="contact@dgraph.io" },
-#]
+authors = [
+  { name="Dgraph Labs", email="contact@dgraph.io" },
+]
 license = {file = "LICENSE" }
 description = "Official Dgraph client implementation for Python"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.7"
 classifiers=[
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     'Topic :: Database',
     'Topic :: Software Development',
     'Programming Language :: Python :: 3.11',
 ]
-dependencies = [ "grpcio==1.53.0", "protobuf==4.22.0" ]
+dependencies = [ "grpcio==1.54.0", "protobuf==4.22.3" ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "pydgraph.meta.VERSION"}
 
+[project.optional-dependencies]
+dev = [
+  "build==0.10.0",
+  "grpcio-tools==1.54.0",
+  "pytest==7.3.1",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/dgraph-io/pydgraph"
```

### Comparing `joshua-test1-23.0.0rc3/tests/test_acct_upsert.py` & `joshua-test1-23.0.1/tests/test_acct_upsert.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_acl.py` & `joshua-test1-23.0.1/tests/test_acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 import subprocess
 import time
 
 __author__ = 'Animesh Pathak <animesh@dgrpah.io>'
 __maintainer__ = 'Animesh Pathak <animesh@dgrpah.io>'
 
 import logging
-import os
+import shutil
 import unittest
 
 from . import helper
 import pydgraph
 
+@unittest.skipIf(shutil.which('dgraph') is None, 'Dgraph binary not found.')
 class TestACL(helper.ClientIntegrationTestCase):
     user_id = 'alice'
     group_id = 'dev'
     user_password = 'simplepassword'
 
     def setUp(self):
         super(TestACL, self).setUp()
```

### Comparing `joshua-test1-23.0.0rc3/tests/test_async.py` & `joshua-test1-23.0.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_client.py` & `joshua-test1-23.0.1/tests/test_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,28 +14,24 @@
 
 """Tests construction of Dgraph client."""
 
 __author__ = 'Garvit Pahal <garvit@dgraph.io>'
 __maintainer__ = 'Martin Martinez Rivera <martinmr@dgraph.io>'
 
 import unittest
-
 import pydgraph
 
-
 class TestDgraphClient(unittest.TestCase):
     """Tests construction of Dgraph client."""
     def test_constructor(self):
         with self.assertRaises(ValueError):
             pydgraph.DgraphClient()
 
-
 def suite():
     """Returns a tests suite object."""
     suite_obj = unittest.TestSuite()
     suite_obj.addTest(TestDgraphClient())
     return suite_obj
 
-
 if __name__ == '__main__':
     runner = unittest.TextTestRunner()
     runner.run(suite())
```

### Comparing `joshua-test1-23.0.0rc3/tests/test_client_stub.py` & `joshua-test1-23.0.1/tests/test_client_stub.py`

 * *Files 25% similar despite different names*

```diff
@@ -48,18 +48,38 @@
     def test_close(self):
         client_stub = pydgraph.DgraphClientStub(addr=self.TEST_SERVER_ADDR)
         self.check_version(client_stub)
         client_stub.close()
         with self.assertRaises(Exception):
             client_stub.check_version(pydgraph.Check())
 
+class TestFromCloud(unittest.TestCase):
+    """Tests the from_cloud function"""
+    def test_from_cloud(self):
+        testcases = [
+            {"endpoint": "godly.grpc.region.aws.cloud.dgraph.io"},
+            {"endpoint": "godly.grpc.region.aws.cloud.dgraph.io:443"},
+            {"endpoint": "https://godly.region.aws.cloud.dgraph.io/graphql"},
+            {"endpoint": "godly.region.aws.cloud.dgraph.io"},
+            {"endpoint": "https://godly.region.aws.cloud.dgraph.io"},
+            {"endpoint": "godly.region.aws.cloud.dgraph.io:random"},
+            {"endpoint": "random:url", "error": True},
+            {"endpoint": "google", "error": True},
+        ]
+
+        for case in testcases:
+            try:
+                pydgraph.DgraphClientStub.from_cloud(case["endpoint"], "api-key")
+            except IndexError as e:
+                if not case["error"]:
+                    # we didn't expect an error
+                    raise(e)
 
 def suite():
     """Returns a test suite object."""
     suite_obj = unittest.TestSuite()
     suite_obj.addTest(TestDgraphClientStub())
     return suite_obj
 
-
 if __name__ == '__main__':
     runner = unittest.TextTestRunner()
     runner.run(suite())
```

### Comparing `joshua-test1-23.0.0rc3/tests/test_essentials.py` & `joshua-test1-23.0.1/tests/test_essentials.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_queries.py` & `joshua-test1-23.0.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_txn.py` & `joshua-test1-23.0.1/tests/test_txn.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 __author__ = 'Garvit Pahal <garvit@dgraph.io>'
 __maintainer__ = 'Garvit Pahal <garvit@dgraph.io>'
 
 import unittest
 import logging
 import json
+import time
 
 import pydgraph
 
 from . import helper
 
 
 class TestTxn(helper.ClientIntegrationTestCase):
@@ -230,16 +231,20 @@
         resp = self.client.txn(read_only=True).query(query)
         self.assertEqual([{'name': 'Manish2'}], json.loads(resp.json).get('me'))
 
     def test_read_only_txn(self):
         """Tests read-only transactions. Read-only transactions should
         not advance the start ts nor should allow mutations or commits."""
 
-        query = '{ me() {} }'
+        # We sleep here so that rollups do not move the MaxAssigned.
+        # Starting Dgraph v23, rollups can move the MaxAssigned too.
+        # PR: https://github.com/dgraph-io/dgraph/pull/8774
+        time.sleep(1)
 
+        query = '{ me() {} }'
         resp1 = self.client.txn(read_only=True).query(query)
         start_ts1 = resp1.txn.start_ts
         resp2 = self.client.txn(read_only=True).query(query)
         start_ts2 = resp2.txn.start_ts
         self.assertEqual(start_ts1, start_ts2)
 
         txn = self.client.txn(read_only=True)
@@ -257,24 +262,29 @@
     def test_best_effort_txn(self):
         """Tests best-effort transactions."""
 
         helper.drop_all(self.client)
         helper.set_schema(self.client, 'name: string @index(exact) .')
 
         txn = self.client.txn()
-        _ = txn.mutate(set_obj={'name': 'Manish'})
+        resp = txn.mutate(set_obj={'name': 'Manish'})
         txn.commit()
+        mu_ts = resp.txn.commit_ts
 
         query = '{ me(func: has(name)) {name} }'
         with self.assertRaises(Exception):
             self.client.txn(read_only=False, best_effort=True)
 
-        txn = self.client.txn(read_only=True, best_effort=True)
-        resp = txn.query(query)
-        self.assertEqual([], json.loads(resp.json).get('me'))
+        while True:
+            txn = self.client.txn(read_only=True, best_effort=True)
+            resp = txn.query(query)
+            if resp.txn.start_ts < mu_ts:
+                continue
+            self.assertEqual([], json.loads(resp.json).get('me'))
+            break
 
         with self.assertRaises(Exception):
             txn.mutate(set_obj={'name': 'Manish'})
         with self.assertRaises(Exception):
             txn.commit()
 
     def test_conflict(self):
```

### Comparing `joshua-test1-23.0.0rc3/tests/test_type_system.py` & `joshua-test1-23.0.1/tests/test_type_system.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_upsert_block.py` & `joshua-test1-23.0.1/tests/test_upsert_block.py`

 * *Files identical despite different names*

### Comparing `joshua-test1-23.0.0rc3/tests/test_util.py` & `joshua-test1-23.0.1/tests/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,32 +16,28 @@
 
 __author__ = 'Garvit Pahal <garvit@dgraph.io>'
 __maintainer__ = 'Martin Martinez Rivera <martinmr@dgraph.io>'
 
 import unittest
 
 from pydgraph import util
-import pydgraph
 
-from . import helper
-
-
-class TestIsString(unittest.TestCase):
-    """Tests is_string utility function."""
+class TestUtil(unittest.TestCase):
+    """Tests util utility functions."""
 
     def test_is_string(self):
         self.assertTrue(util.is_string(''))
         self.assertTrue(util.is_string('a'))
         self.assertFalse(util.is_string(object()))
         self.assertFalse(util.is_string({}))
 
-
 def suite():
     """Returns a test suite object."""
     suite_obj = unittest.TestSuite()
-    suite_obj.addTest(TestIsString())
+    suite_obj.addTest(TestUtil())
     return suite_obj
 
 
 if __name__ == '__main__':
     runner = unittest.TextTestRunner()
     runner.run(suite())
+
```

