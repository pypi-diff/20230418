# Comparing `tmp/xlibs-0.0.1.tar.gz` & `tmp/xlibs-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlibs-0.0.1.tar", last modified: Tue Apr 18 09:11:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

