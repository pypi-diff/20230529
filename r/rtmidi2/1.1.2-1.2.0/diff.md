# Comparing `tmp/rtmidi2-1.1.2.tar.gz` & `tmp/rtmidi2-1.2.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtmidi2-1.1.2.tar", last modified: Sun Oct 16 20:31:25 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

