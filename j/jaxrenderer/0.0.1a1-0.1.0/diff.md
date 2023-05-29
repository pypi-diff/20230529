# Comparing `tmp/jaxrenderer-0.0.1a1.tar.gz` & `tmp/jaxrenderer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.0.1a1.tar", max compression
+gzip compressed data, was "jaxrenderer-0.1.0.tar", max compression
```

## Comparing `jaxrenderer-0.0.1a1.tar` & `jaxrenderer-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11367 2023-05-29 20:23:14.475905 jaxrenderer-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     1700 2023-05-29 20:23:14.476068 jaxrenderer-0.0.1a1/README.md
--rw-r--r--   0        0        0     1548 2023-05-29 20:27:31.205614 jaxrenderer-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-05-29 20:23:14.478847 jaxrenderer-0.0.1a1/renderer/README.md
--rw-r--r--   0        0        0      360 2023-05-29 20:23:14.478997 jaxrenderer-0.0.1a1/renderer/__init__.py
--rw-r--r--   0        0        0    30966 2023-05-29 20:23:14.479269 jaxrenderer-0.0.1a1/renderer/geometry.py
--rw-r--r--   0        0        0     9697 2023-05-29 20:23:14.479503 jaxrenderer-0.0.1a1/renderer/model.py
--rw-r--r--   0        0        0    11913 2023-05-29 20:23:14.479847 jaxrenderer-0.0.1a1/renderer/pipeline.py
--rw-r--r--   0        0        0    15537 2023-05-29 20:23:14.480231 jaxrenderer-0.0.1a1/renderer/renderer.py
--rw-r--r--   0        0        0     8615 2023-05-29 20:23:14.480486 jaxrenderer-0.0.1a1/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-05-29 20:23:14.480746 jaxrenderer-0.0.1a1/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-05-29 20:23:14.481002 jaxrenderer-0.0.1a1/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-05-29 20:23:14.481169 jaxrenderer-0.0.1a1/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-05-29 20:23:14.481333 jaxrenderer-0.0.1a1/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-05-29 20:23:14.481641 jaxrenderer-0.0.1a1/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-05-29 20:23:14.481831 jaxrenderer-0.0.1a1/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-05-29 20:23:14.482024 jaxrenderer-0.0.1a1/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-05-29 20:23:14.482213 jaxrenderer-0.0.1a1/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-05-29 20:23:14.482541 jaxrenderer-0.0.1a1/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-05-29 20:23:14.482768 jaxrenderer-0.0.1a1/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-05-29 20:23:14.483220 jaxrenderer-0.0.1a1/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-05-29 20:23:14.483502 jaxrenderer-0.0.1a1/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-05-29 20:23:14.483660 jaxrenderer-0.0.1a1/renderer/types.py
--rw-r--r--   0        0        0     2531 2023-05-29 20:23:14.483829 jaxrenderer-0.0.1a1/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-05-29 20:23:14.483963 jaxrenderer-0.0.1a1/renderer/value_checker.py
--rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 jaxrenderer-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-05-29 20:54:00.387848 jaxrenderer-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1700 2023-05-29 20:54:00.387848 jaxrenderer-0.1.0/README.md
+-rw-r--r--   0        0        0     1541 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/README.md
+-rw-r--r--   0        0        0      360 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/__init__.py
+-rw-r--r--   0        0        0    30966 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/geometry.py
+-rw-r--r--   0        0        0     9697 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/model.py
+-rw-r--r--   0        0        0    11913 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/pipeline.py
+-rw-r--r--   0        0        0    15537 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/renderer.py
+-rw-r--r--   0        0        0     8615 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/types.py
+-rw-r--r--   0        0        0     2531 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-05-29 20:54:00.391848 jaxrenderer-0.1.0/renderer/value_checker.py
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 jaxrenderer-0.1.0/PKG-INFO
```

### Comparing `jaxrenderer-0.0.1a1/LICENSE` & `jaxrenderer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/README.md` & `jaxrenderer-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/pyproject.toml` & `jaxrenderer-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.0.1-alpha1"
+version = "0.1.0"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
```

### Comparing `jaxrenderer-0.0.1a1/renderer/README.md` & `jaxrenderer-0.1.0/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/geometry.py` & `jaxrenderer-0.1.0/renderer/geometry.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/model.py` & `jaxrenderer-0.1.0/renderer/model.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/pipeline.py` & `jaxrenderer-0.1.0/renderer/pipeline.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/renderer.py` & `jaxrenderer-0.1.0/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/scene.py` & `jaxrenderer-0.1.0/renderer/scene.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shader.py` & `jaxrenderer-0.1.0/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/README.md` & `jaxrenderer-0.1.0/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/depth.py` & `jaxrenderer-0.1.0/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/gouraud.py` & `jaxrenderer-0.1.0/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.1.0/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/phong.py` & `jaxrenderer-0.1.0/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.1.0/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.1.0/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.1.0/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shadow.py` & `jaxrenderer-0.1.0/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shapes/capsule.py` & `jaxrenderer-0.1.0/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/shapes/cube.py` & `jaxrenderer-0.1.0/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/types.py` & `jaxrenderer-0.1.0/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/utils.py` & `jaxrenderer-0.1.0/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/renderer/value_checker.py` & `jaxrenderer-0.1.0/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.0.1a1/PKG-INFO` & `jaxrenderer-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.0.1a1
+Version: 0.1.0
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

