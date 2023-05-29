# Comparing `tmp/pulumi_flux-0.25.3.tar.gz` & `tmp/pulumi_flux-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_flux-0.25.3.tar", last modified: Mon May 29 14:35:00 2023, max compression
+gzip compressed data, was "pulumi_flux-1.0.0.tar", last modified: Sun Sep 25 09:48:59 2022, max compression
```

## Comparing `pulumi_flux-0.25.3.tar` & `pulumi_flux-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:35:00.486286 pulumi_flux-0.25.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-29 14:35:00.486286 pulumi_flux-0.25.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:35:00.482285 pulumi_flux-0.25.3/pulumi_flux/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:35:00.486286 pulumi_flux-0.25.3/pulumi_flux/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    44401 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/flux_bootstrap_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/get_flux_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/get_flux_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:35:00.486286 pulumi_flux-0.25.3/pulumi_flux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/pulumi_flux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:35:00.486286 pulumi_flux-0.25.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-29 14:35:00.000000 pulumi_flux-0.25.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/pulumi_flux/
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11009 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/get_flux_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10645 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/get_flux_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/pulumi_flux/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/pulumi_flux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-25 09:48:59.000000 pulumi_flux-1.0.0/pulumi_flux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-25 09:48:59.123463 pulumi_flux-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-09-25 09:48:58.000000 pulumi_flux-1.0.0/setup.py
```

### Comparing `pulumi_flux-0.25.3/PKG-INFO` & `pulumi_flux-1.0.0/pulumi_flux.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
-Name: pulumi_flux
-Version: 0.25.3
-Summary: A Pulumi package for creating and managing Flux cloud resources.
+Name: pulumi-flux
+Version: 1.0.0
+Summary: A Pulumi package for creating and managing flux cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oun/pulumi-flux
 Keywords: pulumi flux category/cloud
 Platform: UNKNOWN
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Flux Pulumi Provider
+# Flux Resource Provider
 
-The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
-This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
+The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -59,10 +57,10 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
```

### Comparing `pulumi_flux-0.25.3/README.md` & `pulumi_flux-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,21 @@
-# Flux Pulumi Provider
+Metadata-Version: 2.1
+Name: pulumi_flux
+Version: 1.0.0
+Summary: A Pulumi package for creating and managing flux cloud resources.
+Home-page: https://www.pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/oun/pulumi-flux
+Keywords: pulumi flux category/cloud
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
 
-The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
-This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
+# Flux Resource Provider
+
+The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -47,8 +57,10 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
+
+
```

### Comparing `pulumi_flux-0.25.3/pulumi_flux/__init__.py` & `pulumi_flux-1.0.0/pulumi_flux/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,20 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
-from .flux_bootstrap_git import *
 from .get_flux_install import *
 from .get_flux_sync import *
 from .provider import *
-from ._inputs import *
-
-# Make subpackages available:
-if typing.TYPE_CHECKING:
-    import pulumi_flux.config as __config
-    config = __config
-else:
-    config = _utilities.lazy_import('pulumi_flux.config')
-
 _utilities.register(
     resource_modules="""
-[
- {
-  "pkg": "flux",
-  "mod": "index/fluxBootstrapGit",
-  "fqn": "pulumi_flux",
-  "classes": {
-   "flux:index/fluxBootstrapGit:FluxBootstrapGit": "FluxBootstrapGit"
-  }
- }
-]
+[]
 """,
     resource_packages="""
 [
  {
   "pkg": "flux",
   "token": "pulumi:providers:flux",
   "fqn": "pulumi_flux",
```

### Comparing `pulumi_flux-0.25.3/pulumi_flux/_utilities.py` & `pulumi_flux-1.0.0/pulumi_flux/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_flux-0.25.3/pulumi_flux.egg-info/PKG-INFO` & `pulumi_flux-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-Metadata-Version: 2.1
-Name: pulumi-flux
-Version: 0.25.3
-Summary: A Pulumi package for creating and managing Flux cloud resources.
-Home-page: https://www.pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/oun/pulumi-flux
-Keywords: pulumi flux category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# Flux Resource Provider
 
-# Flux Pulumi Provider
-
-The Flux Provider lets you manage [FluxCD](https://fluxcd.io) resources.
-This provider wraps the existing [Terraform Provider Flux](https://github.com/fluxcd/terraform-provider-flux).
+The Flux Resource Provider lets you manage [FluxCD](https://fluxcd.io) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
 
@@ -59,10 +46,8 @@
 
 ## Examples
 
 Find working Python code samples in the [`./examples`](https://github.com/oun/pulumi-flux/tree/main/examples) directory.
 
 ## Reference
 
-For detailed reference documentation, please visit the [the Pulumi registry](https://www.pulumi.com/registry/packages/flux/api-docs/).
-
-
+For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/foo/api-docs/).
```

### Comparing `pulumi_flux-0.25.3/setup.py` & `pulumi_flux-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.25.3"
-PLUGIN_VERSION = "0.25.3"
+VERSION = "1.0.0"
+PLUGIN_VERSION = "1.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'flux', PLUGIN_VERSION, '--server', 'github://api.github.com/oun'])
         except OSError as error:
@@ -34,17 +34,16 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "flux Pulumi Package - Development Version"
 
 
 setup(name='pulumi_flux',
-      python_requires='>=3.7',
       version=VERSION,
-      description="A Pulumi package for creating and managing Flux cloud resources.",
+      description="A Pulumi package for creating and managing flux cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi flux category/cloud',
       url='https://www.pulumi.com',
```

