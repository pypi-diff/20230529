# Comparing `tmp/grafana_django_saml2_auth-3.8.0.tar.gz` & `tmp/grafana_django_saml2_auth-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/django-saml2-auth/django-saml2-auth/dist/tmp4j1kakeg/grafana_django_saml2_auth-3.8.0.tar", last modified: Wed Jul 20 08:07:32 2022, max compression
+gzip compressed data, was "grafana_django_saml2_auth-3.9.0.tar", last modified: Tue Oct 11 13:43:38 2022, max compression
```

## Comparing `grafana_django_saml2_auth-3.8.0.tar` & `grafana_django_saml2_auth-3.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    40799 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    39728 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    15471 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/templates/django_saml2_auth/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/templates/django_saml2_auth/denied.html
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/templates/django_saml2_auth/error.html
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/templates/django_saml2_auth/signout.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    15894 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_saml.py
--rw-r--r--   0 runner    (1001) docker     (121)    15477 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    15852 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     7330 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10974 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/django_saml2_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    40799 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-20 08:07:32.000000 grafana_django_saml2_auth-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-07-20 08:06:38.000000 grafana_django_saml2_auth-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    41874 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    40764 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/django_saml2_auth/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15471 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.793289 grafana_django_saml2_auth-3.9.0/django_saml2_auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/django_saml2_auth/templates/django_saml2_auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/templates/django_saml2_auth/denied.html
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/templates/django_saml2_auth/error.html
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/templates/django_saml2_auth/signout.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15894 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_saml.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19041 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16409 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7330 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11231 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/django_saml2_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    41874 2022-10-11 13:43:38.000000 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-10-11 13:43:38.000000 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 13:43:38.000000 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-11 13:43:38.000000 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-11 13:43:38.000000 grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-11 13:43:38.797289 grafana_django_saml2_auth-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-10-11 13:42:39.000000 grafana_django_saml2_auth-3.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grafana_django_saml2_auth-3.8.0/AUTHORS.md` & `grafana_django_saml2_auth-3.9.0/AUTHORS.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,7 +48,11 @@
 - [kevPo](https://github.com/kevPo)
 - [chriskj](https://github.com/chriskj)
 - [Griffin J Rademacher](https://github.com/favorable-mutation)
 - [Akshit Dhar](https://github.com/akshit-wwstay)
 - [Jean Vincent](https://github.com/jean-sh)
 - [Søren Howe Gersager](https://github.com/syre)
 - [Gabrio Mauri](https://github.com/sgabb)
+- [Hugh Enxing](https://github.com/henxing) (CVision AI)
+- [Tamara Nocentini](https://github.com/TamaraNocentini)
+- [Paolo Romolini](https://github.com/paoloromolini)
+- [Uraiz Ali](https://github.com/UraizAli)
```

### Comparing `grafana_django_saml2_auth-3.8.0/LICENSE` & `grafana_django_saml2_auth-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/PKG-INFO` & `grafana_django_saml2_auth-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana_django_saml2_auth
-Version: 3.8.0
+Version: 3.9.0
 Summary: Django SAML2 Authentication Made Easy.
 Home-page: https://github.com/grafana/django-saml2-auth
 Author: Fang Li
 Author-email: surivlee+djsaml2auth@gmail.com
 Maintainer: Mostafa Moradian
 Maintainer-email: mostafa@grafana.com
 License: Apache 2.0
@@ -12,14 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,37 +35,26 @@
 This plugin supports both identity provider and service provider-initiated SSO:
 
 - For IdP-initiated SSO, the user should sign in to their identity provider platform, e.g., Okta, and click on the application that authorizes and redirects the user to the service provider, that is your platform.
 - For SP-initiated SSO, the user should first exist on your platform, either by signing in via the first method (IdP-initiated SSO) or any other custom solution. It can be configured to be redirected to the correct application on the identity provider platform.
 
 For IdP-initiated SSO, the user will be created if it doesn't exist. Still, for SP-initiated SSO, the user should exist in your platform for the code to detect and redirect them to the correct application on the identity provider platform.
 
-- [Django SAML2 Authentication](#django-saml2-authentication)
-  - [Project Information](#project-information)
-  - [Donate](#donate)
-  - [Installation](#installation)
-  - [How to use?](#how-to-use)
-  - [Module Settings](#module-settings)
-  - [JWT Signing Algorithm and Settings](#jwt-signing-algorithm-and-settings)
-    - [Custom token triggers](#custom-token-triggers)
-  - [Customize Error Messages](#customize-error-messages)
-  - [For Okta Users](#for-okta-users)
-
 ## Project Information
 
 - Original Author: Fang Li ([@fangli](https://github.com/fangli))
 - Maintainer: Mostafa Moradian ([@mostafa](https://github.com/mostafa))
 - Version support matrix:
     | **Python**                  | **Django** | **django-saml2-auth** |
     | --------------------------- | ---------- | --------------------- |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 2.2.x      | >=3.4.0               |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 3.2.x      | >=3.4.0               |
     | 3.8.x, 3.9.x, 3.10.x        | 4.0.x      | >=3.4.0               |
 
-- Release log is available [here](RELEASE-LOG.md).
+- Release logs are available [here](https://github.com/grafana/django-saml2-auth/releases). The old [release log file](RELEASE-LOG.md) still exist, and will be removed in future releases.
 
 - For contribution, read [contributing guide](CONTRIBUTING.md).
 
 ## CycloneDX SBOM
 
 From [v3.6.1](https://github.com/grafana/django-saml2-auth/releases/tag/v3.6.1), CycloneDX SBOMs will be generated for [requirements.txt](./requirements.txt) and [requirements_test.txt](./requirements_test.txt) and it can be accessed from the latest build of GitHub Actions for a tagged release, for example, [this one](https://github.com/grafana/django-saml2-auth/actions/runs/2245422253). The artifacts are only kept for 90 days.
 
@@ -165,14 +155,16 @@
             'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
             'groups': 'Groups',  # Optional
         },
         'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
             'SAML Group Name': 'Django Group Name',
         },
         'TRIGGER': {
+            # Optional: needs to return a User Model instance or None
+            'GET_USER': 'path.to.your.get.user.hook.method',
             'CREATE_USER': 'path.to.your.new.user.hook.method',
             'BEFORE_LOGIN': 'path.to.your.login.hook.method',
             'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
             # Optional. This is executed right before METADATA_AUTO_CONF_URL.
             # For systems with many metadata files registered allows to narrow the search scope.
             'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
             # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
@@ -211,14 +203,15 @@
 | **DEBUG**                                   | Send debug information to a log file                                                                                                                                                                                                                                                                                                                                                                                                                        | `bool`           | `False`                                                                                                                                  |                                                          |
 | **DEFAULT\_NEXT\_URL**                      | Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter `?next=` specificed in the login URL.                                                                                                                                                                                                                                                                         | `str`            | `admin:index`                                                                                                                            | `https://app.example.com/account/login`                  |
 | **CREATE\_USER**                            | Determines if a new Django user should be created for new users                                                                                                                                                                                                                                                                                                                                                                                             | `bool`           | `True`                                                                                                                                   |                                                          |
 | **NEW\_USER\_PROFILE**                      | Default settings for newly created users                                                                                                                                                                                                                                                                                                                                                                                                                    | `dict`           | `{'USER_GROUPS': [], 'ACTIVE_STATUS': True, 'STAFF_STATUS': False, 'SUPERUSER_STATUS': False}`                                           |                                                          |
 | **ATTRIBUTES\_MAP**                         | Mapping of Django user attributes to SAML2 user attributes                                                                                                                                                                                                                                                                                                                                                                                                  | `dict`           | `{'email': 'user.email', 'username': 'user.username', 'first_name': 'user.first_name', 'last_name': 'user.last_name', 'token': 'token'}` | `{'your.field': 'SAML.field'}`                           |
 | **TOKEN\_REQUIRED**                         | Set this to `False` if you don't require the token parameter in the SAML assertion (in the attributes map)                                                                                                                                                                                                                                                                                                                                                  | `bool`           | `True`                                                                                                                                   |                                                          |
 | **TRIGGER**                                 | Hooks to trigger additional actions during user login and creation flows. These `TRIGGER` hooks are strings containing a [dotted module name](https://docs.python.org/3/tutorial/modules.html#packages) which point to a method to be called. The referenced method should accept a single argument: a dictionary of attributes and values sent by the identity provider, representing the user's identity. Triggers will be executed only if they are set. | `dict`           | `{}`                                                                                                                                     |                                                          |
+| **TRIGGER.GET\_USER**                       | A method to be called upon getting an existing user. This method will be called before the new user is logged in and is used to customize the retrieval of an existing user record. This method should accept ONE parameter of user dict and return a User model instance or none.                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.get`                                |
 | **TRIGGER.CREATE\_USER**                    | A method to be called upon new user creation. This method will be called before the new user is logged in and after the user's record is created. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                                                     | `str`            | `None`                                                                                                                                   | `my_app.models.users.create`                             |
 | **TRIGGER.BEFORE\_LOGIN**                   | A method to be called when an existing user logs in. This method will be called before the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                           | `str`            | `None`                                                                                                                                   | `my_app.models.users.before_login`                       |
 | **TRIGGER.AFTER\_LOGIN**                    | A method to be called when an existing user logs in. This method will be called after the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept TWO parameters of session and user dict.                                                                                                                                                                                                               | `str`            | `None`                                                                                                                                   | `my_app.models.users.after_login`                        |
 | **TRIGGER.GET\_METADATA\_AUTO\_CONF\_URLS** | A hook function that returns a list of metadata Autoconf URLs. This can override the `METADATA_AUTO_CONF_URL` to enumerate all existing metadata autoconf URLs.                                                                                                                                                                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_metadata_autoconf_urls`         |
 | **TRIGGER.CUSTOM\_DECODE\_JWT**             | A hook function to decode the user JWT. This method will be called instead of the `decode_jwt_token` default function and should return the user_model.USERNAME_FIELD. This method accepts one parameter: `token`.                                                                                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.decode_custom_token`                |
 | **TRIGGER.CUSTOM\_CREATE\_JWT**             | A hook function to create a custom JWT for the user. This method will be called instead of the `create_jwt_token` default function and should return the token. This method accepts one parameter: `user`.                                                                                                                                                                                                                                                  | `str`            | `None`                                                                                                                                   | `my_app.models.users.create_custom_token`                |
 | **TRIGGER.CUSTOM\_TOKEN\_QUERY**            | A hook function to create a custom query params with the JWT for the user. This method will be called after `CUSTOM_CREATE_JWT` to populate a query and attach it to a URL; should return the query params containing the token (e.g., `?token=encoded.jwt.token`). This method accepts one parameter: `token`.                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_custom_token_query`             |
@@ -229,26 +222,26 @@
 | **JWT\_ALGORITHM**                          | JWT algorithm (str) to sign the message with: [supported algorithms](https://pyjwt.readthedocs.io/en/stable/algorithms.html).                                                                                                                                                                                                                                                                                                                               | `str`            | `HS512` or `RS512`                                                                                                                       |                                                          |
 | **JWT\_SECRET**                             | JWT secret to sign the message if an HMAC is used with the SHA hash algorithm (`HS*`).                                                                                                                                                                                                                                                                                                                                                                      | `str`            | `None`                                                                                                                                   |                                                          |
 | **JWT\_PRIVATE\_KEY**                       | Private key (str) to sign the message with. The algorithm should be set to `RSA256` or a more secure alternative.                                                                                                                                                                                                                                                                                                                                           | `str` or `bytes` | `--- YOUR PRIVATE KEY ---`                                                                                                               |                                                          |
 | **JWT\_PRIVATE\_KEY\_PASSPHRASE**           | If your private key is encrypted, you must provide a passphrase for decryption.                                                                                                                                                                                                                                                                                                                                                                             | `str` or `bytes` | `None`                                                                                                                                   |                                                          |
 | **JWT\_PUBLIC\_KEY**                        | Public key to decode the signed JWT token.                                                                                                                                                                                                                                                                                                                                                                                                                  | `str` or `bytes` | `'--- YOUR PUBLIC KEY ---'`                                                                                                              |                                                          |
 | **JWT\_EXP**                                | JWT expiry time in seconds                                                                                                                                                                                                                                                                                                                                                                                                                                  | `int`            | 60                                                                                                                                       |                                                          |
 | **FRONTEND\_URL**                           | If `USE_JWT` is `True`, you should set the URL to where your frontend is located (will default to `DEFAULT_NEXT_URL` if you fail to do so). Once the client is authenticated through the SAML SSO, your client is redirected to the `FRONTEND_URL` with the JWT token as `token` query parameter. Example: `https://app.example.com/?&token=<your.jwt.token`. With the token, your SPA can now authenticate with your API.                                  | `str`            | `admin:index`                                                                                                                            |                                                          |
-| **AUTHN\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |
-| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   | |
+| **AUTHN\_REQUESTS\_SIGNED**                 | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                               | `bool`           | `True`                                                                                                                                   |
+| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                      | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_ASSERTIONS\_SIGNED**                | Set this to `False` if your provider doesn't sign each assertion.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_RESPONSE\_SIGNED**                  | Set this to `False` if you don't want your provider to sign the response.                                                                                                                                                                                                                                                                                                                                                                                   | `bool`           | `True`                                                                                                                                   |                                                          |
 | **ACCEPTED\_TIME\_DIFF**                    | Sets the [accepted time diff](https://pysaml2.readthedocs.io/en/latest/howto/config.html#accepted-time-diff) in seconds                                                                                                                                                                                                                                                                                                                                     | `int` or `None`  | `None`                                                                                                                                   |                                                          |
 | **ALLOWED\_REDIRECT\_HOSTS**                | Allowed hosts to redirect to using the `?next=` parameter                                                                                                                                                                                                                                                                                                                                                                                                   | `list`           | `[]`                                                                                                                                     | `['https://app.example.com', 'https://api.exmaple.com']` |
 
 ### Triggers
-| **Setting name**                            | **Description**                                                                                                                             | **Interface**                                                                                 |
-|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
-| **GET\_METADATA\_AUTO\_CONF\_URLS**         | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]]  |
-| **GET\_USER_ID\_FROM\_SAML\_RESPONSE**      | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]   |
+| **Setting name**                       | **Description**                                                                                                                             | **Interface**                                                                                |
+| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
+| **GET\_METADATA\_AUTO\_CONF\_URLS**    | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]] |
+| **GET\_USER_ID\_FROM\_SAML\_RESPONSE** | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]  |
 
 
 
 ## JWT Signing Algorithm and Settings
 
 Both symmetric and asymmetric signing functions are [supported](https://pyjwt.readthedocs.io/en/stable/algorithms.html). If you want to use symmetric signing using a secret key, use either of the following algorithms plus a secret key:
 
@@ -341,7 +334,15 @@
 I created this plugin originally for Okta. The `METADATA_AUTO_CONF_URL` needed in `settings.py` can be found in the Okta Web UI by navigating to the SAML2 app's `Sign On` tab. In the `Settings` box, you should see:
 
     Identity Provider metadata is available if this application supports dynamic configuration.
 
 The `Identity Provider metadata` link is the `METADATA_AUTO_CONF_URL`.
 
 More information can be found in the [Okta Developer Documentation](https://developer.okta.com/docs/guides/saml-application-setup/overview/).
+
+## Release Process
+
+I adopted a reasonably simple release process, which is almost automated, except for two actions that needed to be taken to start a release:
+
+1. Update [setup.py](setup.py) and increase the version number in the `setup` function. Unless something backward-incompatible is introduced, only the minor version is upgraded: 3.8.0 becomes 3.9.0.
+2. Tag the `main` branch with the the `vSEMVER`, e.g. `v3.9.0`, and git-push the tag.
+3. The rest is handled in the CI/CD using GitHub Actions.
```

### Comparing `grafana_django_saml2_auth-3.8.0/README.md` & `grafana_django_saml2_auth-3.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,37 +7,26 @@
 This plugin supports both identity provider and service provider-initiated SSO:
 
 - For IdP-initiated SSO, the user should sign in to their identity provider platform, e.g., Okta, and click on the application that authorizes and redirects the user to the service provider, that is your platform.
 - For SP-initiated SSO, the user should first exist on your platform, either by signing in via the first method (IdP-initiated SSO) or any other custom solution. It can be configured to be redirected to the correct application on the identity provider platform.
 
 For IdP-initiated SSO, the user will be created if it doesn't exist. Still, for SP-initiated SSO, the user should exist in your platform for the code to detect and redirect them to the correct application on the identity provider platform.
 
-- [Django SAML2 Authentication](#django-saml2-authentication)
-  - [Project Information](#project-information)
-  - [Donate](#donate)
-  - [Installation](#installation)
-  - [How to use?](#how-to-use)
-  - [Module Settings](#module-settings)
-  - [JWT Signing Algorithm and Settings](#jwt-signing-algorithm-and-settings)
-    - [Custom token triggers](#custom-token-triggers)
-  - [Customize Error Messages](#customize-error-messages)
-  - [For Okta Users](#for-okta-users)
-
 ## Project Information
 
 - Original Author: Fang Li ([@fangli](https://github.com/fangli))
 - Maintainer: Mostafa Moradian ([@mostafa](https://github.com/mostafa))
 - Version support matrix:
     | **Python**                  | **Django** | **django-saml2-auth** |
     | --------------------------- | ---------- | --------------------- |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 2.2.x      | >=3.4.0               |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 3.2.x      | >=3.4.0               |
     | 3.8.x, 3.9.x, 3.10.x        | 4.0.x      | >=3.4.0               |
 
-- Release log is available [here](RELEASE-LOG.md).
+- Release logs are available [here](https://github.com/grafana/django-saml2-auth/releases). The old [release log file](RELEASE-LOG.md) still exist, and will be removed in future releases.
 
 - For contribution, read [contributing guide](CONTRIBUTING.md).
 
 ## CycloneDX SBOM
 
 From [v3.6.1](https://github.com/grafana/django-saml2-auth/releases/tag/v3.6.1), CycloneDX SBOMs will be generated for [requirements.txt](./requirements.txt) and [requirements_test.txt](./requirements_test.txt) and it can be accessed from the latest build of GitHub Actions for a tagged release, for example, [this one](https://github.com/grafana/django-saml2-auth/actions/runs/2245422253). The artifacts are only kept for 90 days.
 
@@ -138,14 +127,16 @@
             'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
             'groups': 'Groups',  # Optional
         },
         'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
             'SAML Group Name': 'Django Group Name',
         },
         'TRIGGER': {
+            # Optional: needs to return a User Model instance or None
+            'GET_USER': 'path.to.your.get.user.hook.method',
             'CREATE_USER': 'path.to.your.new.user.hook.method',
             'BEFORE_LOGIN': 'path.to.your.login.hook.method',
             'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
             # Optional. This is executed right before METADATA_AUTO_CONF_URL.
             # For systems with many metadata files registered allows to narrow the search scope.
             'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
             # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
@@ -184,14 +175,15 @@
 | **DEBUG**                                   | Send debug information to a log file                                                                                                                                                                                                                                                                                                                                                                                                                        | `bool`           | `False`                                                                                                                                  |                                                          |
 | **DEFAULT\_NEXT\_URL**                      | Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter `?next=` specificed in the login URL.                                                                                                                                                                                                                                                                         | `str`            | `admin:index`                                                                                                                            | `https://app.example.com/account/login`                  |
 | **CREATE\_USER**                            | Determines if a new Django user should be created for new users                                                                                                                                                                                                                                                                                                                                                                                             | `bool`           | `True`                                                                                                                                   |                                                          |
 | **NEW\_USER\_PROFILE**                      | Default settings for newly created users                                                                                                                                                                                                                                                                                                                                                                                                                    | `dict`           | `{'USER_GROUPS': [], 'ACTIVE_STATUS': True, 'STAFF_STATUS': False, 'SUPERUSER_STATUS': False}`                                           |                                                          |
 | **ATTRIBUTES\_MAP**                         | Mapping of Django user attributes to SAML2 user attributes                                                                                                                                                                                                                                                                                                                                                                                                  | `dict`           | `{'email': 'user.email', 'username': 'user.username', 'first_name': 'user.first_name', 'last_name': 'user.last_name', 'token': 'token'}` | `{'your.field': 'SAML.field'}`                           |
 | **TOKEN\_REQUIRED**                         | Set this to `False` if you don't require the token parameter in the SAML assertion (in the attributes map)                                                                                                                                                                                                                                                                                                                                                  | `bool`           | `True`                                                                                                                                   |                                                          |
 | **TRIGGER**                                 | Hooks to trigger additional actions during user login and creation flows. These `TRIGGER` hooks are strings containing a [dotted module name](https://docs.python.org/3/tutorial/modules.html#packages) which point to a method to be called. The referenced method should accept a single argument: a dictionary of attributes and values sent by the identity provider, representing the user's identity. Triggers will be executed only if they are set. | `dict`           | `{}`                                                                                                                                     |                                                          |
+| **TRIGGER.GET\_USER**                       | A method to be called upon getting an existing user. This method will be called before the new user is logged in and is used to customize the retrieval of an existing user record. This method should accept ONE parameter of user dict and return a User model instance or none.                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.get`                                |
 | **TRIGGER.CREATE\_USER**                    | A method to be called upon new user creation. This method will be called before the new user is logged in and after the user's record is created. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                                                     | `str`            | `None`                                                                                                                                   | `my_app.models.users.create`                             |
 | **TRIGGER.BEFORE\_LOGIN**                   | A method to be called when an existing user logs in. This method will be called before the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                           | `str`            | `None`                                                                                                                                   | `my_app.models.users.before_login`                       |
 | **TRIGGER.AFTER\_LOGIN**                    | A method to be called when an existing user logs in. This method will be called after the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept TWO parameters of session and user dict.                                                                                                                                                                                                               | `str`            | `None`                                                                                                                                   | `my_app.models.users.after_login`                        |
 | **TRIGGER.GET\_METADATA\_AUTO\_CONF\_URLS** | A hook function that returns a list of metadata Autoconf URLs. This can override the `METADATA_AUTO_CONF_URL` to enumerate all existing metadata autoconf URLs.                                                                                                                                                                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_metadata_autoconf_urls`         |
 | **TRIGGER.CUSTOM\_DECODE\_JWT**             | A hook function to decode the user JWT. This method will be called instead of the `decode_jwt_token` default function and should return the user_model.USERNAME_FIELD. This method accepts one parameter: `token`.                                                                                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.decode_custom_token`                |
 | **TRIGGER.CUSTOM\_CREATE\_JWT**             | A hook function to create a custom JWT for the user. This method will be called instead of the `create_jwt_token` default function and should return the token. This method accepts one parameter: `user`.                                                                                                                                                                                                                                                  | `str`            | `None`                                                                                                                                   | `my_app.models.users.create_custom_token`                |
 | **TRIGGER.CUSTOM\_TOKEN\_QUERY**            | A hook function to create a custom query params with the JWT for the user. This method will be called after `CUSTOM_CREATE_JWT` to populate a query and attach it to a URL; should return the query params containing the token (e.g., `?token=encoded.jwt.token`). This method accepts one parameter: `token`.                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_custom_token_query`             |
@@ -202,26 +194,26 @@
 | **JWT\_ALGORITHM**                          | JWT algorithm (str) to sign the message with: [supported algorithms](https://pyjwt.readthedocs.io/en/stable/algorithms.html).                                                                                                                                                                                                                                                                                                                               | `str`            | `HS512` or `RS512`                                                                                                                       |                                                          |
 | **JWT\_SECRET**                             | JWT secret to sign the message if an HMAC is used with the SHA hash algorithm (`HS*`).                                                                                                                                                                                                                                                                                                                                                                      | `str`            | `None`                                                                                                                                   |                                                          |
 | **JWT\_PRIVATE\_KEY**                       | Private key (str) to sign the message with. The algorithm should be set to `RSA256` or a more secure alternative.                                                                                                                                                                                                                                                                                                                                           | `str` or `bytes` | `--- YOUR PRIVATE KEY ---`                                                                                                               |                                                          |
 | **JWT\_PRIVATE\_KEY\_PASSPHRASE**           | If your private key is encrypted, you must provide a passphrase for decryption.                                                                                                                                                                                                                                                                                                                                                                             | `str` or `bytes` | `None`                                                                                                                                   |                                                          |
 | **JWT\_PUBLIC\_KEY**                        | Public key to decode the signed JWT token.                                                                                                                                                                                                                                                                                                                                                                                                                  | `str` or `bytes` | `'--- YOUR PUBLIC KEY ---'`                                                                                                              |                                                          |
 | **JWT\_EXP**                                | JWT expiry time in seconds                                                                                                                                                                                                                                                                                                                                                                                                                                  | `int`            | 60                                                                                                                                       |                                                          |
 | **FRONTEND\_URL**                           | If `USE_JWT` is `True`, you should set the URL to where your frontend is located (will default to `DEFAULT_NEXT_URL` if you fail to do so). Once the client is authenticated through the SAML SSO, your client is redirected to the `FRONTEND_URL` with the JWT token as `token` query parameter. Example: `https://app.example.com/?&token=<your.jwt.token`. With the token, your SPA can now authenticate with your API.                                  | `str`            | `admin:index`                                                                                                                            |                                                          |
-| **AUTHN\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |
-| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   | |
+| **AUTHN\_REQUESTS\_SIGNED**                 | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                               | `bool`           | `True`                                                                                                                                   |
+| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                      | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_ASSERTIONS\_SIGNED**                | Set this to `False` if your provider doesn't sign each assertion.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_RESPONSE\_SIGNED**                  | Set this to `False` if you don't want your provider to sign the response.                                                                                                                                                                                                                                                                                                                                                                                   | `bool`           | `True`                                                                                                                                   |                                                          |
 | **ACCEPTED\_TIME\_DIFF**                    | Sets the [accepted time diff](https://pysaml2.readthedocs.io/en/latest/howto/config.html#accepted-time-diff) in seconds                                                                                                                                                                                                                                                                                                                                     | `int` or `None`  | `None`                                                                                                                                   |                                                          |
 | **ALLOWED\_REDIRECT\_HOSTS**                | Allowed hosts to redirect to using the `?next=` parameter                                                                                                                                                                                                                                                                                                                                                                                                   | `list`           | `[]`                                                                                                                                     | `['https://app.example.com', 'https://api.exmaple.com']` |
 
 ### Triggers
-| **Setting name**                            | **Description**                                                                                                                             | **Interface**                                                                                 |
-|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
-| **GET\_METADATA\_AUTO\_CONF\_URLS**         | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]]  |
-| **GET\_USER_ID\_FROM\_SAML\_RESPONSE**      | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]   |
+| **Setting name**                       | **Description**                                                                                                                             | **Interface**                                                                                |
+| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
+| **GET\_METADATA\_AUTO\_CONF\_URLS**    | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]] |
+| **GET\_USER_ID\_FROM\_SAML\_RESPONSE** | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]  |
 
 
 
 ## JWT Signing Algorithm and Settings
 
 Both symmetric and asymmetric signing functions are [supported](https://pyjwt.readthedocs.io/en/stable/algorithms.html). If you want to use symmetric signing using a secret key, use either of the following algorithms plus a secret key:
 
@@ -314,7 +306,15 @@
 I created this plugin originally for Okta. The `METADATA_AUTO_CONF_URL` needed in `settings.py` can be found in the Okta Web UI by navigating to the SAML2 app's `Sign On` tab. In the `Settings` box, you should see:
 
     Identity Provider metadata is available if this application supports dynamic configuration.
 
 The `Identity Provider metadata` link is the `METADATA_AUTO_CONF_URL`.
 
 More information can be found in the [Okta Developer Documentation](https://developer.okta.com/docs/guides/saml-application-setup/overview/).
+
+## Release Process
+
+I adopted a reasonably simple release process, which is almost automated, except for two actions that needed to be taken to start a release:
+
+1. Update [setup.py](setup.py) and increase the version number in the `setup` function. Unless something backward-incompatible is introduced, only the minor version is upgraded: 3.8.0 becomes 3.9.0.
+2. Tag the `main` branch with the the `vSEMVER`, e.g. `v3.9.0`, and git-push the tag.
+3. The rest is handled in the CI/CD using GitHub Actions.
```

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/errors.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/errors.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/exceptions.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/saml.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/saml.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/settings.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_saml.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_saml.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_user.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Tests for user.py
 """
 
 from typing import Any, Dict, Union
 
 import pytest
-from django.contrib.auth.models import Group
+from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group, User
 from django_saml2_auth.exceptions import SAMLAuthError
 from django_saml2_auth.user import (create_custom_or_default_jwt, create_new_user,
                                     decode_custom_or_default_jwt, get_or_create_user,
                                     get_user, get_user_id)
 from jwt.exceptions import PyJWTError
 from pytest_django.fixtures import SettingsWrapper
 
@@ -93,14 +94,24 @@
         user (Union[str, Dict[str, str]]): User information
     """
     _user = get_user(user)
     _user.first_name = "CHANGED_FIRSTNAME"
     _user.save()
 
 
+def trigger_get_user(user: Dict) -> User:
+    """Trigger function to get a user.
+
+    Args:
+        user (Union[str, Dict[str, str]]): User information
+    """
+    user_model = get_user_model()
+    return user_model.objects.get(email=user['username'])
+
+
 @pytest.mark.django_db
 def test_create_new_user_success(settings: SettingsWrapper):
     """Test create_new_user function to verify if it works and correctly joins the user to the
     respective group.
 
     Args:
         settings (SettingsWrapper): Fixture for django settings
@@ -118,14 +129,67 @@
     assert user.username == "test@example.com"
     assert user.is_active is True
     assert user.has_usable_password() is False
     assert user.groups.get(name="users") == Group.objects.get(name="users")
 
 
 @pytest.mark.django_db
+def test_create_new_user_with_dict_success(settings: SettingsWrapper):
+    """Test create_new_user function to verify if it works and correctly joins the user to the
+    respective group.
+
+    Args:
+        settings (SettingsWrapper): Fixture for django settings
+    """
+    settings.SAML2_AUTH = {
+        "NEW_USER_PROFILE": {
+            "USER_GROUPS": ["users"],
+        }
+    }
+
+    # Create a group for the users to join
+    Group.objects.create(name="users")
+    params = {
+        "first_name": "test_John",
+        "last_name": "test_Doe"
+    }
+    user = create_new_user("user_test@example.com", **params)
+    # It can also be email depending on USERNAME_FIELD setting
+    assert user.username == "user_test@example.com"
+    assert user.is_active is True
+    assert user.has_usable_password() is False
+    assert user.groups.get(name="users") == Group.objects.get(name="users")
+
+
+@pytest.mark.django_db
+def test_create_new_user_with_dict_success__no_first_and_last_name(settings: SettingsWrapper):
+    """Test create_new_user function to verify if it works and correctly joins the user to the
+    respective group.
+
+    Args:
+        settings (SettingsWrapper): Fixture for django settings
+    """
+    settings.SAML2_AUTH = {
+        "NEW_USER_PROFILE": {
+            "USER_GROUPS": ["users"],
+        }
+    }
+
+    # Create a group for the users to join
+    Group.objects.create(name="users")
+    # Create a user without first and last name (valid use-case)
+    user = create_new_user("user_test@example.com")
+    # It can also be email depending on USERNAME_FIELD setting
+    assert user.username == "user_test@example.com"
+    assert user.is_active is True
+    assert user.has_usable_password() is False
+    assert user.groups.get(name="users") == Group.objects.get(name="users")
+
+
+@pytest.mark.django_db
 def test_create_new_user_no_group_error(settings: SettingsWrapper):
     """Test create_new_user function to verify if it creates the user, but fails to join the user
     to the respective group.
 
     Args:
         settings (SettingsWrapper): Fixture for django settings
     """
@@ -213,14 +277,60 @@
     assert str(exc_info.value) == (
         "module 'django_saml2_auth.tests.test_user' has no attribute 'nonexistent_trigger'")
     assert exc_info.value.extra is not None
     assert isinstance(exc_info.value.extra["exc"], AttributeError)
 
 
 @pytest.mark.django_db
+def test_get_user_trigger_error(settings: SettingsWrapper):
+    """Test get_user function to verify if it raises an exception in case the GET_USER
+    trigger function is nonexistent.
+
+    Args:
+        settings (SettingsWrapper): Fixture for django settings
+    """
+    settings.SAML2_AUTH = {
+        "TRIGGER": {
+            "GET_USER": "django_saml2_auth.tests.test_user.nonexistent_trigger",
+        }
+    }
+    with pytest.raises(SAMLAuthError) as exc_info:
+        get_user({
+            "username": "test@example.com",
+            "first_name": "John",
+            "last_name": "Doe"
+        })
+
+    assert str(exc_info.value) == (
+        "module 'django_saml2_auth.tests.test_user' has no attribute 'nonexistent_trigger'")
+    assert exc_info.value.extra is not None
+    assert isinstance(exc_info.value.extra["exc"], AttributeError)
+
+
+@pytest.mark.django_db
+def test_get_user_trigger(settings: SettingsWrapper):
+
+    settings.SAML2_AUTH = {
+        "TRIGGER": {
+            "GET_USER": "django_saml2_auth.tests.test_user.trigger_get_user",
+        }
+    }
+    user_model = get_user_model()
+    user_model.objects.create(
+        username="test_example_com", email="test@example.com")
+    created, user = get_or_create_user({
+        "username": "test@example.com",
+        "first_name": "John",
+        "last_name": "Doe"
+    })
+    assert created is False
+    assert user.username == "test_example_com"
+
+
+@pytest.mark.django_db
 def test_get_or_create_user_trigger_change_first_name(settings: SettingsWrapper):
     """Test get_or_create_user function to verify if it correctly triggers the CREATE_USER function
     and the trigger updates the user's first name.
 
     Args:
         settings (SettingsWrapper): Fixture for django settings
     """
```

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/tests/test_utils.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/user.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,27 @@
 from django_saml2_auth.utils import run_hook
 from jwt.algorithms import (get_default_algorithms, has_crypto,
                             requires_cryptography)
 from jwt.exceptions import PyJWTError
 from pkg_resources import parse_version
 
 
-def create_new_user(email: str, firstname: str, lastname: str) -> User:
+def create_new_user(email: str,
+                    first_name: Optional[str] = None,
+                    last_name: Optional[str] = None,
+                    **kwargs) -> User:
     """Create a new user with the given information
 
     Args:
         email (str): Email
-        firstname (str): First name
-        lastname (str): Last name
+        first_name (str): First name
+        last_name (str): Last name
+
+    Keyword Args:
+        **kwargs: Additional keyword arguments
 
     Raises:
         SAMLAuthError: There was an error creating the new user.
         SAMLAuthError: There was an error joining the user to the group.
 
     Returns:
         User: Returns a new user object, usually a subclass of the the User model
@@ -44,16 +50,20 @@
     user_model = get_user_model()
 
     is_active = dictor(saml2_auth_settings, "NEW_USER_PROFILE.ACTIVE_STATUS", default=True)
     is_staff = dictor(saml2_auth_settings, "NEW_USER_PROFILE.STAFF_STATUS", default=False)
     is_superuser = dictor(saml2_auth_settings, "NEW_USER_PROFILE.SUPERUSER_STATUS", default=False)
     user_groups = dictor(saml2_auth_settings, "NEW_USER_PROFILE.USER_GROUPS", default=[])
 
+    if first_name and last_name:
+        kwargs['first_name'] = first_name
+        kwargs['last_name'] = last_name
+
     try:
-        user = user_model.objects.create_user(email, first_name=firstname, last_name=lastname)
+        user = user_model.objects.create_user(email, **kwargs)
         user.is_active = is_active
         user.is_staff = is_staff
         user.is_superuser = is_superuser
         user.save()
     except Exception as exc:
         raise SAMLAuthError("There was an error creating the new user.", extra={
             "exc": exc,
@@ -185,15 +195,24 @@
     Args:
         user (Union[str, Dict[str, str]]): Either a user_id (as str) or a cleaned user info object
 
     Returns:
         User: An instance of the User model
     """
     saml2_auth_settings = settings.SAML2_AUTH
+    get_user_custom_method = dictor(saml2_auth_settings, "TRIGGER.GET_USER")
+
     user_model = get_user_model()
+    if get_user_custom_method:
+        found_user = run_hook(get_user_custom_method, user)  # type: ignore
+        if not found_user:
+            raise user_model.DoesNotExist
+        else:
+            return found_user
+
     user_id = get_user_id(user)
 
     # Should email be case-sensitive or not. Default is False (case-insensitive).
     login_case_sensitive = dictor(saml2_auth_settings, "LOGIN_CASE_SENSITIVE", False)
     id_field = (
         user_model.USERNAME_FIELD
         if login_case_sensitive
```

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/utils.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/utils.py`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/django_saml2_auth/views.py` & `grafana_django_saml2_auth-3.9.0/django_saml2_auth/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,15 +138,20 @@
 
         # Use JWT auth to send token to frontend
         frontend_url = dictor(saml2_auth_settings, "FRONTEND_URL", next_url)
 
         return HttpResponseRedirect(frontend_url + query)
 
     if target_user.is_active:
-        model_backend = "django.contrib.auth.backends.ModelBackend"
+        # Try to load from the `AUTHENTICATION_BACKENDS` setting in settings.py
+        if hasattr(settings, "AUTHENTICATION_BACKENDS") and settings.AUTHENTICATION_BACKENDS:
+            model_backend = settings.AUTHENTICATION_BACKENDS[0]
+        else:
+            model_backend = "django.contrib.auth.backends.ModelBackend"
+
         login(request, target_user, model_backend)
 
         after_login_trigger = dictor(saml2_auth_settings, "TRIGGER.AFTER_LOGIN")
         if after_login_trigger:
             run_hook(after_login_trigger, request.session, user)  # type: ignore
     else:
         raise SAMLAuthError("The target user is inactive.", extra={
```

### Comparing `grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/PKG-INFO` & `grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-django-saml2-auth
-Version: 3.8.0
+Version: 3.9.0
 Summary: Django SAML2 Authentication Made Easy.
 Home-page: https://github.com/grafana/django-saml2-auth
 Author: Fang Li
 Author-email: surivlee+djsaml2auth@gmail.com
 Maintainer: Mostafa Moradian
 Maintainer-email: mostafa@grafana.com
 License: Apache 2.0
@@ -12,14 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,37 +35,26 @@
 This plugin supports both identity provider and service provider-initiated SSO:
 
 - For IdP-initiated SSO, the user should sign in to their identity provider platform, e.g., Okta, and click on the application that authorizes and redirects the user to the service provider, that is your platform.
 - For SP-initiated SSO, the user should first exist on your platform, either by signing in via the first method (IdP-initiated SSO) or any other custom solution. It can be configured to be redirected to the correct application on the identity provider platform.
 
 For IdP-initiated SSO, the user will be created if it doesn't exist. Still, for SP-initiated SSO, the user should exist in your platform for the code to detect and redirect them to the correct application on the identity provider platform.
 
-- [Django SAML2 Authentication](#django-saml2-authentication)
-  - [Project Information](#project-information)
-  - [Donate](#donate)
-  - [Installation](#installation)
-  - [How to use?](#how-to-use)
-  - [Module Settings](#module-settings)
-  - [JWT Signing Algorithm and Settings](#jwt-signing-algorithm-and-settings)
-    - [Custom token triggers](#custom-token-triggers)
-  - [Customize Error Messages](#customize-error-messages)
-  - [For Okta Users](#for-okta-users)
-
 ## Project Information
 
 - Original Author: Fang Li ([@fangli](https://github.com/fangli))
 - Maintainer: Mostafa Moradian ([@mostafa](https://github.com/mostafa))
 - Version support matrix:
     | **Python**                  | **Django** | **django-saml2-auth** |
     | --------------------------- | ---------- | --------------------- |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 2.2.x      | >=3.4.0               |
     | 3.7.x, 3.8.x, 3.9.x, 3.10.x | 3.2.x      | >=3.4.0               |
     | 3.8.x, 3.9.x, 3.10.x        | 4.0.x      | >=3.4.0               |
 
-- Release log is available [here](RELEASE-LOG.md).
+- Release logs are available [here](https://github.com/grafana/django-saml2-auth/releases). The old [release log file](RELEASE-LOG.md) still exist, and will be removed in future releases.
 
 - For contribution, read [contributing guide](CONTRIBUTING.md).
 
 ## CycloneDX SBOM
 
 From [v3.6.1](https://github.com/grafana/django-saml2-auth/releases/tag/v3.6.1), CycloneDX SBOMs will be generated for [requirements.txt](./requirements.txt) and [requirements_test.txt](./requirements_test.txt) and it can be accessed from the latest build of GitHub Actions for a tagged release, for example, [this one](https://github.com/grafana/django-saml2-auth/actions/runs/2245422253). The artifacts are only kept for 90 days.
 
@@ -165,14 +155,16 @@
             'token': 'Token',  # Mandatory, can be unrequired if TOKEN_REQUIRED is False
             'groups': 'Groups',  # Optional
         },
         'GROUPS_MAP': {  # Optionally allow mapping SAML2 Groups to Django Groups
             'SAML Group Name': 'Django Group Name',
         },
         'TRIGGER': {
+            # Optional: needs to return a User Model instance or None
+            'GET_USER': 'path.to.your.get.user.hook.method',
             'CREATE_USER': 'path.to.your.new.user.hook.method',
             'BEFORE_LOGIN': 'path.to.your.login.hook.method',
             'AFTER_LOGIN': 'path.to.your.after.login.hook.method',
             # Optional. This is executed right before METADATA_AUTO_CONF_URL.
             # For systems with many metadata files registered allows to narrow the search scope.
             'GET_USER_ID_FROM_SAML_RESPONSE': 'path.to.your.get.user.from.saml.hook.method',
             # This can override the METADATA_AUTO_CONF_URL to enumerate all existing metadata autoconf URLs
@@ -211,14 +203,15 @@
 | **DEBUG**                                   | Send debug information to a log file                                                                                                                                                                                                                                                                                                                                                                                                                        | `bool`           | `False`                                                                                                                                  |                                                          |
 | **DEFAULT\_NEXT\_URL**                      | Custom target redirect URL after the user get logged in. Default to /admin if not set. This setting will be overwritten if you have parameter `?next=` specificed in the login URL.                                                                                                                                                                                                                                                                         | `str`            | `admin:index`                                                                                                                            | `https://app.example.com/account/login`                  |
 | **CREATE\_USER**                            | Determines if a new Django user should be created for new users                                                                                                                                                                                                                                                                                                                                                                                             | `bool`           | `True`                                                                                                                                   |                                                          |
 | **NEW\_USER\_PROFILE**                      | Default settings for newly created users                                                                                                                                                                                                                                                                                                                                                                                                                    | `dict`           | `{'USER_GROUPS': [], 'ACTIVE_STATUS': True, 'STAFF_STATUS': False, 'SUPERUSER_STATUS': False}`                                           |                                                          |
 | **ATTRIBUTES\_MAP**                         | Mapping of Django user attributes to SAML2 user attributes                                                                                                                                                                                                                                                                                                                                                                                                  | `dict`           | `{'email': 'user.email', 'username': 'user.username', 'first_name': 'user.first_name', 'last_name': 'user.last_name', 'token': 'token'}` | `{'your.field': 'SAML.field'}`                           |
 | **TOKEN\_REQUIRED**                         | Set this to `False` if you don't require the token parameter in the SAML assertion (in the attributes map)                                                                                                                                                                                                                                                                                                                                                  | `bool`           | `True`                                                                                                                                   |                                                          |
 | **TRIGGER**                                 | Hooks to trigger additional actions during user login and creation flows. These `TRIGGER` hooks are strings containing a [dotted module name](https://docs.python.org/3/tutorial/modules.html#packages) which point to a method to be called. The referenced method should accept a single argument: a dictionary of attributes and values sent by the identity provider, representing the user's identity. Triggers will be executed only if they are set. | `dict`           | `{}`                                                                                                                                     |                                                          |
+| **TRIGGER.GET\_USER**                       | A method to be called upon getting an existing user. This method will be called before the new user is logged in and is used to customize the retrieval of an existing user record. This method should accept ONE parameter of user dict and return a User model instance or none.                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.get`                                |
 | **TRIGGER.CREATE\_USER**                    | A method to be called upon new user creation. This method will be called before the new user is logged in and after the user's record is created. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                                                     | `str`            | `None`                                                                                                                                   | `my_app.models.users.create`                             |
 | **TRIGGER.BEFORE\_LOGIN**                   | A method to be called when an existing user logs in. This method will be called before the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept ONE parameter of user dict.                                                                                                                                                                                                                           | `str`            | `None`                                                                                                                                   | `my_app.models.users.before_login`                       |
 | **TRIGGER.AFTER\_LOGIN**                    | A method to be called when an existing user logs in. This method will be called after the user is logged in and after the SAML2 identity provider returns user attributes. This method should accept TWO parameters of session and user dict.                                                                                                                                                                                                               | `str`            | `None`                                                                                                                                   | `my_app.models.users.after_login`                        |
 | **TRIGGER.GET\_METADATA\_AUTO\_CONF\_URLS** | A hook function that returns a list of metadata Autoconf URLs. This can override the `METADATA_AUTO_CONF_URL` to enumerate all existing metadata autoconf URLs.                                                                                                                                                                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_metadata_autoconf_urls`         |
 | **TRIGGER.CUSTOM\_DECODE\_JWT**             | A hook function to decode the user JWT. This method will be called instead of the `decode_jwt_token` default function and should return the user_model.USERNAME_FIELD. This method accepts one parameter: `token`.                                                                                                                                                                                                                                          | `str`            | `None`                                                                                                                                   | `my_app.models.users.decode_custom_token`                |
 | **TRIGGER.CUSTOM\_CREATE\_JWT**             | A hook function to create a custom JWT for the user. This method will be called instead of the `create_jwt_token` default function and should return the token. This method accepts one parameter: `user`.                                                                                                                                                                                                                                                  | `str`            | `None`                                                                                                                                   | `my_app.models.users.create_custom_token`                |
 | **TRIGGER.CUSTOM\_TOKEN\_QUERY**            | A hook function to create a custom query params with the JWT for the user. This method will be called after `CUSTOM_CREATE_JWT` to populate a query and attach it to a URL; should return the query params containing the token (e.g., `?token=encoded.jwt.token`). This method accepts one parameter: `token`.                                                                                                                                             | `str`            | `None`                                                                                                                                   | `my_app.models.users.get_custom_token_query`             |
@@ -229,26 +222,26 @@
 | **JWT\_ALGORITHM**                          | JWT algorithm (str) to sign the message with: [supported algorithms](https://pyjwt.readthedocs.io/en/stable/algorithms.html).                                                                                                                                                                                                                                                                                                                               | `str`            | `HS512` or `RS512`                                                                                                                       |                                                          |
 | **JWT\_SECRET**                             | JWT secret to sign the message if an HMAC is used with the SHA hash algorithm (`HS*`).                                                                                                                                                                                                                                                                                                                                                                      | `str`            | `None`                                                                                                                                   |                                                          |
 | **JWT\_PRIVATE\_KEY**                       | Private key (str) to sign the message with. The algorithm should be set to `RSA256` or a more secure alternative.                                                                                                                                                                                                                                                                                                                                           | `str` or `bytes` | `--- YOUR PRIVATE KEY ---`                                                                                                               |                                                          |
 | **JWT\_PRIVATE\_KEY\_PASSPHRASE**           | If your private key is encrypted, you must provide a passphrase for decryption.                                                                                                                                                                                                                                                                                                                                                                             | `str` or `bytes` | `None`                                                                                                                                   |                                                          |
 | **JWT\_PUBLIC\_KEY**                        | Public key to decode the signed JWT token.                                                                                                                                                                                                                                                                                                                                                                                                                  | `str` or `bytes` | `'--- YOUR PUBLIC KEY ---'`                                                                                                              |                                                          |
 | **JWT\_EXP**                                | JWT expiry time in seconds                                                                                                                                                                                                                                                                                                                                                                                                                                  | `int`            | 60                                                                                                                                       |                                                          |
 | **FRONTEND\_URL**                           | If `USE_JWT` is `True`, you should set the URL to where your frontend is located (will default to `DEFAULT_NEXT_URL` if you fail to do so). Once the client is authenticated through the SAML SSO, your client is redirected to the `FRONTEND_URL` with the JWT token as `token` query parameter. Example: `https://app.example.com/?&token=<your.jwt.token`. With the token, your SPA can now authenticate with your API.                                  | `str`            | `admin:index`                                                                                                                            |                                                          |
-| **AUTHN\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |
-| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   | |
+| **AUTHN\_REQUESTS\_SIGNED**                 | Set this to `False` if your provider doesn't sign each authorization request.                                                                                                                                                                                                                                                                                                                                                                               | `bool`           | `True`                                                                                                                                   |
+| **LOGOUT\_REQUESTS\_SIGNED**                | Set this to `False` if your provider doesn't sign each logout request.                                                                                                                                                                                                                                                                                                                                                                                      | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_ASSERTIONS\_SIGNED**                | Set this to `False` if your provider doesn't sign each assertion.                                                                                                                                                                                                                                                                                                                                                                                           | `bool`           | `True`                                                                                                                                   |                                                          |
 | **WANT\_RESPONSE\_SIGNED**                  | Set this to `False` if you don't want your provider to sign the response.                                                                                                                                                                                                                                                                                                                                                                                   | `bool`           | `True`                                                                                                                                   |                                                          |
 | **ACCEPTED\_TIME\_DIFF**                    | Sets the [accepted time diff](https://pysaml2.readthedocs.io/en/latest/howto/config.html#accepted-time-diff) in seconds                                                                                                                                                                                                                                                                                                                                     | `int` or `None`  | `None`                                                                                                                                   |                                                          |
 | **ALLOWED\_REDIRECT\_HOSTS**                | Allowed hosts to redirect to using the `?next=` parameter                                                                                                                                                                                                                                                                                                                                                                                                   | `list`           | `[]`                                                                                                                                     | `['https://app.example.com', 'https://api.exmaple.com']` |
 
 ### Triggers
-| **Setting name**                            | **Description**                                                                                                                             | **Interface**                                                                                 |
-|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
-| **GET\_METADATA\_AUTO\_CONF\_URLS**         | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]]  |
-| **GET\_USER_ID\_FROM\_SAML\_RESPONSE**      | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]   |
+| **Setting name**                       | **Description**                                                                                                                             | **Interface**                                                                                |
+| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
+| **GET\_METADATA\_AUTO\_CONF\_URLS**    | Auto SAML2 metadata configuration URL                                                                                                       | get_metadata_auto_conf_urls(user_id: Optional[str] = None) -> Optional[List[Dict[str, str]]] |
+| **GET\_USER_ID\_FROM\_SAML\_RESPONSE** | Allows retrieving a user ID before GET_METADATA_AUTO_CONF_URLS gets triggered. Warning: SAML response still not verified. Use with caution! | get_user_id_from_saml_response(saml_response: str, user_id: Optional[str]) -> Optional[str]  |
 
 
 
 ## JWT Signing Algorithm and Settings
 
 Both symmetric and asymmetric signing functions are [supported](https://pyjwt.readthedocs.io/en/stable/algorithms.html). If you want to use symmetric signing using a secret key, use either of the following algorithms plus a secret key:
 
@@ -341,7 +334,15 @@
 I created this plugin originally for Okta. The `METADATA_AUTO_CONF_URL` needed in `settings.py` can be found in the Okta Web UI by navigating to the SAML2 app's `Sign On` tab. In the `Settings` box, you should see:
 
     Identity Provider metadata is available if this application supports dynamic configuration.
 
 The `Identity Provider metadata` link is the `METADATA_AUTO_CONF_URL`.
 
 More information can be found in the [Okta Developer Documentation](https://developer.okta.com/docs/guides/saml-application-setup/overview/).
+
+## Release Process
+
+I adopted a reasonably simple release process, which is almost automated, except for two actions that needed to be taken to start a release:
+
+1. Update [setup.py](setup.py) and increase the version number in the `setup` function. Unless something backward-incompatible is introduced, only the minor version is upgraded: 3.8.0 becomes 3.9.0.
+2. Tag the `main` branch with the the `vSEMVER`, e.g. `v3.9.0`, and git-push the tag.
+3. The rest is handled in the CI/CD using GitHub Actions.
```

### Comparing `grafana_django_saml2_auth-3.8.0/grafana_django_saml2_auth.egg-info/SOURCES.txt` & `grafana_django_saml2_auth-3.9.0/grafana_django_saml2_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana_django_saml2_auth-3.8.0/setup.py` & `grafana_django_saml2_auth-3.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Extract requirements from requirements.txt
 requirements = [r.rstrip() for r in open("requirements.txt").readlines()]
 
 setup(
     name="grafana_django_saml2_auth",
 
-    version="3.8.0",
+    version="3.9.0",
 
     description="Django SAML2 Authentication Made Easy.",
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     url="https://github.com/grafana/django-saml2-auth",
 
@@ -42,14 +42,15 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
 
         "License :: OSI Approved :: Apache Software License",
 
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
 
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
```

