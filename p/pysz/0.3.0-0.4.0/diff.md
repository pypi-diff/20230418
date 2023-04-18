# Comparing `tmp/pysz-0.3.0.tar.gz` & `tmp/pysz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysz-0.3.0.tar", max compression
+gzip compressed data, was "pysz-0.4.0.tar", max compression
```

## Comparing `pysz-0.3.0.tar` & `pysz-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-04-01 03:14:40.000000 pysz-0.3.0/LICENSE
--rw-r--r--   0        0        0     2335 2023-04-04 05:28:30.000000 pysz-0.3.0/README.md
--rw-r--r--   0        0        0      606 2023-04-04 05:36:11.000000 pysz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      149 2023-04-04 05:33:45.000000 pysz-0.3.0/src/pysz/__init__.py
--rw-r--r--   0        0        0    13652 2023-04-04 05:19:29.000000 pysz-0.3.0/src/pysz/api.py
--rw-r--r--   0        0        0     2505 2023-04-01 13:00:56.000000 pysz-0.3.0/src/pysz/compression.py
--rw-r--r--   0        0        0     1157 2023-04-04 05:43:13.000000 pysz-0.3.0/src/pysz/utils.py
--rw-r--r--   0        0        0     3226 2023-04-04 05:45:53.742149 pysz-0.3.0/setup.py
--rw-r--r--   0        0        0     3061 2023-04-04 05:45:53.742996 pysz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-01 03:14:40.000000 pysz-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6055 2023-04-18 06:25:54.000000 pysz-0.4.0/README.md
+-rw-r--r--   0        0        0      623 2023-04-18 06:05:19.000000 pysz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-04-04 05:33:45.000000 pysz-0.4.0/src/pysz/__init__.py
+-rw-r--r--   0        0        0    13925 2023-04-18 05:40:45.000000 pysz-0.4.0/src/pysz/api.py
+-rw-r--r--   0        0        0     2663 2023-04-04 06:28:13.000000 pysz-0.4.0/src/pysz/compression.py
+-rw-r--r--   0        0        0     1141 2023-04-04 06:01:26.000000 pysz-0.4.0/src/pysz/utils.py
+-rw-r--r--   0        0        0     7143 2023-04-18 06:26:54.487785 pysz-0.4.0/setup.py
+-rw-r--r--   0        0        0     6781 2023-04-18 06:26:54.488679 pysz-0.4.0/PKG-INFO
```

### Comparing `pysz-0.3.0/LICENSE` & `pysz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysz-0.3.0/pyproject.toml` & `pysz-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysz"
-version = "0.3.0"
+version = "0.4.0"
 description = "Package for reading and writing svb-zstd compressed data"
 authors = ["Jinyang Zhang <zhangjinyang@biols.ac.cn>"]
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -12,14 +12,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.2"
 pandas = "^2.0.0"
 zstandard = "^0.20.0"
+#zfpy = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysz-0.3.0/src/pysz/api.py` & `pysz-0.4.0/src/pysz/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 # For dtype conversion
 Dtypes_names = {
     str: "S",
     np.int16: "I16", np.int32: "I32",
     np.uint16: "U16", np.uint32: "U32",
-    np.float16: "F16", np.float32: "F32",
+    np.float16: "F16", np.float32: "F32", np.float64: "F64", np.float128: "F128",
 }
 Dtypes = {j: i for i, j in Dtypes_names.items()}
 
 # Dtypes that can be svb compressed
 Svb_dtypes = [np.int16, np.int32, np.uint16, np.uint32]
 
 
@@ -240,14 +240,15 @@
             if dataset_dtype in Svb_dtypes:
                 d_bstr, d_size, _ = svb_encode(np.array(getattr(record, dataset_id)).astype(dataset_dtype))
             elif dataset_dtype == str:
                 d_bstr = str_encode(dataset_dtype(getattr(record, dataset_id)))
                 d_size = ''
             else:
                 d_bstr = np.array(getattr(record, dataset_id)).astype(dataset_dtype).tobytes()
+                # d_bstr = zfp_encode(np.array(getattr(record, dataset_id)).astype(dataset_dtype))
                 d_size = ''
 
             d_encoded = zstd_encode(d_bstr)
             dat_encoded.append(d_encoded)
             idx_encoded.append(f"{len(d_encoded)}:{d_size}")
 
         # Convert encoded into simple binary format
@@ -345,14 +346,15 @@
                 d_dtype = self.datasets[d_name]
                 if d_dtype in Svb_dtypes:
                     d_decoded = svb_decode(bstr, int(d_shape), dtype=d_dtype)
                 elif d_dtype == str:
                     d_decoded = str_decode(bstr)
                 else:
                     d_decoded = np.frombuffer(bstr, dtype=d_dtype)
+                    # d_decoded = zfp_decode(bstr)
                 datasets.append(d_decoded)
             record = attr + datasets
             reads.append(self.record(*record))
         return reads
 
     def close(self):
         """
@@ -360,7 +362,11 @@
         """
         if self.mode == 'w':
             for _ in np.arange(self.threads):
                 self.q_in.put(None)
             for p in self.pool:
                 p.join()
             self.worker.join()
+        else:
+            if self.fh is not None:
+                self.fh.close()
+
```

### Comparing `pysz-0.3.0/src/pysz/compression.py` & `pysz-0.4.0/src/pysz/compression.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# import zfpy
 import numpy as np
 import streamvbyte
 from zstandard import ZstdDecompressor, ZstdCompressor
 
 
 def str_to_bytes(bytes_or_str):
     """
@@ -101,8 +102,16 @@
     :param data:
     :param size:
     :param dtype:
     :return:
     """
     decoded = np.frombuffer(data, dtype=np.uint8)
     decompressed = streamvbyte.decode(decoded, size, dtype=dtype)
-    return decompressed
+    return decompressed
+
+
+# def zfp_encode(data):
+#     return zfpy.compress_numpy(data)
+
+
+# def zfp_decode(compressed):
+#     return zfpy.decompress_numpy(compressed)
```

### Comparing `pysz-0.3.0/src/pysz/utils.py` & `pysz-0.4.0/src/pysz/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import warnings
 from pathlib import Path
 
 def mkdir(dir_name, overwrite=False):
     dir_path = dir_name if isinstance(dir_name, Path) else Path(dir_name)
     if dir_path.exists():
         if dir_path.is_dir():
             if overwrite is True:
```

