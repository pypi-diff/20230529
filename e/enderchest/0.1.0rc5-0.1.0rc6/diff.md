# Comparing `tmp/enderchest-0.1.0rc5.tar.gz` & `tmp/enderchest-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc5.tar", last modified: Sun May 28 17:37:25 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc6.tar", last modified: Mon May 29 14:00:36 2023, max compression
```

## Comparing `enderchest-0.1.0rc5.tar` & `enderchest-0.1.0rc6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.504461 enderchest-0.1.0rc5/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 17:37:25.504461 enderchest-0.1.0rc5/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31170 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 17:37:25.000000 enderchest-0.1.0rc5/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-28 17:37:25.500461 enderchest-0.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-28 17:37:17.000000 enderchest-0.1.0rc5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22451 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/versioneer.py
```

### Comparing `enderchest-0.1.0rc5/LICENSE` & `enderchest-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/PKG-INFO` & `enderchest-0.1.0rc6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -131,12 +131,12 @@
 If you're interested in helping develop this project, have a look at the
 [repo backlog](https://github.com/OpenBagTwo/EnderChest/issues) and then read
 through the
 [contributor's guide](https://openbagtwo.github.io/EnderChest/dev/contrib).
 
 ## License
 
-This project--the executable, source code and all documentation are published
+This project--the executable, source code and all documentation--are published
 under the
 [GNU Public License v3](https://github.com/OpenBagTwo/EnderChest/blob/dev/LICENSE),
 and any contributions to or derivatives of this project _must_ be licensed under
 compatible terms.
```

### Comparing `enderchest-0.1.0rc5/README.md` & `enderchest-0.1.0rc6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,12 +119,12 @@
 If you're interested in helping develop this project, have a look at the
 [repo backlog](https://github.com/OpenBagTwo/EnderChest/issues) and then read
 through the
 [contributor's guide](https://openbagtwo.github.io/EnderChest/dev/contrib).
 
 ## License
 
-This project--the executable, source code and all documentation are published
+This project--the executable, source code and all documentation--are published
 under the
 [GNU Public License v3](https://github.com/OpenBagTwo/EnderChest/blob/dev/LICENSE),
 and any contributions to or derivatives of this project _must_ be licensed under
 compatible terms.
```

### Comparing `enderchest-0.1.0rc5/enderchest/cli.py` & `enderchest-0.1.0rc6/enderchest/cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/craft.py` & `enderchest-0.1.0rc6/enderchest/craft.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,16 +318,17 @@
             break
         try:
             remotes.extend(fetch_remotes_from_a_remote_ender_chest(remote_uri))
         except Exception as fetch_fail:
             CRAFT_LOGGER.error(
                 f"Could not fetch remotes from {remote_uri}\n  {fetch_fail}"
             )
-            if confirm(default=True):
-                break
+            if not confirm(default=True):
+                continue
+        break
 
     CRAFT_LOGGER.info(
         "\nYou can always add more remotes later using"
         "\n$ enderchest gather enderchest\n"
     )
 
     while True:
```

### Comparing `enderchest-0.1.0rc5/enderchest/enderchest.py` & `enderchest-0.1.0rc6/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/filesystem.py` & `enderchest-0.1.0rc6/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/gather.py` & `enderchest-0.1.0rc6/enderchest/gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/instance.py` & `enderchest-0.1.0rc6/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/loggers.py` & `enderchest-0.1.0rc6/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/place.py` & `enderchest-0.1.0rc6/enderchest/place.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     shulker_boxes: list[ShulkerBox] = []
 
     for shulker_box in load_shulker_boxes(minecraft_root, log_level=logging.DEBUG):
         if not shulker_box.matches_host(host):
             PLACE_LOGGER.debug(
                 f"{shulker_box.name} is not intended for linking to this host ({host})"
             )
-            break
+            continue
         else:
             shulker_boxes.append(shulker_box)
 
     skip_instances: list[InstanceSpec] = []
 
     def handle_error(instance: InstanceSpec) -> str:
         """Centralized error-handling
```

### Comparing `enderchest-0.1.0rc5/enderchest/prompt.py` & `enderchest-0.1.0rc6/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/remote.py` & `enderchest-0.1.0rc6/enderchest/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,9 +226,11 @@
                     SYNC_LOGGER.error("Aborting")
                     return
             else:
                 SYNC_LOGGER.debug(f"Waiting for {sync_confirm_wait} seconds")
                 sleep(sync_confirm_wait)
         else:
             synced_somewhere = True
+            if pull_or_push == "pull":
+                break
     if not synced_somewhere:
         SYNC_LOGGER.error("Could not sync with any remote EnderChests")
```

### Comparing `enderchest-0.1.0rc5/enderchest/shulker_box.py` & `enderchest-0.1.0rc6/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/sync/__init__.py` & `enderchest-0.1.0rc6/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/sync/file.py` & `enderchest-0.1.0rc6/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/sync/rsync.py` & `enderchest-0.1.0rc6/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/conftest.py` & `enderchest-0.1.0rc6/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_cli.py` & `enderchest-0.1.0rc6/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_craft.py` & `enderchest-0.1.0rc6/enderchest/test/test_craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_gather.py` & `enderchest-0.1.0rc6/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_instance.py` & `enderchest-0.1.0rc6/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_place.py` & `enderchest-0.1.0rc6/enderchest/test/test_place.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,17 +591,36 @@
         place.place_ender_chest(minecraft_root, error_handling="skip-instance")
 
         assert (
             minecraft_root / "instances" / "chest-boat" / ".minecraft" / "options.txt"
         ).read_text() == "autoJump:true"
         assert not (home / ".minecraft" / "data" / "achievements.txt").exists()
 
-    def test_skip_shulker(self, home, minecraft_root):
+    def test_skip_shulker_box(self, home, minecraft_root):
         place.place_ender_chest(minecraft_root, error_handling="skip-shulker")
 
         assert (
             home / ".minecraft" / "data" / "achievements.txt"
         ).read_text() == "Spelled acheivements correctly!"
 
         assert not (
             minecraft_root / "instances" / "chest-boat" / ".minecraft" / "options.txt"
         ).exists()
+
+    def test_skip_shulker_box_that_doesnt_match_host(self, home, minecraft_root):
+        with fs.shulker_box_config(minecraft_root, "1.19").open("a") as config_file:
+            config_file.write(
+                """
+[hosts]
+not-this-chest
+"""
+            )
+
+        place.place_ender_chest(minecraft_root)
+
+        assert not (
+            minecraft_root / "instances" / "chest-boat" / ".minecraft" / "options.txt"
+        ).exists()
+
+        assert (
+            home / ".minecraft" / "data" / "achievements.txt"
+        ).read_text() == "Spelled acheivements correctly!"
```

### Comparing `enderchest-0.1.0rc5/enderchest/test/test_sync.py` & `enderchest-0.1.0rc6/enderchest/test/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,13 +303,36 @@
     def test_close_deletes_remote_copies_when_locals_are_deleted(
         self, minecraft_root, remote
     ):
         gather.update_ender_chest(minecraft_root, remotes=(remote,))
         r.sync_with_remotes(minecraft_root, "push")
         assert not (path_from_uri(remote) / "EnderChest" / "optifine").exists()
 
+    def test_open_stops_at_first_successful_sync(self, minecraft_root, remote, caplog):
+        gather.update_ender_chest(
+            minecraft_root, remotes=(remote, "prayer://unreachable")
+        )
+        r.sync_with_remotes(minecraft_root, "pull")
+        warnings = [
+            record.msg for record in caplog.records if record.levelname == "WARNING"
+        ]
+
+        assert len(warnings) == 0
+
+    def test_close_will_attempt_to_push_to_all(self, minecraft_root, remote, caplog):
+        gather.update_ender_chest(
+            minecraft_root, remotes=(remote, "prayer://unreachable")
+        )
+        r.sync_with_remotes(minecraft_root, "push")
+        warnings = [
+            record.msg for record in caplog.records if record.levelname == "WARNING"
+        ]
+
+        assert len(warnings) == 1
+        assert "Could not sync changes with prayer://unreachable" in warnings[0]
+
 
 @pytest.mark.xfail(
     not shutil.which("rsync"), reason="rsync is not installed on this system"
 )
 class TestRsyncSync(TestFileSync):
     protocol = "rsync"
```

### Comparing `enderchest-0.1.0rc5/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest/test/utils.py` & `enderchest-0.1.0rc6/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -131,12 +131,12 @@
 If you're interested in helping develop this project, have a look at the
 [repo backlog](https://github.com/OpenBagTwo/EnderChest/issues) and then read
 through the
 [contributor's guide](https://openbagtwo.github.io/EnderChest/dev/contrib).
 
 ## License
 
-This project--the executable, source code and all documentation are published
+This project--the executable, source code and all documentation--are published
 under the
 [GNU Public License v3](https://github.com/OpenBagTwo/EnderChest/blob/dev/LICENSE),
 and any contributions to or derivatives of this project _must_ be licensed under
 compatible terms.
```

### Comparing `enderchest-0.1.0rc5/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/setup.py` & `enderchest-0.1.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc5/versioneer.py` & `enderchest-0.1.0rc6/versioneer.py`

 * *Files identical despite different names*

