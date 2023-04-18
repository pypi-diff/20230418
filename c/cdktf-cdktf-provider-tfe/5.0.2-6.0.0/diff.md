# Comparing `tmp/cdktf-cdktf-provider-tfe-5.0.2.tar.gz` & `tmp/cdktf_cdktf_provider_tfe-6.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-tfe-5.0.2.tar", last modified: Tue Apr  4 07:31:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

