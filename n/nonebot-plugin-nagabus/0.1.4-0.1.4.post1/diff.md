# Comparing `tmp/nonebot_plugin_nagabus-0.1.4.tar.gz` & `tmp/nonebot_plugin_nagabus-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.1.4.post1.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.4.tar` & `nonebot_plugin_nagabus-0.1.4.post1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.4/LICENSE
--rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    19092 2023-05-29 12:30:46.133833 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-29 12:07:35.829395 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/auto_retry.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      677 2023-05-29 12:30:46.122833 nonebot_plugin_nagabus-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.4/README.md
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.4.post1/LICENSE
+-rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    18823 2023-05-29 12:41:37.629257 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      683 2023-05-29 12:41:50.868484 nonebot_plugin_nagabus-0.1.4.post1/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.4.post1/README.md
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.4.post1/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.4/LICENSE` & `nonebot_plugin_nagabus-0.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/errors.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,18 @@
     def __init__(self, cookies: Dict[str, str], timeout: float = 90.0):
         if conf.naga_fake_api:
             self.api = FakeNagaApi()
             logger.warning("using fake naga api")
         else:
             self.api = NagaApi(cookies)
 
-        self._order_mutex = Lock()
         self._majsoul_order_mutex = Lock()
         self._tenhou_order_mutex = Lock()
 
-        self._last_majsoul_haihu_id = None
+        self._last_custom_haihu_id = None
 
         self._order_report = ObservableOrderReport(self.api)
         self.timeout = timeout
 
     async def close(self):
         await self.api.close()
 
@@ -126,55 +125,54 @@
         finally:
             cancel_flag = True
 
     async def _order_custom(self, data: Union[list, str],
                             rule: NagaGameRule,
                             model_type: Union[NagaHanchanModelType,
                                               NagaTonpuuModelType]) -> NagaOrder:
-        async with self._order_mutex:
-            current = datetime.now(tz=TZ_TOKYO)
-            await self.api.analyze_custom(data, 0, rule, model_type)
+        current = datetime.now(tz=TZ_TOKYO)
+        await self.api.analyze_custom(data, 0, rule, model_type)
 
-            order_fut = asyncio.get_running_loop().create_future()
-            retry = 0  # 下单完马上获取order的话，有时候order刷新不出来，可以多试几次
+        order_fut = asyncio.get_running_loop().create_future()
+        retry = 0  # 下单完马上获取order的话，有时候order刷新不出来，可以多试几次
 
-            def _make_callback():
-                async def callback(order_report: OrderReportList):
-                    nonlocal retry
-
-                    try:
-                        if len(order_report.order) == 0:
-                            raise OrderError('order failed')
+        def _make_callback():
+            async def callback(order_report: OrderReportList):
+                nonlocal retry
 
-                        order = order_report.order[0]
+                try:
+                    for order in order_report.order:
+                        # order.haihu_id: custom_haihu_2023-05-25T23:46:07_QRIGFOKmA4HT4CJF
+                        if not order.haihu_id.startswith("custom_haihu_"):
+                            continue
 
-                        if order.haihu_id == self._last_majsoul_haihu_id:
-                            raise OrderError('order failed')
+                        if order.haihu_id == self._last_custom_haihu_id:
+                            break
 
-                        # order.haihu_id: custom_haihu_2023-05-25T23:46:07_QRIGFOKmA4HT4CJF
                         order_time = datetime.fromisoformat(order.haihu_id[13:32]).replace(tzinfo=TZ_TOKYO)
                         if abs(current.timestamp() - order_time.timestamp()) >= 30:  # 时间差超过了30s
-                            raise OrderError('order failed')
+                            break
 
-                        self._last_majsoul_haihu_id = order.haihu_id
+                        self._last_custom_haihu_id = order.haihu_id
                         order_fut.set_result(order)
-                    except OrderError as e:
-                        if retry < 5:
-                            self._order_report.observe_once(_make_callback())
-                            retry += 1
-                        else:
-                            order_fut.set_exception(e)
-                    except BaseException as e:
-                        order_fut.set_exception(e)
+                        return
 
-                return callback
+                    if retry < 5:
+                        self._order_report.observe_once(_make_callback())
+                        retry += 1
+                    else:
+                        raise OrderError('order failed')
+                except BaseException as e:
+                    order_fut.set_exception(e)
 
-            self._order_report.observe_once(_make_callback())
+            return callback
+
+        self._order_report.observe_once(_make_callback())
 
-            return await order_fut
+        return await order_fut
 
     async def analyze_majsoul(self, majsoul_uuid: str, kyoku: int, honba: int,
                               customer_id: int,
                               *,
                               model_type: Union[NagaHanchanModelType,
                                                 NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
         sess = get_session()
@@ -309,18 +307,17 @@
             await sess.commit()
 
             return NagaServiceOrder(report, 10)
         else:
             return NagaServiceOrder(report, 0)
 
     async def _order_tenhou(self, haihu_id: str, seat: int, model_type: NagaHanchanModelType):
-        async with self._order_mutex:
-            res = await self.api.analyze_tenhou(haihu_id, seat, model_type)
-            if res.status != 200:
-                raise OrderError(res.msg)
+        res = await self.api.analyze_tenhou(haihu_id, seat, model_type)
+        if res.status != 200:
+            raise OrderError(res.msg)
 
     # needs test
     async def analyze_tenhou(self, haihu_id: str, seat: int, customer_id: int,
                              *,
                              model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> NagaServiceOrder:
         sess = get_session()
```

### Comparing `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/pyproject.toml` & `nonebot_plugin_nagabus-0.1.4.post1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.4"
+version = "0.1.4.post1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.1.4/README.md` & `nonebot_plugin_nagabus-0.1.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4/PKG-INFO` & `nonebot_plugin_nagabus-0.1.4.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

