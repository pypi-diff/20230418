# Comparing `tmp/deride-0.1.tar.gz` & `tmp/deride-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deride-0.1.tar", last modified: Sat Nov  5 06:48:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

