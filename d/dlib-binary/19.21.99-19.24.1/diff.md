# Comparing `tmp/dlib-binary-19.21.99.tar.gz` & `tmp/dlib_binary-19.24.1-cp310-cp310-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlib-binary-19.21.99.tar", last modified: Thu Sep 17 03:02:30 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

