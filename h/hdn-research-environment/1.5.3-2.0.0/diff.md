# Comparing `tmp/hdn-research-environment-1.5.3.tar.gz` & `tmp/hdn-research-environment-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-1.5.3.tar", last modified: Mon Apr 17 10:46:27 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-2.0.0.tar", last modified: Mon May 29 11:59:59 2023, max compression
```

## Comparing `hdn-research-environment-1.5.3.tar` & `hdn-research-environment-2.0.0.tar`

### file list

```diff
@@ -1,85 +1,92 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-1.5.3/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-1.5.3/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-1.5.3/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)     2906 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      749 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.3/environment/api/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      663 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.3/environment/api/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/api/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/api/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1392 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/tests/test_auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1543 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3042 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1298 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1619 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2904 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.3/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      547 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2182 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1444 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1580 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      404 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      421 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2184 2022-03-29 15:52:24.000000 hdn-research-environment-1.5.3/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1821 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.3/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14537 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2556 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.3/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/static/environment/css/environment-base.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-1.5.3/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.3/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3058 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.3/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     1658 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     4511 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.3/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      400 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/_cloud_identity_info.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-1.5.3/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     2193 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/billing_setup.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.3/environment/templates/environment/create_research_environment.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1416 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3866 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/research_environments.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/workspace_being_provisioned.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3460 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.3/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      974 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12256 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3977 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    11233 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     6444 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3847 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      629 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     7755 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1474 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1305 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10168 2023-04-17 10:45:42.000000 hdn-research-environment-1.5.3/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2560 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.3/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.3/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.0.0/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.0.0/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.0.0/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/api/v1/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/v1/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/v1/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/v1/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/api/v2/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1572 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/v2/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      943 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/api/v2/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2832 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2849 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      818 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3562 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      792 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/mailers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2317 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    18754 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4342 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.0.0/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.0.0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2637 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6684 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1111 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-2.0.0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1455 2023-05-29 11:58:57.000000 hdn-research-environment-2.0.0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5481 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3871 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3514 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.0.0/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1555 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.0.0/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    13311 2023-05-29 11:59:00.000000 hdn-research-environment-2.0.0/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2871 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.0/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-05-29 11:59:59.000000 hdn-research-environment-2.0.0/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.0.0/setup.py
```

### Comparing `hdn-research-environment-1.5.3/LICENSE` & `hdn-research-environment-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/PKG-INFO` & `hdn-research-environment-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.5.3
+Version: 2.0.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.5.3/environment/api/__init__.py` & `hdn-research-environment-2.0.0/environment/api/v1/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,122 @@
 from typing import Optional
-
 from requests import Request
 
-from environment.api.decorators import api_request
+from environment.api.v1.decorators import api_request
 
 
 @api_request
 def create_cloud_identity(
-    gcp_user_id: str, given_name: str, family_name: str
+    gcp_user_id: str,
+    given_name: str,
+    family_name: str,
+    password: str,
+    recovery_email: str,
 ) -> Request:
-    json = {"userid": gcp_user_id, "givenName": given_name, "familyName": family_name}
+    json = {
+        "userid": gcp_user_id,
+        "givenName": given_name,
+        "familyName": family_name,
+        "password": password,
+        "recoveryEmail": recovery_email,
+    }
     return Request("POST", url="/user", json=json)
 
 
 @api_request
 def get_user_info(gcp_user_id: str) -> Request:
     return Request("GET", url=f"/user/{gcp_user_id}")
 
 
 @api_request
-def create_workspace(gcp_user_id: str, billing_id: str, region: str) -> Request:
-    json = {"userid": gcp_user_id, "billingid": billing_id, "region": region}
-    return Request("POST", url="/onetimeplatformsetup", json=json)
-
-
-@api_request
-def get_workspace_details(gcp_user_id: str, region: str) -> Request:
-    return Request("GET", url=f"/workspace/{gcp_user_id}/{region}")
+def get_workspace_details(gcp_user_id: str, gcp_project_id: str) -> Request:
+    return Request("GET", url=f"/workspace/{gcp_user_id}/{gcp_project_id}")
 
 
 @api_request
 def get_workspace_list(gcp_user_id: str) -> Request:
     return Request("GET", url=f"/workspace/list/{gcp_user_id}")
 
 
 @api_request
-def stop_workbench(gcp_user_id: str, workbench_id: str, region: str) -> Request:
-    params = {"userid": gcp_user_id, "id": workbench_id, "region": region}
+def stop_workbench(
+    gcp_user_id: str, workbench_id: str, region: str, gcp_project_id: str
+) -> Request:
+    params = {
+        "userid": gcp_user_id,
+        "id": workbench_id,
+        "region": region,
+        "gcp_project_id": gcp_project_id,
+    }
     return Request("PUT", url="/workbench/stop", params=params)
 
 
 @api_request
-def start_workbench(gcp_user_id: str, workbench_id: str, region: str) -> Request:
-    params = {"userid": gcp_user_id, "id": workbench_id, "region": region}
+def start_workbench(
+    gcp_user_id: str, workbench_id: str, region: str, gcp_project_id: str
+) -> Request:
+    params = {
+        "userid": gcp_user_id,
+        "id": workbench_id,
+        "region": region,
+        "gcp_project_id": gcp_project_id,
+    }
     return Request("PUT", url="/workbench/start", params=params)
 
 
 @api_request
 def change_workbench_instance_type(
-    gcp_user_id: str, workbench_id: str, region: str, new_instance_type: str
+    gcp_user_id: str,
+    workbench_id: str,
+    region: str,
+    new_instance_type: str,
+    gcp_project_id: str,
 ) -> Request:
     params = {
         "userid": gcp_user_id,
         "id": workbench_id,
         "region": region,
+        "gcp_project_id": gcp_project_id,
         "machinetype": new_instance_type,
     }
     return Request("PUT", url="/workbench/update", params=params)
 
 
 @api_request
-def delete_workbench(gcp_user_id: str, workbench_id: str, region: str) -> Request:
-    params = {"userid": gcp_user_id, "id": workbench_id, "region": region}
+def delete_workbench(
+    gcp_user_id: str, workbench_id: str, region: str, gcp_project_id: str
+) -> Request:
+    params = {
+        "userid": gcp_user_id,
+        "id": workbench_id,
+        "region": region,
+        "gcp_project_id": gcp_project_id,
+    }
     return Request("DELETE", url="/workbench", params=params)
 
 
 @api_request
 def create_workbench(
     gcp_user_id: str,
-    region: str,
     environment_type: str,
     instance_type: str,
     group_granting_data_access: str,
     persistent_disk: str,
     bucket_name: str,
+    gcp_project_id: str,
     vm_image: Optional[str] = None,
     gpu_accelerator: Optional[str] = None,
 ):
     json = {
         "userid": gcp_user_id,
-        "region": region,
         "type": environment_type,
         "machinetype": instance_type,
         "group_granting_data_access": group_granting_data_access,
         "bucketname": bucket_name,
+        "gcp_project_id": gcp_project_id,
         "persistentdisk": persistent_disk,
         "vmimage": vm_image,
         "gpu_accelerator": gpu_accelerator,
     }
     json_without_empty_values = {
         key: val for key, val in json.items() if val is not None
     }
```

### Comparing `hdn-research-environment-1.5.3/environment/api/auth.py` & `hdn-research-environment-2.0.0/environment/api/v1/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from typing import Callable
 
 import google.auth.jwt as jwt
-from requests import Request
 from django.conf import settings
+from requests import Request
 
 
-def _generate_credentials() -> jwt.Credentials:
+def _credentials_apply_closure() -> Callable[[Request], None]:
     credentials = jwt.Credentials.from_service_account_file(
-        settings.CLOUD_RESEARCH_ENVIRONMENTS_API_JWT_SERVICE_ACCOUNT_PATH,
-        audience=settings.CLOUD_RESEARCH_ENVIRONMENTS_API_JWT_AUDIENCE,
+        settings.CLOUD_RESEARCH_ENVIRONMENTS_API_V1_JWT_SERVICE_ACCOUNT_PATH,
+        audience=settings.CLOUD_RESEARCH_ENVIRONMENTS_API_V1_JWT_AUDIENCE,
     )
-    return credentials
-
-
-def _credentials_apply_closure() -> Callable[[Request], None]:
-    credentials = _generate_credentials()
 
     def apply_api_credentials(request: Request) -> None:
         credentials.before_request(None, request.method, request.url, request.headers)
 
     return apply_api_credentials
```

### Comparing `hdn-research-environment-1.5.3/environment/api/decorators.py` & `hdn-research-environment-2.0.0/environment/api/v1/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-from functools import wraps
 from typing import Callable
-
+from functools import wraps
 from requests import Request, Response, Session
+
 from django.conf import settings
 
-from environment.api.auth import apply_api_credentials
+from environment.api.v1.auth import apply_api_credentials
+
 
+def api_request(
+    request_creator_callable: Callable[..., Request],
+) -> Callable:
+    api_url = settings.CLOUD_RESEARCH_ENVIRONMENTS_API_V1_URL
 
-def api_request(request_creator_callable: Callable[..., Request]) -> Callable:
     @wraps(request_creator_callable)
     def wrapper(*args, **kwargs) -> Response:
         session = Session()
         request = request_creator_callable(*args, **kwargs)
-        request.url = f"{settings.CLOUD_RESEARCH_ENVIRONMENTS_API_URL}{request.url}"
+        request.url = f"{api_url}{request.url}"
         prepped = request.prepare()
         apply_api_credentials(prepped)
+
         return session.send(prepped)
 
     return wrapper
```

### Comparing `hdn-research-environment-1.5.3/environment/deserializers.py` & `hdn-research-environment-2.0.0/environment/deserializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                 workbench.get("url") or workbench.get("version-url")
             ),  # RStudio sends version-url
             instance_type=InstanceType(workbench["machine-type"]),
             region=Region(workbench["region"]),
             bucket_name=workbench.get("bucket-name"),
             type=EnvironmentType.from_string_or_none(workbench["type"]),
             status=EnvironmentStatus(workbench["workbench-setup-status"]),
+            workspace_name=workspace.get("gcp-project-id"),
         )
         for workspace in data["workspace-list"]
         for workbench in workspace["workbench-list"]
     ]
 
 
 def deserialize_workspace_details(data: dict) -> ResearchWorkspace:
@@ -43,7 +44,14 @@
         user_id=data["user-id"],
         region=data["region"],
         gcp_project_id=data["gcp-project-id"],
         gcp_billing_id=data["gcp-billing-id"],
         email_id=data["email-id"],
         workspace_setup_status=WorkspaceStatus(data["workspace-setup-status"]),
     )
+
+
+def deserialize_workspaces(data: dict) -> Iterable[ResearchWorkspace]:
+    return [
+        deserialize_workspace_details(workspace_data)
+        for workspace_data in data["workspace-list"]
+    ]
```

### Comparing `hdn-research-environment-1.5.3/environment/entities.py` & `hdn-research-environment-2.0.0/environment/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,21 @@
     US_CENTRAL = "us-central1"
     NORTHAMERICA_NORTHEAST = "northamerica-northeast1"
     EUROPE_WEST = "europe-west3"
     AUSTRALIA_SOUTHEAST = "australia-southeast1"
 
 
 class InstanceType(Enum):
-    N1_STANDARD_1 = "n1-standard-1"
     N1_STANDARD_2 = "n1-standard-2"
     N1_STANDARD_4 = "n1-standard-4"
     N1_STANDARD_8 = "n1-standard-8"
     N1_STANDARD_16 = "n1-standard-16"
 
     def cpus(self):
         INSTANCE_TO_CPU_MAP = {
-            InstanceType.N1_STANDARD_1: 1,
             InstanceType.N1_STANDARD_2: 2,
             InstanceType.N1_STANDARD_4: 4,
             InstanceType.N1_STANDARD_8: 8,
             InstanceType.N1_STANDARD_16: 16,
         }
 
         return INSTANCE_TO_CPU_MAP[self]
@@ -74,14 +72,15 @@
     group_granting_data_access: str
     region: Region
     type: EnvironmentType
     instance_type: InstanceType
     status: EnvironmentStatus
     bucket_name: Optional[str]
     url: Optional[str]
+    workspace_name: str
 
     @property
     def is_running(self):
         return self.status in [EnvironmentStatus.RUNNING, EnvironmentStatus.UPDATING]
 
     @property
     def is_paused(self):
```

### Comparing `hdn-research-environment-1.5.3/environment/exceptions.py` & `hdn-research-environment-2.0.0/environment/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,37 @@
     pass
 
 
 class BillingVerificationFailed(Exception):
     pass
 
 
+class BillingSharingFailed(Exception):
+    pass
+
+
+class BillingAccessRevokationFailed(Exception):
+    pass
+
+
 class GetAvailableEnvironmentsFailed(Exception):
     pass
 
 
 class GetUserInfoFailed(Exception):
     pass
 
 
 class GetWorkspaceDetailsFailed(Exception):
     pass
+
+
+class GetBillingAccountsListFailed(Exception):
+    pass
+
+
+class GetWorkspacesListFailed(Exception):
+    pass
+
+
+class CreateWorkspaceFailed(Exception):
+    pass
```

### Comparing `hdn-research-environment-1.5.3/environment/migrations/0001_initial.py` & `hdn-research-environment-2.0.0/environment/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django.conf import settings
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `hdn-research-environment-1.5.3/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.0.0/environment/migrations/0002_billingsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.core.validators
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("environment", "0001_initial"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="BillingSetup",
```

### Comparing `hdn-research-environment-1.5.3/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.0.0/environment/migrations/0005_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ("project", "0001_initial"),
         ("environment", "0004_auto_20220309_0330"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="Workflow",
             fields=[
```

### Comparing `hdn-research-environment-1.5.3/environment/models.py` & `hdn-research-environment-2.0.0/environment/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import uuid
+
 from django.db import models
 from django.core.validators import EmailValidator
 
 from environment.validators import gcp_billing_account_id_validator
 from environment.managers import WorkflowManager
 
 
@@ -12,34 +14,48 @@
     gcp_user_id = models.CharField(max_length=50, unique=True)
     email = models.EmailField(
         max_length=255, unique=True, validators=[EmailValidator()]
     )
     initial_workspace_setup_done = models.BooleanField(default=False)
 
 
-class BillingSetup(models.Model):
-    cloud_identity = models.OneToOneField(
-        CloudIdentity, related_name="billing_setup", on_delete=models.CASCADE
+class BillingAccountSharingInvite(models.Model):
+    owner = models.ForeignKey(
+        "user.User",
+        related_name="owner_billingaccountsharinginvite_set",
+        on_delete=models.CASCADE,
+    )
+    user = models.ForeignKey(
+        "user.User",
+        related_name="user_billingaccountsharinginvite_set",
+        on_delete=models.CASCADE,
+        null=True,
     )
+    user_contact_email = models.EmailField()
     billing_account_id = models.CharField(
-        max_length=20, unique=True, validators=[gcp_billing_account_id_validator]
+        max_length=32, validators=[gcp_billing_account_id_validator]
     )
+    token = models.UUIDField(default=uuid.uuid4, unique=True, editable=False)
+    is_consumed = models.BooleanField(default=False)
+    is_revoked = models.BooleanField(default=False)
 
 
 class Workflow(models.Model):
     objects = WorkflowManager()
 
     project = models.ForeignKey(
         "project.PublishedProject", related_name="workflows", on_delete=models.CASCADE
     )
     user = models.ForeignKey(
         "user.User", related_name="workflows", on_delete=models.CASCADE
     )
     execution_resource_name = models.CharField(max_length=256, unique=True)
 
+    workspace_name = models.CharField(max_length=256)
+
     INPROGRESS = 0
     SUCCESS = 1
     FAILED = 2
     STATUS_CHOICES = [
         (INPROGRESS, "In Progress"),
         (SUCCESS, "Succeeded"),
         (FAILED, "Failed"),
```

### Comparing `hdn-research-environment-1.5.3/environment/services.py` & `hdn-research-environment-2.0.0/environment/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-from typing import Tuple, Iterable, Optional, Callable
+from typing import Tuple, Iterable, Optional
+from collections import defaultdict
 
-from django.db.models import Q, Model
+from django.db.models import Model
 from django.core.mail import send_mail
 from django.template import loader
 from django.conf import settings
 from django.apps import apps
 from google.cloud.workflows import executions_v1beta
 from google.cloud.workflows.executions_v1beta.types import executions
 
 import environment.constants as constants
-import environment.api as api
-from environment.models import CloudIdentity, BillingSetup, Workflow
+import environment.mailers as mailers
+import environment.api.v1 as api_v1
+import environment.api.v2 as api_v2
+from environment.models import CloudIdentity, Workflow, BillingAccountSharingInvite
 from environment.exceptions import (
     IdentityProvisioningFailed,
     StopEnvironmentFailed,
     StartEnvironmentFailed,
     DeleteEnvironmentFailed,
     ChangeEnvironmentInstanceTypeFailed,
-    BillingVerificationFailed,
+    BillingSharingFailed,
+    BillingAccessRevokationFailed,
     EnvironmentCreationFailed,
     GetAvailableEnvironmentsFailed,
     GetWorkspaceDetailsFailed,
-    GetUserInfoFailed,
+    GetBillingAccountsListFailed,
+    GetWorkspacesListFailed,
+    CreateWorkspaceFailed,
 )
 from environment.deserializers import (
     deserialize_research_environments,
     deserialize_workspace_details,
+    deserialize_workspaces,
 )
 from environment.entities import (
     ResearchEnvironment,
     InstanceType,
     Region,
     ResearchWorkspace,
 )
@@ -57,77 +64,142 @@
     return "".join(c for c in project.slug + project.version if c.isalnum())
 
 
 def _environment_data_group(environment: ResearchEnvironment) -> str:
     return environment.group_granting_data_access
 
 
-def create_cloud_identity(user: User) -> Tuple[str, CloudIdentity]:
+def create_cloud_identity(
+    user: User, password: str, recovery_email: str
+) -> Tuple[str, CloudIdentity]:
     gcp_user_id = user.username
-    response = api.create_cloud_identity(
-        gcp_user_id, user.profile.first_names, user.profile.last_name
+    response = api_v2.create_cloud_identity(
+        gcp_user_id,
+        user.profile.first_names,
+        user.profile.last_name,
+        password,
+        recovery_email,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise IdentityProvisioningFailed(error_message)
 
     body = response.json()
     identity = CloudIdentity.objects.create(
-        user=user, gcp_user_id=gcp_user_id, email=body["email-id"]
+        user=user,
+        gcp_user_id=gcp_user_id,
+        email=body["primary_email"],
     )
-    otp = body["one-time-password"]
-    return otp, identity
-
+    return identity
 
-def get_user_info(user: User):
-    response = api.get_user_info(gcp_user_id=user.username)
 
-    if (
-        not response.ok
-    ):  # right now response form API is always ok (maybe except Runtime)
-        error_message = response.json()["message"]
-        raise GetUserInfoFailed(error_message)
+def get_billing_accounts_list(user: User):
+    response = api_v2.list_billing_accounts(user.cloud_identity.email)
+    if not response.ok:
+        error_message = None
+        try:
+            error_message = response.json()
+        finally:
+            raise GetBillingAccountsListFailed(error_message)
 
     return response.json()
 
 
-def verify_billing_and_create_workspace(user: User, billing_id: str):
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.create_workspace(
-        gcp_user_id=gcp_user_id,
-        billing_id=billing_id,
-        region=DEFAULT_REGION,
+def get_owned_shares_of_billing_account(owner: User, billing_account_id: str):
+    return owner.owner_billingaccountsharinginvite_set.filter(
+        billing_account_id=billing_account_id, is_revoked=False
+    )
+
+
+def invite_user_to_shared_billing_account(
+    request, owner: User, user_email: str, billing_account_id: str
+) -> BillingAccountSharingInvite:
+    invite = BillingAccountSharingInvite.objects.create(
+        owner=owner,
+        billing_account_id=billing_account_id,
+        user_contact_email=user_email,
+    )
+    mailers.send_billing_sharing_confirmation(request=request, invite=invite)
+    return invite
+
+
+def consume_billing_account_sharing_token(
+    user: User, token: str
+) -> BillingAccountSharingInvite:
+    invite = BillingAccountSharingInvite.objects.get(token=token, is_revoked=False)
+    invite.user = user
+    invite.save()
+
+    return invite
+
+
+def share_billing_account(owner_email: str, user_email: str, billing_account_id: str):
+    response = api_v2.share_billing_account(
+        owner_email=owner_email,
+        user_email=user_email,
+        billing_account_id=billing_account_id,
     )
     if not response.ok:
-        error_message = response.json()["error"]
-        raise BillingVerificationFailed(error_message)
+        error_message = response.json()
+        raise BillingSharingFailed(error_message)
 
 
-def create_billing_setup(user: User, billing_account_id: str) -> BillingSetup:
-    cloud_identity = user.cloud_identity
-    billing_setup = BillingSetup.objects.create(
-        cloud_identity=cloud_identity, billing_account_id=billing_account_id
+def revoke_billing_account_access(billing_account_sharing_invite_id: int):
+    billing_account_sharing_invite = BillingAccountSharingInvite.objects.select_related(
+        "owner__cloud_identity", "user__cloud_identity"
+    ).get(pk=billing_account_sharing_invite_id)
+    billing_account_sharing_invite.is_revoked = True
+    billing_account_sharing_invite.save()
+
+    if billing_account_sharing_invite.is_consumed:
+        _revoke_consumed_billing_account_access(billing_account_sharing_invite)
+
+
+def _revoke_consumed_billing_account_access(
+    billing_account_sharing_invite: BillingAccountSharingInvite,
+):
+    owner_email = billing_account_sharing_invite.owner.cloud_identity.email
+    user_email = billing_account_sharing_invite.user.cloud_identity.email
+    billing_account_id = billing_account_sharing_invite.billing_account_id
+
+    response = api_v2.revoke_billing_account_access(
+        owner_email=owner_email,
+        user_email=user_email,
+        billing_account_id=billing_account_id,
+    )
+    if not response.ok:
+        error_message = response.json()
+        raise BillingAccessRevokationFailed(error_message)
+
+
+def create_workspace(user: User, billing_account_id: str, region: str):
+    response = api_v2.create_workspace(
+        email=user.cloud_identity.email,
+        billing_account_id=billing_account_id,
+        region=region,
     )
-    return billing_setup
+    if not response.ok:
+        error_message = response.json()["error"]
+        raise CreateWorkspaceFailed(error_message)
 
 
 def _create_workbench_kwargs(
     user: User,
     project: PublishedProject,
-    region: str,
+    workspace_name: str,
     instance_type: str,
     environment_type: str,
     persistent_disk: int,
     gpu_accelerator: Optional[str] = None,
 ) -> dict:
     gcp_user_id = user.cloud_identity.gcp_user_id
 
     common = {
         "gcp_user_id": gcp_user_id,
-        "region": region,
+        "gcp_project_id": workspace_name,
         "environment_type": environment_type,
         "instance_type": instance_type,
         "group_granting_data_access": _project_data_group(project),
         "persistent_disk": str(persistent_disk),
         "bucket_name": project.project_file_root(),
     }
     if environment_type == "jupyter":
@@ -144,50 +216,51 @@
     else:
         return common
 
 
 def create_research_environment(
     user: User,
     project: PublishedProject,
-    region: str,
+    workspace_name: str,
     instance_type: str,
     environment_type: str,
     persistent_disk: int,
     gpu_accelerator: Optional[str] = None,
 ) -> str:
     kwargs = _create_workbench_kwargs(
         user,
         project,
-        region,
+        workspace_name,
         instance_type,
         environment_type,
         persistent_disk,
         gpu_accelerator,
     )
-    response = api.create_workbench(**kwargs)
+    response = api_v1.create_workbench(**kwargs)
     if not response.ok:
         error_message = response.json()[
             "error"
         ]  # TODO: Check all uses of "error"/"message"
         raise EnvironmentCreationFailed(error_message)
 
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         project_id=project.pk,
         type=Workflow.CREATE,
+        workspace_name=workspace_name,
     )
 
     return response.json()
 
 
 def get_workspace_details(user: User, region: Region) -> ResearchWorkspace:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.get_workspace_details(
+    response = api_v1.get_workspace_details(
         gcp_user_id=gcp_user_id,
         region=region.value,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise GetWorkspaceDetailsFailed(error_message)
 
@@ -225,15 +298,15 @@
         for project in PublishedProject.objects.all()
         if _project_data_group(project) in group_granting_data_accesses
     ]
 
 
 def get_active_environments(user: User) -> Iterable[ResearchEnvironment]:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.get_workspace_list(gcp_user_id)
+    response = api_v1.get_workspace_list(gcp_user_id)
     if not response.ok:
         error_message = response.json()["error"]
         raise GetAvailableEnvironmentsFailed(error_message)
     all_environments = deserialize_research_environments(response.json())
     return [environment for environment in all_environments if environment.is_active]
 
 
@@ -289,110 +362,149 @@
     return [
         (environment, project)
         for environment, project in all_environment_project_pairs
         if not project.has_access(user)
     ]
 
 
+def sort_environments_per_workspace(
+    environment_project_workflow_triplets: Iterable[
+        Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]
+    ],
+    workspaces: Iterable[ResearchWorkspace],
+):
+    sorted_environments_project_workflow_triplets = defaultdict(
+        list, {workspace.gcp_project_id: [] for workspace in workspaces}
+    )
+    for environment, project, workflows in environment_project_workflow_triplets:
+        if environment:
+            sorted_environments_project_workflow_triplets[
+                environment.workspace_name
+            ].append((environment, project, workflows))
+        else:
+            sorted_environments_project_workflow_triplets[
+                workflows.last().workspace_name
+            ].append((environment, project, workflows))
+    return dict(sorted_environments_project_workflow_triplets)
+
+
+def get_workspaces_list(user: User) -> Iterable[ResearchWorkspace]:
+    gcp_user_id = user.cloud_identity.gcp_user_id
+    response = api_v1.get_workspace_list(gcp_user_id)
+    if not response.ok:
+        error_message = response.json()["error"]
+        raise GetWorkspacesListFailed(error_message)
+    return deserialize_workspaces(response.json())
+
+
 def stop_running_environment(
-    user: User, project_id: str, workbench_id: str, region: Region
+    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
 ) -> str:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.stop_workbench(
+    response = api_v1.stop_workbench(
         gcp_user_id=gcp_user_id,
         workbench_id=workbench_id,
         region=region.value,
+        gcp_project_id=gcp_project_id,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise StopEnvironmentFailed(error_message)
 
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         project_id=project_id,
         type=Workflow.PAUSE,
+        workspace_name=gcp_project_id,
     )
 
     return response.json()
 
 
 def start_stopped_environment(
-    user: User, project_id: str, workbench_id: str, region: Region
+    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
 ) -> str:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.start_workbench(
+    response = api_v1.start_workbench(
         gcp_user_id=gcp_user_id,
         workbench_id=workbench_id,
         region=region.value,
+        gcp_project_id=gcp_project_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise StartEnvironmentFailed(error_message)
 
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         project_id=project_id,
         type=Workflow.START,
+        workspace_name=gcp_project_id,
     )
 
     return response.json()
 
 
 def change_environment_instance_type(
     user: User,
     project_id: str,
     workbench_id: str,
     region: Region,
+    gcp_project_id: str,
     new_instance_type: InstanceType,
 ) -> str:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.change_workbench_instance_type(
+    response = api_v1.change_workbench_instance_type(
         gcp_user_id=gcp_user_id,
         workbench_id=workbench_id,
         region=region.value,
         new_instance_type=new_instance_type.value,
+        gcp_project_id=gcp_project_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise ChangeEnvironmentInstanceTypeFailed(error_message)
 
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         project_id=project_id,
         type=Workflow.CHANGE,
+        workspace_name=gcp_project_id,
     )
 
     return response.json()
 
 
 def delete_environment(
-    user: User, project_id: str, workbench_id: str, region: Region
+    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
 ) -> str:
     gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api.delete_workbench(
+    response = api_v1.delete_workbench(
         gcp_user_id=gcp_user_id,
         workbench_id=workbench_id,
         region=region.value,
+        gcp_project_id=gcp_project_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise DeleteEnvironmentFailed(error_message)
 
     execution_resource_name = response.json()["execution-name"]
     persist_workflow(
         user=user,
         execution_resource_name=execution_resource_name,
         project_id=project_id,
         type=Workflow.DESTROY,
+        workspace_name=gcp_project_id,
     )
 
     return response.json()
 
 
 def send_environment_access_expired_email(
     user: User, projects: Iterable[PublishedProject]
@@ -407,19 +519,24 @@
     )
     send_mail(
         subject, body, settings.DEFAULT_FROM_EMAIL, [user.email], fail_silently=False
     )
 
 
 def persist_workflow(
-    user: User, execution_resource_name: str, project_id: int, type: int
+    user: User,
+    execution_resource_name: str,
+    project_id: int,
+    type: int,
+    workspace_name: str,
 ) -> Workflow:
     return Workflow.objects.create(
         user=user,
         execution_resource_name=execution_resource_name,
+        workspace_name=workspace_name,
         project_id=project_id,
         type=type,
         status=Workflow.INPROGRESS,
     )
 
 
 def get_execution_state(execution_resource_name) -> executions.Execution.State:
@@ -428,14 +545,15 @@
     return execution.state
 
 
 def mark_workflow_as_finished(
     execution_resource_name: str, execution_state: executions.Execution.State
 ):
     workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
+    # workflow.status = Workflow.SUCCESS
     if execution_state == executions.Execution.State.SUCCEEDED:
         workflow.status = Workflow.SUCCESS
     else:
         workflow.status = Workflow.FAILED
 
     workflow.save()
 
@@ -445,14 +563,14 @@
     cpu = sum(environment.instance_type.cpus() for environment in running_environments)
     return value + cpu
 
 
 def exceeded_quotas(user) -> Iterable[str]:
     quotas_exceeded = []
     # Check if user has exceeded MAX_RUNNING_ENVIRONMENTS
-    running_environments = get_active_environments(user)
-    if len(running_environments) >= constants.MAX_RUNNING_ENVIRONMENTS:
+    running_workspaces = get_workspaces_list(user)
+    if len(running_workspaces) >= constants.MAX_RUNNING_WORKSPACES:
         quotas_exceeded.append(
-            f"You can only have {constants.MAX_RUNNING_ENVIRONMENTS} running environments."
+            f"You can only have {constants.MAX_RUNNING_WORKSPACES} running workspaces."
         )
 
     return quotas_exceeded
```

### Comparing `hdn-research-environment-1.5.3/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.0.0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.0.0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.0.0/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.0.0/environment/static/environment/js/pricing_change.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,50 @@
 $(function() {
-    var current_region = $("#id_region").val()
+    // var current_region = $("#id_region").val()
+    // HACK: Use the workspace's region
+    const current_region = "us-central1"
     var current_instance_type = $("#id_instance_type").val()
     var current_instance_price = $(`#${current_region}-${current_instance_type}`)
     var current_data_amount = $("#id_persistent_disk").val()
     var current_data_price = $(`div[id*=${current_region}-Persistent]`)
 
     current_instance_price.show()
     current_data_price.show()
     $("#instance_total_cost span").text(current_instance_price.attr("data-cost"))
     $("#data_total_cost span").text((parseInt(current_data_amount) * current_data_price.attr("data-cost")).toFixed(2))
 
     function change_instance_shown_pricing() {
-        var current_region = $("#id_region").val()
+        // var current_region = $("#id_region").val()
         var current_instance_type = $("#id_instance_type").val()
         var current_instance_price = $(`#${current_region}-${current_instance_type}`)
         $("div.instance-costs").hide()
         current_instance_price.show()
     };
 
     function change_gpu_shown_pricing() {
         var current_gpu_accelerator = $("#id_gpu_accelerator").val()
-        var current_region = $("#id_region").val()
+        // var current_region = $("#id_region").val()
         $("div.gpu-accelerator-costs").hide()
 
         if (current_gpu_accelerator) {
             $("#gpu_accelerator_costs").show()
             $(`#${current_region}-${current_gpu_accelerator}`).show()
         };
     };
 
     function change_data_storage_costs_shown_pricing() {
-        var current_region = $("#id_region").val()
+        // var current_region = $("#id_region").val()
         var current_data_amount = $("#id_persistent_disk").val()
         $("div.data-storage-costs").hide()
         $(`div[id*=${current_region}-Persistent]`).show()
         $("#data_total_cost span").text((parseInt(current_data_amount) * current_data_price.attr("data-cost")).toFixed(2))
     }
 
     $("#id_instance_type, #id_region, #id_gpu_accelerator").on("change", function() {
-        var current_region = $("#id_region").val()
+        // var current_region = $("#id_region").val()
         var current_instance_type = $("#id_instance_type").val()
         var current_instance_price = $(`#${current_region}-${current_instance_type}`).attr("data-cost")
         var current_gpu_accelerator = $("#id_gpu_accelerator").val()
         var current_gpu_accelerator_price = $(`#${current_region}-${current_gpu_accelerator}`).attr("data-cost")
         var instance_total_cost = parseFloat(current_instance_price) + parseFloat(current_gpu_accelerator_price)
 
         if ($("#id_gpu_accelerator").val()) {
```

### Comparing `hdn-research-environment-1.5.3/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.0.0/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.0.0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.0.0/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.0.0/environment/templates/environment/identity_provisioning.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 {% block content %}
 <div class="container">
   {% include "message_snippet.html" %}
     <h2 class="mb-4">Research Environments</h2>
     <div class="card" style="width: 36rem;">
       <div class="card-body">
         <p class="card-text font-weight-bold">You don't have any research environments yet.</p>
-        <p class="card-text">To start, click the button below to provide you Google Cloud Identity.</p>
+        <p class="card-text">Provide a password and click the button below to create your Google Cloud Identity.</p>
         <form id="environment_identity_provisioning_form" action="{% url 'identity_provisioning' %}" method="post">
           {% csrf_token %}
-          <button class="btn btn-primary" type="submit">
+          {{ form }}
+          <button class="btn btn-primary mt-3" type="submit">
             Create Cloud Identity
           </button>
         </form>
       </div>
     </div>
 </div>
 {% endblock %}
```

### Comparing `hdn-research-environment-1.5.3/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.0.0/environment/templates/environment/research_environments.html`

 * *Files 12% similar despite different names*

```diff
@@ -47,22 +47,22 @@
               {{ available_project_environment_workflow_triplets|length }}
             </span>
           </a>
         </li>
         <li class="nav-item">
           <a
             class="nav-link"
-            id="cloud-identity-tab"
+            id="billing-accounts-tab"
             data-toggle="tab"
-            href="#cloud-identity"
+            href="#billing_accounts"
             role="tab"
-            aria-controls="cloud-identity"
+            aria-controls="billing_accounts"
             aria-selected="false"
           >
-            Cloud Identity
+            Billing
           </a>
         </li>
       </ul>
     </div>
     <div class="card-body">
       <div class="tab-content">
         <div
@@ -79,19 +79,19 @@
           role="tabpanel"
           aria-labelledby="projects-tab"
         >
           {% include "environment/_available_projects_list.html" %}
         </div>
         <div
           class="tab-pane fade"
-          id="cloud-identity"
+          id="billing_accounts"
           role="tabpanel"
-          aria-labelledby="cloud-identity-tab"
+          aria-labelledby="billing-accounts-tab"
         >
-          {% include "environment/_cloud_identity_info.html" %}
+          {% include "environment/_billing_accounts_list.html" %}
         </div>
       </div>
     </div>
   </div>
 {% endblock %}
 
 {% block local_js_bottom %}
```

### Comparing `hdn-research-environment-1.5.3/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.0.0/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.3/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.0.0/environment/templatetags/action_buttons.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     button_type: str,
 ) -> dict:
     data = button_types[button_type]
     request_data = {
         "workbench_id": environment.id,
         "project_id": project.pk,
         "region": environment.region.value,
+        "gcp_project_id": environment.workspace_name,
     }
 
     result_data = {
         "button_class": data["button_class"],
         "button_text": data["button_text"],
         "button_type": button_type,
         "url": reverse(data["url_name"]),
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/helpers.py` & `hdn-research-environment-2.0.0/environment/tests/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,17 +17,7 @@
     user = create_user_without_cloud_identity(username, email, password)
     CloudIdentity.objects.create(
         user=user,
         gcp_user_id=user.username,
         email=user.email,
     )
     return user
-
-
-def create_user_with_billing_setup(
-    username: str = "foo", email: str = "bar", password: str = "baz"
-) -> User:
-    user = create_user_with_cloud_identity(username, email, password)
-    BillingSetup.objects.create(
-        cloud_identity=user.cloud_identity, billing_account_id="XXXXXX-XXXXXX-XXXXXX"
-    )
-    return user
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/mocks.py` & `hdn-research-environment-2.0.0/environment/tests/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             "workbench-list": [
                 {
                     "bucket-name": None,
                     "build-id": "1a78b5dd-585a-4ee0-b4ef-b5ad6973db78",
                     "creation-timestamp": None,
                     "group-granting-data-access": "random_value",
                     "id": None,
-                    "machine-type": "n1-standard-1",
+                    "machine-type": "n1-standard-2",
                     "name": None,
                     "persistent_disk": None,
                     "region": "us-central1",
                     "service-accounts": None,
                     "state-file-path": None,
                     "status": None,
                     "type": None,
@@ -46,15 +46,15 @@
                 },
                 {
                     "bucket-name": None,
                     "build-id": "5f004ebb-46b7-4bfb-b4f9-2393966be0e7",
                     "creation-timestamp": None,
                     "group-granting-data-access": "random-value",
                     "id": None,
-                    "machine-type": "n1-standard-1",
+                    "machine-type": "n1-standard-2",
                     "name": None,
                     "persistent_disk": None,
                     "region": "us-central1",
                     "service-accounts": None,
                     "state-file-path": None,
                     "status": None,
                     "type": None,
@@ -80,15 +80,15 @@
                 },
                 {
                     "bucket-name": "reseacher_dataset",
                     "build-id": "abeb90a5-c6af-4533-af67-18d52203b31c",
                     "creation-timestamp": "2022-02-11T05:20:38.433-08:00",
                     "group-granting-data-access": "randomvalue",
                     "id": "7950866383761038413",
-                    "machine-type": "n1-standard-1",
+                    "machine-type": "n1-standard-2",
                     "name": "workspace-randomvalue-jupyterlab",
                     "persistent_disk": "1",
                     "region": "us-central1",
                     "service-accounts": [
                         {
                             "email": "randomvalue-jupyter@karoltest-us-c1-syhzv.iam.gserviceaccount.com",
                             "scopes": [
@@ -100,15 +100,14 @@
                     "state-file-path": "karoltest-us-c1-syhzv-workspace-randomvalue-jupyterlab",
                     "status": "destroyed",
                     "type": "jypyternotebook",
                     "updatable-config": [
                         {
                             "config-name": "instance-type",
                             "possible-values": [
-                                "n1-standard-1",
                                 "n1-standard-2",
                                 "n1-standard-4",
                                 "n1-standard-8",
                                 "n1-standard-16",
                             ],
                         }
                     ],
@@ -139,15 +138,15 @@
                 },
                 {
                     "bucket-name": "reseacher_dataset",
                     "build-id": "e158cd18-7ef2-4d80-babd-0b4b28947d9a",
                     "creation-timestamp": "2022-02-14T03:43:48.926-08:00",
                     "group-granting-data-access": "demopsn",
                     "id": "6122925253156404891",
-                    "machine-type": "n1-standard-1",
+                    "machine-type": "n1-standard-2",
                     "name": "workspace-demopsn-jupyterlab",
                     "persistent_disk": "1",
                     "region": "us-central1",
                     "service-accounts": [
                         {
                             "email": "demopsn-jupyter@karoltest-us-c1-syhzv.iam.gserviceaccount.com",
                             "scopes": [
@@ -159,15 +158,14 @@
                     "state-file-path": "karoltest-us-c1-syhzv-workspace-demopsn-jupyterlab",
                     "status": "running",
                     "type": "jypyternotebook",
                     "updatable-config": [
                         {
                             "config-name": "instance-type",
                             "possible-values": [
-                                "n1-standard-1",
                                 "n1-standard-2",
                                 "n1-standard-4",
                                 "n1-standard-8",
                                 "n1-standard-16",
                             ],
                         }
                     ],
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/test_decorators.py` & `hdn-research-environment-2.0.0/environment/tests/test_decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 from django.test import TestCase
 from django.urls import reverse
 from django.conf import settings
 
 from environment.decorators import (
     cloud_identity_required,
-    billing_setup_required,
     require_PATCH,
     require_DELETE,
 )
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CloudIdentityRequiredTestCase(TestCase):
     def test_redirects_user_without_cloud_identity_to_identity_provisioning(self):
         request_with_user_without_cloud_identity = Mock(
             user=Mock(spec=[]),
         )
         view = Mock()
         decorated_view = cloud_identity_required(view)
@@ -33,39 +35,18 @@
         )
         view = Mock()
         decorated_view = cloud_identity_required(view)
         decorated_view(request_with_user_without_cloud_identity)
         view.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
-class BillingSetupRequiredTestCase(TestCase):
-    def test_redirects_user_without_billing_account_to_billing_setup(self):
-        request_with_user_without_billing_account = Mock(
-            user=Mock(spec=[]),
-        )
-        view = Mock()
-        decorated_view = billing_setup_required(view)
-        response = decorated_view(request_with_user_without_billing_account)
-        self.assertRedirects(
-            response, reverse("billing_setup"), fetch_redirect_response=False
-        )
-        view.assert_not_called()
-
-    def test_does_not_redirect_user_with_billing_account(self):
-        request_with_user_without_billing_account = Mock(
-            user=Mock(spec=["cloud_identity"]),
-        )
-        view = Mock()
-        decorated_view = billing_setup_required(view)
-        decorated_view(request_with_user_without_billing_account)
-        view.assert_called()
-
-
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class RequirePatchTestCase(TestCase):
     def test_returns_405_for_non_patch_requests(self):
         methods = [
             "DELETE",
             "GET",
             "POST",
             "HEAD",
@@ -86,15 +67,18 @@
         request = Mock(method="PATCH")
         view = Mock()
         decorated_view = require_PATCH(view)
         decorated_view(request)
         view.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class RequireDeleteTestCase(TestCase):
     def test_returns_405_for_non_delete_requests(self):
         methods = ["PATCH", "GET", "POST", "HEAD", "PUT", "CONNECT", "OPTIONS", "TRACE"]
         responses = []
         for method in methods:
             request = Mock(method=method)
             view = Mock()
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/test_services.py` & `hdn-research-environment-2.0.0/environment/tests/test_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.conf import settings
 from django.test import TestCase
 from django.contrib.auth import get_user_model
 from django.apps import apps
 
 from environment.services import (
     create_cloud_identity,
-    create_billing_setup,
     create_research_environment,
     stop_running_environment,
     start_stopped_environment,
     change_environment_instance_type,
     delete_environment,
     verify_billing_and_create_workspace,
     get_environments_with_projects,
@@ -33,25 +32,27 @@
     EnvironmentStatus,
     ResearchEnvironment,
 )
 from environment.tests.mocks import get_workspace_list_json
 from environment.tests.helpers import (
     create_user_without_cloud_identity,
     create_user_with_cloud_identity,
-    create_user_with_billing_setup,
 )
 
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 User = get_user_model()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateCloudIdentityTestCase(TestCase):
     def setUp(self):
         self.user = create_user_without_cloud_identity()
 
     @patch("environment.api.create_cloud_identity")
     def test_raises_if_request_fails(self, mock_create_cloud_identity):
         mock_create_cloud_identity.return_value.ok = False
@@ -76,66 +77,60 @@
         otp, identity = create_cloud_identity(self.user)
         self.assertEqual(otp, mock_otp)
         self.assertEqual(identity.gcp_user_id, f"researcher_{self.user.username}")
         self.assertEqual(identity.email, mock_email)
         self.assertEqual(self.user.cloud_identity, identity)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
-class CreateBillingSetupTestCase(TestCase):
-    def setUp(self):
-        self.user = create_user_with_cloud_identity()
-
-    def test_creates_billing_setup_for_specified_user(self):
-        mock_billing_account = "XXXXXX-XXXXXX-XXXXXX"
-        billing_setup = create_billing_setup(self.user, mock_billing_account)
-        self.assertEqual(self.user.cloud_identity.billing_setup, billing_setup)
-        self.assertEqual(billing_setup.billing_account_id, mock_billing_account)
-
-
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class CreateResearchEnvironmentTestCase(TestCase):
     def setUp(self):
         self.project = MagicMock()
         self.project.slug = "slug"
         self.project.get_project_file_root.return_value = "bucket"
-        self.user = create_user_with_billing_setup()
+        self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.create_workbench")
     def test_raises_if_request_fails(self, mock_create_workbench):
         mock_create_workbench.return_value.ok = False
         self.assertRaises(
             EnvironmentCreationFailed,
             create_research_environment,
             self.user,
             self.project,
             "us-central1",
-            "n1-standard-1",
+            "n1-standard-2",
             "enviornment_type",
             "100",
         )
 
     @patch("environment.api.create_workbench")
     def test_returns_api_response_if_request_succeeds(self, mock_create_workbench):
         mock_create_workbench.return_value.ok = True
         result = create_research_environment(
             self.user,
             self.project,
             "us-central1",
-            "n1-standard-1",
+            "n1-standard-2",
             "enviornment_type",
             "100",
         )
         self.assertEqual(result, mock_create_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class StopRunningEnvironmentTestCase(TestCase):
     def setUp(self):
-        self.user = create_user_with_billing_setup()
+        self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.stop_workbench")
     def test_raises_if_request_fails(self, mock_stop_workbench):
         mock_stop_workbench.return_value.ok = False
         self.assertRaises(
             StopEnvironmentFailed,
             stop_running_environment,
@@ -149,18 +144,21 @@
         mock_stop_workbench.return_value.ok = True
         result = stop_running_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_stop_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class StartStoppedEnvironmentTestCase(TestCase):
     def setUp(self):
-        self.user = create_user_with_billing_setup()
+        self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.start_workbench")
     def test_raises_if_request_fails(self, mock_start_workbench):
         mock_start_workbench.return_value.ok = False
         self.assertRaises(
             StartEnvironmentFailed,
             start_stopped_environment,
@@ -174,47 +172,53 @@
         mock_stop_workbench.return_value.ok = True
         result = start_stopped_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_stop_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class ChangeEnvironmentInstanceTypeTestCase(TestCase):
     def setUp(self):
-        self.user = create_user_with_billing_setup()
+        self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.change_workbench_instance_type")
     def test_raises_if_request_fails(self, mock_change_workbench_instance_type):
         mock_change_workbench_instance_type.return_value.ok = False
         self.assertRaises(
             ChangeEnvironmentInstanceTypeFailed,
             change_environment_instance_type,
             self.user,
             "workbench_id",
             Region.AUSTRALIA_SOUTHEAST,
-            InstanceType.N1_STANDARD_1,
+            InstanceType.N1_STANDARD_2,
         )
 
     @patch("environment.api.change_workbench_instance_type")
     def test_raises_if_request_succeeds(self, mock_change_workbench_instance_type):
         mock_change_workbench_instance_type.return_value.ok = True
         result = change_environment_instance_type(
             self.user,
             "workbench_id",
             Region.AUSTRALIA_SOUTHEAST,
-            InstanceType.N1_STANDARD_1,
+            InstanceType.N1_STANDARD_2,
         )
         self.assertEqual(result, mock_change_workbench_instance_type.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class DeleteEnvironmentTestCase(TestCase):
     def setUp(self):
-        self.user = create_user_with_billing_setup()
+        self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.delete_workbench")
     def test_raises_if_request_fails(self, mock_delete_workbench):
         mock_delete_workbench.return_value.ok = False
         self.assertRaises(
             DeleteEnvironmentFailed,
             delete_environment,
@@ -228,15 +232,18 @@
         mock_delete_workbench.return_value.ok = True
         result = delete_environment(
             self.user, "workbench_id", Region.AUSTRALIA_SOUTHEAST
         )
         self.assertEqual(result, mock_delete_workbench.return_value)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class VerifyBillingAndCreateWorkspaceTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
         self.some_billing_id = "XXXXXX-XXXXXX-XXXXXX"
 
     @patch("environment.api.create_workspace")
     def test_raises_if_request_fails(self, mock_create_workspace):
@@ -250,15 +257,18 @@
 
     @patch("environment.api.create_workspace")
     def test_not_raises_if_request_succeeds(self, mock_create_workspace):
         mock_create_workspace.return_value.ok = True
         verify_billing_and_create_workspace(self.user, self.some_billing_id)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class GetAvailableEnvironmentsWithProjectsTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
 
     @patch("environment.api.get_workspace_list")
     def test_fetches_environments_and_parses_to_entity(self, mock_get_workspace_list):
         mock_get_workspace_list.return_value.json.return_value = get_workspace_list_json
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/test_signals.py` & `hdn-research-environment-2.0.0/environment/tests/test_signals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,144 +1,140 @@
-from datetime import timedelta
+from datetime import timedelta, datetime
 from unittest import skipIf
 from unittest.mock import patch
 
+
 from django.test import TestCase
 from django.conf import settings
 from django.utils import timezone
 
-from environment.signals import User, DataAccessRequest, Training
+from environment.signals import User, DataAccessRequest, Training, Event
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class UserSignalsTestCase(TestCase):
     def test_memoizes_original_credentialing_on_init(self):
         new_user = User()
         self.assertEqual(new_user._original_is_credentialed, new_user.is_credentialed)
 
     @patch("environment.signals.stop_environments_with_expired_access")
-    def test_does_not_schedule_task_on_save_if_user_has_no_billing_setup(
-        self, mock_stop_environments_with_expired_access
-    ):
-        new_user = User(is_credentialed=True)
-        new_user.is_credentialed = False
-        new_user.save()
-        mock_stop_environments_with_expired_access.assert_not_called()
-
-    @patch("environment.signals.stop_environments_with_expired_access")
-    @patch("environment.signals.user_has_billing_setup")
     def test_schedules_task_on_save_if_credentialing_was_revoked(
-        self, mock_user_has_billing_setup, mock_stop_environments_with_expired_access
+        self, mock_stop_environments_with_expired_access
     ):
-        mock_user_has_billing_setup.return_value = True
         new_user = User(is_credentialed=True)
         new_user.is_credentialed = False
         new_user.save()
         mock_stop_environments_with_expired_access.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class TrainingSignalsTestCase(TestCase):
     def test_memoizes_original_validity_on_init(self):
         new_user = User()
         new_user.save()
         new_training = Training(user=new_user, training_type_id=1)
         self.assertEqual(new_training._original_is_valid, new_training.is_valid())
 
     @patch("environment.signals.stop_environments_with_expired_access")
-    def test_does_not_schedule_task_on_save_if_user_has_no_billing_setup(
-        self, mock_stop_environments_with_expired_access
-    ):
-        new_user = User()
-        new_user.save()
-        new_training = Training(user=new_user, training_type_id=1)
-        new_training.save()
-        mock_stop_environments_with_expired_access.assert_not_called()
-
-    @patch("environment.signals.stop_environments_with_expired_access")
-    @patch("environment.signals.user_has_billing_setup")
     def test_schedules_task_on_save_if_training_was_accepted(
-        self, mock_user_has_billing_setup, mock_stop_environments_with_expired_access
+        self, mock_stop_environments_with_expired_access
     ):
-        mock_user_has_billing_setup.return_value = True
         new_user = User()
         new_user.save()
         new_training = Training(
             user=new_user, process_datetime=timezone.now(), training_type_id=1
         )
         new_training._original_is_valid = False
         new_training.is_valid = lambda: True
         new_training.save()
         mock_stop_environments_with_expired_access.assert_called()
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class DataAccessRequestSignalsTestCase(TestCase):
     def test_memoizes_original_is_accepted_on_init(self):
         new_access_request = DataAccessRequest()
         self.assertEqual(
             new_access_request._original_is_accepted, new_access_request.is_accepted()
         )
 
     def test_memoizes_original_is_revoked_on_init(self):
         new_access_request = DataAccessRequest()
         self.assertEqual(
             new_access_request._original_is_revoked, new_access_request.is_revoked()
         )
 
     @patch("environment.signals.stop_environments_with_expired_access")
-    def test_does_not_schedule_task_on_save_if_user_has_no_billing_setup(
-        self, mock_stop_environments_with_expired_access
-    ):
-        requester = User()
-        requester.save()
-        new_data_access_request = DataAccessRequest(
-            requester=requester, project_id=1, duration=timedelta(days=10)
-        )
-        new_data_access_request._original_is_accepted = False
-        new_data_access_request.is_accepted = lambda: True
-        new_data_access_request.save()
-        mock_stop_environments_with_expired_access.assert_not_called()
-
-    @patch("environment.signals.stop_environments_with_expired_access")
-    @patch("environment.signals.user_has_billing_setup")
     def test_does_not_schedule_task_on_save_if_access_duration_was_not_specified(
-        self, mock_user_has_billing_setup, mock_stop_environments_with_expired_access
+        self, mock_stop_environments_with_expired_access
     ):
-        mock_user_has_billing_setup.return_value = True
         requester = User()
         requester.save()
         new_data_access_request = DataAccessRequest(requester=requester, project_id=1)
         new_data_access_request._original_is_accepted = False
         new_data_access_request.is_accepted = lambda: True
         new_data_access_request.save()
         mock_stop_environments_with_expired_access.assert_not_called()
 
     @patch("environment.signals.stop_environments_with_expired_access")
-    @patch("environment.signals.user_has_billing_setup")
     def test_schedules_task_on_save_if_request_with_duration_was_accepted(
-        self, mock_user_has_billing_setup, mock_stop_environments_with_expired_access
+        self, mock_stop_environments_with_expired_access
     ):
-        mock_user_has_billing_setup.return_value = True
         requester = User()
         requester.save()
         new_data_access_request = DataAccessRequest(
             requester=requester, project_id=1, duration=timedelta(days=10)
         )
         new_data_access_request._original_is_accepted = False
         new_data_access_request.is_accepted = lambda: True
         new_data_access_request.save()
         mock_stop_environments_with_expired_access.assert_called()
 
     @patch("environment.signals.stop_environments_with_expired_access")
-    @patch("environment.signals.user_has_billing_setup")
     def test_schedules_task_on_save_if_access_was_revoked(
-        self, mock_user_has_billing_setup, mock_stop_environments_with_expired_access
+        self, mock_stop_environments_with_expired_access
     ):
-        mock_user_has_billing_setup.return_value = True
         requester = User()
         requester.save()
         new_data_access_request = DataAccessRequest(requester=requester, project_id=1)
         new_data_access_request._original_is_revoked = False
         new_data_access_request.is_revoked = lambda: True
         new_data_access_request.save()
         mock_stop_environments_with_expired_access.assert_called()
+
+
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
+class EventSignalsTestCase(TestCase):
+    def test_memoize_original_event_end_time(self):
+        new_event = Event()
+        self.assertEqual(new_event._original_end_date, new_event.end_date)
+
+    @patch(
+        "environment.signals.stop_event_participants_environments_with_expired_access"
+    )
+    def test_schedule_stop_environments_if_event_finished(
+        self, mock_stop_event_participants_environments_with_expired_access
+    ):
+        host = User()
+        participant = User(username="participant", email="participant@email.com")
+        host.save()
+        participant.save()
+
+        event = Event(host_id=host.id, end_date=datetime(year=2000, month=12, day=12))
+        event.save()
+        event.enroll_user(participant)
+
+        mock_stop_event_participants_environments_with_expired_access.assert_called_with(
+            event.id, schedule=event.end_date
+        )
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/test_utilities.py` & `hdn-research-environment-2.0.0/environment/tests/test_utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,61 +2,44 @@
 
 from django.test import TestCase
 from django.conf import settings
 
 from environment.tests.helpers import (
     create_user_with_cloud_identity,
     create_user_without_cloud_identity,
-    create_user_with_billing_setup,
 )
 from environment.utilities import (
     user_has_cloud_identity,
-    user_has_billing_setup,
     left_join_iterators,
     inner_join_iterators,
 )
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class UserHasCloudIdentityTestCase(TestCase):
     def setUp(self):
         self.user_without_cloud_identity = create_user_without_cloud_identity()
         self.user_with_cloud_identity = create_user_with_cloud_identity(
             "laa", "loo", "lee"
         )
 
     def test_returns_false_for_user_without_cloud_identity(self):
         self.assertFalse(user_has_cloud_identity(self.user_without_cloud_identity))
 
     def test_returns_true_for_user_with_cloud_identity(self):
         self.assertTrue(user_has_cloud_identity(self.user_with_cloud_identity))
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
-class UserHasBillingSetupTestCase(TestCase):
-    def setUp(self):
-        self.user_without_cloud_identity = create_user_without_cloud_identity()
-        self.user_with_cloud_identity = create_user_with_cloud_identity(
-            "laa", "loo", "lee"
-        )
-        self.user_with_billing_setup = create_user_with_billing_setup(
-            "woo", "waa", "wee"
-        )
-
-    def test_returns_false_for_user_without_cloud_identity(self):
-        self.assertFalse(user_has_billing_setup(self.user_without_cloud_identity))
-
-    def test_returns_false_for_user_without_billing_setup(self):
-        self.assertFalse(user_has_billing_setup(self.user_with_cloud_identity))
-
-    def test_returns_true_for_user_with_billing_setup(self):
-        self.assertTrue(user_has_billing_setup(self.user_with_billing_setup))
-
-
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class InnerJoinIteratorsTestCase(TestCase):
     def test_returns_lists_left_joined_on_keys(self):
         list1 = [
             {"id": 1, "data": "anything1"},
             {"id": 2, "data": "anything2"},
             {"id": 3, "data": "anything3"},
             {"id": 4, "data": "anything3"},
@@ -72,15 +55,18 @@
         expected_output = [
             (list1[1], list2[1]),
             (list1[2], list2[0]),
         ]
         self.assertEqual(inner_joined, expected_output)
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class LeftJoinIteratorsTestCase(TestCase):
     def test_returns_lists_left_joined_on_keys(self):
         list1 = [
             {"id": 1, "data": "anything1"},
             {"id": 2, "data": "anything2"},
             {"id": 3, "data": "anything3"},
             {"id": 4, "data": "anything3"},
```

### Comparing `hdn-research-environment-1.5.3/environment/tests/test_validators.py` & `hdn-research-environment-2.0.0/environment/tests/test_validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from django.forms import ValidationError
 from django.test import TestCase
 from django.conf import settings
 
 from environment.validators import gcp_billing_account_id_validator
 
 
-@skipIf(not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS, "Research environments are disabled")
+@skipIf(
+    not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
+    "Research environments are disabled",
+)
 class BillingAccountValidatorTestCase(TestCase):
     def test_fails_for_invalid_regex(self):
         self.assertRaises(
             ValidationError, gcp_billing_account_id_validator, "some value"
         )
 
     def test_succeeds_for_billing_account_regex(self):
```

### Comparing `hdn-research-environment-1.5.3/environment/utilities.py` & `hdn-research-environment-2.0.0/environment/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 User = Model
 
 
 def user_has_cloud_identity(user: User) -> bool:
     return hasattr(user, "cloud_identity")
 
 
-def user_has_billing_setup(user: User) -> bool:
-    if not user_has_cloud_identity(user):
-        return False
-    return hasattr(user.cloud_identity, "billing_setup")
-
-
 def user_workspace_setup_done(user: User) -> bool:
     if not user_has_cloud_identity(user):
         return False
     return user.cloud_identity.initial_workspace_setup_done
 
 
 def inner_join_iterators(
```

### Comparing `hdn-research-environment-1.5.3/environment/views.py` & `hdn-research-environment-2.0.0/environment/views.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,81 @@
 import json
+import concurrent
 
 from django.shortcuts import render, redirect
 from django.http import JsonResponse
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
+from django.db import transaction
 from django.views.decorators.http import require_http_methods, require_GET
 from google.cloud.workflows.executions_v1beta.types.executions import Execution
 
 import environment.services as services
 import environment.constants as constants
-from environment.forms import BillingAccountIdForm, CreateResearchEnvironmentForm
-from environment.exceptions import BillingVerificationFailed
+from environment.forms import (
+    CreateResearchEnvironmentForm,
+    CloudIdentityPasswordForm,
+    CreateWorkspaceForm,
+    ShareBillingAccountForm,
+)
 from environment.decorators import (
     cloud_identity_required,
-    billing_setup_required,
-    workspace_setup_required,
     require_DELETE,
     require_PATCH,
 )
 from environment.entities import Region, InstanceType
 from environment.utilities import (
     user_has_cloud_identity,
-    user_has_billing_setup,
 )
-from environment.models import CloudIdentity, Workflow
-from collections import namedtuple
+from environment.models import Workflow
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 def identity_provisioning(request):
     if user_has_cloud_identity(request.user):
-        return redirect("billing_setup")
-
-    user_info = services.get_user_info(request.user)
-    if user_info.get("user-status") == "user-added-in-cloud-identity":
-        CloudIdentity.objects.create(
-            user=request.user,
-            gcp_user_id=user_info.get("user-id"),
-            email=user_info.get("email-id"),
-        )
-        return redirect("billing_setup")
-
-    if request.method == "POST":
-        otp, _ = services.create_cloud_identity(request.user)
-        request.session["cloud_identity_otp"] = otp
-        return redirect("billing_setup")
-
-    return render(request, "environment/identity_provisioning.html")
-
-
-@require_http_methods(["GET", "POST"])
-@login_required
-@cloud_identity_required
-def billing_setup(request):
-    if user_has_billing_setup(request.user):
         return redirect("research_environments")
 
+    # TODO: Handle the case where the user was created successfully, but the response was lost.
     if request.method == "POST":
-        form = BillingAccountIdForm(request.POST)
+        form = CloudIdentityPasswordForm(request.POST)
         if form.is_valid():
-            try:
-                services.verify_billing_and_create_workspace(
-                    user=request.user,
-                    billing_id=form.cleaned_data["billing_account_id"],
-                )
-                services.create_billing_setup(
-                    request.user, form.cleaned_data["billing_account_id"]
-                )
-                return redirect("research_environments")
-            except BillingVerificationFailed as err:
-                form.add_error("billing_account_id", err)
+            services.create_cloud_identity(
+                request.user,
+                form.cleaned_data.get("password"),
+                form.cleaned_data.get("recovery_email"),
+            )
+            return redirect("research_environments")
     else:
-        form = BillingAccountIdForm()
+        form = CloudIdentityPasswordForm()
 
-    cloud_identity = request.user.cloud_identity
-    session_otp = request.session.get("cloud_identity_otp")
-    one_time_password = session_otp or services.get_user_info(request.user).get("one-time-password")
-    context = {
-        "email": cloud_identity.email,
-        "otp": one_time_password,
-        "form": form,
-    }
-    return render(request, "environment/billing_setup.html", context)
+    return render(
+        request, "environment/identity_provisioning.html", context={"form": form}
+    )
 
 
 @require_GET
 @login_required
 @cloud_identity_required
-@billing_setup_required
-def workspace_setup(request):
-    if request.user.cloud_identity.initial_workspace_setup_done:
-        return redirect("research_environments")
-
-    is_workspace_done = services.is_user_workspace_setup_done(request.user)
-    if not is_workspace_done:
-        return render(request, "environment/workspace_being_provisioned.html")
-    services.mark_user_workspace_setup_as_done(request.user)
-    return redirect("research_environments")
+def research_environments(request):
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+        workspaces_list_future = executor.submit(
+            services.get_workspaces_list, request.user
+        )
+        billing_accounts_list_future = executor.submit(
+            services.get_billing_accounts_list, request.user
+        )
+        environment_project_workflow_future = executor.submit(
+            services.get_environments_with_projects, request.user
+        )
 
+    workspaces_list = workspaces_list_future.result()
+    environment_project_workflow_triplets = environment_project_workflow_future.result()
+    billing_accounts_list = billing_accounts_list_future.result()
 
-@require_GET
-@login_required
-@cloud_identity_required
-@billing_setup_required
-@workspace_setup_required
-def research_environments(request):
-    environment_project_workflow_triplets = services.get_environments_with_projects(
-        request.user
-    )
     environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
     available_project_environment_workflow_triplets = (
         services.get_available_projects_with_environments(
             request.user,
             environments,
         )
     )
@@ -121,39 +84,74 @@
             available_project_environment_workflow_triplets
         )
     )
     environment_projects_pairs_with_creating = (
         projects_with_environments_being_created + environment_project_workflow_triplets
     )
 
+    sorted_environments_project_workflow_triplets_dict = (
+        services.sort_environments_per_workspace(
+            environment_projects_pairs_with_creating, workspaces_list
+        )
+    )
+
     context = {
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
         "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
-        "cloud_identity": request.user.cloud_identity,
+        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
+        "billing_accounts_list": billing_accounts_list,
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
     )
 
 
 @require_GET
 @login_required
 @cloud_identity_required
-@billing_setup_required
-@workspace_setup_required
 def research_environments_partial(request):
-    environment_project_workflow_triplets = services.get_environments_with_projects(
-        request.user
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+        workspaces_list_future = executor.submit(
+            services.get_workspaces_list, request.user
+        )
+        environment_project_workflow_future = executor.submit(
+            services.get_environments_with_projects, request.user
+        )
+
+    workspaces_list = workspaces_list_future.result()
+    environment_project_workflow_triplets = environment_project_workflow_future.result()
+
+    environments = map(lambda pair: pair[0], environment_project_workflow_triplets)
+    available_project_environment_workflow_triplets = (
+        services.get_available_projects_with_environments(
+            request.user,
+            environments,
+        )
+    )
+    projects_with_environments_being_created = (
+        services.get_projects_with_environment_being_created(
+            available_project_environment_workflow_triplets
+        )
+    )
+    environment_projects_pairs_with_creating = (
+        projects_with_environments_being_created + environment_project_workflow_triplets
+    )
+
+    sorted_environments_project_workflow_triplets_dict = (
+        services.sort_environments_per_workspace(
+            environment_projects_pairs_with_creating, workspaces_list
+        )
     )
 
     context = {
         "environment_project_workflow_triplets": environment_project_workflow_triplets,
+        "workspace_project_environment_workflow_triplets_dict": sorted_environments_project_workflow_triplets_dict,
     }
 
     execution_resource_name = request.GET.get("execution_resource_name")
     if execution_resource_name:
         workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
         workflow_state_context = {
             "recent_workflow": workflow,
@@ -168,137 +166,214 @@
         context,
     )
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
-@billing_setup_required
+def create_workspace(request):
+    billing_accounts_list = services.get_billing_accounts_list(request.user)
+
+    if request.method == "POST":
+        form = CreateWorkspaceForm(
+            request.POST, billing_accounts_list=billing_accounts_list
+        )
+        if form.is_valid():
+            services.create_workspace(
+                user=request.user,
+                billing_account_id=form.cleaned_data["billing_account_id"],
+                region=form.cleaned_data["region"],
+            )
+            return redirect("research_environments")
+    else:
+        form = CreateWorkspaceForm(billing_accounts_list=billing_accounts_list)
+
+    exceeded_quotas = services.exceeded_quotas(request.user)
+    context = {
+        "form": form,
+        "exceeded_quotas": exceeded_quotas,
+    }
+    return render(request, "environment/create_workspace.html", context)
+
+
+@require_http_methods(["GET", "POST"])
+@login_required
+@cloud_identity_required
 def create_research_environment(request, project_slug, project_version):
+    workspaces_list = services.get_workspaces_list(request.user)
     project = services.get_available_projects(request.user).get(
         slug=project_slug, version=project_version
     )
 
     if request.method == "POST":
-        form = CreateResearchEnvironmentForm(request.POST)
+        form = CreateResearchEnvironmentForm(
+            request.POST, workspace_list=workspaces_list
+        )
         if form.is_valid():
             cpu_usage = services.cpu_usage(
                 value=InstanceType(form.cleaned_data["instance_type"]).cpus(),
                 user=request.user,
             )
             if cpu_usage <= constants.MAX_CPU_USAGE:
                 services.create_research_environment(
                     user=request.user,
                     project=project,
-                    region=form.cleaned_data["region"],
+                    workspace_name=form.cleaned_data["workspace_id"],
                     instance_type=form.cleaned_data["instance_type"],
                     environment_type=form.cleaned_data["environment_type"],
                     persistent_disk=form.cleaned_data.get("persistent_disk"),
                     gpu_accelerator=form.cleaned_data.get("gpu_accelerator"),
                 )
                 return redirect("research_environments")
             else:
                 messages.error(
                     request,
                     f"Quota exceeded - the specified configuration would use {cpu_usage} out of {constants.MAX_CPU_USAGE} CPUs",
                 )
     else:
-        form = CreateResearchEnvironmentForm()
+        form = CreateResearchEnvironmentForm(workspace_list=workspaces_list)
 
     exceeded_quotas = services.exceeded_quotas(request.user)
     context = {
         "form": form,
         "project": project,
         "exceeded_quotas": exceeded_quotas,
         "instance_projected_costs": constants.INSTANCE_PROJECTED_COSTS,
         "gpu_projected_costs": constants.GPU_PROJECTED_COSTS,
         "data_storage_projected_costs": constants.DATA_STORAGE_PROJECTED_COSTS,
     }
     return render(request, "environment/create_research_environment.html", context)
 
 
+@require_http_methods(["GET", "POST"])
+@login_required
+@cloud_identity_required
+@transaction.atomic
+def manage_billing_account(request, billing_account_id):
+    owner = request.user
+    billing_account_sharing_form = ShareBillingAccountForm()
+
+    if request.method == "POST":
+        form_action = request.POST["action"]
+        if form_action == "share_account":
+            billing_account_sharing_form = ShareBillingAccountForm(request.POST)
+            if billing_account_sharing_form.is_valid():
+                services.invite_user_to_shared_billing_account(
+                    request=request,
+                    owner=owner,
+                    user_email=billing_account_sharing_form.cleaned_data["user_email"],
+                    billing_account_id=billing_account_id,
+                )
+                return redirect(request.path)
+        elif form_action == "revoke_access":
+            services.revoke_billing_account_access(request.POST["share_id"])
+            return redirect(request.path)
+
+    billing_account_shares = services.get_owned_shares_of_billing_account(
+        owner=owner, billing_account_id=billing_account_id
+    )
+    pending_shares = [
+        share for share in billing_account_shares if not share.is_consumed
+    ]
+    consumed_shares = [share for share in billing_account_shares if share.is_consumed]
+
+    context = {
+        "billing_account_sharing_form": billing_account_sharing_form,
+        "billing_account_id": billing_account_id,
+        "pending_shares": pending_shares,
+        "consumed_shares": consumed_shares,
+    }
+
+    return render(request, "environment/manage_billing_account.html", context)
+
+
+@require_GET
+@login_required
+def confirm_billing_account_sharing(request):
+    token = request.GET.get("token")
+    if token:
+        services.consume_billing_account_sharing_token(user=request.user, token=token)
+
+    return redirect("research_environments")
+
+
 @require_PATCH
 @login_required
 @cloud_identity_required
-@billing_setup_required
 def stop_running_environment(request):
     data = json.loads(request.body)
     services.stop_running_environment(
         user=request.user,
         project_id=data["project_id"],
         workbench_id=data["workbench_id"],
         region=Region(data["region"]),
+        gcp_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
-@billing_setup_required
 def start_stopped_environment(request):
     data = json.loads(request.body)
     services.start_stopped_environment(
         user=request.user,
         project_id=data["project_id"],
         workbench_id=data["workbench_id"],
         region=Region(data["region"]),
+        gcp_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
-@billing_setup_required
 def change_environment_instance_type(request):
     data = json.loads(request.body)
     services.change_environment_instance_type(
         user=request.user,
         project_id=data["project_id"],
         workbench_id=data["workbench_id"],
         region=Region(data["region"]),
         new_instance_type=InstanceType(data["instance_type"]),
+        gcp_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_DELETE
 @login_required
 @cloud_identity_required
-@billing_setup_required
 def delete_environment(request):
     data = json.loads(request.body)
     services.delete_environment(
         user=request.user,
         project_id=data["project_id"],
         workbench_id=data["workbench_id"],
         region=Region(data["region"]),
+        gcp_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_GET
 @login_required
 @cloud_identity_required
-@billing_setup_required
-def is_workspace_setup_done(request):
-    workspace_setup_finished = services.is_user_workspace_setup_done(user=request.user)
-    return JsonResponse({"finished": workspace_setup_finished})
-
-
-@require_GET
-@login_required
-@cloud_identity_required
-@billing_setup_required
 def check_execution_status(request):
     execution_resource_name = request.GET["execution_resource_name"]
     execution_state = services.get_execution_state(
         execution_resource_name=execution_resource_name
     )
     finished = execution_state != Execution.State.ACTIVE
     if finished:
         services.mark_workflow_as_finished(
             execution_resource_name=execution_resource_name,
             execution_state=execution_state,
         )
+    # finished=True
+    # services.mark_workflow_as_finished(
+    #     execution_resource_name=execution_resource_name,
+    #     execution_state=None,
+    # )
     return JsonResponse({"finished": finished})
```

### Comparing `hdn-research-environment-1.5.3/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.0.0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.5.3
+Version: 2.0.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.5.3/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.0.0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,49 +8,55 @@
 environment/apps.py
 environment/constants.py
 environment/decorators.py
 environment/deserializers.py
 environment/entities.py
 environment/exceptions.py
 environment/forms.py
+environment/mailers.py
 environment/managers.py
 environment/models.py
 environment/services.py
 environment/signals.py
 environment/tasks.py
 environment/urls.py
 environment/utilities.py
 environment/validators.py
 environment/views.py
 environment/api/__init__.py
-environment/api/auth.py
-environment/api/decorators.py
-environment/api/tests/__init__.py
-environment/api/tests/test_auth.py
-environment/api/tests/test_decorators.py
+environment/api/v1/__init__.py
+environment/api/v1/auth.py
+environment/api/v1/decorators.py
+environment/api/v2/__init__.py
+environment/api/v2/decorators.py
 environment/migrations/0001_initial.py
 environment/migrations/0002_billingsetup.py
 environment/migrations/0003_cloudidentity_is_workspace_done.py
 environment/migrations/0004_auto_20220309_0330.py
 environment/migrations/0005_workflow.py
+environment/migrations/0006_delete_billingsetup.py
+environment/migrations/0007_billingaccountsharinginvite.py
+environment/migrations/0008_workflow_workspace_name.py
+environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
 environment/migrations/__init__.py
 environment/static/environment/css/create_research_environment.css
 environment/static/environment/css/environment-base.css
+environment/static/environment/css/manage_billing_account.css
 environment/static/environment/js/cookie.js
 environment/static/environment/js/gpu_disabling.js
 environment/static/environment/js/pricing_change.js
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_available_projects_list.html
-environment/templates/environment/_cloud_identity_info.html
+environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/base_environment_home.html
-environment/templates/environment/billing_setup.html
 environment/templates/environment/create_research_environment.html
+environment/templates/environment/create_workspace.html
 environment/templates/environment/identity_provisioning.html
+environment/templates/environment/manage_billing_account.html
 environment/templates/environment/research_environments.html
-environment/templates/environment/workspace_being_provisioned.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/environment_action_button.html
 environment/templates/tag/environment_modal_button.html
 environment/templatetags/__init__.py
 environment/templatetags/action_buttons.py
 environment/tests/__init__.py
 environment/tests/helpers.py
```

### Comparing `hdn-research-environment-1.5.3/setup.cfg` & `hdn-research-environment-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 1.5.3
+version = 2.0.0
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

