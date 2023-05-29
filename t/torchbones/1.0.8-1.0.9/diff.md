# Comparing `tmp/torchbones-1.0.8.tar.gz` & `tmp/torchbones-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.0.8.tar", last modified: Mon May 29 18:17:41 2023, max compression
+gzip compressed data, was "torchbones-1.0.9.tar", last modified: Mon May 29 18:19:30 2023, max compression
```

## Comparing `torchbones-1.0.8.tar` & `torchbones-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:17:41.019489 torchbones-1.0.8/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:17:41.019489 torchbones-1.0.8/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-29 18:17:41.019489 torchbones-1.0.8/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-29 18:17:14.000000 torchbones-1.0.8/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:17:41.019489 torchbones-1.0.8/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.8/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16128 2023-05-29 18:14:23.000000 torchbones-1.0.8/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:17:41.019489 torchbones-1.0.8/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:17:40.000000 torchbones-1.0.8/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-29 18:17:40.000000 torchbones-1.0.8/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-29 18:17:40.000000 torchbones-1.0.8/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-29 18:17:40.000000 torchbones-1.0.8/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-29 18:17:40.000000 torchbones-1.0.8/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:19:30.519493 torchbones-1.0.9/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-29 18:19:30.519493 torchbones-1.0.9/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-29 18:19:21.000000 torchbones-1.0.9/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.9/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16126 2023-05-29 18:19:14.000000 torchbones-1.0.9/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:19:30.519493 torchbones-1.0.9/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-29 18:19:30.000000 torchbones-1.0.9/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.0.8/torchbones/main.py` & `torchbones-1.0.9/torchbones/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         
         self.init_lr = self.lr
         self.lr_decay = kwargs.get('lr_decay', 1)
         self.lr_min = kwargs.get('lr_min', 1e-10)
         self.optimizer = optimizer(self.net.parameters(), lr = self.lr)
             
         self.trainerr, self.testerr, self.err, self.epoch, self.loc, self.save_file = [], [], 0, 0, 0, None #just inits
-        self.plot_ev, self.print_ev = 10, 10
+        self.plotev, self.printev = 10, 10
         
         self.saving = kwargs.get('saving', False)
         self.save_tar = kwargs.get('save_weights', False)
         
         if self.save_tar and not os.path.isdir(weight_path):
             os.makedirs(weight_path)
```

