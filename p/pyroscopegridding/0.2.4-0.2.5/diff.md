# Comparing `tmp/pyroscopegridding-0.2.4.tar.gz` & `tmp/pyroscopegridding-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.2.4.tar", last modified: Tue Apr 18 15:59:02 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.2.5.tar", last modified: Tue Apr 18 16:01:42 2023, max compression
```

## Comparing `pyroscopegridding-0.2.4.tar` & `pyroscopegridding-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 15:59:02.051661 pyroscopegridding-0.2.4/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-18 15:59:02.045664 pyroscopegridding-0.2.4/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.4/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 15:59:01.751004 pyroscopegridding-0.2.4/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.4/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.4/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.4/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.4/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.4/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29557 2023-04-18 15:58:17.000000 pyroscopegridding-0.2.4/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.4/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.4/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.4/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.4/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 15:59:01.998004 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-18 15:59:00.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-18 15:59:01.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-18 15:59:00.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-18 15:59:00.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-04-18 15:59:00.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-18 15:59:00.000000 pyroscopegridding-0.2.4/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-18 15:59:02.055660 pyroscopegridding-0.2.4/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1799 2023-04-18 15:58:51.000000 pyroscopegridding-0.2.4/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 16:01:42.472852 pyroscopegridding-0.2.5/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-18 16:01:42.467853 pyroscopegridding-0.2.5/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.5/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 16:01:42.216793 pyroscopegridding-0.2.5/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.5/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.5/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.5/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.5/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.5/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29558 2023-04-18 16:01:21.000000 pyroscopegridding-0.2.5/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.5/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.5/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.5/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.5/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-18 16:01:42.438014 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-18 16:01:41.000000 pyroscopegridding-0.2.5/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-18 16:01:42.473851 pyroscopegridding-0.2.5/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1799 2023-04-18 16:01:28.000000 pyroscopegridding-0.2.5/setup.py
```

### Comparing `pyroscopegridding-0.2.4/PKG-INFO` & `pyroscopegridding-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.4/README.md` & `pyroscopegridding-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.5/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.5/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.5/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.5/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.5/pyroscopegridding/gtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
         netCDF_yaml_config(str(args.filename))
     elif args.configtime:
         # yaml config 
         # python gtools.py -cfg -fn "C:\Users\swzhao\Desktop\repos\gridtools\config.yml"
         # "C:\Users\bobgr\Desktop\Spring 2022 NASA\Gridtools Package (Code, README, inputs, outputs, examples, verification)\gridtools\config.yml"
         # "C:/Users/bobgr/Desktop/Spring 2022 NASA/Gridtools Package (Code, README, inputs, outputs, examples, verification)/gridtools/config.yml"
         netCDF_yaml_config_time(str(args.filename), str(args.time_start), str(args.time_end))
-    elif args.configtime:
+    elif args.configarray:
         # yaml config 
         # python gtools.py -cfg -fn "C:\Users\swzhao\Desktop\repos\gridtools\config.yml"
         # "C:\Users\bobgr\Desktop\Spring 2022 NASA\Gridtools Package (Code, README, inputs, outputs, examples, verification)\gridtools\config.yml"
         # "C:/Users/bobgr/Desktop/Spring 2022 NASA/Gridtools Package (Code, README, inputs, outputs, examples, verification)/gridtools/config.yml"
         netCDF_yaml_config_array(str(args.filename))
     else:
         print("No command given")
```

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.5/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.5/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.5/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.5/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.2.5/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.4
+Version: 0.2.5
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.4/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.5/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.4/setup.py` & `pyroscopegridding-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.2.4',      # Initial version
+    version = '0.2.5',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

