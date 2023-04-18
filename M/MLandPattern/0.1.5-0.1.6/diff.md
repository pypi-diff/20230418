# Comparing `tmp/MLandPattern-0.1.5.tar.gz` & `tmp/MLandPattern-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.1.5.tar", last modified: Mon Apr 17 08:32:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

