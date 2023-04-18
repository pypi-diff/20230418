# Comparing `tmp/scylla-cqlsh-6.0.7.tar.gz` & `tmp/scylla_cqlsh-6.0.8-cp37-cp37m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scylla-cqlsh-6.0.7.tar", last modified: Sun Mar 26 09:50:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

