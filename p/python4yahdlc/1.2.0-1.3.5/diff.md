# Comparing `tmp/python4yahdlc-1.2.0.tar.gz` & `tmp/python4yahdlc-1.3.5-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python4yahdlc-1.2.0.tar", last modified: Tue Oct 24 12:07:02 2017, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

