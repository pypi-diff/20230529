# Comparing `tmp/twscrape-0.2.0.tar.gz` & `tmp/twscrape-0.2.1.tar.gz`

## Comparing `twscrape-0.2.0.tar` & `twscrape-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.0/.gitattributes
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 twscrape-0.2.0/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_api.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_parser.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_pool.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_queue_client.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/__init__.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/account.py
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/accounts_pool.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/api.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/cli.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/constants.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/db.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/logger.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/login.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/models.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/queue_client.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.0/LICENSE
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.0/readme.md
--rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 twscrape-0.2.1/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_api.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_parser.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_pool.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.1/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/__init__.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/account.py
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/api.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/cli.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/constants.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/login.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/models.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.1/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.1/readme.md
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.1/PKG-INFO
```

### Comparing `twscrape-0.2.0/.github/workflows/publish.yml` & `twscrape-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/conftest.py` & `twscrape-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/test_api.py` & `twscrape-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/test_parser.py` & `twscrape-0.2.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/test_pool.py` & `twscrape-0.2.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/test_queue_client.py` & `twscrape-0.2.1/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/favoriters_raw.json` & `twscrape-0.2.1/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/followers_raw.json` & `twscrape-0.2.1/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/following_raw.json` & `twscrape-0.2.1/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/retweeters_raw.json` & `twscrape-0.2.1/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/search_raw.json` & `twscrape-0.2.1/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.2.1/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.2.1/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.2.1/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.2.1/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.2.1/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/account.py` & `twscrape-0.2.1/twscrape/account.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/accounts_pool.py` & `twscrape-0.2.1/twscrape/accounts_pool.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/api.py` & `twscrape-0.2.1/twscrape/api.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/cli.py` & `twscrape-0.2.1/twscrape/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import io
+import sqlite3
 from importlib.metadata import version
 
 from .api import API, AccountsPool
+from .db import get_sqlite_version
 from .logger import logger, set_log_level
 from .utils import print_table
 
 
 class CustomHelpFormatter(argparse.HelpFormatter):
     def __init__(self, prog):
         super().__init__(prog, max_help_position=30, width=120)
@@ -26,15 +28,17 @@
 
 
 async def main(args):
     if args.debug:
         set_log_level("DEBUG")
 
     if args.command == "version":
-        print(version("twscrape"))
+        print(f"twscrape: {version('twscrape')}")
+        print(f"SQlite client: {sqlite3.version}")
+        print(f"SQlite runtime: {sqlite3.sqlite_version} ({await get_sqlite_version()})")
         return
 
     logger.debug(f"Using database: {args.db}")
     pool = AccountsPool(args.db)
     api = API(pool, debug=args.debug)
 
     if args.command == "accounts":
@@ -104,16 +108,16 @@
 
     def clim(name: str, msg: str, a_name: str, a_msg: str, a_type: type = str):
         p = cone(name, msg, a_name, a_msg, a_type)
         p.add_argument("--limit", type=int, default=-1, help="Max tweets to retrieve")
         return p
 
     subparsers.add_parser("version", help="Show version")
-    subparsers.add_parser("accounts", help="List all accounts")
 
+    subparsers.add_parser("accounts", help="List all accounts")
     add_accounts = subparsers.add_parser("add_accounts", help="Add accounts")
     add_accounts.add_argument("file_path", help="File with accounts")
     add_accounts.add_argument("line_format", help="args of Pool.add_account splited by same delim")
     subparsers.add_parser("login_accounts", help="Login accounts")
 
     clim("search", "Search for tweets", "query", "Search query")
     cone("tweet_details", "Get tweet details", "tweet_id", "Tweet ID", int)
```

### Comparing `twscrape-0.2.0/twscrape/constants.py` & `twscrape-0.2.1/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/db.py` & `twscrape-0.2.1/twscrape/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,23 +23,28 @@
                     await asyncio.sleep(delay)
 
         return wrapper
 
     return decorator
 
 
-async def check_version(db: aiosqlite.Connection):
-    async with db.execute("SELECT SQLITE_VERSION()") as cur:
-        rs = await cur.fetchone()
-        rs = rs[0] if rs else "3.0.0"
-        rs = ".".join(rs.split(".")[:2])
+async def get_sqlite_version():
+    async with aiosqlite.connect(":memory:") as db:
+        async with db.execute("SELECT SQLITE_VERSION()") as cur:
+            rs = await cur.fetchone()
+            return rs[0] if rs else "3.0.0"
+
 
-        if rs < MIN_SQLITE_VERSION:
-            msg = f"SQLite version '{rs}' is too old, please upgrade to {MIN_SQLITE_VERSION}+"
-            raise SystemError(msg)
+async def check_version():
+    ver = await get_sqlite_version()
+    ver = ".".join(ver.split(".")[:2])
+
+    if ver < MIN_SQLITE_VERSION:
+        msg = f"SQLite version '{ver}' is too old, please upgrade to {MIN_SQLITE_VERSION}+"
+        raise SystemError(msg)
 
 
 async def migrate(db: aiosqlite.Connection):
     async with db.execute("PRAGMA user_version") as cur:
         rs = await cur.fetchone()
         uv = rs[0] if rs else 0
 
@@ -88,17 +93,17 @@
     _init_once: defaultdict[str, bool] = defaultdict(bool)
 
     def __init__(self, db_path):
         self.db_path = db_path
         self.conn = None
 
     async def __aenter__(self):
+        await check_version()
         db = await aiosqlite.connect(self.db_path)
         db.row_factory = aiosqlite.Row
-        await check_version(db)
 
         if not self._init_once[self.db_path]:
             await migrate(db)
             self._init_once[self.db_path] = True
 
         self.conn = db
         return db
```

### Comparing `twscrape-0.2.0/twscrape/imap.py` & `twscrape-0.2.1/twscrape/imap.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/login.py` & `twscrape-0.2.1/twscrape/login.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/models.py` & `twscrape-0.2.1/twscrape/models.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/queue_client.py` & `twscrape-0.2.1/twscrape/queue_client.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/twscrape/utils.py` & `twscrape-0.2.1/twscrape/utils.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/.gitignore` & `twscrape-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/LICENSE` & `twscrape-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/pyproject.toml` & `twscrape-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
```

### Comparing `twscrape-0.2.0/readme.md` & `twscrape-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `twscrape-0.2.0/PKG-INFO` & `twscrape-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twscrape
-Version: 0.2.0
+Version: 0.2.1
 Summary: Twitter GraphQL and Search API implementation with SNScrape data models
 Project-URL: repository, https://github.com/vladkens/twscrape
 Author-email: vladkens <v.pronsky@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: api,scrape,scrapper,snscrape,twitter
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twscrape Version: 0.2.0 Summary: Twitter GraphQL
+Metadata-Version: 2.1 Name: twscrape Version: 0.2.1 Summary: Twitter GraphQL
 and Search API implementation with SNScrape data models Project-URL:
 repository, https://github.com/vladkens/twscrape Author-email: vladkens
 pronsky@gmail.com> License: MIT License-File: LICENSE Keywords:
 api,scrape,scrapper,snscrape,twitter Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Requires-Dist: aiosqlite==0.17.0 Requires-Dist: fake-
```

