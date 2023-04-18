# Comparing `tmp/afscgap-0.0.7.tar.gz` & `tmp/afscgap-0.0.8.tar.gz`

## Comparing `afscgap-0.0.7.tar` & `afscgap-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,31 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-0.0.7/.gitattributes
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-0.0.7/CONDUCT.md
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-0.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-0.0.7/gruntfile.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-0.0.7/install_browser.sh
--rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-0.0.7/package-lock.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.7/package.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-0.0.7/setup.cfg
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/README.md
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/__init__.py
--rw-r--r--   0        0        0    42288 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/client.py
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/cursor.py
--rw-r--r--   0        0        0    35177 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/inference.py
--rw-r--r--   0        0        0    35443 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/py.typed
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/query_util.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 afscgap-0.0.7/afscgap/util.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.7/.gitignore
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-0.0.7/LICENSE.md
--rw-r--r--   0        0        0    36664 2020-02-02 00:00:00.000000 afscgap-0.0.7/README.md
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 afscgap-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    38048 2020-02-02 00:00:00.000000 afscgap-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-0.0.8/.gitattributes
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-0.0.8/CONDUCT.md
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-0.0.8/gruntfile.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-0.0.8/install_browser.sh
+-rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-0.0.8/package-lock.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.8/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-0.0.8/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/README.md
+-rw-r--r--   0        0        0    58952 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/__init__.py
+-rw-r--r--   0        0        0    42875 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/client.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/convert.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/cursor.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/http.py
+-rw-r--r--   0        0        0    36994 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/inference.py
+-rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/query_util.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/typesdef.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/README.md
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/architecture.drawio
+-rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/library.png
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/paper.bib
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/paper.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/preview_paper.sh
+-rw-r--r--   0        0        0   176314 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/viz.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 afscgap-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0    43240 2020-02-02 00:00:00.000000 afscgap-0.0.8/README.md
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 afscgap-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    44624 2020-02-02 00:00:00.000000 afscgap-0.0.8/PKG-INFO
```

### Comparing `afscgap-0.0.7/CONDUCT.md` & `afscgap-0.0.8/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.7/CONTRIBUTING.md` & `afscgap-0.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.7/gruntfile.js` & `afscgap-0.0.8/gruntfile.js`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.7/package-lock.json` & `afscgap-0.0.8/package-lock.json`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.7/afscgap/client.py` & `afscgap-0.0.8/afscgap/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 Logic for making actual HTTP requests and managaing pagination when interfacing
 with the NOAA-run AFSC GAP API.
 
 (c) 2023 Regents of University of California / The Eric and Wendy Schmidt Center
 for Data Science and the Environment at UC Berkeley.
 
 This file is part of afscgap released under the BSD 3-Clause License. See
-LICENSE.txt.
+LICENSE.md.
 """
 import copy
 import json
 import queue
 import typing
 
+import afscgap.convert
 import afscgap.cursor
+import afscgap.http
 import afscgap.model
 import afscgap.query_util
-import afscgap.util
 
-from afscgap.util import OPT_FLOAT
-from afscgap.util import OPT_INT
-from afscgap.util import OPT_REQUESTOR
-from afscgap.util import OPT_STR
+from afscgap.typesdef import OPT_FLOAT
+from afscgap.typesdef import OPT_INT
+from afscgap.typesdef import OPT_REQUESTOR
+from afscgap.typesdef import OPT_STR
 
 DEFAULT_DOMAIN = 'https://apps-st.fisheries.noaa.gov'
 DEFAULT_URL = DEFAULT_DOMAIN + '/ods/foss/afsc_groundfish_survey/'
 
 
 def build_api_cursor(params: dict, limit: OPT_INT = None,
     start_offset: OPT_INT = None, filter_incomplete: bool = False,
@@ -49,15 +50,15 @@
         base_url: The URL at which the API service can be found or None to use
             a default. Defaults to None.
 
     Returns:
         Cursor which iterates over the results from the API service.
     """
     params_safe = copy.deepcopy(params)
-    params_safe['date_time'] = afscgap.util.convert_from_iso8601(
+    params_safe['date_time'] = afscgap.convert.convert_from_iso8601(
         params_safe['date_time']
     )
     params_ords = afscgap.query_util.interpret_query_to_ords(params_safe)
 
     query_url = get_query_url(params_ords, base=base_url)
 
     return ApiServiceCursor(
@@ -121,15 +122,15 @@
         self._queue: queue.Queue[afscgap.model.Record] = queue.Queue()
         self._invalid_queue: queue.Queue[dict] = queue.Queue()
         self._done = False
 
         if requestor:
             self._request_strategy = requestor
         else:
-            self._request_strategy = afscgap.util.build_requestor()
+            self._request_strategy = afscgap.http.build_requestor()
 
         self._next_url = self.get_page_url()
 
     def get_base_url(self) -> str:
         """Get the URL at which the first page of query results can be found.
 
         Returns:
@@ -211,15 +212,15 @@
         Returns:
             Results from the page which, regardless of ignore_invalid, may
             contain a mixture of complete and incomplete records.
         """
         url = self.get_page_url(offset, limit)
 
         result = self._request_strategy(url)
-        afscgap.util.check_result(result)
+        afscgap.http.check_result(result)
 
         result_parsed = result.json()
         items_raw = result_parsed['items']
 
         parsed_maybe = map(try_parse, items_raw)
         parsed_with_none = map(lambda x: x.get_parsed(), parsed_maybe)
 
@@ -288,15 +289,15 @@
         into the waiting queues and updating the next url / done internal
         state in the process.
         """
         if self._done:
             return
 
         result = self._request_strategy(self._next_url)
-        afscgap.util.check_result(result)
+        afscgap.http.check_result(result)
 
         result_parsed = result.json()
 
         items_raw = result_parsed['items']
 
         items_parsed = map(try_parse, items_raw)
 
@@ -550,29 +551,41 @@
         Returns:
             The date and time of the haul which has been attempted to be
             transformed to an ISO 8601 string without timezone info. If it
             couldn’t be transformed, the original string is reported.
         """
         return self._date_time
 
-    def get_latitude_dd(self) -> float:
+    def get_latitude(self, units: str = 'dd') -> float:
         """Get the field labeled as latitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Latitude in decimal degrees associated with the haul.
         """
-        return self._latitude_dd
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_degrees(self._latitude_dd, units)
+        )
 
-    def get_longitude_dd(self) -> float:
+    def get_longitude(self, units: str = 'dd') -> float:
         """Get the field labeled as longitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Longitude in decimal degrees associated with the haul.
         """
-        return self._longitude_dd
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_degrees(self._longitude_dd, units)
+        )
 
     def get_species_code(self) -> float:
         """Get the field labeled as species_code in the API.
 
         Returns:
             Unique ID associated with the species observed.
         """
@@ -601,167 +614,227 @@
 
         Returns:
             Confidence flag regarding ability to identify species (High,
             Moderate, Low). In practice, this can also be Unassessed.
         """
         return self._taxon_confidence
 
-    def get_cpue_kgha_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kgha in the API.
-
-        Returns:
-            Catch weight divided by net area (kg / hectares) if available. See
-            metadata. None if could not interpret as a float.
-        """
-        return self._cpue_kgha
-
-    def get_cpue_kgkm2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kgkm2 in the API.
-
-        Returns:
-            Catch weight divided by net area (kg / km^2) if available. See
-            metadata. None if could not interpret as a float.
-        """
-        return self._cpue_kgkm2
-
-    def get_cpue_kg1000km2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kg1000km2 in the API.
-
-        Returns:
-            Catch weight divided by net area (kg / km^2 * 1000) if available.
-            See metadata. None if could not interpret as a float.
-        """
-        return self._cpue_kg1000km2
+    def get_cpue_weight_maybe(self, units: str = 'kg/ha') -> OPT_FLOAT:
+        """Get a field labeled as cpue_* in the API.
 
-    def get_cpue_noha_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_noha in the API.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Returns:
-            Catch number divided by net sweep area if available (count /
-            hectares). See metadata. None if could not interpret as a float.
+            Catch weight divided by net area (in given units) if available. See
+            metadata. None if could not interpret as a float. If an inferred
+            zero catch record, will be zero.
         """
-        return self._cpue_noha
+        return {
+            'kg/ha': self._cpue_kgha,
+            'kg/km2': self._cpue_kgkm2,
+            'kg1000/km2': self._cpue_kg1000km2
+        }[units]
 
-    def get_cpue_nokm2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_nokm2 in the API.
+    def get_cpue_count_maybe(self, units: str = 'kg/ha') -> OPT_FLOAT:
+        """Get the field labeled as cpue_* in the API.
 
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2).
-            See metadata. None if could not interpret as a float.
-        """
-        return self._cpue_nokm2
+        Get the catch per unit effort from the record with one of the following
+        units: kg/ha, kg/km2, kg1000/km2.
 
-    def get_cpue_no1000km2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_no1000km2 in the API.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
 
         Returns:
-            Catch number divided by net sweep area if available (count / km^2 *
-            1000). See metadata. None if could not interpret as a float.
+            Catch weight divided by net area (in given units) if available. See
+            metadata. None if could not interpret as a float. If an inferred
+            zero catch record, will be zero.
         """
-        return self._cpue_no1000km2
+        return {
+            'count/ha': self._cpue_noha,
+            'count/km2': self._cpue_nokm2,
+            'count1000/km2': self._cpue_no1000km2
+        }[units]
 
-    def get_weight_kg_maybe(self) -> OPT_FLOAT:
+    def get_weight_maybe(self, units: str = 'kg') -> OPT_FLOAT:
         """Get the field labeled as weight_kg in the API.
 
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
+
         Returns:
-            Taxon weight (kg) if available. See metadata. None if could not
-            interpret as a float.
+            Taxon weight if available. See metadata. None if could not
+            interpret as a float. If an inferred zero catch record, will be
+            zero.
         """
-        return self._weight_kg
+        return afscgap.convert.convert_weight(self._weight_kg, units)
 
     def get_count_maybe(self) -> OPT_FLOAT:
         """Get the field labeled as count in the API.
 
         Returns:
             Total number of organism individuals in haul. None if could not
             interpret as a float.
         """
         return self._count
 
-    def get_bottom_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_bottom_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as bottom_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
-            Bottom temperature associated with observation if available in
-            Celsius. None if not given or could not interpret as a float.
+            Bottom temperature associated with observation / inferrence if
+            available in desired units. None if not given or could not interpret
+            as a float.
         """
-        return self._bottom_temperature_c
+        return afscgap.convert.convert_temperature(
+            self._bottom_temperature_c,
+            units
+        )
 
-    def get_surface_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_surface_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as surface_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
-            Surface temperature associated with observation if available in
-            Celsius. None if not given or could not interpret as a float.
+            Surface temperature associated with observation / inferrence if
+            available. None if not given or could not interpret as a float.
         """
-        return self._surface_temperature_c
+        return afscgap.convert.convert_temperature(
+            self._surface_temperature_c,
+            units
+        )
 
-    def get_depth_m(self) -> float:
+    def get_depth(self, units: str = 'm') -> float:
         """Get the field labeled as depth_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Depth of the bottom in meters.
+            Depth of the bottom.
         """
-        return self._depth_m
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_distance(self._depth_m, units)
+        )
 
-    def get_distance_fished_km(self) -> float:
+    def get_distance_fished(self, units: str = 'm') -> float:
         """Get the field labeled as distance_fished_km in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as km.
+            Distance of the net fished.
         """
-        return self._distance_fished_km
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_distance(
+                self._distance_fished_km * 1000,
+                units
+            )
+        )
 
-    def get_net_width_m_maybe(self) -> OPT_FLOAT:
+    def get_net_width_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m or None if not given.
+            Distance of the net fished or None if not given.
         """
-        return self._net_width_m
+        return afscgap.convert.convert_distance(
+            self._net_width_m,
+            units
+        )
 
-    def get_net_height_m_maybe(self) -> OPT_FLOAT:
+    def get_net_height_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m or None if not given.
+            Height of the net fished or None if not given.
         """
-        return self._net_height_m
+        return afscgap.convert.convert_distance(
+            self._net_height_m,
+            units
+        )
 
-    def get_net_width_m(self) -> float:
+    def get_net_width(self, units: str = 'm') -> float:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m after asserting it is given.
+            Distance of the net fished after asserting it is given.
         """
-        return afscgap.model.assert_float_present(self._net_width_m)
+        return afscgap.model.assert_float_present(
+            self.get_net_width_maybe(units=units)
+        )
 
-    def get_net_height_m(self) -> float:
+    def get_net_height(self, units: str = 'm') -> float:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m after asserting it is given.
+            Height of the net fished after asserting it is given.
         """
-        return afscgap.model.assert_float_present(self._net_height_m)
+        return afscgap.model.assert_float_present(
+            self.get_net_height_maybe(units=units)
+        )
 
-    def get_area_swept_ha(self) -> float:
+    def get_area_swept(self, units: str = 'ha') -> float:
         """Get the field labeled as area_swept_ha in the API.
 
+        Args:
+            units: The units in which the area should be returned. Options:
+                ha, m2, km2. Defaults to ha.
+
         Returns:
-            Area covered by the net while fishing in hectares.
+            Area covered by the net while fishing in desired units.
         """
-        return self._area_swept_ha
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_area(self._area_swept_ha, units)
+        )
 
-    def get_duration_hr(self) -> float:
+    def get_duration(self, units: str = 'hr') -> float:
         """Get the field labeled as duration_hr in the API.
 
+        Args:
+            units: The units in which the duration should be returned. Options:
+                day, hr, min. Defaults to hr.
+
         Returns:
-            Duration of the haul as number of hours.
+            Duration of the haul.
         """
-        return self._duration_hr
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_time(self._duration_hr, units)
+        )
 
     def get_tsn(self) -> int:
         """Get the field labeled as tsn in the API.
 
         Returns:
             Taxonomic information system species code.
         """
@@ -788,141 +861,121 @@
         """Get the field labeled as ak_survey_id in the API.
 
         Returns:
             AK identifier for the survey or None if not given.
         """
         return self._ak_survey_id
 
-    def get_cpue_kgha(self) -> float:
+    def get_cpue_weight(self, units: str = 'kg/ha') -> float:
         """Get the value of field cpue_kgha with validity assert.
 
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch weight divided by net area (kg / hectares) if available. See
-            metadata.
-        """
-        return afscgap.model.assert_float_present(self._cpue_kgha)
-
-    def get_cpue_kgkm2(self) -> float:
-        """Get the value of field cpue_kgkm2 with validity assert.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Catch weight divided by net area (kg / km^2) if available. See
+            Catch weight divided by net area (kg / hectares) if available. See
             metadata.
         """
-        return afscgap.model.assert_float_present(self._cpue_kgkm2)
-
-    def get_cpue_kg1000km2(self) -> float:
-        """Get the value of field cpue_kg1000km2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch weight divided by net area (kg / km^2 * 1000) if available.
-            See metadata.
-        """
-        return afscgap.model.assert_float_present(self._cpue_kg1000km2)
+        return afscgap.model.assert_float_present(
+            self.get_cpue_weight_maybe(units=units)
+        )
 
-    def get_cpue_noha(self) -> float:
+    def get_cpue_count(self, units: str = 'count/ha') -> float:
         """Get the value of field cpue_noha with validity assert.
 
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Catch number divided by net sweep area if available (count /
             hectares). See metadata.
         """
-        return afscgap.model.assert_float_present(self._cpue_noha)
-
-    def get_cpue_nokm2(self) -> float:
-        """Get the value of field cpue_nokm2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2).
-            See metadata.
-        """
-        return afscgap.model.assert_float_present(self._cpue_nokm2)
-
-    def get_cpue_no1000km2(self) -> float:
-        """Get the value of field cpue_no1000km2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2 *
-            1000). See metadata.
-        """
-        return afscgap.model.assert_float_present(self._cpue_no1000km2)
+        return afscgap.model.assert_float_present(
+            self.get_cpue_count_maybe(units=units)
+        )
 
-    def get_weight_kg(self) -> float:
+    def get_weight(self, units: str = 'kg') -> float:
         """Get the value of field weight_kg with validity assert.
 
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Taxon weight (kg) if available. See metadata.
         """
-        return afscgap.model.assert_float_present(self._weight_kg)
+        return afscgap.model.assert_float_present(
+            self.get_weight_maybe(units=units)
+        )
 
     def get_count(self) -> float:
         """Get the value of field count with validity assert.
 
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Total number of organism individuals in haul.
         """
         return afscgap.model.assert_float_present(self._count)
 
-    def get_bottom_temperature_c(self) -> float:
+    def get_bottom_temperature(self, units='c') -> float:
         """Get the value of field bottom_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Bottom temperature associated with observation if available in
-            Celsius.
+            Bottom temperature associated with observation / inferrence if
+            available.
         """
-        return afscgap.model.assert_float_present(self._bottom_temperature_c)
+        return afscgap.model.assert_float_present(
+            self.get_bottom_temperature_maybe(units=units)
+        )
 
-    def get_surface_temperature_c(self) -> float:
+    def get_surface_temperature(self, units='c') -> float:
         """Get the value of field surface_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Surface temperature associated with observation if available in
-            Celsius. None if not
+            Surface temperature associated with observation / inferrence if
+            available.
         """
-        return afscgap.model.assert_float_present(self._surface_temperature_c)
+        return afscgap.model.assert_float_present(
+            self.get_surface_temperature_maybe(units=units)
+        )
 
     def is_complete(self) -> bool:
         """Determine if this record has all of its values filled in.
 
         Returns:
             True if all optional fields have a parsed value with the expected
             type and false otherwise.
@@ -939,63 +992,18 @@
             self._bottom_temperature_c,
             self._surface_temperature_c,
             self._tsn
         ]
 
         has_none = None in optional_fields
         all_fields_present = not has_none
-        has_valid_date_time = afscgap.util.is_iso8601(self._date_time)
+        has_valid_date_time = afscgap.convert.is_iso8601(self._date_time)
 
         return all_fields_present and has_valid_date_time
 
-    def to_dict(self) -> dict:
-        """Serialize this Record to a dictionary form.
-
-        Returns:
-            Dictionary with field names matching those found in the API results
-            with incomplete records having some values as None.
-        """
-        return {
-            'year': self._year,
-            'srvy': self._srvy,
-            'survey': self._survey,
-            'survey_id': self._survey_id,
-            'cruise': self._cruise,
-            'haul': self._haul,
-            'stratum': self._stratum,
-            'station': self._station,
-            'vessel_name': self._vessel_name,
-            'vessel_id': self._vessel_id,
-            'date_time': self._date_time,
-            'latitude_dd': self._latitude_dd,
-            'longitude_dd': self._longitude_dd,
-            'species_code': self._species_code,
-            'common_name': self._common_name,
-            'scientific_name': self._scientific_name,
-            'taxon_confidence': self._taxon_confidence,
-            'cpue_kgha': self._cpue_kgha,
-            'cpue_kgkm2': self._cpue_kgkm2,
-            'cpue_kg1000km2': self._cpue_kg1000km2,
-            'cpue_noha': self._cpue_noha,
-            'cpue_nokm2': self._cpue_nokm2,
-            'cpue_no1000km2': self._cpue_no1000km2,
-            'weight_kg': self._weight_kg,
-            'count': self._count,
-            'bottom_temperature_c': self._bottom_temperature_c,
-            'surface_temperature_c': self._surface_temperature_c,
-            'depth_m': self._depth_m,
-            'distance_fished_km': self._distance_fished_km,
-            'net_width_m': self._net_width_m,
-            'net_height_m': self._net_height_m,
-            'area_swept_ha': self._area_swept_ha,
-            'duration_hr': self._duration_hr,
-            'tsn': self._tsn,
-            'ak_survey_id': self._ak_survey_id,
-        }
-
 
 def parse_record(target: dict) -> afscgap.model.Record:
     """Parse a record from a returned item dictionary.
 
     Args:
         target: The dictionary from which values should be read.
 
@@ -1013,15 +1021,15 @@
     survey_id = float(target['survey_id'])
     cruise = float(target['cruise'])
     haul = float(target['haul'])
     stratum = float(target['stratum'])
     station = str(target['station'])
     vessel_name = str(target['vessel_name'])
     vessel_id = float(target['vessel_id'])
-    date_time = afscgap.util.convert_to_iso8601(str(target['date_time']))
+    date_time = afscgap.convert.convert_to_iso8601(str(target['date_time']))
     latitude_dd = float(target['latitude_dd'])
     longitude_dd = float(target['longitude_dd'])
     species_code = float(target['species_code'])
     common_name = str(target['common_name'])
     scientific_name = str(target['scientific_name'])
     taxon_confidence = str(target['taxon_confidence'])
     cpue_kgha = afscgap.model.get_opt_float(target['cpue_kgha'])
```

### Comparing `afscgap-0.0.7/afscgap/cursor.py` & `afscgap-0.0.8/afscgap/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Interfaces for cursor objects which iterate over real or inferred records.
 
 (c) 2023 Regents of University of California / The Eric and Wendy Schmidt Center
 for Data Science and the Environment at UC Berkeley.
 
 This file is part of afscgap released under the BSD 3-Clause License. See
-LICENSE.txt.
+LICENSE.md.
 """
 
 import queue
 import typing
 
 import afscgap.model
 
-from afscgap.util import OPT_INT
+from afscgap.typesdef import OPT_INT
 
 
 class Cursor(typing.Iterable[afscgap.model.Record]):
     """Interface for objects allowing generation / retrieval of records."""
 
     def get_base_url(self) -> str:
         """Get the URL at which the first page of query results can be found.
```

### Comparing `afscgap-0.0.7/afscgap/inference.py` & `afscgap-0.0.8/afscgap/inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 Tools for inferring missing, negative, or zero catch records.
 
 (c) 2023 Regents of University of California / The Eric and Wendy Schmidt Center
 for Data Science and the Environment at UC Berkeley.
 
 This file is part of afscgap released under the BSD 3-Clause License. See
-LICENSE.txt.
+LICENSE.md.
 """
 import copy
 import csv
 import io
 import itertools
 import queue
 import typing
 
+import afscgap.convert
 import afscgap.client
 import afscgap.cursor
+import afscgap.http
 import afscgap.model
 import afscgap.query_util
-import afscgap.util
 
-from afscgap.util import OPT_FLOAT
-from afscgap.util import OPT_INT
-from afscgap.util import OPT_REQUESTOR
-from afscgap.util import OPT_STR
+from afscgap.typesdef import OPT_FLOAT
+from afscgap.typesdef import OPT_INT
+from afscgap.typesdef import OPT_REQUESTOR
+from afscgap.typesdef import OPT_STR
 
 DEFAULT_HAULS_URL = 'https://pyafscgap.org/community/hauls.csv'
 SPECIES_DICT = typing.Dict[str, afscgap.model.SpeciesRecord]
 
 HAUL_LIST = typing.List[afscgap.model.Haul]
 OPT_HAUL_LIST = typing.Optional[HAUL_LIST]
 HAUL_FILTERABLE_FIELDS = [
@@ -78,15 +79,15 @@
         Cursor which 1) first iterates over the inner_cursor and then
         2) provides inferred zero catch records (for any hauls without observed
         data from inner_cursor for a species).
     """
     params_safe = copy.deepcopy(params)
 
     if 'date_time' in params_safe:
-        params_safe['date_time'] = afscgap.util.convert_from_iso8601(
+        params_safe['date_time'] = afscgap.convert.convert_from_iso8601(
             params_safe['date_time']
         )
 
     if hauls_prefetch is not None:
         hauls_data = hauls_prefetch
     else:
         hauls_data = get_hauls_data(
@@ -156,18 +157,18 @@
     """
     if hauls_url is None:
         hauls_url = DEFAULT_HAULS_URL
 
     params_checker = build_params_checker(params)
 
     if requestor is None:
-        requestor = afscgap.util.build_requestor()
+        requestor = afscgap.http.build_requestor()
 
     response = requestor(hauls_url)
-    afscgap.util.check_result(response)
+    afscgap.http.check_result(response)
 
     response.encoding = 'utf-8'
     response_io = io.StringIO(response.text, newline='')
 
     response_rows = csv.DictReader(response_io)
     response_hauls = map(parse_haul, response_rows)
     response_hauls_filtered = filter(params_checker, response_hauls)
@@ -599,29 +600,47 @@
         Returns:
             The date and time of the haul which has been attempted to be
             transformed to an ISO 8601 string without timezone info. If it
             couldn’t be transformed, the original string is reported.
         """
         return self._haul.get_date_time()
 
-    def get_latitude_dd(self) -> float:
+    def get_latitude(self, units: str = 'dd') -> float:
         """Get the field labeled as latitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Latitude in decimal degrees associated with the haul.
         """
-        return self._haul.get_latitude_dd()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_degrees(
+                self._haul.get_latitude_dd(),
+                units
+            )
+        )
 
-    def get_longitude_dd(self) -> float:
+    def get_longitude(self, units: str = 'dd') -> float:
         """Get the field labeled as longitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Longitude in decimal degrees associated with the haul.
         """
-        return self._haul.get_longitude_dd()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_degrees(
+                self._haul.get_longitude_dd(),
+                units
+            )
+        )
 
     def get_species_code(self) -> float:
         """Get the field labeled as species_code in the API.
 
         Returns:
             Unique ID associated with the species observed.
         """
@@ -649,159 +668,221 @@
         """Get rating of taxon identification confidence.
 
         Returns:
             Always returns Unassessed.
         """
         return 'Unassessed'
 
-    def get_cpue_kgha_maybe(self) -> OPT_FLOAT:
-        """Get catch weight divided by net area (kg / hectares).
+    def get_cpue_weight_maybe(self, units: str = 'kg/ha') -> OPT_FLOAT:
+        """Get a field labeled as cpue_* in the API.
 
-        Returns:
-            Always returns 0.
-        """
-        return 0
-
-    def get_cpue_kgkm2_maybe(self) -> OPT_FLOAT:
-        """Get catch weight divided by net area (kg / km^2).
-
-        Returns:
-            Always returns 0.
-        """
-        return 0
-
-    def get_cpue_kg1000km2_maybe(self) -> OPT_FLOAT:
-        """Get catch weight divided by net area (kg / km^2 * 1000).
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Returns:
-            Always returns 0.
+            Catch weight divided by net area (in given units) if available. See
+            metadata. None if could not interpret as a float. If an inferred
+            zero catch record, will be zero.
         """
         return 0
 
-    def get_cpue_noha_maybe(self) -> OPT_FLOAT:
-        """Get catch number divided by net sweep area.
+    def get_cpue_count_maybe(self, units: str = 'kg/ha') -> OPT_FLOAT:
+        """Get the field labeled as cpue_* in the API.
 
-        Returns:
-            Always returns 0.
-        """
-        return 0
+        Get the catch per unit effort from the record with one of the following
+        units: kg/ha, kg/km2, kg1000/km2.
 
-    def get_cpue_nokm2_maybe(self) -> OPT_FLOAT:
-        """Get catch number divided by net sweep area.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
 
         Returns:
-            Always returns 0.
+            Catch weight divided by net area (in given units) if available. See
+            metadata. None if could not interpret as a float. If an inferred
+            zero catch record, will be zero.
         """
         return 0
 
-    def get_cpue_no1000km2_maybe(self) -> OPT_FLOAT:
-        """Get catch number divided by net sweep area.
+    def get_weight_maybe(self, units='kg') -> OPT_FLOAT:
+        """Get the field labeled as weight_kg in the API.
 
-        Returns:
-            Always returns 0.
-        """
-        return 0
-
-    def get_weight_kg_maybe(self) -> OPT_FLOAT:
-        """Get taxon weight (kg).
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
 
         Returns:
-            Always returns 0.
+            Taxon weight if available. See metadata. None if could not
+            interpret as a float. If an inferred zero catch record, will be
+            zero.
         """
         return 0
 
     def get_count_maybe(self) -> OPT_FLOAT:
         """Get total number of organism individuals in haul.
 
         Returns:
             Always returns 0.
         """
         return 0
 
-    def get_bottom_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_bottom_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as bottom_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
-            Bottom temperature associated with haul if available in
-            Celsius. None if not given or could not interpret as a float.
-        """
-        return self._haul.get_bottom_temperature_c_maybe()
+            Bottom temperature associated with observation / inferrence if
+            available in desired units. None if not given or could not interpret
+            as a float.
+        """
+        return afscgap.convert.convert_temperature(
+            self._haul.get_bottom_temperature_c_maybe(),
+            units
+        )
 
-    def get_surface_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_surface_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as surface_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
-            Surface temperature associated with haul if available in
-            Celsius. None if not given or could not interpret as a float.
+            Surface temperature associated with observation / inferrence if
+            available. None if not given or could not interpret as a float.
         """
-        return self._haul.get_surface_temperature_c_maybe()
+        return afscgap.convert.convert_temperature(
+            self._haul.get_surface_temperature_c_maybe(),
+            units
+        )
 
-    def get_depth_m(self) -> float:
+    def get_depth(self, units: str = 'm') -> float:
         """Get the field labeled as depth_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Depth of the bottom in meters.
+            Depth of the bottom.
         """
-        return self._haul.get_depth_m()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_distance(self._haul.get_depth_m(), units)
+        )
 
-    def get_distance_fished_km(self) -> float:
+    def get_distance_fished(self, units: str = 'm') -> float:
         """Get the field labeled as distance_fished_km in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to km.
+
         Returns:
-            Distance of the net fished as km.
+            Distance of the net fished.
         """
-        return self._haul.get_distance_fished_km()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_distance(
+                self._haul.get_distance_fished_km() * 1000,
+                units
+            )
+        )
 
-    def get_net_width_m_maybe(self) -> OPT_FLOAT:
+    def get_net_width_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m or None if not given.
+            Distance of the net fished or None if not given.
         """
-        return self._haul.get_net_width_m_maybe()
+        return afscgap.convert.convert_distance(
+            self._haul.get_net_width_m_maybe(),
+            units
+        )
 
-    def get_net_height_m_maybe(self) -> OPT_FLOAT:
+    def get_net_height_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m or None if not given.
+            Height of the net fished or None if not given.
         """
-        return self._haul.get_net_height_m_maybe()
+        return afscgap.convert.convert_distance(
+            self._haul.get_net_height_m_maybe(),
+            units
+        )
 
-    def get_net_width_m(self) -> float:
+    def get_net_width(self, units: str = 'm') -> float:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m after asserting it is given.
+            Distance of the net fished after asserting it is given.
         """
-        return self._haul.get_net_width_m()
+        return afscgap.model.assert_float_present(
+            self.get_net_width_maybe(units=units)
+        )
 
-    def get_net_height_m(self) -> float:
+    def get_net_height(self, units: str = 'm') -> float:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m after asserting it is given.
+            Height of the net fished after asserting it is given.
         """
-        return self._haul.get_net_height_m()
+        return afscgap.model.assert_float_present(
+            self.get_net_height_maybe(units=units)
+        )
 
-    def get_area_swept_ha(self) -> float:
+    def get_area_swept(self, units: str = 'ha') -> float:
         """Get the field labeled as area_swept_ha in the API.
 
+        Args:
+            units: The units in which the area should be returned. Options:
+                ha, m2, km2. Defaults to ha.
+
         Returns:
-            Area covered by the net while fishing in hectares.
+            Area covered by the net while fishing in desired units.
         """
-        return self._haul.get_area_swept_ha()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_area(
+                self._haul.get_area_swept_ha(),
+                units
+            )
+        )
 
-    def get_duration_hr(self) -> float:
+    def get_duration(self, units: str = 'hr') -> float:
         """Get the field labeled as duration_hr in the API.
 
+        Args:
+            units: The units in which the duration should be returned. Options:
+                day, hr, min. Defaults to hr.
+
         Returns:
-            Duration of the haul as number of hours.
+            Duration of the haul.
         """
-        return self._haul.get_duration_hr()
+        return afscgap.model.assert_float_present(
+            afscgap.convert.convert_time(self._haul.get_duration_hr(), units)
+        )
 
     def get_tsn(self) -> int:
         """Get taxonomic information system species code.
 
         Returns:
             TSN for species.
         """
@@ -827,95 +908,61 @@
         """Get the field labeled as ak_survey_id in the API.
 
         Returns:
             AK identifier for the survey or None if not given.
         """
         return self._ak_survey_id
 
-    def get_cpue_kgha(self) -> float:
+    def get_cpue_weight(self, units: str = 'kg/ha') -> float:
         """Get the value of field cpue_kgha with validity assert.
 
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Always returns 0.
-        """
-        return 0
-
-    def get_cpue_kgkm2(self) -> float:
-        """Get the value of field cpue_kgkm2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Always returns 0
-        """
-        return 0
-
-    def get_cpue_kg1000km2(self) -> float:
-        """Get the value of field cpue_kg1000km2 with validity assert.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Always returns 0
+            Catch weight divided by net area (kg / hectares) if available. See
+            metadata. Always returns 0.
         """
         return 0
 
-    def get_cpue_noha(self) -> float:
+    def get_cpue_count(self, units: str = 'count/ha') -> float:
         """Get the value of field cpue_noha with validity assert.
 
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Always returns 0
-        """
-        return 0
-
-    def get_cpue_nokm2(self) -> float:
-        """Get the value of field cpue_nokm2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Always returns 0
-        """
-        return 0
-
-    def get_cpue_no1000km2(self) -> float:
-        """Get the value of field cpue_no1000km2 with validity assert.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
 
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Always returns 0
+            Catch number divided by net sweep area if available (count /
+            hectares). See metadata. Always returns 0.
         """
         return 0
 
-    def get_weight_kg(self) -> float:
+    def get_weight(self, units: str = 'kg') -> float:
         """Get the value of field weight_kg with validity assert.
 
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Always returns 0
+            Taxon weight (kg) if available. See metadata. Always returns 0.
         """
         return 0
 
     def get_count(self) -> float:
         """Get the value of field count with validity assert.
 
         Raises:
@@ -923,96 +970,65 @@
             could not be parsed as expected.
 
         Returns:
             Always returns 0
         """
         return 0
 
-    def get_bottom_temperature_c(self) -> float:
+    def get_bottom_temperature(self, units='c') -> float:
         """Get the value of field bottom_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Bottom temperature associated with observation if available in
-            Celsius.
+            Bottom temperature associated with observation / inferrence if
+            available.
         """
-        return self._haul.get_bottom_temperature_c()
+        return afscgap.model.assert_float_present(
+            self.get_bottom_temperature_maybe(units=units)
+        )
 
-    def get_surface_temperature_c(self) -> float:
+    def get_surface_temperature(self, units='c') -> float:
         """Get the value of field surface_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Surface temperature associated with observation if available in
-            Celsius. None if not
+            Surface temperature associated with observation / inferrence if
+            available.
         """
-        return self._haul.get_surface_temperature_c()
+        return afscgap.model.assert_float_present(
+            self.get_surface_temperature_maybe(units=units)
+        )
 
     def is_complete(self) -> bool:
         """Determine if this record has all of its values filled in.
 
         Returns:
             True if all optional fields have a parsed value with the expected
             type and false otherwise.
         """
         tsn_given = self._tsn is not None
         ak_survey_id_given = self._ak_survey_id is not None
         return tsn_given and ak_survey_id_given and self._haul.is_complete()
 
-    def to_dict(self) -> dict:
-        """Serialize this Record to a dictionary form.
-
-        Returns:
-            Dictionary with field names matching those found in the API results
-            with incomplete records having some values as None.
-        """
-        return {
-            'year': self.get_year(),
-            'srvy': self.get_srvy(),
-            'survey': self.get_survey(),
-            'survey_id': self.get_survey_id(),
-            'cruise': self.get_cruise(),
-            'haul': self.get_haul(),
-            'stratum': self.get_stratum(),
-            'station': self.get_station(),
-            'vessel_name': self.get_vessel_name(),
-            'vessel_id': self.get_vessel_id(),
-            'date_time': self.get_date_time(),
-            'latitude_dd': self.get_latitude_dd(),
-            'longitude_dd': self.get_longitude_dd(),
-            'species_code': self.get_species_code(),
-            'common_name': self.get_common_name(),
-            'scientific_name': self.get_scientific_name(),
-            'taxon_confidence': self.get_taxon_confidence(),
-            'cpue_kgha': self.get_cpue_kgha(),
-            'cpue_kgkm2': self.get_cpue_kgkm2(),
-            'cpue_kg1000km2': self.get_cpue_kg1000km2(),
-            'cpue_noha': self.get_cpue_noha(),
-            'cpue_nokm2': self.get_cpue_nokm2(),
-            'cpue_no1000km2': self.get_cpue_no1000km2(),
-            'weight_kg': self.get_weight_kg(),
-            'count': self.get_count(),
-            'bottom_temperature_c': self.get_bottom_temperature_c_maybe(),
-            'surface_temperature_c': self.get_surface_temperature_c_maybe(),
-            'depth_m': self.get_depth_m(),
-            'distance_fished_km': self.get_distance_fished_km(),
-            'net_width_m': self.get_net_width_m(),
-            'net_height_m': self.get_net_height_m(),
-            'area_swept_ha': self.get_area_swept_ha(),
-            'duration_hr': self.get_duration_hr(),
-            'tsn': self.get_tsn_maybe(),
-            'ak_survey_id': self.get_ak_survey_id()
-        }
-
 
 def parse_haul(target: dict) -> afscgap.model.Haul:
     """Parse a Haul record from a row in the community Hauls flat file.
 
     Args:
         target: Dict describing a single row from the community-maintained
             Hauls flat file.
@@ -1025,15 +1041,15 @@
     survey_id = float(target['Survey Id'])
     cruise = float(target['Cruise'])
     haul = float(target['Haul'])
     stratum = float(target['Stratum'])
     station = str(target['Station'])
     vessel_name = str(target['Vessel Name'])
     vessel_id = float(target['Vessel Id'])
-    date_time = str(afscgap.util.convert_to_iso8601(target['Date Time']))
+    date_time = str(afscgap.convert.convert_to_iso8601(target['Date Time']))
     latitude_dd = float(target['Latitude Dd'])
     longitude_dd = float(target['Longitude Dd'])
     bottom_temperature_c = afscgap.model.get_opt_float(
         target['Bottom Temperature C']
     )
     surface_temperature_c = afscgap.model.get_opt_float(
         target['Surface Temperature C']
```

### Comparing `afscgap-0.0.7/afscgap/model.py` & `afscgap-0.0.8/afscgap/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Definition of common library data with its structures and interfaces.
 
 (c) 2023 Regents of University of California / The Eric and Wendy Schmidt Center
 for Data Science and the Environment at UC Berkeley.
 
 This file is part of afscgap released under the BSD 3-Clause License. See
-LICENSE.txt.
+LICENSE.md.
 """
-from afscgap.util import OPT_FLOAT
-from afscgap.util import OPT_INT
+from afscgap.typesdef import OPT_FLOAT
+from afscgap.typesdef import OPT_INT
 
 OPT_RECORD = 'typing.Optional[Record]'
 
 
 class HaulKeyable:
     """Interface for objects which can be associated to a specific haul.
 
@@ -171,25 +171,33 @@
         Returns:
             The date and time of the haul which has been attempted to be
             transformed to an ISO 8601 string without timezone info. If it
             couldn’t be transformed, the original string is reported.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_latitude_dd(self) -> float:
+    def get_latitude(self, units: str = 'dd') -> float:
         """Get the field labeled as latitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Latitude in decimal degrees associated with the haul.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_longitude_dd(self) -> float:
+    def get_longitude(self, units: str = 'dd') -> float:
         """Get the field labeled as longitude_dd in the API.
 
+        Args:
+            units: The units to return this value in. Only supported is dd for
+                degrees. Deafults to dd.
+
         Returns:
             Longitude in decimal degrees associated with the haul.
         """
         raise NotImplementedError('Use implementor.')
 
     def get_species_code(self) -> float:
         """Get the field labeled as species_code in the API.
@@ -223,79 +231,54 @@
 
         Returns:
             Confidence flag regarding ability to identify species (High,
             Moderate, Low). In practice, this can also be Unassessed.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_kgha_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kgha in the API.
-
-        Returns:
-            Catch weight divided by net area (kg / hectares) if available. See
-            metadata. None if could not interpret as a float. If an inferred
-            zero catch record, will be zero.
-        """
-        raise NotImplementedError('Use implementor.')
+    def get_cpue_weight_maybe(self, units: str = 'kg/ha') -> OPT_FLOAT:
+        """Get a field labeled as cpue_* in the API.
 
-    def get_cpue_kgkm2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kgkm2 in the API.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Returns:
-            Catch weight divided by net area (kg / km^2) if available. See
+            Catch weight divided by net area (in given units) if available. See
             metadata. None if could not interpret as a float. If an inferred
             zero catch record, will be zero.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_kg1000km2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_kg1000km2 in the API.
-
-        Returns:
-            Catch weight divided by net area (kg / km^2 * 1000) if available.
-            See metadata. None if could not interpret as a float. If an inferred
-            zero catch record, will be zero.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_cpue_noha_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_noha in the API.
+    def get_cpue_count_maybe(self, units: str = 'count/ha') -> OPT_FLOAT:
+        """Get the field labeled as cpue_* in the API.
 
-        Returns:
-            Catch number divided by net sweep area if available (count /
-            hectares). See metadata. None if could not interpret as a float. If
-            an inferred zero catch record, will be zero.
-        """
-        raise NotImplementedError('Use implementor.')
+        Get the catch per unit effort from the record with one of the following
+        units: kg/ha, kg/km2, kg1000/km2.
 
-    def get_cpue_nokm2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_nokm2 in the API.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
 
         Returns:
-            Catch number divided by net sweep area if available (count / km^2).
-            See metadata. None if could not interpret as a float. If an inferred
+            Catch weight divided by net area (in given units) if available. See
+            metadata. None if could not interpret as a float. If an inferred
             zero catch record, will be zero.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_no1000km2_maybe(self) -> OPT_FLOAT:
-        """Get the field labeled as cpue_no1000km2 in the API.
-
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2 *
-            1000). See metadata. None if could not interpret as a float. If an
-            inferred zero catch record, will be zero.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_weight_kg_maybe(self) -> OPT_FLOAT:
+    def get_weight_maybe(self, units: str = 'kg') -> OPT_FLOAT:
         """Get the field labeled as weight_kg in the API.
 
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
+
         Returns:
-            Taxon weight (kg) if available. See metadata. None if could not
+            Taxon weight if available. See metadata. None if could not
             interpret as a float. If an inferred zero catch record, will be
             zero.
         """
         raise NotImplementedError('Use implementor.')
 
     def get_count_maybe(self) -> OPT_FLOAT:
         """Get the field labeled as count in the API.
@@ -303,95 +286,136 @@
         Returns:
             Total number of organism individuals in haul. None if could not
             interpret as a float. If an inferred zero catch record, will be
             zero.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_bottom_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_bottom_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as bottom_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
             Bottom temperature associated with observation / inferrence if
-            available in Celsius. None if not given or could not interpret as a
-            float.
+            available in desired units. None if not given or could not interpret
+            as a float.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_surface_temperature_c_maybe(self) -> OPT_FLOAT:
+    def get_surface_temperature_maybe(self, units: str = 'c') -> OPT_FLOAT:
         """Get the field labeled as surface_temperature_c in the API.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Returns:
             Surface temperature associated with observation / inferrence if
-            available in Celsius. None if not given or could not interpret as a
-            float.
+            available. None if not given or could not interpret as a float.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_depth_m(self) -> float:
+    def get_depth(self, units: str = 'm') -> float:
         """Get the field labeled as depth_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Depth of the bottom in meters.
+            Depth of the bottom.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_distance_fished_km(self) -> float:
+    def get_distance_fished(self, units: str = 'm') -> float:
         """Get the field labeled as distance_fished_km in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as km.
+            Distance of the net fished.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_net_width_m(self) -> float:
+    def get_net_width(self, units: str = 'm') -> float:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m after asserting it is given.
+            Distance of the net fished after asserting it is given.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_net_height_m(self) -> float:
+    def get_net_height(self, units: str = 'm') -> float:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m after asserting it is given.
+            Height of the net fished after asserting it is given.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_net_width_m_maybe(self) -> OPT_FLOAT:
+    def get_net_width_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_width_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Distance of the net fished as m or None if not given.
+            Distance of the net fished or None if not given.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_net_height_m_maybe(self) -> OPT_FLOAT:
+    def get_net_height_maybe(self, units: str = 'm') -> OPT_FLOAT:
         """Get the field labeled as net_height_m in the API.
 
+        Args:
+            units: The units in which the distance should be returned. Options:
+                m or km for meters and kilometers respectively. Defaults to m.
+
         Returns:
-            Height of the net fished as m or None if not given.
+            Height of the net fished or None if not given.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_area_swept_ha(self) -> float:
+    def get_area_swept(self, units: str = 'ha') -> float:
         """Get the field labeled as area_swept_ha in the API.
 
+        Args:
+            units: The units in which the area should be returned. Options:
+                ha, m2, km2. Defaults to ha.
+
         Returns:
-            Area covered by the net while fishing in hectares.
+            Area covered by the net while fishing in desired units.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_duration_hr(self) -> float:
+    def get_duration(self, units: str = 'hr') -> float:
         """Get the field labeled as duration_hr in the API.
 
+        Args:
+            units: The units in which the duration should be returned. Options:
+                day, hr, min. Defaults to hr.
+
         Returns:
-            Duration of the haul as number of hours.
+            Duration of the haul.
         """
         raise NotImplementedError('Use implementor.')
 
     def get_tsn(self) -> int:
         """Get the field labeled as tsn in the API.
 
         Returns:
@@ -420,95 +444,55 @@
         """Get the field labeled as ak_survey_id in the API.
 
         Returns:
             AK identifier for the survey or None if not given.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_kgha(self) -> float:
+    def get_cpue_weight(self, units: str = 'kg/ha') -> float:
         """Get the value of field cpue_kgha with validity assert.
 
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch weight divided by net area (kg / hectares) if available. See
-            metadata. Will be zero if a zero catch record.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_cpue_kgkm2(self) -> float:
-        """Get the value of field cpue_kgkm2 with validity assert.
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                kg/ha, kg/km2, kg1000/km2. Defaults to kg/ha.
 
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
-            Catch weight divided by net area (kg / km^2) if available. See
+            Catch weight divided by net area (kg / hectares) if available. See
             metadata. Will be zero if a zero catch record.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_kg1000km2(self) -> float:
-        """Get the value of field cpue_kg1000km2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch weight divided by net area (kg / km^2 * 1000) if available.
-            See metadata. Will be zero if a zero catch record.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_cpue_noha(self) -> float:
+    def get_cpue_count(self, units: str = 'count/ha') -> float:
         """Get the value of field cpue_noha with validity assert.
 
+        Args:
+            units: The desired units for the catch per unit effort. Options:
+                count/ha, count/km2, and count1000/km2. Defaults to count/ha.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Catch number divided by net sweep area if available (count /
             hectares). See metadata. Will be zero if a zero catch record.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_cpue_nokm2(self) -> float:
-        """Get the value of field cpue_nokm2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2).
-            See metadata. Will be zero if a zero catch record.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_cpue_no1000km2(self) -> float:
-        """Get the value of field cpue_no1000km2 with validity assert.
-
-        Raises:
-            AssertionError: Raised if this field was not given by the API or
-            could not be parsed as expected.
-
-        Returns:
-            Catch number divided by net sweep area if available (count / km^2 *
-            1000). See metadata. Will be zero if a zero catch record.
-        """
-        raise NotImplementedError('Use implementor.')
-
-    def get_weight_kg(self) -> float:
+    def get_weight(self, units: str = 'kg') -> float:
         """Get the value of field weight_kg with validity assert.
 
+        Args:
+            units: The units in which the weight should be returned. Options are
+                g, kg for grams and kilograms respectively. Deafults to kg.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Taxon weight (kg) if available. See metadata. Will be zero if a zero
             catch record.
@@ -524,37 +508,47 @@
 
         Returns:
             Total number of organism individuals in haul. Will be zero if a zero
             catch record.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_bottom_temperature_c(self) -> float:
+    def get_bottom_temperature(self, units='c') -> float:
         """Get the value of field bottom_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Bottom temperature associated with observation / inferrence if
-            available in Celsius.
+            available.
         """
         raise NotImplementedError('Use implementor.')
 
-    def get_surface_temperature_c(self) -> float:
+    def get_surface_temperature(self, units='c') -> float:
         """Get the value of field surface_temperature_c with validity assert.
 
+        Args:
+            units: The units in which the temperature should be returned.
+                Options: c or f for Celcius and Fahrenheit respectively.
+                Defaults to c.
+
         Raises:
             AssertionError: Raised if this field was not given by the API or
             could not be parsed as expected.
 
         Returns:
             Surface temperature associated with observation / inferrence if
-            available in Celsius. None if not
+            available.
         """
         raise NotImplementedError('Use implementor.')
 
     def is_complete(self) -> bool:
         """Determine if this record has all of its values filled in.
 
         Returns:
@@ -562,19 +556,62 @@
             type and false otherwise.
         """
         raise NotImplementedError('Use implementor.')
 
     def to_dict(self) -> dict:
         """Serialize this Record to a dictionary form.
 
+        Serialize this Record to a dictionary form, including only field names
+        that would be found on records returned from the API service.
+
         Returns:
             Dictionary with field names matching those found in the API results
             with incomplete records having some values as None.
         """
-        raise NotImplementedError('Use implementor.')
+        return {
+            'year': self.get_year(),
+            'srvy': self.get_srvy(),
+            'survey': self.get_survey(),
+            'survey_id': self.get_survey_id(),
+            'cruise': self.get_cruise(),
+            'haul': self.get_haul(),
+            'stratum': self.get_stratum(),
+            'station': self.get_station(),
+            'vessel_name': self.get_vessel_name(),
+            'vessel_id': self.get_vessel_id(),
+            'date_time': self.get_date_time(),
+            'latitude_dd': self.get_latitude(),
+            'longitude_dd': self.get_longitude(),
+            'species_code': self.get_species_code(),
+            'common_name': self.get_common_name(),
+            'scientific_name': self.get_scientific_name(),
+            'taxon_confidence': self.get_taxon_confidence(),
+            'cpue_kgha': self.get_cpue_weight_maybe(units='kg/ha'),
+            'cpue_kgkm2': self.get_cpue_weight_maybe(units='kg/km2'),
+            'cpue_kg1000km2': self.get_cpue_weight_maybe(units='kg1000/km2'),
+            'cpue_noha': self.get_cpue_count_maybe(units='count/ha'),
+            'cpue_nokm2': self.get_cpue_count_maybe(units='count/km2'),
+            'cpue_no1000km2': self.get_cpue_count_maybe(units='count1000/km2'),
+            'weight_kg': self.get_weight(units='kg'),
+            'count': self.get_count(),
+            'bottom_temperature_c': self.get_bottom_temperature_maybe(
+                units='c'
+            ),
+            'surface_temperature_c': self.get_surface_temperature_maybe(
+                units='c'
+            ),
+            'depth_m': self.get_depth(units='m'),
+            'distance_fished_km': self.get_distance_fished(units='km'),
+            'net_width_m': self.get_net_width(units='m'),
+            'net_height_m': self.get_net_height(units='m'),
+            'area_swept_ha': self.get_area_swept(units='ha'),
+            'duration_hr': self.get_duration(units='hr'),
+            'tsn': self.get_tsn_maybe(),
+            'ak_survey_id': self.get_ak_survey_id()
+        }
 
 
 class Haul(HaulKeyable):
     """Metadata about a haul performed in a survey.
 
     Metadata about a haul performed in a survey which is typically maintained
     for record inferrence and which does not typically leave the internals of
```

### Comparing `afscgap-0.0.7/afscgap/query_util.py` & `afscgap-0.0.8/afscgap/query_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 (c) 2023 Regents of University of California / The Eric and Wendy Schmidt Center
 for Data Science and the Environment at UC Berkeley.
 """
 import numbers
 
 
 def interpret_query_to_ords(target: dict) -> dict:
+    """Convert a description of a query to ORDS syntax.
+
+    Args:
+        target: The "native Python structures" version of the query.
+
+    Returns:
+        Dicitionary encoding the ORDS-expected query format.
+    """
     target_items = target.items()
 
     def interpret_value(value):
         if value is None:
             return None
 
-        if not isinstance(value, tuple):
+        if not (isinstance(value, tuple) or isinstance(value, list)):
             return value
 
         if len(value) != 2:
             raise RuntimeError('Range param given without 2 elements.')
 
         lower_limit_given = value[0] is not None
         upper_limit_given = value[1] is not None
@@ -36,14 +44,23 @@
         lambda x: (x[0], interpret_value(x[1])),
         target_items
     )
     return dict(target_transform_items)
 
 
 def interpret_query_to_py(target: dict) -> dict:
+    """Emulate a query in Python.
+
+    Args:
+        target: The "native Python structures" format of the query.
+
+    Returns:
+        Dictionary mapping from key to function which returns if a candidate
+        value for that field satisfies the criteria described for that field.
+    """
     target_items = target.items()
 
     def interpret_value(value):
         if value is None:
             return None
 
         if isinstance(value, dict):
```

### Comparing `afscgap-0.0.7/LICENSE.md` & `afscgap-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.7/README.md` & `afscgap-0.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# AFSC GAP for Python
-Python-based tool chain for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program).
+# Python Tools for AFSC GAP
+Python-based tool chain ("Pyafscgap.org") for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). This provides information about where certain species were seen and when under what conditions, information useful for research in ocean health.
+
+<br>
 
 | Group | Badges |
 |-------|--------|
 | Status | ![build workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/build.yml/badge.svg?branch=main) ![docs workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/docs.yml/badge.svg?branch=main) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) |
 | Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) |
-| Publication | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) |
+| Publication | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v1)|
 
 See [webpage](https://pyafscgap.org), [project Github](https://github.com/SchmidtDSE/afscgap), and [example notebook](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb).
 
 <br>
 <br>
 
 ## Quickstart
@@ -31,15 +33,15 @@
 <br>
 
 ## Purpose
 Unofficial Python-based tool set for interacting with [bottom trawl surveys](https://www.fisheries.noaa.gov/alaska/commercial-fishing/alaska-groundfish-bottom-trawl-survey-data) from the [Ground Fish Assessment Program (GAP)](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). It offers:
 
  - Pythonic access to the official [NOAA AFSC GAP API service](https://www.fisheries.noaa.gov/foss/f?p=215%3A28).
  - Tools for inference of the "negative" observations not provided by the API service.
- - Visualization tools for quickly exploring and creating comparisons within the datset, including for audiences with limited programming experience.
+ - Visualization tools for quickly exploring and creating comparisons within the dataset, including for audiences with limited programming experience.
 
 Note that GAP is an excellent dataset produced by the [Resource Assessment and Conservation Engineering (RACE) Division](https://www.fisheries.noaa.gov/about/resource-assessment-and-conservation-engineering-division) of the [Alaska Fisheries Science Center (AFSC)](https://www.fisheries.noaa.gov/about/alaska-fisheries-science-center) as part of the National Oceanic and Atmospheric Administration's Fisheries organization ([NOAA Fisheries](https://www.fisheries.noaa.gov/)).
 
 <br>
 
 #### Needs
 Scientists and developers working on ocean health have an interest in survey data from organizations like [NOAA Fisheries](https://www.fisheries.noaa.gov/). However,
@@ -75,108 +77,172 @@
 
 #### Visual analytics
 Visualization tools are available to help both programmers and non-programmers start their investigation, providing a UI that stands on the other functionality provided by this project. This is available online at [https://app.pyafscgap.org](https://app.pyafscgap.org). It can generate both CSV (spreadsheet) exports and Python query code to move investigations to their next steps. To self-host or run this tool locally, see the [visualization readme](https://github.com/SchmidtDSE/afscgap/blob/main/afscgapviz/README.md).
 
 <br>
 
 #### Basic queries
-The `afscgap.query` method is the main entry point into Python-based utilization. Calls can be written manually or generated in the [visual analytics tool](https://app.pyafscgap.org). For example, this requests all records of Pasiphaea pacifica in 2021 from the Gulf of Alaska to get the median bottom temperature when they were observed:
+The `afscgap.Query` object is the main entry point into Python-based utilization. Calls can be written manually or generated in the [visual analytics tool](https://app.pyafscgap.org). For example, this requests all records of Pasiphaea pacifica in 2021 from the Gulf of Alaska to get the median bottom temperature when they were observed:
 
 ```
 import statistics
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Build query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
-temperatures = [record.get_bottom_temperature_c() for record in results]
+# Get temperatures in Celsius
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+
+# Take the median
 print(statistics.median(temperatures))
 ```
 
-Note that `afscgap.query` returns a [Cursor](https://pyafscgap.org/devdocs/afscgap/cursor.html#Cursor). One can iterate over this `Cursor` to access [Record](https://pyafscgap.org/devdocs/afscgap/model.html#Record) objects. You can do this with list comprehensions, maps, etc or with a good old for loop like in this example which gets a histogram of haul temperatures:
+Note that `afscgap.Query.execute` returns a [Cursor](https://pyafscgap.org/devdocs/afscgap/cursor.html#Cursor). One can iterate over this `Cursor` to access [Record](https://pyafscgap.org/devdocs/afscgap/model.html#Record) objects. You can do this with list comprehensions, maps, etc or with a good old for loop like in this example which gets a histogram of haul temperatures:
 
 ```
+# Mapping from temperature in Celsius to count
 count_by_temperature_c = {}
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Build query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
+# Iterate through results and count
 for record in results:
-    temp = record.get_bottom_temperature_c()
+    temp = record.get_bottom_temperature(units='c')
     temp_rounded = round(temp)
     count = count_by_temperature_c.get(temp_rounded, 0) + 1
     count_by_temperature_c[temp_rounded] = count
 
+# Print the result
 print(count_by_temperature_c)
 ```
 
 See [data structure section](#data-structure). Using an iterator will have the library negotiate pagination behind the scenes so this operation will cause multiple HTTP requests while the iterator runs.
 
 <br>
 
 #### Enable absence data
 One of the major limitations of the official API is that it only provides presence data. However, this library can optionally infer absence or "zero catch" records using a separate static file produced by NOAA AFSC GAP. The [algorithm and details for absence inference](#absence-vs-presence-data) is further discussed below.
 
-Absence data / "zero catch" records inference can be turned on by setting `presence_only` to false in `query`. To demonstrate, this example finds total area swept and total weight for Gadus macrocephalus from the Aleutian Islands in 2021:
+Absence data / "zero catch" records inference can be turned on by passing `False` to `set_presence_only` in `Query`. To demonstrate, this example finds total area swept and total weight for Gadus macrocephalus from the Aleutian Islands in 2021:
 
 ```
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+results = query.execute()
 
 total_area = 0
 total_weight = 0
 
 for record in results:
-    total_area += record.get_area_swept_ha()
-    total_weight += record.get_weight()
+    total_area += record.get_area_swept(units='ha')
+    total_weight += record.get_weight(units='kg')
 
 template = '%.2f kg / hectare swept (%.1f kg, %.1f hectares'
 weight_per_area = total_weight / total_area
 message = template % (weight_per_area, total_weight, total_area)
 
 print(message)
 ```
 
 For more [details on the zero catch record feature](#absence-vs-presence-data), please see below.
 
 <br>
 
+#### Chaining
+It is possible to use the Query object for method chaining.
+
+```
+import statistics
+
+import afscgap
+
+# Build query
+results = afscgap.Query() \
+    .filter_year(eq=2021) \
+    .filter_srvy(eq='GOA') \
+    .filter_scientific_name(eq='Pasiphaea pacifica') \
+    .execute()
+
+# Get temperatures in Celsius
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+
+# Take the median
+print(statistics.median(temperatures))
+```
+
+Each filter and set method on Query returns the same query object.
+
+<br>
+
+#### Builder operations
+Note that Query is a builder. So, it may be used to execute a search and then execute another search with slightly modified parameters:
+
+```
+import statistics
+
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+
+# Get temperatures in Celsius for 2021
+query.filter_year(eq=2021)
+results = query.execute()
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+print(statistics.median(temperatures))
+
+# Get temperatures in Celsius for 2019
+query.filter_year(eq=2019)
+results = query.execute()
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+print(statistics.median(temperatures))
+```
+
+When calling filter, all prior filters on the query object for that field are overwritten.
+
+<br>
+
 #### Serialization
 Users may request a dictionary representation:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Create a query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
 # Get dictionary from individual record
 for record in results:
     dict_representation = record.to_dict()
     print(dict_representation['bottom_temperature_c'])
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Execute again
+results = query.execute()
 
 # Get dictionary for all records
 results_dicts = results.to_dicts()
 
 for record in results_dicts:
     print(record['bottom_temperature_c'])
 ```
@@ -189,114 +255,148 @@
 The dictionary form of the data can be used to create a Pandas dataframe:
 
 ```
 import pandas
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
 pandas.DataFrame(results.to_dicts())
 ```
 
 Note that Pandas is not required to use this library.
 
 <br>
 
 #### Advanced filtering
 You can provide range queries which translate to ORDS or Python emulated filters. For example, the following requests before and including 2019:
 
 ```
-results = afscgap.query(
-    year=(None, 2019),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(max_val=2021)  # Note max_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 The following requests data after and including 2019:
 
 ```
-results = afscgap.query(
-    year=(2019, None),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(min_val=2021)  # Note min_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 Finally, the following requests data between 2015 and 2019 (includes 2015 and 2019):
 
 ```
-results = afscgap.query(
-    year=(2015, 2019),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(min_val=2015, max_val=2019)   # Note min/max_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 For more advanced filters, please see manual filtering below.
 
 <br>
 
 #### Manual filtering
 Users may provide advanced queries using Oracle's REST API query parameters. For example, this queries for 2021 records with haul from the Gulf of Alaska in a specific geographic area:
 
 ```
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    latitude_dd={'$between': [56, 57]},
-    longitude_dd={'$between': [-161, -160]}
-)
+# Query with ORDS syntax
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_latitude({'$between': [56, 57]})
+query.filter_longitude({'$between': [-161, -160]})
+results = query.execute()
 
+# Summarize
 count_by_common_name = {}
 
 for record in results:
     common_name = record.get_common_name()
     new_count = record.get_count()
     count = count_by_common_name.get(common_name, 0) + new_count
     count_by_common_name[common_name] = count
+
+# Print
+print(count_by_common_name['walleye pollock'])
 ```
 
 For more info about the options available, consider the [Oracle docs](https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.2/aelig/developing-REST-applications.html#GUID-F0A4D4F9-443B-4EB9-A1D3-1CDE0A8BAFF2) or a helpful unaffiliated [getting started tutorial from Jeff Smith](https://www.thatjeffsmith.com/archive/2019/09/some-query-filtering-examples-in-ords/).
 
 <br>
 
 #### Manual pagination
 By default, the library will iterate through all results and handle pagination behind the scenes. However, one can also request an individual page:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap 
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+results = query.execute()
 
-results_for_page = results.get_page(offset=20, limit=100)
-print(len(results_for_page))  # Will print 32 (results contains 52 records)
+results_for_page = results.get_page(offset=20, limit=53)
+print(len(results_for_page))
 ```
 
 Client code can also change the pagination behavior used when iterating:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica',
-    start_offset=10,
-    limit=200
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_start_offset(10)
+query.set_limit(200)
+query.set_filter_incomplete(True)
+results = query.execute()
 
 for record in results:
-    print(record.get_bottom_temperature_c())
+    print(record.get_bottom_temperature(units='c'))
 ```
 
 Note that records are only requested once during iteration and only after the prior page has been returned via the iterator ("lazy" loading).
 
 <br>
 <br>
 
@@ -351,53 +451,53 @@
 
 <br>
 
 #### Filters and getters
 
 These fields are available as getters on `afscgap.model.Record` (`result.get_srvy()`) and may be used as optional filters on the query `asfcgagp.query(srvy='GOA')`. Fields which are `Optional` have two getters. First, the "regular" getter (`result.get_count()`) will assert that the field is not None before returning a non-optional. The second "maybe" getter (`result.get_count_maybe()`) will return None if the value was not provided or could not be parsed.
 
-| **Filter keyword**    | **Regular Getter**                   | **Maybe Getter**                                     |
-|-----------------------|--------------------------------------|------------------------------------------------------|
-| year                  | get_year() -> float                  |                                                      |
-| srvy                  | get_srvy() -> str                    |                                                      |
-| survey                | get_survey() -> str                  |                                                      |
-| survey_id             | get_survey_id() -> float             |                                                      |
-| cruise                | get_cruise() -> float                |                                                      |
-| haul                  | get_haul() -> float                  |                                                      |
-| stratum               | get_stratum() -> float               |                                                      |
-| station               | get_station() -> str                 |                                                      |
-| vessel_name           | get_vessel_name() -> str             |                                                      |
-| vessel_id             | get_vessel_id() -> float             |                                                      |
-| date_time             | get_date_time() -> str               |                                                      |
-| latitude_dd           | get_latitude_dd() -> float           |                                                      |
-| longitude_dd          | get_longitude_dd() -> float          |                                                      |
-| species_code          | get_species_code() -> float          |                                                      |
-| common_name           | get_common_name() -> str             |                                                      |
-| scientific_name       | get_scientific_name() -> str         |                                                      |
-| taxon_confidence      | get_taxon_confidence() -> str        |                                                      |
-| cpue_kgha             | get_cpue_kgha() -> float             | get_cpue_kgha_maybe() -> Optional[float]             |
-| cpue_kgkm2            | get_cpue_kgkm2() -> float            | get_cpue_kgkm2_maybe() -> Optional[float]            |
-| cpue_kg1000km2        | get_cpue_kg1000km2() -> float        | get_cpue_kg1000km2_maybe() -> Optional[float]        |
-| cpue_noha             | get_cpue_noha() -> float             | get_cpue_noha_maybe() -> Optional[float]             |
-| cpue_nokm2            | get_cpue_nokm2() -> float            | get_cpue_nokm2_maybe() -> Optional[float]            |
-| cpue_no1000km2        | get_cpue_no1000km2() -> float        | get_cpue_no1000km2_maybe() -> Optional[float]        |
-| weight_kg             | get_weight_kg() -> float             | get_weight_kg_maybe() -> Optional[float]             |
-| count                 | get_count() -> float                 | get_count_maybe() -> Optional[float]                 |
-| bottom_temperature_c  | get_bottom_temperature_c() -> float  | get_bottom_temperature_c_maybe() -> Optional[float]  |
-| surface_temperature_c | get_surface_temperature_c() -> float | get_surface_temperature_c_maybe() -> Optional[float] |
-| depth_m               | get_depth_m() -> float               |                                                      |
-| distance_fished_km    | get_distance_fished_km() -> float    |                                                      |
-| net_width_m           | get_net_width_m() -> float           | get_net_width_m_maybe() -> Optional[float]           |
-| net_height_m          | get_net_height_m() -> float          | get_net_height_m_maybe() -> Optional[float]          |
-| area_swept_ha         | get_area_swept_ha() -> float         |                                                      |
-| duration_hr           | get_duration_hr() -> float           |                                                      |
-| tsn                   | get_tsn() -> int                     | get_tsn_maybe() -> Optional[int]                     |
-| ak_survey_id          | get_ak_survey_id() -> int            |                                                      |
+| **API Field**         | **Filter on Query**                      | **Regular Getter**                             | **Maybe Getter**                                                |
+|-----------------------|------------------------------------------|------------------------------------------------|-----------------------------------------------------------------|
+| year                  | filter_year()                            | get_year() -> float                            |                                                                 |
+| srvy                  | filter_srvy()                            | get_srvy() -> str                              |                                                                 |
+| survey                | filter_survey()                          | get_survey() -> str                            |                                                                 |
+| survey_id             | filter_survey_id()                       | get_survey_id() -> float                       |                                                                 |
+| cruise                | filter_cruise()                          | get_cruise() -> float                          |                                                                 |
+| haul                  | filter_haul()                            | get_haul() -> float                            |                                                                 |
+| stratum               | filter_stratum()                         | get_stratum() -> float                         |                                                                 |
+| station               | filter_station()                         | get_station() -> str                           |                                                                 |
+| vessel_name           | filter_vessel_name()                     | get_vessel_name() -> str                       |                                                                 |
+| vessel_id             | filter_vessel_id()                       | get_vessel_id() -> float                       |                                                                 |
+| date_time             | filter_date_time()                       | get_date_time() -> str                         |                                                                 |
+| latitude_dd           | filter_latitude(units='dd')              | get_latitude(units='dd') -> float              |                                                                 |
+| longitude_dd          | filter_longitude(units='dd')             | get_longitude(units='dd') -> float             |                                                                 |
+| species_code          | filter_species_code()                    | get_species_code() -> float                    |                                                                 |
+| common_name           | filter_common_name()                     | get_common_name() -> str                       |                                                                 |
+| scientific_name       | filter_scientific_name()                 | get_scientific_name() -> str                   |                                                                 |
+| taxon_confidence      | filter_taxon_confidence()                | get_taxon_confidence() -> str                  |                                                                 |
+| cpue_kgha             | filter_cpue_weight(units='kg/ha')        | get_cpue_weight(units='kg/ha') -> float        | get_cpue_weight_maybe(units='kg/ha') -> Optional[float]         |
+| cpue_kgkm2            | filter_cpue_weight(units='kg/km2')       | get_cpue_weight(units='kg/km2') -> float       | get_cpue_weight_maybe(units='kg/km2') -> Optional[float]        |
+| cpue_kg1000km2        | filter_cpue_weight(units='kg1000/km2')   | get_cpue_weight(units='kg1000/km2') -> float   | get_cpue_weight_maybe(units='kg1000/km2') -> Optional[float]    |
+| cpue_noha             | filter_cpue_count(units='count/ha')      | get_cpue_count(units='count/ha') -> float      | get_cpue_count_maybe(units='count/ha') -> Optional[float]       |
+| cpue_nokm2            | filter_cpue_count(units='count/km2')     | get_cpue_count(units='count/km2') -> float     | get_cpue_count_maybe(units='count/km2') -> Optional[float]      |
+| cpue_no1000km2        | filter_cpue_count(units='count1000/km2') | get_cpue_count(units='count1000/km2') -> float | get_cpue_count_maybe(units='count1000/km2') -> Optional[float]  |
+| weight_kg             | filter_weight(units='kg')                | get_weight(units='kg') -> float                | get_weight_maybe() -> Optional[float]                           |
+| count                 | filter_count()                           | get_count() -> float                           | get_count_maybe() -> Optional[float]                            |
+| bottom_temperature_c  | filter_bottom_temperature(units='c')     | get_bottom_temperature(units='c') -> float     | get_bottom_temperature_maybe(units='c') -> Optional[float]      |
+| surface_temperature_c | filter_surface_temperature(units='c')    | get_surface_temperature(units='c') -> float    | get_surface_temperature_maybe() -> Optional[float]              |
+| depth_m               | filter_depth(units='m')                  | get_depth(units='m') -> float                  |                                                                 |
+| distance_fished_km    | filter_distance_fished(units='km')       | get_distance_fished(units='km') -> float       |                                                                 |
+| net_width_m           | filter_net_width(units='m')              | get_net_width(units='m') -> float              | get_net_width(units='m') -> Optional[float]                     |
+| net_height_m          | filter_net_height(units='m')             | get_net_height(units='m') -> float             | get_net_height(units='m') -> Optional[float]                    |
+| area_swept_ha         | filter_area_swept(units='ha')            | get_area_swept(units='ha') -> float            |                                                                 |
+| duration_hr           | filter_duration(units='hr')              | get_duration(units='hr') -> float              |                                                                 |
+| tsn                   | filter_tsn()                             | get_tsn() -> int                               | get_tsn_maybe() -> Optional[int]                                |
+| ak_survey_id          | filter_ak_survey_id()                    | get_ak_survey_id() -> int                      |                                                                 |
 
-`Record` objects also have a `is_complete` method which returns true if all the fields with an `Optional` type are non-None and the `date_time` could be parsed and made into an ISO 8601 string.
+Support for additional units are available for some fields and are calculated on the fly within the `afscgap` library when requested. `Record` objects also have a `is_complete` method which returns true if all the fields with an `Optional` type are non-None and the `date_time` could be parsed and made into an ISO 8601 string.
 
 <br>
 <br>
 
 ## Absence vs presence data
 The API itself provides access to presence only data. This means that records are only given for when a species was found. This can cause issues if trying to aggregate data like, for example, to determine the weight of the species in a region in terms of catch weight per hectare. The AFSC GAP API on its own would not necessarily provide the total nubmer of hecatres surveyed in that region because hauls without the species present would be excluded. That in mind, this library provides a method for inferring absence data.
 
@@ -409,30 +509,30 @@
 ```
 import afscgap
 import geolib.geohash
 import toolz.itertoolz
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+results = query.execute()
 
 def simplify_record(full_record):
-    latitude = full_record.get_latitude_dd()
-    longitude = full_record.get_longitude_dd()
+    latitude = full_record.get_latitude(units='dd')
+    longitude = full_record.get_longitude(units='dd')
     geohash = geolib.geohash.encode(latitude, longitude, 5)
     
     return {
         'geohash': geohash,
-        'area': full_record.get_area_swept_ha(),
-        'weight': full_record.get_weight_kg()
+        'area': full_record.get_area_swept(units='ha'),
+        'weight': full_record.get_weight(units='kg')
     }
 
 def combine_record(a, b):
     assert a['geohash'] == b['geohash']
     return {
         'geohash': a['geohash'],
         'area': a['area'] + b['area'],
@@ -495,21 +595,21 @@
 import afscgap
 import afscgap.inference
 
 with open('hauls.csv') as f:
     rows = csv.DictReader(f)
     hauls = [afscgap.inference.parse_haul(row) for row in rows]
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False,
-    hauls_prefetch=hauls
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+query.set_hauls_prefetch(hauls)
+results = query.execute()
 ```
 
 This can be helpful when executing a lot of queries and the bandwidth to download the [hauls metadata file](https://pyafscgap.org/community/hauls.csv) multiple times may not be desireable. 
 
 <br>
 <br>
 
@@ -517,35 +617,44 @@
 There are a few caveats for working with these data that are important for researchers to understand.
 
 <br>
 
 #### Incomplete or invalid records
 Metadata fields such as `year` are always required to make a `Record` whereas others such as catch weight `cpue_kgkm2` are not present on all records returned by the API and are optional. See the [data structure section](#data-structure) for additional details. For fields with optional values:
 
- - A maybe getter (like `get_cpue_kgkm2_maybe`) is provided which will return None without error if the value is not provided or could not be parsed.
- - A regular getter (like `get_cpue_kgkm2`) is provided which asserts the value is not None before it is returned.
+ - A maybe getter (like `get_cpue_weight_maybe`) is provided which will return None without error if the value is not provided or could not be parsed.
+ - A regular getter (like `get_cpue_weight`) is provided which asserts the value is not None before it is returned.
 
 `Record` objects also have an `is_complete` method which returns true if both all optional fields on the `Record` are non-None and the `date_time` field on the `Record` is a valid ISO 8601 string. By default, records for which `is_complete` are false are returned when iterating or through `get_page` but this can be overridden by with the `filter_incomplete` keyword argument like so:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica',
-    filter_incomplete=True
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+query.set_filter_incomplete(True)
+results = query.execute()
 
 for result in results:
     assert result.is_complete()
 ```
 
 Results returned by the API for which non-Optional fields could not be parsed (like missing `year`) are considered "invalid" and always excluded during iteration when those raw unreadable records are kept in a `queue.Queue[dict]` that can be accessed via `get_invalid` like so:
 
 ```
-results = afscgap.query(year=2021, srvy='GOA')
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
 valid = list(results)
 
 invalid_queue = results.get_invalid()
 percent_invalid = invalid_queue.qsize() / len(valid) * 100
 print('Percent invalid: %%%.2f' % percent_invalid)
 
 complete = filter(lambda x: x.is_complete(), valid)
@@ -567,33 +676,50 @@
 ## License
 We are happy to make this library available under the BSD 3-Clause license. See LICENSE for more details. (c) 2023 Regents of University of California. See the [Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu).
 
 <br>
 <br>
 
+## Local development
+After installing dev dependencies (`pip install -e .[dev]`), we recommend the following local checks:
+
+```
+$ nose2 --start-dir=afscgap
+$ mypy afscgap/*.py
+$ pyflakes afscgap/*.py
+$ pycodestyle afscgap/*.py
+```
+
+Note these checks are run by CI / CD. Also, `afscgapviz` has separate tests as described in the [visualization readme](https://github.com/SchmidtDSE/afscgap/blob/main/afscgapviz/README.md).
+
+<br>
+<br>
+
 ## Community
 Thanks for your support! Pull requests and issues very welcome.
 
 <br>
 
 #### Contribution guidelines
 We invite contributions via [our project Github](https://github.com/SchmidtDSE/afscgap). Please read the [CONTRIBUTING.md](https://github.com/SchmidtDSE/afscgap/blob/main/CONTRIBUTING.md) file for more information.
 
 <br>
 
 #### Debugging
 While participating in the community, you may need to debug URL generation. Therefore, for investigating issues or evaluating the underlying operations, you can also request a full URL for a query:
 
 ```
-results = afscgap.query(
-    year=2021,
-    latitude_dd={'$between': [56, 57]},
-    longitude_dd={'$between': [-161, -160]}
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_latitude(eq={'$between': [56, 57]})
+query.filter_longitude(eq={'$between': [-161, -160]})
+results = query.execute()
 
 print(results.get_page_url(limit=10, offset=0))
 ```
 
 The query can be executed by making an HTTP GET request at the provided location.
 
 <br>
```

### Comparing `afscgap-0.0.7/pyproject.toml` & `afscgap-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "afscgap"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="A Samuel Pottinger", email="sam.pottinger@berkeley.edu" },
 ]
 description = "Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `afscgap-0.0.7/PKG-INFO` & `afscgap-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afscgap
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP.
 Project-URL: Homepage, https://pyafscgap.org
 Project-URL: Documentation, https://pyafscgap.org/devdocs/afscgap.html
 Project-URL: Source, https://github.com/SchmidtDSE/afscgap
 Project-URL: Issue Tracker, https://github.com/SchmidtDSE/afscgap/issues
 Project-URL: Changelog, https://github.com/SchmidtDSE/afscgap#version-history
 Author-email: A Samuel Pottinger <sam.pottinger@berkeley.edu>
@@ -26,22 +26,24 @@
 Requires-Dist: pdoc; extra == 'dev'
 Requires-Dist: pycodestyle; extra == 'dev'
 Requires-Dist: pyflakes; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Requires-Dist: types-requests; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# AFSC GAP for Python
-Python-based tool chain for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program).
+# Python Tools for AFSC GAP
+Python-based tool chain ("Pyafscgap.org") for working with the public bottom trawl surveys data from the [NOAA AFSC GAP](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). This provides information about where certain species were seen and when under what conditions, information useful for research in ocean health.
+
+<br>
 
 | Group | Badges |
 |-------|--------|
 | Status | ![build workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/build.yml/badge.svg?branch=main) ![docs workflow status](https://github.com/SchmidtDSE/afscgap/actions/workflows/docs.yml/badge.svg?branch=main) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) |
 | Usage | [![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/) [![Pypi Badge](https://img.shields.io/pypi/v/afscgap)](https://pypi.org/project/afscgap/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) |
-| Publication | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) |
+| Publication | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb) [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/4905407/tree/v1)|
 
 See [webpage](https://pyafscgap.org), [project Github](https://github.com/SchmidtDSE/afscgap), and [example notebook](https://mybinder.org/v2/gh/SchmidtDSE/afscgap/main?urlpath=/tree/index.ipynb).
 
 <br>
 <br>
 
 ## Quickstart
@@ -63,15 +65,15 @@
 <br>
 
 ## Purpose
 Unofficial Python-based tool set for interacting with [bottom trawl surveys](https://www.fisheries.noaa.gov/alaska/commercial-fishing/alaska-groundfish-bottom-trawl-survey-data) from the [Ground Fish Assessment Program (GAP)](https://www.fisheries.noaa.gov/contact/groundfish-assessment-program). It offers:
 
  - Pythonic access to the official [NOAA AFSC GAP API service](https://www.fisheries.noaa.gov/foss/f?p=215%3A28).
  - Tools for inference of the "negative" observations not provided by the API service.
- - Visualization tools for quickly exploring and creating comparisons within the datset, including for audiences with limited programming experience.
+ - Visualization tools for quickly exploring and creating comparisons within the dataset, including for audiences with limited programming experience.
 
 Note that GAP is an excellent dataset produced by the [Resource Assessment and Conservation Engineering (RACE) Division](https://www.fisheries.noaa.gov/about/resource-assessment-and-conservation-engineering-division) of the [Alaska Fisheries Science Center (AFSC)](https://www.fisheries.noaa.gov/about/alaska-fisheries-science-center) as part of the National Oceanic and Atmospheric Administration's Fisheries organization ([NOAA Fisheries](https://www.fisheries.noaa.gov/)).
 
 <br>
 
 #### Needs
 Scientists and developers working on ocean health have an interest in survey data from organizations like [NOAA Fisheries](https://www.fisheries.noaa.gov/). However,
@@ -107,108 +109,172 @@
 
 #### Visual analytics
 Visualization tools are available to help both programmers and non-programmers start their investigation, providing a UI that stands on the other functionality provided by this project. This is available online at [https://app.pyafscgap.org](https://app.pyafscgap.org). It can generate both CSV (spreadsheet) exports and Python query code to move investigations to their next steps. To self-host or run this tool locally, see the [visualization readme](https://github.com/SchmidtDSE/afscgap/blob/main/afscgapviz/README.md).
 
 <br>
 
 #### Basic queries
-The `afscgap.query` method is the main entry point into Python-based utilization. Calls can be written manually or generated in the [visual analytics tool](https://app.pyafscgap.org). For example, this requests all records of Pasiphaea pacifica in 2021 from the Gulf of Alaska to get the median bottom temperature when they were observed:
+The `afscgap.Query` object is the main entry point into Python-based utilization. Calls can be written manually or generated in the [visual analytics tool](https://app.pyafscgap.org). For example, this requests all records of Pasiphaea pacifica in 2021 from the Gulf of Alaska to get the median bottom temperature when they were observed:
 
 ```
 import statistics
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Build query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
-temperatures = [record.get_bottom_temperature_c() for record in results]
+# Get temperatures in Celsius
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+
+# Take the median
 print(statistics.median(temperatures))
 ```
 
-Note that `afscgap.query` returns a [Cursor](https://pyafscgap.org/devdocs/afscgap/cursor.html#Cursor). One can iterate over this `Cursor` to access [Record](https://pyafscgap.org/devdocs/afscgap/model.html#Record) objects. You can do this with list comprehensions, maps, etc or with a good old for loop like in this example which gets a histogram of haul temperatures:
+Note that `afscgap.Query.execute` returns a [Cursor](https://pyafscgap.org/devdocs/afscgap/cursor.html#Cursor). One can iterate over this `Cursor` to access [Record](https://pyafscgap.org/devdocs/afscgap/model.html#Record) objects. You can do this with list comprehensions, maps, etc or with a good old for loop like in this example which gets a histogram of haul temperatures:
 
 ```
+# Mapping from temperature in Celsius to count
 count_by_temperature_c = {}
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Build query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
+# Iterate through results and count
 for record in results:
-    temp = record.get_bottom_temperature_c()
+    temp = record.get_bottom_temperature(units='c')
     temp_rounded = round(temp)
     count = count_by_temperature_c.get(temp_rounded, 0) + 1
     count_by_temperature_c[temp_rounded] = count
 
+# Print the result
 print(count_by_temperature_c)
 ```
 
 See [data structure section](#data-structure). Using an iterator will have the library negotiate pagination behind the scenes so this operation will cause multiple HTTP requests while the iterator runs.
 
 <br>
 
 #### Enable absence data
 One of the major limitations of the official API is that it only provides presence data. However, this library can optionally infer absence or "zero catch" records using a separate static file produced by NOAA AFSC GAP. The [algorithm and details for absence inference](#absence-vs-presence-data) is further discussed below.
 
-Absence data / "zero catch" records inference can be turned on by setting `presence_only` to false in `query`. To demonstrate, this example finds total area swept and total weight for Gadus macrocephalus from the Aleutian Islands in 2021:
+Absence data / "zero catch" records inference can be turned on by passing `False` to `set_presence_only` in `Query`. To demonstrate, this example finds total area swept and total weight for Gadus macrocephalus from the Aleutian Islands in 2021:
 
 ```
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+results = query.execute()
 
 total_area = 0
 total_weight = 0
 
 for record in results:
-    total_area += record.get_area_swept_ha()
-    total_weight += record.get_weight()
+    total_area += record.get_area_swept(units='ha')
+    total_weight += record.get_weight(units='kg')
 
 template = '%.2f kg / hectare swept (%.1f kg, %.1f hectares'
 weight_per_area = total_weight / total_area
 message = template % (weight_per_area, total_weight, total_area)
 
 print(message)
 ```
 
 For more [details on the zero catch record feature](#absence-vs-presence-data), please see below.
 
 <br>
 
+#### Chaining
+It is possible to use the Query object for method chaining.
+
+```
+import statistics
+
+import afscgap
+
+# Build query
+results = afscgap.Query() \
+    .filter_year(eq=2021) \
+    .filter_srvy(eq='GOA') \
+    .filter_scientific_name(eq='Pasiphaea pacifica') \
+    .execute()
+
+# Get temperatures in Celsius
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+
+# Take the median
+print(statistics.median(temperatures))
+```
+
+Each filter and set method on Query returns the same query object.
+
+<br>
+
+#### Builder operations
+Note that Query is a builder. So, it may be used to execute a search and then execute another search with slightly modified parameters:
+
+```
+import statistics
+
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+
+# Get temperatures in Celsius for 2021
+query.filter_year(eq=2021)
+results = query.execute()
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+print(statistics.median(temperatures))
+
+# Get temperatures in Celsius for 2019
+query.filter_year(eq=2019)
+results = query.execute()
+temperatures = [record.get_bottom_temperature(units='c') for record in results]
+print(statistics.median(temperatures))
+```
+
+When calling filter, all prior filters on the query object for that field are overwritten.
+
+<br>
+
 #### Serialization
 Users may request a dictionary representation:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Create a query
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
 # Get dictionary from individual record
 for record in results:
     dict_representation = record.to_dict()
     print(dict_representation['bottom_temperature_c'])
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+# Execute again
+results = query.execute()
 
 # Get dictionary for all records
 results_dicts = results.to_dicts()
 
 for record in results_dicts:
     print(record['bottom_temperature_c'])
 ```
@@ -221,114 +287,148 @@
 The dictionary form of the data can be used to create a Pandas dataframe:
 
 ```
 import pandas
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
 
 pandas.DataFrame(results.to_dicts())
 ```
 
 Note that Pandas is not required to use this library.
 
 <br>
 
 #### Advanced filtering
 You can provide range queries which translate to ORDS or Python emulated filters. For example, the following requests before and including 2019:
 
 ```
-results = afscgap.query(
-    year=(None, 2019),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(max_val=2021)  # Note max_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 The following requests data after and including 2019:
 
 ```
-results = afscgap.query(
-    year=(2019, None),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(min_val=2021)  # Note min_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 Finally, the following requests data between 2015 and 2019 (includes 2015 and 2019):
 
 ```
-results = afscgap.query(
-    year=(2015, 2019),
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap
+
+# Build query
+query = afscgap.Query()
+query.filter_year(min_val=2015, max_val=2019)   # Note min/max_val
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
+# Sum weight
+weights = map(lambda x: x.get_weight(units='kg'), results)
+total_weight = sum(weights)
+print(total_weight)
 ```
 
 For more advanced filters, please see manual filtering below.
 
 <br>
 
 #### Manual filtering
 Users may provide advanced queries using Oracle's REST API query parameters. For example, this queries for 2021 records with haul from the Gulf of Alaska in a specific geographic area:
 
 ```
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    latitude_dd={'$between': [56, 57]},
-    longitude_dd={'$between': [-161, -160]}
-)
+# Query with ORDS syntax
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_latitude({'$between': [56, 57]})
+query.filter_longitude({'$between': [-161, -160]})
+results = query.execute()
 
+# Summarize
 count_by_common_name = {}
 
 for record in results:
     common_name = record.get_common_name()
     new_count = record.get_count()
     count = count_by_common_name.get(common_name, 0) + new_count
     count_by_common_name[common_name] = count
+
+# Print
+print(count_by_common_name['walleye pollock'])
 ```
 
 For more info about the options available, consider the [Oracle docs](https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/19.2/aelig/developing-REST-applications.html#GUID-F0A4D4F9-443B-4EB9-A1D3-1CDE0A8BAFF2) or a helpful unaffiliated [getting started tutorial from Jeff Smith](https://www.thatjeffsmith.com/archive/2019/09/some-query-filtering-examples-in-ords/).
 
 <br>
 
 #### Manual pagination
 By default, the library will iterate through all results and handle pagination behind the scenes. However, one can also request an individual page:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica'
-)
+import afscgap 
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+results = query.execute()
 
-results_for_page = results.get_page(offset=20, limit=100)
-print(len(results_for_page))  # Will print 32 (results contains 52 records)
+results_for_page = results.get_page(offset=20, limit=53)
+print(len(results_for_page))
 ```
 
 Client code can also change the pagination behavior used when iterating:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica',
-    start_offset=10,
-    limit=200
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_start_offset(10)
+query.set_limit(200)
+query.set_filter_incomplete(True)
+results = query.execute()
 
 for record in results:
-    print(record.get_bottom_temperature_c())
+    print(record.get_bottom_temperature(units='c'))
 ```
 
 Note that records are only requested once during iteration and only after the prior page has been returned via the iterator ("lazy" loading).
 
 <br>
 <br>
 
@@ -383,53 +483,53 @@
 
 <br>
 
 #### Filters and getters
 
 These fields are available as getters on `afscgap.model.Record` (`result.get_srvy()`) and may be used as optional filters on the query `asfcgagp.query(srvy='GOA')`. Fields which are `Optional` have two getters. First, the "regular" getter (`result.get_count()`) will assert that the field is not None before returning a non-optional. The second "maybe" getter (`result.get_count_maybe()`) will return None if the value was not provided or could not be parsed.
 
-| **Filter keyword**    | **Regular Getter**                   | **Maybe Getter**                                     |
-|-----------------------|--------------------------------------|------------------------------------------------------|
-| year                  | get_year() -> float                  |                                                      |
-| srvy                  | get_srvy() -> str                    |                                                      |
-| survey                | get_survey() -> str                  |                                                      |
-| survey_id             | get_survey_id() -> float             |                                                      |
-| cruise                | get_cruise() -> float                |                                                      |
-| haul                  | get_haul() -> float                  |                                                      |
-| stratum               | get_stratum() -> float               |                                                      |
-| station               | get_station() -> str                 |                                                      |
-| vessel_name           | get_vessel_name() -> str             |                                                      |
-| vessel_id             | get_vessel_id() -> float             |                                                      |
-| date_time             | get_date_time() -> str               |                                                      |
-| latitude_dd           | get_latitude_dd() -> float           |                                                      |
-| longitude_dd          | get_longitude_dd() -> float          |                                                      |
-| species_code          | get_species_code() -> float          |                                                      |
-| common_name           | get_common_name() -> str             |                                                      |
-| scientific_name       | get_scientific_name() -> str         |                                                      |
-| taxon_confidence      | get_taxon_confidence() -> str        |                                                      |
-| cpue_kgha             | get_cpue_kgha() -> float             | get_cpue_kgha_maybe() -> Optional[float]             |
-| cpue_kgkm2            | get_cpue_kgkm2() -> float            | get_cpue_kgkm2_maybe() -> Optional[float]            |
-| cpue_kg1000km2        | get_cpue_kg1000km2() -> float        | get_cpue_kg1000km2_maybe() -> Optional[float]        |
-| cpue_noha             | get_cpue_noha() -> float             | get_cpue_noha_maybe() -> Optional[float]             |
-| cpue_nokm2            | get_cpue_nokm2() -> float            | get_cpue_nokm2_maybe() -> Optional[float]            |
-| cpue_no1000km2        | get_cpue_no1000km2() -> float        | get_cpue_no1000km2_maybe() -> Optional[float]        |
-| weight_kg             | get_weight_kg() -> float             | get_weight_kg_maybe() -> Optional[float]             |
-| count                 | get_count() -> float                 | get_count_maybe() -> Optional[float]                 |
-| bottom_temperature_c  | get_bottom_temperature_c() -> float  | get_bottom_temperature_c_maybe() -> Optional[float]  |
-| surface_temperature_c | get_surface_temperature_c() -> float | get_surface_temperature_c_maybe() -> Optional[float] |
-| depth_m               | get_depth_m() -> float               |                                                      |
-| distance_fished_km    | get_distance_fished_km() -> float    |                                                      |
-| net_width_m           | get_net_width_m() -> float           | get_net_width_m_maybe() -> Optional[float]           |
-| net_height_m          | get_net_height_m() -> float          | get_net_height_m_maybe() -> Optional[float]          |
-| area_swept_ha         | get_area_swept_ha() -> float         |                                                      |
-| duration_hr           | get_duration_hr() -> float           |                                                      |
-| tsn                   | get_tsn() -> int                     | get_tsn_maybe() -> Optional[int]                     |
-| ak_survey_id          | get_ak_survey_id() -> int            |                                                      |
+| **API Field**         | **Filter on Query**                      | **Regular Getter**                             | **Maybe Getter**                                                |
+|-----------------------|------------------------------------------|------------------------------------------------|-----------------------------------------------------------------|
+| year                  | filter_year()                            | get_year() -> float                            |                                                                 |
+| srvy                  | filter_srvy()                            | get_srvy() -> str                              |                                                                 |
+| survey                | filter_survey()                          | get_survey() -> str                            |                                                                 |
+| survey_id             | filter_survey_id()                       | get_survey_id() -> float                       |                                                                 |
+| cruise                | filter_cruise()                          | get_cruise() -> float                          |                                                                 |
+| haul                  | filter_haul()                            | get_haul() -> float                            |                                                                 |
+| stratum               | filter_stratum()                         | get_stratum() -> float                         |                                                                 |
+| station               | filter_station()                         | get_station() -> str                           |                                                                 |
+| vessel_name           | filter_vessel_name()                     | get_vessel_name() -> str                       |                                                                 |
+| vessel_id             | filter_vessel_id()                       | get_vessel_id() -> float                       |                                                                 |
+| date_time             | filter_date_time()                       | get_date_time() -> str                         |                                                                 |
+| latitude_dd           | filter_latitude(units='dd')              | get_latitude(units='dd') -> float              |                                                                 |
+| longitude_dd          | filter_longitude(units='dd')             | get_longitude(units='dd') -> float             |                                                                 |
+| species_code          | filter_species_code()                    | get_species_code() -> float                    |                                                                 |
+| common_name           | filter_common_name()                     | get_common_name() -> str                       |                                                                 |
+| scientific_name       | filter_scientific_name()                 | get_scientific_name() -> str                   |                                                                 |
+| taxon_confidence      | filter_taxon_confidence()                | get_taxon_confidence() -> str                  |                                                                 |
+| cpue_kgha             | filter_cpue_weight(units='kg/ha')        | get_cpue_weight(units='kg/ha') -> float        | get_cpue_weight_maybe(units='kg/ha') -> Optional[float]         |
+| cpue_kgkm2            | filter_cpue_weight(units='kg/km2')       | get_cpue_weight(units='kg/km2') -> float       | get_cpue_weight_maybe(units='kg/km2') -> Optional[float]        |
+| cpue_kg1000km2        | filter_cpue_weight(units='kg1000/km2')   | get_cpue_weight(units='kg1000/km2') -> float   | get_cpue_weight_maybe(units='kg1000/km2') -> Optional[float]    |
+| cpue_noha             | filter_cpue_count(units='count/ha')      | get_cpue_count(units='count/ha') -> float      | get_cpue_count_maybe(units='count/ha') -> Optional[float]       |
+| cpue_nokm2            | filter_cpue_count(units='count/km2')     | get_cpue_count(units='count/km2') -> float     | get_cpue_count_maybe(units='count/km2') -> Optional[float]      |
+| cpue_no1000km2        | filter_cpue_count(units='count1000/km2') | get_cpue_count(units='count1000/km2') -> float | get_cpue_count_maybe(units='count1000/km2') -> Optional[float]  |
+| weight_kg             | filter_weight(units='kg')                | get_weight(units='kg') -> float                | get_weight_maybe() -> Optional[float]                           |
+| count                 | filter_count()                           | get_count() -> float                           | get_count_maybe() -> Optional[float]                            |
+| bottom_temperature_c  | filter_bottom_temperature(units='c')     | get_bottom_temperature(units='c') -> float     | get_bottom_temperature_maybe(units='c') -> Optional[float]      |
+| surface_temperature_c | filter_surface_temperature(units='c')    | get_surface_temperature(units='c') -> float    | get_surface_temperature_maybe() -> Optional[float]              |
+| depth_m               | filter_depth(units='m')                  | get_depth(units='m') -> float                  |                                                                 |
+| distance_fished_km    | filter_distance_fished(units='km')       | get_distance_fished(units='km') -> float       |                                                                 |
+| net_width_m           | filter_net_width(units='m')              | get_net_width(units='m') -> float              | get_net_width(units='m') -> Optional[float]                     |
+| net_height_m          | filter_net_height(units='m')             | get_net_height(units='m') -> float             | get_net_height(units='m') -> Optional[float]                    |
+| area_swept_ha         | filter_area_swept(units='ha')            | get_area_swept(units='ha') -> float            |                                                                 |
+| duration_hr           | filter_duration(units='hr')              | get_duration(units='hr') -> float              |                                                                 |
+| tsn                   | filter_tsn()                             | get_tsn() -> int                               | get_tsn_maybe() -> Optional[int]                                |
+| ak_survey_id          | filter_ak_survey_id()                    | get_ak_survey_id() -> int                      |                                                                 |
 
-`Record` objects also have a `is_complete` method which returns true if all the fields with an `Optional` type are non-None and the `date_time` could be parsed and made into an ISO 8601 string.
+Support for additional units are available for some fields and are calculated on the fly within the `afscgap` library when requested. `Record` objects also have a `is_complete` method which returns true if all the fields with an `Optional` type are non-None and the `date_time` could be parsed and made into an ISO 8601 string.
 
 <br>
 <br>
 
 ## Absence vs presence data
 The API itself provides access to presence only data. This means that records are only given for when a species was found. This can cause issues if trying to aggregate data like, for example, to determine the weight of the species in a region in terms of catch weight per hectare. The AFSC GAP API on its own would not necessarily provide the total nubmer of hecatres surveyed in that region because hauls without the species present would be excluded. That in mind, this library provides a method for inferring absence data.
 
@@ -441,30 +541,30 @@
 ```
 import afscgap
 import geolib.geohash
 import toolz.itertoolz
 
 import afscgap
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+results = query.execute()
 
 def simplify_record(full_record):
-    latitude = full_record.get_latitude_dd()
-    longitude = full_record.get_longitude_dd()
+    latitude = full_record.get_latitude(units='dd')
+    longitude = full_record.get_longitude(units='dd')
     geohash = geolib.geohash.encode(latitude, longitude, 5)
     
     return {
         'geohash': geohash,
-        'area': full_record.get_area_swept_ha(),
-        'weight': full_record.get_weight_kg()
+        'area': full_record.get_area_swept(units='ha'),
+        'weight': full_record.get_weight(units='kg')
     }
 
 def combine_record(a, b):
     assert a['geohash'] == b['geohash']
     return {
         'geohash': a['geohash'],
         'area': a['area'] + b['area'],
@@ -527,21 +627,21 @@
 import afscgap
 import afscgap.inference
 
 with open('hauls.csv') as f:
     rows = csv.DictReader(f)
     hauls = [afscgap.inference.parse_haul(row) for row in rows]
 
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Gadus macrocephalus',
-    presence_only=False,
-    hauls_prefetch=hauls
-)
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Gadus macrocephalus')
+query.set_presence_only(False)
+query.set_hauls_prefetch(hauls)
+results = query.execute()
 ```
 
 This can be helpful when executing a lot of queries and the bandwidth to download the [hauls metadata file](https://pyafscgap.org/community/hauls.csv) multiple times may not be desireable. 
 
 <br>
 <br>
 
@@ -549,35 +649,44 @@
 There are a few caveats for working with these data that are important for researchers to understand.
 
 <br>
 
 #### Incomplete or invalid records
 Metadata fields such as `year` are always required to make a `Record` whereas others such as catch weight `cpue_kgkm2` are not present on all records returned by the API and are optional. See the [data structure section](#data-structure) for additional details. For fields with optional values:
 
- - A maybe getter (like `get_cpue_kgkm2_maybe`) is provided which will return None without error if the value is not provided or could not be parsed.
- - A regular getter (like `get_cpue_kgkm2`) is provided which asserts the value is not None before it is returned.
+ - A maybe getter (like `get_cpue_weight_maybe`) is provided which will return None without error if the value is not provided or could not be parsed.
+ - A regular getter (like `get_cpue_weight`) is provided which asserts the value is not None before it is returned.
 
 `Record` objects also have an `is_complete` method which returns true if both all optional fields on the `Record` are non-None and the `date_time` field on the `Record` is a valid ISO 8601 string. By default, records for which `is_complete` are false are returned when iterating or through `get_page` but this can be overridden by with the `filter_incomplete` keyword argument like so:
 
 ```
-results = afscgap.query(
-    year=2021,
-    srvy='GOA',
-    scientific_name='Pasiphaea pacifica',
-    filter_incomplete=True
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+query.set_filter_incomplete(True)
+results = query.execute()
 
 for result in results:
     assert result.is_complete()
 ```
 
 Results returned by the API for which non-Optional fields could not be parsed (like missing `year`) are considered "invalid" and always excluded during iteration when those raw unreadable records are kept in a `queue.Queue[dict]` that can be accessed via `get_invalid` like so:
 
 ```
-results = afscgap.query(year=2021, srvy='GOA')
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_srvy(eq='GOA')
+query.filter_scientific_name(eq='Pasiphaea pacifica')
+results = query.execute()
+
 valid = list(results)
 
 invalid_queue = results.get_invalid()
 percent_invalid = invalid_queue.qsize() / len(valid) * 100
 print('Percent invalid: %%%.2f' % percent_invalid)
 
 complete = filter(lambda x: x.is_complete(), valid)
@@ -599,33 +708,50 @@
 ## License
 We are happy to make this library available under the BSD 3-Clause license. See LICENSE for more details. (c) 2023 Regents of University of California. See the [Eric and Wendy Schmidt Center for Data Science and the Environment
 at UC Berkeley](https://dse.berkeley.edu).
 
 <br>
 <br>
 
+## Local development
+After installing dev dependencies (`pip install -e .[dev]`), we recommend the following local checks:
+
+```
+$ nose2 --start-dir=afscgap
+$ mypy afscgap/*.py
+$ pyflakes afscgap/*.py
+$ pycodestyle afscgap/*.py
+```
+
+Note these checks are run by CI / CD. Also, `afscgapviz` has separate tests as described in the [visualization readme](https://github.com/SchmidtDSE/afscgap/blob/main/afscgapviz/README.md).
+
+<br>
+<br>
+
 ## Community
 Thanks for your support! Pull requests and issues very welcome.
 
 <br>
 
 #### Contribution guidelines
 We invite contributions via [our project Github](https://github.com/SchmidtDSE/afscgap). Please read the [CONTRIBUTING.md](https://github.com/SchmidtDSE/afscgap/blob/main/CONTRIBUTING.md) file for more information.
 
 <br>
 
 #### Debugging
 While participating in the community, you may need to debug URL generation. Therefore, for investigating issues or evaluating the underlying operations, you can also request a full URL for a query:
 
 ```
-results = afscgap.query(
-    year=2021,
-    latitude_dd={'$between': [56, 57]},
-    longitude_dd={'$between': [-161, -160]}
-)
+import afscgap
+
+query = afscgap.Query()
+query.filter_year(eq=2021)
+query.filter_latitude(eq={'$between': [56, 57]})
+query.filter_longitude(eq={'$between': [-161, -160]})
+results = query.execute()
 
 print(results.get_page_url(limit=10, offset=0))
 ```
 
 The query can be executed by making an HTTP GET request at the provided location.
 
 <br>
```

