# Comparing `tmp/naapc-1.5.0.tar.gz` & `tmp/naapc-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naapc-1.5.0.tar", last modified: Sat Nov  5 04:17:59 2022, max compression
+gzip compressed data, was "naapc-1.6.0.tar", last modified: Mon May 29 13:35:58 2023, max compression
```

## Comparing `naapc-1.5.0.tar` & `naapc-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matthewbai   (501) staff       (20)        0 2022-11-05 04:17:59.560389 naapc-1.5.0/
--rw-r--r--   0 matthewbai   (501) staff       (20)     1067 2022-11-03 12:01:58.000000 naapc-1.5.0/LICENSE
--rw-r--r--   0 matthewbai   (501) staff       (20)     5964 2022-11-05 04:17:59.560246 naapc-1.5.0/PKG-INFO
--rw-r--r--   0 matthewbai   (501) staff       (20)     4209 2022-11-05 03:49:33.000000 naapc-1.5.0/README.md
--rw-r--r--   0 matthewbai   (501) staff       (20)     1000 2022-11-05 04:17:35.000000 naapc-1.5.0/pyproject.toml
--rw-r--r--   0 matthewbai   (501) staff       (20)       38 2022-11-05 04:17:59.560441 naapc-1.5.0/setup.cfg
-drwxr-xr-x   0 matthewbai   (501) staff       (20)        0 2022-11-05 04:17:59.557590 naapc-1.5.0/src/
-drwxr-xr-x   0 matthewbai   (501) staff       (20)        0 2022-11-05 04:17:59.558744 naapc-1.5.0/src/naapc/
--rw-r--r--   0 matthewbai   (501) staff       (20)      129 2022-11-05 04:17:35.000000 naapc-1.5.0/src/naapc/__init__.py
--rw-r--r--   0 matthewbai   (501) staff       (20)     5974 2022-11-05 04:14:08.000000 naapc-1.5.0/src/naapc/nconfig.py
--rw-r--r--   0 matthewbai   (501) staff       (20)     5211 2022-11-05 04:14:13.000000 naapc-1.5.0/src/naapc/ndict.py
-drwxr-xr-x   0 matthewbai   (501) staff       (20)        0 2022-11-05 04:17:59.559673 naapc-1.5.0/src/naapc.egg-info/
--rw-r--r--   0 matthewbai   (501) staff       (20)     5964 2022-11-05 04:17:59.000000 naapc-1.5.0/src/naapc.egg-info/PKG-INFO
--rw-r--r--   0 matthewbai   (501) staff       (20)      271 2022-11-05 04:17:59.000000 naapc-1.5.0/src/naapc.egg-info/SOURCES.txt
--rw-r--r--   0 matthewbai   (501) staff       (20)        1 2022-11-05 04:17:59.000000 naapc-1.5.0/src/naapc.egg-info/dependency_links.txt
--rw-r--r--   0 matthewbai   (501) staff       (20)        7 2022-11-05 04:17:59.000000 naapc-1.5.0/src/naapc.egg-info/requires.txt
--rw-r--r--   0 matthewbai   (501) staff       (20)        6 2022-11-05 04:17:59.000000 naapc-1.5.0/src/naapc.egg-info/top_level.txt
-drwxr-xr-x   0 matthewbai   (501) staff       (20)        0 2022-11-05 04:17:59.559845 naapc-1.5.0/test/
--rw-r--r--   0 matthewbai   (501) staff       (20)    16019 2022-11-05 04:14:44.000000 naapc-1.5.0/test/test.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.191321 naapc-1.6.0/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.6.0/LICENSE
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-29 13:35:58.190321 naapc-1.6.0/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.6.0/README.md
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-29 13:27:44.000000 naapc-1.6.0/pyproject.toml
+-rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-29 13:35:58.192320 naapc-1.6.0/setup.cfg
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:57.993888 naapc-1.6.0/src/
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.088390 naapc-1.6.0/src/naapc/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-29 13:27:44.000000 naapc-1.6.0/src/naapc/__init__.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.6.0/src/naapc/nconfig.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6661 2023-05-29 13:20:05.000000 naapc-1.6.0/src/naapc/ndict.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.163250 naapc-1.6.0/src/naapc.egg-info/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/requires.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/top_level.txt
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.175260 naapc-1.6.0/test/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.6.0/test/test.py
```

### Comparing `naapc-1.5.0/LICENSE` & `naapc-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `naapc-1.5.0/PKG-INFO` & `naapc-1.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: repository, https://github.com/eiphy/naapc
 Keywords: configuration,config,dictionary,nested,argument parsing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nested Automated Argument Parsing Configuration (NAAPC)
 [NAAPC](https://pypi.org/project/naapc/) contains two classes: NConfig and NDict.
 NDict provides method to easily manipulate nested dictionaries.
 NConfig is a subclass of NDict and can **automatically modify configurations according to CLI arguments**.
@@ -57,23 +57,23 @@
 train:
   pretrain: false
   loss_args:
     lr: 0.1
 ```
 The typical usage is as follows:
 ```python
-from naapc import NConfig
+from naapc import nconfig
 from argparse import parser
 
 parser.add_argument("-c", type=str, dest="config")
 args, extra_args = parser.parse_known_args(["-c", "test.yaml", "--task;task", "regression", "--train;loss_args;lr", "0.2", "--train;pretrain", "1", "--others", "other"])
 
 with open(args.config, "r") as f:
   raw = yaml.safe_load(f)
-config = NConfig(raw)
+config = nconfig(raw)
 extra_args = config.parse_update(parser, extra_args)
 ```
 The resulting configurations:
 ```yaml
 task:
   task: regression
 train:
@@ -97,40 +97,49 @@
   task;task:
     flag: --task
     choices: ["regression", "classification"]
   train;lr:
     flag: lr
 ```
 
-## NDict Usages
+## ndict Usages
 for a sample configuration test.yaml file:
 ```yaml
 task:
   task: classification
 train:
   loss_args:
     lr: 0.1
 ```
 and a sample list configuration test_list.yaml file:
 ```yaml
-
+l:
+- d:
+    task:
+      task: classification
+- d:
+    train:
+      loss_args:
+        lr: 0.1
 ```
 
 ```python
-from naapc import NDict
+from naapc import ndict
 
 with open("test.yaml", "r") as f:
   raw = yaml.safe_load(f)
-nd = NDict(raw, delimiter=";")
+nd = ndict(raw["d"], delimiter=";")
+nd1 = ndict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
+nd2 = ndict.from_list_of_dict(raw["l"]) # nd2 == nd1 == nd
 
-nd1 = NDict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
 "task;path" in nd                      # "task" in raw and "path" in raw["task"]
 del nd["task;path"]                    # del raw["task]["path]
 nd["task;path"] = "cwd"                # raw["task"]["path"] = Path(".").absolute()
 nd.flatten_dict                        # {"task;task": "classification", "train;loss_args;lr": 0.1}
+nd.flatten_dict_split                  # raw["l"]
 nd.paths                               # ["task", "task;task", "train", "train;loss_args", "train;loss_args;lr"]
 nd.get("task;seed", 1)                 # raw["task"].get("seed", 1)
 nd.raw_dict                            # raw
 nd.size                                # len(nd.flatten_dict)
 nd.update({"task;here": "there"})      # raw["task]["here] = "there
 nd.items()                             # raw.items()
 nd.keys()                              # raw.keys()
@@ -138,19 +147,25 @@
 len(nd)                                # len(raw)
 bool(nd)                               # len(nd) > 0
 nd1 == nd                              # nd1.flatten_dict == nd.flatten_dict
 nd1["task;path"] = "xcwd"
 nd1["task;extra"] = "ecwd"
 nd["train;epochs"] = 100
 nd.compare_dict(nd1)                   # {"task;path": ("cwd", "xcwd"), "task;extra": (None, ecwd), "train;epochs": (100, None)}
+nd.is_matched(
+        {
+            "task;path": "ecwd", 
+            "train;epochs": "!QUERY d[path] == d['train;minimum_epochs']"
+        }
+    )                                  # Test if this dictionary is what you want.
 ```
 
-## NConfig Usage
-NConfig only supports int, str, float, bool, and list of these types.
-The NConfig automatically checks data type when modifications are applied.
+## nconfig Usage
+nconfig only supports int, str, float, bool, and list of these types.
+The nconfig automatically checks data type when modifications are applied.
 Note that argument specification ("_ARGUMENT_SPECIFICATION") does not count as part of the configurations but will be saved when use save() method.
 The path specified as "_IGNORE_IN_CLI" will not be added to the parser.
 
 ```python
 config.save("path.yaml")               # Save configurations as a yaml file
 config.add_to_argparse(parser)         # Generate cli arguments for every configuration.
 config.parse_update(parser, args)      # Parse cli arguments and update corresponding configuration. Extra arguments will be returned.
@@ -173,9 +188,9 @@
 ```
 
 Other functionalities are the same to NDict.
 
 ## Typing
 Add a type
 ```python
-NestedOrDict = Union[NDict, dict]
+NestedOrDict = Union[ndict, dict]
 ```
```

### Comparing `naapc-1.5.0/README.md` & `naapc-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 train:
   pretrain: false
   loss_args:
     lr: 0.1
 ```
 The typical usage is as follows:
 ```python
-from naapc import NConfig
+from naapc import nconfig
 from argparse import parser
 
 parser.add_argument("-c", type=str, dest="config")
 args, extra_args = parser.parse_known_args(["-c", "test.yaml", "--task;task", "regression", "--train;loss_args;lr", "0.2", "--train;pretrain", "1", "--others", "other"])
 
 with open(args.config, "r") as f:
   raw = yaml.safe_load(f)
-config = NConfig(raw)
+config = nconfig(raw)
 extra_args = config.parse_update(parser, extra_args)
 ```
 The resulting configurations:
 ```yaml
 task:
   task: regression
 train:
@@ -61,40 +61,49 @@
   task;task:
     flag: --task
     choices: ["regression", "classification"]
   train;lr:
     flag: lr
 ```
 
-## NDict Usages
+## ndict Usages
 for a sample configuration test.yaml file:
 ```yaml
 task:
   task: classification
 train:
   loss_args:
     lr: 0.1
 ```
 and a sample list configuration test_list.yaml file:
 ```yaml
-
+l:
+- d:
+    task:
+      task: classification
+- d:
+    train:
+      loss_args:
+        lr: 0.1
 ```
 
 ```python
-from naapc import NDict
+from naapc import ndict
 
 with open("test.yaml", "r") as f:
   raw = yaml.safe_load(f)
-nd = NDict(raw, delimiter=";")
+nd = ndict(raw["d"], delimiter=";")
+nd1 = ndict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
+nd2 = ndict.from_list_of_dict(raw["l"]) # nd2 == nd1 == nd
 
-nd1 = NDict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
 "task;path" in nd                      # "task" in raw and "path" in raw["task"]
 del nd["task;path"]                    # del raw["task]["path]
 nd["task;path"] = "cwd"                # raw["task"]["path"] = Path(".").absolute()
 nd.flatten_dict                        # {"task;task": "classification", "train;loss_args;lr": 0.1}
+nd.flatten_dict_split                  # raw["l"]
 nd.paths                               # ["task", "task;task", "train", "train;loss_args", "train;loss_args;lr"]
 nd.get("task;seed", 1)                 # raw["task"].get("seed", 1)
 nd.raw_dict                            # raw
 nd.size                                # len(nd.flatten_dict)
 nd.update({"task;here": "there"})      # raw["task]["here] = "there
 nd.items()                             # raw.items()
 nd.keys()                              # raw.keys()
@@ -102,19 +111,25 @@
 len(nd)                                # len(raw)
 bool(nd)                               # len(nd) > 0
 nd1 == nd                              # nd1.flatten_dict == nd.flatten_dict
 nd1["task;path"] = "xcwd"
 nd1["task;extra"] = "ecwd"
 nd["train;epochs"] = 100
 nd.compare_dict(nd1)                   # {"task;path": ("cwd", "xcwd"), "task;extra": (None, ecwd), "train;epochs": (100, None)}
+nd.is_matched(
+        {
+            "task;path": "ecwd", 
+            "train;epochs": "!QUERY d[path] == d['train;minimum_epochs']"
+        }
+    )                                  # Test if this dictionary is what you want.
 ```
 
-## NConfig Usage
-NConfig only supports int, str, float, bool, and list of these types.
-The NConfig automatically checks data type when modifications are applied.
+## nconfig Usage
+nconfig only supports int, str, float, bool, and list of these types.
+The nconfig automatically checks data type when modifications are applied.
 Note that argument specification ("_ARGUMENT_SPECIFICATION") does not count as part of the configurations but will be saved when use save() method.
 The path specified as "_IGNORE_IN_CLI" will not be added to the parser.
 
 ```python
 config.save("path.yaml")               # Save configurations as a yaml file
 config.add_to_argparse(parser)         # Generate cli arguments for every configuration.
 config.parse_update(parser, args)      # Parse cli arguments and update corresponding configuration. Extra arguments will be returned.
@@ -137,9 +152,9 @@
 ```
 
 Other functionalities are the same to NDict.
 
 ## Typing
 Add a type
 ```python
-NestedOrDict = Union[NDict, dict]
+NestedOrDict = Union[ndict, dict]
 ```
```

### Comparing `naapc-1.5.0/pyproject.toml` & `naapc-1.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naapc"
-version = "1.5.0"
+version = "1.6.0"
 description = "Nested Automated Argument Parsing Configuration (NAAPC)."
 readme = "README.md"
 authors = [{name = "Bai Huanyu", email = "eiphnix@gmail.com"}]
 license = {file = "LICENSE"}
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["configuration", "config", "dictionary", "nested", "argument parsing"]
 dependencies = ["pyyaml"]
-requires-python = ">=3.7"
+requires-python = "==3.10.*"
 
 [project.urls]
 repository = "https://github.com/eiphy/naapc"
 
 [tool.bumpver]
-current_version = "1.5.0"
+current_version = "1.6.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `naapc-1.5.0/src/naapc/nconfig.py` & `naapc-1.6.0/src/naapc/nconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import argparse
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
 import yaml
 
-from .ndict import NDict, NestedOrDict
+from .ndict import ndict, NestedOrDict
 
 
 class CustomArgs:
     def __init__(
         self,
         flag: str = None,
         atype=None,
@@ -27,15 +29,15 @@
         self.default = default
         self.isbool = isbool
 
     def __repr__(self):
         return f"{self.flag} {self.path}"
 
 
-class NConfig(NDict):
+class nconfig(ndict):
     """Nested configuration based on NDict class.
     You are not supposed to modify the data outside this class!
     """
 
     _arg_key = "_ARGUMENT_SPECIFICATION"
     _ignore_key = "_IGNORE_IN_CLI"
     reserved_keys = [_arg_key, _ignore_key]
@@ -47,29 +49,29 @@
         # Configuration is supposed to be read-only. Therefore should not be modified in outside.
         config = deepcopy(config)
         if self._arg_key in config:
             self._arg_specification = config[self._arg_key]
             del config[self._arg_key]
         else:
             self._arg_specification = {}
-        super(NConfig, self).__init__(config, delimiter=delimiter)
+        super().__init__(config, delimiter=delimiter)
         self._check_types()
 
     @property
     def raw_dict(self):
         return deepcopy(self._d)
 
     @property
     def flatten_dict(self):
         return deepcopy(self._flatten_dict)
 
     @property
     def flatten_dict_split(self):
         return deepcopy(
-            [NDict.from_flatten_dict({p: v}).raw_dict for p, v in self.flatten_dict.items()]
+            [ndict.from_flatten_dict({p: v}).raw_dict for p, v in self.flatten_dict.items()]
         )
 
     @property
     def paths(self):
         return deepcopy(self._paths)
 
     def _get_custom_args(self) -> list[CustomArgs]:
@@ -139,15 +141,15 @@
             if v is not None:
                 self[carg.path] = bool(v) if carg.isbool else v
 
         return extra_args
 
     ### getters ###
     @property
-    def str_configs(self) -> "NConfig":
+    def str_configs(self) -> nconfig:
         """Return NConfig object with every value in string."""
         d = deepcopy(self)
         for path, v in self._flatten_dict.items():
             d[path] = str(v)
         return d
 
     ### miscs ###
@@ -180,8 +182,8 @@
                 v
             ), f"Unexpected config value type of {path} {type(v)} / {self.allowable_types}"
 
     ### magics ###
     def __setitem__(self, path: str, value: Union[str, int, float, bool]):
         """Same to NDict but do type checking."""
         self._check_type_v(value)
-        super(NConfig, self).__setitem__(path, value)
+        super(nconfig, self).__setitem__(path, value)
```

### Comparing `naapc-1.5.0/src/naapc.egg-info/PKG-INFO` & `naapc-1.6.0/src/naapc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: repository, https://github.com/eiphy/naapc
 Keywords: configuration,config,dictionary,nested,argument parsing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: ==3.10.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nested Automated Argument Parsing Configuration (NAAPC)
 [NAAPC](https://pypi.org/project/naapc/) contains two classes: NConfig and NDict.
 NDict provides method to easily manipulate nested dictionaries.
 NConfig is a subclass of NDict and can **automatically modify configurations according to CLI arguments**.
@@ -57,23 +57,23 @@
 train:
   pretrain: false
   loss_args:
     lr: 0.1
 ```
 The typical usage is as follows:
 ```python
-from naapc import NConfig
+from naapc import nconfig
 from argparse import parser
 
 parser.add_argument("-c", type=str, dest="config")
 args, extra_args = parser.parse_known_args(["-c", "test.yaml", "--task;task", "regression", "--train;loss_args;lr", "0.2", "--train;pretrain", "1", "--others", "other"])
 
 with open(args.config, "r") as f:
   raw = yaml.safe_load(f)
-config = NConfig(raw)
+config = nconfig(raw)
 extra_args = config.parse_update(parser, extra_args)
 ```
 The resulting configurations:
 ```yaml
 task:
   task: regression
 train:
@@ -97,40 +97,49 @@
   task;task:
     flag: --task
     choices: ["regression", "classification"]
   train;lr:
     flag: lr
 ```
 
-## NDict Usages
+## ndict Usages
 for a sample configuration test.yaml file:
 ```yaml
 task:
   task: classification
 train:
   loss_args:
     lr: 0.1
 ```
 and a sample list configuration test_list.yaml file:
 ```yaml
-
+l:
+- d:
+    task:
+      task: classification
+- d:
+    train:
+      loss_args:
+        lr: 0.1
 ```
 
 ```python
-from naapc import NDict
+from naapc import ndict
 
 with open("test.yaml", "r") as f:
   raw = yaml.safe_load(f)
-nd = NDict(raw, delimiter=";")
+nd = ndict(raw["d"], delimiter=";")
+nd1 = ndict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
+nd2 = ndict.from_list_of_dict(raw["l"]) # nd2 == nd1 == nd
 
-nd1 = NDict.from_flatten_dict(nd.flatten_dict) # nd1 == nd
 "task;path" in nd                      # "task" in raw and "path" in raw["task"]
 del nd["task;path"]                    # del raw["task]["path]
 nd["task;path"] = "cwd"                # raw["task"]["path"] = Path(".").absolute()
 nd.flatten_dict                        # {"task;task": "classification", "train;loss_args;lr": 0.1}
+nd.flatten_dict_split                  # raw["l"]
 nd.paths                               # ["task", "task;task", "train", "train;loss_args", "train;loss_args;lr"]
 nd.get("task;seed", 1)                 # raw["task"].get("seed", 1)
 nd.raw_dict                            # raw
 nd.size                                # len(nd.flatten_dict)
 nd.update({"task;here": "there"})      # raw["task]["here] = "there
 nd.items()                             # raw.items()
 nd.keys()                              # raw.keys()
@@ -138,19 +147,25 @@
 len(nd)                                # len(raw)
 bool(nd)                               # len(nd) > 0
 nd1 == nd                              # nd1.flatten_dict == nd.flatten_dict
 nd1["task;path"] = "xcwd"
 nd1["task;extra"] = "ecwd"
 nd["train;epochs"] = 100
 nd.compare_dict(nd1)                   # {"task;path": ("cwd", "xcwd"), "task;extra": (None, ecwd), "train;epochs": (100, None)}
+nd.is_matched(
+        {
+            "task;path": "ecwd", 
+            "train;epochs": "!QUERY d[path] == d['train;minimum_epochs']"
+        }
+    )                                  # Test if this dictionary is what you want.
 ```
 
-## NConfig Usage
-NConfig only supports int, str, float, bool, and list of these types.
-The NConfig automatically checks data type when modifications are applied.
+## nconfig Usage
+nconfig only supports int, str, float, bool, and list of these types.
+The nconfig automatically checks data type when modifications are applied.
 Note that argument specification ("_ARGUMENT_SPECIFICATION") does not count as part of the configurations but will be saved when use save() method.
 The path specified as "_IGNORE_IN_CLI" will not be added to the parser.
 
 ```python
 config.save("path.yaml")               # Save configurations as a yaml file
 config.add_to_argparse(parser)         # Generate cli arguments for every configuration.
 config.parse_update(parser, args)      # Parse cli arguments and update corresponding configuration. Extra arguments will be returned.
@@ -173,9 +188,9 @@
 ```
 
 Other functionalities are the same to NDict.
 
 ## Typing
 Add a type
 ```python
-NestedOrDict = Union[NDict, dict]
+NestedOrDict = Union[ndict, dict]
 ```
```

### Comparing `naapc-1.5.0/test/test.py` & `naapc-1.6.0/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from pathlib import Path
 from typing import Any
 
 import yaml
 
 sys.path.append(str(Path(__file__).parent.parent.absolute()))
 
-from naapc import NConfig, NDict
+from naapc import nconfig, ndict
 
 
 class testNDict:
     def __init__(self, delimiter=";"):
-        self.nd = NDict({"this": "is test"})
+        self.nd = ndict({"this": "is test"})
         print("Pass copy test.")
 
         with open("test/config.yaml", "r") as f:
             self.rawd = yaml.safe_load(f)
-        self.nd = NDict(self.rawd)
+        self.nd = ndict(self.rawd)
         self.test_init()
         print("Pass init test.")
 
         self.test_from_flatten_dict()
         print("Pass from flatten test.")
 
         self.test_paths()
@@ -53,55 +53,55 @@
         self.test_compare()
         print("Pass compare test.")
 
         self.test_delimiter()
         print("Pass delimiter test.")
 
     def test_init(self, delimiter=";"):
-        nd1 = NDict(self.nd, delimiter=delimiter)
+        nd1 = ndict(self.nd, delimiter=delimiter)
         assert nd1 == self.nd
         assert self.nd.raw_dict is not nd1.raw_dict
         assert self.nd is not nd1
 
-        nd1 = NDict(deepcopy(self.nd.raw_dict), delimiter=delimiter)
+        nd1 = ndict(deepcopy(self.nd.raw_dict), delimiter=delimiter)
         assert nd1 is not self.nd
         assert nd1 == self.nd
         del nd1[f"task{delimiter}task"]
         self.nd[f"task{delimiter}task"]
         assert nd1 != self.nd
 
     def test_from_flatten_dict(self, delimiter=";"):
-        nd1 = NDict.from_flatten_dict(self.nd, delimiter=delimiter)
+        nd1 = ndict.from_flatten_dict(self.nd, delimiter=delimiter)
         assert nd1 is not self.nd
         assert nd1._d is not self.nd._d
         assert nd1 == self.nd
 
-        nd1 = NDict.from_flatten_dict(self.nd.flatten_dict, delimiter=delimiter)
+        nd1 = ndict.from_flatten_dict(self.nd.flatten_dict, delimiter=delimiter)
         assert nd1 is not self.nd
         assert nd1._d is not self.nd._d
         assert nd1 == self.nd
 
     def test_from_list(self, delimiter=";"):
-        nd1 = NDict.from_list_of_dict(self.nd.flatten_dict_split, delimiter=delimiter)
+        nd1 = ndict.from_list_of_dict(self.nd.flatten_dict_split, delimiter=delimiter)
         assert nd1 == self.nd
 
     def test_eq(self, delimiter=";"):
         nd = deepcopy(self.nd)
         assert nd == self.nd
         nd[f"task{delimiter}task"] = "not_exist"
         assert nd != self.nd
         nd = deepcopy(self.nd)
         nd["not_exist"] = "not_exist"
         assert nd != self.nd
 
         d = deepcopy(self.nd.raw_dict)
-        nd = NDict(d, delimiter=delimiter)
+        nd = ndict(d, delimiter=delimiter)
         assert nd == self.nd
         del d["task"]
-        nd = NDict(d, delimiter=delimiter)
+        nd = ndict(d, delimiter=delimiter)
         assert nd != self.nd
 
     def test_paths(self, delimiter=";"):
         for p in self.nd.paths:
             self.nd[p]
 
         all_paths = []
@@ -239,15 +239,15 @@
         }
         assert self.nd.compare_dict(nd) == {
             f"not_exist{delimiter}not_exist{delimiter}not_exist": (None, "not_exist")
         }
 
     def test_delimiter(self):
         delimiter = "."
-        self.nd = NDict(self.rawd, delimiter=delimiter)
+        self.nd = ndict(self.rawd, delimiter=delimiter)
         self.test_init(delimiter=delimiter)
         self.test_from_flatten_dict(delimiter=delimiter)
         self.test_paths(delimiter=delimiter)
         self.test_contains(delimiter=delimiter)
         self.test_eq(delimiter=delimiter)
         self.test_del(delimiter=delimiter)
         self.test_getitem(delimiter=delimiter)
@@ -257,27 +257,27 @@
         self.test_compare(delimiter=delimiter)
 
 
 class testNConfig:
     def __init__(self, delimiter=";"):
         with open("test/config.yaml", "r") as f:
             self.rawd = yaml.safe_load(f)
-        self.nd = NDict(self.rawd, delimiter=delimiter)
+        self.nd = ndict(self.rawd, delimiter=delimiter)
 
         self.test_init()
         print("Pass init test.")
 
         self.test_parse()
         print("Pass arg parsing test.")
 
         with open("test/config_arg_spe.yaml", "r") as f:
             rawd_spe = yaml.safe_load(f)
-        nd_spe = NDict(rawd_spe, delimiter=delimiter)
+        nd_spe = ndict(rawd_spe, delimiter=delimiter)
 
-        self.config = NConfig(nd_spe, delimiter=delimiter)
+        self.config = nconfig(nd_spe, delimiter=delimiter)
 
         self.test_update()
         print("Pass update test.")
 
         self.test_setitem()
         print("Pass setitem test.")
 
@@ -286,21 +286,21 @@
 
         self.test_delimiter()
         print("Pass delimiter test.")
 
     def test_init(self, delimiter=";"):
         with open("test/config_arg_spe.yaml", "r") as f:
             rawd_spe = yaml.safe_load(f)
-        nd_spe = NDict(rawd_spe, delimiter=delimiter)
+        nd_spe = ndict(rawd_spe, delimiter=delimiter)
 
-        config = NConfig(self.rawd, delimiter=delimiter)
+        config = nconfig(self.rawd, delimiter=delimiter)
         assert config == self.nd
         assert config != nd_spe
 
-        config = NConfig(nd_spe, delimiter=delimiter)
+        config = nconfig(nd_spe, delimiter=delimiter)
         assert config._arg_specification
         assert config._d is not self.rawd
 
     def test_parse(self, delimiter=";"):
         def _get_test_value(v):
             def _get(v):
                 if isinstance(v, bool):
@@ -323,18 +323,18 @@
                     _v.append(_get(x))
                 return _v
             else:
                 return _get(v)
 
         with open("test/config_arg_spe.yaml", "r") as f:
             rawd_spe = yaml.safe_load(f)
-        nd_spe = NDict(rawd_spe, delimiter=delimiter)
-        config = NConfig(nd_spe, delimiter=delimiter)
+        nd_spe = ndict(rawd_spe, delimiter=delimiter)
+        config = nconfig(nd_spe, delimiter=delimiter)
         for path, v in config.flatten_dict.items():
-            config = NConfig(nd_spe, delimiter=delimiter)
+            config = nconfig(nd_spe, delimiter=delimiter)
             parser = argparse.ArgumentParser()
             if config._arg_specification.get(path, None) == config._ignore_key:
                 parser = config.add_to_argparse(parser)
                 flag = f"--{path.replace(delimiter, '__')}"
                 _args = [flag, "1"]
                 args, extra_args = parser.parse_known_args(_args)
                 assert extra_args == _args
@@ -440,28 +440,28 @@
         except Exception:
             pass
 
     def test_save(self, delimiter=";"):
         self.config.save("tmp.yaml")
         with open("tmp.yaml", "r") as f:
             d = yaml.safe_load(f)
-        config = NConfig(d, delimiter=delimiter)
+        config = nconfig(d, delimiter=delimiter)
         assert config == self.config
         assert config._arg_specification == self.config._arg_specification
         os.system("rm -rf tmp.yaml")
 
     def test_delimiter(self):
         delimiter = "."
-        self.nd = NDict(self.rawd, delimiter=delimiter)
+        self.nd = ndict(self.rawd, delimiter=delimiter)
         self.test_init(delimiter=delimiter)
         self.test_parse(delimiter=delimiter)
         with open("test/config_arg_spe.yaml", "r") as f:
             rawd_spe = yaml.safe_load(f)
-        nd_spe = NDict(rawd_spe, delimiter=delimiter)
-        self.config = NConfig(nd_spe, delimiter=delimiter)
+        nd_spe = ndict(rawd_spe, delimiter=delimiter)
+        self.config = nconfig(nd_spe, delimiter=delimiter)
         self.test_update(delimiter=delimiter)
         self.test_setitem(delimiter=delimiter)
         self.test_save(delimiter=delimiter)
 
 
 testNDict()
```

