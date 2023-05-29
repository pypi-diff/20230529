# Comparing `tmp/tensoul-0.1.1.tar.gz` & `tmp/tensoul-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensoul-0.1.1.tar", max compression
+gzip compressed data, was "tensoul-0.1.2.tar", max compression
```

## Comparing `tensoul-0.1.1.tar` & `tensoul-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      445 2023-05-25 14:41:30.799701 tensoul-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.1/README.md
--rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.1/tensoul/__init__.py
--rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.1/tensoul/cfg.json
--rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.1/tensoul/cfg.py
--rw-r--r--   0        0        0     2037 2023-05-24 15:36:27.100839 tensoul-0.1.1/tensoul/constants.py
--rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.1/tensoul/downloader.py
--rw-r--r--   0        0        0     9745 2023-05-25 14:38:55.766711 tensoul-0.1.1/tensoul/model.py
--rw-r--r--   0        0        0    14196 2023-05-25 03:22:05.532662 tensoul-0.1.1/tensoul/parser.py
--rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.1/tensoul/utils.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      445 2023-05-29 02:06:44.856253 tensoul-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      944 2023-05-25 04:14:31.440763 tensoul-0.1.2/README.md
+-rw-r--r--   0        0        0       48 2023-05-24 15:43:55.027885 tensoul-0.1.2/tensoul/__init__.py
+-rw-r--r--   0        0        0   168833 2023-05-25 02:49:24.087394 tensoul-0.1.2/tensoul/cfg.json
+-rw-r--r--   0        0        0      163 2023-05-24 15:36:34.423992 tensoul-0.1.2/tensoul/cfg.py
+-rw-r--r--   0        0        0     2377 2023-05-29 02:03:29.081206 tensoul-0.1.2/tensoul/constants.py
+-rw-r--r--   0        0        0     7056 2023-05-25 08:27:21.930832 tensoul-0.1.2/tensoul/downloader.py
+-rw-r--r--   0        0        0    10263 2023-05-29 02:05:05.387320 tensoul-0.1.2/tensoul/model.py
+-rw-r--r--   0        0        0    14218 2023-05-29 01:57:19.665195 tensoul-0.1.2/tensoul/parser.py
+-rw-r--r--   0        0        0      452 2023-05-25 04:10:00.171590 tensoul-0.1.2/tensoul/utils.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 tensoul-0.1.2/PKG-INFO
```

### Comparing `tensoul-0.1.1/README.md` & `tensoul-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.1/tensoul/cfg.json` & `tensoul-0.1.2/tensoul/cfg.json`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.1/tensoul/constants.py` & `tensoul-0.1.2/tensoul/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 # senkinin barai yaku - please don't change, yostar..
 DAISANGEN = 37  # daisangen cfg.fan.fan.map_ index
 DAISUUSHI = 50
 
 TSUMOGIRI = 60  # tenhou tsumogiri symbol
 
 RUNES = {
+    # wind
+    "east": ["東", "East ", "East "],
+    "south": ["南", "South ", "South "],
+    "west": ["西", "West ", "West "],
+    "north": ["北", "North ", "North "],
+    # yaku
+    "bakaze": ["場風", "? ", "? "],
+    "jikaze": ["自風", "? ", "? "],
+    "dabururiichi": ["両立直", "Double Riichi ", "Double Riichi "],
     # hand limits
     "mangan": ["満貫", "Mangan ", "Mangan "],
     "haneman": ["跳満", "Haneman ", "Haneman "],
     "baiman": ["倍満", "Baiman ", "Baiman "],
     "sanbaiman": ["三倍満", "Sanbaiman ", "Sanbaiman "],
     "yakuman": ["役満", "Yakuman ", "Yakuman "],
     "kazoeyakuman": ["数え役満", "Kazoe Yakuman ", "Counted Yakuman "],
```

### Comparing `tensoul-0.1.1/tensoul/downloader.py` & `tensoul-0.1.2/tensoul/downloader.py`

 * *Files identical despite different names*

### Comparing `tensoul-0.1.1/tensoul/model.py` & `tensoul-0.1.2/tensoul/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,17 +251,29 @@
             return AgariPointLevel.mangan
         else:
             return None
 
 
 @dataclass
 class Yaku:
+    WIND = ['east', 'south', 'west', 'north']
+
     id: int
     val: int
 
+    def name(self, round: Round, seat: int) -> str:
+        if self.id == 10:
+            return f"{RUNES['jikaze'][JPNAME]} {RUNES[self.WIND[(seat + round.kyoku) % 4]][JPNAME]}"
+        if self.id == 11:
+            return f"{RUNES['bakaze'][JPNAME]} {RUNES[self.WIND[round.kyoku // 4]][JPNAME]}"
+        elif self.id == 18:
+            return RUNES['dabururiichi'][JPNAME]
+        else:
+            return cfg['fan']['fan']['map_'][str(self.id)]['name_jp']
+
 
 @dataclass
 class SingleAgari:
     seat: int
     ldseat: int  # points from (self if tsumo)
     paoseat: int  # who won or if pao: who's responsible
 
@@ -275,14 +287,15 @@
     delta: list[int]
 
 
 @dataclass
 class Agari:
     agari: list[SingleAgari]
     uras: list[Tile]
+    round: Round
 
     def dump(self) -> Sequence:
         li = [RUNES["agari"][JPNAME]]
 
         for agari in self.agari:
             li.append(pad_list(agari.delta, 4, 0))
 
@@ -321,16 +334,15 @@
                     point = RUNES['kiriagemangan'][JPNAME] + point
                 fuhan = ""
 
             point = fuhan + point
             res.append(point)
 
             for e in agari.yaku:
-                name = cfg['fan']['fan']['map_'][str(e.id)]['name_jp']
-
+                name = e.name(self.round, agari.seat)
                 if agari.yakuman:
                     res.append(f"{name}({RUNES['yakuman'][JPNAME]})")
                 else:
                     res.append(f"{name}({e.val}{RUNES['han'][JPNAME]})")
 
             li.append(res)
```

### Comparing `tensoul-0.1.1/tensoul/parser.py` & `tensoul-0.1.2/tensoul/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,14 @@
 
         # take the longest ura list - double ron with riichi + dama
         for f in log.hules:
             if f.li_doras is not None and len(ura) < len(f.li_doras):
                 ura = [Tile.parse(t) for t in f.li_doras]
             agari.append(self._parse_hu_le(f))
 
-        self.cur.result = Agari(agari=agari, uras=ura)
+        self.cur.result = Agari(agari=agari, uras=ura, round=self.cur.round)
 
         self.kyokus.append(self.cur)
         self.cur = None
 
     def getvalue(self) -> List[Kyoku]:
         return self.kyokus
```

### Comparing `tensoul-0.1.1/PKG-INFO` & `tensoul-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensoul
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

