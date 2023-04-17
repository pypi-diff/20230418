# Comparing `tmp/oursin-0.4.4.tar.gz` & `tmp/oursin-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oursin-0.4.4.tar", last modified: Fri Feb 10 00:51:40 2023, max compression
+gzip compressed data, was "oursin-0.4.5.tar", last modified: Mon Apr 17 21:55:32 2023, max compression
```

## Comparing `oursin-0.4.4.tar` & `oursin-0.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 00:51:40.867291 oursin-0.4.4/
--rw-rw-rw-   0        0        0    35823 2022-02-16 22:45:28.000000 oursin-0.4.4/LICENSE
--rw-rw-rw-   0        0        0    41996 2023-02-10 00:51:40.868026 oursin-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-02-09 17:59:33.000000 oursin-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 00:51:40.859287 oursin-0.4.4/oursin/
--rw-rw-rw-   0        0        0      545 2023-02-09 22:17:25.000000 oursin-0.4.4/oursin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 00:51:40.864291 oursin-0.4.4/oursin/atlas/
--rw-rw-rw-   0        0        0       17 2023-02-09 22:17:19.000000 oursin-0.4.4/oursin/atlas/__init__.py
--rw-rw-rw-   0        0        0     3786 2023-02-10 00:00:27.000000 oursin-0.4.4/oursin/atlas/ccf.py
--rw-rw-rw-   0        0        0     2404 2023-02-09 18:59:00.000000 oursin-0.4.4/oursin/camera.py
--rw-rw-rw-   0        0        0     1014 2023-02-09 18:48:43.000000 oursin-0.4.4/oursin/client.py
-drwxrwxrwx   0        0        0        0 2023-02-10 00:51:40.866292 oursin-0.4.4/oursin/colors/
--rw-rw-rw-   0        0        0       46 2023-02-09 18:47:02.000000 oursin-0.4.4/oursin/colors/__init__.py
--rw-rw-rw-   0        0        0     4531 2023-02-09 18:15:54.000000 oursin-0.4.4/oursin/colors/colors.py
--rw-rw-rw-   0        0        0    36410 2023-02-09 18:49:06.000000 oursin-0.4.4/oursin/colors/xkcd_rgb.py
--rw-rw-rw-   0        0        0     1214 2023-02-09 21:10:06.000000 oursin-0.4.4/oursin/lines.py
--rw-rw-rw-   0        0        0     2487 2023-02-09 21:10:52.000000 oursin-0.4.4/oursin/neurons.py
--rw-rw-rw-   0        0        0     1565 2023-02-09 21:11:19.000000 oursin-0.4.4/oursin/primitives.py
--rw-rw-rw-   0        0        0     2438 2023-02-09 21:11:45.000000 oursin-0.4.4/oursin/probes.py
--rw-rw-rw-   0        0        0     1514 2023-02-10 00:51:09.000000 oursin-0.4.4/oursin/renderer.py
--rw-rw-rw-   0        0        0     1927 2023-02-09 21:12:16.000000 oursin-0.4.4/oursin/text.py
--rw-rw-rw-   0        0        0     3524 2023-02-09 21:13:22.000000 oursin-0.4.4/oursin/volumes.py
-drwxrwxrwx   0        0        0        0 2023-02-10 00:51:40.862291 oursin-0.4.4/oursin.egg-info/
--rw-rw-rw-   0        0        0    41996 2023-02-10 00:51:40.000000 oursin-0.4.4/oursin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-02-10 00:51:40.000000 oursin-0.4.4/oursin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 00:51:40.000000 oursin-0.4.4/oursin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-02-10 00:51:40.000000 oursin-0.4.4/oursin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-10 00:51:40.000000 oursin-0.4.4/oursin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      750 2022-12-13 18:12:19.000000 oursin-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-10 00:51:40.868026 oursin-0.4.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.650126 oursin-0.4.5/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 19:55:46.000000 oursin-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0    42009 2023-04-17 21:55:32.650126 oursin-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-02-15 20:37:09.000000 oursin-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.547171 oursin-0.4.5/oursin/
+-rw-rw-rw-   0        0        0      545 2023-02-15 20:37:09.000000 oursin-0.4.5/oursin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.640119 oursin-0.4.5/oursin/atlas/
+-rw-rw-rw-   0        0        0       17 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/atlas/__init__.py
+-rw-rw-rw-   0        0        0     3786 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/atlas/ccf.py
+-rw-rw-rw-   0        0        0     3589 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/camera.py
+-rw-rw-rw-   0        0        0     1244 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.648132 oursin-0.4.5/oursin/colors/
+-rw-rw-rw-   0        0        0       46 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/__init__.py
+-rw-rw-rw-   0        0        0     4531 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/colors.py
+-rw-rw-rw-   0        0        0    36410 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/colors/xkcd_rgb.py
+-rw-rw-rw-   0        0        0     1214 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/lines.py
+-rw-rw-rw-   0        0        0     2487 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/neurons.py
+-rw-rw-rw-   0        0        0     1904 2023-04-17 21:53:19.000000 oursin-0.4.5/oursin/primitives.py
+-rw-rw-rw-   0        0        0     2438 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/probes.py
+-rw-rw-rw-   0        0        0     1514 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/renderer.py
+-rw-rw-rw-   0        0        0     1927 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/text.py
+-rw-rw-rw-   0        0        0     3524 2023-02-15 20:37:10.000000 oursin-0.4.5/oursin/volumes.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:55:32.622105 oursin-0.4.5/oursin.egg-info/
+-rw-rw-rw-   0        0        0    42009 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 21:55:32.000000 oursin-0.4.5/oursin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      772 2023-04-17 21:53:19.000000 oursin-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:55:32.658106 oursin-0.4.5/setup.cfg
```

### Comparing `oursin-0.4.4/LICENSE` & `oursin-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/PKG-INFO` & `oursin-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oursin
-Version: 0.4.4
-Summary: Urchin - Universal Renderer for Neuroscience Python API
+Version: 0.4.5
+Summary: Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API
 Author-email: Daniel Birman <danbirman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html
-Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/UnityNeuroscience/issues
+Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/Urchin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oursin-0.4.4/oursin/__init__.py` & `oursin-0.4.5/oursin/__init__.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/atlas/ccf.py` & `oursin-0.4.5/oursin/atlas/ccf.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/client.py` & `oursin-0.4.5/oursin/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Client for communicating with the echo server"""
 import socketio
 import os
 
+from . import camera
+
 class bcolors:
     WARNING = '\033[93m'
     FAIL = '\033[91m'
 
 sio = socketio.Client()
 @sio.event
 def connect():
@@ -28,14 +30,21 @@
 	if log_messages:
 		print('(Renderer) ' + bcolors.WARNING + data)
 
 @sio.on('log-error')
 def message(data):
 	print('(Renderer) ' + bcolors.FAIL + data)
 
+@sio.on('ReceiveCameraImgMeta')
+def receive_camera_img_meta(data):
+	camera.receive_camera_img_meta(data)
+	
+@sio.on('ReceiveCameraImg')
+def receive_camera_img(data):
+  camera.receive_camera_img(data)
 def connected():
 	return sio.connected
 
 def close():
 	"""Disconnect from the echo server
 	"""
 	sio.disconnect()
```

### Comparing `oursin-0.4.4/oursin/colors/colors.py` & `oursin-0.4.5/oursin/colors/colors.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/colors/xkcd_rgb.py` & `oursin-0.4.5/oursin/colors/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/lines.py` & `oursin-0.4.5/oursin/lines.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/neurons.py` & `oursin-0.4.5/oursin/neurons.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/primitives.py` & `oursin-0.4.5/oursin/primitives.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,8 +68,23 @@
       dictionary of IDs and new hex color of mesh
       
 	Examples
 	--------
 	>>> urn.set_color({'cube1': '#FFFFFF'})
 	
   """
-  client.sio.emit('SetColor', mesh_color)
+  client.sio.emit('SetColor', mesh_color)
+
+def set_material(mesh_material):
+  """Set the material of mesh renderer
+
+  Parameters
+  ----------
+  mesh_material : dict {string : string}
+      dictionary of object IDs and name of new material
+      
+	Examples
+	--------
+	>>> urn.set_material({'cube1': 'unlit'})
+	
+  """
+  client.sio.emit('SetMaterial', mesh_material)
```

### Comparing `oursin-0.4.4/oursin/probes.py` & `oursin-0.4.5/oursin/probes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/renderer.py` & `oursin-0.4.5/oursin/renderer.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/text.py` & `oursin-0.4.5/oursin/text.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin/volumes.py` & `oursin-0.4.5/oursin/volumes.py`

 * *Files identical despite different names*

### Comparing `oursin-0.4.4/oursin.egg-info/PKG-INFO` & `oursin-0.4.5/oursin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oursin
-Version: 0.4.4
-Summary: Urchin - Universal Renderer for Neuroscience Python API
+Version: 0.4.5
+Summary: Urchin - Universal Renderer Creating Helpful Images for Neuroscience Python API
 Author-email: Daniel Birman <danbirman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://virtualbrainlab.org/03_unity_neuro/01_urn_intro.html
-Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/UnityNeuroscience/issues
+Project-URL: Bug Tracker, https://github.com/VirtualBrainLab/Urchin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

