# Comparing `tmp/mxtools-1.0.2.tar.gz` & `tmp/mxtools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxtools-1.0.2.tar", last modified: Tue Jan 31 18:42:34 2023, max compression
+gzip compressed data, was "mxtools-1.0.3.tar", last modified: Tue Apr 18 14:42:23 2023, max compression
```

## Comparing `mxtools-1.0.2.tar` & `mxtools-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-31 18:42:22.000000 mxtools-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-01-31 18:42:22.000000 mxtools-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-31 18:42:22.000000 mxtools-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-31 18:42:22.000000 mxtools-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-31 18:42:34.696007 mxtools-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-31 18:42:22.000000 mxtools-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-31 18:42:22.000000 mxtools-1.0.2/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/mxtools/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-31 18:42:34.696007 mxtools-1.0.2/mxtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/governor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/raster_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/scans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/mxtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/tests/test_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/vector_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-01-31 18:42:22.000000 mxtools-1.0.2/mxtools/zebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 18:42:34.696007 mxtools-1.0.2/mxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 18:42:34.000000 mxtools-1.0.2/mxtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-31 18:42:22.000000 mxtools-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 18:42:22.000000 mxtools-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-31 18:42:34.696007 mxtools-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-01-31 18:42:22.000000 mxtools-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68714 2023-01-31 18:42:22.000000 mxtools-1.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 14:42:12.000000 mxtools-1.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-18 14:42:12.000000 mxtools-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-18 14:42:12.000000 mxtools-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 14:42:12.000000 mxtools-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 14:42:23.524594 mxtools-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 14:42:12.000000 mxtools-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.520594 mxtools-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/governor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/raster_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/scans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/test_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/vector_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/zebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 14:42:12.000000 mxtools-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:42:12.000000 mxtools-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 14:42:23.524594 mxtools-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-18 14:42:12.000000 mxtools-1.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68714 2023-04-18 14:42:12.000000 mxtools-1.0.3/versioneer.py
```

### Comparing `mxtools-1.0.2/CONTRIBUTING.rst` & `mxtools-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/LICENSE` & `mxtools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/PKG-INFO` & `mxtools-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxtools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Common code for the MX beamlines at NSLS-II (AMX, FMX).
 Home-page: https://github.com/NSLS-II-AMX/mxtools
 Author: Jun Aishima
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mxtools-1.0.2/docs/Makefile` & `mxtools-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/docs/make.bat` & `mxtools-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/docs/source/conf.py` & `mxtools-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/docs/source/min_versions.rst` & `mxtools-1.0.3/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/eiger.py` & `mxtools-1.0.3/mxtools/eiger.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/flyer.py` & `mxtools-1.0.3/mxtools/flyer.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         angle_start = kwargs["angle_start"]
         exposurePeriodPerImage = kwargs["exposure_period_per_image"]
         detector_dead_time = kwargs["detector_dead_time"]
         scanWidth = kwargs["scan_width"]
         imgWidth = kwargs["img_width"]
         numImages = kwargs["num_images"]
         self.zebra_daq_prep()
-        ttime.sleep(1.0)
+        ttime.sleep(0.5)
 
         PW = (exposurePeriodPerImage - detector_dead_time) * 1000
         PS = (exposurePeriodPerImage) * 1000
         GW = scanWidth - (1.0 - (PW / PS)) * (imgWidth / 2.0)
         self.setup_zebra_vector_scan(
             angle_start=angle_start,
             gate_width=GW,
@@ -309,15 +309,15 @@
         self.vector.start.z.put(z_um[0])
         self.vector.end.z.put(z_um[1])
         self.vector.frame_exptime.put(exposure_period_per_image * 1000.0)
         self.vector.hold.put(0)
 
     def zebra_daq_prep(self):
         self.zebra.reset.put(1)
-        ttime.sleep(2.0)  # not known why this sleep is so long (done since LSDC 1)
+        ttime.sleep(0.5)  # not known why this sleep is so long (done since LSDC 1)
         self.zebra.out1.put(31)
         self.zebra.m1_set_pos.put(1)
         self.zebra.m2_set_pos.put(1)
         self.zebra.m3_set_pos.put(1)
         self.zebra.pc.arm.trig_source.put(1)
 
     # expected zebra setup:
```

### Comparing `mxtools-1.0.2/mxtools/governor.py` & `mxtools-1.0.3/mxtools/governor.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/handlers.py` & `mxtools-1.0.3/mxtools/handlers.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/raster_flyer.py` & `mxtools-1.0.3/mxtools/raster_flyer.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         exposurePeriodPerImage = kwargs["exposure_period_per_image"]
         detector_dead_time = kwargs["detector_dead_time"]
         scanWidth = kwargs["scan_width"]
         imgWidth = kwargs["img_width"]
         numImages = kwargs["num_images"]
         self.zebra_daq_prep()
         self.zebra.pc.encoder.put(3)  # encoder 0=x, 1=y,2=z,3=omega
-        ttime.sleep(1.0)  # used since LSDC 1 - reason unknown
+        ttime.sleep(0.5)  # used since LSDC 1 - reason unknown
         self.zebra.pc.direction.put(0)  # direction 0 = positive
         self.zebra.pc.gate.sel.put(0)
         self.zebra.pc.pulse.sel.put(1)
         self.zebra.pc.pulse.start.put(0)
 
         PW = (exposurePeriodPerImage - 2 * detector_dead_time) * 1000
         PS = (exposurePeriodPerImage) * 1000
```

### Comparing `mxtools-1.0.2/mxtools/scans.py` & `mxtools-1.0.3/mxtools/scans.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/vector_program.py` & `mxtools-1.0.3/mxtools/vector_program.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools/zebra.py` & `mxtools-1.0.3/mxtools/zebra.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/mxtools.egg-info/PKG-INFO` & `mxtools-1.0.3/mxtools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxtools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Common code for the MX beamlines at NSLS-II (AMX, FMX).
 Home-page: https://github.com/NSLS-II-AMX/mxtools
 Author: Jun Aishima
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mxtools-1.0.2/mxtools.egg-info/SOURCES.txt` & `mxtools-1.0.3/mxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/setup.py` & `mxtools-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.2/versioneer.py` & `mxtools-1.0.3/versioneer.py`

 * *Files identical despite different names*

