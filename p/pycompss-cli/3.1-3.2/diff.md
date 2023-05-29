# Comparing `tmp/pycompss-cli-3.1.tar.gz` & `tmp/pycompss-cli-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompss-cli-3.1.tar", last modified: Wed Jan 18 09:30:42 2023, max compression
+gzip compressed data, was "pycompss-cli-3.2.tar", last modified: Mon May 29 08:03:27 2023, max compression
```

## Comparing `pycompss-cli-3.1.tar` & `pycompss-cli-3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.487895 pycompss-cli-3.1/
--rwxrwxrwx   0 root         (0) root         (0)    11406 2023-01-18 09:30:40.000000 pycompss-cli-3.1/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      266 2023-01-18 09:30:40.000000 pycompss-cli-3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4068 2023-01-18 09:30:42.487895 pycompss-cli-3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3147 2023-01-18 09:30:40.000000 pycompss-cli-3.1/README.rst
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-01-18 09:30:40.000000 pycompss-cli-3.1/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/assets/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/assets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    25356 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/assets/enqueue_compss_args.txt
--rwxrwxrwx   0 root         (0) root         (0)    15861 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/assets/runcompss_args.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/cli/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/cli/compss.py
--rwxrwxrwx   0 root         (0) root         (0)      892 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/cli/dislib.py
--rwxrwxrwx   0 root         (0) root         (0)     1403 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/cli/pycompss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/core/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5298 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/actions.py
--rwxrwxrwx   0 root         (0) root         (0)     4102 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/actions_dispatcher.py
--rwxrwxrwx   0 root         (0) root         (0)    15282 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/arguments.py
--rwxrwxrwx   0 root         (0) root         (0)     1723 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/cmd_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/core/docker/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/docker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7887 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/docker/actions.py
--rwxrwxrwx   0 root         (0) root         (0)     2379 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/docker/arguments.py
--rwxrwxrwx   0 root         (0) root         (0)    22144 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/docker/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/core/local/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/local/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11668 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/local/actions.py
--rwxrwxrwx   0 root         (0) root         (0)     1936 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/local/arguments.py
--rwxrwxrwx   0 root         (0) root         (0)     4666 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/local/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli/core/remote/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14791 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/actions.py
--rwxrwxrwx   0 root         (0) root         (0)     8704 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/arguments.py
--rwxrwxrwx   0 root         (0) root         (0)     6057 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.487895 pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12974 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/core.py
--rwxrwxrwx   0 root         (0) root         (0)     5510 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.487895 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2242 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/cancel.py
--rwxrwxrwx   0 root         (0) root         (0)    10277 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/commons.py
--rwxrwxrwx   0 root         (0) root         (0)     2385 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/find.py
--rwxrwxrwx   0 root         (0) root         (0)     3398 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/info.py
--rwxrwxrwx   0 root         (0) root         (0)     1798 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/status.py
--rwxrwxrwx   0 root         (0) root         (0)     5237 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.487895 pycompss-cli-3.1/pycompss_cli/models/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      766 2023-01-18 09:30:40.000000 pycompss-cli-3.1/pycompss_cli/models/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 09:30:42.477895 pycompss-cli-3.1/pycompss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4068 2023-01-18 09:30:41.000000 pycompss-cli-3.1/pycompss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1649 2023-01-18 09:30:42.000000 pycompss-cli-3.1/pycompss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 09:30:41.000000 pycompss-cli-3.1/pycompss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-01-18 09:30:42.000000 pycompss-cli-3.1/pycompss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-18 09:30:42.000000 pycompss-cli-3.1/pycompss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-18 09:30:42.000000 pycompss-cli-3.1/pycompss_cli.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-01-18 09:30:40.000000 pycompss-cli-3.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 09:30:42.487895 pycompss-cli-3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1536 2023-01-18 09:30:40.000000 pycompss-cli-3.1/setup.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.908141 pycompss-cli-3.2/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11406 2023-01-18 08:52:05.000000 pycompss-cli-3.2/LICENSE.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      266 2023-01-18 08:52:05.000000 pycompss-cli-3.2/MANIFEST.in
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4065 2023-05-29 08:03:27.908141 pycompss-cli-3.2/PKG-INFO
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3144 2023-05-29 06:57:27.000000 pycompss-cli-3.2/README.rst
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        4 2023-05-08 14:01:10.000000 pycompss-cli-3.2/VERSION.txt
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.868141 pycompss-cli-3.2/pycompss_cli/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/__init__.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.868141 pycompss-cli-3.2/pycompss_cli/assets/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/assets/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    25356 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/assets/enqueue_compss_args.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15861 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/assets/runcompss_args.txt
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.878141 pycompss-cli-3.2/pycompss_cli/cli/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/cli/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      775 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/cli/compss.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      892 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/cli/dislib.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1364 2023-05-09 09:24:49.000000 pycompss-cli-3.2/pycompss_cli/cli/pycompss.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.878141 pycompss-cli-3.2/pycompss_cli/core/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5231 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4190 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/actions_dispatcher.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    15261 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1723 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/cmd_helpers.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.888141 pycompss-cli-3.2/pycompss_cli/core/docker/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/docker/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     8556 2023-05-29 07:56:57.000000 pycompss-cli-3.2/pycompss_cli/core/docker/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2588 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/docker/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    23038 2023-05-29 08:00:47.000000 pycompss-cli-3.2/pycompss_cli/core/docker/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.888141 pycompss-cli-3.2/pycompss_cli/core/local/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/local/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    11870 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/local/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1936 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/local/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4666 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/local/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.898141 pycompss-cli-3.2/pycompss_cli/core/remote/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    16325 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/remote/actions.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     9152 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/remote/arguments.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     7395 2023-05-29 06:55:20.000000 pycompss-cli-3.2/pycompss_cli/core/remote/cmd.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.898141 pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    13095 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/core.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5510 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/defaults.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.898141 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2242 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/cancel.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)    10277 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/commons.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     2385 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/find.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     3398 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/info.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1798 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/status.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     5276 2023-05-08 14:01:10.000000 pycompss-cli-3.2/pycompss_cli/core/utils.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.908141 pycompss-cli-3.2/pycompss_cli/models/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      645 2023-01-18 08:52:05.000000 pycompss-cli-3.2/pycompss_cli/models/__init__.py
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      767 2023-05-29 06:55:20.000000 pycompss-cli-3.2/pycompss_cli/models/app.py
+drwxr-xr-x   0 ctatu     (1000) ctatu     (1000)        0 2023-05-29 08:03:27.868141 pycompss-cli-3.2/pycompss_cli.egg-info/
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     4065 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1649 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        1 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)      136 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       11 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/requires.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       13 2023-05-29 08:03:27.000000 pycompss-cli-3.2/pycompss_cli.egg-info/top_level.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)        7 2023-01-18 08:52:05.000000 pycompss-cli-3.2/requirements.txt
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)       38 2023-05-29 08:03:27.908141 pycompss-cli-3.2/setup.cfg
+-rw-r--r--   0 ctatu     (1000) ctatu     (1000)     1536 2023-01-18 08:52:05.000000 pycompss-cli-3.2/setup.py
```

### Comparing `pycompss-cli-3.1/LICENSE.txt` & `pycompss-cli-3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/PKG-INFO` & `pycompss-cli-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss-cli
-Version: 3.1
+Version: 3.2
 Summary: PyCOMPSs cli
 Home-page: https://compss.bsc.es
 Author: Workflows and Distributed Computing Group (WDC) - Barcelona Supercomputing Center (BSC)
 Author-email: support-compss@bsc.es
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -115,15 +115,15 @@
          python3 -m pip install docker
 
 
 Usage
 ~~~~~
 
 For detailed instructions and examples of usage please visit official documentation.
-   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_Player/02_Usage.html>`__
+   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_CLI/02_Usage.html>`__
 
 License
 =======
 
 Apache License Version 2.0
```

### Comparing `pycompss-cli-3.1/README.rst` & `pycompss-cli-3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
          python3 -m pip install docker
 
 
 Usage
 ~~~~~
 
 For detailed instructions and examples of usage please visit official documentation.
-   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_Player/02_Usage.html>`__
+   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_CLI/02_Usage.html>`__
 
 License
 =======
 
 Apache License Version 2.0
```

### Comparing `pycompss-cli-3.1/pycompss_cli/__init__.py` & `pycompss-cli-3.2/pycompss_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/assets/__init__.py` & `pycompss-cli-3.2/pycompss_cli/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/assets/enqueue_compss_args.txt` & `pycompss-cli-3.2/pycompss_cli/assets/enqueue_compss_args.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/assets/runcompss_args.txt` & `pycompss-cli-3.2/pycompss_cli/assets/runcompss_args.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/cli/__init__.py` & `pycompss-cli-3.2/pycompss_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/cli/compss.py` & `pycompss-cli-3.2/pycompss_cli/cli/compss.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/cli/dislib.py` & `pycompss-cli-3.2/pycompss_cli/cli/dislib.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/cli/pycompss.py` & `pycompss-cli-3.2/pycompss_cli/cli/pycompss.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,40 +11,39 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-from pycompss_cli.core import utils
 from pycompss_cli.core.arguments import parse_sys_argv
 from pycompss_cli.core.actions_dispatcher import ActionsDispatcher
+import sys
 
 # Globals
-DEBUG = False
 LINE_LENGTH = 79
 LINE = "-" * LINE_LENGTH
 
 
 def main():
     """
     MAIN ENTRY POINT
-    """
+    """        
     
     arguments = parse_sys_argv()
 
-    if utils.is_debug():
+    if arguments.debug:
         print(LINE)
         
         if 'enqueue_args' in arguments:
             del arguments.enqueue_args
         if 'runcompss_args' in arguments:
             del arguments.runcompss_args
         print("Calling pycompss-cli for action: " + arguments.action)
         print()
         print("Arguments: " + str(arguments))
 
-    ActionsDispatcher().run_action(arguments, DEBUG)
+    ActionsDispatcher().run_action(arguments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/actions.py` & `pycompss-cli-3.2/pycompss_cli/core/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             self.env_conf['env_path'] = self.home_path + '/.COMPSs/envs/' + self.env_conf['name']
 
         if 'name' in self.arguments and self.arguments.name == 'unique uuid':
             self.arguments.name = ''.join(str(uuid()).split('-')[:2])
 
     
     def env_add_conf(self, extra_conf):
-        current_env, env_conf_path = utils.get_current_env_conf(return_path=True)
+        current_env, env_conf_path = utils.get_current_env_conf(env_id=self.arguments.name, return_path=True)
         new_conf =  {**current_env, **extra_conf}
         with open(env_conf_path, 'w') as f:
             json.dump(new_conf, f)
 
 
     @abstractmethod
     def init(self):
@@ -72,20 +72,15 @@
 
         with open(env_path + '/env.json', 'w') as env_conf:
             json.dump(vars(self.arguments), env_conf)
         self.env_conf = vars(self.arguments)
 
         if self.arguments.config:
             shutil.copy2(self.arguments.config, env_path)
-
-        for current_file in glob(self.home_path + '/.COMPSs/envs/*/current'):
-            os.remove(current_file)
-
-        open(env_path + '/current', 'a').close()
-
+            
         print('Environment ID:', self.arguments.name)
 
     @abstractmethod
     def exec(self):
         pass
 
     @abstractmethod
@@ -116,14 +111,18 @@
         pass
 
     @abstractmethod
     def gengraph(self):
         pass
 
     @abstractmethod
+    def gentrace(self):
+        pass
+
+    @abstractmethod
     def components(self):
         pass
     
     def environment(self):
         action_name = 'list'
 
         if self.arguments.environment:
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/actions_dispatcher.py` & `pycompss-cli-3.2/pycompss_cli/core/actions_dispatcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,34 +24,36 @@
 import json
 
 class ActionsDispatcher(object):
     def __init__(self) -> None:
         super().__init__()
         self.home_path = str(Path.home())
 
-    def run_action(self, arguments, debug):
+    def run_action(self, arguments):
         self.__ensure_default_env()
 
         if 'env' in arguments and arguments.env:
             env_type = arguments.env
             env_conf = None
         else:
             envs_path = self.home_path + '/.COMPSs/envs'
             if not os.path.isdir(envs_path) or len(list(os.walk(envs_path))) == 1:
                 print("There are no environments created. Try using `pycompss init`")
                 exit(1)
 
             if arguments.action == 'environment':
                 if arguments.environment and arguments.environment.startswith('r'):
                     self.__delete_envs(arguments.env_id, arguments)
+
+            env_id = arguments.env_id if arguments.env_id else None
                 
-            env_conf = utils.get_current_env_conf()
+            env_conf = utils.get_current_env_conf(env_id=env_id)
             env_type = env_conf['env']
 
-        self.__actions_cmd = self.__getactions_cmd(env_type, arguments, debug, env_conf)
+        self.__actions_cmd = self.__getactions_cmd(env_type, arguments, env_conf)
 
         action_name = utils.get_object_method_by_name(self.__actions_cmd, arguments.action)
         action_func = getattr(self.__actions_cmd, action_name)
         action_func()
 
     def __delete_envs(self, envs_ids, arguments):
         for env_id in envs_ids:
@@ -75,15 +77,17 @@
         envs_names = env_dir_tree[0][1]
         env_dir_tree = env_dir_tree[1:]
         for i in range(len(env_dir_tree)):
             if env_name == envs_names[i]:
                 return json.load(open(env_dir_tree[i][0] + '/env.json'))['env']
         return None
 
-    def __getactions_cmd(self, env_type, arguments, debug=False, env_conf=None):
+    def __getactions_cmd(self, env_type, arguments, env_conf=None):
+        debug = arguments.debug
+
         if env_type == "local":
             return LocalActions(arguments, debug, env_conf)
         elif env_type == "docker":
             return DockerActions(arguments, debug, env_conf)
         elif env_type == "remote":
             return RemoteActions(arguments, debug, env_conf)
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/arguments.py` & `pycompss-cli-3.2/pycompss_cli/core/arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     :returns: All arguments as namespace.
     """
     parser = argparse.ArgumentParser(formatter_class=FORMATTER_CLASS)
     parser.add_argument("-d", "--debug",
                         help="Enable debug mode. Overrides log_level",
                         action="store_true")
 
+    parser.add_argument("-eid", "--env_id",
+                             default="",
+                             type=str,
+                             help="Environment ID")
+
     # Parent parser - includes all arguments which are common to all actions
     parent_parser = argparse.ArgumentParser(add_help=False,
                                             formatter_class=FORMATTER_CLASS)
     # Action sub-parser
     subparsers = parser.add_subparsers(dest="action")
     # INIT
     parser_init = subparsers.add_parser("init",
@@ -77,18 +82,14 @@
                                         aliases=["ex"],
                                         help="Execute the given command within the COMPSs\' environment.",  # noqa: E501
                                         parents=[parent_parser],
                                         formatter_class=FORMATTER_CLASS)
     parser_exec.set_defaults(action='exec')
 
     
-    # parser_exec.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")
     parser_exec.add_argument('exec_cmd', 
                             nargs=argparse.REMAINDER,   
                             help="Exec program arguments")
     # RUN
     parser_run = subparsers.add_parser("run",
                                        aliases=["r"],
                                        help="Run the application (with runcompss) within the COMPSs\' environment.",  # noqa: E501
@@ -98,19 +99,15 @@
 
     if utils.check_exit_code('runcompss -h') == 0:
         parser_run.epilog = subprocess.check_output('runcompss -h', shell=True).decode()
     else:
         assets_folder = os.path.dirname(os.path.abspath(__file__)) + '/..'
         with open(assets_folder + '/assets/runcompss_args.txt', 'r', encoding='utf-8') as f:
             parser_run.epilog = f.read()
-
-    # parser_run.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")
+            
 
     parser_run.add_argument("-app", "--app_name",
                              default="",
                              type=str,
                              help="Name of the app where to execute runcompss. Only required for `remote` type environment")
     parser_run.add_argument('rest_args',
                             nargs=argparse.REMAINDER,   
@@ -128,19 +125,14 @@
     parser_job = subparsers.add_parser("job", aliases=["j"], add_help=False,
                                     help="Manage jobs within remote environments.",  # noqa: E501
                                     parents=[remote_parser_job()],
                                     formatter_class=FORMATTER_CLASS)
     parser_job.set_defaults(action='job')
     
 
-    # parser_job.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")
-
     # MONITOR
     parser_monitor = subparsers.add_parser("monitor",
                                            aliases=["m"],
                                            help="Start the monitor within the COMPSs\' environment.",  # noqa: E501
                                            parents=[parent_parser],
                                            formatter_class=FORMATTER_CLASS)
     parser_monitor.set_defaults(action='monitor')
@@ -155,52 +147,65 @@
     parser_jupyter = subparsers.add_parser("jupyter",
                                            aliases=["jpy"],
                                            help="Starts Jupyter within the COMPSs\' environment.",  # noqa: E501
                                            parents=[parent_parser],
                                            formatter_class=FORMATTER_CLASS)
     parser_jupyter.set_defaults(action='jupyter')
     
-    # parser_jupyter.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")
+    
     parser_jupyter.add_argument("-app", "--app_name",
                              default="",
                              type=str,
                              help="Name of the app where the notebook will be deployed. Only required for `remote` type environment")
     parser_jupyter.add_argument('rest_args', 
                             nargs=argparse.REMAINDER,   
                             help="Jupyter arguments")
+
     # GENGRAPH
     parser_gengraph = subparsers.add_parser("gengraph",
-                                            aliases=["g"],
+                                            aliases=["gg"],
                                             help="Converts the given graph into pdf.",  # noqa: E501
                                             parents=[parent_parser],
                                             formatter_class=FORMATTER_CLASS)
     parser_gengraph.set_defaults(action='gengraph')
 
-    # parser_gengraph.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")                                            
     parser_gengraph.add_argument("dot_file",
                                  type=str,
                                  help="Dot file to convert to pdf")
+
+
+    # GENTRACE
+    parser_gentrace = subparsers.add_parser("gentrace",
+                                            aliases=["gt"],
+                                            help="Merges traces from all nodes into a Paraver trace.",  # noqa: E501
+                                            parents=[parent_parser],
+                                            formatter_class=FORMATTER_CLASS)
+    parser_gentrace.set_defaults(action='gentrace')
+
+    parser_gentrace.add_argument("trace_dir",
+                                 type=str,
+                                 help="Directory where the traces are located.")
+
+    parser_gentrace.add_argument("--download_dir",
+                                    type=str,
+                                    help="Directory where the traces will be downloaded.")
+
+    parser_gentrace.add_argument('rest_args', 
+                            nargs=argparse.REMAINDER,
+                            help="compss_gentrace arguments")
+
     # COMPONENTS
     parser_components = subparsers.add_parser("components",
                                               aliases=["c"],
                                               help="Manage infrastructure components.",  # noqa: E501
                                               parents=[parent_parser],
                                               formatter_class=FORMATTER_CLASS)
     parser_components.set_defaults(action='components')
 
-    # parser_components.add_argument("-eid", "--env_id",
-    #                          default="",
-    #                          type=str,
-    #                          help="Environment ID")                                                  
+                                                 
     subparsers_components = parser_components.add_subparsers(dest="components")
     
     subparsers_components.add_parser("list",
                                     aliases=["l"],
                                     help="List COMPSs active components.",  # noqa: E501
                                     formatter_class=FORMATTER_CLASS)        # noqa: E501
     parser_components_add = subparsers_components.add_parser("add",
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/cmd_helpers.py` & `pycompss-cli-3.2/pycompss_cli/core/cmd_helpers.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/docker/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/docker/actions.py` & `pycompss-cli-3.2/pycompss_cli/core/docker/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,20 @@
         :param debug: Debug mode
         :returns: None
         """
 
         if self.arguments.working_dir == 'current directory':
             self.arguments.working_dir = os.getcwd()
 
+        if self.arguments.log_dir == 'current directory':
+            self.arguments.log_dir = os.getcwd()
+
         try:
             self.docker_cmd.docker_deploy_compss(self.arguments.working_dir,
+                                self.arguments.log_dir,
                                 self.arguments.image,
                                 self.arguments.restart,
                                 self.arguments.privileged)
 
             master_ip = self.docker_cmd.docker_exec_in_daemon("hostname -i", return_output=True)
             self.env_add_conf({'master_ip': master_ip})
         except:
@@ -91,35 +95,37 @@
         super().exec()
         """ Run the given command in the COMPSs infrastructure at docker
 
         :param arguments: Command line arguments
         :param debug: Debug mode
         :returns: None
         """
-        if self.debug:
-            print("Running...")
-            print("Parameters:")
-            print("\t- Application: " + self.arguments.application)
-            print("\t- self.Arguments: " + str(self.arguments.argument))
 
         app_args = self.arguments.rest_args
 
         if '--project' not in app_args:
             app_args.insert(0, '--project=/project.xml ')
         if '--resources' not in app_args:
             app_args.insert(0, '--resources=/resources.xml ')
         if '--master_name' not in app_args:
             app_args.insert(0, f"--master_name={self.env_conf['master_ip']} ")
         if '--base_log_dir' not in app_args:
             app_args.insert(0, '--base_log_dir=/home/user ')
 
         command = "runcompss " + ' '.join(app_args)
 
+        if self.debug:
+            print("Running...")
+            print("\t- Docker command: ", command)
+
         self.docker_cmd.docker_exec_in_daemon(command)
 
+        if 'log_dir' in self.env_conf and \
+            self.env_conf['log_dir'] == self.env_conf['working_dir']:
+            return
         self.docker_cmd.docker_exec_in_daemon('cp -a /home/user/.COMPSs/. /root/.COMPSs/')
 
 
     def monitor(self):
         """ Starts or stops the monitor in the COMPSs infrastructure at docker
 
         :param arguments: Command line arguments
@@ -157,16 +163,20 @@
                 break
 
         jupyter_cmd = "jupyter-notebook " + \
                 arguments + " " + \
                 f"--ip={self.env_conf['master_ip']} " + \
                 "--allow-root " + \
                 "--NotebookApp.token="
-        for out_line in self.docker_cmd.docker_exec_in_daemon(jupyter_cmd, return_stream=True):
-            print(out_line.decode().strip().replace(self.env_conf['master_ip'], 'localhost'))
+
+        try:
+            for out_line in self.docker_cmd.docker_exec_in_daemon(jupyter_cmd, return_stream=True):
+                print(out_line.decode().strip().replace(self.env_conf['master_ip'], 'localhost'), flush=True)
+        except KeyboardInterrupt:
+            print('Closing jupyter server...')
 
         if self.docker_cmd.exists():
             self.docker_cmd.docker_exec_in_daemon('pkill jupyter')
 
 
     def gengraph(self):
         """ Converts the given task dependency graph (dot) into pdf
@@ -177,14 +187,23 @@
         :returns: None
         """
         dot_path = self.arguments.dot_file
         
         command = "compss_gengraph " + dot_path
         self.docker_cmd.docker_exec_in_daemon(command)
 
+
+    def gentrace(self):
+        command = f"compss_gentrace {self.arguments.trace_dir} "
+        command += ' '.join(self.arguments.rest_args)
+        self.docker_cmd.docker_exec_in_daemon(command)
+        if self.arguments.download_dir:
+            self.docker_cmd.docker_exec_in_daemon(f'cp {self.arguments.trace_dir}/* {self.arguments.download_dir}/')
+
+
     def app(self):
         print("ERROR: Wrong Environment! Try using a `remote` or `local` environment")
         exit(1)
 
     def components(self):
         """ Lists/add/remove workers in the COMPSs infrastructure at docker
 
@@ -209,15 +228,15 @@
             if self.debug:
                 print("Removing components:" + str(self.arguments.worker))
             self.docker_cmd.docker_components(self.arguments.components,
                             self.arguments.remove,
                             self.arguments.worker)
 
     def env_remove(self, env_id=None):
-        if self.docker_cmd.exists():
+        if self.docker_cmd.exists(self.env_conf['name']):
             self.docker_cmd.docker_exec_in_daemon('rm -rf .COMPSs')
             self.docker_cmd.docker_kill_compss()
         super().env_remove(eid=env_id)
 
     def job(self):
         print("ERROR: Wrong Environment! Try using a `remote` environment")
         exit(1)
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/docker/arguments.py` & `pycompss-cli-3.2/pycompss_cli/core/docker/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,18 @@
                                         help="Initialize COMPSs with docker.",
                                         parents=[parent_parser],
                                         formatter_class=FORMATTER_CLASS)
     parser_init.add_argument("-w", "--working_dir",
                              default='current directory',
                              type=str,
                              help="Working directory")
+    parser_init.add_argument("-log", "--log_dir",
+                             default='current directory',
+                             type=str,
+                             help="Logs directory (.COMPSs)")
     parser_init.add_argument("-i", "--image",
                              default="",
                              type=str,
                              help="Docker image")
     parser_init.add_argument("-nr", "--no_restart",
                              dest="restart",
                              action="store_false",
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/docker/cmd.py` & `pycompss-cli-3.2/pycompss_cli/core/docker/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
+import io
 import json
 import os
 import sys
 import tarfile
 import tempfile
 import shutil
 from uuid import uuid4
@@ -36,36 +37,34 @@
 default_worker_workdir = default_workdir + ".COMPSsWorker"
 default_cfg_file = "cfg"
 default_cfg = default_workdir + default_cfg_file
 default_image_file = "image"
 default_image = default_workdir + default_image_file
 
 
-IMAGE_NAME = "compss/compss:2.10"  # Update when releasing new version
+IMAGE_NAME = "compss/compss:3.1"  # Update when releasing new version
 DOCKER_AVAILABALE = True
 
 try:
     import docker
     from docker.types import Mount
     from docker.errors import DockerException
+    from docker.models.containers import Container
 except ImportError:
     DOCKER_AVAILABALE = False
 
 # ############# #
 # API FUNCTIONS #
 # ############# #
 
 class ErrorContainerNotRunning(Exception):
     pass
 
 class DockerCmd(object):
     def __init__(self, env_id) -> None:
-        global master_name
-        global worker_name
-
         self.env_id = env_id
 
         if not DOCKER_AVAILABALE:
             print('ERROR: Pip package `docker` is required for creating docker environments.')
             exit(1)
         
         super().__init__()
@@ -74,38 +73,39 @@
             docker.APIClient(base_url="unix://var/run/docker.sock")
             self.client = docker.from_env()
         except DockerException:
             print("ERROR: Docker service is not running", file=sys.stderr)
             print("       Please, start docker service and try again", file=sys.stderr)
             exit(1)
 
+        self.master_name = master_name + "-" + self.env_id
+        self.worker_name = worker_name + "-" + self.env_id
         self.__setup_image_name()
-        master_name = master_name + "-" + self.env_id
-        worker_name = worker_name + "-" + self.env_id
 
     def __setup_image_name(self):
         global IMAGE_NAME
         if os.environ.get("DEFAULT_DISLIB_DOCKER_IMAGE") is not None:
             # This environment variable will be defined by the dislib script.
             # It can be overriden by the COMPSS_DOCKER_IMAGE or the -i flag
             # when running init.
             IMAGE_NAME = os.environ["DEFAULT_DISLIB_DOCKER_IMAGE"]
         elif os.environ.get("COMPSS_DOCKER_IMAGE") is not None:
             # If specified in an environment variable, take it
             IMAGE_NAME = os.environ["COMPSS_DOCKER_IMAGE"]
-        elif len(self.client.containers.list(filters={"name": master_name})) > 0:
+        elif len(self.client.containers.list(filters={"name": self.master_name})) > 0:
             # Condition equivalent to: is_running(master_name):
             # But since it is undefined yet, we do it explicitly.
             # If exists in the file (means that has been defined with init)
-            master = self.client.containers.list(filters={"name": master_name})[0]
+            master = self.client.containers.list(filters={"name": self.master_name})[0]
             # Command equivalent to: master = _get_master()
             # But since it is undefined yet, we do it explicitly.
             IMAGE_NAME = master.image.attrs["RepoTags"][0]
 
-    def docker_deploy_compss(self, working_dir,
+    def docker_deploy_compss(self, working_dir: str,
+                            log_dir: str,
                             image: str = "",
                             restart: bool = True,
                             privileged: bool = False) -> None:
         """ Starts the main COMPSs image in Docker.
         It stops any existing one since it can not coexist with itself.
 
         :param working_dir: Given working directory
@@ -116,46 +116,50 @@
         
 
         if image:
             docker_image = image
         else:
             docker_image = IMAGE_NAME
 
-        masters = self.client.containers.list(filters={"name": master_name},
+        masters = self.client.containers.list(filters={"name": self.master_name},
                                         all=True)
 
         assert len(masters) < 2  # never should we run 2 masters
 
-        if restart or self._exists(master_name):
+        if restart or self._exists(self.master_name):
             self.docker_kill_compss(False)
 
-        if not self.is_running(master_name):
-            print("Starting %s container in dir %s" % (master_name, working_dir))
+        if not self.is_running(self.master_name):
+            print("Starting %s container in dir %s" % (self.master_name, working_dir))
             print("If this is your first time running PyCOMPSs it may take a " +
                 "while because it needs to download the docker image. " +
                 "Please be patient.")
             subprocess.run(f'docker pull {docker_image}', shell=True)
-            mounts = self._get_mounts(user_working_dir=working_dir)
+            mounts = self._get_mounts(user_working_dir=working_dir, log_dir=log_dir)
             ports = {"8888/tcp": 8888,  # required for jupyter notebooks
                     "8080/tcp": 8080}  # required for monitor
-            m = self.client.containers.run(image=docker_image, name=master_name,
+            container: Container = self.client.containers.run(image=docker_image, name=self.master_name,
                                     mounts=mounts, detach=True, ports=ports, privileged=privileged)
             self._generate_resources_cfg(ips=["localhost"])
             self._generate_project_cfg(ips=["localhost"])
+
+            container.exec_run(f'mkdir -p {os.path.dirname(working_dir)}')
+            container.exec_run(f'ln -s {default_workdir} {working_dir}')
+
             # don't pass configs because they need to be  overwritten when adding
             # new nodes
             cfg_content = '{"working_dir":"' + working_dir + \
                         '","resources":"","project":""}'
             tmp_path, cfg_file = self._store_temp_cfg(cfg_content)
             self._copy_file(cfg_file, default_cfg)
             shutil.rmtree(tmp_path)
 
     
     def docker_start_compss(self):
-        self.client.containers.get(master_name).start()
+        self.client.containers.get(self.master_name).start()
 
 
     def docker_update_image(self) -> None:
         """ Updates the default docker image.
 
         :returns: None
         """
@@ -181,26 +185,26 @@
             # Clean the cfg file
             try:
                 master = self._get_master()
                 self._remove_cfg(master)
             except ErrorContainerNotRunning:
                 print("WARNING: No master container running.")
 
-        self._stop_by_name(master_name)
-        self._stop_by_name(worker_name)
+        self._stop_by_name(self.master_name)
+        self._stop_by_name(self.worker_name)
 
 
     def docker_exec_in_daemon(self, cmd: str, return_output=False, return_stream=False) -> None:
         """ Execute the given command in the main COMPSs image in Docker.
 
         :param cmd: Command to execute.
         :returns: The execution stdout.
         """
 
-        if not self.is_running(master_name):
+        if not self.is_running(self.master_name):
             self.docker_start_compss()
 
         master = self._get_master()
         _, output = master.exec_run(cmd, workdir=default_workdir, stream=True)
         
         if return_output:
             return list(output)[-1].decode().strip()
@@ -215,15 +219,15 @@
 
     def docker_start_monitoring(self) -> None:
         """ Starts the COMPSs monitoring within the Docker instance.
 
         :returns: The monitoring initialization stdout.
         """
         print("Starting Monitor")
-        if not self.is_running(master_name):
+        if not self.is_running(self.master_name):
             self.start_daemon()
 
         cmd = "/etc/init.d/compss-monitor start"
         master = self._get_master()
         env = {"COMPSS_MONITOR": str(default_workdir) + "/.COMPSs"}
         _, output = master.exec_run(cmd,
                                     environment=env,
@@ -256,16 +260,16 @@
 
         :param option: Option to perform (supported: list, add and remove)
         :param element: Element to add or remove (not needed for list)
         :param value: Amount of elements to add or remove (not needed for list)
         :returns: None
         """
         if option == "list":
-            masters = self.client.containers.list(filters={"name": master_name})
-            workers = self.client.containers.list(filters={"name": worker_name})
+            masters = self.client.containers.list(filters={"name": self.master_name})
+            workers = self.client.containers.list(filters={"name": self.worker_name})
             for c in masters + workers:
                 print(c.name)
         elif option == "add":
             if resource == "worker":
                 if value.isdigit():
                     self._add_workers(int(value))
                 else:
@@ -289,20 +293,22 @@
 
         :param name: Instance name.
         :returns: True if running. False otherwise.
         """
         cs = self.client.containers.list(filters={"name": name})
         return len(cs) > 0
 
-    def exists(self, name: str = master_name) -> bool:
+    def exists(self, name: str = None) -> bool:
         """ Checks if a docker instance exists.
 
         :param name: Instance name.
         :returns: True if exists. False otherwise.
         """
+        if name is None:
+            name = master_name
         cs = self.client.containers.list(all=True, filters={"name": name})
         return len(cs) > 0
 
 
     # ################# #
     # PRIVATE FUNCTIONS #
     # ################# #
@@ -387,35 +393,36 @@
         output = master.put_archive(os.path.dirname(dst), data)
         if not output:
             print("ERROR COPYING " + str(src) +
                 " TO " + src(dst) +
                 " OF MASTER CONTAINER!!!")
 
 
-    def _get_mounts(self, user_working_dir: str) -> list:
+    def _get_mounts(self, user_working_dir: str, log_dir: str) -> list:
         """ Retrieve the list of folders to be mounted. It gets the Mount object
         from the given user working directory, and can include any other needed
         folder.
 
         :param user_working_dir: User working path.
         :returns: List of docker Mount objects.
         """
         # mount target dir needs to be absolute
         target_dir = default_workdir
         user_dir = Mount(target=target_dir,
                         source=user_working_dir,
                         type="bind")
         # WARNING: mounting .COMPSs makes it fail
-        # compss_logs_dir = os.environ["HOME"] + f"/.COMPSs"
-        # os.makedirs(compss_logs_dir, exist_ok=True)
-
-        # compss_log_dir = Mount(target="/root/.COMPSs",
-        #                        source=compss_logs_dir,
-        #                        type="bind")
-        mounts = [user_dir]
+        if '.COMPSs' not in log_dir:
+            log_dir = log_dir + "/.COMPSs"
+        os.makedirs(log_dir, exist_ok=True)
+
+        compss_log_dir = Mount(target="/root/.COMPSs",
+                               source=log_dir,
+                               type="bind")
+        mounts = [user_dir, compss_log_dir]
         return mounts
 
 
     def _generate_project_cfg(self, ips: list = (), cpus: int = 4,
                             install_dir: str = "/opt/COMPSs",
                             worker_dir: str = default_worker_workdir) -> str:
         """ Generates the project.xml according to the given parameters.
@@ -596,7 +603,21 @@
 
         :param name: Name of the instance to be removed.
         :returns: None
         """
         containers = self.client.containers.list(filters={"name": name}, all=True)
         for c in containers:
             c.remove(force=True)
+
+    def docker_copy_to_host(self, container_name, src, dst):
+        """ Copy files from a container directory to a host directory.
+
+        :param container_name: Name of the container.
+        :param src: Source path.
+        :param dst: Destination path.
+        :returns: None
+        """
+        container = self.client.containers.get(container_name)
+        data, stat = container.get_archive(src)
+        with open(dst, 'wb') as f:
+            for chunk in data:
+                f.write(chunk)
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/local/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/local/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/local/actions.py` & `pycompss-cli-3.2/pycompss_cli/core/local/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,28 +79,26 @@
         super().run()
         """ Run the given command in the COMPSs infrastructure at docker
 
         :param arguments: Command line arguments
         :param debug: Debug mode
         :returns: None
         """
-        if self.debug:
-            print("Running...")
-            print("Parameters:")
-            print("\t- Application: " + self.arguments.application)
-            print("\t- Arguments: " + str(self.arguments.argument))
-
         app_args = self.arguments.rest_args
 
         commands = [
             "runcompss " + ' '.join(app_args)
         ]
 
         if 'working_dir' in self.env_conf:
             commands.insert(0, 'cd ' + self.env_conf['working_dir'])
+
+        if self.debug:
+            print("Running...")
+            print("\t- Local command: ", ' '.join(commands))
                 
         local_run_app(commands)
 
     def jupyter(self):
         if utils.check_exit_code('jupyter') == 127:
             print('ERROR: Jupyter not found!')
             exit(1)
@@ -294,14 +292,21 @@
         print('ERROR: Not Implemented Yet')
         exit(1)
 
     def gengraph(self):
         command = "compss_gengraph " + self.arguments.dot_file
         local_exec_app(command)
 
+    def gentrace(self):
+        command = f"compss_gentrace {self.arguments.trace_dir} "
+        command += ' '.join(self.arguments.rest_args)
+        local_exec_app(command)
+        if self.arguments.download_dir:
+            local_exec_app(f'cp {self.arguments.trace_dir}/* {self.arguments.download_dir}/')
+
     def get_apps(self, env_id=None) -> List[App]:
         if self.apps is not None:
             return self.apps
 
         app_dir = os.path.expanduser('~') + f'/.COMPSsApps/'
 
         if not os.path.isdir(app_dir):
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/local/arguments.py` & `pycompss-cli-3.2/pycompss_cli/core/local/arguments.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/local/cmd.py` & `pycompss-cli-3.2/pycompss_cli/core/local/cmd.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/actions.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pycompss_cli.core.remote.cmd import remote_list_job
 from pycompss_cli.core.remote.cmd import remote_cancel_job
 from pycompss_cli.core.remote.cmd import remote_run_app
 from pycompss_cli.core.remote.cmd import remote_exec_app
 from pycompss_cli.core.remote.cmd import remote_list_apps
 from pycompss_cli.core.remote.cmd import remote_get_home
 from pycompss_cli.core.remote.cmd import remote_env_remove
+from pycompss_cli.core.remote.cmd import remote_download_file
 from pycompss_cli.core.actions import Actions
 from pycompss_cli.core import utils
 from pycompss_cli.core.remote.interactive_sc import core, defaults
 import os, json, time, datetime, traceback, re
 from collections import defaultdict
 
 class RemoteActions(Actions):
@@ -65,16 +66,14 @@
         """
         super().init()
 
         if self.arguments.modules is None:
             self.arguments.modules = ['COMPSs']
         elif len(self.arguments.modules) == 1 and os.path.isfile(self.arguments.modules[0]):
             self.arguments.modules = self.arguments.modules[0]
-        # elif 'COMPSs' not in [m[:len('COMPSs')] for m in self.arguments.modules]:
-        #     self.arguments.modules.insert(0, 'COMPSs')
         
         print('Deploying environment...')
 
         env_id = self.arguments.name
         envars = []
         if re.search(r'mn\d\.bsc\.es', self.env_conf['login']) is not None:
             envars.append('COMPSS_PYTHON_VERSION=3.7.4')
@@ -109,15 +108,17 @@
         env_name = self.env_conf['name']
         modules = self.__get_modules()
 
         print(remote_run_app(remote_dir, login_info, env_name, command, modules))
 
     def __get_modules(self):
         with open(self.env_conf['env_path'] + '/modules.sh', 'r') as mod_file:
-            return mod_file.read().strip().split('\n')
+            mods = mod_file.read().strip().split('\n')
+            mods = [re.sub(r'#.*', '', mod).strip() for mod in mods]
+            return mods
 
     def job(self):
         super().job()
 
         action_name = self.arguments.job
         action_name = utils.get_object_method_by_name(self, 'job_' + action_name, include_in_name=True)
         getattr(self, action_name)()
@@ -152,15 +153,15 @@
         app_args = f'--appdir={remote_dir} ' + app_args
 
         modules = self.__get_modules()
         env_vars = [item for sublist in self.arguments.env_var for item in sublist]
         if 'COMPSS_PYTHON_VERSION' not in ''.join(env_vars):
             env_vars = ['COMPSS_PYTHON_VERSION=3.7.4'] + env_vars
         
-        job_id = remote_submit_job(login_info, remote_dir, app_args, modules, envars=env_vars)
+        job_id = remote_submit_job(login_info, remote_dir, app_args, modules, envars=env_vars, debug=self.debug)
 
         self.past_jobs[job_id] = {
             'app_name': app_name,
             'env_vars': '; '.join(env_vars) if env_vars else 'None',
             'enqueue_args': app_args,
             'timestamp': str(datetime.datetime.utcnow())[:-7] + ' UTC'
         }
@@ -204,15 +205,15 @@
         remote_cancel_job(login_info, jobid, modules)
 
     def job_status(self, jid=None):
         login_info = self.env_conf['login']
         job_id = self.arguments.job_id if jid is None else jid
         modules = self.__get_modules()
         scripts_path = self.env_conf['remote_home'] + '/.COMPSs/job_scripts'
-        job_status = core.job_status(scripts_path, job_id, login_info, modules)
+        job_status = core.job_status(scripts_path, job_id, login_info, modules, debug=self.debug)
         if job_status == 'ERROR' and job_id in self.past_jobs:
             app_name = self.past_jobs[job_id]['app_name']
             env_id = self.env_conf['name']
             app_path = self.env_conf['remote_home'] + f'/.COMPSsApps/{env_id}/{app_name}'
             cmd = f'grep -iF "error" {app_path}/compss-{job_id}.err'
             status = 'ERROR' if remote_exec_app(login_info, cmd) else 'SUCCESS'
             job_status = 'COMPLETED:' + status
@@ -241,25 +242,23 @@
             self.arguments.source_dir = os.getcwd()
         else:
             if not os.path.isdir(self.arguments.source_dir):
                 print(f"ERROR: Local source directory {self.arguments.source_dir} does not exist")
                 exit(1)
 
         app_name = self.arguments.app_name
-        if app_name in self.get_apps():
-            print(f'ERROR: There is already another application named `{app_name}`')
+        if app_name in self.get_apps() and not self.arguments.overwrite:
+            print(f'ERROR: There is already another application named `{app_name}`. Use `--overwrite` to overwrite it.')
             exit(1)
 
-        # if self.arguments.destination_dir:
-        #     self.arguments.destination_dir = self.arguments.destination_dir.replace('{COMPSS_REMOTE_HOME}', )
-
         env_id = self.env_conf['name']
         app_dir = self.env_conf['remote_home'] + f'/.COMPSsApps/{env_id}/{app_name}'
 
-        remote_app_deploy(app_dir, self.env_conf['login'], self.arguments.source_dir, self.arguments.destination_dir)
+        remote_app_deploy(app_dir, self.env_conf['login'], self.arguments.source_dir,
+                          self.arguments.destination_dir, self.arguments.env_file)
 
 
     def app_remove(self):
         app_names = self.arguments.app_name
         for app_name in app_names:
             if app_name in self.get_apps():
                 login_info = self.env_conf['login']
@@ -290,28 +289,64 @@
         env_id = self.arguments.env_id if eid is None else eid
         env_apps = self.get_apps(env_id=env_id)
         if len(env_apps) > 0:
             print('WARNING: There are still applications binded to this environment')
             answer = 'y'
             if not self.arguments.force:
                 answer = input('Do you want to delete this environment and all the applications? (y/N) ')
-            if answer == 'Y' or answer == 'y' or answer == 'yes':
+            if answer.lower() == 'y' or answer == 'yes':
                 login_info = self.env_conf['login']
                 remote_env_remove(login_info, env_id, env_apps)
                 super().env_remove(eid=eid)
         else:
             super().env_remove(eid=eid)
 
     def components(self):
         print('ERROR: Not Implemented Yet')
         exit(1)
 
     def gengraph(self):
-        print('ERROR: Not Implemented Yet')
-        exit(1)
+        dot_path = self.arguments.dot_file
+        
+        command = "compss_gengraph " + dot_path
+        remote_exec_app(self.env_conf['login'], command)
+
+    def gentrace(self):
+        modules = self.__get_modules()
+
+        gentrace_cmd = f"compss_gentrace {self.arguments.trace_dir} "
+        gentrace_cmd += ' '.join(self.arguments.rest_args)
+
+        commands = [
+            *modules,
+            gentrace_cmd
+        ]
+
+        command = ';'.join(commands)
+
+        print('Generating trace...')
+        remote_exec_app(self.env_conf['login'], command, self.debug)
+
+        if self.arguments.download_dir:
+            compressed = False
+            size_cmd = f"du -m {self.arguments.trace_dir}/*.prv | cut -f1"
+            trace_size = remote_exec_app(self.env_conf['login'], size_cmd, self.debug)
+            if int(trace_size) > 100:
+                answer = input(f'Trace size is {trace_size}MB. Do you want to compress it before downloading it? (y/N) ')
+                if answer.lower() == 'y' or answer.lower() == 'yes':
+                    compress_cmd = f"cd {self.arguments.trace_dir};zip -r trace.zip *"
+                    print('Compressing trace...')
+                    remote_exec_app(self.env_conf['login'], compress_cmd, self.debug)
+                    compressed = True
+            
+            print('Downloading trace...')
+            remote_download_file(self.env_conf['login'], self.arguments.trace_dir, self.arguments.download_dir, self.debug, compressed)
+
+        
+
 
     def monitor(self):
         print('ERROR: Not Implemented Yet')
         exit(1)
 
     def jupyter(self):
         app_name = self.arguments.app_name
@@ -344,29 +379,29 @@
 
         app_args = ' '.join(app_args)
         modules = self.__get_modules()
         envars = []
         if re.search(r'mn\d\.bsc\.es', self.env_conf['login']) is not None:
             envars.append('COMPSS_PYTHON_VERSION=3.7.4')
 
-        job_id = remote_submit_job(login_info, remote_dir, app_args, modules, envars)
+        job_id = remote_submit_job(login_info, remote_dir, app_args, modules, envars, debug=self.debug)
 
         scripts_path = self.env_conf['remote_home'] + '/.COMPSs/job_scripts'
 
         print('Waiting for jupyter to start...')
         jupyter_job_status = defaults.NOT_RUNNING_KEYWORD
         try:
             while jupyter_job_status != 'RUNNING':
-                jupyter_job_status = core.job_status(scripts_path, job_id, login_info, modules)
+                jupyter_job_status = core.job_status(scripts_path, job_id, login_info, modules, debug=self.debug)
         except:
             print('ERROR while waiting for jupyter to start')
-            core.cancel_job(scripts_path, [job_id], login_info, modules)
+            core.cancel_job(scripts_path, [job_id], login_info, modules, debug=self.debug)
             exit(1)
         else:
             print('Jupyter started')
 
             print('Connecting to jupyter server...')
             time.sleep(5)
 
-            core.connect_job(scripts_path, job_id, login_info, modules, remote_dir, port_forward=port, web_browser=None)
+            core.connect_job(scripts_path, job_id, login_info, modules, remote_dir, port_forward=port, web_browser=None, debug=self.debug)
             
-            core.cancel_job(scripts_path, [job_id], login_info, modules)
+            core.cancel_job(scripts_path, [job_id], login_info, modules, debug=self.debug)
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/arguments.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,14 +66,15 @@
                                         aliases=["a"],
                                         parents=[parent_parser],
                                         formatter_class=FORMATTER_CLASS)
     parser_app.set_defaults(func=lambda: print(parser_app.format_help()))
 
     app_subparsers = parser_app.add_subparsers(dest="app")
 
+    # DEPLOY
     app_deploy_parser = app_subparsers.add_parser("deploy",
                                 aliases=["d"],
                                 help="Deploy an application to a remote environment",
                                 parents=[parent_parser],
                                 formatter_class=FORMATTER_CLASS)
 
     app_deploy_parser.add_argument("app_name",
@@ -85,25 +86,35 @@
                              type=str,
                              help="Directory from which the files will be copied.")
 
     app_deploy_parser.add_argument("-d", "--destination_dir",
                              type=str,
                              help="Remote destination directory to copy the local app files")
 
+    app_deploy_parser.add_argument("--env_file",
+                                type=str,
+                                help="File containing modules or environment variables to be set for this application.")
+
+    app_deploy_parser.add_argument("-o", "--overwrite",
+                                action="store_true",
+                                help="Overwrite the application if it already exists.")
+
+    # REMOVE
     app_remove_parser = app_subparsers.add_parser("remove",
                                 aliases=["r"],
                                 help="Delete one or more deployed applications",
                                 parents=[parent_parser],
                                 formatter_class=FORMATTER_CLASS)
 
     app_remove_parser.add_argument("app_name",
                              type=str,
                              nargs='+',
                              help="Name of the application")
 
+    # LIST
     app_subparsers.add_parser("list",
                                 aliases=["l"],
                                 help="List all deployed applications",
                                 parents=[parent_parser],
                                 formatter_class=FORMATTER_CLASS)
 
     return parser_app
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/cmd.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import os
 from re import sub
 from sys import stdout
 import tempfile
 from shutil import copyfile
 import subprocess
 import tempfile
+import zipfile
 import pycompss_cli.core.utils as utils
 
 # ################ #
 # GLOBAL VARIABLES #
 # ################ #
 
 # ############# #
@@ -60,25 +61,36 @@
         os.unlink(tmp_modules.name)
 
     path = os.path.abspath(__file__)
     local_job_scripts_dir = os.path.dirname(path) + '/job_scripts/'
     subprocess.run(f"scp -r {local_job_scripts_dir} '{login_info}:~/.COMPSs/'", shell=True, stdout=subprocess.PIPE)
     
 
-def remote_app_deploy(app_dir: str, login_info: str, local_source: str, remote_dest_dir: str = None):
+def remote_app_deploy(app_dir: str, login_info: str, local_source: str, remote_dest_dir: str = None, env_file: str = None):
+
+    if env_file:
+        if not os.path.isfile(env_file):
+            print(f'ERROR: env file `{env_file}` not found.')
+            exit(1)
+            
+
     print('Deploying app...')
     utils.ssh_run_commands(login_info, [f'mkdir -p {app_dir}'])
 
     cmd_copy_files = f"scp -r {local_source}/* {login_info}:'{app_dir}/'"
 
     if os.path.isfile(local_source):
         cmd_copy_files = cmd_copy_files.replace('/*', '')
 
     subprocess.run(cmd_copy_files, shell=True)
 
+    if env_file:
+        cmd_copy_files = f"scp {env_file} {login_info}:'{app_dir}/.env'"
+        subprocess.run(cmd_copy_files, shell=True)
+
     if remote_dest_dir:
         print('App deployed to', remote_dest_dir)
         utils.ssh_run_commands(login_info, [
             f'echo {remote_dest_dir} > {app_dir}/.compss',
             f'mkdir -p {os.path.dirname(remote_dest_dir)}',
             f'ln -s {app_dir} {remote_dest_dir}'
         ])
@@ -93,41 +105,42 @@
     commands = [
         f'cd {remote_dir}',
         *modules,
         command
     ]
     return utils.ssh_run_commands(login_info, commands)[0]
 
-def remote_submit_job(login_info: str, remote_dir: str, app_args: str, modules, envars=None) -> None:
+def remote_submit_job(login_info: str, remote_dir: str, app_args: str, modules, envars=None, debug=False) -> None:
     """ Execute the given command in the remote COMPSs environment.
 
     :param cmd: Command to execute.
     :returns: The execution stdout.
     """
 
-    enqueue_debug = '-d' if utils.is_debug() else ''
+    enqueue_debug = '-d' if debug else ''
 
     commands = [
         f'cd {remote_dir}',
         *modules,
+        'if [ -f .env ]; then source .env; fi',
         f'enqueue_compss {enqueue_debug} {app_args}'
     ]
 
     if envars:
         commands = [f'export {var}' for var in envars] + commands
 
-    if utils.is_debug():
+    if debug:
         print('********* DEBUG *********')
         print('Remote submit job commands:')
         for cmd in commands:
             print('\t', '->', cmd)
         print('***************************')
 
     stdout, stderr = utils.ssh_run_commands(login_info, commands)
-    if utils.is_debug():
+    if debug:
         print('Remote submit job stdout:')
         print(stdout.strip())
         print('***************************')
         print('Remote submit job stderr:')
         print(stderr.strip())
         print('***************************')
     job_id = stdout.strip().split('\n')[-1].split(' ')[-1]
@@ -176,9 +189,39 @@
         *modules,
         f'python3 ~/.COMPSs/job_scripts/cancel.py {job_id}',
     ]
 
     stdout = utils.ssh_run_commands(login_info, commands)[0].strip()
     print(stdout)
 
-def remote_exec_app(login_info: str, exec_cmd: str):
+def remote_exec_app(login_info: str, exec_cmd: str, debug=False):
+    if debug:
+        print('Remote exec app command:')
+        print('\t', '->', exec_cmd)
     return utils.ssh_run_commands(login_info, [exec_cmd])[0].strip()
+
+
+def remote_download_file(login_info: str, remote_path: str, local_path: str, debug=False, compressed=False):
+    if not os.path.isdir(local_path):
+        if os.path.exists(local_path):
+            print(f'ERROR: local path `{local_path}` is not a directory.')
+            exit(1)
+        else:
+            os.makedirs(local_path)
+
+    if compressed:
+        cmd = f'scp -r {login_info}:{remote_path}/trace.zip {local_path}'
+    else:
+        cmd = f'scp -r {login_info}:{remote_path}/* {local_path}'
+
+    if debug:
+        print('Remote download file command:')
+        print('\t', cmd)
+
+    subprocess.run(cmd, shell=True)
+
+    if compressed:
+        print('Uncompressing trace...')
+        zip_path = os.path.join(local_path, 'trace.zip')
+        with zipfile.ZipFile(zip_path, 'r') as zip_ref:
+            zip_ref.extractall(local_path)
+        os.remove(zip_path)
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/core.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,60 +130,60 @@
     """
     Display warning in a common format.
     :return: None
     """
     print("WARNING: " + message)
 
 
-def job_status(scripts_path, job_id, login_info, modules):
+def job_status(scripts_path, job_id, login_info, modules, debug=False):
     """
     Checks the status of a job in the supercomputer.
     :param scripts_path: Remote helper scripts path
     :param job_id: Job identifier
     :return: None
     """
     cmd = [INTERPRETER,
            str(scripts_path + '/' + STATUS_SCRIPT),
            job_id]
-    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules)
+    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules, debug=debug)
     if return_code != 0:
         # __display_error(ERROR_STATUS_JOB, return_code, stdout, stderr)
         return 'ERROR'
 
     # Parse the output for fancy printing
     out = stdout.splitlines()
     if out[-2] == SUCCESS_KEYWORD:
         status = out[-1].split(':')[1].strip()
         if not status:
             return 'ERROR'
         return status
     return ERROR_STATUS_JOB
 
-def job_list(scripts_path, login_info, modules):
+def job_list(scripts_path, login_info, modules, debug=False):
     """
     Checks the list of available jobs in the supercomputer.
     :param scripts_path: Remote helper scripts path
     :return: None
     """
     cmd = [INTERPRETER,
            str(scripts_path + '/' + FIND_SCRIPT)]
-    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules)
+    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules, debug=debug)
     if return_code != 0:
         __display_error(ERROR_STATUS_JOB, return_code, stdout, stderr)
 
     # Parse the output for fancy printing
     out = stdout.splitlines()
     if out[0] == SUCCESS_KEYWORD:
         print("Available notebooks: ")
         for job_id in out[1:]:
             print(job_id)
     else:
         __display_error(ERROR_STATUS_JOB, return_code, stdout, stderr)
 
-def connect_job(scripts_path, job_id, login_info, modules, app_path, port_forward='8888', web_browser='firefox'):
+def connect_job(scripts_path, job_id, login_info, modules, app_path, port_forward='8888', web_browser='firefox', debug=False):
     """
     Establish the connection with an existing notebook.
     :param scripts_path: Remote helper scripts path
     :param arguments: Arguments received from command line.
     :return: None
     """
     # First register the signal (the connection will be ready until CTRL+C)
@@ -192,15 +192,15 @@
     # Second, get information about the job (node and token)
     node = None
     token = None
     
     cmd = [INTERPRETER,
            str(scripts_path + '/' + INFO_SCRIPT),
            job_id, app_path]
-    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules)
+    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules, debug=debug)
     if return_code != 0:
         __display_error(ERROR_INFO_JOB, return_code, stdout, stderr)
 
     # Parse the output
     out = stdout.splitlines()
     if NOT_RUNNING_KEYWORD in stdout:
         __display_warning(WARNING_NOTEBOOK_NOT_RUNNING)
@@ -220,34 +220,34 @@
     else:
         __display_error(ERROR_INFO_JOB, return_code, stdout, stderr)
 
     cmd = ['-L', f'{port_forward}:localhost:{port_forward}',
            'ssh', node,
            '-L', f'{port_forward}:localhost:8888']
 
-    if utils.is_debug():
+    if debug:
         print('****** DEBUG ******')
         print("\t -> Connecting to node: " + node)
         print("\t -> Token: " + token)
     
-    _command_runner(cmd, login_info, blocking=False)
+    _command_runner(cmd, login_info, blocking=False, debug=debug)
 
     time.sleep(5)  # Wait 5 seconds
 
     if web_browser is None:
         print(INFO_CONNECTION_ESTABLISHED)
         print(CONNECTION_URL.replace(':8888', f':{port_forward}') + token)
     else:
         print("Opening the " + web_browser + " browser with the connection URL.")
         if is_windows():
             cmd = ['cmd', '/c', 'start', web_browser]
         else:
             cmd = [web_browser]
         cmd = cmd + [CONNECTION_URL + token]
-        return_code, stdout, stderr = _command_runner(cmd, login_info, remote=False)
+        return_code, stdout, stderr = _command_runner(cmd, login_info, remote=False, debug=debug)
         if return_code != 0:
             message = ERROR_BROWSER + '\n\n' \
                       + "Alternatively, please use the following URL to connect to the job.\n" \
                       + CONNECTION_URL + token
             __display_error(message, return_code, stdout, stderr)
         else:
             print(INFO_CONNECTION_ESTABLISHED)
@@ -264,36 +264,36 @@
             except IOError:
                 pass
     else:
         signal.pause()
     # The signal is captured and everything cleaned and canceled (if needed)
 
 
-def cancel_job(scripts_path, job_ids, login_info, modules):
+def cancel_job(scripts_path, job_ids, login_info, modules, debug=False):
     """
     Cancel a list of notebook jobs running in the supercomputer.
     :param scripts_path: Path where the remote helper scripts are
     :param job_ids: List of job identifiers
     :return: None
     """
     cmd = [INTERPRETER,
            str(scripts_path + '/' + CANCEL_SCRIPT)] + job_ids
-    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules)
+    return_code, stdout, stderr = _command_runner(cmd, login_info, modules=modules, debug=debug)
     if return_code != 0:
         __display_error(ERROR_CANCELLING_JOB, return_code, stdout, stderr)
 
     # Parse the output
     out = stdout.splitlines()
     if out[0] == SUCCESS_KEYWORD:
         print("Jobs successfully cancelled.")
     else:
         __display_error(ERROR_CANCELLING_JOB, return_code, stdout, stderr)
 
 
-def _command_runner(cmd, login_info, modules=None, blocking=True, remote=True):
+def _command_runner(cmd, login_info, modules=None, blocking=True, remote=True, debug=False):
     """
     Run the command defined in the cmd list.
     Decodes the stdout and stderr following the DECODING_FORMAT.
     :param cmd: Command to execute as list.
     :param blocking: blocks until the subprocess finishes. Otherwise,
                      does not wait and appends the process to the global
                      alive processes list
@@ -316,15 +316,15 @@
                 cmd = f"ssh {login_info} {cmd}"
             else:
                 cmd = f"ssh {login_info} '{cmd}'"
     else:
         # Execute the command as requested
         pass
 
-    if utils.is_debug():
+    if debug:
         print('****** DEBUG ******')
         print("\t -> Command: " + cmd)
         print('********************')
 
     p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     if blocking:
         stdout, stderr = p.communicate()   # blocks until cmd is done
```

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/interactive_sc/defaults.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/interactive_sc/defaults.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/__init__.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/cancel.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/cancel.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/commons.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/commons.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/find.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/find.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/info.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/info.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/remote/job_scripts/status.py` & `pycompss-cli-3.2/pycompss_cli/core/remote/job_scripts/status.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/core/utils.py` & `pycompss-cli-3.2/pycompss_cli/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 #
 import json
 from glob import glob
 from pathlib import Path
 import subprocess
 import os
 
-def is_debug():
-    return os.getenv('PYCOMPSS_CLI_DEBUG', 'false').lower() == 'true'
 
 def get_object_method_by_name(obj, method_name, include_in_name=False):
     for class_method_name in dir(obj):
         if not '__' in class_method_name and callable(getattr(obj, class_method_name)):
             if class_method_name.startswith(method_name) or (include_in_name and method_name in class_method_name):
                 return class_method_name
 
 def table_print(col_names, data):
     print_table(data, header=col_names)
 
-def get_current_env_conf(return_path=False):
+def get_current_env_conf(env_id=None, return_path=False):
     home_path = str(Path.home())
-    current_env = glob(home_path + '/.COMPSs/envs/*/current')[0].replace('current', 'env.json')
+    if env_id:
+        current_env = glob(home_path + '/.COMPSs/envs/' + env_id + '/env.json')[0]
+    else:
+        current_env = glob(home_path + '/.COMPSs/envs/*/current')[0].replace('current', 'env.json')
     with open(current_env, 'r') as env:
         if return_path:
             return json.load(env), current_env
         return json.load(env)
 
 def get_env_conf_by_name(env_name):
     home_path = str(Path.home())
```

### Comparing `pycompss-cli-3.1/pycompss_cli/models/__init__.py` & `pycompss-cli-3.2/pycompss_cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/pycompss_cli/models/app.py` & `pycompss-cli-3.2/pycompss_cli/models/app.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 #  limitations under the License.
 #
 
 
 class App:
     def __init__(self, name, remote_dir=None):
         self.name = name
-        self.remote_dir = remote_dir
+        self.remote_dir = remote_dir
```

### Comparing `pycompss-cli-3.1/pycompss_cli.egg-info/PKG-INFO` & `pycompss-cli-3.2/pycompss_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompss-cli
-Version: 3.1
+Version: 3.2
 Summary: PyCOMPSs cli
 Home-page: https://compss.bsc.es
 Author: Workflows and Distributed Computing Group (WDC) - Barcelona Supercomputing Center (BSC)
 Author-email: support-compss@bsc.es
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -115,15 +115,15 @@
          python3 -m pip install docker
 
 
 Usage
 ~~~~~
 
 For detailed instructions and examples of usage please visit official documentation.
-   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_Player/02_Usage.html>`__
+   -  `PyCOMPSs-CLI Usage Documentation <https://compss-doc.readthedocs.io/en/stable/Sections/08_PyCOMPSs_CLI/02_Usage.html>`__
 
 License
 =======
 
 Apache License Version 2.0
```

### Comparing `pycompss-cli-3.1/pycompss_cli.egg-info/SOURCES.txt` & `pycompss-cli-3.2/pycompss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycompss-cli-3.1/setup.py` & `pycompss-cli-3.2/setup.py`

 * *Files identical despite different names*

