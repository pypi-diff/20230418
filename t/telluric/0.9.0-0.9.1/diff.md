# Comparing `tmp/telluric-0.9.0.tar.gz` & `tmp/telluric-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/telluric-0.9.0.tar", last modified: Wed Dec 12 17:14:20 2018, max compression
+gzip compressed data, was "dist/telluric-0.9.1.tar", last modified: Fri Dec 14 13:51:14 2018, max compression
```

## Comparing `telluric-0.9.0.tar` & `telluric-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-12 17:14:20.000000 telluric-0.9.0/
--rw-rw-r--   0 denis     (1001) denis     (1001)      363 2018-12-12 17:14:20.000000 telluric-0.9.0/setup.cfg
--rw-rw-r--   0 denis     (1001) denis     (1001)     1802 2018-10-01 16:44:05.000000 telluric-0.9.0/README.md
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)      734 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        9 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)     3504 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2018-10-02 08:43:04.000000 telluric-0.9.0/telluric.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       96 2018-12-04 14:22:08.000000 telluric-0.9.0/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     3504 2018-12-12 17:14:20.000000 telluric-0.9.0/PKG-INFO
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric/
--rw-rw-r--   0 denis     (1001) denis     (1001)    10616 2018-12-11 14:27:14.000000 telluric-0.9.0/telluric/vrt.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    20513 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/collections.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3275 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/rasterization.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      300 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5214 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/plotting.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric/util/
--rw-rw-r--   0 denis     (1001) denis     (1001)     2586 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/util/tileserver_utils.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    16516 2018-12-11 14:27:14.000000 telluric-0.9.0/telluric/util/raster_utils.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1540 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/util/projections.py
--rw-rw-r--   0 denis     (1001) denis     (1001)        0 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/util/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2527 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/util/histogram.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      608 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/util/general.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4798 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/util/local_tile_server.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6216 2018-12-11 14:27:14.000000 telluric-0.9.0/telluric/base_vrt.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      497 2018-12-12 17:14:20.000000 telluric-0.9.0/telluric/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      840 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/constants.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    15160 2018-12-12 17:06:13.000000 telluric-0.9.0/telluric/vectors.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    11678 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/features.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    19835 2018-12-04 12:02:36.000000 telluric-0.9.0/telluric/gdalvrt.xsd
--rw-rw-r--   0 denis     (1001) denis     (1001)    81891 2018-12-12 17:06:13.000000 telluric-0.9.0/telluric/georaster.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4845 2018-10-01 16:44:06.000000 telluric-0.9.0/telluric/context.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    68611 2018-10-01 16:44:06.000000 telluric-0.9.0/versioneer.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1067 2018-10-01 16:44:05.000000 telluric-0.9.0/LICENSE
--rwxrwxr-x   0 denis     (1001) denis     (1001)     2239 2018-12-11 14:27:14.000000 telluric-0.9.0/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-14 13:51:14.000000 telluric-0.9.1/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      363 2018-12-14 13:51:14.000000 telluric-0.9.1/setup.cfg
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1802 2018-10-01 16:44:05.000000 telluric-0.9.1/README.md
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      734 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        9 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3504 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2018-10-02 08:43:04.000000 telluric-0.9.1/telluric.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       96 2018-12-04 14:22:08.000000 telluric-0.9.1/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3504 2018-12-14 13:51:14.000000 telluric-0.9.1/PKG-INFO
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric/
+-rw-rw-r--   0 denis     (1001) denis     (1001)    10616 2018-12-11 14:27:14.000000 telluric-0.9.1/telluric/vrt.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    21088 2018-12-14 13:45:37.000000 telluric-0.9.1/telluric/collections.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3275 2018-12-04 12:02:36.000000 telluric-0.9.1/telluric/rasterization.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      300 2018-12-04 12:02:36.000000 telluric-0.9.1/telluric/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5214 2018-12-13 16:41:09.000000 telluric-0.9.1/telluric/plotting.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric/util/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2586 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/util/tileserver_utils.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    16580 2018-12-14 11:56:11.000000 telluric-0.9.1/telluric/util/raster_utils.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1540 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/util/projections.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)        0 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/util/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2527 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/util/histogram.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      608 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/util/general.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4992 2018-12-14 12:01:41.000000 telluric-0.9.1/telluric/util/local_tile_server.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6216 2018-12-11 14:27:14.000000 telluric-0.9.1/telluric/base_vrt.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      497 2018-12-14 13:51:14.000000 telluric-0.9.1/telluric/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      840 2018-12-04 12:02:36.000000 telluric-0.9.1/telluric/constants.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    15160 2018-12-14 11:42:57.000000 telluric-0.9.1/telluric/vectors.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    11678 2018-12-04 12:02:36.000000 telluric-0.9.1/telluric/features.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    19835 2018-12-04 12:02:36.000000 telluric-0.9.1/telluric/gdalvrt.xsd
+-rw-rw-r--   0 denis     (1001) denis     (1001)    82461 2018-12-14 11:56:11.000000 telluric-0.9.1/telluric/georaster.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4845 2018-10-01 16:44:06.000000 telluric-0.9.1/telluric/context.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    68611 2018-10-01 16:44:06.000000 telluric-0.9.1/versioneer.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1067 2018-10-01 16:44:05.000000 telluric-0.9.1/LICENSE
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     2239 2018-12-11 14:27:14.000000 telluric-0.9.1/setup.py
```

### Comparing `telluric-0.9.0/README.md` & `telluric-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric.egg-info/SOURCES.txt` & `telluric-0.9.1/telluric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric.egg-info/PKG-INFO` & `telluric-0.9.1/telluric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: telluric
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interactive geospatial data manipulation in Python
 Home-page: https://github.com/satellogic/telluric/
 Author: Juan Luis Cano, Guy Doulberg, Slava Kerner, Lucio Torre, Ariel Zerahia, Denis Rykov
 Maintainer-email: juanlu@satellogic.com
 License: MIT
-Download-URL: https://github.com/satellogic/telluric/tags/v0.9.0
+Download-URL: https://github.com/satellogic/telluric/tags/v0.9.1
 Description: # telluric
         
         ## Overview
         
         telluric is a Python library to manage vector and raster geospatial data in an interactive
         and easy way.
```

### Comparing `telluric-0.9.0/PKG-INFO` & `telluric-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: telluric
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interactive geospatial data manipulation in Python
 Home-page: https://github.com/satellogic/telluric/
 Author: Juan Luis Cano, Guy Doulberg, Slava Kerner, Lucio Torre, Ariel Zerahia, Denis Rykov
 Maintainer-email: juanlu@satellogic.com
 License: MIT
-Download-URL: https://github.com/satellogic/telluric/tags/v0.9.0
+Download-URL: https://github.com/satellogic/telluric/tags/v0.9.1
 Description: # telluric
         
         ## Overview
         
         telluric is a Python library to manage vector and raster geospatial data in an interactive
         and easy way.
```

### Comparing `telluric-0.9.0/telluric/vrt.py` & `telluric-0.9.1/telluric/vrt.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/collections.py` & `telluric-0.9.1/telluric/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,18 +518,19 @@
         ----------
         filename : str
             Path of the file to read.
         crs : CRS
             overrides the crs of the collection, this funtion will not reprojects
 
         """
-        with fiona.open(filename, 'r') as source:
-            original_crs = CRS(source.crs)
-            schema = source.schema
-            length = len(source)
+        with fiona.Env():
+            with fiona.open(filename, 'r') as source:
+                original_crs = CRS(source.crs)
+                schema = source.schema
+                length = len(source)
         crs = crs or original_crs
         ret_val = cls(filename, crs, schema, length)
         return ret_val
 
     @property
     def crs(self):
         return self._crs
@@ -545,25 +546,41 @@
         with fiona.open(self._filename, 'r') as source:
             for record in source:
                 yield GeoFeature.from_record(record, self.crs, source.schema)
 
     def __getitem__(self, index):
         # See https://github.com/Toblerity/Fiona/issues/327 for discussion
         # about random access in Fiona
+        def adjust(bound):
+            if bound is not None:
+                if bound > 0 and bound > len(self):
+                    bound = len(self)
+                elif bound < 0 and abs(bound) >= len(self):
+                    bound = 0
+            return bound
+
         if isinstance(index, int):
+            if (
+                (index < 0 and abs(index) > len(self)) or
+                (index >= 0 and index >= len(self))
+            ):
+                raise IndexError("collection index out of range")
+
             # We have to convert to positive indices to use islice here, see
             # https://bugs.python.org/issue33040
             index = index % len(self)
             return list(islice(self, index, index + 1))[0]
 
         else:
-            start, stop, step = index.start, index.stop, index.step
+            start, stop, step = adjust(index.start), adjust(index.stop), index.step
 
-            start = start % len(self) if start is not None else None
-            stop = stop % len(self) if stop is not None else None
+            if start is not None and start < 0:
+                start = start % len(self)
+            if stop is not None and stop < 0:
+                stop = stop % len(self)
 
             try:
                 results = list(islice(self, start, stop, step))
 
             except ValueError:
                 # Some value is negative, open the whole file first and then slice
                 # Optimizing this requires some non trivial logic, which essentially means
```

### Comparing `telluric-0.9.0/telluric/rasterization.py` & `telluric-0.9.1/telluric/rasterization.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/plotting.py` & `telluric-0.9.1/telluric/plotting.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/util/tileserver_utils.py` & `telluric-0.9.1/telluric/util/tileserver_utils.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/util/raster_utils.py` & `telluric-0.9.1/telluric/util/raster_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,18 @@
     and guarantees we will have tiled raster and blocksize
     """
     if not(creation_options):
         creation_options = {}
 
     creation_options["blocksize"] = blocksize
     creation_options["tiled"] = True
+    defaults = {"nodata": None, "compress": "lzw"}
     for key in ["nodata", "compress"]:
         if key not in creation_options:
-            creation_options[key] = source_profile.get(key, None)
+            creation_options[key] = source_profile.get(key, defaults.get(key))
     return creation_options
 
 
 def convert_to_cog(source_file, destination_file, resampling=rasterio.enums.Resampling.gauss, blocksize=256,
                    overview_blocksize=256, creation_options=None):
     """Convert source file to a Cloud Optimized GeoTiff new file.
```

### Comparing `telluric-0.9.0/telluric/util/projections.py` & `telluric-0.9.1/telluric/util/projections.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/util/histogram.py` & `telluric-0.9.1/telluric/util/histogram.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/util/general.py` & `telluric-0.9.1/telluric/util/general.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/util/local_tile_server.py` & `telluric-0.9.1/telluric/util/local_tile_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import os
 import folium
 import concurrent.futures
 from threading import Thread, Lock
 from collections import namedtuple
 import tornado.web
 from tornado import gen
 from tornado.ioloop import IOLoop
@@ -107,17 +108,22 @@
 rasters_lock = Lock()
 
 
 class TileServer:
     objects = {}  # type:dict
     running_app = None
 
+    @staticmethod
+    def default_port():
+        return int(os.getenv("TILESERVER_PORT", "4000"))
+
     @classmethod
     def folium_client(cls, obj, bounds, mp=None, capture=None,
-                      base_map_name="Stamen Terrain", port=4000):
+                      base_map_name="Stamen Terrain", port=None):
+        port = port or cls.default_port()
         shape = bounds.get_shape(WGS84_CRS)
         mp = mp or folium.Map(tiles=base_map_name)
 
         folium.raster_layers.TileLayer(
             tiles=cls.server_url(obj, port),
             attr=capture,
             overlay=True
@@ -128,15 +134,16 @@
         return mp
 
     @classmethod
     def server_url(cls, obj, port):
         return "http://localhost:%s/%s/{x}/{y}/{z}.png" % (port, id(obj))
 
     @classmethod
-    def run_tileserver(cls, obj, footprint, resampling=Resampling.nearest, port=4000):
+    def run_tileserver(cls, obj, footprint, resampling=Resampling.nearest, port=None):
+        port = port or cls.default_port()
         cls.add_object(obj, footprint)
         if cls.running_app is None:
             try:
                 cls.running_app = Thread(None, _run_app, args=(cls.objects, resampling, port),
                                          name='TileServer', daemon=True)
                 cls.running_app.start()
                 return cls.running_app
```

### Comparing `telluric-0.9.0/telluric/base_vrt.py` & `telluric-0.9.1/telluric/base_vrt.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/constants.py` & `telluric-0.9.1/telluric/constants.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/vectors.py` & `telluric-0.9.1/telluric/vectors.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/features.py` & `telluric-0.9.1/telluric/features.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/gdalvrt.xsd` & `telluric-0.9.1/telluric/gdalvrt.xsd`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/telluric/georaster.py` & `telluric-0.9.1/telluric/georaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1699,28 +1699,33 @@
         """
         with self._raster_opener(self.source_file) as r:
             return r.overviews(1)
 
     def _overviews_factors(self, blocksize=256):
         return _calc_overviews_factors(self, blocksize=blocksize)
 
-    def save_cloud_optimized(self, dest_url, resampling=Resampling.gauss):
+    def save_cloud_optimized(self, dest_url, resampling=Resampling.gauss, blocksize=256,
+                             overview_blocksize=256, creation_options=None):
         """Save as Cloud Optimized GeoTiff object to a new file.
 
         :param dest_url: path to the new raster
         :param resampling: which Resampling to use on reading, default Resampling.gauss
-
-        :return: new VirtualGeoRaster of the tiled object
+        :param blocksize: the size of the blocks default 256
+        :param overview_blocksize: the block size of the overviews, default 256
+        :param creation_options: dict, options that can override the source raster profile,
+                              notice that you can't override tiled=True, and the blocksize
+                              the list of creation_options can be found here https://www.gdal.org/frmt_gtiff.html
+        :return: new GeoRaster of the tiled object
         """
 
         src = self  # GeoRaster2.open(self._filename)
 
         with tempfile.NamedTemporaryFile(suffix='.tif') as tf:
             src.save(tf.name, overviews=False)
-            convert_to_cog(tf.name, dest_url, resampling)
+            convert_to_cog(tf.name, dest_url, resampling, blocksize, overview_blocksize, creation_options)
 
         geotiff = GeoRaster2.open(dest_url)
         return geotiff
 
     def _get_window_out_shape(self, bands, window, xsize, ysize):
         """Get the outshape of a window.
```

### Comparing `telluric-0.9.0/telluric/context.py` & `telluric-0.9.1/telluric/context.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/versioneer.py` & `telluric-0.9.1/versioneer.py`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/LICENSE` & `telluric-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telluric-0.9.0/setup.py` & `telluric-0.9.1/setup.py`

 * *Files identical despite different names*

