# Comparing `tmp/mysql-oop-0.0.5.tar.gz` & `tmp/mysql-oop-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-oop-0.0.5.tar", last modified: Wed Mar  9 11:23:09 2022, max compression
+gzip compressed data, was "mysql-oop-0.1.0.tar", last modified: Mon May 29 11:47:51 2023, max compression
```

## Comparing `mysql-oop-0.0.5.tar` & `mysql-oop-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-03-09 11:23:09.166457 mysql-oop-0.0.5/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1084 2021-12-28 03:50:54.000000 mysql-oop-0.0.5/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)     1293 2022-03-09 11:23:09.166457 mysql-oop-0.0.5/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      808 2022-03-09 08:32:38.000000 mysql-oop-0.0.5/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      105 2022-02-23 14:35:58.000000 mysql-oop-0.0.5/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      608 2022-03-09 11:23:09.166457 mysql-oop-0.0.5/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-03-09 11:23:09.162457 mysql-oop-0.0.5/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-03-09 11:23:09.162457 mysql-oop-0.0.5/src/mysql_oop.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     1293 2022-03-09 11:23:08.000000 mysql-oop-0.0.5/src/mysql_oop.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      240 2022-03-09 11:23:09.000000 mysql-oop-0.0.5/src/mysql_oop.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2022-03-09 11:23:09.000000 mysql-oop-0.0.5/src/mysql_oop.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        9 2022-03-09 11:23:09.000000 mysql-oop-0.0.5/src/mysql_oop.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-03-09 11:23:09.166457 mysql-oop-0.0.5/src/mysqloop/
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2022-03-04 11:21:01.000000 mysql-oop-0.0.5/src/mysqloop/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14682 2022-03-09 11:12:43.000000 mysql-oop-0.0.5/src/mysqloop/mysqloop.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 11:47:51.744931 mysql-oop-0.1.0/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1084 2023-05-28 08:47:28.000000 mysql-oop-0.1.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-29 11:47:51.744931 mysql-oop-0.1.0/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-29 08:33:20.000000 mysql-oop-0.1.0/README.md
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      157 2023-05-29 11:46:25.000000 mysql-oop-0.1.0/pyproject.toml
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      608 2023-05-29 11:47:51.744931 mysql-oop-0.1.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 11:47:51.740931 mysql-oop-0.1.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 11:47:51.744931 mysql-oop-0.1.0/src/mysql_oop.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1535 2023-05-29 11:47:51.000000 mysql-oop-0.1.0/src/mysql_oop.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2023-05-29 11:47:51.000000 mysql-oop-0.1.0/src/mysql_oop.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-29 11:47:51.000000 mysql-oop-0.1.0/src/mysql_oop.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-29 11:47:51.000000 mysql-oop-0.1.0/src/mysql_oop.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-29 11:47:51.744931 mysql-oop-0.1.0/src/mysqloop/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-29 11:33:32.000000 mysql-oop-0.1.0/src/mysqloop/Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      153 2023-05-29 08:53:58.000000 mysql-oop-0.1.0/src/mysqloop/Users.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       64 2023-05-29 08:15:37.000000 mysql-oop-0.1.0/src/mysqloop/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14915 2023-05-29 11:24:19.000000 mysql-oop-0.1.0/src/mysqloop/mysqloop.py
```

### Comparing `mysql-oop-0.0.5/LICENSE` & `mysql-oop-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-oop-0.0.5/PKG-INFO` & `mysql-oop-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.0.5
+Version: 0.1.0
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# mysql oop
+# mysql
 
-### sqlite Object Oriented
+### mysql Object Oriented
 
-```python
-from sqliteoop import sqlite
-db = sqlite("./demo.db")
+```shell
+touch .env #and edit .env file
+```
+project root path command run 'touch .env' and paste environment config
+```text
+DB_HOST = "127.0.0.1" #host
+DB_PORT = 3306 #port
+DB_USER = 'root' #database login user
+DB_PASSWORD = None #password
+DB_NAME = 'name' #database
+```
 
+```python
+from mysqloop.mysqloop import mysqloop
+import time
+db = mysqloop()
 # create table
 createtable = db.table("user_name").create_table({
     "id":"INTEGER PRIMARY KEY AUTOINCREMENT",
     "name":"VARCHAR(80) NOT NULL"
 })
 print(createtable)
 
@@ -46,9 +56,7 @@
 # select
 db.table("user_name").where("name","<>","davie").limit(5).select("*")
 
 # find
 db.table("user_name").where("name","johan").find("*")
 
 ```
-
-
```

### Comparing `mysql-oop-0.0.5/setup.cfg` & `mysql-oop-0.1.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mysql-oop
-version = 0.0.5
+version = 0.1.0
 author = hahadu
 author_email = mhyzhu@163.com
 description = python mysql OOP class
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hahadu/mysql-py-oop
 project_urls =
```

### Comparing `mysql-oop-0.0.5/src/mysql_oop.egg-info/PKG-INFO` & `mysql-oop-0.1.0/src/mysql_oop.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: mysql-oop
-Version: 0.0.5
+Version: 0.1.0
 Summary: python mysql OOP class
 Home-page: https://github.com/hahadu/mysql-py-oop
 Author: hahadu
 Author-email: mhyzhu@163.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hahadu/mysql-py-oop/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# mysql oop
+# mysql
 
-### sqlite Object Oriented
+### mysql Object Oriented
 
-```python
-from sqliteoop import sqlite
-db = sqlite("./demo.db")
+```shell
+touch .env #and edit .env file
+```
+project root path command run 'touch .env' and paste environment config
+```text
+DB_HOST = "127.0.0.1" #host
+DB_PORT = 3306 #port
+DB_USER = 'root' #database login user
+DB_PASSWORD = None #password
+DB_NAME = 'name' #database
+```
 
+```python
+from mysqloop.mysqloop import mysqloop
+import time
+db = mysqloop()
 # create table
 createtable = db.table("user_name").create_table({
     "id":"INTEGER PRIMARY KEY AUTOINCREMENT",
     "name":"VARCHAR(80) NOT NULL"
 })
 print(createtable)
 
@@ -46,9 +56,7 @@
 # select
 db.table("user_name").where("name","<>","davie").limit(5).select("*")
 
 # find
 db.table("user_name").where("name","johan").find("*")
 
 ```
-
-
```

### Comparing `mysql-oop-0.0.5/src/mysqloop/mysqloop.py` & `mysql-oop-0.1.0/src/mysqloop/mysqloop.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from mysql import connector
-
+from dotenv.main import load_dotenv
+import os
+load_dotenv()
 
 class mysqloop:
     SPACE_CHARACTER = " "
     SINGLE_QUOTES_CHARACTER = "\'"
     SEMICOLON_CHARACTER = ";"
     EQUAL_SIGN_CHARACTER = "="
     LINE_BREAK_CHARACTER = "\n"
     DIRECTORY_SEPARATOR = "/"
 
-    __table_name = ""
+    """
+    表名
+    """
+    _table_name = ""
     __base_where_clause_string = ""
     __base_where_limit_clause_string = ""
     __base_where_orderby_clause_string = ""
     """
     GROUP BY 子句放在 WHERE 子句之后，放在 ORDER BY 子句之前
     """
     __base_where_groupby_clause_string = ""
@@ -23,53 +28,66 @@
     __base_where_distinct_clause_string = ""
     __base_where_join_clause_string = ""
     __base_where_offset_clause_string = ""
     __operators = [
         "<=>", "=", "!=", "<>", ">", "<", ">=", "<=", "!<", "!>", "!",
         "AND", "BETWEEN", "NOT BETWEEN", "IN", "NOT IN", "LIKE", "EXISTS",
         "GLOB", "NOT", "OR", "XOR", "IS NULL", "IS", "IS NOT", "||", "UNIQUE",
-        "REGEXP", "RLIKE", "NULL",
+        "REGEXP", "RLIKE",
     ]
     __config = {
-        "db_host": "127.0.0.1",
-        "port": "3306",
-        "db_user": "",
-        "db_password": "",
-        "db_name": ""
+        "db_host": os.getenv("DB_HOST"),
+        "db_port": os.getenv("DB_PORT"),
+        "db_user": os.getenv("DB_USER"),
+        "db_password": os.getenv("DB_PASSWORD"),
+        "db_name": os.getenv("DB_NAME")
     }
 
+    db = None
+
     def __init__(self, config=None):
+        """
+        :param config:
+        """
+
         if config is not None:
             self.__config.update(config)
-        self.db = connector.connect(host=self.__config['db_host'], user=self.__config['db_user'], passwd=self.__config['db_password'], database=self.__config['db_name'])
+        self.db = connector.connect(host=self.__config['db_host'], port=self.__config['db_port'],
+                                    user=self.__config['db_user'], password=self.__config['db_password'],
+                                    database=self.__config['db_name'])
 
-    def connect(self, db_host="127.0.0.1", db_user="root", db_password=None, db_name="root"):
+    def connect(self, db_host="127.0.0.1", db_port=3306, db_user="root", db_password=None, db_name="root"):
         self.db = connector.connect(
             host=db_host,
+            port=db_port,
             user=db_user,
             passwd=db_password,
             database=db_name
         )
+        print('---db---', self.db)
         return self
 
     def table(self, table_name):
         """
         设置连接table
         :param table_name:
         :return:
         """
-        self.__table_name = table_name
-        self._cursor = self.db.cursor()
+        self._table_name = table_name
+        self._set_cursor()
         return self
 
+    def _set_cursor(self):
+        self._cursor = self.db.cursor()
+
     def get_table_name(self):
-        return self.__table_name
+        return self._table_name
 
     def __is_tablename(self):
-        if len(self.__table_name) == 0:
+        if len(self._table_name) == 0:
             return "No query form is specified 亲，叫个表吧，求你了！"
         else:
             return True
 
     def query(self, sql):
         self._cursor.execute(sql)
         columns_tuple = self._cursor.description
@@ -95,15 +113,15 @@
         selected += self.SPACE_CHARACTER
         selected += self.__base_where_distinct_clause_string
         selected += self.SPACE_CHARACTER
         selected += columns
         selected += self.SPACE_CHARACTER
         selected += "FROM"
         selected += self.SPACE_CHARACTER
-        selected += self.__table_name
+        selected += self._table_name
         selected += self.SPACE_CHARACTER
         selected += self.__base_where_clause_string
         selected += self.__base_where_groupby_clause_string
         selected += self.__base_where_orderby_clause_string
         selected += self.__base_where_limit_clause_string
         selected += self.__base_where_join_clause_string
         selected += self.__base_where_offset_clause_string
@@ -125,49 +143,37 @@
         :param op:
         :param value:
         :param _boolean:
         :return:
         """
 
         if value is None:
-            if op is None:
-                op = "IS"
-                value = "NULL"
-            else:
-                value = op
-                op = "="
+            value = op
+            op = "="
 
         op = str(op)
         value = str(value)
 
         if len(self.__base_where_clause_string) > 0:
             self.__base_where_clause_string += _boolean
             self.__base_where_clause_string += self.SPACE_CHARACTER
+
         else:
             self.__base_where_clause_string += "WHERE"
             self.__base_where_clause_string += self.SPACE_CHARACTER
         self.__base_where_clause_string += column
         self.__base_where_clause_string += self.SPACE_CHARACTER
         self.__base_where_clause_string += op
         self.__base_where_clause_string += self.SPACE_CHARACTER
-        self.__base_where_clause_string += self.__parse_value(value)
+        self.__base_where_clause_string += self.SINGLE_QUOTES_CHARACTER
+        self.__base_where_clause_string += str(value)
+        self.__base_where_clause_string += self.SINGLE_QUOTES_CHARACTER
         self.__base_where_clause_string += self.SPACE_CHARACTER
-
         return self
 
-    def __parse_value(self, value):
-        value_str = ""
-        if self.__operators.count(value) == 0:
-            value_str += self.SINGLE_QUOTES_CHARACTER
-            value_str += value
-            value_str += self.SINGLE_QUOTES_CHARACTER
-        else:
-            value_str += value
-        return value_str
-
     def limit(self, limit):
         """
         查询数量
         :param limit:
         :return:
         """
         self.__base_where_limit_clause_string = "LIMIT"
@@ -226,14 +232,17 @@
         self.__base_where_join_clause_string += self.SPACE_CHARACTER
         return self
 
     def count(self):
         data = self.select("count(*)")
         return data[0]["count(*)"]
 
+    def exists(self):
+        return True if self.count() > 0 else False
+
     def insert(self, columns: dict or list):
         """
         批量插入数据
         :param columns:
         :return:
         """
         # print(type(type(columns)))
@@ -274,15 +283,15 @@
         :return:
         """
         _insert_string = self.__set_insert_string(columns)
         columns_string = _insert_string[0]
         values_tuple = _insert_string[1]
         values_string = _insert_string[2]
         insert = "INSERT INTO "
-        insert += self.__table_name
+        insert += self._table_name
         insert += " ( "
         insert += columns_string
         insert += " ) VALUES ( "
         insert += values_string
         insert += "); "
         self._cursor.execute(insert, values_tuple)
 
@@ -318,29 +327,29 @@
             update_string += self.SINGLE_QUOTES_CHARACTER
             update_string += str(column_value)
             update_string += self.SINGLE_QUOTES_CHARACTER
             update_string += ","
 
         update_string = update_string[:-1]
         update = "UPDATE "
-        update += self.__table_name
+        update += self._table_name
         update += self.SPACE_CHARACTER
         update += "SET"
         update += self.SPACE_CHARACTER
         update += update_string
         update += self.SPACE_CHARACTER
         update += self.__base_where_clause_string
         self._cursor.execute(update)
         self.db.commit()
         return self._cursor.rowcount
 
     def delete(self):
         delete_data = "DELETE FROM"
         delete_data += self.SPACE_CHARACTER
-        delete_data += self.__table_name
+        delete_data += self._table_name
         delete_data += self.SPACE_CHARACTER
         delete_data += self.__base_where_clause_string
         delete_data += self.SEMICOLON_CHARACTER
         self._cursor.execute(delete_data)
         self.db.commit()
 
         return self._cursor.rowcount
@@ -363,15 +372,15 @@
             columns_string += self.SPACE_CHARACTER
             columns_string += column_value
             columns_string += ","
 
         # 移除最后一个，
         columns_string = columns_string[:-1]
         created = "CREATE TABLE "
-        created += self.__table_name
+        created += self._table_name
         created += " ( "
         created += columns_string
         if primary_key is not None:
             created += ", PRIMARY KEY ( "
             created += primary_key
             created += " )"
         created += " )ENGINE=InnoDB DEFAULT CHARSET=utf8; "
@@ -381,34 +390,34 @@
             return self.desc_table()
         except ValueError:
             raise Exception("create table fail!")
 
     def delete_table(self):
         delete_table = "DROP TABLE"
         delete_table += self.SPACE_CHARACTER
-        delete_table += self.__table_name
+        delete_table += self._table_name
         self._cursor.execute(delete_table)
         self.db.commit()
         if not self.is_table():
             return True
         else:
             return False
 
     def desc_table(self):
         if not self.is_table():
             return None
-        table_name = self.__table_name
+        table_name = self._table_name
         sql = "desc " + table_name + ";"
         return self.query(sql)
 
     def show_table(self):
-        table_name = self.__table_name
+        table_name = self._table_name
         sql = "SHOW TABLES LIKE '" + table_name + "';"
         result = self.query(sql)
-        self.__table_name = table_name
+        self._table_name = table_name
         return result
 
     def show_tables(self):
         sql = "SHOW TABLES;"
         result = self.query(sql)
         return result
```

