# Comparing `tmp/nonebot_plugin_nagabus-0.1.3.tar.gz` & `tmp/nonebot_plugin_nagabus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.3.tar` & `nonebot_plugin_nagabus-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.3/LICENSE
--rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3002 2023-05-27 02:36:44.852322 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    17472 2023-05-29 01:34:37.295704 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      677 2023-05-29 02:07:41.819768 nonebot_plugin_nagabus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.3/README.md
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    19092 2023-05-29 12:30:46.133833 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1014 2023-05-29 12:07:35.829395 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/auto_retry.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      677 2023-05-29 12:30:46.122833 nonebot_plugin_nagabus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.4/README.md
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.3/LICENSE` & `nonebot_plugin_nagabus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/errors.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,46 +20,50 @@
 
     async def close(self):
         ...
 
     async def order_report_list(self, year: int, month: int) -> OrderReportList:
         return OrderReportList(report=self.report, order=self.order)
 
+    async def _produce_order(self, order: NagaOrder):
+        await asyncio.sleep(1)
+
+        self.order.insert(0, order)
+        logger.debug(f"Insert order (haihu_id: {order.haihu_id})")
+
     async def _produce_report(self, report: NagaReport):
         await asyncio.sleep(20)
 
         self.report.insert(0, report)
-        logger.info(f"Insert report (haihu_id: {report.haihu_id}, report_id: {report.report_id})")
+        logger.debug(f"Insert report (haihu_id: {report.haihu_id}, report_id: {report.report_id})")
 
     async def analyze_custom(self, data: Union[dict, str], seat: int = 0,
                              rule: NagaGameRule = NagaGameRule.hanchan,
                              model_type: Union[
                                  NagaHanchanModelType, NagaTonpuuModelType] = NagaHanchanModelType.nishiki):
         time = datetime.now(tz=TZ_TOKYO).replace(tzinfo=None).isoformat(timespec='seconds')
         feat = ''.join(str(random.randint(1, 9)) for _ in range(16))
         haihu_id = f"custom_haihu_{time}_{feat}"
         order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok, model=NagaModel(2, 0, model_type), rule=rule)
-        self.order.insert(0, order)
-        logger.info(f"Insert order (haihu_id: {order.haihu_id})")
+        create_task(self._produce_order(order))
 
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=0,
                             model=NagaModel(2, 0, model_type), rule=rule)
         create_task(self._produce_report(report))
 
     async def analyze_tenhou(self, haihu_id: str, seat: int,
                              model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> AnalyzeTenhou:
         for o in self.order:
             if o.haihu_id == haihu_id:
                 return AnalyzeTenhou(status=400, msg="すでに解析済みの牌譜です")
 
         order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok, model=NagaModel(2, 0, model_type),
                           rule=NagaGameRule.hanchan)
-        self.order.insert(0, order)
-        logger.info(f"Insert order (haihu_id: {order.haihu_id})")
+        create_task(self._produce_order(order))
 
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=seat,
                             model=NagaModel(2, 0, model_type), rule=NagaGameRule.hanchan)
         create_task(self._produce_report(report))
 
         return AnalyzeTenhou(status=200, msg="")
```

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/naga/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     async def _refresh(self):
         while True:
             observers = self._observers
             self._observers = []
 
             if len(observers) != 0:
-                logger.info("refreshing naga orders and reports...")
+                logger.trace("refreshing naga orders and reports...")
 
                 current = datetime.now(tz=TZ_TOKYO)
                 prev_month = current - monthdelta(months=1)
 
                 list_this_month = await self.api.order_report_list(current.year, current.month)
                 list_prev_month = await self.api.order_report_list(prev_month.year, prev_month.month)
 
@@ -85,14 +85,16 @@
         else:
             self.api = NagaApi(cookies)
 
         self._order_mutex = Lock()
         self._majsoul_order_mutex = Lock()
         self._tenhou_order_mutex = Lock()
 
+        self._last_majsoul_haihu_id = None
+
         self._order_report = ObservableOrderReport(self.api)
         self.timeout = timeout
 
     async def close(self):
         await self.api.close()
 
     async def _get_report(self, haihu_id: str) -> NagaReport:
@@ -128,25 +130,51 @@
                             rule: NagaGameRule,
                             model_type: Union[NagaHanchanModelType,
                                               NagaTonpuuModelType]) -> NagaOrder:
         async with self._order_mutex:
             current = datetime.now(tz=TZ_TOKYO)
             await self.api.analyze_custom(data, 0, rule, model_type)
 
-            res = await self.api.order_report_list(current.year, current.month)
-            if len(res.order) == 0:
-                raise OrderError('order failed')
-
-            order = res.order[0]
-            # order.haihu_id: custom_haihu_2023-05-25T23:46:07_QRIGFOKmA4HT4CJF
-            order_time = datetime.fromisoformat(order.haihu_id[13:32]).replace(tzinfo=TZ_TOKYO)
-            if abs(current.timestamp() - order_time.timestamp()) >= 30:  # 时间差超过了30s
-                raise OrderError('order failed')
+            order_fut = asyncio.get_running_loop().create_future()
+            retry = 0  # 下单完马上获取order的话，有时候order刷新不出来，可以多试几次
+
+            def _make_callback():
+                async def callback(order_report: OrderReportList):
+                    nonlocal retry
+
+                    try:
+                        if len(order_report.order) == 0:
+                            raise OrderError('order failed')
+
+                        order = order_report.order[0]
+
+                        if order.haihu_id == self._last_majsoul_haihu_id:
+                            raise OrderError('order failed')
+
+                        # order.haihu_id: custom_haihu_2023-05-25T23:46:07_QRIGFOKmA4HT4CJF
+                        order_time = datetime.fromisoformat(order.haihu_id[13:32]).replace(tzinfo=TZ_TOKYO)
+                        if abs(current.timestamp() - order_time.timestamp()) >= 30:  # 时间差超过了30s
+                            raise OrderError('order failed')
+
+                        self._last_majsoul_haihu_id = order.haihu_id
+                        order_fut.set_result(order)
+                    except OrderError as e:
+                        if retry < 5:
+                            self._order_report.observe_once(_make_callback())
+                            retry += 1
+                        else:
+                            order_fut.set_exception(e)
+                    except BaseException as e:
+                        order_fut.set_exception(e)
+
+                return callback
 
-            return order
+            self._order_report.observe_once(_make_callback())
+
+            return await order_fut
 
     async def analyze_majsoul(self, majsoul_uuid: str, kyoku: int, honba: int,
                               customer_id: int,
                               *,
                               model_type: Union[NagaHanchanModelType,
                                                 NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
         sess = get_session()
@@ -179,17 +207,18 @@
             if order_orm is not None:
                 if order_orm.order.status == NagaOrderStatus.ok or \
                         datetime.now(tz=timezone.utc).timestamp() - order_orm.order.update_time.timestamp() < 90:
                     return order_orm.order
                 else:  # 超过90s仍未分析完成则删除重来
                     logger.opt(colors=True).info(f"Delete majsoul paipu <y>{majsoul_uuid} "
                                                  f"(kyoku: {kyoku}, honba: {honba}, "
-                                                 f"model_type: {model_type.name})</y> analyze order "
+                                                 f"model_type: {model_type.name})</y> analyze order: {order_orm.naga_haihu_id}, "
                                                  f"because it takes over 90 seconds and still not done")
                     await sess.delete(order_orm.order)
+                    await sess.delete(order_orm)
                     await sess.commit()
                     return None
 
         # 加锁防止重复下单
         local_order = await _get_local_order()
         if local_order is None:
             async with self._majsoul_order_mutex:
@@ -245,58 +274,54 @@
 
         if local_order is not None:
             # 存在记录
             if local_order.status == NagaOrderStatus.ok:
                 logger.opt(colors=True).info(f"Found a existing majsoul paipu <y>{majsoul_uuid} "
                                              f"(kyoku: {kyoku}, honba: {honba}, "
                                              f"model_type: {model_type.name})</y> "
-                                             "analyze report")
+                                             f"analyze report: {local_order.haihu_id}")
                 report = NagaReport(*json.loads(local_order.naga_report))
                 return NagaServiceOrder(report, 0)
 
+            haihu_id = local_order.naga_haihu_id
             logger.opt(colors=True).info(f"Found a processing majsoul paipu <y>{majsoul_uuid} "
                                          f"(kyoku: {kyoku}, honba: {honba}, "
                                          f"model_type: {model_type.name})</y> "
-                                         "analyze order")
-            haihu_id = local_order.naga_haihu_id
+                                         f"analyze order: {haihu_id}")
 
         assert haihu_id != ""
 
+        logger.opt(colors=True).info(f"Waiting for majsoul paipu <y>{majsoul_uuid} "
+                                     f"(kyoku: {kyoku}, honba: {honba}, "
+                                     f"model_type: {model_type.name})</y> "
+                                     f"analyze report: {haihu_id} ...")
         report = await self._get_report(haihu_id)
 
         if new_order:
             # 需要更新之前创建的NagaOrderOrm
             logger.opt(colors=True).debug(f"Updating majsoul paipu <y>{majsoul_uuid} "
-                                          f"(kyoku: {kyoku}, honba: {honba},"
-                                          f" model_type: {model_type.name})</y> "
-                                          "analyze report...")
+                                          f"(kyoku: {kyoku}, honba: {honba}, "
+                                          f"model_type: {model_type.name})</y> "
+                                          f"analyze report: {haihu_id}...")
             stmt = update(NagaOrderOrm).where(NagaOrderOrm.haihu_id == haihu_id).values(
                 status=NagaOrderStatus.ok, naga_report=json.dumps(report), update_time=datetime.now(timezone.utc)
             )
             await sess.execute(stmt)
             await sess.commit()
 
             return NagaServiceOrder(report, 10)
         else:
             return NagaServiceOrder(report, 0)
 
-    async def _order_tenhou(self, haihu_id: str, seat: int, model_type: NagaHanchanModelType) -> NagaOrder:
+    async def _order_tenhou(self, haihu_id: str, seat: int, model_type: NagaHanchanModelType):
         async with self._order_mutex:
-            current = datetime.now(tz=TZ_TOKYO)
             res = await self.api.analyze_tenhou(haihu_id, seat, model_type)
             if res.status != 200:
                 raise OrderError(res.msg)
 
-            res = await self.api.order_report_list(current.year, current.month)
-            for o in res.order:
-                if o.haihu_id == haihu_id:
-                    return o
-
-            raise OrderError("order failed")
-
     # needs test
     async def analyze_tenhou(self, haihu_id: str, seat: int, customer_id: int,
                              *,
                              model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> NagaServiceOrder:
         sess = get_session()
 
         new_order = False
@@ -324,15 +349,15 @@
             async with self._tenhou_order_mutex:
                 local_order = await _get_local_order()
                 if local_order is None:
                     # 不存在记录，安排解析
                     logger.opt(colors=True).info(f"Ordering tenhou paipu <y>{haihu_id} "
                                                  f"(model_type: {model_type.name})</y> analyze...")
 
-                    order = await self._order_tenhou(haihu_id, seat, model_type)
+                    await self._order_tenhou(haihu_id, seat, model_type)
 
                     new_order = True
 
                     order_orm = NagaOrderOrm(haihu_id=haihu_id,
                                              customer_id=customer_id,
                                              cost_np=50,
                                              source=NagaOrderSource.tenhou,
@@ -353,14 +378,17 @@
                 report = NagaReport(*json.loads(local_order.naga_report))
                 return NagaServiceOrder(report, 0)
 
             logger.opt(colors=True).info(f"Found a processing tenhou paipu <y>{haihu_id} "
                                          f"(model_type: {model_type.name})</y> "
                                          "analyze order")
 
+        logger.opt(colors=True).info(f"Waiting for tenhou paipu <y>{haihu_id} "
+                                     f"(model_type: {model_type.name})</y> "
+                                     f"analyze report...")
         report = await self._get_report(haihu_id)
 
         if new_order:
             # 需要更新之前创建的NagaOrderOrm
             logger.opt(colors=True).debug(f"Updating tenhou paipu <y>{haihu_id} "
                                           f"(model_type: {model_type.name})</y> "
                                           "analyze report...")
@@ -377,15 +405,16 @@
     async def statistic(self, year: int, month: int) -> List[NagaServiceUserStatistic]:
         sess = get_session()
 
         t_begin = datetime(year, month, 1)
         t_end = datetime(year, month, 1) + monthdelta(months=1)
 
         stmt = select(NagaOrderOrm).where(NagaOrderOrm.create_time >= t_begin,
-                                          NagaOrderOrm.create_time < t_end)
+                                          NagaOrderOrm.create_time < t_end,
+                                          NagaOrderOrm.status == NagaOrderStatus.ok)
 
         orders = (await sess.execute(stmt)).scalars()
 
         statistic = {}
 
         for order in orders:
             if order.customer_id not in statistic:
```

### Comparing `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.1.4/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/pyproject.toml` & `nonebot_plugin_nagabus-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.1.3/README.md` & `nonebot_plugin_nagabus-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.3/PKG-INFO` & `nonebot_plugin_nagabus-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

