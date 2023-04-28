# Comparing `tmp/coverage-7.2.3.tar.gz` & `tmp/coverage-7.2.4-cp37-cp37m-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.2.3.tar", last modified: Thu Apr  6 14:06:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

