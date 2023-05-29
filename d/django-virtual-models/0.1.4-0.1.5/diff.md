# Comparing `tmp/django-virtual-models-0.1.4.tar.gz` & `tmp/django-virtual-models-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-virtual-models-0.1.4.tar", last modified: Fri Oct 28 21:28:37 2022, max compression
+gzip compressed data, was "django-virtual-models-0.1.5.tar", last modified: Mon May 29 19:31:39 2023, max compression
```

## Comparing `django-virtual-models-0.1.4.tar` & `django-virtual-models-0.1.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      200 2022-10-28 21:28:19.525946 django-virtual-models-0.1.4/.bumpversion.cfg
--rw-r--r--   0        0        0      503 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/.editorconfig
--rw-r--r--   0        0        0      165 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/.flake8
--rw-r--r--   0        0        0      234 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1841 2022-10-28 21:19:56.879549 django-virtual-models-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      978 2022-10-07 13:44:00.199208 django-virtual-models-0.1.4/.gitignore
--rw-r--r--   0        0        0     1353 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/AUTHORS.rst
--rw-r--r--   0        0        0      737 2022-10-28 21:26:41.118113 django-virtual-models-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     5498 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3078 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1106 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/LICENSE
--rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0     6773 2022-10-20 23:29:19.957112 django-virtual-models-0.1.4/README.md
--rw-r--r--   0        0        0      365 2022-10-28 21:28:19.525946 django-virtual-models-0.1.4/django_virtual_models/__init__.py
--rw-r--r--   0        0        0      348 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/exceptions.py
--rw-r--r--   0        0        0    12337 2022-10-20 22:59:22.312626 django-virtual-models-0.1.4/django_virtual_models/fields.py
--rw-r--r--   0        0        0     1878 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/generic_views.py
--rw-r--r--   0        0        0        0 2022-10-11 23:33:37.024666 django-virtual-models-0.1.4/django_virtual_models/prefetch/__init__.py
--rw-r--r--   0        0        0      123 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/prefetch/exceptions.py
--rw-r--r--   0        0        0     4260 2022-10-11 23:37:09.682064 django-virtual-models-0.1.4/django_virtual_models/prefetch/hints.py
--rw-r--r--   0        0        0    19443 2022-10-20 22:25:31.135032 django-virtual-models-0.1.4/django_virtual_models/prefetch/serializer_optimization.py
--rw-r--r--   0        0        0       21 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/query_capture/__init__.py
--rw-r--r--   0        0        0     4463 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/query_capture/capture.py
--rw-r--r--   0        0        0     6027 2022-10-07 14:23:37.970878 django-virtual-models-0.1.4/django_virtual_models/query_capture/utils.py
--rw-r--r--   0        0        0     3628 2022-10-07 14:23:37.974878 django-virtual-models-0.1.4/django_virtual_models/serializers.py
--rw-r--r--   0        0        0     2586 2022-10-07 14:23:37.974878 django-virtual-models-0.1.4/django_virtual_models/utils.py
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/LICENSE.md -> ../LICENSE
-lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/README.md -> ../README.md
--rw-r--r--   0        0        0     1992 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/img/4d-black.svg
--rw-r--r--   0        0        0     2656 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/img/4d-small.svg
--rw-r--r--   0        0        0     2004 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/img/4d-white.svg
--rw-r--r--   0        0        0     4286 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/docs/img/favicon.ico
--rw-r--r--   0        0        0      537 2022-10-07 18:25:46.429082 django-virtual-models-0.1.4/docs/installation.md
--rw-r--r--   0        0        0    24190 2022-10-20 23:07:33.598593 django-virtual-models-0.1.4/docs/tutorial.md
--rw-r--r--   0        0        0      732 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/README.md
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/example/__init__.py
--rw-r--r--   0        0        0     3149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/example/settings.py
--rw-r--r--   0        0        0      192 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/example/urls.py
--rw-r--r--   0        0        0      168 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/example/wsgi.py
--rwxr-xr-x   0        0        0      663 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/manage.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/__init__.py
--rw-r--r--   0        0        0      226 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/admin.py
--rw-r--r--   0        0        0      144 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/apps.py
--rw-r--r--   0        0        0     1574 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/fixtures/movies_initial.yaml
--rw-r--r--   0        0        0     2465 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/migrations/__init__.py
--rw-r--r--   0        0        0     1056 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/models.py
--rw-r--r--   0        0        0      796 2022-10-18 18:40:58.786984 django-virtual-models-0.1.4/example/movies/serializers.py
--rw-r--r--   0        0        0      149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/urls.py
--rw-r--r--   0        0        0      234 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/movies/views.py
--rw-r--r--   0        0        0      690 2022-10-20 23:06:37.427302 django-virtual-models-0.1.4/example/movies/virtual_models.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/tests/__init__.py
--rw-r--r--   0        0        0      865 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/tests/conftest.py
--rw-r--r--   0        0        0     2100 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/example/tests/test_views.py
--rw-r--r--   0        0        0      906 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/mkdocs.yml
--rwxr-xr-x   0        0        0     3679 2022-10-28 21:20:05.567500 django-virtual-models-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      773 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/optimization/__init__.py
--rw-r--r--   0        0        0    19025 2022-10-20 23:10:41.622610 django-virtual-models-0.1.4/tests/optimization/test_exceptions.py
--rw-r--r--   0        0        0    16704 2022-10-20 23:13:20.619211 django-virtual-models-0.1.4/tests/optimization/test_lookup_finder.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/query_capture/__init__.py
--rw-r--r--   0        0        0      896 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/query_capture/test_capture.py
--rw-r--r--   0        0        0      634 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/query_capture/test_utils.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/views/__init__.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/virtual_models/__init__.py
--rw-r--r--   0        0        0      591 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/virtual_models/db_utils.py
--rw-r--r--   0        0        0     7845 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/virtual_models/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.4/tests/virtual_models/migrations/__init__.py
--rw-r--r--   0        0        0     4626 2022-10-11 23:37:13.802015 django-virtual-models-0.1.4/tests/virtual_models/models.py
--rw-r--r--   0        0        0     3757 2022-10-20 23:14:21.424762 django-virtual-models-0.1.4/tests/virtual_models/test_exceptions.py
--rw-r--r--   0        0        0      847 2022-10-07 13:42:04.430893 django-virtual-models-0.1.4/tests/virtual_models/test_utils.py
--rw-r--r--   0        0        0    17310 2022-10-20 23:10:23.647569 django-virtual-models-0.1.4/tests/virtual_models/test_virtual_models.py
--rw-r--r--   0        0        0     8763 1970-01-01 00:00:00.000000 django-virtual-models-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      503 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.editorconfig
+-rw-r--r--   0        0        0      165 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.flake8
+-rw-r--r--   0        0        0      234 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1848 2023-05-29 18:52:15.951093 django-virtual-models-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      978 2022-10-07 13:44:00.199208 django-virtual-models-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1352 2023-05-29 19:02:03.370944 django-virtual-models-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/AUTHORS.rst
+-rw-r--r--   0        0        0      812 2023-05-29 19:24:01.679040 django-virtual-models-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     5498 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3078 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1106 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/LICENSE
+-rw-r--r--   0        0        0      287 2022-10-07 13:42:04.422893 django-virtual-models-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0     6773 2022-10-20 23:29:19.957112 django-virtual-models-0.1.5/README.md
+-rw-r--r--   0        0        0      365 2023-05-29 19:30:51.461765 django-virtual-models-0.1.5/django_virtual_models/__init__.py
+-rw-r--r--   0        0        0      348 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/exceptions.py
+-rw-r--r--   0        0        0    12337 2022-10-20 22:59:22.312626 django-virtual-models-0.1.5/django_virtual_models/fields.py
+-rw-r--r--   0        0        0     1878 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/generic_views.py
+-rw-r--r--   0        0        0        0 2022-10-11 23:33:37.024666 django-virtual-models-0.1.5/django_virtual_models/prefetch/__init__.py
+-rw-r--r--   0        0        0      123 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/prefetch/exceptions.py
+-rw-r--r--   0        0        0     4260 2022-10-11 23:37:09.682064 django-virtual-models-0.1.5/django_virtual_models/prefetch/hints.py
+-rw-r--r--   0        0        0    19443 2022-10-20 22:25:31.135032 django-virtual-models-0.1.5/django_virtual_models/prefetch/serializer_optimization.py
+-rw-r--r--   0        0        0       21 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/__init__.py
+-rw-r--r--   0        0        0     4463 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/capture.py
+-rw-r--r--   0        0        0     6027 2022-10-07 14:23:37.970878 django-virtual-models-0.1.5/django_virtual_models/query_capture/utils.py
+-rw-r--r--   0        0        0     3628 2022-10-07 14:23:37.974878 django-virtual-models-0.1.5/django_virtual_models/serializers.py
+-rw-r--r--   0        0        0     2586 2022-10-07 14:23:37.974878 django-virtual-models-0.1.5/django_virtual_models/utils.py
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/LICENSE.md -> ../LICENSE
+lrwxr-xr-x   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/README.md -> ../README.md
+-rw-r--r--   0        0        0     1992 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-black.svg
+-rw-r--r--   0        0        0     2656 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-small.svg
+-rw-r--r--   0        0        0     2004 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/4d-white.svg
+-rw-r--r--   0        0        0     4286 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/docs/img/favicon.ico
+-rw-r--r--   0        0        0      537 2022-10-07 18:25:46.429082 django-virtual-models-0.1.5/docs/installation.md
+-rw-r--r--   0        0        0    24190 2022-10-20 23:07:33.598593 django-virtual-models-0.1.5/docs/tutorial.md
+-rw-r--r--   0        0        0      732 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/README.md
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/__init__.py
+-rw-r--r--   0        0        0     3149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/settings.py
+-rw-r--r--   0        0        0      192 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/urls.py
+-rw-r--r--   0        0        0      168 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/example/wsgi.py
+-rwxr-xr-x   0        0        0      663 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/manage.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/__init__.py
+-rw-r--r--   0        0        0      226 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/admin.py
+-rw-r--r--   0        0        0      144 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/apps.py
+-rw-r--r--   0        0        0     1574 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/fixtures/movies_initial.yaml
+-rw-r--r--   0        0        0     2465 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/migrations/__init__.py
+-rw-r--r--   0        0        0     1056 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/models.py
+-rw-r--r--   0        0        0      796 2022-10-18 18:40:58.786984 django-virtual-models-0.1.5/example/movies/serializers.py
+-rw-r--r--   0        0        0      149 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/urls.py
+-rw-r--r--   0        0        0      234 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/movies/views.py
+-rw-r--r--   0        0        0      690 2022-10-20 23:06:37.427302 django-virtual-models-0.1.5/example/movies/virtual_models.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/__init__.py
+-rw-r--r--   0        0        0      865 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/conftest.py
+-rw-r--r--   0        0        0     2100 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/example/tests/test_views.py
+-rw-r--r--   0        0        0      906 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/mkdocs.yml
+-rwxr-xr-x   0        0        0     3698 2023-05-29 19:30:21.230066 django-virtual-models-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      773 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/optimization/__init__.py
+-rw-r--r--   0        0        0    19025 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/optimization/test_exceptions.py
+-rw-r--r--   0        0        0    16704 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/optimization/test_lookup_finder.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/__init__.py
+-rw-r--r--   0        0        0      896 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/test_capture.py
+-rw-r--r--   0        0        0      634 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/query_capture/test_utils.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/views/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-15 19:48:28.523655 django-virtual-models-0.1.5/tests/virtual_models/db_utils.py
+-rw-r--r--   0        0        0     7845 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-10-07 13:42:04.426893 django-virtual-models-0.1.5/tests/virtual_models/migrations/__init__.py
+-rw-r--r--   0        0        0     4626 2022-11-09 14:10:13.043069 django-virtual-models-0.1.5/tests/virtual_models/models.py
+-rw-r--r--   0        0        0     3436 2023-05-15 19:48:28.523655 django-virtual-models-0.1.5/tests/virtual_models/test_db_utils.py
+-rw-r--r--   0        0        0     3757 2022-10-20 23:14:21.424762 django-virtual-models-0.1.5/tests/virtual_models/test_exceptions.py
+-rw-r--r--   0        0        0      847 2022-10-07 13:42:04.430893 django-virtual-models-0.1.5/tests/virtual_models/test_utils.py
+-rw-r--r--   0        0        0    17310 2022-10-20 23:10:23.647569 django-virtual-models-0.1.5/tests/virtual_models/test_virtual_models.py
+-rw-r--r--   0        0        0     8710 1970-01-01 00:00:00.000000 django-virtual-models-0.1.5/PKG-INFO
```

### Comparing `django-virtual-models-0.1.4/.github/workflows/tests.yml` & `django-virtual-models-0.1.5/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   test:
     timeout-minutes: 10
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest]
         python-version: ['3.8', '3.9', '3.10', '3.11']
-        django-version: ['3.2', '4.0', '4.1']
+        django-version: ['3.2', '4.0', '4.1', '4.2']
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `django-virtual-models-0.1.4/.gitignore` & `django-virtual-models-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/.pre-commit-config.yaml` & `django-virtual-models-0.1.5/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
       - id: check-added-large-files
@@ -12,40 +12,40 @@
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: debug-statements
       - id: detect-private-key
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.0
+    rev: v3.4.0
     hooks:
     - id: pyupgrade
       args:
         - --py3-plus
         - --keep-runtime-typing
   - repo: https://github.com/myint/autoflake
-    rev: v1.5.3
+    rev: v2.1.1
     hooks:
     - id: autoflake
       args:
         - --recursive
         - --in-place
         - --remove-all-unused-imports
         - --remove-duplicate-keys
         - --exclude
         - __init__.py,migrations/*
   - repo: https://github.com/pycqa/isort
-    rev: "5.10.1"
+    rev: "5.12.0"
     hooks:
       - id: isort
         name: isort (python)
   - repo: https://github.com/psf/black
-    rev: "22.8.0"
+    rev: "23.3.0"
     hooks:
       - id: black
         exclude: ^.*\b(migrations)\b.*$
   - repo: https://github.com/PyCQA/bandit
-    rev: "1.7.4"
+    rev: "1.7.5"
     hooks:
       - id: bandit
         args: ["-c", "pyproject.toml"]
         additional_dependencies: [ "bandit[toml]" ]
```

### Comparing `django-virtual-models-0.1.4/CHANGELOG.md` & `django-virtual-models-0.1.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.5]
+
+- More robust `is_preloaded` check
+- Add Django 4.2 to tests.
+
 ## [0.1.4]
 
 - Add Python 3.11 to tests.
 
 ## [0.1.3]
 
 - README update.
```

### Comparing `django-virtual-models-0.1.4/CODE_OF_CONDUCT.md` & `django-virtual-models-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/CONTRIBUTING.rst` & `django-virtual-models-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/LICENSE` & `django-virtual-models-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/README.md` & `django-virtual-models-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/fields.py` & `django-virtual-models-0.1.5/django_virtual_models/fields.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/generic_views.py` & `django-virtual-models-0.1.5/django_virtual_models/generic_views.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/prefetch/hints.py` & `django-virtual-models-0.1.5/django_virtual_models/prefetch/hints.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/prefetch/serializer_optimization.py` & `django-virtual-models-0.1.5/django_virtual_models/prefetch/serializer_optimization.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/query_capture/capture.py` & `django-virtual-models-0.1.5/django_virtual_models/query_capture/capture.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/query_capture/utils.py` & `django-virtual-models-0.1.5/django_virtual_models/query_capture/utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/serializers.py` & `django-virtual-models-0.1.5/django_virtual_models/serializers.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/django_virtual_models/utils.py` & `django-virtual-models-0.1.5/django_virtual_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/img/4d-black.svg` & `django-virtual-models-0.1.5/docs/img/4d-black.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/img/4d-small.svg` & `django-virtual-models-0.1.5/docs/img/4d-small.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/img/4d-white.svg` & `django-virtual-models-0.1.5/docs/img/4d-white.svg`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/img/favicon.ico` & `django-virtual-models-0.1.5/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/installation.md` & `django-virtual-models-0.1.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/docs/tutorial.md` & `django-virtual-models-0.1.5/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/README.md` & `django-virtual-models-0.1.5/example/README.md`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/example/settings.py` & `django-virtual-models-0.1.5/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/manage.py` & `django-virtual-models-0.1.5/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/movies/fixtures/movies_initial.yaml` & `django-virtual-models-0.1.5/example/movies/fixtures/movies_initial.yaml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/movies/migrations/0001_initial.py` & `django-virtual-models-0.1.5/example/movies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/movies/models.py` & `django-virtual-models-0.1.5/example/movies/models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/movies/serializers.py` & `django-virtual-models-0.1.5/example/movies/serializers.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/movies/virtual_models.py` & `django-virtual-models-0.1.5/example/movies/virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/tests/conftest.py` & `django-virtual-models-0.1.5/example/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/example/tests/test_views.py` & `django-virtual-models-0.1.5/example/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/mkdocs.yml` & `django-virtual-models-0.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/pyproject.toml` & `django-virtual-models-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,28 +38,27 @@
 Documentation = "https://vintasoftware.github.io/django-virtual-models/"
 
 [project.optional-dependencies]
 doc = [
     "mkdocs-material==8.5.6",
 ]
 dev = [
-    "mypy ==0.971",
-    "autoflake >=1.5.3,<2.0.0",
-    "flake8 >=5.0.4,<6.0.0",
-    "black ==22.8.0",
-    "isort >=5.10.1,<6.0.0",
-    "pre-commit >=2.20.0,<3.0.0",
-    "bump2version ==1.0.1",
+    "mypy ==1.3.0 ",
+    "autoflake >=2.1.1,<3.0.0",
+    "flake8 >=6.0.0,<7.0.0",
+    "black ==23.3.0",
+    "isort >=5.12.0,<6.0.0",
+    "pre-commit >=3.3.2,<4.0.0",
 ]
 test = [
-    "pytest >=7.1.3,<8.0.0",
-    "pytest-cov[toml] >=3.0.0,<4.0.0",
+    "pytest >=7.3.1,<8.0.0",
+    "pytest-cov[toml] >=4.1.0,<5.0.0",
     "pytest-django >=4.5.2,<5.0.0",
-    "tox >=3.26.0,<4.0.0",
-    "model_bakery >=1.7.0,<2.0.0",
+    "tox >=4.5.2,<5.0.0",
+    "model_bakery >=1.11.0,<2.0.0",
 ]
 example = [
     "django >= 3.2,<4.0",
     "pyyaml >= 6.0,<7.0",
 ]
 
 [tool.black]
@@ -109,15 +108,15 @@
 # filterwarnings = [
 #     "ignore::django.utils.deprecation.RemovedInDjango50Warning",
 # ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = {linux}-py{38,39,310,311}-django{32,40,41}
+envlist = {linux}-py{38,39,310,311}-django{32,40,41,42}
 isolated_build = True
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
@@ -126,20 +125,22 @@
 [gh-actions:env]
 OS =
     ubuntu-latest: linux
 DJANGO =
     3.2: django32
     4.0: django40
     4.1: django41
+    4.2: django42
 
 [testenv]
 deps =
     django32: django~=3.2
     django40: django~=4.0
     django41: django~=4.1
+    django42: django~=4.2
     .[test]
 commands =
     coverage run -m pytest --basetemp={envtmpdir}
     coverage xml
 """
 
 [tool.coverage.run]
```

### Comparing `django-virtual-models-0.1.4/tests/conftest.py` & `django-virtual-models-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/optimization/test_exceptions.py` & `django-virtual-models-0.1.5/tests/optimization/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/optimization/test_lookup_finder.py` & `django-virtual-models-0.1.5/tests/optimization/test_lookup_finder.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/query_capture/test_capture.py` & `django-virtual-models-0.1.5/tests/query_capture/test_capture.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/query_capture/test_utils.py` & `django-virtual-models-0.1.5/tests/query_capture/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/virtual_models/migrations/0001_initial.py` & `django-virtual-models-0.1.5/tests/virtual_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/virtual_models/models.py` & `django-virtual-models-0.1.5/tests/virtual_models/models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/virtual_models/test_exceptions.py` & `django-virtual-models-0.1.5/tests/virtual_models/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/virtual_models/test_utils.py` & `django-virtual-models-0.1.5/tests/virtual_models/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/tests/virtual_models/test_virtual_models.py` & `django-virtual-models-0.1.5/tests/virtual_models/test_virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-virtual-models-0.1.4/PKG-INFO` & `django-virtual-models-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-virtual-models
-Version: 0.1.4
+Version: 0.1.5
 Summary: Improve performance and maintainability with a prefetching layer in your Django / Django REST Framework project
 Keywords: django,prefetch,performance,optimization
 Author-email: "Flávio Juvenal (Vinta Software)" <flavio@vinta.com.br>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,29 +14,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django >=3.2
 Requires-Dist: djangorestframework >=3.13.1
 Requires-Dist: typing-extensions >=4.3.0
-Requires-Dist: mypy ==0.971 ; extra == "dev"
-Requires-Dist: autoflake >=1.5.3,<2.0.0 ; extra == "dev"
-Requires-Dist: flake8 >=5.0.4,<6.0.0 ; extra == "dev"
-Requires-Dist: black ==22.8.0 ; extra == "dev"
-Requires-Dist: isort >=5.10.1,<6.0.0 ; extra == "dev"
-Requires-Dist: pre-commit >=2.20.0,<3.0.0 ; extra == "dev"
-Requires-Dist: bump2version ==1.0.1 ; extra == "dev"
+Requires-Dist: mypy ==1.3.0  ; extra == "dev"
+Requires-Dist: autoflake >=2.1.1,<3.0.0 ; extra == "dev"
+Requires-Dist: flake8 >=6.0.0,<7.0.0 ; extra == "dev"
+Requires-Dist: black ==23.3.0 ; extra == "dev"
+Requires-Dist: isort >=5.12.0,<6.0.0 ; extra == "dev"
+Requires-Dist: pre-commit >=3.3.2,<4.0.0 ; extra == "dev"
 Requires-Dist: mkdocs-material==8.5.6 ; extra == "doc"
 Requires-Dist: django >= 3.2,<4.0 ; extra == "example"
 Requires-Dist: pyyaml >= 6.0,<7.0 ; extra == "example"
-Requires-Dist: pytest >=7.1.3,<8.0.0 ; extra == "test"
-Requires-Dist: pytest-cov[toml] >=3.0.0,<4.0.0 ; extra == "test"
+Requires-Dist: pytest >=7.3.1,<8.0.0 ; extra == "test"
+Requires-Dist: pytest-cov[toml] >=4.1.0,<5.0.0 ; extra == "test"
 Requires-Dist: pytest-django >=4.5.2,<5.0.0 ; extra == "test"
-Requires-Dist: tox >=3.26.0,<4.0.0 ; extra == "test"
-Requires-Dist: model_bakery >=1.7.0,<2.0.0 ; extra == "test"
+Requires-Dist: tox >=4.5.2,<5.0.0 ; extra == "test"
+Requires-Dist: model_bakery >=1.11.0,<2.0.0 ; extra == "test"
 Project-URL: Documentation, https://vintasoftware.github.io/django-virtual-models/
 Project-URL: Homepage, https://github.com/vintasoftware/django-virtual-models
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: example
 Provides-Extra: test
```

