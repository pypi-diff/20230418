# Comparing `tmp/Video_Audio_Image_Downloader-0.0.5.tar.gz` & `tmp/Video_Audio_Image_Downloader-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Video_Audio_Image_Downloader-0.0.5.tar", last modified: Tue Apr 18 11:12:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

