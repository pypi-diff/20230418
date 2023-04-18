# Comparing `tmp/django-letsmaintain-1.0.2.tar.gz` & `tmp/django_letsmaintain-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-letsmaintain-1.0.2.tar", last modified: Wed Dec 29 16:35:19 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

