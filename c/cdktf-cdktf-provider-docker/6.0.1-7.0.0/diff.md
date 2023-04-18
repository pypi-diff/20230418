# Comparing `tmp/cdktf-cdktf-provider-docker-6.0.1.tar.gz` & `tmp/cdktf_cdktf_provider_docker-7.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-docker-6.0.1.tar", last modified: Sat Mar 18 03:18:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

