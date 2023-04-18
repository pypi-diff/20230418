# Comparing `tmp/betp-libv-0.1.1.tar.gz` & `tmp/betp_libv-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/betp-libv-0.1.1.tar", last modified: Tue Apr 18 19:46:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

