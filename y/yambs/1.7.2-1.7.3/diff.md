# Comparing `tmp/yambs-1.7.2.tar.gz` & `tmp/yambs-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.7.2.tar", last modified: Sat May 27 09:22:15 2023, max compression
+gzip compressed data, was "yambs-1.7.3.tar", last modified: Mon May 29 08:21:15 2023, max compression
```

## Comparing `yambs-1.7.2.tar` & `yambs-1.7.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.944950 yambs-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 09:21:04.000000 yambs-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-27 09:22:15.944950 yambs-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-27 09:21:04.000000 yambs-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-27 09:21:04.000000 yambs-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:22:15.944950 yambs-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 09:21:04.000000 yambs-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.936950 yambs-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-27 09:21:04.000000 yambs-1.7.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-27 09:21:04.000000 yambs-1.7.2/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.936950 yambs-1.7.2/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.944950 yambs-1.7.2/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.944950 yambs-1.7.2/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.944950 yambs-1.7.2/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.944950 yambs-1.7.2/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-27 09:21:04.000000 yambs-1.7.2/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:22:15.940950 yambs-1.7.2/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 09:22:15.000000 yambs-1.7.2/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 08:19:59.000000 yambs-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-29 08:21:15.289452 yambs-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-29 08:19:59.000000 yambs-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-29 08:19:59.000000 yambs-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:21:15.289452 yambs-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 08:19:59.000000 yambs-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.281452 yambs-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-29 08:19:59.000000 yambs-1.7.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 08:19:59.000000 yambs-1.7.3/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.289452 yambs-1.7.3/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-29 08:19:59.000000 yambs-1.7.3/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:21:15.285452 yambs-1.7.3/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 08:21:15.000000 yambs-1.7.3/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.7.2/LICENSE` & `yambs-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/PKG-INFO` & `yambs-1.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.7.2
+Version: 1.7.3
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d9a350c124b30b4ca51128a5abacfe22
+    hash=bb422a51478a96037d8ddd3a3e4597a7
     =====================================
 -->
 
-# yambs ([1.7.2](https://pypi.org/project/yambs/))
+# yambs ([1.7.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.7.2/README.md` & `yambs-1.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d9a350c124b30b4ca51128a5abacfe22
+    hash=bb422a51478a96037d8ddd3a3e4597a7
     =====================================
 -->
 
-# yambs ([1.7.2](https://pypi.org/project/yambs/))
+# yambs ([1.7.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.7.2/pyproject.toml` & `yambs-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.7.2"
+version = "1.7.3"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.7.2/setup.py` & `yambs-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/tests/test_entry.py` & `yambs-1.7.3/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/app.py` & `yambs-1.7.3/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/commands/all.py` & `yambs-1.7.3/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/commands/gen.py` & `yambs-1.7.3/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/commands/uf2conv.py` & `yambs-1.7.3/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/config/__init__.py` & `yambs-1.7.3/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/config/board.py` & `yambs-1.7.3/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/includes/chips.yaml` & `yambs-1.7.3/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/includes/infineon.yaml` & `yambs-1.7.3/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/includes/microchip.yaml` & `yambs-1.7.3/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/schemas/Chip.yaml` & `yambs-1.7.3/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/schemas/Config.yaml` & `yambs-1.7.3/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/templates/rules.ninja.j2` & `yambs-1.7.3/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/data/uf2families.json` & `yambs-1.7.3/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/entry.py` & `yambs-1.7.3/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/environment/__init__.py` & `yambs-1.7.3/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/__init__.py` & `yambs-1.7.3/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/architectures.py` & `yambs-1.7.3/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/boards.py` & `yambs-1.7.3/yambs/generate/boards.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,31 @@
     """Add a directory to set of paths."""
 
     LOG.debug("%s: checking '%s' for sources.", comment, path)
 
     headers = set()
 
     if path.is_dir():
-        stream.write(linesep + f"# {comment}." + linesep)
+        if comment:
+            stream.write(linesep + f"# {comment}." + linesep)
+
         for item in path.iterdir():
+            # Recurse into other directories.
+            if item.is_dir():
+                add_dir(
+                    stream,
+                    paths,
+                    item,
+                    "",
+                    base,
+                    current_sources,
+                    board,
+                    board_specific=board_specific,
+                )
+
             translator = is_source(item)
             if translator is not None:
                 paths.add(
                     write_source_line(
                         stream,
                         item,
                         base,
```

### Comparing `yambs-1.7.2/yambs/generate/chips.py` & `yambs-1.7.3/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/common.py` & `yambs-1.7.3/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/ninja/__init__.py` & `yambs-1.7.3/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/ninja/format.py` & `yambs-1.7.3/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/generate/toolchains.py` & `yambs-1.7.3/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/schemas.py` & `yambs-1.7.3/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/translation/__init__.py` & `yambs-1.7.3/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs/uf2/__init__.py` & `yambs-1.7.3/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.7.2/yambs.egg-info/PKG-INFO` & `yambs-1.7.3/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.7.2
+Version: 1.7.3
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d9a350c124b30b4ca51128a5abacfe22
+    hash=bb422a51478a96037d8ddd3a3e4597a7
     =====================================
 -->
 
-# yambs ([1.7.2](https://pypi.org/project/yambs/))
+# yambs ([1.7.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.7.2/yambs.egg-info/SOURCES.txt` & `yambs-1.7.3/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

