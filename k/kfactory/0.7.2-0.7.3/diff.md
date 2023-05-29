# Comparing `tmp/kfactory-0.7.2.tar.gz` & `tmp/kfactory-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.7.2.tar", last modified: Thu May 25 14:44:47 2023, max compression
+gzip compressed data, was "kfactory-0.7.3.tar", last modified: Mon May 29 18:44:27 2023, max compression
```

## Comparing `kfactory-0.7.2.tar` & `kfactory-0.7.3.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.818908 kfactory-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 14:44:26.000000 kfactory-0.7.2/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.806908 kfactory-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.806908 kfactory-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 14:44:26.000000 kfactory-0.7.2/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 14:44:26.000000 kfactory-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 14:44:26.000000 kfactory-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 14:44:26.000000 kfactory-0.7.2/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 14:44:26.000000 kfactory-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 14:44:26.000000 kfactory-0.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 14:44:47.818908 kfactory-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-25 14:44:26.000000 kfactory-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.810908 kfactory-0.7.2/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-25 14:44:26.000000 kfactory-0.7.2/docs/source/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-25 14:44:26.000000 kfactory-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:44:47.818908 kfactory-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.806908 kfactory-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/cells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    90612 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/klayout_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/layer_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/technology/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-25 14:44:26.000000 kfactory-0.7.2/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.814908 kfactory-0.7.2/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 14:44:47.000000 kfactory-0.7.2/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 14:44:47.000000 kfactory-0.7.2/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:44:47.000000 kfactory-0.7.2/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 14:44:47.000000 kfactory-0.7.2/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 14:44:47.000000 kfactory-0.7.2/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:44:47.818908 kfactory-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 14:44:26.000000 kfactory-0.7.2/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-29 18:44:11.000000 kfactory-0.7.3/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-29 18:44:11.000000 kfactory-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-29 18:44:11.000000 kfactory-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 18:44:11.000000 kfactory-0.7.3/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 18:44:11.000000 kfactory-0.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 18:44:11.000000 kfactory-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 18:44:11.000000 kfactory-0.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 18:44:27.615246 kfactory-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-29 18:44:11.000000 kfactory-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 18:44:11.000000 kfactory-0.7.3/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 18:44:11.000000 kfactory-0.7.3/docs/source/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 18:44:11.000000 kfactory-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:44:27.615246 kfactory-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.607246 kfactory-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/cells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90744 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/klayout_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/layer_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/technology/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-29 18:44:11.000000 kfactory-0.7.3/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.611246 kfactory-0.7.3/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 18:44:27.000000 kfactory-0.7.3/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:27.615246 kfactory-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-29 18:44:11.000000 kfactory-0.7.3/tests/test_spiral.py
```

### Comparing `kfactory-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.7.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/.github/workflows/pages.yml` & `kfactory-0.7.3/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/.github/workflows/release.yml` & `kfactory-0.7.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/.github/workflows/test_code.yml` & `kfactory-0.7.3/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/.pre-commit-config.yaml` & `kfactory-0.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/LICENSE` & `kfactory-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/Makefile` & `kfactory-0.7.3/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/PKG-INFO` & `kfactory-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.2
+Version: 0.7.3
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
 
-# KFactory 0.7.2
+# KFactory 0.7.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.2/README.md` & `kfactory-0.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.7.2
+# KFactory 0.7.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.2/docs/mkdocs.yml` & `kfactory-0.7.3/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/_static/complex.png` & `kfactory-0.7.3/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/_static/klive.webm` & `kfactory-0.7.3/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/_static/waveguide.png` & `kfactory-0.7.3/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/complex_cell.py` & `kfactory-0.7.3/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/config.md` & `kfactory-0.7.3/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/gen_ref_pages.py` & `kfactory-0.7.3/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/intro.md` & `kfactory-0.7.3/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/notebooks/00_geometry.py` & `kfactory-0.7.3/docs/source/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/notebooks/01_references.py` & `kfactory-0.7.3/docs/source/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/notebooks/02_DRC.py` & `kfactory-0.7.3/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/notebooks/03_Enclosures.py` & `kfactory-0.7.3/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/pre.md` & `kfactory-0.7.3/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/star.py` & `kfactory-0.7.3/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/docs/source/waveguide.py` & `kfactory-0.7.3/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/__init__.py` & `kfactory-0.7.3/src/kfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     LayerEnum,
     show,
 )
 from . import cells, placer, routing, utils, port, pdk
 from .conf import config
 from .pdk import Pdk
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
```

### Comparing `kfactory-0.7.2/src/kfactory/cells/bezier.py` & `kfactory-0.7.3/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/circular.py` & `kfactory-0.7.3/src/kfactory/cells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/dbu/taper.py` & `kfactory-0.7.3/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/dbu/waveguide.py` & `kfactory-0.7.3/src/kfactory/cells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/euler.py` & `kfactory-0.7.3/src/kfactory/cells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/taper.py` & `kfactory-0.7.3/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/cells/waveguide.py` & `kfactory-0.7.3/src/kfactory/cells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/conf.py` & `kfactory-0.7.3/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/kcell.py` & `kfactory-0.7.3/src/kfactory/kcell.py`

 * *Files 0% similar despite different names*

```diff
@@ -930,14 +930,18 @@
         self.ports: Ports = ports or Ports(self.kcl)
         self.complex = False
 
         if kdb_cell is not None:
             for inst in kdb_cell.each_inst():
                 self.insts.append(Instance(self.kcl, inst))
 
+    def __getitem__(self, key: int | str | None) -> Port:
+        """Returns port from instance."""
+        return self.ports[key]
+
     @property
     def name(self) -> str:
         """Name of the KCell."""
         return self._kdb_cell.name
 
     @name.setter
     def name(self, value: str) -> None:
```

### Comparing `kfactory-0.7.2/src/kfactory/pdk.py` & `kfactory-0.7.3/src/kfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/placer.py` & `kfactory-0.7.3/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/port.py` & `kfactory-0.7.3/src/kfactory/port.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,23 @@
         regex: Regex string to filter the port names by.
         prefix: Prefix to add to all ports.
         start: Start index per orientation.
     """
     _ports = filter_layer_pt_reg(ports, layer, port_type, regex)
 
     def sort_key(port: "Port") -> tuple[int, int, int]:
-        angle = (2 - port.angle) % 4  # angles should follow the order 2, 1, 0, 3
+        match port.angle:
+            case 2:
+                angle = 0
+            case 1:
+                angle = 1
+            case 0:
+                angle = 2
+            case 3:
+                angle = 3
         dir_1 = 1 if angle < 2 else -1
         dir_2 = -1 if port.angle < 2 else 1
         key_1 = dir_1 * (
             port.trans.disp.x if angle % 2 else port.trans.disp.y
         )  # order should be y, x, -y, -x
         key_2 = dir_2 * (
             port.trans.disp.y if angle % 2 else port.trans.disp.x
```

### Comparing `kfactory-0.7.2/src/kfactory/routing/electrical.py` & `kfactory-0.7.3/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/routing/manhattan.py` & `kfactory-0.7.3/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/routing/optical.py` & `kfactory-0.7.3/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/klayout_tech.py` & `kfactory-0.7.3/src/kfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/layer_map.py` & `kfactory-0.7.3/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/layer_stack.py` & `kfactory-0.7.3/src/kfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/layer_views.py` & `kfactory-0.7.3/src/kfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/xml_utils.py` & `kfactory-0.7.3/src/kfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/technology/yaml_utils.py` & `kfactory-0.7.3/src/kfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/typings.py` & `kfactory-0.7.3/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/utils/__init__.py` & `kfactory-0.7.3/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/utils/enclosure.py` & `kfactory-0.7.3/src/kfactory/utils/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/utils/fill.py` & `kfactory-0.7.3/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/utils/simplify.py` & `kfactory-0.7.3/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/utils/violations.py` & `kfactory-0.7.3/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory/widgets/interactive.py` & `kfactory-0.7.3/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.7.3/src/kfactory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.2
+Version: 0.7.3
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
 
-# KFactory 0.7.2
+# KFactory 0.7.3
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.2` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.3` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.2/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.7.3/src/kfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-.bumpversion.cfg
 .gitignore
 .pre-commit-config.yaml
 .sourcery.yaml
+CHANGELOG.md
 LICENSE
 Makefile
 README.md
 pyproject.toml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/pages.yml
 .github/workflows/release.yml
 .github/workflows/test_code.yml
+changelog.d/changelog_template.jinja
 docs/mkdocs.yml
 docs/overrides/main.html
-docs/source/CHANGELOG.md
+docs/source/changelog.md
 docs/source/complex_cell.py
 docs/source/config.md
 docs/source/gen_ref_pages.py
 docs/source/index.md
 docs/source/intro.md
 docs/source/layers.py
 docs/source/pre.md
```

### Comparing `kfactory-0.7.2/src/kfactory.egg-info/requires.txt` & `kfactory-0.7.3/src/kfactory.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 gitpython
 pylsp-mypy
 python-lsp-server[all]
 python-lsp-ruff
 types-cachetools
 python-lsp-black
 kfactory[git]
+towncrier
 
 [docs]
 kfactory[ipy]
 mkdocs
 mkdocs-jupyter>=0.24
 mkdocstrings[python]
 mkdocs-material
```

### Comparing `kfactory-0.7.2/tests/conftest.py` & `kfactory-0.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_cells.py` & `kfactory-0.7.3/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_cplxcells.py` & `kfactory-0.7.3/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_enclosure.py` & `kfactory-0.7.3/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_extrude.py` & `kfactory-0.7.3/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_pdk.py` & `kfactory-0.7.3/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_ports.py` & `kfactory-0.7.3/tests/test_ports.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,27 +88,15 @@
     c.add_port(wg1.ports["o1"])
     c.add_port(wg2.ports["o2"])
 
     kf.config.logfilter.regex = None
     c.flatten()
 
 
-# def test_floating(wg_floating_off_grid):
-#     c = kf.KCell()
-
-#     wg1 = c << wg_floating_off_grid
-#     wg2 = c << wg_floating_off_grid
-#     wg2.connect("o2", wg1, "o1")
-
-
 def test_connect_integer(wg):
     c = kf.KCell()
 
     wg1 = c << wg
     wg2 = c << wg
     wg2.connect("o1", wg1, "o1")
 
     assert wg2.ports["o1"].trans == kf.kdb.Trans(0, False, 0, 0)
-
-
-# if __name__ == "__main__":
-#     test_waveguide()
```

### Comparing `kfactory-0.7.2/tests/test_rename.py` & `kfactory-0.7.3/tests/test_rename.py`

 * *Files 17% similar despite different names*

```diff
@@ -85,7 +85,35 @@
         [f"E{i}" for i in [3, 0, 2, 4, 1]]
         + [f"N{i}" for i in [3, 4, 2, 0, 1]]
         + [f"W{i}" for i in [3, 4, 2, 0, 1]]
         + [f"S{i}" for i in [3, 0, 2, 4, 1]]
     )
 
     assert [p.name for p in port_list] == names
+
+
+def test_rename_setter():
+    kcl = kf.KCLayout()
+
+    assert kcl.rename_function == kf.port.rename_clockwise
+
+    c1 = kf.KCell(kcl=kcl)
+    c1.create_port(
+        trans=kf.kdb.Trans(2, False, 0, 0), width=1000, layer=kcl.layer(1, 0)
+    )
+    c1.create_port(trans=kf.kdb.Trans(), width=1000, layer=kcl.layer(1, 0))
+    c1.autorename_ports()
+
+    kcl.rename_function = kf.port.rename_by_direction
+
+    c2 = kf.KCell(kcl=kcl)
+    c2.create_port(
+        trans=kf.kdb.Trans(2, False, 0, 0), width=1000, layer=kcl.layer(1, 0)
+    )
+    c2.create_port(trans=kf.kdb.Trans(), width=1000, layer=kcl.layer(1, 0))
+    c2.autorename_ports()
+
+    print(c1.ports)
+    print(c2.ports)
+
+    assert c1.ports[0].name == "o1"
+    assert c2.ports[0].name == "W0"
```

### Comparing `kfactory-0.7.2/tests/test_routing.py` & `kfactory-0.7.3/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.2/tests/test_spiral.py` & `kfactory-0.7.3/tests/test_spiral.py`

 * *Files identical despite different names*

