# Comparing `tmp/cliparse-1.0.0b5.tar.gz` & `tmp/cliparse-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cliparse-1.0.0b5.tar", last modified: Thu Nov 12 13:55:37 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

