# Comparing `tmp/linkplay-cli-0.0.1.tar.gz` & `tmp/linkplay-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkplay-cli-0.0.1.tar", last modified: Sun May 28 21:28:59 2023, max compression
+gzip compressed data, was "linkplay-cli-0.0.2.tar", last modified: Mon May 29 19:51:08 2023, max compression
```

## Comparing `linkplay-cli-0.0.1.tar` & `linkplay-cli-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:28:59.393378 linkplay-cli-0.0.1/
--rw-rw-rw-   0        0        0     1211 2023-05-26 14:29:31.000000 linkplay-cli-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1161 2023-05-28 21:28:59.392379 linkplay-cli-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      804 2023-05-28 21:18:52.000000 linkplay-cli-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:28:59.388382 linkplay-cli-0.0.1/linkplay_cli.egg-info/
--rw-rw-rw-   0        0        0     1161 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:28:59.000000 linkplay-cli-0.0.1/linkplay_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:28:59.394379 linkplay-cli-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-05-28 13:14:08.000000 linkplay-cli-0.0.1/setup.py
+drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/
+-rw-rw-r--   0 rami      (1000) rami      (1000)     1211 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/LICENSE
+-rw-rw-r--   0 rami      (1000) rami      (1000)     1086 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/PKG-INFO
+-rw-rw-r--   0 rami      (1000) rami      (1000)      804 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/README.md
+drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/linkplay_cli/
+-rw-rw-r--   0 rami      (1000) rami      (1000)        1 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/linkplay_cli/__init__.py
+-rw-rw-r--   0 rami      (1000) rami      (1000)    10556 2023-05-29 19:49:07.000000 linkplay-cli-0.0.2/linkplay_cli/cli.py
+drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/linkplay_cli.egg-info/
+-rw-rw-r--   0 rami      (1000) rami      (1000)     1086 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 rami      (1000) rami      (1000)      289 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 rami      (1000) rami      (1000)        1 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 rami      (1000) rami      (1000)       55 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 rami      (1000) rami      (1000)       27 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/requires.txt
+-rw-rw-r--   0 rami      (1000) rami      (1000)       13 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/top_level.txt
+-rw-rw-r--   0 rami      (1000) rami      (1000)       38 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/setup.cfg
+-rw-rw-r--   0 rami      (1000) rami      (1000)      787 2023-05-29 19:50:51.000000 linkplay-cli-0.0.2/setup.py
```

### Comparing `linkplay-cli-0.0.1/LICENSE` & `linkplay-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.1/PKG-INFO` & `linkplay-cli-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.1
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
-
-
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.2
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
```

### Comparing `linkplay-cli-0.0.1/README.md` & `linkplay-cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.1/linkplay_cli.egg-info/PKG-INFO` & `linkplay-cli-0.0.2/linkplay_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.1
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
-
-
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.2
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
```

### Comparing `linkplay-cli-0.0.1/setup.py` & `linkplay-cli-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = readme.read()
 
 setup(name='linkplay-cli',
       description='Control Linkplay devices from the comfort of your shell',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ramikg/linkplay-cli',
-      version='0.0.1',
+      version='0.0.2',
       packages=find_packages(),
       install_requires=[
           'async_upnp_client',
           'requests'
       ],
       entry_points={
           'console_scripts': [
```

