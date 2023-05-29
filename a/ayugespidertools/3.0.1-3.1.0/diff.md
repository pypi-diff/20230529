# Comparing `tmp/ayugespidertools-3.0.1.tar.gz` & `tmp/ayugespidertools-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-3.0.1.tar", max compression
+gzip compressed data, was "ayugespidertools-3.1.0.tar", max compression
```

## Comparing `ayugespidertools-3.0.1.tar` & `ayugespidertools-3.1.0.tar`

### file list

```diff
@@ -1,85 +1,88 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/LICENSE
--rw-r--r--   0        0        0    13919 2023-05-17 08:57:35.000000 ayugespidertools-3.0.1/README.md
--rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.0.1/ayugespidertools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.0.1/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.0.1/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.0.1/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.0.1/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-3.0.1/ayugespidertools/common/encryption.py
--rw-r--r--   0        0        0     6622 2023-04-25 02:55:24.000000 ayugespidertools-3.0.1/ayugespidertools/common/expend.py
--rw-r--r--   0        0        0     6407 2023-05-16 02:31:54.000000 ayugespidertools-3.0.1/ayugespidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    15755 2023-05-17 02:27:54.000000 ayugespidertools-3.0.1/ayugespidertools/common/multiplexing.py
--rw-r--r--   0        0        0    13558 2023-05-15 09:13:35.000000 ayugespidertools-3.0.1/ayugespidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-3.0.1/ayugespidertools/common/params.py
--rw-r--r--   0        0        0     4264 2023-04-25 02:56:33.000000 ayugespidertools-3.0.1/ayugespidertools/common/spiderdbconf.py
--rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-3.0.1/ayugespidertools/common/sqlformat.py
--rw-r--r--   0        0        0     2368 2023-04-27 03:08:07.000000 ayugespidertools-3.0.1/ayugespidertools/common/typevars.py
--rw-r--r--   0        0        0    11325 2023-05-17 02:11:53.000000 ayugespidertools-3.0.1/ayugespidertools/common/utils.py
--rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-3.0.1/ayugespidertools/common/yidungap.py
--rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-3.0.1/ayugespidertools/config.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-3.0.1/ayugespidertools/formatdata.py
--rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-3.0.1/ayugespidertools/imgoperation.py
--rw-r--r--   0        0        0     4994 2023-05-16 09:33:56.000000 ayugespidertools-3.0.1/ayugespidertools/items.py
--rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-3.0.1/ayugespidertools/middlewares.py
--rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/mongoclient.py
--rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/mysqlclient.py
--rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-3.0.1/ayugespidertools/oss.py
--rw-r--r--   0        0        0      802 2023-05-10 05:50:47.000000 ayugespidertools-3.0.1/ayugespidertools/pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/processmanager.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.0.1/ayugespidertools/request.py
--rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/rpa.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/runjs.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10519 2023-04-27 07:35:00.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     2055 2023-05-16 09:34:33.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     2877 2023-05-16 08:50:58.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     1361 2023-05-16 08:56:28.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    12469 2023-05-16 08:48:07.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     4371 2023-05-16 08:51:08.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3854 2023-05-16 08:50:14.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     7167 2023-05-17 01:13:17.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.0.1/ayugespidertools/spiders.py
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      613 2023-05-11 03:15:22.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1337 2023-05-14 07:20:40.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.0.1/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6327 2023-05-17 06:24:21.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1829 2023-05-17 06:32:25.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.0.1/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5943 2023-05-09 01:54:08.000000 ayugespidertools-3.0.1/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.0.1/ayugespidertools/verificationcode.py
--rw-r--r--   0        0        0     3074 2023-05-17 08:47:49.000000 ayugespidertools-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    15659 1970-01-01 00:00:00.000000 ayugespidertools-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/LICENSE
+-rw-r--r--   0        0        0    14107 2023-05-29 07:10:35.000000 ayugespidertools-3.1.0/README.md
+-rw-r--r--   0        0        0      482 2023-04-26 03:31:14.000000 ayugespidertools-3.1.0/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:21:23.000000 ayugespidertools-3.1.0/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-3.1.0/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3880 2023-05-12 03:27:33.000000 ayugespidertools-3.1.0/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      524 2023-04-18 02:24:43.000000 ayugespidertools-3.1.0/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0     3704 2023-04-21 05:52:41.000000 ayugespidertools-3.1.0/ayugespidertools/common/encryption.py
+-rw-r--r--   0        0        0     6618 2023-05-26 02:04:03.000000 ayugespidertools-3.1.0/ayugespidertools/common/expend.py
+-rw-r--r--   0        0        0     6622 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    16599 2023-05-29 02:04:03.000000 ayugespidertools-3.1.0/ayugespidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    13558 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    32707 2023-04-26 06:59:16.000000 ayugespidertools-3.1.0/ayugespidertools/common/params.py
+-rw-r--r--   0        0        0     4240 2023-05-26 02:05:31.000000 ayugespidertools-3.1.0/ayugespidertools/common/spiderdbconf.py
+-rw-r--r--   0        0        0     3726 2023-04-12 09:31:20.000000 ayugespidertools-3.1.0/ayugespidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     2838 2023-05-29 03:26:37.000000 ayugespidertools-3.1.0/ayugespidertools/common/typevars.py
+-rw-r--r--   0        0        0    11321 2023-05-26 02:04:35.000000 ayugespidertools-3.1.0/ayugespidertools/common/utils.py
+-rw-r--r--   0        0        0     3693 2023-04-25 02:57:48.000000 ayugespidertools-3.1.0/ayugespidertools/common/yidungap.py
+-rw-r--r--   0        0        0      455 2023-04-13 07:37:35.000000 ayugespidertools-3.1.0/ayugespidertools/config.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-3.1.0/ayugespidertools/formatdata.py
+-rw-r--r--   0        0        0     7681 2023-04-25 03:03:41.000000 ayugespidertools-3.1.0/ayugespidertools/imgoperation.py
+-rw-r--r--   0        0        0     5065 2023-05-25 07:32:25.000000 ayugespidertools-3.1.0/ayugespidertools/items.py
+-rw-r--r--   0        0        0      898 2023-04-24 02:31:51.000000 ayugespidertools-3.1.0/ayugespidertools/middlewares.py
+-rw-r--r--   0        0        0     8550 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/mongoclient.py
+-rw-r--r--   0        0        0     1140 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/mysqlclient.py
+-rw-r--r--   0        0        0     5431 2023-04-25 03:03:58.000000 ayugespidertools-3.1.0/ayugespidertools/oss.py
+-rw-r--r--   0        0        0      904 2023-05-29 03:26:43.000000 ayugespidertools-3.1.0/ayugespidertools/pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/processmanager.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:04.000000 ayugespidertools-3.1.0/ayugespidertools/request.py
+-rw-r--r--   0        0        0     2397 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/rpa.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/runjs.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-26 03:31:29.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1350 2023-04-25 02:58:04.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-27 08:03:48.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0     1195 2023-04-24 02:25:23.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1742 2023-04-25 02:58:16.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      374 2023-04-24 02:00:59.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10515 2023-05-26 02:02:45.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0     4331 2023-04-25 02:58:59.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0      408 2023-04-24 02:20:24.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     4228 2023-04-25 02:59:18.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2876 2023-04-26 02:43:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11201 2023-04-25 02:59:35.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0     1042 2023-05-26 07:14:18.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     2115 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     2898 2023-05-26 06:58:42.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1361 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      148 2023-05-26 02:23:50.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     2673 2023-05-29 05:56:21.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0    12465 2023-05-26 02:04:46.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     4371 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     1754 2023-04-25 03:01:24.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2842 2023-05-04 02:07:52.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3956 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     7167 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      442 2023-04-12 09:55:11.000000 ayugespidertools-3.1.0/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      182 2023-04-25 03:15:03.000000 ayugespidertools-3.1.0/ayugespidertools/spiders.py
+-rw-r--r--   0        0        0     2065 2023-05-18 08:39:18.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      729 2023-05-29 07:36:32.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      817 2023-04-25 08:43:59.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-04-17 13:23:51.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1337 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-3.1.0/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1650 2023-04-25 06:08:11.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6327 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1829 2023-05-17 09:02:33.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-3.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-3.1.0/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5943 2023-05-18 08:39:18.000000 ayugespidertools-3.1.0/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     6924 2023-04-25 03:04:11.000000 ayugespidertools-3.1.0/ayugespidertools/verificationcode.py
+-rw-r--r--   0        0        0     3091 2023-05-29 07:19:55.000000 ayugespidertools-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15882 1970-01-01 00:00:00.000000 ayugespidertools-3.1.0/PKG-INFO
```

### Comparing `ayugespidertools-3.0.1/LICENSE` & `ayugespidertools-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/README.md` & `ayugespidertools-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 刚开始我也只是想把它用来适配 `Mysql` 存储的场景，可以自动创建相关数据库，数据表，字段注释，自动添加新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等等）的存储问题。后来不断优化和添加各种场景，使得爬虫开发在通用场景下几乎只用在意 `spider` 脚本的解析规则和 `VIT` 下的 `.conf` 配置即可，脱离无意义的重复操作。
 
 至于此库做了哪些功能，只要你熟悉 `python` 语法和 `scrapy` 库，再结合 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 中的应用示例，你可以很快上手。具体的内容和注意事项也可以在 [AyugeSpiderTools readthedocs 文档](https://ayugespidertools.readthedocs.io/en/latest/) 中查看。
 
 ## 1. 前提条件
 
-> `python 3.8+` 可以直接输入以下命令：
+> `python 3.8.1+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
 注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.4` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
@@ -58,21 +58,22 @@
 
 # 创建项目
 ayuge startproject <project_name>
 
 # 进入项目根目录
 cd <project_name>
 
+# 替换(覆盖)为真实的配置 .conf 文件：
+# 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上你需要的配置即可
+# 不需要的配置设置为空，或者不用理会它，或者删除它也可以，看个人选择
+cp /root/mytemp/.conf DemoSpider/VIT/.conf
+
 # 生成爬虫脚本
 ayuge genspider <spider_name> <example.com>
 
-# 替换(覆盖)为真实的配置 .conf 文件；
-# 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
-cp /root/mytemp/.conf DemoSpider/VIT/.conf
-
 # 运行脚本
 scrapy crawl <spider_name>
 # 注：也可以使用 ayuge crawl <spider_name>
 ```
 
 具体使用方法请在 [DemoSpider 之 AyugeSpiderTools 工具应用示例](https://github.com/shengchenyang/DemoSpider) 项目中查看，目前已适配以下场景：
 
@@ -101,17 +102,18 @@
 + 12).demo_proxy_two: 测试快代理独享代理
 
 +13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
--16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目标已经可以很方便的使用 Item Loaders 功能了
+-16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
++18).demo_mq: 数据存入 rabbitmq 的模板示例，通过 pika 库实现
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/commands/startproject.py` & `ayugespidertools-3.1.0/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/commands/version.py` & `ayugespidertools-3.1.0/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/encryption.py` & `ayugespidertools-3.1.0/ayugespidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/expend.py` & `ayugespidertools-3.1.0/ayugespidertools/common/expend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 
 import pymysql
 from retrying import retry
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import MysqlConfig
+from ayugespidertools.common.typevars import MysqlConf
 from ayugespidertools.config import logger
 
 __all__ = [
     "MysqlPipeEnhanceMixin",
 ]
 
 
@@ -21,15 +21,15 @@
     @retry(
         stop_max_attempt_number=Param.retry_num,
         wait_random_min=Param.retry_time_min,
         wait_random_max=Param.retry_time_max,
     )
     def _connect(
         self,
-        mysql_conf: MysqlConfig,
+        mysql_conf: MysqlConf,
     ) -> pymysql.connections.Connection:
         """
         链接数据库操作：
             1.如果链接正常，则返回链接句柄；
             2.如果目标数据库不存在，则创建数据库后再返回链接句柄。
         Args:
             mysql_conf: pymysql 链接所需的参数
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/mongodbpipe.py` & `ayugespidertools-3.1.0/ayugespidertools/common/mongodbpipe.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-from abc import ABC, abstractmethod
-from typing import Union
-
-from itemadapter import ItemAdapter
-
-from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.params import Param
-
-__all__ = [
-    "Synchronize",
-    "TwistedAsynchronous",
-    "AsyncioAsynchronous",
-    "mongodb_pipe",
-]
-
-
-class AbstractClass(ABC):
-    """
-    用于处理 mongodb pipeline 存储的模板方法类
-    """
-
-    def _get_collection_name(self, table: str, collection_prefix: str = "") -> str:
-        """
-        获取集合名称
-        Args:
-            table: item 中的 table 字段
-            collection_prefix: 集合前缀
-
-        Returns:
-            full_collection_name: 完整的集合名称
-        """
-        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
-        full_collection_name = f"""{collection_prefix}{table}"""
-
-        assert (
-            " " not in full_collection_name
-        ), "集合名不能含空格，请检查 MONGODB_COLLECTION_PREFIX 参数和 item 中的 table 参数"
-        return full_collection_name
-
-    def _get_insert_data(
-        self,
-        item_dict: Union[ItemAdapter, dict],
-    ) -> dict:
-        """
-        获取要插入的数据，将 item 中的存储数据提取出来
-        Args:
-            item_dict: item ItemAdapter 或者 dict 格式数据，可像字典一样操作
-
-        Returns:
-            None
-        """
-        insert_data = ReuseOperation.get_items_except_keys(
-            dict_conf=item_dict,
-            key_list=["_table", "_item_mode", "_mongo_update_rule"],
-        )
-        judge_item = next(iter(insert_data.values()))
-        # 是 namedtuple 类型
-        if ReuseOperation.is_namedtuple_instance(judge_item):
-            insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
-        # 是普通的 dict 格式，则直接为 insert_data
-        return insert_data
-
-    def process_item_template(
-        self,
-        item_dict: Union[ItemAdapter, dict],
-        db: Param.PymongoDataBase,
-        collection_prefix: str = "",
-    ) -> None:
-        """
-        模板方法，用于处理 mongodb pipeline 存储的模板方法类
-        Args:
-            item_dict: item ItemAdapter 或 dict 格式数据
-            db: mongodb 数据库连接
-            collection_prefix: 集合前缀
-
-        Returns:
-            None
-        """
-        insert_data = self._get_insert_data(item_dict)
-        # 真实的集合名称为：集合前缀名 + 集合名称
-        collection_name = self._get_collection_name(
-            table=item_dict["_table"],
-            collection_prefix=collection_prefix,
-        )
-        self._data_storage_logic(
-            db=db,
-            item_dict=item_dict,
-            collection_name=collection_name,
-            insert_data=insert_data,
-        )
-
-    @abstractmethod
-    def _data_storage_logic(
-        self,
-        db: Param.PymongoDataBase,
-        item_dict: Union[ItemAdapter, dict],
-        collection_name: str,
-        insert_data: dict,
-        *args,
-        **kwargs,
-    ) -> None:
-        """
-        数据存储逻辑，需要子类实现
-        Args:
-            db: mongodb 数据库连接
-            item_dict: item ItemAdapter 或 dict 格式数据
-            collection_name: 集合名称
-            insert_data: 要插入的数据
-            *args: 可变参数
-            **kwargs:关键字参数
-
-        Returns:
-            None
-        """
-        pass
-
-
-class Synchronize(AbstractClass):
-    """
-    pipeline 同步执行 mongodb 存储的场景
-    """
-
-    def _data_storage_logic(
-        self,
-        db: Param.PymongoDataBase,
-        item_dict: Union[ItemAdapter, dict],
-        collection_name: str,
-        insert_data: dict,
-        *args,
-        **kwargs,
-    ) -> None:
-        # 如果没有查重字段时，就直接插入数据（不去重）
-        if not item_dict.get("_mongo_update_rule"):
-            db[collection_name].insert(insert_data)
-        else:
-            db[collection_name].update(
-                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-            )
-
-
-class TwistedAsynchronous(AbstractClass):
-    """
-    pipeline twisted 异步执行 mongodb 存储的场景
-    """
-
-    def _data_storage_logic(
-        self,
-        db: Param.PymongoDataBase,
-        item_dict: Union[ItemAdapter, dict],
-        collection_name: str,
-        insert_data: dict,
-        *args,
-        **kwargs,
-    ) -> None:
-        if not item_dict.get("_mongo_update_rule"):
-            db[collection_name].insert(insert_data)
-        else:
-            db[collection_name].update(
-                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-            )
-
-
-class AsyncioAsynchronous(AbstractClass):
-    """
-    pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现
-    """
-
-    async def _data_storage_logic(
-        self,
-        db: Param.PymongoDataBase,
-        item_dict: Union[ItemAdapter, dict],
-        collection_name: str,
-        insert_data: dict,
-        *args,
-        **kwargs,
-    ) -> None:
-        if not item_dict.get("_mongo_update_rule"):
-            await db[collection_name].insert_one(insert_data)
-        else:
-            await db[collection_name].update_many(
-                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
-            )
-
-    async def process_item_template(
-        self,
-        item_dict: Union[ItemAdapter, dict],
-        db: Param.PymongoDataBase,
-        collection_prefix: str = "",
-    ) -> None:
-        insert_data = self._get_insert_data(item_dict)
-        # 真实的集合名称为：集合前缀名 + 集合名称
-        collection_name = self._get_collection_name(
-            table=item_dict["_table"],
-            collection_prefix=collection_prefix,
-        )
-        await self._data_storage_logic(
-            db=db,
-            item_dict=item_dict,
-            collection_name=collection_name,
-            insert_data=insert_data,
-        )
-
-
-def mongodb_pipe(
-    abstract_class: AbstractClass,
-    item_dict: Union[ItemAdapter, dict],
-    db: Param.PymongoDataBase,
-    collection_prefix: str = "",
-) -> None:
-    """
-    mongodb pipeline 存储的通用调用方法
-    """
-    abstract_class.process_item_template(
-        item_dict=item_dict, db=db, collection_prefix=collection_prefix
-    )
+from abc import ABC, abstractmethod
+from typing import Union
+
+from itemadapter import ItemAdapter
+
+from ayugespidertools.common.multiplexing import ReuseOperation
+from ayugespidertools.common.params import Param
+
+__all__ = [
+    "Synchronize",
+    "TwistedAsynchronous",
+    "AsyncioAsynchronous",
+    "mongodb_pipe",
+]
+
+
+class AbstractClass(ABC):
+    """
+    用于处理 mongodb pipeline 存储的模板方法类
+    """
+
+    def _get_collection_name(self, table: str, collection_prefix: str = "") -> str:
+        """
+        获取集合名称
+        Args:
+            table: item 中的 table 字段
+            collection_prefix: 集合前缀
+
+        Returns:
+            full_collection_name: 完整的集合名称
+        """
+        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
+        full_collection_name = f"""{collection_prefix}{table}"""
+
+        assert (
+            " " not in full_collection_name
+        ), "集合名不能含空格，请检查 MONGODB_COLLECTION_PREFIX 参数和 item 中的 table 参数"
+        return full_collection_name
+
+    def _get_insert_data(
+        self,
+        item_dict: Union[ItemAdapter, dict],
+    ) -> dict:
+        """
+        获取要插入的数据，将 item 中的存储数据提取出来
+        Args:
+            item_dict: item ItemAdapter 或者 dict 格式数据，可像字典一样操作
+
+        Returns:
+            None
+        """
+        insert_data = ReuseOperation.get_items_except_keys(
+            dict_conf=item_dict,
+            key_list=["_table", "_item_mode", "_mongo_update_rule"],
+        )
+        judge_item = next(iter(insert_data.values()))
+        # 是 namedtuple 类型
+        if ReuseOperation.is_namedtuple_instance(judge_item):
+            insert_data = {v: insert_data[v].key_value for v in insert_data.keys()}
+        # 是普通的 dict 格式，则直接为 insert_data
+        return insert_data
+
+    def process_item_template(
+        self,
+        item_dict: Union[ItemAdapter, dict],
+        db: Param.PymongoDataBase,
+        collection_prefix: str = "",
+    ) -> None:
+        """
+        模板方法，用于处理 mongodb pipeline 存储的模板方法类
+        Args:
+            item_dict: item ItemAdapter 或 dict 格式数据
+            db: mongodb 数据库连接
+            collection_prefix: 集合前缀
+
+        Returns:
+            None
+        """
+        insert_data = self._get_insert_data(item_dict)
+        # 真实的集合名称为：集合前缀名 + 集合名称
+        collection_name = self._get_collection_name(
+            table=item_dict["_table"],
+            collection_prefix=collection_prefix,
+        )
+        self._data_storage_logic(
+            db=db,
+            item_dict=item_dict,
+            collection_name=collection_name,
+            insert_data=insert_data,
+        )
+
+    @abstractmethod
+    def _data_storage_logic(
+        self,
+        db: Param.PymongoDataBase,
+        item_dict: Union[ItemAdapter, dict],
+        collection_name: str,
+        insert_data: dict,
+        *args,
+        **kwargs,
+    ) -> None:
+        """
+        数据存储逻辑，需要子类实现
+        Args:
+            db: mongodb 数据库连接
+            item_dict: item ItemAdapter 或 dict 格式数据
+            collection_name: 集合名称
+            insert_data: 要插入的数据
+            *args: 可变参数
+            **kwargs:关键字参数
+
+        Returns:
+            None
+        """
+        pass
+
+
+class Synchronize(AbstractClass):
+    """
+    pipeline 同步执行 mongodb 存储的场景
+    """
+
+    def _data_storage_logic(
+        self,
+        db: Param.PymongoDataBase,
+        item_dict: Union[ItemAdapter, dict],
+        collection_name: str,
+        insert_data: dict,
+        *args,
+        **kwargs,
+    ) -> None:
+        # 如果没有查重字段时，就直接插入数据（不去重）
+        if not item_dict.get("_mongo_update_rule"):
+            db[collection_name].insert(insert_data)
+        else:
+            db[collection_name].update(
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+            )
+
+
+class TwistedAsynchronous(AbstractClass):
+    """
+    pipeline twisted 异步执行 mongodb 存储的场景
+    """
+
+    def _data_storage_logic(
+        self,
+        db: Param.PymongoDataBase,
+        item_dict: Union[ItemAdapter, dict],
+        collection_name: str,
+        insert_data: dict,
+        *args,
+        **kwargs,
+    ) -> None:
+        if not item_dict.get("_mongo_update_rule"):
+            db[collection_name].insert(insert_data)
+        else:
+            db[collection_name].update(
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+            )
+
+
+class AsyncioAsynchronous(AbstractClass):
+    """
+    pipeline asyncio 异步执行 mongodb 存储的场景 - 使用 motor 实现
+    """
+
+    async def _data_storage_logic(
+        self,
+        db: Param.PymongoDataBase,
+        item_dict: Union[ItemAdapter, dict],
+        collection_name: str,
+        insert_data: dict,
+        *args,
+        **kwargs,
+    ) -> None:
+        if not item_dict.get("_mongo_update_rule"):
+            await db[collection_name].insert_one(insert_data)
+        else:
+            await db[collection_name].update_many(
+                item_dict["_mongo_update_rule"], {"$set": insert_data}, True
+            )
+
+    async def process_item_template(
+        self,
+        item_dict: Union[ItemAdapter, dict],
+        db: Param.PymongoDataBase,
+        collection_prefix: str = "",
+    ) -> None:
+        insert_data = self._get_insert_data(item_dict)
+        # 真实的集合名称为：集合前缀名 + 集合名称
+        collection_name = self._get_collection_name(
+            table=item_dict["_table"],
+            collection_prefix=collection_prefix,
+        )
+        await self._data_storage_logic(
+            db=db,
+            item_dict=item_dict,
+            collection_name=collection_name,
+            insert_data=insert_data,
+        )
+
+
+def mongodb_pipe(
+    abstract_class: AbstractClass,
+    item_dict: Union[ItemAdapter, dict],
+    db: Param.PymongoDataBase,
+    collection_prefix: str = "",
+) -> None:
+    """
+    mongodb pipeline 存储的通用调用方法
+    """
+    abstract_class.process_item_template(
+        item_dict=item_dict, db=db, collection_prefix=collection_prefix
+    )
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/multiplexing.py` & `ayugespidertools-3.1.0/ayugespidertools/common/multiplexing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
 import configparser
 import json
 import os
 import random
-import re
 from typing import Any, List, Union
 
 import cv2
 import numpy as np
 import pymysql
 from scrapy.settings import Settings
 from twisted.internet.defer import Deferred
 
-from ayugespidertools.common.typevars import MysqlConfig
+from ayugespidertools.common.typevars import MysqlConf
 from ayugespidertools.config import logger
 from ayugespidertools.items import MongoDataItem, MysqlDataItem, ScrapyItem
 
 __all__ = [
     "ReuseOperation",
 ]
 
@@ -105,14 +104,35 @@
             "accesskeysecret": config_parser.get(
                 "ali_oss", "accesskeysecret", fallback=None
             ),
             "endpoint": config_parser.get("ali_oss", "endpoint", fallback=None),
             "bucket": config_parser.get("ali_oss", "bucket", fallback=None),
             "doc": config_parser.get("ali_oss", "doc", fallback=None),
         }
+        # mq 配置
+        inner_settings["MQ_CONFIG"] = {
+            "host": config_parser.get("mq", "host", fallback=None),
+            "port": config_parser.getint("mq", "port", fallback=5672),
+            "username": config_parser.get("mq", "username", fallback="guest"),
+            "password": config_parser.get("mq", "password", fallback="guest"),
+            "virtualhost": config_parser.get("mq", "virtualhost", fallback="/"),
+            "queue": config_parser.get("mq", "queue", fallback=None),
+            "durable": config_parser.getboolean("mq", "durable", fallback=True),
+            "exclusive": config_parser.getboolean("mq", "exclusive", fallback=False),
+            "auto_delete": config_parser.getboolean(
+                "mq", "auto_delete", fallback=False
+            ),
+            "exchange": config_parser.get("mq", "exchange", fallback=None),
+            "routing_key": config_parser.get("mq", "routing_key", fallback=None),
+            "content_type": config_parser.getint(
+                "mq", "content_type", fallback="text/plain"
+            ),
+            "delivery_mode": config_parser.getint("mq", "delivery_mode", fallback=1),
+            "mandatory": config_parser.getboolean("mq", "mandatory", fallback=True),
+        }
         return inner_settings
 
     @staticmethod
     def item_to_dict(
         item: Union[MysqlDataItem, MongoDataItem, ScrapyItem, dict]
     ) -> dict:
         """
@@ -137,29 +157,14 @@
 
         Returns:
             1). 是否符合 namedtuple 类型
         """
         return isinstance(x, tuple) and hasattr(x, "_fields")
 
     @staticmethod
-    def get_file_name_by_url(file_url: str) -> str:
-        """
-        根据文件链接取出文件的名称
-        Args:
-            file_url: 文件链接
-
-        Returns:
-            1). 文件名称
-        """
-        pattern = re.compile(r""".*/(.*?)\..*?""")
-        if file_name_list := pattern.findall(file_url):
-            return file_name_list[0]
-        return ""
-
-    @staticmethod
     def get_files_from_path(path: str) -> list:
         """
         获取 path 文件夹下的所有文件，而且输出以 path 为根目录的相对路径
         Args:
             path: 需要判断的文件夹路径
 
         Returns:
@@ -288,15 +293,15 @@
 
         Returns:
             1). dict_conf 排除 key_list 中的键值后的值
         """
         return {k: dict_conf[k] for k in dict_conf if k not in key_list}
 
     @classmethod
-    def create_database(cls, mysql_conf: MysqlConfig) -> None:
+    def create_database(cls, mysql_conf: MysqlConf) -> None:
         """
         创建数据库
         由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
         Args:
             mysql_conf: pymysql 的数据库连接配置
 
         Returns:
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/mysqlerrhandle.py` & `ayugespidertools-3.1.0/ayugespidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/params.py` & `ayugespidertools-3.1.0/ayugespidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/spiderdbconf.py` & `ayugespidertools-3.1.0/ayugespidertools/common/spiderdbconf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from abc import ABC, abstractmethod
 from typing import Union
 
 from scrapy.settings import Settings
 
 from ayugespidertools.common.multiplexing import ReuseOperation
-from ayugespidertools.common.typevars import MongoDBConfig, MysqlConfig
+from ayugespidertools.common.typevars import MongoDBConf, MysqlConf
 from ayugespidertools.common.utils import ToolsForAyu
 
 __all__ = [
     "get_spider_db_conf",
     "MysqlConfCreator",
     "MongoDBConfCreator",
 ]
 
 
 class Product(ABC):
     @abstractmethod
-    def get_db_conn_conf(self) -> Union[MysqlConfig, MongoDBConfig, None]:
+    def get_db_conn_conf(self) -> Union[MysqlConf, MongoDBConf, None]:
         """
         获取数据库链接配置信息，目前支持 mysql 和 mongodb
         """
         pass
 
 
 class Creator(ABC):
@@ -30,70 +30,70 @@
 
 
 class MysqlConfProduct(Product):
     def __init__(self, settings: Settings, consul_conf: dict):
         self._settings = settings
         self._consul_conf = consul_conf
 
-    def get_db_conn_conf(self) -> Union[MysqlConfig, None]:
+    def get_db_conn_conf(self) -> Union[MysqlConf, None]:
         # 自定义 mysql 链接配置
         local_mysql_conf = self._settings.get("LOCAL_MYSQL_CONFIG", {})
         # 是否开启应用配置管理
         app_conf_manage = self._settings.get("APP_CONF_MANAGE", False)
         if all([not local_mysql_conf.get("database"), not app_conf_manage]):
             return None
 
         # 1). 如果开启应用管理，从 consul 中获取应用配置
         if app_conf_manage:
             _consul_conf_dict = ToolsForAyu.get_conf_by_consul(
                 conf_name="mysql", **self._consul_conf
             )
-            return MysqlConfig(**_consul_conf_dict)
+            return MysqlConf(**_consul_conf_dict)
 
         # 2). 从本地 local_mysql_config 的参数中取值
         if ReuseOperation.is_dict_meet_min_limit(
             dict_conf=local_mysql_conf,
             key_list=["host", "port", "user", "password", "charset", "database"],
         ):
-            return MysqlConfig(
+            return MysqlConf(
                 host=local_mysql_conf.get("host"),
                 port=local_mysql_conf.get("port"),
                 user=local_mysql_conf.get("user"),
                 password=local_mysql_conf.get("password"),
                 database=local_mysql_conf.get("database"),
                 charset=local_mysql_conf.get("charset") or "utf8mb4",
             )
 
 
 class MongoDBConfProduct(Product):
     def __init__(self, settings, consul_conf):
         self._settings = settings
         self._consul_conf = consul_conf
 
-    def get_db_conn_conf(self) -> Union[MongoDBConfig, None]:
+    def get_db_conn_conf(self) -> Union[MongoDBConf, None]:
         # 自定义 mysql 链接配置
         local_mongodb_conf = self._settings.get("LOCAL_MONGODB_CONFIG", {})
         # 是否开启应用配置管理
         app_conf_manage = self._settings.get("APP_CONF_MANAGE", False)
         if all([not local_mongodb_conf.get("database"), not app_conf_manage]):
             return None
 
         # 1). 如果开启应用管理，从 consul 中获取应用配置
         if app_conf_manage:
             _consul_conf_dict = ToolsForAyu.get_conf_by_consul(
                 conf_name="mongodb", **self._consul_conf
             )
-            return MongoDBConfig(**_consul_conf_dict)
+            return MongoDBConf(**_consul_conf_dict)
 
         # 2). 从本地 local_mongo_conf 的参数中取值
         if ReuseOperation.is_dict_meet_min_limit(
             dict_conf=local_mongodb_conf,
             key_list=["host", "port", "user", "password", "database"],
         ):
-            return MongoDBConfig(
+            return MongoDBConf(
                 host=local_mongodb_conf.get("host"),
                 port=local_mongodb_conf.get("port"),
                 user=local_mongodb_conf.get("user"),
                 password=local_mongodb_conf.get("password"),
                 database=local_mongodb_conf.get("database"),
                 authsource=local_mongodb_conf.get("authsource"),
             )
@@ -107,9 +107,9 @@
 class MongoDBConfCreator(Creator):
     def create_product(self, settings: Settings, consul_conf: dict) -> Product:
         return MongoDBConfProduct(settings, consul_conf)
 
 
 def get_spider_db_conf(
     product: Product,
-) -> Union[MysqlConfig, MongoDBConfig, None]:
+) -> Union[MysqlConf, MongoDBConf, None]:
     return product.get_db_conn_conf()
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/sqlformat.py` & `ayugespidertools-3.1.0/ayugespidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/typevars.py` & `ayugespidertools-3.1.0/ayugespidertools/common/typevars.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from enum import Enum, unique
 from typing import Any, Literal, NamedTuple, Optional, TypedDict, TypeVar, Union
 
 __all__ = [
     "TableTemplate",
     "TableEnumTypeVar",
     "AlterItem",
-    "MysqlConfig",
-    "MongoDBConfig",
-    "AiohttpConfig",
+    "MysqlConf",
+    "MongoDBConf",
+    "AiohttpConf",
     "AiohttpRequestArgs",
+    "MQConf",
 ]
 
 AiohttpRequestMethodStr = Literal["GET", "POST"]
 TableEnumTypeVar = TypeVar("TableEnumTypeVar", bound="TableEnum")
 
 sentinel: Any = object()
 
@@ -40,33 +41,33 @@
     demo_table = TableTemplate(
         value="表名(eg: demo)",
         notes="表注释信息(eg: 示例表信息)",
         demand_code="需求表对应数据(eg: Demo_table_demand_code，此示例没有意义，需要自定义)",
     )
 
 
-class MysqlConfig(NamedTuple):
+class MysqlConf(NamedTuple):
     host: str
     port: int
     user: str
     password: str
     database: Optional[str] = None
     charset: Optional[str] = "utf8mb4"
 
 
-class MongoDBConfig(NamedTuple):
+class MongoDBConf(NamedTuple):
     host: str
     port: int
     user: str
     password: str
     database: Optional[str] = None
     authsource: Optional[str] = None
 
 
-class AiohttpConfig(NamedTuple):
+class AiohttpConf(NamedTuple):
     sleep: int
     proxy: str
     proxy_auth: str
     proxy_headers: dict
     retry_times: int
     limit: int
     ssl: bool
@@ -87,7 +88,24 @@
     cookies: Union[dict, None] = field(default=None)
     method: AiohttpRequestMethodStr = field(default="GET")
     timeout: Union[int, None] = field(default=None)
     data: Union[dict, str, None] = field(default=None)
     proxy: Union[str, None] = field(default=None)
     proxy_auth: Union[str, None] = field(default=None)
     proxy_headers: Union[dict, None] = field(default=None)
+
+
+class MQConf(NamedTuple):
+    host: str
+    port: int
+    username: str
+    password: str
+    virtualhost: Optional[str] = "/"
+    queue: Optional[str] = None
+    durable: Optional[bool] = True
+    exclusive: Optional[bool] = False
+    auto_delete: Optional[bool] = False
+    exchange: Optional[str] = None
+    routing_key: Optional[str] = None
+    content_type: Optional[str] = "text/plain"
+    delivery_mode: Optional[int] = 1
+    mandatory: Optional[bool] = True
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/utils.py` & `ayugespidertools-3.1.0/ayugespidertools/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import requests
 import yaml
 from itemadapter import ItemAdapter
 
 from ayugespidertools.common.encryption import EncryptOperation
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import MysqlConfig
+from ayugespidertools.common.typevars import MysqlConf
 from ayugespidertools.config import logger
 from ayugespidertools.formatdata import DataHandle
 
 __all__ = [
     "ToolsForAyu",
 ]
 
@@ -205,15 +205,15 @@
 
         for query in query_rules:
             if extract_res := cls.extract_with_json(json_data=json_data, query=query):
                 return extract_res
         return ""
 
     @staticmethod
-    def get_collate_by_charset(mysql_conf: MysqlConfig) -> str:
+    def get_collate_by_charset(mysql_conf: MysqlConf) -> str:
         """
         根据 mysql 的 charset 获取对应默认的 collate
         Args:
             mysql_conf: mysql 连接配置
 
         Returns:
             collate: 排序规则
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/common/yidungap.py` & `ayugespidertools-3.1.0/ayugespidertools/common/yidungap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/formatdata.py` & `ayugespidertools-3.1.0/ayugespidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/imgoperation.py` & `ayugespidertools-3.1.0/ayugespidertools/imgoperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/items.py` & `ayugespidertools-3.1.0/ayugespidertools/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
 
     def asitem(self, assignment: bool = True):
         return self._asitem(assignment)
 
 
 @dataclass
 class MongoDataItem(metaclass=ItemMeta):
+    """
+    这个是 Scrapy item 的 mongoDB 的存储结构
+    """
+
     _table: str = None
     _item_mode: MongoDBItemModeStr = "MongoDB"
     _mongo_update_rule: Dict[str, Any] = None
 
     def __init__(
         self,
         _table,
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/middlewares.py` & `ayugespidertools-3.1.0/ayugespidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/mongoclient.py` & `ayugespidertools-3.1.0/ayugespidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/mysqlclient.py` & `ayugespidertools-3.1.0/ayugespidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/oss.py` & `ayugespidertools-3.1.0/ayugespidertools/oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/pipelines.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from ayugespidertools.scraper.pipelines.mongo.asynced import AsyncMongoPipeline
-from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
-from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
-from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
-from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
-from ayugespidertools.scraper.pipelines.mysql.turbo import AyuTurboMysqlPipeline
-from ayugespidertools.scraper.pipelines.mysql.twisted import AyuTwistedMysqlPipeline
-
-__all__ = [
-    "AyuFtyMysqlPipeline",
-    "AyuTurboMysqlPipeline",
-    "AyuTwistedMysqlPipeline",
-    "AsyncMongoPipeline",
-    "AsyncMysqlPipeline",
-    "AyuFtyMongoPipeline",
-    "AyuTwistedMongoPipeline",
-]
+# Define your item pipelines here
+#
+# Don"t forget to add your pipeline to the ITEM_PIPELINES setting
+# See: https://docs.scrapy.org/en/latest/topics/item-pipeline.html
+from ayugespidertools.scraper.pipelines.mongo.fantasy import AyuFtyMongoPipeline
+from ayugespidertools.scraper.pipelines.mongo.twisted import AyuTwistedMongoPipeline
+from ayugespidertools.scraper.pipelines.msgproducer.mqpub import AyuMQPipeline
+from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
+from ayugespidertools.scraper.pipelines.mysql.asynced import AsyncMysqlPipeline
+from ayugespidertools.scraper.pipelines.mysql.fantasy import AyuFtyMysqlPipeline
+from ayugespidertools.scraper.pipelines.mysql.turbo import AyuTurboMysqlPipeline
+from ayugespidertools.scraper.pipelines.mysql.twisted import AyuTwistedMysqlPipeline
+
+__all__ = [
+    "AyuMysqlPipeline",
+    "AyuFtyMysqlPipeline",
+    "AyuTurboMysqlPipeline",
+    "AyuTwistedMysqlPipeline",
+    "AsyncMysqlPipeline",
+    "AyuFtyMongoPipeline",
+    "AyuTwistedMongoPipeline",
+    "AyuMQPipeline",
+]
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/rpa.py` & `ayugespidertools-3.1.0/ayugespidertools/rpa.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/runjs.py` & `ayugespidertools-3.1.0/ayugespidertools/runjs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import scrapy
 from aiohttp.connector import BaseConnector
 from scrapy.http import HtmlResponse
 from scrapy.utils.python import global_object_name
 
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import AiohttpConfig, AiohttpRequestArgs
+from ayugespidertools.common.typevars import AiohttpConf, AiohttpRequestArgs
 from ayugespidertools.common.utils import ToolsForAyu
 from ayugespidertools.config import logger
 
 __all__ = [
     "AiohttpDownloaderMiddleware",
     "AiohttpAsyncDownloaderMiddleware",
 ]
@@ -80,15 +80,15 @@
         """
         初始化 middleware
         """
         settings = crawler.settings
         # 自定义 aiohttp 全局配置信息，优先级小于 aiohttp_meta 中的配置
         if local_aiohttp_conf := settings.get("LOCAL_AIOHTTP_CONFIG", {}):
             # 这里的配置信息如果在 aiohttp_meta 中重复设置，则会更新当前请求的参数
-            _aiohttp_conf = AiohttpConfig(
+            _aiohttp_conf = AiohttpConf(
                 timeout=local_aiohttp_conf.get("timeout"),
                 sleep=local_aiohttp_conf.get("sleep"),
                 proxy=local_aiohttp_conf.get("proxy"),
                 proxy_auth=local_aiohttp_conf.get("proxy_auth"),
                 proxy_headers=local_aiohttp_conf.get("proxy_headers"),
                 retry_times=local_aiohttp_conf.get(
                     "retry_times", Param.aiohttp_retry_times_default
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/asynced.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/asynced.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import asyncio
-import urllib.parse
-
-import motor.motor_asyncio
-
-from ayugespidertools.common.mongodbpipe import AsyncioAsynchronous
-from ayugespidertools.common.multiplexing import ReuseOperation
-
-
-class AsyncMongoPipeline(object):
-    """
-    通过 motor 实现异步写入 MongoDB 的存储管道
-    """
-
-    def __init__(
-        self,
-        collection_prefix: str = "",
-    ) -> None:
-        assert isinstance(collection_prefix, str), "mongoDB 所要存储的集合前缀名称需要是 str 格式！"
-
-        self.collection_prefix = collection_prefix or ""
-        self.mongo_uri = None
-
-    @classmethod
-    def from_crawler(cls, crawler):
-        return cls(
-            collection_prefix=crawler.settings.get("MONGODB_COLLECTION_PREFIX", ""),
-        )
-
-    def open_spider(self, spider):
-        assert hasattr(
-            spider, "mongodb_conf"
-        ), "未配置 MongoDB 连接信息，请查看 .conf 或 consul 上对应配置信息！"
-
-        _encoded_pwd = urllib.parse.quote_plus(spider.mongodb_conf.password)
-        self.mongo_uri = (
-            f"mongodb://{spider.mongodb_conf.user}:{_encoded_pwd}"
-            f"@{spider.mongodb_conf.host}:{spider.mongodb_conf.port}/"
-            f"?authSource={spider.mongodb_conf.authsource}&authMechanism=SCRAM-SHA-1",
-        )
-        return ReuseOperation.as_deferred(self._open_spider(spider))
-
-    async def _open_spider(self, spider):
-        self.client = motor.motor_asyncio.AsyncIOMotorClient(self.mongo_uri)
-        self.db = self.client[spider.mongodb_conf.database]
-
-    async def close_spider(self, spider):
-        self.client.close()
-
-    async def process_item(self, item, spider):
-        item_dict = ReuseOperation.item_to_dict(item)
-        if item_dict["_item_mode"] == "MongoDB":
-            await asyncio.shield(
-                AsyncioAsynchronous().process_item_template(
-                    item_dict=item_dict,
-                    db=self.db,
-                    collection_prefix=self.collection_prefix,
-                )
-            )
-        return item
+import asyncio
+import urllib.parse
+
+import motor.motor_asyncio
+
+from ayugespidertools.common.mongodbpipe import AsyncioAsynchronous
+from ayugespidertools.common.multiplexing import ReuseOperation
+
+
+class AsyncMongoPipeline(object):
+    """
+    通过 motor 实现异步写入 MongoDB 的存储管道
+    """
+
+    def __init__(
+        self,
+        collection_prefix: str = "",
+    ) -> None:
+        assert isinstance(collection_prefix, str), "mongoDB 所要存储的集合前缀名称需要是 str 格式！"
+
+        self.collection_prefix = collection_prefix or ""
+        self.mongo_uri = None
+
+    @classmethod
+    def from_crawler(cls, crawler):
+        return cls(
+            collection_prefix=crawler.settings.get("MONGODB_COLLECTION_PREFIX", ""),
+        )
+
+    def open_spider(self, spider):
+        assert hasattr(
+            spider, "mongodb_conf"
+        ), "未配置 MongoDB 连接信息，请查看 .conf 或 consul 上对应配置信息！"
+
+        _encoded_pwd = urllib.parse.quote_plus(spider.mongodb_conf.password)
+        self.mongo_uri = (
+            f"mongodb://{spider.mongodb_conf.user}:{_encoded_pwd}"
+            f"@{spider.mongodb_conf.host}:{spider.mongodb_conf.port}/"
+            f"?authSource={spider.mongodb_conf.authsource}&authMechanism=SCRAM-SHA-1",
+        )
+        return ReuseOperation.as_deferred(self._open_spider(spider))
+
+    async def _open_spider(self, spider):
+        self.client = motor.motor_asyncio.AsyncIOMotorClient(self.mongo_uri)
+        self.db = self.client[spider.mongodb_conf.database]
+
+    async def close_spider(self, spider):
+        self.client.close()
+
+    async def process_item(self, item, spider):
+        item_dict = ReuseOperation.item_to_dict(item)
+        if item_dict["_item_mode"] == "MongoDB":
+            await asyncio.shield(
+                AsyncioAsynchronous().process_item_template(
+                    item_dict=item_dict,
+                    db=self.db,
+                    collection_prefix=self.collection_prefix,
+                )
+            )
+        return item
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/fantasy.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             database=spider.mongodb_conf.database,
             authsource=spider.mongodb_conf.authsource,
         )
 
         # 用于输出日志
         if all([self.conn, self.db]):
             spider.slog.info(
-                f"已连接至 host: {spider.mongodb_conf.host}, database: {spider.mongodb_conf.database} 的 MongoDB 目标数据库"
+                f"已连接至 host: {spider.mongodb_conf.host}, "
+                f"database: {spider.mongodb_conf.database} 的 MongoDB 目标数据库"
             )
 
     def close_spider(self, spider):
         if self.conn:
             self.conn.close()
 
     def process_item(self, item, spider):
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mongo/twisted.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pymysql
 from retrying import retry
 
 from ayugespidertools.common.expend import MysqlPipeEnhanceMixin
 from ayugespidertools.common.multiplexing import ReuseOperation
 from ayugespidertools.common.mysqlerrhandle import Synchronize, deal_mysql_err
 from ayugespidertools.common.params import Param
-from ayugespidertools.common.typevars import AlterItem, MysqlConfig, TableEnumTypeVar
+from ayugespidertools.common.typevars import AlterItem, MysqlConf, TableEnumTypeVar
 from ayugespidertools.common.utils import ToolsForAyu
 
 # 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
 warnings.filterwarnings(
     "error", category=pymysql.Warning, message=".*Data truncated for column.*"
 )
 
@@ -44,15 +44,15 @@
         """
         self.table_prefix = table_prefix
         self.table_enum = table_enum
         self.env = env
         self.record_log_to_mysql = record_log_to_mysql
         # 排序规则，用于创建数据库时使用
         self.collate = None
-        self.mysql_conf: Optional[MysqlConfig] = None
+        self.mysql_conf: Optional[MysqlConf] = None
         self.conn = None
         self.slog = None
         self.cursor = None
         self.crawl_time = datetime.date.today()
 
     @classmethod
     def from_crawler(cls, crawler):
```

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-3.1.0/ayugespidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/items.py.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/items.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-3.1.0/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/utils/cmdline.py` & `ayugespidertools-3.1.0/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/ayugespidertools/verificationcode.py` & `ayugespidertools-3.1.0/ayugespidertools/verificationcode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-3.0.1/pyproject.toml` & `ayugespidertools-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "3.0.1"
+version = "3.1.0"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
@@ -37,14 +37,15 @@
 oss2 = "^2.16.0"
 aiomysql = "^0.1.1"
 attrs = "^22.2.0"
 toml = "^0.10.2"
 python-hcl2 = "^4.3.0"
 motor = "2.5.1"
 urllib3 = "~1.26.15"
+pika = "~1.3.2"
 
 [tool.poetry.scripts]
 ayuge = "ayugespidertools.utils.cmdline:execute"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.1.0"
```

### Comparing `ayugespidertools-3.0.1/PKG-INFO` & `ayugespidertools-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 3.0.1
+Version: 3.1.0
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -29,14 +29,15 @@
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: motor (==2.5.1)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: oss2 (>=2.16.0,<3.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pika (>=1.3.2,<1.4.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pymongo (>=3.12.3,<4.0.0)
 Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=1.26.15,<1.27.0)
@@ -64,15 +65,15 @@
 
 刚开始我也只是想把它用来适配 `Mysql` 存储的场景，可以自动创建相关数据库，数据表，字段注释，自动添加新添加的字段，和自动修复常见（字段编码，`Data too long`，存储字段不存在等等）的存储问题。后来不断优化和添加各种场景，使得爬虫开发在通用场景下几乎只用在意 `spider` 脚本的解析规则和 `VIT` 下的 `.conf` 配置即可，脱离无意义的重复操作。
 
 至于此库做了哪些功能，只要你熟悉 `python` 语法和 `scrapy` 库，再结合 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 中的应用示例，你可以很快上手。具体的内容和注意事项也可以在 [AyugeSpiderTools readthedocs 文档](https://ayugespidertools.readthedocs.io/en/latest/) 中查看。
 
 ## 1. 前提条件
 
-> `python 3.8+` 可以直接输入以下命令：
+> `python 3.8.1+` 可以直接输入以下命令：
 
 ```shell
 pip install ayugespidertools -i https://pypi.org/simple
 ```
 
 注：本库依赖中的 `pymongo` 版本要在 `^3.12.3` (即`3.13.0` 及以下) 是因为我的 `mongoDB` 的版本为 `3.4`，`pymogo` 官方从 `3.13.0` 以后的版本开始不再支持 `3.4` 版本以下的 `MongoDB` 数据库了，望周知！**你也可以根据 [3.3](#3.3.-Build-Your-Own-Library) 自定义库**
 
@@ -104,21 +105,22 @@
 
 # 创建项目
 ayuge startproject <project_name>
 
 # 进入项目根目录
 cd <project_name>
 
+# 替换(覆盖)为真实的配置 .conf 文件：
+# 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上你需要的配置即可
+# 不需要的配置设置为空，或者不用理会它，或者删除它也可以，看个人选择
+cp /root/mytemp/.conf DemoSpider/VIT/.conf
+
 # 生成爬虫脚本
 ayuge genspider <spider_name> <example.com>
 
-# 替换(覆盖)为真实的配置 .conf 文件；
-# 这里是为了演示方便，正常情况是直接在 VIT 路径下的 .conf 配置文件填上相关配置即可
-cp /root/mytemp/.conf DemoSpider/VIT/.conf
-
 # 运行脚本
 scrapy crawl <spider_name>
 # 注：也可以使用 ayuge crawl <spider_name>
 ```
 
 具体使用方法请在 [DemoSpider 之 AyugeSpiderTools 工具应用示例](https://github.com/shengchenyang/DemoSpider) 项目中查看，目前已适配以下场景：
 
@@ -147,17 +149,18 @@
 + 12).demo_proxy_two: 测试快代理独享代理
 
 +13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
 +14).demo_crawl: 支持 scrapy CrawlSpider 的示例
 
 # 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
 +15).demo_item_loader: 本库中使用 Item Loaders 的示例
--16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目标已经可以很方便的使用 Item Loaders 功能了
+-16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例，此示例已删除，可查看上个 demo_item_loader 中的示例，目前已经可以很方便的使用 Item Loaders 功能了
 
 +17).demo_mongo_async: asyncio 版本存储 mongoDB 的 pipelines 示例
++18).demo_mq: 数据存入 rabbitmq 的模板示例，通过 pika 库实现
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
```

