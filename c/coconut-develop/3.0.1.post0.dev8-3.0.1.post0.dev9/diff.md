# Comparing `tmp/coconut-develop-3.0.1.post0.dev8.tar.gz` & `tmp/coconut-develop-3.0.1.post0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev8.tar", last modified: Sat May 27 05:22:29 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev9.tar", last modified: Sat May 27 06:26:53 2023, max compression
```

## Comparing `coconut-develop-3.0.1.post0.dev8.tar` & `coconut-develop-3.0.1.post0.dev9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/
--rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)   194890 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6916 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/__coconut__/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/_coconut/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/mypy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   192494 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    92832 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    31834 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)   100424 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    36161 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/highlighter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/icoconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    29466 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    62531 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42128 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)    46257 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)    21832 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/coconut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 05:22:29.000000 coconut-develop-3.0.1.post0.dev8/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-27 04:25:40.000000 coconut-develop-3.0.1.post0.dev8/xontrib/coconut.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/FAQ.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)   194890 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    46257 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    62531 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42128 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    21832 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    29466 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)   100441 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    31841 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    92832 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192528 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-27 06:26:52.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36161 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-27 06:26:53.000000 coconut-develop-3.0.1.post0.dev9/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-27 05:47:14.000000 coconut-develop-3.0.1.post0.dev9/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.0.1.post0.dev8/CONTRIBUTING.md` & `coconut-develop-3.0.1.post0.dev9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/DOCS.md` & `coconut-develop-3.0.1.post0.dev9/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/FAQ.md` & `coconut-develop-3.0.1.post0.dev9/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/HELP.md` & `coconut-develop-3.0.1.post0.dev9/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/LICENSE.txt` & `coconut-develop-3.0.1.post0.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/PKG-INFO` & `coconut-develop-3.0.1.post0.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,100 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.1.post0.dev8
+Version: 3.0.1.post0.dev9
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
+Description: |logo| Coconut
+        ==============
+        
+        ..
+            <insert toctree here>
+        
+        .. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
+        
+        .. image:: https://opencollective.com/coconut/backers/badge.svg
+            :alt: Backers on Open Collective
+            :target: #backers
+        .. image:: https://opencollective.com/coconut/sponsors/badge.svg
+            :alt: Sponsors on Open Collective
+            :target: #sponsors
+        .. image:: https://badges.gitter.im/evhub/coconut.svg
+            :alt: Join the chat at https://gitter.im/evhub/coconut
+            :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
+        Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
+        
+        __ Coconut_
+        .. _Coconut: http://coconut-lang.org/
+        
+        Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
+        
+            pip install coconut
+        
+        To help you get started, check out these links for more information about Coconut:
+        
+        - Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
+        - Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
+        - `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
+        - FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
+        - `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
+        - Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
+        - Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
+        
+        .. _Python: https://www.python.org/
+        .. _PyPI: https://pypi.python.org/pypi/coconut
+        .. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
+        .. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
+        .. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
+        .. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
+        .. _GitHub: https://github.com/evhub/coconut
+        .. _Gitter: https://gitter.im/evhub/coconut
+        .. _Releases: https://github.com/evhub/coconut/releases
+        
+        Credits
+        +++++++
+        
+        Contributors
+        ------------
+        
+        This project exists thanks to all the people who contribute! `Become a contributor`__.
+        
+        .. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
+            :target: https://github.com/evhub/coconut/graphs/contributors
+        
+        __ Contributor_
+        .. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
+        
+        Backers
+        -------
+        
+        Thank you to all our backers! `Become a backer`__.
+        
+        .. image:: https://opencollective.com/coconut/backers.svg?width=890
+            :target: https://opencollective.com/coconut#backers
+        
+        __ Backer_
+        .. _Backer: https://opencollective.com/coconut#backer
+        
+        Sponsors
+        --------
+        
+        Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
+        
+        .. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
+            :target: https://opencollective.com/coconut/sponsor/0/website
+        
+        __ Sponsor_
+        .. _Sponsor: https://opencollective.com/coconut#sponsor
+        
 Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,parallel_map,addpattern,recursive_iterator,concurrent_map,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,all_equal,collectby,multi_enumerate,cartesian_product,multiset,cycle,windowsof,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
@@ -47,91 +131,7 @@
 Provides-Extra: xonsh
 Provides-Extra: jupyter
 Provides-Extra: all
 Provides-Extra: ipython
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-|logo| Coconut
-==============
-
-..
-    <insert toctree here>
-
-.. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
-
-.. image:: https://opencollective.com/coconut/backers/badge.svg
-    :alt: Backers on Open Collective
-    :target: #backers
-.. image:: https://opencollective.com/coconut/sponsors/badge.svg
-    :alt: Sponsors on Open Collective
-    :target: #sponsors
-.. image:: https://badges.gitter.im/evhub/coconut.svg
-    :alt: Join the chat at https://gitter.im/evhub/coconut
-    :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
-
-__ Coconut_
-.. _Coconut: http://coconut-lang.org/
-
-Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
-
-    pip install coconut
-
-To help you get started, check out these links for more information about Coconut:
-
-- Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
-- Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
-- `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
-- FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
-- `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
-- Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
-- Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
-
-.. _Python: https://www.python.org/
-.. _PyPI: https://pypi.python.org/pypi/coconut
-.. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
-.. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
-.. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
-.. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
-.. _GitHub: https://github.com/evhub/coconut
-.. _Gitter: https://gitter.im/evhub/coconut
-.. _Releases: https://github.com/evhub/coconut/releases
-
-Credits
-+++++++
-
-Contributors
-------------
-
-This project exists thanks to all the people who contribute! `Become a contributor`__.
-
-.. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
-    :target: https://github.com/evhub/coconut/graphs/contributors
-
-__ Contributor_
-.. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
-
-Backers
--------
-
-Thank you to all our backers! `Become a backer`__.
-
-.. image:: https://opencollective.com/coconut/backers.svg?width=890
-    :target: https://opencollective.com/coconut#backers
-
-__ Backer_
-.. _Backer: https://opencollective.com/coconut#backer
-
-Sponsors
---------
-
-Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
-
-.. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
-    :target: https://opencollective.com/coconut/sponsor/0/website
-
-__ Sponsor_
-.. _Sponsor: https://opencollective.com/coconut#sponsor
```

### Comparing `coconut-develop-3.0.1.post0.dev8/README.rst` & `coconut-develop-3.0.1.post0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/__coconut__/__init__.py` & `coconut-develop-3.0.1.post0.dev9/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/__coconut__/__init__.pyi` & `coconut-develop-3.0.1.post0.dev9/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/_coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev9/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/_coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev9/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/__coconut__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/__coconut__.pyi` & `coconut-develop-3.0.1.post0.dev9/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev9/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/__main__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/_pyparsing.py` & `coconut-develop-3.0.1.post0.dev9/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/api.py` & `coconut-develop-3.0.1.post0.dev9/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/api.pyi` & `coconut-develop-3.0.1.post0.dev9/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/__init__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/cli.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/command.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/command.pyi` & `coconut-develop-3.0.1.post0.dev9/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/mypy.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/util.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/command/watch.py` & `coconut-develop-3.0.1.post0.dev9/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/__init__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/compiler.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -3098,18 +3098,18 @@
             fake_mods = imp_as.split(".")
             for i in range(1, len(fake_mods)):
                 mod_name = ".".join(fake_mods[:i])
                 out.extend((
                     "try:",
                     openindent + mod_name,
                     closeindent + "except:",
-                    openindent + mod_name + ' = _coconut.types.ModuleType("' + mod_name + '")',
+                    openindent + mod_name + ' = _coconut.types.ModuleType(_coconut_py_str("' + mod_name + '"))',
                     closeindent + "else:",
                     openindent + "if not _coconut.isinstance(" + mod_name + ", _coconut.types.ModuleType):",
-                    openindent + mod_name + ' = _coconut.types.ModuleType("' + mod_name + '")' + closeindent * 2,
+                    openindent + mod_name + ' = _coconut.types.ModuleType(_coconut_py_str("' + mod_name + '"))' + closeindent * 2,
                 ))
             out.append(".".join(fake_mods) + " = " + import_as_var)
         else:
             out.append(import_stmt(imp_from, imp, imp_as))
 
         if type_ignore:
             for i, line in enumerate(out):
```

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/grammar.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/header.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
     if not hasattr(typing, _name):
         setattr(typing, _name, getattr(_typing, _name))
             ''',
             if_lt='''
 if not hasattr(typing, "TYPE_CHECKING"):
     typing.TYPE_CHECKING = False
 if not hasattr(typing, "Any"):
-    Any = Ellipsis
+    typing.Any = Ellipsis
 if not hasattr(typing, "cast"):
     def cast(t, x):
         """typing.cast[T](t: Type[T], x: Any) -> T = x"""
         return x
     typing.cast = cast
     cast = staticmethod(cast)
 if not hasattr(typing, "TypeVar"):
```

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/matching.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/templates/header.py_template`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     import collections, copy, functools, types, itertools, operator, threading, os, warnings, contextlib, traceback, weakref, multiprocessing
     from multiprocessing import dummy as multiprocessing_dummy
 {maybe_bind_lru_cache}{import_copyreg}
 {import_asyncio}
 {import_pickle}
 {import_OrderedDict}
 {import_collections_abc}
-    typing = types.ModuleType("typing")
+    typing = types.ModuleType(_coconut_py_str("typing"))
     try:
         import typing_extensions
     except ImportError:
         typing_extensions = None
     else:
         for _name in dir(typing_extensions):
             if not _name.startswith("__"):
```

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/compiler/util.py` & `coconut-develop-3.0.1.post0.dev9/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/constants.py` & `coconut-develop-3.0.1.post0.dev9/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/convenience.py` & `coconut-develop-3.0.1.post0.dev9/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/convenience.pyi` & `coconut-develop-3.0.1.post0.dev9/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/exceptions.py` & `coconut-develop-3.0.1.post0.dev9/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/highlighter.py` & `coconut-develop-3.0.1.post0.dev9/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/icoconut/__init__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/icoconut/__main__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/icoconut/embed.py` & `coconut-develop-3.0.1.post0.dev9/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/icoconut/root.py` & `coconut-develop-3.0.1.post0.dev9/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/integrations.py` & `coconut-develop-3.0.1.post0.dev9/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/main.py` & `coconut-develop-3.0.1.post0.dev9/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/requirements.py` & `coconut-develop-3.0.1.post0.dev9/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/root.py` & `coconut-develop-3.0.1.post0.dev9/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.1"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 8
+DEVELOP = 9
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/terminal.py` & `coconut-develop-3.0.1.post0.dev9/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/__init__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/__main__.py` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/constants_test.py` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/main_test.py` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/tests/src/extras.coco` & `coconut-develop-3.0.1.post0.dev9/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut/util.py` & `coconut-develop-3.0.1.post0.dev9/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.1.post0.dev9/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/conf.py` & `coconut-develop-3.0.1.post0.dev9/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/setup.py` & `coconut-develop-3.0.1.post0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev8/xontrib/coconut.py` & `coconut-develop-3.0.1.post0.dev9/xontrib/coconut.py`

 * *Files identical despite different names*

