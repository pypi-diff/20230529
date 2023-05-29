# Comparing `tmp/tr0nz0d-0.1.5.tar.gz` & `tmp/tr0nz0d-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tr0nz0d-0.1.5.tar", last modified: Mon Mar 13 01:38:55 2023, max compression
+gzip compressed data, was "tr0nz0d-0.1.6.tar", last modified: Mon May 29 02:00:36 2023, max compression
```

## Comparing `tr0nz0d-0.1.5.tar` & `tr0nz0d-0.1.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.752905 tr0nz0d-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.752905 tr0nz0d-0.1.5/src/tr0nz0d/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.752905 tr0nz0d-0.1.5/src/tr0nz0d/discord_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/discord_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/discord_tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.752905 tr0nz0d-0.1.5/src/tr0nz0d/django_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/django_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/django_tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/src/tr0nz0d/security/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/security/criptografia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/security/pswd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/src/tr0nz0d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/manual_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_discord_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_django_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    95770 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_math_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_random_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_security_criptografia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_security_pswd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_cnpj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_cpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.756905 tr0nz0d-0.1.5/src/tr0nz0d/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/cnpj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/cpf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    94086 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/math_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/random_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-03-13 01:38:27.000000 tr0nz0d-0.1.5/src/tr0nz0d/tools/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 01:38:55.752905 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-13 01:38:55.000000 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-13 01:38:55.000000 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 01:38:55.000000 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 01:38:55.000000 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 01:38:55.000000 tr0nz0d-0.1.5/src/tr0nz0d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.182377 tr0nz0d-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-29 02:00:36.182377 tr0nz0d-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 02:00:36.182377 tr0nz0d-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.174377 tr0nz0d-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.178377 tr0nz0d-0.1.6/src/tr0nz0d/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.178377 tr0nz0d-0.1.6/src/tr0nz0d/discord_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/discord_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/discord_tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.178377 tr0nz0d-0.1.6/src/tr0nz0d/django_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/django_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/django_tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.178377 tr0nz0d-0.1.6/src/tr0nz0d/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/security/criptografia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/security/pswd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.182377 tr0nz0d-0.1.6/src/tr0nz0d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/manual_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_discord_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_django_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95770 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_math_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_random_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_security_criptografia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_security_pswd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_cnpj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_cpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.182377 tr0nz0d-0.1.6/src/tr0nz0d/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/cnpj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94086 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/math_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/random_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-29 02:00:02.000000 tr0nz0d-0.1.6/src/tr0nz0d/tools/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:00:36.178377 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-29 02:00:36.000000 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-29 02:00:36.000000 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:00:36.000000 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:00:36.000000 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 02:00:36.000000 tr0nz0d-0.1.6/src/tr0nz0d.egg-info/top_level.txt
```

### Comparing `tr0nz0d-0.1.5/LICENSE` & `tr0nz0d-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/PKG-INFO` & `tr0nz0d-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: tr0nz0d
-Version: 0.1.5
+Version: 0.1.6
 Summary: TR0NZ0D Lib is a library created in python to facilitate the use of some tools.
-Home-page: https://tr0nz0d.com/
 Author: Gabriel Menezes de Antonio
-Author-email: tr0nz0d@tr0nz0d.com
 License: MIT
 Project-URL: Source, https://github.com/TR0NZ0D/TR0NZ0D_Lib
-Project-URL: Project Info, https://tr0nz0d.com/projetos/tr0nz0d-lib-python-library
 Project-URL: Bug Tracker, https://github.com/TR0NZ0D/TR0NZ0D_Lib/issues
-Project-URL: Documentation (PT-BR), https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/
-Project-URL: Change Log (PT-BR), https://tr0nz0d.com/docs/changes/tr0nz0d-lib-python-library/
 Keywords: tronzod,tr0nz0d,TR0NZ0D,TRONZOD,tools
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Topic :: Utilities
@@ -41,15 +37,15 @@
 
 TR0NZ0D Lib é uma biblioteca criada em python para facilitar o uso de algumas ferramentas. O projeto está em versão Beta, melhorias e novas funcionalidades serão adicionadas futuramente.
 
 O idioma principal da biblioteca é português, traduções serão adicionadas no futuro.
 
 ## Documentação
 
-* [Português](https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/)
+Website fora do ar por tempo indeterminado devido a financiamento de hospedagem.
 
 ## Módulos existentes
 
 * Tools
 * Security
 * Discord
 * Django
```

### Comparing `tr0nz0d-0.1.5/README.md` & `tr0nz0d-0.1.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 TR0NZ0D Lib é uma biblioteca criada em python para facilitar o uso de algumas ferramentas. O projeto está em versão Beta, melhorias e novas funcionalidades serão adicionadas futuramente.
 
 O idioma principal da biblioteca é português, traduções serão adicionadas no futuro.
 
 ## Documentação
 
-* [Português](https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/)
+Website fora do ar por tempo indeterminado devido a financiamento de hospedagem.
 
 ## Módulos existentes
 
 * Tools
 * Security
 * Discord
 * Django
```

### Comparing `tr0nz0d-0.1.5/setup.py` & `tr0nz0d-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,23 +37,22 @@
     'cryptography',
     'requests',
     'python-dateutil'
 ]
 
 setup(
     name='tr0nz0d',
-    version="0.1.5",
+    version="0.1.6",
     description="TR0NZ0D Lib is a library created in python to facilitate the use of some tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://tr0nz0d.com/',
     author='Gabriel Menezes de Antonio',
-    author_email='tr0nz0d@tr0nz0d.com',
     classifiers=[
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Environment :: No Input/Output (Daemon)",
         "Intended Audience :: Developers",
         "Natural Language :: Portuguese (Brazilian)",
         "Topic :: Utilities",
@@ -68,13 +67,10 @@
     setup_requires=requirements,
     install_requires=requirements,
     tests_require=["unittest"],
     python_requires='>=3.10',
     license="MIT",
     project_urls={
         "Source": "https://github.com/TR0NZ0D/TR0NZ0D_Lib",
-        "Project Info": "https://tr0nz0d.com/projetos/tr0nz0d-lib-python-library",
-        "Bug Tracker": "https://github.com/TR0NZ0D/TR0NZ0D_Lib/issues",
-        "Documentation (PT-BR)": "https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/",
-        "Change Log (PT-BR)": "https://tr0nz0d.com/docs/changes/tr0nz0d-lib-python-library/"
+        "Bug Tracker": "https://github.com/TR0NZ0D/TR0NZ0D_Lib/issues"
     }
 )
```

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/__init__.py` & `tr0nz0d-0.1.6/src/tr0nz0d/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 # Imports
 import logging
 
 __title__ = 'tr0nz0d'
 __author__ = 'TR0NZ0D'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2021 TR0NZ0D'
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 # Instances
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/discord_tools/tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/discord_tools/tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/django_tools/tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/django_tools/tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/security/criptografia.py` & `tr0nz0d-0.1.6/src/tr0nz0d/security/criptografia.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/security/pswd.py` & `tr0nz0d-0.1.6/src/tr0nz0d/security/pswd.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/manual_testing.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/manual_testing.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_discord_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_discord_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_django_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_django_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_math_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_math_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_random_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_random_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_security_criptografia.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_security_criptografia.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_security_pswd.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_security_pswd.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_cnpj.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_cnpj.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_cpf.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_cpf.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_generics.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_generics.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_logging.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_logging.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tests/test_tools_text.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tests/test_tools_text.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/cnpj.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/cnpj.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/cpf.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/cpf.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/generics.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/generics.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/logging.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/logging.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/math_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/math_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/random_tools.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/random_tools.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d/tools/text.py` & `tr0nz0d-0.1.6/src/tr0nz0d/tools/text.py`

 * *Files identical despite different names*

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d.egg-info/PKG-INFO` & `tr0nz0d-0.1.6/src/tr0nz0d.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: tr0nz0d
-Version: 0.1.5
+Version: 0.1.6
 Summary: TR0NZ0D Lib is a library created in python to facilitate the use of some tools.
-Home-page: https://tr0nz0d.com/
 Author: Gabriel Menezes de Antonio
-Author-email: tr0nz0d@tr0nz0d.com
 License: MIT
 Project-URL: Source, https://github.com/TR0NZ0D/TR0NZ0D_Lib
-Project-URL: Project Info, https://tr0nz0d.com/projetos/tr0nz0d-lib-python-library
 Project-URL: Bug Tracker, https://github.com/TR0NZ0D/TR0NZ0D_Lib/issues
-Project-URL: Documentation (PT-BR), https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/
-Project-URL: Change Log (PT-BR), https://tr0nz0d.com/docs/changes/tr0nz0d-lib-python-library/
 Keywords: tronzod,tr0nz0d,TR0NZ0D,TRONZOD,tools
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Topic :: Utilities
@@ -41,15 +37,15 @@
 
 TR0NZ0D Lib é uma biblioteca criada em python para facilitar o uso de algumas ferramentas. O projeto está em versão Beta, melhorias e novas funcionalidades serão adicionadas futuramente.
 
 O idioma principal da biblioteca é português, traduções serão adicionadas no futuro.
 
 ## Documentação
 
-* [Português](https://tr0nz0d.com/docs/tr0nz0d-lib-python-library/)
+Website fora do ar por tempo indeterminado devido a financiamento de hospedagem.
 
 ## Módulos existentes
 
 * Tools
 * Security
 * Discord
 * Django
```

### Comparing `tr0nz0d-0.1.5/src/tr0nz0d.egg-info/SOURCES.txt` & `tr0nz0d-0.1.6/src/tr0nz0d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

