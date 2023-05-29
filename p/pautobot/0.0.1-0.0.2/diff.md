# Comparing `tmp/pautobot-0.0.1.tar.gz` & `tmp/pautobot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pautobot-0.0.1.tar", last modified: Mon May 29 16:54:29 2023, max compression
+gzip compressed data, was "pautobot-0.0.2.tar", last modified: Mon May 29 17:08:24 2023, max compression
```

## Comparing `pautobot-0.0.1.tar` & `pautobot-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.285418 pautobot-0.0.1/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       43 2023-05-29 15:46:53.000000 pautobot-0.0.1/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2179 2023-05-29 16:54:29.285206 pautobot-0.0.1/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1581 2023-05-29 16:47:40.000000 pautobot-0.0.1/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.256446 pautobot-0.0.1/pautobot/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.1/pautobot/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2143 2023-05-29 16:33:14.000000 pautobot-0.0.1/pautobot/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-29 16:49:00.000000 pautobot-0.0.1/pautobot/app_info.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      361 2023-05-28 11:30:55.000000 pautobot-0.0.1/pautobot/constants.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2203 2023-05-29 16:32:42.000000 pautobot-0.0.1/pautobot/engine.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.257948 pautobot-0.0.1/pautobot/frontend-dist/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/404.html
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.253948 pautobot-0.0.1/pautobot/frontend-dist/_next/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.254303 pautobot-0.0.1/pautobot/frontend-dist/_next/static/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.258247 pautobot-0.0.1/pautobot/frontend-dist/_next/static/5tPIGmEDN4M3XOC52jOUs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/5tPIGmEDN4M3XOC52jOUs/_buildManifest.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/5tPIGmEDN4M3XOC52jOUs/_ssgManifest.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.263962 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/
--rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.264502 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26529 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.264681 pautobot-0.0.1/pautobot/frontend-dist/_next/static/css/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31796 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/css/af0d632cb8ccd237.css
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.284960 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
--rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/favicon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9441 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/index.html
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/loading.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-29 16:54:25.000000 pautobot-0.0.1/pautobot/frontend-dist/pautobot.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)       97 2023-05-29 16:32:04.000000 pautobot-0.0.1/pautobot/global_state.py
--rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.1/pautobot/ingest.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       72 2023-05-29 14:44:03.000000 pautobot-0.0.1/pautobot/models.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      504 2023-05-29 16:14:07.000000 pautobot-0.0.1/pautobot/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 16:54:29.257234 pautobot-0.0.1/pautobot.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2179 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2944 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      239 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-29 16:54:29.000000 pautobot-0.0.1/pautobot.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.1/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-29 16:54:29.285494 pautobot-0.0.1/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2133 2023-05-29 16:49:13.000000 pautobot-0.0.1/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.624459 pautobot-0.0.2/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       43 2023-05-29 15:46:53.000000 pautobot-0.0.2/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2660 2023-05-29 17:08:24.624258 pautobot-0.0.2/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2062 2023-05-29 17:07:46.000000 pautobot-0.0.2/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.617248 pautobot-0.0.2/pautobot/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.2/pautobot/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2143 2023-05-29 16:33:14.000000 pautobot-0.0.2/pautobot/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-29 16:56:53.000000 pautobot-0.0.2/pautobot/app_info.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      361 2023-05-28 11:30:55.000000 pautobot-0.0.2/pautobot/constants.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2203 2023-05-29 16:32:42.000000 pautobot-0.0.2/pautobot/engine.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.618862 pautobot-0.0.2/pautobot/frontend-dist/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/404.html
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.615264 pautobot-0.0.2/pautobot/frontend-dist/_next/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.615614 pautobot-0.0.2/pautobot/frontend-dist/_next/static/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.619732 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.620201 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26529 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.620359 pautobot-0.0.2/pautobot/frontend-dist/_next/static/css/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31796 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/css/af0d632cb8ccd237.css
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.623736 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.624017 pautobot-0.0.2/pautobot/frontend-dist/_next/static/qcHNZJ7hKdY11NzKTWRhT/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/qcHNZJ7hKdY11NzKTWRhT/_buildManifest.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/_next/static/qcHNZJ7hKdY11NzKTWRhT/_ssgManifest.js
+-rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/favicon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9441 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/index.html
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/loading.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-29 17:08:20.000000 pautobot-0.0.2/pautobot/frontend-dist/pautobot.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       97 2023-05-29 16:32:04.000000 pautobot-0.0.2/pautobot/global_state.py
+-rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.2/pautobot/ingest.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       72 2023-05-29 14:44:03.000000 pautobot-0.0.2/pautobot/models.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      504 2023-05-29 16:14:07.000000 pautobot-0.0.2/pautobot/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 17:08:24.618119 pautobot-0.0.2/pautobot.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2660 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2944 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      239 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-29 17:08:24.000000 pautobot-0.0.2/pautobot.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.2/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-29 17:08:24.624512 pautobot-0.0.2/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2133 2023-05-29 16:49:13.000000 pautobot-0.0.2/setup.py
```

### Comparing `pautobot-0.0.1/PKG-INFO` & `pautobot-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-Metadata-Version: 2.1
-Name: pautobot
-Version: 0.0.1
-Summary: Private AutoGPT Robot - Your private task assistant with GPT!
-Home-page: https://github.com/vietanhdev/pautobot
-Author: Viet-Anh Nguyen
-Author-email: vietanh.dev@gmail.com
-License: Apache License 2.0
-Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-
 <p align="center">
-  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="./docs/pautobot.png"/>
+  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/pautobot.png"/>
   <h1 align="center">🔥 PⒶutoBot 🔥</h1>
   <p align="center" style="font-size:18px">Private AutoGPT Robot - Your private task assistant with GPT!</p>
 </p>
 
 **NOTE: This project is still in development.**
 
 - **Ask questions** to your documents without an internet connection, using the power of LLMs. 100% private, no data leaves your execution environment at any point. You can ingest documents and ask questions without an internet connection! Engine developed based on [PrivateGPT](https://github.com/imartinez/privateGPT).
 - **Automate tasks** easily with PAutoBot plugins. Easy for everyone!
 
-![PAutoBot](./docs/screenshot.png)
+![PAutoBot](https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/screenshot.png)
 
 **The supported extensions are:**
 
 - `.csv`: CSV,
 - `.docx`: Word Document,
 - `.doc`: Word Document,
 - `.enex`: EverNote,
@@ -40,15 +24,43 @@
 - `.msg`: Outlook Message,
 - `.odt`: Open Document Text,
 - `.pdf`: Portable Document Format (PDF),
 - `.pptx` : PowerPoint Document,
 - `.ppt` : PowerPoint Document,
 - `.txt`: Text file (UTF-8),
 
-## I. Installation
+# I. Installation and Usage
+
+## 1. Installation
+
+- Python 3.10 or higher.
+- Install **PAutoBot**:
+
+```shell
+pip install pautobot
+```
+
+## 2. Usage
+
+- Put your documents in `pautobot-data/documents` folder.
+- Ingest documents:
+
+```shell
+python -m pautobot.ingest
+```
+
+- Run the app:
+
+```shell
+python -m pautobot.app
+```
+
+Go to <http://localhost:5678/> to see the app.
+
+## II. Development
 
 ### 1. Backend
 
 - Python 3.10 or higher.
 - Install dependencies:
 
 ```shell
```

### Comparing `pautobot-0.0.1/README.md` & `pautobot-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,35 @@
+Metadata-Version: 2.1
+Name: pautobot
+Version: 0.0.2
+Summary: Private AutoGPT Robot - Your private task assistant with GPT!
+Home-page: https://github.com/vietanhdev/pautobot
+Author: Viet-Anh Nguyen
+Author-email: vietanh.dev@gmail.com
+License: Apache License 2.0
+Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+
 <p align="center">
-  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="./docs/pautobot.png"/>
+  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/pautobot.png"/>
   <h1 align="center">🔥 PⒶutoBot 🔥</h1>
   <p align="center" style="font-size:18px">Private AutoGPT Robot - Your private task assistant with GPT!</p>
 </p>
 
 **NOTE: This project is still in development.**
 
 - **Ask questions** to your documents without an internet connection, using the power of LLMs. 100% private, no data leaves your execution environment at any point. You can ingest documents and ask questions without an internet connection! Engine developed based on [PrivateGPT](https://github.com/imartinez/privateGPT).
 - **Automate tasks** easily with PAutoBot plugins. Easy for everyone!
 
-![PAutoBot](./docs/screenshot.png)
+![PAutoBot](https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/screenshot.png)
 
 **The supported extensions are:**
 
 - `.csv`: CSV,
 - `.docx`: Word Document,
 - `.doc`: Word Document,
 - `.enex`: EverNote,
@@ -24,15 +40,43 @@
 - `.msg`: Outlook Message,
 - `.odt`: Open Document Text,
 - `.pdf`: Portable Document Format (PDF),
 - `.pptx` : PowerPoint Document,
 - `.ppt` : PowerPoint Document,
 - `.txt`: Text file (UTF-8),
 
-## I. Installation
+# I. Installation and Usage
+
+## 1. Installation
+
+- Python 3.10 or higher.
+- Install **PAutoBot**:
+
+```shell
+pip install pautobot
+```
+
+## 2. Usage
+
+- Put your documents in `pautobot-data/documents` folder.
+- Ingest documents:
+
+```shell
+python -m pautobot.ingest
+```
+
+- Run the app:
+
+```shell
+python -m pautobot.app
+```
+
+Go to <http://localhost:5678/> to see the app.
+
+## II. Development
 
 ### 1. Backend
 
 - Python 3.10 or higher.
 - Install dependencies:
 
 ```shell
```

### Comparing `pautobot-0.0.1/pautobot/app.py` & `pautobot-0.0.2/pautobot/app.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/engine.py` & `pautobot-0.0.2/pautobot/engine.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/404.html` & `pautobot-0.0.2/pautobot/frontend-dist/404.html`

 * *Files 10% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/af0d632cb8ccd237.css" as="style"/><link rel="stylesheet" href="/_next/static/css/af0d632cb8ccd237.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/5tPIGmEDN4M3XOC52jOUs/_buildManifest.js" defer=""></script><script src="/_next/static/5tPIGmEDN4M3XOC52jOUs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"5tPIGmEDN4M3XOC52jOUs","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/af0d632cb8ccd237.css" as="style"/><link rel="stylesheet" href="/_next/static/css/af0d632cb8ccd237.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/qcHNZJ7hKdY11NzKTWRhT/_buildManifest.js" defer=""></script><script src="/_next/static/qcHNZJ7hKdY11NzKTWRhT/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"qcHNZJ7hKdY11NzKTWRhT","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/css/af0d632cb8ccd237.css` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/css/af0d632cb8ccd237.css`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2` & `pautobot-0.0.2/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/favicon.ico` & `pautobot-0.0.2/pautobot/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/index.html` & `pautobot-0.0.2/pautobot/frontend-dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/af0d632cb8ccd237.css" as="style"/><link rel="stylesheet" href="/_next/static/css/af0d632cb8ccd237.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js" defer=""></script><script src="/_next/static/5tPIGmEDN4M3XOC52jOUs/_buildManifest.js" defer=""></script><script src="/_next/static/5tPIGmEDN4M3XOC52jOUs/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 p-2"><button type="button" class="inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg><span class="sr-only">Upload image</span></button><textarea rows="2" class="block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"5tPIGmEDN4M3XOC52jOUs","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/af0d632cb8ccd237.css" as="style"/><link rel="stylesheet" href="/_next/static/css/af0d632cb8ccd237.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js" defer=""></script><script src="/_next/static/qcHNZJ7hKdY11NzKTWRhT/_buildManifest.js" defer=""></script><script src="/_next/static/qcHNZJ7hKdY11NzKTWRhT/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 p-2"><button type="button" class="inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg><span class="sr-only">Upload image</span></button><textarea rows="2" class="block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-lg border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"qcHNZJ7hKdY11NzKTWRhT","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/loading.svg` & `pautobot-0.0.2/pautobot/frontend-dist/loading.svg`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/frontend-dist/pautobot.png` & `pautobot-0.0.2/pautobot/frontend-dist/pautobot.png`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot/ingest.py` & `pautobot-0.0.2/pautobot/ingest.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.1/pautobot.egg-info/PKG-INFO` & `pautobot-0.0.2/pautobot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="./docs/pautobot.png"/>
+  <img alt="PAutoBot" style="width: 128px; max-width: 100%; height: auto;" src="https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/pautobot.png"/>
   <h1 align="center">🔥 PⒶutoBot 🔥</h1>
   <p align="center" style="font-size:18px">Private AutoGPT Robot - Your private task assistant with GPT!</p>
 </p>
 
 **NOTE: This project is still in development.**
 
 - **Ask questions** to your documents without an internet connection, using the power of LLMs. 100% private, no data leaves your execution environment at any point. You can ingest documents and ask questions without an internet connection! Engine developed based on [PrivateGPT](https://github.com/imartinez/privateGPT).
 - **Automate tasks** easily with PAutoBot plugins. Easy for everyone!
 
-![PAutoBot](./docs/screenshot.png)
+![PAutoBot](https://raw.githubusercontent.com/vietanhdev/pautobot/main/docs/screenshot.png)
 
 **The supported extensions are:**
 
 - `.csv`: CSV,
 - `.docx`: Word Document,
 - `.doc`: Word Document,
 - `.enex`: EverNote,
@@ -40,15 +40,43 @@
 - `.msg`: Outlook Message,
 - `.odt`: Open Document Text,
 - `.pdf`: Portable Document Format (PDF),
 - `.pptx` : PowerPoint Document,
 - `.ppt` : PowerPoint Document,
 - `.txt`: Text file (UTF-8),
 
-## I. Installation
+# I. Installation and Usage
+
+## 1. Installation
+
+- Python 3.10 or higher.
+- Install **PAutoBot**:
+
+```shell
+pip install pautobot
+```
+
+## 2. Usage
+
+- Put your documents in `pautobot-data/documents` folder.
+- Ingest documents:
+
+```shell
+python -m pautobot.ingest
+```
+
+- Run the app:
+
+```shell
+python -m pautobot.app
+```
+
+Go to <http://localhost:5678/> to see the app.
+
+## II. Development
 
 ### 1. Backend
 
 - Python 3.10 or higher.
 - Install dependencies:
 
 ```shell
```

### Comparing `pautobot-0.0.1/pautobot.egg-info/SOURCES.txt` & `pautobot-0.0.2/pautobot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 pautobot.egg-info/requires.txt
 pautobot.egg-info/top_level.txt
 pautobot/frontend-dist/404.html
 pautobot/frontend-dist/favicon.ico
 pautobot/frontend-dist/index.html
 pautobot/frontend-dist/loading.svg
 pautobot/frontend-dist/pautobot.png
-pautobot/frontend-dist/_next/static/5tPIGmEDN4M3XOC52jOUs/_buildManifest.js
-pautobot/frontend-dist/_next/static/5tPIGmEDN4M3XOC52jOUs/_ssgManifest.js
 pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
 pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
 pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
 pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
 pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 pautobot/frontend-dist/_next/static/chunks/pages/index-8c42ca55b8b83a4c.js
@@ -51,8 +49,10 @@
 pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
 pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
 pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
 pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
 pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
-pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+pautobot/frontend-dist/_next/static/qcHNZJ7hKdY11NzKTWRhT/_buildManifest.js
+pautobot/frontend-dist/_next/static/qcHNZJ7hKdY11NzKTWRhT/_ssgManifest.js
```

### Comparing `pautobot-0.0.1/setup.py` & `pautobot-0.0.2/setup.py`

 * *Files identical despite different names*

