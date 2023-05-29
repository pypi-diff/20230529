# Comparing `tmp/yggdrasil_mc-0.1b3.tar.gz` & `tmp/yggdrasil_mc-0.1b4.tar.gz`

## Comparing `yggdrasil_mc-0.1b3.tar` & `yggdrasil_mc-0.1b4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/requirements.txt
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/example/get_uuid.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/src/yggdrasil_mc/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/src/yggdrasil_mc/model.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/src/yggdrasil_mc/ygg.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/src/yggdrasil_mc/ygg_async.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/LICENSE
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/README.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/pyproject.toml
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b3/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/requirements.txt
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/example/get_uuid.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/src/yggdrasil_mc/__init__.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/src/yggdrasil_mc/model.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/src/yggdrasil_mc/wrapper.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/src/yggdrasil_mc/ygg.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/src/yggdrasil_mc/ygg_async.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/LICENSE
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/README.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 yggdrasil_mc-0.1b4/PKG-INFO
```

### Comparing `yggdrasil_mc-0.1b3/.github/workflows/pypi-publish.yml` & `yggdrasil_mc-0.1b4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `yggdrasil_mc-0.1b3/src/yggdrasil_mc/model.py` & `yggdrasil_mc-0.1b4/src/yggdrasil_mc/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import json
 from base64 import b64decode
 from datetime import date
 from typing import Literal
+from urllib.parse import urlparse
 
 from pydantic import BaseModel, Field, root_validator
 
 
-class YggdrasilPlayerUuidApi(BaseModel):
+class YggdrasilPlayerUuidApiModel(BaseModel):
     id: str | None = None
     name: str | None = None
     existed: bool = True
 
 
-def _make_hash(cls, values):
-    url: str = values["url"]
-    last_slash_location = url.rindex("/")
-    real_hash = url[last_slash_location + 1 :]
-    values["hash"] = real_hash
+def get_hash(cls, values):
+    url = values.get("url")
+    if url:
+        parsed = urlparse(url)
+        # get last path element
+        values["hash"] = parsed.path.split("/")[-1]
     return values
 
 
-class YggdrasilTextures(BaseModel):
-    class _Skin(BaseModel):
-        class MetaData(BaseModel):
-            model: Literal["default", "slim"] = "default"
+class _SkinMetaData(BaseModel):
+    model: Literal["default", "slim"] = "default"
 
-        url: str | None = None
-        hash: str | None = None
-        metadata: MetaData | None = MetaData(model="default")
-        _hash: str | None = None
 
-        root_validator(pre=True, allow_reuse=True)(_make_hash)
+class _Skin(BaseModel):
+    url: str | None = None
+    hash: str | None = None
+    metadata: _SkinMetaData | None = _SkinMetaData(model="default")
+    _get_hash = root_validator(allow_reuse=True)(get_hash)
 
-    class _Cape(BaseModel):
-        url: str | None = None
-        hash: str | None = None
-        _hash: str | None = None
 
-        root_validator(pre=True, allow_reuse=True)(_make_hash)
+class _Cape(BaseModel):
+    url: str | None = None
+    hash: str | None = None
+    _get_hash = root_validator(allow_reuse=True)(get_hash)
 
-    skin: _Skin = Field(default_factory=_Skin, alias="SKIN")
-    cape: _Cape = Field(default_factory=_Cape, alias="CAPE")
 
+class YggdrasilTexturesModel(BaseModel):
+    skin: _Skin = Field(default=_Skin(), alias="SKIN")
+    cape: _Cape = Field(default=_Cape(), alias="CAPE")
 
-class YggdrasilPropertiesTextures(BaseModel):
+
+class YggdrasilPropertiesTexturesModel(BaseModel):
     timestamp: date
     profileId: str
     profileName: str
-    textures: YggdrasilTextures
+    textures: YggdrasilTexturesModel
 
 
-class YggdrasilGameProfileApi(BaseModel):
+class YggdrasilGameProfileApiModel(BaseModel):
     class Properties(BaseModel):
-        textures: YggdrasilPropertiesTextures
+        textures: YggdrasilPropertiesTexturesModel
 
     id: str
     name: str
     properties: Properties  # a bit difference between API
 
     @root_validator(pre=True)
     def pre_processer(cls, values):
```

### Comparing `yggdrasil_mc-0.1b3/.gitignore` & `yggdrasil_mc-0.1b4/.gitignore`

 * *Files identical despite different names*

### Comparing `yggdrasil_mc-0.1b3/LICENSE` & `yggdrasil_mc-0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `yggdrasil_mc-0.1b3/README.md` & `yggdrasil_mc-0.1b4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # yggdrasil-mc
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/jinzhijie/yggdrasil-mc?style=social) ![PyPI](https://img.shields.io/pypi/v/yggdrasil-mc?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yggdrasil-mc?style=flat-square) ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/jinzhijie/yggdrasil-mc/main?style=flat-square) ![GitHub](https://img.shields.io/github/license/jinzhijie/yggdrasil-mc?style=flat-square)
 
-A simple Python lib to get player info and texture from Mojang and Blessing Skin.
+A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs.
 
-一个简单的 Python 库，可从 Mojang 和 Blessing Skin 获取玩家的信息和材质。
+一个简单的 Python 库，可从 Mojang 和 Yggdrasil APIs 获取玩家的信息和材质。
 
 ## Attention
 
 This package can run in **Python 3.10+ ONLY**.
 
 ## Usage
 
 1. Download the package from PyPI
+
     ```bash
     pip3 install -U yggdrasil-mc
     ```
 
-2.  ```python
-    from yggdrasil_mc.ygg import YggdrasilPlayerUuidApi
+2. ```python
+    from yggdrasil_mc import YggPlayerUuid, YggPlayerProfile
 
     player_name = "w84"
-    player = YggdrasilPlayerUuidApi.getMojangServer(player_name)
+    player = YggPlayerUuid().getMojang(player_name)
     if player.existed:
-        print(player.id)
+        print(YggPlayerProfile().getMojang(player.id))
     ```
 
 After you run these snippet, you will get the following output:
+
 ```plain
-ca244462f8e5494791ec98f0ccf505ac
+id='ca244462f8e5494791ec98f0ccf505ac' name='w84' properties=Properties(...
 ```
 
 Note that this package also provide the asyncio version which is powered by aiohttp:
+
 ```python
-from yggdrasil_mc.ygg_async import YggdrasilPlayerUuidApi
+from yggdrasil_mc import YggPlayerUuid, YggPlayerProfile
 
 player_name = "w84"
-
-async get_player_uuid(player_name: str = player_name)
-    player = await YggdrasilPlayerUuidApi.getMojangServer(player_name)
-    return player.id
-```
+player = await YggPlayerUuid().getMojangAsync(player_name)
+if player.existed:
+    print(await YggPlayerProfile().getMojangAsync(player.id))
+```
```

### Comparing `yggdrasil_mc-0.1b3/pyproject.toml` & `yggdrasil_mc-0.1b4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yggdrasil-mc"
-version = "0.1b3"
+version = "0.1b4"
 authors = [
   { name="Xiao_Jin", email="i@xiaojin233.cn" },
 ]
-description = "A simple Python lib to get player info and texture from Mojang and Blessing Skin."
+description = "A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs."
 keywords = ["minecraft", "yggdrasil", "api", "mojang", "blessing skin"]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Natural Language :: Chinese (Simplified)",
     "Natural Language :: English",
@@ -20,14 +20,13 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "Topic :: Games/Entertainment",
     "Topic :: Utilities",
 ]
 dependencies = [
   "pydantic",
-  "aiohttp",
-  "requests",
+  "httpx",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jinzhijie/yggdrasil-mc"
 "Bug Tracker" = "https://github.com/jinzhijie/yggdrasil-mc/issues"
```

### Comparing `yggdrasil_mc-0.1b3/PKG-INFO` & `yggdrasil_mc-0.1b4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 Metadata-Version: 2.1
 Name: yggdrasil-mc
-Version: 0.1b3
-Summary: A simple Python lib to get player info and texture from Mojang and Blessing Skin.
+Version: 0.1b4
+Summary: A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs.
 Project-URL: Homepage, https://github.com/jinzhijie/yggdrasil-mc
 Project-URL: Bug Tracker, https://github.com/jinzhijie/yggdrasil-mc/issues
 Author-email: Xiao_Jin <i@xiaojin233.cn>
 License-File: LICENSE
 Keywords: api,blessing skin,minecraft,mojang,yggdrasil
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
-Requires-Dist: aiohttp
+Requires-Dist: httpx
 Requires-Dist: pydantic
-Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # yggdrasil-mc
 
 ![GitHub Repo stars](https://img.shields.io/github/stars/jinzhijie/yggdrasil-mc?style=social) ![PyPI](https://img.shields.io/pypi/v/yggdrasil-mc?style=flat-square) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/yggdrasil-mc?style=flat-square) ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/jinzhijie/yggdrasil-mc/main?style=flat-square) ![GitHub](https://img.shields.io/github/license/jinzhijie/yggdrasil-mc?style=flat-square)
 
-A simple Python lib to get player info and texture from Mojang and Blessing Skin.
+A simple Python lib to get player info and texture from Mojang and Yggdrasil APIs.
 
-一个简单的 Python 库，可从 Mojang 和 Blessing Skin 获取玩家的信息和材质。
+一个简单的 Python 库，可从 Mojang 和 Yggdrasil APIs 获取玩家的信息和材质。
 
 ## Attention
 
 This package can run in **Python 3.10+ ONLY**.
 
 ## Usage
 
 1. Download the package from PyPI
+
     ```bash
     pip3 install -U yggdrasil-mc
     ```
 
-2.  ```python
-    from yggdrasil_mc.ygg import YggdrasilPlayerUuidApi
+2. ```python
+    from yggdrasil_mc import YggPlayerUuid, YggPlayerProfile
 
     player_name = "w84"
-    player = YggdrasilPlayerUuidApi.getMojangServer(player_name)
+    player = YggPlayerUuid().getMojang(player_name)
     if player.existed:
-        print(player.id)
+        print(YggPlayerProfile().getMojang(player.id))
     ```
 
 After you run these snippet, you will get the following output:
+
 ```plain
-ca244462f8e5494791ec98f0ccf505ac
+id='ca244462f8e5494791ec98f0ccf505ac' name='w84' properties=Properties(...
 ```
 
 Note that this package also provide the asyncio version which is powered by aiohttp:
+
 ```python
-from yggdrasil_mc.ygg_async import YggdrasilPlayerUuidApi
+from yggdrasil_mc import YggPlayerUuid, YggPlayerProfile
 
 player_name = "w84"
-
-async get_player_uuid(player_name: str = player_name)
-    player = await YggdrasilPlayerUuidApi.getMojangServer(player_name)
-    return player.id
-```
+player = await YggPlayerUuid().getMojangAsync(player_name)
+if player.existed:
+    print(await YggPlayerProfile().getMojangAsync(player.id))
+```
```

