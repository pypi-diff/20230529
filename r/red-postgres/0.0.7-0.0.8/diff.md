# Comparing `tmp/red-postgres-0.0.7.tar.gz` & `tmp/red-postgres-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red-postgres-0.0.7.tar", last modified: Mon May 29 17:04:22 2023, max compression
+gzip compressed data, was "red-postgres-0.0.8.tar", last modified: Mon May 29 19:20:18 2023, max compression
```

## Comparing `red-postgres-0.0.7.tar` & `red-postgres-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 17:04:22.818798 red-postgres-0.0.7/
--rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2452 2023-05-29 17:04:22.817774 red-postgres-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2023-05-29 16:43:40.000000 red-postgres-0.0.7/README.md
--rw-rw-rw-   0        0        0     1630 2023-05-29 17:04:04.000000 red-postgres-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-29 17:04:22.802775 red-postgres-0.0.7/red_postgres/
--rw-rw-rw-   0        0        0      180 2023-05-29 16:51:21.000000 red-postgres-0.0.7/red_postgres/__init__.py
--rw-rw-rw-   0        0        0     4077 2023-05-29 16:41:50.000000 red-postgres-0.0.7/red_postgres/engine.py
-drwxrwxrwx   0        0        0        0 2023-05-29 17:04:22.816772 red-postgres-0.0.7/red_postgres.egg-info/
--rw-rw-rw-   0        0        0     2452 2023-05-29 17:04:22.000000 red-postgres-0.0.7/red_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-05-29 17:04:22.000000 red-postgres-0.0.7/red_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 17:04:22.000000 red-postgres-0.0.7/red_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 17:04:22.000000 red-postgres-0.0.7/red_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 17:04:22.818798 red-postgres-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.766191 red-postgres-0.0.8/
+-rw-rw-rw-   0        0        0    18431 2023-05-29 15:03:19.000000 red-postgres-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4680 2023-05-29 19:20:18.766191 red-postgres-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4143 2023-05-29 17:36:29.000000 red-postgres-0.0.8/README.md
+-rw-rw-rw-   0        0        0     1630 2023-05-29 19:19:53.000000 red-postgres-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.750188 red-postgres-0.0.8/red_postgres/
+-rw-rw-rw-   0        0        0      180 2023-05-29 17:18:29.000000 red-postgres-0.0.8/red_postgres/__init__.py
+-rw-rw-rw-   0        0        0     4306 2023-05-29 19:20:03.000000 red-postgres-0.0.8/red_postgres/engine.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:20:18.765191 red-postgres-0.0.8/red_postgres.egg-info/
+-rw-rw-rw-   0        0        0     4680 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 19:20:18.000000 red-postgres-0.0.8/red_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:20:18.767197 red-postgres-0.0.8/setup.cfg
```

### Comparing `red-postgres-0.0.7/LICENSE` & `red-postgres-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `red-postgres-0.0.7/pyproject.toml` & `red-postgres-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "discord.py==2.2.3", "piccolo[postgres]==0.113.0"]
+requires = ["setuptools>=61.0", "discord.py>=2.2.3", "piccolo[postgres]>=0.113.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "red-postgres"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Vertyco" },
 ]
 description = "Piccolo Postgres integration for Red"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `red-postgres-0.0.7/red_postgres/engine.py` & `red-postgres-0.0.8/red_postgres/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 import subprocess
 from pathlib import Path
 
 from discord.ext.commands import Cog
 from piccolo.engine.postgres import PostgresEngine
 from piccolo.table import Table, create_db_tables
 
-log = logging.getLogger("red.postgres.engine")
+log = logging.getLogger("red.red-postgres.engine")
 
 
 def acquire_db_engine(config: dict) -> PostgresEngine:
     """This is ran in executor since it blocks if connection info is bad"""
     return PostgresEngine(config=config)
 
 
 async def create_database_and_tables(
-    cog: Cog, config: dict, tables: list[type[Table]]
+    cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
 ) -> PostgresEngine:
     """Connect to postgres, create database/tables and return engine
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
+        max_size (int): maximum number of database connections, 20 by default
 
     Returns:
         PostgresEngine instance
     """
     log.debug("Initializing database")
     engine = await asyncio.to_thread(acquire_db_engine, config)
     await engine.start_connection_pool()
@@ -44,15 +45,15 @@
 
     # Close old database connection
     await engine.close_connection_pool()
 
     # Connect to the new database
     config["database"] = cog_name
     engine = await asyncio.to_thread(acquire_db_engine, config)
-    await engine.start_connection_pool()
+    await engine.start_connection_pool(max_size=max_size)
 
     # Update table engines
     for table_class in tables:
         table_class._meta.db = engine
 
     # Create any tables that don't already exist
     await create_db_tables(*tables, if_not_exists=True)
@@ -106,22 +107,23 @@
 
         return migration_result
 
     return await asyncio.to_thread(run)
 
 
 async def register_cog(
-    cog: Cog, config: dict, tables: list[type[Table]]
+    cog: Cog, config: dict, tables: list[type[Table]], max_size: int = 20
 ) -> tuple[PostgresEngine, str]:
     """Registers a cog by creating a database for it and initializing any tables it has
 
     Args:
         cog (Cog): Cog instance
         config (dict): database connection info
         tables (list[type[Table]]): list of piccolo table subclasses
+        max_size (int): maximum number of database connections, 20 by default
 
     Returns:
         Tuple[PostgresEngine, str]: Postgres Engine instance, migration results
     """
-    engine = await create_database_and_tables(cog, config, tables)
+    engine = await create_database_and_tables(cog, config, tables, max_size)
     result = await run_migrations(cog, config)
     return engine, result
```

