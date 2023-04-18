# Comparing `tmp/yabadaba-0.1.3.tar.gz` & `tmp/yabadaba-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\yabadaba\dist\tmpvy8n3b_j\yabadaba-0.1.3.tar", last modified: Mon Oct  3 13:58:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

