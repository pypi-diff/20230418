# Comparing `tmp/flask-moreshell-0.0.1.tar.gz` & `tmp/flask_moreshell-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-moreshell-0.0.1.tar", last modified: Tue Feb 28 12:35:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

