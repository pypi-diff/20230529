# Comparing `tmp/cucumber_test_release_automation-0.0.8.tar.gz` & `tmp/cucumber_test_release_automation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cucumber_test_release_automation-0.0.8.tar", max compression
+gzip compressed data, was "cucumber_test_release_automation-0.0.9.tar", max compression
```

## Comparing `cucumber_test_release_automation-0.0.8.tar` & `cucumber_test_release_automation-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2022-12-01 20:55:14.687998 cucumber_test_release_automation-0.0.8/README.md
--rw-r--r--   0        0        0        0 2022-12-01 20:55:14.687998 cucumber_test_release_automation-0.0.8/cucumber_test_release_automation/__init__.py
--rw-r--r--   0        0        0      347 2022-12-01 20:55:37.892230 cucumber_test_release_automation-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 cucumber_test_release_automation-0.0.8/setup.py
--rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 cucumber_test_release_automation-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-01 20:56:34.962104 cucumber_test_release_automation-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-12-01 20:56:34.962104 cucumber_test_release_automation-0.0.9/cucumber_test_release_automation/__init__.py
+-rw-r--r--   0        0        0      347 2022-12-01 20:57:06.270404 cucumber_test_release_automation-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 cucumber_test_release_automation-0.0.9/setup.py
+-rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 cucumber_test_release_automation-0.0.9/PKG-INFO
```

### Comparing `cucumber_test_release_automation-0.0.8/setup.py` & `cucumber_test_release_automation-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['cucumber_test_release_automation']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'cucumber-test-release-automation',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': '',
     'author': 'Matt Wynne',
     'author_email': 'matt@cucumber.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

