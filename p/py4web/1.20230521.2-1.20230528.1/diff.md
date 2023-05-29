# Comparing `tmp/py4web-1.20230521.2.tar.gz` & `tmp/py4web-1.20230528.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230521.2.tar", last modified: Mon May 22 06:14:22 2023, max compression
+gzip compressed data, was "py4web-1.20230528.1.tar", last modified: Mon May 29 04:17:13 2023, max compression
```

## Comparing `py4web-1.20230521.2.tar` & `py4web-1.20230528.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230521.2/LICENSE.md
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 06:14:22.651144 py4web-1.20230521.2/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230521.2/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.631138 py4web-1.20230521.2/py4web/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      721 2023-05-22 06:13:47.000000 py4web-1.20230521.2/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.643141 py4web-1.20230521.2/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995779 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4356813 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1385465 2023-05-22 06:14:11.000000 py4web-1.20230521.2/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67416 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.647143 py4web-1.20230521.2/py4web/utils/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    69608 2023-05-22 05:41:10.000000 py4web-1.20230521.2/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/py4web/utils/auth_plugins/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2github.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/pam.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/misc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/recaptcha.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230521.2/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.631138 py4web-1.20230521.2/py4web.egg-info/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7692 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1830 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/SOURCES.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/dependency_links.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       43 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/entry_points.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      239 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/requires.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        7 2023-05-22 06:14:22.000000 py4web-1.20230521.2/py4web.egg-info/top_level.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1211 2023-05-22 06:13:31.000000 py4web-1.20230521.2/pyproject.toml
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-05-22 06:14:22.655145 py4web-1.20230521.2/setup.cfg
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 06:14:22.651144 py4web-1.20230521.2/tests/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_action.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_auth.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_cache.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_fixture.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_get_error_snapshot.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_json.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_main.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_session.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_template.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230521.2/tests/test_url.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.946053 py4web-1.20230528.1/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20230528.1/LICENSE.md
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     7692 2023-05-29 04:17:13.946053 py4web-1.20230528.1/PKG-INFO
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     7120 2023-05-08 00:39:42.000000 py4web-1.20230528.1/README.rst
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.934054 py4web-1.20230528.1/py4web/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      721 2023-05-28 21:05:21.000000 py4web-1.20230528.1/py4web/__init__.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.942053 py4web-1.20230528.1/py4web/assets/
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  2995779 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)   187155 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  4356813 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     5245 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)    21524 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)  1385465 2023-05-29 04:17:06.000000 py4web-1.20230528.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    67479 2023-05-28 21:03:23.000000 py4web-1.20230528.1/py4web/core.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     7510 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/server_adapters.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.946053 py4web-1.20230528.1/py4web/utils/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    69608 2023-05-22 05:41:10.000000 py4web-1.20230528.1/py4web/utils/auth.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.946053 py4web-1.20230528.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6207 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      798 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1441 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    35513 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      514 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2084 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6090 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     5051 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6672 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2848 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/cors.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1628 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2075 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3142 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/factories.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    35844 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/form.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    68937 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/grid.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1651 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    34865 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     9196 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/misc.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/param.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)    18269 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/populate.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1694 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2225 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3728 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/security.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      158 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/tags.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     6554 2023-05-08 00:39:45.000000 py4web-1.20230528.1/py4web/utils/url_signer.py
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.934054 py4web-1.20230528.1/py4web.egg-info/
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     7692 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/PKG-INFO
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)     1847 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)        1 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)       43 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/entry_points.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)      239 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/requires.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)        7 2023-05-29 04:17:13.000000 py4web-1.20230528.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      843 2023-05-28 21:05:01.000000 py4web-1.20230528.1/pyproject.toml
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)      466 2023-05-29 04:13:06.000000 py4web-1.20230528.1/requirements.txt
+-rw-rw-r--   0 mdp       (1000) mdp       (1000)       38 2023-05-29 04:17:13.946053 py4web-1.20230528.1/setup.cfg
+drwxrwxr-x   0 mdp       (1000) mdp       (1000)        0 2023-05-29 04:17:13.946053 py4web-1.20230528.1/tests/
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     3462 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_action.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     8508 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_auth.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     2025 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_cache.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1619 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_fixture.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      654 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_form.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      634 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     1043 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_json.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      847 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_main.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)     4545 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_session.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      989 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_tags.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      396 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_template.py
+-rw-r--r--   0 mdp       (1000) mdp       (1000)      392 2023-05-08 00:39:45.000000 py4web-1.20230528.1/tests/test_url.py
```

### Comparing `py4web-1.20230521.2/LICENSE.md` & `py4web-1.20230528.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/PKG-INFO` & `py4web-1.20230528.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230521.2
+Version: 1.20230528.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230521.2/README.rst` & `py4web-1.20230528.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/__init__.py` & `py4web-1.20230528.1/py4web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230521.2"
+__version__ = "1.20230528.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,381 +1,381 @@
 Zip file size: 2995779 bytes, number of entries: 379
--rw-rw-r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
--rw-rw-r--  3.0 unx     8089 tx defN 23-May-08 00:39 static/components/mtable.js
--rw-rw-r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
--rw-rw-r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
--rw-rw-r--  3.0 unx    12305 bx defN 23-May-08 00:39 static/images/alert-blue.gif
--rw-rw-r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
--rw-rw-r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
--rw-rw-r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
--rw-rw-r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
--rw-rw-r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
--rw-rw-r--  3.0 unx     5926 tx defN 23-May-08 00:39 static/css/future.css
--rw-rw-r--  3.0 unx      708 tx defN 23-May-08 00:39 static/css/gitlog.min.css
--rw-rw-r--  3.0 unx    10467 tx defN 23-May-08 00:39 static/js/index.js
--rw-rw-r--  3.0 unx     3362 tx defN 23-May-08 00:39 static/js/translations.js
--rw-rw-r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
--rw-rw-r--  3.0 unx     8947 tx defN 23-May-08 00:39 static/js/ace/mode-d.js
--rw-rw-r--  3.0 unx   470435 tx defN 23-May-08 00:39 static/js/ace/mode-php.js
--rw-rw-r--  3.0 unx     6495 tx defN 23-May-08 00:39 static/js/ace/mode-rust.js
--rw-rw-r--  3.0 unx     4933 tx defN 23-May-08 00:39 static/js/ace/mode-elm.js
--rw-rw-r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/ext-elastic_tabstops_lite.js
--rw-rw-r--  3.0 unx    58909 tx defN 23-May-08 00:39 static/js/ace/mode-curly.js
--rw-rw-r--  3.0 unx     2791 tx defN 23-May-08 00:39 static/js/ace/theme-mono_industrial.js
--rw-rw-r--  3.0 unx     2585 tx defN 23-May-08 00:39 static/js/ace/theme-textmate.js
--rw-rw-r--  3.0 unx     2712 tx defN 23-May-08 00:39 static/js/ace/theme-chrome.js
--rw-rw-r--  3.0 unx    62955 tx defN 23-May-08 00:39 static/js/ace/mode-rhtml.js
--rw-rw-r--  3.0 unx     5005 tx defN 23-May-08 00:39 static/js/ace/mode-r.js
--rw-rw-r--  3.0 unx     1762 tx defN 23-May-08 00:39 static/js/ace/mode-ada.js
--rw-rw-r--  3.0 unx     4559 tx defN 23-May-08 00:39 static/js/ace/mode-pascal.js
--rw-rw-r--  3.0 unx    30624 tx defN 23-May-08 00:39 static/js/ace/mode-ftl.js
--rw-rw-r--  3.0 unx     3818 tx defN 23-May-08 00:39 static/js/ace/ext-beautify.js
--rw-rw-r--  3.0 unx     1464 tx defN 23-May-08 00:39 static/js/ace/mode-gcode.js
--rw-rw-r--  3.0 unx  1177601 tx defN 23-May-08 00:39 static/js/ace/worker-xquery.js
--rw-rw-r--  3.0 unx    49991 tx defN 23-May-08 00:39 static/js/ace/mode-jade.js
--rw-rw-r--  3.0 unx    20085 tx defN 23-May-08 00:39 static/js/ace/mode-less.js
--rw-rw-r--  3.0 unx    63640 tx defN 23-May-08 00:39 static/js/ace/mode-autohotkey.js
--rw-rw-r--  3.0 unx     3189 tx defN 23-May-08 00:39 static/js/ace/mode-mipsassembler.js
--rw-rw-r--  3.0 unx     2819 tx defN 23-May-08 00:39 static/js/ace/ext-static_highlight.js
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/js/ace/mode-text.js
--rw-rw-r--  3.0 unx     2409 tx defN 23-May-08 00:39 static/js/ace/mode-diff.js
--rw-rw-r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/mode-space.js
--rw-rw-r--  3.0 unx     2313 tx defN 23-May-08 00:39 static/js/ace/mode-cobol.js
--rw-rw-r--  3.0 unx     4193 tx defN 23-May-08 00:39 static/js/ace/ext-split.js
--rw-rw-r--  3.0 unx     3024 tx defN 23-May-08 00:39 static/js/ace/mode-rst.js
--rw-rw-r--  3.0 unx     3031 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_blue.js
--rw-rw-r--  3.0 unx    40358 tx defN 23-May-08 00:39 static/js/ace/mode-mask.js
--rw-rw-r--  3.0 unx    16415 tx defN 23-May-08 00:39 static/js/ace/mode-sqlserver.js
--rw-rw-r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-yaml.js
--rw-rw-r--  3.0 unx     2556 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow.js
--rw-rw-r--  3.0 unx    20545 tx defN 23-May-08 00:39 static/js/ace/mode-actionscript.js
--rw-rw-r--  3.0 unx    61525 tx defN 23-May-08 00:39 static/js/ace/mode-twig.js
--rw-rw-r--  3.0 unx     6913 tx defN 23-May-08 00:39 static/js/ace/mode-golang.js
--rw-rw-r--  3.0 unx    32911 tx defN 23-May-08 00:39 static/js/ace/worker-json.js
--rw-rw-r--  3.0 unx     3729 tx defN 23-May-08 00:39 static/js/ace/ext-modelist.js
--rw-rw-r--  3.0 unx     2087 tx defN 23-May-08 00:39 static/js/ace/mode-textile.js
--rw-rw-r--  3.0 unx     6120 tx defN 23-May-08 00:39 static/js/ace/mode-tcl.js
--rw-rw-r--  3.0 unx    61356 tx defN 23-May-08 00:39 static/js/ace/mode-smarty.js
--rw-rw-r--  3.0 unx     3138 tx defN 23-May-08 00:39 static/js/ace/theme-dreamweaver.js
--rw-rw-r--  3.0 unx     4104 bx defN 23-May-08 00:39 static/js/ace/mode-c9search.js
--rw-rw-r--  3.0 unx    11837 tx defN 23-May-08 00:39 static/js/ace/mode-kotlin.js
--rw-rw-r--  3.0 unx     2312 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_dark.js
--rw-rw-r--  3.0 unx    55541 tx defN 23-May-08 00:39 static/js/ace/worker-xml.js
--rw-rw-r--  3.0 unx     2844 tx defN 23-May-08 00:39 static/js/ace/mode-eiffel.js
--rw-rw-r--  3.0 unx   140879 tx defN 23-May-08 00:39 static/js/ace/worker-css.js
--rw-rw-r--  3.0 unx     2081 tx defN 23-May-08 00:39 static/js/ace/theme-clouds.js
--rw-rw-r--  3.0 unx    21273 tx defN 23-May-08 00:39 static/js/ace/mode-sjs.js
--rw-rw-r--  3.0 unx     8226 tx defN 23-May-08 00:39 static/js/ace/mode-dockerfile.js
--rw-rw-r--  3.0 unx     3658 tx defN 23-May-08 00:39 static/js/ace/mode-scheme.js
--rw-rw-r--  3.0 unx    19962 tx defN 23-May-08 00:39 static/js/ace/mode-live_script.js
--rw-rw-r--  3.0 unx   232939 tx defN 23-May-08 00:39 static/js/ace/mode-jsoniq.js
--rw-rw-r--  3.0 unx     6540 tx defN 23-May-08 00:39 static/js/ace/mode-haxe.js
--rw-rw-r--  3.0 unx    20269 tx defN 23-May-08 00:39 static/js/ace/mode-wollok.js
--rw-rw-r--  3.0 unx     3126 tx defN 23-May-08 00:39 static/js/ace/theme-katzenmilch.js
--rw-rw-r--  3.0 unx     6476 tx defN 23-May-08 00:39 static/js/ace/theme-iplastic.js
--rw-rw-r--  3.0 unx     7382 tx defN 23-May-08 00:39 static/js/ace/mode-perl.js
--rw-rw-r--  3.0 unx    24465 tx defN 23-May-08 00:39 static/js/ace/keybinding-emacs.js
--rw-rw-r--  3.0 unx    15753 tx defN 23-May-08 00:39 static/js/ace/mode-elixir.js
--rw-rw-r--  3.0 unx     2380 tx defN 23-May-08 00:39 static/js/ace/mode-gherkin.js
--rw-rw-r--  3.0 unx    21805 tx defN 23-May-08 00:39 static/js/ace/mode-java.js
--rw-rw-r--  3.0 unx    34689 tx defN 23-May-08 00:39 static/js/ace/mode-jsp.js
--rw-rw-r--  3.0 unx     2892 tx defN 23-May-08 00:39 static/js/ace/theme-sqlserver.js
--rw-rw-r--  3.0 unx     8840 tx defN 23-May-08 00:39 static/js/ace/mode-csharp.js
--rw-rw-r--  3.0 unx    20332 tx defN 23-May-08 00:39 static/js/ace/mode-gobstones.js
--rw-rw-r--  3.0 unx     8367 tx defN 23-May-08 00:39 static/js/ace/mode-prolog.js
--rw-rw-r--  3.0 unx     2499 tx defN 23-May-08 00:39 static/js/ace/theme-twilight.js
--rw-rw-r--  3.0 unx     1099 tx defN 23-May-08 00:39 static/js/ace/mode-properties.js
--rw-rw-r--  3.0 unx    62630 tx defN 23-May-08 00:39 static/js/ace/mode-velocity.js
--rw-rw-r--  3.0 unx    12235 tx defN 23-May-08 00:39 static/js/ace/mode-stylus.js
--rw-rw-r--  3.0 unx    57890 tx defN 23-May-08 00:39 static/js/ace/mode-html.js
--rw-rw-r--  3.0 unx   164518 tx defN 23-May-08 00:39 static/js/ace/worker-javascript.js
--rw-rw-r--  3.0 unx    32692 tx defN 23-May-08 00:39 static/js/ace/mode-powershell.js
--rw-rw-r--  3.0 unx     5970 tx defN 23-May-08 00:39 static/js/ace/mode-hjson.js
--rw-rw-r--  3.0 unx     3874 tx defN 23-May-08 00:39 static/js/ace/mode-latex.js
--rw-rw-r--  3.0 unx     1918 tx defN 23-May-08 00:39 static/js/ace/theme-xcode.js
--rw-rw-r--  3.0 unx    15600 tx defN 23-May-08 00:39 static/js/ace/mode-ocaml.js
--rw-rw-r--  3.0 unx     8028 tx defN 23-May-08 00:39 static/js/ace/mode-clojure.js
--rw-rw-r--  3.0 unx     6554 tx defN 23-May-08 00:39 static/js/ace/mode-makefile.js
--rw-rw-r--  3.0 unx   190654 tx defN 23-May-08 00:39 static/js/ace/worker-coffee.js
--rw-rw-r--  3.0 unx     5399 tx defN 23-May-08 00:39 static/js/ace/mode-applescript.js
--rw-rw-r--  3.0 unx     7595 tx defN 23-May-08 00:39 static/js/ace/mode-dot.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/objectivec.js
--rw-rw-r--  3.0 unx      607 tx defN 23-May-08 00:39 static/js/ace/snippets/gobstones.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/kotlin.js
--rw-rw-r--  3.0 unx      128 tx defN 23-May-08 00:39 static/js/ace/snippets/hjson.js
--rw-rw-r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/assembly_x86.js
--rw-rw-r--  3.0 unx    21279 tx defN 23-May-08 00:39 static/js/ace/snippets/ruby.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/logiql.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/text.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/html_ruby.js
--rw-rw-r--  3.0 unx     6763 tx defN 23-May-08 00:39 static/js/ace/snippets/php.js
--rw-rw-r--  3.0 unx      198 tx defN 23-May-08 00:39 static/js/ace/snippets/makefile.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/vbscript.js
--rw-rw-r--  3.0 unx      297 tx defN 23-May-08 00:39 static/js/ace/snippets/snippets.js
--rw-rw-r--  3.0 unx      448 tx defN 23-May-08 00:39 static/js/ace/snippets/haml.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/json.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/svg.js
--rw-rw-r--  3.0 unx      370 tx defN 23-May-08 00:39 static/js/ace/snippets/drools.js
--rw-rw-r--  3.0 unx     1975 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/vhdl.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/gcode.js
--rw-rw-r--  3.0 unx     3574 tx defN 23-May-08 00:39 static/js/ace/snippets/erlang.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/matlab.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/properties.js
--rw-rw-r--  3.0 unx     1219 tx defN 23-May-08 00:39 static/js/ace/snippets/io.js
--rw-rw-r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/xquery.js
--rw-rw-r--  3.0 unx      164 tx defN 23-May-08 00:39 static/js/ace/snippets/razor.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/typescript.js
--rw-rw-r--  3.0 unx      151 tx defN 23-May-08 00:39 static/js/ace/snippets/mips_assembler.js
--rw-rw-r--  3.0 unx      540 tx defN 23-May-08 00:39 static/js/ace/snippets/textile.js
--rw-rw-r--  3.0 unx     5513 tx defN 23-May-08 00:39 static/js/ace/snippets/perl.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/mel.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/applescript.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/less.js
--rw-rw-r--  3.0 unx      134 tx defN 23-May-08 00:39 static/js/ace/snippets/live_script.js
--rw-rw-r--  3.0 unx     2233 tx defN 23-May-08 00:39 static/js/ace/snippets/coffee.js
--rw-rw-r--  3.0 unx      126 tx defN 23-May-08 00:39 static/js/ace/snippets/bro.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/prolog.js
--rw-rw-r--  3.0 unx      651 tx defN 23-May-08 00:39 static/js/ace/snippets/velocity.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ini.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rdoc.js
--rw-rw-r--  3.0 unx     2973 tx defN 23-May-08 00:39 static/js/ace/snippets/actionscript.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cirru.js
--rw-rw-r--  3.0 unx    18271 tx defN 23-May-08 00:39 static/js/ace/snippets/html.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/groovy.js
--rw-rw-r--  3.0 unx    35423 tx defN 23-May-08 00:39 static/js/ace/snippets/lsl.js
--rw-rw-r--  3.0 unx     2630 tx defN 23-May-08 00:39 static/js/ace/snippets/r.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/plain_text.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/mysql.js
--rw-rw-r--  3.0 unx    19650 tx defN 23-May-08 00:39 static/js/ace/snippets/css.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/pgsql.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/lucene.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/ocaml.js
--rw-rw-r--  3.0 unx     4322 tx defN 23-May-08 00:39 static/js/ace/snippets/java.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/mushcode.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/dot.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/verilog.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/twig.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/eiffel.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/dockerfile.js
--rw-rw-r--  3.0 unx      942 tx defN 23-May-08 00:39 static/js/ace/snippets/sql.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/fortran.js
--rw-rw-r--  3.0 unx     1690 tx defN 23-May-08 00:39 static/js/ace/snippets/tcl.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/golang.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/curly.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lean.js
--rw-rw-r--  3.0 unx     2778 tx defN 23-May-08 00:39 static/js/ace/snippets/jsp.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ejs.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/swig.js
--rw-rw-r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/soy_template.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/gitignore.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/pascal.js
--rw-rw-r--  3.0 unx     1263 tx defN 23-May-08 00:39 static/js/ace/snippets/wollok.js
--rw-rw-r--  3.0 unx     2663 tx defN 23-May-08 00:39 static/js/ace/snippets/c_cpp.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/haxe.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/gherkin.js
--rw-rw-r--  3.0 unx     3672 tx defN 23-May-08 00:39 static/js/ace/snippets/python.js
--rw-rw-r--  3.0 unx      270 tx defN 23-May-08 00:39 static/js/ace/snippets/maze.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/autohotkey.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/scheme.js
--rw-rw-r--  3.0 unx      947 tx defN 23-May-08 00:39 static/js/ace/snippets/abc.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scss.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/html_elixir.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/latex.js
--rw-rw-r--  3.0 unx      127 tx defN 23-May-08 00:39 static/js/ace/snippets/nsis.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/sjs.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/jsx.js
--rw-rw-r--  3.0 unx     3636 tx defN 23-May-08 00:39 static/js/ace/snippets/tex.js
--rw-rw-r--  3.0 unx     3127 tx defN 23-May-08 00:39 static/js/ace/snippets/vala.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/tsx.js
--rw-rw-r--  3.0 unx      442 tx defN 23-May-08 00:39 static/js/ace/snippets/rst.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/scala.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/yaml.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ada.js
--rw-rw-r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/batchfile.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/smarty.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/praat.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/asciidoc.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/swift.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scad.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elm.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/glsl.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/mask.js
--rw-rw-r--  3.0 unx      508 tx defN 23-May-08 00:39 static/js/ace/snippets/lua.js
--rw-rw-r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/c9search.js
--rw-rw-r--  3.0 unx      551 tx defN 23-May-08 00:39 static/js/ace/snippets/diff.js
--rw-rw-r--  3.0 unx     2040 tx defN 23-May-08 00:39 static/js/ace/snippets/clojure.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/livescript.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rust.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/powershell.js
--rw-rw-r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/jsoniq.js
--rw-rw-r--  3.0 unx      125 tx defN 23-May-08 00:39 static/js/ace/snippets/d.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/toml.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/csharp.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lisp.js
--rw-rw-r--  3.0 unx     2139 tx defN 23-May-08 00:39 static/js/ace/snippets/sqlserver.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/nix.js
--rw-rw-r--  3.0 unx     1319 tx defN 23-May-08 00:39 static/js/ace/snippets/dart.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cobol.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jade.js
--rw-rw-r--  3.0 unx      132 tx defN 23-May-08 00:39 static/js/ace/snippets/protobuf.js
--rw-rw-r--  3.0 unx      136 tx defN 23-May-08 00:39 static/js/ace/snippets/mipsassembler.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/liquid.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jack.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/rhtml.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/handlebars.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/xml.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/abap.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elixir.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/forth.js
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/apache_conf.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/julia.js
--rw-rw-r--  3.0 unx      149 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell_cabal.js
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/stylus.js
--rw-rw-r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/sass.js
--rw-rw-r--  3.0 unx     4000 tx defN 23-May-08 00:39 static/js/ace/snippets/django.js
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/coldfusion.js
--rw-rw-r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/snippets/javascript.js
--rw-rw-r--  3.0 unx     2055 tx defN 23-May-08 00:39 static/js/ace/snippets/sh.js
--rw-rw-r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ftl.js
--rw-rw-r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/space.js
--rw-rw-r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/luapage.js
--rw-rw-r--  3.0 unx     1973 tx defN 23-May-08 00:39 static/js/ace/snippets/markdown.js
--rw-rw-r--  3.0 unx    96918 tx defN 23-May-08 00:39 static/js/ace/keybinding-vim.js
--rw-rw-r--  3.0 unx     6989 tx defN 23-May-08 00:39 static/js/ace/mode-forth.js
--rw-rw-r--  3.0 unx     7189 tx defN 23-May-08 00:39 static/js/ace/mode-sh.js
--rw-rw-r--  3.0 unx     2572 tx defN 23-May-08 00:39 static/js/ace/ext-whitespace.js
--rw-rw-r--  3.0 unx    13909 tx defN 23-May-08 00:39 static/js/ace/mode-apache_conf.js
--rw-rw-r--  3.0 unx     6712 tx defN 23-May-08 00:39 static/js/ace/mode-mushcode.js
--rw-rw-r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/mode-toml.js
--rw-rw-r--  3.0 unx     1811 tx defN 23-May-08 00:39 static/js/ace/mode-sql.js
--rw-rw-r--  3.0 unx     2088 tx defN 23-May-08 00:39 static/js/ace/mode-vhdl.js
--rw-rw-r--  3.0 unx     7283 tx defN 23-May-08 00:39 static/js/ace/mode-lua.js
--rw-rw-r--  3.0 unx     8898 tx defN 23-May-08 00:39 static/js/ace/mode-assembly_x86.js
--rw-rw-r--  3.0 unx    13008 tx defN 23-May-08 00:39 static/js/ace/mode-glsl.js
--rw-rw-r--  3.0 unx     2913 tx defN 23-May-08 00:39 static/js/ace/theme-terminal.js
--rw-rw-r--  3.0 unx     3003 tx defN 23-May-08 00:39 static/js/ace/mode-cirru.js
--rw-rw-r--  3.0 unx    22619 tx defN 23-May-08 00:39 static/js/ace/mode-scala.js
--rw-rw-r--  3.0 unx     6965 tx defN 23-May-08 00:39 static/js/ace/mode-jsx.js
--rw-rw-r--  3.0 unx    60415 tx defN 23-May-08 00:39 static/js/ace/mode-coldfusion.js
--rw-rw-r--  3.0 unx    10220 tx defN 23-May-08 00:39 static/js/ace/mode-sass.js
--rw-rw-r--  3.0 unx     2176 tx defN 23-May-08 00:39 static/js/ace/theme-github.js
--rw-rw-r--  3.0 unx    31988 tx defN 23-May-08 00:39 static/js/ace/mode-svg.js
--rw-rw-r--  3.0 unx    12951 tx defN 23-May-08 00:39 static/js/ace/mode-scss.js
--rw-rw-r--  3.0 unx   354781 tx defN 23-May-08 00:39 static/js/ace/ace.js
--rw-rw-r--  3.0 unx     2761 tx defN 23-May-08 00:39 static/js/ace/mode-tex.js
--rw-rw-r--  3.0 unx     5665 tx defN 23-May-08 00:39 static/js/ace/mode-io.js
--rw-rw-r--  3.0 unx    10785 tx defN 23-May-08 00:39 static/js/ace/mode-drools.js
--rw-rw-r--  3.0 unx     2375 tx defN 23-May-08 00:39 static/js/ace/theme-monokai.js
--rw-rw-r--  3.0 unx     2125 tx defN 23-May-08 00:39 static/js/ace/theme-eclipse.js
--rw-rw-r--  3.0 unx    12546 tx defN 23-May-08 00:39 static/js/ace/mode-protobuf.js
--rw-rw-r--  3.0 unx    10025 tx defN 23-May-08 00:39 static/js/ace/mode-ruby.js
--rw-rw-r--  3.0 unx     2842 tx defN 23-May-08 00:39 static/js/ace/theme-chaos.js
--rw-rw-r--  3.0 unx      825 tx defN 23-May-08 00:39 static/js/ace/ext-linking.js
--rw-rw-r--  3.0 unx     1088 tx defN 23-May-08 00:39 static/js/ace/ext-statusbar.js
--rw-rw-r--  3.0 unx   217401 tx defN 23-May-08 00:39 static/js/ace/worker-html.js
--rw-rw-r--  3.0 unx    10035 tx defN 23-May-08 00:39 static/js/ace/mode-nsis.js
--rw-rw-r--  3.0 unx    78297 tx defN 23-May-08 00:39 static/js/ace/worker-php.js
--rw-rw-r--  3.0 unx    54512 tx defN 23-May-08 00:39 static/js/ace/mode-objectivec.js
--rw-rw-r--  3.0 unx     1440 bx defN 23-May-08 00:39 static/js/ace/ext-spellcheck.js
--rw-rw-r--  3.0 unx    18060 tx defN 23-May-08 00:39 static/js/ace/mode-javascript.js
--rw-rw-r--  3.0 unx    10260 tx defN 23-May-08 00:39 static/js/ace/mode-praat.js
--rw-rw-r--  3.0 unx    20567 tx defN 23-May-08 00:39 static/js/ace/mode-matlab.js
--rw-rw-r--  3.0 unx      506 tx defN 23-May-08 00:39 static/js/ace/mode-plain_text.js
--rw-rw-r--  3.0 unx    24939 tx defN 23-May-08 00:39 static/js/ace/mode-mel.js
--rw-rw-r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-rdoc.js
--rw-rw-r--  3.0 unx     2820 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night.js
--rw-rw-r--  3.0 unx    22440 tx defN 23-May-08 00:39 static/js/ace/mode-groovy.js
--rw-rw-r--  3.0 unx    64800 tx defN 23-May-08 00:39 static/js/ace/mode-markdown.js
--rw-rw-r--  3.0 unx     6523 tx defN 23-May-08 00:39 static/js/ace/mode-mysql.js
--rw-rw-r--  3.0 unx     4856 tx defN 23-May-08 00:39 static/js/ace/mode-batchfile.js
--rw-rw-r--  3.0 unx      899 tx defN 23-May-08 00:39 static/js/ace/mode-gitignore.js
--rw-rw-r--  3.0 unx     7539 tx defN 23-May-08 00:39 static/js/ace/mode-julia.js
--rw-rw-r--  3.0 unx     2296 tx defN 23-May-08 00:39 static/js/ace/theme-kr_theme.js
--rw-rw-r--  3.0 unx      140 tx defN 23-May-08 00:39 static/js/ace/ext-error_marker.js
--rw-rw-r--  3.0 unx     5097 tx defN 23-May-08 00:39 static/js/ace/mode-json.js
--rw-rw-r--  3.0 unx    66385 tx defN 23-May-08 00:39 static/js/ace/mode-soy_template.js
--rw-rw-r--  3.0 unx    12293 tx defN 23-May-08 00:39 static/js/ace/ext-settings_menu.js
--rw-rw-r--  3.0 unx    16578 tx defN 23-May-08 00:39 static/js/ace/mode-vala.js
--rw-rw-r--  3.0 unx     5712 tx defN 23-May-08 00:39 static/js/ace/mode-logiql.js
--rw-rw-r--  3.0 unx     5813 tx defN 23-May-08 00:39 static/js/ace/mode-abap.js
--rw-rw-r--  3.0 unx     1961 tx defN 23-May-08 00:39 static/js/ace/mode-lisp.js
--rw-rw-r--  3.0 unx    14198 tx defN 23-May-08 00:39 static/js/ace/mode-dart.js
--rw-rw-r--  3.0 unx     1470 tx defN 23-May-08 00:39 static/js/ace/ext-themelist.js
--rw-rw-r--  3.0 unx     2248 tx defN 23-May-08 00:39 static/js/ace/theme-idle_fingers.js
--rw-rw-r--  3.0 unx    10005 tx defN 23-May-08 00:39 static/js/ace/ext-searchbox.js
--rw-rw-r--  3.0 unx     2710 tx defN 23-May-08 00:39 static/js/ace/mode-ini.js
--rw-rw-r--  3.0 unx    10840 tx defN 23-May-08 00:39 static/js/ace/mode-c_cpp.js
--rw-rw-r--  3.0 unx    47114 tx defN 23-May-08 00:39 static/js/ace/worker-lua.js
--rw-rw-r--  3.0 unx     2812 tx defN 23-May-08 00:39 static/js/ace/theme-crimson_editor.js
--rw-rw-r--  3.0 unx    20510 tx defN 23-May-08 00:39 static/js/ace/mode-tsx.js
--rw-rw-r--  3.0 unx    59769 tx defN 23-May-08 00:39 static/js/ace/mode-handlebars.js
--rw-rw-r--  3.0 unx    34464 tx defN 23-May-08 00:39 static/js/ace/ext-language_tools.js
--rw-rw-r--  3.0 unx    20198 tx defN 23-May-08 00:39 static/js/ace/mode-typescript.js
--rw-rw-r--  3.0 unx     5576 tx defN 23-May-08 00:39 static/js/ace/mode-lean.js
--rw-rw-r--  3.0 unx     2689 tx defN 23-May-08 00:39 static/js/ace/mode-verilog.js
--rw-rw-r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/theme-vibrant_ink.js
--rw-rw-r--  3.0 unx     5764 tx defN 23-May-08 00:39 static/js/ace/mode-jack.js
--rw-rw-r--  3.0 unx    30271 tx defN 23-May-08 00:39 static/js/ace/mode-liquid.js
--rw-rw-r--  3.0 unx    64984 tx defN 23-May-08 00:39 static/js/ace/mode-razor.js
--rw-rw-r--  3.0 unx     3687 tx defN 23-May-08 00:39 static/js/ace/mode-snippets.js
--rw-rw-r--  3.0 unx     4881 tx defN 23-May-08 00:39 static/js/ace/mode-maze.js
--rw-rw-r--  3.0 unx     9112 tx defN 23-May-08 00:39 static/js/ace/ext-textarea.js
--rw-rw-r--  3.0 unx    11468 tx defN 23-May-08 00:39 static/js/ace/mode-haskell.js
--rw-rw-r--  3.0 unx     6211 tx defN 23-May-08 00:39 static/js/ace/mode-bro.js
--rw-rw-r--  3.0 unx    26620 tx defN 23-May-08 00:39 static/js/ace/mode-lsl.js
--rw-rw-r--  3.0 unx    68412 tx defN 23-May-08 00:39 static/js/ace/mode-ejs.js
--rw-rw-r--  3.0 unx    27779 tx defN 23-May-08 00:39 static/js/ace/theme-ambiance.js
--rw-rw-r--  3.0 unx    11914 tx defN 23-May-08 00:39 static/js/ace/ext-old_ie.js
--rw-rw-r--  3.0 unx     1173 tx defN 23-May-08 00:39 static/js/ace/mode-lucene.js
--rw-rw-r--  3.0 unx     7416 tx defN 23-May-08 00:39 static/js/ace/mode-coffee.js
--rw-rw-r--  3.0 unx    37225 tx defN 23-May-08 00:39 static/js/ace/mode-haml.js
--rw-rw-r--  3.0 unx     2282 tx defN 23-May-08 00:39 static/js/ace/mode-haskell_cabal.js
--rw-rw-r--  3.0 unx    18046 tx defN 23-May-08 00:39 static/js/ace/mode-css.js
--rw-rw-r--  3.0 unx     2448 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore_soft.js
--rw-rw-r--  3.0 unx     5073 tx defN 23-May-08 00:39 static/js/ace/mode-vbscript.js
--rw-rw-r--  3.0 unx    68741 tx defN 23-May-08 00:39 static/js/ace/mode-html_ruby.js
--rw-rw-r--  3.0 unx    55911 tx defN 23-May-08 00:39 static/js/ace/mode-pgsql.js
--rw-rw-r--  3.0 unx     4709 tx defN 23-May-08 00:39 static/js/ace/mode-abc.js
--rw-rw-r--  3.0 unx     3221 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_eighties.js
--rw-rw-r--  3.0 unx    21478 tx defN 23-May-08 00:39 static/js/ace/ext-emmet.js
--rw-rw-r--  3.0 unx    75093 tx defN 23-May-08 00:39 static/js/ace/mode-html_elixir.js
--rw-rw-r--  3.0 unx    29711 tx defN 23-May-08 00:39 static/js/ace/mode-erlang.js
--rw-rw-r--  3.0 unx     3640 tx defN 23-May-08 00:39 static/js/ace/ext-keybinding_menu.js
--rw-rw-r--  3.0 unx     2240 tx defN 23-May-08 00:39 static/js/ace/theme-dawn.js
--rw-rw-r--  3.0 unx     8159 tx defN 23-May-08 00:39 static/js/ace/mode-asciidoc.js
--rw-rw-r--  3.0 unx     2633 tx defN 23-May-08 00:39 static/js/ace/theme-pastel_on_dark.js
--rw-rw-r--  3.0 unx    31151 tx defN 23-May-08 00:39 static/js/ace/mode-swig.js
--rw-rw-r--  3.0 unx     6929 tx defN 23-May-08 00:39 static/js/ace/mode-swift.js
--rw-rw-r--  3.0 unx     4681 tx defN 23-May-08 00:39 static/js/ace/mode-python.js
--rw-rw-r--  3.0 unx     4984 tx defN 23-May-08 00:39 static/js/ace/mode-livescript.js
--rw-rw-r--  3.0 unx     2353 tx defN 23-May-08 00:39 static/js/ace/theme-cobalt.js
--rw-rw-r--  3.0 unx    59262 tx defN 23-May-08 00:39 static/js/ace/mode-django.js
--rw-rw-r--  3.0 unx   230322 tx defN 23-May-08 00:39 static/js/ace/mode-xquery.js
--rw-rw-r--  3.0 unx     6520 tx defN 23-May-08 00:39 static/js/ace/mode-scad.js
--rw-rw-r--  3.0 unx     2432 tx defN 23-May-08 00:39 static/js/ace/theme-clouds_midnight.js
--rw-rw-r--  3.0 unx     6360 tx defN 23-May-08 00:39 static/js/ace/ext-chromevox.js
--rw-rw-r--  3.0 unx     2360 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_light.js
--rw-rw-r--  3.0 unx    13129 tx defN 23-May-08 00:39 static/js/ace/mode-nix.js
--rw-rw-r--  3.0 unx    66336 tx defN 23-May-08 00:39 static/js/ace/mode-luapage.js
--rw-rw-r--  3.0 unx     2054 tx defN 23-May-08 00:39 static/js/ace/theme-kuroir.js
--rw-rw-r--  3.0 unx     8428 tx defN 23-May-08 00:39 static/js/ace/mode-fortran.js
--rw-rw-r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore.js
--rw-rw-r--  3.0 unx     3496 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_bright.js
--rw-rw-r--  3.0 unx    11847 tx defN 23-May-08 00:39 static/js/ace/mode-xml.js
--rw-rw-r--  3.0 unx     5959 tx defN 23-May-08 00:39 static/js/ace/mode-mips_assembler.js
--rw-rw-r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
--rw-rw-r--  3.0 unx    14265 tx defN 23-May-08 00:39 static/js/axios.min.js
--rw-rw-r--  3.0 unx      484 tx defN 23-May-08 00:39 static/js/dbadmin.js
--rw-rw-r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
--rw-rw-r--  3.0 unx    88145 tx defN 23-May-08 00:39 static/js/jquery.min.js
--rw-rw-r--  3.0 unx    95432 tx defN 23-May-08 00:39 static/js/highlight.min.js
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx    20612 tx defN 23-May-22 05:34 __init__.py
--rw-rw-r--  3.0 unx     2994 tx defN 23-May-08 00:39 templates/translations.html
--rw-rw-r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx     4849 tx defN 23-May-08 00:39 templates/gitlog.html
--rw-rw-r--  3.0 unx      993 tx defN 23-May-08 00:39 templates/dbadmin.html
--rw-rw-r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
--rw-rw-r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
+-rw-r--r--  3.0 unx     3751 tx defN 23-May-22 05:34 utils.py
+-rw-r--r--  3.0 unx     8089 tx defN 23-May-08 00:39 static/components/mtable.js
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
+-rw-r--r--  3.0 unx    10467 tx defN 23-May-08 00:39 static/js/index.js
+-rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 static/js/ace/ext-themelist.js
+-rw-r--r--  3.0 unx     8367 tx defN 23-May-08 00:39 static/js/ace/mode-prolog.js
+-rw-r--r--  3.0 unx    26620 tx defN 23-May-08 00:39 static/js/ace/mode-lsl.js
+-rw-r--r--  3.0 unx    20332 tx defN 23-May-08 00:39 static/js/ace/mode-gobstones.js
+-rw-r--r--  3.0 unx     2087 tx defN 23-May-08 00:39 static/js/ace/mode-textile.js
+-rw-r--r--  3.0 unx     2585 tx defN 23-May-08 00:39 static/js/ace/theme-textmate.js
+-rw-r--r--  3.0 unx     5712 tx defN 23-May-08 00:39 static/js/ace/mode-logiql.js
+-rw-r--r--  3.0 unx  1177601 tx defN 23-May-08 00:39 static/js/ace/worker-xquery.js
+-rw-r--r--  3.0 unx   164518 tx defN 23-May-08 00:39 static/js/ace/worker-javascript.js
+-rw-r--r--  3.0 unx     2176 tx defN 23-May-08 00:39 static/js/ace/theme-github.js
+-rw-r--r--  3.0 unx     2240 tx defN 23-May-08 00:39 static/js/ace/theme-dawn.js
+-rw-r--r--  3.0 unx     4933 tx defN 23-May-08 00:39 static/js/ace/mode-elm.js
+-rw-r--r--  3.0 unx    24939 tx defN 23-May-08 00:39 static/js/ace/mode-mel.js
+-rw-r--r--  3.0 unx    40358 tx defN 23-May-08 00:39 static/js/ace/mode-mask.js
+-rw-r--r--  3.0 unx     4193 tx defN 23-May-08 00:39 static/js/ace/ext-split.js
+-rw-r--r--  3.0 unx     5813 tx defN 23-May-08 00:39 static/js/ace/mode-abap.js
+-rw-r--r--  3.0 unx     2791 tx defN 23-May-08 00:39 static/js/ace/theme-mono_industrial.js
+-rw-r--r--  3.0 unx     1961 tx defN 23-May-08 00:39 static/js/ace/mode-lisp.js
+-rw-r--r--  3.0 unx    29711 tx defN 23-May-08 00:39 static/js/ace/mode-erlang.js
+-rw-r--r--  3.0 unx     7189 tx defN 23-May-08 00:39 static/js/ace/mode-sh.js
+-rw-r--r--  3.0 unx    68412 tx defN 23-May-08 00:39 static/js/ace/mode-ejs.js
+-rw-r--r--  3.0 unx   190654 tx defN 23-May-08 00:39 static/js/ace/worker-coffee.js
+-rw-r--r--  3.0 unx    37225 tx defN 23-May-08 00:39 static/js/ace/mode-haml.js
+-rw-r--r--  3.0 unx     1464 tx defN 23-May-08 00:39 static/js/ace/mode-gcode.js
+-rw-r--r--  3.0 unx     2820 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night.js
+-rw-r--r--  3.0 unx     3640 tx defN 23-May-08 00:39 static/js/ace/ext-keybinding_menu.js
+-rw-r--r--  3.0 unx     2892 tx defN 23-May-08 00:39 static/js/ace/theme-sqlserver.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/mode-space.js
+-rw-r--r--  3.0 unx     5970 tx defN 23-May-08 00:39 static/js/ace/mode-hjson.js
+-rw-r--r--  3.0 unx    12546 tx defN 23-May-08 00:39 static/js/ace/mode-protobuf.js
+-rw-r--r--  3.0 unx     3138 tx defN 23-May-08 00:39 static/js/ace/theme-dreamweaver.js
+-rw-r--r--  3.0 unx     1099 tx defN 23-May-08 00:39 static/js/ace/mode-properties.js
+-rw-r--r--  3.0 unx    14198 tx defN 23-May-08 00:39 static/js/ace/mode-dart.js
+-rw-r--r--  3.0 unx    60415 tx defN 23-May-08 00:39 static/js/ace/mode-coldfusion.js
+-rw-r--r--  3.0 unx     4709 tx defN 23-May-08 00:39 static/js/ace/mode-abc.js
+-rw-r--r--  3.0 unx    10260 tx defN 23-May-08 00:39 static/js/ace/mode-praat.js
+-rw-r--r--  3.0 unx     7539 tx defN 23-May-08 00:39 static/js/ace/mode-julia.js
+-rw-r--r--  3.0 unx     2913 tx defN 23-May-08 00:39 static/js/ace/theme-terminal.js
+-rw-r--r--  3.0 unx     2409 tx defN 23-May-08 00:39 static/js/ace/mode-diff.js
+-rw-r--r--  3.0 unx    12293 tx defN 23-May-08 00:39 static/js/ace/ext-settings_menu.js
+-rw-r--r--  3.0 unx    10785 tx defN 23-May-08 00:39 static/js/ace/mode-drools.js
+-rw-r--r--  3.0 unx    55541 tx defN 23-May-08 00:39 static/js/ace/worker-xml.js
+-rw-r--r--  3.0 unx    64984 tx defN 23-May-08 00:39 static/js/ace/mode-razor.js
+-rw-r--r--  3.0 unx    66385 tx defN 23-May-08 00:39 static/js/ace/mode-soy_template.js
+-rw-r--r--  3.0 unx    19962 tx defN 23-May-08 00:39 static/js/ace/mode-live_script.js
+-rw-r--r--  3.0 unx   230322 tx defN 23-May-08 00:39 static/js/ace/mode-xquery.js
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/js/ace/mode-text.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-yaml.js
+-rw-r--r--  3.0 unx     6989 tx defN 23-May-08 00:39 static/js/ace/mode-forth.js
+-rw-r--r--  3.0 unx     2633 tx defN 23-May-08 00:39 static/js/ace/theme-pastel_on_dark.js
+-rw-r--r--  3.0 unx   354781 tx defN 23-May-08 00:39 static/js/ace/ace.js
+-rw-r--r--  3.0 unx     1762 tx defN 23-May-08 00:39 static/js/ace/mode-ada.js
+-rw-r--r--  3.0 unx     6211 tx defN 23-May-08 00:39 static/js/ace/mode-bro.js
+-rw-r--r--  3.0 unx     8898 tx defN 23-May-08 00:39 static/js/ace/mode-assembly_x86.js
+-rw-r--r--  3.0 unx    31988 tx defN 23-May-08 00:39 static/js/ace/mode-svg.js
+-rw-r--r--  3.0 unx     6913 tx defN 23-May-08 00:39 static/js/ace/mode-golang.js
+-rw-r--r--  3.0 unx    24465 tx defN 23-May-08 00:39 static/js/ace/keybinding-emacs.js
+-rw-r--r--  3.0 unx     9112 tx defN 23-May-08 00:39 static/js/ace/ext-textarea.js
+-rw-r--r--  3.0 unx     2054 tx defN 23-May-08 00:39 static/js/ace/theme-kuroir.js
+-rw-r--r--  3.0 unx    20269 tx defN 23-May-08 00:39 static/js/ace/mode-wollok.js
+-rw-r--r--  3.0 unx    20567 tx defN 23-May-08 00:39 static/js/ace/mode-matlab.js
+-rw-r--r--  3.0 unx    20085 tx defN 23-May-08 00:39 static/js/ace/mode-less.js
+-rw-r--r--  3.0 unx     2088 tx defN 23-May-08 00:39 static/js/ace/mode-vhdl.js
+-rw-r--r--  3.0 unx     2572 tx defN 23-May-08 00:39 static/js/ace/ext-whitespace.js
+-rw-r--r--  3.0 unx     8226 tx defN 23-May-08 00:39 static/js/ace/mode-dockerfile.js
+-rw-r--r--  3.0 unx     2312 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_dark.js
+-rw-r--r--  3.0 unx     4984 tx defN 23-May-08 00:39 static/js/ace/mode-livescript.js
+-rw-r--r--  3.0 unx     5399 tx defN 23-May-08 00:39 static/js/ace/mode-applescript.js
+-rw-r--r--  3.0 unx    10005 tx defN 23-May-08 00:39 static/js/ace/ext-searchbox.js
+-rw-r--r--  3.0 unx     6965 tx defN 23-May-08 00:39 static/js/ace/mode-jsx.js
+-rw-r--r--  3.0 unx    66336 tx defN 23-May-08 00:39 static/js/ace/mode-luapage.js
+-rw-r--r--  3.0 unx    10840 tx defN 23-May-08 00:39 static/js/ace/mode-c_cpp.js
+-rw-r--r--  3.0 unx     7416 tx defN 23-May-08 00:39 static/js/ace/mode-coffee.js
+-rw-r--r--  3.0 unx    58909 tx defN 23-May-08 00:39 static/js/ace/mode-curly.js
+-rw-r--r--  3.0 unx    20510 tx defN 23-May-08 00:39 static/js/ace/mode-tsx.js
+-rw-r--r--  3.0 unx    13909 tx defN 23-May-08 00:39 static/js/ace/mode-apache_conf.js
+-rw-r--r--  3.0 unx    59769 tx defN 23-May-08 00:39 static/js/ace/mode-handlebars.js
+-rw-r--r--  3.0 unx     3031 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_blue.js
+-rw-r--r--  3.0 unx     6476 tx defN 23-May-08 00:39 static/js/ace/theme-iplastic.js
+-rw-r--r--  3.0 unx     2296 tx defN 23-May-08 00:39 static/js/ace/theme-kr_theme.js
+-rw-r--r--  3.0 unx     2710 tx defN 23-May-08 00:39 static/js/ace/mode-ini.js
+-rw-r--r--  3.0 unx     6523 tx defN 23-May-08 00:39 static/js/ace/mode-mysql.js
+-rw-r--r--  3.0 unx     2761 tx defN 23-May-08 00:39 static/js/ace/mode-tex.js
+-rw-r--r--  3.0 unx     2499 tx defN 23-May-08 00:39 static/js/ace/theme-twilight.js
+-rw-r--r--  3.0 unx     8428 tx defN 23-May-08 00:39 static/js/ace/mode-fortran.js
+-rw-r--r--  3.0 unx     5764 tx defN 23-May-08 00:39 static/js/ace/mode-jack.js
+-rw-r--r--  3.0 unx     3818 tx defN 23-May-08 00:39 static/js/ace/ext-beautify.js
+-rw-r--r--  3.0 unx      506 tx defN 23-May-08 00:39 static/js/ace/mode-plain_text.js
+-rw-r--r--  3.0 unx     3003 tx defN 23-May-08 00:39 static/js/ace/mode-cirru.js
+-rw-r--r--  3.0 unx     3126 tx defN 23-May-08 00:39 static/js/ace/theme-katzenmilch.js
+-rw-r--r--  3.0 unx     6120 tx defN 23-May-08 00:39 static/js/ace/mode-tcl.js
+-rw-r--r--  3.0 unx    57890 tx defN 23-May-08 00:39 static/js/ace/mode-html.js
+-rw-r--r--  3.0 unx     2380 tx defN 23-May-08 00:39 static/js/ace/mode-gherkin.js
+-rw-r--r--  3.0 unx     3729 tx defN 23-May-08 00:39 static/js/ace/ext-modelist.js
+-rw-r--r--  3.0 unx     2353 tx defN 23-May-08 00:39 static/js/ace/theme-cobalt.js
+-rw-r--r--  3.0 unx    18060 tx defN 23-May-08 00:39 static/js/ace/mode-javascript.js
+-rw-r--r--  3.0 unx    16415 tx defN 23-May-08 00:39 static/js/ace/mode-sqlserver.js
+-rw-r--r--  3.0 unx     2432 tx defN 23-May-08 00:39 static/js/ace/theme-clouds_midnight.js
+-rw-r--r--  3.0 unx    20545 tx defN 23-May-08 00:39 static/js/ace/mode-actionscript.js
+-rw-r--r--  3.0 unx    30271 tx defN 23-May-08 00:39 static/js/ace/mode-liquid.js
+-rw-r--r--  3.0 unx    47114 tx defN 23-May-08 00:39 static/js/ace/worker-lua.js
+-rw-r--r--  3.0 unx     6712 tx defN 23-May-08 00:39 static/js/ace/mode-mushcode.js
+-rw-r--r--  3.0 unx    34689 tx defN 23-May-08 00:39 static/js/ace/mode-jsp.js
+-rw-r--r--  3.0 unx    49991 tx defN 23-May-08 00:39 static/js/ace/mode-jade.js
+-rw-r--r--  3.0 unx     2282 tx defN 23-May-08 00:39 static/js/ace/mode-haskell_cabal.js
+-rw-r--r--  3.0 unx     3658 tx defN 23-May-08 00:39 static/js/ace/mode-scheme.js
+-rw-r--r--  3.0 unx    20198 tx defN 23-May-08 00:39 static/js/ace/mode-typescript.js
+-rw-r--r--  3.0 unx    11914 tx defN 23-May-08 00:39 static/js/ace/ext-old_ie.js
+-rw-r--r--  3.0 unx    10035 tx defN 23-May-08 00:39 static/js/ace/mode-nsis.js
+-rw-r--r--  3.0 unx    11468 tx defN 23-May-08 00:39 static/js/ace/mode-haskell.js
+-rw-r--r--  3.0 unx      899 tx defN 23-May-08 00:39 static/js/ace/mode-gitignore.js
+-rw-r--r--  3.0 unx    62955 tx defN 23-May-08 00:39 static/js/ace/mode-rhtml.js
+-rw-r--r--  3.0 unx    27779 tx defN 23-May-08 00:39 static/js/ace/theme-ambiance.js
+-rw-r--r--  3.0 unx     6929 tx defN 23-May-08 00:39 static/js/ace/mode-swift.js
+-rw-r--r--  3.0 unx     8947 tx defN 23-May-08 00:39 static/js/ace/mode-d.js
+-rw-r--r--  3.0 unx     4559 tx defN 23-May-08 00:39 static/js/ace/mode-pascal.js
+-rw-r--r--  3.0 unx     2313 tx defN 23-May-08 00:39 static/js/ace/mode-cobol.js
+-rw-r--r--  3.0 unx     2125 tx defN 23-May-08 00:39 static/js/ace/theme-eclipse.js
+-rw-r--r--  3.0 unx    78297 tx defN 23-May-08 00:39 static/js/ace/worker-php.js
+-rw-r--r--  3.0 unx   232939 tx defN 23-May-08 00:39 static/js/ace/mode-jsoniq.js
+-rw-r--r--  3.0 unx     5665 tx defN 23-May-08 00:39 static/js/ace/mode-io.js
+-rw-r--r--  3.0 unx      825 tx defN 23-May-08 00:39 static/js/ace/ext-linking.js
+-rw-r--r--  3.0 unx     2842 tx defN 23-May-08 00:39 static/js/ace/theme-chaos.js
+-rw-r--r--  3.0 unx    32911 tx defN 23-May-08 00:39 static/js/ace/worker-json.js
+-rw-r--r--  3.0 unx     2712 tx defN 23-May-08 00:39 static/js/ace/theme-chrome.js
+-rw-r--r--  3.0 unx    32692 tx defN 23-May-08 00:39 static/js/ace/mode-powershell.js
+-rw-r--r--  3.0 unx    61356 tx defN 23-May-08 00:39 static/js/ace/mode-smarty.js
+-rw-r--r--  3.0 unx     4104 bx defN 23-May-08 00:39 static/js/ace/mode-c9search.js
+-rw-r--r--  3.0 unx     5073 tx defN 23-May-08 00:39 static/js/ace/mode-vbscript.js
+-rw-r--r--  3.0 unx    18046 tx defN 23-May-08 00:39 static/js/ace/mode-css.js
+-rw-r--r--  3.0 unx    11847 tx defN 23-May-08 00:39 static/js/ace/mode-xml.js
+-rw-r--r--  3.0 unx   140879 tx defN 23-May-08 00:39 static/js/ace/worker-css.js
+-rw-r--r--  3.0 unx    21805 tx defN 23-May-08 00:39 static/js/ace/mode-java.js
+-rw-r--r--  3.0 unx     2081 tx defN 23-May-08 00:39 static/js/ace/theme-clouds.js
+-rw-r--r--  3.0 unx     2556 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow.js
+-rw-r--r--  3.0 unx    10220 tx defN 23-May-08 00:39 static/js/ace/mode-sass.js
+-rw-r--r--  3.0 unx     6554 tx defN 23-May-08 00:39 static/js/ace/mode-makefile.js
+-rw-r--r--  3.0 unx     4856 tx defN 23-May-08 00:39 static/js/ace/mode-batchfile.js
+-rw-r--r--  3.0 unx    15753 tx defN 23-May-08 00:39 static/js/ace/mode-elixir.js
+-rw-r--r--  3.0 unx    63640 tx defN 23-May-08 00:39 static/js/ace/mode-autohotkey.js
+-rw-r--r--  3.0 unx     2248 tx defN 23-May-08 00:39 static/js/ace/theme-idle_fingers.js
+-rw-r--r--  3.0 unx    13008 tx defN 23-May-08 00:39 static/js/ace/mode-glsl.js
+-rw-r--r--  3.0 unx     4681 tx defN 23-May-08 00:39 static/js/ace/mode-python.js
+-rw-r--r--  3.0 unx    13129 tx defN 23-May-08 00:39 static/js/ace/mode-nix.js
+-rw-r--r--  3.0 unx    59262 tx defN 23-May-08 00:39 static/js/ace/mode-django.js
+-rw-r--r--  3.0 unx     7283 tx defN 23-May-08 00:39 static/js/ace/mode-lua.js
+-rw-r--r--  3.0 unx     2360 tx defN 23-May-08 00:39 static/js/ace/theme-solarized_light.js
+-rw-r--r--  3.0 unx     1918 tx defN 23-May-08 00:39 static/js/ace/theme-xcode.js
+-rw-r--r--  3.0 unx     6360 tx defN 23-May-08 00:39 static/js/ace/ext-chromevox.js
+-rw-r--r--  3.0 unx    61525 tx defN 23-May-08 00:39 static/js/ace/mode-twig.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elm.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/typescript.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/handlebars.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/mysql.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cobol.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/sass.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/haxe.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ini.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/twig.js
+-rw-r--r--  3.0 unx     2040 tx defN 23-May-08 00:39 static/js/ace/snippets/clojure.js
+-rw-r--r--  3.0 unx      134 tx defN 23-May-08 00:39 static/js/ace/snippets/live_script.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/swift.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/ocaml.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/plain_text.js
+-rw-r--r--  3.0 unx     3127 tx defN 23-May-08 00:39 static/js/ace/snippets/vala.js
+-rw-r--r--  3.0 unx    35423 tx defN 23-May-08 00:39 static/js/ace/snippets/lsl.js
+-rw-r--r--  3.0 unx      942 tx defN 23-May-08 00:39 static/js/ace/snippets/sql.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/less.js
+-rw-r--r--  3.0 unx     1973 tx defN 23-May-08 00:39 static/js/ace/snippets/markdown.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/liquid.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/space.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/golang.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/properties.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/vhdl.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/vbscript.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ftl.js
+-rw-r--r--  3.0 unx     2233 tx defN 23-May-08 00:39 static/js/ace/snippets/coffee.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/lucene.js
+-rw-r--r--  3.0 unx     1319 tx defN 23-May-08 00:39 static/js/ace/snippets/dart.js
+-rw-r--r--  3.0 unx      151 tx defN 23-May-08 00:39 static/js/ace/snippets/mips_assembler.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/pgsql.js
+-rw-r--r--  3.0 unx     2630 tx defN 23-May-08 00:39 static/js/ace/snippets/r.js
+-rw-r--r--  3.0 unx      442 tx defN 23-May-08 00:39 static/js/ace/snippets/rst.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/dot.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/xml.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/scala.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/text.js
+-rw-r--r--  3.0 unx      128 tx defN 23-May-08 00:39 static/js/ace/snippets/hjson.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/asciidoc.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/apache_conf.js
+-rw-r--r--  3.0 unx      164 tx defN 23-May-08 00:39 static/js/ace/snippets/razor.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/snippets/javascript.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/scheme.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/curly.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/glsl.js
+-rw-r--r--  3.0 unx      370 tx defN 23-May-08 00:39 static/js/ace/snippets/drools.js
+-rw-r--r--  3.0 unx     2055 tx defN 23-May-08 00:39 static/js/ace/snippets/sh.js
+-rw-r--r--  3.0 unx      551 tx defN 23-May-08 00:39 static/js/ace/snippets/diff.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/html_ruby.js
+-rw-r--r--  3.0 unx      126 tx defN 23-May-08 00:39 static/js/ace/snippets/bro.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ejs.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/jsoniq.js
+-rw-r--r--  3.0 unx     1263 tx defN 23-May-08 00:39 static/js/ace/snippets/wollok.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/smarty.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/json.js
+-rw-r--r--  3.0 unx     2663 tx defN 23-May-08 00:39 static/js/ace/snippets/c_cpp.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/gcode.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/batchfile.js
+-rw-r--r--  3.0 unx    19650 tx defN 23-May-08 00:39 static/js/ace/snippets/css.js
+-rw-r--r--  3.0 unx     5513 tx defN 23-May-08 00:39 static/js/ace/snippets/perl.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/nix.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/abap.js
+-rw-r--r--  3.0 unx    18271 tx defN 23-May-08 00:39 static/js/ace/snippets/html.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lisp.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/verilog.js
+-rw-r--r--  3.0 unx      947 tx defN 23-May-08 00:39 static/js/ace/snippets/abc.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/kotlin.js
+-rw-r--r--  3.0 unx      508 tx defN 23-May-08 00:39 static/js/ace/snippets/lua.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/jsx.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/c9search.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/mask.js
+-rw-r--r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/assembly_x86.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jack.js
+-rw-r--r--  3.0 unx      297 tx defN 23-May-08 00:39 static/js/ace/snippets/snippets.js
+-rw-r--r--  3.0 unx      136 tx defN 23-May-08 00:39 static/js/ace/snippets/mipsassembler.js
+-rw-r--r--  3.0 unx     4000 tx defN 23-May-08 00:39 static/js/ace/snippets/django.js
+-rw-r--r--  3.0 unx      448 tx defN 23-May-08 00:39 static/js/ace/snippets/haml.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scad.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/elixir.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/toml.js
+-rw-r--r--  3.0 unx    21279 tx defN 23-May-08 00:39 static/js/ace/snippets/ruby.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/coldfusion.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/praat.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/forth.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/mel.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/groovy.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/prolog.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rdoc.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/luapage.js
+-rw-r--r--  3.0 unx     2973 tx defN 23-May-08 00:39 static/js/ace/snippets/actionscript.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/tsx.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/applescript.js
+-rw-r--r--  3.0 unx      607 tx defN 23-May-08 00:39 static/js/ace/snippets/gobstones.js
+-rw-r--r--  3.0 unx     3574 tx defN 23-May-08 00:39 static/js/ace/snippets/erlang.js
+-rw-r--r--  3.0 unx     6763 tx defN 23-May-08 00:39 static/js/ace/snippets/php.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/swig.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/pascal.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/autohotkey.js
+-rw-r--r--  3.0 unx      139 tx defN 23-May-08 00:39 static/js/ace/snippets/mushcode.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/logiql.js
+-rw-r--r--  3.0 unx      540 tx defN 23-May-08 00:39 static/js/ace/snippets/textile.js
+-rw-r--r--  3.0 unx      132 tx defN 23-May-08 00:39 static/js/ace/snippets/protobuf.js
+-rw-r--r--  3.0 unx      147 tx defN 23-May-08 00:39 static/js/ace/snippets/soy_template.js
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 static/js/ace/snippets/html_elixir.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/rust.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/sjs.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/livescript.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/julia.js
+-rw-r--r--  3.0 unx      270 tx defN 23-May-08 00:39 static/js/ace/snippets/maze.js
+-rw-r--r--  3.0 unx     3636 tx defN 23-May-08 00:39 static/js/ace/snippets/tex.js
+-rw-r--r--  3.0 unx     3672 tx defN 23-May-08 00:39 static/js/ace/snippets/python.js
+-rw-r--r--  3.0 unx      141 tx defN 23-May-08 00:39 static/js/ace/snippets/gitignore.js
+-rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 static/js/ace/snippets/jsp.js
+-rw-r--r--  3.0 unx     1975 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell.js
+-rw-r--r--  3.0 unx     1690 tx defN 23-May-08 00:39 static/js/ace/snippets/tcl.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/scss.js
+-rw-r--r--  3.0 unx     1219 tx defN 23-May-08 00:39 static/js/ace/snippets/io.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/fortran.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/svg.js
+-rw-r--r--  3.0 unx     2139 tx defN 23-May-08 00:39 static/js/ace/snippets/sqlserver.js
+-rw-r--r--  3.0 unx      137 tx defN 23-May-08 00:39 static/js/ace/snippets/gherkin.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/powershell.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/cirru.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/jade.js
+-rw-r--r--  3.0 unx      198 tx defN 23-May-08 00:39 static/js/ace/snippets/makefile.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/stylus.js
+-rw-r--r--  3.0 unx      651 tx defN 23-May-08 00:39 static/js/ace/snippets/velocity.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-May-08 00:39 static/js/ace/snippets/xquery.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/csharp.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/dockerfile.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/rhtml.js
+-rw-r--r--  3.0 unx      125 tx defN 23-May-08 00:39 static/js/ace/snippets/d.js
+-rw-r--r--  3.0 unx      133 tx defN 23-May-08 00:39 static/js/ace/snippets/latex.js
+-rw-r--r--  3.0 unx      127 tx defN 23-May-08 00:39 static/js/ace/snippets/nsis.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/matlab.js
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 static/js/ace/snippets/objectivec.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/lean.js
+-rw-r--r--  3.0 unx     4322 tx defN 23-May-08 00:39 static/js/ace/snippets/java.js
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 static/js/ace/snippets/eiffel.js
+-rw-r--r--  3.0 unx      129 tx defN 23-May-08 00:39 static/js/ace/snippets/ada.js
+-rw-r--r--  3.0 unx      149 tx defN 23-May-08 00:39 static/js/ace/snippets/haskell_cabal.js
+-rw-r--r--  3.0 unx      131 tx defN 23-May-08 00:39 static/js/ace/snippets/yaml.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-May-08 00:39 static/js/ace/ext-elastic_tabstops_lite.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore.js
+-rw-r--r--  3.0 unx     3687 tx defN 23-May-08 00:39 static/js/ace/mode-snippets.js
+-rw-r--r--  3.0 unx     2819 tx defN 23-May-08 00:39 static/js/ace/ext-static_highlight.js
+-rw-r--r--  3.0 unx    34464 tx defN 23-May-08 00:39 static/js/ace/ext-language_tools.js
+-rw-r--r--  3.0 unx     5959 tx defN 23-May-08 00:39 static/js/ace/mode-mips_assembler.js
+-rw-r--r--  3.0 unx    22440 tx defN 23-May-08 00:39 static/js/ace/mode-groovy.js
+-rw-r--r--  3.0 unx    55911 tx defN 23-May-08 00:39 static/js/ace/mode-pgsql.js
+-rw-r--r--  3.0 unx    64800 tx defN 23-May-08 00:39 static/js/ace/mode-markdown.js
+-rw-r--r--  3.0 unx     6520 tx defN 23-May-08 00:39 static/js/ace/mode-scad.js
+-rw-r--r--  3.0 unx    12235 tx defN 23-May-08 00:39 static/js/ace/mode-stylus.js
+-rw-r--r--  3.0 unx    15600 tx defN 23-May-08 00:39 static/js/ace/mode-ocaml.js
+-rw-r--r--  3.0 unx    31151 tx defN 23-May-08 00:39 static/js/ace/mode-swig.js
+-rw-r--r--  3.0 unx     6540 tx defN 23-May-08 00:39 static/js/ace/mode-haxe.js
+-rw-r--r--  3.0 unx     4881 tx defN 23-May-08 00:39 static/js/ace/mode-maze.js
+-rw-r--r--  3.0 unx    12951 tx defN 23-May-08 00:39 static/js/ace/mode-scss.js
+-rw-r--r--  3.0 unx     6495 tx defN 23-May-08 00:39 static/js/ace/mode-rust.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-May-08 00:39 static/js/ace/mode-rdoc.js
+-rw-r--r--  3.0 unx     2844 tx defN 23-May-08 00:39 static/js/ace/mode-eiffel.js
+-rw-r--r--  3.0 unx     3874 tx defN 23-May-08 00:39 static/js/ace/mode-latex.js
+-rw-r--r--  3.0 unx    22619 tx defN 23-May-08 00:39 static/js/ace/mode-scala.js
+-rw-r--r--  3.0 unx     7595 tx defN 23-May-08 00:39 static/js/ace/mode-dot.js
+-rw-r--r--  3.0 unx     7382 tx defN 23-May-08 00:39 static/js/ace/mode-perl.js
+-rw-r--r--  3.0 unx    54512 tx defN 23-May-08 00:39 static/js/ace/mode-objectivec.js
+-rw-r--r--  3.0 unx   217401 tx defN 23-May-08 00:39 static/js/ace/worker-html.js
+-rw-r--r--  3.0 unx     2448 tx defN 23-May-08 00:39 static/js/ace/theme-merbivore_soft.js
+-rw-r--r--  3.0 unx    62630 tx defN 23-May-08 00:39 static/js/ace/mode-velocity.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/theme-vibrant_ink.js
+-rw-r--r--  3.0 unx     8028 tx defN 23-May-08 00:39 static/js/ace/mode-clojure.js
+-rw-r--r--  3.0 unx   470435 tx defN 23-May-08 00:39 static/js/ace/mode-php.js
+-rw-r--r--  3.0 unx     2375 tx defN 23-May-08 00:39 static/js/ace/theme-monokai.js
+-rw-r--r--  3.0 unx    21478 tx defN 23-May-08 00:39 static/js/ace/ext-emmet.js
+-rw-r--r--  3.0 unx     8159 tx defN 23-May-08 00:39 static/js/ace/mode-asciidoc.js
+-rw-r--r--  3.0 unx     8840 tx defN 23-May-08 00:39 static/js/ace/mode-csharp.js
+-rw-r--r--  3.0 unx     3221 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_eighties.js
+-rw-r--r--  3.0 unx     1811 tx defN 23-May-08 00:39 static/js/ace/mode-sql.js
+-rw-r--r--  3.0 unx     1440 bx defN 23-May-08 00:39 static/js/ace/ext-spellcheck.js
+-rw-r--r--  3.0 unx     3496 tx defN 23-May-08 00:39 static/js/ace/theme-tomorrow_night_bright.js
+-rw-r--r--  3.0 unx    30624 tx defN 23-May-08 00:39 static/js/ace/mode-ftl.js
+-rw-r--r--  3.0 unx    96918 tx defN 23-May-08 00:39 static/js/ace/keybinding-vim.js
+-rw-r--r--  3.0 unx     3189 tx defN 23-May-08 00:39 static/js/ace/mode-mipsassembler.js
+-rw-r--r--  3.0 unx     5005 tx defN 23-May-08 00:39 static/js/ace/mode-r.js
+-rw-r--r--  3.0 unx     5576 tx defN 23-May-08 00:39 static/js/ace/mode-lean.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-May-08 00:39 static/js/ace/mode-toml.js
+-rw-r--r--  3.0 unx    68741 tx defN 23-May-08 00:39 static/js/ace/mode-html_ruby.js
+-rw-r--r--  3.0 unx     1173 tx defN 23-May-08 00:39 static/js/ace/mode-lucene.js
+-rw-r--r--  3.0 unx      140 tx defN 23-May-08 00:39 static/js/ace/ext-error_marker.js
+-rw-r--r--  3.0 unx    11837 tx defN 23-May-08 00:39 static/js/ace/mode-kotlin.js
+-rw-r--r--  3.0 unx     3024 tx defN 23-May-08 00:39 static/js/ace/mode-rst.js
+-rw-r--r--  3.0 unx    10025 tx defN 23-May-08 00:39 static/js/ace/mode-ruby.js
+-rw-r--r--  3.0 unx    16578 tx defN 23-May-08 00:39 static/js/ace/mode-vala.js
+-rw-r--r--  3.0 unx     1088 tx defN 23-May-08 00:39 static/js/ace/ext-statusbar.js
+-rw-r--r--  3.0 unx    75093 tx defN 23-May-08 00:39 static/js/ace/mode-html_elixir.js
+-rw-r--r--  3.0 unx     5097 tx defN 23-May-08 00:39 static/js/ace/mode-json.js
+-rw-r--r--  3.0 unx    21273 tx defN 23-May-08 00:39 static/js/ace/mode-sjs.js
+-rw-r--r--  3.0 unx     2812 tx defN 23-May-08 00:39 static/js/ace/theme-crimson_editor.js
+-rw-r--r--  3.0 unx     2689 tx defN 23-May-08 00:39 static/js/ace/mode-verilog.js
+-rw-r--r--  3.0 unx    95432 tx defN 23-May-08 00:39 static/js/highlight.min.js
+-rw-r--r--  3.0 unx    88145 tx defN 23-May-08 00:39 static/js/jquery.min.js
+-rw-r--r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
+-rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
+-rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    14265 tx defN 23-May-08 00:39 static/js/axios.min.js
+-rw-r--r--  3.0 unx      484 tx defN 23-May-08 00:39 static/js/dbadmin.js
+-rw-r--r--  3.0 unx     3362 tx defN 23-May-08 00:39 static/js/translations.js
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx      708 tx defN 23-May-08 00:39 static/css/gitlog.min.css
+-rw-r--r--  3.0 unx     5926 tx defN 23-May-08 00:39 static/css/future.css
+-rw-r--r--  3.0 unx    12305 bx defN 23-May-08 00:39 static/images/alert-blue.gif
+-rw-r--r--  3.0 unx  1010153 bx defN 23-May-08 00:39 static/images/widget.gif
+-rw-r--r--  3.0 unx    13380 bx defN 23-May-08 00:39 static/images/alert-yellow.gif
+-rw-r--r--  3.0 unx    12025 bx defN 23-May-08 00:39 static/images/alert-red.gif
+-rw-r--r--  3.0 unx    11068 bx defN 23-May-08 00:39 static/images/alert-green.gif
+-rw-r--r--  3.0 unx     7927 bx defN 23-May-08 00:39 static/images/forkme.png
+-rw-r--r--  3.0 unx    13366 bx defN 23-May-08 00:39 static/images/alert-orange.gif
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 translations/README.md
+-rw-r--r--  3.0 unx    20612 tx defN 23-May-22 05:34 __init__.py
+-rw-r--r--  3.0 unx     6493 tx defN 23-May-08 00:39 diff2kryten.py
+-rw-r--r--  3.0 unx     4849 tx defN 23-May-08 00:39 templates/gitlog.html
+-rw-r--r--  3.0 unx     1141 tx defN 23-May-08 00:39 templates/ticket.html
+-rw-r--r--  3.0 unx      993 tx defN 23-May-08 00:39 templates/dbadmin.html
+-rw-r--r--  3.0 unx     2994 tx defN 23-May-08 00:39 templates/translations.html
+-rw-r--r--  3.0 unx    13851 tx defN 23-May-08 00:39 templates/index.html
 379 files, 8019993 bytes uncompressed, 2924821 bytes compressed:  63.5%
```

#### zipnote {}

```diff
@@ -3,1136 +3,1136 @@
 
 Filename: static/components/mtable.js
 Comment: 
 
 Filename: static/components/mtable.html
 Comment: 
 
-Filename: static/images/alert-red.gif
+Filename: static/js/index.js
 Comment: 
 
-Filename: static/images/alert-blue.gif
+Filename: static/js/ace/ext-themelist.js
 Comment: 
 
-Filename: static/images/alert-orange.gif
+Filename: static/js/ace/mode-prolog.js
 Comment: 
 
-Filename: static/images/widget.gif
+Filename: static/js/ace/mode-lsl.js
 Comment: 
 
-Filename: static/images/forkme.png
+Filename: static/js/ace/mode-gobstones.js
 Comment: 
 
-Filename: static/images/alert-yellow.gif
+Filename: static/js/ace/mode-textile.js
 Comment: 
 
-Filename: static/images/alert-green.gif
+Filename: static/js/ace/theme-textmate.js
 Comment: 
 
-Filename: static/css/future.css
+Filename: static/js/ace/mode-logiql.js
 Comment: 
 
-Filename: static/css/gitlog.min.css
+Filename: static/js/ace/worker-xquery.js
 Comment: 
 
-Filename: static/js/index.js
+Filename: static/js/ace/worker-javascript.js
 Comment: 
 
-Filename: static/js/translations.js
+Filename: static/js/ace/theme-github.js
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/js/ace/theme-dawn.js
 Comment: 
 
-Filename: static/js/ace/mode-d.js
+Filename: static/js/ace/mode-elm.js
 Comment: 
 
-Filename: static/js/ace/mode-php.js
+Filename: static/js/ace/mode-mel.js
 Comment: 
 
-Filename: static/js/ace/mode-rust.js
+Filename: static/js/ace/mode-mask.js
 Comment: 
 
-Filename: static/js/ace/mode-elm.js
+Filename: static/js/ace/ext-split.js
 Comment: 
 
-Filename: static/js/ace/ext-elastic_tabstops_lite.js
+Filename: static/js/ace/mode-abap.js
 Comment: 
 
-Filename: static/js/ace/mode-curly.js
+Filename: static/js/ace/theme-mono_industrial.js
 Comment: 
 
-Filename: static/js/ace/theme-mono_industrial.js
+Filename: static/js/ace/mode-lisp.js
 Comment: 
 
-Filename: static/js/ace/theme-textmate.js
+Filename: static/js/ace/mode-erlang.js
 Comment: 
 
-Filename: static/js/ace/theme-chrome.js
+Filename: static/js/ace/mode-sh.js
 Comment: 
 
-Filename: static/js/ace/mode-rhtml.js
+Filename: static/js/ace/mode-ejs.js
 Comment: 
 
-Filename: static/js/ace/mode-r.js
+Filename: static/js/ace/worker-coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-ada.js
+Filename: static/js/ace/mode-haml.js
 Comment: 
 
-Filename: static/js/ace/mode-pascal.js
+Filename: static/js/ace/mode-gcode.js
 Comment: 
 
-Filename: static/js/ace/mode-ftl.js
+Filename: static/js/ace/theme-tomorrow_night.js
 Comment: 
 
-Filename: static/js/ace/ext-beautify.js
+Filename: static/js/ace/ext-keybinding_menu.js
 Comment: 
 
-Filename: static/js/ace/mode-gcode.js
+Filename: static/js/ace/theme-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/worker-xquery.js
+Filename: static/js/ace/mode-space.js
 Comment: 
 
-Filename: static/js/ace/mode-jade.js
+Filename: static/js/ace/mode-hjson.js
 Comment: 
 
-Filename: static/js/ace/mode-less.js
+Filename: static/js/ace/mode-protobuf.js
 Comment: 
 
-Filename: static/js/ace/mode-autohotkey.js
+Filename: static/js/ace/theme-dreamweaver.js
 Comment: 
 
-Filename: static/js/ace/mode-mipsassembler.js
+Filename: static/js/ace/mode-properties.js
 Comment: 
 
-Filename: static/js/ace/ext-static_highlight.js
+Filename: static/js/ace/mode-dart.js
 Comment: 
 
-Filename: static/js/ace/mode-text.js
+Filename: static/js/ace/mode-coldfusion.js
 Comment: 
 
-Filename: static/js/ace/mode-diff.js
+Filename: static/js/ace/mode-abc.js
 Comment: 
 
-Filename: static/js/ace/mode-space.js
+Filename: static/js/ace/mode-praat.js
 Comment: 
 
-Filename: static/js/ace/mode-cobol.js
+Filename: static/js/ace/mode-julia.js
 Comment: 
 
-Filename: static/js/ace/ext-split.js
+Filename: static/js/ace/theme-terminal.js
 Comment: 
 
-Filename: static/js/ace/mode-rst.js
+Filename: static/js/ace/mode-diff.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_blue.js
+Filename: static/js/ace/ext-settings_menu.js
 Comment: 
 
-Filename: static/js/ace/mode-mask.js
+Filename: static/js/ace/mode-drools.js
 Comment: 
 
-Filename: static/js/ace/mode-sqlserver.js
+Filename: static/js/ace/worker-xml.js
 Comment: 
 
-Filename: static/js/ace/mode-yaml.js
+Filename: static/js/ace/mode-razor.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow.js
+Filename: static/js/ace/mode-soy_template.js
 Comment: 
 
-Filename: static/js/ace/mode-actionscript.js
+Filename: static/js/ace/mode-live_script.js
 Comment: 
 
-Filename: static/js/ace/mode-twig.js
+Filename: static/js/ace/mode-xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-golang.js
+Filename: static/js/ace/mode-text.js
 Comment: 
 
-Filename: static/js/ace/worker-json.js
+Filename: static/js/ace/mode-yaml.js
 Comment: 
 
-Filename: static/js/ace/ext-modelist.js
+Filename: static/js/ace/mode-forth.js
 Comment: 
 
-Filename: static/js/ace/mode-textile.js
+Filename: static/js/ace/theme-pastel_on_dark.js
 Comment: 
 
-Filename: static/js/ace/mode-tcl.js
+Filename: static/js/ace/ace.js
 Comment: 
 
-Filename: static/js/ace/mode-smarty.js
+Filename: static/js/ace/mode-ada.js
 Comment: 
 
-Filename: static/js/ace/theme-dreamweaver.js
+Filename: static/js/ace/mode-bro.js
 Comment: 
 
-Filename: static/js/ace/mode-c9search.js
+Filename: static/js/ace/mode-assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/mode-kotlin.js
+Filename: static/js/ace/mode-svg.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_dark.js
+Filename: static/js/ace/mode-golang.js
 Comment: 
 
-Filename: static/js/ace/worker-xml.js
+Filename: static/js/ace/keybinding-emacs.js
 Comment: 
 
-Filename: static/js/ace/mode-eiffel.js
+Filename: static/js/ace/ext-textarea.js
 Comment: 
 
-Filename: static/js/ace/worker-css.js
+Filename: static/js/ace/theme-kuroir.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds.js
+Filename: static/js/ace/mode-wollok.js
 Comment: 
 
-Filename: static/js/ace/mode-sjs.js
+Filename: static/js/ace/mode-matlab.js
 Comment: 
 
-Filename: static/js/ace/mode-dockerfile.js
+Filename: static/js/ace/mode-less.js
 Comment: 
 
-Filename: static/js/ace/mode-scheme.js
+Filename: static/js/ace/mode-vhdl.js
 Comment: 
 
-Filename: static/js/ace/mode-live_script.js
+Filename: static/js/ace/ext-whitespace.js
 Comment: 
 
-Filename: static/js/ace/mode-jsoniq.js
+Filename: static/js/ace/mode-dockerfile.js
 Comment: 
 
-Filename: static/js/ace/mode-haxe.js
+Filename: static/js/ace/theme-solarized_dark.js
 Comment: 
 
-Filename: static/js/ace/mode-wollok.js
+Filename: static/js/ace/mode-livescript.js
 Comment: 
 
-Filename: static/js/ace/theme-katzenmilch.js
+Filename: static/js/ace/mode-applescript.js
 Comment: 
 
-Filename: static/js/ace/theme-iplastic.js
+Filename: static/js/ace/ext-searchbox.js
 Comment: 
 
-Filename: static/js/ace/mode-perl.js
+Filename: static/js/ace/mode-jsx.js
 Comment: 
 
-Filename: static/js/ace/keybinding-emacs.js
+Filename: static/js/ace/mode-luapage.js
 Comment: 
 
-Filename: static/js/ace/mode-elixir.js
+Filename: static/js/ace/mode-c_cpp.js
 Comment: 
 
-Filename: static/js/ace/mode-gherkin.js
+Filename: static/js/ace/mode-coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-java.js
+Filename: static/js/ace/mode-curly.js
 Comment: 
 
-Filename: static/js/ace/mode-jsp.js
+Filename: static/js/ace/mode-tsx.js
 Comment: 
 
-Filename: static/js/ace/theme-sqlserver.js
+Filename: static/js/ace/mode-apache_conf.js
 Comment: 
 
-Filename: static/js/ace/mode-csharp.js
+Filename: static/js/ace/mode-handlebars.js
 Comment: 
 
-Filename: static/js/ace/mode-gobstones.js
+Filename: static/js/ace/theme-tomorrow_night_blue.js
 Comment: 
 
-Filename: static/js/ace/mode-prolog.js
+Filename: static/js/ace/theme-iplastic.js
 Comment: 
 
-Filename: static/js/ace/theme-twilight.js
+Filename: static/js/ace/theme-kr_theme.js
 Comment: 
 
-Filename: static/js/ace/mode-properties.js
+Filename: static/js/ace/mode-ini.js
 Comment: 
 
-Filename: static/js/ace/mode-velocity.js
+Filename: static/js/ace/mode-mysql.js
 Comment: 
 
-Filename: static/js/ace/mode-stylus.js
+Filename: static/js/ace/mode-tex.js
 Comment: 
 
-Filename: static/js/ace/mode-html.js
+Filename: static/js/ace/theme-twilight.js
 Comment: 
 
-Filename: static/js/ace/worker-javascript.js
+Filename: static/js/ace/mode-fortran.js
 Comment: 
 
-Filename: static/js/ace/mode-powershell.js
+Filename: static/js/ace/mode-jack.js
 Comment: 
 
-Filename: static/js/ace/mode-hjson.js
+Filename: static/js/ace/ext-beautify.js
 Comment: 
 
-Filename: static/js/ace/mode-latex.js
+Filename: static/js/ace/mode-plain_text.js
 Comment: 
 
-Filename: static/js/ace/theme-xcode.js
+Filename: static/js/ace/mode-cirru.js
 Comment: 
 
-Filename: static/js/ace/mode-ocaml.js
+Filename: static/js/ace/theme-katzenmilch.js
 Comment: 
 
-Filename: static/js/ace/mode-clojure.js
+Filename: static/js/ace/mode-tcl.js
 Comment: 
 
-Filename: static/js/ace/mode-makefile.js
+Filename: static/js/ace/mode-html.js
 Comment: 
 
-Filename: static/js/ace/worker-coffee.js
+Filename: static/js/ace/mode-gherkin.js
 Comment: 
 
-Filename: static/js/ace/mode-applescript.js
+Filename: static/js/ace/ext-modelist.js
 Comment: 
 
-Filename: static/js/ace/mode-dot.js
+Filename: static/js/ace/theme-cobalt.js
 Comment: 
 
-Filename: static/js/ace/snippets/objectivec.js
+Filename: static/js/ace/mode-javascript.js
 Comment: 
 
-Filename: static/js/ace/snippets/gobstones.js
+Filename: static/js/ace/mode-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/snippets/kotlin.js
+Filename: static/js/ace/theme-clouds_midnight.js
 Comment: 
 
-Filename: static/js/ace/snippets/hjson.js
+Filename: static/js/ace/mode-actionscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/assembly_x86.js
+Filename: static/js/ace/mode-liquid.js
 Comment: 
 
-Filename: static/js/ace/snippets/ruby.js
+Filename: static/js/ace/worker-lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/logiql.js
+Filename: static/js/ace/mode-mushcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/text.js
+Filename: static/js/ace/mode-jsp.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_ruby.js
+Filename: static/js/ace/mode-jade.js
 Comment: 
 
-Filename: static/js/ace/snippets/php.js
+Filename: static/js/ace/mode-haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/snippets/makefile.js
+Filename: static/js/ace/mode-scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/vbscript.js
+Filename: static/js/ace/mode-typescript.js
 Comment: 
 
-Filename: static/js/ace/snippets/snippets.js
+Filename: static/js/ace/ext-old_ie.js
 Comment: 
 
-Filename: static/js/ace/snippets/haml.js
+Filename: static/js/ace/mode-nsis.js
 Comment: 
 
-Filename: static/js/ace/snippets/json.js
+Filename: static/js/ace/mode-haskell.js
 Comment: 
 
-Filename: static/js/ace/snippets/svg.js
+Filename: static/js/ace/mode-gitignore.js
 Comment: 
 
-Filename: static/js/ace/snippets/drools.js
+Filename: static/js/ace/mode-rhtml.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell.js
+Filename: static/js/ace/theme-ambiance.js
 Comment: 
 
-Filename: static/js/ace/snippets/vhdl.js
+Filename: static/js/ace/mode-swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/gcode.js
+Filename: static/js/ace/mode-d.js
 Comment: 
 
-Filename: static/js/ace/snippets/erlang.js
+Filename: static/js/ace/mode-pascal.js
 Comment: 
 
-Filename: static/js/ace/snippets/matlab.js
+Filename: static/js/ace/mode-cobol.js
 Comment: 
 
-Filename: static/js/ace/snippets/properties.js
+Filename: static/js/ace/theme-eclipse.js
 Comment: 
 
-Filename: static/js/ace/snippets/io.js
+Filename: static/js/ace/worker-php.js
 Comment: 
 
-Filename: static/js/ace/snippets/xquery.js
+Filename: static/js/ace/mode-jsoniq.js
 Comment: 
 
-Filename: static/js/ace/snippets/razor.js
+Filename: static/js/ace/mode-io.js
 Comment: 
 
-Filename: static/js/ace/snippets/typescript.js
+Filename: static/js/ace/ext-linking.js
 Comment: 
 
-Filename: static/js/ace/snippets/mips_assembler.js
+Filename: static/js/ace/theme-chaos.js
 Comment: 
 
-Filename: static/js/ace/snippets/textile.js
+Filename: static/js/ace/worker-json.js
 Comment: 
 
-Filename: static/js/ace/snippets/perl.js
+Filename: static/js/ace/theme-chrome.js
 Comment: 
 
-Filename: static/js/ace/snippets/mel.js
+Filename: static/js/ace/mode-powershell.js
 Comment: 
 
-Filename: static/js/ace/snippets/applescript.js
+Filename: static/js/ace/mode-smarty.js
 Comment: 
 
-Filename: static/js/ace/snippets/less.js
+Filename: static/js/ace/mode-c9search.js
 Comment: 
 
-Filename: static/js/ace/snippets/live_script.js
+Filename: static/js/ace/mode-vbscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/coffee.js
+Filename: static/js/ace/mode-css.js
 Comment: 
 
-Filename: static/js/ace/snippets/bro.js
+Filename: static/js/ace/mode-xml.js
 Comment: 
 
-Filename: static/js/ace/snippets/prolog.js
+Filename: static/js/ace/worker-css.js
 Comment: 
 
-Filename: static/js/ace/snippets/velocity.js
+Filename: static/js/ace/mode-java.js
 Comment: 
 
-Filename: static/js/ace/snippets/ini.js
+Filename: static/js/ace/theme-clouds.js
 Comment: 
 
-Filename: static/js/ace/snippets/rdoc.js
+Filename: static/js/ace/theme-tomorrow.js
 Comment: 
 
-Filename: static/js/ace/snippets/actionscript.js
+Filename: static/js/ace/mode-sass.js
 Comment: 
 
-Filename: static/js/ace/snippets/cirru.js
+Filename: static/js/ace/mode-makefile.js
 Comment: 
 
-Filename: static/js/ace/snippets/html.js
+Filename: static/js/ace/mode-batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/groovy.js
+Filename: static/js/ace/mode-elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/lsl.js
+Filename: static/js/ace/mode-autohotkey.js
 Comment: 
 
-Filename: static/js/ace/snippets/r.js
+Filename: static/js/ace/theme-idle_fingers.js
 Comment: 
 
-Filename: static/js/ace/snippets/plain_text.js
+Filename: static/js/ace/mode-glsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/mysql.js
+Filename: static/js/ace/mode-python.js
 Comment: 
 
-Filename: static/js/ace/snippets/css.js
+Filename: static/js/ace/mode-nix.js
 Comment: 
 
-Filename: static/js/ace/snippets/pgsql.js
+Filename: static/js/ace/mode-django.js
 Comment: 
 
-Filename: static/js/ace/snippets/lucene.js
+Filename: static/js/ace/mode-lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/ocaml.js
+Filename: static/js/ace/theme-solarized_light.js
 Comment: 
 
-Filename: static/js/ace/snippets/java.js
+Filename: static/js/ace/theme-xcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/mushcode.js
+Filename: static/js/ace/ext-chromevox.js
 Comment: 
 
-Filename: static/js/ace/snippets/dot.js
+Filename: static/js/ace/mode-twig.js
 Comment: 
 
-Filename: static/js/ace/snippets/verilog.js
+Filename: static/js/ace/snippets/elm.js
 Comment: 
 
-Filename: static/js/ace/snippets/twig.js
+Filename: static/js/ace/snippets/typescript.js
 Comment: 
 
-Filename: static/js/ace/snippets/eiffel.js
+Filename: static/js/ace/snippets/handlebars.js
 Comment: 
 
-Filename: static/js/ace/snippets/dockerfile.js
+Filename: static/js/ace/snippets/mysql.js
 Comment: 
 
-Filename: static/js/ace/snippets/sql.js
+Filename: static/js/ace/snippets/cobol.js
 Comment: 
 
-Filename: static/js/ace/snippets/fortran.js
+Filename: static/js/ace/snippets/sass.js
 Comment: 
 
-Filename: static/js/ace/snippets/tcl.js
+Filename: static/js/ace/snippets/haxe.js
 Comment: 
 
-Filename: static/js/ace/snippets/golang.js
+Filename: static/js/ace/snippets/ini.js
 Comment: 
 
-Filename: static/js/ace/snippets/curly.js
+Filename: static/js/ace/snippets/twig.js
 Comment: 
 
-Filename: static/js/ace/snippets/lean.js
+Filename: static/js/ace/snippets/clojure.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsp.js
+Filename: static/js/ace/snippets/live_script.js
 Comment: 
 
-Filename: static/js/ace/snippets/ejs.js
+Filename: static/js/ace/snippets/swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/swig.js
+Filename: static/js/ace/snippets/ocaml.js
 Comment: 
 
-Filename: static/js/ace/snippets/soy_template.js
+Filename: static/js/ace/snippets/plain_text.js
 Comment: 
 
-Filename: static/js/ace/snippets/gitignore.js
+Filename: static/js/ace/snippets/vala.js
 Comment: 
 
-Filename: static/js/ace/snippets/pascal.js
+Filename: static/js/ace/snippets/lsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/wollok.js
+Filename: static/js/ace/snippets/sql.js
 Comment: 
 
-Filename: static/js/ace/snippets/c_cpp.js
+Filename: static/js/ace/snippets/less.js
 Comment: 
 
-Filename: static/js/ace/snippets/haxe.js
+Filename: static/js/ace/snippets/markdown.js
 Comment: 
 
-Filename: static/js/ace/snippets/gherkin.js
+Filename: static/js/ace/snippets/liquid.js
 Comment: 
 
-Filename: static/js/ace/snippets/python.js
+Filename: static/js/ace/snippets/space.js
 Comment: 
 
-Filename: static/js/ace/snippets/maze.js
+Filename: static/js/ace/snippets/golang.js
 Comment: 
 
-Filename: static/js/ace/snippets/autohotkey.js
+Filename: static/js/ace/snippets/properties.js
 Comment: 
 
-Filename: static/js/ace/snippets/scheme.js
+Filename: static/js/ace/snippets/vhdl.js
 Comment: 
 
-Filename: static/js/ace/snippets/abc.js
+Filename: static/js/ace/snippets/vbscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/scss.js
+Filename: static/js/ace/snippets/ftl.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_elixir.js
+Filename: static/js/ace/snippets/coffee.js
 Comment: 
 
-Filename: static/js/ace/snippets/latex.js
+Filename: static/js/ace/snippets/lucene.js
 Comment: 
 
-Filename: static/js/ace/snippets/nsis.js
+Filename: static/js/ace/snippets/dart.js
 Comment: 
 
-Filename: static/js/ace/snippets/sjs.js
+Filename: static/js/ace/snippets/mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsx.js
+Filename: static/js/ace/snippets/pgsql.js
 Comment: 
 
-Filename: static/js/ace/snippets/tex.js
+Filename: static/js/ace/snippets/r.js
 Comment: 
 
-Filename: static/js/ace/snippets/vala.js
+Filename: static/js/ace/snippets/rst.js
 Comment: 
 
-Filename: static/js/ace/snippets/tsx.js
+Filename: static/js/ace/snippets/dot.js
 Comment: 
 
-Filename: static/js/ace/snippets/rst.js
+Filename: static/js/ace/snippets/xml.js
 Comment: 
 
 Filename: static/js/ace/snippets/scala.js
 Comment: 
 
-Filename: static/js/ace/snippets/yaml.js
+Filename: static/js/ace/snippets/text.js
 Comment: 
 
-Filename: static/js/ace/snippets/ada.js
+Filename: static/js/ace/snippets/hjson.js
 Comment: 
 
-Filename: static/js/ace/snippets/batchfile.js
+Filename: static/js/ace/snippets/asciidoc.js
 Comment: 
 
-Filename: static/js/ace/snippets/smarty.js
+Filename: static/js/ace/snippets/apache_conf.js
 Comment: 
 
-Filename: static/js/ace/snippets/praat.js
+Filename: static/js/ace/snippets/razor.js
 Comment: 
 
-Filename: static/js/ace/snippets/asciidoc.js
+Filename: static/js/ace/snippets/javascript.js
 Comment: 
 
-Filename: static/js/ace/snippets/swift.js
+Filename: static/js/ace/snippets/scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/scad.js
+Filename: static/js/ace/snippets/curly.js
 Comment: 
 
-Filename: static/js/ace/snippets/elm.js
+Filename: static/js/ace/snippets/glsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/glsl.js
+Filename: static/js/ace/snippets/drools.js
 Comment: 
 
-Filename: static/js/ace/snippets/mask.js
+Filename: static/js/ace/snippets/sh.js
 Comment: 
 
-Filename: static/js/ace/snippets/lua.js
+Filename: static/js/ace/snippets/diff.js
 Comment: 
 
-Filename: static/js/ace/snippets/c9search.js
+Filename: static/js/ace/snippets/html_ruby.js
 Comment: 
 
-Filename: static/js/ace/snippets/diff.js
+Filename: static/js/ace/snippets/bro.js
 Comment: 
 
-Filename: static/js/ace/snippets/clojure.js
+Filename: static/js/ace/snippets/ejs.js
 Comment: 
 
-Filename: static/js/ace/snippets/livescript.js
+Filename: static/js/ace/snippets/jsoniq.js
 Comment: 
 
-Filename: static/js/ace/snippets/rust.js
+Filename: static/js/ace/snippets/wollok.js
 Comment: 
 
-Filename: static/js/ace/snippets/powershell.js
+Filename: static/js/ace/snippets/smarty.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsoniq.js
+Filename: static/js/ace/snippets/json.js
 Comment: 
 
-Filename: static/js/ace/snippets/d.js
+Filename: static/js/ace/snippets/c_cpp.js
 Comment: 
 
-Filename: static/js/ace/snippets/toml.js
+Filename: static/js/ace/snippets/gcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/csharp.js
+Filename: static/js/ace/snippets/batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/lisp.js
+Filename: static/js/ace/snippets/css.js
 Comment: 
 
-Filename: static/js/ace/snippets/sqlserver.js
+Filename: static/js/ace/snippets/perl.js
 Comment: 
 
 Filename: static/js/ace/snippets/nix.js
 Comment: 
 
-Filename: static/js/ace/snippets/dart.js
+Filename: static/js/ace/snippets/abap.js
 Comment: 
 
-Filename: static/js/ace/snippets/cobol.js
+Filename: static/js/ace/snippets/html.js
 Comment: 
 
-Filename: static/js/ace/snippets/jade.js
+Filename: static/js/ace/snippets/lisp.js
 Comment: 
 
-Filename: static/js/ace/snippets/protobuf.js
+Filename: static/js/ace/snippets/verilog.js
 Comment: 
 
-Filename: static/js/ace/snippets/mipsassembler.js
+Filename: static/js/ace/snippets/abc.js
 Comment: 
 
-Filename: static/js/ace/snippets/liquid.js
+Filename: static/js/ace/snippets/kotlin.js
 Comment: 
 
-Filename: static/js/ace/snippets/jack.js
+Filename: static/js/ace/snippets/lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/rhtml.js
+Filename: static/js/ace/snippets/jsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/handlebars.js
+Filename: static/js/ace/snippets/c9search.js
 Comment: 
 
-Filename: static/js/ace/snippets/xml.js
+Filename: static/js/ace/snippets/mask.js
 Comment: 
 
-Filename: static/js/ace/snippets/abap.js
+Filename: static/js/ace/snippets/assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/snippets/elixir.js
+Filename: static/js/ace/snippets/jack.js
 Comment: 
 
-Filename: static/js/ace/snippets/forth.js
+Filename: static/js/ace/snippets/snippets.js
 Comment: 
 
-Filename: static/js/ace/snippets/apache_conf.js
+Filename: static/js/ace/snippets/mipsassembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/julia.js
+Filename: static/js/ace/snippets/django.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell_cabal.js
+Filename: static/js/ace/snippets/haml.js
 Comment: 
 
-Filename: static/js/ace/snippets/stylus.js
+Filename: static/js/ace/snippets/scad.js
 Comment: 
 
-Filename: static/js/ace/snippets/sass.js
+Filename: static/js/ace/snippets/elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/django.js
+Filename: static/js/ace/snippets/toml.js
 Comment: 
 
-Filename: static/js/ace/snippets/coldfusion.js
+Filename: static/js/ace/snippets/ruby.js
 Comment: 
 
-Filename: static/js/ace/snippets/javascript.js
+Filename: static/js/ace/snippets/coldfusion.js
 Comment: 
 
-Filename: static/js/ace/snippets/sh.js
+Filename: static/js/ace/snippets/praat.js
 Comment: 
 
-Filename: static/js/ace/snippets/ftl.js
+Filename: static/js/ace/snippets/forth.js
 Comment: 
 
-Filename: static/js/ace/snippets/space.js
+Filename: static/js/ace/snippets/mel.js
 Comment: 
 
-Filename: static/js/ace/snippets/luapage.js
+Filename: static/js/ace/snippets/groovy.js
 Comment: 
 
-Filename: static/js/ace/snippets/markdown.js
+Filename: static/js/ace/snippets/prolog.js
 Comment: 
 
-Filename: static/js/ace/keybinding-vim.js
+Filename: static/js/ace/snippets/rdoc.js
 Comment: 
 
-Filename: static/js/ace/mode-forth.js
+Filename: static/js/ace/snippets/luapage.js
 Comment: 
 
-Filename: static/js/ace/mode-sh.js
+Filename: static/js/ace/snippets/actionscript.js
 Comment: 
 
-Filename: static/js/ace/ext-whitespace.js
+Filename: static/js/ace/snippets/tsx.js
 Comment: 
 
-Filename: static/js/ace/mode-apache_conf.js
+Filename: static/js/ace/snippets/applescript.js
 Comment: 
 
-Filename: static/js/ace/mode-mushcode.js
+Filename: static/js/ace/snippets/gobstones.js
 Comment: 
 
-Filename: static/js/ace/mode-toml.js
+Filename: static/js/ace/snippets/erlang.js
 Comment: 
 
-Filename: static/js/ace/mode-sql.js
+Filename: static/js/ace/snippets/php.js
 Comment: 
 
-Filename: static/js/ace/mode-vhdl.js
+Filename: static/js/ace/snippets/swig.js
 Comment: 
 
-Filename: static/js/ace/mode-lua.js
+Filename: static/js/ace/snippets/pascal.js
 Comment: 
 
-Filename: static/js/ace/mode-assembly_x86.js
+Filename: static/js/ace/snippets/autohotkey.js
 Comment: 
 
-Filename: static/js/ace/mode-glsl.js
+Filename: static/js/ace/snippets/mushcode.js
 Comment: 
 
-Filename: static/js/ace/theme-terminal.js
+Filename: static/js/ace/snippets/logiql.js
 Comment: 
 
-Filename: static/js/ace/mode-cirru.js
+Filename: static/js/ace/snippets/textile.js
 Comment: 
 
-Filename: static/js/ace/mode-scala.js
+Filename: static/js/ace/snippets/protobuf.js
 Comment: 
 
-Filename: static/js/ace/mode-jsx.js
+Filename: static/js/ace/snippets/soy_template.js
 Comment: 
 
-Filename: static/js/ace/mode-coldfusion.js
+Filename: static/js/ace/snippets/html_elixir.js
 Comment: 
 
-Filename: static/js/ace/mode-sass.js
+Filename: static/js/ace/snippets/rust.js
 Comment: 
 
-Filename: static/js/ace/theme-github.js
+Filename: static/js/ace/snippets/sjs.js
 Comment: 
 
-Filename: static/js/ace/mode-svg.js
+Filename: static/js/ace/snippets/livescript.js
 Comment: 
 
-Filename: static/js/ace/mode-scss.js
+Filename: static/js/ace/snippets/julia.js
 Comment: 
 
-Filename: static/js/ace/ace.js
+Filename: static/js/ace/snippets/maze.js
 Comment: 
 
-Filename: static/js/ace/mode-tex.js
+Filename: static/js/ace/snippets/tex.js
 Comment: 
 
-Filename: static/js/ace/mode-io.js
+Filename: static/js/ace/snippets/python.js
 Comment: 
 
-Filename: static/js/ace/mode-drools.js
+Filename: static/js/ace/snippets/gitignore.js
 Comment: 
 
-Filename: static/js/ace/theme-monokai.js
+Filename: static/js/ace/snippets/jsp.js
 Comment: 
 
-Filename: static/js/ace/theme-eclipse.js
+Filename: static/js/ace/snippets/haskell.js
 Comment: 
 
-Filename: static/js/ace/mode-protobuf.js
+Filename: static/js/ace/snippets/tcl.js
 Comment: 
 
-Filename: static/js/ace/mode-ruby.js
+Filename: static/js/ace/snippets/scss.js
 Comment: 
 
-Filename: static/js/ace/theme-chaos.js
+Filename: static/js/ace/snippets/io.js
 Comment: 
 
-Filename: static/js/ace/ext-linking.js
+Filename: static/js/ace/snippets/fortran.js
 Comment: 
 
-Filename: static/js/ace/ext-statusbar.js
+Filename: static/js/ace/snippets/svg.js
 Comment: 
 
-Filename: static/js/ace/worker-html.js
+Filename: static/js/ace/snippets/sqlserver.js
 Comment: 
 
-Filename: static/js/ace/mode-nsis.js
+Filename: static/js/ace/snippets/gherkin.js
 Comment: 
 
-Filename: static/js/ace/worker-php.js
+Filename: static/js/ace/snippets/powershell.js
 Comment: 
 
-Filename: static/js/ace/mode-objectivec.js
+Filename: static/js/ace/snippets/cirru.js
 Comment: 
 
-Filename: static/js/ace/ext-spellcheck.js
+Filename: static/js/ace/snippets/jade.js
 Comment: 
 
-Filename: static/js/ace/mode-javascript.js
+Filename: static/js/ace/snippets/makefile.js
 Comment: 
 
-Filename: static/js/ace/mode-praat.js
+Filename: static/js/ace/snippets/stylus.js
 Comment: 
 
-Filename: static/js/ace/mode-matlab.js
+Filename: static/js/ace/snippets/velocity.js
 Comment: 
 
-Filename: static/js/ace/mode-plain_text.js
+Filename: static/js/ace/snippets/xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-mel.js
+Filename: static/js/ace/snippets/csharp.js
 Comment: 
 
-Filename: static/js/ace/mode-rdoc.js
+Filename: static/js/ace/snippets/dockerfile.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night.js
+Filename: static/js/ace/snippets/rhtml.js
 Comment: 
 
-Filename: static/js/ace/mode-groovy.js
+Filename: static/js/ace/snippets/d.js
 Comment: 
 
-Filename: static/js/ace/mode-markdown.js
+Filename: static/js/ace/snippets/latex.js
 Comment: 
 
-Filename: static/js/ace/mode-mysql.js
+Filename: static/js/ace/snippets/nsis.js
 Comment: 
 
-Filename: static/js/ace/mode-batchfile.js
+Filename: static/js/ace/snippets/matlab.js
 Comment: 
 
-Filename: static/js/ace/mode-gitignore.js
+Filename: static/js/ace/snippets/objectivec.js
 Comment: 
 
-Filename: static/js/ace/mode-julia.js
+Filename: static/js/ace/snippets/lean.js
 Comment: 
 
-Filename: static/js/ace/theme-kr_theme.js
+Filename: static/js/ace/snippets/java.js
 Comment: 
 
-Filename: static/js/ace/ext-error_marker.js
+Filename: static/js/ace/snippets/eiffel.js
 Comment: 
 
-Filename: static/js/ace/mode-json.js
+Filename: static/js/ace/snippets/ada.js
 Comment: 
 
-Filename: static/js/ace/mode-soy_template.js
+Filename: static/js/ace/snippets/haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/ext-settings_menu.js
+Filename: static/js/ace/snippets/yaml.js
 Comment: 
 
-Filename: static/js/ace/mode-vala.js
+Filename: static/js/ace/ext-elastic_tabstops_lite.js
 Comment: 
 
-Filename: static/js/ace/mode-logiql.js
+Filename: static/js/ace/theme-merbivore.js
 Comment: 
 
-Filename: static/js/ace/mode-abap.js
+Filename: static/js/ace/mode-snippets.js
 Comment: 
 
-Filename: static/js/ace/mode-lisp.js
+Filename: static/js/ace/ext-static_highlight.js
 Comment: 
 
-Filename: static/js/ace/mode-dart.js
+Filename: static/js/ace/ext-language_tools.js
 Comment: 
 
-Filename: static/js/ace/ext-themelist.js
+Filename: static/js/ace/mode-mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/theme-idle_fingers.js
+Filename: static/js/ace/mode-groovy.js
 Comment: 
 
-Filename: static/js/ace/ext-searchbox.js
+Filename: static/js/ace/mode-pgsql.js
 Comment: 
 
-Filename: static/js/ace/mode-ini.js
+Filename: static/js/ace/mode-markdown.js
 Comment: 
 
-Filename: static/js/ace/mode-c_cpp.js
+Filename: static/js/ace/mode-scad.js
 Comment: 
 
-Filename: static/js/ace/worker-lua.js
+Filename: static/js/ace/mode-stylus.js
 Comment: 
 
-Filename: static/js/ace/theme-crimson_editor.js
+Filename: static/js/ace/mode-ocaml.js
 Comment: 
 
-Filename: static/js/ace/mode-tsx.js
+Filename: static/js/ace/mode-swig.js
 Comment: 
 
-Filename: static/js/ace/mode-handlebars.js
+Filename: static/js/ace/mode-haxe.js
 Comment: 
 
-Filename: static/js/ace/ext-language_tools.js
+Filename: static/js/ace/mode-maze.js
 Comment: 
 
-Filename: static/js/ace/mode-typescript.js
+Filename: static/js/ace/mode-scss.js
 Comment: 
 
-Filename: static/js/ace/mode-lean.js
+Filename: static/js/ace/mode-rust.js
 Comment: 
 
-Filename: static/js/ace/mode-verilog.js
+Filename: static/js/ace/mode-rdoc.js
 Comment: 
 
-Filename: static/js/ace/theme-vibrant_ink.js
+Filename: static/js/ace/mode-eiffel.js
 Comment: 
 
-Filename: static/js/ace/mode-jack.js
+Filename: static/js/ace/mode-latex.js
 Comment: 
 
-Filename: static/js/ace/mode-liquid.js
+Filename: static/js/ace/mode-scala.js
 Comment: 
 
-Filename: static/js/ace/mode-razor.js
+Filename: static/js/ace/mode-dot.js
 Comment: 
 
-Filename: static/js/ace/mode-snippets.js
+Filename: static/js/ace/mode-perl.js
 Comment: 
 
-Filename: static/js/ace/mode-maze.js
+Filename: static/js/ace/mode-objectivec.js
 Comment: 
 
-Filename: static/js/ace/ext-textarea.js
+Filename: static/js/ace/worker-html.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell.js
+Filename: static/js/ace/theme-merbivore_soft.js
 Comment: 
 
-Filename: static/js/ace/mode-bro.js
+Filename: static/js/ace/mode-velocity.js
 Comment: 
 
-Filename: static/js/ace/mode-lsl.js
+Filename: static/js/ace/theme-vibrant_ink.js
 Comment: 
 
-Filename: static/js/ace/mode-ejs.js
+Filename: static/js/ace/mode-clojure.js
 Comment: 
 
-Filename: static/js/ace/theme-ambiance.js
+Filename: static/js/ace/mode-php.js
 Comment: 
 
-Filename: static/js/ace/ext-old_ie.js
+Filename: static/js/ace/theme-monokai.js
 Comment: 
 
-Filename: static/js/ace/mode-lucene.js
+Filename: static/js/ace/ext-emmet.js
 Comment: 
 
-Filename: static/js/ace/mode-coffee.js
+Filename: static/js/ace/mode-asciidoc.js
 Comment: 
 
-Filename: static/js/ace/mode-haml.js
+Filename: static/js/ace/mode-csharp.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell_cabal.js
+Filename: static/js/ace/theme-tomorrow_night_eighties.js
 Comment: 
 
-Filename: static/js/ace/mode-css.js
+Filename: static/js/ace/mode-sql.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore_soft.js
+Filename: static/js/ace/ext-spellcheck.js
 Comment: 
 
-Filename: static/js/ace/mode-vbscript.js
+Filename: static/js/ace/theme-tomorrow_night_bright.js
 Comment: 
 
-Filename: static/js/ace/mode-html_ruby.js
+Filename: static/js/ace/mode-ftl.js
 Comment: 
 
-Filename: static/js/ace/mode-pgsql.js
+Filename: static/js/ace/keybinding-vim.js
 Comment: 
 
-Filename: static/js/ace/mode-abc.js
+Filename: static/js/ace/mode-mipsassembler.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_eighties.js
+Filename: static/js/ace/mode-r.js
 Comment: 
 
-Filename: static/js/ace/ext-emmet.js
+Filename: static/js/ace/mode-lean.js
 Comment: 
 
-Filename: static/js/ace/mode-html_elixir.js
+Filename: static/js/ace/mode-toml.js
 Comment: 
 
-Filename: static/js/ace/mode-erlang.js
+Filename: static/js/ace/mode-html_ruby.js
 Comment: 
 
-Filename: static/js/ace/ext-keybinding_menu.js
+Filename: static/js/ace/mode-lucene.js
 Comment: 
 
-Filename: static/js/ace/theme-dawn.js
+Filename: static/js/ace/ext-error_marker.js
 Comment: 
 
-Filename: static/js/ace/mode-asciidoc.js
+Filename: static/js/ace/mode-kotlin.js
 Comment: 
 
-Filename: static/js/ace/theme-pastel_on_dark.js
+Filename: static/js/ace/mode-rst.js
 Comment: 
 
-Filename: static/js/ace/mode-swig.js
+Filename: static/js/ace/mode-ruby.js
 Comment: 
 
-Filename: static/js/ace/mode-swift.js
+Filename: static/js/ace/mode-vala.js
 Comment: 
 
-Filename: static/js/ace/mode-python.js
+Filename: static/js/ace/ext-statusbar.js
 Comment: 
 
-Filename: static/js/ace/mode-livescript.js
+Filename: static/js/ace/mode-html_elixir.js
 Comment: 
 
-Filename: static/js/ace/theme-cobalt.js
+Filename: static/js/ace/mode-json.js
 Comment: 
 
-Filename: static/js/ace/mode-django.js
+Filename: static/js/ace/mode-sjs.js
 Comment: 
 
-Filename: static/js/ace/mode-xquery.js
+Filename: static/js/ace/theme-crimson_editor.js
 Comment: 
 
-Filename: static/js/ace/mode-scad.js
+Filename: static/js/ace/mode-verilog.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds_midnight.js
+Filename: static/js/highlight.min.js
 Comment: 
 
-Filename: static/js/ace/ext-chromevox.js
+Filename: static/js/jquery.min.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_light.js
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/js/ace/mode-nix.js
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: static/js/ace/mode-luapage.js
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: static/js/ace/theme-kuroir.js
+Filename: static/js/axios.min.js
 Comment: 
 
-Filename: static/js/ace/mode-fortran.js
+Filename: static/js/dbadmin.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore.js
+Filename: static/js/translations.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_bright.js
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/js/ace/mode-xml.js
+Filename: static/css/gitlog.min.css
 Comment: 
 
-Filename: static/js/ace/mode-mips_assembler.js
+Filename: static/css/future.css
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/images/alert-blue.gif
 Comment: 
 
-Filename: static/js/axios.min.js
+Filename: static/images/widget.gif
 Comment: 
 
-Filename: static/js/dbadmin.js
+Filename: static/images/alert-yellow.gif
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/images/alert-red.gif
 Comment: 
 
-Filename: static/js/jquery.min.js
+Filename: static/images/alert-green.gif
 Comment: 
 
-Filename: static/js/highlight.min.js
+Filename: static/images/forkme.png
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/images/alert-orange.gif
 Comment: 
 
-Filename: __init__.py
+Filename: translations/README.md
 Comment: 
 
-Filename: templates/translations.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/index.html
+Filename: diff2kryten.py
 Comment: 
 
 Filename: templates/gitlog.html
 Comment: 
 
-Filename: templates/dbadmin.html
+Filename: templates/ticket.html
 Comment: 
 
-Filename: templates/ticket.html
+Filename: templates/dbadmin.html
 Comment: 
 
-Filename: diff2kryten.py
+Filename: templates/translations.html
 Comment: 
 
-Filename: translations/README.md
+Filename: templates/index.html
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app._default.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 187155 bytes, number of entries: 4
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx      135 tx defN 23-May-08 00:39 __init__.py
--rw-rw-r--  3.0 unx     1811 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/images/logo.png
+-rw-r--r--  3.0 unx      135 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx     1811 tx defN 23-May-08 00:39 templates/index.html
 4 files, 215409 bytes uncompressed, 186479 bytes compressed:  13.4%
```

#### zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: static/images/logo.png
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/images/logo.png
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
 Filename: templates/index.html
 Comment:
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app._documentation.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,158 +1,158 @@
 Zip file size: 4356813 bytes, number of entries: 156
--rw-rw-r--  3.0 unx   111701 tx defN 23-May-08 02:54 static/en/chapter-10.html
--rw-rw-r--  3.0 unx    54171 tx defN 23-May-08 02:54 static/en/chapter-14.html
--rw-rw-r--  3.0 unx    45554 tx defN 23-May-08 02:54 static/en/chapter-03.html
--rw-rw-r--  3.0 unx    42541 tx defN 23-May-08 02:54 static/en/chapter-05.html
--rw-rw-r--  3.0 unx    85412 tx defN 23-May-08 02:54 static/en/chapter-16.html
--rw-rw-r--  3.0 unx    94874 tx defN 23-May-08 02:54 static/en/chapter-06.html
--rw-rw-r--  3.0 unx    19979 tx defN 23-May-08 02:54 static/en/index.html
--rw-rw-r--  3.0 unx    63565 tx defN 23-May-08 02:54 static/en/chapter-09.html
--rw-rw-r--  3.0 unx     1804 tx defN 23-May-08 01:34 static/en/_static/tabs.css
--rw-rw-r--  3.0 unx      427 tx defN 23-May-08 02:54 static/en/_static/documentation_options.js
--rw-rw-r--  3.0 unx     4231 tx defN 23-May-08 01:34 static/en/_static/tabs.js
--rw-rw-r--  3.0 unx     4712 tx defN 23-May-08 01:43 static/en/_static/sphinx_highlight.js
--rw-rw-r--  3.0 unx    89501 tx defN 23-May-08 02:13 static/en/_static/jquery.js
--rw-rw-r--  3.0 unx       90 bx defN 23-May-08 01:43 static/en/_static/minus.png
--rw-rw-r--  3.0 unx       90 bx defN 23-May-08 01:43 static/en/_static/plus.png
--rw-rw-r--  3.0 unx     4758 tx defN 23-May-08 02:54 static/en/_static/language_data.js
--rw-rw-r--  3.0 unx     4819 tx defN 23-May-08 02:13 static/en/_static/pygments.css
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_static/logo.png
--rw-rw-r--  3.0 unx    18215 tx defN 23-May-08 02:54 static/en/_static/searchtools.js
--rw-rw-r--  3.0 unx     4289 tx defN 23-May-08 02:13 static/en/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--  3.0 unx   135235 tx defN 23-May-08 02:54 static/en/_static/css/theme.css
--rw-rw-r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/_static/css/toggle.css
--rw-rw-r--  3.0 unx     3229 tx defN 23-May-08 01:34 static/en/_static/css/badge_only.css
--rw-rw-r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/_static/css/dark.css
--rw-rw-r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/en/_static/logo-32x32.ico
--rw-rw-r--  3.0 unx     4370 tx defN 23-May-08 01:34 static/en/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--  3.0 unx      934 tx defN 23-May-08 01:34 static/en/_static/js/badge_only.js
--rw-rw-r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/en/_static/js/toggle.js
--rw-rw-r--  3.0 unx     5023 tx defN 23-May-08 01:34 static/en/_static/js/theme.js
--rw-rw-r--  3.0 unx     2734 tx defN 23-May-08 01:34 static/en/_static/js/html5shiv.min.js
--rw-rw-r--  3.0 unx      286 bx stor 23-May-08 01:43 static/en/_static/file.png
--rw-rw-r--  3.0 unx     4472 tx defN 23-May-08 02:54 static/en/_static/doctools.js
--rw-rw-r--  3.0 unx    14813 tx defN 23-May-08 02:54 static/en/_static/basic.css
--rw-rw-r--  3.0 unx    43200 tx defN 23-May-08 02:54 static/en/chapter-15.html
--rw-rw-r--  3.0 unx   189735 tx defN 23-May-08 02:54 static/en/chapter-12.html
--rw-rw-r--  3.0 unx    91571 tx defN 23-May-08 02:54 static/en/searchindex.js
--rw-rw-r--  3.0 unx    19145 tx defN 23-May-08 02:54 static/en/chapter-02.html
--rw-rw-r--  3.0 unx    11517 tx defN 23-May-08 02:54 static/en/chapter-11.html
--rw-rw-r--  3.0 unx    15647 tx defN 23-May-08 02:54 static/en/chapter-01.html
--rw-rw-r--  3.0 unx     6797 tx defN 23-May-08 02:54 static/en/genindex.html
--rw-rw-r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/toggle.css
--rw-rw-r--  3.0 unx   129408 tx defN 23-May-08 02:54 static/en/chapter-08.html
--rw-rw-r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/en/_images/form1.png
--rw-rw-r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/en/_images/dashboard_ticket.png
--rw-rw-r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/en/_images/form3.png
--rw-rw-r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/en/_images/dashboard_edit.png
--rw-rw-r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/en/_images/form2.png
--rw-rw-r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/en/_images/grid.png
--rw-rw-r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/en/_images/restapi2.png
--rw-rw-r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/en/_images/simple_counter.png
--rw-rw-r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/en/_images/restapi.png
--rw-rw-r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/en/_images/form5.png
--rw-rw-r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/en/_images/dashboard_login.png
--rw-rw-r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/en/_images/dashboard_restapi.png
--rw-rw-r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/en/_images/dashboard_main.png
--rw-rw-r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/en/_images/grid_columns.png
--rw-rw-r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/en/_images/grid_bulmacss.png
--rw-rw-r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/en/_images/_scaffold.png
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_images/logo.png
--rw-rw-r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/en/_images/dashboard.png
--rw-rw-r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/en/_images/tags2.png
--rw-rw-r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/en/_images/form4.png
--rw-rw-r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/en/_images/dashboard_error.png
--rw-rw-r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/en/_images/grid_nocss.png
--rw-rw-r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/en/_images/tags_db.png
--rw-rw-r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/en/_images/dashboard_new_app.png
--rw-rw-r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/en/_images/main_page.png
--rw-rw-r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/en/_images/command.png
--rw-rw-r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/en/_images/first_run.png
--rw-rw-r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/en/_images/form6.png
--rw-rw-r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/dark.css
--rw-rw-r--  3.0 unx   500088 tx defN 23-May-08 02:54 static/en/chapter-07.html
--rw-rw-r--  3.0 unx    12025 tx defN 23-May-08 02:54 static/en/chapter-04.html
--rw-rw-r--  3.0 unx     7072 tx defN 23-May-08 02:54 static/en/search.html
--rw-rw-r--  3.0 unx    50820 tx defN 23-May-08 02:54 static/en/chapter-13.html
--rw-rw-r--  3.0 unx      248 tx defN 23-May-08 02:13 static/index.html
--rw-rw-r--  3.0 unx   105227 tx defN 23-May-08 02:54 static/pt/chapter-10.html
--rw-rw-r--  3.0 unx    54793 tx defN 23-May-08 02:54 static/pt/chapter-14.html
--rw-rw-r--  3.0 unx    44854 tx defN 23-May-08 02:54 static/pt/chapter-03.html
--rw-rw-r--  3.0 unx    41291 tx defN 23-May-08 02:54 static/pt/chapter-05.html
--rw-rw-r--  3.0 unx    85534 tx defN 23-May-08 02:54 static/pt/chapter-16.html
--rw-rw-r--  3.0 unx    93497 tx defN 23-May-08 02:54 static/pt/chapter-06.html
--rw-rw-r--  3.0 unx    19994 tx defN 23-May-08 02:54 static/pt/index.html
--rw-rw-r--  3.0 unx    61495 tx defN 23-May-08 02:54 static/pt/chapter-09.html
--rw-rw-r--  3.0 unx     1804 tx defN 23-May-08 01:34 static/pt/_static/tabs.css
--rw-rw-r--  3.0 unx      427 tx defN 23-May-08 02:54 static/pt/_static/documentation_options.js
--rw-rw-r--  3.0 unx     4231 tx defN 23-May-08 01:34 static/pt/_static/tabs.js
--rw-rw-r--  3.0 unx     4712 tx defN 23-May-08 01:43 static/pt/_static/sphinx_highlight.js
--rw-rw-r--  3.0 unx    89501 tx defN 23-May-08 02:13 static/pt/_static/jquery.js
--rw-rw-r--  3.0 unx       90 bx defN 23-May-08 01:43 static/pt/_static/minus.png
--rw-rw-r--  3.0 unx     2412 tx defN 23-May-08 01:43 static/pt/_static/translations.js
--rw-rw-r--  3.0 unx       90 bx defN 23-May-08 01:43 static/pt/_static/plus.png
--rw-rw-r--  3.0 unx    14417 tx defN 23-May-08 02:54 static/pt/_static/language_data.js
--rw-rw-r--  3.0 unx     4819 tx defN 23-May-08 02:13 static/pt/_static/pygments.css
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_static/logo.png
--rw-rw-r--  3.0 unx     8133 tx defN 23-May-08 01:43 static/pt/_static/base-stemmer.js
--rw-rw-r--  3.0 unx    18215 tx defN 23-May-08 02:54 static/pt/_static/searchtools.js
--rw-rw-r--  3.0 unx     4289 tx defN 23-May-08 02:13 static/pt/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--  3.0 unx   135235 tx defN 23-May-08 02:54 static/pt/_static/css/theme.css
--rw-rw-r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/_static/css/toggle.css
--rw-rw-r--  3.0 unx     3229 tx defN 23-May-08 01:34 static/pt/_static/css/badge_only.css
--rw-rw-r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/_static/css/dark.css
--rw-rw-r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/pt/_static/logo-32x32.ico
--rw-rw-r--  3.0 unx    26718 tx defN 23-May-08 01:43 static/pt/_static/portuguese-stemmer.js
--rw-rw-r--  3.0 unx     4370 tx defN 23-May-08 01:34 static/pt/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--  3.0 unx      934 tx defN 23-May-08 01:34 static/pt/_static/js/badge_only.js
--rw-rw-r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/pt/_static/js/toggle.js
--rw-rw-r--  3.0 unx     5023 tx defN 23-May-08 01:34 static/pt/_static/js/theme.js
--rw-rw-r--  3.0 unx     2734 tx defN 23-May-08 01:34 static/pt/_static/js/html5shiv.min.js
--rw-rw-r--  3.0 unx      286 bx stor 23-May-08 01:43 static/pt/_static/file.png
--rw-rw-r--  3.0 unx     4472 tx defN 23-May-08 02:54 static/pt/_static/doctools.js
--rw-rw-r--  3.0 unx    14813 tx defN 23-May-08 02:54 static/pt/_static/basic.css
--rw-rw-r--  3.0 unx    43359 tx defN 23-May-08 02:54 static/pt/chapter-15.html
--rw-rw-r--  3.0 unx   189425 tx defN 23-May-08 02:54 static/pt/chapter-12.html
--rw-rw-r--  3.0 unx   125717 tx defN 23-May-08 02:54 static/pt/searchindex.js
--rw-rw-r--  3.0 unx    19683 tx defN 23-May-08 02:54 static/pt/chapter-02.html
--rw-rw-r--  3.0 unx    11813 tx defN 23-May-08 02:54 static/pt/chapter-11.html
--rw-rw-r--  3.0 unx    16039 tx defN 23-May-08 02:54 static/pt/chapter-01.html
--rw-rw-r--  3.0 unx     6934 tx defN 23-May-08 02:54 static/pt/genindex.html
--rw-rw-r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/toggle.css
--rw-rw-r--  3.0 unx   129323 tx defN 23-May-08 02:54 static/pt/chapter-08.html
--rw-rw-r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/pt/_images/form1.png
--rw-rw-r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/pt/_images/dashboard_ticket.png
--rw-rw-r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/pt/_images/form3.png
--rw-rw-r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/pt/_images/dashboard_edit.png
--rw-rw-r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/pt/_images/form2.png
--rw-rw-r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/pt/_images/grid.png
--rw-rw-r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/pt/_images/restapi2.png
--rw-rw-r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/pt/_images/simple_counter.png
--rw-rw-r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/pt/_images/restapi.png
--rw-rw-r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/pt/_images/form5.png
--rw-rw-r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/pt/_images/dashboard_login.png
--rw-rw-r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/pt/_images/dashboard_restapi.png
--rw-rw-r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/pt/_images/dashboard_main.png
--rw-rw-r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/pt/_images/grid_columns.png
--rw-rw-r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/pt/_images/grid_bulmacss.png
--rw-rw-r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/pt/_images/_scaffold.png
--rw-rw-r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_images/logo.png
--rw-rw-r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/pt/_images/dashboard.png
--rw-rw-r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/pt/_images/tags2.png
--rw-rw-r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/pt/_images/form4.png
--rw-rw-r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/pt/_images/dashboard_error.png
--rw-rw-r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/pt/_images/grid_nocss.png
--rw-rw-r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/pt/_images/tags_db.png
--rw-rw-r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/pt/_images/dashboard_new_app.png
--rw-rw-r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/pt/_images/main_page.png
--rw-rw-r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/pt/_images/command.png
--rw-rw-r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/pt/_images/first_run.png
--rw-rw-r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/pt/_images/form6.png
--rw-rw-r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/dark.css
--rw-rw-r--  3.0 unx   464626 tx defN 23-May-08 02:54 static/pt/chapter-07.html
--rw-rw-r--  3.0 unx    12189 tx defN 23-May-08 02:54 static/pt/chapter-04.html
--rw-rw-r--  3.0 unx     7213 tx defN 23-May-08 02:54 static/pt/search.html
--rw-rw-r--  3.0 unx    50772 tx defN 23-May-08 02:54 static/pt/chapter-13.html
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 02:13 static/favicon.ico
--rw-rw-r--  3.0 unx      112 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    15647 tx defN 23-May-08 02:54 static/en/chapter-01.html
+-rw-r--r--  3.0 unx     7072 tx defN 23-May-08 02:54 static/en/search.html
+-rw-r--r--  3.0 unx    12025 tx defN 23-May-08 02:54 static/en/chapter-04.html
+-rw-r--r--  3.0 unx     1804 tx defN 23-May-08 01:34 static/en/_static/tabs.css
+-rw-r--r--  3.0 unx    18215 tx defN 23-May-08 02:54 static/en/_static/searchtools.js
+-rw-r--r--  3.0 unx      934 tx defN 23-May-08 01:34 static/en/_static/js/badge_only.js
+-rw-r--r--  3.0 unx     2734 tx defN 23-May-08 01:34 static/en/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-May-08 01:34 static/en/_static/js/theme.js
+-rw-r--r--  3.0 unx     4370 tx defN 23-May-08 01:34 static/en/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/en/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4712 tx defN 23-May-08 01:43 static/en/_static/sphinx_highlight.js
+-rw-r--r--  3.0 unx      286 bx stor 23-May-08 01:43 static/en/_static/file.png
+-rw-r--r--  3.0 unx     4819 tx defN 23-May-08 02:13 static/en/_static/pygments.css
+-rw-r--r--  3.0 unx     4758 tx defN 23-May-08 02:54 static/en/_static/language_data.js
+-rw-r--r--  3.0 unx       90 bx defN 23-May-08 01:43 static/en/_static/minus.png
+-rw-r--r--  3.0 unx    89501 tx defN 23-May-08 02:13 static/en/_static/jquery.js
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_static/logo.png
+-rw-r--r--  3.0 unx       90 bx defN 23-May-08 01:43 static/en/_static/plus.png
+-rw-r--r--  3.0 unx   135235 tx defN 23-May-08 02:54 static/en/_static/css/theme.css
+-rw-r--r--  3.0 unx     3229 tx defN 23-May-08 01:34 static/en/_static/css/badge_only.css
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/_static/css/dark.css
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/_static/css/toggle.css
+-rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/en/_static/logo-32x32.ico
+-rw-r--r--  3.0 unx     4289 tx defN 23-May-08 02:13 static/en/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--  3.0 unx    14813 tx defN 23-May-08 02:54 static/en/_static/basic.css
+-rw-r--r--  3.0 unx      427 tx defN 23-May-08 02:54 static/en/_static/documentation_options.js
+-rw-r--r--  3.0 unx     4472 tx defN 23-May-08 02:54 static/en/_static/doctools.js
+-rw-r--r--  3.0 unx     4231 tx defN 23-May-08 01:34 static/en/_static/tabs.js
+-rw-r--r--  3.0 unx    91571 tx defN 23-May-08 02:54 static/en/searchindex.js
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/en/dark.css
+-rw-r--r--  3.0 unx    11517 tx defN 23-May-08 02:54 static/en/chapter-11.html
+-rw-r--r--  3.0 unx    19145 tx defN 23-May-08 02:54 static/en/chapter-02.html
+-rw-r--r--  3.0 unx    85412 tx defN 23-May-08 02:54 static/en/chapter-16.html
+-rw-r--r--  3.0 unx     6797 tx defN 23-May-08 02:54 static/en/genindex.html
+-rw-r--r--  3.0 unx    50820 tx defN 23-May-08 02:54 static/en/chapter-13.html
+-rw-r--r--  3.0 unx   111701 tx defN 23-May-08 02:54 static/en/chapter-10.html
+-rw-r--r--  3.0 unx    54171 tx defN 23-May-08 02:54 static/en/chapter-14.html
+-rw-r--r--  3.0 unx    45554 tx defN 23-May-08 02:54 static/en/chapter-03.html
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/en/toggle.css
+-rw-r--r--  3.0 unx   500088 tx defN 23-May-08 02:54 static/en/chapter-07.html
+-rw-r--r--  3.0 unx   189735 tx defN 23-May-08 02:54 static/en/chapter-12.html
+-rw-r--r--  3.0 unx   129408 tx defN 23-May-08 02:54 static/en/chapter-08.html
+-rw-r--r--  3.0 unx    94874 tx defN 23-May-08 02:54 static/en/chapter-06.html
+-rw-r--r--  3.0 unx    63565 tx defN 23-May-08 02:54 static/en/chapter-09.html
+-rw-r--r--  3.0 unx    42541 tx defN 23-May-08 02:54 static/en/chapter-05.html
+-rw-r--r--  3.0 unx    19979 tx defN 23-May-08 02:54 static/en/index.html
+-rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/en/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/en/_images/command.png
+-rw-r--r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/en/_images/dashboard_new_app.png
+-rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/en/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/en/_images/form3.png
+-rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/en/_images/form5.png
+-rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/en/_images/restapi.png
+-rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/en/_images/form2.png
+-rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/en/_images/tags2.png
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/en/_images/logo.png
+-rw-r--r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/en/_images/first_run.png
+-rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/en/_images/simple_counter.png
+-rw-r--r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/en/_images/dashboard_login.png
+-rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/en/_images/_scaffold.png
+-rw-r--r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/en/_images/main_page.png
+-rw-r--r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/en/_images/grid.png
+-rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/en/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/en/_images/grid_nocss.png
+-rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/en/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/en/_images/form4.png
+-rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/en/_images/form1.png
+-rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/en/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/en/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/en/_images/dashboard.png
+-rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/en/_images/grid_columns.png
+-rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/en/_images/form6.png
+-rw-r--r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/en/_images/restapi2.png
+-rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/en/_images/dashboard_error.png
+-rw-r--r--  3.0 unx    43200 tx defN 23-May-08 02:54 static/en/chapter-15.html
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 02:13 static/favicon.ico
+-rw-r--r--  3.0 unx    16039 tx defN 23-May-08 02:54 static/pt/chapter-01.html
+-rw-r--r--  3.0 unx     7213 tx defN 23-May-08 02:54 static/pt/search.html
+-rw-r--r--  3.0 unx    12189 tx defN 23-May-08 02:54 static/pt/chapter-04.html
+-rw-r--r--  3.0 unx     1804 tx defN 23-May-08 01:34 static/pt/_static/tabs.css
+-rw-r--r--  3.0 unx    18215 tx defN 23-May-08 02:54 static/pt/_static/searchtools.js
+-rw-r--r--  3.0 unx      934 tx defN 23-May-08 01:34 static/pt/_static/js/badge_only.js
+-rw-r--r--  3.0 unx     2734 tx defN 23-May-08 01:34 static/pt/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-May-08 01:34 static/pt/_static/js/theme.js
+-rw-r--r--  3.0 unx     4370 tx defN 23-May-08 01:34 static/pt/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--  3.0 unx     1333 tx defN 23-May-08 00:39 static/pt/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4712 tx defN 23-May-08 01:43 static/pt/_static/sphinx_highlight.js
+-rw-r--r--  3.0 unx      286 bx stor 23-May-08 01:43 static/pt/_static/file.png
+-rw-r--r--  3.0 unx     4819 tx defN 23-May-08 02:13 static/pt/_static/pygments.css
+-rw-r--r--  3.0 unx    14417 tx defN 23-May-08 02:54 static/pt/_static/language_data.js
+-rw-r--r--  3.0 unx       90 bx defN 23-May-08 01:43 static/pt/_static/minus.png
+-rw-r--r--  3.0 unx    89501 tx defN 23-May-08 02:13 static/pt/_static/jquery.js
+-rw-r--r--  3.0 unx     8133 tx defN 23-May-08 01:43 static/pt/_static/base-stemmer.js
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_static/logo.png
+-rw-r--r--  3.0 unx       90 bx defN 23-May-08 01:43 static/pt/_static/plus.png
+-rw-r--r--  3.0 unx   135235 tx defN 23-May-08 02:54 static/pt/_static/css/theme.css
+-rw-r--r--  3.0 unx     3229 tx defN 23-May-08 01:34 static/pt/_static/css/badge_only.css
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/_static/css/dark.css
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/_static/css/toggle.css
+-rw-r--r--  3.0 unx     1989 bx stor 23-May-08 00:39 static/pt/_static/logo-32x32.ico
+-rw-r--r--  3.0 unx     4289 tx defN 23-May-08 02:13 static/pt/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--  3.0 unx    14813 tx defN 23-May-08 02:54 static/pt/_static/basic.css
+-rw-r--r--  3.0 unx      427 tx defN 23-May-08 02:54 static/pt/_static/documentation_options.js
+-rw-r--r--  3.0 unx    26718 tx defN 23-May-08 01:43 static/pt/_static/portuguese-stemmer.js
+-rw-r--r--  3.0 unx     4472 tx defN 23-May-08 02:54 static/pt/_static/doctools.js
+-rw-r--r--  3.0 unx     4231 tx defN 23-May-08 01:34 static/pt/_static/tabs.js
+-rw-r--r--  3.0 unx     2412 tx defN 23-May-08 01:43 static/pt/_static/translations.js
+-rw-r--r--  3.0 unx   125717 tx defN 23-May-08 02:54 static/pt/searchindex.js
+-rw-r--r--  3.0 unx     6515 tx defN 23-May-08 00:39 static/pt/dark.css
+-rw-r--r--  3.0 unx    11813 tx defN 23-May-08 02:54 static/pt/chapter-11.html
+-rw-r--r--  3.0 unx    19683 tx defN 23-May-08 02:54 static/pt/chapter-02.html
+-rw-r--r--  3.0 unx    85534 tx defN 23-May-08 02:54 static/pt/chapter-16.html
+-rw-r--r--  3.0 unx     6934 tx defN 23-May-08 02:54 static/pt/genindex.html
+-rw-r--r--  3.0 unx    50772 tx defN 23-May-08 02:54 static/pt/chapter-13.html
+-rw-r--r--  3.0 unx   105227 tx defN 23-May-08 02:54 static/pt/chapter-10.html
+-rw-r--r--  3.0 unx    54793 tx defN 23-May-08 02:54 static/pt/chapter-14.html
+-rw-r--r--  3.0 unx    44854 tx defN 23-May-08 02:54 static/pt/chapter-03.html
+-rw-r--r--  3.0 unx     1456 tx defN 23-May-08 00:39 static/pt/toggle.css
+-rw-r--r--  3.0 unx   464626 tx defN 23-May-08 02:54 static/pt/chapter-07.html
+-rw-r--r--  3.0 unx   189425 tx defN 23-May-08 02:54 static/pt/chapter-12.html
+-rw-r--r--  3.0 unx   129323 tx defN 23-May-08 02:54 static/pt/chapter-08.html
+-rw-r--r--  3.0 unx    93497 tx defN 23-May-08 02:54 static/pt/chapter-06.html
+-rw-r--r--  3.0 unx    61495 tx defN 23-May-08 02:54 static/pt/chapter-09.html
+-rw-r--r--  3.0 unx    41291 tx defN 23-May-08 02:54 static/pt/chapter-05.html
+-rw-r--r--  3.0 unx    19994 tx defN 23-May-08 02:54 static/pt/index.html
+-rw-r--r--  3.0 unx    40745 bx defN 23-May-08 00:39 static/pt/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    40478 bx defN 23-May-08 00:39 static/pt/_images/command.png
+-rw-r--r--  3.0 unx    40467 bx defN 23-May-08 00:39 static/pt/_images/dashboard_new_app.png
+-rw-r--r--  3.0 unx   174817 bx defN 23-May-08 00:39 static/pt/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    37805 bx defN 23-May-08 00:39 static/pt/_images/form3.png
+-rw-r--r--  3.0 unx    39765 bx defN 23-May-08 00:39 static/pt/_images/form5.png
+-rw-r--r--  3.0 unx    30536 bx defN 23-May-08 00:39 static/pt/_images/restapi.png
+-rw-r--r--  3.0 unx    40409 bx defN 23-May-08 00:39 static/pt/_images/form2.png
+-rw-r--r--  3.0 unx    30931 bx defN 23-May-08 00:39 static/pt/_images/tags2.png
+-rw-r--r--  3.0 unx   181425 bx defN 23-May-08 00:39 static/pt/_images/logo.png
+-rw-r--r--  3.0 unx    50011 bx defN 23-May-08 00:39 static/pt/_images/first_run.png
+-rw-r--r--  3.0 unx    16627 bx defN 23-May-08 00:39 static/pt/_images/simple_counter.png
+-rw-r--r--  3.0 unx    86267 bx defN 23-May-08 00:39 static/pt/_images/dashboard_login.png
+-rw-r--r--  3.0 unx    12086 bx defN 23-May-08 00:39 static/pt/_images/_scaffold.png
+-rw-r--r--  3.0 unx    77606 bx defN 23-May-08 00:39 static/pt/_images/main_page.png
+-rw-r--r--  3.0 unx    41285 bx defN 23-May-08 00:39 static/pt/_images/grid.png
+-rw-r--r--  3.0 unx   135864 bx defN 23-May-08 00:39 static/pt/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    44559 bx defN 23-May-08 00:39 static/pt/_images/grid_nocss.png
+-rw-r--r--  3.0 unx    24753 bx defN 23-May-08 00:39 static/pt/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 23-May-08 00:39 static/pt/_images/form4.png
+-rw-r--r--  3.0 unx    11257 bx defN 23-May-08 00:39 static/pt/_images/form1.png
+-rw-r--r--  3.0 unx   154315 bx defN 23-May-08 00:39 static/pt/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   147429 bx defN 23-May-08 00:39 static/pt/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    52898 bx defN 23-May-08 00:39 static/pt/_images/dashboard.png
+-rw-r--r--  3.0 unx    58653 bx defN 23-May-08 00:39 static/pt/_images/grid_columns.png
+-rw-r--r--  3.0 unx    38066 bx defN 23-May-08 00:39 static/pt/_images/form6.png
+-rw-r--r--  3.0 unx    29268 bx defN 23-May-08 00:39 static/pt/_images/restapi2.png
+-rw-r--r--  3.0 unx    53747 bx defN 23-May-08 00:39 static/pt/_images/dashboard_error.png
+-rw-r--r--  3.0 unx    43359 tx defN 23-May-08 02:54 static/pt/chapter-15.html
+-rw-r--r--  3.0 unx      248 tx defN 23-May-08 02:13 static/index.html
+-rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 __init__.py
 156 files, 7744000 bytes uncompressed, 4327657 bytes compressed:  44.1%
```

#### zipnote {}

```diff
@@ -1,469 +1,469 @@
-Filename: static/en/chapter-10.html
-Comment: 
-
-Filename: static/en/chapter-14.html
+Filename: static/en/chapter-01.html
 Comment: 
 
-Filename: static/en/chapter-03.html
+Filename: static/en/search.html
 Comment: 
 
-Filename: static/en/chapter-05.html
+Filename: static/en/chapter-04.html
 Comment: 
 
-Filename: static/en/chapter-16.html
+Filename: static/en/_static/tabs.css
 Comment: 
 
-Filename: static/en/chapter-06.html
+Filename: static/en/_static/searchtools.js
 Comment: 
 
-Filename: static/en/index.html
+Filename: static/en/_static/js/badge_only.js
 Comment: 
 
-Filename: static/en/chapter-09.html
+Filename: static/en/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/en/_static/tabs.css
+Filename: static/en/_static/js/theme.js
 Comment: 
 
-Filename: static/en/_static/documentation_options.js
+Filename: static/en/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/en/_static/tabs.js
+Filename: static/en/_static/js/toggle.js
 Comment: 
 
 Filename: static/en/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/en/_static/jquery.js
-Comment: 
-
-Filename: static/en/_static/minus.png
+Filename: static/en/_static/file.png
 Comment: 
 
-Filename: static/en/_static/plus.png
+Filename: static/en/_static/pygments.css
 Comment: 
 
 Filename: static/en/_static/language_data.js
 Comment: 
 
-Filename: static/en/_static/pygments.css
+Filename: static/en/_static/minus.png
 Comment: 
 
-Filename: static/en/_static/logo.png
+Filename: static/en/_static/jquery.js
 Comment: 
 
-Filename: static/en/_static/searchtools.js
+Filename: static/en/_static/logo.png
 Comment: 
 
-Filename: static/en/_static/_sphinx_javascript_frameworks_compat.js
+Filename: static/en/_static/plus.png
 Comment: 
 
 Filename: static/en/_static/css/theme.css
 Comment: 
 
-Filename: static/en/_static/css/toggle.css
-Comment: 
-
 Filename: static/en/_static/css/badge_only.css
 Comment: 
 
 Filename: static/en/_static/css/dark.css
 Comment: 
 
+Filename: static/en/_static/css/toggle.css
+Comment: 
+
 Filename: static/en/_static/logo-32x32.ico
 Comment: 
 
-Filename: static/en/_static/js/html5shiv-printshiv.min.js
+Filename: static/en/_static/_sphinx_javascript_frameworks_compat.js
 Comment: 
 
-Filename: static/en/_static/js/badge_only.js
+Filename: static/en/_static/basic.css
 Comment: 
 
-Filename: static/en/_static/js/toggle.js
+Filename: static/en/_static/documentation_options.js
 Comment: 
 
-Filename: static/en/_static/js/theme.js
+Filename: static/en/_static/doctools.js
 Comment: 
 
-Filename: static/en/_static/js/html5shiv.min.js
+Filename: static/en/_static/tabs.js
 Comment: 
 
-Filename: static/en/_static/file.png
+Filename: static/en/searchindex.js
 Comment: 
 
-Filename: static/en/_static/doctools.js
+Filename: static/en/dark.css
 Comment: 
 
-Filename: static/en/_static/basic.css
+Filename: static/en/chapter-11.html
 Comment: 
 
-Filename: static/en/chapter-15.html
+Filename: static/en/chapter-02.html
 Comment: 
 
-Filename: static/en/chapter-12.html
+Filename: static/en/chapter-16.html
 Comment: 
 
-Filename: static/en/searchindex.js
+Filename: static/en/genindex.html
 Comment: 
 
-Filename: static/en/chapter-02.html
+Filename: static/en/chapter-13.html
 Comment: 
 
-Filename: static/en/chapter-11.html
+Filename: static/en/chapter-10.html
 Comment: 
 
-Filename: static/en/chapter-01.html
+Filename: static/en/chapter-14.html
 Comment: 
 
-Filename: static/en/genindex.html
+Filename: static/en/chapter-03.html
 Comment: 
 
 Filename: static/en/toggle.css
 Comment: 
 
+Filename: static/en/chapter-07.html
+Comment: 
+
+Filename: static/en/chapter-12.html
+Comment: 
+
 Filename: static/en/chapter-08.html
 Comment: 
 
-Filename: static/en/_images/form1.png
+Filename: static/en/chapter-06.html
 Comment: 
 
-Filename: static/en/_images/dashboard_ticket.png
+Filename: static/en/chapter-09.html
 Comment: 
 
-Filename: static/en/_images/form3.png
+Filename: static/en/chapter-05.html
 Comment: 
 
-Filename: static/en/_images/dashboard_edit.png
+Filename: static/en/index.html
 Comment: 
 
-Filename: static/en/_images/form2.png
+Filename: static/en/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/en/_images/grid.png
+Filename: static/en/_images/command.png
 Comment: 
 
-Filename: static/en/_images/restapi2.png
+Filename: static/en/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/en/_images/simple_counter.png
+Filename: static/en/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/en/_images/restapi.png
+Filename: static/en/_images/form3.png
 Comment: 
 
 Filename: static/en/_images/form5.png
 Comment: 
 
-Filename: static/en/_images/dashboard_login.png
+Filename: static/en/_images/restapi.png
 Comment: 
 
-Filename: static/en/_images/dashboard_restapi.png
+Filename: static/en/_images/form2.png
 Comment: 
 
-Filename: static/en/_images/dashboard_main.png
+Filename: static/en/_images/tags2.png
 Comment: 
 
-Filename: static/en/_images/grid_columns.png
+Filename: static/en/_images/logo.png
 Comment: 
 
-Filename: static/en/_images/grid_bulmacss.png
+Filename: static/en/_images/first_run.png
 Comment: 
 
-Filename: static/en/_images/_scaffold.png
+Filename: static/en/_images/simple_counter.png
 Comment: 
 
-Filename: static/en/_images/logo.png
+Filename: static/en/_images/dashboard_login.png
 Comment: 
 
-Filename: static/en/_images/dashboard.png
+Filename: static/en/_images/_scaffold.png
 Comment: 
 
-Filename: static/en/_images/tags2.png
+Filename: static/en/_images/main_page.png
 Comment: 
 
-Filename: static/en/_images/form4.png
+Filename: static/en/_images/grid.png
 Comment: 
 
-Filename: static/en/_images/dashboard_error.png
+Filename: static/en/_images/dashboard_main.png
 Comment: 
 
 Filename: static/en/_images/grid_nocss.png
 Comment: 
 
 Filename: static/en/_images/tags_db.png
 Comment: 
 
-Filename: static/en/_images/dashboard_new_app.png
-Comment: 
-
-Filename: static/en/_images/main_page.png
+Filename: static/en/_images/form4.png
 Comment: 
 
-Filename: static/en/_images/command.png
+Filename: static/en/_images/form1.png
 Comment: 
 
-Filename: static/en/_images/first_run.png
+Filename: static/en/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/en/_images/form6.png
+Filename: static/en/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/en/dark.css
+Filename: static/en/_images/dashboard.png
 Comment: 
 
-Filename: static/en/chapter-07.html
+Filename: static/en/_images/grid_columns.png
 Comment: 
 
-Filename: static/en/chapter-04.html
+Filename: static/en/_images/form6.png
 Comment: 
 
-Filename: static/en/search.html
+Filename: static/en/_images/restapi2.png
 Comment: 
 
-Filename: static/en/chapter-13.html
+Filename: static/en/_images/dashboard_error.png
 Comment: 
 
-Filename: static/index.html
+Filename: static/en/chapter-15.html
 Comment: 
 
-Filename: static/pt/chapter-10.html
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/pt/chapter-14.html
+Filename: static/pt/chapter-01.html
 Comment: 
 
-Filename: static/pt/chapter-03.html
+Filename: static/pt/search.html
 Comment: 
 
-Filename: static/pt/chapter-05.html
+Filename: static/pt/chapter-04.html
 Comment: 
 
-Filename: static/pt/chapter-16.html
+Filename: static/pt/_static/tabs.css
 Comment: 
 
-Filename: static/pt/chapter-06.html
+Filename: static/pt/_static/searchtools.js
 Comment: 
 
-Filename: static/pt/index.html
+Filename: static/pt/_static/js/badge_only.js
 Comment: 
 
-Filename: static/pt/chapter-09.html
+Filename: static/pt/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/pt/_static/tabs.css
+Filename: static/pt/_static/js/theme.js
 Comment: 
 
-Filename: static/pt/_static/documentation_options.js
+Filename: static/pt/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/pt/_static/tabs.js
+Filename: static/pt/_static/js/toggle.js
 Comment: 
 
 Filename: static/pt/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/pt/_static/jquery.js
+Filename: static/pt/_static/file.png
 Comment: 
 
-Filename: static/pt/_static/minus.png
+Filename: static/pt/_static/pygments.css
 Comment: 
 
-Filename: static/pt/_static/translations.js
+Filename: static/pt/_static/language_data.js
 Comment: 
 
-Filename: static/pt/_static/plus.png
+Filename: static/pt/_static/minus.png
 Comment: 
 
-Filename: static/pt/_static/language_data.js
+Filename: static/pt/_static/jquery.js
 Comment: 
 
-Filename: static/pt/_static/pygments.css
+Filename: static/pt/_static/base-stemmer.js
 Comment: 
 
 Filename: static/pt/_static/logo.png
 Comment: 
 
-Filename: static/pt/_static/base-stemmer.js
+Filename: static/pt/_static/plus.png
 Comment: 
 
-Filename: static/pt/_static/searchtools.js
+Filename: static/pt/_static/css/theme.css
 Comment: 
 
-Filename: static/pt/_static/_sphinx_javascript_frameworks_compat.js
+Filename: static/pt/_static/css/badge_only.css
 Comment: 
 
-Filename: static/pt/_static/css/theme.css
+Filename: static/pt/_static/css/dark.css
 Comment: 
 
 Filename: static/pt/_static/css/toggle.css
 Comment: 
 
-Filename: static/pt/_static/css/badge_only.css
+Filename: static/pt/_static/logo-32x32.ico
 Comment: 
 
-Filename: static/pt/_static/css/dark.css
+Filename: static/pt/_static/_sphinx_javascript_frameworks_compat.js
 Comment: 
 
-Filename: static/pt/_static/logo-32x32.ico
+Filename: static/pt/_static/basic.css
+Comment: 
+
+Filename: static/pt/_static/documentation_options.js
 Comment: 
 
 Filename: static/pt/_static/portuguese-stemmer.js
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv-printshiv.min.js
+Filename: static/pt/_static/doctools.js
 Comment: 
 
-Filename: static/pt/_static/js/badge_only.js
+Filename: static/pt/_static/tabs.js
 Comment: 
 
-Filename: static/pt/_static/js/toggle.js
+Filename: static/pt/_static/translations.js
 Comment: 
 
-Filename: static/pt/_static/js/theme.js
+Filename: static/pt/searchindex.js
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv.min.js
+Filename: static/pt/dark.css
 Comment: 
 
-Filename: static/pt/_static/file.png
+Filename: static/pt/chapter-11.html
 Comment: 
 
-Filename: static/pt/_static/doctools.js
+Filename: static/pt/chapter-02.html
 Comment: 
 
-Filename: static/pt/_static/basic.css
+Filename: static/pt/chapter-16.html
 Comment: 
 
-Filename: static/pt/chapter-15.html
+Filename: static/pt/genindex.html
 Comment: 
 
-Filename: static/pt/chapter-12.html
+Filename: static/pt/chapter-13.html
 Comment: 
 
-Filename: static/pt/searchindex.js
+Filename: static/pt/chapter-10.html
 Comment: 
 
-Filename: static/pt/chapter-02.html
+Filename: static/pt/chapter-14.html
 Comment: 
 
-Filename: static/pt/chapter-11.html
+Filename: static/pt/chapter-03.html
 Comment: 
 
-Filename: static/pt/chapter-01.html
+Filename: static/pt/toggle.css
 Comment: 
 
-Filename: static/pt/genindex.html
+Filename: static/pt/chapter-07.html
 Comment: 
 
-Filename: static/pt/toggle.css
+Filename: static/pt/chapter-12.html
 Comment: 
 
 Filename: static/pt/chapter-08.html
 Comment: 
 
-Filename: static/pt/_images/form1.png
+Filename: static/pt/chapter-06.html
 Comment: 
 
-Filename: static/pt/_images/dashboard_ticket.png
+Filename: static/pt/chapter-09.html
 Comment: 
 
-Filename: static/pt/_images/form3.png
+Filename: static/pt/chapter-05.html
 Comment: 
 
-Filename: static/pt/_images/dashboard_edit.png
+Filename: static/pt/index.html
 Comment: 
 
-Filename: static/pt/_images/form2.png
+Filename: static/pt/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/pt/_images/grid.png
+Filename: static/pt/_images/command.png
 Comment: 
 
-Filename: static/pt/_images/restapi2.png
+Filename: static/pt/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/pt/_images/simple_counter.png
+Filename: static/pt/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/pt/_images/restapi.png
+Filename: static/pt/_images/form3.png
 Comment: 
 
 Filename: static/pt/_images/form5.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_login.png
+Filename: static/pt/_images/restapi.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_restapi.png
+Filename: static/pt/_images/form2.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_main.png
+Filename: static/pt/_images/tags2.png
 Comment: 
 
-Filename: static/pt/_images/grid_columns.png
+Filename: static/pt/_images/logo.png
 Comment: 
 
-Filename: static/pt/_images/grid_bulmacss.png
+Filename: static/pt/_images/first_run.png
 Comment: 
 
-Filename: static/pt/_images/_scaffold.png
+Filename: static/pt/_images/simple_counter.png
 Comment: 
 
-Filename: static/pt/_images/logo.png
+Filename: static/pt/_images/dashboard_login.png
 Comment: 
 
-Filename: static/pt/_images/dashboard.png
+Filename: static/pt/_images/_scaffold.png
 Comment: 
 
-Filename: static/pt/_images/tags2.png
+Filename: static/pt/_images/main_page.png
 Comment: 
 
-Filename: static/pt/_images/form4.png
+Filename: static/pt/_images/grid.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_error.png
+Filename: static/pt/_images/dashboard_main.png
 Comment: 
 
 Filename: static/pt/_images/grid_nocss.png
 Comment: 
 
 Filename: static/pt/_images/tags_db.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_new_app.png
+Filename: static/pt/_images/form4.png
 Comment: 
 
-Filename: static/pt/_images/main_page.png
+Filename: static/pt/_images/form1.png
 Comment: 
 
-Filename: static/pt/_images/command.png
+Filename: static/pt/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/pt/_images/first_run.png
+Filename: static/pt/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/pt/_images/form6.png
+Filename: static/pt/_images/dashboard.png
 Comment: 
 
-Filename: static/pt/dark.css
+Filename: static/pt/_images/grid_columns.png
 Comment: 
 
-Filename: static/pt/chapter-07.html
+Filename: static/pt/_images/form6.png
 Comment: 
 
-Filename: static/pt/chapter-04.html
+Filename: static/pt/_images/restapi2.png
 Comment: 
 
-Filename: static/pt/search.html
+Filename: static/pt/_images/dashboard_error.png
 Comment: 
 
-Filename: static/pt/chapter-13.html
+Filename: static/pt/chapter-15.html
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/index.html
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app._minimal.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,5 +1,5 @@
 Zip file size: 5245 bytes, number of entries: 3
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 __init__.py
 3 files, 32122 bytes uncompressed, 4749 bytes compressed:  85.2%
```

#### zipnote {}

```diff
@@ -1,10 +1,10 @@
-Filename: static/README.md
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/README.md
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
 Zip file size: 21524 bytes, number of entries: 16
--rw-rw-r--  3.0 unx     7744 tx defN 23-May-08 00:39 common.py
--rw-rw-r--  3.0 unx     3002 tx defN 23-May-08 00:39 settings.py
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
--rw-rw-r--  3.0 unx    11431 tx defN 23-May-08 00:39 static/css/no.css
--rw-rw-r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx      852 tx defN 23-May-08 00:39 tasks.py
--rw-rw-r--  3.0 unx      375 tx defN 23-May-08 00:39 __init__.py
--rw-rw-r--  3.0 unx      254 tx defN 23-May-08 00:39 models.py
--rw-rw-r--  3.0 unx      103 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 templates/README.md
--rw-rw-r--  3.0 unx      264 tx defN 23-May-08 00:39 templates/generic.html
--rw-rw-r--  3.0 unx     2860 tx defN 23-May-08 00:39 templates/layout.html
--rw-rw-r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
--rw-rw-r--  3.0 unx     1470 tx defN 23-May-08 00:39 controllers.py
--rw-rw-r--  3.0 unx       97 tx defN 23-May-08 00:39 translations/it.json
+-rw-r--r--  3.0 unx      254 tx defN 23-May-08 00:39 models.py
+-rw-r--r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx    11431 tx defN 23-May-08 00:39 static/css/no.css
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/README.md
+-rw-r--r--  3.0 unx      852 tx defN 23-May-08 00:39 tasks.py
+-rw-r--r--  3.0 unx       97 tx defN 23-May-08 00:39 translations/it.json
+-rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 controllers.py
+-rw-r--r--  3.0 unx     3002 tx defN 23-May-08 00:39 settings.py
+-rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
+-rw-r--r--  3.0 unx      103 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 templates/generic.html
+-rw-r--r--  3.0 unx     2860 tx defN 23-May-08 00:39 templates/layout.html
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 templates/README.md
+-rw-r--r--  3.0 unx     7744 tx defN 23-May-08 00:39 common.py
 16 files, 72658 bytes uncompressed, 18950 bytes compressed:  73.9%
```

#### zipnote {}

```diff
@@ -1,49 +1,49 @@
-Filename: common.py
+Filename: models.py
 Comment: 
 
-Filename: settings.py
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/README.md
+Filename: static/favicon.ico
 Comment: 
 
 Filename: static/css/no.css
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/README.md
 Comment: 
 
-Filename: static/favicon.ico
+Filename: tasks.py
 Comment: 
 
-Filename: tasks.py
+Filename: translations/it.json
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
-Filename: models.py
+Filename: controllers.py
 Comment: 
 
-Filename: templates/index.html
+Filename: settings.py
 Comment: 
 
-Filename: templates/README.md
+Filename: templates/auth.html
 Comment: 
 
-Filename: templates/generic.html
+Filename: templates/index.html
 Comment: 
 
-Filename: templates/layout.html
+Filename: templates/generic.html
 Comment: 
 
-Filename: templates/auth.html
+Filename: templates/layout.html
 Comment: 
 
-Filename: controllers.py
+Filename: templates/README.md
 Comment: 
 
-Filename: translations/it.json
+Filename: common.py
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230521.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230528.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,145 +1,145 @@
 Zip file size: 1385465 bytes, number of entries: 143
--rw-rw-r--  3.0 unx      264 tx defN 23-May-08 00:39 examples/session_counter.py
--rw-rw-r--  3.0 unx      396 tx defN 23-May-08 00:39 examples/custom_form.py
--rw-rw-r--  3.0 unx     1616 tx defN 23-May-08 00:39 examples/hcaptcha_form.py
--rw-rw-r--  3.0 unx      227 tx defN 23-May-08 00:39 examples/page_with_query.py
--rw-rw-r--  3.0 unx      125 tx defN 23-May-08 00:39 examples/hello_world.py
--rw-rw-r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
--rw-rw-r--  3.0 unx      181 tx defN 23-May-08 00:39 examples/page_with_redirect.py
--rw-rw-r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
--rw-rw-r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
--rw-rw-r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
--rw-rw-r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
--rw-rw-r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
--rw-rw-r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
--rw-rw-r--  3.0 unx      372 tx defN 23-May-08 00:39 examples/flash_example_fixture.py
--rw-rw-r--  3.0 unx      370 tx defN 23-May-08 00:39 examples/example_ajax_grid.py
--rw-rw-r--  3.0 unx      517 tx defN 23-May-08 00:39 examples/socketio.py
--rw-rw-r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
--rw-rw-r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
--rw-rw-r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
--rw-rw-r--  3.0 unx     1583 tx defN 23-May-08 00:39 examples/example_html_grid.py
--rw-rw-r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
--rw-rw-r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
--rw-rw-r--  3.0 unx      647 tx defN 23-May-08 00:39 examples/auth_forms.py
--rw-rw-r--  3.0 unx     1470 tx defN 23-May-08 00:39 examples/settings.py
--rw-rw-r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
--rw-rw-r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
--rw-rw-r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
--rw-rw-r--  3.0 unx      644 tx defN 23-May-08 00:39 examples/rpc.py
--rw-rw-r--  3.0 unx      197 tx defN 23-May-08 00:39 examples/session_clear.py
--rw-rw-r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
--rw-rw-r--  3.0 unx      228 tx defN 23-May-08 00:39 examples/flash_example_naive.py
--rw-rw-r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
--rw-rw-r--  3.0 unx     2617 tx defN 23-May-08 00:39 examples/models.py
--rw-rw-r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
--rw-rw-r--  3.0 unx     2749 tx defN 23-May-08 00:39 examples/rest.py
--rw-rw-r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
--rwxrwxr-x  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
--rw-rw-r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
--rw-rw-r--  3.0 unx       12 tx stor 23-May-08 00:39 static/hello.txt
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/ws/README.md
--rw-rw-r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components/grid/grid.js
--rw-rw-r--  3.0 unx     3299 tx defN 23-May-08 00:39 static/components/grid/grid.html
--rw-rw-r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components/grid/grid.css
--rw-rw-r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components/vueform/luxon.js
--rw-rw-r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components/vueform/luxon.min.js
--rw-rw-r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components/vueform/vueform.html
--rw-rw-r--  3.0 unx     7263 tx defN 23-May-08 00:39 static/components/vueform/vueform.js
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.html
--rw-rw-r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components/fileupload/fileupload.css
--rw-rw-r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components/starrater/starrater.html
--rw-rw-r--  3.0 unx     1681 tx defN 23-May-08 00:39 static/components/starrater/starrater.js
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components/starrater/starrater.css
--rw-rw-r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
--rw-rw-r--  3.0 unx      977 tx defN 23-May-08 00:39 static/firebase-push.html
--rw-rw-r--  3.0 unx        1 tx stor 23-May-08 00:39 static/socketio/README.md
--rw-rw-r--  3.0 unx     9998 tx defN 23-May-08 00:39 static/error.html
--rw-rw-r--  3.0 unx     1903 tx defN 23-May-08 00:39 static/css/prism.css
--rw-rw-r--  3.0 unx    11417 tx defN 23-May-08 00:39 static/css/no.css
--rw-rw-r--  3.0 unx      496 tx defN 23-May-08 00:39 static/js/star_rater_vue.js
--rw-rw-r--  3.0 unx      868 tx defN 23-May-08 00:39 static/js/firebase-push.js
--rw-rw-r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
--rw-rw-r--  3.0 unx     8311 tx defN 23-May-08 00:39 static/js/utils.min.js
--rw-rw-r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
--rw-rw-r--  3.0 unx    14265 tx defN 23-May-08 00:39 static/js/axios.min.js
--rw-rw-r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
--rw-rw-r--  3.0 unx    19055 tx defN 23-May-08 00:39 static/js/prism.js
--rw-rw-r--  3.0 unx   341462 tx defN 23-May-08 00:39 static/js/vue.js
--rw-rw-r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
--rw-rw-r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.js
--rw-rw-r--  3.0 unx     3369 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.html
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/grid/luxon.js
--rw-rw-r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.css
--rw-rw-r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components-bulma/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.js
--rw-rw-r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.min.js
--rw-rw-r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.html
--rw-rw-r--  3.0 unx     7257 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.js
--rw-rw-r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.html
--rw-rw-r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components-bulma/fileupload/fileupload.css
--rw-rw-r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components-bulma/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.html
--rw-rw-r--  3.0 unx     1687 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.js
--rw-rw-r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components-bulma/starrater/starrater.css
--rw-rw-r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components-bulma/mtable.html
--rw-rw-r--  3.0 unx  7330359 tx defN 23-May-08 00:39 static/data/uscities.json
--rw-rw-r--  3.0 unx   295408 tx defN 23-May-08 00:39 static/data/zip_codes.json
--rw-rw-r--  3.0 unx     4146 tx defN 23-May-08 00:39 __init__.py
--rw-rw-r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
--rw-rw-r--  3.0 unx     6788 tx defN 23-May-08 00:39 templates/index.html
--rw-rw-r--  3.0 unx     2172 tx defN 23-May-08 00:39 templates/ws/ws_index.html
--rw-rw-r--  3.0 unx      263 tx defN 23-May-08 00:39 templates/examples/session_counter.html
--rw-rw-r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/flash_example.html
--rw-rw-r--  3.0 unx     1711 tx defN 23-May-08 00:39 templates/examples/tagsinput_form.html
--rw-rw-r--  3.0 unx       26 tx stor 23-May-08 00:39 templates/examples/flash_example_next.html
--rw-rw-r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
--rw-rw-r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
--rw-rw-r--  3.0 unx      869 tx defN 23-May-08 00:39 templates/examples/custom_form.html
--rw-rw-r--  3.0 unx      305 tx defN 23-May-08 00:39 templates/examples/form.html
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
--rw-rw-r--  3.0 unx      646 tx defN 23-May-08 00:39 templates/examples/auth_forms.html
--rw-rw-r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
--rw-rw-r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
--rw-rw-r--  3.0 unx       82 tx defN 23-May-08 00:39 templates/examples/page_with_template.html
--rw-rw-r--  3.0 unx      551 tx defN 23-May-08 00:39 templates/examples/auth_custom_login.html
--rw-rw-r--  3.0 unx     1025 tx defN 23-May-08 00:39 templates/examples/rest_info.html
--rw-rw-r--  3.0 unx      189 tx defN 23-May-08 00:39 templates/examples/hcaptcha_form.html
--rw-rw-r--  3.0 unx       69 tx defN 23-May-08 00:39 templates/examples/ajax_grid.html
--rw-rw-r--  3.0 unx     1913 tx defN 23-May-08 00:39 templates/socketio/socketio_index.html
--rw-rw-r--  3.0 unx      502 tx defN 23-May-08 00:39 templates/vue/star_rater_vue.html
--rw-rw-r--  3.0 unx      448 tx defN 23-May-08 00:39 templates/vue/starrating.html
--rw-rw-r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/edit_form.html
--rw-rw-r--  3.0 unx      372 tx defN 23-May-08 00:39 templates/vue/file_uploader.html
--rw-rw-r--  3.0 unx      544 tx defN 23-May-08 00:39 templates/vue/star_rater_vue_bulma.html
--rw-rw-r--  3.0 unx      488 tx defN 23-May-08 00:39 templates/vue/insert_form.html
--rw-rw-r--  3.0 unx      683 tx defN 23-May-08 00:39 templates/vue/vue_grid_and_forms.html
--rw-rw-r--  3.0 unx      392 tx defN 23-May-08 00:39 templates/vue/vuegrid_bulma.html
--rw-rw-r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/view_form.html
--rw-rw-r--  3.0 unx      374 tx defN 23-May-08 00:39 templates/vue/vuegrid.html
--rw-rw-r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
--rw-rw-r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
--rw-rw-r--  3.0 unx     2156 tx defN 23-May-08 00:39 templates/layout_bulma.html
--rw-rw-r--  3.0 unx      430 tx defN 23-May-08 00:39 templates/show.html
--rw-rw-r--  3.0 unx      236 tx defN 23-May-08 00:39 translations/it.json
--rw-rw-r--  3.0 unx      196 tx defN 23-May-08 00:39 translations/en.json
--rw-rw-r--  3.0 unx     3031 tx defN 23-May-08 00:39 vue_components_examples/vue_grid_and_forms.py
--rw-rw-r--  3.0 unx     1597 tx defN 23-May-08 00:39 vue_components_examples/components/fileupload.py
--rw-rw-r--  3.0 unx    10333 tx defN 23-May-08 00:39 vue_components_examples/components/vueform.py
--rw-rw-r--  3.0 unx     7777 tx defN 23-May-08 00:39 vue_components_examples/components/grid.py
--rw-rw-r--  3.0 unx     7858 tx defN 23-May-08 00:39 vue_components_examples/components/README.md
--rw-rw-r--  3.0 unx     2078 tx defN 23-May-08 00:39 vue_components_examples/components/starrater.py
--rw-rw-r--  3.0 unx      324 tx defN 23-May-08 00:39 vue_components_examples/vue_file_uploader.py
--rw-rw-r--  3.0 unx     1215 tx defN 23-May-08 00:39 vue_components_examples/vue_star_rater.py
--rw-rw-r--  3.0 unx       32 tx stor 23-May-08 00:39 vue_components_examples/common.py
--rw-rw-r--  3.0 unx     1124 tx defN 23-May-08 00:39 vue_components_examples/vue_edit_form.py
--rw-rw-r--  3.0 unx      853 tx defN 23-May-08 00:39 vue_components_examples/vue_insert_form.py
--rw-rw-r--  3.0 unx     1149 tx defN 23-May-08 00:39 vue_components_examples/vue_view_form.py
--rw-rw-r--  3.0 unx       34 tx stor 23-May-08 00:39 vue_components_examples/settings.py
--rw-rw-r--  3.0 unx     1390 tx defN 23-May-08 00:39 vue_components_examples/models.py
--rw-rw-r--  3.0 unx      302 tx defN 23-May-08 00:39 vue_components_examples/vue_grid.py
+-rw-r--r--  3.0 unx      181 tx defN 23-May-08 00:39 examples/page_with_redirect.py
+-rw-r--r--  3.0 unx      197 tx defN 23-May-08 00:39 examples/session_clear.py
+-rw-r--r--  3.0 unx      281 tx defN 23-May-08 00:39 examples/page_with_parameters.py
+-rw-r--r--  3.0 unx     2617 tx defN 23-May-08 00:39 examples/models.py
+-rw-r--r--  3.0 unx     1616 tx defN 23-May-08 00:39 examples/hcaptcha_form.py
+-rw-r--r--  3.0 unx      517 tx defN 23-May-08 00:39 examples/socketio.py
+-rw-r--r--  3.0 unx      255 tx defN 23-May-08 00:39 examples/show_a_button.py
+-rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 examples/flash_example_naive.py
+-rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 examples/flash_example_fixture.py
+-rw-r--r--  3.0 unx      414 tx defN 23-May-08 00:39 examples/test_expose.py
+-rw-r--r--  3.0 unx     2749 tx defN 23-May-08 00:39 examples/rest.py
+-rw-r--r--  3.0 unx     1583 tx defN 23-May-08 00:39 examples/example_html_grid.py
+-rw-r--r--  3.0 unx      349 tx defN 23-May-08 00:39 examples/count.py
+-rw-r--r--  3.0 unx      171 tx defN 23-May-08 00:39 examples/page_with_template.py
+-rw-r--r--  3.0 unx      396 tx defN 23-May-08 00:39 examples/custom_form.py
+-rw-r--r--  3.0 unx     1966 tx defN 23-May-08 00:39 examples/example_multiple_forms.py
+-rw-r--r--  3.0 unx      456 tx defN 23-May-08 00:39 examples/create_form.py
+-rw-r--r--  3.0 unx      644 tx defN 23-May-08 00:39 examples/rpc.py
+-rw-r--r--  3.0 unx      370 tx defN 23-May-08 00:39 examples/example_ajax_grid.py
+-rw-r--r--  3.0 unx      647 tx defN 23-May-08 00:39 examples/auth_forms.py
+-rw-r--r--  3.0 unx      465 tx defN 23-May-08 00:39 examples/update_form.py
+-rw-r--r--  3.0 unx      264 tx defN 23-May-08 00:39 examples/session_counter.py
+-rw-r--r--  3.0 unx      375 tx defN 23-May-08 00:39 examples/tagsinput_form.py
+-rw-r--r--  3.0 unx      870 tx defN 23-May-08 00:39 examples/component_loader.py
+-rw-r--r--  3.0 unx      378 tx defN 23-May-08 00:39 examples/auth_form.py
+-rw-r--r--  3.0 unx      227 tx defN 23-May-08 00:39 examples/page_with_query.py
+-rw-r--r--  3.0 unx      420 tx defN 23-May-08 00:39 examples/page_with_postback.py
+-rw-r--r--  3.0 unx      272 tx defN 23-May-08 00:39 examples/ws.py
+-rw-r--r--  3.0 unx       88 tx defN 23-May-08 00:39 examples/page_with_error.py
+-rw-r--r--  3.0 unx     1470 tx defN 23-May-08 00:39 examples/settings.py
+-rw-r--r--  3.0 unx      145 tx defN 23-May-08 00:39 examples/hello_world_msg.py
+-rw-r--r--  3.0 unx      106 tx defN 23-May-08 00:39 examples/page_without_template.py
+-rwxr--r--  3.0 unx      422 tx defN 23-May-08 00:39 examples/ws_client_example.py
+-rw-r--r--  3.0 unx      112 tx defN 23-May-08 00:39 examples/page_with_raise.py
+-rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 examples/example_helpers.py
+-rw-r--r--  3.0 unx      130 tx defN 23-May-08 00:39 examples/hello.py
+-rw-r--r--  3.0 unx     4809 tx defN 23-May-08 00:39 examples/common.py
+-rw-r--r--  3.0 unx      125 tx defN 23-May-08 00:39 examples/hello_world.py
+-rw-r--r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components/mtable.js
+-rw-r--r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components/grid/grid.css
+-rw-r--r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components/grid/grid.js
+-rw-r--r--  3.0 unx     3299 tx defN 23-May-08 00:39 static/components/grid/grid.html
+-rw-r--r--  3.0 unx     7263 tx defN 23-May-08 00:39 static/components/vueform/vueform.js
+-rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components/vueform/vueform.css
+-rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components/vueform/luxon.min.js
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components/vueform/luxon.js
+-rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components/vueform/vueform.html
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components/starrater/starrater.css
+-rw-r--r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components/starrater/starrater.html
+-rw-r--r--  3.0 unx     1681 tx defN 23-May-08 00:39 static/components/starrater/starrater.js
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components/mtable.html
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.html
+-rw-r--r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components/fileupload/fileupload.css
+-rw-r--r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components/fileupload/fileupload.js
+-rw-r--r--  3.0 unx    19055 tx defN 23-May-08 00:39 static/js/prism.js
+-rw-r--r--  3.0 unx      496 tx defN 23-May-08 00:39 static/js/star_rater_vue.js
+-rw-r--r--  3.0 unx      868 tx defN 23-May-08 00:39 static/js/firebase-push.js
+-rw-r--r--  3.0 unx    11888 tx defN 23-May-08 00:39 static/js/utils.js
+-rw-r--r--  3.0 unx    93670 tx defN 23-May-08 00:39 static/js/vue.min.js
+-rw-r--r--  3.0 unx    68547 tx defN 23-May-08 00:39 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    14265 tx defN 23-May-08 00:39 static/js/axios.min.js
+-rw-r--r--  3.0 unx   341462 tx defN 23-May-08 00:39 static/js/vue.js
+-rw-r--r--  3.0 unx     8311 tx defN 23-May-08 00:39 static/js/utils.min.js
+-rw-r--r--  3.0 unx     9998 tx defN 23-May-08 00:39 static/error.html
+-rw-r--r--  3.0 unx   295408 tx defN 23-May-08 00:39 static/data/zip_codes.json
+-rw-r--r--  3.0 unx  7330359 tx defN 23-May-08 00:39 static/data/uscities.json
+-rw-r--r--  3.0 unx    32038 bx defN 23-May-08 00:39 static/favicon.ico
+-rw-r--r--  3.0 unx      977 tx defN 23-May-08 00:39 static/firebase-push.html
+-rw-r--r--  3.0 unx     1903 tx defN 23-May-08 00:39 static/css/prism.css
+-rw-r--r--  3.0 unx    11417 tx defN 23-May-08 00:39 static/css/no.css
+-rw-r--r--  3.0 unx     8097 tx defN 23-May-08 00:39 static/components-bulma/mtable.js
+-rw-r--r--  3.0 unx      411 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.css
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/grid/luxon.js
+-rw-r--r--  3.0 unx     5384 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.js
+-rw-r--r--  3.0 unx     3369 tx defN 23-May-08 00:39 static/components-bulma/grid/grid.html
+-rw-r--r--  3.0 unx     7257 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.js
+-rw-r--r--  3.0 unx       43 tx stor 23-May-08 00:39 static/components-bulma/vueform/vueform.css
+-rw-r--r--  3.0 unx    70115 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.min.js
+-rw-r--r--  3.0 unx   257636 tx defN 23-May-08 00:39 static/components-bulma/vueform/luxon.js
+-rw-r--r--  3.0 unx     3400 tx defN 23-May-08 00:39 static/components-bulma/vueform/vueform.html
+-rw-r--r--  3.0 unx        0 bx stor 23-May-08 00:39 static/components-bulma/starrater/starrater.css
+-rw-r--r--  3.0 unx      308 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.html
+-rw-r--r--  3.0 unx     1687 tx defN 23-May-08 00:39 static/components-bulma/starrater/starrater.js
+-rw-r--r--  3.0 unx     7447 tx defN 23-May-08 00:39 static/components-bulma/mtable.html
+-rw-r--r--  3.0 unx       83 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.html
+-rw-r--r--  3.0 unx       35 tx stor 23-May-08 00:39 static/components-bulma/fileupload/fileupload.css
+-rw-r--r--  3.0 unx     1232 tx defN 23-May-08 00:39 static/components-bulma/fileupload/fileupload.js
+-rw-r--r--  3.0 unx       12 tx stor 23-May-08 00:39 static/hello.txt
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/ws/README.md
+-rw-r--r--  3.0 unx        1 tx stor 23-May-08 00:39 static/socketio/README.md
+-rw-r--r--  3.0 unx      236 tx defN 23-May-08 00:39 translations/it.json
+-rw-r--r--  3.0 unx      196 tx defN 23-May-08 00:39 translations/en.json
+-rw-r--r--  3.0 unx     4146 tx defN 23-May-08 00:39 __init__.py
+-rw-r--r--  3.0 unx    10333 tx defN 23-May-08 00:39 vue_components_examples/components/vueform.py
+-rw-r--r--  3.0 unx     2078 tx defN 23-May-08 00:39 vue_components_examples/components/starrater.py
+-rw-r--r--  3.0 unx     1597 tx defN 23-May-08 00:39 vue_components_examples/components/fileupload.py
+-rw-r--r--  3.0 unx     7777 tx defN 23-May-08 00:39 vue_components_examples/components/grid.py
+-rw-r--r--  3.0 unx     7858 tx defN 23-May-08 00:39 vue_components_examples/components/README.md
+-rw-r--r--  3.0 unx     1390 tx defN 23-May-08 00:39 vue_components_examples/models.py
+-rw-r--r--  3.0 unx     1215 tx defN 23-May-08 00:39 vue_components_examples/vue_star_rater.py
+-rw-r--r--  3.0 unx      853 tx defN 23-May-08 00:39 vue_components_examples/vue_insert_form.py
+-rw-r--r--  3.0 unx     1149 tx defN 23-May-08 00:39 vue_components_examples/vue_view_form.py
+-rw-r--r--  3.0 unx      324 tx defN 23-May-08 00:39 vue_components_examples/vue_file_uploader.py
+-rw-r--r--  3.0 unx     3031 tx defN 23-May-08 00:39 vue_components_examples/vue_grid_and_forms.py
+-rw-r--r--  3.0 unx       34 tx stor 23-May-08 00:39 vue_components_examples/settings.py
+-rw-r--r--  3.0 unx      302 tx defN 23-May-08 00:39 vue_components_examples/vue_grid.py
+-rw-r--r--  3.0 unx       32 tx stor 23-May-08 00:39 vue_components_examples/common.py
+-rw-r--r--  3.0 unx     1124 tx defN 23-May-08 00:39 vue_components_examples/vue_edit_form.py
+-rw-r--r--  3.0 unx       20 tx stor 23-May-08 00:39 uploads/README.md
+-rw-r--r--  3.0 unx      430 tx defN 23-May-08 00:39 templates/show.html
+-rw-r--r--  3.0 unx      278 tx defN 23-May-08 00:39 templates/auth.html
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/component_loader.html
+-rw-r--r--  3.0 unx       82 tx defN 23-May-08 00:39 templates/examples/page_with_template.html
+-rw-r--r--  3.0 unx      869 tx defN 23-May-08 00:39 templates/examples/custom_form.html
+-rw-r--r--  3.0 unx      143 tx defN 23-May-08 00:39 templates/examples/html_grid.html
+-rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/flash_example.html
+-rw-r--r--  3.0 unx     1025 tx defN 23-May-08 00:39 templates/examples/rest_info.html
+-rw-r--r--  3.0 unx      551 tx defN 23-May-08 00:39 templates/examples/auth_custom_login.html
+-rw-r--r--  3.0 unx      242 tx defN 23-May-08 00:39 templates/examples/forms.html
+-rw-r--r--  3.0 unx       69 tx defN 23-May-08 00:39 templates/examples/ajax_grid.html
+-rw-r--r--  3.0 unx     1711 tx defN 23-May-08 00:39 templates/examples/tagsinput_form.html
+-rw-r--r--  3.0 unx       26 tx stor 23-May-08 00:39 templates/examples/flash_example_next.html
+-rw-r--r--  3.0 unx      189 tx defN 23-May-08 00:39 templates/examples/hcaptcha_form.html
+-rw-r--r--  3.0 unx      193 tx defN 23-May-08 00:39 templates/examples/auth_form.html
+-rw-r--r--  3.0 unx      305 tx defN 23-May-08 00:39 templates/examples/form.html
+-rw-r--r--  3.0 unx      263 tx defN 23-May-08 00:39 templates/examples/session_counter.html
+-rw-r--r--  3.0 unx      646 tx defN 23-May-08 00:39 templates/examples/auth_forms.html
+-rw-r--r--  3.0 unx      228 tx defN 23-May-08 00:39 templates/examples/generic.html
+-rw-r--r--  3.0 unx     2156 tx defN 23-May-08 00:39 templates/layout_bulma.html
+-rw-r--r--  3.0 unx     2172 tx defN 23-May-08 00:39 templates/ws/ws_index.html
+-rw-r--r--  3.0 unx      502 tx defN 23-May-08 00:39 templates/vue/star_rater_vue.html
+-rw-r--r--  3.0 unx      488 tx defN 23-May-08 00:39 templates/vue/insert_form.html
+-rw-r--r--  3.0 unx      374 tx defN 23-May-08 00:39 templates/vue/vuegrid.html
+-rw-r--r--  3.0 unx      544 tx defN 23-May-08 00:39 templates/vue/star_rater_vue_bulma.html
+-rw-r--r--  3.0 unx      392 tx defN 23-May-08 00:39 templates/vue/vuegrid_bulma.html
+-rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/edit_form.html
+-rw-r--r--  3.0 unx      683 tx defN 23-May-08 00:39 templates/vue/vue_grid_and_forms.html
+-rw-r--r--  3.0 unx      372 tx defN 23-May-08 00:39 templates/vue/file_uploader.html
+-rw-r--r--  3.0 unx      486 tx defN 23-May-08 00:39 templates/vue/view_form.html
+-rw-r--r--  3.0 unx      448 tx defN 23-May-08 00:39 templates/vue/starrating.html
+-rw-r--r--  3.0 unx     6788 tx defN 23-May-08 00:39 templates/index.html
+-rw-r--r--  3.0 unx     1913 tx defN 23-May-08 00:39 templates/socketio/socketio_index.html
+-rw-r--r--  3.0 unx     2778 tx defN 23-May-08 00:39 templates/layout.html
 143 files, 9330085 bytes uncompressed, 1358309 bytes compressed:  85.4%
```

#### zipnote {}

```diff
@@ -1,430 +1,430 @@
-Filename: examples/session_counter.py
+Filename: examples/page_with_redirect.py
 Comment: 
 
-Filename: examples/custom_form.py
+Filename: examples/session_clear.py
 Comment: 
 
-Filename: examples/hcaptcha_form.py
+Filename: examples/page_with_parameters.py
 Comment: 
 
-Filename: examples/page_with_query.py
+Filename: examples/models.py
 Comment: 
 
-Filename: examples/hello_world.py
+Filename: examples/hcaptcha_form.py
 Comment: 
 
-Filename: examples/example_multiple_forms.py
+Filename: examples/socketio.py
 Comment: 
 
-Filename: examples/page_with_redirect.py
+Filename: examples/show_a_button.py
 Comment: 
 
-Filename: examples/page_without_template.py
+Filename: examples/flash_example_naive.py
 Comment: 
 
-Filename: examples/page_with_postback.py
+Filename: examples/flash_example_fixture.py
 Comment: 
 
-Filename: examples/hello.py
+Filename: examples/test_expose.py
 Comment: 
 
-Filename: examples/component_loader.py
+Filename: examples/rest.py
 Comment: 
 
-Filename: examples/page_with_raise.py
+Filename: examples/example_html_grid.py
 Comment: 
 
-Filename: examples/common.py
+Filename: examples/count.py
 Comment: 
 
-Filename: examples/flash_example_fixture.py
+Filename: examples/page_with_template.py
 Comment: 
 
-Filename: examples/example_ajax_grid.py
+Filename: examples/custom_form.py
 Comment: 
 
-Filename: examples/socketio.py
+Filename: examples/example_multiple_forms.py
 Comment: 
 
-Filename: examples/page_with_error.py
+Filename: examples/create_form.py
 Comment: 
 
-Filename: examples/page_with_parameters.py
+Filename: examples/rpc.py
 Comment: 
 
-Filename: examples/hello_world_msg.py
+Filename: examples/example_ajax_grid.py
 Comment: 
 
-Filename: examples/example_html_grid.py
+Filename: examples/auth_forms.py
 Comment: 
 
-Filename: examples/example_helpers.py
+Filename: examples/update_form.py
 Comment: 
 
-Filename: examples/auth_form.py
+Filename: examples/session_counter.py
 Comment: 
 
-Filename: examples/auth_forms.py
+Filename: examples/tagsinput_form.py
 Comment: 
 
-Filename: examples/settings.py
+Filename: examples/component_loader.py
 Comment: 
 
-Filename: examples/ws.py
+Filename: examples/auth_form.py
 Comment: 
 
-Filename: examples/count.py
+Filename: examples/page_with_query.py
 Comment: 
 
-Filename: examples/page_with_template.py
+Filename: examples/page_with_postback.py
 Comment: 
 
-Filename: examples/rpc.py
+Filename: examples/ws.py
 Comment: 
 
-Filename: examples/session_clear.py
+Filename: examples/page_with_error.py
 Comment: 
 
-Filename: examples/tagsinput_form.py
+Filename: examples/settings.py
 Comment: 
 
-Filename: examples/flash_example_naive.py
+Filename: examples/hello_world_msg.py
 Comment: 
 
-Filename: examples/update_form.py
+Filename: examples/page_without_template.py
 Comment: 
 
-Filename: examples/models.py
+Filename: examples/ws_client_example.py
 Comment: 
 
-Filename: examples/test_expose.py
+Filename: examples/page_with_raise.py
 Comment: 
 
-Filename: examples/rest.py
+Filename: examples/example_helpers.py
 Comment: 
 
-Filename: examples/create_form.py
+Filename: examples/hello.py
 Comment: 
 
-Filename: examples/ws_client_example.py
+Filename: examples/common.py
 Comment: 
 
-Filename: examples/show_a_button.py
+Filename: examples/hello_world.py
 Comment: 
 
-Filename: static/hello.txt
+Filename: static/components/mtable.js
 Comment: 
 
-Filename: static/ws/README.md
+Filename: static/components/grid/grid.css
 Comment: 
 
 Filename: static/components/grid/grid.js
 Comment: 
 
 Filename: static/components/grid/grid.html
 Comment: 
 
-Filename: static/components/grid/grid.css
+Filename: static/components/vueform/vueform.js
 Comment: 
 
 Filename: static/components/vueform/vueform.css
 Comment: 
 
-Filename: static/components/vueform/luxon.js
+Filename: static/components/vueform/luxon.min.js
 Comment: 
 
-Filename: static/components/vueform/luxon.min.js
+Filename: static/components/vueform/luxon.js
 Comment: 
 
 Filename: static/components/vueform/vueform.html
 Comment: 
 
-Filename: static/components/vueform/vueform.js
+Filename: static/components/starrater/starrater.css
 Comment: 
 
-Filename: static/components/fileupload/fileupload.html
+Filename: static/components/starrater/starrater.html
 Comment: 
 
-Filename: static/components/fileupload/fileupload.js
+Filename: static/components/starrater/starrater.js
 Comment: 
 
-Filename: static/components/fileupload/fileupload.css
+Filename: static/components/mtable.html
 Comment: 
 
-Filename: static/components/mtable.js
+Filename: static/components/fileupload/fileupload.html
 Comment: 
 
-Filename: static/components/starrater/starrater.html
+Filename: static/components/fileupload/fileupload.css
 Comment: 
 
-Filename: static/components/starrater/starrater.js
+Filename: static/components/fileupload/fileupload.js
 Comment: 
 
-Filename: static/components/starrater/starrater.css
+Filename: static/js/prism.js
 Comment: 
 
-Filename: static/components/mtable.html
+Filename: static/js/star_rater_vue.js
 Comment: 
 
-Filename: static/firebase-push.html
+Filename: static/js/firebase-push.js
 Comment: 
 
-Filename: static/socketio/README.md
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/error.html
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: static/css/prism.css
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: static/css/no.css
+Filename: static/js/axios.min.js
 Comment: 
 
-Filename: static/js/star_rater_vue.js
+Filename: static/js/vue.js
 Comment: 
 
-Filename: static/js/firebase-push.js
+Filename: static/js/utils.min.js
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/error.html
 Comment: 
 
-Filename: static/js/utils.min.js
+Filename: static/data/zip_codes.json
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/data/uscities.json
 Comment: 
 
-Filename: static/js/axios.min.js
+Filename: static/favicon.ico
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/firebase-push.html
 Comment: 
 
-Filename: static/js/prism.js
+Filename: static/css/prism.css
 Comment: 
 
-Filename: static/js/vue.js
+Filename: static/css/no.css
 Comment: 
 
-Filename: static/favicon.ico
+Filename: static/components-bulma/mtable.js
 Comment: 
 
-Filename: static/components-bulma/grid/grid.js
+Filename: static/components-bulma/grid/grid.css
 Comment: 
 
-Filename: static/components-bulma/grid/grid.html
+Filename: static/components-bulma/grid/luxon.js
 Comment: 
 
-Filename: static/components-bulma/grid/luxon.js
+Filename: static/components-bulma/grid/grid.js
 Comment: 
 
-Filename: static/components-bulma/grid/grid.css
+Filename: static/components-bulma/grid/grid.html
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.css
+Filename: static/components-bulma/vueform/vueform.js
 Comment: 
 
-Filename: static/components-bulma/vueform/luxon.js
+Filename: static/components-bulma/vueform/vueform.css
 Comment: 
 
 Filename: static/components-bulma/vueform/luxon.min.js
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.html
+Filename: static/components-bulma/vueform/luxon.js
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.js
+Filename: static/components-bulma/vueform/vueform.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.html
+Filename: static/components-bulma/starrater/starrater.css
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.js
+Filename: static/components-bulma/starrater/starrater.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.css
+Filename: static/components-bulma/starrater/starrater.js
 Comment: 
 
-Filename: static/components-bulma/mtable.js
+Filename: static/components-bulma/mtable.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.html
+Filename: static/components-bulma/fileupload/fileupload.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.js
+Filename: static/components-bulma/fileupload/fileupload.css
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.css
+Filename: static/components-bulma/fileupload/fileupload.js
 Comment: 
 
-Filename: static/components-bulma/mtable.html
+Filename: static/hello.txt
 Comment: 
 
-Filename: static/data/uscities.json
+Filename: static/ws/README.md
 Comment: 
 
-Filename: static/data/zip_codes.json
+Filename: static/socketio/README.md
 Comment: 
 
-Filename: __init__.py
+Filename: translations/it.json
 Comment: 
 
-Filename: uploads/README.md
+Filename: translations/en.json
 Comment: 
 
-Filename: templates/index.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/ws/ws_index.html
+Filename: vue_components_examples/components/vueform.py
 Comment: 
 
-Filename: templates/examples/session_counter.html
+Filename: vue_components_examples/components/starrater.py
 Comment: 
 
-Filename: templates/examples/flash_example.html
+Filename: vue_components_examples/components/fileupload.py
 Comment: 
 
-Filename: templates/examples/tagsinput_form.html
+Filename: vue_components_examples/components/grid.py
 Comment: 
 
-Filename: templates/examples/flash_example_next.html
+Filename: vue_components_examples/components/README.md
 Comment: 
 
-Filename: templates/examples/forms.html
+Filename: vue_components_examples/models.py
 Comment: 
 
-Filename: templates/examples/auth_form.html
+Filename: vue_components_examples/vue_star_rater.py
 Comment: 
 
-Filename: templates/examples/custom_form.html
+Filename: vue_components_examples/vue_insert_form.py
 Comment: 
 
-Filename: templates/examples/form.html
+Filename: vue_components_examples/vue_view_form.py
 Comment: 
 
-Filename: templates/examples/component_loader.html
+Filename: vue_components_examples/vue_file_uploader.py
 Comment: 
 
-Filename: templates/examples/auth_forms.html
+Filename: vue_components_examples/vue_grid_and_forms.py
 Comment: 
 
-Filename: templates/examples/html_grid.html
+Filename: vue_components_examples/settings.py
 Comment: 
 
-Filename: templates/examples/generic.html
+Filename: vue_components_examples/vue_grid.py
 Comment: 
 
-Filename: templates/examples/page_with_template.html
+Filename: vue_components_examples/common.py
 Comment: 
 
-Filename: templates/examples/auth_custom_login.html
+Filename: vue_components_examples/vue_edit_form.py
 Comment: 
 
-Filename: templates/examples/rest_info.html
+Filename: uploads/README.md
 Comment: 
 
-Filename: templates/examples/hcaptcha_form.html
+Filename: templates/show.html
 Comment: 
 
-Filename: templates/examples/ajax_grid.html
+Filename: templates/auth.html
 Comment: 
 
-Filename: templates/socketio/socketio_index.html
+Filename: templates/examples/component_loader.html
 Comment: 
 
-Filename: templates/vue/star_rater_vue.html
+Filename: templates/examples/page_with_template.html
 Comment: 
 
-Filename: templates/vue/starrating.html
+Filename: templates/examples/custom_form.html
 Comment: 
 
-Filename: templates/vue/edit_form.html
+Filename: templates/examples/html_grid.html
 Comment: 
 
-Filename: templates/vue/file_uploader.html
+Filename: templates/examples/flash_example.html
 Comment: 
 
-Filename: templates/vue/star_rater_vue_bulma.html
+Filename: templates/examples/rest_info.html
 Comment: 
 
-Filename: templates/vue/insert_form.html
+Filename: templates/examples/auth_custom_login.html
 Comment: 
 
-Filename: templates/vue/vue_grid_and_forms.html
+Filename: templates/examples/forms.html
 Comment: 
 
-Filename: templates/vue/vuegrid_bulma.html
+Filename: templates/examples/ajax_grid.html
 Comment: 
 
-Filename: templates/vue/view_form.html
+Filename: templates/examples/tagsinput_form.html
 Comment: 
 
-Filename: templates/vue/vuegrid.html
+Filename: templates/examples/flash_example_next.html
 Comment: 
 
-Filename: templates/layout.html
+Filename: templates/examples/hcaptcha_form.html
 Comment: 
 
-Filename: templates/auth.html
+Filename: templates/examples/auth_form.html
 Comment: 
 
-Filename: templates/layout_bulma.html
+Filename: templates/examples/form.html
 Comment: 
 
-Filename: templates/show.html
+Filename: templates/examples/session_counter.html
 Comment: 
 
-Filename: translations/it.json
+Filename: templates/examples/auth_forms.html
 Comment: 
 
-Filename: translations/en.json
+Filename: templates/examples/generic.html
 Comment: 
 
-Filename: vue_components_examples/vue_grid_and_forms.py
+Filename: templates/layout_bulma.html
 Comment: 
 
-Filename: vue_components_examples/components/fileupload.py
+Filename: templates/ws/ws_index.html
 Comment: 
 
-Filename: vue_components_examples/components/vueform.py
+Filename: templates/vue/star_rater_vue.html
 Comment: 
 
-Filename: vue_components_examples/components/grid.py
+Filename: templates/vue/insert_form.html
 Comment: 
 
-Filename: vue_components_examples/components/README.md
+Filename: templates/vue/vuegrid.html
 Comment: 
 
-Filename: vue_components_examples/components/starrater.py
+Filename: templates/vue/star_rater_vue_bulma.html
 Comment: 
 
-Filename: vue_components_examples/vue_file_uploader.py
+Filename: templates/vue/vuegrid_bulma.html
 Comment: 
 
-Filename: vue_components_examples/vue_star_rater.py
+Filename: templates/vue/edit_form.html
 Comment: 
 
-Filename: vue_components_examples/common.py
+Filename: templates/vue/vue_grid_and_forms.html
 Comment: 
 
-Filename: vue_components_examples/vue_edit_form.py
+Filename: templates/vue/file_uploader.html
 Comment: 
 
-Filename: vue_components_examples/vue_insert_form.py
+Filename: templates/vue/view_form.html
 Comment: 
 
-Filename: vue_components_examples/vue_view_form.py
+Filename: templates/vue/starrating.html
 Comment: 
 
-Filename: vue_components_examples/settings.py
+Filename: templates/index.html
 Comment: 
 
-Filename: vue_components_examples/models.py
+Filename: templates/socketio/socketio_index.html
 Comment: 
 
-Filename: vue_components_examples/vue_grid.py
+Filename: templates/layout.html
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230521.2/py4web/core.py` & `py4web-1.20230528.1/py4web/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,38 +462,38 @@
     def on_success(self, context):
         # if we redirect and have a flash message we move it to the session
         status = context["status"]
         if status == 303 and self.local.flash:
             response.set_cookie("py4web-flash", json.dumps(self.local.flash), path="/")
         else:
             response.delete_cookie("py4web-flash", path="/")
-        context["output"] = self.transform(context["output"])
+        # if we have a valid flash message, we store it for the template to use later
+        output = context["output"]
+        flash = self.local.flash or ""
+        if isinstance(output, dict):
+            if "template_inject" in context:
+                context["template_inject"]["flash"] = flash
+            else:
+                context["template_inject"] = dict(flash=flash)
+        else:
+            if self.local.flash is not None:
+                response.headers["component-flash"] = json.dumps(flash)
+        self.local.flash = None
         self.local.__dict__.clear()
 
     def on_error(self, context):
         """Clears the local to prevent leakage."""
         self.local.__dict__.clear()
 
     def set(self, message, _class="", sanitize=True):
         # we set a flash message
         if sanitize:
             message = yatl.sanitizer.xmlescape(message)
         self.local.flash = {"message": message, "class": _class}
 
-    def transform(self, data):
-        # if we have a valid flash message, we inject it in the response dict
-        if isinstance(data, dict):
-            if "flash" not in data:
-                data["flash"] = self.local.flash or ""
-        else:
-            if self.local.flash is not None:
-                response.headers["component-flash"] = json.dumps(self.local.flash)
-        self.local.flash = None
-        return data
-
 
 #########################################################################################
 # The Template Rendered Fixture
 #########################################################################################
 
 
 class RenoirXMLEscapeMixin:
@@ -551,14 +551,15 @@
         self.path = path
         self.delimiters = delimiters
 
     def on_success(self, context):
         output = context["output"]
         if not isinstance(output, dict):
             return output
+
         ctx = dict(request=request)
         ctx.update(HELPERS)
         ctx.update(URL=URL)
         ctx.update(context.get("template_inject", {}))
         ctx.update(output)
         ctx["__vars__"] = output
         app_folder = os.path.join(os.environ["PY4WEB_APPS_FOLDER"], request.app_name)
@@ -931,15 +932,15 @@
         """Catches and logs errors in an action; also sets request.app_name"""
 
         @functools.wraps(func)
         def wrapper(*func_args, **func_kwargs):
             try:
                 request.app_name = app_name
                 ret = func(*func_args, **func_kwargs)
-                if isinstance(ret, dict):
+                if isinstance(ret, (list, dict)):
                     response.headers["Content-Type"] = "application/json"
                     ret = dumps(ret)
                 return ret
             except HTTP as http:
                 response.status = http.status
                 response.headers.update(http.headers)
                 return http.body
```

### Comparing `py4web-1.20230521.2/py4web/server_adapters.py` & `py4web-1.20230528.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth.py` & `py4web-1.20230528.1/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230528.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/cors.py` & `py4web-1.20230528.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/dbstore.py` & `py4web-1.20230528.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/downloader.py` & `py4web-1.20230528.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/factories.py` & `py4web-1.20230528.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/form.py` & `py4web-1.20230528.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/grid.py` & `py4web-1.20230528.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/jsonrpc.py` & `py4web-1.20230528.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/mailer.py` & `py4web-1.20230528.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/misc.py` & `py4web-1.20230528.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/populate.py` & `py4web-1.20230528.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/publisher.py` & `py4web-1.20230528.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/recaptcha.py` & `py4web-1.20230528.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/security.py` & `py4web-1.20230528.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web/utils/url_signer.py` & `py4web-1.20230528.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/py4web.egg-info/PKG-INFO` & `py4web-1.20230528.1/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20230521.2
+Version: 1.20230528.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20230521.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20230528.1/py4web.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 README.rst
 pyproject.toml
+requirements.txt
 py4web/__init__.py
 py4web/core.py
 py4web/server_adapters.py
 py4web.egg-info/PKG-INFO
 py4web.egg-info/SOURCES.txt
 py4web.egg-info/dependency_links.txt
 py4web.egg-info/entry_points.txt
```

### Comparing `py4web-1.20230521.2/tests/test_action.py` & `py4web-1.20230528.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_auth.py` & `py4web-1.20230528.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_cache.py` & `py4web-1.20230528.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_fixture.py` & `py4web-1.20230528.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_form.py` & `py4web-1.20230528.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_get_error_snapshot.py` & `py4web-1.20230528.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_json.py` & `py4web-1.20230528.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_main.py` & `py4web-1.20230528.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_session.py` & `py4web-1.20230528.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230521.2/tests/test_tags.py` & `py4web-1.20230528.1/tests/test_tags.py`

 * *Files identical despite different names*

