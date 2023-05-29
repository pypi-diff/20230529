# Comparing `tmp/lab-partner-utils-0.5.25.tar.gz` & `tmp/lab-partner-utils-0.7.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.5.25.tar", last modified: Sun Sep  4 17:19:30 2022, max compression
+gzip compressed data, was "lab-partner-utils-0.7.32.tar", last modified: Mon May 29 14:46:27 2023, max compression
```

## Comparing `lab-partner-utils-0.5.25.tar` & `lab-partner-utils-0.7.32.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:19:30.596118 lab-partner-utils-0.5.25/
--rw-rw-r--   0 root         (0) root         (0)     1094 2021-07-11 18:42:57.000000 lab-partner-utils-0.5.25/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      581 2022-09-04 17:19:30.596118 lab-partner-utils-0.5.25/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       65 2022-09-03 20:51:05.000000 lab-partner-utils-0.5.25/README.md
--rw-rw-r--   0 root         (0) root         (0)      103 2021-08-01 03:42:52.000000 lab-partner-utils-0.5.25/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      975 2022-09-04 17:19:30.596118 lab-partner-utils-0.5.25/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:19:30.592117 lab-partner-utils-0.5.25/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:19:30.592117 lab-partner-utils-0.5.25/src/lab_partner_utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-11-12 14:53:39.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     7963 2022-09-04 17:01:18.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/cli.py
--rw-rw-r--   0 root         (0) root         (0)     1706 2021-12-12 20:19:44.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/command_builder.py
--rwxrwxr-x   0 root         (0) root         (0)     7256 2022-09-04 16:18:47.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/commands.py
--rw-rw-r--   0 root         (0) root         (0)     1164 2022-01-29 20:18:56.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/kernel_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:19:30.596118 lab-partner-utils-0.5.25/src/lab_partner_utils/overrides/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-31 22:03:38.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/overrides/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      371 2022-09-04 16:57:14.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/overrides/build_image_override.py
--rw-rw-r--   0 root         (0) root         (0)      366 2022-09-03 23:50:43.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/overrides/run_image_override.py
--rw-rw-r--   0 root         (0) root         (0)      366 2022-09-03 23:50:43.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/overrides/start_kernel_override.py
--rw-rw-r--   0 root         (0) root         (0)     1182 2021-08-01 03:42:52.000000 lab-partner-utils-0.5.25/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:19:30.596118 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      581 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      738 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      123 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-09-04 17:19:30.000000 lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:27.656444 lab-partner-utils-0.7.32/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 14:46:27.652444 lab-partner-utils-0.7.32/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/README.md
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 14:46:21.000000 lab-partner-utils-0.7.32/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 14:46:27.656444 lab-partner-utils-0.7.32/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:27.648444 lab-partner-utils-0.7.32/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:27.652444 lab-partner-utils-0.7.32/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 14:45:51.000000 lab-partner-utils-0.7.32/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:27.652444 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 14:46:27.000000 lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/top_level.txt
```

### Comparing `lab-partner-utils-0.5.25/LICENSE.md` & `lab-partner-utils-0.7.32/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.5.25/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.32/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.5.25/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.32/src/lab_partner_utils/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         self.options.add(f'-e DISPLAY={display}')
         self.options.add('-e QT_X11_NO_MITSHM=1')
         self.options.add('-v /tmp/.X11-unix:/tmp/.X11-unix:ro')
         return self
 
     def with_shared_memory(self) -> 'DockerRunOptions':
         self.options.add(f'--ipc=host')
-        self.options.add('--ulimit "memlock=-1:-1"')
-        self.options.add('--ulimit "stack=-1:-1"')
+        self.options.add('--ulimit memlock=-1:-1')
+        self.options.add('--ulimit stack=-1:-1')
         self.with_add_devices()
         return self
 
     def build(self):
         return ' '.join(self.options)
```

### Comparing `lab-partner-utils-0.5.25/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.32/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.5.25/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.32/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 LICENSE.md
 README.md
 pyproject.toml
-setup.cfg
+run.sh
 src/lab_partner_utils/__init__.py
-src/lab_partner_utils/cli.py
+src/lab_partner_utils/cli_command_factory.py
 src/lab_partner_utils/command_builder.py
 src/lab_partner_utils/commands.py
 src/lab_partner_utils/kernel_launcher.py
 src/lab_partner_utils/utils.py
 src/lab_partner_utils.egg-info/PKG-INFO
 src/lab_partner_utils.egg-info/SOURCES.txt
 src/lab_partner_utils.egg-info/dependency_links.txt
 src/lab_partner_utils.egg-info/entry_points.txt
 src/lab_partner_utils.egg-info/requires.txt
-src/lab_partner_utils.egg-info/top_level.txt
-src/lab_partner_utils/overrides/__init__.py
-src/lab_partner_utils/overrides/build_image_override.py
-src/lab_partner_utils/overrides/run_image_override.py
-src/lab_partner_utils/overrides/start_kernel_override.py
+src/lab_partner_utils.egg-info/top_level.txt
```

