# Comparing `tmp/plotarchive-0.0.5.tar.gz` & `tmp/plotarchive-0.0.9-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plotarchive-0.0.5.tar", last modified: Tue Sep 15 23:20:39 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

