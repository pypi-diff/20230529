# Comparing `tmp/aws-sso-magic-1.0.34.tar.gz` & `tmp/aws_sso_magic-1.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-sso-magic-1.0.34.tar", max compression
+gzip compressed data, was "aws_sso_magic-1.0.35.tar", max compression
```

## Comparing `aws-sso-magic-1.0.34.tar` & `aws_sso_magic-1.0.35.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11346 2021-08-02 00:31:09.532292 aws-sso-magic-1.0.34/LICENSE
--rw-r--r--   0        0        0     5614 2021-08-04 00:41:19.946408 aws-sso-magic-1.0.34/README.md
--rw-r--r--   0        0        0     1088 2021-08-04 00:41:46.708390 aws-sso-magic-1.0.34/pyproject.toml
--rw-r--r--   0        0        0       54 2021-08-04 00:41:49.770166 aws-sso-magic-1.0.34/src/aws_sso_magic/__init__.py
--rw-r--r--   0        0        0      641 2021-08-02 00:31:09.533729 aws-sso-magic-1.0.34/src/aws_sso_magic/__main__.py
--rw-r--r--   0        0        0     1108 2021-08-02 00:31:09.533871 aws-sso-magic-1.0.34/src/aws_sso_magic/cli.py
--rw-r--r--   0        0        0     1553 2021-08-02 00:31:09.534026 aws-sso-magic-1.0.34/src/aws_sso_magic/configure.py
--rw-r--r--   0        0        0     3295 2021-08-02 00:31:09.534194 aws-sso-magic-1.0.34/src/aws_sso_magic/eks.py
--rw-r--r--   0        0        0    13966 2021-08-02 00:31:09.534387 aws-sso-magic-1.0.34/src/aws_sso_magic/login.py
--rw-r--r--   0        0        0     1979 2021-08-02 00:31:09.534626 aws-sso-magic-1.0.34/src/aws_sso_magic/logout.py
--rw-r--r--   0        0        0    26297 2021-08-02 00:31:09.534912 aws-sso-magic-1.0.34/src/aws_sso_magic/utils.py
--rw-r--r--   0        0        0     6804 2021-08-04 00:43:43.280332 aws-sso-magic-1.0.34/setup.py
--rw-r--r--   0        0        0     6883 2021-08-04 00:43:43.280970 aws-sso-magic-1.0.34/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/LICENSE
+-rw-r--r--   0        0        0     5614 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/README.md
+-rw-r--r--   0        0        0     1088 2023-05-29 03:33:56.829309 aws_sso_magic-1.0.35/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/src/aws_sso_magic/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/src/aws_sso_magic/__main__.py
+-rw-r--r--   0        0        0     1108 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/src/aws_sso_magic/cli.py
+-rw-r--r--   0        0        0     1553 2023-05-29 02:25:08.756993 aws_sso_magic-1.0.35/src/aws_sso_magic/configure.py
+-rw-r--r--   0        0        0     3295 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/src/aws_sso_magic/eks.py
+-rw-r--r--   0        0        0    14045 2023-05-29 03:01:35.091273 aws_sso_magic-1.0.35/src/aws_sso_magic/login.py
+-rw-r--r--   0        0        0     1979 2023-05-26 21:49:42.952441 aws_sso_magic-1.0.35/src/aws_sso_magic/logout.py
+-rw-r--r--   0        0        0    28511 2023-05-29 03:28:37.447896 aws_sso_magic-1.0.35/src/aws_sso_magic/utils.py
+-rw-r--r--   0        0        0     6985 1970-01-01 00:00:00.000000 aws_sso_magic-1.0.35/PKG-INFO
```

### Comparing `aws-sso-magic-1.0.34/LICENSE` & `aws_sso_magic-1.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/README.md` & `aws_sso_magic-1.0.35/README.md`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/pyproject.toml` & `aws_sso_magic-1.0.35/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-sso-magic"
-version = "1.0.34" # change in aws_sso_magic/__init__.py too
+version = "1.0.35" # change in aws_sso_magic/__init__.py too
 description = "Magic credentials on the AWS CLI home using AWS SSO login"
 authors = ["Javier Ortiz <jahor2@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/javiortizmol/aws-sso-magic"
 repository = "https://github.com/javiortizmol/aws-sso-magic"
 classifiers = [
```

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/__main__.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/cli.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/configure.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/configure.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/eks.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/eks.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/login.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,19 +104,20 @@
     configure_logging(LOGGER, verbose)
     _check_flag_combinations(eks, profile_arg, cluster_arg, eks_profile_arg, custom_profile_arg)
     _check_aws_v2()
 
     missing = []
 
     try:
-        instance = get_instance(
+        instance, sso_session_selected = get_instance(
             sso_start_url,
             sso_region,
             sso_start_url_vars=CONFIGURE_DEFAULT_START_URL_VARS,
-            sso_region_vars=CONFIGURE_DEFAULT_SSO_REGION_VARS,)
+            sso_region_vars=CONFIGURE_DEFAULT_SSO_REGION_VARS,
+            profile_name=profile_arg)
     except GetInstanceError as e:
         LOGGER.fatal(str(e))
         sys.exit(1)
 
     if not regions:
         for var_name in CONFIGURE_DEFAULT_REGION_VARS:
             value = os.environ.get(var_name)
@@ -295,15 +296,15 @@
 
     default_profile = True
 
     _create_credentials_profile(configs)
 
     if not eks:
         if profile_arg == None:
-            profile_name = _add_prefix(get_config_profile_list())
+            profile_name = _add_prefix(get_config_profile_list(sso_session_selected))
         else:
             profile_name = _add_prefix(profile_arg)
         if custom_profile_arg != None:
             default_profile = False
         _set_profile_credentials(profile_name, default_profile, custom_profile_arg)
         _set_profile_in_use(profile_name)
     else:
```

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/logout.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/logout.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.34/src/aws_sso_magic/utils.py` & `aws_sso_magic-1.0.35/src/aws_sso_magic/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import boto3
+import botocore
+from typing import Optional
 import hashlib
 import json
 import logging
 import logging.handlers
 import os
 import re
 import subprocess
@@ -27,14 +29,15 @@
 from configparser import ConfigParser
 from dateutil.tz import UTC, tzlocal
 from dateutil.parser import parse
 from aws_sso_lib.compat import shell_join
 from aws_sso_lib.config import find_instances, SSOInstance
 from botocore.compat import compat_shell_split as shell_split
 from aws_sso_lib.config_file_writer import process_profile_name
+from botocore.exceptions import ProfileNotFound
 
 AWS_CONFIG_PATH = f'{Path.home()}/.aws/config'
 AWS_CREDENTIAL_PATH = f'{Path.home()}/.aws/credentials'
 AWS_SSO_CACHE_PATH = f'{Path.home()}/.aws/sso/cache'
 AWS_SSO_PROFILE = "aws-sso"
 AWS_SSO_DIR = f".{AWS_SSO_PROFILE}-magic"
 AWS_SSO_CONFIG_PATH = f'{Path.home()}/{AWS_SSO_DIR}/config'
@@ -104,38 +107,66 @@
         aws_sso_magic_logger.setLevel(logging.DEBUG)
         aws_sso_lib_logger.setLevel(logging.DEBUG)
         root_logger.setLevel(logging.DEBUG)
 
 class GetInstanceError(Exception):
     pass
 
-def get_instance(sso_start_url, sso_region, sso_start_url_vars=None, sso_region_vars=None):
+def get_sso_sessions():
+    sso_sessions = []
+    config = _read_config(AWS_CONFIG_PATH)
+    for section in config.sections():
+        if "sso-session" in section:
+            section_name = _get_section_name(section, "sso-session ")
+            sso_sessions.append(section_name)
+    sso_sessions.sort()
+    questions = [{
+        'type': 'list',
+        'name': 'name',
+        'message': 'Please select an AWS SSO profile',
+        'choices': sso_sessions
+    }]
+
+    answer = prompt(questions)    
+    return answer.get('name')
+
+def get_sso_details(profile_name):
+    config_sso_profile = _read_section_configuration(AWS_CONFIG_PATH, f"sso-session {profile_name}")
+    sso_start_url = config_sso_profile.get("sso_start_url")
+    sso_region = config_sso_profile.get("sso_region")
+    print(f"sso_region: {sso_region}")
+    add_new_key_value_conf_file(AWS_CONFIG_PATH, f"profile {profile_name}", "sso_start_url", sso_start_url)
+    add_new_key_value_conf_file(AWS_CONFIG_PATH, f"profile {profile_name}", "sso_region", sso_region)
+    return sso_start_url, sso_region
+
+def get_instance(sso_start_url, sso_region, sso_start_url_vars=None, sso_region_vars=None, profile_name=None):
+    profile_name = get_sso_sessions()
+    sso_start_url, sso_region = get_sso_details(profile_name)
     instances, specifier, all_instances = find_instances(
-        profile_name=None,
+        profile_name=profile_name,
         profile_source=None,
         start_url=sso_start_url,
         start_url_source="CLI input",
         region=sso_region,
         region_source="CLI input",
         start_url_vars=sso_start_url_vars,
         region_vars=sso_region_vars
     )
-
     if not instances:
         if all_instances:
             raise GetInstanceError(
                 f"No AWS SSO instance matched {specifier.to_str(region=True)} " +
                 f"from {SSOInstance.to_strs(all_instances)}")
         else:
             raise GetInstanceError("No AWS SSO instance found, run aws-sso-magic configure")
 
     if len(instances) > 1:
         raise GetInstanceError(f"Found {len(instances)} SSO instance, please specify one: {SSOInstance.to_strs(instances)}")
 
-    return instances[0]
+    return instances[0], profile_name
 
 class Printer:
     def __init__(self, *,
             separator,
             default_separator,
             header_fields,
             disable_header=False,
@@ -338,40 +369,51 @@
             kwargs["role_name"] = re.sub(pattern, "", kwargs["role_name"])
         return formatter(i, n, **kwargs)
     return trim_formatter
 
 def get_safe_account_name(name):
     return re.sub(r"[\s\[\]]+", "-", name).strip("-")
 
+def _get_section_name(section_name, string_to_seach):
+    section = str(section_name).replace(string_to_seach,'')
+    return section 
+
 def _get_profile_name(profile):
     profile = str(profile).replace('profile ','')
     return profile 
 
-def _select_profile():
-    config = _read_config(AWS_CONFIG_PATH)
-
+def _profile_filter(sso_session):
     profiles = []
+    config = _read_config(AWS_CONFIG_PATH)
+    config_sso_profile = _read_section_configuration(AWS_CONFIG_PATH, f"sso-session {sso_session}")
+    sso_start_url_selected = config_sso_profile.get("sso_start_url")
     for section in config.sections():
-        x = _get_profile_name(section)
-        profiles.append(x)
+        profile = _read_section_configuration(AWS_CONFIG_PATH, f"profile {sso_session}")
+        if sso_start_url_selected in profile.get("sso_start_url"):
+            if sso_session not in section and "aws-sso" not in section and "default" not in section:
+                x = _get_profile_name(section)
+                profiles.append(x)
     profiles.sort()
+    return profiles
 
+def _select_profile(sso_session):
+    profiles = _profile_filter(sso_session)
     questions = [{
         'type': 'list',
         'name': 'name',
         'message': 'Please select an AWS config profile',
         'choices': profiles
     }]
 
     answer = prompt(questions)
     return answer['name'] if answer else sys.exit(1)
 
-def get_config_profile_list():
+def get_config_profile_list(sso_session):
     configure_logging(LOGGER, False)
-    answer = _select_profile()
+    answer = _select_profile(sso_session)
     return answer
 
 def _get_account_id_profile(path, profile_name):
     profile_name = f"profile {profile_name}"
     config = _read_section_configuration(path, profile_name)
     key_list = list(config.keys())
     val_list = list(config.values())
@@ -708,8 +750,14 @@
 
         # Add content to the file
         Config = ConfigParser()
         Config.add_section(AWS_SSO_DEFAULT_PROXY_ROLE_SECTION)
         Config.set(AWS_SSO_DEFAULT_PROXY_ROLE_SECTION, AWS_SSO_DEFAULT_PROXY_ROLE_KEY, proxy_role_name)
         Config.write(cfgfile)
         cfgfile.close()
-        print(f"{configfile_name} file created")
+        print(f"{configfile_name} file created")
+
+def add_new_key_value_conf_file(configfile_name, section_name, key, value):
+    config = _read_config(configfile_name)
+    config.set(section_name, key, value)
+    _write_config(configfile_name, config)
+
```

### Comparing `aws-sso-magic-1.0.34/setup.py` & `aws_sso_magic-1.0.35/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,150 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aws-sso-magic
+Version: 1.0.35
+Summary: Magic credentials on the AWS CLI home using AWS SSO login
+Home-page: https://github.com/javiortizmol/aws-sso-magic
+License: Apache-2.0
+Author: Javier Ortiz
+Author-email: jahor2@gmail.com
+Requires-Python: >=3.6,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: PyInquirer (>=1.0.3,<2.0.0)
+Requires-Dist: aws-error-utils (>=1.0.4,<2.0.0)
+Requires-Dist: aws-sso-lib (>=1.7.0,<2.0.0)
+Requires-Dist: boto3 (>=1.17.20,<2.0.0)
+Requires-Dist: click (>=7.1.2,<8.0.0)
+Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
+Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
+Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
+Project-URL: Repository, https://github.com/javiortizmol/aws-sso-magic
+Description-Content-Type: text/markdown
+
+#
+# aws-sso-magic tool cli 
+This tool update the aws credentials file for the default profile from the aws sso login.
+
+This solution mixed the following repositories:
+
+1. [aws-sso-util](https://github.com/benkehoe/aws-sso-util) AWS SSO has some rough edges, and aws-sso-util is here to smooth them out, hopefully temporarily until AWS makes it better.
+2. [aws-sso-credentials](https://github.com/NeilJed/aws-sso-credentials) A simple Python tool to simplify getting short-term credential tokens for CLI/Boto3 operations when using AWS SSO.
+
+### Content of the repository
+
+- [src](src) - The main folder with the aws_sso_magic folder with the .py files & the requirements.txt.
+    - [aws_sso_magic](src/aws_sso_magic)
+- [docker-build.sh](cli/docker-build.sh) - A docker build tool (Linux/MacOS) to build the docker image locally.
+    ```bash
+    sudo ./docker-build.sh
+    ```     
+- [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    
+- [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.
+- [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).
+    ```bash
+    eks-login develop-readonly
+    ```
+NOTE: I got this interesting repo of [marianonamoroso](https://github.com/marianonamoroso), He developed an awesome shell script to get information from the eks cluster, for more details click on https://github.com/marianonamoroso/kubernetes, and heyy give to him an star :).
+#
+## Installation 
+### Using pyp installer
+#### - Prerequisites
+1. [Python 3.9](https://www.python.org/downloads/) installed.
+2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.
+
+#### - Installation
+
+1. Follow the pyp [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) project instructions to install it.
+
+    Note: If you want upgrade it, please run this `pip install aws-sso-magic --upgrade`
+
+### Using Docker
+
+1. Please follow the instructions from the docker hub repository of [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)
+
+#
+## Configuration Instructions
+These steps will create the config files on the paths $HOME/.aws and $HOME/.aws-sso-magic.
+
+1. Execute the following command to configure the sso tool: `aws-sso-magic configure`
+2. Type the following information:
+    - SSO start URL
+    - SSO Region
+    - Select the default profile of SSO
+    - CLI default client Region
+    - CLI default output format
+    - CLI profile name. Eg: default
+    - Enter only the name of the proxy role to use by default. Eg: MyAdminRole or just press Enter (This option will mandatory for the --eks flag)
+3. Optional: In case that you want to set an account alias, you can modify the file on $HOME/.aws-sso-magic/config adding the [AliasAccounts] section with key (account name) and value (alias account) Eg:
+    ```
+    [AliasAccounts]
+    test1 = dev
+    test2 = qa
+    test3 = staging
+    test4 = prod
+    ```
+    making the above configuration, it will now show the aliases in the profile selection menu when aws-sso-magic login command is executed.
+    ```
+    [?] Please select an AWS config profile:    
+      aws-sso
+      default
+      dev-admin
+    > qa-admin 
+      staging-admin   
+      prod-admin
+    ```
+
+#
+## How to use it
+
+1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`
+2. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-magic login --profile ssoprofile` if you already know the profile name.
+
+NOTE: If you don't want to copy the credentials to the default profile, you can use the --custom-profile flag to create the profile with the name that you prefer and copy the credentials there. 
+Eg: `aws-sso-magic login --profile ssoprofile --custom-profile myprofile`
+
+
+## How to use it for eks support
+### - Prerequisites
+1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.
+2. `aws-sso-magic login` or `aws-sso-magic login --profile myprofile` executed previouly.
+
+### - Instructions
+1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.
+    ```
+    [default-proxy-role-name]
+    proxy_role_name = replacethis    
+    ```
+
+    or just add the profile section in the file. Eg:
+
+    ```
+    [myprofile]
+    proxy_role_name = myrolename
+    ```
+2. Execute the following command to select and log the eks cluster: `aws-sso-magic login --eks` or if you have configured an aws account as trusted entity having granted to assume roles on the rest of the accounts from there, please execute `aws-sso-magic login` selecting profile (account and role configured as trusted identity) and then execute `aws-sso-magic login --eks --eks-profile env-eks-profile`. Eg:
+    ```
+    aws-sso-magic login --profile main-admin
+    aws-sso-magic login --eks --eks-profile qa-admin
+    ```
+3. Please select the EKS cluster or send the cluster name using the flag --cluster. Eg: `aws-sso-magic login --eks --cluster myekscluster`
+4. Copy and paste the commands according to your OS.
+    
+    NOTE: If you will select another profile, please first unset the AWS_PROFILE environment variable or close this terminal and open a new one
+#
+## Links
+### - pypi.org
+- [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) 
+### - [Docker Hub](https://hub.docker.com/u/javiortizmol)
+- [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['aws_sso_magic']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyInquirer>=1.0.3,<2.0.0',
- 'aws-error-utils>=1.0.4,<2.0.0',
- 'aws-sso-lib>=1.7.0,<2.0.0',
- 'boto3>=1.17.20,<2.0.0',
- 'click>=7.1.2,<8.0.0',
- 'jsonschema>=3.2.0,<4.0.0',
- 'python-dateutil>=2.8.1,<3.0.0',
- 'pyyaml>=5.3.1,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['aws-sso-magic = aws_sso_magic.cli:cli']}
-
-setup_kwargs = {
-    'name': 'aws-sso-magic',
-    'version': '1.0.34',
-    'description': 'Magic credentials on the AWS CLI home using AWS SSO login',
-    'long_description': '#\n# aws-sso-magic tool cli \nThis tool update the aws credentials file for the default profile from the aws sso login.\n\nThis solution mixed the following repositories:\n\n1. [aws-sso-util](https://github.com/benkehoe/aws-sso-util) AWS SSO has some rough edges, and aws-sso-util is here to smooth them out, hopefully temporarily until AWS makes it better.\n2. [aws-sso-credentials](https://github.com/NeilJed/aws-sso-credentials) A simple Python tool to simplify getting short-term credential tokens for CLI/Boto3 operations when using AWS SSO.\n\n### Content of the repository\n\n- [src](src) - The main folder with the aws_sso_magic folder with the .py files & the requirements.txt.\n    - [aws_sso_magic](src/aws_sso_magic)\n- [docker-build.sh](cli/docker-build.sh) - A docker build tool (Linux/MacOS) to build the docker image locally.\n    ```bash\n    sudo ./docker-build.sh\n    ```     \n- [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    \n- [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.\n- [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).\n    ```bash\n    eks-login develop-readonly\n    ```\nNOTE: I got this interesting repo of [marianonamoroso](https://github.com/marianonamoroso), He developed an awesome shell script to get information from the eks cluster, for more details click on https://github.com/marianonamoroso/kubernetes, and heyy give to him an star :).\n#\n## Installation \n### Using pyp installer\n#### - Prerequisites\n1. [Python 3.9](https://www.python.org/downloads/) installed.\n2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.\n\n#### - Installation\n\n1. Follow the pyp [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) project instructions to install it.\n\n    Note: If you want upgrade it, please run this `pip install aws-sso-magic --upgrade`\n\n### Using Docker\n\n1. Please follow the instructions from the docker hub repository of [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n\n#\n## Configuration Instructions\nThese steps will create the config files on the paths $HOME/.aws and $HOME/.aws-sso-magic.\n\n1. Execute the following command to configure the sso tool: `aws-sso-magic configure`\n2. Type the following information:\n    - SSO start URL\n    - SSO Region\n    - Select the default profile of SSO\n    - CLI default client Region\n    - CLI default output format\n    - CLI profile name. Eg: default\n    - Enter only the name of the proxy role to use by default. Eg: MyAdminRole or just press Enter (This option will mandatory for the --eks flag)\n3. Optional: In case that you want to set an account alias, you can modify the file on $HOME/.aws-sso-magic/config adding the [AliasAccounts] section with key (account name) and value (alias account) Eg:\n    ```\n    [AliasAccounts]\n    test1 = dev\n    test2 = qa\n    test3 = staging\n    test4 = prod\n    ```\n    making the above configuration, it will now show the aliases in the profile selection menu when aws-sso-magic login command is executed.\n    ```\n    [?] Please select an AWS config profile:    \n      aws-sso\n      default\n      dev-admin\n    > qa-admin \n      staging-admin   \n      prod-admin\n    ```\n\n#\n## How to use it\n\n1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`\n2. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-magic login --profile ssoprofile` if you already know the profile name.\n\nNOTE: If you don\'t want to copy the credentials to the default profile, you can use the --custom-profile flag to create the profile with the name that you prefer and copy the credentials there. \nEg: `aws-sso-magic login --profile ssoprofile --custom-profile myprofile`\n\n\n## How to use it for eks support\n### - Prerequisites\n1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.\n2. `aws-sso-magic login` or `aws-sso-magic login --profile myprofile` executed previouly.\n\n### - Instructions\n1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.\n    ```\n    [default-proxy-role-name]\n    proxy_role_name = replacethis    \n    ```\n\n    or just add the profile section in the file. Eg:\n\n    ```\n    [myprofile]\n    proxy_role_name = myrolename\n    ```\n2. Execute the following command to select and log the eks cluster: `aws-sso-magic login --eks` or if you have configured an aws account as trusted entity having granted to assume roles on the rest of the accounts from there, please execute `aws-sso-magic login` selecting profile (account and role configured as trusted identity) and then execute `aws-sso-magic login --eks --eks-profile env-eks-profile`. Eg:\n    ```\n    aws-sso-magic login --profile main-admin\n    aws-sso-magic login --eks --eks-profile qa-admin\n    ```\n3. Please select the EKS cluster or send the cluster name using the flag --cluster. Eg: `aws-sso-magic login --eks --cluster myekscluster`\n4. Copy and paste the commands according to your OS.\n    \n    NOTE: If you will select another profile, please first unset the AWS_PROFILE environment variable or close this terminal and open a new one\n#\n## Links\n### - pypi.org\n- [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) \n### - [Docker Hub](https://hub.docker.com/u/javiortizmol)\n- [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n',
-    'author': 'Javier Ortiz',
-    'author_email': 'jahor2@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/javiortizmol/aws-sso-magic',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

