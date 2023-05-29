# Comparing `tmp/aalink-0.0.3.tar.gz` & `tmp/aalink-0.0.4-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aalink-0.0.3.tar", last modified: Sun May 28 14:28:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

