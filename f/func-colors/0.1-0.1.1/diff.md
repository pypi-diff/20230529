# Comparing `tmp/func_colors-0.1.tar.gz` & `tmp/func_colors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_colors-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "func_colors-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `func_colors-0.1.tar` & `func_colors-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-05-29 01:13:16.866088 func_colors-0.1/LICENSE
--rw-r--r--   0        0        0      177 2023-05-29 01:13:16.866088 func_colors-0.1/func_colors/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-29 01:13:16.866088 func_colors-0.1/func_colors/colors.py
--rw-r--r--   0        0        0      323 2023-05-29 01:23:04.065695 func_colors-0.1/pyproject.toml
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 func_colors-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-29 01:13:16.866088 func_colors-0.1.1/LICENSE
+-rw-r--r--   0        0        0      179 2023-05-29 01:57:08.076941 func_colors-0.1.1/func_colors/__init__.py
+-rw-r--r--   0        0        0     2297 2023-05-29 01:55:07.549703 func_colors-0.1.1/func_colors/colors.py
+-rw-r--r--   0        0        0      323 2023-05-29 01:23:04.065695 func_colors-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 func_colors-0.1.1/PKG-INFO
```

### Comparing `func_colors-0.1/LICENSE` & `func_colors-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `func_colors-0.1/func_colors/colors.py` & `func_colors-0.1.1/func_colors/colors.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         if depth == 0:
             result += Code.reset.code
 
         return result
 
     def __repr__(self):
-        return f"<ColoredString color={self.color} values={self.values}>"
+        return self.__str__().__repr__()
 
     def __add__(self, other):
         return str(self) + str(other)
 
     def __radd__(self, other):
         return str(other) + str(self)
```

