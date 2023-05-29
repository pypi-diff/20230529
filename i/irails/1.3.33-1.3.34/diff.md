# Comparing `tmp/irails-1.3.33.tar.gz` & `tmp/irails-1.3.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.33.tar", last modified: Sun May 28 15:30:25 2023, max compression
+gzip compressed data, was "irails-1.3.34.tar", last modified: Mon May 29 12:31:05 2023, max compression
```

## Comparing `irails-1.3.33.tar` & `irails-1.3.34.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.659110 irails-1.3.33/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.33/MANIFEST.in
--rw-rw-rw-   0        0        0     4956 2023-05-28 15:30:25.659110 irails-1.3.33/PKG-INFO
--rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.33/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.560706 irails-1.3.33/irails/
--rw-rw-rw-   0        0        0      307 2023-05-28 15:29:45.000000 irails-1.3.33/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.33/irails/_i18n.py
--rw-rw-rw-   0        0        0     4199 2023-05-27 15:17:05.000000 irails-1.3.33/irails/_loader.py
--rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.33/irails/_utils.py
--rw-rw-rw-   0        0        0    15330 2023-05-28 15:25:34.000000 irails-1.3.33/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.33/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.570680 irails-1.3.33/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.572675 irails-1.3.33/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.33/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.33/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.33/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.33/irails/controller_utils.py
--rw-rw-rw-   0        0        0    26026 2023-05-27 10:48:38.000000 irails-1.3.33/irails/core.py
--rw-rw-rw-   0        0        0    20962 2023-05-28 14:25:03.000000 irails-1.3.33/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.33/irails/log.py
--rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.33/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.33/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.33/irails/midware_session.py
--rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.33/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.585144 irails-1.3.33/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.33/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.33/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.33/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.33/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.33/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.33/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.33/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.33/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.33/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.33/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.33/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.524657 irails-1.3.33/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.596794 irails-1.3.33/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.33/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.33/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.33/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.33/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.33/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.33/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.33/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.33/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.33/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.599795 irails-1.3.33/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.33/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.601780 irails-1.3.33/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.33/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.611680 irails-1.3.33/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.33/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.33/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.33/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.626640 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      319 2023-05-28 15:30:10.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.33/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.33/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.33/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.33/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.528485 irails-1.3.33/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.630629 irails-1.3.33/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.33/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.635451 irails-1.3.33/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.33/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.33/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.638449 irails-1.3.33/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.533215 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.644964 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.652555 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.534212 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.654854 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.33/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.33/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.568685 irails-1.3.33/irails.egg-info/
--rw-rw-rw-   0        0        0     4956 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 15:30:25.660121 irails-1.3.33/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.33/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.759971 irails-1.3.34/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.34/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-05-29 12:31:05.758976 irails-1.3.34/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.34/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.608878 irails-1.3.34/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-29 12:26:25.000000 irails-1.3.34/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.34/irails/_i18n.py
+-rw-rw-rw-   0        0        0     4358 2023-05-29 06:44:16.000000 irails-1.3.34/irails/_loader.py
+-rw-rw-rw-   0        0        0     5605 2023-05-29 06:19:25.000000 irails-1.3.34/irails/_utils.py
+-rw-rw-rw-   0        0        0    15325 2023-05-29 12:21:14.000000 irails-1.3.34/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.34/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.616382 irails-1.3.34/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.619374 irails-1.3.34/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9307 2023-05-29 06:35:41.000000 irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10617 2023-05-29 06:35:35.000000 irails-1.3.34/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.34/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.34/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.34/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    26096 2023-05-29 06:20:04.000000 irails-1.3.34/irails/core.py
+-rw-rw-rw-   0        0        0    20962 2023-05-29 08:27:47.000000 irails-1.3.34/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.34/irails/log.py
+-rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.34/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.34/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.34/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.34/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.632426 irails-1.3.34/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.34/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.34/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.34/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.34/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.34/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.34/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.34/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.34/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.34/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.34/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.34/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.578959 irails-1.3.34/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.645392 irails-1.3.34/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.34/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.34/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.34/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.34/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.34/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.34/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.34/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.34/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.34/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.656364 irails-1.3.34/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.34/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.658358 irails-1.3.34/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.34/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.704235 irails-1.3.34/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.34/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.34/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.34/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.726177 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.34/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.34/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.34/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.34/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.581950 irails-1.3.34/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.730165 irails-1.3.34/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.34/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.733492 irails-1.3.34/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.34/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.34/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.736498 irails-1.3.34/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.583946 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.744758 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.750492 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.584942 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.753627 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.34/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.34/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.615382 irails-1.3.34/irails.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 12:31:05.759971 irails-1.3.34/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.34/setup.py
```

### Comparing `irails-1.3.33/PKG-INFO` & `irails-1.3.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.33
+Version: 1.3.34
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.33/README.md` & `irails-1.3.34/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/_i18n.py` & `irails-1.3.34/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/_loader.py` & `irails-1.3.34/irails/_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,19 +43,23 @@
 
 def __check_if_enabled(app_name):
     return (app_enabled == "*" or 
             not app_enabled or 
             (isinstance(app_enabled,list) and app_name in app_enabled))
 
 def load_module(module_name:str,module_path:str):
-    if os.path.exists(module_path):
+    if os.path.exists(module_path) and not module_name in sys.modules:
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
+
         spec.loader.exec_module(module)
+        sys.modules[module_name] = module
         return module
+    elif module_name in sys.modules:
+        return sys.modules[module_name]
     return None
 def _load_app(app_dir,manifest:dict): 
     if not manifest:
         return 0
     from .log import _log
     _modules = manifest['packages'] # ['controllers','services','models']
     cnt =  0
```

### Comparing `irails-1.3.33/irails/_utils.py` & `irails-1.3.34/irails/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,17 @@
         _pluralizer = inflect.engine()
     referred_name = referred_cls.__name__
     uncamelized = re.sub(r'[A-Z]',
                          lambda m: "_%s" % m.group(0).lower(),
                          referred_name)[1:]
     pluralized = _pluralizer.plural(uncamelized)
     return pluralized
-def copy_attr(obj1:object, obj2:object,copy_none:bool=True):
+async def copy_attr(obj1:object, obj2:object,copy_none:bool=True):
     """
         将obj1的属性复制到obj2（如果obj2有相同的属性）。
     """
     for key, value in obj1.__dict__.items():
         if hasattr(obj2, key):
             if copy_none or value:
-                setattr(obj2, key, value)
+                    setattr(obj2, key, value)
```

### Comparing `irails-1.3.33/irails/auth.py` & `irails-1.3.34/irails/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 from typing import List, Optional, Tuple, Type, Union, Dict
 from ._utils import iJSONEncoder, is_datetime_format
 from ._i18n import _
 AUTH_EXPIRED = '[EXPIRED]!'
 _session_name: str = ""
 default_domain = "system"
 
+cfg = config.get("auth")
+super_domain = cfg.get('super_domain','system')
+super_group = cfg.get('super_group','admin')
+_gEnforor:Enforcer = None
+def is_super(username,domain,*args,**kwargs): 
+    roles =_gEnforor.get_roles_for_user_in_domain(username,super_domain)
+    super_users =  _gEnforor.get_users_for_role_in_domain(super_group,super_domain)#['root', 'bruce']
+    # p = _gEnforor.get_permissions_for_user_in_domain(username,domain)
+    return super_group in roles and username in super_users
 
 class DomainUser(BaseUser):
     def __init__(self, username: str = 'anonymous', roles = [], domain: str = "") -> None:
         '''
         :group Roles 
         :domain Tenant
         '''
@@ -38,16 +47,15 @@
         self._timezone = 'Asia/Shanghai'
         super().__init__()
 
     @property
     def roles(self):
         return self._roles
 
-    @roles.setter
-    def roles(self, value:List):
+    def set_roles(self, value:List):
         names=[]
         for row in value:
             names.append(row.name)
         self._roles = names
 
     @property
     def domain(self):
@@ -69,15 +77,15 @@
 
     @property
     def identity(self) -> str:
         identity = self.username
         if self._roles:
             group = self._roles
             if self._domain:
-                group = self._domain+"."+group
+                group = self._domain+"."+ ','.join(group)
             identity += '@'+group
         return identity
 
     def __repr__(self):
         return self.identity
 
 
@@ -135,20 +143,20 @@
 
     def _auth(self, request: Request, user: DomainUser):
         '''
         do verity,return True means `Success` and others `Failed`
         '''
         if not user.roles:
             raise RuntimeError(_("User must have a role %s") % user)
-        sub = ','.join(user.roles)
-        path = request.url.path
-        method = request.method
-        param: Tuple = (sub, user.domain, path, method,)
+        sub = user.username  
+        dom = user.domain  
+        obj = request.url.path
+        act = request.method 
 
-        return self.enforcer.enforce(*param)
+        return self.enforcer.enforce(sub, dom, obj, act)
 
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
         """Parses the Authorization header and returns only the token"""
         try:
             scheme, token = authorization.split()
         except ValueError as e:
             raise AuthenticationError(
@@ -163,21 +171,24 @@
         payload = None
         username = ''
 
         if is_jwt:
             username_field = kwargs['username_field']
             auth = request.headers["Authorization"] if 'Authorization' in request.headers else None
             if auth:
-                scheme, credentials = auth.split()
-                token = self.__get_token_from_header(
-                    authorization=auth, prefix=prefix)
-
-                del kwargs['username_field']
+                scheme, credentials = auth.split(' ')
                 try:
+                    token = self.__get_token_from_header(
+                        authorization=auth, prefix=prefix)
+
+                    del kwargs['username_field']
+                
                     payload = jwt.decode(token, **kwargs)
+                except  AuthenticationError as e:
+                    return "", "", None
                 except jwt.InvalidTokenError as e:
                     msg = _('token %s has been expired(%s)' % (token, e.args))
                     _log.debug(msg)
                     request.session[self.__session_name] = None
                     return "", "", None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
@@ -347,18 +358,16 @@
 
 
 def init(app: FastAPI, backend: AuthenticationBackend, adapter_class: Type = None, **kwagrs) -> AuthenticationBackend:
     """
         kwargs:secret_key=KEY
     """
     __session_name = config.get("auth").get("session_name", 'user')
-    global _casbin_auth
-    cfg = config.get("auth")
-    super_domain = cfg.get('super_domain','system')
-    super_group = cfg.get('super_group','admin')
+    global _casbin_auth,_gEnforor
+    
 
     adapter_uri = kwagrs.get('adapter_uri', None)
 
     del kwagrs['adapter_uri']
     model_file = cfg.get("auth_model", './configs/casbin-model.conf')
     if not os.path.isabs(model_file):
         model_file = os.path.abspath(os.path.join(ROOT_PATH, model_file))
@@ -371,33 +380,22 @@
     from casbin.model import Model
     model = Model()
     with open(model_file,'r',encoding='utf-8') as f: 
         model_content = f.read()
         # if super_user and super_group:
         #     model_content = model_content.replace("${super_user}",super_user).replace("${super_group}",super_group)
         model.load_model_from_text(model_content)
-    enforcer = casbin.Enforcer(model, adapter)
-
-    def is_super(roles,domain): 
-        return super_group in roles and domain == super_domain
-    
+    enforcer = casbin.Enforcer(model, adapter) 
     enforcer.add_function('is_super',is_super)
+    _gEnforor=enforcer
     _casbin_auth = CasbinAuth(enforcer=enforcer, session_name=__session_name)
 
     return backend(**kwagrs)
 
-
-def reload_adapter(app: FastAPI, adapter: Adapter = None):
-    cfg = config.get("auth")
-    model_file = cfg.get("auth_model", './configs/casbin-model.conf')
-    if not adapter:
-        adapter_file = cfg.get("auth_adapter", './configs/casbin-adapter.csv')
-        adapter = FileAdapter(adapter_file)
-    enforcer = casbin.Enforcer(model_file, adapter)
-    app.router.current_casbin_instance = enforcer
+ 
 
 
 def get_auth_backend(name: str) -> AuthenticationBackend_:
     _auth_types = {'basic': BasicAuth, 'jwt': JWTAuthenticationBackend}
     return _auth_types[name] if name in _auth_types else None
```

### Comparing `irails-1.3.33/irails/base_controller.py` & `irails-1.3.34/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 05:11:49 2023 UTC, .py size: 10591 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 15ee 6e64 5f29 0000  o.........nd_)..
+00000000: 6f0d 0d0a 0000 0000 b747 7464 7929 0000  o........Gtdy)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c06 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -23,559 +23,560 @@
 00000160: da03 6f72 5f29 01da 1064 6563 6c61 7261  ..or_)...declara
 00000170: 7469 7665 5f62 6173 6529 01da 0c73 6573  tive_base)...ses
 00000180: 7369 6f6e 6d61 6b65 7229 01da 0864 6174  sionmaker)...dat
 00000190: 6162 6173 6529 01da 0663 6f6e 6669 675a  abase)...configZ
 000001a0: 0b63 6173 6269 6e5f 7275 6c65 da04 6175  .casbin_rule..au
 000001b0: 7468 5a0d 6164 6170 7465 725f 7461 626c  thZ.adapter_tabl
 000001c0: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
-000001d0: 0000 0400 0000 4000 0000 7384 0000 0065  ......@...s....e
-000001e0: 005a 0164 005a 0265 035a 0464 015a 0565  .Z.d.Z.e.Z.d.Z.e
-000001f0: 0665 0764 0164 028d 025a 0865 0665 0964  .e.d.d...Z.e.e.d
-00000200: 0383 0183 015a 0a65 0665 0964 0383 0183  .....Z.e.e.d....
-00000210: 015a 0b65 0665 0964 0383 0183 015a 0c65  .Z.e.e.d.....Z.e
-00000220: 0665 0964 0383 0183 015a 0d65 0665 0964  .e.d.....Z.e.e.d
-00000230: 0383 0183 015a 0e65 0665 0964 0383 0183  .....Z.e.e.d....
-00000240: 015a 0f65 0665 0964 0383 0183 015a 1064  .Z.e.e.d.....Z.d
-00000250: 0464 0584 005a 1164 0664 0784 005a 1264  .d...Z.d.d...Z.d
-00000260: 0853 0029 09da 0a43 6173 6269 6e52 756c  .S.)...CasbinRul
-00000270: 6554 2901 da0b 7072 696d 6172 795f 6b65  eT)...primary_ke
-00000280: 79e9 ff00 0000 6301 0000 0000 0000 0000  y.....c.........
-00000290: 0000 0003 0000 0006 0000 0043 0000 0073  ...........C...s
-000002a0: 4a00 0000 7c00 6a00 6701 7d01 7c00 6a01  J...|.j.g.}.|.j.
-000002b0: 7c00 6a02 7c00 6a03 7c00 6a04 7c00 6a05  |.j.|.j.|.j.|.j.
-000002c0: 7c00 6a06 6606 4400 5d0d 7d02 7c02 6400  |.j.f.D.].}.|.d.
-000002d0: 7500 721a 0100 6e06 7c01 a007 7c02 a101  u.r...n.|...|...
-000002e0: 0100 7112 6401 a008 7c01 a101 5300 2902  ..q.d...|...S.).
-000002f0: 4e7a 022c 2029 09da 0570 7479 7065 da02  Nz., )...ptype..
-00000300: 7630 da02 7631 da02 7632 da02 7633 da02  v0..v1..v2..v3..
-00000310: 7634 da02 7635 da06 6170 7065 6e64 da04  v4..v5..append..
-00000320: 6a6f 696e 2903 da04 7365 6c66 da03 6172  join)...self..ar
-00000330: 72da 0176 a900 721e 0000 00fa 3f45 3a5c  r..v..r.....?E:\
-00000340: 636f 6465 6465 6d6f 5c49 5241 494c 535c  codedemo\IRAILS\
-00000350: 6972 6169 6c73 5c63 6173 6269 6e5f 6164  irails\casbin_ad
-00000360: 6170 7465 7273 5c73 716c 616c 6368 656d  apters\sqlalchem
-00000370: 795f 6164 6170 7465 722e 7079 da07 5f5f  y_adapter.py..__
-00000380: 7374 725f 5f1e 0000 0073 0c00 0000 0801  str__....s......
-00000390: 2001 0801 0401 0c01 0a01 7a12 4361 7362   .........z.Casb
-000003a0: 696e 5275 6c65 2e5f 5f73 7472 5f5f 6301  inRule.__str__c.
-000003b0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-000003c0: 0000 0043 0000 0073 1200 0000 6401 a000  ...C...s....d...
-000003d0: 7c00 6a01 7402 7c00 8301 a102 5300 2902  |.j.t.|.....S.).
-000003e0: 4e7a 153c 4361 7362 696e 5275 6c65 207b  Nz.<CasbinRule {
-000003f0: 7d3a 2022 7b7d 223e 2903 da06 666f 726d  }: "{}">)...form
-00000400: 6174 da02 6964 da03 7374 72a9 0172 1b00  at..id..str..r..
-00000410: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000420: 00da 085f 5f72 6570 725f 5f26 0000 0073  ...__repr__&...s
-00000430: 0200 0000 1201 7a13 4361 7362 696e 5275  ......z.CasbinRu
-00000440: 6c65 2e5f 5f72 6570 725f 5f4e 2913 da08  le.__repr__N)...
-00000450: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000460: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000470: 5f5f da0a 7275 6c65 5f74 6162 6c65 da0d  __..rule_table..
-00000480: 5f5f 7461 626c 656e 616d 655f 5fda 0a5f  __tablename__.._
-00000490: 5f73 7973 7465 6d5f 5f72 0500 0000 7206  _system__r....r.
-000004a0: 0000 0072 2200 0000 7207 0000 0072 1200  ...r"...r....r..
-000004b0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000004c0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000004d0: 7220 0000 0072 2500 0000 721e 0000 0072  r ...r%...r....r
-000004e0: 1e00 0000 721e 0000 0072 1f00 0000 720f  ....r....r....r.
-000004f0: 0000 0012 0000 0073 1a00 0000 0800 0401  .......s........
-00000500: 0401 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000510: 0c01 0802 0c08 720f 0000 0063 0000 0000  ......r....c....
-00000520: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00000530: 4000 0000 7328 0000 0065 005a 0164 005a  @...s(...e.Z.d.Z
-00000540: 0267 005a 0367 005a 0467 005a 0567 005a  .g.Z.g.Z.g.Z.g.Z
-00000550: 0667 005a 0767 005a 0867 005a 0964 0153  .g.Z.g.Z.g.Z.d.S
-00000560: 0029 02da 0646 696c 7465 724e 290a 7226  .)...FilterN).r&
-00000570: 0000 0072 2700 0000 7228 0000 0072 1200  ...r'...r(...r..
-00000580: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000590: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000005a0: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-000005b0: 1f00 0000 722c 0000 002a 0000 0073 1000  ....r,...*...s..
-000005c0: 0000 0800 0401 0401 0401 0401 0401 0401  ................
-000005d0: 0801 722c 0000 0063 0000 0000 0000 0000  ..r,...c........
-000005e0: 0000 0000 0000 0000 0a00 0000 4000 0000  ............@...
-000005f0: 7310 0100 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000600: 0364 2d64 0464 0584 015a 0465 0564 0664  .d-d.d...Z.e.d.d
-00000610: 0784 0083 015a 0664 0864 0984 005a 0764  .....Z.d.d...Z.d
-00000620: 0a64 0b84 005a 0864 2e64 0d64 0e84 045a  .d...Z.d.d.d...Z
-00000630: 0964 0f64 1084 005a 0a64 1164 1284 005a  .d.d...Z.d.d...Z
-00000640: 0b64 1364 1484 005a 0c64 1564 1684 005a  .d.d...Z.d.d...Z
-00000650: 0d64 1764 1884 005a 0e64 1964 1a84 005a  .d.d...Z.d.d...Z
-00000660: 0f64 1b64 1c84 005a 1064 1d64 1e84 005a  .d.d...Z.d.d...Z
-00000670: 1164 1f65 1264 2065 1264 2165 1365 1219  .d.e.d e.d!e.e..
-00000680: 0064 2265 1365 1219 0064 0c64 0266 0a64  .d"e.e...d.d.f.d
-00000690: 2364 2484 045a 1464 1f65 1264 2065 1264  #d$..Z.d.e.d e.d
-000006a0: 2565 1365 1365 1219 0066 0119 0064 2665  %e.e.e...f...d&e
-000006b0: 1365 1365 1219 0066 0119 0064 0c64 0266  .e.e...f...d.d.f
-000006c0: 0a64 2764 2884 045a 1564 2665 1365 1365  .d'd(..Z.d&e.e.e
-000006d0: 1219 0019 0064 0c65 1365 1365 1219 0019  .....d.e.e.e....
-000006e0: 0066 0464 2964 2a84 045a 1664 0c65 1365  .f.d)d*..Z.d.e.e
-000006f0: 1365 1219 0019 0066 0264 2b64 2c84 045a  .e.....f.d+d,..Z
-00000700: 1764 0253 0029 2fda 0741 6461 7074 6572  .d.S.)/..Adapter
-00000710: 7a22 7468 6520 696e 7465 7266 6163 6520  z"the interface 
-00000720: 666f 7220 4361 7362 696e 2061 6461 7074  for Casbin adapt
-00000730: 6572 732e 4e46 6304 0000 0000 0000 0000  ers.NFc.........
-00000740: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
-00000750: 8400 0000 7400 7c01 7401 8302 7218 7c01  ....t.|.t...r.|.
-00000760: 7401 7402 6a03 6a04 8301 6b02 7212 7402  t.t.j.j...k.r.t.
-00000770: 6a03 7c00 5f05 6e09 7406 7c01 8301 7c00  j.|._.n.t.|...|.
-00000780: 5f05 6e03 7c01 7c00 5f05 7c02 6400 7500  _.n.|.|._.|.d.u.
-00000790: 7222 7407 7d02 6e11 6401 4400 5d0e 7d04  r"t.}.n.d.D.].}.
-000007a0: 7408 7c02 7c04 8302 7332 7409 7c04 9b00  t.|.|...s2t.|...
-000007b0: 6402 9d02 8301 8201 7124 7c02 7c00 5f0a  d.......q$|.|._.
-000007c0: 740b 7c00 6a05 6403 8d01 7c00 5f0c 7c03  t.|.j.d...|._.|.
-000007d0: 7c00 5f0d 6400 5300 2904 4e29 0872 2200  |._.d.S.).N).r".
-000007e0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-000007f0: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000800: 7218 0000 007a 2320 6e6f 7420 666f 756e  r....z# not foun
-00000810: 6420 696e 2063 7573 746f 6d20 4461 7461  d in custom Data
-00000820: 6261 7365 436c 6173 732e 2901 da04 6269  baseClass.)...bi
-00000830: 6e64 290e da0a 6973 696e 7374 616e 6365  nd)...isinstance
-00000840: 7223 0000 0072 0c00 0000 da06 656e 6769  r#...r......engi
-00000850: 6e65 da03 7572 6c5a 075f 656e 6769 6e65  ne..urlZ._engine
-00000860: 7208 0000 0072 0f00 0000 da07 6861 7361  r....r......hasa
-00000870: 7474 72da 0945 7863 6570 7469 6f6e da09  ttr..Exception..
-00000880: 5f64 625f 636c 6173 7372 0b00 0000 da0d  _db_classr......
-00000890: 7365 7373 696f 6e5f 6c6f 6361 6cda 095f  session_local.._
-000008a0: 6669 6c74 6572 6564 2905 721b 0000 005a  filtered).r....Z
-000008b0: 0a65 6e67 696e 655f 7572 695a 0864 625f  .engine_uriZ.db_
-000008c0: 636c 6173 73da 0866 696c 7465 7265 64da  class..filtered.
-000008d0: 0461 7474 7272 1e00 0000 721e 0000 0072  .attrr....r....r
-000008e0: 1f00 0000 da08 5f5f 696e 6974 5f5f 3700  ......__init__7.
-000008f0: 0000 731c 0000 000a 0210 010a 010c 0206  ..s.............
-00000900: 0208 0206 0108 020a 0a0e 0102 ff06 040e  ................
-00000910: 010a 037a 1041 6461 7074 6572 2e5f 5f69  ...z.Adapter.__i
-00000920: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000930: 0000 0300 0000 0a00 0000 6300 0000 735c  ..........c...s\
-00000940: 0000 0081 007c 00a0 00a1 007d 017a 237a  .....|.....}.z#z
-00000950: 097c 0156 0001 007c 01a0 01a1 0001 0057  .|.V...|.......W
-00000960: 006e 1204 0074 0279 2101 007d 0201 007a  .n...t.y!..}...z
-00000970: 067c 01a0 03a1 0001 007c 0282 0164 017d  .|.......|...d.}
-00000980: 027e 0277 0177 0057 007c 01a0 04a1 0001  .~.w.w.W.|......
-00000990: 0064 0153 007c 01a0 04a1 0001 0077 0029  .d.S.|.......w.)
-000009a0: 027a 3c50 726f 7669 6465 2061 2074 7261  .z<Provide a tra
-000009b0: 6e73 6163 7469 6f6e 616c 2073 636f 7065  nsactional scope
-000009c0: 2061 726f 756e 6420 6120 7365 7269 6573   around a series
-000009d0: 206f 6620 6f70 6572 6174 696f 6e73 2e4e   of operations.N
-000009e0: 2905 7235 0000 00da 0663 6f6d 6d69 7472  ).r5.....commitr
-000009f0: 3300 0000 da08 726f 6c6c 6261 636b da05  3.....rollback..
-00000a00: 636c 6f73 6529 0372 1b00 0000 da07 7365  close).r......se
-00000a10: 7373 696f 6eda 0165 721e 0000 0072 1e00  ssion..er....r..
-00000a20: 0000 721f 0000 00da 0e5f 7365 7373 696f  ..r......_sessio
-00000a30: 6e5f 7363 6f70 6558 0000 0073 1800 0000  n_scopeX...s....
-00000a40: 0280 0803 0401 0601 0c01 0e01 0801 0401  ................
-00000a50: 0880 02fe 02ff 1605 7a16 4164 6170 7465  ........z.Adapte
-00000a60: 722e 5f73 6573 7369 6f6e 5f73 636f 7065  r._session_scope
-00000a70: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00000a80: 0008 0000 0043 0000 0073 5800 0000 7c00  .....C...sX...|.
-00000a90: a000 a100 8f1e 7d02 7c02 a001 7c00 6a02  ......}.|...|.j.
-00000aa0: a101 a003 a100 7d03 7c03 4400 5d0a 7d04  ......}.|.D.].}.
-00000ab0: 7404 a005 7406 7c04 8301 7c01 a102 0100  t...t.|...|.....
-00000ac0: 710f 5700 6401 0400 0400 8303 0100 6401  q.W.d.........d.
-00000ad0: 5300 3100 7325 7701 0100 0100 0100 5900  S.1.s%w.......Y.
-00000ae0: 0100 6401 5300 2902 fa28 6c6f 6164 7320  ..d.S.)..(loads 
-00000af0: 616c 6c20 706f 6c69 6379 2072 756c 6573  all policy rules
-00000b00: 2066 726f 6d20 7468 6520 7374 6f72 6167   from the storag
-00000b10: 652e 4e29 0772 3f00 0000 da05 7175 6572  e.N).r?.....quer
-00000b20: 7972 3400 0000 da03 616c 6c72 0400 0000  yr4.....allr....
-00000b30: da10 6c6f 6164 5f70 6f6c 6963 795f 6c69  ..load_policy_li
-00000b40: 6e65 7223 0000 0029 0572 1b00 0000 da05  ner#...).r......
-00000b50: 6d6f 6465 6c72 3d00 0000 da05 6c69 6e65  modelr=.....line
-00000b60: 73da 046c 696e 6572 1e00 0000 721e 0000  s..liner....r...
-00000b70: 0072 1f00 0000 da0b 6c6f 6164 5f70 6f6c  .r......load_pol
-00000b80: 6963 7965 0000 0073 0c00 0000 0a02 1001  icye...s........
-00000b90: 0801 1201 02ff 22fe 7a13 4164 6170 7465  ......".z.Adapte
-00000ba0: 722e 6c6f 6164 5f70 6f6c 6963 7963 0100  r.load_policyc..
-00000bb0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000bc0: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
-00000bd0: 0029 014e 2901 7236 0000 0072 2400 0000  .).N).r6...r$...
-00000be0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-00000bf0: 0b69 735f 6669 6c74 6572 6564 6c00 0000  .is_filteredl...
-00000c00: 7302 0000 0006 017a 1341 6461 7074 6572  s......z.Adapter
-00000c10: 2e69 735f 6669 6c74 6572 6564 da06 7265  .is_filtered..re
-00000c20: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-00000c30: 0007 0000 0008 0000 0043 0000 0073 6e00  .........C...sn.
-00000c40: 0000 7c00 a000 a100 8f29 7d03 7c03 a001  ..|......)}.|...
-00000c50: 7c00 6a02 a101 7d04 7c00 a003 7c04 7c02  |.j...}.|...|.|.
-00000c60: a102 7d05 7c05 a004 a100 7d05 7c05 4400  ..}.|.....}.|.D.
-00000c70: 5d0a 7d06 7405 a006 7407 7c06 8301 7c01  ].}.t...t.|...|.
-00000c80: a102 0100 7117 6401 7c00 5f08 5700 6402  ....q.d.|._.W.d.
-00000c90: 0400 0400 8303 0100 6402 5300 3100 7330  ........d.S.1.s0
-00000ca0: 7701 0100 0100 0100 5900 0100 6402 5300  w.......Y...d.S.
-00000cb0: 2903 7240 0000 0054 4e29 0972 3f00 0000  ).r@...TN).r?...
-00000cc0: 7241 0000 0072 3400 0000 da0c 6669 6c74  rA...r4.....filt
-00000cd0: 6572 5f71 7565 7279 7242 0000 0072 0400  er_queryrB...r..
-00000ce0: 0000 7243 0000 0072 2300 0000 7236 0000  ..rC...r#...r6..
-00000cf0: 0029 0772 1b00 0000 7244 0000 00da 0666  .).r....rD.....f
-00000d00: 696c 7465 7272 3d00 0000 7241 0000 00da  ilterr=...rA....
-00000d10: 0766 696c 7465 7273 7246 0000 0072 1e00  .filtersrF...r..
-00000d20: 0000 721e 0000 0072 1f00 0000 da14 6c6f  ..r....r......lo
-00000d30: 6164 5f66 696c 7465 7265 645f 706f 6c69  ad_filtered_poli
-00000d40: 6379 6f00 0000 7310 0000 000a 020c 010c  cyo...s.........
-00000d50: 0108 0108 0212 0108 0122 f97a 1c41 6461  .........".z.Ada
-00000d60: 7074 6572 2e6c 6f61 645f 6669 6c74 6572  pter.load_filter
-00000d70: 6564 5f70 6f6c 6963 7963 0300 0000 0000  ed_policyc......
-00000d80: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00000d90: 0000 7348 0000 0064 0144 005d 1a7d 0374  ..sH...d.D.].}.t
-00000da0: 0074 017c 027c 0383 0283 0164 026b 0472  .t.|.|.....d.k.r
-00000db0: 1c7c 01a0 0274 017c 006a 037c 0383 02a0  .|...t.|.j.|....
-00000dc0: 0474 017c 027c 0383 02a1 01a1 017d 0171  .t.|.|.......}.q
-00000dd0: 027c 01a0 057c 006a 036a 06a1 0153 0029  .|...|.j.j...S.)
-00000de0: 034e 2907 7212 0000 0072 1300 0000 7214  .N).r....r....r.
-00000df0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00000e00: 0000 7218 0000 0072 0100 0000 2907 da03  ..r....r....)...
-00000e10: 6c65 6eda 0767 6574 6174 7472 724b 0000  len..getattrrK..
-00000e20: 0072 3400 0000 da03 696e 5fda 086f 7264  .r4.....in_..ord
-00000e30: 6572 5f62 7972 2200 0000 2904 721b 0000  er_byr"...).r...
-00000e40: 005a 0771 7565 7279 6462 724b 0000 0072  .Z.querydbrK...r
-00000e50: 3800 0000 721e 0000 0072 1e00 0000 721f  8...r....r....r.
-00000e60: 0000 0072 4a00 0000 7a00 0000 730e 0000  ...rJ...z...s...
-00000e70: 0008 0112 0104 0116 0104 ff02 800e 037a  ...............z
-00000e80: 1441 6461 7074 6572 2e66 696c 7465 725f  .Adapter.filter_
-00000e90: 7175 6572 7963 0300 0000 0000 0000 0000  queryc..........
-00000ea0: 0000 0700 0000 0800 0000 4300 0000 7368  ..........C...sh
-00000eb0: 0000 007c 00a0 00a1 008f 267d 037c 006a  ...|......&}.|.j
-00000ec0: 017c 0164 018d 017d 0474 027c 0283 0144  .|.d...}.t.|...D
-00000ed0: 005d 0d5c 027d 057d 0674 037c 0464 02a0  .].\.}.}.t.|.d..
-00000ee0: 047c 05a1 017c 0683 0301 0071 0f7c 03a0  .|...|.....q.|..
-00000ef0: 057c 04a1 0101 0057 0064 0004 0004 0083  .|.....W.d......
-00000f00: 0301 0064 0053 0031 0073 2d77 0101 0001  ...d.S.1.s-w....
-00000f10: 0001 0059 0001 0064 0053 0029 034e 2901  ...Y...d.S.).N).
-00000f20: 7212 0000 00fa 0376 7b7d 2906 723f 0000  r......v{}).r?..
-00000f30: 0072 3400 0000 da09 656e 756d 6572 6174  .r4.....enumerat
-00000f40: 65da 0773 6574 6174 7472 7221 0000 00da  e..setattrr!....
-00000f50: 0361 6464 2907 721b 0000 0072 1200 0000  .add).r....r....
-00000f60: da04 7275 6c65 723d 0000 0072 4600 0000  ..ruler=...rF...
-00000f70: da01 6972 1d00 0000 721e 0000 0072 1e00  ..ir....r....r..
-00000f80: 0000 721f 0000 00da 115f 7361 7665 5f70  ..r......_save_p
-00000f90: 6f6c 6963 795f 6c69 6e65 8200 0000 730c  olicy_line....s.
-00000fa0: 0000 000a 010c 0110 0114 010c 0122 fc7a  .............".z
-00000fb0: 1941 6461 7074 6572 2e5f 7361 7665 5f70  .Adapter._save_p
-00000fc0: 6f6c 6963 795f 6c69 6e65 6302 0000 0000  olicy_linec.....
-00000fd0: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
-00000fe0: 0000 0073 8c00 0000 7c00 a000 a100 8f38  ...s....|......8
-00000ff0: 7d02 7c02 a001 7c00 6a02 a101 7d03 7c03  }.|...|.j...}.|.
-00001000: a003 a100 0100 6401 4400 5d22 7d04 7c04  ......d.D.]"}.|.
-00001010: 7c01 6a04 a005 a100 7601 721b 7111 7c01  |.j.....v.r.q.|.
-00001020: 6a04 7c04 1900 a006 a100 4400 5d10 5c02  j.|.......D.].\.
-00001030: 7d05 7d06 7c06 6a07 4400 5d08 7d07 7c00  }.}.|.j.D.].}.|.
-00001040: a008 7c05 7c07 a102 0100 7129 7122 7111  ..|.|.....q)q"q.
-00001050: 5700 6402 0400 0400 8303 0100 6403 5300  W.d.........d.S.
-00001060: 3100 733f 7701 0100 0100 0100 5900 0100  1.s?w.......Y...
-00001070: 6403 5300 2904 7a26 7361 7665 7320 616c  d.S.).z&saves al
-00001080: 6c20 706f 6c69 6379 2072 756c 6573 2074  l policy rules t
-00001090: 6f20 7468 6520 7374 6f72 6167 652e 2902  o the storage.).
-000010a0: da01 70da 0167 4e54 2909 723f 0000 0072  ..p..gNT).r?...r
-000010b0: 4100 0000 7234 0000 00da 0664 656c 6574  A...r4.....delet
-000010c0: 6572 4400 0000 da04 6b65 7973 da05 6974  erD.....keys..it
-000010d0: 656d 73da 0670 6f6c 6963 7972 5800 0000  ems..policyrX...
-000010e0: 2908 721b 0000 0072 4400 0000 723d 0000  ).r....rD...r=..
-000010f0: 0072 4100 0000 da03 7365 6372 1200 0000  .rA.....secr....
-00001100: da03 6173 7472 5600 0000 721e 0000 0072  ..astrV...r....r
-00001110: 1e00 0000 721f 0000 00da 0b73 6176 655f  ....r......save_
-00001120: 706f 6c69 6379 8900 0000 7320 0000 000a  policy....s ....
-00001130: 020c 0108 0108 010e 0102 0116 010a 010e  ................
-00001140: 0102 ff02 ff02 fd0a fd04 0910 f704 097a  ...............z
-00001150: 1341 6461 7074 6572 2e73 6176 655f 706f  .Adapter.save_po
-00001160: 6c69 6379 6304 0000 0000 0000 0000 0000  licyc...........
-00001170: 0004 0000 0004 0000 0043 0000 0073 1000  .........C...s..
-00001180: 0000 7c00 a000 7c02 7c03 a102 0100 6401  ..|...|.|.....d.
-00001190: 5300 2902 7a22 6164 6473 2061 2070 6f6c  S.).z"adds a pol
-000011a0: 6963 7920 7275 6c65 2074 6f20 7468 6520  icy rule to the 
-000011b0: 7374 6f72 6167 652e 4ea9 0172 5800 0000  storage.N..rX...
-000011c0: 2904 721b 0000 0072 5f00 0000 7212 0000  ).r....r_...r...
-000011d0: 0072 5600 0000 721e 0000 0072 1e00 0000  .rV...r....r....
-000011e0: 721f 0000 00da 0a61 6464 5f70 6f6c 6963  r......add_polic
-000011f0: 7996 0000 0073 0200 0000 1002 7a12 4164  y....s......z.Ad
-00001200: 6170 7465 722e 6164 645f 706f 6c69 6379  apter.add_policy
-00001210: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
-00001220: 0005 0000 0043 0000 0073 1a00 0000 7c03  .....C...s....|.
-00001230: 4400 5d08 7d04 7c00 a000 7c02 7c04 a102  D.].}.|...|.|...
-00001240: 0100 7102 6401 5300 2902 7a23 6164 6473  ..q.d.S.).z#adds
-00001250: 2061 2070 6f6c 6963 7920 7275 6c65 7320   a policy rules 
-00001260: 746f 2074 6865 2073 746f 7261 6765 2e4e  to the storage.N
-00001270: 7262 0000 0029 0572 1b00 0000 725f 0000  rb...).r....r_..
-00001280: 0072 1200 0000 da05 7275 6c65 7372 5600  .r......rulesrV.
-00001290: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-000012a0: 00da 0c61 6464 5f70 6f6c 6963 6965 739a  ...add_policies.
-000012b0: 0000 0073 0600 0000 0802 0e01 04ff 7a14  ...s..........z.
-000012c0: 4164 6170 7465 722e 6164 645f 706f 6c69  Adapter.add_poli
-000012d0: 6369 6573 6304 0000 0000 0000 0000 0000  ciesc...........
-000012e0: 0009 0000 0009 0000 0043 0000 0073 8c00  .........C...s..
-000012f0: 0000 7c00 a000 a100 8f32 7d04 7c04 a001  ..|......2}.|...
-00001300: 7c00 6a02 a101 7d05 7c05 a003 7c00 6a02  |.j...}.|...|.j.
-00001310: 6a04 7c02 6b02 a101 7d05 7405 7c03 8301  j.|.k...}.t.|...
-00001320: 4400 5d12 5c02 7d06 7d07 7c05 a003 7406  D.].\.}.}.|...t.
-00001330: 7c00 6a02 6401 a007 7c06 a101 8302 7c07  |.j.d...|.....|.
-00001340: 6b02 a101 7d05 7118 7c05 a008 a100 7d08  k...}.q.|.....}.
-00001350: 5700 6402 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00001360: 7339 7701 0100 0100 0100 5900 0100 7c08  s9w.......Y...|.
-00001370: 6403 6b04 7244 6404 5300 6405 5300 2906  d.k.rDd.S.d.S.).
-00001380: 7a27 7265 6d6f 7665 7320 6120 706f 6c69  z'removes a poli
-00001390: 6379 2072 756c 6520 6672 6f6d 2074 6865  cy rule from the
-000013a0: 2073 746f 7261 6765 2e72 5200 0000 4e72   storage.rR...Nr
-000013b0: 0100 0000 5446 2909 723f 0000 0072 4100  ....TF).r?...rA.
-000013c0: 0000 7234 0000 0072 4b00 0000 7212 0000  ..r4...rK...r...
-000013d0: 0072 5300 0000 724f 0000 0072 2100 0000  .rS...rO...r!...
-000013e0: 725b 0000 0029 0972 1b00 0000 725f 0000  r[...).r....r_..
-000013f0: 0072 1200 0000 7256 0000 0072 3d00 0000  .r....rV...r=...
-00001400: 7241 0000 0072 5700 0000 721d 0000 00da  rA...rW...r.....
-00001410: 0172 721e 0000 0072 1e00 0000 721f 0000  .rr....r....r...
-00001420: 00da 0d72 656d 6f76 655f 706f 6c69 6379  ...remove_policy
-00001430: 9f00 0000 7310 0000 000a 020c 0112 0110  ....s...........
-00001440: 011e 010a 011c fb10 077a 1541 6461 7074  .........z.Adapt
-00001450: 6572 2e72 656d 6f76 655f 706f 6c69 6379  er.remove_policy
-00001460: 6304 0000 0000 0000 0000 0000 0007 0000  c...............
-00001470: 0008 0000 0003 0000 0073 9400 0000 7c03  .........s....|.
-00001480: 7304 6401 5300 8801 a000 a100 8f38 7d04  s.d.S........8}.
-00001490: 7c04 a001 8801 6a02 a101 7d05 7c05 a003  |.....j...}.|...
-000014a0: 8801 6a02 6a04 7c02 6b02 a101 7d05 7405  ..j.j.|.k...}.t.
-000014b0: 7c03 8e00 7d03 7406 7c03 8301 4400 5d13  |...}.t.|...D.].
-000014c0: 5c02 8900 7d06 7c05 a003 7407 8700 8701  \...}.|...t.....
-000014d0: 6602 6402 6403 8408 7c06 4400 8301 8301  f.d.d...|.D.....
-000014e0: a101 7d05 7120 7c05 a008 a100 0100 5700  ..}.q |.......W.
-000014f0: 6401 0400 0400 8303 0100 6401 5300 3100  d.........d.S.1.
-00001500: 7343 7701 0100 0100 0100 5900 0100 6401  sCw.......Y...d.
-00001510: 5300 2904 7a25 7265 6d6f 7665 2070 6f6c  S.).z%remove pol
-00001520: 6963 7920 7275 6c65 7320 6672 6f6d 2074  icy rules from t
-00001530: 6865 2073 746f 7261 6765 2e4e 6301 0000  he storage.Nc...
-00001540: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00001550: 0033 0000 0073 2600 0000 8100 7c00 5d0e  .3...s&.....|.].
-00001560: 7d01 7400 8801 6a01 6400 a002 8800 a101  }.t...j.d.......
-00001570: 8302 7c01 6b02 5600 0100 7102 6401 5300  ..|.k.V...q.d.S.
-00001580: 2902 7252 0000 004e 2903 724f 0000 0072  ).rR...N).rO...r
-00001590: 3400 0000 7221 0000 0029 02da 022e 3072  4...r!...)....0r
-000015a0: 1d00 0000 a902 7257 0000 0072 1b00 0000  ......rW...r....
-000015b0: 721e 0000 0072 1f00 0000 da09 3c67 656e  r....r......<gen
-000015c0: 6578 7072 3eb4 0000 0073 0400 0000 0280  expr>....s......
-000015d0: 2400 7a2a 4164 6170 7465 722e 7265 6d6f  $.z*Adapter.remo
-000015e0: 7665 5f70 6f6c 6963 6965 732e 3c6c 6f63  ve_policies.<loc
-000015f0: 616c 733e 2e3c 6765 6e65 7870 723e 2909  als>.<genexpr>).
-00001600: 723f 0000 0072 4100 0000 7234 0000 0072  r?...rA...r4...r
-00001610: 4b00 0000 7212 0000 00da 037a 6970 7253  K...r......ziprS
-00001620: 0000 0072 0900 0000 725b 0000 0029 0772  ...r....r[...).r
-00001630: 1b00 0000 725f 0000 0072 1200 0000 7264  ....r_...r....rd
-00001640: 0000 0072 3d00 0000 7241 0000 0072 5600  ...r=...rA...rV.
-00001650: 0000 721e 0000 0072 6900 0000 721f 0000  ..r....ri...r...
-00001660: 00da 0f72 656d 6f76 655f 706f 6c69 6369  ...remove_polici
-00001670: 6573 aa00 0000 7318 0000 0004 0204 010a  es....s.........
-00001680: 010c 0112 0108 0110 0104 0116 0106 ff0a  ................
-00001690: 0322 f87a 1741 6461 7074 6572 2e72 656d  .".z.Adapter.rem
-000016a0: 6f76 655f 706f 6c69 6369 6573 6304 0000  ove_policiesc...
-000016b0: 0000 0000 0000 0000 000b 0000 0008 0000  ................
-000016c0: 0047 0000 0073 f000 0000 7c00 a000 a100  .G...s....|.....
-000016d0: 8f64 7d05 7c05 a001 7c00 6a02 a101 a003  .d}.|...|.j.....
-000016e0: 7c00 6a02 6a04 7c02 6b02 a101 7d06 6401  |.j.j.|.k...}.d.
-000016f0: 7c03 0400 0300 6b01 721c 6402 6b01 7326  |.....k.r.d.k.s&
-00001700: 6e01 0100 0900 5700 6403 0400 0400 8303  n.....W.d.......
-00001710: 0100 6404 5300 6405 7c03 7405 7c04 8301  ..d.S.d.|.t.|...
-00001720: 1700 0400 0300 6b01 7234 6406 6b01 733e  ......k.r4d.k.s>
-00001730: 6e01 0100 0900 5700 6403 0400 0400 8303  n.....W.d.......
-00001740: 0100 6404 5300 7406 7c04 8301 4400 5d1a  ..d.S.t.|...D.].
-00001750: 5c02 7d07 7d08 7c08 6407 6b03 725c 7407  \.}.}.|.d.k.r\t.
-00001760: 7c00 6a02 6408 a008 7c03 7c07 1700 a101  |.j.d...|.|.....
-00001770: 8302 7d09 7c06 a003 7c09 7c08 6b02 a101  ..}.|...|.|.k...
-00001780: 7d06 7142 7c06 a009 a100 7d0a 5700 6403  }.qB|.....}.W.d.
-00001790: 0400 0400 8303 0100 6e08 3100 736b 7701  ........n.1.skw.
-000017a0: 0100 0100 0100 5900 0100 7c0a 6401 6b04  ......Y...|.d.k.
-000017b0: 7276 6409 5300 6404 5300 290a 7a74 7265  rvd.S.d.S.).ztre
-000017c0: 6d6f 7665 7320 706f 6c69 6379 2072 756c  moves policy rul
-000017d0: 6573 2074 6861 7420 6d61 7463 6820 7468  es that match th
-000017e0: 6520 6669 6c74 6572 2066 726f 6d20 7468  e filter from th
-000017f0: 6520 7374 6f72 6167 652e 0a20 2020 2020  e storage..     
-00001800: 2020 2054 6869 7320 6973 2070 6172 7420     This is part 
-00001810: 6f66 2074 6865 2041 7574 6f2d 5361 7665  of the Auto-Save
-00001820: 2066 6561 7475 7265 2e0a 2020 2020 2020   feature..      
-00001830: 2020 7201 0000 00e9 0500 0000 4e46 e901    r.........NF..
-00001840: 0000 00e9 0600 0000 da00 7252 0000 0054  ..........rR...T
-00001850: 290a 723f 0000 0072 4100 0000 7234 0000  ).r?...rA...r4..
-00001860: 0072 4b00 0000 7212 0000 0072 4e00 0000  .rK...r....rN...
-00001870: 7253 0000 0072 4f00 0000 7221 0000 0072  rS...rO...r!...r
-00001880: 5b00 0000 290b 721b 0000 0072 5f00 0000  [...).r....r_...
-00001890: 7212 0000 00da 0b66 6965 6c64 5f69 6e64  r......field_ind
-000018a0: 6578 da0c 6669 656c 645f 7661 6c75 6573  ex..field_values
-000018b0: 723d 0000 0072 4100 0000 7257 0000 0072  r=...rA...rW...r
-000018c0: 1d00 0000 da07 765f 7661 6c75 6572 6600  ......v_valuerf.
-000018d0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-000018e0: 00da 1672 656d 6f76 655f 6669 6c74 6572  ...remove_filter
-000018f0: 6564 5f70 6f6c 6963 79b8 0000 0073 2000  ed_policy....s .
-00001900: 0000 0a04 1a01 1602 0201 10fc 1e05 0201  ................
-00001910: 10fa 1007 0801 1601 0e01 0280 0a01 1cf5  ................
-00001920: 100d 7a1e 4164 6170 7465 722e 7265 6d6f  ..z.Adapter.remo
-00001930: 7665 5f66 696c 7465 7265 645f 706f 6c69  ve_filtered_poli
-00001940: 6379 725f 0000 0072 1200 0000 da08 6f6c  cyr_...r......ol
-00001950: 645f 7275 6c65 da08 6e65 775f 7275 6c65  d_rule..new_rule
-00001960: 6305 0000 0000 0000 0000 0000 000c 0000  c...............
-00001970: 0008 0000 0043 0000 0073 e000 0000 7c00  .....C...s....|.
-00001980: a000 a100 8f62 7d05 7c05 a001 7c00 6a02  .....b}.|...|.j.
-00001990: a101 a003 7c00 6a02 6a04 7c02 6b02 a101  ....|.j.j.|.k...
-000019a0: 7d06 7405 7c03 8301 4400 5d14 5c02 7d07  }.t.|...D.].\.}.
-000019b0: 7d08 7406 7c00 6a02 6401 a007 7c07 a101  }.t.|.j.d...|...
-000019c0: 8302 7d09 7c06 a003 7c09 7c08 6b02 a101  ..}.|...|.|.k...
-000019d0: 7d06 7116 7408 7c03 8301 7408 7c04 8301  }.q.t.|...t.|...
-000019e0: 6b04 7235 7c03 6e01 7c04 7d0a 7c06 a009  k.r5|.n.|.}.|...
-000019f0: a100 7d0b 740a 7408 7c0a 8301 8301 4400  ..}.t.t.|.....D.
-00001a00: 5d1c 7d07 7c07 7408 7c04 8301 6b00 7255  ].}.|.t.|...k.rU
-00001a10: 740b 6402 7c07 9b00 6403 7c07 9b00 6404  t.d.|...d.|...d.
-00001a20: 9d05 8301 0100 7141 740b 6402 7c07 9b00  ......qAt.d.|...
-00001a30: 6405 9d03 8301 0100 7141 5700 6406 0400  d.......qAW.d...
-00001a40: 0400 8303 0100 6406 5300 3100 7369 7701  ......d.S.1.siw.
-00001a50: 0100 0100 0100 5900 0100 6406 5300 2907  ......Y...d.S.).
-00001a60: 612b 0100 000a 2020 2020 2020 2020 5570  a+....        Up
-00001a70: 6461 7465 2074 6865 206f 6c64 5f72 756c  date the old_rul
-00001a80: 6520 7769 7468 2074 6865 206e 6577 5f72  e with the new_r
-00001a90: 756c 6520 696e 2074 6865 2064 6174 6162  ule in the datab
-00001aa0: 6173 6520 2873 746f 7261 6765 292e 0a0a  ase (storage)...
-00001ab0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00001ac0: 6563 3a20 7365 6374 696f 6e20 7479 7065  ec: section type
-00001ad0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001ae0: 7074 7970 653a 2070 6f6c 6963 7920 7479  ptype: policy ty
-00001af0: 7065 0a20 2020 2020 2020 203a 7061 7261  pe.        :para
-00001b00: 6d20 6f6c 645f 7275 6c65 3a20 7468 6520  m old_rule: the 
-00001b10: 6f6c 6420 7275 6c65 2074 6861 7420 6e65  old rule that ne
-00001b20: 6564 7320 746f 2062 6520 6d6f 6469 6669  eds to be modifi
-00001b30: 6564 0a20 2020 2020 2020 203a 7061 7261  ed.        :para
-00001b40: 6d20 6e65 775f 7275 6c65 3a20 7468 6520  m new_rule: the 
-00001b50: 6e65 7720 7275 6c65 2074 6f20 7265 706c  new rule to repl
-00001b60: 6163 6520 7468 6520 6f6c 6420 7275 6c65  ace the old rule
-00001b70: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001b80: 6e3a 204e 6f6e 650a 2020 2020 2020 2020  n: None.        
-00001b90: 7252 0000 007a 0f6f 6c64 5f72 756c 655f  rR...z.old_rule_
-00001ba0: 6c69 6e65 2e76 7a0c 203d 206e 6577 5f72  line.vz. = new_r
-00001bb0: 756c 655b da01 5d7a 0720 3d20 4e6f 6e65  ule[..]z. = None
-00001bc0: 4e29 0c72 3f00 0000 7241 0000 0072 3400  N).r?...rA...r4.
-00001bd0: 0000 724b 0000 0072 1200 0000 7253 0000  ..rK...r....rS..
-00001be0: 0072 4f00 0000 7221 0000 0072 4e00 0000  .rO...r!...rN...
-00001bf0: da03 6f6e 65da 0572 616e 6765 da04 6578  ..one..range..ex
-00001c00: 6563 290c 721b 0000 0072 5f00 0000 7212  ec).r....r_...r.
-00001c10: 0000 0072 7500 0000 7276 0000 0072 3d00  ...ru...rv...r=.
-00001c20: 0000 7241 0000 00da 0569 6e64 6578 da05  ..rA.....index..
-00001c30: 7661 6c75 6572 7300 0000 5a0c 6c6f 6e67  valuers...Z.long
-00001c40: 6573 745f 7275 6c65 5a0d 6f6c 645f 7275  est_ruleZ.old_ru
-00001c50: 6c65 5f6c 696e 6572 1e00 0000 721e 0000  le_liner....r...
-00001c60: 0072 1f00 0000 da0d 7570 6461 7465 5f70  .r......update_p
-00001c70: 6f6c 6963 79cb 0000 0073 1a00 0000 0a0e  olicy....s......
-00001c80: 1a01 1003 1201 1001 1803 0801 1003 0c01  ................
-00001c90: 1801 1202 02fc 22f3 7a15 4164 6170 7465  ......".z.Adapte
-00001ca0: 722e 7570 6461 7465 5f70 6f6c 6963 79da  r.update_policy.
-00001cb0: 096f 6c64 5f72 756c 6573 da09 6e65 775f  .old_rules..new_
-00001cc0: 7275 6c65 7363 0500 0000 0000 0000 0000  rulesc..........
-00001cd0: 0000 0600 0000 0800 0000 4300 0000 732e  ..........C...s.
-00001ce0: 0000 0074 0074 017c 0383 0183 0144 005d  ...t.t.|.....D.]
-00001cf0: 0e7d 057c 00a0 027c 017c 027c 037c 0519  .}.|...|.|.|.|..
-00001d00: 007c 047c 0519 00a1 0401 0071 0664 0153  .|.|.......q.d.S
-00001d10: 0029 0261 3101 0000 0a20 2020 2020 2020  .).a1....       
-00001d20: 2055 7064 6174 6520 7468 6520 6f6c 645f   Update the old_
-00001d30: 7275 6c65 7320 7769 7468 2074 6865 206e  rules with the n
-00001d40: 6577 5f72 756c 6573 2069 6e20 7468 6520  ew_rules in the 
-00001d50: 6461 7461 6261 7365 2028 7374 6f72 6167  database (storag
-00001d60: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
-00001d70: 7261 6d20 7365 633a 2073 6563 7469 6f6e  ram sec: section
-00001d80: 2074 7970 650a 2020 2020 2020 2020 3a70   type.        :p
-00001d90: 6172 616d 2070 7479 7065 3a20 706f 6c69  aram ptype: poli
-00001da0: 6379 2074 7970 650a 2020 2020 2020 2020  cy type.        
-00001db0: 3a70 6172 616d 206f 6c64 5f72 756c 6573  :param old_rules
-00001dc0: 3a20 7468 6520 6f6c 6420 7275 6c65 7320  : the old rules 
-00001dd0: 7468 6174 206e 6565 6420 746f 2062 6520  that need to be 
-00001de0: 6d6f 6469 6669 6564 0a20 2020 2020 2020  modified.       
-00001df0: 203a 7061 7261 6d20 6e65 775f 7275 6c65   :param new_rule
-00001e00: 733a 2074 6865 206e 6577 2072 756c 6573  s: the new rules
-00001e10: 2074 6f20 7265 706c 6163 6520 7468 6520   to replace the 
-00001e20: 6f6c 6420 7275 6c65 730a 0a20 2020 2020  old rules..     
-00001e30: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
-00001e40: 0a20 2020 2020 2020 204e 2903 7279 0000  .        N).ry..
-00001e50: 0072 4e00 0000 727d 0000 0029 0672 1b00  .rN...r}...).r..
-00001e60: 0000 725f 0000 0072 1200 0000 727e 0000  ..r_...r....r~..
-00001e70: 0072 7f00 0000 7257 0000 0072 1e00 0000  .r....rW...r....
-00001e80: 721e 0000 0072 1f00 0000 da0f 7570 6461  r....r......upda
-00001e90: 7465 5f70 6f6c 6963 6965 73ec 0000 0073  te_policies....s
-00001ea0: 0600 0000 1015 1a01 04ff 7a17 4164 6170  ..........z.Adap
-00001eb0: 7465 722e 7570 6461 7465 5f70 6f6c 6963  ter.update_polic
-00001ec0: 6965 7363 0500 0000 0000 0000 0000 0000  iesc............
-00001ed0: 0800 0000 0700 0000 4700 0000 7362 0000  ........G...sb..
-00001ee0: 0074 0083 007d 067c 027c 065f 0174 0274  .t...}.|.|._.t.t
-00001ef0: 037c 0583 0183 0144 005d 1c7d 077c 047c  .|.....D.].}.|.|
-00001f00: 076b 0172 287c 077c 0474 037c 0583 0117  .k.r(|.|.t.|....
-00001f10: 006b 0072 2874 047c 0664 017c 079b 009d  .k.r(t.|.d.|....
-00001f20: 027c 057c 077c 0418 0019 0083 0301 0071  .|.|.|.........q
-00001f30: 0c01 007c 00a0 057c 037c 06a1 0201 0064  ...|...|.|.....d
-00001f40: 0253 0029 037a 4d75 7064 6174 655f 6669  .S.).zMupdate_fi
-00001f50: 6c74 6572 6564 5f70 6f6c 6963 6965 7320  ltered_policies 
-00001f60: 7570 6461 7465 7320 616c 6c20 7468 6520  updates all the 
-00001f70: 706f 6c69 6369 6573 206f 6e20 7468 6520  policies on the 
-00001f80: 6261 7369 7320 6f66 2074 6865 2066 696c  basis of the fil
-00001f90: 7465 722e 721d 0000 004e 2906 722c 0000  ter.r....N).r,..
-00001fa0: 0072 1200 0000 7279 0000 0072 4e00 0000  .r....ry...rN...
-00001fb0: 7254 0000 00da 195f 7570 6461 7465 5f66  rT....._update_f
-00001fc0: 696c 7465 7265 645f 706f 6c69 6369 6573  iltered_policies
-00001fd0: 2908 721b 0000 0072 5f00 0000 7212 0000  ).r....r_...r...
-00001fe0: 0072 7f00 0000 7271 0000 0072 7200 0000  .r....rq...rr...
-00001ff0: 724b 0000 0072 5700 0000 721e 0000 0072  rK...rW...r....r
-00002000: 1e00 0000 721f 0000 00da 1875 7064 6174  ....r......updat
-00002010: 655f 6669 6c74 6572 6564 5f70 6f6c 6963  e_filtered_polic
-00002020: 6965 7304 0100 0073 0e00 0000 0605 0601  ies....s........
-00002030: 1003 1801 1c01 0202 1002 7a20 4164 6170  ..........z Adap
-00002040: 7465 722e 7570 6461 7465 5f66 696c 7465  ter.update_filte
-00002050: 7265 645f 706f 6c69 6369 6573 6303 0000  red_policiesc...
-00002060: 0000 0000 0000 0000 0007 0000 0008 0000  ................
-00002070: 0043 0000 0073 8000 0000 7c00 a000 a100  .C...s....|.....
-00002080: 8f32 7d03 7c03 a001 7c00 6a02 a101 a003  .2}.|...|.j.....
-00002090: 7c00 6a02 6a04 7c02 6a04 6b02 a101 7d04  |.j.j.|.j.k...}.
-000020a0: 7c00 a005 7c04 7c02 a102 7d05 7c05 a006  |...|.|...}.|...
-000020b0: a100 7d06 7c00 a007 6401 7c02 6a04 7c06  ..}.|...d.|.j.|.
-000020c0: a103 0100 7c00 a008 6401 7c02 6a04 7c01  ....|...d.|.j.|.
-000020d0: a103 0100 7c06 5700 0200 6402 0400 0400  ....|.W...d.....
-000020e0: 8303 0100 5300 3100 7339 7701 0100 0100  ....S.1.s9w.....
-000020f0: 0100 5900 0100 6402 5300 2903 7a4e 5f75  ..Y...d.S.).zN_u
-00002100: 7064 6174 655f 6669 6c74 6572 6564 5f70  pdate_filtered_p
-00002110: 6f6c 6963 6965 7320 7570 6461 7465 7320  olicies updates 
-00002120: 616c 6c20 7468 6520 706f 6c69 6369 6573  all the policies
-00002130: 206f 6e20 7468 6520 6261 7369 7320 6f66   on the basis of
-00002140: 2074 6865 2066 696c 7465 722e 7259 0000   the filter.rY..
-00002150: 004e 2909 723f 0000 0072 4100 0000 7234  .N).r?...rA...r4
-00002160: 0000 0072 4b00 0000 7212 0000 0072 4a00  ...rK...r....rJ.
-00002170: 0000 7242 0000 0072 6c00 0000 7265 0000  ..rB...rl...re..
-00002180: 0029 0772 1b00 0000 727f 0000 0072 4b00  .).r....r....rK.
-00002190: 0000 723d 0000 0072 4100 0000 5a0e 6669  ..r=...rA...Z.fi
-000021a0: 6c74 6572 6564 5f71 7565 7279 727e 0000  ltered_queryr~..
-000021b0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000021c0: 7281 0000 0015 0100 0073 1400 0000 0a03  r........s......
-000021d0: 0c04 0c01 04ff 0c03 0801 1004 1004 0204  ................
-000021e0: 24ec 7a21 4164 6170 7465 722e 5f75 7064  $.z!Adapter._upd
-000021f0: 6174 655f 6669 6c74 6572 6564 5f70 6f6c  ate_filtered_pol
-00002200: 6963 6965 7329 024e 4629 0272 4900 0000  icies).NF).rI...
-00002210: 4e29 1872 2600 0000 7227 0000 0072 2800  N).r&...r'...r(.
-00002220: 0000 da07 5f5f 646f 635f 5f72 3900 0000  ....__doc__r9...
-00002230: 7202 0000 0072 3f00 0000 7247 0000 0072  r....r?...rG...r
-00002240: 4800 0000 724d 0000 0072 4a00 0000 7258  H...rM...rJ...rX
-00002250: 0000 0072 6100 0000 7263 0000 0072 6500  ...ra...rc...re.
-00002260: 0000 7267 0000 0072 6c00 0000 7274 0000  ..rg...rl...rt..
-00002270: 0072 2300 0000 7203 0000 0072 7d00 0000  .r#...r....r}...
-00002280: 7280 0000 0072 8200 0000 7281 0000 0072  r....r....r....r
-00002290: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
-000022a0: 0000 0072 2d00 0000 3400 0000 7360 0000  ...r-...4...s`..
-000022b0: 0008 0004 010a 0202 210a 0108 0c08 070a  ........!.......
-000022c0: 0308 0b08 0808 0708 0d08 0408 0508 0b08  ................
-000022d0: 0e02 1302 0102 ff02 0102 ff06 0102 ff06  ................
-000022e0: 0102 ff02 020a fe02 2102 0202 fe02 0302  ........!.......
-000022f0: fd02 0408 0102 ff02 fc02 0708 0102 ff02  ................
-00002300: f902 0a0a f602 180a 0102 ff0a 020a fe1a  ................
-00002310: 1172 2d00 0000 4e29 1dda 0a63 6f6e 7465  .r-...N)...conte
-00002320: 7874 6c69 6272 0200 0000 da06 7479 7069  xtlibr......typi
-00002330: 6e67 7203 0000 00da 0663 6173 6269 6e72  ngr......casbinr
-00002340: 0400 0000 da0a 7371 6c61 6c63 6865 6d79  ......sqlalchemy
-00002350: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00002360: 0800 0000 7209 0000 005a 1a73 716c 616c  ....r....Z.sqlal
-00002370: 6368 656d 792e 6578 742e 6465 636c 6172  chemy.ext.declar
-00002380: 6174 6976 6572 0a00 0000 da0e 7371 6c61  ativer......sqla
-00002390: 6c63 6865 6d79 2e6f 726d 720b 0000 00da  lchemy.ormr.....
-000023a0: 0669 7261 696c 7372 0c00 0000 5a0d 6972  .irailsr....Z.ir
-000023b0: 6169 6c73 2e63 6f6e 6669 6772 0d00 0000  ails.configr....
-000023c0: 7229 0000 00da 0367 6574 da03 6366 67da  r).....get..cfg.
-000023d0: 0442 6173 6572 0f00 0000 722c 0000 0072  .Baser....r,...r
-000023e0: 2d00 0000 da08 6164 6170 7465 7273 da0d  -.....adapters..
-000023f0: 5570 6461 7465 4164 6170 7465 7272 1e00  UpdateAdapterr..
-00002400: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00002410: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00002420: 2000 0000 0c00 0c01 0c02 1401 1001 0c01   ...............
-00002430: 0c01 0c03 0c01 0401 0a01 0c01 0c01 1202  ................
-00002440: 0e18 1c0a                                ....
+000001d0: 0000 0400 0000 4000 0000 7388 0000 0065  ......@...s....e
+000001e0: 005a 0164 005a 0264 015a 0365 045a 0564  .Z.d.Z.d.Z.e.Z.d
+000001f0: 015a 0665 0765 0864 0164 028d 025a 0965  .Z.e.e.d.d...Z.e
+00000200: 0765 0a64 0383 0183 015a 0b65 0765 0a64  .e.d.....Z.e.e.d
+00000210: 0383 0183 015a 0c65 0765 0a64 0383 0183  .....Z.e.e.d....
+00000220: 015a 0d65 0765 0a64 0383 0183 015a 0e65  .Z.e.e.d.....Z.e
+00000230: 0765 0a64 0383 0183 015a 0f65 0765 0a64  .e.d.....Z.e.e.d
+00000240: 0383 0183 015a 1065 0765 0a64 0383 0183  .....Z.e.e.d....
+00000250: 015a 1164 0464 0584 005a 1264 0664 0784  .Z.d.d...Z.d.d..
+00000260: 005a 1364 0853 0029 09da 0a43 6173 6269  .Z.d.S.)...Casbi
+00000270: 6e52 756c 6554 2901 da0b 7072 696d 6172  nRuleT)...primar
+00000280: 795f 6b65 79e9 ff00 0000 6301 0000 0000  y_key.....c.....
+00000290: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
+000002a0: 0000 0073 4a00 0000 7c00 6a00 6701 7d01  ...sJ...|.j.g.}.
+000002b0: 7c00 6a01 7c00 6a02 7c00 6a03 7c00 6a04  |.j.|.j.|.j.|.j.
+000002c0: 7c00 6a05 7c00 6a06 6606 4400 5d0d 7d02  |.j.|.j.f.D.].}.
+000002d0: 7c02 6400 7500 721a 0100 6e06 7c01 a007  |.d.u.r...n.|...
+000002e0: 7c02 a101 0100 7112 6401 a008 7c01 a101  |.....q.d...|...
+000002f0: 5300 2902 4e7a 022c 2029 09da 0570 7479  S.).Nz., )...pty
+00000300: 7065 da02 7630 da02 7631 da02 7632 da02  pe..v0..v1..v2..
+00000310: 7633 da02 7634 da02 7635 da06 6170 7065  v3..v4..v5..appe
+00000320: 6e64 da04 6a6f 696e 2903 da04 7365 6c66  nd..join)...self
+00000330: da03 6172 72da 0176 a900 721e 0000 00fa  ..arr..v..r.....
+00000340: 3f45 3a5c 636f 6465 6465 6d6f 5c49 5241  ?E:\codedemo\IRA
+00000350: 494c 535c 6972 6169 6c73 5c63 6173 6269  ILS\irails\casbi
+00000360: 6e5f 6164 6170 7465 7273 5c73 716c 616c  n_adapters\sqlal
+00000370: 6368 656d 795f 6164 6170 7465 722e 7079  chemy_adapter.py
+00000380: da07 5f5f 7374 725f 5f1f 0000 0073 0c00  ..__str__....s..
+00000390: 0000 0801 2001 0801 0401 0c01 0a01 7a12  .... .........z.
+000003a0: 4361 7362 696e 5275 6c65 2e5f 5f73 7472  CasbinRule.__str
+000003b0: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+000003c0: 0000 0005 0000 0043 0000 0073 1200 0000  .......C...s....
+000003d0: 6401 a000 7c00 6a01 7402 7c00 8301 a102  d...|.j.t.|.....
+000003e0: 5300 2902 4e7a 153c 4361 7362 696e 5275  S.).Nz.<CasbinRu
+000003f0: 6c65 207b 7d3a 2022 7b7d 223e 2903 da06  le {}: "{}">)...
+00000400: 666f 726d 6174 da02 6964 da03 7374 72a9  format..id..str.
+00000410: 0172 1b00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000420: 721f 0000 00da 085f 5f72 6570 725f 5f27  r......__repr__'
+00000430: 0000 0073 0200 0000 1201 7a13 4361 7362  ...s......z.Casb
+00000440: 696e 5275 6c65 2e5f 5f72 6570 725f 5f4e  inRule.__repr__N
+00000450: 2914 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000460: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000470: 6e61 6d65 5f5f da0f 6578 7465 6e64 5f65  name__..extend_e
+00000480: 7869 7374 696e 67da 0a72 756c 655f 7461  xisting..rule_ta
+00000490: 626c 65da 0d5f 5f74 6162 6c65 6e61 6d65  ble..__tablename
+000004a0: 5f5f da0a 5f5f 7379 7374 656d 5f5f 7205  __..__system__r.
+000004b0: 0000 0072 0600 0000 7222 0000 0072 0700  ...r....r"...r..
+000004c0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+000004d0: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+000004e0: 7218 0000 0072 2000 0000 7225 0000 0072  r....r ...r%...r
+000004f0: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00000500: 0000 0072 0f00 0000 1200 0000 731c 0000  ...r........s...
+00000510: 0008 0004 0104 0104 010c 010c 010c 010c  ................
+00000520: 010c 010c 010c 010c 0108 020c 0872 0f00  .............r..
+00000530: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000540: 0000 0001 0000 0040 0000 0073 2800 0000  .......@...s(...
+00000550: 6500 5a01 6400 5a02 6700 5a03 6700 5a04  e.Z.d.Z.g.Z.g.Z.
+00000560: 6700 5a05 6700 5a06 6700 5a07 6700 5a08  g.Z.g.Z.g.Z.g.Z.
+00000570: 6700 5a09 6401 5300 2902 da06 4669 6c74  g.Z.d.S.)...Filt
+00000580: 6572 4e29 0a72 2600 0000 7227 0000 0072  erN).r&...r'...r
+00000590: 2800 0000 7212 0000 0072 1300 0000 7214  (...r....r....r.
+000005a0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
+000005b0: 0000 7218 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+000005c0: 0072 1e00 0000 721f 0000 0072 2d00 0000  .r....r....r-...
+000005d0: 2b00 0000 7310 0000 0008 0004 0104 0104  +...s...........
+000005e0: 0104 0104 0104 0108 0172 2d00 0000 6300  .........r-...c.
+000005f0: 0000 0000 0000 0000 0000 0000 0000 000a  ................
+00000600: 0000 0040 0000 0073 1001 0000 6500 5a01  ...@...s....e.Z.
+00000610: 6400 5a02 6401 5a03 642d 6404 6405 8401  d.Z.d.Z.d-d.d...
+00000620: 5a04 6505 6406 6407 8400 8301 5a06 6408  Z.e.d.d.....Z.d.
+00000630: 6409 8400 5a07 640a 640b 8400 5a08 642e  d...Z.d.d...Z.d.
+00000640: 640d 640e 8404 5a09 640f 6410 8400 5a0a  d.d...Z.d.d...Z.
+00000650: 6411 6412 8400 5a0b 6413 6414 8400 5a0c  d.d...Z.d.d...Z.
+00000660: 6415 6416 8400 5a0d 6417 6418 8400 5a0e  d.d...Z.d.d...Z.
+00000670: 6419 641a 8400 5a0f 641b 641c 8400 5a10  d.d...Z.d.d...Z.
+00000680: 641d 641e 8400 5a11 641f 6512 6420 6512  d.d...Z.d.e.d e.
+00000690: 6421 6513 6512 1900 6422 6513 6512 1900  d!e.e...d"e.e...
+000006a0: 640c 6402 660a 6423 6424 8404 5a14 641f  d.d.f.d#d$..Z.d.
+000006b0: 6512 6420 6512 6425 6513 6513 6512 1900  e.d e.d%e.e.e...
+000006c0: 6601 1900 6426 6513 6513 6512 1900 6601  f...d&e.e.e...f.
+000006d0: 1900 640c 6402 660a 6427 6428 8404 5a15  ..d.d.f.d'd(..Z.
+000006e0: 6426 6513 6513 6512 1900 1900 640c 6513  d&e.e.e.....d.e.
+000006f0: 6513 6512 1900 1900 6604 6429 642a 8404  e.e.....f.d)d*..
+00000700: 5a16 640c 6513 6513 6512 1900 1900 6602  Z.d.e.e.e.....f.
+00000710: 642b 642c 8404 5a17 6402 5300 292f da07  d+d,..Z.d.S.)/..
+00000720: 4164 6170 7465 727a 2274 6865 2069 6e74  Adapterz"the int
+00000730: 6572 6661 6365 2066 6f72 2043 6173 6269  erface for Casbi
+00000740: 6e20 6164 6170 7465 7273 2e4e 4663 0400  n adapters.NFc..
+00000750: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00000760: 0000 4300 0000 7384 0000 0074 007c 0174  ..C...s....t.|.t
+00000770: 0183 0272 187c 0174 0174 026a 036a 0483  ...r.|.t.t.j.j..
+00000780: 016b 0272 1274 026a 037c 005f 056e 0974  .k.r.t.j.|._.n.t
+00000790: 067c 0183 017c 005f 056e 037c 017c 005f  .|...|._.n.|.|._
+000007a0: 057c 0264 0075 0072 2274 077d 026e 1164  .|.d.u.r"t.}.n.d
+000007b0: 0144 005d 0e7d 0474 087c 027c 0483 0273  .D.].}.t.|.|...s
+000007c0: 3274 097c 049b 0064 029d 0283 0182 0171  2t.|...d.......q
+000007d0: 247c 027c 005f 0a74 0b7c 006a 0564 038d  $|.|._.t.|.j.d..
+000007e0: 017c 005f 0c7c 037c 005f 0d64 0053 0029  .|._.|.|._.d.S.)
+000007f0: 044e 2908 7222 0000 0072 1200 0000 7213  .N).r"...r....r.
+00000800: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00000810: 0000 7217 0000 0072 1800 0000 7a23 206e  ..r....r....z# n
+00000820: 6f74 2066 6f75 6e64 2069 6e20 6375 7374  ot found in cust
+00000830: 6f6d 2044 6174 6162 6173 6543 6c61 7373  om DatabaseClass
+00000840: 2e29 01da 0462 696e 6429 0eda 0a69 7369  .)...bind)...isi
+00000850: 6e73 7461 6e63 6572 2300 0000 720c 0000  nstancer#...r...
+00000860: 00da 0665 6e67 696e 65da 0375 726c 5a07  ...engine..urlZ.
+00000870: 5f65 6e67 696e 6572 0800 0000 720f 0000  _enginer....r...
+00000880: 00da 0768 6173 6174 7472 da09 4578 6365  ...hasattr..Exce
+00000890: 7074 696f 6eda 095f 6462 5f63 6c61 7373  ption.._db_class
+000008a0: 720b 0000 00da 0d73 6573 7369 6f6e 5f6c  r......session_l
+000008b0: 6f63 616c da09 5f66 696c 7465 7265 6429  ocal.._filtered)
+000008c0: 0572 1b00 0000 5a0a 656e 6769 6e65 5f75  .r....Z.engine_u
+000008d0: 7269 5a08 6462 5f63 6c61 7373 da08 6669  riZ.db_class..fi
+000008e0: 6c74 6572 6564 da04 6174 7472 721e 0000  ltered..attrr...
+000008f0: 0072 1e00 0000 721f 0000 00da 085f 5f69  .r....r......__i
+00000900: 6e69 745f 5f38 0000 0073 1c00 0000 0a02  nit__8...s......
+00000910: 1001 0a01 0c02 0602 0802 0601 0802 0a0a  ................
+00000920: 0e01 02ff 0604 0e01 0a03 7a10 4164 6170  ..........z.Adap
+00000930: 7465 722e 5f5f 696e 6974 5f5f 6301 0000  ter.__init__c...
+00000940: 0000 0000 0000 0000 0003 0000 000a 0000  ................
+00000950: 0063 0000 0073 5c00 0000 8100 7c00 a000  .c...s\.....|...
+00000960: a100 7d01 7a23 7a09 7c01 5600 0100 7c01  ..}.z#z.|.V...|.
+00000970: a001 a100 0100 5700 6e12 0400 7402 7921  ......W.n...t.y!
+00000980: 0100 7d02 0100 7a06 7c01 a003 a100 0100  ..}...z.|.......
+00000990: 7c02 8201 6401 7d02 7e02 7701 7700 5700  |...d.}.~.w.w.W.
+000009a0: 7c01 a004 a100 0100 6401 5300 7c01 a004  |.......d.S.|...
+000009b0: a100 0100 7700 2902 7a3c 5072 6f76 6964  ....w.).z<Provid
+000009c0: 6520 6120 7472 616e 7361 6374 696f 6e61  e a transactiona
+000009d0: 6c20 7363 6f70 6520 6172 6f75 6e64 2061  l scope around a
+000009e0: 2073 6572 6965 7320 6f66 206f 7065 7261   series of opera
+000009f0: 7469 6f6e 732e 4e29 0572 3600 0000 da06  tions.N).r6.....
+00000a00: 636f 6d6d 6974 7234 0000 00da 0872 6f6c  commitr4.....rol
+00000a10: 6c62 6163 6bda 0563 6c6f 7365 2903 721b  lback..close).r.
+00000a20: 0000 00da 0773 6573 7369 6f6e da01 6572  .....session..er
+00000a30: 1e00 0000 721e 0000 0072 1f00 0000 da0e  ....r....r......
+00000a40: 5f73 6573 7369 6f6e 5f73 636f 7065 5900  _session_scopeY.
+00000a50: 0000 7318 0000 0002 8008 0304 0106 010c  ..s.............
+00000a60: 010e 0108 0104 0108 8002 fe02 ff16 057a  ...............z
+00000a70: 1641 6461 7074 6572 2e5f 7365 7373 696f  .Adapter._sessio
+00000a80: 6e5f 7363 6f70 6563 0200 0000 0000 0000  n_scopec........
+00000a90: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
+00000aa0: 7358 0000 007c 00a0 00a1 008f 1e7d 027c  sX...|.......}.|
+00000ab0: 02a0 017c 006a 02a1 01a0 03a1 007d 037c  ...|.j.......}.|
+00000ac0: 0344 005d 0a7d 0474 04a0 0574 067c 0483  .D.].}.t...t.|..
+00000ad0: 017c 01a1 0201 0071 0f57 0064 0104 0004  .|.....q.W.d....
+00000ae0: 0083 0301 0064 0153 0031 0073 2577 0101  .....d.S.1.s%w..
+00000af0: 0001 0001 0059 0001 0064 0153 0029 02fa  .....Y...d.S.)..
+00000b00: 286c 6f61 6473 2061 6c6c 2070 6f6c 6963  (loads all polic
+00000b10: 7920 7275 6c65 7320 6672 6f6d 2074 6865  y rules from the
+00000b20: 2073 746f 7261 6765 2e4e 2907 7240 0000   storage.N).r@..
+00000b30: 00da 0571 7565 7279 7235 0000 00da 0361  ...queryr5.....a
+00000b40: 6c6c 7204 0000 00da 106c 6f61 645f 706f  llr......load_po
+00000b50: 6c69 6379 5f6c 696e 6572 2300 0000 2905  licy_liner#...).
+00000b60: 721b 0000 00da 056d 6f64 656c 723e 0000  r......modelr>..
+00000b70: 00da 056c 696e 6573 da04 6c69 6e65 721e  ...lines..liner.
+00000b80: 0000 0072 1e00 0000 721f 0000 00da 0b6c  ...r....r......l
+00000b90: 6f61 645f 706f 6c69 6379 6600 0000 730c  oad_policyf...s.
+00000ba0: 0000 000a 0210 0108 0112 0102 ff22 fe7a  .............".z
+00000bb0: 1341 6461 7074 6572 2e6c 6f61 645f 706f  .Adapter.load_po
+00000bc0: 6c69 6379 6301 0000 0000 0000 0000 0000  licyc...........
+00000bd0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+00000be0: 0000 7c00 6a00 5300 2901 4e29 0172 3700  ..|.j.S.).N).r7.
+00000bf0: 0000 7224 0000 0072 1e00 0000 721e 0000  ..r$...r....r...
+00000c00: 0072 1f00 0000 da0b 6973 5f66 696c 7465  .r......is_filte
+00000c10: 7265 646d 0000 0073 0200 0000 0601 7a13  redm...s......z.
+00000c20: 4164 6170 7465 722e 6973 5f66 696c 7465  Adapter.is_filte
+00000c30: 7265 64da 0672 6574 7572 6e63 0300 0000  red..returnc....
+00000c40: 0000 0000 0000 0000 0700 0000 0800 0000  ................
+00000c50: 4300 0000 736e 0000 007c 00a0 00a1 008f  C...sn...|......
+00000c60: 297d 037c 03a0 017c 006a 02a1 017d 047c  )}.|...|.j...}.|
+00000c70: 00a0 037c 047c 02a1 027d 057c 05a0 04a1  ...|.|...}.|....
+00000c80: 007d 057c 0544 005d 0a7d 0674 05a0 0674  .}.|.D.].}.t...t
+00000c90: 077c 0683 017c 01a1 0201 0071 1764 017c  .|...|.....q.d.|
+00000ca0: 005f 0857 0064 0204 0004 0083 0301 0064  ._.W.d.........d
+00000cb0: 0253 0031 0073 3077 0101 0001 0001 0059  .S.1.s0w.......Y
+00000cc0: 0001 0064 0253 0029 0372 4100 0000 544e  ...d.S.).rA...TN
+00000cd0: 2909 7240 0000 0072 4200 0000 7235 0000  ).r@...rB...r5..
+00000ce0: 00da 0c66 696c 7465 725f 7175 6572 7972  ...filter_queryr
+00000cf0: 4300 0000 7204 0000 0072 4400 0000 7223  C...r....rD...r#
+00000d00: 0000 0072 3700 0000 2907 721b 0000 0072  ...r7...).r....r
+00000d10: 4500 0000 da06 6669 6c74 6572 723e 0000  E.....filterr>..
+00000d20: 0072 4200 0000 da07 6669 6c74 6572 7372  .rB.....filtersr
+00000d30: 4700 0000 721e 0000 0072 1e00 0000 721f  G...r....r....r.
+00000d40: 0000 00da 146c 6f61 645f 6669 6c74 6572  .....load_filter
+00000d50: 6564 5f70 6f6c 6963 7970 0000 0073 1000  ed_policyp...s..
+00000d60: 0000 0a02 0c01 0c01 0801 0802 1201 0801  ................
+00000d70: 22f9 7a1c 4164 6170 7465 722e 6c6f 6164  ".z.Adapter.load
+00000d80: 5f66 696c 7465 7265 645f 706f 6c69 6379  _filtered_policy
+00000d90: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00000da0: 0008 0000 0043 0000 0073 4800 0000 6401  .....C...sH...d.
+00000db0: 4400 5d1a 7d03 7400 7401 7c02 7c03 8302  D.].}.t.t.|.|...
+00000dc0: 8301 6402 6b04 721c 7c01 a002 7401 7c00  ..d.k.r.|...t.|.
+00000dd0: 6a03 7c03 8302 a004 7401 7c02 7c03 8302  j.|.....t.|.|...
+00000de0: a101 a101 7d01 7102 7c01 a005 7c00 6a03  ....}.q.|...|.j.
+00000df0: 6a06 a101 5300 2903 4e29 0772 1200 0000  j...S.).N).r....
+00000e00: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000e10: 1600 0000 7217 0000 0072 1800 0000 7201  ....r....r....r.
+00000e20: 0000 0029 07da 036c 656e da07 6765 7461  ...)...len..geta
+00000e30: 7474 7272 4c00 0000 7235 0000 00da 0369  ttrrL...r5.....i
+00000e40: 6e5f da08 6f72 6465 725f 6279 7222 0000  n_..order_byr"..
+00000e50: 0029 0472 1b00 0000 5a07 7175 6572 7964  .).r....Z.queryd
+00000e60: 6272 4c00 0000 7239 0000 0072 1e00 0000  brL...r9...r....
+00000e70: 721e 0000 0072 1f00 0000 724b 0000 007b  r....r....rK...{
+00000e80: 0000 0073 0e00 0000 0801 1201 0401 1601  ...s............
+00000e90: 04ff 0280 0e03 7a14 4164 6170 7465 722e  ......z.Adapter.
+00000ea0: 6669 6c74 6572 5f71 7565 7279 6303 0000  filter_queryc...
+00000eb0: 0000 0000 0000 0000 0007 0000 0008 0000  ................
+00000ec0: 0043 0000 0073 6800 0000 7c00 a000 a100  .C...sh...|.....
+00000ed0: 8f26 7d03 7c00 6a01 7c01 6401 8d01 7d04  .&}.|.j.|.d...}.
+00000ee0: 7402 7c02 8301 4400 5d0d 5c02 7d05 7d06  t.|...D.].\.}.}.
+00000ef0: 7403 7c04 6402 a004 7c05 a101 7c06 8303  t.|.d...|...|...
+00000f00: 0100 710f 7c03 a005 7c04 a101 0100 5700  ..q.|...|.....W.
+00000f10: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
+00000f20: 732d 7701 0100 0100 0100 5900 0100 6400  s-w.......Y...d.
+00000f30: 5300 2903 4e29 0172 1200 0000 fa03 767b  S.).N).r......v{
+00000f40: 7d29 0672 4000 0000 7235 0000 00da 0965  }).r@...r5.....e
+00000f50: 6e75 6d65 7261 7465 da07 7365 7461 7474  numerate..setatt
+00000f60: 7272 2100 0000 da03 6164 6429 0772 1b00  rr!.....add).r..
+00000f70: 0000 7212 0000 00da 0472 756c 6572 3e00  ..r......ruler>.
+00000f80: 0000 7247 0000 00da 0169 721d 0000 0072  ..rG.....ir....r
+00000f90: 1e00 0000 721e 0000 0072 1f00 0000 da11  ....r....r......
+00000fa0: 5f73 6176 655f 706f 6c69 6379 5f6c 696e  _save_policy_lin
+00000fb0: 6583 0000 0073 0c00 0000 0a01 0c01 1001  e....s..........
+00000fc0: 1401 0c01 22fc 7a19 4164 6170 7465 722e  ....".z.Adapter.
+00000fd0: 5f73 6176 655f 706f 6c69 6379 5f6c 696e  _save_policy_lin
+00000fe0: 6563 0200 0000 0000 0000 0000 0000 0800  ec..............
+00000ff0: 0000 0800 0000 4300 0000 738c 0000 007c  ......C...s....|
+00001000: 00a0 00a1 008f 387d 027c 02a0 017c 006a  ......8}.|...|.j
+00001010: 02a1 017d 037c 03a0 03a1 0001 0064 0144  ...}.|.......d.D
+00001020: 005d 227d 047c 047c 016a 04a0 05a1 0076  .]"}.|.|.j.....v
+00001030: 0172 1b71 117c 016a 047c 0419 00a0 06a1  .r.q.|.j.|......
+00001040: 0044 005d 105c 027d 057d 067c 066a 0744  .D.].\.}.}.|.j.D
+00001050: 005d 087d 077c 00a0 087c 057c 07a1 0201  .].}.|...|.|....
+00001060: 0071 2971 2271 1157 0064 0204 0004 0083  .q)q"q.W.d......
+00001070: 0301 0064 0353 0031 0073 3f77 0101 0001  ...d.S.1.s?w....
+00001080: 0001 0059 0001 0064 0353 0029 047a 2673  ...Y...d.S.).z&s
+00001090: 6176 6573 2061 6c6c 2070 6f6c 6963 7920  aves all policy 
+000010a0: 7275 6c65 7320 746f 2074 6865 2073 746f  rules to the sto
+000010b0: 7261 6765 2e29 02da 0170 da01 674e 5429  rage.)...p..gNT)
+000010c0: 0972 4000 0000 7242 0000 0072 3500 0000  .r@...rB...r5...
+000010d0: da06 6465 6c65 7465 7245 0000 00da 046b  ..deleterE.....k
+000010e0: 6579 73da 0569 7465 6d73 da06 706f 6c69  eys..items..poli
+000010f0: 6379 7259 0000 0029 0872 1b00 0000 7245  cyrY...).r....rE
+00001100: 0000 0072 3e00 0000 7242 0000 00da 0373  ...r>...rB.....s
+00001110: 6563 7212 0000 00da 0361 7374 7257 0000  ecr......astrW..
+00001120: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001130: da0b 7361 7665 5f70 6f6c 6963 798a 0000  ..save_policy...
+00001140: 0073 2000 0000 0a02 0c01 0801 0801 0e01  .s .............
+00001150: 0201 1601 0a01 0e01 02ff 02ff 02fd 0afd  ................
+00001160: 0409 10f7 0409 7a13 4164 6170 7465 722e  ......z.Adapter.
+00001170: 7361 7665 5f70 6f6c 6963 7963 0400 0000  save_policyc....
+00001180: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00001190: 4300 0000 7310 0000 007c 00a0 007c 027c  C...s....|...|.|
+000011a0: 03a1 0201 0064 0153 0029 027a 2261 6464  .....d.S.).z"add
+000011b0: 7320 6120 706f 6c69 6379 2072 756c 6520  s a policy rule 
+000011c0: 746f 2074 6865 2073 746f 7261 6765 2e4e  to the storage.N
+000011d0: a901 7259 0000 0029 0472 1b00 0000 7260  ..rY...).r....r`
+000011e0: 0000 0072 1200 0000 7257 0000 0072 1e00  ...r....rW...r..
+000011f0: 0000 721e 0000 0072 1f00 0000 da0a 6164  ..r....r......ad
+00001200: 645f 706f 6c69 6379 9700 0000 7302 0000  d_policy....s...
+00001210: 0010 027a 1241 6461 7074 6572 2e61 6464  ...z.Adapter.add
+00001220: 5f70 6f6c 6963 7963 0400 0000 0000 0000  _policyc........
+00001230: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
+00001240: 731a 0000 007c 0344 005d 087d 047c 00a0  s....|.D.].}.|..
+00001250: 007c 027c 04a1 0201 0071 0264 0153 0029  .|.|.....q.d.S.)
+00001260: 027a 2361 6464 7320 6120 706f 6c69 6379  .z#adds a policy
+00001270: 2072 756c 6573 2074 6f20 7468 6520 7374   rules to the st
+00001280: 6f72 6167 652e 4e72 6300 0000 2905 721b  orage.Nrc...).r.
+00001290: 0000 0072 6000 0000 7212 0000 00da 0572  ...r`...r......r
+000012a0: 756c 6573 7257 0000 0072 1e00 0000 721e  ulesrW...r....r.
+000012b0: 0000 0072 1f00 0000 da0c 6164 645f 706f  ...r......add_po
+000012c0: 6c69 6369 6573 9b00 0000 7306 0000 0008  licies....s.....
+000012d0: 020e 0104 ff7a 1441 6461 7074 6572 2e61  .....z.Adapter.a
+000012e0: 6464 5f70 6f6c 6963 6965 7363 0400 0000  dd_policiesc....
+000012f0: 0000 0000 0000 0000 0900 0000 0900 0000  ................
+00001300: 4300 0000 738c 0000 007c 00a0 00a1 008f  C...s....|......
+00001310: 327d 047c 04a0 017c 006a 02a1 017d 057c  2}.|...|.j...}.|
+00001320: 05a0 037c 006a 026a 047c 026b 02a1 017d  ...|.j.j.|.k...}
+00001330: 0574 057c 0383 0144 005d 125c 027d 067d  .t.|...D.].\.}.}
+00001340: 077c 05a0 0374 067c 006a 0264 01a0 077c  .|...t.|.j.d...|
+00001350: 06a1 0183 027c 076b 02a1 017d 0571 187c  .....|.k...}.q.|
+00001360: 05a0 08a1 007d 0857 0064 0204 0004 0083  .....}.W.d......
+00001370: 0301 006e 0831 0073 3977 0101 0001 0001  ...n.1.s9w......
+00001380: 0059 0001 007c 0864 036b 0472 4464 0453  .Y...|.d.k.rDd.S
+00001390: 0064 0553 0029 067a 2772 656d 6f76 6573  .d.S.).z'removes
+000013a0: 2061 2070 6f6c 6963 7920 7275 6c65 2066   a policy rule f
+000013b0: 726f 6d20 7468 6520 7374 6f72 6167 652e  rom the storage.
+000013c0: 7253 0000 004e 7201 0000 0054 4629 0972  rS...Nr....TF).r
+000013d0: 4000 0000 7242 0000 0072 3500 0000 724c  @...rB...r5...rL
+000013e0: 0000 0072 1200 0000 7254 0000 0072 5000  ...r....rT...rP.
+000013f0: 0000 7221 0000 0072 5c00 0000 2909 721b  ..r!...r\...).r.
+00001400: 0000 0072 6000 0000 7212 0000 0072 5700  ...r`...r....rW.
+00001410: 0000 723e 0000 0072 4200 0000 7258 0000  ..r>...rB...rX..
+00001420: 0072 1d00 0000 da01 7272 1e00 0000 721e  .r......rr....r.
+00001430: 0000 0072 1f00 0000 da0d 7265 6d6f 7665  ...r......remove
+00001440: 5f70 6f6c 6963 79a0 0000 0073 1000 0000  _policy....s....
+00001450: 0a02 0c01 1201 1001 1e01 0a01 1cfb 1007  ................
+00001460: 7a15 4164 6170 7465 722e 7265 6d6f 7665  z.Adapter.remove
+00001470: 5f70 6f6c 6963 7963 0400 0000 0000 0000  _policyc........
+00001480: 0000 0000 0700 0000 0800 0000 0300 0000  ................
+00001490: 7394 0000 007c 0373 0464 0153 0088 01a0  s....|.s.d.S....
+000014a0: 00a1 008f 387d 047c 04a0 0188 016a 02a1  ....8}.|.....j..
+000014b0: 017d 057c 05a0 0388 016a 026a 047c 026b  .}.|.....j.j.|.k
+000014c0: 02a1 017d 0574 057c 038e 007d 0374 067c  ...}.t.|...}.t.|
+000014d0: 0383 0144 005d 135c 0289 007d 067c 05a0  ...D.].\...}.|..
+000014e0: 0374 0787 0087 0166 0264 0264 0384 087c  .t.....f.d.d...|
+000014f0: 0644 0083 0183 01a1 017d 0571 207c 05a0  .D.......}.q |..
+00001500: 08a1 0001 0057 0064 0104 0004 0083 0301  .....W.d........
+00001510: 0064 0153 0031 0073 4377 0101 0001 0001  .d.S.1.sCw......
+00001520: 0059 0001 0064 0153 0029 047a 2572 656d  .Y...d.S.).z%rem
+00001530: 6f76 6520 706f 6c69 6379 2072 756c 6573  ove policy rules
+00001540: 2066 726f 6d20 7468 6520 7374 6f72 6167   from the storag
+00001550: 652e 4e63 0100 0000 0000 0000 0000 0000  e.Nc............
+00001560: 0200 0000 0600 0000 3300 0000 7326 0000  ........3...s&..
+00001570: 0081 007c 005d 0e7d 0174 0088 016a 0164  ...|.].}.t...j.d
+00001580: 00a0 0288 00a1 0183 027c 016b 0256 0001  .........|.k.V..
+00001590: 0071 0264 0153 0029 0272 5300 0000 4e29  .q.d.S.).rS...N)
+000015a0: 0372 5000 0000 7235 0000 0072 2100 0000  .rP...r5...r!...
+000015b0: 2902 da02 2e30 721d 0000 00a9 0272 5800  )....0r......rX.
+000015c0: 0000 721b 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+000015d0: 00da 093c 6765 6e65 7870 723e b500 0000  ...<genexpr>....
+000015e0: 7304 0000 0002 8024 007a 2a41 6461 7074  s......$.z*Adapt
+000015f0: 6572 2e72 656d 6f76 655f 706f 6c69 6369  er.remove_polici
+00001600: 6573 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  es.<locals>.<gen
+00001610: 6578 7072 3e29 0972 4000 0000 7242 0000  expr>).r@...rB..
+00001620: 0072 3500 0000 724c 0000 0072 1200 0000  .r5...rL...r....
+00001630: da03 7a69 7072 5400 0000 7209 0000 0072  ..ziprT...r....r
+00001640: 5c00 0000 2907 721b 0000 0072 6000 0000  \...).r....r`...
+00001650: 7212 0000 0072 6500 0000 723e 0000 0072  r....re...r>...r
+00001660: 4200 0000 7257 0000 0072 1e00 0000 726a  B...rW...r....rj
+00001670: 0000 0072 1f00 0000 da0f 7265 6d6f 7665  ...r......remove
+00001680: 5f70 6f6c 6963 6965 73ab 0000 0073 1800  _policies....s..
+00001690: 0000 0402 0401 0a01 0c01 1201 0801 1001  ................
+000016a0: 0401 1601 06ff 0a03 22f8 7a17 4164 6170  ........".z.Adap
+000016b0: 7465 722e 7265 6d6f 7665 5f70 6f6c 6963  ter.remove_polic
+000016c0: 6965 7363 0400 0000 0000 0000 0000 0000  iesc............
+000016d0: 0b00 0000 0800 0000 4700 0000 73f0 0000  ........G...s...
+000016e0: 007c 00a0 00a1 008f 647d 057c 05a0 017c  .|......d}.|...|
+000016f0: 006a 02a1 01a0 037c 006a 026a 047c 026b  .j.....|.j.j.|.k
+00001700: 02a1 017d 0664 017c 0304 0003 006b 0172  ...}.d.|.....k.r
+00001710: 1c64 026b 0173 266e 0101 0009 0057 0064  .d.k.s&n.....W.d
+00001720: 0304 0004 0083 0301 0064 0453 0064 057c  .........d.S.d.|
+00001730: 0374 057c 0483 0117 0004 0003 006b 0172  .t.|.........k.r
+00001740: 3464 066b 0173 3e6e 0101 0009 0057 0064  4d.k.s>n.....W.d
+00001750: 0304 0004 0083 0301 0064 0453 0074 067c  .........d.S.t.|
+00001760: 0483 0144 005d 1a5c 027d 077d 087c 0864  ...D.].\.}.}.|.d
+00001770: 076b 0372 5c74 077c 006a 0264 08a0 087c  .k.r\t.|.j.d...|
+00001780: 037c 0717 00a1 0183 027d 097c 06a0 037c  .|.......}.|...|
+00001790: 097c 086b 02a1 017d 0671 427c 06a0 09a1  .|.k...}.qB|....
+000017a0: 007d 0a57 0064 0304 0004 0083 0301 006e  .}.W.d.........n
+000017b0: 0831 0073 6b77 0101 0001 0001 0059 0001  .1.skw.......Y..
+000017c0: 007c 0a64 016b 0472 7664 0953 0064 0453  .|.d.k.rvd.S.d.S
+000017d0: 0029 0a7a 7472 656d 6f76 6573 2070 6f6c  .).ztremoves pol
+000017e0: 6963 7920 7275 6c65 7320 7468 6174 206d  icy rules that m
+000017f0: 6174 6368 2074 6865 2066 696c 7465 7220  atch the filter 
+00001800: 6672 6f6d 2074 6865 2073 746f 7261 6765  from the storage
+00001810: 2e0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00001820: 7320 7061 7274 206f 6620 7468 6520 4175  s part of the Au
+00001830: 746f 2d53 6176 6520 6665 6174 7572 652e  to-Save feature.
+00001840: 0a20 2020 2020 2020 2072 0100 0000 e905  .        r......
+00001850: 0000 004e 46e9 0100 0000 e906 0000 00da  ...NF...........
+00001860: 0072 5300 0000 5429 0a72 4000 0000 7242  .rS...T).r@...rB
+00001870: 0000 0072 3500 0000 724c 0000 0072 1200  ...r5...rL...r..
+00001880: 0000 724f 0000 0072 5400 0000 7250 0000  ..rO...rT...rP..
+00001890: 0072 2100 0000 725c 0000 0029 0b72 1b00  .r!...r\...).r..
+000018a0: 0000 7260 0000 0072 1200 0000 da0b 6669  ..r`...r......fi
+000018b0: 656c 645f 696e 6465 78da 0c66 6965 6c64  eld_index..field
+000018c0: 5f76 616c 7565 7372 3e00 0000 7242 0000  _valuesr>...rB..
+000018d0: 0072 5800 0000 721d 0000 00da 0776 5f76  .rX...r......v_v
+000018e0: 616c 7565 7267 0000 0072 1e00 0000 721e  aluerg...r....r.
+000018f0: 0000 0072 1f00 0000 da16 7265 6d6f 7665  ...r......remove
+00001900: 5f66 696c 7465 7265 645f 706f 6c69 6379  _filtered_policy
+00001910: b900 0000 7320 0000 000a 041a 0116 0202  ....s ..........
+00001920: 0110 fc1e 0502 0110 fa10 0708 0116 010e  ................
+00001930: 0102 800a 011c f510 0d7a 1e41 6461 7074  .........z.Adapt
+00001940: 6572 2e72 656d 6f76 655f 6669 6c74 6572  er.remove_filter
+00001950: 6564 5f70 6f6c 6963 7972 6000 0000 7212  ed_policyr`...r.
+00001960: 0000 00da 086f 6c64 5f72 756c 65da 086e  .....old_rule..n
+00001970: 6577 5f72 756c 6563 0500 0000 0000 0000  ew_rulec........
+00001980: 0000 0000 0c00 0000 0800 0000 4300 0000  ............C...
+00001990: 73e0 0000 007c 00a0 00a1 008f 627d 057c  s....|......b}.|
+000019a0: 05a0 017c 006a 02a1 01a0 037c 006a 026a  ...|.j.....|.j.j
+000019b0: 047c 026b 02a1 017d 0674 057c 0383 0144  .|.k...}.t.|...D
+000019c0: 005d 145c 027d 077d 0874 067c 006a 0264  .].\.}.}.t.|.j.d
+000019d0: 01a0 077c 07a1 0183 027d 097c 06a0 037c  ...|.....}.|...|
+000019e0: 097c 086b 02a1 017d 0671 1674 087c 0383  .|.k...}.q.t.|..
+000019f0: 0174 087c 0483 016b 0472 357c 036e 017c  .t.|...k.r5|.n.|
+00001a00: 047d 0a7c 06a0 09a1 007d 0b74 0a74 087c  .}.|.....}.t.t.|
+00001a10: 0a83 0183 0144 005d 1c7d 077c 0774 087c  .....D.].}.|.t.|
+00001a20: 0483 016b 0072 5574 0b64 027c 079b 0064  ...k.rUt.d.|...d
+00001a30: 037c 079b 0064 049d 0583 0101 0071 4174  .|...d.......qAt
+00001a40: 0b64 027c 079b 0064 059d 0383 0101 0071  .d.|...d.......q
+00001a50: 4157 0064 0604 0004 0083 0301 0064 0653  AW.d.........d.S
+00001a60: 0031 0073 6977 0101 0001 0001 0059 0001  .1.siw.......Y..
+00001a70: 0064 0653 0029 0761 2b01 0000 0a20 2020  .d.S.).a+....   
+00001a80: 2020 2020 2055 7064 6174 6520 7468 6520       Update the 
+00001a90: 6f6c 645f 7275 6c65 2077 6974 6820 7468  old_rule with th
+00001aa0: 6520 6e65 775f 7275 6c65 2069 6e20 7468  e new_rule in th
+00001ab0: 6520 6461 7461 6261 7365 2028 7374 6f72  e database (stor
+00001ac0: 6167 6529 2e0a 0a20 2020 2020 2020 203a  age)...        :
+00001ad0: 7061 7261 6d20 7365 633a 2073 6563 7469  param sec: secti
+00001ae0: 6f6e 2074 7970 650a 2020 2020 2020 2020  on type.        
+00001af0: 3a70 6172 616d 2070 7479 7065 3a20 706f  :param ptype: po
+00001b00: 6c69 6379 2074 7970 650a 2020 2020 2020  licy type.      
+00001b10: 2020 3a70 6172 616d 206f 6c64 5f72 756c    :param old_rul
+00001b20: 653a 2074 6865 206f 6c64 2072 756c 6520  e: the old rule 
+00001b30: 7468 6174 206e 6565 6473 2074 6f20 6265  that needs to be
+00001b40: 206d 6f64 6966 6965 640a 2020 2020 2020   modified.      
+00001b50: 2020 3a70 6172 616d 206e 6577 5f72 756c    :param new_rul
+00001b60: 653a 2074 6865 206e 6577 2072 756c 6520  e: the new rule 
+00001b70: 746f 2072 6570 6c61 6365 2074 6865 206f  to replace the o
+00001b80: 6c64 2072 756c 650a 0a20 2020 2020 2020  ld rule..       
+00001b90: 203a 7265 7475 726e 3a20 4e6f 6e65 0a20   :return: None. 
+00001ba0: 2020 2020 2020 2072 5300 0000 7a0f 6f6c         rS...z.ol
+00001bb0: 645f 7275 6c65 5f6c 696e 652e 767a 0c20  d_rule_line.vz. 
+00001bc0: 3d20 6e65 775f 7275 6c65 5bda 015d 7a07  = new_rule[..]z.
+00001bd0: 203d 204e 6f6e 654e 290c 7240 0000 0072   = NoneN).r@...r
+00001be0: 4200 0000 7235 0000 0072 4c00 0000 7212  B...r5...rL...r.
+00001bf0: 0000 0072 5400 0000 7250 0000 0072 2100  ...rT...rP...r!.
+00001c00: 0000 724f 0000 00da 036f 6e65 da05 7261  ..rO.....one..ra
+00001c10: 6e67 65da 0465 7865 6329 0c72 1b00 0000  nge..exec).r....
+00001c20: 7260 0000 0072 1200 0000 7276 0000 0072  r`...r....rv...r
+00001c30: 7700 0000 723e 0000 0072 4200 0000 da05  w...r>...rB.....
+00001c40: 696e 6465 78da 0576 616c 7565 7274 0000  index..valuert..
+00001c50: 005a 0c6c 6f6e 6765 7374 5f72 756c 655a  .Z.longest_ruleZ
+00001c60: 0d6f 6c64 5f72 756c 655f 6c69 6e65 721e  .old_rule_liner.
+00001c70: 0000 0072 1e00 0000 721f 0000 00da 0d75  ...r....r......u
+00001c80: 7064 6174 655f 706f 6c69 6379 cc00 0000  pdate_policy....
+00001c90: 731a 0000 000a 0e1a 0110 0312 0110 0118  s...............
+00001ca0: 0308 0110 030c 0118 0112 0202 fc22 f37a  .............".z
+00001cb0: 1541 6461 7074 6572 2e75 7064 6174 655f  .Adapter.update_
+00001cc0: 706f 6c69 6379 da09 6f6c 645f 7275 6c65  policy..old_rule
+00001cd0: 73da 096e 6577 5f72 756c 6573 6305 0000  s..new_rulesc...
+00001ce0: 0000 0000 0000 0000 0006 0000 0008 0000  ................
+00001cf0: 0043 0000 0073 2e00 0000 7400 7401 7c03  .C...s....t.t.|.
+00001d00: 8301 8301 4400 5d0e 7d05 7c00 a002 7c01  ....D.].}.|...|.
+00001d10: 7c02 7c03 7c05 1900 7c04 7c05 1900 a104  |.|.|...|.|.....
+00001d20: 0100 7106 6401 5300 2902 6131 0100 000a  ..q.d.S.).a1....
+00001d30: 2020 2020 2020 2020 5570 6461 7465 2074          Update t
+00001d40: 6865 206f 6c64 5f72 756c 6573 2077 6974  he old_rules wit
+00001d50: 6820 7468 6520 6e65 775f 7275 6c65 7320  h the new_rules 
+00001d60: 696e 2074 6865 2064 6174 6162 6173 6520  in the database 
+00001d70: 2873 746f 7261 6765 292e 0a0a 2020 2020  (storage)...    
+00001d80: 2020 2020 3a70 6172 616d 2073 6563 3a20      :param sec: 
+00001d90: 7365 6374 696f 6e20 7479 7065 0a20 2020  section type.   
+00001da0: 2020 2020 203a 7061 7261 6d20 7074 7970       :param ptyp
+00001db0: 653a 2070 6f6c 6963 7920 7479 7065 0a20  e: policy type. 
+00001dc0: 2020 2020 2020 203a 7061 7261 6d20 6f6c         :param ol
+00001dd0: 645f 7275 6c65 733a 2074 6865 206f 6c64  d_rules: the old
+00001de0: 2072 756c 6573 2074 6861 7420 6e65 6564   rules that need
+00001df0: 2074 6f20 6265 206d 6f64 6966 6965 640a   to be modified.
+00001e00: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
+00001e10: 6577 5f72 756c 6573 3a20 7468 6520 6e65  ew_rules: the ne
+00001e20: 7720 7275 6c65 7320 746f 2072 6570 6c61  w rules to repla
+00001e30: 6365 2074 6865 206f 6c64 2072 756c 6573  ce the old rules
+00001e40: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00001e50: 6e3a 204e 6f6e 650a 2020 2020 2020 2020  n: None.        
+00001e60: 4e29 0372 7a00 0000 724f 0000 0072 7e00  N).rz...rO...r~.
+00001e70: 0000 2906 721b 0000 0072 6000 0000 7212  ..).r....r`...r.
+00001e80: 0000 0072 7f00 0000 7280 0000 0072 5800  ...r....r....rX.
+00001e90: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00001ea0: 00da 0f75 7064 6174 655f 706f 6c69 6369  ...update_polici
+00001eb0: 6573 ed00 0000 7306 0000 0010 151a 0104  es....s.........
+00001ec0: ff7a 1741 6461 7074 6572 2e75 7064 6174  .z.Adapter.updat
+00001ed0: 655f 706f 6c69 6369 6573 6305 0000 0000  e_policiesc.....
+00001ee0: 0000 0000 0000 0008 0000 0007 0000 0047  ...............G
+00001ef0: 0000 0073 6200 0000 7400 8300 7d06 7c02  ...sb...t...}.|.
+00001f00: 7c06 5f01 7402 7403 7c05 8301 8301 4400  |._.t.t.|.....D.
+00001f10: 5d1c 7d07 7c04 7c07 6b01 7228 7c07 7c04  ].}.|.|.k.r(|.|.
+00001f20: 7403 7c05 8301 1700 6b00 7228 7404 7c06  t.|.....k.r(t.|.
+00001f30: 6401 7c07 9b00 9d02 7c05 7c07 7c04 1800  d.|.....|.|.|...
+00001f40: 1900 8303 0100 710c 0100 7c00 a005 7c03  ......q...|...|.
+00001f50: 7c06 a102 0100 6402 5300 2903 7a4d 7570  |.....d.S.).zMup
+00001f60: 6461 7465 5f66 696c 7465 7265 645f 706f  date_filtered_po
+00001f70: 6c69 6369 6573 2075 7064 6174 6573 2061  licies updates a
+00001f80: 6c6c 2074 6865 2070 6f6c 6963 6965 7320  ll the policies 
+00001f90: 6f6e 2074 6865 2062 6173 6973 206f 6620  on the basis of 
+00001fa0: 7468 6520 6669 6c74 6572 2e72 1d00 0000  the filter.r....
+00001fb0: 4e29 0672 2d00 0000 7212 0000 0072 7a00  N).r-...r....rz.
+00001fc0: 0000 724f 0000 0072 5500 0000 da19 5f75  ..rO...rU....._u
+00001fd0: 7064 6174 655f 6669 6c74 6572 6564 5f70  pdate_filtered_p
+00001fe0: 6f6c 6963 6965 7329 0872 1b00 0000 7260  olicies).r....r`
+00001ff0: 0000 0072 1200 0000 7280 0000 0072 7200  ...r....r....rr.
+00002000: 0000 7273 0000 0072 4c00 0000 7258 0000  ..rs...rL...rX..
+00002010: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00002020: da18 7570 6461 7465 5f66 696c 7465 7265  ..update_filtere
+00002030: 645f 706f 6c69 6369 6573 0501 0000 730e  d_policies....s.
+00002040: 0000 0006 0506 0110 0318 011c 0102 0210  ................
+00002050: 027a 2041 6461 7074 6572 2e75 7064 6174  .z Adapter.updat
+00002060: 655f 6669 6c74 6572 6564 5f70 6f6c 6963  e_filtered_polic
+00002070: 6965 7363 0300 0000 0000 0000 0000 0000  iesc............
+00002080: 0700 0000 0800 0000 4300 0000 7380 0000  ........C...s...
+00002090: 007c 00a0 00a1 008f 327d 037c 03a0 017c  .|......2}.|...|
+000020a0: 006a 02a1 01a0 037c 006a 026a 047c 026a  .j.....|.j.j.|.j
+000020b0: 046b 02a1 017d 047c 00a0 057c 047c 02a1  .k...}.|...|.|..
+000020c0: 027d 057c 05a0 06a1 007d 067c 00a0 0764  .}.|.....}.|...d
+000020d0: 017c 026a 047c 06a1 0301 007c 00a0 0864  .|.j.|.....|...d
+000020e0: 017c 026a 047c 01a1 0301 007c 0657 0002  .|.j.|.....|.W..
+000020f0: 0064 0204 0004 0083 0301 0053 0031 0073  .d.........S.1.s
+00002100: 3977 0101 0001 0001 0059 0001 0064 0253  9w.......Y...d.S
+00002110: 0029 037a 4e5f 7570 6461 7465 5f66 696c  .).zN_update_fil
+00002120: 7465 7265 645f 706f 6c69 6369 6573 2075  tered_policies u
+00002130: 7064 6174 6573 2061 6c6c 2074 6865 2070  pdates all the p
+00002140: 6f6c 6963 6965 7320 6f6e 2074 6865 2062  olicies on the b
+00002150: 6173 6973 206f 6620 7468 6520 6669 6c74  asis of the filt
+00002160: 6572 2e72 5a00 0000 4e29 0972 4000 0000  er.rZ...N).r@...
+00002170: 7242 0000 0072 3500 0000 724c 0000 0072  rB...r5...rL...r
+00002180: 1200 0000 724b 0000 0072 4300 0000 726d  ....rK...rC...rm
+00002190: 0000 0072 6600 0000 2907 721b 0000 0072  ...rf...).r....r
+000021a0: 8000 0000 724c 0000 0072 3e00 0000 7242  ....rL...r>...rB
+000021b0: 0000 005a 0e66 696c 7465 7265 645f 7175  ...Z.filtered_qu
+000021c0: 6572 7972 7f00 0000 721e 0000 0072 1e00  eryr....r....r..
+000021d0: 0000 721f 0000 0072 8200 0000 1601 0000  ..r....r........
+000021e0: 7314 0000 000a 030c 040c 0104 ff0c 0308  s...............
+000021f0: 0110 0410 0402 0424 ec7a 2141 6461 7074  .......$.z!Adapt
+00002200: 6572 2e5f 7570 6461 7465 5f66 696c 7465  er._update_filte
+00002210: 7265 645f 706f 6c69 6369 6573 2902 4e46  red_policies).NF
+00002220: 2902 724a 0000 004e 2918 7226 0000 0072  ).rJ...N).r&...r
+00002230: 2700 0000 7228 0000 00da 075f 5f64 6f63  '...r(.....__doc
+00002240: 5f5f 723a 0000 0072 0200 0000 7240 0000  __r:...r....r@..
+00002250: 0072 4800 0000 7249 0000 0072 4e00 0000  .rH...rI...rN...
+00002260: 724b 0000 0072 5900 0000 7262 0000 0072  rK...rY...rb...r
+00002270: 6400 0000 7266 0000 0072 6800 0000 726d  d...rf...rh...rm
+00002280: 0000 0072 7500 0000 7223 0000 0072 0300  ...ru...r#...r..
+00002290: 0000 727e 0000 0072 8100 0000 7283 0000  ..r~...r....r...
+000022a0: 0072 8200 0000 721e 0000 0072 1e00 0000  .r....r....r....
+000022b0: 721e 0000 0072 1f00 0000 722e 0000 0035  r....r....r....5
+000022c0: 0000 0073 6000 0000 0800 0401 0a02 0221  ...s`..........!
+000022d0: 0a01 080c 0807 0a03 080b 0808 0807 080d  ................
+000022e0: 0804 0805 080b 080e 0213 0201 02ff 0201  ................
+000022f0: 02ff 0601 02ff 0601 02ff 0202 0afe 0221  ...............!
+00002300: 0202 02fe 0203 02fd 0204 0801 02ff 02fc  ................
+00002310: 0207 0801 02ff 02f9 020a 0af6 0218 0a01  ................
+00002320: 02ff 0a02 0afe 1a11 722e 0000 004e 291d  ........r....N).
+00002330: da0a 636f 6e74 6578 746c 6962 7202 0000  ..contextlibr...
+00002340: 00da 0674 7970 696e 6772 0300 0000 da06  ...typingr......
+00002350: 6361 7362 696e 7204 0000 00da 0a73 716c  casbinr......sql
+00002360: 616c 6368 656d 7972 0500 0000 7206 0000  alchemyr....r...
+00002370: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+00002380: 5a1a 7371 6c61 6c63 6865 6d79 2e65 7874  Z.sqlalchemy.ext
+00002390: 2e64 6563 6c61 7261 7469 7665 720a 0000  .declarativer...
+000023a0: 00da 0e73 716c 616c 6368 656d 792e 6f72  ...sqlalchemy.or
+000023b0: 6d72 0b00 0000 da06 6972 6169 6c73 720c  mr......irailsr.
+000023c0: 0000 00da 0d69 7261 696c 732e 636f 6e66  .....irails.conf
+000023d0: 6967 720d 0000 0072 2a00 0000 da03 6765  igr....r*.....ge
+000023e0: 74da 0363 6667 da04 4261 7365 720f 0000  t..cfg..Baser...
+000023f0: 0072 2d00 0000 722e 0000 00da 0861 6461  .r-...r......ada
+00002400: 7074 6572 73da 0d55 7064 6174 6541 6461  pters..UpdateAda
+00002410: 7074 6572 721e 0000 0072 1e00 0000 721e  pterr....r....r.
+00002420: 0000 0072 1f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00002430: 653e 0100 0000 7320 0000 000c 000c 010c  e>....s ........
+00002440: 0214 0110 010c 010c 010c 030c 0104 010a  ................
+00002450: 010c 010c 0112 020e 191c 0a              ...........
```

### Comparing `irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.34/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from irails.config import config
 rule_table = 'casbin_rule'
 cfg = config.get("auth")
 if cfg and 'adapter_table' in cfg:
     rule_table = cfg.get('adapter_table','casbin_rule')
     
 class CasbinRule(database.Base):
+    extend_existing=True
     __tablename__ = rule_table
     __system__ = True
     id = Column(Integer, primary_key=True)
     ptype = Column(String(255))
     v0 = Column(String(255))
     v1 = Column(String(255))
     v2 = Column(String(255))
```

### Comparing `irails-1.3.33/irails/cbv.py` & `irails-1.3.34/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/config.py` & `irails-1.3.34/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/controller_utils.py` & `irails-1.3.34/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/core.py` & `irails-1.3.34/irails/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,23 @@
         self.__app_views_dirs = {} 
         self.routers_map = {}
         self.__apps_dirs = []
         self.__apps = {}
         self.auth_user_class:auth.DomainUser = None
         super().__init__(**kwargs)
 
-    def new_user(self,user:Union[database.Base,str])->auth.DomainUser:
+    async def new_user(self,user:Union[database.Base,str])->auth.DomainUser:
         if not self.auth_user_class:
             raise RuntimeError('application.auth_class is None')
         if isinstance(user,str):
             return self.auth_user_class(username=user)
         elif isinstance(user,database.Base):
-            userobj = self.auth_user_class(user.name)
-            copy_attr(user,userobj,False)
+            userobj:auth.DomainUser = self.auth_user_class(user.name)
+            await copy_attr(user,userobj,False)
+            userobj.set_roles(user.roles) 
             return userobj
     @property
     def apps(self)->Dict:
         return self.__apps
     
     @property
     def app_views_dirs(self)->Dict:
@@ -301,15 +302,15 @@
                 if user and user.is_authenticated: #continue singture 
                     if config.get("session").get('auto_refresh_token',True):
                         application.casbin_auth.create_access_token(user=user, expires_delta=None,request=request)
                  
                 if not ret and not user or not user.is_authenticated: 
                     # _log.debug(_('Failed Auth on type:%s at url:%s') % (auth_type,str(request.url)))
                     if accept_header == "application/json":
-                        return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
+                        return  JSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
                     _auth_url = getattr(application,f"{auth_type}_auth_url") 
 
                     if _auth_url: 
                         if 'flash' not in request.session:
                             request.session['flash']=''
                         if request.session['flash']=="":
```

### Comparing `irails-1.3.33/irails/database.py` & `irails-1.3.34/irails/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
             session.merge(model)
         session.commit()
 
     
     @classmethod
     def execute(cls,cmd:Union[str,TextClause],**kwargs):
         if not isinstance(cmd,TextClause):
-            cmd = text(str)
+            cmd = text(cmd)
         with engine.begin() as conn:
             ret = conn.execute(cmd,**kwargs)
         return ret
     @classmethod
     def get_all_mapped_tables(cls):
         """ for `dbfirst` """
         if DataMap:
```

### Comparing `irails-1.3.33/irails/log.py` & `irails-1.3.34/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/midware.py` & `irails-1.3.34/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/midware_casbin.py` & `irails-1.3.34/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/midware_session.py` & `irails-1.3.34/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/mvc_router.py` & `irails-1.3.34/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_app.py` & `irails-1.3.34/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_controller.py` & `irails-1.3.34/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_i18n.py` & `irails-1.3.34/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_migrate.py` & `irails-1.3.34/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_model.py` & `irails-1.3.34/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_project.py` & `irails-1.3.34/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_run.py` & `irails-1.3.34/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_shell.py` & `irails-1.3.34/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/_test.py` & `irails-1.3.34/irails/scripts/_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,35 +19,49 @@
     for root, dirs, files in os.walk(os.path.join(_root_path,'tests')):
         for file in files:
             name,ext = os.path.splitext(file)
             file_path = os.path.join(root, file)
             if file.endswith('.py') and file.startswith('test_'):
                 all_files[name] = file_path
     return all_files
+
+def do_test_file(app_dir,file_name,print_out=None):
+    if not os.path.isabs(file_name):
+        test_files = _get_tests(app_dir)
+        if file_name in test_files:
+            file_name = test_files[file_name]
+        else:
+            raise FileNotFoundError(file_name)
+    name,ext = os.path.splitext(os.path.basename(file_name))
+
+    app_package = os.path.basename(app_dir)    
+    module = load_module(f"{app_package}.tests.{name}",file_name)
+    
+    if module:
+        
+        set_module_i18n(module,f"{app_package}.tests.{name}")
+        sys.argv = [file_name]
+        kwargs = {'module':module,'exit':False}
+        if print_out:
+            kwargs['buffer']=print_out
+        unittest.main(**kwargs)
+
 def do_test_app(app_dir, print_out=None):
     
     test_files = _get_tests(app_dir)
-    app_package = os.path.basename(app_dir)
+    
     app_package_dir = os.path.dirname(app_dir)
     if not app_package_dir in sys.path:
         sys.path.insert(0,app_package_dir)
     for name in test_files:
         print(f"Starting test {test_files[name]}")
-        module = load_module(f"{app_package}.tests.{name}",test_files[name])
-        
-        if module:
-            
-            set_module_i18n(module,f"{app_package}.tests.{name}")
-            sys.argv = [test_files[name]]
-            kwargs = {'module':module,'exit':False}
-            if print_out:
-                kwargs['buffer']=print_out
-            unittest.main(**kwargs)
+        do_test_file(app_dir, test_files[name])
     
     sys.path.remove(app_package_dir)
+
 def get_all_enabled_apps():
     from irails._loader import _load_apps
     apps = _load_apps(do_load=False)
     return apps
 def do_test_project(print_out=None): 
      
     response = input("Do you want to continue to test all apps? (y/n)")
@@ -67,25 +81,36 @@
      
 def main():
     self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
     parser = argparse.ArgumentParser(
         usage=f"{sys.argv[0]} {self_file} [-h] [--verbose]",
           description='run project or app tests')
     parser.add_argument('-v','--verbose',action='store_true', help="full verbose with testing")  
+    parser.add_argument('args', nargs=argparse.REMAINDER,help="test names in app `tests` dir...")
     args = parser.parse_args()  
     import io
     print_out = io.StringIO() if not args.verbose else None
     if print_out:
         sys.stdout = print_out
         sys.stderr = print_out
     if args.verbose:
-        sys.argv.pop()
+        if '-v' in sys.argv:
+            sys.argv.remove('-v')
+        if '--verbose' in sys.argv:
+            sys.argv.remove('--verbose')
     try:
+        if args.args:
+            for name in args.args:
+                sys.argv.remove(name)
         if is_in_app(curdir):
-            do_test_app(curdir,print_out)
+            if args.args: 
+                for name in args.args:
+                    do_test_file(curdir,name,print_out)
+            else:
+                do_test_app(curdir,print_out)
         elif is_in_irails(curdir):
             do_test_project(print_out)
     except Exception as e:
         raise
     sys.stdout = sys.__stdout__
     sys.stderr = sys.__stderr__
     if not print_out:
```

### Comparing `irails-1.3.33/irails/scripts/main.py` & `irails-1.3.34/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.34/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/app/home.tpl` & `irails-1.3.34/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/app/model.jinja` & `irails-1.3.34/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.34/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.34/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.34/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.34/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.34/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.34/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.34/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails/unit_test.py` & `irails-1.3.34/irails/unit_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,9 +38,9 @@
             db_cfg = config.get("database")
             db_uri = db_cfg.get("uri")
             alembic_ini = db_cfg.get("alembic_ini")
             ServiceTest.engine = init_database(db_uri,debug=True,cfg = db_cfg)
             check_init_auth(db_cfg)
             if ServiceTest.engine:
                 check_migration(engine=ServiceTest.engine,uri= db_uri,alembic_ini= alembic_ini )
-            ServiceTest.service = Service 
+            self.service = Service()
```

### Comparing `irails-1.3.33/irails/view.py` & `irails-1.3.34/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/irails.egg-info/PKG-INFO` & `irails-1.3.34/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.33
+Version: 1.3.34
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.33/irails.egg-info/SOURCES.txt` & `irails-1.3.34/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.33/setup.py` & `irails-1.3.34/setup.py`

 * *Files identical despite different names*

