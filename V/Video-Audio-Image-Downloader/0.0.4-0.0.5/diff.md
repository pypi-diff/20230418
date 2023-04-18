# Comparing `tmp/Video_Audio_Image_Downloader-0.0.4.tar.gz` & `tmp/Video_Audio_Image_Downloader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Video_Audio_Image_Downloader-0.0.4.tar", last modified: Tue Apr 18 11:09:19 2023, max compression
+gzip compressed data, was "Video_Audio_Image_Downloader-0.0.5.tar", last modified: Tue Apr 18 11:12:19 2023, max compression
```

## Comparing `Video_Audio_Image_Downloader-0.0.4.tar` & `Video_Audio_Image_Downloader-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      326 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/PKG-INFO
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      326 2023-04-18 11:09:19.000000 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      403 2023-04-18 11:09:19.000000 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-18 11:09:19.000000 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-18 11:09:19.000000 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-18 11:09:19.000000 Video_Audio_Image_Downloader-0.0.4/Video_Audio_Image_Downloader.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      624 2023-04-18 11:08:57.000000 Video_Audio_Image_Downloader-0.0.4/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 10:56:32.000000 Video_Audio_Image_Downloader-0.0.4/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:09:19.474995 Video_Audio_Image_Downloader-0.0.4/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.4/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1901 2023-04-17 14:20:59.000000 Video_Audio_Image_Downloader-0.0.4/source/lib/Command_function.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.4/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2742 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.4/source/lib/help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4424 2023-04-18 11:03:45.000000 Video_Audio_Image_Downloader-0.0.4/source/source.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      362 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/PKG-INFO
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      362 2023-04-18 11:12:19.000000 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      403 2023-04-18 11:12:19.000000 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-18 11:12:19.000000 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-18 11:12:19.000000 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-18 11:12:19.000000 Video_Audio_Image_Downloader-0.0.5/Video_Audio_Image_Downloader.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      660 2023-04-18 11:12:13.000000 Video_Audio_Image_Downloader-0.0.5/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 10:56:32.000000 Video_Audio_Image_Downloader-0.0.5/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 11:12:19.475155 Video_Audio_Image_Downloader-0.0.5/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.5/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1901 2023-04-17 14:20:59.000000 Video_Audio_Image_Downloader-0.0.5/source/lib/Command_function.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.5/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2742 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.5/source/lib/help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4424 2023-04-18 11:03:45.000000 Video_Audio_Image_Downloader-0.0.5/source/source.py
```

### Comparing `Video_Audio_Image_Downloader-0.0.4/setup.py` & `Video_Audio_Image_Downloader-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 # requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 
 
 
 setup(
     name='Video_Audio_Image_Downloader',
-    version='0.0.4',
+    version='0.0.5',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
-    description='In this tool is used to Download the Youtube Video,Audio and Images',
+    description="In this tool is used to Download the Youtube Video,Audio and Any type of Google and other site's Images",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1',
     # install_requires=requirements,
     entry_points={
         'console_scripts': [
             'Downloader=source.source:main',
         ],
```

### Comparing `Video_Audio_Image_Downloader-0.0.4/source/lib/Argument.py` & `Video_Audio_Image_Downloader-0.0.5/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.0.4/source/lib/Command_function.py` & `Video_Audio_Image_Downloader-0.0.5/source/lib/Command_function.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.0.4/source/lib/help.py` & `Video_Audio_Image_Downloader-0.0.5/source/lib/help.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.0.4/source/source.py` & `Video_Audio_Image_Downloader-0.0.5/source/source.py`

 * *Files identical despite different names*

