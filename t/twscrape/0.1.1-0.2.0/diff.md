# Comparing `tmp/twscrape-0.1.1.tar.gz` & `tmp/twscrape-0.2.0.tar.gz`

## Comparing `twscrape-0.1.1.tar` & `twscrape-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.1.1/.gitattributes
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 twscrape-0.1.1/Makefile
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 twscrape-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/test_parser.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/test_pool.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/favoriters_raw.json
--rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/followers_raw.json
--rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/following_raw.json
--rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/retweeters_raw.json
--rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/search_raw.json
--rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/tweet_details_raw.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_by_id_raw.json
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_by_login_raw.json
--rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_tweets_and_replies_raw.json
--rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.1.1/tests/mocked-data/user_tweets_raw.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/account.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/accounts_pool.py
--rw-r--r--   0        0        0    12984 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/api.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/constants.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/db.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/imap.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/logger.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/login.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/models.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 twscrape-0.1.1/twscrape/utils.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.1.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.1.1/LICENSE
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 twscrape-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 twscrape-0.1.1/readme.md
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 twscrape-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 twscrape-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 twscrape-0.2.0/Makefile
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 twscrape-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 twscrape-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_api.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_parser.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_pool.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/test_queue_client.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/favoriters_raw.json
+-rw-r--r--   0        0        0   152580 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/followers_raw.json
+-rw-r--r--   0        0        0   142243 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/following_raw.json
+-rw-r--r--   0        0        0    69669 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/retweeters_raw.json
+-rw-r--r--   0        0        0   177570 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/search_raw.json
+-rw-r--r--   0        0        0    95327 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/tweet_details_raw.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_by_id_raw.json
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_by_login_raw.json
+-rw-r--r--   0        0        0   497799 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_tweets_and_replies_raw.json
+-rw-r--r--   0        0        0   496101 2020-02-02 00:00:00.000000 twscrape-0.2.0/tests/mocked-data/user_tweets_raw.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/__init__.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/account.py
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/accounts_pool.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/api.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/cli.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/constants.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/db.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/imap.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/logger.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/login.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/models.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/queue_client.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 twscrape-0.2.0/twscrape/utils.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 twscrape-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 twscrape-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 twscrape-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 twscrape-0.2.0/readme.md
+-rw-r--r--   0        0        0     7868 2020-02-02 00:00:00.000000 twscrape-0.2.0/PKG-INFO
```

### Comparing `twscrape-0.1.1/tests/test_parser.py` & `twscrape-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/test_pool.py` & `twscrape-0.2.0/tests/test_pool.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,137 @@
-import os
-
 from twscrape.accounts_pool import AccountsPool
-from twscrape.db import DB
 from twscrape.utils import utc_ts
 
-DB_FILE = "/tmp/twscrape_test.db"
-
-
-def remove_db():
-    DB._init_once[DB_FILE] = False
-    if os.path.exists(DB_FILE):
-        os.remove(DB_FILE)
-
-
-async def test_add_accounts():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
 
+async def test_add_accounts(pool_mock: AccountsPool):
     # should add account
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    acc = await pool.get("user1")
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    acc = await pool_mock.get("user1")
     assert acc.username == "user1"
     assert acc.password == "pass1"
     assert acc.email == "email1"
     assert acc.email_password == "email_pass1"
 
     # should not add account with same username
-    await pool.add_account("user1", "pass2", "email2", "email_pass2")
-    acc = await pool.get("user1")
+    await pool_mock.add_account("user1", "pass2", "email2", "email_pass2")
+    acc = await pool_mock.get("user1")
     assert acc.username == "user1"
     assert acc.password == "pass1"
     assert acc.email == "email1"
     assert acc.email_password == "email_pass1"
 
     # should not add account with different username case
-    await pool.add_account("USER1", "pass2", "email2", "email_pass2")
-    acc = await pool.get("user1")
+    await pool_mock.add_account("USER1", "pass2", "email2", "email_pass2")
+    acc = await pool_mock.get("user1")
     assert acc.username == "user1"
     assert acc.password == "pass1"
     assert acc.email == "email1"
     assert acc.email_password == "email_pass1"
 
     # should add account with different username
-    await pool.add_account("user2", "pass2", "email2", "email_pass2")
-    acc = await pool.get("user2")
+    await pool_mock.add_account("user2", "pass2", "email2", "email_pass2")
+    acc = await pool_mock.get("user2")
     assert acc.username == "user2"
     assert acc.password == "pass2"
     assert acc.email == "email2"
     assert acc.email_password == "email_pass2"
 
 
-async def test_get_all():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
-
+async def test_get_all(pool_mock: AccountsPool):
     # should return empty list
-    accs = await pool.get_all()
+    accs = await pool_mock.get_all()
     assert len(accs) == 0
 
     # should return all accounts
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    await pool.add_account("user2", "pass2", "email2", "email_pass2")
-    accs = await pool.get_all()
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    await pool_mock.add_account("user2", "pass2", "email2", "email_pass2")
+    accs = await pool_mock.get_all()
     assert len(accs) == 2
     assert accs[0].username == "user1"
     assert accs[1].username == "user2"
 
 
-async def test_save():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
-
+async def test_save(pool_mock: AccountsPool):
     # should save account
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    acc = await pool.get("user1")
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    acc = await pool_mock.get("user1")
     acc.password = "pass2"
-    await pool.save(acc)
-    acc = await pool.get("user1")
+    await pool_mock.save(acc)
+    acc = await pool_mock.get("user1")
     assert acc.password == "pass2"
 
     # should not save account
-    acc = await pool.get("user1")
+    acc = await pool_mock.get("user1")
     acc.username = "user2"
-    await pool.save(acc)
-    acc = await pool.get("user1")
+    await pool_mock.save(acc)
+    acc = await pool_mock.get("user1")
     assert acc.username == "user1"
 
 
-async def test_get_for_queue():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
+async def test_get_for_queue(pool_mock: AccountsPool):
     Q = "test_queue"
 
     # should return account
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    await pool.set_active("user1", True)
-    acc = await pool.get_for_queue(Q)
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    await pool_mock.set_active("user1", True)
+    acc = await pool_mock.get_for_queue(Q)
     assert acc is not None
     assert acc.username == "user1"
     assert acc.active is True
     assert acc.locks is not None
     assert Q in acc.locks
     assert acc.locks[Q] is not None
 
     # should return None
-    acc = await pool.get_for_queue(Q)
+    acc = await pool_mock.get_for_queue(Q)
     assert acc is None
 
 
-async def test_account_unlock():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
+async def test_account_unlock(pool_mock: AccountsPool):
     Q = "test_queue"
 
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    await pool.set_active("user1", True)
-    acc = await pool.get_for_queue(Q)
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    await pool_mock.set_active("user1", True)
+    acc = await pool_mock.get_for_queue(Q)
     assert acc is not None
     assert acc.locks[Q] is not None
 
     # should unlock account and make available for queue
-    await pool.unlock(acc.username, Q)
-    acc = await pool.get_for_queue(Q)
+    await pool_mock.unlock(acc.username, Q)
+    acc = await pool_mock.get_for_queue(Q)
     assert acc is not None
     assert acc.locks[Q] is not None
 
     # should update lock time
     end_time = utc_ts() + 60  # + 1 minute
-    await pool.lock_until(acc.username, Q, end_time)
+    await pool_mock.lock_until(acc.username, Q, end_time)
 
-    acc = await pool.get(acc.username)
+    acc = await pool_mock.get(acc.username)
     assert int(acc.locks[Q].timestamp()) == end_time
 
 
-async def test_get_stats():
-    remove_db()
-    pool = AccountsPool(DB_FILE)
+async def test_get_stats(pool_mock: AccountsPool):
     Q = "search"
 
     # should return empty stats
-    stats = await pool.stats()
+    stats = await pool_mock.stats()
     for k, v in stats.items():
         assert v == 0, f"{k} should be 0"
 
     # should increate total
-    await pool.add_account("user1", "pass1", "email1", "email_pass1")
-    stats = await pool.stats()
+    await pool_mock.add_account("user1", "pass1", "email1", "email_pass1")
+    stats = await pool_mock.stats()
     assert stats["total"] == 1
     assert stats["active"] == 0
 
     # should increate active
-    await pool.set_active("user1", True)
-    stats = await pool.stats()
+    await pool_mock.set_active("user1", True)
+    stats = await pool_mock.stats()
     assert stats["total"] == 1
     assert stats["active"] == 1
 
     # should update queue stats
-    await pool.get_for_queue(Q)
-    stats = await pool.stats()
+    await pool_mock.get_for_queue(Q)
+    stats = await pool_mock.stats()
     assert stats["total"] == 1
     assert stats["active"] == 1
     assert stats["locked_search"] == 1
```

### Comparing `twscrape-0.1.1/tests/mocked-data/favoriters_raw.json` & `twscrape-0.2.0/tests/mocked-data/favoriters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/followers_raw.json` & `twscrape-0.2.0/tests/mocked-data/followers_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/following_raw.json` & `twscrape-0.2.0/tests/mocked-data/following_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/retweeters_raw.json` & `twscrape-0.2.0/tests/mocked-data/retweeters_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/search_raw.json` & `twscrape-0.2.0/tests/mocked-data/search_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/tweet_details_raw.json` & `twscrape-0.2.0/tests/mocked-data/tweet_details_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/user_by_id_raw.json` & `twscrape-0.2.0/tests/mocked-data/user_by_id_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/user_by_login_raw.json` & `twscrape-0.2.0/tests/mocked-data/user_by_login_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/user_tweets_and_replies_raw.json` & `twscrape-0.2.0/tests/mocked-data/user_tweets_and_replies_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/tests/mocked-data/user_tweets_raw.json` & `twscrape-0.2.0/tests/mocked-data/user_tweets_raw.json`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/twscrape/account.py` & `twscrape-0.2.0/twscrape/account.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,53 @@
 import json
 import sqlite3
-from dataclasses import asdict, dataclass
+from dataclasses import asdict, dataclass, field
 from datetime import datetime
 
 from httpx import AsyncClient, AsyncHTTPTransport
 
 from .constants import TOKEN
+from .models import JSONTrait
 from .utils import from_utciso
 
 
 @dataclass
-class Account:
+class Account(JSONTrait):
     username: str
     password: str
     email: str
     email_password: str
     user_agent: str
     active: bool
-    locks: dict[str, datetime]
-    headers: dict[str, str] | None = None
-    cookies: dict[str, str] | None = None
+    locks: dict[str, datetime] = field(default_factory=dict)  # queue: datetime
+    stats: dict[str, int] = field(default_factory=dict)  # queue: requests
+    headers: dict[str, str] = field(default_factory=dict)
+    cookies: dict[str, str] = field(default_factory=dict)
     proxy: str | None = None
     error_msg: str | None = None
-
-    @staticmethod
-    def create_sql():
-        return """
-        CREATE TABLE IF NOT EXISTS accounts (
-            username TEXT PRIMARY KEY NOT NULL COLLATE NOCASE,
-            password TEXT NOT NULL,
-            email TEXT NOT NULL COLLATE NOCASE,
-            email_password TEXT NOT NULL,
-            user_agent TEXT NOT NULL,
-            active BOOLEAN DEFAULT FALSE NOT NULL,
-            locks TEXT DEFAULT '{}' NOT NULL,
-            headers TEXT DEFAULT '{}' NOT NULL,
-            cookies TEXT DEFAULT '{}' NOT NULL,
-            proxy TEXT DEFAULT NULL,
-            error_msg TEXT DEFAULT NULL
-        );
-        """
+    last_used: datetime | None = None
 
     @staticmethod
     def from_rs(rs: sqlite3.Row):
         doc = dict(rs)
         doc["locks"] = {k: from_utciso(v) for k, v in json.loads(doc["locks"]).items()}
+        doc["stats"] = {k: v for k, v in json.loads(doc["stats"]).items() if isinstance(v, int)}
         doc["headers"] = json.loads(doc["headers"])
         doc["cookies"] = json.loads(doc["cookies"])
         doc["active"] = bool(doc["active"])
+        doc["last_used"] = from_utciso(doc["last_used"]) if doc["last_used"] else None
         return Account(**doc)
 
     def to_rs(self):
         rs = asdict(self)
         rs["locks"] = json.dumps(rs["locks"], default=lambda x: x.isoformat())
+        rs["stats"] = json.dumps(rs["stats"])
         rs["headers"] = json.dumps(rs["headers"])
         rs["cookies"] = json.dumps(rs["cookies"])
+        rs["last_used"] = rs["last_used"].isoformat() if rs["last_used"] else None
         return rs
 
     def make_client(self) -> AsyncClient:
         transport = AsyncHTTPTransport(retries=2)
         client = AsyncClient(proxies=self.proxy, follow_redirects=True, transport=transport)
 
         # saved from previous usage
```

### Comparing `twscrape-0.1.1/twscrape/constants.py` & `twscrape-0.2.0/twscrape/constants.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/twscrape/imap.py` & `twscrape-0.2.0/twscrape/imap.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,43 @@
 from datetime import datetime
 
 from .logger import logger
 
 MAX_WAIT_SEC = 30
 
 
+class EmailLoginError(Exception):
+    def __init__(self, message="Email login error"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class EmailCodeTimeoutError(Exception):
+    def __init__(self, message="Email code timeout"):
+        self.message = message
+        super().__init__(self.message)
+
+
+IMAP_MAPPING: dict[str, str] = {
+    "yahoo.com": "imap.mail.yahoo.com",
+    "icloud.com": "imap.mail.me.com",
+    "outlook.com": "imap-mail.outlook.com",
+    "hotmail.com": "imap-mail.outlook.com",
+}
+
+
+def add_imap_mapping(email_domain: str, imap_domain: str):
+    IMAP_MAPPING[email_domain] = imap_domain
+
+
 def get_imap_domain(email: str) -> str:
-    return f"imap.{email.split('@')[1]}"
+    email_domain = email.split("@")[1]
+    if email_domain in IMAP_MAPPING:
+        return IMAP_MAPPING[email_domain]
+    return f"imap.{email_domain}"
 
 
 def search_email_code(imap: imaplib.IMAP4_SSL, count: int, min_t: datetime | None) -> str | None:
     for i in range(count, 0, -1):
         _, rep = imap.fetch(str(i), "(RFC822)")
         for x in rep:
             if isinstance(x, tuple):
@@ -35,22 +62,27 @@
     return None
 
 
 async def get_email_code(email: str, password: str, min_t: datetime | None = None) -> str:
     domain = get_imap_domain(email)
     start_time = time.time()
     with imaplib.IMAP4_SSL(domain) as imap:
-        imap.login(email, password)
+        try:
+            imap.login(email, password)
+        except imaplib.IMAP4.error as e:
+            logger.error(f"Error logging into {email}: {e}")
+            raise EmailLoginError() from e
 
         was_count = 0
         while True:
             _, rep = imap.select("INBOX")
             now_count = int(rep[0].decode("utf-8")) if len(rep) > 0 and rep[0] is not None else 0
             if now_count > was_count:
                 code = search_email_code(imap, now_count, min_t)
                 if code is not None:
                     return code
 
             logger.debug(f"Waiting for confirmation code for {email}, msg_count: {now_count}")
             if MAX_WAIT_SEC < time.time() - start_time:
-                raise Exception(f"Timeout on getting confirmation code for {email}")
+                logger.error(f"Timeout waiting for confirmation code for {email}")
+                raise EmailCodeTimeoutError()
             await asyncio.sleep(5)
```

### Comparing `twscrape-0.1.1/twscrape/login.py` & `twscrape-0.2.0/twscrape/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             if task_id == "LoginEnterPassword":
                 return await login_enter_password(client, acc, prev)
             if task_id == "LoginEnterUserIdentifierSSO":
                 return await login_enter_username(client, acc, prev)
             if task_id == "LoginJsInstrumentationSubtask":
                 return await login_instrumentation(client, acc, prev)
         except Exception as e:
-            acc.error_msg = f"task={task_id} err={e}"
+            acc.error_msg = f"login_step={task_id} err={e}"
             logger.error(f"Error in {task_id}: {e}")
             raise e
 
     return None
 
 
 async def login(acc: Account, fresh=False) -> Account:
```

### Comparing `twscrape-0.1.1/twscrape/models.py` & `twscrape-0.2.0/twscrape/models.py`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/twscrape/utils.py` & `twscrape-0.2.0/twscrape/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -138,7 +138,35 @@
 
 def utc_ts() -> int:
     return int(datetime.utcnow().replace(tzinfo=timezone.utc).timestamp())
 
 
 def from_utciso(iso: str) -> datetime:
     return datetime.fromisoformat(iso).replace(tzinfo=timezone.utc)
+
+
+def print_table(rows: list[dict]):
+    if not rows:
+        return
+
+    def prt(x):
+        if isinstance(x, str):
+            return x
+
+        if isinstance(x, int):
+            return f"{x:,}"
+
+        return str(x)
+
+    keys = list(rows[0].keys())
+    rows = [{k: k for k in keys}, *[{k: prt(x.get(k, "")) for k in keys} for x in rows]]
+    colw = [max(len(x[k]) for x in rows) + 1 for k in keys]
+
+    lines = []
+    for row in rows:
+        line = [f"{row[k]:<{colw[i]}}" for i, k in enumerate(keys)]
+        lines.append(" ".join(line))
+
+    max_len = max(len(x) for x in lines)
+    lines.insert(1, "─" * max_len)
+    lines.insert(0, "─" * max_len)
+    print("\n".join(lines))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twscrape-0.1.1/.gitignore` & `twscrape-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/LICENSE` & `twscrape-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twscrape-0.1.1/pyproject.toml` & `twscrape-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "twscrape"
-version = "0.1.1"
+version = "0.2.0"
 authors = [{name = "vladkens", email = "v.pronsky@gmail.com"}]
 description = "Twitter GraphQL and Search API implementation with SNScrape data models"
 readme = "readme.md"
 requires-python = ">=3.10"
 keywords = ["twitter", "scrape", "scrapper", "api", "snscrape"]
 license = {text = "MIT"}
 classifiers = [
@@ -25,21 +25,25 @@
 ]
 
 [project.optional-dependencies]
 dev = [
   "pylint==2.17.3",
   "pytest-asyncio==0.21.0",
   "pytest-cov==4.0.0",
+  "pytest-httpx==0.22.0",
   "pytest==7.3.1",
   "ruff==0.0.263",
 ]
 
 [project.urls]
 repository = "https://github.com/vladkens/twscrape"
 
+[project.scripts]
+twscrape = "twscrape.cli:run"
+
 [tool.setuptools]
 packages = ['twscrape']
 
 [tool.pylint]
 max-line-length = 99
 disable = [
     "C0103", # invalid-name
```

