# Comparing `tmp/authomize-rest-api-client-4.1.2.tar.gz` & `tmp/authomize-rest-api-client-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.2.tar", last modified: Tue May 23 14:31:43 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.3.tar", last modified: Mon May 29 21:32:33 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.2.tar` & `authomize-rest-api-client-4.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75246 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35822 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189364 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89185 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-23 14:31:24.000000 authomize-rest-api-client-4.1.2/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-23 14:31:43.000000 authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-23 14:31:43.831340 authomize-rest-api-client-4.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-23 14:31:27.000000 authomize-rest-api-client-4.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75246 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35372 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   189364 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87696 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-29 21:32:14.000000 authomize-rest-api-client-4.1.3/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-29 21:32:33.000000 authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-29 21:32:33.860420 authomize-rest-api-client-4.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-29 21:32:17.000000 authomize-rest-api-client-4.1.3/setup.py
```

### Comparing `authomize-rest-api-client-4.1.2/LICENSE.txt` & `authomize-rest-api-client-4.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/README.md` & `authomize-rest-api-client-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-17T14:13:00+00:00
+#   timestamp: 2023-05-25T09:00:40+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -17,18 +17,14 @@
 
 
 class AccessToType(Enum):
     asset = 'asset'
     grouping = 'grouping'
 
 
-class Object(Enum):
-    account = 'account'
-
-
 class AddIncidentCommentRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     content: constr(max_length=1025) = Field(
         ..., description='Content of comment.', title='Content'
     )
@@ -89,18 +85,14 @@
         extra = Extra.forbid
 
     field_in: Optional[List[str]] = Field(
         default=[], alias='$in', description='In', title='$In'
     )
 
 
-class Object1(Enum):
-    asset = 'asset'
-
-
 class AttackTacticType(Enum):
     Collection = 'Collection'
     Credential_Access = 'Credential Access'
     Defense_Evasion = 'Defense Evasion'
     Discovery = 'Discovery'
     Exfiltration = 'Exfiltration'
     Impact = 'Impact'
@@ -252,18 +244,14 @@
 
 
 class IdentityExpansion(Enum):
     account = 'account'
     tags = 'tags'
 
 
-class Object2(Enum):
-    identity = 'identity'
-
-
 class IncidentExpansion(Enum):
     policy = 'policy'
     assignee = 'assignee'
 
 
 class IncidentsCreatedAtFilter(BaseModel):
     class Config:
@@ -375,15 +363,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.1.0', description='**version**', title='Version'
+        default='4.1.2', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -539,17 +527,19 @@
 
 class SourceAppSchema(BaseModel):
     id: str = Field(..., description='Unique ID', title='Id')
     name: str = Field(..., description='Name', title='Name')
 
 
 class TagSchema(BaseModel):
-    id: str = Field(..., description='Id', title='Id')
-    name: str = Field(..., description='Name', title='Name')
-    description: str = Field(..., description='Description', title='Description')
+    id: str = Field(..., description='Authomize ID for the Tag', title='Id')
+    name: str = Field(..., description='Name of the tag', title='Name')
+    description: str = Field(
+        ..., description='Description of the tag', title='Description'
+    )
 
 
 class UniqueIdFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[str]] = Field(
@@ -597,59 +587,54 @@
     name: Optional[str] = Field(
         default='SOC 2 (TSC 2017)', description='Name', title='Name'
     )
 
 
 class AssetSchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    object: Object1 = Field(
-        ..., description='Type of entity (here `asset`)', title='Object'
-    )
     name: str = Field(..., description='Name', title='Name')
     type: str = Field(..., description='Type', title='Type')
     originType: Optional[str] = Field(
         default=None,
         description='The asset type in the source system. The default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
-    sourceAppId: Optional[str] = Field(
-        default=None, description='Source App ID', title='Sourceappid'
-    )
     sourceApp: Optional[SourceAppSchema] = Field(
         default=None, description='Source App', title='Sourceapp'
     )
-    tagIds: Optional[List[str]] = Field(
-        default=[], description='Tag IDs', title='Tagids'
-    )
     createdAt: Optional[datetime] = Field(
         default=None,
         description='The date (in ISO 8601 format) that the asset was created.\n',
         title='Createdat',
     )
-    lastUsedAt: Optional[datetime] = Field(
+    lastUsedAt: Optional[str] = Field(
         default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.',
         title='Lastusedat',
     )
     href: Optional[str] = Field(default=None, description='HREF', title='Href')
-    isDeleted: bool = Field(..., description='HREF', title='Isdeleted')
     uniqueId: Optional[str] = Field(
         default=None, description='The Unique Identifier.', title='Uniqueid'
     )
     originId: Optional[str] = Field(
         default=None,
         description='The identifier of the asset from the origin system.',
         title='Originid',
     )
     description: Optional[str] = Field(
         default=None, description='Asset description', title='Description'
     )
     tags: Optional[List[TagSchema]] = Field(
         default=None, description='Expanded Tags', title='Tags'
     )
+    incidentsCount: Optional[int] = Field(
+        default=None,
+        description='Number of associated incidents',
+        title='Incidentscount',
+    )
 
 
 class CampaignPermissionDecisionFilter(BaseModel):
     class Config:
         extra = Extra.forbid
 
     field_in: Optional[List[Selection]] = Field(
@@ -801,37 +786,41 @@
     data: List[CampaignSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
 
 
 class RawIdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    object: Object2 = Field(
-        ..., description='Type of entity (here `identity`)', title='Object'
-    )
     name: Optional[str] = Field(
         default=None, description='Name of Identity', title='Name'
     )
     title: Optional[str] = Field(default=None, description='Title', title='Title')
     department: Optional[str] = Field(
         default=None, description='Department', title='Department'
     )
-    tagIds: Optional[List[str]] = Field(
-        default=[], description='List of tags', title='Tagids'
-    )
     accountIds: Optional[List[str]] = Field(
         default=[], description='List of associated account IDs', title='Accountids'
     )
-    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
     email: Optional[str] = Field(
         default=None, description="User's work email address.\n", title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
         default=None, description='Expanded Tags', title='Tags'
     )
+    terminatedAt: Optional[str] = Field(
+        default=None, description='Time of termination', title='Terminatedat'
+    )
+    hiredAt: Optional[str] = Field(
+        default=None, description='Hired At', title='Hiredat'
+    )
+    incidentsCount: Optional[int] = Field(
+        default=None,
+        description='Number of associated incidents',
+        title='Incidentscount',
+    )
 
 
 class ReviewerSchema(BaseModel):
     userId: str = Field(..., description='User ID of the Reviewer', title='Userid')
     campaignId: str = Field(..., description='Campaign ID', title='Campaignid')
     lastNotifiedAt: datetime = Field(
         ..., description='Time of last notified', title='Lastnotifiedat'
@@ -970,40 +959,33 @@
         title='Originid',
     )
     uniqueId: Optional[str] = Field(
         default=None,
         description='Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.',
         title='Uniqueid',
     )
-    object: Object = Field(
-        ..., description='type of object (here `account`)', title='Object'
-    )
     name: Optional[str] = Field(default=None, description='Name', title='Name')
     type: str = Field(..., description='Type', title='Type')
     isExternal: bool = Field(..., description='Is External', title='Isexternal')
     email: Optional[str] = Field(default=None, description='Email', title='Email')
-    tagIds: Optional[List[str]] = Field(
-        default=[], description='Tag IDs', title='Tagids'
-    )
     identityId: Optional[str] = Field(
         default=None, description='Associated Identity ID ', title='Identityid'
     )
     identity: Optional[RawIdentitySchema] = Field(
         default=None, description='Associated Identity', title='Identity'
     )
-    sourceAppId: Optional[str] = Field(
-        default=None, description='Source App ID', title='Sourceappid'
-    )
     sourceApp: Optional[SourceAppSchema] = Field(
         default=None, description='Source App', title='Sourceapp'
     )
     isAdmin: Optional[bool] = Field(
         default=None, description='Is Admin', title='Isadmin'
     )
-    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
+    tags: Optional[List[TagSchema]] = Field(
+        default=None, description='Expanded Tags', title='Tags'
+    )
 
 
 class CampaignsPermissionSchema(BaseModel):
     id: str = Field(..., description='Campaign ID (unique). \n', title='Id')
     campaignId: str = Field(
         ..., description='ID of the Campaign.\n', title='Campaignid'
     )
@@ -1041,37 +1023,41 @@
         description='Reviewer decision for keeping or revoking the reviewed access.  \n',
         title='Decisionreason',
     )
 
 
 class IdentitySchema(BaseModel):
     authomizeId: str = Field(..., description='Unique ID', title='Authomizeid')
-    object: Object2 = Field(
-        ..., description='Type of entity (here `identity`)', title='Object'
-    )
     name: Optional[str] = Field(
         default=None, description='Name of Identity', title='Name'
     )
     title: Optional[str] = Field(default=None, description='Title', title='Title')
     department: Optional[str] = Field(
         default=None, description='Department', title='Department'
     )
-    tagIds: Optional[List[str]] = Field(
-        default=[], description='List of tags', title='Tagids'
-    )
     accountIds: Optional[List[str]] = Field(
         default=[], description='List of associated account IDs', title='Accountids'
     )
-    isDeleted: bool = Field(..., description='Is Deleted', title='Isdeleted')
     email: Optional[str] = Field(
         default=None, description="User's work email address.\n", title='Email'
     )
     tags: Optional[List[TagSchema]] = Field(
         default=None, description='Expanded Tags', title='Tags'
     )
+    terminatedAt: Optional[str] = Field(
+        default=None, description='Time of termination', title='Terminatedat'
+    )
+    hiredAt: Optional[str] = Field(
+        default=None, description='Hired At', title='Hiredat'
+    )
+    incidentsCount: Optional[int] = Field(
+        default=None,
+        description='Number of associated incidents',
+        title='Incidentscount',
+    )
     accounts: Optional[List[AccountSchema]] = Field(
         default=[], description='List of associated accounts', title='Accounts'
     )
 
 
 class IncidentSchema(BaseModel):
     id: str = Field(..., description='Unique id', title='Id')
```

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.3/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874357558296987%*

 * *Differences: {"'components'": "{'schemas': {'AccountSchema': {'required': {delete: [4, 1]}, 'properties': "*

 * *                 "{'tags': OrderedDict([('title', 'Tags'), ('type', 'array'), ('items', "*

 * *                 "OrderedDict([('$ref', '#/components/schemas/TagSchema')])), ('description', "*

 * *                 "'Expanded Tags')]), delete: ['object', 'tagIds', 'sourceAppId', 'isDeleted']}}, "*

 * *                 "'AssetSchema': {'required': {delete: [4, 1]}, 'properties': {'lastUsedAt': "*

 * *                 "{delete: ['format' […]*

```diff
@@ -46,63 +46,44 @@
                         "type": "string"
                     },
                     "isAdmin": {
                         "description": "Is Admin",
                         "title": "Isadmin",
                         "type": "boolean"
                     },
-                    "isDeleted": {
-                        "description": "Is Deleted",
-                        "title": "Isdeleted",
-                        "type": "boolean"
-                    },
                     "isExternal": {
                         "description": "Is External",
                         "title": "Isexternal",
                         "type": "boolean"
                     },
                     "name": {
                         "description": "Name",
                         "title": "Name",
                         "type": "string"
                     },
-                    "object": {
-                        "description": "type of object (here `account`)",
-                        "enum": [
-                            "account"
-                        ],
-                        "title": "Object",
-                        "type": "string"
-                    },
                     "originId": {
                         "description": "The identifier of the account from the origin system.",
                         "title": "Originid",
                         "type": "string"
                     },
                     "sourceApp": {
                         "allOf": [
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "Source App",
                         "title": "Sourceapp"
                     },
-                    "sourceAppId": {
-                        "description": "Source App ID",
-                        "title": "Sourceappid",
-                        "type": "string"
-                    },
-                    "tagIds": {
-                        "default": [],
-                        "description": "Tag IDs",
+                    "tags": {
+                        "description": "Expanded Tags",
                         "items": {
-                            "type": "string"
+                            "$ref": "#/components/schemas/TagSchema"
                         },
-                        "title": "Tagids",
+                        "title": "Tags",
                         "type": "array"
                     },
                     "type": {
                         "description": "Type",
                         "title": "Type",
                         "type": "string"
                     },
@@ -110,18 +91,16 @@
                         "description": "Unique ID is an identifier coming from the connector that is guaranteed to be unique across all accounts coming from that connector.",
                         "title": "Uniqueid",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId",
-                    "object",
                     "type",
-                    "isExternal",
-                    "isDeleted"
+                    "isExternal"
                 ],
                 "title": "AccountSchema",
                 "type": "object"
             },
             "AddIncidentCommentRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
@@ -265,38 +244,29 @@
                         "type": "string"
                     },
                     "href": {
                         "description": "HREF",
                         "title": "Href",
                         "type": "string"
                     },
-                    "isDeleted": {
-                        "description": "HREF",
-                        "title": "Isdeleted",
-                        "type": "boolean"
+                    "incidentsCount": {
+                        "description": "Number of associated incidents",
+                        "title": "Incidentscount",
+                        "type": "integer"
                     },
                     "lastUsedAt": {
                         "description": "The date (in ISO 8601 format) of the last time that the asset was in use.",
-                        "format": "date-time",
                         "title": "Lastusedat",
                         "type": "string"
                     },
                     "name": {
                         "description": "Name",
                         "title": "Name",
                         "type": "string"
                     },
-                    "object": {
-                        "description": "Type of entity (here `asset`)",
-                        "enum": [
-                            "asset"
-                        ],
-                        "title": "Object",
-                        "type": "string"
-                    },
                     "originId": {
                         "description": "The identifier of the asset from the origin system.",
                         "title": "Originid",
                         "type": "string"
                     },
                     "originType": {
                         "description": "The asset type in the source system. The default is the canonical type (if not mentioned).\n",
@@ -308,28 +278,14 @@
                             {
                                 "$ref": "#/components/schemas/SourceAppSchema"
                             }
                         ],
                         "description": "Source App",
                         "title": "Sourceapp"
                     },
-                    "sourceAppId": {
-                        "description": "Source App ID",
-                        "title": "Sourceappid",
-                        "type": "string"
-                    },
-                    "tagIds": {
-                        "default": [],
-                        "description": "Tag IDs",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "Tagids",
-                        "type": "array"
-                    },
                     "tags": {
                         "description": "Expanded Tags",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
@@ -343,18 +299,16 @@
                         "description": "The Unique Identifier.",
                         "title": "Uniqueid",
                         "type": "string"
                     }
                 },
                 "required": [
                     "authomizeId",
-                    "object",
                     "name",
-                    "type",
-                    "isDeleted"
+                    "type"
                 ],
                 "title": "AssetSchema",
                 "type": "object"
             },
             "AttackTacticType": {
                 "description": "An enumeration.",
                 "enum": [
@@ -940,59 +894,50 @@
                         "type": "string"
                     },
                     "email": {
                         "description": "User's work email address.\n",
                         "title": "Email",
                         "type": "string"
                     },
-                    "isDeleted": {
-                        "description": "Is Deleted",
-                        "title": "Isdeleted",
-                        "type": "boolean"
+                    "hiredAt": {
+                        "description": "Hired At",
+                        "title": "Hiredat",
+                        "type": "string"
+                    },
+                    "incidentsCount": {
+                        "description": "Number of associated incidents",
+                        "title": "Incidentscount",
+                        "type": "integer"
                     },
                     "name": {
                         "description": "Name of Identity",
                         "title": "Name",
                         "type": "string"
                     },
-                    "object": {
-                        "description": "Type of entity (here `identity`)",
-                        "enum": [
-                            "identity"
-                        ],
-                        "title": "Object",
-                        "type": "string"
-                    },
-                    "tagIds": {
-                        "default": [],
-                        "description": "List of tags",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "Tagids",
-                        "type": "array"
-                    },
                     "tags": {
                         "description": "Expanded Tags",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
+                    "terminatedAt": {
+                        "description": "Time of termination",
+                        "title": "Terminatedat",
+                        "type": "string"
+                    },
                     "title": {
                         "description": "Title",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
-                    "authomizeId",
-                    "object",
-                    "isDeleted"
+                    "authomizeId"
                 ],
                 "title": "IdentitySchema",
                 "type": "object"
             },
             "IncidentEntitiesSchema": {
                 "properties": {
                     "email": {
@@ -1427,15 +1372,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.1.0",
+                        "default": "4.1.2",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -1768,59 +1713,50 @@
                         "type": "string"
                     },
                     "email": {
                         "description": "User's work email address.\n",
                         "title": "Email",
                         "type": "string"
                     },
-                    "isDeleted": {
-                        "description": "Is Deleted",
-                        "title": "Isdeleted",
-                        "type": "boolean"
+                    "hiredAt": {
+                        "description": "Hired At",
+                        "title": "Hiredat",
+                        "type": "string"
+                    },
+                    "incidentsCount": {
+                        "description": "Number of associated incidents",
+                        "title": "Incidentscount",
+                        "type": "integer"
                     },
                     "name": {
                         "description": "Name of Identity",
                         "title": "Name",
                         "type": "string"
                     },
-                    "object": {
-                        "description": "Type of entity (here `identity`)",
-                        "enum": [
-                            "identity"
-                        ],
-                        "title": "Object",
-                        "type": "string"
-                    },
-                    "tagIds": {
-                        "default": [],
-                        "description": "List of tags",
-                        "items": {
-                            "type": "string"
-                        },
-                        "title": "Tagids",
-                        "type": "array"
-                    },
                     "tags": {
                         "description": "Expanded Tags",
                         "items": {
                             "$ref": "#/components/schemas/TagSchema"
                         },
                         "title": "Tags",
                         "type": "array"
                     },
+                    "terminatedAt": {
+                        "description": "Time of termination",
+                        "title": "Terminatedat",
+                        "type": "string"
+                    },
                     "title": {
                         "description": "Title",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
-                    "authomizeId",
-                    "object",
-                    "isDeleted"
+                    "authomizeId"
                 ],
                 "title": "RawIdentitySchema",
                 "type": "object"
             },
             "ReviewStatus": {
                 "description": "An enumeration.",
                 "enum": [
@@ -2387,25 +2323,25 @@
                 ],
                 "title": "SourceAppSchema",
                 "type": "object"
             },
             "TagSchema": {
                 "properties": {
                     "description": {
-                        "description": "Description",
+                        "description": "Description of the tag",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
-                        "description": "Id",
+                        "description": "Authomize ID for the Tag",
                         "title": "Id",
                         "type": "string"
                     },
                     "name": {
-                        "description": "Name",
+                        "description": "Name of the tag",
                         "title": "Name",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "name",
@@ -2525,15 +2461,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.0",
+        "version": "4.1.2",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-4.1.2/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.3/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.2/setup.py` & `authomize-rest-api-client-4.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.2',
+        version='4.1.3',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

