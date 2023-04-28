# Comparing `tmp/dcona-0.1.1.tar.gz` & `tmp/dcona-0.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcona-0.1.1.tar", last modified: Thu Nov 24 10:27:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

