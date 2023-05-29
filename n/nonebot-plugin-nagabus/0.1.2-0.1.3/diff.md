# Comparing `tmp/nonebot_plugin_nagabus-0.1.2.tar.gz` & `tmp/nonebot_plugin_nagabus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.2.tar` & `nonebot_plugin_nagabus-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.2/LICENSE
--rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0     5604 2023-05-28 14:45:03.123992 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3002 2023-05-27 02:36:44.852322 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    17472 2023-05-28 01:09:03.118081 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      677 2023-05-28 14:46:51.725082 nonebot_plugin_nagabus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.2/README.md
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3002 2023-05-27 02:36:44.852322 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    17472 2023-05-29 01:34:37.295704 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      677 2023-05-29 02:07:41.819768 nonebot_plugin_nagabus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.3/README.md
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.2/LICENSE` & `nonebot_plugin_nagabus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/errors.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/errors.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         else:
             raise e
     except InvalidKyokuHonbaError as e:
         await token.retire()
         kyoku_honba = []
         for kyoku, honba in e.available_kyoku_honba:
             if kyoku <= 3:
-                kyoku_honba.append(f"东{kyoku}局{honba}本场")
+                kyoku_honba.append(f"东{kyoku + 1}局{honba}本场")
             elif kyoku <= 7:
                 kyoku_honba.append(f"南{kyoku - 3}局{honba}本场")
             else:
                 kyoku_honba.append(f"西{kyoku - 7}局{honba}本场")
 
         raise BadRequestError(f"请输入正确的场次与本场（{'、'.join(kyoku_honba)}）") from e
     except UnsupportedGameError as e:
@@ -97,41 +97,37 @@
     if "maj-soul" in args[0]:
         mat = uuid_reg.search(args[0])
         if not mat:
             raise BadRequestError("不正确的雀魂牌谱")
 
         uuid = mat.group(0)
 
-        if len(args) < 2:
-            raise BadRequestError("请指定场次与本场")
-
         kyoku = None
         honba = None
 
-        mat = kyoku_honba_reg.search(args[1])
-        if not mat:
-            raise BadRequestError("请输入正确的场次与本场")
-
-        raw_wind, raw_kyoku, raw_honba = mat.groups()
-
-        try:
-            kyoku = decode_integer(raw_kyoku) - 1
-            if raw_wind == '南':
-                kyoku += 4
-            elif raw_wind == '西':
-                kyoku += 8
-
-            honba = decode_integer(raw_honba)
-        except ValueError:
-            pass
+        if len(args) >= 2:
+            mat = kyoku_honba_reg.search(args[1])
+            if mat:
+                raw_wind, raw_kyoku, raw_honba = mat.groups()
+
+                try:
+                    kyoku = decode_integer(raw_kyoku) - 1
+                    if raw_wind == '南':
+                        kyoku += 4
+                    elif raw_wind == '西':
+                        kyoku += 8
+
+                    honba = decode_integer(raw_honba)
+                except ValueError:
+                    pass
 
         if kyoku is None or honba is None:
-            raise BadRequestError("请输入正确的场次与本场")
-
-        await analyze_majsoul(bot, event, matcher, uuid, kyoku, honba)
+            await analyze_majsoul(bot, event, matcher, uuid, -1, -1)  # 让其发送该局的场次本场信息
+        else:
+            await analyze_majsoul(bot, event, matcher, uuid, kyoku, honba)
     elif "tenhou" in args[0]:
         tenhou_url = args[0].strip()
 
         _, _, _, _, tenhou_query, _ = urlparse(tenhou_url)
         tenhou_query = parse_qs(tenhou_query)
 
         haihu_id = tenhou_query["log"][0]
```

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/naga/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
 
                     order = await self._order_tenhou(haihu_id, seat, model_type)
 
                     new_order = True
 
                     order_orm = NagaOrderOrm(haihu_id=haihu_id,
                                              customer_id=customer_id,
-                                             cost_np=10,
+                                             cost_np=50,
                                              source=NagaOrderSource.tenhou,
                                              model_type=model_type.value,
                                              status=NagaOrderStatus.analyzing,
                                              create_time=datetime.now(tz=timezone.utc),
                                              update_time=datetime.now(tz=timezone.utc))
 
                     sess.add(order_orm)
```

### Comparing `nonebot_plugin_nagabus-0.1.2/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.1.3/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/pyproject.toml` & `nonebot_plugin_nagabus-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.1.2/README.md` & `nonebot_plugin_nagabus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.2/PKG-INFO` & `nonebot_plugin_nagabus-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

