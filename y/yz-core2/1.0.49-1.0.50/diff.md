# Comparing `tmp/yz-core2-1.0.49.tar.gz` & `tmp/yz-core2-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.49.tar", last modified: Thu May 11 09:21:01 2023, max compression
+gzip compressed data, was "yz-core2-1.0.50.tar", last modified: Mon May 29 05:53:22 2023, max compression
```

## Comparing `yz-core2-1.0.49.tar` & `yz-core2-1.0.50.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.485937 yz-core2-1.0.49/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.49/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-11 09:21:01.485784 yz-core2-1.0.49/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.49/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-11 09:21:01.485978 yz-core2-1.0.49/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-11 09:20:51.000000 yz-core2-1.0.49/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.471148 yz-core2-1.0.49/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.49/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.471948 yz-core2-1.0.49/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-11 09:21:01.000000 yz-core2-1.0.49/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.472978 yz-core2-1.0.49/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.473880 yz-core2-1.0.49/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.474391 yz-core2-1.0.49/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.474965 yz-core2-1.0.49/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.49/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.475558 yz-core2-1.0.49/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2599 2023-05-08 08:37:20.000000 yz-core2-1.0.49/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.49/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.475815 yz-core2-1.0.49/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.476801 yz-core2-1.0.49/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.49/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.477117 yz-core2-1.0.49/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7411 2023-05-11 08:40:13.000000 yz-core2-1.0.49/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10752 2023-05-11 08:37:54.000000 yz-core2-1.0.49/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.49/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.477311 yz-core2-1.0.49/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8216 2023-05-11 08:40:13.000000 yz-core2-1.0.49/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.478249 yz-core2-1.0.49/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.49/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.478718 yz-core2-1.0.49/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.49/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1203 2023-04-24 09:03:30.000000 yz-core2-1.0.49/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.49/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479314 yz-core2-1.0.49/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479562 yz-core2-1.0.49/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.479975 yz-core2-1.0.49/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.480188 yz-core2-1.0.49/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.480958 yz-core2-1.0.49/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481353 yz-core2-1.0.49/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481572 yz-core2-1.0.49/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.481740 yz-core2-1.0.49/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482212 yz-core2-1.0.49/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482342 yz-core2-1.0.49/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.482952 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483404 yz-core2-1.0.49/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483738 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.483917 yz-core2-1.0.49/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-11 09:21:01.485467 yz-core2-1.0.49/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-05-10 06:22:06.000000 yz-core2-1.0.49/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.49/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.49/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.848796 yz-core2-1.0.50/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.50/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-29 05:53:22.848644 yz-core2-1.0.50/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.50/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-29 05:53:22.848836 yz-core2-1.0.50/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-29 05:49:16.000000 yz-core2-1.0.50/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.832580 yz-core2-1.0.50/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.50/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.50/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.50/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.833464 yz-core2-1.0.50/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3409 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-29 05:53:22.000000 yz-core2-1.0.50/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.834422 yz-core2-1.0.50/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.835989 yz-core2-1.0.50/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.836586 yz-core2-1.0.50/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.837064 yz-core2-1.0.50/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1695 2023-05-18 02:53:50.000000 yz-core2-1.0.50/yzcore/core/release.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.50/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.837615 yz-core2-1.0.50/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.50/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.50/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.837958 yz-core2-1.0.50/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.839229 yz-core2-1.0.50/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.50/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.839564 yz-core2-1.0.50/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7411 2023-05-11 08:40:13.000000 yz-core2-1.0.50/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10752 2023-05-11 08:37:54.000000 yz-core2-1.0.50/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.50/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.839782 yz-core2-1.0.50/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9414 2023-05-29 05:47:23.000000 yz-core2-1.0.50/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.840806 yz-core2-1.0.50/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.50/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.50/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.50/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.50/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.841323 yz-core2-1.0.50/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.50/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.50/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1228 2023-05-29 03:14:52.000000 yz-core2-1.0.50/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.50/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.841990 yz-core2-1.0.50/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.842504 yz-core2-1.0.50/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.843004 yz-core2-1.0.50/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.843345 yz-core2-1.0.50/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.844184 yz-core2-1.0.50/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.844646 yz-core2-1.0.50/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.844873 yz-core2-1.0.50/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.845003 yz-core2-1.0.50/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.845361 yz-core2-1.0.50/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.845493 yz-core2-1.0.50/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.846072 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.846489 yz-core2-1.0.50/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.846773 yz-core2-1.0.50/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.846910 yz-core2-1.0.50/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-29 05:53:22.848335 yz-core2-1.0.50/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-05-10 06:22:06.000000 yz-core2-1.0.50/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.50/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.50/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.49/LICENSE` & `yz-core2-1.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/PKG-INFO` & `yz-core2-1.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.49
+Version: 1.0.50
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.49/README.md` & `yz-core2-1.0.50/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/setup.py` & `yz-core2-1.0.50/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.49",
+    version="1.0.50",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.49/tests/test_setting_reload.py` & `yz-core2-1.0.50/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/tests/test_uid.py` & `yz-core2-1.0.50/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.50/yz_core2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.49
+Version: 1.0.50
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.49/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.50/yz_core2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 yzcore/default_settings.py
 yzcore/exceptions.py
 yzcore/core/__init__.py
 yzcore/core/const.py
 yzcore/core/data_hash.py
 yzcore/core/datastructures.py
 yzcore/core/encoders.py
+yzcore/core/release.py
 yzcore/core/storage.py
 yzcore/core/management/__init__.py
 yzcore/core/management/base.py
 yzcore/core/management/templates.py
 yzcore/core/management/commands/__init__.py
 yzcore/core/management/commands/startapp.py
 yzcore/core/management/commands/startproject.py
```

### Comparing `yz-core2-1.0.49/yzcore/core/datastructures.py` & `yz-core2-1.0.50/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/encoders.py` & `yz-core2-1.0.50/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/management/__init__.py` & `yz-core2-1.0.50/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.50/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.50/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/management/templates.py` & `yz-core2-1.0.50/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/core/storage.py` & `yz-core2-1.0.50/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/db/db_session.py` & `yz-core2-1.0.50/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.50/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.50/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/decorators.py` & `yz-core2-1.0.50/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/default_settings.py` & `yz-core2-1.0.50/yzcore/default_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ID_URL: AnyUrl = None
     GENERATE_UUID_PATH: str = '/uuid/generate/'
     EXPLAIN_UUID_PATH: str = '/uuid/explain/'
     TRANSLATE_PATH: str = '/uuid/translate/'
     MAKE_UUID_PATH: str = '/uuid/make/'
 
     STORAGE_CONF: dict = None
-    STORAGE_ORG_ENABLE: bool = False  # 启用组织自定义对象存储
 
 
 default_setting = DefaultSetting()
 
 
 def reload_reload_settings(instance):
     settings = default_setting
```

### Comparing `yz-core2-1.0.49/yzcore/exceptions.py` & `yz-core2-1.0.50/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.50/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.50/yzcore/extensions/storage/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/base.py` & `yz-core2-1.0.50/yzcore/extensions/storage/base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/const.py` & `yz-core2-1.0.50/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.50/yzcore/extensions/storage/minio/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     Minio = None
 
 
 class MinioManager(StorageManagerBase):
 
     def __init__(self, conf: MinioConfig):
         super(MinioManager, self).__init__(conf)
+        self.internal_endpoint = conf.internal_endpoint
+        self.internal_minioClient = None
 
         self.__init()
 
     def __init(self, bucket_name=None):
         """初始化对象"""
 
         if Minio is None:
@@ -43,27 +45,45 @@
         self.minioClient = Minio(
             self.endpoint,
             access_key=self.access_key_id,
             secret_key=self.access_key_secret,
             secure=True if self.scheme == 'https' else False,
         )
 
+        if self.internal_endpoint:
+            self.internal_minioClient = Minio(
+                self.internal_endpoint,
+                access_key=self.access_key_id,
+                secret_key=self.access_key_secret,
+                secure=True if self.scheme == 'https' else False,
+            )
+
         if self.cache_path:
             try:
                 os.makedirs(self.cache_path)
             except OSError:
                 pass
 
+    def _internal_minio_client_first(self):
+        """优先使用内网连接minio服务"""
+        if self.internal_endpoint:
+            client = self.internal_minioClient
+        else:
+            client = self.minioClient
+        return client
+
     def get_bucket_cors(self):
         """返回的内容格式和OSS/OBS差异太大"""
-        result = self.minioClient.get_bucket_policy(self.bucket_name)
+        client = self._internal_minio_client_first()
+        result = client.get_bucket_policy(self.bucket_name)
         return json.loads(result)
 
     def set_bucket_cors(self, policy: dict):
-        return self.minioClient.set_bucket_policy(self.bucket_name, policy)
+        client = self._internal_minio_client_first()
+        return client.set_bucket_policy(self.bucket_name, policy)
 
     def _cors_check(self):
         passed = False
         action_slots = ['s3:AbortMultipartUpload', 's3:DeleteObject', 's3:GetObject',
                         's3:ListMultipartUploadParts', 's3:PutObject']
 
         cors_dict = self.get_bucket_cors()
@@ -76,29 +96,33 @@
                 if resource == f'arn:aws:s3:::{self.bucket_name}/*' or resource == 'arn:aws:s3:::*':
                     if all([False for i in action_slots if i not in actions]):
                         passed = True
         return passed
 
     def create_bucket(self, bucket_name=None):
         """创建bucket，并且作为当前操作bucket"""
-        self.minioClient.make_bucket(bucket_name)
+        client = self._internal_minio_client_first()
+        client.make_bucket(bucket_name)
         self.bucket_name = bucket_name
 
     def list_buckets(self):
-        return self.minioClient.list_buckets()
+        client = self._internal_minio_client_first()
+        return client.list_buckets()
 
     def is_exist_bucket(self, bucket_name=None):
+        client = self._internal_minio_client_first()
         if bucket_name is None:
             bucket_name = self.bucket_name
-        return self.minioClient.bucket_exists(bucket_name)
+        return client.bucket_exists(bucket_name)
 
     def delete_bucket(self, bucket_name=None):
+        client = self._internal_minio_client_first()
         if bucket_name is None:
             bucket_name = self.bucket_name
-        return self.minioClient.remove_bucket(bucket_name)
+        return client.remove_bucket(bucket_name)
 
     def get_sign_url(self, key, expire=0):
         expire_time = timedelta(seconds=expire or self.private_expire_time)
         url = self.minioClient.presigned_get_object(self.bucket_name, key, expires=expire_time)
         return '//' + url.split('//', 1)[-1]
 
     def post_sign_url(self, key):
@@ -108,66 +132,73 @@
         # policy.add_content_length_range_condition(1, 1024*1024*1024)  # 限制文件大小
         return self.minioClient.presigned_post_policy(policy)
 
     def put_sign_url(self, key):
         return self.minioClient.presigned_put_object(self.bucket_name, key)
 
     def iter_objects(self, prefix='', marker=None, delimiter=None, max_keys=100):
-        objects = self.minioClient.list_objects(self.bucket_name, prefix=prefix, recursive=True)
+        client = self._internal_minio_client_first()
+        objects = client.list_objects(self.bucket_name, prefix=prefix, recursive=True)
         _result = []
         for obj in objects:
             _result.append({
                 'key': obj.object_name,
                 'url': self.get_file_url(obj.object_name),
                 'size': obj.size,
             })
         return _result
 
     def get_object_meta(self, key: str):
         """获取文件基本元信息，包括该Object的ETag、Size（文件大小）、LastModified，Content-Type，并不返回其内容"""
-        meta = self.minioClient.stat_object(self.bucket_name, key)
+        client = self._internal_minio_client_first()
+        meta = client.stat_object(self.bucket_name, key)
         return {
             'etag': meta.etag,
             'size': meta.size,
             'last_modified': datetime2str(meta.last_modified),
             'content_type': meta.content_type,
         }
 
     def update_file_headers(self, key, headers: dict):
-        self.minioClient.copy_object(self.bucket_name, key, CopySource(self.bucket_name, key), metadata=headers, metadata_directive='REPLACE')
+        client = self._internal_minio_client_first()
+        client.copy_object(self.bucket_name, key, CopySource(self.bucket_name, key), metadata=headers, metadata_directive='REPLACE')
         return True
 
     def file_exists(self, key):
+        client = self._internal_minio_client_first()
         try:
-            self.minioClient.stat_object(self.bucket_name, key)
+            client.stat_object(self.bucket_name, key)
             return True
         except S3Error as e:
             if e.code == 'NoSuchKey':
                 return False
             raise e
 
     def download_stream(self, key, **kwargs):
-        return self.minioClient.get_object(self.bucket_name, key)
+        client = self._internal_minio_client_first()
+        return client.get_object(self.bucket_name, key)
 
     def download_file(self, key, local_name, **kwargs):
-        self.minioClient.fget_object(self.bucket_name, key, local_name)
+        client = self._internal_minio_client_first()
+        client.fget_object(self.bucket_name, key, local_name)
 
     def upload(self, filepath, key: str):
         """
         文件上传
         :param filepath:
         :param key:
         """
+        client = self._internal_minio_client_first()
         try:
             content_type = self.parse_content_type(key)
 
             if isinstance(filepath, str):
-                self.minioClient.fput_object(self.bucket_name, key, filepath, content_type=content_type)
+                client.fput_object(self.bucket_name, key, filepath, content_type=content_type)
             else:
-                self.minioClient.put_object(self.bucket_name, key, filepath, length=-1, content_type=content_type, part_size=1024*1024*5)
+                client.put_object(self.bucket_name, key, filepath, length=-1, content_type=content_type, part_size=1024*1024*5)
             return self.get_file_url(key)
         except Exception as e:
             raise StorageRequestError(f'minio upload error: {e}')
 
     def get_policy(
             self,
             filepath: str,
```

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.50/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.50/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.50/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.50/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.50/yzcore/extensions/storage/oss/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.50/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.50/yzcore/extensions/storage/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 class ObsConfig(BaseConfig):
     pass
 
 
 class MinioConfig(BaseConfig):
-    pass
+    internal_endpoint: str = None
 
 
 class AzureConfig(BaseConfig):
     connection_string: str
     account_key: str
     account_name: str
     access_key_id: Optional[str] = None
```

### Comparing `yz-core2-1.0.49/yzcore/extensions/uid.py` & `yz-core2-1.0.50/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/logger/__init__.py` & `yz-core2-1.0.50/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/logger/config.py` & `yz-core2-1.0.50/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/logger/filters.py` & `yz-core2-1.0.50/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/logger/handlers.py` & `yz-core2-1.0.50/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/request/aio_http.py` & `yz-core2-1.0.50/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/response/response.py` & `yz-core2-1.0.50/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/response/response_code.py` & `yz-core2-1.0.50/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.50/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.50/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/app_template/views.py` & `yz-core2-1.0.50/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.50/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/README.md` & `yz-core2-1.0.50/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.50/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.50/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.50/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.50/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/check_sys.py` & `yz-core2-1.0.50/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/crypto.py` & `yz-core2-1.0.50/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/decorator.py` & `yz-core2-1.0.50/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/encoding.py` & `yz-core2-1.0.50/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/nacos.py` & `yz-core2-1.0.50/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.49/yzcore/utils/time_utils.py` & `yz-core2-1.0.50/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

