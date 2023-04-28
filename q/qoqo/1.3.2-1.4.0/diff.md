# Comparing `tmp/qoqo-1.3.2.tar.gz` & `tmp/qoqo-1.4.0-cp37-cp37m-macosx_10_7_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

