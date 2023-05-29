# Comparing `tmp/neatpush-0.2.0.tar.gz` & `tmp/neatpush-0.3.1.tar.gz`

## Comparing `neatpush-0.2.0.tar` & `neatpush-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 neatpush-0.2.0/.cruft.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 neatpush-0.2.0/.dockerignore
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 neatpush-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 neatpush-0.2.0/Dockerfile
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 neatpush-0.2.0/Makefile
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 neatpush-0.2.0/docker-compose.yaml
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 neatpush-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 neatpush-0.2.0/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 neatpush-0.2.0/.vscode/extensions.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 neatpush-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/abbreviations.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/changelog.md
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/index.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/reference.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/css/termynal.css
--rw-r--r--   0        0        0    50761 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/img/favicon.ico
--rw-r--r--   0        0        0    52359 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/img/gp_logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neatpush-0.2.0/docs/js/custom.js
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/__main__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/app.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/config.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/manga.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/notify.py
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 neatpush-0.2.0/neatpush/scraping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neatpush-0.2.0/requirements/.gitkeep
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 neatpush-0.2.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/test_scraping.py
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/data/vcr_cassettes/scrap_jujutsu-kaisen.yaml
--rw-r--r--   0        0        0    81121 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/data/vcr_cassettes/scrap_overgeared.yaml
--rw-r--r--   0        0        0   450537 2020-02-02 00:00:00.000000 neatpush-0.2.0/tests/data/vcr_cassettes/scrap_tales-of-demons-and-gods.yaml
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 neatpush-0.2.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 neatpush-0.2.0/LICENSE
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neatpush-0.2.0/README.md
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 neatpush-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 neatpush-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 neatpush-0.3.1/.cruft.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 neatpush-0.3.1/.dockerignore
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 neatpush-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 neatpush-0.3.1/Dockerfile
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 neatpush-0.3.1/Makefile
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 neatpush-0.3.1/docker-compose.yaml
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 neatpush-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 neatpush-0.3.1/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 neatpush-0.3.1/.vscode/extensions.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 neatpush-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/abbreviations.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/changelog.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/index.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/reference.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/css/termynal.css
+-rw-r--r--   0        0        0    50761 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/img/favicon.ico
+-rw-r--r--   0        0        0    52359 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/img/gp_logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neatpush-0.3.1/docs/js/custom.js
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/__init__.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/__main__.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/app.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/config.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/manga.py
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 neatpush-0.3.1/neatpush/scraping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neatpush-0.3.1/requirements/.gitkeep
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 neatpush-0.3.1/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/test_scraping.py
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/data/vcr_cassettes/scrap_jujutsu-kaisen.yaml
+-rw-r--r--   0        0        0    81121 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/data/vcr_cassettes/scrap_overgeared.yaml
+-rw-r--r--   0        0        0   450537 2020-02-02 00:00:00.000000 neatpush-0.3.1/tests/data/vcr_cassettes/scrap_tales-of-demons-and-gods.yaml
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 neatpush-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 neatpush-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 neatpush-0.3.1/README.md
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 neatpush-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 neatpush-0.3.1/PKG-INFO
```

### Comparing `neatpush-0.2.0/.cruft.json` & `neatpush-0.3.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.pre-commit-config.yaml` & `neatpush-0.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
         entry: make mypy
         types: [python]
         language: system
         pass_filenames: false
 
 
   - repo: https://github.com/jazzband/pip-tools
-    rev: 6.9.0
+    rev: 6.13.0
     hooks:
       - id: pip-compile
         name: pip-compile pyproject.toml
         files: ^pyproject.toml$
         args:
           [
             --no-emit-index-url,
             --extra,
             prod,
             --output-file,
             requirements/requirements-prod.txt,
             pyproject.toml,
-          ]
+          ]
```

### Comparing `neatpush-0.2.0/Makefile` & `neatpush-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/docker-compose.yaml` & `neatpush-0.3.1/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/mkdocs.yml` & `neatpush-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `neatpush-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.github/ISSUE_TEMPLATE/question.md` & `neatpush-0.3.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.github/workflows/ci.yml` & `neatpush-0.3.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   lint:
     name: Lint (pre-commit)
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v4.6.1
         with:
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: pyproject.toml
 
       - uses: actions/cache@v3
         id: cache
```

### Comparing `neatpush-0.2.0/.github/workflows/smokeshow.yml` & `neatpush-0.3.1/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.vscode/extensions.json` & `neatpush-0.3.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.vscode/settings.json` & `neatpush-0.3.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/docs/css/termynal.css` & `neatpush-0.3.1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/docs/img/favicon.ico` & `neatpush-0.3.1/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/docs/img/gp_logo.png` & `neatpush-0.3.1/docs/img/gp_logo.png`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/neatpush/manga.py` & `neatpush-0.3.1/neatpush/manga.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,28 +126,28 @@
                 logger.info(f"First time checking chapters for {name}. Just caching.")
                 continue
 
             manga = map_name_cache[name]
             new_chapters = sorted(
                 set(chapters) - set(manga.chapters), key=lambda x: x.timestamp
             )
+            all_chapters = sorted(
+                set(manga.chapters) | set(chapters),
+                key=lambda x: x.timestamp,
+            )
 
             if not new_chapters:
                 logger.debug(f"Found nothing new chapter for {name}.")
             else:
                 logger.info(
                     f"Found new chapters for {name}: "
                     + ", ".join(chap.num for chap in new_chapters)
                 )
+                to_notify_map[name] = new_chapters
 
-            to_notify_map[name] = new_chapters
             updated_mangas.append(
-                Manga(
-                    name=name,
-                    source=source,
-                    chapters=set(manga.chapters) | set(chapters),
-                )
+                Manga(name=name, source=source, chapters=all_chapters)
             )
 
     save_cached_mangas(s3, mangas=updated_mangas)
 
     return to_notify_map
```

### Comparing `neatpush-0.2.0/neatpush/scraping.py` & `neatpush-0.3.1/neatpush/scraping.py`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/requirements/requirements-prod.txt` & `neatpush-0.3.1/requirements/requirements-prod.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --extra=prod --no-emit-index-url --output-file=requirements/requirements-prod.txt pyproject.toml
 #
 anyio==3.6.2
     # via
     #   httpcore
     #   starlette
+apprise==1.4.0
+    # via neatpush (pyproject.toml)
 boto3==1.26.37
     # via neatpush (pyproject.toml)
 botocore==1.29.37
     # via
     #   boto3
     #   s3transfer
 certifi==2022.12.7
     # via
+    #   apprise
     #   httpcore
     #   httpx
+    #   requests
+charset-normalizer==3.1.0
+    # via requests
 click==8.1.3
     # via
+    #   apprise
     #   typer
     #   uvicorn
 dateparser==1.1.4
     # via neatpush (pyproject.toml)
 gazpacho==1.1
     # via neatpush (pyproject.toml)
 h11==0.14.0
@@ -33,35 +40,48 @@
 httpcore==0.16.3
     # via httpx
 httpx==0.23.1
     # via neatpush (pyproject.toml)
 idna==3.4
     # via
     #   anyio
+    #   requests
     #   rfc3986
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
+markdown==3.4.3
+    # via apprise
+oauthlib==3.2.2
+    # via requests-oauthlib
 orjson==3.8.3
     # via neatpush (pyproject.toml)
 pydantic[dotenv]==1.10.2
     # via neatpush (pyproject.toml)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   dateparser
 python-dotenv==0.21.0
     # via pydantic
 pytz==2022.7
     # via dateparser
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
+pyyaml==6.0
+    # via apprise
 regex==2022.10.31
     # via dateparser
+requests==2.31.0
+    # via
+    #   apprise
+    #   requests-oauthlib
+requests-oauthlib==1.3.1
+    # via apprise
 rfc3986[idna2008]==1.5.0
     # via httpx
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via python-dateutil
 sniffio==1.3.0
@@ -78,10 +98,12 @@
 typing-extensions==4.4.0
     # via pydantic
 tzdata==2022.7
     # via pytz-deprecation-shim
 tzlocal==4.2
     # via dateparser
 urllib3==1.26.13
-    # via botocore
+    # via
+    #   botocore
+    #   requests
 uvicorn==0.20.0
     # via neatpush (pyproject.toml)
```

### Comparing `neatpush-0.2.0/tests/conftest.py` & `neatpush-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/tests/test_scraping.py` & `neatpush-0.3.1/tests/test_scraping.py`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/tests/data/vcr_cassettes/scrap_jujutsu-kaisen.yaml` & `neatpush-0.3.1/tests/data/vcr_cassettes/scrap_jujutsu-kaisen.yaml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/tests/data/vcr_cassettes/scrap_overgeared.yaml` & `neatpush-0.3.1/tests/data/vcr_cassettes/scrap_overgeared.yaml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/tests/data/vcr_cassettes/scrap_tales-of-demons-and-gods.yaml` & `neatpush-0.3.1/tests/data/vcr_cassettes/scrap_tales-of-demons-and-gods.yaml`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/.gitignore` & `neatpush-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/LICENSE` & `neatpush-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/README.md` & `neatpush-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `neatpush-0.2.0/pyproject.toml` & `neatpush-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 dependencies = [
   "typer",
   "structlog",
 
   "pydantic[dotenv]<2.0.0",
   "boto3",
   "orjson",
+  "apprise",
 
   # webserver
   "starlette",
   "uvicorn",
 
   # scraping:
   "httpx",
```

### Comparing `neatpush-0.2.0/PKG-INFO` & `neatpush-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: neatpush
-Version: 0.2.0
+Version: 0.3.1
 Summary: Notify me of new manga chapters.
 Project-URL: Homepage, https://github.com/gjeusel/neatpush
 Project-URL: Source, https://github.com/gjeusel/neatpush
 Author-email: gjeusel <gjeusel@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
+Requires-Dist: apprise
 Requires-Dist: boto3
 Requires-Dist: dateparser
 Requires-Dist: gazpacho
 Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: pydantic[dotenv]<2.0.0
 Requires-Dist: starlette
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: neatpush Version: 0.2.0 Summary: Notify me of new
+Metadata-Version: 2.1 Name: neatpush Version: 0.3.1 Summary: Notify me of new
 manga chapters. Project-URL: Homepage, https://github.com/gjeusel/neatpush
 Project-URL: Source, https://github.com/gjeusel/neatpush Author-email: gjeusel
 gmail.com> License-File: LICENSE Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development Requires-Python: >=3.10 Requires-
-Dist: boto3 Requires-Dist: dateparser Requires-Dist: gazpacho Requires-Dist:
-httpx Requires-Dist: orjson Requires-Dist: pydantic[dotenv]<2.0.0 Requires-
-Dist: starlette Requires-Dist: structlog Requires-Dist: typer Requires-Dist:
-uvicorn Provides-Extra: all Requires-Dist: neatpush[dev]; extra == 'all'
-Requires-Dist: neatpush[doc]; extra == 'all' Provides-Extra: dev Requires-Dist:
-black==22.10.*; extra == 'dev' Requires-Dist: cookiecutter; extra == 'dev'
-Requires-Dist: coverage[toml]<7.0,>=6.5.0; extra == 'dev' Requires-Dist: cruft;
-extra == 'dev' Requires-Dist: mypy==0.991; extra == 'dev' Requires-Dist: pdbpp;
-extra == 'dev' Requires-Dist: pip-tools; extra == 'dev' Requires-Dist: pre-
-commit==2.20.*; extra == 'dev' Requires-Dist: ptpython; extra == 'dev'
-Requires-Dist: pytest-mock==3.10.*; extra == 'dev' Requires-Dist: pytest-
-sugar==0.9.*; extra == 'dev' Requires-Dist: pytest==7.1.*; extra == 'dev'
-Requires-Dist: rich; extra == 'dev' Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: types-dateparser; extra == 'dev' Requires-Dist: types-pytz;
-extra == 'dev' Requires-Dist: vcrpy; extra == 'dev' Provides-Extra: doc
+Dist: apprise Requires-Dist: boto3 Requires-Dist: dateparser Requires-Dist:
+gazpacho Requires-Dist: httpx Requires-Dist: orjson Requires-Dist: pydantic
+[dotenv]<2.0.0 Requires-Dist: starlette Requires-Dist: structlog Requires-Dist:
+typer Requires-Dist: uvicorn Provides-Extra: all Requires-Dist: neatpush[dev];
+extra == 'all' Requires-Dist: neatpush[doc]; extra == 'all' Provides-Extra: dev
+Requires-Dist: black==22.10.*; extra == 'dev' Requires-Dist: cookiecutter;
+extra == 'dev' Requires-Dist: coverage[toml]<7.0,>=6.5.0; extra == 'dev'
+Requires-Dist: cruft; extra == 'dev' Requires-Dist: mypy==0.991; extra == 'dev'
+Requires-Dist: pdbpp; extra == 'dev' Requires-Dist: pip-tools; extra == 'dev'
+Requires-Dist: pre-commit==2.20.*; extra == 'dev' Requires-Dist: ptpython;
+extra == 'dev' Requires-Dist: pytest-mock==3.10.*; extra == 'dev' Requires-
+Dist: pytest-sugar==0.9.*; extra == 'dev' Requires-Dist: pytest==7.1.*; extra
+== 'dev' Requires-Dist: rich; extra == 'dev' Requires-Dist: ruff; extra ==
+'dev' Requires-Dist: types-dateparser; extra == 'dev' Requires-Dist: types-
+pytz; extra == 'dev' Requires-Dist: vcrpy; extra == 'dev' Provides-Extra: doc
 Requires-Dist: markdown-include; extra == 'doc' Requires-Dist: mdx-truly-sane-
 lists; extra == 'doc' Requires-Dist: mkdocs; extra == 'doc' Requires-Dist:
 mkdocs-exclude; extra == 'doc' Requires-Dist: mkdocs-material; extra == 'doc'
 Requires-Dist: mkdocstrings[python]; extra == 'doc' Description-Content-Type:
 text/markdown
                             ****** NeatPush ******
   [Test_Suite] [Coverage] [Package_version] [MKDocs_github_page] [pre-commit]
```

