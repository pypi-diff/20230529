# Comparing `tmp/coverage-7.2.6.tar.gz` & `tmp/coverage-7.2.7-cp37-cp37m-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.2.6.tar", last modified: Wed May 24 01:24:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

