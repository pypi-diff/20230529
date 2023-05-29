# Comparing `tmp/aws-sso-magic-1.0.29.tar.gz` & `tmp/aws-sso-magic-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-sso-magic-1.0.29.tar", max compression
+gzip compressed data, was "aws-sso-magic-1.0.34.tar", max compression
```

## Comparing `aws-sso-magic-1.0.29.tar` & `aws-sso-magic-1.0.34.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11346 2021-06-22 02:55:44.720000 aws-sso-magic-1.0.29/LICENSE
--rw-r--r--   0        0        0     5071 2021-07-12 20:09:57.890179 aws-sso-magic-1.0.29/README.md
--rw-r--r--   0        0        0     1065 2021-07-27 13:59:45.857936 aws-sso-magic-1.0.29/pyproject.toml
--rw-r--r--   0        0        0       54 2021-07-27 13:59:51.023929 aws-sso-magic-1.0.29/src/aws_sso_magic/__init__.py
--rw-r--r--   0        0        0      641 2021-06-22 02:13:29.196918 aws-sso-magic-1.0.29/src/aws_sso_magic/__main__.py
--rw-r--r--   0        0        0     1108 2021-06-28 17:39:48.229449 aws-sso-magic-1.0.29/src/aws_sso_magic/cli.py
--rw-r--r--   0        0        0     1553 2021-07-12 18:25:17.542189 aws-sso-magic-1.0.29/src/aws_sso_magic/configure.py
--rw-r--r--   0        0        0     3295 2021-07-12 18:04:23.868143 aws-sso-magic-1.0.29/src/aws_sso_magic/eks.py
--rw-r--r--   0        0        0    13716 2021-07-08 04:05:59.295355 aws-sso-magic-1.0.29/src/aws_sso_magic/login.py
--rw-r--r--   0        0        0     1979 2021-06-22 01:42:55.984383 aws-sso-magic-1.0.29/src/aws_sso_magic/logout.py
--rw-r--r--   0        0        0    26019 2021-07-27 03:31:52.873365 aws-sso-magic-1.0.29/src/aws_sso_magic/utils.py
--rw-r--r--   0        0        0     6255 2021-07-27 14:00:11.649047 aws-sso-magic-1.0.29/setup.py
--rw-r--r--   0        0        0     6340 2021-07-27 14:00:11.649790 aws-sso-magic-1.0.29/PKG-INFO
+-rw-r--r--   0        0        0    11346 2021-08-02 00:31:09.532292 aws-sso-magic-1.0.34/LICENSE
+-rw-r--r--   0        0        0     5614 2021-08-04 00:41:19.946408 aws-sso-magic-1.0.34/README.md
+-rw-r--r--   0        0        0     1088 2021-08-04 00:41:46.708390 aws-sso-magic-1.0.34/pyproject.toml
+-rw-r--r--   0        0        0       54 2021-08-04 00:41:49.770166 aws-sso-magic-1.0.34/src/aws_sso_magic/__init__.py
+-rw-r--r--   0        0        0      641 2021-08-02 00:31:09.533729 aws-sso-magic-1.0.34/src/aws_sso_magic/__main__.py
+-rw-r--r--   0        0        0     1108 2021-08-02 00:31:09.533871 aws-sso-magic-1.0.34/src/aws_sso_magic/cli.py
+-rw-r--r--   0        0        0     1553 2021-08-02 00:31:09.534026 aws-sso-magic-1.0.34/src/aws_sso_magic/configure.py
+-rw-r--r--   0        0        0     3295 2021-08-02 00:31:09.534194 aws-sso-magic-1.0.34/src/aws_sso_magic/eks.py
+-rw-r--r--   0        0        0    13966 2021-08-02 00:31:09.534387 aws-sso-magic-1.0.34/src/aws_sso_magic/login.py
+-rw-r--r--   0        0        0     1979 2021-08-02 00:31:09.534626 aws-sso-magic-1.0.34/src/aws_sso_magic/logout.py
+-rw-r--r--   0        0        0    26297 2021-08-02 00:31:09.534912 aws-sso-magic-1.0.34/src/aws_sso_magic/utils.py
+-rw-r--r--   0        0        0     6804 2021-08-04 00:43:43.280332 aws-sso-magic-1.0.34/setup.py
+-rw-r--r--   0        0        0     6883 2021-08-04 00:43:43.280970 aws-sso-magic-1.0.34/PKG-INFO
```

### Comparing `aws-sso-magic-1.0.29/LICENSE` & `aws-sso-magic-1.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/README.md` & `aws-sso-magic-1.0.34/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     sudo ./docker-build.sh
     ```     
 - [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    
 - [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.
 - [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).
     ```bash
     eks-login develop-readonly
-    ```     
+    ```
+NOTE: I got this interesting repo of [marianonamoroso](https://github.com/marianonamoroso), He developed an awesome shell script to get information from the eks cluster, for more details click on https://github.com/marianonamoroso/kubernetes, and heyy give to him an star :).
 #
 ## Installation 
 ### Using pyp installer
 #### - Prerequisites
 1. [Python 3.9](https://www.python.org/downloads/) installed.
 2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.
 
@@ -70,20 +71,24 @@
       prod-admin
     ```
 
 #
 ## How to use it
 
 1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`
-3. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-login login --profile myprofile` if you already know the profile name.
+2. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-magic login --profile ssoprofile` if you already know the profile name.
+
+NOTE: If you don't want to copy the credentials to the default profile, you can use the --custom-profile flag to create the profile with the name that you prefer and copy the credentials there. 
+Eg: `aws-sso-magic login --profile ssoprofile --custom-profile myprofile`
+
 
 ## How to use it for eks support
 ### - Prerequisites
 1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.
-2. `aws-sso-magic login` or `aws-sso-login login --profile myprofile` executed previouly.
+2. `aws-sso-magic login` or `aws-sso-magic login --profile myprofile` executed previouly.
 
 ### - Instructions
 1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.
     ```
     [default-proxy-role-name]
     proxy_role_name = replacethis    
     ```
```

### Comparing `aws-sso-magic-1.0.29/pyproject.toml` & `aws-sso-magic-1.0.34/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-sso-magic"
-version = "1.0.29" # change in aws_sso_magic/__init__.py too
+version = "1.0.34" # change in aws_sso_magic/__init__.py too
 description = "Magic credentials on the AWS CLI home using AWS SSO login"
 authors = ["Javier Ortiz <jahor2@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/javiortizmol/aws-sso-magic"
 repository = "https://github.com/javiortizmol/aws-sso-magic"
 classifiers = [
@@ -30,9 +30,9 @@
 aws-sso-lib = "^1.7.0"
 PyInquirer = "^1.0.3"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.5.2"
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=0.12", "setuptools", "wheel"]
 build-backend = "poetry.masonry.api"
```

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/__main__.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/__main__.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/cli.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/cli.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/configure.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/configure.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/eks.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/eks.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/login.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from .utils import generate_profile_name_format, get_formatter, get_process_formatter
 from .utils import get_trim_formatter, get_safe_account_name, get_config_profile_list
 from .utils import _set_profile_credentials, _add_prefix, _set_profile_in_use
 from .utils import (
     AWS_SSO_CONFIG_ALIAS,
     AWS_SSO_CONFIG_PATH,
     AWS_DEFAULT_REGION,
-    AWS_SSO_PROFILE,
     VERBOSE
 )
 
 LOGGER = logging.getLogger(__name__)
 
 DEFAULT_SEPARATOR = "."
 UTC_TIME_FORMAT = "%Y-%m-%d %H:%M UTC"
@@ -51,14 +50,15 @@
 LOGIN_ALL_VAR = "AWS_SSO_LOGIN_ALL"
 
 ConfigParams = namedtuple("ConfigParams", ["profile_name", "account_name", "account_id", "role_name", "region"])
 
 @click.command()
 @click.option("--eks", is_flag=True, help="The flag to use for the update-kubeconfig")
 @click.option("--profile", "profile_arg", help="The main profile name to use")
+@click.option("--custom-profile", "custom_profile_arg", help="The profile name to copy the aws sso credentials")
 @click.option("--eks-profile", "eks_profile_arg", help="The eks profile name to use")
 @click.option("--cluster", "cluster_arg", help="The eks cluster name to use, this argument is only allowed using the --eks flag")
 @click.option("--sso-start-url", "-u", metavar="URL", help="Your AWS SSO start URL")
 @click.option("--sso-region", help="The AWS region your AWS SSO instance is deployed in")
 @click.option("--region", "-r", "regions", multiple=True, metavar="REGION", help="AWS region for the profiles, can provide multiple times")
 @click.option("--dry-run", is_flag=True, help="Print the config to stdout instead of writing to your config file")
 @click.option("--config-default", "-c", multiple=True, metavar="KEY=VALUE", help="Additional config field to set, can provide multiple times")
@@ -73,14 +73,15 @@
 @click.option("--safe-account-names/--raw-account-names", default=True, help="In profiles, replace any character sequences not in A-Za-z0-9-._ with a single -")
 @click.option("--force-refresh", is_flag=True, help="Re-login")
 @click.option("--verbose", "-v", count=True)
 
 def login(
         eks,
         profile_arg,
+        custom_profile_arg,
         eks_profile_arg,
         cluster_arg,
         sso_start_url,
         sso_region,    
         regions,
         dry_run,
         config_default,
@@ -97,15 +98,15 @@
         verbose):
     """Log in to the AWS SSO instance.
 
     Note this only needs to be done once for a given SSO instance (i.e., start URL),
     as all profiles sharing the same start URL will share the same login.
     """
     configure_logging(LOGGER, verbose)
-    _check_flag_combinations(eks, profile_arg, cluster_arg, eks_profile_arg)
+    _check_flag_combinations(eks, profile_arg, cluster_arg, eks_profile_arg, custom_profile_arg)
     _check_aws_v2()
 
     missing = []
 
     try:
         instance = get_instance(
             sso_start_url,
@@ -288,23 +289,25 @@
                 continue
             config_values[k] = v
         LOGGER.debug("Config values for profile {}: {}".format(config.profile_name, config_values))
         write_config(config.profile_name, config_values)
 
     global VERBOSE
 
-    default_profile = 'default'
+    default_profile = True
 
     _create_credentials_profile(configs)
 
     if not eks:
         if profile_arg == None:
-            profile = _add_prefix(get_config_profile_list())
+            profile_name = _add_prefix(get_config_profile_list())
         else:
-            profile = _add_prefix(profile_arg)
-        _set_profile_credentials(profile, default_profile)
-        _set_profile_in_use(profile)
+            profile_name = _add_prefix(profile_arg)
+        if custom_profile_arg != None:
+            default_profile = False
+        _set_profile_credentials(profile_name, default_profile, custom_profile_arg)
+        _set_profile_in_use(profile_name)
     else:
         _eks_cluster_configuration(cluster_arg, eks_profile_arg)
 
 if __name__ == "__main__":
     login(prog_name="python -m aws_sso_magic.login")  #pylint: disable=unexpected-keyword-arg,no-value-for-parameter
```

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/logout.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/logout.py`

 * *Files identical despite different names*

### Comparing `aws-sso-magic-1.0.29/src/aws_sso_magic/utils.py` & `aws-sso-magic-1.0.34/src/aws_sso_magic/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 AWS_SSO_DIR = f".{AWS_SSO_PROFILE}-magic"
 AWS_SSO_CONFIG_PATH = f'{Path.home()}/{AWS_SSO_DIR}/config'
 AWS_SSO_DEFAULT_PROXY_ROLE_SECTION="default-proxy-role-name"
 AWS_SSO_DEFAULT_PROXY_ROLE_KEY="proxy_role_name"
 AWS_SSO_PROFILE_IN_USE = "ProfileInUse"
 AWS_SSO_CONFIG_ALIAS = "AliasAccounts"
 AWS_SSO_EKS_ROLE_NAME_DEFAULT = "replacethis"
+AWS_DEFAULT_PROFILE = 'default'
 AWS_DEFAULT_REGION = 'us-east-1'
 VERBOSE = True
 
 KNOWN_COMPONENTS = [
     "account_name",
     "account_id",
     "account_number",
@@ -211,17 +212,19 @@
             self.printer(self._sep.join(just(row_to_print)))
 
             prev_row = row
             first_loop = False
 
 # Check Utils
 
-def _check_flag_combinations(eks, profile_arg, cluster_arg, eks_profile_arg):
+def _check_flag_combinations(eks, profile_arg, cluster_arg, eks_profile_arg, custom_profile_arg):
     if eks and profile_arg != None:
-        _print_error(f"\nERROR: Not use the flag combination --eks --profile")    
+        _print_error(f"\nERROR: Not use the flag combination --eks --profile") 
+    if eks and custom_profile_arg != None:
+        _print_error(f"\nERROR: Not use the flag combination --eks --custom-profile")             
     if not eks and cluster_arg != None:
         _print_error(f"\nERROR: Not use the flag combination login --cluster")
     if not eks and eks_profile_arg != None:
         _print_error(f"\nERROR: Not use the flag combination login --eks-profile")                      
 
 def _check_kubectl():
     try:
@@ -405,25 +408,25 @@
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
-def _set_profile_credentials(profile_name, default_profile):
+def _set_profile_credentials(profile_name, default_profile, custom_profile_name):
     profile_opts = _get_aws_profile(profile_name)
     cache_login = _get_sso_cached_login(profile_opts)
     credentials = _get_sso_role_credentials(profile_opts, cache_login)
-    if default_profile == 'default':
-        _store_aws_credentials(default_profile, profile_opts, credentials)
+    if default_profile == True:
+        _store_aws_credentials(AWS_DEFAULT_PROFILE, profile_opts, credentials)
         _store_aws_credentials(AWS_SSO_PROFILE, profile_opts, credentials)
         _copy_to_default_profile(profile_name)
         _copy_to_aws_sso_profile(profile_name)
     else:
-        _store_aws_credentials(profile_name, profile_opts, credentials)
+        _store_aws_credentials(custom_profile_name, profile_opts, credentials)
 
 def _get_role_arn(profile_name, role_name):
     account_id = _get_account_id_profile(AWS_CONFIG_PATH, profile_name)
     role_arn = f"arn:aws:iam::{account_id}:role/{role_name}"
     return role_arn
 
 def _get_role_name(profile_name, origin_request = "main"):
@@ -503,22 +506,22 @@
     print("\nCredentials copied successfully") 
 
 def _copy_to_default_profile(profile_name):
     print(f"\nCopying profile [{profile_name}] to [default]")
 
     config = _read_config(AWS_CONFIG_PATH)
 
-    if config.has_section('default'):
-        config.remove_section('default')
+    if config.has_section(AWS_DEFAULT_PROFILE):
+        config.remove_section(AWS_DEFAULT_PROFILE)
 
-    config.add_section('default')
+    config.add_section(AWS_DEFAULT_PROFILE)
 
     for key, value in config.items(profile_name):
         if key != "role_arn" and key != "source_profile" :
-            config.set('default', key, value)
+            config.set(AWS_DEFAULT_PROFILE, key, value)
 
     _write_config(AWS_CONFIG_PATH, config)
     print("\nCredentials copied successfully") 
 
 def _get_aws_profile(profile_name):
     print(f'\nReading profile: [{profile_name}]')
     config = _read_config(AWS_CONFIG_PATH)
@@ -578,15 +581,15 @@
     config.set(profile_name, "region", region)
     config.set(profile_name, "aws_access_key_id", credentials["accessKeyId"])
     config.set(profile_name, "aws_secret_access_key ", credentials["secretAccessKey"])
     config.set(profile_name, "aws_session_token", credentials["sessionToken"])
     _write_config(AWS_CREDENTIAL_PATH, config)
 
 def _add_prefix(name):
-    return f'profile {name}' if name != 'default' else 'default'
+    return f'profile {name}' if name != AWS_DEFAULT_PROFILE else AWS_DEFAULT_PROFILE
 
 def _print_colour(colour, message, always=False):
     if always or VERBOSE:
         if os.environ.get('CLI_NO_COLOR', False):
             print(message)
         else:
             print(''.join([colour, message, Colour.ENDC]))
```

### Comparing `aws-sso-magic-1.0.29/setup.py` & `aws-sso-magic-1.0.34/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'pyyaml>=5.3.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['aws-sso-magic = aws_sso_magic.cli:cli']}
 
 setup_kwargs = {
     'name': 'aws-sso-magic',
-    'version': '1.0.29',
+    'version': '1.0.34',
     'description': 'Magic credentials on the AWS CLI home using AWS SSO login',
-    'long_description': '#\n# aws-sso-magic tool cli \nThis tool update the aws credentials file for the default profile from the aws sso login.\n\nThis solution mixed the following repositories:\n\n1. [aws-sso-util](https://github.com/benkehoe/aws-sso-util) AWS SSO has some rough edges, and aws-sso-util is here to smooth them out, hopefully temporarily until AWS makes it better.\n2. [aws-sso-credentials](https://github.com/NeilJed/aws-sso-credentials) A simple Python tool to simplify getting short-term credential tokens for CLI/Boto3 operations when using AWS SSO.\n\n### Content of the repository\n\n- [src](src) - The main folder with the aws_sso_magic folder with the .py files & the requirements.txt.\n    - [aws_sso_magic](src/aws_sso_magic)\n- [docker-build.sh](cli/docker-build.sh) - A docker build tool (Linux/MacOS) to build the docker image locally.\n    ```bash\n    sudo ./docker-build.sh\n    ```     \n- [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    \n- [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.\n- [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).\n    ```bash\n    eks-login develop-readonly\n    ```     \n#\n## Installation \n### Using pyp installer\n#### - Prerequisites\n1. [Python 3.9](https://www.python.org/downloads/) installed.\n2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.\n\n#### - Installation\n\n1. Follow the pyp [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) project instructions to install it.\n\n    Note: If you want upgrade it, please run this `pip install aws-sso-magic --upgrade`\n\n### Using Docker\n\n1. Please follow the instructions from the docker hub repository of [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n\n#\n## Configuration Instructions\nThese steps will create the config files on the paths $HOME/.aws and $HOME/.aws-sso-magic.\n\n1. Execute the following command to configure the sso tool: `aws-sso-magic configure`\n2. Type the following information:\n    - SSO start URL\n    - SSO Region\n    - Select the default profile of SSO\n    - CLI default client Region\n    - CLI default output format\n    - CLI profile name. Eg: default\n    - Enter only the name of the proxy role to use by default. Eg: MyAdminRole or just press Enter (This option will mandatory for the --eks flag)\n3. Optional: In case that you want to set an account alias, you can modify the file on $HOME/.aws-sso-magic/config adding the [AliasAccounts] section with key (account name) and value (alias account) Eg:\n    ```\n    [AliasAccounts]\n    test1 = dev\n    test2 = qa\n    test3 = staging\n    test4 = prod\n    ```\n    making the above configuration, it will now show the aliases in the profile selection menu when aws-sso-magic login command is executed.\n    ```\n    [?] Please select an AWS config profile:    \n      aws-sso\n      default\n      dev-admin\n    > qa-admin \n      staging-admin   \n      prod-admin\n    ```\n\n#\n## How to use it\n\n1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`\n3. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-login login --profile myprofile` if you already know the profile name.\n\n## How to use it for eks support\n### - Prerequisites\n1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.\n2. `aws-sso-magic login` or `aws-sso-login login --profile myprofile` executed previouly.\n\n### - Instructions\n1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.\n    ```\n    [default-proxy-role-name]\n    proxy_role_name = replacethis    \n    ```\n\n    or just add the profile section in the file. Eg:\n\n    ```\n    [myprofile]\n    proxy_role_name = myrolename\n    ```\n2. Execute the following command to select and log the eks cluster: `aws-sso-magic login --eks` or if you have configured an aws account as trusted entity having granted to assume roles on the rest of the accounts from there, please execute `aws-sso-magic login` selecting profile (account and role configured as trusted identity) and then execute `aws-sso-magic login --eks --eks-profile env-eks-profile`. Eg:\n    ```\n    aws-sso-magic login --profile main-admin\n    aws-sso-magic login --eks --eks-profile qa-admin\n    ```\n3. Please select the EKS cluster or send the cluster name using the flag --cluster. Eg: `aws-sso-magic login --eks --cluster myekscluster`\n4. Copy and paste the commands according to your OS.\n    \n    NOTE: If you will select another profile, please first unset the AWS_PROFILE environment variable or close this terminal and open a new one\n#\n## Links\n### - pypi.org\n- [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) \n### - [Docker Hub](https://hub.docker.com/u/javiortizmol)\n- [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n',
+    'long_description': '#\n# aws-sso-magic tool cli \nThis tool update the aws credentials file for the default profile from the aws sso login.\n\nThis solution mixed the following repositories:\n\n1. [aws-sso-util](https://github.com/benkehoe/aws-sso-util) AWS SSO has some rough edges, and aws-sso-util is here to smooth them out, hopefully temporarily until AWS makes it better.\n2. [aws-sso-credentials](https://github.com/NeilJed/aws-sso-credentials) A simple Python tool to simplify getting short-term credential tokens for CLI/Boto3 operations when using AWS SSO.\n\n### Content of the repository\n\n- [src](src) - The main folder with the aws_sso_magic folder with the .py files & the requirements.txt.\n    - [aws_sso_magic](src/aws_sso_magic)\n- [docker-build.sh](cli/docker-build.sh) - A docker build tool (Linux/MacOS) to build the docker image locally.\n    ```bash\n    sudo ./docker-build.sh\n    ```     \n- [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    \n- [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.\n- [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).\n    ```bash\n    eks-login develop-readonly\n    ```\nNOTE: I got this interesting repo of [marianonamoroso](https://github.com/marianonamoroso), He developed an awesome shell script to get information from the eks cluster, for more details click on https://github.com/marianonamoroso/kubernetes, and heyy give to him an star :).\n#\n## Installation \n### Using pyp installer\n#### - Prerequisites\n1. [Python 3.9](https://www.python.org/downloads/) installed.\n2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.\n\n#### - Installation\n\n1. Follow the pyp [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) project instructions to install it.\n\n    Note: If you want upgrade it, please run this `pip install aws-sso-magic --upgrade`\n\n### Using Docker\n\n1. Please follow the instructions from the docker hub repository of [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n\n#\n## Configuration Instructions\nThese steps will create the config files on the paths $HOME/.aws and $HOME/.aws-sso-magic.\n\n1. Execute the following command to configure the sso tool: `aws-sso-magic configure`\n2. Type the following information:\n    - SSO start URL\n    - SSO Region\n    - Select the default profile of SSO\n    - CLI default client Region\n    - CLI default output format\n    - CLI profile name. Eg: default\n    - Enter only the name of the proxy role to use by default. Eg: MyAdminRole or just press Enter (This option will mandatory for the --eks flag)\n3. Optional: In case that you want to set an account alias, you can modify the file on $HOME/.aws-sso-magic/config adding the [AliasAccounts] section with key (account name) and value (alias account) Eg:\n    ```\n    [AliasAccounts]\n    test1 = dev\n    test2 = qa\n    test3 = staging\n    test4 = prod\n    ```\n    making the above configuration, it will now show the aliases in the profile selection menu when aws-sso-magic login command is executed.\n    ```\n    [?] Please select an AWS config profile:    \n      aws-sso\n      default\n      dev-admin\n    > qa-admin \n      staging-admin   \n      prod-admin\n    ```\n\n#\n## How to use it\n\n1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`\n2. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-magic login --profile ssoprofile` if you already know the profile name.\n\nNOTE: If you don\'t want to copy the credentials to the default profile, you can use the --custom-profile flag to create the profile with the name that you prefer and copy the credentials there. \nEg: `aws-sso-magic login --profile ssoprofile --custom-profile myprofile`\n\n\n## How to use it for eks support\n### - Prerequisites\n1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.\n2. `aws-sso-magic login` or `aws-sso-magic login --profile myprofile` executed previouly.\n\n### - Instructions\n1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.\n    ```\n    [default-proxy-role-name]\n    proxy_role_name = replacethis    \n    ```\n\n    or just add the profile section in the file. Eg:\n\n    ```\n    [myprofile]\n    proxy_role_name = myrolename\n    ```\n2. Execute the following command to select and log the eks cluster: `aws-sso-magic login --eks` or if you have configured an aws account as trusted entity having granted to assume roles on the rest of the accounts from there, please execute `aws-sso-magic login` selecting profile (account and role configured as trusted identity) and then execute `aws-sso-magic login --eks --eks-profile env-eks-profile`. Eg:\n    ```\n    aws-sso-magic login --profile main-admin\n    aws-sso-magic login --eks --eks-profile qa-admin\n    ```\n3. Please select the EKS cluster or send the cluster name using the flag --cluster. Eg: `aws-sso-magic login --eks --cluster myekscluster`\n4. Copy and paste the commands according to your OS.\n    \n    NOTE: If you will select another profile, please first unset the AWS_PROFILE environment variable or close this terminal and open a new one\n#\n## Links\n### - pypi.org\n- [aw-sso-magic](https://pypi.org/project/aws-sso-magic/) \n### - [Docker Hub](https://hub.docker.com/u/javiortizmol)\n- [aws_sso_magic](https://hub.docker.com/r/javiortizmol/aws_sso_magic)\n',
     'author': 'Javier Ortiz',
     'author_email': 'jahor2@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/javiortizmol/aws-sso-magic',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `aws-sso-magic-1.0.29/PKG-INFO` & `aws-sso-magic-1.0.34/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-sso-magic
-Version: 1.0.29
+Version: 1.0.34
 Summary: Magic credentials on the AWS CLI home using AWS SSO login
 Home-page: https://github.com/javiortizmol/aws-sso-magic
 License: Apache-2.0
 Author: Javier Ortiz
 Author-email: jahor2@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,16 @@
     sudo ./docker-build.sh
     ```     
 - [pyproject.toml](pyproject.toml) - The metadata file with the dependencies and application information.    
 - [Dockerfile](Dockerfile) - The docker file with the instructions to build the aws-sso-magic cli.
 - [eks-login](utils/eks-login) - A script tool to add on the /usr/local/bin (Only for linux/macOS or Windows WSL).
     ```bash
     eks-login develop-readonly
-    ```     
+    ```
+NOTE: I got this interesting repo of [marianonamoroso](https://github.com/marianonamoroso), He developed an awesome shell script to get information from the eks cluster, for more details click on https://github.com/marianonamoroso/kubernetes, and heyy give to him an star :).
 #
 ## Installation 
 ### Using pyp installer
 #### - Prerequisites
 1. [Python 3.9](https://www.python.org/downloads/) installed.
 2. [AWS CLI v2](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed, please click on the link depending of your OS.
 
@@ -101,20 +102,24 @@
       prod-admin
     ```
 
 #
 ## How to use it
 
 1. Execute the following command to select and log into the aws accounts: `aws-sso-magic login`
-3. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-login login --profile myprofile` if you already know the profile name.
+2. Execute the following command to log: `aws-sso-magic login` and select the profile to use or `aws-sso-magic login --profile ssoprofile` if you already know the profile name.
+
+NOTE: If you don't want to copy the credentials to the default profile, you can use the --custom-profile flag to create the profile with the name that you prefer and copy the credentials there. 
+Eg: `aws-sso-magic login --profile ssoprofile --custom-profile myprofile`
+
 
 ## How to use it for eks support
 ### - Prerequisites
 1. [kubectl](https://kubernetes.io/docs/tasks/tools/) installed.
-2. `aws-sso-magic login` or `aws-sso-login login --profile myprofile` executed previouly.
+2. `aws-sso-magic login` or `aws-sso-magic login --profile myprofile` executed previouly.
 
 ### - Instructions
 1. Go to the file $HOME/.aws-sso-magic/config and replace the string "replacethis" on the section default-proxy-role-name if you want to use that role name for all profiles.
     ```
     [default-proxy-role-name]
     proxy_role_name = replacethis    
     ```
```

