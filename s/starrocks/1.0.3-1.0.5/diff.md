# Comparing `tmp/starrocks-1.0.3.tar.gz` & `tmp/starrocks-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrocks-1.0.3.tar", last modified: Thu Mar  2 04:41:21 2023, max compression
+gzip compressed data, was "starrocks-1.0.5.tar", last modified: Mon May 29 11:02:55 2023, max compression
```

## Comparing `starrocks-1.0.3.tar` & `starrocks-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-03-02 04:41:21.626432 starrocks-1.0.3/
--rw-r--r--   0 wangriyu   (501) staff       (20)    10234 2023-03-01 07:54:04.000000 starrocks-1.0.3/LICENSE
--rw-r--r--   0 wangriyu   (501) staff       (20)     2141 2023-03-02 04:41:21.626227 starrocks-1.0.3/PKG-INFO
--rw-r--r--   0 wangriyu   (501) staff       (20)     1419 2023-03-02 03:49:44.000000 starrocks-1.0.3/README.md
--rw-r--r--   0 wangriyu   (501) staff       (20)       38 2023-03-02 04:41:21.626490 starrocks-1.0.3/setup.cfg
--rw-r--r--   0 wangriyu   (501) staff       (20)     2246 2023-03-02 03:49:44.000000 starrocks-1.0.3/setup.py
-drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-03-02 04:41:21.623306 starrocks-1.0.3/starrocks/
--rw-r--r--   0 wangriyu   (501) staff       (20)      653 2023-03-02 04:40:37.000000 starrocks-1.0.3/starrocks/__init__.py
-drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-03-02 04:41:21.625763 starrocks-1.0.3/starrocks/sqlalchemy/
--rw-r--r--   0 wangriyu   (501) staff       (20)      755 2023-03-02 04:39:57.000000 starrocks-1.0.3/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 wangriyu   (501) staff       (20)     7364 2023-03-01 07:54:04.000000 starrocks-1.0.3/starrocks/sqlalchemy/dialect.py
-drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-03-02 04:41:21.625205 starrocks-1.0.3/starrocks.egg-info/
--rw-r--r--   0 wangriyu   (501) staff       (20)     2141 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/PKG-INFO
--rw-r--r--   0 wangriyu   (501) staff       (20)      345 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/SOURCES.txt
--rw-r--r--   0 wangriyu   (501) staff       (20)        1 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/dependency_links.txt
--rw-r--r--   0 wangriyu   (501) staff       (20)       80 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/entry_points.txt
--rw-r--r--   0 wangriyu   (501) staff       (20)        1 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/not-zip-safe
--rw-r--r--   0 wangriyu   (501) staff       (20)       50 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/requires.txt
--rw-r--r--   0 wangriyu   (501) staff       (20)       10 2023-03-02 04:41:21.000000 starrocks-1.0.3/starrocks.egg-info/top_level.txt
+drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-05-29 11:02:55.646245 starrocks-1.0.5/
+-rw-r--r--   0 wangriyu   (501) staff       (20)    10234 2023-05-27 04:35:02.000000 starrocks-1.0.5/LICENSE
+-rw-r--r--   0 wangriyu   (501) staff       (20)     2141 2023-05-29 11:02:55.646062 starrocks-1.0.5/PKG-INFO
+-rw-r--r--   0 wangriyu   (501) staff       (20)     1419 2023-05-27 04:35:02.000000 starrocks-1.0.5/README.md
+-rw-r--r--   0 wangriyu   (501) staff       (20)       38 2023-05-29 11:02:55.646296 starrocks-1.0.5/setup.cfg
+-rw-r--r--   0 wangriyu   (501) staff       (20)     2280 2023-05-27 04:35:02.000000 starrocks-1.0.5/setup.py
+drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-05-29 11:02:55.643027 starrocks-1.0.5/starrocks/
+-rw-r--r--   0 wangriyu   (501) staff       (20)      653 2023-05-29 08:41:18.000000 starrocks-1.0.5/starrocks/__init__.py
+drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-05-29 11:02:55.645649 starrocks-1.0.5/starrocks/sqlalchemy/
+-rw-r--r--   0 wangriyu   (501) staff       (20)      755 2023-05-27 04:35:02.000000 starrocks-1.0.5/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 wangriyu   (501) staff       (20)     2520 2023-05-29 08:41:18.000000 starrocks-1.0.5/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 wangriyu   (501) staff       (20)     5693 2023-05-29 08:41:18.000000 starrocks-1.0.5/starrocks/sqlalchemy/dialect.py
+drwxr-xr-x   0 wangriyu   (501) staff       (20)        0 2023-05-29 11:02:55.644819 starrocks-1.0.5/starrocks.egg-info/
+-rw-r--r--   0 wangriyu   (501) staff       (20)     2141 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/PKG-INFO
+-rw-r--r--   0 wangriyu   (501) staff       (20)      378 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/SOURCES.txt
+-rw-r--r--   0 wangriyu   (501) staff       (20)        1 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/dependency_links.txt
+-rw-r--r--   0 wangriyu   (501) staff       (20)       80 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/entry_points.txt
+-rw-r--r--   0 wangriyu   (501) staff       (20)        1 2023-05-29 08:50:35.000000 starrocks-1.0.5/starrocks.egg-info/not-zip-safe
+-rw-r--r--   0 wangriyu   (501) staff       (20)       72 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/requires.txt
+-rw-r--r--   0 wangriyu   (501) staff       (20)       10 2023-05-29 11:02:55.000000 starrocks-1.0.5/starrocks.egg-info/top_level.txt
```

### Comparing `starrocks-1.0.3/LICENSE` & `starrocks-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starrocks-1.0.3/PKG-INFO` & `starrocks-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrocks
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python interface to StarRocks
 Home-page: https://github.com/StarRocks/starrocks
 Author: StarRocks Team
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `starrocks-1.0.3/README.md` & `starrocks-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `starrocks-1.0.3/setup.py` & `starrocks-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Database :: Front-Ends",
     ],
     install_requires=[
         "sqlalchemy>=1.4, <2",
         "sqlalchemy-utils>=0.38.3, <0.39",
+        "mysqlclient>=2.1.0, <3",
     ],
     packages=find_packages(include=["starrocks", "starrocks.*"]),
     package_data={"": ["LICENSE", "README.md"]},
     include_package_data=True,
     zip_safe=False,
     entry_points={
         'sqlalchemy.dialects': [
```

### Comparing `starrocks-1.0.3/starrocks/__init__.py` & `starrocks-1.0.5/starrocks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.3"
+__version__ = "1.0.5"
```

### Comparing `starrocks-1.0.3/starrocks/sqlalchemy/__init__.py` & `starrocks-1.0.5/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `starrocks-1.0.3/starrocks.egg-info/PKG-INFO` & `starrocks-1.0.5/starrocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrocks
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python interface to StarRocks
 Home-page: https://github.com/StarRocks/starrocks
 Author: StarRocks Team
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

