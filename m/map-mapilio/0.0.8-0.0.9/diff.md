# Comparing `tmp/map-mapilio-0.0.8.tar.gz` & `tmp/map-mapilio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/map-mapilio-0.0.8.tar", last modified: Sat Mar 20 17:21:24 2021, max compression
+gzip compressed data, was "dist/map-mapilio-0.0.9.tar", last modified: Mon Mar 22 14:46:33 2021, max compression
```

## Comparing `map-mapilio-0.0.8.tar` & `map-mapilio-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/map_mapilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-20 17:21:23.000000 map-mapilio-0.0.8/map_mapilio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/map_mapilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-20 17:21:23.000000 map-mapilio-0.0.8/map_mapilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-20 17:21:23.000000 map-mapilio-0.0.8/map_mapilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-20 17:21:23.000000 map-mapilio-0.0.8/map_mapilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/map/
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/geojson.py
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/shape.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/geo_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-20 17:21:10.000000 map-mapilio-0.0.8/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-20 17:21:24.000000 map-mapilio-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map_mapilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/map/
+-rw-r--r--   0 runner    (1001) docker     (121)     5329 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/map/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/map/shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/map/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/map/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-22 14:46:19.000000 map-mapilio-0.0.9/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2021-03-22 14:46:33.000000 map-mapilio-0.0.9/PKG-INFO
```

### Comparing `map-mapilio-0.0.8/setup.py` & `map-mapilio-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `map-mapilio-0.0.8/map/shape.py` & `map-mapilio-0.0.9/map/shape.py`

 * *Files identical despite different names*

### Comparing `map-mapilio-0.0.8/map/base.py` & `map-mapilio-0.0.9/map/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-import json
 import os
 
 from folium import folium, plugins
 from folium.plugins import MeasureControl, Draw
-import map.geo_json as geo
 import folium
+import re
+import ast
 
 
 class Map:
     def __init__(self, **kwargs):
+        """
+
+        Parameters
+        ----------
+        kwargs
+            geojsonData
+        """
         self.__dict__.update(kwargs)
 
         self.map = self._create()
-        self._geojson()
+        self._gps_point_tracer()
 
     def _create(self):
         self.map = folium.Map(location=[41.105645123000002, 28.790535551000001],
                               tiles='http://mt0.google.com/vt/lyrs=y&hl=en&x={x}&y={y}&z={z}&s=Ga', attr="google",
                               max_zoom=25,
                               control_scale=True, zoom_start=16)
 
@@ -40,16 +47,16 @@
         icon = folium.Icon(angle=angle, **kw)
         folium.Marker(location=[36.893651, 30.616686], icon=icon, tooltip=str(angle)).add_to(self.map)
 
         angle = 90
         icon = folium.Icon(angle=angle, **kw)
         folium.Marker([36.893651, 30.616986], icon=icon, tooltip=str(angle)).add_to(self.map)
 
-    def _geojson(self):
-        geojson = json.loads(geo.getData(self.conn, self.config, self.database, self.gui))
+    def _gps_point_tracer(self):
+        geojson = ast.literal_eval(re.search('({.+})', self.geojsonData).group(0)) # because of coming data dict in str
         outlines = folium.FeatureGroup("outlines")
         line_bg = folium.FeatureGroup("lineBg")
         bus_lines = folium.FeatureGroup("busLines")
         bus_stops = folium.FeatureGroup("busStops")
 
         line_weight = 6
         line_colors = ["red", "#08f", "#0c0", "#f80"]
```

