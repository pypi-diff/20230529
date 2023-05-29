# Comparing `tmp/ProjectB_clientside_template_package-0.1.tar.gz` & `tmp/ProjectB_clientside_template_package-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectB_clientside_template_package-0.1.tar", last modified: Sun May 28 12:31:09 2023, max compression
+gzip compressed data, was "ProjectB_clientside_template_package-0.2.tar", last modified: Mon May 29 03:56:24 2023, max compression
```

## Comparing `ProjectB_clientside_template_package-0.1.tar` & `ProjectB_clientside_template_package-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 patrickfung   (501) wheel        (0)        0 2023-05-28 12:31:09.816918 ProjectB_clientside_template_package-0.1/
--rw-r--r--   0 patrickfung   (501) wheel        (0)      514 2023-05-28 12:31:09.816364 ProjectB_clientside_template_package-0.1/PKG-INFO
-drwxr-xr-x   0 patrickfung   (501) wheel        (0)        0 2023-05-28 12:31:09.815716 ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/
--rw-r--r--   0 patrickfung   (501) wheel        (0)      514 2023-05-28 12:31:09.000000 ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/PKG-INFO
--rw-r--r--   0 patrickfung   (501) wheel        (0)      248 2023-05-28 12:31:09.000000 ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/SOURCES.txt
--rw-r--r--   0 patrickfung   (501) wheel        (0)        1 2023-05-28 12:31:09.000000 ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/dependency_links.txt
--rw-r--r--   0 patrickfung   (501) wheel        (0)        1 2023-05-28 12:31:09.000000 ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/top_level.txt
--rw-r--r--   0 patrickfung   (501) wheel        (0)       38 2023-05-28 12:31:09.817052 ProjectB_clientside_template_package-0.1/setup.cfg
--rw-r--r--   0 patrickfung   (501) wheel        (0)      712 2023-05-28 12:28:22.000000 ProjectB_clientside_template_package-0.1/setup.py
+drwxr-xr-x   0 patrickfung   (501) wheel        (0)        0 2023-05-29 03:56:24.803792 ProjectB_clientside_template_package-0.2/
+-rw-r--r--   0 patrickfung   (501) wheel        (0)      514 2023-05-29 03:56:24.803500 ProjectB_clientside_template_package-0.2/PKG-INFO
+drwxr-xr-x   0 patrickfung   (501) wheel        (0)        0 2023-05-29 03:56:24.803110 ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/
+-rw-r--r--   0 patrickfung   (501) wheel        (0)      514 2023-05-29 03:56:24.000000 ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/PKG-INFO
+-rw-r--r--   0 patrickfung   (501) wheel        (0)      248 2023-05-29 03:56:24.000000 ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickfung   (501) wheel        (0)        1 2023-05-29 03:56:24.000000 ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickfung   (501) wheel        (0)        1 2023-05-29 03:56:24.000000 ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/top_level.txt
+-rw-r--r--   0 patrickfung   (501) wheel        (0)       38 2023-05-29 03:56:24.803877 ProjectB_clientside_template_package-0.2/setup.cfg
+-rw-r--r--   0 patrickfung   (501) wheel        (0)      781 2023-05-29 03:52:42.000000 ProjectB_clientside_template_package-0.2/setup.py
```

### Comparing `ProjectB_clientside_template_package-0.1/PKG-INFO` & `ProjectB_clientside_template_package-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjectB_clientside_template_package
-Version: 0.1
+Version: 0.2
 Summary: This is the pip package of ProjectB_clientside_template_package
 Home-page: https://github.com/ProjectBSource/ProjectB_clientside_JAVA_template/tree/change_TradeController_features_to_local
 Author: ProjectB
 Author-email: admin@projectb.click
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ProjectB_clientside_template_package-0.1/ProjectB_clientside_template_package.egg-info/PKG-INFO` & `ProjectB_clientside_template_package-0.2/ProjectB_clientside_template_package.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjectB-clientside-template-package
-Version: 0.1
+Version: 0.2
 Summary: This is the pip package of ProjectB_clientside_template_package
 Home-page: https://github.com/ProjectBSource/ProjectB_clientside_JAVA_template/tree/change_TradeController_features_to_local
 Author: ProjectB
 Author-email: admin@projectb.click
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ProjectB_clientside_template_package-0.1/setup.py` & `ProjectB_clientside_template_package-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import setuptools
 
 
 setuptools.setup(
      name='ProjectB_clientside_template_package',  
-     version='0.1',
+     version='0.2',
      #scripts=['ProjectB_clientside_template_package'] ,
      author="ProjectB",
      author_email="admin@projectb.click",
      description="This is the pip package of ProjectB_clientside_template_package",
      long_description_content_type="text/markdown",
      url="https://github.com/ProjectBSource/ProjectB_clientside_JAVA_template/tree/change_TradeController_features_to_local",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
- )
+ )
+
+#https://pypi.org/project/ProjectB-clientside-template-package/0.1/
```

