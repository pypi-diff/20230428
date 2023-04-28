# Comparing `tmp/nabPy-0.1.64.tar.gz` & `tmp/nabPy-0.1.65-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nabPy-0.1.64.tar", last modified: Wed Sep  7 21:04:39 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

