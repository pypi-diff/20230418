# Comparing `tmp/ta-cmi-1.4.0.tar.gz` & `tmp/ta_cmi-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ta-cmi-1.4.0.tar", last modified: Wed Jan 25 18:18:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

