# Comparing `tmp/django-data-schema-2.0.0.tar.gz` & `tmp/django_data_schema-2.0.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-schema-2.0.0.tar", last modified: Tue Jan 24 20:04:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

