# Comparing `tmp/processingtools-0.2.8.tar.gz` & `tmp/processingtools-0.2.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/processingtools-0.2.8.tar", last modified: Fri Oct  7 01:20:59 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

