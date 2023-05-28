# Comparing `tmp/edaplore-0.2.3.tar.gz` & `tmp/edaplore-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edaplore-0.2.3.tar", last modified: Sun May 28 19:47:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

