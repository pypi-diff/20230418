# Comparing `tmp/peakina-0.9.3.tar.gz` & `tmp/peakina-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakina-0.9.3.tar", max compression
+gzip compressed data, was "peakina-0.9.4.tar", max compression
```

## Comparing `peakina-0.9.3.tar` & `peakina-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1510 2023-03-30 15:05:39.576699 peakina-0.9.3/LICENSE
--rw-r--r--   0        0        0     3490 2023-03-30 15:05:39.576699 peakina-0.9.3/README.md
--rw-r--r--   0        0        0      462 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/__init__.py
--rw-r--r--   0        0        0     6598 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/cache.py
--rw-r--r--   0        0        0     1041 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/datapool.py
--rw-r--r--   0        0        0     6778 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/datasource.py
--rw-r--r--   0        0        0     6949 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/helpers.py
--rw-r--r--   0        0        0      344 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/__init__.py
--rw-r--r--   0        0        0     4253 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/fetcher.py
--rw-r--r--   0        0        0        0 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/ftp/__init__.py
--rw-r--r--   0        0        0     1751 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/ftp/ftp_fetcher.py
--rw-r--r--   0        0        0     8033 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/ftp/ftp_utils.py
--rw-r--r--   0        0        0        0 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/http/__init__.py
--rw-r--r--   0        0        0     1369 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/http/http_fetcher.py
--rw-r--r--   0        0        0        0 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/local/__init__.py
--rw-r--r--   0        0        0      378 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/local/file_fetcher.py
--rw-r--r--   0        0        0        0 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/s3/__init__.py
--rw-r--r--   0        0        0     1206 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/s3/s3_fetcher.py
--rw-r--r--   0        0        0     4230 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/io/s3/s3_utils.py
--rw-r--r--   0        0        0        0 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/py.typed
--rw-r--r--   0        0        0      361 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/readers/__init__.py
--rw-r--r--   0        0        0     4107 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/readers/csv.py
--rw-r--r--   0        0        0     1477 2023-03-30 15:05:39.576699 peakina-0.9.3/peakina/readers/excel.py
--rw-r--r--   0        0        0      491 2023-03-30 15:05:39.580699 peakina-0.9.3/peakina/readers/geodata.py
--rw-r--r--   0        0        0     1626 2023-03-30 15:05:39.580699 peakina-0.9.3/peakina/readers/json.py
--rw-r--r--   0        0        0     1435 2023-03-30 15:05:39.580699 peakina-0.9.3/peakina/readers/xml.py
--rw-r--r--   0        0        0     2598 2023-03-30 15:05:39.580699 peakina-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 peakina-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-03 15:38:42.924878 peakina-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3490 2023-04-03 15:38:42.924878 peakina-0.9.4/README.md
+-rw-r--r--   0        0        0      462 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/__init__.py
+-rw-r--r--   0        0        0     6598 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/cache.py
+-rw-r--r--   0        0        0     1041 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/datapool.py
+-rw-r--r--   0        0        0     6778 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/datasource.py
+-rw-r--r--   0        0        0     6949 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/helpers.py
+-rw-r--r--   0        0        0      344 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/__init__.py
+-rw-r--r--   0        0        0     4253 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/ftp_fetcher.py
+-rw-r--r--   0        0        0     8033 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/ftp/ftp_utils.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/http/__init__.py
+-rw-r--r--   0        0        0     1369 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/http/http_fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/local/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/local/file_fetcher.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/__init__.py
+-rw-r--r--   0        0        0     1206 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/s3_fetcher.py
+-rw-r--r--   0        0        0     4478 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/io/s3/s3_utils.py
+-rw-r--r--   0        0        0        0 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/py.typed
+-rw-r--r--   0        0        0      361 2023-04-03 15:38:42.924878 peakina-0.9.4/peakina/readers/__init__.py
+-rw-r--r--   0        0        0     4107 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/csv.py
+-rw-r--r--   0        0        0     1477 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/excel.py
+-rw-r--r--   0        0        0      491 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/geodata.py
+-rw-r--r--   0        0        0     1626 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/json.py
+-rw-r--r--   0        0        0     1435 2023-04-03 15:38:42.928877 peakina-0.9.4/peakina/readers/xml.py
+-rw-r--r--   0        0        0     2598 2023-04-03 15:38:42.928877 peakina-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 peakina-0.9.4/PKG-INFO
```

### Comparing `peakina-0.9.3/LICENSE` & `peakina-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/README.md` & `peakina-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/cache.py` & `peakina-0.9.4/peakina/cache.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/datapool.py` & `peakina-0.9.4/peakina/datapool.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/datasource.py` & `peakina-0.9.4/peakina/datasource.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/helpers.py` & `peakina-0.9.4/peakina/helpers.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/fetcher.py` & `peakina-0.9.4/peakina/io/fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/ftp/ftp_fetcher.py` & `peakina-0.9.4/peakina/io/ftp/ftp_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/ftp/ftp_utils.py` & `peakina-0.9.4/peakina/io/ftp/ftp_utils.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/http/http_fetcher.py` & `peakina-0.9.4/peakina/io/http/http_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/s3/s3_fetcher.py` & `peakina-0.9.4/peakina/io/s3/s3_fetcher.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/io/s3/s3_utils.py` & `peakina-0.9.4/peakina/io/s3/s3_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,22 @@
             # and we give some time to S3 to settle the file status
             sleep(1)
 
 
 def s3_open(url: str, *, client_kwargs: dict[str, Any] | None = None) -> IO[bytes]:
     """opens a s3 url and returns a file-like object"""
     access_key, secret, bucketname, objectname = parse_s3_url(url)
-    fs = s3fs.S3FileSystem(key=access_key, secret=secret, client_kwargs=client_kwargs)
+
+    token = None
+    if client_kwargs is not None and "session_token" in client_kwargs:
+        token = client_kwargs["session_token"]
+        client_kwargs = {k: v for k, v in client_kwargs.items() if k != "session_token"} or None
+
+    fs = s3fs.S3FileSystem(key=access_key, secret=secret, client_kwargs=client_kwargs, token=token)
+
     path = f"{bucketname}/{objectname}"
     ret = tempfile.NamedTemporaryFile(suffix=".s3tmp")
     file = _s3_open_file_with_retries(fs, path, 3)
     ret.write(file.read())
     ret.seek(0)
     file.close()
     return ret
```

### Comparing `peakina-0.9.3/peakina/readers/csv.py` & `peakina-0.9.4/peakina/readers/csv.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/readers/excel.py` & `peakina-0.9.4/peakina/readers/excel.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/readers/json.py` & `peakina-0.9.4/peakina/readers/json.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/peakina/readers/xml.py` & `peakina-0.9.4/peakina/readers/xml.py`

 * *Files identical despite different names*

### Comparing `peakina-0.9.3/pyproject.toml` & `peakina-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peakina"
-version = "0.9.3"
+version = "0.9.4"
 description = "pandas readers on steroids (remote files, glob patterns, cache, etc.)"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 readme = "README.md"
 homepage = "https://github.com/ToucanToco/peakina"
 documentation = "https://toucantoco.github.io/peakina"
 repository = "https://github.com/ToucanToco/peakina"
 license = "BSD-3-Clause"
```

### Comparing `peakina-0.9.3/PKG-INFO` & `peakina-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakina
-Version: 0.9.3
+Version: 0.9.4
 Summary: pandas readers on steroids (remote files, glob patterns, cache, etc.)
 Home-page: https://github.com/ToucanToco/peakina
 License: BSD-3-Clause
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

