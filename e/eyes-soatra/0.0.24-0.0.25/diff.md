# Comparing `tmp/eyes_soatra-0.0.24.tar.gz` & `tmp/eyes_soatra-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.24.tar", last modified: Tue May 23 06:21:56 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.25.tar", last modified: Mon May 29 05:04:49 2023, max compression
```

## Comparing `eyes_soatra-0.0.24.tar` & `eyes_soatra-0.0.25.tar`

### file list

```diff
@@ -1,46 +1,55 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.981136 eyes_soatra-0.0.24/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.24/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-23 06:21:56.980962 eyes_soatra-0.0.24/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.24/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.973509 eyes_soatra-0.0.24/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.24/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974510 eyes_soatra-0.0.24/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.24/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974739 eyes_soatra-0.0.24/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.975449 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      395 2023-05-23 05:04:15.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/end.py
--rw-r--r--   0 soatra     (501) staff       (20)      260 2023-05-23 04:44:21.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      261 2023-05-23 04:44:37.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976019 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/not_found.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976352 eyes_soatra-0.0.24/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.24/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.24/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976656 eyes_soatra-0.0.24/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.24/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.24/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      220 2023-05-23 02:00:10.000000 eyes_soatra-0.0.24/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      109 2023-05-23 06:21:34.000000 eyes_soatra-0.0.24/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.979417 eyes_soatra-0.0.24/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6994 2023-05-23 06:20:17.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/app_span.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.980047 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)       82 2023-05-23 02:06:48.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)    12655 2023-05-23 06:16:25.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974240 eyes_soatra-0.0.24/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1050 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-23 06:21:56.981193 eyes_soatra-0.0.24/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-23 02:47:19.000000 eyes_soatra-0.0.24/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.980607 eyes_soatra-0.0.24/test/
--rw-r--r--   0 soatra     (501) staff       (20)     4574 2023-05-23 05:08:45.000000 eyes_soatra-0.0.24/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)      250 2023-05-23 06:16:40.000000 eyes_soatra-0.0.24/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.985983 eyes_soatra-0.0.25/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.25/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-29 05:04:49.985853 eyes_soatra-0.0.25/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.25/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.977736 eyes_soatra-0.0.25/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.25/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978774 eyes_soatra-0.0.25/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.25/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978921 eyes_soatra-0.0.25/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.979504 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980141 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980548 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.25/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.980816 eyes_soatra-0.0.25/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.25/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.25/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.981171 eyes_soatra-0.0.25/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.25/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.25/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      747 2023-05-29 02:30:09.000000 eyes_soatra-0.0.25/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      107 2023-05-23 06:52:23.000000 eyes_soatra-0.0.25/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.983714 eyes_soatra-0.0.25/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    19464 2023-05-29 04:46:40.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.984301 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1221 2023-05-27 07:50:00.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    12976 2023-05-29 05:03:23.000000 eyes_soatra-0.0.25/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.978423 eyes_soatra-0.0.25/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1363 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-29 05:04:49.000000 eyes_soatra-0.0.25/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-29 05:04:49.986027 eyes_soatra-0.0.25/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-29 05:00:38.000000 eyes_soatra-0.0.25/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-29 05:04:49.985223 eyes_soatra-0.0.25/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.25/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.25/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      373 2023-05-29 05:02:06.000000 eyes_soatra-0.0.25/test/test2.py
+-rw-r--r--   0 soatra     (501) staff       (20)    86427 2023-05-28 08:14:58.000000 eyes_soatra-0.0.25/test/test3.py
```

### Comparing `eyes_soatra-0.0.24/PKG-INFO` & `eyes_soatra-0.0.25/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes_soatra
-Version: 0.0.24
+Name: eyes-soatra
+Version: 0.0.25
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.25/eyes_soatra/constant/depends/view/not_found.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,23 @@
     "NotFound",
     "Oops! That page can’t be found.",
     "Page not found.",
     "The page you were looking for doesn't exist.",
     "Web ページが見つかりません。",
     "【404 NOT FOUND】 ご指定のページは見つかりませんでした",
     "【NOT FOUND】 ご指定のページは見つかりませんでした。",
-    "お手数ですが、再度キーワードを入力してください",
     "お探しのコンテンツはみつかりませんでした。",
     "お探しのページ、またはファイルは見つかりませんでした。",
-    # "お探しのページが", the page you looking for
     "お探しのページが見つかりません",
     "お探しのページが見つかりません / NotFound",
     "お探しのページが見つかりません。",
     "お探しのページが見つかりませんでした",
     "お探しのページが見つかりませんでした。",
     "お探しのページが見つかりませんでした！",
-    "お探しのページが見つかりません（サイト内検索をご利用ください）",
+    "お探しのページが見つかりません",
     "お探しのページは、更新中のため、表示することができませんでした。",
     "お探しのページはありません",
     "お探しのページはありません。",
     "お探しのページはありませんでした",
     "お探しのページはありません（404）",
     "お探しのページはみつかりません",
     "お探しのページはみつかりませんでした（404 Not Found）",
@@ -90,15 +88,14 @@
     "エラーが発生しました。",
     "エラーページ",
     "コンテンツを表示することができません",
     "コンテンツを表示することができません。",
     "サーバー エラーが発生しました。（タイムアウトの可能性もあります）",
     "システムエラー",
     "ファイルが見つかりません",
-    "ブックマーク、他サイトからのリンク、サーチエンジンなどから訪問された方へ",
     "ページがみつかりません",
     "ページがみつかりません - 404 Not Found -",
     "ページがみつかりませんでした",
     "ページが見つかりません",
     "ページが見つかりません Not Found",
     "ページが見つかりません （404 Not Found)",
     "ページが見つかりません。",
@@ -131,12 +128,11 @@
     "指定のページは見つかりませんでした",
     "検索したページは見つかりませんでした",
     "現在接続されているページは、ページ移行されました。",
     "表示できません",
     "見つかりません",
     "見つかりません。",
     "見つかりませんでした。",
-    "該当のページを表示できません。",
     "お探しのページが見つかりません-",
     "時的にご利用いただけません",
     "ホームページはリニューアルしました"
 ]
```

### Comparing `eyes_soatra-0.0.24/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.25/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.24/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.25/eyes_soatra/funcs/view_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!python3
 from eyes_soatra.constant.depends.view.no_data import depends as __depends_no_data
 from eyes_soatra.constant.depends.view.not_found import depends as __depends_404
 from eyes_soatra.constant.user.user_agents import User_Agents as __User_Agents
 from eyes_soatra.constant.libs.requests import requests as __requests
-from eyes_soatra.constant.vars import all_header_xpaths as __header_xpaths_all
-from eyes_soatra.funcs.utils.dict import sort_dict as __sort_dict
-from eyes_soatra.funcs.utils.string import strip as __strip
+from eyes_soatra.constant.vars import header_xpaths as __header_xpaths_all
+from eyes_soatra.constant.vars import remove_tags as __remove_tags
+from eyes_soatra.funcs.utils.string import strip_space as __strip_space
 
 from translate import Translator as __Translator
-from requests_html import HTML as __HTML
+from lxml import html as __html
+from lxml import etree as __etree
 
 import jellyfish as __jellyfish
 import random as __random
 import time as __time
 import re as __re
 
-
 # private global variables
 __separator = '\||-|:'
 __header_min_length = 3
 __paragraph_min_length = 7
+__content_min_length = 1
 __container = 'self::div or self::span or self::table'
 __header_xpaths = [
     '//title',
     '//h1[self::*//text() and last()=1]',
     '//h2[self::*//text() and last()=1]'
 ]
 __paragraph_xpaths = [
@@ -32,93 +33,87 @@
     '//h1[self::*//text()]/following-sibling::*//p[1]',
     f'//*[({__container}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{__container}]//p[1]'
 ]
 __content_xpaths = [
     '//h1[self::*//text()]/following-sibling::*|//h1[self::*//text()]/following-sibling::*//*|//*[self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1]//*'
 ]
 
-def __get_highlight(
-    html,
-    header_xpath,
-    paragraph_xpath,
-    content_xpath,
-    allow_all_tags,
-):
-    html = __HTML(html=html)
-    highlight = __highlighter(
-        html,
-        header_xpath,
-        paragraph_xpath,
-        content_xpath,
-        allow_all_tags,
-    )
-    
+def __translate(lang, highlight):
+    if not (lang == 'ja' or lang == 'en'):
+        translate = __Translator(from_lang=lang, to_lang='en')
+        
+        for key in highlight:
+            for i in range(0, len(highlight[key])):
+                highlight[key][i] = translate.translate(highlight[key][i])
+                
     return highlight
 
 def __highlighter(
     html,
     header_xpath,
     paragraph_xpath,
     content_xpath,
     allow_all_tags,
+    separator
 ):
     header_texts = []
     paragraph_texts = []
     content_texts = []
+    separator = __separator + (separator if separator else '')
     
     for xpath in (__header_xpaths_all if allow_all_tags else __header_xpaths) + (header_xpath if type(header_xpath) == list else []):
-        header_list = html.xpath(f'({xpath})//text()')
+        element_list = html.xpath(xpath)
         
-        for header in header_list:
-            header = __strip(header)
+        for element in element_list:
+            header_list = element.xpath('.//text()')
             
-            if len(header) >= __header_min_length:
-                header_texts.append(header)
+            for header in header_list:
+                for token in __re.split(separator, header):
+                    token = __strip_space(token)
+                    
+                    if len(token) >= __header_min_length:
+                        header_texts.append(token)
     
     for xpath in __paragraph_xpaths + (paragraph_xpath if type(paragraph_xpath) == list else []):
-        paragraph_list = html.xpath(f'({xpath})//text()')
+        element_list = html.xpath(xpath)
         
-        for paragraph in paragraph_list:
-            paragraph = __strip(paragraph)
+        for element in element_list:
+            paragraph_list = element.xpath('.//text()')
             
-            if len(paragraph) >= __paragraph_min_length:
-                paragraph_texts.append(paragraph)
+            for paragraph in paragraph_list:
+                for token in __re.split(separator, paragraph):
+                    token = __strip_space(token)
 
-            if len(paragraph_texts):
-                break
-            
-        # for paragraph in paragraph_list:
+                    if len(token) >= __paragraph_min_length:
+                        paragraph_texts.append(token)
     
     for xpath in __content_xpaths + (content_xpath if type(content_xpath) == list else []):
-        content_list = html.xpath(f'({xpath})//text()')
+        element_list = html.xpath(xpath)
         
-        for content in content_list:
-            content = __strip(content)
+        for element in element_list:
+            content_list = element.xpath('.//text()')
             
-            if len(content) > 0:
-                content_texts.append(content)
-
-            if len(content_texts):
-                break
-            
-        # for content in content_list:
+            for content in content_list:
+                for token in __re.split(separator, content):
+                    token = __strip_space(token)
+                    
+                    if len(token) >= __content_min_length:
+                        content_texts.append(token)
             
     return {
         'headers': header_texts,
         'paragraphs': paragraph_texts,
         'contents': content_texts,
     }
 
 def __bad_page(
     highlight,
-    separator,
     depends,
     header_min_point,
     paragraph_min_point,
-    
     show_highlight,
     show_header,
     show_paragraph,
     show_content,
 ):
     header_high_point = 0
     paragraph_high_point = 0
@@ -130,103 +125,79 @@
     result = {
         'active': True,
         'informed': False,
         'blank': False,
         'checked': True,
         **({'highlight': highlight} if show_highlight else {})
     }
-    
-    # check active
+
     if len(headers):
         header_similar = ''
         header_keyword = ''
-        broke = False
         
         for depend in __depends_404 + (depends if type(depends) == list else []):
-            for header in headers:                
-                for token_header in __re.split(__separator + (separator if separator else ''), header):
-                    token_header = __strip(token_header)
+            for token in headers:                
+                point = __jellyfish.jaro_similarity(depend, token)
+                
+                if point > header_high_point:
+                    header_high_point = point
+                    header_similar = depend
+                    header_keyword = token
                     
-                    if len(token_header) >= __header_min_length:
-                        s1 = __jellyfish.jaro_similarity(depend, token_header)
-                        points = s1
-                        
-                        if points > header_high_point:
-                            header_high_point = points
-                            header_similar = depend
-                            header_keyword = token_header
-                            
-                        if points >= header_min_point:
-                            result = {
-                                **result,
-                                'active': False,
-                            }
-                            
-                            broke = True
-                            break
-                if broke:
+                if point >= header_min_point:
+                    result = {
+                        **result,
+                        'active': False,
+                    }
                     break
                 
         if header_high_point > 0 and show_header:
             result = {
                 **result,
                 'header': {
                     'keyword': header_keyword,
                     'similar-to': header_similar,
                     'points': round(header_high_point, 2),
                 }
             }
 
-    # check informed
     if len(paragraphs):
         paragraph_similar = ''
         paragraph_keyword = ''
-        broke = False
         
         for depend in __depends_no_data + (depends if type(depends) == list else []):
-            for paragraph in paragraphs:
-                for token_paragraph in __re.split(__separator + (separator if separator else ''), paragraph):
-                    token_paragraph = __strip(token_paragraph)
+            for token in paragraphs:
+                point = __jellyfish.jaro_similarity(depend, token)
+                
+                if point > paragraph_high_point:
+                    paragraph_high_point = point
+                    paragraph_similar = depend
+                    paragraph_keyword = token
                     
-                    if len(token_paragraph) >= __paragraph_min_length:
-                        s1 = __jellyfish.jaro_similarity(depend, token_paragraph)
-                        points = s1
-                        
-                        if points > paragraph_high_point:
-                            paragraph_high_point = points
-                            paragraph_similar = depend
-                            paragraph_keyword = token_paragraph
-                            
-                        if points >= paragraph_min_point:
-                            result = {
-                                **result,
-                                'informed': True,
-                            }
-                            
-                            broke = True
-                            break
-                if broke:
+                if point >= paragraph_min_point:
+                    result = {
+                        **result,
+                        'informed': True,
+                    }
                     break
                 
         if paragraph_high_point > 0 and show_paragraph:
             result = {
                 **result,
                 'paragraph': {
                     'keyword': paragraph_keyword,
                     'similar-to': paragraph_similar,
                     'points': round(paragraph_high_point, 2)
                 }
             }
-    
-    # check blank
+
     if len(contents) == 0 and show_content:
         result = {
             **result,
             'blank': True,
-            'content': contents
         }
         
     return result
 
 # ------------------------ public function
 def view_page(
     url,
@@ -235,31 +206,34 @@
     verify=False,
     headers=None,
     depends=None,
     separator=None,
     sleep_reject=2,
     tries_timeout=3,
     tries_reject=25,
+    tries_forward=10,
     header_xpath=None,
     paragraph_xpath=None,
     content_xpath=None,
     allow_redirects=True,
     allow_all_header_tags=True,
     header_min_point=0.8,
     paragraph_min_point=0.85,
     
-    show_highlight = False,
-    show_header = False,
-    show_paragraph = False,
-    show_content = False,
+    show_highlight=False,
+    show_header=False,
+    show_paragraph=False,
+    show_content=False,
     
     **requests_options
 ):
+    url = __re.sub(r'\s', '', url)
     tried = 0
     agents = []
+    redirected_forward = False
     
     while True:
         try:
             tried += 1
             user_agent = __random.choice(__User_Agents)
             
             while user_agent in agents:
@@ -279,98 +253,122 @@
                     'ACCEPT' : 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
                     'ACCEPT-ENCODING' : 'gzip, deflate, br',
                     'ACCEPT-LANGUAGE' : 'en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,km-KH;q=0.6,km;q=0.5,ja-JP;q=0.4,ja;q=0.3',
                     'REFERER' : 'https://www.google.com/'
                 },
             )
             status_code = response.status_code
-            redirected = response.is_redirect
+            redirected = redirected_forward if redirected_forward else response.is_redirect
             expired = response.headers.get('Expires')
             expired = expired if expired else (response.headers.get('expires') or False)
             expired_obj = {'expired': expired} if expired else {}
             
             if status_code >= 400 and status_code <= 499:
-                return __sort_dict({
+                return {
                     'active': False,
                     'checked': False,
                     **expired_obj,
                     'error': f'Client error responses: {status_code}',
                     'redirected': redirected,
                     'url': response.url,
                     'status': status_code,
                     'tried': tried,
-                })
+                }
                 
             if status_code >= 500 and status_code <= 599:
-                return __sort_dict({
+                return {
                     'active': False,
                     'checked': False,
                     **expired_obj,
                     'error': f'Server error responses: {status_code}',
                     'redirected': redirected,
                     'url': response.url,
                     'status': status_code,
                     'tried': tried,
-                })
-    
-            html = response.content
-            highlight = __get_highlight(
+                }
+
+            html = __html.fromstring(response.content)
+            __etree.strip_elements(html, *__remove_tags)
+            
+            if allow_redirects:
+                meta_refresh = html.xpath("//meta[translate(@http-equiv,'REFSH','refsh')='refresh']/@content")
+                
+                if len(meta_refresh):
+                    if tried < tries_forward:
+                        content_refresh = meta_refresh[0]
+                        content_slices = content_refresh.split(';')
+                        
+                        if len(content_slices) > 1:
+                            url_refresh = __strip_space(content_slices[1])
+                            
+                            if url_refresh.lower().startswith('url='):
+                                url_refresh = url_refresh[4:]
+                                
+                            redirected_forward = True
+                            url = url_refresh
+                            continue
+
+                    else:
+                        return {
+                            'active': None,
+                            'checked': False,
+                            'error': f'Out of forwarding tries.',
+                            'redirected': True,
+                            'url': url,
+                            'tried': tried
+                        }
+
+            highlight = __highlighter(
                 html,
                 header_xpath,
                 paragraph_xpath,
                 content_xpath,
-                allow_all_header_tags
+                allow_all_header_tags,
+                separator
             )
+            highlight = __translate(lang, highlight)
             
-            if not (lang == 'ja' or lang == 'en'):
-                translate = __Translator(from_lang=lang, to_lang='en')
-                
-                for key in highlight:
-                    for i in range(0, len(highlight[key])):
-                        highlight[key][i] = translate.translate(highlight[key][i])
-            
-            return __sort_dict({
+            return {
                 **__bad_page(
                     highlight,
-                    separator,
                     depends,
                     header_min_point,
                     paragraph_min_point,
                     
                     show_highlight,
                     show_header,
                     show_paragraph,
                     show_content,
                 ),
                 **expired_obj,
                 'redirected': redirected,
                 'url': response.url,
                 'status': status_code,
                 'tried': tried,
-            })
+            }
 
-        except Exception as error:                    
+        except Exception as error:
             if (
                 type(error) == __requests.exceptions.ConnectionError or
                 type(error) == __requests.exceptions.SSLError
             ):
                 if tried >= tries_reject:
-                    return __sort_dict({
+                    return {
                         'active': None,
                         'checked': False,
                         'error': f'{error.__class__.__name__}: {error}',
                         'redirected': False,
                         'url': url,
                         'tried': tried
-                    })
+                    }
                 __time.sleep(sleep_reject)
                 
             else :
                 if tried >= tries_timeout:
-                    return __sort_dict({
+                    return {
                         'active': None,
                         'checked': False,
                         'error': f'{error.__class__.__name__}: {error}',
                         'redirected': False,
                         'url': url,
                         'tried': tried
-                    })
+                    }
```

### Comparing `eyes_soatra-0.0.24/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.25/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes-soatra
-Version: 0.0.24
+Name: eyes_soatra
+Version: 0.0.25
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.24/setup.py` & `eyes_soatra-0.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.24'
+VERSION = '0.0.25'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

