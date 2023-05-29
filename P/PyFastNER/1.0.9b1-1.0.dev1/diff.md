# Comparing `tmp/PyFastNER-1.0.9b1.tar.gz` & `tmp/PyFastNER-1.0.dev1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFastNER-1.0.9b1.tar", last modified: Mon May 29 03:26:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

