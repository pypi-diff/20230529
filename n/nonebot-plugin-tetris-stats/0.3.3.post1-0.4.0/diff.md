# Comparing `tmp/nonebot_plugin_tetris_stats-0.3.3.post1.tar.gz` & `tmp/nonebot_plugin_tetris_stats-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-0.3.3.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-0.3.3.post1.tar` & `nonebot_plugin_tetris_stats-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/LICENSE
--rw-r--r--   0        0        0     1043 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/README.md
--rw-r--r--   0        0        0       34 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0       72 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      874 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0     9834 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
--rw-r--r--   0        0        0     5296 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py
--rw-r--r--   0        0        0     8908 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py
--rw-r--r--   0        0        0     7272 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py
--rw-r--r--   0        0        0       49 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/config.py
--rw-r--r--   0        0        0     2675 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/database.py
--rw-r--r--   0        0        0     3595 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/message_analyzer.py
--rw-r--r--   0        0        0      895 2023-02-14 23:52:42.362000 nonebot_plugin_tetris_stats-0.3.3.post1/pyproject.toml
--rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-0.3.3.post1/setup.py
--rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-0.3.3.post1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1043 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/README.md
+-rw-r--r--   0        0        0       34 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0    12820 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
+-rw-r--r--   0        0        0     5296 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py
+-rw-r--r--   0        0        0     8908 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py
+-rw-r--r--   0        0        0     7272 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py
+-rw-r--r--   0        0        0       49 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/config.py
+-rw-r--r--   0        0        0     4609 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/database.py
+-rw-r--r--   0        0        0     3981 2023-05-29 21:00:04.935483 nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/message_analyzer.py
+-rw-r--r--   0        0        0      889 2023-05-29 21:00:04.939483 nonebot_plugin_tetris_stats-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2080 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/LICENSE` & `nonebot_plugin_tetris_stats-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/README.md` & `nonebot_plugin_tetris_stats-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from nonebot.adapters.onebot.v11 import GROUP, MessageEvent
 from nonebot.matcher import Matcher
 
 from .processor import Processor
 
 IOBind = on_regex(pattern=r'^io绑定|^iobind', flags=I, permission=GROUP)
 IOStats = on_regex(pattern=r'^io查|^iostats', flags=I, permission=GROUP)
-
+IORank = on_regex(pattern=r'^io段位|^iorank', flags=I, permission=GROUP)
 
 @IOBind.handle()
 async def _(event: MessageEvent, matcher: Matcher):
     await matcher.finish(
         await Processor.handle_bind(
             message=event.raw_message,
             qq_number=event.sender.user_id
@@ -26,7 +26,15 @@
         await matcher.finish('不能查询bot的信息')
     await matcher.finish(
         await Processor.handle_query(
             message=event.raw_message,
             qq_number=event.sender.user_id
         )
     )
+
+@IORank.handle()
+async def _(event: MessageEvent, matcher: Matcher):
+    await matcher.finish(
+        await Processor.handle_rank(
+            message=event.raw_message
+        )
+    )
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import math
 from asyncio import gather
 from typing import Any
 
 from nonebot.log import logger
 
 from ...utils.database import DataBase
 from ...utils.message_analyzer import (
     handle_bind_message,
-    handle_stats_query_message
+    handle_rank_message,
+    handle_stats_query_message,
 )
 from .request import Request
 
 
 class Processor:
     @classmethod
     async def handle_bind(cls, message: str, qq_number: int | None) -> str:
@@ -40,14 +42,90 @@
                     game_type='IO'
                 )
             )
         logger.error('预期外行为, 请上报GitHub')
         return '出现预期外行为，请查看后台信息'
 
     @classmethod
+    async def handle_rank(cls, message: str):
+        query_rank = await handle_rank_message(message)
+        rank_info = await DataBase.query_rank_info_today(rank=query_rank.lower())
+
+        if rank_info is None:
+            ranks_percentiles = {
+                'x': 1,
+                'u': 5,
+                'ss': 11,
+                's+': 17,
+                's': 23,
+                's-': 30,
+                'a+': 38,
+                'a': 46,
+                'a-': 54,
+                'b+': 62,
+                'b': 70,
+                'b-': 78,
+                'c+': 84,
+                'c': 90,
+                'c-': 95,
+                'd+': 97.5,
+                'd': 100,
+            }
+
+            if query_rank.lower() not in (i for i in ranks_percentiles.keys()):
+                return '未知段位'
+
+            result = await Request.request('https://ch.tetr.io/api/users/lists/league/all')
+            users: list = result[2]['data']['users']
+
+            def avg(rank_users: list, column: str, playercount: int | None = None) -> float:
+                return sum(i['league'][column] for i in rank_users) / (playercount or len(rank_users))
+
+            for rank, percentile in ranks_percentiles.items():
+                offset = math.floor((percentile / 100) * len(users)) - 1
+                tr = users[offset]['league']['rating']
+
+                rank_users = list(filter(lambda x: x['league']['rank'] == rank, users))
+                playercount = len(rank_users)
+
+                avg_apm = avg(rank_users, 'apm', playercount)
+                avg_pps = avg(rank_users, 'pps', playercount)
+                avg_vs = avg(rank_users, 'vs', playercount)
+
+                await DataBase.write_rank_info_today(
+                    rank=rank,
+                    trline=tr,
+                    playercount=playercount,
+                    avgapm=avg_apm,
+                    avgpps=avg_pps,
+                    avgvs=avg_vs
+                    )
+
+            return await Processor.handle_rank(message=message)
+        else:
+            avg_apm = round(rank_info[3], 2)
+            avg_pps = round(rank_info[4], 2)
+            avg_vs = round(rank_info[5], 2)
+            avg_lpm = round((avg_pps * 24), 2)
+            avg_apl = round((avg_apm / avg_lpm), 2)
+            avg_adpm = round((avg_vs * 0.6), 2)
+            avg_adpl = round((avg_adpm / avg_lpm), 2)
+
+            message = f'{query_rank.upper()} 段, 分数线 {round(rank_info[1], 2)} TR, {rank_info[2]} 名玩家'
+            message += f'\n对比昨日趋势: {rank_info[0]}'
+            message += '\n'
+            message += f"\nL'PM: {avg_lpm} ( {avg_pps} pps )"
+            message += f'\nAPM: {avg_apm} ( x{avg_apl} )'
+            message += f'\nADPM: {avg_adpm} ( x{avg_adpl} ) ( {avg_vs}vs )'
+            message += '\n'
+            message += f'\n数据更新时间: {rank_info[6]}'
+
+        return message
+
+    @classmethod
     async def handle_query(cls, message: str, qq_number: int | None):
         '''处理查询消息'''
         decoded_message = await handle_stats_query_message(message=message, game_type='IO')
         if decoded_message[0] is None:
             return decoded_message[1][0]
         if decoded_message[0] == 'AT':  # 在入口处判断是否@bot本身
             bind_info = await DataBase.query_bind_info(qq_number=decoded_message[1][1], game_type='IO')
@@ -65,32 +143,32 @@
         if decoded_message[0] == 'ID':
             return await Processor.generate_message(user_id=decoded_message[1][1])
         if decoded_message[0] == 'Name':
             return await Processor.generate_message(user_name=decoded_message[1][1])
 
     @classmethod
     async def get_user_data(
-        cls,
-        user_name: str | None = None,
-        user_id: str | None = None
+            cls,
+            user_name: str | None = None,
+            user_id: str | None = None
     ) -> tuple[bool, bool, dict[str, Any]]:
         '''获取用户数据'''
         if user_name is not None and user_id is None:
             user_data_url = f'https://ch.tetr.io/api/users/{user_name}'
         elif user_name is None and user_id is not None:
             user_data_url = f'https://ch.tetr.io/api/users/{user_id}'
         else:
             raise ValueError('预期外行为, 请上报GitHub')
         return await Request.request(user_data_url)
 
     @classmethod
     async def get_solo_data(
-        cls,
-        user_name: str | None = None,
-        user_id: str | None = None
+            cls,
+            user_name: str | None = None,
+            user_id: str | None = None
     ) -> tuple[bool, bool, dict[str, Any]]:
         '''获取Solo数据'''
         if user_name is not None and user_id is None:
             user_solo_url = f'https://ch.tetr.io/api/users/{user_name}/records'
         elif user_name is None and user_id is not None:
             user_solo_url = f'https://ch.tetr.io/api/users/{user_id}/records'
         else:
@@ -161,17 +239,17 @@
             blitz_stats['Score'] = blitz['record']['endcontext']['score']
             if blitz['rank'] is not None:
                 blitz_stats['Rank'] = blitz['rank']
         return blitz_stats
 
     @classmethod
     async def generate_message(
-        cls,
-        user_name: str | None = None,
-        user_id: str | None = None
+            cls,
+            user_name: str | None = None,
+            user_id: str | None = None
     ) -> str:
         '''生成消息'''
         user_data, solo_data = await gather(
             cls.get_user_data(user_name=user_name, user_id=user_id),
             cls.get_solo_data(user_name=user_name, user_id=user_id)
         )
         if user_data[0] is False:
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/database.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/database.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import os
 from asyncio import gather
 from sqlite3 import Connection, connect
 
 from nonebot import get_driver
 from nonebot.log import logger
 
@@ -35,19 +36,70 @@
         cursor = cls._db.cursor()
         cursor.execute('''CREATE TABLE IF NOT EXISTS IOBIND
                         (QQ INTEGER NOT NULL,
                         USER TEXT NOT NULL)''')
         cursor.execute('''CREATE TABLE IF NOT EXISTS TOPBIND
                         (QQ INTEGER NOT NULL,
                         USER TEXT NOT NULL)''')
+        cursor.execute('''CREATE TABLE IF NOT EXISTS IORANK
+                        (RANK VARCHAR(2) NOT NULL,
+                         TRENDING CHAR(1) NOT NULL,
+                         TRLINE FLOAT NOT NULL,
+                         PLAYERCOUNT INTEGER NOT NULL,
+                         AVGAPM FLOAT NOT NULL,
+                         AVGPPS FLOAT NOT NULL,
+                         ARGVS FLOAT NOT NULL,
+                         DATE TEXT NOT NULL)''')
         cls._db.commit()
         logger.info('数据库初始化完成')
         return cls._db
 
     @classmethod
+    async def query_rank_info_today(cls, rank: str) -> list | None:
+        '''查询段位信息'''
+        db = await cls._get_db()
+        cursor = db.cursor()
+        cursor.execute('''SELECT TRENDING, TRLINE, PLAYERCOUNT, AVGAPM, AVGPPS, ARGVS, DATE
+                        FROM IORANK
+                        WHERE RANK = ? AND DATE = ?''', (rank, datetime.date.today()))
+        result = cursor.fetchone()
+
+        if result is None:
+            return None
+
+        return list(result)
+
+    @classmethod
+    async def write_rank_info_today(cls, rank: str, trline: int, playercount: int, avgapm: float, avgpps: float, avgvs: float):
+        '''写入段位信息'''
+
+        db = await cls._get_db()
+        cursor = db.cursor()
+        cursor.execute('''SELECT TRLINE
+                        FROM IORANK
+                        WHERE RANK = ? AND DATE = ?''', (rank, datetime.date.today()))
+
+        result = cursor.fetchone()
+
+        if result is None:
+            trending = '?'
+        else:
+            if result[0] > trline:
+                trending = '↑'
+            else:
+                trending = '↓'
+
+        cursor.execute('''INSERT INTO IORANK
+                        (RANK, TRENDING, TRLINE, PLAYERCOUNT, AVGAPM, AVGPPS, ARGVS, DATE)
+                        VALUES (?,?,?,?,?,?,?,?)''',
+                       (rank, trending, trline, playercount, avgapm, avgpps, avgvs, datetime.date.today()))
+
+        db.commit()
+
+    @classmethod
     async def _get_db(cls) -> Connection:
         '''获取数据库对象'''
         return cls._db or await cls.init_db()
 
     @classmethod
     async def query_bind_info(cls, qq_number: str | int, game_type: str) -> str | None:
         '''查询绑定信息'''
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/nonebot_plugin_tetris_stats/utils/message_analyzer.py` & `nonebot_plugin_tetris_stats-0.4.0/nonebot_plugin_tetris_stats/utils/message_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,27 @@
         # 会不会有人叫本姑娘 本大爷这种或许可以成为id的名字呢
         # TODO: 在判断是否可能是查自己的情况的时候 也去判断是否能成立为一个UserName
         return 'ME', (None, None)
     else:
         return await check_name(message, game_type)
 
 
+async def handle_rank_message(message: str) -> str:
+    _cmd_aliases = ['io段位', 'iorank']
+    # 剔除命令前缀
+    for i in _cmd_aliases:
+        if match(rf'(?i){i}', message):
+            message = sub(rf'(?i){i}', '', message)
+            message = message.strip()
+            break
+    else:
+        raise ValueError('预期外行为, 请上报GitHub')
+    return message
+
+
 async def check_name(name: str, game_type: str) -> tuple[str | None, tuple]:
     '''返回值为tuple[gameType, tuple[message, user]]'''
     if game_type == 'IO':
         if match(r'^[a-f0-9]{24}$', name):
             return 'ID', (None, name)
         if match(r'^[a-zA-Z0-9_-]{3,16}$', name):
             return 'Name', (None, name.lower())
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/pyproject.toml` & `nonebot_plugin_tetris_stats-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-tetris-stats"
-version = "0.3.3.post1"
+version = "0.4.0"
 description = "一个基于nonebot2的用于查询TETRIS相关游戏玩家数据的插件"
 authors = ["scdhh <wallfjjd@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats"
 repository = "https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats"
 license = "MIT"
```

### Comparing `nonebot_plugin_tetris_stats-0.3.3.post1/PKG-INFO` & `nonebot_plugin_tetris_stats-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 0.3.3.post1
+Version: 0.4.0
 Summary: 一个基于nonebot2的用于查询TETRIS相关游戏玩家数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: MIT
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

