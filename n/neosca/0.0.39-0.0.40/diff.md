# Comparing `tmp/neosca-0.0.39.tar.gz` & `tmp/neosca-0.0.40-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosca-0.0.39.tar", last modified: Sat Apr  8 05:11:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

