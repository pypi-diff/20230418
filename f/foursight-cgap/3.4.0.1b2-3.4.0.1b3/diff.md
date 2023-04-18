# Comparing `tmp/foursight_cgap-3.4.0.1b2.tar.gz` & `tmp/foursight_cgap-3.4.0.1b3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.4.0.1b2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

