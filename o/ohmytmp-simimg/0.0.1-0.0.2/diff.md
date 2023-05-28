# Comparing `tmp/ohmytmp-simimg-0.0.1.tar.gz` & `tmp/ohmytmp-simimg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-simimg-0.0.1.tar", last modified: Sun May 28 15:16:48 2023, max compression
+gzip compressed data, was "ohmytmp-simimg-0.0.2.tar", last modified: Sun May 28 23:16:19 2023, max compression
```

## Comparing `ohmytmp-simimg-0.0.1.tar` & `ohmytmp-simimg-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 15:16:48.292291 ohmytmp-simimg-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-05-28 15:10:26.000000 ohmytmp-simimg-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1973 2023-05-28 15:16:48.292291 ohmytmp-simimg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-05-28 15:14:55.000000 ohmytmp-simimg-0.0.1/README.md
--rw-rw-rw-   0        0        0      867 2023-05-28 15:16:22.000000 ohmytmp-simimg-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 15:16:48.292291 ohmytmp-simimg-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 15:16:48.277288 ohmytmp-simimg-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:16:48.277288 ohmytmp-simimg-0.0.1/src/ohmytmp_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-28 15:16:48.281287 ohmytmp-simimg-0.0.1/src/ohmytmp_plugins/simimg/
--rw-rw-rw-   0        0        0       61 2023-05-28 15:12:52.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_plugins/simimg/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-05-28 15:11:59.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_plugins/simimg/simimg.py
-drwxrwxrwx   0        0        0        0 2023-05-28 15:16:48.291288 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/
--rw-rw-rw-   0        0        0     1973 2023-05-28 15:16:48.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-28 15:16:48.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 15:16:48.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 15:16:48.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 15:16:48.000000 ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:16:19.198020 ohmytmp-simimg-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 15:10:26.000000 ohmytmp-simimg-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1973 2023-05-28 23:16:19.197501 ohmytmp-simimg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-05-28 15:14:55.000000 ohmytmp-simimg-0.0.2/README.md
+-rw-rw-rw-   0        0        0      867 2023-05-28 23:15:37.000000 ohmytmp-simimg-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:16:19.198543 ohmytmp-simimg-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:16:19.177962 ohmytmp-simimg-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:16:19.177442 ohmytmp-simimg-0.0.2/src/ohmytmp_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:16:19.182688 ohmytmp-simimg-0.0.2/src/ohmytmp_plugins/simimg/
+-rw-rw-rw-   0        0        0       61 2023-05-28 23:15:13.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_plugins/simimg/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-05-28 23:11:46.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_plugins/simimg/simimg.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:16:19.196653 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/
+-rw-rw-rw-   0        0        0     1973 2023-05-28 23:16:19.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-28 23:16:19.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:16:19.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 23:16:19.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-28 23:16:19.000000 ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/top_level.txt
```

### Comparing `ohmytmp-simimg-0.0.1/LICENSE` & `ohmytmp-simimg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-simimg-0.0.1/PKG-INFO` & `ohmytmp-simimg-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-simimg
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin simimg
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

### Comparing `ohmytmp-simimg-0.0.1/pyproject.toml` & `ohmytmp-simimg-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp-simimg"
-version = "0.0.1"
+version = "0.0.2"
 description = "ohmytmp plugin simimg"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["ohmytmp"]
 
 authors = [
```

### Comparing `ohmytmp-simimg-0.0.1/src/ohmytmp_plugins/simimg/simimg.py` & `ohmytmp-simimg-0.0.2/src/ohmytmp_plugins/simimg/simimg.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,50 +66,42 @@
         ans += 1
         d &= d-1
     return ans
 
 
 class SimImg(PluginAfter):
     def __init__(self) -> None:
+        super().__init__()
         self.data = dict()
 
-        def __func(info: Info):
-            if info.TYPE != TYPE.IMAGE:
-                return
-            self.add(info.SRC)
-
-        super().__init__(__func)
-
     def findsim(self, x: int, d: int) -> list:
         return [i for i in self.data if hamming_distance(self.data[i], x) <= d]
 
     def add(self, pth: str) -> None:
         self.data[pth] = phash64(pth)
 
+    def func(self, info: Info) -> None:
+        if info.TYPE != TYPE.IMAGE:
+            return
+        self.add(info.SRC)
+
 
 LSHBIT = 64
 
 
-class SimImgPlus(PluginAfter):
+class SimImgPlus(SimImg):
     def __init__(self, distance: int = 8) -> None:
+        super().__init__()
         if distance < 0 or distance >= LSHBIT:
             raise ValueError(distance)
         self.distance = distance
         self.m = max(distance+1, 4)
         # 4 5 [13 13 13 13 12]
         self.split = list(range(self.m)) * (LSHBIT//self.m + 1)
         self.block = dict()
-        self.data = dict()
-
-        def __func(info: Info):
-            if info.TYPE != TYPE.IMAGE:
-                return
-            self.add(info.SRC)
-
-        super().__init__(__func)
 
     def phash(self, pth: str) -> tuple:
         try:
             img = cv2.imread(pth, cv2.IMREAD_UNCHANGED)
             img = cv2.resize(img, (32, 32), cv2.INTER_AREA)
             img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
         except:
@@ -122,16 +114,13 @@
             w = 0 if j < avg else 1
             ans = ans << 1 | w
             ansl[i % self.m] = (ansl[i % self.m] << 1) | w
         for i, j in enumerate(ansl):
             ansl[i] = ansl[i]*self.m + i
         return ans, ansl
 
-    def findsim(self, x: int, d: int) -> list:
-        return [i[1] for i in self.block if hamming_distance(i[0], x) <= d]
-
     def add(self, pth: str) -> None:
         ans, ansl = self.phash(pth)
         for i in ansl:
             self.block.setdefault(i, list())
             self.block[i].append(pth)
         self.data[pth] = ans
```

### Comparing `ohmytmp-simimg-0.0.1/src/ohmytmp_simimg.egg-info/PKG-INFO` & `ohmytmp-simimg-0.0.2/src/ohmytmp_simimg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp-simimg
-Version: 0.0.1
+Version: 0.0.2
 Summary: ohmytmp plugin simimg
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
```

