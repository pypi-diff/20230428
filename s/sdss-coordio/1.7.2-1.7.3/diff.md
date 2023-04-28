# Comparing `tmp/sdss-coordio-1.7.2.tar.gz` & `tmp/sdss_coordio-1.7.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-coordio-1.7.2.tar", last modified: Thu Apr 27 15:39:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

