# Comparing `tmp/cdktf-cdktf-provider-opc-3.0.0.tar.gz` & `tmp/cdktf_cdktf_provider_opc-4.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-opc-3.0.0.tar", last modified: Tue Jan 17 14:52:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

