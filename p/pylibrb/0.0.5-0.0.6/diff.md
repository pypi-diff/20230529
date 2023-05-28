# Comparing `tmp/pylibrb-0.0.5.tar.gz` & `tmp/pylibrb-0.0.6-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.5.tar", last modified: Wed May 24 10:27:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

