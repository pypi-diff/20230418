# Comparing `tmp/fabio-2023.4.0.tar.gz` & `tmp/fabio-2023.4.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabio-2023.4.0.tar", last modified: Mon Apr  3 08:08:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

