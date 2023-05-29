# Comparing `tmp/cycode-0.2.4.dev8.tar.gz` & `tmp/cycode-0.2.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.4.dev8.tar", max compression
+gzip compressed data, was "cycode-0.2.5.dev1.tar", max compression
```

## Comparing `cycode-0.2.4.dev8.tar` & `cycode-0.2.5.dev1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    31536 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/README.md
--rw-r--r--   0        0        0      102 2023-05-15 10:12:10.664827 cycode-0.2.4.dev8/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47714 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.yaml
--rw-r--r--   0        0        0     4994 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2191 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2931 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     6734 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/main.py
--rw-r--r--   0        0        0     1106 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/models.py
--rw-r--r--   0        0        0      195 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      356 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0      982 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1068 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/results_printer.py
--rw-r--r--   0        0        0     5670 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     8749 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4348 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6470 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2054 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      910 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1217 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      865 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     2706 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1596 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     8126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     1893 2023-05-15 10:12:10.660827 cycode-0.2.4.dev8/pyproject.toml
--rw-r--r--   0        0        0    33354 1970-01-01 00:00:00.000000 cycode-0.2.4.dev8/PKG-INFO
+-rw-r--r--   0        0        0    32320 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/README.md
+-rw-r--r--   0        0        0      115 2023-05-29 11:33:04.228289 cycode-0.2.5.dev1/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2191 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2931 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     6734 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      564 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1709 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-05-29 11:32:39.811962 cycode-0.2.5.dev1/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5813 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9166 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4348 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6470 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      910 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1229 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     2706 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     8126 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-05-29 11:32:39.815962 cycode-0.2.5.dev1/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     1990 2023-05-29 11:33:04.224288 cycode-0.2.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev1/PKG-INFO
```

### Comparing `cycode-0.2.4.dev8/README.md` & `cycode-0.2.5.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     3. [Ignoring a Path](#ignoring-a-path)
     4. [Ignoring a Secret, IaC, or SCA Rule](#ignoring-a-secret-iac-sca-or-sast-rule)
     5. [Ignoring a Package](#ignoring-a-package)
 7. [Syntax Help](#syntax-help)
 
 # Prerequisites
 
-- The Cycode CLI application requires Python version 3.8 or later.
+- The Cycode CLI application requires Python version 3.7 or later.
 - Use the [`cycode auth` command](#use-auth-command) to authenticate to Cycode with the CLI
   - Alternatively, a Cycode Client ID and Client Secret Key can be acquired using the steps from the [Service Account Token](https://docs.cycode.com/reference/creating-a-service-account-access-token) and [Personal Access Token](https://docs.cycode.com/reference/creating-a-personal-access-token-1) pages for details on obtaining these values.
 
 # Installation
 
 The following installation steps are applicable on both Windows and UNIX / Linux operating systems.
 
@@ -82,32 +82,32 @@
 
 1. Type the following command into your terminal/command line window:
 
    `cycode auth`
 
 2. A browser window will appear, asking you to log into Cycode (as seen below):
 
-![](./images/cycode_login.png)
+![Cycode login](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/cycode_login.png)
 
 3. Enter you login credentials on this page and log in.
 
 4. You will eventually be taken to this page, where you will be asked to choose the business group you want to authorize Cycode with (if applicable):
 
-![](./images/authorize_cli.png)
+![authorize CLI](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/authorize_cli.png)
 
 > :memo: **Note**<br/>
 > This will be the default method for authenticating with the Cycode CLI.
 
 5. Click the **Allow** button to authorize the Cycode CLI on the chosen business group.
 
-![](./images/allow_cli.png)
+![allow CLI](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/allow_cli.png)
 
 6. Once done, you will see the following screen, if it was successfully selected:
 
-![](./images/successfully_auth.png)
+![successfully auth](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/successfully_auth.png)
 
 7. In the terminal/command line screen, you will see the following when exiting the browser window:
 
   ```bash
   Successfully logged into cycode
   ```
 
@@ -156,27 +156,27 @@
 export CYCODE_CLIENT_SECRET={your Cycode Secret Key}
 ```
 
 #### On Windows
 
 1. From the Control Panel, navigate to the System menu:
 
-![](./images/image1.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image1.png)
 
 2. Next, click Advanced system settings:
 
-![](./images/image2.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image2.png)
 
 3. In the System Properties window that opens, click the Environment Variables button:
 
-![](./images/image3.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image3.png)
 
 4. Create `CYCODE_CLIENT_ID` and `CYCODE_CLIENT_SECRET` variables with values matching your ID and Secret Key, respectively:
 
-![](./images/image4.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image4.png)
 
 ## Install Pre-Commit Hook
 
 Cycode’s pre-commit hook can be set up within your local repository so that the Cycode CLI application will automatically identify any issues with your code before you commit it to your codebase.
 
 Perform the following steps to install the pre-commit hook:
 
@@ -187,15 +187,15 @@
 2. Navigate to the top directory of the local repository you wish to scan.
 
 3. Create a new YAML file named `.pre-commit-config.yaml` (include the beginning `.`) in the repository’s top directory that contains the following:
 
 ```yaml
 repos:
   - repo: https://github.com/cycodehq-public/cycode-cli
-    rev: 0.2.3
+    rev: stable
     hooks:
       - id: cycode
         language_version: python3
         stages:
           - commit
 ```
 
@@ -207,19 +207,20 @@
 > Successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode Command
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option            | Description                 |
-|-------------------|-----------------------------|
-| `-v`, `--verbose` | Show detailed logs          |
-| `--version`       | Show the version and exit.  |
-| `--help`          | Show options for given command. |
+| Option                  | Description                                               |
+|-------------------------|-----------------------------------------------------------|
+| `--output [text\|json]` | Specify the output (`text`/`json`). The default is `text` |
+| `-v`, `--verbose`       | Show detailed logs                                        |
+| `--version`             | Show the version and exit.                                |
+| `--help`                | Show options for given command.                           |
 
 | Command                             | Description |
 |-------------------------------------|-------------|
 | [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
 | [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
 | [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
 | [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
@@ -231,15 +232,14 @@
 | Option                               | Description                                                                |
 |--------------------------------------|----------------------------------------------------------------------------|
 | `-t, --scan-type [secret\|iac\|sca\|sast]` | Specify the scan you wish to execute (`secret`/`iac`/`sca`/`sast`), the default is `secret` |
 | `--secret TEXT`                      | Specify a Cycode client secret for this specific scan execution |
 | `--client-id TEXT`                   | Specify a Cycode client ID for this specific scan execution   |
 | `--show-secret BOOLEAN`              | Show secrets in plain text. See [Show/Hide Secrets](#showhide-secrets) section for more details. |
 | `--soft-fail BOOLEAN`                | Run scan without failing, always return a non-error status code. See [Soft Fail](#soft-fail) section for more details. |
-| `--output [text\|json]`              | Specify the results output (`text`/`json`). The default is `text` |
 | `--severity-threshold [INFO\|LOW\|MEDIUM\|HIGH\|CRITICAL]`  | Show only violations at the specified level or higher (supported for the SCA scan type only). |
 | `--sca-scan`                         | Specify the SCA scan you wish to execute (`package-vulnerabilities`/`license-compliance`). The default is both |
 | `--monitor`                          | When specified, the scan results will be recorded in the knowledge graph. Please note that when working in `monitor` mode, the knowledge graph will not be updated as a result of SCM events (Push, Repo creation). (Supported for SCA scan type only). |
 | `--report`                           | When specified, a violations report will be generated. A URL link to the report will be printed as an output to the command execution |
 | `--help`                             | Show options for given command.                                                |
 
 | Command                                | Description                                                     |
@@ -356,15 +356,15 @@
 3 | cleo==1.0.0a5
 
 Report URL: https://app.cycode.com/on-demand-scans/617ecc3d-9ff2-493e-8be8-2c1fecaf6939
 ```
 
 The report page will look something like below:
 
-![](./images/scan_details.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/scan_details.png)
 
 ## Package Vulnerabilities Option
 
 > :memo: **Note**<br/>
 > This option is only available to SCA scans.
 
 To scan a specific package vulnerability of your local repository, add the argument `--sca-scan package-vulnerabilities` following the `-t sca` or `--scan-type sca` option.
@@ -694,8 +694,8 @@
 
 For example, to see options available for a Path Scan, you would simply enter:
 
 `cycode scan path --help`
 
 To see the options available for the ignore scan function, use this command:
 
-`cycode ignore --help`
+`cycode ignore --help`
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/auth/auth_command.py` & `cycode-0.2.5.dev1/cycode/cli/auth/auth_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import json
-
 import click
 import traceback
 
+from cycode.cli.models import CliResult, CliErrors, CliError
+from cycode.cli.printers import ConsolePrinter
 from cycode.cli.auth.auth_manager import AuthManager
 from cycode.cli.user_settings.credentials_manager import CredentialsManager
 from cycode.cli.exceptions.custom_exceptions import AuthProcessError, NetworkError, HttpUnauthorizedError
 from cycode.cyclient import logger
 from cycode.cyclient.cycode_token_based_client import CycodeTokenBasedClient
 
 
@@ -15,65 +15,64 @@
 def authenticate(context: click.Context):
     """ Authenticates your machine to associate CLI with your cycode account """
     if context.invoked_subcommand is not None:
         # if it is a subcommand do nothing
         return
 
     try:
-        logger.debug("starting authentication process")
+        logger.debug('Starting authentication process')
+
         auth_manager = AuthManager()
         auth_manager.authenticate()
-        click.echo("Successfully logged into cycode")
+
+        result = CliResult(success=True, message='Successfully logged into cycode')
+        ConsolePrinter(context).print_result(result)
     except Exception as e:
         _handle_exception(context, e)
 
 
 @authenticate.command(name='check')
 @click.pass_context
 def authorization_check(context: click.Context):
     """ Check your machine associating CLI with your cycode account """
-    passed_auth_check_args = {'context': context, 'content': {
-        'success': True,
-        'message': 'You are authorized'
-    }, 'color': 'green'}
-    failed_auth_check_args = {'context': context, 'content': {
-        'success': False,
-        'message': 'You are not authorized'
-    }, 'color': 'red'}
+    printer = ConsolePrinter(context)
+
+    passed_auth_check_res = CliResult(success=True, message='You are authorized')
+    failed_auth_check_res = CliResult(success=False, message='You are not authorized')
 
     client_id, client_secret = CredentialsManager().get_credentials()
     if not client_id or not client_secret:
-        return _print_result(**failed_auth_check_args)
+        return printer.print_result(failed_auth_check_res)
 
     try:
-        # TODO(MarshalX): This property performs HTTP request to refresh the token. This must be the method.
         if CycodeTokenBasedClient(client_id, client_secret).api_token:
-            return _print_result(**passed_auth_check_args)
+            return printer.print_result(passed_auth_check_res)
     except (NetworkError, HttpUnauthorizedError):
         if context.obj['verbose']:
             click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
 
-        return _print_result(**failed_auth_check_args)
-
-
-def _print_result(context: click.Context, content: dict, color: str) -> None:
-    # the current impl of printers supports only results of scans
-    if context.obj['output'] == 'text':
-        return click.secho(content['message'], fg=color)
-
-    return click.echo(json.dumps({'result': content['success'], 'message': content['message']}))
+        return printer.print_result(failed_auth_check_res)
 
 
 def _handle_exception(context: click.Context, e: Exception):
-    verbose = context.obj["verbose"]
-    if verbose:
+    if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
-    if isinstance(e, AuthProcessError):
-        click.secho('Authentication failed. Please try again later using the command `cycode auth`',
-                    fg='red', nl=False)
-    elif isinstance(e, NetworkError):
-        click.secho('Authentication failed. Please try again later using the command `cycode auth`',
-                    fg='red', nl=False)
-    elif isinstance(e, click.ClickException):
+
+    errors: CliErrors = {
+        AuthProcessError: CliError(
+            code='auth_error',
+            message='Authentication failed. Please try again later using the command `cycode auth`'
+        ),
+        NetworkError: CliError(
+            code='cycode_error',
+            message='Authentication failed. Please try again later using the command `cycode auth`'
+        ),
+    }
+
+    error = errors.get(type(e))
+    if error:
+        return ConsolePrinter(context).print_error(error)
+
+    if isinstance(e, click.ClickException):
         raise e
-    else:
-        raise click.ClickException(str(e))
+
+    raise click.ClickException(str(e))
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py` & `cycode-0.2.5.dev1/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/ci_integrations.py` & `cycode-0.2.5.dev1/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/code_scanner.py` & `cycode-0.2.5.dev1/cycode/cli/code_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import Type, NamedTuple
-
 import click
 import json
 import logging
 import os
 import sys
 import time
 import traceback
 from platform import platform
 from uuid import uuid4, UUID
 from git import Repo, NULL_TREE, InvalidGitRepositoryError
 from sys import getsizeof
 
 from halo import Halo
 
-from cycode.cli.printers import ResultsPrinter
-from cycode.cli.models import Document, DocumentDetections, Severity
+from cycode.cli.printers import ConsolePrinter
+from cycode.cli.models import Document, DocumentDetections, Severity, CliError, CliErrors
 from cycode.cli.ci_integrations import get_commit_range
 from cycode.cli.consts import *
 from cycode.cli.config import configuration_manager
 from cycode.cli.utils.path_utils import is_sub_path, is_binary_file, get_file_size, get_relevant_files_in_path, \
     get_path_by_os, get_file_content
 from cycode.cli.utils.string_utils import get_content_size, is_binary_content
 from cycode.cli.utils.task_timer import TimeoutAfter
@@ -442,22 +440,23 @@
 
 def print_scan_details(scan_details_response: ScanDetailsResponse):
     logger.info(f"Scan update: (scan_id: {scan_details_response.id})")
     logger.info(f"Scan status: {scan_details_response.scan_status}")
     if scan_details_response.message is not None:
         logger.info(f"Scan message: {scan_details_response.message}")
 
-def print_results(context: click.Context, document_detections_list: List[DocumentDetections]):
-    output_type = context.obj['output']
-    printer = ResultsPrinter()
-    printer.print_results(context, document_detections_list, output_type)
+
+def print_results(context: click.Context, document_detections_list: List[DocumentDetections]) -> None:
+    printer = ConsolePrinter(context)
+    printer.print_scan_results(document_detections_list)
 
 
-def enrich_scan_result(scan_result: ZippedFileScanResult, documents_to_scan: List[Document]) -> \
-        List[DocumentDetections]:
+def enrich_scan_result(
+        scan_result: ZippedFileScanResult, documents_to_scan: List[Document]
+) -> List[DocumentDetections]:
     logger.debug('enriching scan result')
     document_detections_list = []
     for detections_per_file in scan_result.detections_per_file:
         file_name = get_path_by_os(detections_per_file.file_name)
         commit_id = detections_per_file.commit_id
         logger.debug("going to find document of violated file, %s", {'file_name': file_name, 'commit_id': commit_id})
         document = _get_document_by_file_name(documents_to_scan, file_name, commit_id)
@@ -727,14 +726,22 @@
     if package_name == '':
         package_name = detection.detection_details.get('package_name', '')
         package_version = detection.detection_details.get('package_version', '')
 
     return f'{package_name}@{package_version}'
 
 
+def _is_file_relevant_for_sca_scan(filename: str) -> bool:
+    if any([sca_excluded_path in filename for sca_excluded_path in SCA_EXCLUDED_PATHS]):
+        logger.debug("file is irrelevant because it is from node_modules's inner path, %s",
+                     {'filename': filename})
+        return False
+    return True
+
+
 def _is_relevant_file_to_scan(scan_type: str, filename: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
         logger.debug("file is irrelevant because it is in cycode configuration directory, %s",
                      {'filename': filename})
         return False
 
     if _is_path_configured_in_exclusions(scan_type, filename):
@@ -752,14 +759,18 @@
                      {'filename': filename})
         return False
 
     if scan_type != SCA_SCAN_TYPE and _does_file_exceed_max_size_limit(filename):
         logger.debug("file is irrelevant because its exceeded max size limit, %s",
                      {'filename': filename})
         return False
+
+    if scan_type == SCA_SCAN_TYPE and not _is_file_relevant_for_sca_scan(filename):
+        return False
+
     return True
 
 
 def _is_relevant_document_to_scan(scan_type: str, filename: str, content: str) -> bool:
     if _is_subpath_of_cycode_configuration_folder(filename):
         logger.debug("document is irrelevant because it is in cycode configuration directory, %s",
                      {'filename': filename})
@@ -811,90 +822,72 @@
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
     return FILE_MAX_SIZE_LIMIT_IN_BYTES < get_content_size(content)
 
 
 def _is_subpath_of_cycode_configuration_folder(filename: str) -> bool:
     return is_sub_path(configuration_manager.global_config_file_manager.get_config_directory_path(), filename) \
-           or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename) \
-           or filename.endswith(ConfigFileManager.get_config_file_route())
-
-
-class CliScanError(NamedTuple):
-    soft_fail: bool
-    code: str
-    message: str
-
-
-CliScanErrors = Dict[Type[Exception], CliScanError]
+        or is_sub_path(configuration_manager.local_config_file_manager.get_config_directory_path(), filename) \
+        or filename.endswith(ConfigFileManager.get_config_file_route())
 
 
 def _handle_exception(context: click.Context, e: Exception):
     context.obj['did_fail'] = True
 
     if context.obj['verbose']:
         click.secho(f'Error: {traceback.format_exc()}', fg='red', nl=False)
 
-    # TODO(MarshalX): Create global CLI errors database and move this
-    errors: CliScanErrors = {
-        NetworkError: CliScanError(
+    errors: CliErrors = {
+        NetworkError: CliError(
             soft_fail=True,
             code='cycode_error',
             message='Cycode was unable to complete this scan. '
                     'Please try again by executing the `cycode scan` command'
         ),
-        ScanAsyncError: CliScanError(
+        ScanAsyncError: CliError(
             soft_fail=True,
             code='scan_error',
             message='Cycode was unable to complete this scan. '
                     'Please try again by executing the `cycode scan` command'
         ),
-        HttpUnauthorizedError: CliScanError(
+        HttpUnauthorizedError: CliError(
             soft_fail=True,
             code='auth_error',
             message='Unable to authenticate to Cycode, your token is either invalid or has expired. '
                     'Please re-generate your token and reconfigure it by running the `cycode configure` command'
         ),
-        ZipTooLargeError: CliScanError(
+        ZipTooLargeError: CliError(
             soft_fail=True,
             code='zip_too_large_error',
             message='The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
                     'Please try ignoring irrelevant paths using the ‘cycode ignore --by-path’ command '
                     'and execute the scan again'
         ),
-        InvalidGitRepositoryError: CliScanError(
+        InvalidGitRepositoryError: CliError(
             soft_fail=False,
             code='invalid_git_error',
             message='The path you supplied does not correlate to a git repository. '
                     'Should you still wish to scan this path, use: ‘cycode scan path <path>’'
         ),
     }
 
     if type(e) in errors:
         error = errors[type(e)]
 
         if error.soft_fail is True:
             context.obj['soft_fail'] = True
 
-        return _print_error(context, error)
+        return ConsolePrinter(context).print_error(error)
 
     if isinstance(e, click.ClickException):
         raise e
 
     raise click.ClickException(str(e))
 
 
-def _print_error(context: click.Context, error: CliScanError) -> None:
-    # TODO(MarshalX): Extend functionality of CLI printers and move this
-    if context.obj['output'] == 'text':
-        click.secho(error.message, fg='red', nl=False)
-    elif context.obj['output'] == 'json':
-        click.echo(json.dumps({'error': error.code, 'message': error.message}, ensure_ascii=False))
-
-
 def _report_scan_status(context: click.Context, scan_type: str, scan_id: str, scan_completed: bool,
                         output_detections_count: int, all_detections_count: int, files_to_scan_count: int,
                         zip_size: int, command_scan_type: str, error_message: Optional[str]):
     try:
         cycode_client = context.obj["client"]
         end_scan_time = time.time()
         scan_status = {
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/consts.py` & `cycode-0.2.5.dev1/cycode/cli/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     'packages.config', 'project.assets.json', 'packages.lock.json', 'nuget.config', '.csproj',
     'gemfile', 'gemfile.lock',
     'build.sbt', 'build.scala', 'build.sbt.lock',
     'pyproject.toml', 'poetry.lock',
     'pipfile', 'pipfile.lock', 'requirements.txt', 'setup.py'
 ]
 
+SCA_EXCLUDED_PATHS = [
+    'node_modules'
+]
+
 PROJECT_FILES_BY_ECOSYSTEM_MAP = {
     "crates": ["Cargo.lock", "Cargo.toml"],
     "composer": ["composer.json", "composer.lock"],
     "go": ["go.sum", "go.mod", "Gopkg.lock"],
     "maven_pom": ["pom.xml"],
     "maven_gradle": ["build.gradle", "build.gradle.kts", "gradle.lockfile"],
     "npm": ["package.json", "package-lock.json", "yarn.lock", "npm-shrinkwrap.json", ".npmrc"],
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.5.dev1/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.5.dev1/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.5.dev1/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.5.dev1/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.5.dev1/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/main.py` & `cycode-0.2.5.dev1/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/models.py` & `cycode-0.2.5.dev1/cycode/cli/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
-from typing import List
+from typing import List, NamedTuple, Dict, Type
+
 from cycode.cyclient.models import Detection
 
 
 class Document:
     def __init__(self, path: str, content: str, is_git_diff_format: bool = False, unique_id: str = None):
         self.path = path
         self.content = content
@@ -39,7 +40,21 @@
 
     @staticmethod
     def try_get_value(name: str) -> any:
         if name not in Severity.__members__:
             return None
 
         return Severity[name].value
+
+
+class CliError(NamedTuple):
+    code: str
+    message: str
+    soft_fail: bool = False
+
+
+CliErrors = Dict[Type[Exception], CliError]
+
+
+class CliResult(NamedTuple):
+    success: bool
+    message: str
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py` & `cycode-0.2.5.dev1/cycode/cli/printers/table_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,139 +1,162 @@
+from collections import defaultdict
 from typing import List, Dict
 
 import click
 from texttable import Texttable
 
-from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, \
-    PACKAGE_VULNERABILITY_POLICY_ID
-from cycode.cli.models import DocumentDetections, Detection
+from cycode.cli.consts import LICENSE_COMPLIANCE_POLICY_ID, PACKAGE_VULNERABILITY_POLICY_ID
+from cycode.cli.models import DocumentDetections, Detection, CliError, CliResult
 from cycode.cli.printers.base_printer import BasePrinter
 
 SEVERITY_COLUMN = 'Severity'
 LICENSE_COLUMN = 'License'
 UPGRADE_COLUMN = 'Upgrade'
 REPOSITORY_COLUMN = 'Repository'
-PREVIEW_DETECTIONS_COMMON_HEADERS = ['File Path', 'Ecosystem', 'Dependency Name',
-                                     'Direct Dependency',
-                                     'Development Dependency']
+CVE_COLUMN = 'CVE'
+
+PREVIEW_DETECTIONS_COMMON_HEADERS = [
+    'File Path',
+    'Ecosystem',
+    'Dependency Name',
+    'Direct Dependency',
+    'Development Dependency'
+]
 
 
 class TablePrinter(BasePrinter):
     RED_COLOR_NAME = 'red'
     WHITE_COLOR_NAME = 'white'
     GREEN_COLOR_NAME = 'green'
 
-    scan_id: str
-
     def __init__(self, context: click.Context):
         super().__init__(context)
         self.scan_id = context.obj.get('scan_id')
 
-    def print_results(self, results: List[DocumentDetections]):
+    def print_result(self, result: CliResult) -> None:
+        raise NotImplemented
+
+    def print_error(self, error: CliError) -> None:
+        raise NotImplemented
+
+    def print_scan_results(self, results: List[DocumentDetections]):
         click.secho(f"Scan Results: (scan_id: {self.scan_id})")
 
         if not results:
             click.secho("Good job! No issues were found!!! 👏👏👏", fg=self.GREEN_COLOR_NAME)
             return
 
         detections_per_detection_type_id = self._extract_detections_per_detection_type_id(results)
 
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
-        if self.context.obj.get('report_url'):
-            click.secho(f"Report URL: {self.context.obj.get('report_url')}")
-
-    def _extract_detections_per_detection_type_id(self, results: List[DocumentDetections]):
-        detections_per_detection_type_id = {}
+        report_url = self.context.obj.get('report_url')
+        if report_url:
+            click.secho(f'Report URL: {report_url}')
+
+    @staticmethod
+    def _extract_detections_per_detection_type_id(results: List[DocumentDetections]) -> Dict[str, List[Detection]]:
+        detections_per_detection_type_id = defaultdict(list)
 
         for document_detection in results:
             for detection in document_detection.detections:
-                if detection.detection_type_id not in detections_per_detection_type_id:
-                    detections_per_detection_type_id[detection.detection_type_id] = []
                 detections_per_detection_type_id[detection.detection_type_id].append(detection)
 
         return detections_per_detection_type_id
 
-    def _print_detection_per_detection_type_id(self, detections_per_detection_type_id: Dict[str, Detection]):
+    def _print_detection_per_detection_type_id(
+            self, detections_per_detection_type_id: Dict[str, List[Detection]]
+    ) -> None:
         for detection_type_id in detections_per_detection_type_id:
             detections = detections_per_detection_type_id[detection_type_id]
             headers = self._get_table_headers()
 
+            title = None
+            rows = []
+
             if detection_type_id == PACKAGE_VULNERABILITY_POLICY_ID:
                 title = "Dependencies Vulnerabilities"
+
                 headers = [SEVERITY_COLUMN] + headers
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
+                headers.append(CVE_COLUMN)
                 headers.append(UPGRADE_COLUMN)
-                rows = []
+
                 for detection in detections:
                     rows.append(self._get_upgrade_package_vulnerability(detection))
-
-            if detection_type_id == LICENSE_COMPLIANCE_POLICY_ID:
+            elif detection_type_id == LICENSE_COMPLIANCE_POLICY_ID:
                 title = "License Compliance"
+
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
                 headers.append(LICENSE_COLUMN)
-                rows = []
+
                 for detection in detections:
                     rows.append(self._get_license(detection))
 
-            if len(rows) > 0:
-                self._print_table_detections(detections,
-                                             headers,
-                                             rows,
-                                             title)
-
-    def _get_table_headers(self):
-        headers = [REPOSITORY_COLUMN] if self._is_git_repository() else []
-        return headers
+            if rows:
+                self._print_table_detections(detections, headers, rows, title)
+
+    def _get_table_headers(self) -> list:
+        if self._is_git_repository():
+            return [REPOSITORY_COLUMN]
+
+        return []
 
-    def _print_table_detections(self, detections: List[Detection], headers: List[str],
-                                rows, title: str):
+    def _print_table_detections(
+            self, detections: List[Detection], headers: List[str], rows, title: str
+    ) -> None:
         self._print_summary_issues(detections, title)
         text_table = Texttable()
         text_table.header(headers)
 
         self.set_table_width(headers, text_table)
+
         for row in rows:
             text_table.add_row(row)
+
         click.echo(text_table.draw())
 
-    def set_table_width(self, headers, text_table):
+    @staticmethod
+    def set_table_width(headers: List[str], text_table: Texttable) -> None:
         header_width_size_cols = []
         for header in headers:
             header_width_size_cols.append(len(header))
+
         text_table.set_cols_width(header_width_size_cols)
 
-    def _print_summary_issues(self, detections: List, title: str):
-        click.echo(
-            f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
+    @staticmethod
+    def _print_summary_issues(detections: List, title: str) -> None:
+        click.echo(f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
 
-    def _get_common_detection_fields(self, detection: Detection):
+    def _get_common_detection_fields(self, detection: Detection) -> List[str]:
         row = [
             detection.detection_details.get('file_name'),
             detection.detection_details.get('ecosystem'),
             detection.detection_details.get('package_name'),
             detection.detection_details.get('is_direct_dependency_str'),
-            detection.detection_details.get('is_dev_dependency_str')
+            detection.detection_details.get('is_dev_dependency_str'),
+            detection.detection_details.get('vulnerability_id')
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
 
-    def _is_git_repository(self):
+    def _is_git_repository(self) -> bool:
         return self.context.obj.get("remote_url") is not None
 
-    def _get_upgrade_package_vulnerability(self, detection: Detection):
+    def _get_upgrade_package_vulnerability(self, detection: Detection) -> List[str]:
         alert = detection.detection_details.get('alert')
-        row = [detection.detection_details.get('advisory_severity')]
-        row.extend(self._get_common_detection_fields(detection))
-        upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}' if alert.get(
-            "first_patched_version") is not None else ''
+        row = [detection.detection_details.get('advisory_severity')] + self._get_common_detection_fields(detection)
+
+        upgrade = ''
+        if alert.get("first_patched_version"):
+            upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
         row.append(upgrade)
 
         return row
 
-    def _get_license(self, detection: Detection):
+    def _get_license(self, detection: Detection) -> List[str]:
         row = self._get_common_detection_fields(detection)
         row.append(f'{detection.detection_details.get("license")}')
         return row
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py` & `cycode-0.2.5.dev1/cycode/cli/printers/text_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import math
 from typing import List, Optional
 
 import click
 
 from cycode.cli.printers.base_printer import BasePrinter
-from cycode.cli.models import DocumentDetections, Detection, Document
+from cycode.cli.models import DocumentDetections, Detection, Document, CliResult, CliError
 from cycode.cli.config import config
 from cycode.cli.consts import SECRET_SCAN_TYPE, COMMIT_RANGE_BASED_COMMAND_SCAN_TYPES
 from cycode.cli.utils.string_utils import obfuscate_text
 
 
 class TextPrinter(BasePrinter):
     RED_COLOR_NAME = 'red'
     WHITE_COLOR_NAME = 'white'
     GREEN_COLOR_NAME = 'green'
 
-    scan_id: str
-    scan_type: str
-    command_scan_type: str
-    show_secret: bool = False
-
     def __init__(self, context: click.Context):
         super().__init__(context)
-        self.scan_id = context.obj.get('scan_id')
-        self.scan_type = context.obj.get('scan_type')
-        self.command_scan_type = context.info_name
-        self.show_secret = context.obj.get('show_secret', False)
+        self.scan_id: str = context.obj.get('scan_id')
+        self.scan_type: str = context.obj.get('scan_type')
+        self.command_scan_type: str = context.info_name
+        self.show_secret: bool = context.obj.get('show_secret', False)
+
+    def print_result(self, result: CliResult) -> None:
+        color = None
+        if not result.success:
+            color = self.RED_COLOR_NAME
+
+        click.secho(result.message, fg=color)
 
-    def print_results(self, results: List[DocumentDetections]):
+    def print_error(self, error: CliError) -> None:
+        click.secho(error.message, fg=self.RED_COLOR_NAME, nl=False)
+
+    def print_scan_results(self, results: List[DocumentDetections]):
         click.secho(f"Scan Results: (scan_id: {self.scan_id})")
 
         if not results:
             click.secho("Good job! No issues were found!!! 👏👏👏", fg=self.GREEN_COLOR_NAME)
             return
 
         for document_detections in results:
             self._print_document_detections(document_detections)
 
-        if self.context.obj.get('report_url'):
-            click.secho(f"Report URL: {self.context.obj.get('report_url')}")
+        report_url = self.context.obj.get('report_url')
+        if report_url:
+            click.secho(f'Report URL: {report_url}')
 
     def _print_document_detections(self, document_detections: DocumentDetections):
         document = document_detections.document
         lines_to_display = self._get_lines_to_display_count()
         for detection in document_detections.detections:
             self._print_detection_summary(detection, document.path)
             self._print_detection_code_segment(detection, document, lines_to_display)
@@ -50,17 +56,18 @@
     def _print_detection_summary(self, detection: Detection, document_path: str):
         detection_name = detection.type if self.scan_type == SECRET_SCAN_TYPE else detection.message
         detection_sha = detection.detection_details.get('sha512')
         detection_sha_message = f'\nSecret SHA: {detection_sha}' if detection_sha else ''
         detection_commit_id = detection.detection_details.get('commit_id')
         detection_commit_id_message = f'\nCommit SHA: {detection_commit_id}' if detection_commit_id else ''
         click.echo(
-            f'⛔  Found issue of type: {click.style(detection_name, fg="bright_red", bold=True)} ' +
-            f'(rule ID: {detection.detection_rule_id}) in file: {click.format_filename(document_path)} ' +
-            f'{detection_sha_message}{detection_commit_id_message}  ⛔ ')
+            f'⛔  Found issue of type: {click.style(detection_name, fg="bright_red", bold=True)} '
+            f'(rule ID: {detection.detection_rule_id}) in file: {click.format_filename(document_path)} '
+            f'{detection_sha_message}{detection_commit_id_message}  ⛔'
+        )
 
     def _print_detection_code_segment(self, detection: Detection, document: Document, code_segment_size: int):
         if self._is_git_diff_based_scan():
             self._print_detection_from_git_diff(detection, document)
             return
 
         self._print_detection_from_file(detection, document, code_segment_size)
@@ -73,42 +80,51 @@
                                     detection_position_in_line: int, violation_length: int, is_detection_line: bool):
         if is_detection_line:
             self._print_detection_line(document, line, line_number, detection_position_in_line, violation_length)
         else:
             self._print_line(document, line, line_number)
 
     def _print_detection_line(self, document: Document, line: str, line_number: int, detection_position_in_line: int,
-                              violation_length: int):
+                              violation_length: int) -> None:
         click.echo(
             f'{self._get_line_number_style(line_number)} '
-            f'{self._get_detection_line_style(line, document.is_git_diff_format, detection_position_in_line, violation_length)}')
+            f'{self._get_detection_line_style(line, document.is_git_diff_format, detection_position_in_line, violation_length)}'
+        )
 
     def _print_line(self, document: Document, line: str, line_number: int):
-        click.echo(
-            f'{self._get_line_number_style(line_number)} {self._get_line_style(line, document.is_git_diff_format)}')
+        line_no = self._get_line_number_style(line_number)
+        line = self._get_line_style(line, document.is_git_diff_format)
 
-    def _get_detection_line_style(self, line: str, is_git_diff: bool, start_position: int, length: int):
+        click.echo(f'{line_no} {line}')
+
+    def _get_detection_line_style(self, line: str, is_git_diff: bool, start_position: int, length: int) -> str:
         line_color = self._get_line_color(line, is_git_diff)
         if self.scan_type != SECRET_SCAN_TYPE or start_position < 0 or length < 0:
             return self._get_line_style(line, is_git_diff, line_color)
 
         violation = line[start_position: start_position + length]
         if not self.show_secret:
             violation = obfuscate_text(violation)
+
         line_to_violation = line[0: start_position]
         line_from_violation = line[start_position + length:]
+
         return f'{self._get_line_style(line_to_violation, is_git_diff, line_color)}' \
                f'{self._get_line_style(violation, is_git_diff, line_color, underline=True)}' \
                f'{self._get_line_style(line_from_violation, is_git_diff, line_color)}'
 
-    def _get_line_style(self, line: str, is_git_diff: bool, color: Optional[str] = None, underline: bool = False):
-        color = color or self._get_line_color(line, is_git_diff)
+    def _get_line_style(
+            self, line: str, is_git_diff: bool, color: Optional[str] = None, underline: bool = False
+    ) -> str:
+        if color is None:
+            color = self._get_line_color(line, is_git_diff)
+
         return click.style(line, fg=color, bold=False, underline=underline)
 
-    def _get_line_color(self, line: str, is_git_diff: bool):
+    def _get_line_color(self, line: str, is_git_diff: bool) -> str:
         if not is_git_diff:
             return self.WHITE_COLOR_NAME
 
         if line.startswith('+'):
             return self.GREEN_COLOR_NAME
 
         if line.startswith('-'):
@@ -116,15 +132,16 @@
 
         return self.WHITE_COLOR_NAME
 
     def _get_position_in_line(self, text: str, position: int) -> int:
         return position - text.rfind('\n', 0, position) - 1
 
     def _get_line_number_style(self, line_number: int):
-        return f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} {click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
+        return f'{click.style(str(line_number), fg=self.WHITE_COLOR_NAME, bold=False)} ' \
+               f'{click.style("|", fg=self.RED_COLOR_NAME, bold=False)}'
 
     def _get_lines_to_display_count(self) -> int:
         result_printer_configuration = config.get('result_printer')
         lines_to_display_of_scan = result_printer_configuration.get(self.scan_type, {}) \
             .get(self.command_scan_type, {}).get('lines_to_display')
         if lines_to_display_of_scan:
             return lines_to_display_of_scan
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.5.dev1/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.5.dev1/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.5.dev1/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.5.dev1/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.5.dev1/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py` & `cycode-0.2.5.dev1/cycode/cli/utils/path_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,20 @@
     spec = pathspec.PathSpec.from_lines(pathspec.patterns.GitWildMatchPattern, exclude_patterns)
     exclude_file_paths = set(spec.match_files(file_paths))
 
     return [file_path for file_path in (file_paths - exclude_file_paths) if os.path.isfile(file_path)]
 
 
 def is_sub_path(path: str, sub_path: str) -> bool:
-    common_path = os.path.commonpath([get_absolute_path(path), get_absolute_path(sub_path)])
-    return path == common_path
+    try:
+        common_path = os.path.commonpath([get_absolute_path(path), get_absolute_path(sub_path)])
+        return path == common_path
+    except ValueError:
+        # if paths are on the different drives
+        return False
 
 
 def get_absolute_path(path: str) -> str:
     if path.startswith('~'):
         return os.path.expanduser(path)
     return os.path.abspath(path)
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py` & `cycode-0.2.5.dev1/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py` & `cycode-0.2.5.dev1/cycode/cli/utils/string_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 
     return f'{text[:start_reveled_len]}{obfuscated[start_reveled_len:end_reveled_len]}{text[end_reveled_len:]}'
 
 
 obfuscate_regex = re.compile(r"[^+\-\s]")
 
 
-"""
-get the first 1024 chars and check if its binary or not
-"""
-def is_binary_content(content: str):
+def is_binary_content(content: str) -> bool:
+    """Get the first 1024 chars and check if it's binary or not."""
     chunk = content[:1024]
     chunk_bytes = convert_string_to_bytes(chunk)
     return is_binary_string(chunk_bytes)
 
 
 def get_content_size(content: str):
     return getsizeof(content)
```

### Comparing `cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py` & `cycode-0.2.5.dev1/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.5.dev1/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cli/zip_file.py` & `cycode-0.2.5.dev1/cycode/cli/zip_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,27 @@
     def __init__(self):
         # Create the in-memory file-like object
         self.in_memory_zip = BytesIO()
         self.zip = ZipFile(self.in_memory_zip, "a", ZIP_DEFLATED, False)
 
     def append(self, filename, unique_id, content):
         # Write the file to the in-memory zip
-        filename = filename if unique_id is None else concat_unique_id(filename, unique_id)
+        if unique_id:
+            filename = concat_unique_id(filename, unique_id)
+
         self.zip.writestr(filename, content)
 
     def close(self):
         self.zip.close()
 
     # to bytes
     def read(self) -> bytes:
         self.in_memory_zip.seek(0)
         return self.in_memory_zip.read()
 
 
 def concat_unique_id(filename: str, unique_id: str) -> str:
-    return f'{unique_id}{filename}' if filename.startswith(os.sep) else os.path.join(unique_id, filename)
+    if filename.startswith(os.sep):
+        # remove leading slash to join path correctly
+        filename = filename[len(os.sep):]
+
+    return os.path.join(unique_id, filename)
```

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/auth_client.py` & `cycode-0.2.5.dev1/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/config.py` & `cycode-0.2.5.dev1/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.5.dev1/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.5.dev1/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.5.dev1/cycode/cyclient/cycode_token_based_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         self._api_token = None
         self._expires_in = None
 
         self.lock = Lock()
 
     @property
     def api_token(self) -> str:
+        # TODO(MarshalX): This property performs HTTP request to refresh the token. This must be the method.
         with self.lock:
             self.refresh_api_token_if_needed()
             return self._api_token
 
     def refresh_api_token_if_needed(self) -> None:
         if self._api_token is None or self._expires_in is None or arrow.utcnow() >= self._expires_in:
             self.refresh_api_token()
```

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/models.py` & `cycode-0.2.5.dev1/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/scan_client.py` & `cycode-0.2.5.dev1/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.5.dev1/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.5.dev1/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev8/pyproject.toml` & `cycode-0.2.5.dev1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.4.dev8" # placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.5.dev1" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
@@ -22,20 +22,19 @@
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.scripts]
 cycode = "cycode.cli.main:main_cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.7,<3.12"
 click = ">=8.1.0,<8.2.0"
 colorama = ">=0.4.3,<0.5.0"
 pyyaml = ">=6.0,<7.0"
 marshmallow = ">=3.8.0,<3.9.0"
-typing = ">=3.7.4.3,<3.8.0.0"
 pathspec = ">=0.8.0,<0.9.0"
 gitpython = ">=3.1.30,<3.2.0"
 arrow = ">=0.17.0,<0.18.0"
 binaryornot = ">=0.4.4,<0.5.0"
 halo = "==0.0.31"
 texttable = ">=1.6.7,<1.7.0"
 requests = ">=2.24,<3.0"
@@ -43,16 +42,20 @@
 [tool.poetry.group.test.dependencies]
 mock = ">=4.0.3,<4.1.0"
 pytest = ">=7.3.1,<7.4.0"
 pytest-mock = ">=3.10.0,<3.11.0"
 coverage = ">=7.2.3,<7.3.0"
 responses = ">=0.23.1,<0.24.0"
 
-# poetry self add "poetry-dynamic-versioning[plugin]"
+[tool.poetry.group.executable.dependencies]
+pyinstaller = ">=5.11.0,<5.12.0"
+dunamai = ">=1.16.1,<1.17.0"
+
 [tool.poetry-dynamic-versioning]
+# poetry self add "poetry-dynamic-versioning[plugin]"
 enable = false
 strict = true
 bump = true
 metadata = false
 vcs = "git"
 style = "pep440"
```

### Comparing `cycode-0.2.4.dev8/PKG-INFO` & `cycode-0.2.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.4.dev8
+Version: 0.2.5.dev1
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: arrow (>=0.17.0,<0.18.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: gitpython (>=3.1.30,<3.2.0)
 Requires-Dist: halo (==0.0.31)
 Requires-Dist: marshmallow (>=3.8.0,<3.9.0)
 Requires-Dist: pathspec (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.24,<3.0)
 Requires-Dist: texttable (>=1.6.7,<1.7.0)
-Requires-Dist: typing (>=3.7.4.3,<3.8.0.0)
 Project-URL: Repository, https://github.com/cycodehq-public/cycode-cli
 Description-Content-Type: text/markdown
 
 # Cycode CLI User Guide
 
 The Cycode Command Line Interface (CLI) is an application you can install on your local machine which can scan your locally stored repositories for any secrets or infrastructure as code misconfigurations.
 
@@ -85,15 +79,15 @@
     3. [Ignoring a Path](#ignoring-a-path)
     4. [Ignoring a Secret, IaC, or SCA Rule](#ignoring-a-secret-iac-sca-or-sast-rule)
     5. [Ignoring a Package](#ignoring-a-package)
 7. [Syntax Help](#syntax-help)
 
 # Prerequisites
 
-- The Cycode CLI application requires Python version 3.8 or later.
+- The Cycode CLI application requires Python version 3.7 or later.
 - Use the [`cycode auth` command](#use-auth-command) to authenticate to Cycode with the CLI
   - Alternatively, a Cycode Client ID and Client Secret Key can be acquired using the steps from the [Service Account Token](https://docs.cycode.com/reference/creating-a-service-account-access-token) and [Personal Access Token](https://docs.cycode.com/reference/creating-a-personal-access-token-1) pages for details on obtaining these values.
 
 # Installation
 
 The following installation steps are applicable on both Windows and UNIX / Linux operating systems.
 
@@ -125,32 +119,32 @@
 
 1. Type the following command into your terminal/command line window:
 
    `cycode auth`
 
 2. A browser window will appear, asking you to log into Cycode (as seen below):
 
-![](./images/cycode_login.png)
+![Cycode login](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/cycode_login.png)
 
 3. Enter you login credentials on this page and log in.
 
 4. You will eventually be taken to this page, where you will be asked to choose the business group you want to authorize Cycode with (if applicable):
 
-![](./images/authorize_cli.png)
+![authorize CLI](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/authorize_cli.png)
 
 > :memo: **Note**<br/>
 > This will be the default method for authenticating with the Cycode CLI.
 
 5. Click the **Allow** button to authorize the Cycode CLI on the chosen business group.
 
-![](./images/allow_cli.png)
+![allow CLI](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/allow_cli.png)
 
 6. Once done, you will see the following screen, if it was successfully selected:
 
-![](./images/successfully_auth.png)
+![successfully auth](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/successfully_auth.png)
 
 7. In the terminal/command line screen, you will see the following when exiting the browser window:
 
   ```bash
   Successfully logged into cycode
   ```
 
@@ -199,27 +193,27 @@
 export CYCODE_CLIENT_SECRET={your Cycode Secret Key}
 ```
 
 #### On Windows
 
 1. From the Control Panel, navigate to the System menu:
 
-![](./images/image1.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image1.png)
 
 2. Next, click Advanced system settings:
 
-![](./images/image2.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image2.png)
 
 3. In the System Properties window that opens, click the Environment Variables button:
 
-![](./images/image3.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image3.png)
 
 4. Create `CYCODE_CLIENT_ID` and `CYCODE_CLIENT_SECRET` variables with values matching your ID and Secret Key, respectively:
 
-![](./images/image4.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/image4.png)
 
 ## Install Pre-Commit Hook
 
 Cycode’s pre-commit hook can be set up within your local repository so that the Cycode CLI application will automatically identify any issues with your code before you commit it to your codebase.
 
 Perform the following steps to install the pre-commit hook:
 
@@ -230,15 +224,15 @@
 2. Navigate to the top directory of the local repository you wish to scan.
 
 3. Create a new YAML file named `.pre-commit-config.yaml` (include the beginning `.`) in the repository’s top directory that contains the following:
 
 ```yaml
 repos:
   - repo: https://github.com/cycodehq-public/cycode-cli
-    rev: 0.2.3
+    rev: stable
     hooks:
       - id: cycode
         language_version: python3
         stages:
           - commit
 ```
 
@@ -250,19 +244,20 @@
 > Successful hook installation will result in the message:<br/>
 `Pre-commit installed at .git/hooks/pre-commit`
 
 # Cycode Command
 
 The following are the options and commands available with the Cycode CLI application:
 
-| Option            | Description                 |
-|-------------------|-----------------------------|
-| `-v`, `--verbose` | Show detailed logs          |
-| `--version`       | Show the version and exit.  |
-| `--help`          | Show options for given command. |
+| Option                  | Description                                               |
+|-------------------------|-----------------------------------------------------------|
+| `--output [text\|json]` | Specify the output (`text`/`json`). The default is `text` |
+| `-v`, `--verbose`       | Show detailed logs                                        |
+| `--version`             | Show the version and exit.                                |
+| `--help`                | Show options for given command.                           |
 
 | Command                             | Description |
 |-------------------------------------|-------------|
 | [auth](#use-auth-command)           | Authenticates your machine to associate CLI with your Cycode account. |
 | [configure](#use-configure-command) | Initial command to authenticate your CLI client with Cycode using client ID and client secret. |
 | [ignore](#ingoring-scan-results)    | Ignore a specific value, path or rule ID |
 | [scan](#running-a-scan)             | Scan content for secrets/IaC/SCA/SAST violations. You need to specify which scan type: `ci`/`commit_history`/`path`/`repository`/etc |
@@ -274,15 +269,14 @@
 | Option                               | Description                                                                |
 |--------------------------------------|----------------------------------------------------------------------------|
 | `-t, --scan-type [secret\|iac\|sca\|sast]` | Specify the scan you wish to execute (`secret`/`iac`/`sca`/`sast`), the default is `secret` |
 | `--secret TEXT`                      | Specify a Cycode client secret for this specific scan execution |
 | `--client-id TEXT`                   | Specify a Cycode client ID for this specific scan execution   |
 | `--show-secret BOOLEAN`              | Show secrets in plain text. See [Show/Hide Secrets](#showhide-secrets) section for more details. |
 | `--soft-fail BOOLEAN`                | Run scan without failing, always return a non-error status code. See [Soft Fail](#soft-fail) section for more details. |
-| `--output [text\|json]`              | Specify the results output (`text`/`json`). The default is `text` |
 | `--severity-threshold [INFO\|LOW\|MEDIUM\|HIGH\|CRITICAL]`  | Show only violations at the specified level or higher (supported for the SCA scan type only). |
 | `--sca-scan`                         | Specify the SCA scan you wish to execute (`package-vulnerabilities`/`license-compliance`). The default is both |
 | `--monitor`                          | When specified, the scan results will be recorded in the knowledge graph. Please note that when working in `monitor` mode, the knowledge graph will not be updated as a result of SCM events (Push, Repo creation). (Supported for SCA scan type only). |
 | `--report`                           | When specified, a violations report will be generated. A URL link to the report will be printed as an output to the command execution |
 | `--help`                             | Show options for given command.                                                |
 
 | Command                                | Description                                                     |
@@ -399,15 +393,15 @@
 3 | cleo==1.0.0a5
 
 Report URL: https://app.cycode.com/on-demand-scans/617ecc3d-9ff2-493e-8be8-2c1fecaf6939
 ```
 
 The report page will look something like below:
 
-![](./images/scan_details.png)
+![](https://raw.githubusercontent.com/cycodehq-public/cycode-cli/main/images/scan_details.png)
 
 ## Package Vulnerabilities Option
 
 > :memo: **Note**<br/>
 > This option is only available to SCA scans.
 
 To scan a specific package vulnerability of your local repository, add the argument `--sca-scan package-vulnerabilities` following the `-t sca` or `--scan-type sca` option.
@@ -738,7 +732,8 @@
 For example, to see options available for a Path Scan, you would simply enter:
 
 `cycode scan path --help`
 
 To see the options available for the ignore scan function, use this command:
 
 `cycode ignore --help`
+
```

