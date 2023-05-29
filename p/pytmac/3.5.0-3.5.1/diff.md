# Comparing `tmp/pytmac-3.5.0.tar.gz` & `tmp/pytmac-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.5.0.tar", last modified: Sat May 27 20:27:31 2023, max compression
+gzip compressed data, was "pytmac-3.5.1.tar", last modified: Mon May 29 11:10:31 2023, max compression
```

## Comparing `pytmac-3.5.0.tar` & `pytmac-3.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 20:27:31.213015 pytmac-3.5.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-27 20:27:28.000000 pytmac-3.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7054 2023-05-27 20:27:31.213015 pytmac-3.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6941 2023-05-27 20:27:28.000000 pytmac-3.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-27 20:27:29.000000 pytmac-3.5.0/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 20:27:31.209015 pytmac-3.5.0/bin/
--rw-r--r--   0 root         (0) root         (0)     5175 2023-05-27 20:27:28.000000 pytmac-3.5.0/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-05-27 20:27:28.000000 pytmac-3.5.0/bin/init.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-05-27 20:27:28.000000 pytmac-3.5.0/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2823 2023-05-27 20:27:28.000000 pytmac-3.5.0/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 20:27:31.213015 pytmac-3.5.0/docs/
--rw-r--r--   0 root         (0) root         (0)      238 2023-05-27 20:27:28.000000 pytmac-3.5.0/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-27 20:27:28.000000 pytmac-3.5.0/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1061 2023-05-27 20:27:28.000000 pytmac-3.5.0/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7402 2023-05-27 20:27:28.000000 pytmac-3.5.0/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-27 20:27:28.000000 pytmac-3.5.0/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-27 20:27:28.000000 pytmac-3.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    23614 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 20:27:31.213015 pytmac-3.5.0/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7054 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-27 20:27:31.000000 pytmac-3.5.0/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 20:27:31.213015 pytmac-3.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-27 20:27:28.000000 pytmac-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-29 11:10:28.000000 pytmac-3.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-05-29 11:10:31.425851 pytmac-3.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-05-29 11:10:28.000000 pytmac-3.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-29 11:10:29.000000 pytmac-3.5.1/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/bin/
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/init.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-05-29 11:10:28.000000 pytmac-3.5.1/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-29 11:10:28.000000 pytmac-3.5.1/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-29 11:10:28.000000 pytmac-3.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    23607 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:31.425851 pytmac-3.5.1/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-29 11:10:31.000000 pytmac-3.5.1/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:10:31.425851 pytmac-3.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-29 11:10:28.000000 pytmac-3.5.1/setup.py
```

### Comparing `pytmac-3.5.0/LICENSE` & `pytmac-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.0/PKG-INFO` & `pytmac-3.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.5.0
+Version: 3.5.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -122,39 +122,15 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
-```## Config file
-
-pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
-
-```
-resource_file: "docs/resources.yaml"
-config_file: "docs/config.yaml"
-defaults_file: "docs/defaults.yaml"
 ```
-
-If both a config file value and a manual override is added via the command line, the command line value will take precedence.
-
-Eg if you have a .pytmac file with the following:
-
-```
-resource_file: "docs/resources.yaml"
-```
-
-and call pytmac with the following:
-
-```
-pytmac --resources-file resources.yaml
-```
-
-the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.5.0/README.md` & `pytmac-3.5.1/pytmac.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pytmac
+Version: 3.5.1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -116,39 +122,15 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
-```## Config file
-
-pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
-
-```
-resource_file: "docs/resources.yaml"
-config_file: "docs/config.yaml"
-defaults_file: "docs/defaults.yaml"
-```
-
-If both a config file value and a manual override is added via the command line, the command line value will take precedence.
-
-Eg if you have a .pytmac file with the following:
-
-```
-resource_file: "docs/resources.yaml"
-```
-
-and call pytmac with the following:
-
-```
-pytmac --resources-file resources.yaml
 ```
-
-the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.5.0/bin/get_config.py` & `pytmac-3.5.1/bin/get_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""
-Modules to load the configuration files for pytmac from provided data files.
-"""
+"""Modules to load the configuration files for pytmac from provided data files."""
 import json
 import os
 
 import yaml
 
 docs_dir = os.path.join(os.path.dirname(__file__), "../", "docs")
 
 
 def resources(file):
     """
-    Function to return a list of resources to be included in the package
+    Return a list of resources to be included in the package.
 
     :param file: File to load resources from
     :raises FileNotFoundError: If file is not found
     :raises YAMLError: If file is not valid YAML
 
     :return: List of resources
     """
@@ -32,15 +30,15 @@
         raise FileNotFoundError("No resources file found at " + file) from error_message
 
     return resources_yaml
 
 
 def config(file):
     """
-    Function to return a list of config to be included in the package
+    Return a list of config to be included in the package.
 
     :param file: File to load resources from
     :raises FileNotFoundError: If file is not found
     :raises YAMLError: If file is not valid YAML
 
     :return: List of resources
     """
@@ -57,15 +55,15 @@
         raise FileNotFoundError("No config file found at " + file) from error_message
 
     return config_yaml
 
 
 def defaults(file):
     """
-    Function to return a list of defaults to be included in the package
+    Return a list of defaults to be included in the package.
 
     :param file: File to load resources from
     :raises FileNotFoundError: If file is not found
     :raises YAMLError: If file is not valid YAML
 
     :return: List of resources
     """
@@ -82,15 +80,15 @@
         raise FileNotFoundError("No defaults file found at " + file) from error_message
 
     return default_yaml
 
 
 def security_checks(file):
     """
-    Function to return a list of security_checks to be included in the package
+    Return a list of security_checks to be included in the package.
 
     :param file: File to load resources from
     :raises FileNotFoundError: If file is not found
     :raises YAMLError: If file is not valid YAML
 
     :return: List of resources
     """
@@ -112,23 +110,22 @@
         ) from error_message
 
     return security_checks_yaml
 
 
 def swagger(file):
     """
-    Function to get and return swagger file contents
+    Get and return swagger file contents.
 
     :param file: File to load resources from
     :raises FileNotFoundError: If file is not found
     :raises Exception: If file is not valid JSON
 
     :return: List of resources
     """
-
     if file == "demo":
         file = docs_dir + "/swagger.json"
 
     try:
         with open(file, "r", encoding="UTF-8") as swagger_file:
             try:
                 swagger_json = json.loads(swagger_file.read())
@@ -142,15 +139,15 @@
         ) from error_message
 
     return swagger_json
 
 
 def settings():
     """
-    Function to get and return settings file contents from .pytmac file
+    Get and return settings file contents from .pytmac file.
 
     :raises FileNotFoundError: If file is not found
     :raises YAMLError: If file is not valid YAML
 
     :return: settings file contents
     """
     try:
```

### Comparing `pytmac-3.5.0/bin/init.py` & `pytmac-3.5.1/bin/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""
-This file contains functions for creating a new pytmac project
-"""
+"""This file contains functions for creating a new pytmac project."""
 import os
 
 import inquirer
 import yaml
 
 from bin import get_config
 
 
 def get_inputs():
     """
-    Gets user input for project configuration
+    Get user input for project configuration.
 
     :raises KeyboardInterrupt: if user cancels input
 
     :return: Dictionary with user input
     """
     try:
         print("Okay lets get your directory setup for pytmac!")
@@ -33,15 +31,15 @@
         "project_description": project_description,
         "config_directory": config_directory,
     }
 
 
 def create_directory(name):
     """
-    Creates a directory if it does not exist
+    Create a directory if it does not exist.
 
     :raises OSError: if directory cannot be created
     :param name: Name of directory to create
     :return: True if directory was created, False if it already exists
     """
     try:
         if not os.path.exists(name):
@@ -53,24 +51,23 @@
         raise OSError from error_message
 
     return True
 
 
 def create_config_file(project_config):
     """
-    Creates a config file for the project with user provided values
+    Create a config file for the project with user provided values.
 
     :raises OSError: if config file cannot be loaded
     :raises YAMLError: if values cannot be updated
     :raises KeyError: if config file cannot be created
 
     :param project_config: User provided input for project.
     :return: True if config file was created
     """
-
     # Get default config file
     try:
         config_input = get_config.config("demo")
     except OSError as error_message:
         print("Error: Getting default config file.")
         raise OSError from error_message
 
@@ -90,43 +87,41 @@
         raise yaml.YAMLError from error_message
 
     return True
 
 
 def create_defaults_file(project_config):
     """
-    Creates a defaults file for the project
+    Create a defaults file for the project.
 
     :raises OSError: if defaults file cannot be loaded
     :raises YAMLError: if values cannot be updated
 
     :param project_config: User provided input for project.
     :return: True if defaults file was created
     """
-
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
     """
-    Returns a summary of the project configuration
+    Return a summary of the project configuration.
 
     :param project_config: User provided input for project.
     :return: True if summary was returned
     """
-
     print(
         "\n".join(
             [
                 "",
                 "Great! Project " + project_config["project_name"] + " created! 🫡",
                 "Config files stored in " + project_config["config_directory"] + " 📁",
                 "You can now run pytmac with `pytmac` 🚀",
@@ -138,40 +133,39 @@
     )
 
     return True
 
 
 def create_resources_file(project_config, all_resources):
     """
-    Creates a resources file for the project
+    Create a resources file for the project.
 
     :raises OSError: if resources file cannot be loaded
     :raises YAMLError: if values cannot be updated
 
 
     :param project_config:  User provided input for project.
     :param all_resources: json file with all resources
     :return: True if resources file was created
     """
-
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
     """
-    Gets networks for project configuration
+    Get networks for project configuration.
 
     :return: List of networks
     """
     networks = []
 
     while True:
         if len(networks) > 0:
@@ -199,21 +193,20 @@
             networks.append({"name": network_name})
 
     return networks
 
 
 def get_users(network, users):
     """
-    Gets users for project configuration
+    Get users for project configuration.
 
     :param network: Name of network
     :param users: List of users already added
     :return: List of users
     """
-
     while True:
         more_users = input(
             "Do you have any more users to add on network " + network + " ? (yes/no) "
         ).lower()
         if more_users == "yes":
             user_name = (
                 input("Please enter the name of your user? ").replace(" ", "_").lower()
@@ -234,21 +227,20 @@
             print("Please enter either yes or no. " + more_users + " entered")
 
         return users
 
 
 def get_databases(network, databases):
     """
-    Gets databases for project configuration
+    Get databases for project configuration.
 
     :param network: Name of network
     :param databases: List of databases already added
     :return: list of databases
     """
-
     while True:
         more_databases = input(
             "Do you have any more databases to add on network "
             + network
             + " ? (yes/no) "
         ).lower()
         if more_databases == "yes":
@@ -273,21 +265,20 @@
             print("Please enter either yes or no. " + more_databases + " entered")
 
     return databases
 
 
 def get_systems(network, systems):
     """
-    Gets systems for project configuration
+    Get systems for project configuration.
 
     :param network: Name of network
     :param systems: List of systems already added
     :return: list of systems
     """
-
     while True:
         more_systems = input(
             "Do you have any more systems to add on network " + network + " ? (yes/no) "
         ).lower()
         if more_systems == "yes":
             system_name = (
                 input("Please enter the name of your system? ")
@@ -310,15 +301,15 @@
             print("Please enter either yes or no. " + more_systems + " entered")
 
     return systems
 
 
 def get_resource_names(all_resources):
     """
-    Gets all resource names from all_resources
+    Get all resource names from all_resources.
 
     :param all_resources: json file with all resources
     :return: List of resource names
     """
     all_resource_names = []
     for key in all_resources["resources"]:
         if key != "networks" and all_resources["resources"][key] is not None:
@@ -326,15 +317,15 @@
                 all_resource_names.append(resource["name"])
 
     return all_resource_names
 
 
 def get_links(all_resource_names):
     """
-    Gets links for project configuration
+    Get links for project configuration.
 
     :param all_resource_names: List of all resource names
     :return: List of links
     """
     links = []
     # Create some links between resources
     while True:
@@ -375,15 +366,15 @@
             print("Please enter either yes or no. " + more_links + " entered")
 
     return links
 
 
 def create_settings_file(project_config):
     """
-    Creates settings file for project
+    Create settings file for project.
 
     :raises OSError: If unable to create settings file
     :param project_config: Project configuration
     :return: True if successful, False otherwise
     """
     try:
         with open(".pytmac", "w", encoding="utf-8") as settings_file:
```

### Comparing `pytmac-3.5.0/bin/input_validator.py` & `pytmac-3.5.1/bin/input_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""
-Functions that validate the input files provided by the pytmac user.
-"""
+"""Functions that validate the input files provided by the pytmac user."""
 import json
 import logging
 import os
 
 
 def config(config_json):
     """
-    Validate required fields in config.json
+    Validate required fields in config.json.
 
     :param config_json: Json structure containing the app running config
     :return: True/False
     """
     try:
         title = config_json["title"]
         description = config_json["description"]
@@ -33,20 +31,19 @@
         return False
 
     return True
 
 
 def resources(resources_json):
     """
-    Validate required fields in resources.json
+    Validate required fields in resources.json.
 
     :param resources_json: Json structure containing the app resources
     :return: True/False
     """
-
     # Validate top level fields set
     resource_types = list(resources_json["resources"].keys())
     required_network_types = ["networks", "databases", "users", "systems"]
     for required_type in required_network_types:
         if required_type not in resource_types:
             logging.error("%s not found in resources", required_type)
             return False
@@ -137,15 +134,15 @@
         return False
 
     return True
 
 
 def defaults(defaults_json):
     """
-    Validate required fields set in defaults.json
+    Validate required fields set in defaults.json.
 
     :param defaults_json: Json structure containing resource defaults
     :return: True/False
     """
     resource_types = defaults_json.keys()
 
     required_network_types = ["networks", "databases", "users", "systems"]
@@ -155,15 +152,15 @@
             logging.error("%s not found in defaults", required_type)
             return False
     return True
 
 
 def swagger(swagger_json):
     """
-    Validate required fields set in swagger.json (If ENABLE_SWAGGER is set to True)
+    Validate required fields set in swagger.json (If ENABLE_SWAGGER is set to True).
 
     :param swagger_json: Json structure containing swagger file contents
     :return: True/False
     """
     swagger_json = json.loads(swagger_json)
     # Validate paths exist
     if len(swagger_json["paths"]) < 1:
```

### Comparing `pytmac-3.5.0/bin/resource_validator.py` & `pytmac-3.5.1/bin/resource_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-"""
-Module used to initiate and collate security findings from the json report generated in the main
-document function.
-"""
+"""Module used to initiate and collate security findings from the json report generated."""
 import logging
 
 
 def main(security_checks_yaml, output_json_report):
     """
-    Function to collect responses from required security scans and return to be written to the final
-    report.
+    Collect responses from required security scans and return.
+
     :param security_checks_yaml: A json document containing all security checks to be run.
     :param output_json_report: A json document containing all resources and configuration settings
 
     :return: List of insecure resources.
     """
-
     insecure_resources = []
 
     for security_check in security_checks_yaml:
         logging.info("Starting security check %s", security_check)
         results = do_check(output_json_report, security_checks_yaml[security_check])
         if len(results) > 0:
             logging.info("Results found! Appending to insecure_resources")
@@ -31,16 +27,15 @@
     logging.info("Insecure resources: %s", str(insecure_resources))
 
     return insecure_resources
 
 
 def do_check(output_json_report, check_details):
     """
-    Function that looks up a check type in security_checks.json and checks resources using a given
-    function.
+    Look up a check type in security_checks.json and checks resources using a given function.
 
     Insecure resources are returned in the format:
 
     [{
         "name": [The name of the check],
         "resource": [List of non-compliant resources],
         "description": [Description of what the check does],
```

### Comparing `pytmac-3.5.0/docs/defaults.yaml` & `pytmac-3.5.1/docs/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.0/docs/resources.yaml` & `pytmac-3.5.1/docs/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.0/docs/security_checks.yaml` & `pytmac-3.5.1/docs/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.0/docs/swagger.json` & `pytmac-3.5.1/docs/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.5.0/pytmac` & `pytmac-3.5.1/pytmac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 
-"""
-Python based programmatic threat modelling tool tmacs
-"""
+"""Python based programmatic threat modelling tool tmacs."""
 import argparse
 import json
 import logging
 import os
 import subprocess
 import sys
 from copy import deepcopy
@@ -97,16 +95,16 @@
     config_yaml,
     defaults_yaml,
     security_checks_yaml,
     output_dir,
     swagger_json="",
 ):
     """
-    Main function used to open up provided config and resource files, generating DFD and output
-    report
+    Primary function used to open up provided config and resource files, generating DFD and output.
+
     :param resources_yaml: The resources yaml file
     :param config_yaml: The config yaml file
     :param defaults_yaml: The defaults yaml file
     :param security_checks_yaml: The security checks yaml file
     :param output_dir: The output directory
     :param swagger_json: The swagger json file
```

### Comparing `pytmac-3.5.0/pytmac.egg-info/PKG-INFO` & `pytmac-3.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pytmac
-Version: 3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -122,39 +116,15 @@
 ## Security Checks
 
 Security checks have been included to cover use cases for the Owasp top 10, however you may want to extend pytmac with custom checks can be written and added to `./docs/security_checks.yaml`. These files should be written as below, the 
 checks are iterated over and executed individually, all fields are required.
 
 Severity should be used as a combination of Risk vs Likelihood, any security findings are prioritised by severity in the report output. 
 
-```## Config file
-
-pytmac on launch will look for a file in the current directory named `.pytmac` as a source of settings. This file can be used to set the following settings:
-
-```
-resource_file: "docs/resources.yaml"
-config_file: "docs/config.yaml"
-defaults_file: "docs/defaults.yaml"
-```
-
-If both a config file value and a manual override is added via the command line, the command line value will take precedence.
-
-Eg if you have a .pytmac file with the following:
-
-```
-resource_file: "docs/resources.yaml"
-```
-
-and call pytmac with the following:
-
-```
-pytmac --resources-file resources.yaml
 ```
-
-the resources.yaml file will be used over the one defined in the .pytmac file.
 user_owned_device:
   name: Non company device used
   description: Checks for users with company_user true and company_device false.
   remediation: Understand and remediate or document known exception.
   severity: 3
   resource_scope:
     - users
```

### Comparing `pytmac-3.5.0/setup.py` & `pytmac-3.5.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Setup file for pytmac
-"""
+"""Setup file for pytmac."""
 from setuptools import setup
 
 from _version import __version__
 
 with open("README.md", encoding="UTF-8") as readme_file:
     readme_contents = readme_file.read()
```

