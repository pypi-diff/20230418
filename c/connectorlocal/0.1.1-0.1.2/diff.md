# Comparing `tmp/connectorlocal-0.1.1.tar.gz` & `tmp/connectorlocal-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\connectorlocal-0.1.1.tar", last modified: Mon Apr  3 09:14:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

