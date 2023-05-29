# Comparing `tmp/bulma_sphinx_theme-0.0.4.tar.gz` & `tmp/bulma_sphinx_theme-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.4.tar", last modified: Sat May 27 11:44:01 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.5.tar", last modified: Mon May 29 00:47:04 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.4.tar` & `bulma_sphinx_theme-0.0.5.tar`

### file list

```diff
@@ -1,172 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:01.808868 bulma_sphinx_theme-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-27 11:43:41.593054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-27 11:43:41.597054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 11:43:41.601054 bulma_sphinx_theme-0.0.4/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:47:03.943229 bulma_sphinx_theme-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-29 00:46:39.615099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_docutils.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 00:46:39.619099 bulma_sphinx_theme-0.0.5/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.5/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.4/LICENSE` & `bulma_sphinx_theme-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/README.md` & `bulma_sphinx_theme-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.5/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/conf.py` & `bulma_sphinx_theme-0.0.5/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
-    "myst_parser",
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
     "bulma_sphinx_theme.demo.sphinxext",
+    "myst_parser",
+    # "jupyter_sphinx",
+    # "myst_nb",
+    # "matplotlib.sphinxext.plot_directive",
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
 exclude_patterns = [
     "_build",
     "Thumbs.db",
@@ -50,20 +53,20 @@
 html_last_updated_fmt = ""
 html_logo = "_static/logo.svg"
 html_show_sourcelink = True
 
 todo_include_todos = True
 
 # https://github.com/hung1001/font-awesome-pro-v6
-html_css_files = [
-    "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
-]
+# html_css_files = [
+#     "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
+# ]
 
 html_theme_options = {
-    "header_links_before_dropdown": 3,
+    "header_links_before_dropdown": 5,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
     "logo": {"text": "Bulma Sphinx Theme", "logo": "_static/logo.svg"},
     "header_icons": [
         {
             "name": "Github",
             "url": "https://github.com/zclab/bulma-sphinx-theme",
             "image": "https://www.svgrepo.com/show/433505/github-o.svg",
@@ -99,7 +102,9 @@
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
     "navbar_start": [],
     "navbar_end": ["navbar-nav.html", "header-icons.html"],
     "have_top_navbar": True,
 }
+
+html_context = {"default_mode": "auto"}
```

### Comparing `bulma_sphinx_theme-0.0.4/docs/develop.md` & `bulma_sphinx_theme-0.0.5/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.5/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.5/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/docs/web-components.rst` & `bulma_sphinx_theme-0.0.5/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/noxfile.py` & `bulma_sphinx_theme-0.0.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/package-lock.json` & `bulma_sphinx_theme-0.0.5/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/package.json` & `bulma_sphinx_theme-0.0.5/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/pyproject.toml` & `bulma_sphinx_theme-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -54,30 +54,31 @@
         _add_asset_hashes(
             context["scripts"],
             ["scripts/bulma-sphinx-theme.js"],
         )
 
     # determine the startdepth for building the theme
     theme_options = utils.get_theme_options(app)
-    start_depth = theme_options.get("have_top_navbar", True)
-    if not isinstance(start_depth, bool):
-        start_depth = True
-    context["start_depth"] = int(start_depth)
+    have_navbar = theme_options.get("have_top_navbar", True)
+    if not isinstance(have_navbar, bool):
+        have_navbar = True
+    context["start_depth"] = int(have_navbar)
 
     # Basic constants
     context["theme_version"] = __version__
     # Translations
     translation = get_translation(MESSAGE_CATALOG_NAME)
     context["translate"] = translation
 
 
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
     theme_options = utils.get_theme_options(app)
 
-    if not theme_options.get("have_top_navbar"):
+    have_navbar = theme_options.get("have_top_navbar", True)
+    if not (have_navbar):
         theme_options["fix_navbar"] = False
 
     # Add an analytics ID to the site if provided
     analytics = theme_options.get("analytics", {})
     if analytics:
         # Google Analytics
         gid = analytics.get("google_analytics_id")
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 25% similar despite different names*

```diff
@@ -91,7 +91,13 @@
     margin-bottom: 0;
   }
 }
 
 strong {
   color: var(--bst-color-text-base);
 }
+
+a.reference.download:before {
+  content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2'/%3E%3Cpath d='M7 11l5 5l5 -5'/%3E%3Cpath d='M12 4l0 12'/%3E%3C/svg%3E");
+  margin-right: 0.3rem;
+  vertical-align: middle;
+}
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files 8% similar despite different names*

```diff
@@ -56,7 +56,15 @@
  */
 code.literal {
   padding: 0.1rem 0.25rem;
   background-color: var(--bst-color-surface);
   border: 1px solid var(--bst-color-on-surface);
   border-radius: 0.25rem;
 }
+
+div.highlight {
+  .gp,
+  span.linenos {
+    user-select: none;
+    pointer-events: none;
+  }
+}
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files 21% similar despite different names*

```diff
@@ -39,22 +39,42 @@
     }
 
     &.upperroman {
       list-style: upper-roman;
     }
   }
 
-  .simple,
   .toctree-wrapper {
-    li {
-      > ul,
-      > ol {
-        margin-top: 0;
-        margin-bottom: 0;
+    p.caption {
+      font-size: $size-4;
+      margin-bottom: 0em;
+    }
+
+    & > ul {
+      padding-left: 0;
+    }
+
+    li[class^="toctree-l"] {
+      list-style: none;
+      margin-bottom: 0.2em;
+
+      & > a {
+        list-style: none;
+        font-size: 1.1em;
       }
+
+      & > ul {
+        list-style: none;
+        padding-inline-start: 1.5em;
+      }
+    }
+
+    // slightly bigger font for l1
+    .toctree-l1 > a {
+      font-size: $size-5;
     }
   }
 
   .field-list,
   .option-list,
   dl:not([class]),
   dl.simple,
@@ -112,7 +132,18 @@
         & > li {
           list-style-type: square;
         }
       }
     }
   }
 }
+
+div.topic.contents,
+// Docutils <= 0.17
+nav.contents // Docutils >= 0.18
+{
+  // Style similarly to toctree
+  ul.simple {
+    list-style: none;
+    padding-left: 0;
+  }
+}
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 20% similar despite different names*

```diff
@@ -102,21 +102,39 @@
     display: none;
 
     ~ ul {
       display: none;
     }
 
     ~ label i {
-      transform: rotate(0deg);
+      transform: rotate(90deg);
     }
   }
 
   .toctree-checkbox:checked {
     ~ ul {
       display: block;
     }
 
     ~ label i {
-      transform: rotate(180deg);
+      transform: rotate(-90deg);
+    }
+  }
+
+  .svg-icon {
+    height: 20px;
+    width: 20px;
+
+    svg {
+      height: 100%;
+      width: 100%;
+    }
+  }
+
+  .reference {
+    &.external:after {
+      content: url("data:image/svg+xml;charset=utf-8,%3Csvg width='16' height='16' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M11 7H6a2 2 0 0 0-2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2-2v-5M10 14 20 4M15 4h5v5'/%3E%3C/svg%3E");
+      margin-left: 0.3rem;
+      vertical-align: middle;
     }
   }
 }
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!doctype html>
 <html class="no-js {% if theme_fix_navbar %} has-navbar-fixed-top {% endif %}" {% if language is not none %}
-    lang="{{ language }}" {% endif %}>
+    lang="{{ language }}" {% endif %} {% if default_mode %}data-theme="{{ default_mode }}" {% endif %}>
 {%- import "static/webpack-macros.html" as _webpack with context %}
 {%- import "partials/_icon_links_declare.html" as _icon_declare with context %}
 
 <head>
     {%- block site_meta -%}
     <meta charset="utf-8" />
     <meta name="keywords" content="python, sphinx, sphinx-theme, sphinx-doc, documentation" />
@@ -86,15 +86,15 @@
     {{ _webpack.head_js_preload() }}
     {%- endblock styles -%}
 
     {#- Custom front matter #}
     {%- block extrahead -%}{%- endblock extrahead -%}
 </head>
 
-<body>
+<body data-default-mode="{{ default_mode }}">
     {% block htmlbody %}
     {% endblock htmlbody %}
 
     {%- block scripts -%}
 
     {# Custom JS #}
     {%- block regular_scripts -%}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 
-% if language is not none %} lang="{{ language }}" {% endif %}> {%- import
-"static/webpack-macros.html" as _webpack with context %} {%- import "partials/
+% if language is not none %} lang="{{ language }}" {% endif %} {% if
+default_mode %}data-theme="{{ default_mode }}" {% endif %}> {%- import "static/
+webpack-macros.html" as _webpack with context %} {%- import "partials/
 _icon_links_declare.html" as _icon_declare with context %}
 {%- block site_meta -%}
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 {%- block breadcrumbs %}
 {#
 If we have more than 3 parents (excluding the home page) then we remove
 The ones in the middle and add an ellipsis.
 This code is from
 https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html
 #}
+
+{# djlint:off #}
 {% if parents|length>2 %}
-{% set parents=[parents[0], {"title": '<i class="fa-solid fa-ellipsis"></i>'}, parents[-1]] %}
+{% set parents=[parents[0], {"title": '&bull;&bull;&bull;'}, parents[-1]] %}
 {% endif %}
-
+{# djlint:on #}
 
 {#- Hide breadcrumbs on the home page #}
 {% if title and pagename != root_doc %}
 <nav class="breadcrumb" aria-label="breadcrumbs">
     <ul>
         <li><a href="{{ pathto(root_doc) }}"><svg xmlns="http://www.w3.org/2000/svg"
                     class="icon icon-tabler icon-tabler-home" width="44" height="44" viewBox="0 0 24 24"
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {%- block breadcrumbs %} {# If we have more than 3 parents (excluding the home
 page) then we remove The ones in the middle and add an ellipsis. This code is
 from https://github.com/pydata/pydata-sphinx-theme/blob/main/src/
-pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html #} {%
-if parents|length>2 %} {% set parents=[parents[0], {"title": ''}, parents[-1]]
-%} {% endif %} {#- Hide breadcrumbs on the home page #} {% if title and
-pagename != root_doc %}
+pydata_sphinx_theme/theme/pydata_sphinx_theme/components/breadcrumbs.html #} {#
+djlint:off #} {% if parents|length>2 %} {% set parents=[parents[0], {"title":
+'•••'}, parents[-1]] %} {% endif %} {# djlint:on #} {#- Hide breadcrumbs on the
+home page #} {% if title and pagename != root_doc %}
     * ___
     * {%- for doc in parents %} {% if doc.link %}
     * {{_doc.title_}}
     * {% else %}
     * {{_doc.title_}}
     * {% endif %} {%- endfor %}
     * {{ title }}
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/panel-test.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-<button class="button is-fullwidth search-button search-button__button level">
+<button class="button is-fullwidth search-button search-button__button level" title="{{ _('Search') }}"
+    aria-label="{{ _('Search') }}">
     <div class="level-left">
         <div class="level-item">
             <svg class="flex-none mr-1.5" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                 aria-hidden="true" focusable="false" role="img" width="1em" height="1em"
                 preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32">
                 <path d="M30 28.59L22.45 21A11 11 0 1 0 21 22.45L28.59 30zM5 14a9 9 0 1 1 9 9a9 9 0 0 1-9-9z"
                     fill="currentColor" />
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<button class="button is-inverted theme-switch-button">
+<button class="button is-inverted theme-switch-button" title="{{ _('light/dark') }}" aria-label="{{ _('light/dark') }}">
     <span class="theme-switch nav-link" data-mode="light">
         <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-sun" width="44" height="44"
             viewBox="0 0 24 24" stroke-width="1.5" stroke="#2c3e50" fill="none" stroke-linecap="round"
             stroke-linejoin="round">
             <path stroke="none" d="M0 0h24v24H0z" fill="none" />
             <path d="M12 12m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0" />
             <path d="M3 12h1m8 -9v1m8 8h1m-9 8v1m-6.4 -15.4l.7 .7m12.1 -.7l-.7 .7m0 11.4l.7 .7m-12.1 -.7l-.7 .7" />
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 maxdepth=theme_navigation_depth|int,
 collapse=theme_collapse_navigation|tobool,
 includehidden=True,
 titles_only=True)
 -%}
 
 {% block htmlbody -%}
+{% include "partials/icons.html" %}
 
 {% block docs_headnav %}
 {% if theme_have_top_navbar %}
 <nav class="navbar has-shadow {% if theme_fix_navbar %} is-fixed-top {% endif %} {% if theme_navbar_color_style %} {{ theme_navbar_color_style }} {% endif %}"
     role="navigation" aria-label="main navigation">
     {% include "sections/headnav.html" %}
 </nav>
@@ -54,15 +55,15 @@
 
                 {% set page_toc = generate_toc_html() %}
                 {%- if page_toc | length >= 1 %}
                 <aside class="column is-one-quarter bulma-tocnav is-hidden-mobile">
                     <div class="toc-wrapper toc-scroll">
                         {% if theme_toc_title %}
                         <div class="toc-title">
-                            <i class="fa-solid fa-list"></i> {{ theme_toc_title }}
+                            {{ theme_toc_title }}
                         </div>
                         {% endif %}
                         {{ page_toc }}
                     </div>
                 </aside>
                 {% endif %}
             </div>
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/toctree.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,22 @@
         # Add the "label" for the checkbox which will get filled.
         if soup.new_tag is None:
             continue
 
         label = soup.new_tag(
             "label", attrs={"for": checkbox_name, "class": "toctree-toggle"}
         )
-        label.append(soup.new_tag("i", attrs={"class": "fa-solid fa-chevron-down"}))
+        ##########################################################
+        retval = soup.new_tag("i", attrs={"class": "svg-icon"})
+        svg_element = soup.new_tag("svg")
+        svg_use_element = soup.new_tag("use", href="#svg-arrow-right")
+        svg_element.append(svg_use_element)
+        retval.append(svg_element)
+        ##########################################################
+        label.append(retval)
         if "toctree-l0" in classes:
             # making label cover the whole caption text with css
             label["class"] = "label-parts"
         element.insert(1, label)
 
         # Add the checkbox that's used to store expanded/collapsed state.
         checkbox = soup.new_tag(
```

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.5/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/webpack.config.js` & `bulma_sphinx_theme-0.0.5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.4/PKG-INFO` & `bulma_sphinx_theme-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.4
+Version: 0.0.5
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.4 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.5 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

