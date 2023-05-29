# Comparing `tmp/mask_util-0.0.9.tar.gz` & `tmp/mask_util-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mask_util-0.0.9.tar", last modified: Mon May 29 08:25:13 2023, max compression
+gzip compressed data, was "dist\mask_util-0.1.0.tar", last modified: Mon May 29 09:52:04 2023, max compression
```

## Comparing `mask_util-0.0.9.tar` & `mask_util-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 08:25:13.293283 mask_util-0.0.9/
--rw-rw-rw-   0        0        0      271 2023-05-29 08:25:13.292286 mask_util-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 08:25:13.281335 mask_util-0.0.9/mask_util/
--rw-rw-rw-   0        0        0       32 2023-05-29 05:04:13.000000 mask_util-0.0.9/mask_util/__init__.py
--rw-rw-rw-   0        0        0      313 2023-05-29 08:09:38.000000 mask_util-0.0.9/mask_util/const.py
--rw-rw-rw-   0        0        0      762 2023-05-29 08:24:56.000000 mask_util-0.0.9/mask_util/mask.py
--rw-rw-rw-   0        0        0      315 2023-05-29 02:55:36.000000 mask_util-0.0.9/mask_util/replacer.py
-drwxrwxrwx   0        0        0        0 2023-05-29 08:25:13.291319 mask_util-0.0.9/mask_util.egg-info/
--rw-rw-rw-   0        0        0      271 2023-05-29 08:25:13.000000 mask_util-0.0.9/mask_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-29 08:25:13.000000 mask_util-0.0.9/mask_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 08:25:13.000000 mask_util-0.0.9/mask_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 08:25:13.000000 mask_util-0.0.9/mask_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 08:25:13.293283 mask_util-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-05-29 08:25:08.000000 mask_util-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:52:04.595611 mask_util-0.1.0/
+-rw-rw-rw-   0        0        0      271 2023-05-29 09:52:04.595611 mask_util-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 09:52:04.582646 mask_util-0.1.0/mask_util/
+-rw-rw-rw-   0        0        0       32 2023-05-29 05:04:13.000000 mask_util-0.1.0/mask_util/__init__.py
+-rw-rw-rw-   0        0        0      313 2023-05-29 08:09:38.000000 mask_util-0.1.0/mask_util/const.py
+-rw-rw-rw-   0        0        0      805 2023-05-29 09:49:54.000000 mask_util-0.1.0/mask_util/mask.py
+-rw-rw-rw-   0        0        0      358 2023-05-29 09:49:54.000000 mask_util-0.1.0/mask_util/replacer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:52:04.594615 mask_util-0.1.0/mask_util.egg-info/
+-rw-rw-rw-   0        0        0      271 2023-05-29 09:52:04.000000 mask_util-0.1.0/mask_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-29 09:52:04.000000 mask_util-0.1.0/mask_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 09:52:04.000000 mask_util-0.1.0/mask_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 09:52:04.000000 mask_util-0.1.0/mask_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 09:52:04.596608 mask_util-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      439 2023-05-29 09:52:01.000000 mask_util-0.1.0/setup.py
```

### Comparing `mask_util-0.0.9/mask_util/mask.py` & `mask_util-0.1.0/mask_util/mask.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,11 +15,11 @@
             }
     :param input: need to desensitize text
     :return: Desensitized text
     """
     replacement: str = "***"
     replacer = Replacer(replacement)
     masked_input: str = input
-    for keyword in KEYWORDS:
-        pattern = r"([\"']?" + keyword + "[\"']?\s*[,:]\s*[\"']?|" + keyword + "\s*=\s*[\"']?)([^\"']*)([\"']?)"
-        masked_input = re.sub(pattern, replacer.replacement, masked_input)
+    keyword_reg = '|'.join(r'\b' + keyword + r'\b' for keyword in KEYWORDS)
+    pattern = r"(([\"']?)(" + keyword_reg + r")(\2?)\s*[,:]\s*|(" + keyword_reg + r")\s*=\s*)([\"']?)(\w+)(\4?)"
+    masked_input = re.sub(pattern, replacer.replacement, masked_input)
     return masked_input
```

