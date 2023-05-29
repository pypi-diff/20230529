# Comparing `tmp/reviewcheck-0.5.1.tar.gz` & `tmp/reviewcheck-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviewcheck-0.5.1.tar", max compression
+gzip compressed data, was "reviewcheck-0.6.0.tar", max compression
```

## Comparing `reviewcheck-0.5.1.tar` & `reviewcheck-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11349 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/LICENSE
--rw-r--r--   0        0        0     1565 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/README.md
--rw-r--r--   0        0        0     1107 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/__init__.py
--rwxr-xr-x   0        0        0       92 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/__main__.py
--rwxr-xr-x   0        0        0    12980 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/app.py
--rw-r--r--   0        0        0     3560 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/cli.py
--rw-r--r--   0        0        0        0 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/common/__init__.py
--rw-r--r--   0        0        0     1193 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/common/constants.py
--rw-r--r--   0        0        0      261 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/common/exceptions.py
--rw-r--r--   0        0        0     1113 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/common/url_builder.py
--rw-r--r--   0        0        0     2399 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/config.py
--rw-r--r--   0        0        0     3473 2022-10-26 15:50:40.033387 reviewcheck-0.5.1/reviewcheck/utils.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 reviewcheck-0.5.1/setup.py
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 reviewcheck-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-29 07:31:02.735716 reviewcheck-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4637 2023-05-29 07:31:02.735716 reviewcheck-0.6.0/README.md
+-rw-r--r--   0        0        0     1189 2023-05-29 07:31:02.735716 reviewcheck-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/__init__.py
+-rwxr-xr-x   0        0        0      218 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/__main__.py
+-rwxr-xr-x   0        0        0    10093 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/app.py
+-rw-r--r--   0        0        0     4605 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/cli.py
+-rw-r--r--   0        0        0     2946 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/config.py
+-rw-r--r--   0        0        0     1376 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/constants.py
+-rw-r--r--   0        0        0      442 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/exceptions.py
+-rw-r--r--   0        0        0     7580 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/merge_request.py
+-rw-r--r--   0        0        0     5030 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/rich_components.py
+-rw-r--r--   0        0        0     4819 2023-05-29 07:31:02.743716 reviewcheck-0.6.0/reviewcheck/utils.py
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 reviewcheck-0.6.0/PKG-INFO
```

### Comparing `reviewcheck-0.5.1/LICENSE` & `reviewcheck-0.6.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 onwards, Volvo Cars
+   Copyright 2022 Volvo Car Corporation
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `reviewcheck-0.5.1/pyproject.toml` & `reviewcheck-0.6.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "reviewcheck"
-version = "0.5.1"
+version = "0.6.0"
 description = "Tool to stay up to date with your reviews on GitLab – Don't let a comment slip you by"
 authors = ["Simon Bengtsson <simon.bengtsson.3@volvocars.com>", "Pontus Laos <pontus.laos@volvocars.com>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 homepage = "https://github.com/volvo-cars/Reviewcheck"
 keywords = ["code review", "gitlab"]
 
 [tool.poetry.scripts]
 reviewcheck = "reviewcheck.app:run"
 
 [tool.poetry.dependencies]
-python = "^3.6.9"
-requests = "^2.27.1"
-pyyaml = "^5.1"
-shtab = "^1.5.4"
-colorama = "^0.4.4"
-rich = "^12.4.4"
+python = ">=3.8.1"
+requests = ">=2.27.1"
+pyyaml = ">=5.1"
+shtab = ">=1.5.4"
+colorama = ">=0.4.4"
+rich = ">=12.4.4"
 
-[tool.poetry.dev-dependencies]
-flake8 = "^4.0.1"
+[tool.poetry.group.dev.dependencies]
+flake8 = ">=4.0.1"
 pytest = ">=7.0.1"
-types-PyYAML = "^6.0.7"
-types-requests = "^2.27.29"
-isort = "^5.10.1"
-black = "^22.1.0"
-mypy = "^0.961"
+types-PyYAML = ">=6.0.7"
+types-requests = ">=2.27.29"
+isort = ">=5.10.1"
+black = ">=22.1.0"
+mypy = ">=0.961"
+flake8-docstrings = ">=1.6.0"
+flake8-rst-docstrings = ">=0.2.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 color_output = true
```

### Comparing `reviewcheck-0.5.1/reviewcheck/cli.py` & `reviewcheck-0.6.0/reviewcheck/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,53 @@
+# Copyright 2023 Volvo Car Corporation
+# Licensed under Apache 2.0.
+
+"""Parse the command line arguments given to reviewcheck."""
 import argparse
 from argparse import Namespace, RawTextHelpFormatter
 
 import shtab
 
 
 class Cli:
+    """Class with the functions associated with argument parsing."""
+
     @staticmethod
     def check_positive_int(value: str) -> int:
+        """Return positive int if possible, otherwise raise exception.
+
+        Validator for checking that a variable is a positive integer and
+        converting it to the int type.
+
+        :param value: The value given on command line.
+
+        :raises:ArgumentTypeError: Raised when the value cannot be
+            converted to a positive integer.
+
+        :return: The value as a positive int if possible.
+        """
         try:
             ivalue = int(value)
         except Exception:
             raise argparse.ArgumentTypeError("Flag argument must be a positive integer")
 
         if ivalue > 0:
             return ivalue
         else:
             raise argparse.ArgumentTypeError("Flag argument must be a positive integer")
 
     @staticmethod
     def parse_arguments() -> Namespace:
+        """Parse the arguments given on the command line.
+
+        Create an argument parser and use it to parse the arguments
+        given on the command line.
+
+        :return: The parsed arguments as a Namespace object.
+        """
         parser = argparse.ArgumentParser(
             description="""
         This script will tell you which discussions on GitLab you need to respond to.
         You will be shown the discussions from MRs where:
 
         - You are the author
         - Someone has replied to your comment but you haven't replied back
@@ -52,15 +77,15 @@
             help="Show version",
             dest="print_version",
             required=False,
             action="store_true",
             default=False,
         )
 
-        shtab.add_argument_to(parser, ["-s", "--print-completion"])  # type: ignore
+        shtab.add_argument_to(parser, ["-s", "--print-completion"])
 
         parser.add_argument(
             "-a",
             "--all",
             help="Show all threads, even when you don't need to reply",
             action="store_true",
             default=False,
@@ -110,14 +135,22 @@
             "--width",
             help="Terminal display width",
             type=Cli.check_positive_int,
             action="store",
             dest="output_width",
         )
 
+        parser.add_argument(
+            "-N",
+            "--no-notifications",
+            help="Do not invoke notify-send(1)",
+            action="store_true",
+            default=False,
+        )
+
         subparsers = parser.add_subparsers(dest="command")
 
         subparsers.add_parser(
             "configure",
             help="Interactively set up configuration file",
             description="Asks for input to write to the configuration file.",
         )
```

### Comparing `reviewcheck-0.5.1/reviewcheck/common/constants.py` & `reviewcheck-0.6.0/reviewcheck/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+# Copyright 2023 Volvo Car Corporation
+# Licensed under Apache 2.0.
+
+"""File for holding constants used in reviewcheck."""
 import os
 from pathlib import Path
 from typing import List
 
 
 class Constants:
+    """Class for holding constants used in reviewcheck."""
+
     COLORS: List[str] = [
         "green",
         "yellow",
         "blue",
         "magenta",
         "cyan",
         "white",
```

### Comparing `reviewcheck-0.5.1/reviewcheck/config.py` & `reviewcheck-0.6.0/reviewcheck/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,35 @@
+# Copyright 2023 Volvo Car Corporation
+# Licensed under Apache 2.0.
+
+"""File containing the Config class for working with config files."""
 from typing import Any, Dict, Optional
 
 import yaml
 
-from reviewcheck.common.constants import Constants
+from reviewcheck.constants import Constants
 
 
 class Config:
-    """
-    Class for interacting with the configuration file.
-    """
+    """Class for interacting with the configuration file."""
 
     def __init__(self, reconfigure: bool):
+        """Set initial variable state for the Config class.
+
+        :param reconfigure: Whether or not the user has requested to
+            update the configuration of reviewcheck.
+        """
         self.reconfigure = reconfigure
 
     def setup_configuration(self) -> None:
+        """Let the user configure the application.
+
+        This will be done if the user has requested to configure
+        reviewcheck or if no config file can be found.
+        """
         # Only attempt to write the configuration file if it does not
         # already exist.
         if self.reconfigure or not Constants.CONFIG_PATH.exists():
             Constants.CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
             if not self.reconfigure:
                 print(
@@ -44,23 +56,23 @@
                 "project_ids": project_ids_list,
             }
 
             with open(Constants.CONFIG_PATH, "w") as f:
                 f.write(yaml.safe_dump(config_object))
 
     def get_configuration(self) -> Optional[Dict[str, Any]]:
-        """
+        """Read the configuration file into a dictionary.
+
         Reads the configuration file into a dictionary. If the
         configuration file does not exist, queries the user for
         information and writes it.
 
         :return: A dict containing the contents of the configuration
             file, or None if the file does not exist.
         """
-
         self.setup_configuration()
         try:
             with open(Constants.CONFIG_PATH, "r") as f:
                 content = yaml.safe_load(f)
         except FileNotFoundError:
             return None
```

