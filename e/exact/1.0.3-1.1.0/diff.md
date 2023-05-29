# Comparing `tmp/exact-1.0.3.tar.gz` & `tmp/exact-1.1.0-py3-none-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exact-1.0.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

