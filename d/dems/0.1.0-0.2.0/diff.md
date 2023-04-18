# Comparing `tmp/dems-0.1.0.tar.gz` & `tmp/dems-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dems-0.1.0.tar", max compression
+gzip compressed data, was "dems-0.2.0.tar", max compression
```

## Comparing `dems-0.1.0.tar` & `dems-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1064 2022-10-25 14:17:19.826939 dems-0.1.0/LICENSE
--rw-r--r--   0        0        0       31 2022-10-25 14:17:19.827016 dems-0.1.0/README.md
--rw-r--r--   0        0        0       94 2023-02-17 06:33:56.913056 dems-0.1.0/dems/__init__.py
--rw-r--r--   0        0        0     1182 2023-01-16 15:11:16.752367 dems-0.1.0/dems/d1.py
--rw-r--r--   0        0        0     6792 2023-02-17 06:25:38.540246 dems-0.1.0/dems/d2.py
--rw-r--r--   0        0        0        0 2023-01-16 15:11:16.752894 dems-0.1.0/dems/py.typed
--rw-r--r--   0        0        0      517 2023-02-17 06:33:56.914201 dems-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 dems-0.1.0/setup.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 dems-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 12:33:28.758332 dems-0.2.0/LICENSE
+-rw-r--r--   0        0        0       31 2023-04-18 12:33:28.758332 dems-0.2.0/README.md
+-rw-r--r--   0        0        0       94 2023-04-18 12:33:28.758332 dems-0.2.0/dems/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-18 12:33:28.758332 dems-0.2.0/dems/d1.py
+-rw-r--r--   0        0        0     6975 2023-04-18 12:33:28.758332 dems-0.2.0/dems/d2.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:33:28.758332 dems-0.2.0/dems/py.typed
+-rw-r--r--   0        0        0      509 2023-04-18 12:33:28.758332 dems-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 dems-0.2.0/PKG-INFO
```

### Comparing `dems-0.1.0/LICENSE` & `dems-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dems-0.1.0/dems/d1.py` & `dems-0.2.0/dems/d1.py`

 * *Files identical despite different names*

### Comparing `dems-0.1.0/dems/d2.py` & `dems-0.2.0/dems/d2.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 
 
 # type hints
 Ti = Literal["time"]
 Ch = Literal["chan"]
 
 
+# constants
+ASTE_ITRS_COORDS = (
+    +2230817.2140945992,
+    -5440188.022176585,
+    -2475718.801708271,
+)
+DEMS_VERSION = "v0.2.0"
+DMERGE_VERSION = "v1.0.0"
+
+
 @dataclass
 class Data_:
     data: Data[Tuple[Ti, Ch], Any]
     long_name: Attr[str] = "Data values"
 
 
 @dataclass
@@ -30,41 +40,41 @@
 @dataclass
 class Weight:
     data: Data[Tuple[Ti, Ch], float]
     long_name: Attr[str] = "Data weights"
 
 
 @dataclass
-class Chan:
-    data: Data[Ch, int]
-    long_name: Attr[str] = "Generic channel"
-
-
-@dataclass
 class Time:
     data: Data[Ti, Literal["datetime64[ns]"]]
     long_name: Attr[str] = "Start time in UTC"
 
 
 @dataclass
+class Chan:
+    data: Data[Ch, int]
+    long_name: Attr[str] = "Channel ID"
+
+
+@dataclass
 class Beam:
     data: Data[Ti, str]
-    long_name: Attr[str] = "Beam ID"
+    long_name: Attr[str] = "Beam label"
 
 
 @dataclass
 class Scan:
     data: Data[Ti, str]
-    long_name: Attr[str] = "Scan ID"
+    long_name: Attr[str] = "Scan label"
 
 
 @dataclass
 class State:
     data: Data[Ti, str]
-    long_name: Attr[str] = "State ID"
+    long_name: Attr[str] = "State label"
 
 
 @dataclass
 class Lon:
     data: Data[Ti, float]
     long_name: Attr[str] = "Sky longitude"
     units: Attr[str] = "deg"
@@ -94,73 +104,52 @@
 @dataclass
 class Frame:
     data: Data[Tuple[()], str]
     long_name: Attr[str] = "Sky coordinate frame"
 
 
 @dataclass
-class GroundTemperature:
-    data: Data[Ti, float]
-    long_name: Attr[str] = "Ground temperature"
-    units: Attr[str] = "K"
-
-
-@dataclass
-class CabinTemperature:
+class Temperature:
     data: Data[Ti, float]
-    long_name: Attr[str] = "Cabin temperature"
+    long_name: Attr[str] = "Ground atmospheric temperature"
     units: Attr[str] = "K"
 
 
 @dataclass
 class Pressure:
     data: Data[Ti, float]
-    long_name: Attr[str] = "Atmospheric pressure"
+    long_name: Attr[str] = "Ground atmospheric pressure"
     units: Attr[str] = "Pa"
 
 
 @dataclass
 class Humidity:
     data: Data[Ti, float]
-    long_name: Attr[str] = "Relative humidity"
+    long_name: Attr[str] = "Ground relative humidity"
     units: Attr[str] = "%"
 
 
 @dataclass
 class WindSpeed:
     data: Data[Ti, float]
-    long_name: Attr[str] = "Wind speed"
+    long_name: Attr[str] = "Ground wind speed"
     units: Attr[str] = "m/s"
 
 
 @dataclass
 class WindDirection:
     data: Data[Ti, float]
-    long_name: Attr[str] = "Wind direction"
+    long_name: Attr[str] = "Ground wind direction"
     units: Attr[str] = "deg"
 
 
 @dataclass
-class Exposure:
-    data: Data[Ti, float]
-    long_name: Attr[str] = "Sample exposure time"
-    units: Attr[str] = "s"
-
-
-@dataclass
-class Interval:
-    data: Data[Ti, float]
-    long_name: Attr[str] = "Sample interval time"
-    units: Attr[str] = "s"
-
-
-@dataclass
 class Bandwidth:
     data: Data[Ch, float]
-    long_name: Attr[str] = "Channel band width"
+    long_name: Attr[str] = "Effective channel bandwidth"
     units: Attr[str] = "Hz"
 
 
 @dataclass
 class Frequency:
     data: Data[Ch, float]
     long_name: Attr[str] = "Channel center frequency"
@@ -178,136 +167,149 @@
 class BeamMinor:
     data: Data[Ch, float]
     long_name: Attr[str] = "Beam minor axis"
     units: Attr[str] = "deg"
 
 
 @dataclass
-class BeamPA:
+class BeamPa:
     data: Data[Ch, float]
     long_name: Attr[str] = "Beam position angle"
     units: Attr[str] = "deg"
 
 
 @dataclass
-class AsteSubrefX:
-    data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] Subref X position."
-    units: Attr[str] = "mm"
+class Exposure:
+    data: Data[Tuple[()], float]
+    long_name: Attr[str] = "Sample exposure time"
+    units: Attr[str] = "s"
 
 
 @dataclass
-class AsteSubrefY:
-    data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] Subref Y position."
-    units: Attr[str] = "mm"
+class Interval:
+    data: Data[Tuple[()], float]
+    long_name: Attr[str] = "Sample interval time"
+    units: Attr[str] = "s"
 
 
 @dataclass
-class AsteSubrefZ:
+class AsteCabinTemperature:
     data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] Subref Z position."
-    units: Attr[str] = "mm"
+    long_name: Attr[str] = "[ASTE] Cabin temperature"
+    units: Attr[str] = "K"
 
 
 @dataclass
-class AsteMistiAz:
+class AsteMistiLon:
     data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] MiSTI azimuth."
+    long_name: Attr[str] = "[ASTE] MiSTI sky longitude"
     units: Attr[str] = "deg"
 
 
 @dataclass
-class AsteMistiEl:
+class AsteMistiLat:
     data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] MiSTI elevation."
+    long_name: Attr[str] = "[ASTE] MiSTI sky latitude"
     units: Attr[str] = "deg"
 
 
 @dataclass
 class AsteMistiPwv:
     data: Data[Ti, float]
-    long_name: Attr[str] = "[ASTE] MiSTI PWV."
+    long_name: Attr[str] = "[ASTE] MiSTI measured PWV"
     units: Attr[str] = "mm"
 
 
 @dataclass
+class AsteMistiFrame:
+    data: Data[Tuple[()], str]
+    long_name: Attr[str] = "[ASTE] MiSTI sky coordinate frame"
+
+
+@dataclass
 class D2MkidID:
     data: Data[Ch, int]
     long_name: Attr[str] = "[DESHIMA 2.0] MKID ID"
 
 
 @dataclass
 class D2MkidType:
     data: Data[Ch, str]
     long_name: Attr[str] = "[DESHIMA 2.0] MKID type"
 
 
 @dataclass
-class D2MkidFreq:
-    data: Data[Ch, str]
-    long_name: Attr[str] = "[DESHIMA 2.0] MKID center response frequency"
+class D2MkidFrequency:
+    data: Data[Ch, float]
+    long_name: Attr[str] = "[DESHIMA 2.0] MKID center frequency"
     units: Attr[str] = "Hz"
 
 
 @dataclass
-class D2RoomChopperState:
-    data: Data[Ch, str]
-    long_name: Attr[str] = "[DESHIMA 2.0] Room chopper state"
+class D2RoomchopperIsblocking:
+    data: Data[Ti, bool]
+    long_name: Attr[str] = "[DESHIMA 2.0] Whether room chopper is blocking sensor"
 
 
 @dataclass
-class D2SkyChopperIsopen:
-    data: Data[Ch, bool]
-    long_name: Attr[str] = "[DESHIMA 2.0] Whether sky chopper is open"
+class D2SkychopperIsblocking:
+    data: Data[Ti, bool]
+    long_name: Attr[str] = "[DESHIMA 2.0] Whether sky chopper is blocking sensor"
 
 
 @dataclass(frozen=True)
 class MS(AsDataArray):
     """Measurement set of DESHIMA 2.0."""
 
+    # data
     data: Dataof[Data_]
     mask: Coordof[Mask] = False
     weight: Coordof[Weight] = 1.0
-    time: Coordof[Time] = "2020-01-01"
+    # dimensions
+    time: Coordof[Time] = "1970-01-01T00:00:00"
     chan: Coordof[Chan] = 0
+    # labels
     beam: Coordof[Beam] = ""
     scan: Coordof[Scan] = ""
     state: Coordof[State] = ""
+    # telescope pointing
     lon: Coordof[Lon] = 0.0
     lat: Coordof[Lat] = 0.0
     lon_origin: Coordof[LonOrigin] = 0.0
     lat_origin: Coordof[LatOrigin] = 0.0
     frame: Coordof[Frame] = "altaz"
-    ground_temperature: Coordof[GroundTemperature] = 0.0
-    cabin_temperature: Coordof[CabinTemperature] = 0.0
+    # weather information
+    temperature: Coordof[Temperature] = 0.0
     pressure: Coordof[Pressure] = 0.0
-    humidity: Coordof[Pressure] = 0.0
+    humidity: Coordof[Humidity] = 0.0
     wind_speed: Coordof[WindSpeed] = 0.0
     wind_direction: Coordof[WindDirection] = 0.0
-    exposure: Coordof[Exposure] = 0.0
-    interval: Coordof[Interval] = 0.0
+    # data information
     bandwidth: Coordof[Bandwidth] = 0.0
     frequency: Coordof[Frequency] = 0.0
     beam_major: Coordof[BeamMajor] = 0.0
     beam_minor: Coordof[BeamMinor] = 0.0
-    beam_pa: Coordof[BeamPA] = 0.0
+    beam_pa: Coordof[BeamPa] = 0.0
+    exposure: Coordof[Exposure] = 0.00625
+    interval: Coordof[Interval] = 0.00625
+    # observation information
     observation: Attr[str] = ""
     observer: Attr[str] = ""
     project: Attr[str] = ""
-    telescope: Attr[str] = ""
-    telescope_coords: Attr[Tuple[float, float, float]] = (0.0, 0.0, 0.0)
-    telescope_diameter: Attr[float] = 0.0
-    aste_subref_x: Coordof[AsteSubrefX] = 0.0
-    aste_subref_y: Coordof[AsteSubrefY] = 0.0
-    aste_subref_x: Coordof[AsteSubrefZ] = 0.0
-    aste_misti_az: Coordof[AsteMistiAz] = 0.0
-    aste_misti_el: Coordof[AsteMistiEl] = 0.0
+    object: Attr[str] = ""
+    telescope_name: Attr[str] = "ASTE"
+    telescope_diameter: Attr[float] = 10.0
+    telescope_coordinates: Attr[Tuple[float, float, float]] = ASTE_ITRS_COORDS
+    # ASTE specific
+    aste_cabin_temperature: Coordof[AsteCabinTemperature] = 0.0
+    aste_misti_lon: Coordof[AsteMistiLon] = 0.0
+    aste_misti_lat: Coordof[AsteMistiLat] = 0.0
     aste_misti_pwv: Coordof[AsteMistiPwv] = 0.0
+    aste_misti_frame: Coordof[AsteMistiFrame] = "altaz"
+    # DESHIMA 2.0 specific
     d2_mkid_id: Coordof[D2MkidID] = 0
     d2_mkid_type: Coordof[D2MkidType] = ""
-    d2_mkid_freq: Coordof[D2MkidFreq] = 0.0
-    d2_roomchopper_state: Coordof[D2RoomChopperState] = ""
-    d2_skychopper_isopen: Coordof[D2SkyChopperIsopen] = False
-    d2_dmerge_version: Attr[str] = ""
-    d2_ddb_version: Attr[str] = ""
-    d2_dems_version: Attr[str] = ""
+    d2_mkid_frequency: Coordof[D2MkidFrequency] = 0.0
+    d2_roomchopper_isblocking: Coordof[D2RoomchopperIsblocking] = False
+    d2_skychopper_isblocking: Coordof[D2SkychopperIsblocking] = False
+    d2_dems_version: Attr[str] = DEMS_VERSION
+    d2_dmerge_version: Attr[str] = DMERGE_VERSION
```

### Comparing `dems-0.1.0/PKG-INFO` & `dems-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dems
-Version: 0.1.0
+Version: 0.2.0
 Summary: DESHIMA measurement set
 License: MIT
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: typing-extensions (>=3.10,<5.0)
-Requires-Dist: xarray-dataclasses (>=1.4,<2.0)
+Requires-Dist: typing-extensions (>=4.0,<5.0)
+Requires-Dist: xarray-dataclasses (>=1.5,<2.0)
 Description-Content-Type: text/markdown
 
 # dems
 DESHIMA measurement set
```

