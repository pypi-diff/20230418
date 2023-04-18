# Comparing `tmp/lorettOrbital-1.0.13042023.tar.gz` & `tmp/lorettOrbital-1.0.18042023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorettOrbital-1.0.13042023.tar", last modified: Thu Apr 13 02:59:43 2023, max compression
+gzip compressed data, was "lorettOrbital-1.0.18042023.tar", last modified: Tue Apr 18 11:55:42 2023, max compression
```

## Comparing `lorettOrbital-1.0.13042023.tar` & `lorettOrbital-1.0.18042023.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.432335 lorettOrbital-1.0.13042023/
--rw-rw-rw-   0        0        0     1086 2022-06-25 18:31:46.000000 lorettOrbital-1.0.13042023/LICENSE
--rw-rw-rw-   0        0        0      649 2023-04-13 02:59:43.431335 lorettOrbital-1.0.13042023/PKG-INFO
--rw-rw-rw-   0        0        0      146 2022-06-25 18:31:46.000000 lorettOrbital-1.0.13042023/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.414337 lorettOrbital-1.0.13042023/lorettOrbital/
--rw-rw-rw-   0        0        0      636 2023-04-13 02:57:40.000000 lorettOrbital-1.0.13042023/lorettOrbital/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.423336 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/
--rw-rw-rw-   0        0        0      337 2023-03-23 04:11:03.000000 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/__init__.py
--rw-rw-rw-   0        0        0      971 2022-07-16 19:16:18.000000 lorettOrbital-1.0.13042023/lorettOrbital/exceptions/exceptions.py
--rw-rw-rw-   0        0        0     8951 2022-12-02 21:46:20.000000 lorettOrbital-1.0.13042023/lorettOrbital/orbital.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.426341 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/
--rw-rw-rw-   0        0        0      595 2023-03-23 04:24:14.000000 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/__init__.py
--rw-rw-rw-   0        0        0    29209 2023-04-13 02:28:56.000000 lorettOrbital-1.0.13042023/lorettOrbital/scheduler/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.429337 lorettOrbital-1.0.13042023/lorettOrbital/tests/
--rw-rw-rw-   0        0        0      411 2023-03-23 04:30:24.000000 lorettOrbital-1.0.13042023/lorettOrbital/tests/SchedulerUnitTest.py
--rw-rw-rw-   0        0        0        0 2023-03-23 03:01:19.000000 lorettOrbital-1.0.13042023/lorettOrbital/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:59:43.420341 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/
--rw-rw-rw-   0        0        0      649 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 02:59:43.000000 lorettOrbital-1.0.13042023/lorettOrbital.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 02:59:43.433338 lorettOrbital-1.0.13042023/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-03-23 03:15:31.000000 lorettOrbital-1.0.13042023/setup.py
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.051613 lorettOrbital-1.0.18042023/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)     1086 2022-06-25 18:31:46.000000 lorettOrbital-1.0.18042023/LICENSE
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      607 2023-04-18 11:55:42.051322 lorettOrbital-1.0.18042023/PKG-INFO
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      146 2022-06-25 18:31:46.000000 lorettOrbital-1.0.18042023/README.md
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.044856 lorettOrbital-1.0.18042023/lorettOrbital/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      638 2023-04-18 11:53:01.000000 lorettOrbital-1.0.18042023/lorettOrbital/__init__.py
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.048379 lorettOrbital-1.0.18042023/lorettOrbital/exceptions/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      337 2023-03-23 04:11:03.000000 lorettOrbital-1.0.18042023/lorettOrbital/exceptions/__init__.py
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      971 2022-07-16 19:16:18.000000 lorettOrbital-1.0.18042023/lorettOrbital/exceptions/exceptions.py
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)     8951 2022-12-02 21:46:20.000000 lorettOrbital-1.0.18042023/lorettOrbital/orbital.py
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.049481 lorettOrbital-1.0.18042023/lorettOrbital/scheduler/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      653 2023-04-18 11:52:41.000000 lorettOrbital-1.0.18042023/lorettOrbital/scheduler/__init__.py
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)    29641 2023-04-18 11:52:50.000000 lorettOrbital-1.0.18042023/lorettOrbital/scheduler/scheduler.py
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.050795 lorettOrbital-1.0.18042023/lorettOrbital/tests/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      411 2023-03-23 04:30:24.000000 lorettOrbital-1.0.18042023/lorettOrbital/tests/SchedulerUnitTest.py
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-03-23 03:01:19.000000 lorettOrbital-1.0.18042023/lorettOrbital/tests/__init__.py
+drwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        0 2023-04-18 11:55:42.047469 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      607 2023-04-18 11:55:42.000000 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/PKG-INFO
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)      483 2023-04-18 11:55:42.000000 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)        1 2023-04-18 11:55:42.000000 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)       93 2023-04-18 11:55:42.000000 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/requires.txt
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)       14 2023-04-18 11:55:42.000000 lorettOrbital-1.0.18042023/lorettOrbital.egg-info/top_level.txt
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)       38 2023-04-18 11:55:42.051711 lorettOrbital-1.0.18042023/setup.cfg
+-rwxrwxrwx   0 mrfentazis  (1000) mrfentazis  (1000)     1013 2023-04-13 03:13:10.000000 lorettOrbital-1.0.18042023/setup.py
```

### Comparing `lorettOrbital-1.0.13042023/LICENSE` & `lorettOrbital-1.0.18042023/LICENSE`

 * *Files identical despite different names*

### Comparing `lorettOrbital-1.0.13042023/lorettOrbital/__init__.py` & `lorettOrbital-1.0.18042023/lorettOrbital/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,13 +10,11 @@
 # @section scheduler Notes
 # Contains several classes that provide TLE processing, calculation of flight schedules by parameters, etc.
 #
 
 from . import scheduler
 from . import exceptions
 
+__version__= scheduler.__version__
 # Global Constants
 ## Elements of the lorettOrbital
-__all__ = ["scheduler", "exceptions"]
-
-## Library version
-__version__ = "1.0.13042023"
+__all__ = ["scheduler", "exceptions", "__version__"]
```

### Comparing `lorettOrbital-1.0.13042023/lorettOrbital/exceptions/exceptions.py` & `lorettOrbital-1.0.18042023/lorettOrbital/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `lorettOrbital-1.0.13042023/lorettOrbital/orbital.py` & `lorettOrbital-1.0.18042023/lorettOrbital/orbital.py`

 * *Files identical despite different names*

### Comparing `lorettOrbital-1.0.13042023/lorettOrbital/scheduler/__init__.py` & `lorettOrbital-1.0.18042023/lorettOrbital/scheduler/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,23 @@
                         SchedulerConfig, 
                         SatPass, 
                         TrackFile, 
                         SphereAltCoordinates, 
                         SphereCoordinates, 
                         XYCoordinates, 
                         sources, 
-                        satLists )
+                        satLists,
+                        __version__ )
 
 ## Elements of the scheduler module
 __all__ = [
     "Scheduler",
     "sources",
     "satLists",
     "SchedulerConfig",
     "SatPass",
     "TrackFile",
     "SphereCoordinates",
     "SphereAltCoordinates",
-    "XYCoordinates"
+    "XYCoordinates",
+    "__version__"
 ]
```

### Comparing `lorettOrbital-1.0.13042023/lorettOrbital/scheduler/scheduler.py` & `lorettOrbital-1.0.18042023/lorettOrbital/scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,21 @@
 from lorettOrbital.exceptions import *
 
 from requests import get, exceptions
 from typing import List, Tuple, Any, Callable
 
 from dataclasses import dataclass, field
 
+
+
+
+## Library version
+__version__ = "1.0.18042023"
+
+
 # Global Constants
 ## Station types list; rotator - classic azimuth and elevation systems; legacy - minutes:seconds special type for V. Rosental lorett systems.
 stationTypes = [
                 "rotator",
                 "legacy" # for Rosental systems
                 ]
 
@@ -455,14 +462,22 @@
                     file.write( now.strftime("# %Y%m%d %H%M%S\n"))
                     file.write(content)
 
                 if self.logger != None:
                     self.logger.info("TLE updated")
 
                 return True
+            
+            else:
+                diff = set(self.satList) - set(newSats)
+                if self.logger != None:
+                    self.logger.error(f"Sattelites not found in tle: {', '.join(diff)}")
+                    self.logger.warning(f"Ignore {', '.join(diff)}")
+                    self.satList = list(set(self.satList) - diff)
+                return True
 
             if content == "" and self.logger != None:
                 self.logger.warning("Failed update TLE")
 
             ## the update failed, but the old file has all the satellites
             if content == "" and all(i in oldSats for i in self.config.satList) and self.logger != None:
                 self.logger.warning(f"Use old TLE {dateTLE}")
```

### Comparing `lorettOrbital-1.0.13042023/setup.py` & `lorettOrbital-1.0.18042023/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from lorettOrbital import __version__
 
 
 with open("requirements.txt", 'r') as file:
-      requirements =  file.readlines()
+      requirements = file.readlines()
  
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setup(name='lorettOrbital',
       version=__version__,
       url='https://gitlab.com/lpmrfentazis/lorettorbital',
@@ -21,8 +21,12 @@
       test_suite="tests",
       classifiers=[
 		"Programming Language :: Python :: 3.9",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
       python_requires='>=3.9'
-      )
+      )
+
+# python setup.py sdist bdist_wheel --universal
+# python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+# python -m twine upload dist/*
```

