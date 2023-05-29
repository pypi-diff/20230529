# Comparing `tmp/torchbones-1.0.9.tar.gz` & `tmp/torchbones-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.0.9.tar", last modified: Mon May 29 18:19:30 2023, max compression
+gzip compressed data, was "torchbones-1.1.0.tar", last modified: Mon May 29 18:24:28 2023, max compression
```

## Comparing `torchbones-1.0.9.tar` & `torchbones-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:19:30.519493 torchbones-1.0.9/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-29 18:19:30.519493 torchbones-1.0.9/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-29 18:19:21.000000 torchbones-1.0.9/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.9/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16126 2023-05-29 18:19:14.000000 torchbones-1.0.9/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:24:28.109497 torchbones-1.1.0/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-29 18:24:28.109497 torchbones-1.1.0/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-29 18:24:06.000000 torchbones-1.1.0/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.0/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16101 2023-05-29 18:24:24.000000 torchbones-1.1.0/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.0.9/torchbones/main.py` & `torchbones-1.1.0/torchbones/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,11 +377,8 @@
         test, testtruth = data[split:], self.truth[split:]
         if type(self.cov)!=int:
             cov = torch.tensor(self.cov).double()
             traincov = cov[:split]
             testcov = cov[split:]
         else:
             traincov, testcov = 1, 1
-        return train, traintruth, traincov, test, testtruth, testcov
-
-            
-          
+        return train, traintruth, traincov, test, testtruth, testcov
```

