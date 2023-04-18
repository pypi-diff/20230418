# Comparing `tmp/rapid_pe-0.0.7.dev20230417.tar.gz` & `tmp/rapid_pe-0.0.7.dev20230418-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapid_pe-0.0.7.dev20230417.tar", last modified: Mon Apr 17 05:03:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

