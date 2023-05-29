# Comparing `tmp/rosecape_airflow-0.0.3.tar.gz` & `tmp/rosecape_airflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosecape_airflow-0.0.3.tar", last modified: Mon May 29 15:30:11 2023, max compression
+gzip compressed data, was "rosecape_airflow-0.0.4.tar", last modified: Mon May 29 15:37:44 2023, max compression
```

## Comparing `rosecape_airflow-0.0.3.tar` & `rosecape_airflow-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:30:11.216340 rosecape_airflow-0.0.3/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 15:30:11.216201 rosecape_airflow-0.0.3/PKG-INFO
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:30:11.214553 rosecape_airflow-0.0.3/rosecape_airflow/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.3/rosecape_airflow/__init__.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:30:11.215809 rosecape_airflow-0.0.3/rosecape_airflow/aws/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.3/rosecape_airflow/aws/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.3/rosecape_airflow/aws/ec2.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.3/rosecape_airflow/aws/ecs.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)    10081 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.3/rosecape_airflow/aws/efs.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:30:11.216026 rosecape_airflow-0.0.3/rosecape_airflow/slack/
--rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.3/rosecape_airflow/slack/__init__.py
--rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.3/rosecape_airflow/slack/task_failed_slack_alert.py
-drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:30:11.215331 rosecape_airflow-0.0.3/rosecape_airflow.egg-info/
--rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 15:30:11.000000 rosecape_airflow-0.0.3/rosecape_airflow.egg-info/PKG-INFO
--rw-r--r--   0 nickjoanis   (501) staff       (20)      399 2023-05-29 15:30:11.000000 rosecape_airflow-0.0.3/rosecape_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-05-29 15:30:11.000000 rosecape_airflow-0.0.3/rosecape_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-05-29 15:30:11.000000 rosecape_airflow-0.0.3/rosecape_airflow.egg-info/top_level.txt
--rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-05-29 15:30:11.216386 rosecape_airflow-0.0.3/setup.cfg
--rw-r--r--   0 nickjoanis   (501) staff       (20)      712 2023-05-29 15:30:07.000000 rosecape_airflow-0.0.3/setup.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:37:44.878390 rosecape_airflow-0.0.4/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 15:37:44.878269 rosecape_airflow-0.0.4/PKG-INFO
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:37:44.876698 rosecape_airflow-0.0.4/rosecape_airflow/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:02:59.000000 rosecape_airflow-0.0.4/rosecape_airflow/__init__.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:37:44.877827 rosecape_airflow-0.0.4/rosecape_airflow/aws/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:57.000000 rosecape_airflow-0.0.4/rosecape_airflow/aws/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1801 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.4/rosecape_airflow/aws/ec2.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     3941 2023-05-29 14:43:16.000000 rosecape_airflow-0.0.4/rosecape_airflow/aws/ecs.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)    10081 2023-05-29 03:03:35.000000 rosecape_airflow-0.0.4/rosecape_airflow/aws/efs.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:37:44.878090 rosecape_airflow-0.0.4/rosecape_airflow/slack/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        0 2023-05-29 03:03:52.000000 rosecape_airflow-0.0.4/rosecape_airflow/slack/__init__.py
+-rw-r--r--   0 nickjoanis   (501) staff       (20)     1507 2023-05-29 12:48:08.000000 rosecape_airflow-0.0.4/rosecape_airflow/slack/task_failed_slack_alert.py
+drwxr-xr-x   0 nickjoanis   (501) staff       (20)        0 2023-05-29 15:37:44.877258 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      492 2023-05-29 15:37:44.000000 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      438 2023-05-29 15:37:44.000000 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)        1 2023-05-29 15:37:44.000000 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       16 2023-05-29 15:37:44.000000 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/requires.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       17 2023-05-29 15:37:44.000000 rosecape_airflow-0.0.4/rosecape_airflow.egg-info/top_level.txt
+-rw-r--r--   0 nickjoanis   (501) staff       (20)       38 2023-05-29 15:37:44.878431 rosecape_airflow-0.0.4/setup.cfg
+-rw-r--r--   0 nickjoanis   (501) staff       (20)      743 2023-05-29 15:37:10.000000 rosecape_airflow-0.0.4/setup.py
```

### Comparing `rosecape_airflow-0.0.3/rosecape_airflow/aws/ec2.py` & `rosecape_airflow-0.0.4/rosecape_airflow/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.3/rosecape_airflow/aws/ecs.py` & `rosecape_airflow-0.0.4/rosecape_airflow/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.3/rosecape_airflow/aws/efs.py` & `rosecape_airflow-0.0.4/rosecape_airflow/aws/efs.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.3/rosecape_airflow/slack/task_failed_slack_alert.py` & `rosecape_airflow-0.0.4/rosecape_airflow/slack/task_failed_slack_alert.py`

 * *Files identical despite different names*

### Comparing `rosecape_airflow-0.0.3/setup.py` & `rosecape_airflow-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Airflow utilities'
 LONG_DESCRIPTION = 'A package that makes it easy to interact with AWS services from Airflow using PythonOperator'
 
 setup(
     name="rosecape_airflow",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author="Nick Joanis",
     author_email="nicholas@rosecape.ca",
     license='MIT',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        'boto3==1.26.142'
+    ],
     keywords='Airflow',
     classifiers= [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         'License :: OSI Approved :: MIT License',
         "Programming Language :: Python :: 3",
     ]
```

