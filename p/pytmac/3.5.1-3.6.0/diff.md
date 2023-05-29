# Comparing `tmp/pytmac-3.5.1.tar.gz` & `tmp/pytmac-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.5.1.tar", last modified: Mon May 29 11:10:31 2023, max compression
+gzip compressed data, was "pytmac-3.6.0.tar", last modified: Mon May 29 20:14:37 2023, max compression
```

## Comparing `pytmac-3.5.1.tar` & `pytmac-3.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-29 11:10:28.000000 pytmac-3.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6379 2023-05-29 11:10:31.425851 pytmac-3.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6266 2023-05-29 11:10:28.000000 pytmac-3.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-29 11:10:29.000000 pytmac-3.5.1/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/bin/
--rw-r--r--   0 root         (0) root         (0)     5106 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/init.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2722 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/docs/
--rw-r--r--   0 root         (0) root         (0)      238 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1061 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7402 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-29 11:10:28.000000 pytmac-3.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    23607 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6379 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:10:31.425851 pytmac-3.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-29 11:10:28.000000 pytmac-3.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:14:37.652241 pytmac-3.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-29 20:14:34.000000 pytmac-3.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-05-29 20:14:37.652241 pytmac-3.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6935 2023-05-29 20:14:34.000000 pytmac-3.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-29 20:14:35.000000 pytmac-3.6.0/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:14:37.648241 pytmac-3.6.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     5194 2023-05-29 20:14:34.000000 pytmac-3.6.0/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)    12274 2023-05-29 20:14:34.000000 pytmac-3.6.0/bin/init.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2023-05-29 20:14:34.000000 pytmac-3.6.0/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-05-29 20:14:34.000000 pytmac-3.6.0/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:14:37.652241 pytmac-3.6.0/conf/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-29 20:14:34.000000 pytmac-3.6.0/conf/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-29 20:14:34.000000 pytmac-3.6.0/conf/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-05-29 20:14:34.000000 pytmac-3.6.0/conf/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-05-29 20:14:34.000000 pytmac-3.6.0/conf/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-29 20:14:34.000000 pytmac-3.6.0/conf/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-29 20:14:34.000000 pytmac-3.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    23684 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:14:37.652241 pytmac-3.6.0/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-29 20:14:37.000000 pytmac-3.6.0/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:14:37.652241 pytmac-3.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-29 20:14:34.000000 pytmac-3.6.0/setup.py
```

### Comparing `pytmac-3.5.1/LICENSE` & `pytmac-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.1/PKG-INFO` & `pytmac-3.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pytmac
-Version: 3.5.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -154,7 +148,28 @@
 Python-semantic-release relies on conventional commits being used for all commit messages to determine the next version number / semantic release type (major/minor/patch).
 
 Once the new version number has been determined, a new release is created on github, and the new version is published to PyPi.
 
 ## gpush
 
 You can use my other project [gpush](https://github.com/tjtharrison/gpush) to ensure you always push commits with the correct format for this project, otherwise, details on commit message structure can be found on the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) website.
+
+## Documentation
+
+Documentation is generated using [mkdocs](https://www.mkdocs.org/), and is hosted on github pages. To generate the documentation locally, run the following command:
+
+> NOTE: Before running for the first time you will need to ensure that you have the required packages installed, you can do this as:
+
+
+```agsl
+pip3 install -r requirements.docs.txt
+```
+
+Now run the following make command to generate and serve the docs
+
+```bash
+make mkdocs
+```
+
+This will generate a new copy of the documentation in the `./docs` directory and serve it on `http://localhost:8000`.
+
+> NOTE: This action will also run during CI to ensure the documentation is up-to-date.
```

### Comparing `pytmac-3.5.1/README.md` & `pytmac-3.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pytmac
+Version: 3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -148,7 +154,28 @@
 Python-semantic-release relies on conventional commits being used for all commit messages to determine the next version number / semantic release type (major/minor/patch).
 
 Once the new version number has been determined, a new release is created on github, and the new version is published to PyPi.
 
 ## gpush
 
 You can use my other project [gpush](https://github.com/tjtharrison/gpush) to ensure you always push commits with the correct format for this project, otherwise, details on commit message structure can be found on the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) website.
+
+## Documentation
+
+Documentation is generated using [mkdocs](https://www.mkdocs.org/), and is hosted on github pages. To generate the documentation locally, run the following command:
+
+> NOTE: Before running for the first time you will need to ensure that you have the required packages installed, you can do this as:
+
+
+```agsl
+pip3 install -r requirements.docs.txt
+```
+
+Now run the following make command to generate and serve the docs
+
+```bash
+make mkdocs
+```
+
+This will generate a new copy of the documentation in the `./docs` directory and serve it on `http://localhost:8000`.
+
+> NOTE: This action will also run during CI to ensure the documentation is up-to-date.
```

### Comparing `pytmac-3.5.1/bin/get_config.py` & `pytmac-3.6.0/bin/get_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Modules to load the configuration files for pytmac from provided data files."""
 import json
 import os
 
 import yaml
 
-docs_dir = os.path.join(os.path.dirname(__file__), "../", "docs")
+docs_dir = os.path.join(os.path.dirname(__file__), "../", "conf")
 
 
 def resources(file):
-    """
-    Return a list of resources to be included in the package.
+    """Return a list of resources to be included in the package.
+
+    Args:
+        file: File to load resources from
+
+    Returns:
+        List of resources
 
-    :param file: File to load resources from
-    :raises FileNotFoundError: If file is not found
-    :raises YAMLError: If file is not valid YAML
+    Raises:
+        FileNotFoundError: If file is not found
+        YAMLError: If file is not valid YAML
 
-    :return: List of resources
     """
     if file == "demo":
         file = docs_dir + "/resources.yaml"
 
     try:
         with open(file, "r", encoding="UTF-8") as resources_file:
             try:
@@ -29,22 +33,26 @@
     except FileNotFoundError as error_message:
         raise FileNotFoundError("No resources file found at " + file) from error_message
 
     return resources_yaml
 
 
 def config(file):
-    """
-    Return a list of config to be included in the package.
+    """Return a list of config to be included in the package.
+
+    Args:
+        file: File to load resources from
 
-    :param file: File to load resources from
-    :raises FileNotFoundError: If file is not found
-    :raises YAMLError: If file is not valid YAML
+    Returns:
+        List of resources
+
+    Raises:
+        FileNotFoundError: If file is not found
+        YAMLError: If file is not valid YAML
 
-    :return: List of resources
     """
     if file == "demo":
         file = docs_dir + "/config.yaml"
 
     try:
         with open(file, "r", encoding="UTF-8") as config_file:
             try:
@@ -54,22 +62,26 @@
     except FileNotFoundError as error_message:
         raise FileNotFoundError("No config file found at " + file) from error_message
 
     return config_yaml
 
 
 def defaults(file):
-    """
-    Return a list of defaults to be included in the package.
+    """Return a list of defaults to be included in the package.
+
+    Args:
+        file: File to load resources from
+
+    Returns:
+        List of resources
 
-    :param file: File to load resources from
-    :raises FileNotFoundError: If file is not found
-    :raises YAMLError: If file is not valid YAML
+    Raises:
+        FileNotFoundError: If file is not found
+        YAMLError: If file is not valid YAML
 
-    :return: List of resources
     """
     if file == "demo":
         file = docs_dir + "/defaults.yaml"
 
     try:
         with open(file, "r", encoding="UTF-8") as default_file:
             try:
@@ -79,22 +91,26 @@
     except FileNotFoundError as error_message:
         raise FileNotFoundError("No defaults file found at " + file) from error_message
 
     return default_yaml
 
 
 def security_checks(file):
-    """
-    Return a list of security_checks to be included in the package.
+    """Return a list of security_checks to be included in the package.
+
+    Args:
+        file: File to load resources from
 
-    :param file: File to load resources from
-    :raises FileNotFoundError: If file is not found
-    :raises YAMLError: If file is not valid YAML
+    Returns:
+        List of resources
+
+    Raises:
+        FileNotFoundError: If file is not found
+        YAMLError: If file is not valid YAML
 
-    :return: List of resources
     """
     if file == "default":
         file = docs_dir + "/security_checks.yaml"
 
     try:
         with open(file, "r", encoding="UTF-8") as security_checks_file:
             try:
@@ -109,22 +125,26 @@
             "No security_checks file found at " + file
         ) from error_message
 
     return security_checks_yaml
 
 
 def swagger(file):
-    """
-    Get and return swagger file contents.
+    """Get and return swagger file contents.
 
-    :param file: File to load resources from
-    :raises FileNotFoundError: If file is not found
-    :raises Exception: If file is not valid JSON
+    Args:
+        file: File to load resources from
+
+    Returns:
+        List of resources
+
+    Raises:
+        FileNotFoundError: If file is not found
+        Exception: If file is not valid JSON
 
-    :return: List of resources
     """
     if file == "demo":
         file = docs_dir + "/swagger.json"
 
     try:
         with open(file, "r", encoding="UTF-8") as swagger_file:
             try:
@@ -138,21 +158,23 @@
             "No swagger.json file found at " + file
         ) from error_message
 
     return swagger_json
 
 
 def settings():
-    """
-    Get and return settings file contents from .pytmac file.
+    """Get and return settings file contents from .pytmac file.
+
+    Returns:
+        settings file contents
 
-    :raises FileNotFoundError: If file is not found
-    :raises YAMLError: If file is not valid YAML
+    Raises:
+        FileNotFoundError: If file is not found
+        YAMLError: If file is not valid YAML
 
-    :return: settings file contents
     """
     try:
         with open(".pytmac", "r", encoding="UTF-8") as settings_file:
             try:
                 settings_yaml = yaml.safe_load(settings_file)
             except yaml.YAMLError as error_message:
                 raise yaml.YAMLError(
```

### Comparing `pytmac-3.5.1/bin/init.py` & `pytmac-3.6.0/bin/init.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import inquirer
 import yaml
 
 from bin import get_config
 
 
 def get_inputs():
-    """
-    Get user input for project configuration.
+    """Get user input for project configuration.
+
+    Returns:
+        Dictionary with user input
 
-    :raises KeyboardInterrupt: if user cancels input
+    Raises:
+        KeyboardInterrupt: if user cancels input
 
-    :return: Dictionary with user input
     """
     try:
         print("Okay lets get your directory setup for pytmac!")
         project_name = input("First, what shall we name your project? ")
         project_description = input("What is your project about? ")
         config_directory = (
             input("Where shall we store your configuration files? (default: ./docs) ")
@@ -30,43 +32,52 @@
         "project_name": project_name,
         "project_description": project_description,
         "config_directory": config_directory,
     }
 
 
 def create_directory(name):
-    """
-    Create a directory if it does not exist.
+    """Create a directory if it does not exist.
+
+    Args:
+        name: Name of directory to create
+
+    Returns:
+        True if directory was created, False if it already exists
+
+    Raises:
+        OSError: if directory cannot be created
 
-    :raises OSError: if directory cannot be created
-    :param name: Name of directory to create
-    :return: True if directory was created, False if it already exists
     """
     try:
         if not os.path.exists(name):
             os.makedirs(name)
         else:
             print("Directory already exists..")
     except OSError as error_message:
         print("Error: Creating directory. " + name)
         raise OSError from error_message
 
     return True
 
 
 def create_config_file(project_config):
-    """
-    Create a config file for the project with user provided values.
+    """Create a config file for the project with user provided values.
+
+    Args:
+        project_config: User provided input for project.
 
-    :raises OSError: if config file cannot be loaded
-    :raises YAMLError: if values cannot be updated
-    :raises KeyError: if config file cannot be created
+    Returns:
+        True if config file was created
+
+    Raises:
+        OSError: if config file cannot be loaded
+        YAMLError: if values cannot be updated
+        KeyError: if config file cannot be created
 
-    :param project_config: User provided input for project.
-    :return: True if config file was created
     """
     # Get default config file
     try:
         config_input = get_config.config("demo")
     except OSError as error_message:
         print("Error: Getting default config file.")
         raise OSError from error_message
@@ -86,41 +97,48 @@
     except yaml.YAMLError as error_message:
         raise yaml.YAMLError from error_message
 
     return True
 
 
 def create_defaults_file(project_config):
-    """
-    Create a defaults file for the project.
+    """Create a defaults file for the project.
 
-    :raises OSError: if defaults file cannot be loaded
-    :raises YAMLError: if values cannot be updated
+    Args:
+        project_config: User provided input for project.
+
+    Returns:
+        True if defaults file was created
+
+    Raises:
+        OSError: if defaults file cannot be loaded
+        YAMLError: if values cannot be updated
 
-    :param project_config: User provided input for project.
-    :return: True if defaults file was created
     """
     defaults_file = project_config["config_directory"] + "/defaults.yaml"
     try:
         with open(defaults_file, "w", encoding="UTF-8") as defaults_file_update:
             yaml.dump(get_config.defaults("demo"), defaults_file_update)
     except OSError as error_message:
         raise OSError from error_message
     except yaml.YAMLError as error_message:
         raise yaml.YAMLError from error_message
 
     return True
 
 
 def return_summary(project_config):
-    """
-    Return a summary of the project configuration.
+    """Return a summary of the project configuration.
+
+    Args:
+        project_config: User provided input for project.
+
+    Returns:
+        True if summary was returned
 
-    :param project_config: User provided input for project.
-    :return: True if summary was returned
     """
     print(
         "\n".join(
             [
                 "",
                 "Great! Project " + project_config["project_name"] + " created! 🫡",
                 "Config files stored in " + project_config["config_directory"] + " 📁",
@@ -132,42 +150,46 @@
         )
     )
 
     return True
 
 
 def create_resources_file(project_config, all_resources):
-    """
-    Create a resources file for the project.
-
-    :raises OSError: if resources file cannot be loaded
-    :raises YAMLError: if values cannot be updated
+    """Create a resources file for the project.
 
+    Args:
+        project_config: User provided input for project.
+        all_resources: json file with all resources
+
+    Returns:
+        True if resources file was created
+
+    Raises:
+        OSError: if resources file cannot be loaded
+        YAMLError: if values cannot be updated
 
-    :param project_config:  User provided input for project.
-    :param all_resources: json file with all resources
-    :return: True if resources file was created
     """
     resources_file = project_config["config_directory"] + "/resources.yaml"
     try:
         with open(resources_file, "w", encoding="UTF-8") as resources_file_update:
             yaml.dump(all_resources, resources_file_update)
     except OSError as error_message:
         raise OSError from error_message
     except yaml.YAMLError as error_message:
         raise yaml.YAMLError from error_message
 
     return True
 
 
 def get_networks():
-    """
-    Get networks for project configuration.
+    """Get networks for project configuration.
+
+    Returns:
+        List of networks
 
-    :return: List of networks
     """
     networks = []
 
     while True:
         if len(networks) > 0:
             more_networks = input(
                 "Do you have any more networks to add? (yes/no) "
@@ -192,20 +214,23 @@
             )
             networks.append({"name": network_name})
 
     return networks
 
 
 def get_users(network, users):
-    """
-    Get users for project configuration.
+    """Get users for project configuration.
+
+    Args:
+        network: Name of network
+        users: List of users already added
+
+    Returns:
+        List of users
 
-    :param network: Name of network
-    :param users: List of users already added
-    :return: List of users
     """
     while True:
         more_users = input(
             "Do you have any more users to add on network " + network + " ? (yes/no) "
         ).lower()
         if more_users == "yes":
             user_name = (
@@ -226,20 +251,23 @@
         else:
             print("Please enter either yes or no. " + more_users + " entered")
 
         return users
 
 
 def get_databases(network, databases):
-    """
-    Get databases for project configuration.
+    """Get databases for project configuration.
+
+    Args:
+        network: Name of network
+        databases: List of databases already added
+
+    Returns:
+        list of databases
 
-    :param network: Name of network
-    :param databases: List of databases already added
-    :return: list of databases
     """
     while True:
         more_databases = input(
             "Do you have any more databases to add on network "
             + network
             + " ? (yes/no) "
         ).lower()
@@ -264,20 +292,23 @@
         else:
             print("Please enter either yes or no. " + more_databases + " entered")
 
     return databases
 
 
 def get_systems(network, systems):
-    """
-    Get systems for project configuration.
+    """Get systems for project configuration.
+
+    Args:
+        network: Name of network
+        systems: List of systems already added
+
+    Returns:
+        list of systems
 
-    :param network: Name of network
-    :param systems: List of systems already added
-    :return: list of systems
     """
     while True:
         more_systems = input(
             "Do you have any more systems to add on network " + network + " ? (yes/no) "
         ).lower()
         if more_systems == "yes":
             system_name = (
@@ -300,35 +331,41 @@
         else:
             print("Please enter either yes or no. " + more_systems + " entered")
 
     return systems
 
 
 def get_resource_names(all_resources):
-    """
-    Get all resource names from all_resources.
+    """Get all resource names from all_resources.
+
+    Args:
+        all_resources: json file with all resources
+
+    Returns:
+        List of resource names
 
-    :param all_resources: json file with all resources
-    :return: List of resource names
     """
     all_resource_names = []
     for key in all_resources["resources"]:
         if key != "networks" and all_resources["resources"][key] is not None:
             for resource in all_resources["resources"][key]:
                 all_resource_names.append(resource["name"])
 
     return all_resource_names
 
 
 def get_links(all_resource_names):
-    """
-    Get links for project configuration.
+    """Get links for project configuration.
+
+    Args:
+        all_resource_names: List of all resource names
+
+    Returns:
+        List of links
 
-    :param all_resource_names: List of all resource names
-    :return: List of links
     """
     links = []
     # Create some links between resources
     while True:
         more_links = input("Do you have any more links to add? (yes/no) ").lower()
         if more_links == "yes":
             questions = [
@@ -365,20 +402,25 @@
         else:
             print("Please enter either yes or no. " + more_links + " entered")
 
     return links
 
 
 def create_settings_file(project_config):
-    """
-    Create settings file for project.
+    """Create settings file for project.
+
+    Args:
+        project_config: Project configuration
+
+    Returns:
+        True if successful, False otherwise
+
+    Raises:
+        OSError: If unable to create settings file
 
-    :raises OSError: If unable to create settings file
-    :param project_config: Project configuration
-    :return: True if successful, False otherwise
     """
     try:
         with open(".pytmac", "w", encoding="utf-8") as settings_file:
             settings_file.write(
                 'resource_file: "'
                 + project_config["config_directory"]
                 + '/resources.yaml"'
```

### Comparing `pytmac-3.5.1/bin/input_validator.py` & `pytmac-3.6.0/bin/input_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Functions that validate the input files provided by the pytmac user."""
 import json
 import logging
 import os
 
 
 def config(config_json):
-    """
-    Validate required fields in config.json.
+    """Validate required fields in config.json.
+
+    Args:
+        config_json: Json structure containing the app running config
+
+    Returns:
+        True/False
 
-    :param config_json: Json structure containing the app running config
-    :return: True/False
     """
     try:
         title = config_json["title"]
         description = config_json["description"]
         logging.debug(json.dumps({"title": title, "description": description}))
         if os.environ.get("ENABLE_SWAGGER"):
             swagger_resource_type = config_json["swagger_resource_type"]
@@ -30,19 +33,22 @@
         logging.error(str(error_message))
         return False
 
     return True
 
 
 def resources(resources_json):
-    """
-    Validate required fields in resources.json.
+    """Validate required fields in resources.json.
+
+    Args:
+        resources_json: Json structure containing the app resources
+
+    Returns:
+        True/False
 
-    :param resources_json: Json structure containing the app resources
-    :return: True/False
     """
     # Validate top level fields set
     resource_types = list(resources_json["resources"].keys())
     required_network_types = ["networks", "databases", "users", "systems"]
     for required_type in required_network_types:
         if required_type not in resource_types:
             logging.error("%s not found in resources", required_type)
@@ -133,37 +139,43 @@
         )
         return False
 
     return True
 
 
 def defaults(defaults_json):
-    """
-    Validate required fields set in defaults.json.
+    """Validate required fields set in defaults.json.
+
+    Args:
+        defaults_json: Json structure containing resource defaults
+
+    Returns:
+        bool: True/False
 
-    :param defaults_json: Json structure containing resource defaults
-    :return: True/False
     """
     resource_types = defaults_json.keys()
 
     required_network_types = ["networks", "databases", "users", "systems"]
 
     for required_type in required_network_types:
         if required_type not in resource_types:
             logging.error("%s not found in defaults", required_type)
             return False
     return True
 
 
 def swagger(swagger_json):
-    """
-    Validate required fields set in swagger.json (If ENABLE_SWAGGER is set to True).
+    """Validate required fields set in swagger.json (If ENABLE_SWAGGER is set to True).
+
+    Args:
+        swagger_json: Json structure containing swagger file contents
+
+    Returns:
+        True/False
 
-    :param swagger_json: Json structure containing swagger file contents
-    :return: True/False
     """
     swagger_json = json.loads(swagger_json)
     # Validate paths exist
     if len(swagger_json["paths"]) < 1:
         logging.error("No paths provided in swagger.json")
         return False
```

### Comparing `pytmac-3.5.1/bin/resource_validator.py` & `pytmac-3.6.0/bin/resource_validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Module used to initiate and collate security findings from the json report generated."""
 import logging
 
 
 def main(security_checks_yaml, output_json_report):
-    """
-    Collect responses from required security scans and return.
+    """Collect responses from required security scans and return.
+
+    Args:
+        security_checks_yaml: A json document containing all security checks to be run.
+        output_json_report: A json document containing all resources and configuration settings
 
-    :param security_checks_yaml: A json document containing all security checks to be run.
-    :param output_json_report: A json document containing all resources and configuration settings
+    Returns:
+        List of insecure resources.
 
-    :return: List of insecure resources.
     """
     insecure_resources = []
 
     for security_check in security_checks_yaml:
         logging.info("Starting security check %s", security_check)
         results = do_check(output_json_report, security_checks_yaml[security_check])
         if len(results) > 0:
@@ -26,31 +28,34 @@
 
     logging.info("Insecure resources: %s", str(insecure_resources))
 
     return insecure_resources
 
 
 def do_check(output_json_report, check_details):
-    """
-    Look up a check type in security_checks.json and checks resources using a given function.
+    """Look up a check type in security_checks.json and checks resources using a given function.
 
     Insecure resources are returned in the format:
 
     [{
         "name": [The name of the check],
         "resource": [List of non-compliant resources],
         "description": [Description of what the check does],
         "check_query": [The query that returns True to generate this vulnerability type],
         "remediation": [Steps that should be taken to remediate the concern],
         "severity": [1-4 score on the impact of the insecurity]
     }]
 
-    :param output_json_report: The json report of resources and configuration
-    :param check_details: A json containing the details for the check to run.
-    :return: list(dict)
+    Args:
+        output_json_report: The json report of resources and configuration
+        check_details: A json containing the details for the check to run.
+
+    Returns:
+        list(dict)
+
     """
     resources = {}
     for resource_scope in check_details["resource_scope"]:
         resources = resources | output_json_report[resource_scope]
     insecure_resources = []
 
     for resource in resources:
```

### Comparing `pytmac-3.5.1/docs/defaults.yaml` & `pytmac-3.6.0/conf/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.1/docs/resources.yaml` & `pytmac-3.6.0/conf/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.1/docs/security_checks.yaml` & `pytmac-3.6.0/conf/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.1/docs/swagger.json` & `pytmac-3.6.0/conf/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.1/pytmac` & `pytmac-3.6.0/pytmac`

 * *Files 1% similar despite different names*

```diff
@@ -94,25 +94,27 @@
     resources_yaml,
     config_yaml,
     defaults_yaml,
     security_checks_yaml,
     output_dir,
     swagger_json="",
 ):
-    """
-    Primary function used to open up provided config and resource files, generating DFD and output.
+    """Primary function used to open up provided config and resource files, generating DFD and output.
+
+    Args:
+        resources_yaml: The resources yaml file.
+        config_yaml: The config yaml file.
+        defaults_yaml: The defaults yaml file.
+        security_checks_yaml: The security checks yaml file.
+        output_dir: The output directory.
+        swagger_json: The swagger json file (Default value = "").
 
-    :param resources_yaml: The resources yaml file
-    :param config_yaml: The config yaml file
-    :param defaults_yaml: The defaults yaml file
-    :param security_checks_yaml: The security checks yaml file
-    :param output_dir: The output directory
-    :param swagger_json: The swagger json file
+    Returns:
+        bool: The return value. True for success, False otherwise.
 
-    :return: True
     """
     # Validate configuration
     if not input_validator.config(config_yaml):
         logging.error("Config validation failed!")
         sys.exit(1)
 
     # Validate resources
```

### Comparing `pytmac-3.5.1/pytmac.egg-info/PKG-INFO` & `pytmac-3.6.0/pytmac.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.5.1
+Version: 3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -154,7 +154,28 @@
 Python-semantic-release relies on conventional commits being used for all commit messages to determine the next version number / semantic release type (major/minor/patch).
 
 Once the new version number has been determined, a new release is created on github, and the new version is published to PyPi.
 
 ## gpush
 
 You can use my other project [gpush](https://github.com/tjtharrison/gpush) to ensure you always push commits with the correct format for this project, otherwise, details on commit message structure can be found on the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) website.
+
+## Documentation
+
+Documentation is generated using [mkdocs](https://www.mkdocs.org/), and is hosted on github pages. To generate the documentation locally, run the following command:
+
+> NOTE: Before running for the first time you will need to ensure that you have the required packages installed, you can do this as:
+
+
+```agsl
+pip3 install -r requirements.docs.txt
+```
+
+Now run the following make command to generate and serve the docs
+
+```bash
+make mkdocs
+```
+
+This will generate a new copy of the documentation in the `./docs` directory and serve it on `http://localhost:8000`.
+
+> NOTE: This action will also run during CI to ensure the documentation is up-to-date.
```

### Comparing `pytmac-3.5.1/setup.py` & `pytmac-3.6.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 setup(
     name="pytmac",
     version=__version__,
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     install_requires=required,
     scripts=["pytmac", "_version.py"],
-    packages=["bin", "docs"],
-    package_data={"docs": ["*"]},
-    exclude_package_data={"docs": ["*bak*"]},
+    packages=["bin", "conf"],
+    package_data={"conf": ["*"]},
+    exclude_package_data={"conf": ["*bak*"]},
 )
```

