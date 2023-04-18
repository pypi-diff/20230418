# Comparing `tmp/codepiper-0.1.8.tar.gz` & `tmp/codepiper-0.1.9a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codepiper-0.1.8.tar", last modified: Thu Apr 21 16:33:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

