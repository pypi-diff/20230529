# Comparing `tmp/indexed_bzip2-1.4.0.tar.gz` & `tmp/indexed_bzip2-1.5.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexed_bzip2-1.4.0.tar", last modified: Sat Nov 12 19:57:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

