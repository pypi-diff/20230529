# Comparing `tmp/seaplane-0.3.4.tar.gz` & `tmp/seaplane-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.3.4.tar", max compression
+gzip compressed data, was "seaplane-0.3.5.tar", max compression
```

## Comparing `seaplane-0.3.4.tar` & `seaplane-0.3.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.4/README.md
--rw-r--r--   0        0        0     2682 2023-05-29 16:57:26.458011 seaplane-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1120 2023-05-26 12:37:12.573449 seaplane-0.3.4/src/seaplane/__init__.py
--rw-r--r--   0        0        0       84 2023-05-10 16:07:33.887055 seaplane-0.3.4/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.4/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2558 2023-05-26 12:37:12.574515 seaplane-0.3.4/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-05-10 16:07:33.887468 seaplane-0.3.4/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-05-10 16:07:33.887602 seaplane-0.3.4/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-05-10 16:07:33.887749 seaplane-0.3.4/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-05-10 16:07:33.887880 seaplane-0.3.4/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-05-10 16:07:33.888017 seaplane-0.3.4/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1552 2023-05-10 16:07:33.888145 seaplane-0.3.4/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.4/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0     7075 2023-05-29 15:51:55.432747 seaplane-0.3.4/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1818 2023-05-26 12:37:12.575554 seaplane-0.3.4/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      213 2023-05-10 16:07:33.888776 seaplane-0.3.4/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.4/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.4/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.4/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.4/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-05-10 16:07:33.889518 seaplane-0.3.4/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-05-10 16:07:33.889686 seaplane-0.3.4/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.4/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.4/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-05-10 16:07:33.890085 seaplane-0.3.4/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.4/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      228 2023-05-26 12:37:12.575703 seaplane-0.3.4/src/seaplane/smartpipes/__init__.py
--rw-r--r--   0        0        0     6919 2023-05-29 16:39:25.320434 seaplane-0.3.4/src/seaplane/smartpipes/coprocessor.py
--rw-r--r--   0        0        0     8767 2023-05-29 16:37:53.773697 seaplane-0.3.4/src/seaplane/smartpipes/decorators.py
--rw-r--r--   0        0        0     3435 2023-05-29 16:56:13.680134 seaplane-0.3.4/src/seaplane/smartpipes/smartapi.py
--rw-r--r--   0        0        0     1810 2023-05-29 14:38:17.372462 seaplane-0.3.4/src/seaplane/smartpipes/smartpipe.py
--rw-r--r--   0        0        0     2141 2023-05-29 16:25:30.567871 seaplane-0.3.4/src/seaplane/smartpipes/store.py
--rw-r--r--   0        0        0       33 2023-05-29 06:02:49.125920 seaplane-0.3.4/src/seaplane/smartpipes/website/.gitignore
--rw-r--r--   0        0        0     1750 2023-05-26 12:37:12.578128 seaplane-0.3.4/src/seaplane/smartpipes/website/README.md
--rw-r--r--   0        0        0       77 2023-05-26 12:37:12.578349 seaplane-0.3.4/src/seaplane/smartpipes/website/jsconfig.json
--rw-r--r--   0        0        0      118 2023-05-26 12:37:12.578651 seaplane-0.3.4/src/seaplane/smartpipes/website/next.config.js
--rw-r--r--   0        0        0      650 2023-05-26 12:37:12.579148 seaplane-0.3.4/src/seaplane/smartpipes/website/package.json
--rw-r--r--   0        0        0       82 2023-05-26 12:37:12.579367 seaplane-0.3.4/src/seaplane/smartpipes/website/postcss.config.js
--rw-r--r--   0        0        0      717 2023-05-26 12:37:12.579749 seaplane-0.3.4/src/seaplane/smartpipes/website/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-05-26 12:37:12.579990 seaplane-0.3.4/src/seaplane/smartpipes/website/public/next.svg
--rw-r--r--   0        0        0    39147 2023-05-26 12:37:12.580576 seaplane-0.3.4/src/seaplane/smartpipes/website/public/openai.png
--rw-r--r--   0        0        0    11580 2023-05-26 12:37:12.581026 seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo.svg
--rw-r--r--   0        0        0     2296 2023-05-26 12:37:12.581272 seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
--rw-r--r--   0        0        0   195272 2023-05-26 12:37:12.582964 seaplane-0.3.4/src/seaplane/smartpipes/website/public/stabilityai.png
--rw-r--r--   0        0        0      629 2023-05-26 12:37:12.583286 seaplane-0.3.4/src/seaplane/smartpipes/website/public/vercel.svg
--rw-r--r--   0        0        0     3691 2023-05-26 12:37:12.583538 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/Header.jsx
--rw-r--r--   0        0        0    10990 2023-05-29 06:31:52.174486 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
--rw-r--r--   0        0        0     4313 2023-05-26 12:37:12.584085 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
--rw-r--r--   0        0        0      127 2023-05-26 12:37:12.584496 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/_app.js
--rw-r--r--   0        0        0      231 2023-05-26 12:37:12.584691 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/_document.js
--rw-r--r--   0        0        0     1962 2023-05-29 06:31:52.174956 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/index.js
--rw-r--r--   0        0        0     2626 2023-05-26 12:37:12.585484 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/tutorial.js
--rw-r--r--   0        0        0      228 2023-05-26 12:37:12.585759 seaplane-0.3.4/src/seaplane/smartpipes/website/src/styles/globals.css
--rw-r--r--   0        0        0      528 2023-05-26 12:37:12.586061 seaplane-0.3.4/src/seaplane/smartpipes/website/tailwind.config.js
--rw-r--r--   0        0        0   143162 2023-05-26 12:37:12.587625 seaplane-0.3.4/src/seaplane/smartpipes/website/yarn.lock
--rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.4/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.4/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     6545 2023-05-29 17:02:42.170563 seaplane-0.3.4/setup.py
--rw-r--r--   0        0        0     3182 2023-05-29 17:02:42.170917 seaplane-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.5/README.md
+-rw-r--r--   0        0        0     2682 2023-05-29 17:27:07.798183 seaplane-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1120 2023-05-26 12:37:12.573449 seaplane-0.3.5/src/seaplane/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-10 16:07:33.887055 seaplane-0.3.5/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.5/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2558 2023-05-26 12:37:12.574515 seaplane-0.3.5/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-05-10 16:07:33.887468 seaplane-0.3.5/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-05-10 16:07:33.887602 seaplane-0.3.5/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-05-10 16:07:33.887749 seaplane-0.3.5/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-05-10 16:07:33.887880 seaplane-0.3.5/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-05-10 16:07:33.888017 seaplane-0.3.5/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-05-10 16:07:33.888145 seaplane-0.3.5/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.5/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0     7077 2023-05-29 17:20:51.111035 seaplane-0.3.5/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1818 2023-05-26 12:37:12.575554 seaplane-0.3.5/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-10 16:07:33.888776 seaplane-0.3.5/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.5/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.5/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.5/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.5/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-05-10 16:07:33.889518 seaplane-0.3.5/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-10 16:07:33.889686 seaplane-0.3.5/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.5/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.5/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-05-10 16:07:33.890085 seaplane-0.3.5/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.5/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-26 12:37:12.575703 seaplane-0.3.5/src/seaplane/smartpipes/__init__.py
+-rw-r--r--   0        0        0     6919 2023-05-29 16:39:25.320434 seaplane-0.3.5/src/seaplane/smartpipes/coprocessor.py
+-rw-r--r--   0        0        0     8767 2023-05-29 16:37:53.773697 seaplane-0.3.5/src/seaplane/smartpipes/decorators.py
+-rw-r--r--   0        0        0     3512 2023-05-29 17:26:02.456891 seaplane-0.3.5/src/seaplane/smartpipes/smartapi.py
+-rw-r--r--   0        0        0     1810 2023-05-29 14:38:17.372462 seaplane-0.3.5/src/seaplane/smartpipes/smartpipe.py
+-rw-r--r--   0        0        0     2141 2023-05-29 16:25:30.567871 seaplane-0.3.5/src/seaplane/smartpipes/store.py
+-rw-r--r--   0        0        0       33 2023-05-29 06:02:49.125920 seaplane-0.3.5/src/seaplane/smartpipes/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-05-26 12:37:12.578128 seaplane-0.3.5/src/seaplane/smartpipes/website/README.md
+-rw-r--r--   0        0        0       77 2023-05-26 12:37:12.578349 seaplane-0.3.5/src/seaplane/smartpipes/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-05-26 12:37:12.578651 seaplane-0.3.5/src/seaplane/smartpipes/website/next.config.js
+-rw-r--r--   0        0        0      650 2023-05-26 12:37:12.579148 seaplane-0.3.5/src/seaplane/smartpipes/website/package.json
+-rw-r--r--   0        0        0       82 2023-05-26 12:37:12.579367 seaplane-0.3.5/src/seaplane/smartpipes/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-05-26 12:37:12.579749 seaplane-0.3.5/src/seaplane/smartpipes/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-05-26 12:37:12.579990 seaplane-0.3.5/src/seaplane/smartpipes/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-05-26 12:37:12.580576 seaplane-0.3.5/src/seaplane/smartpipes/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-05-26 12:37:12.581026 seaplane-0.3.5/src/seaplane/smartpipes/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-05-26 12:37:12.581272 seaplane-0.3.5/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-05-26 12:37:12.582964 seaplane-0.3.5/src/seaplane/smartpipes/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-05-26 12:37:12.583286 seaplane-0.3.5/src/seaplane/smartpipes/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-05-26 12:37:12.583538 seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10990 2023-05-29 06:31:52.174486 seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     4313 2023-05-26 12:37:12.584085 seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-05-26 12:37:12.584496 seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-05-26 12:37:12.584691 seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/_document.js
+-rw-r--r--   0        0        0     1962 2023-05-29 06:31:52.174956 seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/index.js
+-rw-r--r--   0        0        0     2626 2023-05-26 12:37:12.585484 seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/tutorial.js
+-rw-r--r--   0        0        0      228 2023-05-26 12:37:12.585759 seaplane-0.3.5/src/seaplane/smartpipes/website/src/styles/globals.css
+-rw-r--r--   0        0        0      528 2023-05-26 12:37:12.586061 seaplane-0.3.5/src/seaplane/smartpipes/website/tailwind.config.js
+-rw-r--r--   0        0        0   143162 2023-05-26 12:37:12.587625 seaplane-0.3.5/src/seaplane/smartpipes/website/yarn.lock
+-rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.5/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.5/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     6545 2023-05-29 17:27:54.973163 seaplane-0.3.5/setup.py
+-rw-r--r--   0        0        0     3182 2023-05-29 17:27:54.973824 seaplane-0.3.5/PKG-INFO
```

### Comparing `seaplane-0.3.4/README.md` & `seaplane-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/pyproject.toml` & `seaplane-0.3.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.3.4"
+version = "0.3.5"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
```

### Comparing `seaplane-0.3.4/src/seaplane/__init__.py` & `seaplane-0.3.5/src/seaplane/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/api_http.py` & `seaplane-0.3.5/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/api_request.py` & `seaplane-0.3.5/src/seaplane/api/api_request.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/compute_api.py` & `seaplane-0.3.5/src/seaplane/api/compute_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/formation_configuration_api.py` & `seaplane-0.3.5/src/seaplane/api/formation_configuration_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/lock_api.py` & `seaplane-0.3.5/src/seaplane/api/lock_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/metadata_api.py` & `seaplane-0.3.5/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/restrict_api.py` & `seaplane-0.3.5/src/seaplane/api/restrict_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/sql_api.py` & `seaplane-0.3.5/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/api/token_api.py` & `seaplane-0.3.5/src/seaplane/api/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/configuration.py` & `seaplane-0.3.5/src/seaplane/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .model.errors import SeaplaneError
 
 _SEAPLANE_COMPUTE_API_ENDPOINT = "https://compute.cplane.cloud/v2beta"
 _SEAPLANE_COORDINATION_API_ENDPOINT = "https://metadata.cplane.cloud/v1"
 _SEAPLANE_IDENTIFY_API_ENDPOINT = "https://flightdeck.cplane.cloud/v1"
 _SEAPLANE_GLOBAL_SQL_API_ENDPOINT = "https://sql.cplane.cloud/v1"
 
-_SEAPLANE_ENV_VAR_PRODUCTION = "SEAPLANE_PRODUCTION"
+_SEAPLANE_ENV_VAR_PRODUCTION = "SMARTPIPES_PRODUCTION"
 
 
 class Configuration:
     """
     Seaplane SDK Configuration.
 
     Everytime the configuration is changed,
```

### Comparing `seaplane-0.3.4/src/seaplane/logging/__init__.py` & `seaplane-0.3.5/src/seaplane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/compute/__init__.py` & `seaplane-0.3.5/src/seaplane/model/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/compute/formation_configuration.py` & `seaplane-0.3.5/src/seaplane/model/compute/formation_configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/locks/__init__.py` & `seaplane-0.3.5/src/seaplane/model/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/metadata/__init__.py` & `seaplane-0.3.5/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/restrict/__init__.py` & `seaplane-0.3.5/src/seaplane/model/restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/model/sql/__init__.py` & `seaplane-0.3.5/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/coprocessor.py` & `seaplane-0.3.5/src/seaplane/smartpipes/coprocessor.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/decorators.py` & `seaplane-0.3.5/src/seaplane/smartpipes/decorators.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/smartapi.py` & `seaplane-0.3.5/src/seaplane/smartpipes/smartapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from .decorators import context, smart_pipes_json
 from .smartpipe import SmartPipe
 import boto3 
 import os
 
 BUCKET_NAME = os.getenv("AWS_BUCKET_NAME")
 BUCKET_URL = f"https://{BUCKET_NAME}.s3.amazonaws.com/"
+SMARTPIPES_CORS = [i for i in os.getenv("SMARTPIPES_CORS", "http://localhost:3000").split(" ")] 
 
 s3 = boto3.client("s3")
 app = Flask(__name__)
-sio = SocketIO(app, cors_allowed_origins=["http://localhost:3000"], async_mode="threading")
-CORS(app, origins=["http://localhost:3000"])
+sio = SocketIO(app, cors_allowed_origins=SMARTPIPES_CORS, async_mode="threading")
+CORS(app, origins=SMARTPIPES_CORS)
 
 
 @sio.on("message")  # type: ignore
 def handle_message(data: Any) -> None:
     print("received message:", data)
```

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/smartpipe.py` & `seaplane-0.3.5/src/seaplane/smartpipes/smartpipe.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/store.py` & `seaplane-0.3.5/src/seaplane/smartpipes/store.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/README.md` & `seaplane-0.3.5/src/seaplane/smartpipes/website/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/package.json` & `seaplane-0.3.5/src/seaplane/smartpipes/website/package.json`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/favicon.ico` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/next.svg` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/next.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/openai.png` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/openai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo.svg` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/seaplane_logo.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/stabilityai.png` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/stabilityai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/public/vercel.svg` & `seaplane-0.3.5/src/seaplane/smartpipes/website/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/Header.jsx` & `seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/Header.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx` & `seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx` & `seaplane-0.3.5/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/index.js` & `seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/tutorial.js` & `seaplane-0.3.5/src/seaplane/smartpipes/website/src/pages/tutorial.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/tailwind.config.js` & `seaplane-0.3.5/src/seaplane/smartpipes/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/src/seaplane/smartpipes/website/yarn.lock` & `seaplane-0.3.5/src/seaplane/smartpipes/website/yarn.lock`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.4/setup.py` & `seaplane-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
  'tqdm>=4.65.0,<5.0.0',
  'types-requests>=2.28.0,<3.0.0',
  'types-simplejson>=3.17.7,<4.0.0',
  'urllib3==1.26.9']
 
 setup_kwargs = {
     'name': 'seaplane',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Seaplane Python SDK',
     'long_description': '# Seaplane Python SDK\n[![PyPI](https://badge.fury.io/py/seaplane.svg)](https://badge.fury.io/py/seaplane)\n[![Python](https://img.shields.io/pypi/pyversions/seaplane.svg?style=plastic)](https://badge.fury.io/py/seaplane)\n\nSimple Python library to manage your resources at seaplane.\n\n## What is Seaplane?\n\nSeaplane is the global platform for building and scaling your application stack\nwithout the complexity of managing cloud infrastructure.\n\nIt serves as a reference application for how our APIs can be utilized.\n\nNot sure where to go to quickly run a workload on Seaplane? See our [Getting\nStarted] guide.\n\nTo build and test this software yourself, see the CONTRIBUTING document that is a peer to this one.\n\n## Installation\n\n```shell\npip install seaplane\n```\n\n## Configure your API KEY\n\n* Set `SEAPLANE_API_KEY` environment variable.\n* Use `config` object in order to set the api key.\n\n```python\nfrom seaplane import sea\n\nsea.config.set_api_key("your_api_key")\n```\n\n## License\n\nLicensed under the Apache License, Version 2.0, [LICENSE]. Copyright 2022 Seaplane IO, Inc.\n\n[//]: # (Links)\n\n[Seaplane]: https://seaplane.io/\n[CLI]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-cli\n[SDK]: https://github.com/seaplane-io/seaplane/tree/main/seaplane\n[Getting Started]: https://github.com/seaplane-io/seaplane/blob/main/seaplane-sdk/python/docs/quickstart.md\n[CONTRIBUTING]: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python/CONTRIBUTIONS.md\n[LICENSE]: https://github.com/seaplane-io/seaplane/blob/main/LICENSE\n',
     'author': 'Seaplane IO, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python',
```

### Comparing `seaplane-0.3.4/PKG-INFO` & `seaplane-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.3.4
+Version: 0.3.5
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

