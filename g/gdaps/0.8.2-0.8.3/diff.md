# Comparing `tmp/gdaps-0.8.2.tar.gz` & `tmp/gdaps-0.8.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdaps-0.8.2.tar", last modified: Sun Mar 26 17:34:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

