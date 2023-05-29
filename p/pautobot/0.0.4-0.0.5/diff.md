# Comparing `tmp/pautobot-0.0.4.tar.gz` & `tmp/pautobot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pautobot-0.0.4.tar", last modified: Mon May 29 18:50:39 2023, max compression
+gzip compressed data, was "pautobot-0.0.5.tar", last modified: Mon May 29 19:20:52 2023, max compression
```

## Comparing `pautobot-0.0.4.tar` & `pautobot-0.0.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.291016 pautobot-0.0.4/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       43 2023-05-29 15:46:53.000000 pautobot-0.0.4/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2412 2023-05-29 18:50:39.290601 pautobot-0.0.4/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1948 2023-05-29 17:29:44.000000 pautobot-0.0.4/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.280416 pautobot-0.0.4/pautobot/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.4/pautobot/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1297 2023-05-29 18:29:27.000000 pautobot-0.0.4/pautobot/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-29 18:48:14.000000 pautobot-0.0.4/pautobot/app_info.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      361 2023-05-28 11:30:55.000000 pautobot-0.0.4/pautobot/constants.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5057 2023-05-29 18:38:03.000000 pautobot-0.0.4/pautobot/engine.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.282041 pautobot-0.0.4/pautobot/frontend-dist/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/404.html
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.277987 pautobot-0.0.4/pautobot/frontend-dist/_next/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.278334 pautobot-0.0.4/pautobot/frontend-dist/_next/static/
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.282908 pautobot-0.0.4/pautobot/frontend-dist/_next/static/ODkvowHBq7dIAIxGbudlb/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/ODkvowHBq7dIAIxGbudlb/_buildManifest.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/ODkvowHBq7dIAIxGbudlb/_ssgManifest.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.284389 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/
--rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.285097 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26587 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.285496 pautobot-0.0.4/pautobot/frontend-dist/_next/static/css/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    32027 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.290403 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
--rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/favicon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9488 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/index.html
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/loading.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-29 18:50:36.000000 pautobot-0.0.4/pautobot/frontend-dist/pautobot.png
--rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.4/pautobot/ingest.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       72 2023-05-29 14:44:03.000000 pautobot-0.0.4/pautobot/models.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      504 2023-05-29 16:14:07.000000 pautobot-0.0.4/pautobot/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 18:50:39.281268 pautobot-0.0.4/pautobot.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2412 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2919 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      239 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-29 18:50:39.000000 pautobot-0.0.4/pautobot.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.4/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-29 18:50:39.291054 pautobot-0.0.4/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2416 2023-05-29 17:41:30.000000 pautobot-0.0.4/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.800531 pautobot-0.0.5/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       71 2023-05-29 18:54:55.000000 pautobot-0.0.5/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-29 19:20:52.800382 pautobot-0.0.5/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1518 2023-05-29 19:20:36.000000 pautobot-0.0.5/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.794236 pautobot-0.0.5/pautobot/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-05-29 14:28:20.000000 pautobot-0.0.5/pautobot/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1517 2023-05-29 19:17:04.000000 pautobot-0.0.5/pautobot/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       47 2023-05-29 19:18:36.000000 pautobot-0.0.5/pautobot/app_info.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      418 2023-05-29 18:58:38.000000 pautobot-0.0.5/pautobot/constants.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5057 2023-05-29 18:38:03.000000 pautobot-0.0.5/pautobot/engine.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      243 2023-05-29 16:06:06.000000 pautobot-0.0.5/pautobot/example.env
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.795725 pautobot-0.0.5/pautobot/frontend-dist/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4096 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/404.html
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.792008 pautobot-0.0.5/pautobot/frontend-dist/_next/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.792346 pautobot-0.0.5/pautobot/frontend-dist/_next/static/
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.796011 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      282 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       77 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.796711 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   141052 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    95653 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.797072 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      727 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      247 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26587 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    91460 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1430 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.797216 pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    32027 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.800207 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8852 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8972 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8992 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3528 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3492 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9012 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9392 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3572 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9564 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10728 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9276 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9004 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10656 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9144 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8828 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9036 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10428 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3488 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3576 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9604 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10632 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3516 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10840 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10808 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2
+-rw-rw-r--   0 vietanhdev   (501) staff       (20)    15406 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/favicon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9488 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/index.html
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2925 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/loading.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26848 2023-05-29 19:20:49.000000 pautobot-0.0.5/pautobot/frontend-dist/pautobot.png
+-rwxr-xr-x   0 vietanhdev   (501) staff       (20)     6468 2023-05-29 16:52:48.000000 pautobot-0.0.5/pautobot/ingest.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       72 2023-05-29 14:44:03.000000 pautobot-0.0.5/pautobot/models.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2437 2023-05-29 19:13:47.000000 pautobot-0.0.5/pautobot/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-05-29 19:20:52.795052 pautobot-0.0.5/pautobot.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1982 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2940 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       86 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      248 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        9 2023-05-29 19:20:52.000000 pautobot-0.0.5/pautobot.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      266 2023-05-29 14:25:31.000000 pautobot-0.0.5/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-05-29 19:20:52.800568 pautobot-0.0.5/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2436 2023-05-29 19:08:44.000000 pautobot-0.0.5/setup.py
```

### Comparing `pautobot-0.0.4/PKG-INFO` & `pautobot-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
@@ -67,43 +67,7 @@
 - Run the app:
 
 ```shell
 python -m pautobot.app
 ```
 
 Go to <http://localhost:5678/> to see the app.
-
-## II. Development
-
-### 1. Backend
-
-- Python 3.10 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-backend
-pip install -r requirements.txt
-```
-
-- Run the backend:
-
-```shell
-uvicorn main:app --reload --port 5678
-```
-
-### 2. Frontend
-
-- Node.js 16.0.0 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-frontend
-npm install
-```
-
-- Run the frontend:
-
-```shell
-npm run dev
-```
-
-Go to <http://localhost:3000/> to see the app.
```

### Comparing `pautobot-0.0.4/README.md` & `pautobot-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -51,43 +51,7 @@
 - Run the app:
 
 ```shell
 python -m pautobot.app
 ```
 
 Go to <http://localhost:5678/> to see the app.
-
-## II. Development
-
-### 1. Backend
-
-- Python 3.10 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-backend
-pip install -r requirements.txt
-```
-
-- Run the backend:
-
-```shell
-uvicorn main:app --reload --port 5678
-```
-
-### 2. Frontend
-
-- Node.js 16.0.0 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-frontend
-npm install
-```
-
-- Run the frontend:
-
-```shell
-npm run dev
-```
-
-Go to <http://localhost:3000/> to see the app.
```

### Comparing `pautobot-0.0.4/pautobot/app.py` & `pautobot-0.0.5/pautobot/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 import uvicorn
 from fastapi.staticfiles import StaticFiles
 from fastapi import FastAPI, BackgroundTasks
 from fastapi.middleware.cors import CORSMiddleware
 
 from pautobot.engine import PautoBotEngine, BotStatus, BotMode
 from pautobot.models import Query
-from pautobot.utils import extract_frontend_dist
-
-static_folder = "pautobot-data/frontend-dist"
-
-engine = PautoBotEngine(mode=BotMode.CHAT)
-
-app = FastAPI()
-app.add_middleware(
-    CORSMiddleware,
-    allow_origins=["*"],
-    allow_methods=["*"],
-    allow_headers=["*"],
+from pautobot.utils import (
+    extract_frontend_dist,
+    init_env_file,
+    download_model_if_needed,
 )
 
 
-@app.post("/api/ask")
-async def ask(query: Query, background_tasks: BackgroundTasks):
-    global engine
-    if engine.current_answer["status"] == BotStatus.THINKING:
-        raise Exception("I am still thinking! Please wait.")
-    engine.current_answer = {
-        "status": BotStatus.THINKING,
-        "answer": "",
-        "docs": [],
-    }
-    background_tasks.add_task(engine.query, query.query)
-    return {"message": "Query received"}
-
-
-@app.get("/api/get_answer")
-async def get_answer():
-    global engine
-    return engine.get_answer()
-
+def main():
+    init_env_file()
+    download_model_if_needed()
+    static_folder = "pautobot-data/frontend-dist"
+    extract_frontend_dist(static_folder)
 
-app.mount("/", StaticFiles(directory=static_folder, html=True), name="static")
+    # PautoBot engine
+    engine = PautoBotEngine(mode=BotMode.CHAT)
 
+    # Backend app
+    app = FastAPI()
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["*"],
+        allow_methods=["*"],
+        allow_headers=["*"],
+    )
+
+    @app.post("/api/ask")
+    async def ask(query: Query, background_tasks: BackgroundTasks):
+        if engine.current_answer["status"] == BotStatus.THINKING:
+            raise Exception("I am still thinking! Please wait.")
+        engine.current_answer = {
+            "status": BotStatus.THINKING,
+            "answer": "",
+            "docs": [],
+        }
+        background_tasks.add_task(engine.query, query.query)
+        return {"message": "Query received"}
+
+    @app.get("/api/get_answer")
+    async def get_answer():
+        return engine.get_answer()
+
+    app.mount(
+        "/", StaticFiles(directory=static_folder, html=True), name="static"
+    )
 
-def main():
-    extract_frontend_dist(static_folder)
     uvicorn.run(app, host="0.0.0.0", port=5678)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pautobot-0.0.4/pautobot/engine.py` & `pautobot-0.0.5/pautobot/engine.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/404.html` & `pautobot-0.0.5/pautobot/frontend-dist/404.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/ODkvowHBq7dIAIxGbudlb/_buildManifest.js" defer=""></script><script src="/_next/static/ODkvowHBq7dIAIxGbudlb/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"ODkvowHBq7dIAIxGbudlb","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"Dl9fVCNsnbVyvPy7nTli-","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/css/a4a6346dff75e1d3.css`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/037c6ceced78c87a-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/03a2ebda46411260-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/2cffe11a47028c14-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4ab03c045edad786-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/4cf1eda6528c4545-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/51fbb2aa5ef2b5cf-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/560bcc4e09749527-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/6cb9e821df97febd-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/723f3c07bb1fbaab-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/7da2a3ff16027414-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/84c22514fc6f1667-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/8bbb723f6276338f-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/996798fe8aee0dc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9b206b5a69aba6d3-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/9d76af61a4574a5c-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/a8c682a8f4ee9d69-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/c5fea7478aa47814-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/d77e36fa1e563bf0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/efe191cf7953ff64-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1144ac8e703eb32-s.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f1520da2fce335b3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f5ea4559b0835633-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/f6441c9c7c6cedc3-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2` & `pautobot-0.0.5/pautobot/frontend-dist/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/favicon.ico` & `pautobot-0.0.5/pautobot/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/index.html` & `pautobot-0.0.5/pautobot/frontend-dist/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-62fdb7c7217c2fea.js" defer=""></script><script src="/_next/static/ODkvowHBq7dIAIxGbudlb/_buildManifest.js" defer=""></script><script src="/_next/static/ODkvowHBq7dIAIxGbudlb/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 px-2 pt-4 rounded-t-2xl overflow-hidden pb-8"><button type="button" class="inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg><span class="sr-only">Upload image</span></button><textarea rows="2" class="block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"ODkvowHBq7dIAIxGbudlb","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="preload" href="/_next/static/media/4ab03c045edad786-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/c5fea7478aa47814-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/d77e36fa1e563bf0-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/7da2a3ff16027414-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/4cf1eda6528c4545-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f1520da2fce335b3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/6cb9e821df97febd-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/fc3bb0c43ad3be3b-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/efe191cf7953ff64-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f6441c9c7c6cedc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/f5ea4559b0835633-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/media/996798fe8aee0dc3-s.p.woff2" as="font" type="font/woff2" crossorigin="anonymous" data-next-font="size-adjust"/><link rel="preload" href="/_next/static/css/a4a6346dff75e1d3.css" as="style"/><link rel="stylesheet" href="/_next/static/css/a4a6346dff75e1d3.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-8fa1640cc84ba8fe.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-7c8966651ff4862e.js" defer=""></script><script src="/_next/static/chunks/pages/_app-276158b358146aa7.js" defer=""></script><script src="/_next/static/chunks/pages/index-62fdb7c7217c2fea.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js" defer=""></script><script src="/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js" defer=""></script></head><body><div id="__next"><div class="__className_57cb44"><div class="relative w-full h-full"><div class="bg-gray-200 shadow-md fixed w-[400px] h-full top-0"><div class="py-4 px-4"><div align="center" class="mb-4"><img alt="PAutoBot" class="w-12 h-auto mx-auto mb-2" src="/pautobot.png"/><h1 align="center" class="text-3xl font-semibold">🔥 PⒶutoBot 🔥</h1><p align="center">Your private task assistant with GPT</p></div><div class="border-b border-gray-200 dark:border-gray-700 mb-6"><ul class="flex flex-wrap text-sm font-md text-center text-gray-500 dark:text-gray-400"><li class="mr-2"><div class="inline-flex p-4 text-blue-600 border-b-2 border-blue-600 rounded-t-lg active dark:text-blue-500 dark:border-blue-500 group"><svg class="w-5 h-5 mr-2 text-blue-600 group-hover:text-blue-500 dark:text-blue-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path fill-rule="evenodd" d="M4.848 2.771A49.144 49.144 0 0112 2.25c2.43 0 4.817.178 7.152.52 1.978.292 3.348 2.024 3.348 3.97v6.02c0 1.946-1.37 3.678-3.348 3.97a48.901 48.901 0 01-3.476.383.39.39 0 00-.297.17l-2.755 4.133a.75.75 0 01-1.248 0l-2.755-4.133a.39.39 0 00-.297-.17 48.9 48.9 0 01-3.476-.384c-1.978-.29-3.348-2.024-3.348-3.97V6.741c0-1.946 1.37-3.68 3.348-3.97zM6.75 8.25a.75.75 0 01.75-.75h9a.75.75 0 010 1.5h-9a.75.75 0 01-.75-.75zm.75 2.25a.75.75 0 000 1.5H12a.75.75 0 000-1.5H7.5z" clip-rule="evenodd"></path></svg>Query</div></li><li class="mr-2"><div class="inline-flex p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300 dark:hover:text-gray-300 group"><svg aria-hidden="true" class="w-5 h-5 mr-2 text-gray-400 group-hover:text-gray-500 dark:text-gray-500 dark:group-hover:text-gray-300" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M5 3a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2V5a2 2 0 00-2-2H5zM5 11a2 2 0 00-2 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 00-2-2H5zM11 5a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V5zM11 13a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path></svg>Manage Knowledge DB</div></li></ul></div><div class="flex"><select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" disabled=""><option value="GPT4All" selected="">GPT4All</option><option value="LlamaCpp">LlamaCpp</option></select></div><div class="pt-6"><div class="flex items-center justify-center w-full"><label for="dropzone-file" class="flex flex-col items-center justify-center w-full h-64 border-2 border-gray-300 border-dashed rounded-lg cursor-pointer bg-gray-50 dark:hover:bg-bray-800 dark:bg-gray-700 hover:bg-gray-100 dark:border-gray-600 dark:hover:border-gray-500 dark:hover:bg-gray-600 p-3"><div class="flex flex-col items-center justify-center pt-5 pb-6"><svg aria-hidden="true" class="w-10 h-10 mb-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path></svg><p class="mb-2 text-sm text-gray-500 dark:text-gray-400"><span class="font-semibold">Click to upload</span> or drag and drop</p><p class="text-xs text-gray-500 dark:text-gray-400">CSV, DOCX, DOC, ENEX, EML, EPUB, HTML, MD, MSG, ODT, PDF, PPTX, PPT, TXT, images, zip, and more</p></div><input id="dropzone-file" type="file" class="hidden"/></label></div></div><div class="mt-3"><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Upload File</button><button class="w-full text-white bg-gray-800 hover:bg-gray-900 focus:outline-none focus:ring-4 focus:ring-gray-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-gray-800 dark:hover:bg-gray-700 dark:focus:ring-gray-700 dark:border-gray-700">Clear History</button></div></div></div><div class="h-full fixed left-[400px] right-0 top-0 bottom-0 overflow-auto"><div class="flex flex-col w-full"><div class="mx-2 md:px-5 sm:py-4 flex-grow mb-[150px]"><div class="text-black"><div class="text-center pt-20"><h1 class="text-4xl mb-4">Hello World!</h1><h3 class="text-2xl text-gray-500 max-w-[600px] mx-auto">We are in the mission of building an all-in-one task assistant with PrivateGPT!</h3></div><div></div></div></div><div class="fixed left-[400px] right-0 bottom-0"><form class="w-full px-2"><label for="chat" class="sr-only">Your message</label><div class="flex items-center bg-gray-300 px-2 pt-4 rounded-t-2xl overflow-hidden pb-8"><button type="button" class="inline-flex justify-center p-2 text-gray-500 rounded-lg cursor-pointer hover:text-gray-900 hover:bg-gray-100 dark:text-gray-400 dark:hover:text-white dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zm12 12H4l4-8 3 6 2-4 3 6z" clip-rule="evenodd"></path></svg><span class="sr-only">Upload image</span></button><textarea rows="2" class="block mx-4 p-2.5 w-full text-lg text-gray-900 bg-gray-50 rounded-2xl border border-gray-300 focus:ring-gray-500 focus:border-gray-500 dark:bg-gray-800 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-gray-500 dark:focus:border-gray-500" placeholder="What are you thinking about?..."></textarea><button type="submit" class="inline-flex justify-center p-2 text-gray-600 rounded-full cursor-pointer hover:bg-blue-100 dark:text-gray-500 dark:hover:bg-gray-600"><svg aria-hidden="true" class="w-8 h-8 rotate-90" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10.894 2.553a1 1 0 00-1.788 0l-7 14a1 1 0 001.169 1.409l5-1.429A1 1 0 009 15.571V11a1 1 0 112 0v4.571a1 1 0 00.725.962l5 1.428a1 1 0 001.17-1.408l-7-14z"></path></svg><span class="sr-only">Send message</span></button></div></form></div></div><div class="Toastify"></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"Dl9fVCNsnbVyvPy7nTli-","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/loading.svg` & `pautobot-0.0.5/pautobot/frontend-dist/loading.svg`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/frontend-dist/pautobot.png` & `pautobot-0.0.5/pautobot/frontend-dist/pautobot.png`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot/ingest.py` & `pautobot-0.0.5/pautobot/ingest.py`

 * *Files identical despite different names*

### Comparing `pautobot-0.0.4/pautobot.egg-info/PKG-INFO` & `pautobot-0.0.5/pautobot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pautobot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Private AutoGPT Robot - Your private task assistant with GPT!
 Home-page: https://github.com/vietanhdev/pautobot
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: Apache License 2.0
 Keywords: Personal Assistant,Automation,GPT,LLM,PrivateGPT
 Classifier: Natural Language :: English
@@ -67,43 +67,7 @@
 - Run the app:
 
 ```shell
 python -m pautobot.app
 ```
 
 Go to <http://localhost:5678/> to see the app.
-
-## II. Development
-
-### 1. Backend
-
-- Python 3.10 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-backend
-pip install -r requirements.txt
-```
-
-- Run the backend:
-
-```shell
-uvicorn main:app --reload --port 5678
-```
-
-### 2. Frontend
-
-- Node.js 16.0.0 or higher.
-- Install dependencies:
-
-```shell
-cd pauto-frontend
-npm install
-```
-
-- Run the frontend:
-
-```shell
-npm run dev
-```
-
-Go to <http://localhost:3000/> to see the app.
```

### Comparing `pautobot-0.0.4/pautobot.egg-info/SOURCES.txt` & `pautobot-0.0.5/pautobot.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 pyproject.toml
 setup.py
 pautobot/__init__.py
 pautobot/app.py
 pautobot/app_info.py
 pautobot/constants.py
 pautobot/engine.py
+pautobot/example.env
 pautobot/ingest.py
 pautobot/models.py
 pautobot/utils.py
 pautobot.egg-info/PKG-INFO
 pautobot.egg-info/SOURCES.txt
 pautobot.egg-info/dependency_links.txt
 pautobot.egg-info/entry_points.txt
 pautobot.egg-info/requires.txt
 pautobot.egg-info/top_level.txt
 pautobot/frontend-dist/404.html
 pautobot/frontend-dist/favicon.ico
 pautobot/frontend-dist/index.html
 pautobot/frontend-dist/loading.svg
 pautobot/frontend-dist/pautobot.png
-pautobot/frontend-dist/_next/static/ODkvowHBq7dIAIxGbudlb/_buildManifest.js
-pautobot/frontend-dist/_next/static/ODkvowHBq7dIAIxGbudlb/_ssgManifest.js
+pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_buildManifest.js
+pautobot/frontend-dist/_next/static/Dl9fVCNsnbVyvPy7nTli-/_ssgManifest.js
 pautobot/frontend-dist/_next/static/chunks/framework-2c79e2a64abdb08b.js
 pautobot/frontend-dist/_next/static/chunks/main-7c8966651ff4862e.js
 pautobot/frontend-dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 pautobot/frontend-dist/_next/static/chunks/webpack-8fa1640cc84ba8fe.js
 pautobot/frontend-dist/_next/static/chunks/pages/_app-276158b358146aa7.js
 pautobot/frontend-dist/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 pautobot/frontend-dist/_next/static/chunks/pages/index-62fdb7c7217c2fea.js
```

### Comparing `pautobot-0.0.4/setup.py` & `pautobot-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "unstructured>=0.6.6",
         "extract-msg>=0.41.1",
         "tabulate>=0.9.0",
         "pandoc>=2.3",
         "pypandoc>=1.11",
         "tqdm>=4.65.0",
         "fastapi",
+        "requests",
     ]
 
     return install_requires
 
 
 def get_long_description():
     """Read long description from README"""
```

