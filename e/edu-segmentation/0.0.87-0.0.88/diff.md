# Comparing `tmp/edu_segmentation-0.0.87.tar.gz` & `tmp/edu_segmentation-0.0.88-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.87.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

