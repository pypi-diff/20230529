# Comparing `tmp/rampedpyrox-1.0.3.tar.gz` & `tmp/rampedpyrox-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rampedpyrox-1.0.3.tar", last modified: Sat Jul 25 17:40:48 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

