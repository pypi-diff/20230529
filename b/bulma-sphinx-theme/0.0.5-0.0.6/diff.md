# Comparing `tmp/bulma_sphinx_theme-0.0.5.tar.gz` & `tmp/bulma_sphinx_theme-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.5.tar", last modified: Mon May 29 00:47:04 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.6.tar", last modified: Mon May 29 16:20:06 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.5.tar` & `bulma_sphinx_theme-0.0.6.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:47:03.943229 bulma_sphinx_theme-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/source-buttons.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_docutils.scss
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:20:06.176795 bulma_sphinx_theme-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-29 16:19:43.939177 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_docutils.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-29 16:19:43.943178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 16:19:43.947178 bulma_sphinx_theme-0.0.6/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.6/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.5/LICENSE` & `bulma_sphinx_theme-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/README.md` & `bulma_sphinx_theme-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.6/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/conf.py` & `bulma_sphinx_theme-0.0.6/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
     "bulma_sphinx_theme.demo.sphinxext",
     "myst_parser",
+    # "ablog",
     # "jupyter_sphinx",
     # "myst_nb",
     # "matplotlib.sphinxext.plot_directive",
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
@@ -56,14 +57,15 @@
 
 todo_include_todos = True
 
 # https://github.com/hung1001/font-awesome-pro-v6
 # html_css_files = [
 #     "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 # ]
+# fontawesome_included = True
 
 html_theme_options = {
     "header_links_before_dropdown": 5,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
     "logo": {"text": "Bulma Sphinx Theme", "logo": "_static/logo.svg"},
     "header_icons": [
         {
@@ -104,7 +106,34 @@
     "fix_navbar": True,
     "navbar_start": [],
     "navbar_end": ["navbar-nav.html", "header-icons.html"],
     "have_top_navbar": True,
 }
 
 html_context = {"default_mode": "auto"}
+
+# blog_path = "blog"
+# blog_post_pattern = "posts/*/*"
+# blog_authors = {
+#     "zclab": ("子川", "https://github.com/zclab"),
+# }
+
+# html_sidebars = {
+#     "posts/**": [
+#         "ablog/postcard.html",
+#         "ablog/categories.html",
+#         "ablog/tagcloud.html",
+#         "ablog/recentposts.html",
+#     ],
+#     "blog": [
+#         "ablog/categories.html",
+#         "ablog/tagcloud.html",
+#         "ablog/archives.html",
+#         "ablog/recentposts.html",
+#     ],
+#     "blog/**": [
+#         "ablog/categories.html",
+#         "ablog/tagcloud.html",
+#         "ablog/archives.html",
+#         "ablog/recentposts.html",
+#     ],
+# }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bulma_sphinx_theme-0.0.5/docs/develop.md` & `bulma_sphinx_theme-0.0.6/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/index.md` & `bulma_sphinx_theme-0.0.6/docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.6/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.0.6/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.0.6/docs/user_guide/navbar.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/user_guide/source-buttons.md` & `bulma_sphinx_theme-0.0.6/docs/user_guide/source-buttons.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/docs/web-components.rst` & `bulma_sphinx_theme-0.0.6/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/noxfile.py` & `bulma_sphinx_theme-0.0.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/package-lock.json` & `bulma_sphinx_theme-0.0.6/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/package.json` & `bulma_sphinx_theme-0.0.6/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/pyproject.toml` & `bulma_sphinx_theme-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,12 @@
 /*********************************************
 * SASS Mixins
 *********************************************/
 
 /**
-* Scrollbars should be thinner and slightly rounded, with a grey background
-* ref: https://www.nngroup.com/articles/scrolling-and-scrollbars/
-*/
-@mixin scrollbar-style() {
-  &::-webkit-scrollbar {
-    width: 0.5rem;
-    height: 0.5rem;
-  }
-
-  &::-webkit-scrollbar-thumb {
-    background: var(--bst-color-text-muted);
-    border-radius: 0.25rem;
-  }
-
-  &::-webkit-scrollbar-track {
-    background: transparent;
-  }
-
-  &::-webkit-scrollbar-thumb {
-    background: var(--bst-color-on-surface);
-  }
-
-  // Hovering behavior for the scrollbar
-  // Include both hovering on the parent and on the thumb in case thumb is outside parent
-  &:hover {
-    &::-webkit-scrollbar-thumb {
-      background: var(--bst-color-text-muted);
-    }
-  }
-
-  &::-webkit-scrollbar-thumb:hover {
-    background: var(--bst-color-text-muted);
-  }
-}
-
-/**
  * A consistent box shadow style we apply across elements.
  */
 @mixin box-shadow() {
   box-shadow: 0 0.2rem 0.5rem var(--bst-color-shadow),
     0 0 0.0625rem var(--bst-color-shadow) !important;
 }
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 6% similar despite different names*

```diff
@@ -92,12 +92,19 @@
   }
 }
 
 strong {
   color: var(--bst-color-text-base);
 }
 
-a.reference.download:before {
-  content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2'/%3E%3Cpath d='M7 11l5 5l5 -5'/%3E%3Cpath d='M12 4l0 12'/%3E%3C/svg%3E");
-  margin-right: 0.3rem;
-  vertical-align: middle;
+a {
+  &.reference.download {
+    &::before {
+      margin-right: 0.25rem;
+      vertical-align: middle;
+    }
+  }
+
+  &.reference.download::before {
+    content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2'/%3E%3Cpath d='M7 11l5 5l5 -5'/%3E%3Cpath d='M12 4l0 12'/%3E%3C/svg%3E");
+  }
 }
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files 1% similar despite different names*

```diff
@@ -42,24 +42,24 @@
     display: flex;
     align-items: center;
     color: var(--bst-color-text-base);
 
     &:after {
       position: absolute;
       left: 0.5rem;
-      width: 1rem;
-      height: 1rem;
+      width: 1.2rem;
+      height: 1.2rem;
       line-height: inherit;
       background-color: var(--bst-color-info);
       content: "";
       mask-image: var(--bst-icon-admonition-default);
       opacity: 1;
     }
 
-    @include background-from-color-variable(--bst-color-info, 0.2);
+    @include background-from-color-variable(--bst-color-info, 0.1);
 
     // Next element after title needs some extra upper-space
     + * {
       margin-top: 0.4em;
     }
   }
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 // Blockquote
 blockquote
   border-left: 4px solid var(--bst-color-border)
   background: var(--bst-color-surface)
 
   margin-left: 0
   margin-right: 0
+  margin-top: 0.5rem
+  margin-bottom: 0.5rem
   padding: 0.5rem 1rem
 
   .attribution
     font-weight: 600
     text-align: right
 
   &.pull-quote,
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   border-radius: 0.2rem
   border-spacing: 0
   border-collapse: collapse
 
   box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), 0 0 0.0625rem rgba(0, 0, 0, 0.1)
 
   th
-    background: var(--bst-color-background-sidenav)
+    background: var(--bst-color-canvas)
     color: var(--bst-color-text-base)
 
   td,
   th
     // Space things out properly
     padding: 0 0.25rem
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 12% similar despite different names*

```diff
@@ -85,19 +85,14 @@
   li {
     position: relative;
 
     &.has-children {
       > .reference {
         padding-right: 30px;
       }
-
-      > ul {
-        background-color: var(--bst-color-background-sidenav);
-        padding: 0 0 0 1rem;
-      }
     }
   }
 
   .toctree-checkbox {
     position: absolute;
     display: none;
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .bulma-tocnav {
   width: var(--tocnav-width);
   padding: 0 1rem;
-  word-break: break-all;
+  word-break: break-word;
 
   .toc-wrapper {
     position: sticky;
     top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
     overflow-y: auto;
     max-height: calc(
       100vh - var(--navbar-height) - var(--top-content-to-navbar-gap)
@@ -19,15 +19,14 @@
       border-left: 1px solid var(--bst-color-border);
 
       a {
         display: inline-block;
         color: var(--bst-color-text-base);
         padding-left: 16px;
         height: 1.6rem;
-        line-height: 1.5rem;
       }
 
       &.scroll-current > .reference {
         border-left: 1px solid $link;
         color: $link;
         font-weight: bold;
       }
@@ -46,10 +45,12 @@
     > .active > ul {
       display: block;
     }
   }
 }
 
 .toc-title {
+  font-weight: 600;
   padding-left: 16px;
+  padding-bottom: 5px;
   font-size: var(--toc-title-font-size);
 }
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 html {
   /*****************************************************************************
   * Admonitions
   **/
 
   --bst-icon-admonition-default: var(--icon-bell);
   --bst-icon-admonition-note: var(--icon-pencil);
-  --bst-icon-admonition-attention: var(--icon-warning);
-  --bst-icon-admonition-caution: var(--icon-spark);
+  --bst-icon-admonition-attention: var(--icon-horn);
+  --bst-icon-admonition-caution: var(--icon-signmark);
   --bst-icon-admonition-warning: var(--icon-warning);
   --bst-icon-admonition-danger: var(--icon-spark);
   --bst-icon-admonition-error: var(--icon-failure);
-  --bst-icon-admonition-hint: var(--icon-question);
-  --bst-icon-admonition-tip: var(--icon-info);
+  --bst-icon-admonition-hint: var(--icon-bulb);
+  --bst-icon-admonition-tip: var(--icon-edit);
   --bst-icon-admonition-important: var(--icon-flame);
-  --bst-icon-admonition-seealso: var(--icon-info);
+  --bst-icon-admonition-seealso: var(--icon-share);
   --bst-icon-admonition-todo: var(--icon-pencil);
 }
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     "light": rgb(240, 248, 255),
     "dark": rgb(18, 18, 18),
   ),
   "background-info-panel": (
     "light": linear-gradient(0.25turn, #e3e5f7, #d9e1ef, #e8ebfb),
     "dark": linear-gradient(0.25turn, #5e605a, #51544e, #5a5c58),
   ),
+  "canvas": (
+    "light": rgb(246, 248, 250),
+    "dark": rgb(22, 27, 34),
+  ),
 );
 
 /*******************************************************************************
 * write the color rules for each theme (light/dark)
 */
 
 /* NOTE:
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   --sidebar-caption-font-size: var(--font-size--small--2);
   --sidebar-item-font-size: var(--font-size--small);
   --sidebar-search-input-font-size: var(--font-size--small);
 
   // Table of Contents
   --toc-font-size: var(--font-size--small);
   --toc-font-size--mobile: var(--font-size--normal);
-  --toc-title-font-size: var(--font-size--small--2);
+  --toc-title-font-size: var(--font-size--small);
 
   // Admonitions
   //
   // These aren't defined in terms of %ages, since nesting these is permitted.
   --admonition-font-size: 1em;
   --admonition-title-font-size: 1em;
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 navbar_start = navbar-nav.html
 navbar_end = header-icons.html
 navbar_include_directly = navbar-nav.html, header-icons.html
 analytics =
 footer = copyright.html, sphinx-version.html
 toc_title = On this page
 dropdown_label_name = More
+dropdown_label_target_url =
 navigation_with_keys = True
 search_bar_text = Search the docs ...
 show_back_to_top = True
 article_top_left = breadcrumbs.html
 article_top_right = edit-this-page.html
 article_bottom_left = last-updated.html
 article_bottom_right = sourcelink.html
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/toctree.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,22 +252,33 @@
         links_solo = links_html[:n_links_before_dropdown]
         out_headnav = "\n".join(links_solo)
 
         # Wrap the final few header items in a "more" dropdown
         links_dropdown = links_html[n_links_before_dropdown:]
         if links_dropdown:
             links_dropdown_html = "\n".join(links_dropdown)
-            out_headnav += f"""
-            <div class="navbar-item has-dropdown is-hoverable">
-                <a class="navbar-link">{context["theme_dropdown_label_name"]}</a>
-                <div class="navbar-dropdown">
-                    {links_dropdown_html}
+            if context["theme_dropdown_label_target_url"]:
+                out_headnav += f"""
+                <div class="navbar-item has-dropdown is-hoverable">
+                    <a class="navbar-link" href={context["theme_dropdown_label_target_url"]}>{context["theme_dropdown_label_name"]}</a>
+                    <div class="navbar-dropdown">
+                        {links_dropdown_html}
+                    </div>
                 </div>
-            </div>
-            """  # noqa
+                """  # noqa
+
+            else:
+                out_headnav += f"""
+                <div class="navbar-item has-dropdown is-hoverable">
+                    <span class="navbar-link">{context["theme_dropdown_label_name"]}</span>
+                    <div class="navbar-dropdown">
+                        {links_dropdown_html}
+                    </div>
+                </div>
+                """  # noqa
 
         return out_headnav
 
     # Cache this function because it is expensive to run, and becaues Sphinx
     # somehow runs this twice in some circumstances in unpredictable ways.
     @functools.lru_cache(maxsize=None)
     def generate_toctree_html(kind, startdepth=1, show_nav_level=1, **kwargs):
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/translations.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             with out_path.open("a") as f:
                 f.write("\n")
                 f.write(f'msgid "{english}"\n')
                 text = item["text"].replace('"', '\\"')
                 f.write(f'msgstr "{text}"\n')
 
     # compile mo
-    for path in (out_folder / "locales").glob("**/bulmasphinxthemepo"):
+    for path in (out_folder / "locales").glob("**/bulmasphinxtheme.po"):
         print(path)
         subprocess.check_call(
             [
                 "msgfmt",
                 os.path.abspath(path),
                 "-o",
                 os.path.abspath(path.parent / "bulmasphinxtheme.mo"),
```

### Comparing `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.6/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/webpack.config.js` & `bulma_sphinx_theme-0.0.6/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.5/PKG-INFO` & `bulma_sphinx_theme-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.5
+Version: 0.0.6
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.5 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.6 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

