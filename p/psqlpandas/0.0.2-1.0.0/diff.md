# Comparing `tmp/psqlpandas-0.0.2.tar.gz` & `tmp/psqlpandas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-0.0.2.tar", max compression
+gzip compressed data, was "psqlpandas-1.0.0.tar", max compression
```

## Comparing `psqlpandas-0.0.2.tar` & `psqlpandas-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      900 2023-05-16 14:37:03.958903 psqlpandas-0.0.2/LICENSE
--rw-r--r--   0        0        0      199 2023-05-16 14:37:03.958903 psqlpandas-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-16 14:37:03.959903 psqlpandas-0.0.2/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-05-16 14:37:03.959903 psqlpandas-0.0.2/psqlpandas/__version__.py
--rw-r--r--   0        0        0     8037 2023-05-16 14:37:03.959903 psqlpandas-0.0.2/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-05-16 14:37:03.959903 psqlpandas-0.0.2/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     1909 2023-05-16 14:37:03.959903 psqlpandas-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-0.0.2/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-05-29 11:07:32.790702 psqlpandas-1.0.0/LICENSE
+-rw-r--r--   0        0        0      199 2023-05-29 11:07:32.790702 psqlpandas-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 11:07:32.814702 psqlpandas-1.0.0/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     7674 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     1909 2023-05-29 11:07:32.791702 psqlpandas-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.0.0/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.0.0/PKG-INFO
```

### Comparing `psqlpandas-0.0.2/LICENSE` & `psqlpandas-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-0.0.2/psqlpandas/postgresql.py` & `psqlpandas-1.0.0/psqlpandas/postgresql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,119 @@
-from abc import ABC, abstractmethod
 from typing import List, Dict, Tuple, Any
 import logging
 
 import pandas as pd
 import numpy as np
 import psycopg2
 import psycopg2.extras as pgex
 from sqlalchemy import create_engine, text
 
 
-class DatabaseConnector(ABC):
-    """
-    This class act as a wrapper for the connector chosen.
-    """
+class PostgresqlDatabaseConnector:
+    def __init__(
+        self, dbname: str, user: str, host: str, port: str, password: str
+    ) -> None:
+        self._conn = psycopg2.connect(
+            user=user,
+            password=password,
+            host=host,
+            port=port,
+            database=dbname,
+        )
+        self._sqlalchemy_conn = create_engine(
+            f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{dbname}"
+        )
 
-    def __init__(self, dbname: str):
-        """
-        Constructor
+    def __del__(self) -> None:
+        self._conn.close()
+        self._sqlalchemy_conn.dispose()
 
-        Args:
-            dbname (str): database name
-        """
-        self._dbname = dbname
+    @staticmethod
+    def execute_values(cursor, query, tuples):
+        return pgex.execute_values(cursor, query, tuples)
 
-    @abstractmethod
-    def connect(self):
-        """
-        Returns connection
+    def read(self, query: str) -> List[Tuple[str]]:
         """
-        pass
+        Reads values from database.
 
-    @abstractmethod
-    def get_sqlalchemy_connection(self):
-        pass
-
-
-class PostgresqlDatabaseConnector(DatabaseConnector):
-    def __init__(self, dbname: str, user: str, host: str, port: str, password: str):
-        super().__init__(dbname)
-        self._user = user
-        self._host = host
-        self._port = port
-        self._password = password
-
-    def connect(self):
-        return psycopg2.connect(
-            user=self._user,
-            password=self._password,
-            host=self._host,
-            port=self._port,
-            database=self._dbname,
-        )
+        NOTE: around 3x faster than self.read_df
 
-    def get_sqlalchemy_connection(self):
-        engine = create_engine(
-            f"postgresql+psycopg2://{self._user}:{self._password}@{self._host}:{self._port}/{self._dbname}"
-        )
-        return engine
+        Args:
+            query (str): select query to be executed
 
-    @staticmethod
-    def execute_values(cursor, query, tuples):
-        return pgex.execute_values(cursor, query, tuples)
+        Returns:
+            List[Tuple[str]]: list of rows retrieved
+        """
+        cur = self._conn.cursor()
 
-    def read_from_db(
+        try:
+            cur.execute(query)
+            data = cur.fetchall()
+        except Exception as e:
+            logging.error(f"Error while reading query: {query}")
+            logging.error(e)
+            cur.close()
+            raise
+        else:
+            cur.close()
+            return data
+
+    def read_df(
         self, query: str, parse_dates: List[str] | str | None = None
     ) -> pd.DataFrame:
         """
-        Reads data from postgres db.
+        Reads values from database directly into pandas dataframe
+
+        NOTE: generally slower than self.read. But can be usefult for automatic casting of types (including dates).
 
         Args:
-            query (str): query
-            parse_dates (List[str] | str | None, optional): list of columns to be parsed as dates. Defaults to None.
+            query (str): select query to be executed
+            parse_dates (List[str] | str | None, optional): columns to be parsed at dates. Defaults to None.
 
         Returns:
-            pd.DataFrame: dataframe of the read data
+            pd.DataFrame: dataframe of data retrieved
         """
-        if isinstance(parse_dates, str):
-            parse_dates = [parse_dates]
         try:
-            engine = self.get_sqlalchemy_connection()
-            with engine.begin() as connection:
-                table = pd.read_sql_query(
-                    text(query), con=connection, parse_dates=parse_dates
-                )
-            engine.dispose()
+            return pd.read_sql_query(
+                text(query), con=self._sqlalchemy_conn, parse_dates=parse_dates
+            )
         except Exception as e:
-            logging.error(f"Error while executing query: {query}")
+            logging.error(f"Error while reading query: {query}")
             logging.error(e)
             raise
-        if parse_dates is not None:
-            for col in parse_dates:
-                table[col] = pd.to_datetime(table[col])
-
-        return table
 
     def execute_sql_query(self, query, row=None):
-        conn = self.connect()
-        cur = conn.cursor()
+        cur = self._conn.cursor()
 
         try:
             if row is None:
                 cur.execute(query)
             else:
                 cur.execute(query, row)
-            conn.commit()
+            self._conn.commit()
             cur.close()
-            conn.close()
             return True
         except Exception as e:
             logging.error(f"Error while executing query: {query}")
             logging.error(e)
             cur.close()
-            conn.close()
             raise
 
     def execute_sql_query_values(self, query: str, tuples: Tuple[Any]):
-        conn = self.connect()
-        cur = conn.cursor()
+        cur = self._conn.cursor()
 
         try:
             self.execute_values(cur, query, tuples)
-            conn.commit()
+            self._conn.commit()
             cur.close()
-            conn.close()
             return True
         except Exception as e:
             logging.error(f"Error while executing query: {query}")
             logging.error(e)
             cur.close()
-            conn.close()
             raise
 
     def update_db_row(
         self,
         df_dict: Dict[str, object],
         tablename: str,
         sql_where_condition: str | None = None,
```

### Comparing `psqlpandas-0.0.2/pyproject.toml` & `psqlpandas-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "0.0.2"
+version = "1.0.0"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
```

### Comparing `psqlpandas-0.0.2/setup.py` & `psqlpandas-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '0.0.2',
+    'version': '1.0.0',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-0.0.2/PKG-INFO` & `psqlpandas-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 0.0.2
+Version: 1.0.0
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

