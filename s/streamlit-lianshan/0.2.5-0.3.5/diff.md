# Comparing `tmp/streamlit_lianshan-0.2.5.tar.gz` & `tmp/streamlit_lianshan-0.3.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_lianshan-0.2.5.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

