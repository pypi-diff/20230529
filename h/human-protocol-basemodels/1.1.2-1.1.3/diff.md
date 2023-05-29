# Comparing `tmp/human-protocol-basemodels-1.1.2.tar.gz` & `tmp/human-protocol-basemodels-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human-protocol-basemodels-1.1.2.tar", last modified: Wed Mar  1 15:02:53 2023, max compression
+gzip compressed data, was "human-protocol-basemodels-1.1.3.tar", last modified: Mon May 29 14:33:50 2023, max compression
```

## Comparing `human-protocol-basemodels-1.1.2.tar` & `human-protocol-basemodels-1.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.902413 human-protocol-basemodels-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-01 15:02:53.902413 human-protocol-basemodels-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.890413 human-protocol-basemodels-1.1.2/basemodels/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 15:02:51.000000 human-protocol-basemodels-1.1.2/basemodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.894413 human-protocol-basemodels-1.1.2/basemodels/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.898413 human-protocol-basemodels-1.1.2/basemodels/manifest/data/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/data/groundtruth.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/data/taskdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/manifest/restricted_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/basemodels/via.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.898413 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:02:53.000000 human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:02:53.902413 human-protocol-basemodels-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:02:53.898413 human-protocol-basemodels-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/test/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-01 15:00:31.000000 human-protocol-basemodels-1.1.2/test/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 14:33:47.000000 human-protocol-basemodels-1.1.3/basemodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/manifest/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/groundtruth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/taskdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/restricted_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/via.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/test_preprocess.py
```

### Comparing `human-protocol-basemodels-1.1.2/basemodels/manifest/data/groundtruth.py` & `human-protocol-basemodels-1.1.3/basemodels/manifest/data/groundtruth.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/basemodels/manifest/data/taskdata.py` & `human-protocol-basemodels-1.1.3/basemodels/manifest/data/taskdata.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/basemodels/manifest/manifest.py` & `human-protocol-basemodels-1.1.3/basemodels/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/basemodels/manifest/restricted_audience.py` & `human-protocol-basemodels-1.1.3/basemodels/manifest/restricted_audience.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
     min_difficulty: Optional[conint(ge=0, le=4, strict=True)]
     min_user_score: Optional[confloat(ge=0, le=1)]
     max_user_score: Optional[confloat(ge=0, le=1)]
 
     launch_group_id: Optional[conint(ge=0, strict=True)]
 
+    interests: Optional[List[conint(strict=True)]]
+
     def dict(self, **kwargs):
         kwargs["exclude_unset"] = True
         return super().dict(**kwargs)
 
     def json(self, **kwargs):
         kwargs["exclude_unset"] = True
         return super().json(**kwargs)
```

### Comparing `human-protocol-basemodels-1.1.2/basemodels/via.py` & `human-protocol-basemodels-1.1.3/basemodels/via.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/human_protocol_basemodels.egg-info/SOURCES.txt` & `human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/setup.py` & `human-protocol-basemodels-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.2/test/test_manifest.py` & `human-protocol-basemodels-1.1.3/test/test_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,14 +391,21 @@
         for data in [
             {"launch_group_id": "launch_group_id"},
             {"launch_group_id": -3},
             {"launch_group_id": 1.1},
         ]:
             assert_raises(data)
 
+        for data in [
+            {"interests": 1},
+            {"interests": {"mapped": 1}},
+            {"interests": ["as", "string"]},
+        ]:
+            assert_raises(data)
+
         data = {
             "lang": [
                 {"us": {"score": 0}},
                 {"es": {"score": 0.5}},
                 {"en-us": {"score": 1}},
             ],
             "country": [
@@ -423,14 +430,15 @@
                 {"3hcaptcha.com": {"score": 1}},
             ],
             "confidence": [{"minimum_client_confidence": {"score": 0.5}}],
             "min_difficulty": 2,
             "min_user_score": 0,
             "max_user_score": 0.3,
             "launch_group_id": 101,
+            "interests": [1, 2, 3, 4],
         }
 
         RestrictedAudience(**data)
 
     def test_realistic_multi_challenge_example(self):
         """validates a realistic multi_challenge manifest"""
         obj = {
```

### Comparing `human-protocol-basemodels-1.1.2/test/test_preprocess.py` & `human-protocol-basemodels-1.1.3/test/test_preprocess.py`

 * *Files identical despite different names*

