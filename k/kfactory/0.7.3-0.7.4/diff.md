# Comparing `tmp/kfactory-0.7.3.tar.gz` & `tmp/kfactory-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.7.3.tar", last modified: Mon May 29 18:44:27 2023, max compression
+gzip compressed data, was "kfactory-0.7.4.tar", last modified: Mon May 29 21:48:49 2023, max compression
```

## Comparing `kfactory-0.7.3.tar` & `kfactory-0.7.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-29 18:44:11.000000 kfactory-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-29 18:44:11.000000 kfactory-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 18:44:11.000000 kfactory-0.7.3/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 18:44:11.000000 kfactory-0.7.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 18:44:11.000000 kfactory-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 18:44:11.000000 kfactory-0.7.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 18:44:27.615246 kfactory-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-29 18:44:11.000000 kfactory-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 18:44:11.000000 kfactory-0.7.3/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 18:44:11.000000 kfactory-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:44:27.615246 kfactory-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    90744 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/klayout_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-29 21:48:25.000000 kfactory-0.7.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-29 21:48:25.000000 kfactory-0.7.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 21:48:25.000000 kfactory-0.7.4/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-29 21:48:25.000000 kfactory-0.7.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 21:48:25.000000 kfactory-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-29 21:48:25.000000 kfactory-0.7.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-29 21:48:49.708952 kfactory-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-29 21:48:25.000000 kfactory-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 21:48:25.000000 kfactory-0.7.4/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.696952 kfactory-0.7.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.696952 kfactory-0.7.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-29 21:48:25.000000 kfactory-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 21:48:49.708952 kfactory-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.688952 kfactory-0.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90744 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/klayout_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_spiral.py
```

### Comparing `kfactory-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/.github/workflows/pages.yml` & `kfactory-0.7.4/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/.github/workflows/release.yml` & `kfactory-0.7.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/.github/workflows/test_code.yml` & `kfactory-0.7.4/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/.pre-commit-config.yaml` & `kfactory-0.7.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
         args: []
       - id: debug-statements
       - id: end-of-file-fixer
+        exclude: "changelog.d/.*"
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/asottile/pyupgrade
```

### Comparing `kfactory-0.7.3/LICENSE` & `kfactory-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/PKG-INFO` & `kfactory-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.3
+Version: 0.7.4
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.3
+# KFactory 0.7.4
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
@@ -39,14 +39,15 @@
 
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
 
 
 New/Improved Features:
+
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
 - Enclosures: use the concept of enclosures, similar to cross sections, to allow automatic
   calculation of boolean layers for structures based on [minkowski sum](https://en.wikipedia.org/wiki/Minkowski_addition),
   which are built into KLayout
@@ -56,15 +57,15 @@
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
 ```bash
 pip install kfactory
 ```
 
-At the moment kfactory works only on python 3.10
+At the moment kfactory works only on python 3.10 and above
 
 ### Development Installation
 
 
 A development environment can be installed with
 
 ```bash
```

### Comparing `kfactory-0.7.3/README.md` & `kfactory-0.7.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.7.3
+# KFactory 0.7.4
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
@@ -23,14 +23,15 @@
 
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
 
 
 New/Improved Features:
+
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
 - Enclosures: use the concept of enclosures, similar to cross sections, to allow automatic
   calculation of boolean layers for structures based on [minkowski sum](https://en.wikipedia.org/wiki/Minkowski_addition),
   which are built into KLayout
@@ -40,15 +41,15 @@
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
 ```bash
 pip install kfactory
 ```
 
-At the moment kfactory works only on python 3.10
+At the moment kfactory works only on python 3.10 and above
 
 ### Development Installation
 
 
 A development environment can be installed with
 
 ```bash
```

### Comparing `kfactory-0.7.3/docs/mkdocs.yml` & `kfactory-0.7.4/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/_static/complex.png` & `kfactory-0.7.4/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/_static/klive.webm` & `kfactory-0.7.4/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/_static/waveguide.png` & `kfactory-0.7.4/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/complex_cell.py` & `kfactory-0.7.4/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/config.md` & `kfactory-0.7.4/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/gen_ref_pages.py` & `kfactory-0.7.4/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/intro.md` & `kfactory-0.7.4/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/notebooks/02_DRC.py` & `kfactory-0.7.4/docs/source/notebooks/02_DRC.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,55 @@
+# ---
+# jupyter:
+#   jupytext:
+#     cell_metadata_filter: -all
+#     custom_cell_magics: kql
+#     text_representation:
+#       extension: .py
+#       format_name: percent
+#       format_version: '1.3'
+#       jupytext_version: 1.11.2
+#   kernelspec:
+#     display_name: base
+#     language: python
+#     name: python3
+# ---
+
+# %% [markdown]
 # # Fixing DRC Errors
 #
+# ## Min space violations
 #
+# You can fix Min space violations.
 
-# +
-import kfactory as kf
-
+# %%
 from datetime import datetime
+import kfactory as kf
 
-# -
-
-triangle = kf.KCell("triangle")
+# %%
+triangle = kf.KCell()
 triangle_poly = kf.kdb.DPolygon(
     [kf.kdb.DPoint(0, 10), kf.kdb.DPoint(30, 10), kf.kdb.DPoint(30, 0)]
 )
 triangle.shapes(triangle.layer(1, 0)).insert(triangle_poly)
 triangle
 
+# %%
 box = kf.KCell("Box")
 box_rect = kf.kdb.DBox(0, 0, 20, 5)
 box.shapes(box.kcl.layer(1, 0)).insert(box_rect)
 box
 
+# %%
 c = kf.KCell("fix_accute_angle")
 c << triangle
 c << box
 c
 
-# +
+# %%
 c = kf.KCell("tiled_test")
 
 
 d1 = datetime.now()
 
 for i in range(50):
     ellipse = kf.kdb.Polygon.ellipse(kf.kdb.Box(10000, 20000), i * 2)
@@ -63,18 +82,16 @@
 
 print(f"time to draw: {d2-d1}")
 print(f"time to clean: {d3-d2}")
 print(f"total time: {d3-d1}")
 
 c
 
-# +
-c = kf.KCell("minkowski_tiled_test")
-
-
+# %%
+c = kf.KCell()
 d1 = datetime.now()
 
 for i in range(50):
     ellipse = kf.kdb.Polygon.ellipse(kf.kdb.Box(10000, 20000), i * 2)
 
     x0 = 0
     for j in range(5000, 30000, 500):
@@ -102,43 +119,56 @@
 
 d3 = datetime.now()
 
 print(f"time to draw: {d2-d1}")
 print(f"time to clean: {d3-d2}")
 print(f"total time: {d3-d1}")
 
-c
-# -
+c.show()
+c.plot()
+
+# %% [markdown]
+# ## Dummy fill
+#
+# To keep density constant you can add dummy fill.
 
-c = kf.KCell("ToFill")
+# %%
+c = kf.KCell()
 c.shapes(kf.kcl.layer(1, 0)).insert(
     kf.kdb.DPolygon.ellipse(kf.kdb.DBox(5000, 3000), 512)
 )
 c.shapes(kf.kcl.layer(10, 0)).insert(
     kf.kdb.DPolygon(
         [kf.kdb.DPoint(0, 0), kf.kdb.DPoint(5000, 0), kf.kdb.DPoint(5000, 3000)]
     )
 )
 c
 
-fc = kf.KCell("fill")
+# %%
+fc = kf.KCell()
 fc.shapes(fc.kcl.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
 fc.shapes(fc.kcl.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
 fc
 
+# %%
 import kfactory.utils.fill as fill
 
+# %%
 # fill.fill_tiled(c, fc, [(kf.kcl.layer(1,0), 0)], exclude_layers = [(kf.kcl.layer(10,0), 100), (kf.kcl.layer(2,0), 0), (kf.kcl.layer(3,0),0)], x_space=5, y_space=5)
 fill.fill_tiled(
     c,
     fc,
     [(kf.kcl.layer(1, 0), 0)],
     exclude_layers=[
         (kf.kcl.layer(10, 0), 100),
         (kf.kcl.layer(2, 0), 0),
         (kf.kcl.layer(3, 0), 0),
     ],
     x_space=5,
     y_space=5,
 )
 
-c
+# %%
+c.show()
+c.plot()
+
+# %%
```

### Comparing `kfactory-0.7.3/docs/source/pre.md` & `kfactory-0.7.4/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/star.py` & `kfactory-0.7.4/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/docs/source/waveguide.py` & `kfactory-0.7.4/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/pyproject.toml` & `kfactory-0.7.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.7.3"
+version = "0.7.4"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
@@ -39,14 +39,15 @@
 	"pylsp-mypy",
 	"python-lsp-server[all]",
 	"python-lsp-ruff",
 	"types-cachetools",
 	"python-lsp-black",
 	"kfactory[git]",
 	"towncrier",
+	"tbump",
 ]
 docs = [
 	"kfactory[ipy]",
   "mkdocs",
 	"mkdocs-jupyter>=0.24",
   "mkdocstrings[python]",
   "mkdocs-material",
@@ -232,15 +233,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.7.3"
+current = "0.7.4"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
@@ -264,16 +265,18 @@
 
 [[tool.tbump.file]]
 src = "src/kfactory/__init__.py"
 # You can specify a list of commands to
 # run after the files have been patched
 # and before the git commit is made
 
-[[tbump.before_commit]]
+[[tool.tbump.before_commit]]
 name = "create & check changelog"
-cmd = "towncrier build --yes --version {new_version} && git commit -m 'update CHANGELOG.md' && grep -q {new_version} CHANGELOG.md"
+cmd = "towncrier build --yes --version {new_version}"
 
-# Or run some commands after the git tag and the branch
-# have been pushed:
-#  [[after_push]]
-#  name = "publish"
-#  cmd = "./publish.sh"
+[[tool.tbump.before_commit]]
+name = "create & check changelog"
+cmd = "git add CHANGELOG.md"
+
+[[tool.tbump.before_commit]]
+name = "create & check changelog"
+cmd = "grep -q -F {new_version} CHANGELOG.md"
```

### Comparing `kfactory-0.7.3/src/kfactory/__init__.py` & `kfactory-0.7.4/src/kfactory/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     LayerEnum,
     show,
 )
 from . import cells, placer, routing, utils, port, pdk
 from .conf import config
 from .pdk import Pdk
 
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
```

### Comparing `kfactory-0.7.3/src/kfactory/cells/bezier.py` & `kfactory-0.7.4/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/cells/circular.py` & `kfactory-0.7.4/src/kfactory/cells/circular.py`

 * *Files 25% similar despite different names*

```diff
@@ -54,25 +54,14 @@
     )
 
     c.create_port(
         trans=kdb.Trans(2, False, 0, 0),
         width=int(width / c.kcl.dbu),
         layer=layer,
     )
-
-    match theta:
-        case 90:
-            c.create_port(
-                trans=kdb.DTrans(1, False, radius, radius).to_itype(c.kcl.dbu),
-                width=int(width / c.kcl.dbu),
-                layer=layer,
-            )
-        case 180:
-            c.create_port(
-                trans=kdb.DTrans(0, False, 0, 2 * radius).to_itype(c.kcl.dbu),
-                width=int(width / c.kcl.dbu),
-                layer=layer,
-            )
-
+    c.create_port(
+        dcplx_trans=kdb.DCplxTrans(1, theta, False, backbone[-1].to_v()),
+        dwidth=width,
+        layer=layer,
+    )
     c.autorename_ports()
-
     return c
```

### Comparing `kfactory-0.7.3/src/kfactory/cells/dbu/taper.py` & `kfactory-0.7.4/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/cells/dbu/waveguide.py` & `kfactory-0.7.4/src/kfactory/cells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/cells/euler.py` & `kfactory-0.7.4/src/kfactory/cells/euler.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,37 +186,26 @@
         layer=layer,
         path=backbone,
         width=width,
         enclosure=enclosure,
         start_angle=0,
         end_angle=theta,
     )
+    c.create_port(
+        layer=layer,
+        width=int(width / c.kcl.dbu),
+        trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
+    )
+
+    c.create_port(
+        dcplx_trans=kdb.DCplxTrans(1, theta, False, backbone[-1].to_v()),
+        dwidth=width,
+        layer=layer,
+    )
 
-    if theta == 90:
-        c.create_port(
-            layer=layer,
-            width=int(width / c.kcl.dbu),
-            trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
-        )
-        c.create_port(
-            layer=layer,
-            width=int(width / c.kcl.dbu),
-            trans=kdb.Trans(1, False, backbone[-1].to_itype(dbu).to_v()),
-        )
-    elif theta == 180:
-        c.create_port(
-            layer=layer,
-            width=int(width / c.kcl.dbu),
-            trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
-        )
-        c.create_port(
-            layer=layer,
-            width=int(width / c.kcl.dbu),
-            trans=kdb.Trans(2, False, backbone[-1].to_itype(dbu).to_v()),
-        )
     c.autorename_ports()
     return c
 
 
 @cell
 def bend_s_euler(
     offset: float,
```

### Comparing `kfactory-0.7.3/src/kfactory/cells/taper.py` & `kfactory-0.7.4/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/cells/waveguide.py` & `kfactory-0.7.4/src/kfactory/cells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/conf.py` & `kfactory-0.7.4/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/kcell.py` & `kfactory-0.7.4/src/kfactory/kcell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/pdk.py` & `kfactory-0.7.4/src/kfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/placer.py` & `kfactory-0.7.4/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/port.py` & `kfactory-0.7.4/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/routing/electrical.py` & `kfactory-0.7.4/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/routing/manhattan.py` & `kfactory-0.7.4/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/routing/optical.py` & `kfactory-0.7.4/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/klayout_tech.py` & `kfactory-0.7.4/src/kfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/layer_map.py` & `kfactory-0.7.4/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/layer_stack.py` & `kfactory-0.7.4/src/kfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/layer_views.py` & `kfactory-0.7.4/src/kfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/xml_utils.py` & `kfactory-0.7.4/src/kfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/technology/yaml_utils.py` & `kfactory-0.7.4/src/kfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/typings.py` & `kfactory-0.7.4/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/utils/__init__.py` & `kfactory-0.7.4/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/utils/enclosure.py` & `kfactory-0.7.4/src/kfactory/utils/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/utils/fill.py` & `kfactory-0.7.4/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/utils/simplify.py` & `kfactory-0.7.4/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/utils/violations.py` & `kfactory-0.7.4/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory/widgets/interactive.py` & `kfactory-0.7.4/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.7.4/src/kfactory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.3
+Version: 0.7.4
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.3
+# KFactory 0.7.4
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
@@ -39,14 +39,15 @@
 
 - [ ] CrossSection
 - [ ] Netlist/Schematics and LVS
 - [ ] More advanced routing
 
 
 New/Improved Features:
+
 - Fully hierarchical bi-directional conversion to YAML
 - Automatic snapping to grid thanks to KLayout
 - More features for vector geometries due to concept of Point/Edge/Vector/Polygon from Klayout
 - Easy booleans thanks to KLayout Regions
 - Enclosures: use the concept of enclosures, similar to cross sections, to allow automatic
   calculation of boolean layers for structures based on [minkowski sum](https://en.wikipedia.org/wiki/Minkowski_addition),
   which are built into KLayout
@@ -56,15 +57,15 @@
 
 kfactory is available on [pypi](https://pypi.org/project/kfactory/)
 
 ```bash
 pip install kfactory
 ```
 
-At the moment kfactory works only on python 3.10
+At the moment kfactory works only on python 3.10 and above
 
 ### Development Installation
 
 
 A development environment can be installed with
 
 ```bash
```

### Comparing `kfactory-0.7.3/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.7.4/src/kfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/src/kfactory.egg-info/requires.txt` & `kfactory-0.7.4/src/kfactory.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pylsp-mypy
 python-lsp-server[all]
 python-lsp-ruff
 types-cachetools
 python-lsp-black
 kfactory[git]
 towncrier
+tbump
 
 [docs]
 kfactory[ipy]
 mkdocs
 mkdocs-jupyter>=0.24
 mkdocstrings[python]
 mkdocs-material
```

### Comparing `kfactory-0.7.3/tests/conftest.py` & `kfactory-0.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_cells.py` & `kfactory-0.7.4/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_cplxcells.py` & `kfactory-0.7.4/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_enclosure.py` & `kfactory-0.7.4/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_extrude.py` & `kfactory-0.7.4/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_pdk.py` & `kfactory-0.7.4/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_ports.py` & `kfactory-0.7.4/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_rename.py` & `kfactory-0.7.4/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_routing.py` & `kfactory-0.7.4/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.3/tests/test_spiral.py` & `kfactory-0.7.4/tests/test_spiral.py`

 * *Files identical despite different names*

