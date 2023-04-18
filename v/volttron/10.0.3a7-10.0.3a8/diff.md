# Comparing `tmp/volttron-10.0.3a7.tar.gz` & `tmp/volttron-10.0.3a8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron-10.0.3a7.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

