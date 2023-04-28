# Comparing `tmp/sqlite_sync-0.0.6.tar.gz` & `tmp/sqlite_sync-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_sync-0.0.6.tar", last modified: Fri Apr 28 13:43:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

