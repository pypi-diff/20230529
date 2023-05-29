# Comparing `tmp/pybase62-0.6.0.tar.gz` & `tmp/pybase62-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybase62-0.6.0.tar", last modified: Sun Feb  5 02:28:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

