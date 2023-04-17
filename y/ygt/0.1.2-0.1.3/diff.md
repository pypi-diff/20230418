# Comparing `tmp/ygt-0.1.2.tar.gz` & `tmp/ygt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygt-0.1.2.tar", last modified: Fri Apr  7 02:55:55 2023, max compression
+gzip compressed data, was "ygt-0.1.3.tar", last modified: Mon Apr 17 22:47:49 2023, max compression
```

## Comparing `ygt-0.1.2.tar` & `ygt-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-07 02:55:55.307119 ygt-0.1.2/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.2/LICENSE
--rw-r--r--   0 peterbaker   (504) staff       (20)      153 2023-04-06 23:40:23.000000 ygt-0.1.2/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     1849 2023-04-07 02:55:55.306961 ygt-0.1.2/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1453 2023-04-07 02:54:42.000000 ygt-0.1.2/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      738 2023-04-07 02:01:19.000000 ygt-0.1.2/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-07 02:55:55.307163 ygt-0.1.2/setup.cfg
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.2/setup.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-07 02:55:55.292940 ygt-0.1.2/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-07 02:55:55.299855 ygt-0.1.2/src/ygt/
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/__main__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1687 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/autohint.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3524 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/cvGuesser.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     3352 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/fontViewDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    11193 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/freetypeFont.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-07 02:55:55.306736 ygt-0.1.2/src/ygt/icons/
--rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/align.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/anchor.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/black_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/cursor-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/cursor-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.2/src/ygt/icons/cv.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.2/src/ygt/icons/cv_guess.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/gray_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/hand-icon-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/hand-icon-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.2/src/ygt/icons/horizontal-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.2/src/ygt/icons/horizontal-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/interpolate.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/make_set.png
--rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.2/src/ygt/icons/program.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/shift.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.2/src/ygt/icons/vertical-off.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.2/src/ygt/icons/vertical-on.png
--rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.2/src/ygt/icons/white_distance.png
--rw-r--r--   0 peterbaker   (504) staff       (20)     5582 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/macfuncDialog.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    53539 2023-04-06 20:42:38.000000 ygt-0.1.2/src/ygt/makeCVDialog.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)    64822 2023-04-06 14:55:02.000000 ygt-0.1.2/src/ygt/window.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     1938 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/ygError.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   106912 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/ygHintEditor.py
--rw-rw-r--   0 peterbaker   (504) staff       (20)   135219 2023-04-06 20:37:58.000000 ygt-0.1.2/src/ygt/ygModel.py
--rwxrwxrwx   0 peterbaker   (504) staff       (20)     8474 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/ygPreferences.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    19542 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/ygPreview.py
--rw-r--r--   0 peterbaker   (504) staff       (20)     9630 2023-04-06 15:04:52.000000 ygt-0.1.2/src/ygt/ygSchema.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    12216 2023-04-06 20:53:14.000000 ygt-0.1.2/src/ygt/ygYAMLEditor.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-07 02:55:55.300741 ygt-0.1.2/src/ygt.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     1849 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1160 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      129 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-07 02:55:55.000000 ygt-0.1.2/src/ygt.egg-info/top_level.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.2/src/ygt.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.022160 ygt-0.1.3/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11358 2022-11-11 22:39:04.000000 ygt-0.1.3/LICENSE
+-rw-r--r--   0 peterbaker   (504) staff       (20)      181 2023-04-16 16:44:10.000000 ygt-0.1.3/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2417 2023-04-17 22:47:49.022026 ygt-0.1.3/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2021 2023-04-17 21:42:41.000000 ygt-0.1.3/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      786 2023-04-17 21:31:23.000000 ygt-0.1.3/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-04-17 22:47:49.022198 ygt-0.1.3/setup.cfg
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2022-11-11 22:39:05.000000 ygt-0.1.3/setup.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.006921 ygt-0.1.3/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.013398 ygt-0.1.3/src/ygt/
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       64 2023-04-06 15:04:52.000000 ygt-0.1.3/src/ygt/__main__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1673 2023-04-12 11:23:21.000000 ygt-0.1.3/src/ygt/autohint_trash.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3729 2023-04-14 00:53:44.000000 ygt-0.1.3/src/ygt/cvGuesser.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4771 2023-04-17 11:45:55.000000 ygt-0.1.3/src/ygt/fontViewDialog.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.014352 ygt-0.1.3/src/ygt/fonts/
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   119788 2012-09-20 04:00:00.000000 ygt-0.1.3/src/ygt/fonts/SourceCodePro-Regular.ttf
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12008 2023-04-17 10:52:42.000000 ygt-0.1.3/src/ygt/freetypeFont.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.021816 ygt-0.1.3/src/ygt/icons/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    26646 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/align.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24080 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/anchor.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15786 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/black_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6769 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/cursor-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6681 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/cursor-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10657 2022-12-01 22:00:45.000000 ygt-0.1.3/src/ygt/icons/cv.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     9754 2022-12-18 19:55:30.000000 ygt-0.1.3/src/ygt/icons/cv_guess.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15405 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/gray_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6447 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/hand-icon-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6330 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/hand-icon-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7662 2023-01-23 03:27:58.000000 ygt-0.1.3/src/ygt/icons/horizontal-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7714 2023-01-23 03:31:16.000000 ygt-0.1.3/src/ygt/icons/horizontal-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    16295 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/interpolate.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22063 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/make_set.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)   536171 2022-11-12 02:29:09.000000 ygt-0.1.3/src/ygt/icons/program.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    28381 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/shift.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    24089 2023-04-12 17:06:29.000000 ygt-0.1.3/src/ygt/icons/stem_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     7025 2023-01-23 03:32:57.000000 ygt-0.1.3/src/ygt/icons/vertical-off.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6856 2023-01-23 03:32:24.000000 ygt-0.1.3/src/ygt/icons/vertical-on.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15484 2022-11-11 22:39:05.000000 ygt-0.1.3/src/ygt/icons/white_distance.png
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6060 2023-04-14 21:42:13.000000 ygt-0.1.3/src/ygt/macfuncDialog.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    55765 2023-04-11 17:09:51.000000 ygt-0.1.3/src/ygt/makeCVDialog.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)    64711 2023-04-17 10:32:58.000000 ygt-0.1.3/src/ygt/window.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2052 2023-04-13 13:41:11.000000 ygt-0.1.3/src/ygt/ygError.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   112941 2023-04-16 17:05:35.000000 ygt-0.1.3/src/ygt/ygHintEditor.py
+-rw-rw-r--   0 peterbaker   (504) staff       (20)   136647 2023-04-15 23:29:54.000000 ygt-0.1.3/src/ygt/ygModel.py
+-rwxrwxrwx   0 peterbaker   (504) staff       (20)     8929 2023-04-13 14:28:02.000000 ygt-0.1.3/src/ygt/ygPreferences.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22475 2023-04-17 16:29:50.000000 ygt-0.1.3/src/ygt/ygPreview.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10000 2023-04-13 02:48:06.000000 ygt-0.1.3/src/ygt/ygSchema.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4847 2023-04-15 15:27:33.000000 ygt-0.1.3/src/ygt/ygStems.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13056 2023-04-17 10:22:52.000000 ygt-0.1.3/src/ygt/ygYAMLEditor.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-04-17 22:47:49.014247 ygt-0.1.3/src/ygt.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2417 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1257 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       40 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      159 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        4 2023-04-17 22:47:49.000000 ygt-0.1.3/src/ygt.egg-info/top_level.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-30 03:58:20.000000 ygt-0.1.3/src/ygt.py
```

### Comparing `ygt-0.1.2/LICENSE` & `ygt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/PKG-INFO` & `ygt-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ygt
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
-- it emphasizes modern requirements for TrueType hinting while backgrounding the obsolete;
+- it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
 - it will read either a TrueType font or a UFO;
 - it can save hints in an easily understood and edited YAML file,
 - which can be compiled to a hinted font either from inside the program or from the command line,
 - or it can save compiled hints to a UFO (from which fontmake can produce a hinted font)
 
 Ygt is in an alpha state, with features yet to be added (especially auto-hinting). But it is already a workable program, which the developer has used to hint thousands of glyphs in several large fonts.
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
+
+## Changes
+
+Version 0.1.23 (2023-4-17) changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
+```
+s/blackspace/blackdist/g
+s/whitesapce/whitedist/g
+s/grayspace/graydist/g
+```
+Among other changes intended to improve stability, this version consolidates various font-level edits in a “Font Info” dialog, summoned with Ctrl-I or Cmd-I, and honors “dark themes” on various platforms.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ygt-0.1.2/pyproject.toml` & `ygt-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ygt"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "A graphical hint editor for TrueType fonts"
 readme = "README.md"
 requires-python = ">=3.10.4"
 classifiers = [
@@ -16,17 +16,19 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "PyQt6 >= 6.4.0",
     "fonttools >= 4.38.0",
     "freetype-py >= 2.3.0",
+    "defcon >= 0.10.1",
     "xgridfit >= 3.2.16",
     "setuptools >= 65.3.0",
     "PyYAML >= 6.0",
     "schema >= 0.7.5",
     "fs >= 2.4.15",
+    "ufo2ft >= 2.28.0",
     "numpy",
 ]
 
 [project.scripts]
     ygt = "ygt.window:main"
```

### Comparing `ygt-0.1.2/src/ygt/autohint.py` & `ygt-0.1.3/src/ygt/autohint_trash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import copy
-
-
 class keyPoint:
     def __init__(self, pt, desc):
         self.point = pt
         self.label = desc
 
 
 class autohinter:
```

### Comparing `ygt-0.1.2/src/ygt/cvGuesser.py` & `ygt-0.1.3/src/ygt/cvGuesser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-from fontTools.varLib import instancer
+from typing import Optional
+from fontTools.varLib import instancer  # type: ignore
+from fontTools.ttLib.ttFont import TTFont # type: ignore
 
 
 class instanceChecker:
     """This class will build an instance for a variable font and check
     the y positions of points from which the cvt table was made. If
     the y positions are different, the y position of the point is
     recorded and reported.
     """
 
-    def __init__(self, ft_font, cvt, masters):
+    def __init__(self, ft_font, cvt, masters) -> None:
         self.ft_font = ft_font
         self.cvt = cvt
         self.masters = masters
         self.axes = self.masters.yg_font.axes
-        self.current_instance = None
+        self.current_instance: Optional[TTFont] = None
 
-    def refresh(self):
+    def refresh(self) -> None:
         self.delete_all_vars()
         d = self.get_all_variant_cvs()
         self.add_variants_to_cvt(d)
 
-    def delete_all_vars(self):
+    def delete_all_vars(self) -> None:
         k = self.cvt.keys()
         for kk in k:
             cv = self.cvt.get_cv(kk)
             try:
                 # if there's no "origin" in the cv, we can't replace the vars.
                 if "origin" in cv:
                     del cv["var"]
             except Exception:
                 pass
 
-    def make_instance(self, vals):
+    def make_instance(self, vals: dict) -> None:
         self.current_instance = instancer.instantiateVariableFont(self.ft_font, vals)
 
-    def get_all_variant_cvs(self):
+    def get_all_variant_cvs(self) -> dict:
         # We end up with a dict:
         # {master_id: {cv_name: val, ...}, ...}
         result = {}
         k = self.masters.keys()
         for kk in k:
             c = self.get_cvs_for_master(kk)
             if len(c) > 0:
                 result[kk] = c
         return result
 
-    def add_variants_to_cvt(self, d):
+    def add_variants_to_cvt(self, d: dict) -> None:
         # d is a dict in the format produced by get_all_variant_cvs.
         ck = self.cvt.keys()
         dk = d.keys()
         for ckk in ck:  # iterate through CVs.
             for dkk in dk:  # iterate through masters
                 if ckk in d[dkk]:  # if the master has an entry for the current CV,
                     cv = self.cvt.get_cv(ckk)  # create a "var" entry in the CV.
                     if not "var" in cv:
                         cv["var"] = {}
                     cv["var"][dkk] = d[dkk][ckk]
 
-    def get_cvs_for_master(self, master_id):
+    def get_cvs_for_master(self, master_id: str) -> dict:
         # Get the glyph name and point index (or indices) from the
         # "origin" field. Get the list of y values (function below) and
         # use those to figure out the value of the cv for this glyph.
         # Compare the new position with that of the default cv.
         # If different, store. If the same, discard.
         result = {}
         coords = self.masters.get_master_coords(master_id)
@@ -81,15 +83,15 @@
                     ptnum = cv["origin"]["ptnum"]
                     yl = self.y_list(glyph_name)
                     y_diff = abs(yl[ptnum[0]] - yl[ptnum[1]])
                     if cv["val"] != y_diff:
                         result[kk] = y_diff
         return result
 
-    def y_list(self, glyph_name):
+    def y_list(self, glyph_name: str) -> list:
         gl = self.current_instance["glyf"][glyph_name].getCoordinates(
             self.ft_font["glyf"][glyph_name]
         )
         y_points = []
         for p in gl[0]:
             y_points.append(p[1])
         return y_points
```

### Comparing `ygt-0.1.2/src/ygt/freetypeFont.py` & `ygt-0.1.3/src/ygt/freetypeFont.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import freetype as ft
+from typing import Optional
+import freetype as ft # type: ignore
 import numpy
 import copy
 from tempfile import SpooledTemporaryFile
 from PyQt6.QtGui import QColor, QPen
 from PyQt6.QtCore import QRect
 
 
@@ -42,16 +43,21 @@
       ftf = freetypeFont("Elstob-Regular.ttf")
       # The GID of the desired character
       ftf.set_char(60)
       ftf.draw_char(painter)
     """
 
     def __init__(
-        self, font, size=30, render_mode=RENDER_LCD_1, hinting_on=True, instance=None
-    ):
+        self,
+        font: SpooledTemporaryFile | str,
+        size: int = 30,
+        render_mode: int = RENDER_LCD_1,
+        hinting_on: bool = True,
+        instance: str = None
+    ) -> None:
         self.valid = True
         try:
             if type(font) is SpooledTemporaryFile:
                 font.seek(0)
                 self.face = ft.Face(font)
                 font.close()
             else:
@@ -61,33 +67,37 @@
             return
         self.char_size = size * 64
         self.size = 30
         self.ascender = 0
         self.descender = 0
         self.face_height = 0
         self.advance = 0
-        self.glyph_slot = None
+        self.glyph_slot: Optional[ft.GlyphSlot] = None
         self.glyph_index = 0
         self.bitmap_top = 0
         self.bitmap_left = 0
         self.top_offset = 0
         self.instance = instance
         self.hinting_on = hinting_on
         self.bw_colors = self.mk_bw_color_list()
+        self.bw_colors_dark = self.mk_bw_color_list(dark = True)
         self.draw_char = self._draw_char_lcd
         self.set_render_mode(render_mode)
         self.face.set_char_size(self.char_size)
         self._get_font_metrics()
         self.last_glyph_index = None
-        self.rect_list = []
+        self.rect_list: list = []
 
-    def mk_bw_color_list(self):
+    def mk_bw_color_list(self, dark: bool = False) -> list:
         l = [0] * 256
         for count, c in enumerate(l):
-            l[count] = QColor(0, 0, 0, count)
+            if dark:
+                l[count] = QColor(255, 255, 255, count)
+            else:
+                l[count] = QColor(0, 0, 0, count)
         return l
 
     def reset_rect_list(self):
         self.rect_list = []
 
     def set_params(
         self, glyph=None, render_mode=None, hinting_on=None, size=None, instance=None
@@ -173,15 +183,15 @@
         for i in range(rows):
             data.extend(self.glyph_slot.bitmap.buffer[i * pitch : i * pitch + width])
         if render_mode == RENDER_GRAYSCALE:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, width)
         else:
             return numpy.array(data, dtype=numpy.ubyte).reshape(rows, int(width / 3), 3)
 
-    def _draw_char_lcd(self, painter, x, y, spacing_mark=False):
+    def _draw_char_lcd(self, painter, x, y, spacing_mark = False, dark_theme = False):
         """Draws a bitmap with subpixel rendering (suitable for an lcd screen)
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
@@ -196,24 +206,31 @@
         is_mark = spacing_mark and gdata["advance"] == 0
         if is_mark:
             starting_xpos = xpos = x
             xpos += 2
             gdata["advance"] = self.advance = round(gdata["width"] / 3) + 4
         else:
             starting_xpos = xpos = x + gdata["bitmap_left"]
-        qp = QPen(QColor("black"))
+        if dark_theme:
+            qp = QPen(QColor("white"))
+            white_color = QColor("black")
+        else:
+            qp = QPen(QColor("black"))
+            white_color = QColor("white")
         qp.setWidth(1)
-        white_color = QColor("white")
         for row in Z:
             xpos = starting_xpos
             for col in row:
                 rgb = []
                 for elem in col:
                     rgb.append(elem)
-                qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
+                if dark_theme:
+                    qc = QColor(rgb[0], rgb[1], rgb[2])
+                else:
+                    qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
                 if qc != white_color:
                     qp.setColor(qc)
                     painter.setPen(qp)
                     painter.drawPoint(xpos, ypos)
                 xpos += 1
             ypos += 1
         ending_xpos = starting_xpos + round(gdata["advance"])
@@ -230,15 +247,15 @@
                 glyph_index=self.glyph_index,
                 size=self.size,
                 gname=self.index_to_name(self.glyph_index),
             )
         )
         return gdata["advance"]
 
-    def _draw_char_grayscale(self, painter, x, y, spacing_mark=False):
+    def _draw_char_grayscale(self, painter, x, y, spacing_mark=False, dark_theme = False):
         """Draws a bitmap with grayscale rendering
 
         Params:
 
         painter (QPainter): a Qt tool to draw with
 
         x (int): The left origin of the glyph
@@ -258,15 +275,18 @@
         else:
             starting_xpos = xpos = x + gdata["bitmap_left"]
         qp = QPen(QColor("black"))
         qp.setWidth(1)
         for row in Z:
             xpos = starting_xpos
             for col in row:
-                qp.setColor(self.bw_colors[col])
+                if dark_theme:
+                    qp.setColor(self.bw_colors_dark[col])
+                else:
+                    qp.setColor(self.bw_colors[col])
                 painter.setPen(qp)
                 painter.drawPoint(xpos, ypos)
                 xpos += 1
             ypos += 1
         ending_xpos = starting_xpos + round(gdata["advance"])
         ending_ypos = starting_ypos + gdata["rows"]
         if abs(ending_ypos - starting_ypos) <= 5:
@@ -315,28 +335,28 @@
                 i = self.char_to_index(ss)
                 if i != None:
                     indices.append(i)
             except Exception:
                 pass
         return indices
 
-    def draw_string(self, painter, s, x, y, x_limit=200, y_increment=67):
+    def draw_string(self, painter, s, x, y, x_limit = 200, y_increment = 67, dark_theme = False):
         self.last_glyph_index = None
         self.reset_rect_list()
         indices = self.string_to_indices(s)
         xpos = x
         ypos = y
         for i in indices:
             self.set_char(i)
             if self.last_glyph_index != None:
                 k = self.face.get_kerning(
                     self.last_glyph_index, i, ft.FT_KERNING_DEFAULT
                 )
                 xpos += k.x
-            xpos += self.draw_char(painter, xpos, ypos)
+            xpos += self.draw_char(painter, xpos, ypos, dark_theme = dark_theme)
             if xpos >= x_limit:
                 xpos = x
                 ypos += y_increment
                 self.last_glyph_index = None
             if ypos > y + y_increment:
                 break
             self.last_glyph_index = i
```

### Comparing `ygt-0.1.2/src/ygt/icons/align.png` & `ygt-0.1.3/src/ygt/icons/align.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/anchor.png` & `ygt-0.1.3/src/ygt/icons/anchor.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/black_distance.png` & `ygt-0.1.3/src/ygt/icons/black_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/cursor-icon-off.png` & `ygt-0.1.3/src/ygt/icons/cursor-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/cursor-icon-on.png` & `ygt-0.1.3/src/ygt/icons/cursor-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/cv.png` & `ygt-0.1.3/src/ygt/icons/cv.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/cv_guess.png` & `ygt-0.1.3/src/ygt/icons/cv_guess.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/gray_distance.png` & `ygt-0.1.3/src/ygt/icons/gray_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/hand-icon-off.png` & `ygt-0.1.3/src/ygt/icons/hand-icon-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/hand-icon-on.png` & `ygt-0.1.3/src/ygt/icons/hand-icon-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/horizontal-off.png` & `ygt-0.1.3/src/ygt/icons/horizontal-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/horizontal-on.png` & `ygt-0.1.3/src/ygt/icons/horizontal-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/interpolate.png` & `ygt-0.1.3/src/ygt/icons/interpolate.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/make_set.png` & `ygt-0.1.3/src/ygt/icons/make_set.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/program.png` & `ygt-0.1.3/src/ygt/icons/program.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/shift.png` & `ygt-0.1.3/src/ygt/icons/shift.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/vertical-off.png` & `ygt-0.1.3/src/ygt/icons/vertical-off.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/vertical-on.png` & `ygt-0.1.3/src/ygt/icons/vertical-on.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/icons/white_distance.png` & `ygt-0.1.3/src/ygt/icons/white_distance.png`

 * *Files identical despite different names*

### Comparing `ygt-0.1.2/src/ygt/macfuncDialog.py` & `ygt-0.1.3/src/ygt/macfuncDialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from typing import Optional, Any
+from PyQt6.QtGui import QIntValidator, QDoubleValidator
 from PyQt6.QtWidgets import (
     QDialog,
     QVBoxLayout,
     QHBoxLayout,
     QDialogButtonBox,
     QComboBox,
     QLineEdit,
     QLabel,
 )
+# from .ygHintEditor import ygHintView
 
 
 class macfuncDialog(QDialog):
-    def __init__(self, _hint):
+    def __init__(self, _hint) -> None:
         super(macfuncDialog, self).__init__(
             _hint.yg_hint.yg_glyph.preferences.top_window()
         )
         self.yg_hint = _hint.yg_hint
-        self.result_dict = None
+        self.result_dict: Optional[dict] = None
         self.setWindowTitle("Parameters for " + str(self.yg_hint.name))
         self.yg_font = self.yg_hint.yg_glyph.yg_font
         self.yg_callable = None
         try:
             self.yg_callable = self.yg_font.functions[self.yg_hint.name]
         except Exception as e:
             # print("in function dialog:")
@@ -29,15 +32,15 @@
             try:
                 self.yg_callable = self.yg_font.macros[self.yg_hint.name]
             except Exception as e:
                 # print("in function dialog:")
                 # print("Error: " + str(e))
                 pass
         self.hint_type = _hint.yg_hint.hint_type()
-        self.layout = QVBoxLayout()
+        self._layout = QVBoxLayout()
         QBtn = (
             QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
         )
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
         self.params = self.yg_hint._get_macfunc()
@@ -69,52 +72,54 @@
                     self.widgets[-1].addWidget(QLineEdit())
                     if kk in self.params:
                         default_value = self.params[kk]
                     elif "val" in self.yg_callable[kk]:
                         default_value = self.yg_callable[kk]["val"]
                     else:
                         default_value = None
-                    self.widgets[-1].itemAt(1).widget().setInputMask("####")
+                    # self.widgets[-1].itemAt(1).widget().setInputMask("####") # type: ignore
+                    self.widgets[-1].itemAt(1).widget().setValidator(QIntValidator())
                     if default_value:
-                        self.widgets[-1].itemAt(1).widget().setText(str(default_value))
+                        self.widgets[-1].itemAt(1).widget().setText(str(default_value)) # type: ignore
                 elif self.yg_callable[kk]["type"] == "float":
                     self.widgets.append(QHBoxLayout())
                     self.widgets[-1].addWidget(QLabel(kk))
                     self.widgets[-1].addWidget(QLineEdit())
                     if kk in self.params:
                         default_value = self.params[kk]
                     elif "val" in self.yg_callable[kk]:
                         default_value = self.yg_callable[kk]["val"]
                     else:
                         default_value = None
-                    self.widgets[-1].itemAt(1).widget().setInputMask("####")
+                    # self.widgets[-1].itemAt(1).widget().setInputMask("####") # type: ignore
+                    self.widgets[-1].itemAt(1).widget().setValidator(QDoubleValidator())
                     if default_value:
-                        self.widgets[-1].itemAt(1).widget().setText(str(default_value))
+                        self.widgets[-1].itemAt(1).widget().setText(str(default_value)) # type: ignore
                 else:
                     pass
         for w in self.widgets:
-            self.layout.addLayout(w)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
+            self._layout.addLayout(w)
+        self._layout.addWidget(self.buttonBox)
+        self.setLayout(self._layout)
 
-    def accept(self):
+    def accept(self) -> None:
         self.result_dict = {"nm": self.yg_hint.macfunc_name()}
         for w in self.widgets:
-            if w.itemAt(1).widget().text() != "None":
-                self.result_dict[w.itemAt(0).widget().text()] = (
-                    w.itemAt(1).widget().text()
+            if w.itemAt(1).widget().text() != "None": # type: ignore
+                self.result_dict[w.itemAt(0).widget().text()] = ( # type: ignore
+                    w.itemAt(1).widget().text() # type: ignore
                 )
         # So param_list is the answer from this dialog. Don't plug it into the
         # hint here, but rather in a QUndoCommand.
         # self.yg_hint._source[self.yg_hint.hint_type()] = param_list
         super().accept()
 
 
 class ygCVTWidget(QComboBox):
-    def __init__(self, hint, _type, default):
+    def __init__(self, hint: Any, _type: str, default: str) -> None:
         super().__init__()
         self.addItem("None")
         # self.setInsertPolicy(QComboBox.InsertPolicy.InsertAlphabetically)
         # cv_list = hint.yg_glyph.yg_font.cvt.get_list(_type, hint.yg_glyph.current_axis())
         cv_list = hint.yg_glyph.yg_font.cvt.get_list(
             hint.yg_glyph,
             type=_type,
@@ -126,9 +131,9 @@
         for c in cv_list:
             self.addItem(c)
             if c == default:
                 self.setCurrentText(default)
         if hint.cv():
             self.setCurrentText(hint.cv())
 
-    def text(self):
+    def text(self) -> str:
         return self.currentText()
```

### Comparing `ygt-0.1.2/src/ygt/makeCVDialog.py` & `ygt-0.1.3/src/ygt/makeCVDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,37 @@
+from typing import Union, Any, Tuple, Optional
 from PyQt6.QtWidgets import (
     QDialog,
     QVBoxLayout,
     QHBoxLayout,
     QDialogButtonBox,
     QComboBox,
     QLineEdit,
     QLabel,
     QWidget,
     QTabWidget,
     QListWidget,
     QPushButton,
     QTableView,
     QCheckBox,
+    QListWidgetItem,
 )
-from PyQt6.QtCore import Qt, pyqtSlot
+from PyQt6.QtCore import Qt, pyqtSlot, QEvent
 from PyQt6.QtGui import QIntValidator, QDoubleValidator
-from .ygModel import unicode_cat_names, reverse_unicode_cat_names, ygMasters, random_id
+from .ygModel import (
+    unicode_cat_names,
+    reverse_unicode_cat_names,
+    ygMasters,
+    random_id,
+    ygFont,
+    ygGlyph,
+    ygPoint,
+    ygcvt
+)
+from .ygPreferences import ygPreferences
 
 NEW_CV_NAME = "New_Control_Value"
 NEW_CV_CONTENT = {"val": 0, "axis": "y", "type": "pos"}
 
 #
 # A dialog (makeCVDialog) for creating a CV based on one or two selected points.
 #
@@ -65,15 +77,15 @@
 
     def set_cv_name(self, s: str):
         ...
 
     def from_current_cv(self, s: str):
         ...
 
-    def set_in_current_cv(self, k: str, s, fallback: None):
+    def set_in_current_cv(self, k: str, s, fallback: Any):
         ...
 
     def has_key(self, k: str):
         ...
 
     def del_key(self, k: str):
         ...
@@ -89,21 +101,21 @@
 
     yg_font (ygFont): The font being edited.
 
     preferences (ygPreferences): The preferences for this app.
 
     """
 
-    def __init__(self, owner, yg_font, preferences):
+    def __init__(self, owner, yg_font: ygFont, preferences: ygPreferences) -> None:
         super().__init__()
         self.owner = owner
         self.yg_font = yg_font
         self._cvt = self.yg_font.cvt
         self.preferences = preferences
-        self.layout = QHBoxLayout()
+        self.layout_obj = QHBoxLayout()
 
         # Set up CV list.
 
         self.cv_list_layout = QVBoxLayout()
         self.button_layout = QHBoxLayout()
 
         self.cv_list = QListWidget()
@@ -124,46 +136,46 @@
         add_button = QPushButton("Add")
         del_button = QPushButton("Delete")
         self.button_layout.addWidget(add_button)
         self.button_layout.addWidget(del_button)
         add_button.clicked.connect(self.add_cv)
         del_button.clicked.connect(self.del_cv)
         self.cv_list_layout.addLayout(self.button_layout)
-        self.layout.addLayout(self.cv_list_layout)
-        self.layout.addWidget(self.edit_pane)
-        self.setLayout(self.layout)
+        self.layout_obj.addLayout(self.cv_list_layout)
+        self.layout_obj.addWidget(self.edit_pane)
+        self.setLayout(self.layout_obj)
 
-    def send_error_message(self, d: dict):
+    def send_error_message(self, d: dict) -> None:
         self.yg_font.send_error_message(d)
 
-    def add_cv(self):
+    def add_cv(self) -> None:
         self._current_cv_name = NEW_CV_NAME
         self._cvt.add_cv(self._current_cv_name, NEW_CV_CONTENT)
         self.cv_list.addItem(self._current_cv_name)
         matches = self.cv_list.findItems(
             self._current_cv_name, Qt.MatchFlag.MatchExactly
         )
         if len(matches) > 0:
             self.current_list_item = matches[0]
             self.cv_list.setCurrentItem(self.current_list_item)
             self.new_item(self.current_list_item, forced=True)
 
-    def change_name_in_list(self, n):
+    def change_name_in_list(self, n) -> None:
         self.current_list_item.setText(n)
 
-    def del_cv(self):
+    def del_cv(self) -> None:
         self._cvt.del_cv(self._current_cv_name)
         self.cv_list.clear()
         try:
             self._current_cv_name = list(self._cvt.keys())[0]
         except IndexError:
             return
         self.refresh()
 
-    def refresh(self):
+    def refresh(self) -> None:
         """This is the place to figure out whether the source
         or masters have been changed: if not, we don't have to
         go through all this.
         """
         if not len(self._cvt):
             self.add_cv()
         self._current_cv = self._cvt.get_cv(self._current_cv_name)
@@ -180,73 +192,73 @@
                 self.cv_list.setCurrentItem(current_item)
                 self._current_cv_name = current_item.text()
                 self._current_cv = self._cvt.get_cv(self._current_cv_name)
             except Exception:
                 pass
         self.edit_pane.refresh(self)
 
-    def fixup(self):
+    def fixup(self) -> None:
         self.edit_pane.fixup()
 
-    def new_item(self, list_item, forced=False):
+    def new_item(self, list_item, forced: bool = False) -> None:
         """Switch the view to another cv. Simply delete the
         old cv editing pane and create a new one to put
         in its place.
         """
         new_cv_name = list_item.text()
         if forced or new_cv_name != self._current_cv_name:
-            old_pane = self.layout.itemAt(1)
-            self.layout.removeItem(old_pane)
+            old_pane = self.layout_obj.itemAt(1)
+            self.layout_obj.removeItem(old_pane)
             old_pane.widget().deleteLater()
             self._current_cv_name = new_cv_name
             self._current_cv = self._cvt.get_cv(self._current_cv_name)
             self.edit_pane = cvWidget(self, self.yg_font, self)
-            self.layout.addWidget(self.edit_pane)
+            self.layout_obj.addWidget(self.edit_pane)
 
-    def cvt(self):
+    def cvt(self) -> ygcvt:
         return self._cvt
 
-    def current_cv(self):
+    def current_cv(self) -> Union[int, dict]:
         return self._current_cv
 
-    def current_cv_name(self):
+    def current_cv_name(self) -> str:
         return self._current_cv_name
 
-    def set_cv_name(self, s: str):
+    def set_cv_name(self, s: str) -> None:
         self._current_cv_name = s
 
     def from_current_cv(self, s: str):
         try:
-            return self._current_cv[s]
+            return self._current_cv[s] # type: ignore
         except KeyError:
             return None
 
-    def set_in_current_cv(self, k: str, s, fallback=None):
+    def set_in_current_cv(self, k: str, s: Any, fallback = Optional[str]) -> None:
         if s == "None" or s == "" or s == None:
             if fallback != None:
                 self._cvt.set_cv_property(self.current_cv_name(), k, fallback)
             else:
-                if k in self._current_cv:
+                if k in self._current_cv: # type: ignore
                     self._cvt.del_cv(k)
         else:
             self._cvt.set_cv_property(self.current_cv_name(), k, s)
 
     def has_key(self, k: str) -> bool:
-        return k in self._current_cv
+        return k in self._current_cv # type: ignore
 
-    def del_key(self, k: str):
+    def del_key(self, k: str) -> None:
         self._cvt.del_cv_property(self.current_cv_name(), k)
 
-    def rename_cv(self, old_name, new_name):
+    def rename_cv(self, old_name: str, new_name: str) -> None:
         self._cvt.rename(old_name, new_name)
 
-    def showEvent(self, event):
+    def showEvent(self, event) -> None:
         self.refresh()
 
-    def hideEvent(self, event):
+    def hideEvent(self, event) -> None:
         self.fixup()
 
 
 class fontInfoWindow(QWidget):
     """A one-stop shop for font-level settings: CVs, masters, font-wide
     defaults.
 
@@ -254,53 +266,53 @@
 
     yg_font (ygFont): The font being edited.
 
     preferences (ygPreferences): The preferences for this app.
 
     """
 
-    def __init__(self, yg_font, preferences):
+    def __init__(self, yg_font: ygFont, preferences: ygPreferences) -> None:
         super().__init__()
         self.yg_font = yg_font
         self.cvt = self.yg_font.cvt
         self.preferences = preferences
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
 
         # Set up tabs
 
         self.tabs = QTabWidget()
         self.cv_tab = cvEditPane(self, self.yg_font, self.preferences)
         self._empty_string = "{}\n"
         self.masters_tab = None
         if self.yg_font.is_variable_font:
             self.masters_tab = mastersWidget(self, self.yg_font)
         self.tabs.addTab(self.cv_tab, "Control Values")
         if self.yg_font.is_variable_font:
             self.tabs.addTab(self.masters_tab, "Masters")
         self.defaults_pane = defaultsPane(self.yg_font)
         self.tabs.addTab(self.defaults_pane, "Defaults")
-        self.layout.addWidget(self.tabs)
-        self.setLayout(self.layout)
+        self.layout_obj.addWidget(self.tabs)
+        self.setLayout(self.layout_obj)
         self.window().setWindowTitle("Font Info")
 
-    def undo_state_active(self):
+    def undo_state_active(self) -> None:
         if not self.yg_font.undo_stack.isActive():
             self.yg_font.undo_stack.setActive(True)
 
-    def closeEvent(self, event):
+    def closeEvent(self, event) -> None:
         self.hide()
 
     @pyqtSlot()
-    def refresh(self):
+    def refresh(self) -> None:
         self.cv_tab.refresh()
         self.defaults_pane.refresh()
         if self.masters_tab:
             self.masters_tab.refresh()
 
-    def event(self, event):
+    def event(self, event) -> bool:
         if event.type() == event.Type.WindowActivate:
             self.undo_state_active()
             # self.yg_font.undo_stack.setActive(True)
         return super().event(event)
 
 
 class mastersWidget(QWidget):
@@ -310,21 +322,21 @@
 
     owner: The owner of this widget.
 
     yg_font (ygFont): The font being edited.
 
     """
 
-    def __init__(self, owner, yg_font):
+    def __init__(self, owner: fontInfoWindow, yg_font: ygFont) -> None:
         super().__init__()
         self.owner = owner
         self.yg_font = yg_font
         self.masters = self.yg_font.masters
 
-        self.layout = QHBoxLayout()
+        self.layout_obj = QHBoxLayout()
         self.master_list_layout = QVBoxLayout()
         self.button_layout = QHBoxLayout()
 
         self.master_list = QListWidget()
         self.master_list.addItems(self.masters.names())
         self.current_list_item = self.master_list.item(0)
         self.master_list.setCurrentItem(self.current_list_item)
@@ -347,59 +359,59 @@
         self.button_layout.addWidget(del_button)
         add_button.clicked.connect(self.add_master)
         del_button.clicked.connect(self.del_master)
         self.master_list_layout.addLayout(self.button_layout)
         self.refresh_variants_button = QPushButton("Generate Variant Control Values")
         self.refresh_variants_button.clicked.connect(self.yg_font.refresh_variant_cvs)
         self.master_list_layout.addWidget(self.refresh_variants_button)
-        self.layout.addLayout(self.master_list_layout)
-        self.layout.addWidget(self.edit_pane)
-        self.setLayout(self.layout)
+        self.layout_obj.addLayout(self.master_list_layout)
+        self.layout_obj.addWidget(self.edit_pane)
+        self.setLayout(self.layout_obj)
 
-    def current_master_name(self):
+    def current_master_name(self) -> str:
         return self._current_master[1]["name"]
 
-    def current_master_id(self):
+    def current_master_id(self) -> str:
         return self._current_master[0]
 
-    def new_item(self, list_item, forced=False):
+    def new_item(self, list_item: QListWidgetItem, forced: bool = False) -> None:
         new_master_name = list_item.text()
         new_master = self.masters.master_by_name(new_master_name)
         if forced or new_master_name != self.current_master_name():
-            old_pane = self.layout.itemAt(1)
-            self.layout.removeItem(old_pane)
+            old_pane = self.layout_obj.itemAt(1)
+            self.layout_obj.removeItem(old_pane)
             old_pane.widget().deleteLater()
             self._current_master = new_master
             self.edit_pane = masterWidget(
                 self.masters, self.current_master_id(), self.yg_font
             )
-            self.layout.addWidget(self.edit_pane)
+            self.layout_obj.addWidget(self.edit_pane)
 
-    def add_master(self):
+    def add_master(self) -> None:
         master_dict = {}
         axis_tags = self.yg_font.axis_tags()
         for a in axis_tags:
             master_dict[a] = 0.0
         master_id = random_id("master")
         master_vals = {"name": master_id, "vals": master_dict}
         self.yg_font.masters.add_master(master_id, master_vals)
         self.refresh()
 
-    def del_master(self):
+    def del_master(self) -> None:
         self.yg_font.masters.del_by_name(self.current_master_name())
         self.master_list.clear()
         try:
             self._current_master = self.masters.master_by_name(
                 self.yg_font.masters.names()[0]
             )
         except IndexError:
             return
         self.refresh()
 
-    def refresh(self):
+    def refresh(self) -> None:
         if not len(self.yg_font.masters):
             return
         self.master_list.clear()
         self.master_list.addItems(self.yg_font.masters.names())
         matches = self.master_list.findItems(
             self.current_master_name(), Qt.MatchFlag.MatchExactly
         )
@@ -426,15 +438,15 @@
 
     m_id (str): The ID of the present master.
 
     yg_font (ygFont): The font being edited.
 
     """
 
-    def __init__(self, masters, m_id, yg_font):
+    def __init__(self, masters: ygMasters, m_id: str, yg_font: ygFont) -> None:
         super().__init__()
         self.masters = masters
         self.m_id = m_id
         self.master_layout = QVBoxLayout()
         self.name_layout = QHBoxLayout()
         self.name_layout.addWidget(QLabel("Name"))
         self.master_name_widget = masterNameWidget(self.masters, self.m_id)
@@ -447,15 +459,15 @@
             axis_val_layout.addWidget(QLabel(axis_name))
             n = masterValWidget(self.masters, self.m_id, axis_name)
             self.names.append(n)
             axis_val_layout.addWidget(n)
             self.master_layout.addLayout(axis_val_layout)
         self.setLayout(self.master_layout)
 
-    def refresh(self, m):
+    def refresh(self, m: Tuple[str, dict]) -> None:
         """Where m is a master tuple (id, dict of axis:val)"""
         self.m_id = m[0]
         self.master_name_widget.refresh(m)
         for n in self.names:
             n.refresh(m)
 
     # def event(self, event):
@@ -468,15 +480,15 @@
 class cvDeltaWidget(QTableView):
     """A table for creating and editing CV Deltas.
 
     params: cv_source (cvSource): The CV to which deltas will be applied.
 
     """
 
-    def __init__(self, cv_source: cvSource):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.delta_data = self.cv_source.cvt().get_deltas(
             self.cv_source.current_cv_name()
         )
         self.setModel(self.delta_data)
 
@@ -502,25 +514,25 @@
     variant pane should be included.
 
     """
 
     def __init__(
         self,
         cv_source: cvSource,
-        yg_font,
-        owner,
+        yg_font: ygFont,
+        owner: cvEditPane,
         parent=None,
-        delta_pane=True,
-        variant_pane=True,
+        delta_pane: bool = True,
+        variant_pane: bool = True,
     ):
         super().__init__(parent=parent)
         self.yg_font = yg_font
         self.owner = owner
         self.cv_source = cv_source
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
 
         # Set up tabs
 
         self.tabs = QTabWidget()
         self.general_tab = QWidget()
         self.link_tab = QWidget()
         self.delta_tab = None
@@ -586,16 +598,16 @@
         self.cv_above_ppem_widget = cvPPEMWidget(self.cv_source, "above")
         self.cv_below_names_widget = cvNamesWidget(
             self.cv_source, "below", self.yg_font, ppem_widget=self.cv_below_ppem_widget
         )
         self.cv_above_names_widget = cvNamesWidget(
             self.cv_source, "above", self.yg_font, ppem_widget=self.cv_above_ppem_widget
         )
-        self.cv_below_ppem_widget.name_widget = self.cv_below_names_widget
-        self.cv_above_ppem_widget.name_widget = self.cv_above_names_widget
+        self.cv_below_ppem_widget.name_widget = self.cv_below_names_widget # type: ignore
+        self.cv_above_ppem_widget.name_widget = self.cv_above_names_widget # type: ignore
 
         self.link_widgets = []
 
         self.link_widgets.append(QHBoxLayout())
         self.link_widgets[-1].addWidget(QLabel("same as"))
         self.link_widgets[-1].addWidget(self.cv_below_names_widget)
 
@@ -621,58 +633,58 @@
         self.delta_tab_layout = None
         if self.delta_tab:
             self.delta_tab_layout = QVBoxLayout()
             self.delta_pane = cvDeltaWidget(self.cv_source)
             self.delta_button_layout = QHBoxLayout()
             add_delta_button = QPushButton("Add")
             del_delta_button = QPushButton("Delete")
-            add_delta_button.clicked.connect(self.delta_pane.model().new_row)
+            add_delta_button.clicked.connect(self.delta_pane.model().new_row) # type: ignore
             del_delta_button.clicked.connect(self.del_delta_row)
             self.delta_button_layout.addWidget(add_delta_button)
             self.delta_button_layout.addWidget(del_delta_button)
             self.delta_tab_layout.addWidget(self.delta_pane)
             self.delta_tab_layout.addLayout(self.delta_button_layout)
 
         # Set up variants tab
 
         self.variants_tab_layout = None
         if self.variants_tab:
             self.variants_tab_layout = QVBoxLayout()
             self.var_widgets = []
             self.var_layouts = []
-            master_keys = self.masters.keys()
+            master_keys = self.masters.keys() # type: ignore
             for k in master_keys:
                 self.var_layouts.append(QHBoxLayout())
-                self.var_layouts[-1].addWidget(QLabel(self.masters.get_master_name(k)))
+                self.var_layouts[-1].addWidget(QLabel(self.masters.get_master_name(k))) # type: ignore
                 self.var_widgets.append(cvVarWidget(k, self.cv_source))
                 self.var_layouts[-1].addWidget(self.var_widgets[-1])
 
         for w in self.gen_widgets:
             self.general_tab_layout.addLayout(w)
         for w in self.link_widgets:
             self.link_tab_layout.addLayout(w)
         if self.variants_tab:
             for w in self.var_layouts:
-                self.variants_tab_layout.addLayout(w)
+                self.variants_tab_layout.addLayout(w) # type: ignore
 
         self.general_tab.setLayout(self.general_tab_layout)
         self.link_tab.setLayout(self.link_tab_layout)
         if self.delta_tab:
-            self.delta_tab.setLayout(self.delta_tab_layout)
+            self.delta_tab.setLayout(self.delta_tab_layout) # type: ignore
         if self.variants_tab:
-            self.variants_tab.setLayout(self.variants_tab_layout)
-        self.layout.addWidget(self.tabs)
-        self.setLayout(self.layout)
+            self.variants_tab.setLayout(self.variants_tab_layout) # type: ignore
+        self.layout_obj.addWidget(self.tabs)
+        self.setLayout(self.layout_obj)
 
-    def del_delta_row(self):
+    def del_delta_row(self) -> None:
         i = self.delta_pane.selectedIndexes()
         if len(i) > 0:
-            self.delta_pane.model().deleteRows(i[0].row(), 1)
+            self.delta_pane.model().deleteRows(i[0].row(), 1) # type: ignore
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         """If we're coming from the source pane, every cv in the
         cvt will have been replaced, so references to it have
         got to be refreshed and the widgets updated as needed.
         Think about whether there's a less awkward way to do
         this.
         """
         self.cv_source = cv_source
@@ -687,15 +699,15 @@
         self.cv_above_ppem_widget.refresh(self.cv_source)
         self.cv_below_names_widget.refresh(self.cv_source)
         self.cv_above_names_widget.refresh(self.cv_source)
         if self.masters:
             for w in self.var_widgets:
                 w.refresh(self.cv_source)
 
-    def fixup(self):
+    def fixup(self) -> None:
         self.cv_name_widget.fixup()
         self.cv_type_widget.fixup()
         self.cv_axis_widget.fixup()
         self.cv_color_widget.fixup()
         self.cv_val_widget.fixup()
         self.cv_cat_widget.fixup()
         self.cv_suffix_widget.fixup()
@@ -718,111 +730,111 @@
 
     params:
 
     yg_font (ygFont): The font being edited.
 
     """
 
-    def __init__(self, yg_font):
+    def __init__(self, yg_font: ygFont) -> None:
         super().__init__()
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
         self.tabs = QTabWidget()
         self.round_widget = hintRoundWidget(yg_font)
         self.misc_widget = miscDefaultsWidget(yg_font)
         self.tabs.addTab(self.round_widget, "Rounding")
         self.tabs.addTab(self.misc_widget, "Miscellaneous")
-        self.layout.addWidget(self.tabs)
-        self.setLayout(self.layout)
+        self.layout_obj.addWidget(self.tabs)
+        self.setLayout(self.layout_obj)
 
-    def refresh(self):
+    def refresh(self) -> None:
         self.round_widget.refresh()
         self.misc_widget.refresh()
 
 
 class hintRoundWidget(QWidget):
     """Widget for editing the initial round state of the seven types of
     hint.
 
     params:
 
     yg_font (ygFont): The font being edited.
 
     """
 
-    def __init__(self, yg_font):
+    def __init__(self, yg_font: ygFont) -> None:
         super().__init__()
         self.yg_font = yg_font
         self.defaults = yg_font.defaults
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
         self.ignore_signal = False
 
         self.anchor_layout = QHBoxLayout()
         self.anchor_checkbox = QCheckBox("Anchor")
         self.anchor_layout.addWidget(self.anchor_checkbox)
-        self.layout.addLayout(self.anchor_layout)
+        self.layout_obj.addLayout(self.anchor_layout)
 
         self.blackdist_layout = QHBoxLayout()
         self.blackdist_checkbox = QCheckBox("Black distance")
         self.blackdist_layout.addWidget(self.blackdist_checkbox)
-        self.layout.addLayout(self.blackdist_layout)
+        self.layout_obj.addLayout(self.blackdist_layout)
 
         self.whitedist_layout = QHBoxLayout()
         self.whitedist_checkbox = QCheckBox("White distance")
         self.whitedist_layout.addWidget(self.whitedist_checkbox)
-        self.layout.addLayout(self.whitedist_layout)
+        self.layout_obj.addLayout(self.whitedist_layout)
 
         self.graydist_layout = QHBoxLayout()
         self.graydist_checkbox = QCheckBox("Gray distance")
         self.graydist_layout.addWidget(self.graydist_checkbox)
-        self.layout.addLayout(self.graydist_layout)
+        self.layout_obj.addLayout(self.graydist_layout)
 
         self.shift_layout = QHBoxLayout()
         self.shift_checkbox = QCheckBox("Shift")
         self.shift_layout.addWidget(self.shift_checkbox)
-        self.layout.addLayout(self.shift_layout)
+        self.layout_obj.addLayout(self.shift_layout)
 
         self.align_layout = QHBoxLayout()
         self.align_checkbox = QCheckBox("Align")
         self.align_layout.addWidget(self.align_checkbox)
-        self.layout.addLayout(self.align_layout)
+        self.layout_obj.addLayout(self.align_layout)
 
         self.interpolate_layout = QHBoxLayout()
         self.interpolate_checkbox = QCheckBox("Interpolate")
         self.interpolate_layout.addWidget(self.interpolate_checkbox)
-        self.layout.addLayout(self.interpolate_layout)
+        self.layout_obj.addLayout(self.interpolate_layout)
 
         self.refresh()
 
         self.anchor_checkbox.stateChanged.connect(self.button_state_changed)
         self.blackdist_checkbox.stateChanged.connect(self.button_state_changed)
         self.whitedist_checkbox.stateChanged.connect(self.button_state_changed)
         self.graydist_checkbox.stateChanged.connect(self.button_state_changed)
         self.shift_checkbox.stateChanged.connect(self.button_state_changed)
         self.align_checkbox.stateChanged.connect(self.button_state_changed)
         self.interpolate_checkbox.stateChanged.connect(self.button_state_changed)
 
-        self.setLayout(self.layout)
+        self.setLayout(self.layout_obj)
 
-    def button_state_changed(self):
+    def button_state_changed(self) -> None:
         if self.ignore_signal:
             return
         r = {}
         r["anchor"] = self.anchor_checkbox.isChecked()
         r["blackdist"] = self.blackdist_checkbox.isChecked()
         r["whitedist"] = self.whitedist_checkbox.isChecked()
         r["graydist"] = self.graydist_checkbox.isChecked()
         r["shift"] = self.shift_checkbox.isChecked()
         r["align"] = self.align_checkbox.isChecked()
         r["interpolate"] = self.interpolate_checkbox.isChecked()
         self.defaults.set_rounding_defaults(r)
 
-    def fixup(self):
+    def fixup(self) -> None:
         pass
 
-    def refresh(self):
+    def refresh(self) -> None:
         self.ignore_signal = True
         self.anchor_checkbox.setChecked(self.defaults.rounding_state("anchor"))
         self.blackdist_checkbox.setChecked(self.defaults.rounding_state("blackdist"))
         self.whitedist_checkbox.setChecked(self.defaults.rounding_state("whitedist"))
         self.graydist_checkbox.setChecked(self.defaults.rounding_state("graydist"))
         self.shift_checkbox.setChecked(self.defaults.rounding_state("shift"))
         self.align_checkbox.setChecked(self.defaults.rounding_state("align"))
@@ -836,77 +848,77 @@
     """GUI for setting defaults that have nothing to do with rounding.
 
     params:
 
     yg_font (ygFont): the font now being edited.
     """
 
-    def __init__(self, yg_font):
+    def __init__(self, yg_font: ygFont) -> None:
         super().__init__()
         self.yg_font = yg_font
         self.defaults = yg_font.defaults
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
         self.ignore_signal = False
 
         self.tt_defaults = QCheckBox("Use TrueType defaults")
         self.tt_defaults.stateChanged.connect(self.toggle_tt_defaults)
 
         self.init_graphics = QCheckBox("Initialize graphics")
         self.init_graphics.stateChanged.connect(self.toggle_init_graphics)
 
         self.assume_always_y = QCheckBox("Assume axis always y")
         self.assume_always_y.stateChanged.connect(self.toggle_assume_always_y)
 
         self.cleartype = QCheckBox("Cleartype")
         self.cleartype.stateChanged.connect(self.toggle_cleartype)
 
-        self.layout.addWidget(self.tt_defaults)
-        self.layout.addWidget(self.init_graphics)
-        self.layout.addWidget(self.assume_always_y)
-        self.layout.addWidget(self.cleartype)
-        self.setLayout(self.layout)
+        self.layout_obj.addWidget(self.tt_defaults)
+        self.layout_obj.addWidget(self.init_graphics)
+        self.layout_obj.addWidget(self.assume_always_y)
+        self.layout_obj.addWidget(self.cleartype)
+        self.setLayout(self.layout_obj)
 
         self.refresh()
 
-    def toggle_tt_defaults(self):
+    def toggle_tt_defaults(self) -> None:
         if self.ignore_signal:
             return
         if self.tt_defaults.isChecked():
             self.defaults.set_default({"use-truetype-defaults": True})
         else:
             self.defaults.del_default("use-truetype-defaults")
 
-    def toggle_init_graphics(self):
+    def toggle_init_graphics(self) -> None:
         if self.ignore_signal:
             return
         if not self.init_graphics.isChecked():
             self.defaults.set_default({"init-graphics": False})
         else:
             self.defaults.del_default("init-graphics")
 
-    def toggle_assume_always_y(self):
+    def toggle_assume_always_y(self) -> None:
         if self.ignore_signal:
             return
         if self.assume_always_y.isChecked():
             self.defaults.set_default({"assume-always-y": True})
         else:
             self.defaults.del_default("assume-always-y")
 
-    def toggle_cleartype(self):
+    def toggle_cleartype(self) -> None:
         if self.ignore_signal:
             return
         if self.cleartype.isChecked():
             self.defaults.set_default({"cleartype": True})
         else:
             self.defaults.del_default("cleartype")
 
-    def fixup(self):
+    def fixup(self) -> None:
         pass
 
-    def refresh(self, ign: bool = True):
+    def refresh(self, ign: bool = True) -> None:
         self.ignore_signal = ign
 
         t = self.defaults.get_default("use-truetype-defaults")
         self.tt_defaults.setChecked(bool(t))
 
         t = self.defaults.get_default("init-graphics")
         if t == None:
@@ -935,16 +947,15 @@
     point is selected.
 
     yg_glyph (ygGlyph): The current glyph.
 
     preferences (ygPreferences): the preferences for this app.
 
     """
-
-    def __init__(self, p1, p2, yg_glyph, preferences):
+    def __init__(self, p1: ygPoint, p2: ygPoint, yg_glyph: ygGlyph, preferences: ygPreferences) -> None:
         super().__init__()
         self.top_window = preferences.top_window()
         self.yg_font = yg_glyph.yg_font
         self._cvt = self.yg_font.cvt
         self.cv = {}
         self.cv_name = ""
         self.axis = preferences.top_window().current_axis
@@ -966,120 +977,122 @@
             if init_type == "pos":
                 val = p1.font_x
             else:
                 val = abs(p1.font_x - p2.font_x)
         self.cv["val"] = val
         self.cv["origin"] = {"glyph": yg_glyph.gname, "ptnum": origin_indices}
 
-        self.layout = QVBoxLayout()
+        self.layout_obj = QVBoxLayout()
 
         self.pane = cvWidget(
             self, self.yg_font, None, delta_pane=False, variant_pane=False
         )
 
         # Set up buttons
 
         QBtn = (
             QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
         )
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
 
-        self.layout.addWidget(self.pane)
-        self.layout.addWidget(self.buttonBox)
-        self.setLayout(self.layout)
+        self.layout_obj.addWidget(self.pane)
+        self.layout_obj.addWidget(self.buttonBox)
+        self.setLayout(self.layout_obj)
         self.setWindowTitle("Make Control Value")
 
-    def send_error_message(self, d: dict):
+    def send_error_message(self, d: dict) -> None:
         self.yg_font.send_error_message(d)
 
-    def cvt(self):
+    def cvt(self) -> ygcvt:
         return self._cvt
 
-    def current_cv(self):
+    def current_cv(self) -> dict:
         return self.cv
 
-    def current_cv_name(self):
+    def current_cv_name(self) -> str:
         return self.cv_name
 
     def set_cv_name(self, s: str):
         self.cv_name = s
 
-    def from_current_cv(self, s: str):
+    def from_current_cv(self, s: str) -> None:
         try:
             return self.cv[s]
         except KeyError:
-            return None
+            pass
 
-    def set_in_current_cv(self, k: str, s, fallback=None):
+    def set_in_current_cv(self, k: str, s: Any, fallback=None) -> None:
         if s == "None" or s == "" or s == None:
             if fallback != None:
                 self.cv[k] = fallback
             else:
-                if k in self._current_cv:
-                    del self._current_cv[k]
+                if k in self.cv:
+                    del self.cv[k]
+                #if k in self._current_cv:
+                #    del self._current_cv[k]
         else:
             self.cv[k] = s
 
-    def has_key(self, k: str):
+    def has_key(self, k: str) -> bool:
         return k in self.cv
 
-    def del_key(self, k: str):
+    def del_key(self, k: str) -> None:
         try:
             del self.cv[k]
         except KeyError:
             pass
 
-    def accept(self):
+    def accept(self) -> None:
         self.pane.fixup()
         if self.cv_name and len(self.cv) > 0:
             self._cvt.add_cv(self.cv_name, self.cv)
         super().accept()
 
-    def showEvent(self, event):
+    def showEvent(self, event) -> None:
         self.yg_font.undo_stack.setActive(True)
 
 
 class cvNameWidget(QLineEdit):
     """A widget for editing the name of a cv. Disable when it shouldn't
     be edited.
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     owner: The owner of this widget.
     """
 
-    def __init__(self, cv_source: cvSource, owner=None):
+    def __init__(self, cv_source: cvSource, owner: Any = None) -> None:
         super().__init__()
         self.owner = owner
         self.cv_source = cv_source
         self.cv_name = self.cv_source.current_cv_name()
         self.dirty = False
         if len(self.cv_name) > 0:
             self.setText(self.cv_name)
             if self.cv_name != NEW_CV_NAME:
                 self.setEnabled(False)
         if self.isEnabled():
             self.editingFinished.connect(self.text_changed)
             self.textChanged.connect(self.set_dirty)
         self.last_val = self.cv_name
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def fixup(self):
+    def fixup(self) -> None:
         t = self._text()
         if self.isEnabled() and self.dirty and t != self.last_val:
             # If the cv name changes, the original cv in the source tree
             # has to be deleted and a new cv entered under the new name.
             # We can either do that (at some risk of bugginess) or disable
             # the cv name widget when the cv is being edited (as opposed
             # to created).
@@ -1087,97 +1100,97 @@
             self.cv_source.set_cv_name(t)
             if self.owner != None:
                 self.owner.change_name_in_list(t)
                 self.owner.rename_cv(old_name, t)
             self.last_val = t
             self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         self.setText(self.cv_source.current_cv_name())
         self.set_clean()
 
 
 class cvTypeWidget(QComboBox):
     """Widget for choosing a CV type.
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     """
 
-    def __init__(self, cv_source: cvSource):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.addItem("pos")
         self.addItem("dist")
         t = self.cv_source.from_current_cv("type")
         self.setCurrentText((lambda: "y" if not t else t)())
         self.currentTextChanged.connect(self.text_changed)
         self.last_val = self.currentText()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.currentText()
 
-    def fixup(self):
+    def fixup(self) -> None:
         t = self.currentText()
         if t != self.last_val:
-            self.cv_source.set_in_current_cv("type", self.currentText())
+            self.cv_source.set_in_current_cv("type", self.currentText(), None)
             self.last_val = t
 
-    def text_changed(self, event):
+    def text_changed(self, event) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         self.setCurrentText(self.cv_source.from_current_cv("type"))
 
 
 class cvColorWidget(QComboBox):
     """Widget for choosing a distance type.
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     """
 
-    def __init__(self, cv_source):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.addItem("None")
         self.addItem("black")
         self.addItem("white")
         self.addItem("gray")
         col = self.cv_source.from_current_cv("col")
         self.setCurrentText((lambda: "None" if not col else col)())
         self.currentTextChanged.connect(self.text_changed)
         self.last_val = self.currentText()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.currentText()
 
-    def fixup(self):
+    def fixup(self) -> None:
         new_text = self.currentText()
         if new_text != self.last_val:
             if self.cv_source.current_cv():
                 if new_text != "None":
-                    self.cv_source.set_in_current_cv("col", new_text)
+                    self.cv_source.set_in_current_cv("col", new_text, None)
                 else:
                     self.cv_source.del_key("col")
             self.last_val = new_text
 
-    def text_changed(self, s):
+    def text_changed(self, s) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         if self.cv_source.has_key("col"):
             self.setCurrentText(self.cv_source.from_current_cv("col"))
         else:
             self.setCurrentText("None")
 
 
@@ -1186,37 +1199,37 @@
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     """
 
-    def __init__(self, cv_source: cvSource):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.addItem("y")
         self.addItem("x")
         axis = self.cv_source.from_current_cv("axis")
         self.setCurrentText((lambda: "y" if not axis else axis)())
         self.currentTextChanged.connect(self.text_changed)
         self.last_val = self.currentText()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.currentText()
 
-    def fixup(self):
+    def fixup(self) -> None:
         t = self.currentText()
         if t != self.last_val:
-            self.cv_source.set_in_current_cv("axis", self.currentText())
+            self.cv_source.set_in_current_cv("axis", self.currentText(), None)
             self.last_val = t
 
-    def text_changed(self, s):
+    def text_changed(self, s) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source) -> None:
         self.cv_source = cv_source
         if self.cv_source.has_key("axis"):
             self.setCurrentText(self.cv_source.from_current_cv("axis"))
         else:
             self.setCurrentText("y")
 
 
@@ -1239,32 +1252,32 @@
         ct = "None"
         if self.cv_source.has_key("cat"):
             ct = unicode_cat_names[self.cv_source.from_current_cv("cat")]
         self.setCurrentText(ct)
         self.currentTextChanged.connect(self.text_changed)
         self.last_val = self.currentText()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.currentText()
 
-    def fixup(self):
+    def fixup(self) -> None:
         new_text = self.currentText()
         if new_text != self.last_val:
             if not new_text or new_text == "None":
                 self.cv_source.del_key("cat")
             else:
                 self.cv_source.set_in_current_cv(
-                    "cat", reverse_unicode_cat_names[new_text]
+                    "cat", reverse_unicode_cat_names[new_text], None
                 )
             self.last_val = new_text
 
-    def text_changed(self, s):
+    def text_changed(self, s) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source) -> None:
         self.cv_source = cv_source
         if self.cv_source.has_key("cat"):
             self.setCurrentText(
                 unicode_cat_names[self.cv_source.from_current_cv("cat")]
             )
         else:
             self.setCurrentText("None")
@@ -1276,45 +1289,45 @@
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     """
 
-    def __init__(self, cv_source: cvSource):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.dirty = False
         suff = self.cv_source.from_current_cv("suffix")
         self.setText((lambda: "None" if not suff else suff)())
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = self.text()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def fixup(self):
+    def fixup(self) -> None:
         if self.dirty:
-            self.cv_source.set_in_current_cv("suffix", self._text())
+            self.cv_source.set_in_current_cv("suffix", self._text(), None)
             self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if t != self.last_val:
             self.fixup()
             self.last_val = t
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         suff = self.cv_source.from_current_cv("suffix")
         self.setText((lambda: "None" if not suff else suff)())
         self.set_clean()
 
 
 class cvVarWidget(QLineEdit):
@@ -1339,50 +1352,50 @@
             k = v[self.var_id]
         self.setText(str(k))
         self.setValidator(QIntValidator(-9999, 9999))
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = str(k)
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def fixup(self):
+    def fixup(self) -> None:
         """The behavior we want is this: if the widget is blank,
         delete the value for this master and display "None"
         in the widget. If widget has a valid integer, plug
         that in.
         """
         if self.dirty:
             new_text = self._text()
             current_vars = self.cv_source.from_current_cv("var")
             if not current_vars:
                 current_vars = {}
             if new_text:
                 current_vars[self.var_id] = int(new_text)
-                self.cv_source.set_in_current_cv("var", current_vars)
+                self.cv_source.set_in_current_cv("var", current_vars, None)
             else:
                 if len(current_vars) == 0:
                     self.cv_source.del_key("var")
-                    self.refresh()
+                    self.refresh(self.cv_source)
             self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if t != self.last_val:
             self.fixup()
             self.last_val = t
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         v = self.cv_source.from_current_cv("var")
         k = "None"
         if v and self.var_id in v:
             k = v[self.var_id]
         self.setText(str(k))
         self.set_clean()
@@ -1393,50 +1406,50 @@
 
     params:
 
     cv_source (cvSource): Data for currently selected CV.
 
     """
 
-    def __init__(self, cv_source: cvSource):
+    def __init__(self, cv_source: cvSource) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.dirty = False
         self.setText(str(self.cv_source.from_current_cv("val")))
         self.setValidator(QIntValidator(-9999, 9999))
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = self.text()
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def fixup(self):
+    def fixup(self) -> None:
         t = self._text()
         if t != self.last_val:
             try:
                 i = int(t)
             except ValueError:
                 i = 0
-            self.cv_source.set_in_current_cv("val", i, fallback=0)
+            self.cv_source.set_in_current_cv("val", i, fallback = 0)
             self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if t != self.last_val:
             self.fixup()
             self.last_val = t
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         i = self.cv_source.from_current_cv("val")
         self.setText((lambda: "0" if not i else str(i))())
         self.set_clean()
 
 
 class cvPPEMWidget(QLineEdit):
@@ -1446,72 +1459,72 @@
 
     cv_source (cvSource): Data for currently selected CV.
 
     above_below (str): Indicating which widget pair is being edited.
 
     """
 
-    def __init__(self, cv_source: cvSource, above_below: str):
+    def __init__(self, cv_source: cvSource, above_below: str) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.above_below = above_below
-        self.name_widget = None
+        self.name_widget: Optional[cvNameWidget] = None
         self.dirty = False
         s = self.cv_source.from_current_cv("same-as")
         v = "40"
         if s:
             try:
                 self.setText(s[self.above_below])
             except Exception:
                 self.setText("40")
         self.setValidator(QIntValidator(0, 500))
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = "40"
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def fixup(self):
+    def fixup(self) -> None:
         new_name = self.name_widget._text()
         name_valid = new_name != "None"
         try:
             new_val = int(self._text())
         except Exception:
             new_val = 40
             self.setText(str(new_val))
         if name_valid:
             s = self.cv_source.from_current_cv("same-as")
             if not s:
                 s = {self.above_below: {}}
             s[self.above_below]["cv"] = new_name
             s[self.above_below]["ppem"] = new_val
-            self.cv_source.set_in_current_cv("same-as", s)
+            self.cv_source.set_in_current_cv("same-as", s, None)
         else:
             if self.cv_source.has_key("same-as"):
                 s = self.cv_source.from_current_cv("same-as")
                 if self.above_below in s:
                     del s[self.above_below]
                 if len(s) == 0:
                     self.cv_source.del_key("same-as")
         self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if t != self.last_val:
             self.fixup()
             self.last_val = t
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         p = "40"
         s = self.cv_source.from_current_cv("same-as")
         if s and self.above_below in s:
             p = str(s[self.above_below]["ppem"])
         self.setText(p)
         self.set_clean()
@@ -1528,15 +1541,21 @@
 
     yg_font (ygFont): The font being edited.
 
     ppem_widget: The associated cvPPEMWidget (if any).
 
     """
 
-    def __init__(self, cv_source: cvSource, above_below, yg_font, ppem_widget=None):
+    def __init__(
+            self,
+            cv_source: cvSource,
+            above_below: str,
+            yg_font: ygFont,
+            ppem_widget: cvPPEMWidget = None
+        ) -> None:
         super().__init__()
         self.cv_source = cv_source
         self.yg_font = yg_font
         self.cvt = yg_font.cvt
         self.above_below = above_below
         self.ppem_widget = ppem_widget
         cv_list = self.cvt.get_list(None)
@@ -1546,25 +1565,25 @@
         n = "None"
         cv = self.cv_source.from_current_cv("same-as")
         if cv and self.above_below in cv:
             n = cv[self.above_below]["cv"]
         self.setCurrentText(n)
         self.currentTextChanged.connect(self.text_changed)
 
-    def _text(self):
+    def _text(self) -> str:
         return self.currentText()
 
-    def fixup(self):
+    def fixup(self) -> None:
         if self.ppem_widget:
             self.ppem_widget.fixup()
 
-    def text_changed(self, s):
+    def text_changed(self, s) -> None:
         self.fixup()
 
-    def refresh(self, cv_source):
+    def refresh(self, cv_source: cvSource) -> None:
         self.cv_source = cv_source
         n = "None"
         if self.cv_source.has_key("same-as"):
             s = self.cv_source.from_current_cv("same-as")
             if self.above_below in s:
                 n = s[self.above_below]["cv"]
         self.setCurrentText(n)
@@ -1578,48 +1597,48 @@
 
     masters (ygMasters): The collection of masters for this font.
 
     m_id (str): The ID of the master associated with this widget.
 
     """
 
-    def __init__(self, masters: ygMasters, m_id: str):
+    def __init__(self, masters: ygMasters, m_id: str) -> None:
         super().__init__()
         self.masters = masters
         self.m_id = m_id
         master_name = self.masters.get_master_name(self.m_id)
         self.setText(master_name)
         self.dirty = False
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = master_name
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def refresh(self, m):
+    def refresh(self, m: tuple) -> None:
         """refresh is for updating editing widgets from the model."""
         self.m_id = m[0]
         self.setText(self.masters.get_master_name(self.m_id))
         self.set_clean()
 
-    def fixup(self):
+    def fixup(self) -> None:
         """fixup is for changing the model based on what's in the editing
         widgets.
         """
         self.masters.set_master_name(self.m_id, self._text())
         self.set_clean()
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if self.dirty and t != self.last_val:
             self.fixup()
             self.last_val = t
 
 
 class masterValWidget(QLineEdit):
@@ -1631,46 +1650,46 @@
 
     m_id (str): The ID of the master associated with this widget.
 
     axis: The variation axis associated with this widget.
 
     """
 
-    def __init__(self, masters: ygMasters, m_id: str, axis):
+    def __init__(self, masters: ygMasters, m_id: str, axis: str) -> None:
         super().__init__()
         self.masters = masters
         self.m_id = m_id
         self.axis = axis
         self.init_val = self.masters.get_axis_value(self.m_id, self.axis)
         if self.init_val == None:
             self.init_val = 0.0
         self.setText(str(self.init_val))
         self.setValidator(QDoubleValidator(-1.0, 1.0, 4))
         self.dirty = False
         self.editingFinished.connect(self.text_changed)
         self.textChanged.connect(self.set_dirty)
         self.last_val = str(self.init_val)
 
-    def _text(self):
+    def _text(self) -> str:
         return self.text().strip()
 
-    def set_dirty(self):
+    def set_dirty(self) -> None:
         self.dirty = True
 
-    def set_clean(self):
+    def set_clean(self) -> None:
         self.dirty = False
 
-    def refresh(self, m):
+    def refresh(self, m: tuple) -> None:
         """refresh is for updating editing widgets from the model."""
         if m:
             self.m_id = m[0]
         self.setText(str(self.masters.get_axis_value(self.m_id, self.axis)))
         self.set_clean()
 
-    def fixup(self):
+    def fixup(self) -> None:
         """fixup is for changing the model based on what's in the editing
         widgets.
         """
         try:
             v = self._text()
             if v == "" or v == "0.0":
                 self.masters.del_axis(self.m_id, self.axis)
@@ -1681,12 +1700,12 @@
                     self.masters.set_axis_value(self.m_id, self.axis, 0.0)
                 self.refresh(None)
             self.set_clean()
         except Exception as e:
             print(e)
             pass
 
-    def text_changed(self):
+    def text_changed(self) -> None:
         t = self._text()
         if self.dirty and t != self.last_val:
             self.fixup()
             self.last_val = t
```

### Comparing `ygt-0.1.2/src/ygt/window.py` & `ygt-0.1.3/src/ygt/window.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import inspect
-from typing import Any, TypeVar, Union
+from typing import Any, TypeVar, Union, Optional
 import sys
 import os
 import copy
 import yaml
 from .ygModel import ygFont, ygGlyph, unicode_cat_names
-from .fontViewDialog import fontViewDialog
+from .fontViewDialog import fontViewWindow
 from .ygPreview import ygPreview, ygStringPreview, ygPreviewContainer
 from .ygYAMLEditor import ygYAMLEditor, editorDialog
 from .ygHintEditor import ygGlyphScene, ygGlyphView
 from .ygPreferences import ygPreferences, open_config
 from .ygSchema import (
     is_cvt_valid,
     is_cvar_valid,
@@ -18,16 +18,16 @@
     are_functions_valid,
     are_defaults_valid,
     are_names_valid,
     are_properties_valid,
 )
 from .ygError import ygErrorMessages
 from .makeCVDialog import fontInfoWindow
-from xgridfit import compile_list, compile_all
-from fontTools import ufoLib
+from xgridfit import compile_list, compile_all # type: ignore
+from fontTools import ufoLib # type: ignore
 from PyQt6.QtCore import Qt, QSize, QThread, pyqtSlot, pyqtSignal, QObject, QEvent
 from PyQt6.QtWidgets import (
     QWidget,
     QApplication,
     QMainWindow,
     QSplitter,
     QMessageBox,
@@ -36,24 +36,28 @@
     QFileDialog,
     QScrollArea,
     QSizePolicy,
     QGraphicsView,
     QLabel,
     QProgressBar,
     QVBoxLayout,
+    QMenu,
 )
 from PyQt6.QtGui import (
     QKeySequence,
     QIcon,
     QPixmap,
     QActionGroup,
     QUndoStack,
     QUndoGroup,
     QCloseEvent,
+    QAction,
+    QFontDatabase,
 )
+from fontTools import ttLib, ufoLib # type: ignore
 
 # FileNameVar = TypeVar("FileNameVar", str, tuple[str, Any])
 FileNameVar = Union[str, tuple[str, Any]]
 # FileNameVar = Any
 
 
 class ygPreviewFontMaker(QThread):
@@ -70,22 +74,22 @@
 
     glyph_list: the names of the glyphs for which we want to make the preview.
     """
 
     sig_preview_ready = pyqtSignal(object)
     sig_preview_error = pyqtSignal()
 
-    def __init__(self, font, source, glyph_list):
+    def __init__(self, font: ttLib.TTFont, source: dict, glyph_list: list) -> None:
         super().__init__()
         self.ft_font = font
         self.source = source
         self.glyph_list = glyph_list
         self.error = False
 
-    def run(self):
+    def run(self) -> None:
         try:
             font = copy.deepcopy(self.ft_font)
             tmp_font, glyph_index, failed_glyph_list = compile_list(
                 font, self.source, self.glyph_list
             )
             self.sig_preview_ready.emit(
                 {"font": tmp_font, "gindex": glyph_index, "failed": failed_glyph_list}
@@ -96,104 +100,110 @@
 
 class ygFontGenerator(QThread):
     """For generating whole fonts."""
 
     sig_font_gen_done = pyqtSignal(object)
     sig_font_gen_error = pyqtSignal()
 
-    def __init__(self, font, source, output_font):
+    def __init__(self, font: ttLib.TTFont, source: dict, output_font: str) -> None:
         super().__init__()
         self.ft_font = font
         self.source = source
         self.output_font = output_font
         self.error = False
 
-    def run(self):
+    def run(self) -> None:
         try:
             font = copy.deepcopy(self.ft_font)
             failed_glyph_list = compile_all(font, self.source, self.output_font)
             self.sig_font_gen_done.emit(failed_glyph_list)
         except KeyError as e:
             self.sig_font_gen_error.emit()
 
 
 class MainWindow(QMainWindow):
-    def __init__(self, app, win_list=None, prefs=None, parent=None):
+    def __init__(
+            self,
+            app: QApplication,
+            win_list: Optional[list] = None,
+            prefs: Optional[ygPreferences] = None,
+            parent = None
+        ):
         super(MainWindow, self).__init__(parent=parent)
         self.undo_group = QUndoGroup()
         self.undo_group.cleanChanged.connect(self.clean_changed)
         # The undo registry should keep a record of undo stacks for each
         # glyph that has been edited, and for the prep, cvar, fpgm, macros,
         # and defaults.
         self.error_manager = ygErrorMessages(self)
         if not win_list:
             self.win_list = [self]
         else:
             self.win_list = win_list
-        self.filename = None
-        self.filename_extension = None
-        self.font_info_editor = None
-        self.cvt_editor = None
+        self.filename = ""
+        # self.filename_extension = ""
+        self.font_info_editor: Optional[fontInfoWindow] = None
+        self.cvt_editor: Optional[editorDialog] = None
         # self.cvar_editor = None
-        self.prep_editor = None
-        self.function_editor = None
-        self.macro_editor = None
-        self.default_editor = None
-        self.font_viewer = None
+        self.prep_editor: Optional[editorDialog] = None
+        self.function_editor: Optional[editorDialog] = None
+        self.macro_editor: Optional[editorDialog] = None
+        self.default_editor: Optional[editorDialog] = None
+        self.font_viewer: Optional[fontViewWindow] = None
         self.statusbar = self.statusBar()
         self.statusbar_label = QLabel()
         self.statusbar_label.setStyleSheet(
             "QLabel {font-family: Source Code Pro, monospace; margin-left: 10px; }"
         )
         self.statusbar.addWidget(self.statusbar_label)
 
         self.prog_path = os.path.split(__file__)[0]
         self.icon_path = self.prog_path + "/icons/"
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.setWindowTitle("YGT")
         self.toolbar = self.addToolBar("Tools")
         self.toolbar.setIconSize(QSize(32, 32))
-        self.progress_bar = None
-        self.progress_bar_action = None
+        self.progress_bar: Optional[QProgressBar] = None
+        self.progress_bar_action: Optional[QAction] = None
         self.spacer = QWidget()
         self.spacer.setSizePolicy(
             QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
         )
         self.spacer_action = self.toolbar.addWidget(self.spacer)
         self.preview_container = QVBoxLayout()
         self.qs = QSplitter(self)
-        self.glyph_pane = None
-        self.preview_glyph_name = None
-        self.preview_glyph_name_list = []
-        self.yg_font = None
-        self.source_editor = None
-        self.preview_scroller = None
-        self.yg_preview = None
-        self.yg_string_preview = None
+        self.glyph_pane: Optional[ygGlyphView] = None
+        self.preview_glyph_name: Optional[str] = None
+        self.preview_glyph_name_list: list = []
+        self.yg_font: Optional[ygFont] = None
+        self.source_editor: Optional[ygYAMLEditor] = None
+        self.preview_scroller: Optional[QScrollArea] = None
+        self.yg_preview = None # type: Optional[ygPreview]
+        self.yg_string_preview: Optional[ygStringPreview] = None
         self.app = app
 
         # Stuff that's stored in the preference file
-        self.preferences = None
-        self.points_as_coords = None
-        self.zoom_factor = None
-        self.show_off_curve_points = None
-        self.show_point_numbers = None
+        self.preferences: Optional[ygPreferences] = None
+        self.points_as_coords = False
+        self.zoom_factor: Optional[float] = None
+        self.show_off_curve_points: Optional[bool] = None
+        self.show_point_numbers: Optional[bool] = None
         self.current_axis = "y"
         if prefs == None:
             self.get_preferences(ygPreferences())
         else:
             self.get_preferences(prefs)
 
-        self.recents_display = []
-        self.recents_actions = []
-        self.instance_actions = []
-        self.window_list = []
-        self.thread = None
-        self.preview_maker = None
-        self.font_generator = None
+        self.recents_display: list = []
+        self.recents_actions: list = []
+        self.instance_actions: list = []
+        self.window_list: list = []
+        # self.thread = None
+        self.preview_maker: Optional[ygPreviewFontMaker] = None
+        self.font_generator: Optional[ygFontGenerator] = None
         self.auto_preview_update = True
 
         self.menu = self.menuBar()
 
         #
         # File menu
         #
@@ -285,40 +295,40 @@
         self.pv_bigger_one_action.setShortcut(
             QKeySequence.StandardKey.MoveToPreviousLine
         )
         self.pv_bigger_one_action.setEnabled(False)
 
         self.pv_bigger_ten_action = self.preview_menu.addAction("Grow by Ten")
         self.pv_bigger_ten_action.setShortcut(
-            QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Up)
+            QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Up) # type: ignore
         )
         self.pv_bigger_ten_action.setEnabled(False)
 
         self.pv_smaller_one_action = self.preview_menu.addAction("Shrink by One")
         self.pv_smaller_one_action.setShortcut(QKeySequence.StandardKey.MoveToNextLine)
         self.pv_smaller_one_action.setEnabled(False)
 
         self.pv_smaller_ten_action = self.preview_menu.addAction("Shrink by Ten")
         self.pv_smaller_ten_action.setShortcut(
-            QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Down)
+            QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_Down) # type: ignore
         )
         self.pv_smaller_ten_action.setEnabled(False)
 
         self.pv_show_hints_action = self.preview_menu.addAction("Show hinting")
         self.pv_show_hints_action.setShortcut(QKeySequence("Ctrl+t"))
         self.pv_show_hints_action.setCheckable(True)
         self.pv_show_hints_action.setChecked(True)
         self.pv_show_hints_action.setEnabled(False)
 
         self.pv_show_grid_action = self.preview_menu.addAction("Show grid")
         self.pv_show_grid_action.setCheckable(True)
         self.pv_show_grid_action.setChecked(True)
         self.pv_show_grid_action.setEnabled(False)
 
-        self.instance_menu = None
+        self.instance_menu: Optional[QMenu] = None
 
         self.preview_menu.addSeparator()
 
         self.pv_set_size_action = self.preview_menu.addAction("Pixels per Em...")
         self.pv_set_size_action.setShortcut(QKeySequence("Ctrl+p"))
         self.pv_set_size_action.setEnabled(False)
 
@@ -479,83 +489,59 @@
 
         cursor_action_group.addAction(self.cursor_action)
         cursor_action_group.addAction(self.hand_action)
         self.cursor_action.setChecked(True)
         self.cursor_action.setEnabled(False)
         self.hand_action.setEnabled(False)
 
-        self.black_action = self.toolbar.addAction("Black Distance (B)")
-        self.black_action.setIcon(QIcon(QPixmap(self.icon_path + "black_distance.png")))
-        self.black_action.setShortcuts(
+        self.stem_action = self.toolbar.addAction("Stem (T)")
+        self.stem_action.setIcon(QIcon(QPixmap(self.icon_path + "stem_distance.png")))
+        self.stem_action.setShortcuts(
             [
-                QKeySequence(Qt.Key.Key_B),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_B),
-                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_B),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_B),
+                QKeySequence(Qt.Key.Key_T),
+                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_T), # type: ignore
+                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_T), # type: ignore
+                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_T), # type: ignore
             ]
         )
-        self.black_action.setEnabled(False)
+        self.stem_action.setEnabled(False)
 
-        self.toolbar.insertSeparator(self.black_action)
+        self.toolbar.insertSeparator(self.stem_action)
 
-        self.white_action = self.toolbar.addAction("White Distance (W)")
-        self.white_action.setIcon(QIcon(QPixmap(self.icon_path + "white_distance.png")))
-        self.white_action.setShortcuts(
-            [
-                QKeySequence(Qt.Key.Key_W),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_W),
-                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_W),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_W),
-            ]
-        )
-        self.white_action.setEnabled(False)
-
-        self.gray_action = self.toolbar.addAction("Gray Distance (G)")
-        self.gray_action.setIcon(QIcon(QPixmap(self.icon_path + "gray_distance.png")))
-        self.gray_action.setShortcuts(
-            [
-                QKeySequence(Qt.Key.Key_G),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_G),
-                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_G),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_G),
-            ]
-        )
-        self.gray_action.setEnabled(False)
-
-        self.shift_action = self.toolbar.addAction("Shift (S)")
+        self.shift_action = self.toolbar.addAction("Shift (H)")
         self.shift_action.setIcon(QIcon(QPixmap(self.icon_path + "shift.png")))
         self.shift_action.setShortcuts(
-            [QKeySequence(Qt.Key.Key_S), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_S)]
+            [QKeySequence(Qt.Key.Key_H), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_H)] # type: ignore
         )
         self.shift_action.setEnabled(False)
 
         self.align_action = self.toolbar.addAction("Align (L)")
         self.align_action.setIcon(QIcon(QPixmap(self.icon_path + "align.png")))
         self.align_action.setShortcuts(
-            [QKeySequence(Qt.Key.Key_L), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_L)]
+            [QKeySequence(Qt.Key.Key_L), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_L)] # type: ignore
         )
         self.align_action.setEnabled(False)
 
         self.interpolate_action = self.toolbar.addAction("Interpolate (I)")
         self.interpolate_action.setIcon(
             QIcon(QPixmap(self.icon_path + "interpolate.png"))
         )
         self.interpolate_action.setShortcuts(
-            [QKeySequence(Qt.Key.Key_I), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_I)]
+            [QKeySequence(Qt.Key.Key_I), QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_I)] # type: ignore
         )
         self.interpolate_action.setEnabled(False)
 
         self.anchor_action = self.toolbar.addAction("Anchor (A)")
         self.anchor_action.setIcon(QIcon(QPixmap(self.icon_path + "anchor.png")))
         self.anchor_action.setShortcuts(
             [
                 QKeySequence(Qt.Key.Key_A),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_A),
-                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_A),
-                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_A),
+                QKeySequence(Qt.Modifier.CTRL | Qt.Key.Key_A), # type: ignore
+                QKeySequence(Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
+                QKeySequence(Qt.Modifier.CTRL | Qt.Modifier.SHIFT | Qt.Key.Key_A), # type: ignore
             ]
         )
         self.anchor_action.setEnabled(False)
 
         self.make_set_action = self.toolbar.addAction("Make Set (K)")
         self.make_set_action.setIcon(QIcon(QPixmap(self.icon_path + "make_set.png")))
         self.make_set_action.setShortcut(QKeySequence(Qt.Key.Key_K))
@@ -690,19 +676,19 @@
 
     #
     # Font view window
     #
 
     @pyqtSlot()
     def show_font_view(self) -> None:
-        """Display the modeless dialog in fontViewDialog.py."""
+        """Display the modeless dialog in fontViewWindow.py."""
         if not self.font_viewer:
             font_name = self.yg_font.font_files.in_font()
             glyph_list = self.yg_font.glyph_list
-            self.font_viewer = fontViewDialog(font_name, self.yg_font, glyph_list, self)
+            self.font_viewer = fontViewWindow(font_name, self.yg_font, glyph_list, self)
         if self.font_viewer.valid:
             self.font_viewer.show()
             self.font_viewer.raise_()
             self.font_viewer.activateWindow()
         else:
             self.error_manager.new_message(
                 {"msg": "Can't create the font view dialog.", "mode": "console"}
@@ -827,17 +813,15 @@
             a.triggered.connect(self.open_recent)
 
     def disconnect_recents_connections(self) -> None:
         for a in self.recents_actions:
             a.triggered.disconnect(self.open_recent)
 
     def setup_hint_connections(self) -> None:
-        self.black_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
-        self.white_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
-        self.gray_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
+        self.stem_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.anchor_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.interpolate_action.triggered.connect(
             self.glyph_pane.make_hint_from_selection
         )
         self.shift_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.align_action.triggered.connect(self.glyph_pane.make_hint_from_selection)
         self.make_set_action.triggered.connect(self.glyph_pane.make_set)
@@ -1042,15 +1026,15 @@
         glyph = self.glyph_pane.viewer.yg_glyph
         glyph_backup = copy.deepcopy(glyph.gsource)
         glyph.cleanup_glyph()
         self.yg_font.source_file.save_source(top_window=self)
         glyph.gsource.clear()
         for k in glyph_backup.keys():
             glyph.gsource[k] = glyph_backup[k]
-        self.undo_group.set_all_clean()
+        self.set_all_clean()
 
     @pyqtSlot()
     def export_font(self) -> None:
         try:
             if self.font_generator != None and self.font_generator.isRunning():
                 return
         except RuntimeError as e:
@@ -1104,15 +1088,15 @@
         emsg = "Failed to generate the font. This most likely due to an error "
         emsg += "in function, macro, or prep code or in your cvt or cvar "
         emsg += "entries."
         self.error_manager.new_message({"msg": emsg, "mode": "console"})
 
     @pyqtSlot()
     def open_recent(self) -> None:
-        f = self.sender().text()
+        f = self.sender().text() # type: ignore
         ff = None
         try:
             i = self.recents_display.index(f)
             ff = self.preferences["recents"][i]
         except Exception as e:
             print("Failure while trying to open recent file:")
             print(e)
@@ -1260,15 +1244,16 @@
         self.code_menu.setEnabled(True)
         self.view_menu.setEnabled(True)
 
         if filename:
             self.preferences.add_recent(filename)
             split_fn = os.path.splitext(filename)
             fn_base = split_fn[0]
-            self.filename_extension = extension = split_fn[1]
+            # self.filename_extension = extension = split_fn[1]
+            extension = split_fn[1]
             yaml_source = {}
             # If file is .ttf, create a skeleton yaml_source and a ygt_filename.
             # If file is .ufo, read yaml source if possible, or if not create skeleton.
             if extension == ".ttf":
                 ygt_filename = fn_base + ".yaml"
                 self.preferences.add_recent(ygt_filename)
                 yaml_source = self._initialize_source(filename, fn_base, extension)
@@ -1320,71 +1305,64 @@
             self.setup_point_label_connections()
         return 0
 
     #
     # GUI management
     #
 
-    def selection_changed(self, selection_profile):
+    def setup_stem_buttons(self, axis):
+        pass
+
+    def selection_changed(self, selection_profile: list):
         total_selected = selection_profile[0] + selection_profile[1]
         # fix up make cv button
         if total_selected >= 1 and total_selected <= 2:
             self.make_cv_action.setEnabled(True)
         else:
             self.make_cv_action.setEnabled(False)
         if 0 in selection_profile[3] or 3 in selection_profile[3]:
             self.make_cv_guess_action.setEnabled(True)
         else:
             self.make_cv_guess_action.setEnabled(False)
         if selection_profile[0] == 0 and selection_profile[1] == 1:
             # enable anchor button
             self.anchor_action.setEnabled(True)
-            self.black_action.setEnabled(False)
-            self.white_action.setEnabled(False)
-            self.gray_action.setEnabled(False)
+            self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.make_set_action.setEnabled(False)
         elif selection_profile[0] == 1 and selection_profile[1] >= 1:
             # Enable make set button
             if 1 in selection_profile[2] or 2 in selection_profile[2]:
                 self.make_set_action.setEnabled(True)
             else:
                 self.make_set_action.setEnabled(False)
             if selection_profile[1] == 1:
                 # Enable link buttons
-                self.black_action.setEnabled(True)
-                self.white_action.setEnabled(True)
-                self.gray_action.setEnabled(True)
+                self.stem_action.setEnabled(True)
                 self.shift_action.setEnabled(True)
                 self.align_action.setEnabled(True)
             else:
-                self.black_action.setEnabled(False)
-                self.white_action.setEnabled(False)
-                self.gray_action.setEnabled(False)
+                self.stem_action.setEnabled(False)
                 self.shift_action.setEnabled(False)
                 self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
         elif selection_profile[0] == 2 and selection_profile[1] == 1:
             # Enable interpolation button
             self.interpolate_action.setEnabled(True)
-            self.black_action.setEnabled(False)
-            self.white_action.setEnabled(False)
-            self.gray_action.setEnabled(False)
+            self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
             self.make_set_action.setEnabled(False)
         else:
             # "Disable all hint editing buttons
-            self.black_action.setEnabled(False)
-            self.white_action.setEnabled(False)
-            self.gray_action.setEnabled(False)
+            self.stem_action.setEnabled(False)
             self.shift_action.setEnabled(False)
             self.align_action.setEnabled(False)
             self.interpolate_action.setEnabled(False)
             self.anchor_action.setEnabled(False)
             self.make_set_action.setEnabled(False)
 
     @pyqtSlot()
@@ -1562,16 +1540,16 @@
 
     #
     # Program exit
     #
 
     def save_query(self) -> int:
         msg_box = QMessageBox()
-        msg_box.setText("The YAML source has been modified.")
-        msg_box.setInformativeText("Do you want to save it?")
+        msg_box.setText("This font’s hints have been modified.")
+        msg_box.setInformativeText("Do you want to save your work?")
         msg_box.setStandardButtons(
             QMessageBox.StandardButton.Discard
             | QMessageBox.StandardButton.Cancel
             | QMessageBox.StandardButton.Save
         )
         msg_box.setDefaultButton(QMessageBox.StandardButton.Save)
         ret = msg_box.exec()
@@ -1644,15 +1622,20 @@
         self.preferences.set_top_window_size(
             event.size().width(), event.size().height()
         )
 
     def moveEvent(self, event):
         self.preferences.set_top_window_pos(event.pos().x(), event.pos().y())
 
-    def get_preferences(self, prefs: ygPreferences) -> None:
+    def event(self, event) -> bool:
+        if event.type() == event.Type.WindowActivate and self.glyph_pane:
+                self.glyph_pane.viewer.yg_glyph.undo_stack.setActive(True)
+        return super().event(event)
+
+    def get_preferences(self, prefs: Optional[ygPreferences]) -> None:
         self.preferences = prefs
         self.points_as_coords = self.preferences.points_as_coords()
         self.zoom_factor = self.preferences.zoom_factor()
         self.show_off_curve_points = self.preferences.show_off_curve_points()
         self.show_point_numbers = self.preferences.show_point_numbers()
 
     def set_preferences(self) -> None:
@@ -1674,17 +1657,21 @@
         if event.type() == QEvent.Type.ActivationChange:
             if self.top_window.isActiveWindow():
                 self.top_window.preferences["top_window"] = self.top_window
         return super().eventFilter(source, event)
 
 
 def main():
-    # print(dir(Qt))
+    # from PyQt6.QtGui import QPalette
+    # print(dir(QPalette))
     # print(inspect.getargspec(freetype.Face.get_glyph_name))
 
     app = QApplication([])
+    font_id = QFontDatabase.addApplicationFont(os.path.dirname(__file__) + "/fonts/SourceCodePro-Regular.ttf")
+    if font_id == -1:
+        print("Can't find the font Source Code Pro.")
     top_window = MainWindow(app)
     top_window.get_preferences(open_config(top_window))
     app.setWindowIcon(QIcon(top_window.icon_path + "program.png"))
     top_window.set_size_and_position()
     top_window.show()
     sys.exit(app.exec())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ygt-0.1.2/src/ygt/ygError.py` & `ygt-0.1.3/src/ygt/ygError.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
+from typing import Any, Optional
 from collections import deque
 from PyQt6.QtWidgets import QPlainTextEdit
 from PyQt6.QtCore import Qt, QSize, QThread, pyqtSlot, pyqtSignal, QObject, QEvent
 
 
 class ygErrorWindow(QPlainTextEdit):
     def __init__(self, init_text: list = []) -> None:
         super().__init__()
         self.setMaximumBlockCount(100)
         self.setReadOnly(True)
         if len(init_text) > 0:
             self.fill_in(init_text)
         self.window().setWindowTitle("Error Console")
 
-    def fill_in(self, msg_list):
+    def fill_in(self, msg_list: list) -> None:
         self.clear()
         for m in msg_list:
             self.appendPlainText(m)
         self.centerCursor()
 
-    def add_message(self, m):
+    def add_message(self, m: str) -> None:
         self.appendPlainText("")
         self.appendPlainText(m)
         self.centerCursor()
 
-    def closeEvent(self, event):
+    def closeEvent(self, event) -> None:
         self.hide()
 
 
 class ygErrorMessages:
-    def __init__(self, top_window):
-        self.error_pane = None
+    def __init__(self, top_window: Any) -> None:
+        self.error_pane: Optional[ygErrorWindow] = None
         self.top_window = top_window
         self.last_message = ""
 
     # @pyqtSlot(object)
-    def new_message(self, m: dict):
+    def new_message(self, m: dict) -> None:
         msg = m["msg"]
         if msg and (msg != self.last_message):
             self.last_message = msg
             if m["mode"] == "console":
                 if not self.error_pane:
                     self.error_pane = ygErrorWindow()
                     qg = self.top_window.screen().availableGeometry()
```

### Comparing `ygt-0.1.2/src/ygt/ygHintEditor.py` & `ygt-0.1.3/src/ygt/ygHintEditor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,82 @@
+from typing import Any, TypeVar, Union, Optional, List, Dict, Callable, overload, Tuple
 import sys
 import uuid
 import copy
 from .macfuncDialog import macfuncDialog
 from .makeCVDialog import makeCVDialog
 from .ygModel import (
+    ygFont,
     ygSet,
     ygParams,
     ygPoint,
     ygPointSorter,
     ygHint,
     hint_type_nums,
     ygCaller,
     ygFunction,
     ygMacro,
     ygGlyph,
     unicode_cat_names,
 )
+from .ygStems import stemFinder
 from PyQt6.QtCore import (
     Qt,
+    QPoint,
     QPointF,
     QSizeF,
     QRectF,
     pyqtSignal,
     QLine,
     QLineF,
     pyqtSlot,
     QObject,
 )
-from PyQt6.QtGui import QPainterPath, QPen, QBrush, QColor, QPolygonF, QAction
+from PyQt6.QtGui import (
+    QPainterPath,
+    QPen,
+    QBrush,
+    QColor,
+    QPolygonF,
+    QAction,
+    QPainter,
+)
 from PyQt6.QtWidgets import (
+    QWidget,
     QApplication,
     QGraphicsScene,
     QGraphicsView,
     QGraphicsItem,
     QGraphicsEllipseItem,
     QGraphicsRectItem,
     QGraphicsLineItem,
     QGraphicsPathItem,
     QGraphicsPolygonItem,
     QMenu,
     QLabel,
     QDialog,
     QInputDialog,
     QLineEdit,
+    QGraphicsProxyWidget,
+    QStyleOptionGraphicsItem,
 )
-from fontTools.pens.basePen import BasePen
+from fontTools.pens.basePen import BasePen  # type: ignore
+from .ygPreferences import ygPreferences
 
 
 HINT_ARROW_WIDTH = 3
 HINT_ANCHOR_WIDTH = 3
 HINT_LINK_WIDTH = 1
 HINT_ARROWHEAD_WIDTH = 2
 HINT_COLLECTION_COLOR = QColor(0, 255, 0, 128)
 HINT_COLLECTION_SELECT_COLOR = QColor(0, 205, 0, 128)
 HINT_ANCHOR_COLOR = QColor(255, 0, 255, 128)
 HINT_ANCHOR_SELECT_COLOR = QColor(175, 0, 175, 128)
 HINT_STEM_COLOR = QColor(255, 0, 0, 128)
-HINT_STEM_SELECT_COLOR = QColor(205, 0, 0, 128)
+HINT_STEM_SELECT_COLOR = QColor(175, 0, 0, 128)
 HINT_SHIFT_COLOR = QColor(100, 100, 255, 128)
 HINT_SHIFT_SELECT_COLOR = QColor(0, 0, 150, 128)
 HINT_ALIGN_COLOR = QColor(0, 255, 0, 128)
 HINT_ALIGN_SELECT_COLOR = QColor(0, 205, 0, 128)
 HINT_LINK_COLOR = QColor(127, 127, 255, 255)
 HINT_LINK_SELECT_COLOR = QColor(87, 87, 215, 255)
 HINT_FUNC_COLOR = QColor(0, 205, 0, 128)
@@ -194,34 +210,36 @@
         self.path.quadTo(*p1, *p2)
 
     def _closePath(self):
         self.path.closeSubpath()
 
 
 class ygSelectable:
-    def _prepare_graphics(self):
+    """Mixin superclass for graphical objects that can be selected."""
+
+    def _prepare_graphics(self) -> None:
         pass
 
-    def update(self):
+    def update(self) -> None:
         pass
 
-    def _is_yg_selected(self):
+    def _is_yg_selected(self) -> bool:
         pass
 
-    def yg_select(self):
+    def yg_select(self) -> None:
         pass
 
-    def yg_unselect(self):
+    def yg_unselect(self) -> None:
         pass
 
 
 class ygHintView(QGraphicsItem, ygSelectable):
     """Wrapper for a ygModel.ygHint object."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Constructor for ygHintView
 
         Parameters:
         args[0] (ygGlyphScene): The scene that owns this. We can't always
         call scene() because we sometimes need that reference before this
         is added to the scene.
 
@@ -230,114 +248,119 @@
         args[2]: either a component of the graphical hint or a list of them.
 
         """
         super().__init__()
         self._is_selected = False
         self.yg_glyph_view = args[0]
         self.yg_hint = args[1]
-        self.label = None
+        self.label: Optional[QLabel] = None
         self.label_proxy = None
         self.description = self._set_description()
         if len(args) >= 3:
             # graphical_hint may arrive as an irregularly nested list.
             # flatten it into a simple list
             self.graphical_hint = list(self._traverse(args[2]))
             for g in self.graphical_hint:
                 g.setParentItem(self)
 
-    def _set_description(self):
+    def _set_description(self) -> str:
         result = self.yg_hint.hint_type()
         if hasattr(self.yg_hint, "cvt"):
             result += " (" + str(self.yg_hint.cv()) + ")"
         # Tooltip not yet. By default, the tooltip appears when the mouse is
         # anywhere in a widget's bounding rect. For hints that is not helpful.
         # *** There is a way to change this behavior: figure it out later.
         # self.setToolTip(result)
         return result
 
-    def _set_name(self, name):
+    def _set_name(self, name: str) -> None:
         self.yg_hint.name = name
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: gray;}")
         self.label.setText(name)
         self.label_proxy = self.yg_glyph_view.addWidget(self.label)
         rect = self.boundingRect()
         self.label.move(
             round(rect.topLeft().x()), round(rect.topLeft().y() - self.label.height())
         )
 
-    def _remove_labels(self):
+    def _remove_labels(self) -> None:
         if self.label_proxy:
             self.yg_glyph_view.removeItem(self.label_proxy)
         for g in self.graphical_hint:
             if hasattr(g, "_remove_labels"):
                 g._remove_labels()
 
     # Adapted from https://stackoverflow.com/questions/6340351/iterating-through-list-of-list-in-python
     # Presumed public domain.
-    def _traverse(self, o):
+    def _traverse(self, o) -> Any:
         if isinstance(o, list):
             for value in o:
                 for subvalue in self._traverse(value):
                     yield subvalue
         else:
             yield o
 
-    def paint(self, painter, option, widget):
+    def paint(
+        self,
+        painter: QPainter,
+        option: QStyleOptionGraphicsItem,
+        widget: Optional[QWidget] = None,
+    ) -> None:
         """Got to be here, but it doesn't have to do anything."""
         pass
 
-    def boundingRect(self):
+    def boundingRect(self) -> QRectF:
         if len(self.graphical_hint) >= 1:
             resultRect = None
             for g in self.graphical_hint:
                 if resultRect == None:
                     resultRect = g.boundingRect()
                 else:
                     resultRect = g.boundingRect().united(resultRect)
             return resultRect
         else:
             return None  # This shouldn't happen. Behavior undefined if it does.
 
-    def contains(self, pt):
+    def contains(self, pt: QPointF) -> bool:
         if len(self.graphical_hint) >= 1:
             for g in self.graphical_hint:
                 if g.contains(pt):
                     return True
         return False
 
-    def mouse_over_point(self, pt):
+    def mouse_over_point(self, pt: QPointF) -> "ygPointMarker":
         """In ygHintView. Returns a ygPointMarker."""
         if len(self.graphical_hint) >= 1:
             for g in self.graphical_hint:
                 if type(g) is ygPointMarker and g.contains(pt):
                     return g
         return None
 
-    def get_scene(self):
+    def get_scene(self) -> "ygGlyphScene":
         return self.yg_glyph_view
 
-    def _target_list(self):
+    def _target_list(self) -> list:
         """Returns a list of target points for this hint."""
         mpt = self.yg_glyph_view.resolve_point_identifier(self.yg_hint.target())
         mypoints = []
         if type(mpt) is ygSet:
             for p in mpt.point_list():
                 mypoints.append(p)
         elif type(mpt) is ygParams:
             mypoints.extend(self._get_macfunc_targets(mpt))
         elif type(mpt) is not list:
             mypoints.append(self.yg_glyph_view.resolve_point_identifier(mpt))
         return mypoints
 
-    def _update_touches(self):
+    def _update_touches(self) -> None:
         self._remove_touches()
         self._touch_all_points()
 
-    def _get_macfunc_targets(self, p):
+    def _get_macfunc_targets(self, p: ygParams) -> list:
         """p should be the point_dict from a ygParams object. Survey all the
         point params in a macro or function definition and touch any marked
         as "target."
 
         """
         macfunc_name = self.yg_hint.name
         plist = []
@@ -346,39 +369,40 @@
                 if self.yg_hint.hint_type() == "macro":
                     macfunc = self.yg_glyph_view.yg_glyph.yg_font.macros[macfunc_name]
                 elif self.yg_hint.hint_type() == "function":
                     macfunc = self.yg_glyph_view.yg_glyph.yg_font.functions[
                         macfunc_name
                     ]
                 else:
-                    raise Exception(str(macfunc_name) + " not function or macro!")
+                    # raise Exception(str(macfunc_name) + " not function or macro!")
+                    return plist
                 k = p.point_dict.keys()
                 for kk in k:
                     if (
                         kk in macfunc
                         and "subtype" in macfunc[kk]
                         and macfunc[kk]["subtype"] == "target"
                     ):
                         plist.append(p.point_dict[kk])
             except Exception as e:
                 print(e)
         return plist
 
-    def _touch_untouch(self, point_list, touch):
+    def _touch_untouch(self, point_list: list, touch: bool) -> None:
         """Touch or untouch the points in point_list. When touch=False,
         remove self from the owners list, and mark the point as untouched
         only if there are no other owners.
 
         """
         ptindex = self.yg_glyph_view.yg_point_view_index
         for p in point_list:
             if type(p) is ygSet:
                 self._touch_untouch(p.point_list(), touch)
             elif type(p) is ygParams:
-                self._touch_untouch(self._get_macfunc_targets(p))
+                self._touch_untouch(self._get_macfunc_targets(p), touch)
             else:
                 if touch:
                     try:
                         ptindex[p.id].touched = True
                         ptindex[p.id].owners.append(self)
                     except Exception:
                         pass
@@ -386,89 +410,90 @@
                     try:
                         ptindex[p.id].owners.remove(self)
                         if len(ptindex[p.id].owners) == 0:
                             ptindex[p.id].touched = False
                     except Exception:
                         pass
 
-    def _touch_all_points(self):
+    def _touch_all_points(self) -> None:
         """Mark each point affected by this hint as 'touched,' and record
         this hint as an owner in its 'owners" list. To orient new hints
         correctly, we need to be accurate about which points are touched.
 
         """
         self._touch_untouch(self._target_list(), True)
 
-    def _remove_touches(self):
+    def _remove_touches(self) -> None:
         """Remove reference to this hint from the "owners" list for each
         point, and if the owner's list is empty afterwards, mark the
         point as untouched.
 
         """
         self._touch_untouch(self._target_list(), False)
 
-    def _process_click_on_hint(self, obj, with_shift, is_left):
+    def _process_click_on_hint(self, obj, with_shift: bool, is_left: bool) -> None:
         if is_left:
             if with_shift:
                 self.yg_glyph_view.yg_selection._toggle_object(self)
             else:
                 self.yg_glyph_view.yg_selection._add_object(self, False)
 
-    def _prepare_graphics(self):
+    def _prepare_graphics(self) -> None:
         # In ygHintView
         if len(self.graphical_hint) >= 1:
             for c in self.graphical_hint:
                 if isinstance(c, ygGraphicalHintComponent):
                     c._prepare_graphics(
                         is_selected=self._is_selected,
                         hint_type=self.yg_hint.hint_type(),
                     )
 
-    def _is_yg_selected(self):
+    def _is_yg_selected(self) -> bool:
         return self._is_selected
 
-    def update(self):
+    def update(self, rect: QRectF = None) -> None:  # type: ignore
         if len(self.graphical_hint) >= 1:
             for c in self.graphical_hint:
                 c.update()
-        super().update()
+        super().update(rect=self.boundingRect())
 
-    def yg_select(self):
+    def yg_select(self) -> None:
         self._is_selected = True
         self._prepare_graphics()
         self.update()
 
-    def yg_unselect(self):
+    def yg_unselect(self) -> None:
         self._is_selected = False
         self._prepare_graphics()
         self.update()
 
 
 class ygGraphicalHintComponent:
-    def _prepare_graphics(self, **kwargs):
-        pass
+    def _prepare_graphics(self, **kwargs) -> None:
+        ...
 
 
 class ygArrowHead(QGraphicsPolygonItem, ygGraphicalHintComponent):
     """Arrowhead to mount on the end of a line
 
     A reference should be kept only in ygHintView.
 
     This is separate from the line (ygHintStem) it goes with, chiefly so that
     it can be clickable.
     """
 
-    def __init__(self, tip, direction, hint_type, id, parent=None):
+    def __init__(self, tip, direction: str, hint_type: str, id, parent=None) -> None:
         super().__init__()
         self.setCursor(Qt.CursorShape.CrossCursor)
         self.direction = direction
         self.hint_type = hint_type
         self.parent = parent
         self.id = id
         tp = QPointF(0, 0)
+        self.tip = tip
         qpolygon = QPolygonF([tp, tp, tp, tp])
         if direction == "down":
             self.tip = QPointF(8, 8)
             pt1 = QPointF(self.tip.x() - 6, self.tip.y() - 8)
             pt2 = QPointF(self.tip.x() + 6, self.tip.y() - 8)
             qpolygon = QPolygonF([self.tip, pt1, pt2, self.tip])  # 8,8
         elif direction == "up":
@@ -556,17 +581,39 @@
 
 
 class ygHintStem(QGraphicsPathItem, ygGraphicalHintComponent):
     """Line for connecting related points
 
     The connecting line with arrow represents a hint. There are different kinds,
     which will be represented by different colors.
+
+    params:
+
+    p1 (ygPointable): point for one end of the stem.
+
+    p2 (ygPointable): point for the other end of the stem.
+
+    axis: Not sure if this is ever used.
+
+    hint_type (str): The type of this hint.
+
+    id: A unique id for this object.
+
+    parent: The parent of this item.
     """
 
-    def __init__(self, p1, p2, axis, hint_type, id=None, parent=None):
+    def __init__(
+        self,
+        p1: "ygPointable",
+        p2: "ygPointable",
+        axis: str,
+        hint_type: str,
+        id: Any = None,
+        parent=None,
+    ) -> None:
         # "axis" param not used. Get rid of it.
         super().__init__()
         #
         # This class looks very messy. Clean it up!
         #
         # p1 and p2 must be ygPointable objects (ygPointView, ygPointCollectionView).
         #
@@ -597,35 +644,35 @@
         self.arrowhead = None
         try:
             box_ratio = xdistance / ydistance
         except ZeroDivisionError:
             box_ratio = 0
         # Generate a keyword to describe the shape of the box.
         if xdistance == 0 and ydistance == 0:
-            self.shape = "invisible"
+            self._shape = "invisible"
             self.arrow_axis = None
         # elif box_ratio < 0.05:
         elif xdistance < 10:
-            self.shape = "y only"
+            self._shape = "y only"
             self.arrow_axis = "y"
         # elif box_ratio >= 1.0 and box_ratio <= 1.5:
         elif ydistance < 10:
-            self.shape = "x only"
+            self._shape = "x only"
             self.arrow_axis = "x"
         elif box_ratio < 0.3333:
-            self.shape = "tall"
+            self._shape = "tall"
             self.arrow_axis = "y"
         elif box_ratio > 3:
-            self.shape = "flat"
+            self._shape = "flat"
             self.arrow_axis = "x"
         elif ydistance > xdistance:
-            self.shape = "tallish"
+            self._shape = "tallish"
             self.arrow_axis = "y"
         else:
-            self.shape = "flattish"
+            self._shape = "flattish"
             self.arrow_axis = "x"
         self.arrowhead_direction = None
         # Should these direction words be "positive" and "negative"?
         if self.arrow_axis == "x":
             if begin_x < end_x:
                 self.arrowhead_direction = "right"
             if begin_x > end_x:
@@ -661,23 +708,23 @@
                 bottomPoint = self.lineEnd
             else:
                 self.lineEnd = self._adjustPoint(self.topadjust, end_x, end_y)
                 self.lineBegin = self._adjustPoint(self.bottomadjust, begin_x, begin_y)
                 bottomPoint = self.lineBegin
                 topPoint = self.lineEnd
         # The "0.25" that governs the length of the handles for the cubic drawing
-        # needs to be abstracted, so it can change with the shape of the box.
+        # needs to be abstracted, so it can change with the _shape of the box.
         partial_y_distance = ydistance * 0.25
         partial_x_distance = xdistance * 0.25
-        if self.shape == "invisible":
+        if self._shape == "invisible":
             path = QPainterPath()
-        elif self.shape in ["tall", "tallish", "y only"]:
+        elif self._shape in ["tall", "tallish", "y only"]:
             top_point_x = topPoint.x()
             bottom_point_x = bottomPoint.x()
-            if self.shape == "y only":
+            if self._shape == "y only":
                 flat_adjust = round(ydistance * 0.05)
                 if flat_adjust > 15:
                     flat_adjust = 15
                 top_point_x -= flat_adjust
                 bottom_point_x -= flat_adjust
             handle1 = QPointF(top_point_x, topPoint.y() + partial_y_distance)
             handle2 = QPointF(bottom_point_x, bottomPoint.y() - partial_y_distance)
@@ -686,18 +733,18 @@
                 path = QPainterPath(bottomPoint)
                 path.quadTo(handle2, self._center_point)
                 path.quadTo(handle1, topPoint)
             else:
                 path = QPainterPath(topPoint)
                 path.quadTo(handle1, self._center_point)
                 path.quadTo(handle2, bottomPoint)
-        elif self.shape in ["flat", "flattish", "x only"]:
+        elif self._shape in ["flat", "flattish", "x only"]:
             left_point_y = leftPoint.y()
             right_point_y = rightPoint.y()
-            if self.shape == "x only":
+            if self._shape == "x only":
                 flat_adjust = round(xdistance * 0.05)
                 if flat_adjust > 15:
                     flat_adjust = 15
                 left_point_y += flat_adjust
                 right_point_y += flat_adjust
             handle1 = QPointF(leftPoint.x() + partial_x_distance, left_point_y)
             handle2 = QPointF(rightPoint.x() - partial_x_distance, right_point_y)
@@ -712,15 +759,15 @@
                 path.quadTo(handle2, rightPoint)
         else:
             # This has never happened.
             print("What's going on?")
         self.setPath(path)
         self._prepare_graphics(is_selected=False, hint_type=self.hint_type)
 
-    def _prepare_graphics(self, **kwargs):
+    def _prepare_graphics(self, **kwargs) -> None:
         # For ygHintStem
         is_selected = kwargs["is_selected"]
         hint_type = kwargs["hint_type"]
         pen = QPen()
         pen.setWidth(HINT_ARROW_WIDTH)
         if is_selected:
             pen.setColor(SELECTED_HINT_COLOR[hint_type])
@@ -728,57 +775,57 @@
             pen.setColor(HINT_COLOR[hint_type])
         if hint_type == "whitedist":
             pen.setDashPattern([2, 2])
         if hint_type == "graydist":
             pen.setDashPattern([4, 2])
         self.setPen(pen)
 
-    def find_mid_point(self, pt1, pt2):
+    def find_mid_point(self, pt1: QPointF, pt2: QPointF) -> QPointF:
         """For placing the point in the middle of a quadratic curve: get the
         mid-point on a line between two points.
         """
         l = QLineF(pt1, pt2)
         return l.center()
 
     def center_point(self):
         return self._center_point
 
-    def _adjustPoint(self, adjustment, x, y):
+    def _adjustPoint(self, adjustment: list, x: int, y: int) -> QPointF:
         return QPointF(x + adjustment[0], y + adjustment[1])
 
-    def endPoint(self):
+    def endPoint(self) -> QPointF:
         return self.lineEnd
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         # In ygHintStem
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
-        self.parentItem()._process_click_on_hint(self, with_shift, is_left)
+        self.parentItem()._process_click_on_hint(self, with_shift, is_left)  # type: ignore
 
 
 class ygHintButton(QGraphicsEllipseItem, ygGraphicalHintComponent):
     """A button to display mid-stem, to make an easy target for a mouse."""
 
-    def __init__(self, viewer, location, hint):
+    def __init__(self, viewer: "ygGlyphScene", location: QPoint, hint: ygHint) -> None:
         """viewer: a ygGlyphScene object
         location: QPoint
         hint: ygModel.ygHint
         """
         self.viewer = viewer
         self.diameter = HINT_BUTTON_DIA + 2
         loc_offset = self.diameter - (self.diameter / 2)
         self.location = QPointF(location.x() - loc_offset, location.y() - loc_offset)
         self.yg_hint = hint
         super().__init__(QRectF(self.location, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self._prepare_graphics(is_selected=False, hint_type=self.yg_hint.hint_type())
 
-    def _prepare_graphics(self, **kwargs):
+    def _prepare_graphics(self, **kwargs) -> None:
         # for ygHintButton
         is_selected = kwargs["is_selected"]
         hint_type = kwargs["hint_type"]
         pen = QPen()
         brush = QBrush()
         pen.setWidth(HINT_ANCHOR_WIDTH)
         if is_selected:
@@ -786,54 +833,62 @@
         else:
             color = HINT_COLOR[hint_type]
         brush.setColor(color)
         pen.setColor(color)
         self.setPen(pen)
         self.setBrush(brush)
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         # In ygHintButton
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
-        self.parentItem()._process_click_on_hint(self, with_shift, is_left)
+        self.parentItem()._process_click_on_hint(self, with_shift, is_left)  # type: ignore
 
 
 class ygPointMarker(QGraphicsEllipseItem, ygGraphicalHintComponent):
     """pt has got to be a ygPointView."""
 
-    def __init__(self, viewer, pt, hint_type, name=None, id=None, parent=None):
+    def __init__(
+        self,
+        viewer: "ygGlyphScene",
+        pt: "ygPointView",
+        hint_type: str,
+        name: str = None,
+        id=None,
+        parent=None,
+    ):
         self.pt = pt
         self.name = name
-        self.label = None
+        self.label: Optional[QLabel] = None
         # This is "placed" when user has associated it with a point.
-        self.x = self.pt.glocation.x() - 1
-        self.y = self.pt.glocation.y() - 1
-        self.glocation = QPointF(self.x, self.y)
+        self._x = self.pt.glocation.x() - 1
+        self._y = self.pt.glocation.y() - 1
+        self.glocation = QPointF(self._x, self._y)
         if self.pt.yg_point.on_curve:
             self.diameter = POINT_ONCURVE_DIA + 2
         else:
             self.diameter = POINT_OFFCURVE_DIA + 2
         super().__init__(QRectF(self.glocation, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self._prepare_graphics(is_selected=False, hint_type=hint_type)
         self.label_proxy = None
         if self.name != None:
             self._prepare_label()
             self.label_proxy = viewer.addWidget(self.label)
         self.viewer = viewer
 
-    def _prepare_label(self):
+    def _prepare_label(self) -> None:
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: gray;}")
         self.label.setText(str(self.name))
-        self.label.move(round(self.x + self.diameter), round(self.y + self.diameter))
+        self.label.move(round(self._x + self.diameter), round(self._y + self.diameter))
 
-    def _get_model_point(self):
+    def _get_model_point(self) -> ygPoint:
         return self.pt.yg_point
 
     def _get_view_point(self):
         return self.pt
 
     def _remove_labels(self):
         if self.label_proxy:
@@ -864,15 +919,15 @@
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
         self.parentItem()._process_click_on_hint(self, with_shift, is_left)
 
 
 class ygPointable:
-    """For getting the point that a hint line should attach to. For points,
+    """Mixin for getting the point that a hint line should attach to. For points,
     this is very simple. For sets, not so much.
 
     """
 
     def attachment_point(self, pt):
         pass
 
@@ -891,15 +946,15 @@
     or macro
 
     hint_type (str): The type of this hint (it must be "function" or
     "macro")
 
     """
 
-    def __init__(self, viewer, *args):
+    def __init__(self, viewer: "ygGlyphScene", *args) -> None:
         super().__init__()
         self.yg_viewer = viewer
         self.point_dict = {}
         if type(args[0]) is ygParams:
             self.yg_params = args[0]
             kk = self.yg_params.point_dict.keys()
             for k in kk:
@@ -958,57 +1013,57 @@
             marker_list.append(h)
         return marker_list
 
     def paint(self, painter, option, widget):
         """Got to be here, but it doesn't have to do anything."""
         pass
 
-    def boundingRect(self):
+    def boundingRect(self) -> QRectF:
         return self.rect
 
-    def height(self):
+    def height(self) -> int:
         return self.rect.height()
 
-    def width(self):
+    def width(self) -> int:
         return self.rect.width()
 
-    def _boundingLines(self):
+    def _boundingLines(self) -> tuple:
         # Four visible lines for border, plus the bounding rect
         markers = self.point_markers
         min_x = max_x = min_y = max_y = None
         for m in markers:
             if not min_x:
-                min_x = m.x
+                min_x = m._x
             else:
-                min_x = min(min_x, m.x)
+                min_x = min(min_x, m._x)
             if not min_y:
-                min_y = m.y
+                min_y = m._y
             else:
-                min_y = min(min_y, m.y)
+                min_y = min(min_y, m._y)
             if not max_x:
-                max_x = m.x
+                max_x = m._x
             else:
-                max_x = max(max_x, m.x)
+                max_x = max(max_x, m._x)
             if not max_y:
-                max_y = m.y
+                max_y = m._y
             else:
-                max_y = max(max_y, m.y)
+                max_y = max(max_y, m._y)
         min_x -= 5
         min_y -= 5
         max_x += 15
         max_y += 15
         lines = []
         lines.append(QLineF(min_x, min_y, max_x, min_y))
         lines.append(QLineF(max_x, min_y, max_x, max_y))
         lines.append(QLineF(max_x, max_y, min_x, max_y))
         lines.append(QLineF(min_x, min_y, min_x, max_y))
         rect = QRectF(min_x, min_y, max_x - min_x, max_y - min_y)
         return lines, rect
 
-    def attachment_point(self, pt):
+    def attachment_point(self, pt: "ygPointView") -> QPointF:
         if pt.x() < self.rect.x() - 1:
             x = self.rect.x() - 1
             if pt.y() < self.rect.y() - 1:
                 return QPointF(x, self.rect.y() - 4)
             elif pt.y() > self.rect.y() + self.rect.height():
                 return QPointF(x, self.rect.y() + self.rect.height() - 3)
             else:
@@ -1024,121 +1079,125 @@
         else:
             x = self.rect.x() + self.rect.width() / 2
             if pt.y() < self.rect.y() + (self.rect.height() / 2):
                 return QPointF(x, self.rect.y() - 4)
             else:
                 return QPointF(x, self.rect.y() + self.height() - 3)
 
-    def center_point(self):
+    def center_point(self) -> QPointF:
         return QPointF(self.x() + (self.width() / 2), self.y() + (self.height() / 2))
 
-    def contains(self, pt):
+    def contains(self, pt: QPointF) -> bool:
         for p in self.point_markers:
             if p.contains(pt):
                 return True
         for b in self.borders:
             if b.contains(pt):
                 return True
         return False
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         # In ygPointCollectionView
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         is_left = event.button() == Qt.MouseButton.LeftButton
-        self.parentItem()._process_click_on_hint(self, with_shift, is_left)
+        self.parentItem()._process_click_on_hint(self, with_shift, is_left)  # type: ignore
 
 
 class ygSetView(ygPointCollectionView):
     """A graphical representation of a list of points."""
 
-    def __init__(self, viewer, yg_set, hint_type):
+    def __init__(self, viewer: "ygGlyphScene", yg_set: ygSet, hint_type: str) -> None:
         super().__init__(viewer, yg_set.point_list(), hint_type)
         self.viewer = viewer
         self.hint_type = hint_type
 
 
 class ygSelection(QObject):
     """A list of selected objects (points, hints, or both).
 
     The class has functions for manipulating the list.
     """
 
     sig_selection_changed = pyqtSignal(object)
 
-    def __init__(self, viewer):
+    def __init__(self, viewer: "ygGlyphScene") -> None:
         super().__init__()
-        self.selected_objects = []
+        self.selected_objects: list = []
         self.viewer = viewer
 
-    def setup_selection_signal(self, f):
+    def setup_selection_signal(self, f: Optional[Callable]) -> None:
         self.sig_selection_changed.connect(f)
 
-    def get_scene(self):
+    def get_scene(self) -> "ygGlyphScene":
         return self.viewer
 
-    def send_signal(self):
+    def send_signal(self) -> None:
         self.sig_selection_changed.emit(self.viewer.selection_profile())
 
-    def _cancel_selection(self, emit_signal: bool = True):
+    def _cancel_selection(self, emit_signal: bool = True) -> None:
         for p in self.selected_objects:
             if p._is_yg_selected:
                 p.yg_unselect()
                 p._prepare_graphics()
                 p.update()
         self.selected_objects = []
         self.viewer.update()
         if emit_signal:
             self.sig_selection_changed.emit(self.viewer.selection_profile())
 
-    def _add_object(self, obj, add_to_selection):
+    def _add_object(self, obj: ygSelectable, add_to_selection: bool) -> None:
         if not add_to_selection:
             self._cancel_selection(emit_signal=False)
-        if obj.isVisible():
+        # Not sure what to do about next line. Study Protocol further?
+        # isVisible is inherited from QGraphicsItem, and here we look
+        # both at that and at things inherited from ygSelectable.
+        if obj.isVisible():  # type: ignore
             obj.yg_select()
             self.selected_objects.append(obj)
             obj._prepare_graphics()
             obj.update()
         self.sig_selection_changed.emit(self.viewer.selection_profile())
 
     # This is never called.
     # def _cancel_object(self, obj):
     #     obj.yg_unselect()
     #     self.selected_objects.remove(obj)
     #     obj._prepare_graphics()
     #     obj.update()
     #     self.sig_selection_changed.emit(self.viewer.selection_profile())
 
-    def _toggle_object(self, obj):
-        if not obj.isVisible():
+    def _toggle_object(self, obj: ygSelectable) -> None:
+        # Problem as in _add_object above.
+        if not obj.isVisible():  # type: ignore
             return
         if obj._is_yg_selected():
             obj.yg_unselect()
             self.selected_objects.remove(obj)
         else:
             obj.yg_select()
             self.selected_objects.append(obj)
         obj._prepare_graphics()
         obj.update()
         self.sig_selection_changed.emit(self.viewer.selection_profile())
 
-    def _add_rect(self, rect, add_to_selection):
+    def _add_rect(self, rect: QRectF, add_to_selection: bool) -> None:
         """This method of selecting doesn't work on hints."""
         if not add_to_selection:
             self._cancel_selection()
         for ptv in self.viewer.yg_point_view_list:
             if ptv.isVisible() and rect.contains(ptv.glocation):
                 ptv.yg_select()
                 self.selected_objects.append(ptv)
                 ptv._prepare_graphics()
                 ptv.update()
         self.sig_selection_changed.emit(self.viewer.selection_profile())
 
-    def _toggle_rect(self, rect):
+    def _toggle_rect(self, rect: QRectF) -> None:
         """This method of selecting doesn't work on hints."""
         for ptv in self.viewer.yg_point_view_list:
             if ptv.isVisible() and rect.contains(ptv.glocation):
                 if ptv._is_yg_selected():
                     ptv.yg_unselect()
                 else:
                     ptv.yg_select()
@@ -1150,44 +1209,44 @@
                 ptv.update()
         self.sig_selection_changed.emit(self.viewer.selection_profile())
 
 
 class ygPointView(QGraphicsEllipseItem, ygSelectable, ygPointable):
     """A visible point"""
 
-    def __init__(self, viewer, yg_point):
+    def __init__(self, viewer: "ygGlyphScene", yg_point: ygPoint):
         self._is_selected = False
         self.yg_point = yg_point
         if yg_point.on_curve:
             self.diameter = POINT_ONCURVE_DIA
         else:
             self.diameter = POINT_OFFCURVE_DIA
         # glocation is a QPointF. Initialize at 0,0: must be set later.
         self.glocation = QPointF(0, 0)
         super().__init__(QRectF(self.glocation, QSizeF(self.diameter, self.diameter)))
         self.setCursor(Qt.CursorShape.CrossCursor)
         self.border_width = 1
         self.index = -1
         self.viewer = viewer
-        self.point_number_label = None
-        self.point_number_label_proxy = None
+        self.point_number_label: Optional[QLabel] = None
+        self.point_number_label_proxy: Optional[QGraphicsProxyWidget] = None
         self.touched = False
         # These are the ygHintView objects that touch this point. When a hint
         # is removed from ygGlyphScene, remove the reference from this list.
         # If a hint being removed makes this list empty, remove the "touched"
         # flag from this ygPointView.
-        self.owners = []
+        self.owners: List[ygHintView] = []
 
-    def attachment_point(self, pt):
+    def attachment_point(self, pt: Any) -> QPointF:
         return self.glocation
 
-    def center_point(self):
+    def center_point(self) -> QPointF:
         return self.glocation
 
-    def _prepare_graphics(self):
+    def _prepare_graphics(self) -> None:
         # For ygPointView
         if self._is_yg_selected():
             if self.yg_point.on_curve:
                 brushColor = POINT_ONCURVE_SELECTED
             else:
                 brushColor = POINT_OFFCURVE_SELECTED
         else:
@@ -1198,61 +1257,65 @@
             penColor = POINT_OFFCURVE_OUTLINE
         pen = QPen(penColor)
         pen.setWidth(self.border_width)
         brush = QBrush(brushColor)
         self.setBrush(brush)
         self.setPen(pen)
 
-    def get_scene(self):
+    def get_scene(self) -> "ygGlyphScene":
         return self.viewer
 
-    def has_label(self):
+    def has_label(self) -> bool:
         return self.point_number_label != None
 
-    def add_label(self):
+    def add_label(self) -> None:
+        """Adds a label for this point. The label is supplied by the model
+        point, which will supply an index, a pair of coordinates, or a
+        name, depending on current settings.
+        """
         if self.point_number_label:
             self.del_label()
         self.point_number_label = QLabel()
         self.point_number_label.setStyleSheet(
             "QLabel {background-color: transparent; color: red; font-size: 90%}"
         )
         self.point_number_label.setText(
             str(self.yg_point.preferred_label(normalized=True))
         )
         self.point_number_label_proxy = self.viewer.addWidget(self.point_number_label)
         label_x = self.glocation.x() + self.diameter
         label_y = self.glocation.y() - self.point_number_label.height()
         self.point_number_label.move(round(label_x), round(label_y))
 
-    def del_label(self):
+    def del_label(self) -> None:
         if self.point_number_label:
             self.viewer.removeItem(self.point_number_label_proxy)
             self.point_number_label = None
             self.point_number_label_proxy = None
 
     def update(self):
         pass
 
-    def _is_yg_selected(self):
+    def _is_yg_selected(self) -> bool:
         return self._is_selected
 
-    def yg_select(self):
+    def yg_select(self) -> None:
         self._is_selected = True
         self._prepare_graphics()
         self.update()
 
-    def yg_unselect(self):
+    def yg_unselect(self) -> None:
         self._is_selected = False
         self._prepare_graphics()
         self.update()
 
-    def contains(self, p):
+    def contains(self, p: QPointF) -> bool:
         return self.mapToScene(self.boundingRect()).boundingRect().contains(p)
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         # In ygPointView
         # Select when clicked, eiher adding to or replacing current selection.
         modifier = QApplication.keyboardModifiers()
         if (
             modifier & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier:
             if event.button() == Qt.MouseButton.LeftButton:
@@ -1261,15 +1324,15 @@
             if event.button() == Qt.MouseButton.LeftButton:
                 self.viewer.yg_selection._add_object(self, False)
 
 
 class SelectionRect(QGraphicsRectItem):
     """The rubber band that appears while dragging to select points."""
 
-    def __init__(self, qr):
+    def __init__(self, qr: QRectF) -> None:
         super(SelectionRect, self).__init__(qr)
         self.setRect(qr)
 
 
 class ygGlyphScene(QGraphicsScene):
     """The workspace.
 
@@ -1285,70 +1348,70 @@
     sig_make_macfunc = pyqtSignal(object)
     sig_assign_macfunc_point = pyqtSignal(object)
     sig_edit_macfunc_params = pyqtSignal(object)
     sig_change_cv = pyqtSignal(object)
     sig_round_hint = pyqtSignal(object)
     sig_min_dist = pyqtSignal(object)
     sig_swap_macfunc_points = pyqtSignal(object)
-    # sig_macfunc_target = pyqtSignal(object)
-    # sig_macfunc_ref = pyqtSignal(object)
     sig_toggle_point_numbers = pyqtSignal()
     sig_set_category = pyqtSignal(object)
     sig_name_points = pyqtSignal(object)
 
-    def __init__(self, preferences, yg_glyph):
+    def __init__(self, preferences: ygPreferences, yg_glyph: ygGlyph) -> None:
         """yg_glyph is a ygGlyph object from ygModel."""
         self.preferences = preferences
 
-        self.yg_point_view_index = {}
-        self.yg_point_view_list = []
-        self.yg_hint_view_index = {}
-        self.yg_hint_view_list = []
+        self.yg_point_view_index: dict = {}
+        self.yg_point_view_list: list = []
+        # No use for this one (right now)
+        # self.yg_hint_view_index: dict = {}
+        self.yg_hint_view_list: list = []
         super(ygGlyphScene, self).__init__()
         self.cv_error_msg = "Error while looking for a control value."
 
         # Current display preferences
 
         self.off_curve_points_showing = self.preferences.show_off_curve_points()
         self.point_numbers_showing = self.preferences.top_window().show_point_numbers
         self.zoom_factor = self.preferences.zoom_factor()
 
         # Set up glyph info
 
         self.yg_glyph = yg_glyph
 
         # Try to get rid of ref to this scene in the model's ygGlyph class.
-        self.yg_glyph.glyph_viewer = self
+        # For now, we've got to ignore the type so as to avoid circular imports.
+        self.yg_glyph.glyph_viewer = self  # type: ignore
 
         # Make graphical points
 
         for p in self.yg_glyph.points():
             yg_point_view = ygPointView(self, p)
             self.yg_point_view_index[p.id] = yg_point_view
             self.yg_point_view_list.append(yg_point_view)
 
         # Set up dimensions; scale the glyph.
 
         self.adv = 0
         self.lsb = 0
         self.xTranslate = 0
         self.yTranslate = 0
-        self.original_coordinates = None
+        # Not gonna mess with types from fontTools.
+        self.original_coordinates: Any = None
         self.scale_glyph()
         self.center_x = self.xTranslate + round(self.adv / 2)
         self.center_x = self.xTranslate + round(self.adv / 2)
 
         # Setup for selecting
 
-        self.selectionRect = (
-            None  # The rubber band. None when no selection is underway.
-        )
-        self.dragBeginPoint = QPointF(
-            0, 0
-        )  # Set whenever left mouse button is pressed, in case of rubber band selection
+        # selectionRect is the rubber band. None when no selection is underway.
+        self.selectionRect: Optional[SelectionRect] = None
+        # Set dragBeginPoint whenever left mouse button is pressed, in case of
+        # rubber band selection.
+        self.dragBeginPoint = QPointF(0, 0)
         self.yg_selection = ygSelection(self)
         self.yg_selection.setup_selection_signal(
             self.preferences.top_window().selection_changed
         )
 
         # Add the points and manage their visibility.
 
@@ -1382,49 +1445,49 @@
 
         self.install_hints(self.yg_glyph.hints())
 
     #
     # Sizing and zooming
     #
 
-    def size_report(self):
+    def size_report(self) -> None:
         """For diagnostics."""
         print("Zoom factor: " + str(self.zoom_factor))
         print("xTranslate: " + str(self.xTranslate))
         print("yTranslate: " + str(self.yTranslate))
         ft_font = self.yg_glyph.yg_font.ft_font
         oc = ft_font["glyf"]._getCoordinatesAndControls(
             self.yg_glyph.gname, ft_font["hmtx"].metrics
         )[0]
         print("First point: " + str(oc[0]))
         print("Canvas rect: " + str(self.sceneRect()))
         print("")
 
-    def set_zoom_factor(self, new_zoom):
+    def set_zoom_factor(self, new_zoom: float) -> None:
         self.zoom_factor = new_zoom
         self.preferences.top_window().zoom_factor = self.zoom_factor
         self.scale_glyph()
         self.center_x = self.xTranslate + round(self.adv / 2)
         self.center_x = self.xTranslate + round(self.adv / 2)
         self.update()
         self.install_hints(self.yg_glyph.hints())
         # This will have the effect of moving point labels to the new positions
         # of the points. Affect only those already visible.
         for p in self.yg_point_view_list:
             if p.has_label():
                 p.add_label()
 
-    def reset_scale(self):
+    def reset_scale(self) -> None:
         c = self.original_coordinates
         ft_font = self.yg_glyph.yg_font.ft_font
         ft_font["glyf"]._setCoordinates(
             self.yg_glyph.glyph_name(), c, ft_font["hmtx"].metrics
         )
 
-    def scale_glyph(self):
+    def scale_glyph(self) -> None:
         # Start out clean, with coordinates as in original font. That way,
         # zoom_factor always operates on the original, as opposed to the last
         # value.
         ft_font = self.yg_glyph.yg_font.ft_font
         ft_glyph = self.yg_glyph.ft_glyph
         if self.original_coordinates:
             ft_font["glyf"]._setCoordinates(
@@ -1459,15 +1522,15 @@
                 pass
 
         glyph_set = {self.yg_glyph.glyph_name(): self.yg_glyph.ft_glyph}
         self.path = QPainterPath()
         self.qt_pen = QtPen(glyph_set, path=self.path)
         self.yg_glyph.ft_glyph.draw(self.qt_pen, self.yg_glyph.yg_font.ft_font["glyf"])
 
-    def _calc_canvas_size(self):
+    def _calc_canvas_size(self) -> Tuple[int, int, int, int]:
         """This calculates a canvas that will do for the entire font. The result
         can be awkward (see the absurd situation in Junicode, which has an
         extremely wide canvas because of one glyph, threeemdash (U+2E3B)).
         """
         f = self.yg_glyph.yg_font.ft_font
         x_size = abs(f["head"].xMin) + abs(f["head"].xMax) + (GLYPH_WIDGET_MARGIN * 2)
         y_size = abs(f["head"].yMin) + abs(f["head"].yMax) + (GLYPH_WIDGET_MARGIN * 2)
@@ -1476,15 +1539,15 @@
         return (
             round(x_size * self.zoom_factor),
             round(y_size * self.zoom_factor),
             round(zero_x * self.zoom_factor),
             round(zero_y * self.zoom_factor),
         )
 
-    def _font2Qt(self, x, y, onCurve=False):
+    def _font2Qt(self, x: int, y: int, onCurve: bool = False) -> QPointF:
         """Converts font coordinate system to Qt, for positioning points
 
         The font coordinate system has zero at the baseline and
         higher y values towards the top. The Qt system has 0,0
         at the top left of the canvas and higher y values towards
         the bottom.
         """
@@ -1499,15 +1562,15 @@
         # print("y: " + str(thisy - adjust))
         return QPointF(thisx - adjust, thisy - adjust)
 
     #
     # Overrides
     #
 
-    def drawBackground(self, painter, rect):
+    def drawBackground(self, painter: QPainter, rect) -> None:
         """The glyph outline is drawn as the background layer for this scene.
         Points and hints are drawn in the item layer, and the foreground
         layer is not used at this time.
         """
         painter.scale(1.0, -1.0)
         painter.translate(QPointF(self.xTranslate, self.yTranslate * -1))
 
@@ -1527,16 +1590,20 @@
         painter.setPen(pen)
         painter.drawPath(self.path)
 
     #
     # Editing slots
     #
 
-    def guess_cv(self):
-        """Called from a slot in ygGlyphView"""
+    @pyqtSlot()
+    def guess_cv(self) -> None:
+        """Called from a slot in ygGlyphView, this function
+        guesses the right CV for selected point(s) or
+        hint.
+        """
         _selected_objects = self.selected_objects(False)
         selected_hint = None
         for s in _selected_objects:
             if type(s) is ygHintView or type(s) is ygHint:
                 selected_hint = self._model_hint(s)
                 break
         if selected_hint != None:
@@ -1555,15 +1622,15 @@
                 cv_name = self.yg_glyph.yg_font.cvt.get_closest_cv_name(
                     cv_list, selected_hint
                 )
                 selected_hint.set_cv(cv_name)
             except Exception:
                 pass
 
-    def guess_cv_for_hint(self, hint):
+    def guess_cv_for_hint(self, hint: ygHint) -> None:
         """Like guess_cv(), but this is called as part of the process of constructing
         a hint, and therefore should not trigger a signal.
         """
         if hint != None:
             htn = self.get_hint_type_num(hint.hint_type())
             cv_type = "pos"
             if htn == 3:
@@ -1580,23 +1647,23 @@
                 hint._set_cv(cv_name)
             except Exception as e:
                 print(e)
                 print(e.args)
                 pass
 
     @pyqtSlot(object)
-    def edit_macfunc_params(self, hint):
+    def edit_macfunc_params(self, hint: ygHintView) -> None:
         ed_dialog = macfuncDialog(hint)
         r = ed_dialog.exec()
         if r == QDialog.DialogCode.Accepted:
             hint.yg_hint.set_macfunc_other_args(ed_dialog.result_dict)
             # hint.yg_hint.hint_has_changed(hint.yg_hint)
 
     @pyqtSlot()
-    def toggle_off_curve_visibility(self):
+    def toggle_off_curve_visibility(self) -> None:
         self.off_curve_points_showing = not self.off_curve_points_showing
         self.preferences.top_window().show_off_curve_points = (
             self.off_curve_points_showing
         )
         for p in self.yg_point_view_list:
             if not p.yg_point.on_curve:
                 if self.off_curve_points_showing:
@@ -1604,15 +1671,15 @@
                     if self.point_numbers_showing:
                         p.add_label()
                 else:
                     p.hide()
                     if self.point_numbers_showing:
                         p.del_label()
 
-    def make_set(self):
+    def make_set(self) -> None:
         """In the hint model, the target can be either a ygPoint or a ygSet.
         This function takes the current selection, several ygPoint, and turns
         them into a ygSet, which it substitutes for the ygPoint. Note that
         exactly one selected point must be touched, and at least one
         selected point must be untouched.
 
         """
@@ -1636,29 +1703,29 @@
             new_list.append(self._model_point(p))
         # params: ygModel.ygHint, list of ygModel.ygPoint, touched ygModel.ygPoint, callback func.
         self.yg_glyph.make_set(
             hint_model, new_list, touched_point.yg_point, hint._update_touches
         )
         self.yg_glyph.hint_changed(hint_model)
 
-    def make_control_value(self):
+    def make_control_value(self) -> None:
         sel = self.selected_objects(True)
         if len(sel) == 0:
             return
         if len(sel) >= 1:
             p1 = self._model_point(sel[0])
         p2 = None
         if len(sel) >= 2:
             p2 = self._model_point(sel[1])
         cv_dialog = makeCVDialog(p1, p2, self.yg_glyph, self.preferences)
         r = cv_dialog.exec()
         if r == QDialog.DialogCode.Accepted:
             self.yg_glyph.yg_font.cvt.set_clean(False)
 
-    def name_points(self, pts):
+    def name_points(self, pts: List[ygPointView]) -> None:
         msg = "Name the point"
         if len(pts) > 1:
             msg += "s"
         msg += ":"
         text, ok = QInputDialog().getText(
             self.preferences.top_window(), "Name points", msg, QLineEdit.EchoMode.Normal
         )
@@ -1672,98 +1739,98 @@
                     lambda: "coord"
                     if self.preferences.top_window().points_as_coords
                     else "index"
                 )()
             )
 
     @pyqtSlot(object)
-    def change_hint_color(self, _params):
+    def change_hint_color(self, _params: dict) -> None:
         _params["hint"].yg_hint.change_hint_color(_params["color"])
 
     @pyqtSlot(object)
-    def toggle_hint_rounding(self, hint):
+    def toggle_hint_rounding(self, hint: ygHintView) -> None:
         self._model_hint(hint).toggle_rounding()
 
     @pyqtSlot(object)
-    def toggle_min_dist(self, hint):
+    def toggle_min_dist(self, hint: ygHintView) -> None:
         self._model_hint(hint).toggle_min_dist()
 
     @pyqtSlot()
-    def toggle_point_numbers(self):
+    def toggle_point_numbers(self) -> None:
         self.point_numbers_showing = not self.point_numbers_showing
         self.preferences.top_window().show_point_numbers = self.point_numbers_showing
         for p in self.yg_point_view_list:
             if self.point_numbers_showing:
                 if p.isVisible():
                     p.add_label()
             else:
                 p.del_label()
 
     @pyqtSlot(object)
-    def set_category(self, c):
+    def set_category(self, c: str) -> None:
         if c == "Default":
             try:
                 self.yg_glyph.props.del_property("category")
             except Exception:
                 pass
         else:
             self.yg_glyph.set_category(c)
 
-    def set_point_display(self, pv):
+    def set_point_display(self, pv: str) -> None:
         for p in self.yg_point_view_list:
             p.yg_point.label_pref = pv
             if self.point_numbers_showing:
                 if p.isVisible():
                     p.add_label()
 
     @pyqtSlot(object)
-    def swap_macfunc_points(self, data):
+    def swap_macfunc_points(self, data: dict) -> None:
         hint = data["hint"].yg_hint
         new_pt_name = data["new_pt"]
         old_pt_name = data["old_pt"]
         hint.swap_macfunc_points(new_pt_name, old_pt_name)
 
     @pyqtSlot(object)
-    def reverse_hint(self, h):
+    def reverse_hint(self, h: ygHint) -> None:
         """Recipient of a signal for reversing a hint. Communicates to the
         model that a hint must be added to the hint tree.
 
         Parameters:
         h (ygModel.ygHint): the hint to be reversed
 
         """
         h.reverse_hint(h)
 
     @pyqtSlot(dict)
-    def change_cv(self, param_dict):
+    def change_cv(self, param_dict: dict) -> None:
         """Recipient of a signal for adding or changing a control value.
 
         Parameters:
         param_dict (dict): A dictionary containing "hint" (the affected
         hint, ygHintView) and "cv" (the new cv)
 
         """
         if type(param_dict["hint"]) is ygHintView:
             param_dict["hint"].yg_hint.set_cv(param_dict["cv"])
 
     @pyqtSlot(object)
-    def add_hint(self, h):
+    def add_hint(self, h: ygHint) -> None:
         """Recipient of a signal for adding a hint. Communicates to the model
         that a hint must be added to the hint tree.
 
         Parameters:
         h (ygModel.ygHint): the hint to add to the tree
 
         """
         if type(h) is ygHint:
             h.add_hint(h)
         elif type(h) is ygHintView:
             h.add_hint(h.yg_hint)
 
-    def install_hints(self, hint_list):
+    def install_hints(self, hint_list: List[ygHint]) -> None:
         """Installs a collection of hints sent from the model.
 
         Parameters:
         hint_list: All the hints for either the y or the x axis
         for this glyph, in a list.
 
         """
@@ -1780,67 +1847,67 @@
         # ygHintView object.
         for h in hint_list:
             vh = self._make_visible_hint(h)
             self.yg_hint_view_list.append(vh)
         self.update()
         self.yg_selection.send_signal()
 
-    def delete_selected_hints(self):
+    def delete_selected_hints(self) -> None:
         oo = self.selected_objects(False)
         hh = []
         for o in oo:
             if type(o) is ygHintView:
                 hh.append(o.yg_hint)
         if len(hh) > 0:
             # Call a function in the model.
             hh[0].delete_hints(hh)
 
     #
     # Utilities
     #
 
-    def get_scene(self):
+    def get_scene(self) -> "ygGlyphScene":
         """Returns the current scene (always this object!)
 
         Returns:
         ygGlyphScene: this scene
         """
         return self
 
-    def _mouse_over_point(self, qp):
+    def _mouse_over_point(self, qp: QPoint) -> ygPointView:
         """In ygGlyphScene. Determines whether the mouse is positioned over a point.
 
         Parameters:
         qp (QPos): The current position of the mouse
 
         Returns:
-        bool: True if the mouse is over a point; False otherwise
+        ygPointView if the mouse is over a point; otherwise None
 
         """
         pt_keys = self.yg_point_view_index.keys()
         for pk in pt_keys:
             if self.yg_point_view_index[pk].contains(qp):
                 return self.yg_point_view_index[pk]
         return None
 
-    def _mouse_over_hint(self, qp):
+    def _mouse_over_hint(self, qp: QPointF) -> Optional[ygHintView]:
         """Determines whether the mouse is positioned over a hint.
 
         Parameters:
         qp (QPos): The current position of the mouse
 
         Returns:
-        bool: True if the mouse is over a hint; False otherwise
+        ygHintView if the mouse is over a hint; otherwise None
         """
         for h in self.yg_hint_view_list:
             if h.contains(qp):
                 return h
         return None
 
-    def _adjust_rect(self, current_point):
+    def _adjust_rect(self, current_point: ygPointView) -> QRectF:
         """Flips points around to account for rubber band rotating around
         the origin point.
 
         Parameters:
         current_point: The fixed point at which the selection began
 
         Returns:
@@ -1859,15 +1926,21 @@
             qr.setCoords(origin_x, current_y, current_x, origin_y)
         elif current_x < origin_x and current_y < origin_y:
             qr.setCoords(current_x, current_y, origin_x, origin_y)
         else:
             qr.setCoords(origin_x, origin_y, origin_x, origin_y)
         return qr
 
-    def selection_profile(self) -> tuple:
+    def selection_profile(self) -> Tuple[int, int, List[int], List[int]]:
+        """Surveys the current selection and returns a tuple containing:
+        - The number of touched points
+        - The number of untouched points
+        - The (integer) types of the owners of touched points
+        - The (integer) types of any selected hints
+        """
         s = self.selected_objects(True)
         touched_point_count = untouched_point_count = 0
         owner_types = []
         for ss in s:
             if ss.touched:
                 touched_point_count += 1
                 for h in ss.owners:
@@ -1882,15 +1955,15 @@
         return (
             touched_point_count,
             untouched_point_count,
             owner_types,
             selected_hint_types,
         )
 
-    def selected_objects(self, points_only):
+    def selected_objects(self, points_only: bool) -> list:
         """Get a list of objects (points and hints) selected by the user.
 
         Parameters:
         points_only (bool): if true, return only selected points (not hints)
 
         Returns:
         A list of all selected objects
@@ -1900,15 +1973,15 @@
             return self.yg_selection.selected_objects
         result = []
         for o in self.yg_selection.selected_objects:
             if type(o) is ygPointView:
                 result.append(o)
         return result
 
-    def get_hint_type_num(self, htype):
+    def get_hint_type_num(self, htype: str) -> int:
         """Translates the string description of the hint type (e.g. 'stem')
         into an int used by the program for deciding the shape of the
         visible hint.
 
         Parameters:
         htype (str): The string that describes the hint
 
@@ -1916,53 +1989,60 @@
         int: 0: no reference point; 1: one reference point; any number of
         targets; 2: two reference points; any number of targets; 3: one
         reference point; one target; 4:
 
         """
         return hint_type_nums[htype]
 
-    def resolve_point_identifier(self, pt, kwargs=None):
+    def resolve_point_identifier(
+        self, pt: Union[ygPointView, ygPoint], kwargs=None
+    ) -> ygPoint:
         """Gets a ygModel.ygPoint object.
 
         Parameters:
         pt: A ygModel.ygPoint or ygPointView object, or any kind of idenfifier
         accepted by Xgridfit.
 
         Returns: A ygModel.ygPoint object.
 
         """
         if type(pt) is ygPointView:
             return pt.yg_point
         return self.yg_glyph.resolve_point_identifier(pt)
 
-    def _model_hint(self, h):
+    def _model_hint(self, h: Union[ygHintView, ygHint]) -> ygHint:
         if type(h) is ygHintView:
             return h.yg_hint
-        return h
+        return h  # type: ignore
 
-    def _model_point(self, p):
+    def _model_point(self, p: Union[ygPointView, ygPoint]) -> ygPoint:
         if type(p) is ygPointView:
             return p.yg_point
-        return p
+        return p  # type: ignore
 
-    def current_axis(self):
+    def current_axis(self) -> str:
         return self.yg_glyph.current_axis()
 
-    def _distance(self, pt_a, pt_b):
+    def _distance(
+        self, pt_a: Union[ygPointView, ygPoint], pt_b: Union[ygPointView, ygPoint]
+    ) -> int:
+        """Returns the distance between two points (in font units) along
+        the current axis.
+        """
         pa = self._model_point(pt_a)
         pb = self._model_point(pt_b)
         if self.current_axis() == "y":
             return abs(pa.font_y - pb.font_y)
         return abs(pa.font_x - pb.font_x)
 
     #
     # Factories
     #
 
-    def _make_visible_hint(self, hint):
+    def _make_visible_hint(self, hint: ygHint) -> ygHintView:
         """Builds ygHintView objects from ygHint objects and adds them to
         this ygGlyphScene (a QGraphicsScene).
 
         Parameters:
         hint (ygHint): The hint from the model
 
         Returns:
@@ -1991,18 +2071,20 @@
             if type(target) is ygSet:
                 gtarget = ygSetView(self, target, hint_type)
             else:
                 gtarget = self.yg_point_view_index[target.id]
             # *** If this is going to crash, need to catch it and recover. Maybe
             # mark the hint as invalid and skip it when drawing or compiling?
             if hint.ref() == None:
-                print("Warning: ref is None (target is " + str(target.index) + ")")
+                print("Warning: ref is None (target is " + str(target) + ")")
             ref = self.resolve_point_identifier(hint.ref())
             gref = self.yg_point_view_index[ref.id]
-            ha = ygHintStem(gref, gtarget, 0, hint_type, parent=self)
+            ha = ygHintStem(
+                gref, gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+            )
             hb = ygHintButton(self, ha.center_point(), hint)
             ah = ygArrowHead(
                 ha.endPoint(), ha.arrowhead_direction, hint_type, ha.id, parent=self
             )
             ah.setPos(ha.endPoint())
             glist = [ha, hb, ah]
             if type(gtarget) is ygSetView:
@@ -2028,17 +2110,21 @@
                     "There must be two reference points for an interpolation hint"
                 )
             gref = []
             ref_one = self.resolve_point_identifier(ref_list.point_list()[0])
             ref_two = self.resolve_point_identifier(ref_list.point_list()[1])
             gref.append(self.yg_point_view_index[ref_one.id])
             gref.append(self.yg_point_view_index[ref_two.id])
-            ha1 = ygHintStem(gref[0], gtarget, 0, hint_type, parent=self)
+            ha1 = ygHintStem(
+                gref[0], gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+            )
             hb1 = ygHintButton(self, ha1.center_point(), hint)
-            ha2 = ygHintStem(gref[1], gtarget, 0, hint_type, parent=self)
+            ha2 = ygHintStem(
+                gref[1], gtarget, self.yg_glyph.current_axis(), hint_type, parent=self
+            )
             ah1 = ygArrowHead(
                 ha1.endPoint(), ha1.arrowhead_direction, hint_type, ha1.id, parent=self
             )
             hb2 = ygHintButton(self, ha2.center_point(), hint)
             ah2 = ygArrowHead(
                 ha2.endPoint(), ha2.arrowhead_direction, hint_type, ha2.id, parent=self
             )
@@ -2066,38 +2152,40 @@
                 self.addItem(yg_hint_view)
             else:
                 raise Exception(
                     "Something went wrong with gtarget in _make_visible_hint"
                 )
         else:
             raise Exception("Unknown hint type " + str(hint_type_num))
-        self.yg_hint_view_index[hint.id] = yg_hint_view
+        # self.yg_hint_view_index[hint.id] = yg_hint_view
         self.yg_hint_view_list.append(yg_hint_view)
         return yg_hint_view
 
     @pyqtSlot(dict)
-    def make_macfunc(self, _params):
+    def make_macfunc(self, _params: dict) -> None:
         hint_type = _params["hint_type"]
         name = _params["name"]
         self.make_macfunc_from_selection(hint_type, name=name)
         # Called function will send the signal to the model.
 
-    def get_round_default(self, hint):
+    def get_round_default(self, hint: ygHint) -> Optional[bool]:
         t = hint.hint_type()
         l = self.yg_glyph.yg_font.defaults.get_default("round")
         if l != None:
             if t in l:
                 return True
         l = self.yg_glyph.yg_font.defaults.get_default("no-round")
         if l != None:
             if t in l:
                 return False
         return None
 
-    def make_hint_from_selection(self, hint_type, ctrl=False, shift=False):
+    def make_hint_from_selection(
+        self, hint_type: str, ctrl: bool = False, shift: bool = False
+    ) -> None:
         """Make a hint based on selection in the editing panel.
 
         Should we be making ygModel.ygHint instances here? Since
         we're making valid yaml source, wouldn't it be better to
         pass that with the signal?
         """
         hint_type_num = self.get_hint_type_num(hint_type)
@@ -2114,14 +2202,23 @@
                 if ctrl:
                     self.guess_cv_for_hint(new_yg_hint)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
         if hint_type_num in [1, 3]:
             if pplen >= 2:
+                try:
+                    if hint_type_num == 3:
+                        hint_type = stemFinder(
+                            self._model_point(pp[0]),
+                            self._model_point(pp[1]),
+                            self.yg_glyph,
+                        ).get_color()
+                except Exception as e:
+                    print(e)
                 # ref should be a touched point and target an untouched point.
                 # If it's the other way around, reverse them.
                 if pp[1].touched and not pp[0].touched:
                     pp[0], pp[1] = pp[1], pp[0]
                 target_name = self._model_point(pp[1]).preferred_label()
                 ref_name = self._model_point(pp[0]).preferred_label()
                 h = {"ptid": target_name, "ref": ref_name, "rel": hint_type}
@@ -2154,38 +2251,39 @@
                             untouched_points.append(self._model_point(t))
                 if len(touched_points) == 2 and len(untouched_points) == 1:
                     touched_names = [
                         touched_points[0].preferred_label(),
                         touched_points[1].preferred_label(),
                     ]
                     untouched_name = untouched_points[0].preferred_label()
-                    h = {"ptid": untouched_name, "ref": touched_names, "rel": hint_type}
+                    # Think about this more. Why does mypy not like it?
+                    h = {"ptid": untouched_name, "ref": touched_names, "rel": hint_type}  # type: ignore
                     new_yg_hint = ygHint(self.yg_glyph, h)
                 else:
                     newlist = []
                     for p in pp:
                         newlist.append(self._model_point(p))
                     sorter = ygPointSorter(self.yg_glyph.current_axis())
                     sorter.sort(newlist)
                     target = newlist.pop(1)
                     ref_names = [
                         newlist[0].preferred_label(),
                         newlist[1].preferred_label(),
                     ]
                     target_name = target.preferred_label()
-                    h = {"ptid": target_name, "ref": ref_names, "rel": hint_type}
+                    h = {"ptid": target_name, "ref": ref_names, "rel": hint_type}  # type: ignore
                     new_yg_hint = ygHint(self.yg_glyph, h)
                 dr = self.get_round_default(new_yg_hint)
                 if dr != None:
                     new_yg_hint.set_round(dr)
                 if shift:
                     new_yg_hint.set_round(True)
                 self.sig_new_hint.emit(new_yg_hint)
 
-    def make_macfunc_from_selection(self, hint_type, **kwargs):
+    def make_macfunc_from_selection(self, hint_type: str, **kwargs) -> None:
         hint_type_num = self.get_hint_type_num(hint_type)
         pp = self.selected_objects(True)
         if hint_type_num == 4:
             name = kwargs["name"]
             if hint_type == "function":
                 fu = ygFunction(name, self.yg_glyph.yg_font)
                 pt_names = fu.required_point_list() + fu.optional_point_list()
@@ -2215,15 +2313,15 @@
 
             self.sig_new_hint.emit(yg_hint)
 
     #
     # Event handlers
     #
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         # In ygGlyphScene
         super().mousePressEvent(event)
         modifier = QApplication.keyboardModifiers()
         if event.button() == Qt.MouseButton.LeftButton:
             if not self._mouse_over_point(
                 event.scenePos()
             ) and not self._mouse_over_hint(event.scenePos()):
@@ -2233,28 +2331,28 @@
                     self.yg_selection._cancel_selection()
                 self.dragBeginPoint = event.scenePos()
                 self.selectionRect = SelectionRect(
                     QRectF(self.dragBeginPoint, QSizeF(0, 0))
                 )
                 self.addItem(self.selectionRect)
 
-    def mouseMoveEvent(self, event):
+    def mouseMoveEvent(self, event) -> None:
         super().mouseMoveEvent(event)
         if self.selectionRect != None:
             thisx = abs(self.dragBeginPoint.x() - event.scenePos().x())
             thisy = abs(self.dragBeginPoint.y() - event.scenePos().y())
             if thisy > 4 or thisx > 4:
                 self.selectionRect.setRect(self._adjust_rect(event.scenePos()))
                 self.selectionRect.setPen(QPen(QColor("gray")))
                 if self.selectionRect.isVisible():
                     self.selectionRect.update()
                 else:
                     self.selectionRect.show()
 
-    def mouseReleaseEvent(self, event):
+    def mouseReleaseEvent(self, event) -> None:
         super().mouseReleaseEvent(event)
         if self.selectionRect == None:
             return
         if (
             self.selectionRect.rect().isNull()
             or self.selectionRect.rect().height() == 0
             or self.selectionRect.rect().width() == 0
@@ -2268,15 +2366,15 @@
         ) != Qt.KeyboardModifier.ShiftModifier:
             self.yg_selection._add_rect(self.selectionRect.rect(), False)
         else:
             self.yg_selection._toggle_rect(self.selectionRect.rect())
         self.removeItem(self.selectionRect)
         self.selectionRect = None
 
-    def contextMenuEvent(self, event):
+    def contextMenuEvent(self, event) -> None:
         """This seems horrible, but the most stable procedure (so far) seems
         to be to build every possible menu item and disable/hide the ones
         we don't want.
 
         Checklist of features:
             Toggle visibility of off-curve points: Done
             Toggle point numbers: Done
@@ -2332,24 +2430,24 @@
         point_param_list = []
         black_space = white_space = gray_space = None
 
         cmenu.addSeparator()
 
         # Round point (any ntype but 4)
 
-        round_hint = QAction("Round target point", checkable=True)
+        round_hint = QAction("Round target point", checkable=True)  # type: ignore
         cmenu.addAction(round_hint)
         if hint == None or ntype == 4:
             round_hint.setEnabled(False)
             round_hint.setVisible(False)
         else:
             if self._model_hint(hint).rounded():
                 round_hint.setChecked(True)
 
-        min_dist_action = QAction("Minimum distance", checkable=True)
+        min_dist_action = QAction("Minimum distance", checkable=True)  # type: ignore
         cmenu.addAction(min_dist_action)
         if hint == None or ntype != 3:
             min_dist_action.setEnabled(False)
             min_dist_action.setVisible(False)
         else:
             mh = self._model_hint(hint)
             min_dist_action.setChecked(mh.min_dist())
@@ -2364,15 +2462,15 @@
             cat=self.yg_glyph.get_category(),
             suffix=self.yg_glyph.get_suffixes(),
         )
         cv_list.sort()
         cv_list = ["None", "Guess"] + cv_list
 
         for c in cv_list:
-            ccv = QAction(c, self, checkable=True)
+            ccv = QAction(c, self, checkable=True)  # type: ignore
             if hint != None:
                 if ccv.text() == "None":
                     if hint.yg_hint.cv() == None:
                         ccv.setChecked(True)
                 else:
                     if c == hint.yg_hint.cv():
                         ccv.setChecked(True)
@@ -2397,15 +2495,15 @@
             cat=self.yg_glyph.get_category(),
             suffix=self.yg_glyph.get_suffixes(),
         )
         cv_list.sort()
         cv_list = ["None", "Guess"] + cv_list
         # if len(cv_list) > 0:
         for c in cv_list:
-            ccv = QAction(c, self, checkable=True)
+            ccv = QAction(c, self, checkable=True)  # type: ignore
             if hint != None:
                 if ccv.text() == "None":
                     if hint.yg_hint.cv() == None:
                         ccv.setChecked(True)
                 else:
                     if c == hint.yg_hint.cv():
                         ccv.setChecked(True)
@@ -2422,33 +2520,33 @@
         # Color. We don't recommend setting the "color" bits directly,
         # but rather set "rel" to blackdist, whitedist, etc.
 
         hint_color_menu = cmenu.addMenu("Set distance type...")
 
         no_color_menu = hint == None or ntype != 3
 
-        black_space = QAction("Black", self, checkable=True)
+        black_space = QAction("Black", self, checkable=True)  # type: ignore
         if hint != None:
             if hint.yg_hint.hint_type() in ["stem", "blackdist"]:
                 black_space.setChecked(True)
         hint_color_menu.addAction(black_space)
         if no_color_menu:
             black_space.setEnabled(False)
             black_space.setVisible(False)
 
-        white_space = QAction("White", self, checkable=True)
+        white_space = QAction("White", self, checkable=True)  # type: ignore
         if hint != None:
             if hint.yg_hint.hint_type() == "whitedist":
                 white_space.setChecked(True)
         hint_color_menu.addAction(white_space)
         if no_color_menu:
             white_space.setEnabled(False)
             white_space.setVisible(False)
 
-        gray_space = QAction("Gray", self, checkable=True)
+        gray_space = QAction("Gray", self, checkable=True)  # type: ignore
         if hint != None:
             if hint.yg_hint.hint_type() == "graydist":
                 gray_space.setChecked(True)
         hint_color_menu.addAction(gray_space)
         if no_color_menu:
             gray_space.setEnabled(False)
             gray_space.setVisible(False)
@@ -2494,15 +2592,15 @@
         try:
             # mouse_over_point actually returns a ygPointMarker.
             target_point = hint.mouse_over_point(QPointF(event.scenePos()))
             if hint.yg_hint.hint_type() == "macro":
                 mafu = ygMacro(hint.yg_hint.name, self.yg_glyph.yg_font)
                 point_list = mafu.point_list()
             else:
-                mafu = ygFunction(hint.yg_hint.name, self.yg_glyph.yg_font)
+                mafu = ygFunction(hint.yg_hint.name, self.yg_glyph.yg_font)  # type: ignore
                 point_list = mafu.point_list()
             swap_old_name = target_point.name
             point_list.remove(swap_old_name)
         except Exception as e:
             disable_point_params = True
         point_param_menu = cmenu.addMenu("Point params")
         for p in point_list:
@@ -2517,33 +2615,39 @@
             a = point_param_menu.menuAction()
             a.setEnabled(False)
             a.setVisible(False)
 
         # Set a target or reference point for a function or macro. Only for use in ordering
         # hints: it has no effect on the rendering otherwise.
 
-        if hint:
-            target_point = hint.mouse_over_point(QPointF(event.scenePos()))
-            if target_point != None:
-                target_point = target_point._get_model_point()
-        else:
-            target_point = None
-        new_target = target_point
+        # The next few lines may be stranded. There used to be a "set target" menu item, but
+        # I removed it because it wasn't working, or was causing a crash, or something.
+
+        # if hint:
+        #     target_point = hint.mouse_over_point(QPointF(event.scenePos()))
+        #     if target_point != None:
+        #         target_point = target_point._get_model_point()
+        # else:
+        #     target_point = None
+        # new_target = target_point
 
         # def tgt_pt_check(pt):
         #    if pt == None:
         #        return False
         #    return self.resolve_point_identifier(pt) == target_point
 
         # Make a set. Pointer can be anywhere for this.
 
         # Test whether user can make a set. The rules are:
         #    1. More than one point must be selected.
         #    2. One selected point must be touched by a shift, align or
         #       interpolate instruction (types 1 and 2).
+        #
+        # Is this stranded code? We're no longer offering "Make Set" via the context menu,
+        # and the point of this code seems to be to set a variable that's never consulted.
         touched_point = None
         num_of_selected_points = len(selected_points)
         try:
             if num_of_selected_points >= 2:
                 for p in selected_points:
                     if p.touched and len(p.owners) >= 1:
                         if hint_type_nums[p.owners[0].yg_hint.hint_type()] in [1, 2]:
@@ -2683,71 +2787,77 @@
     font.
 
     parent: Is this used at all?
     """
 
     sig_goto = pyqtSignal(object)
 
-    def __init__(self, preferences, viewer, font, parent=None):
+    def __init__(
+        self,
+        preferences: ygPreferences,
+        viewer: ygGlyphScene,
+        font: ygFont,
+        parent=None,
+    ) -> None:
         super(ygGlyphView, self).__init__(viewer, parent=parent)
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.viewer = viewer
         self.yg_font = font
         self.preferences = preferences
-        self.visited_glyphs = {}
+        self.visited_glyphs: Dict[str, ygGlyphScene] = {}
 
     @pyqtSlot()
-    def make_control_value(self):
+    def make_control_value(self) -> None:
         self.viewer.make_control_value()
 
-    def setup_goto_signal(self, o):
+    def setup_goto_signal(self, o: Callable) -> None:
         self.sig_goto.connect(o)
 
-    def _current_index(self):
+    def _current_index(self) -> int:
         return self.yg_font.get_glyph_index(
             self.viewer.yg_glyph.gname, short_index=True
         )
 
-    def go_to_glyph(self, g):
+    def go_to_glyph(self, g: str) -> None:
         self.preferences["top_window"].disconnect_editor_signals()
         try:
             self.yg_font.get_glyph_index(g, short_index=True)
             self.switch_to(g)
         except Exception as e:
             # print(e)
             self.yg_font.send_error_message(
                 {"msg": "Can't load requested glyph.", "mode": "dialog"}
             )
         self.preferences["top_window"].connect_editor_signals()
 
     # sender returns None when we use the decorator. Rethink these signals?
     @pyqtSlot()
-    def next_glyph(self):
+    def next_glyph(self) -> None:
         current_index = self._current_index()
         if current_index < len(self.yg_font.glyph_list) - 1:
             gname = self.yg_font.glyph_list[current_index + 1][1]
             self.preferences["top_window"].disconnect_editor_signals()
             self.switch_to(gname)
             self.preferences["top_window"].connect_editor_signals()
 
     @pyqtSlot()
-    def previous_glyph(self):
+    def previous_glyph(self) -> None:
         current_index = self._current_index()
         if current_index > 0:
             gname = self.yg_font.glyph_list[current_index - 1][1]
             self.preferences["top_window"].disconnect_editor_signals()
             self.switch_to(gname)
             self.preferences["top_window"].connect_editor_signals()
 
-    def switch_from_font_viewer(self, gname):
+    def switch_from_font_viewer(self, gname: str) -> None:
         self.preferences["top_window"].disconnect_editor_signals()
         self.switch_to(gname)
         self.preferences["top_window"].connect_editor_signals()
 
-    def switch_to(self, gname):
+    def switch_to(self, gname: str) -> None:
         self.viewer.reset_scale()
         self.viewer.yg_glyph.cleanup_glyph()
         # Store the current glyph if it is changed.
         if not self.viewer.yg_glyph.undo_stack.isClean():
             self.visited_glyphs[self.viewer.yg_glyph.gname] = self.viewer
         if gname in self.visited_glyphs:
             self.viewer = self.visited_glyphs[gname]
@@ -2758,77 +2868,78 @@
             new_glyph.restore_gsource()
         else:
             new_glyph = ygGlyph(self.preferences, self.yg_font, gname)
             self.viewer = ygGlyphScene(self.preferences, new_glyph)
         self.preferences.set_current_glyph(self.yg_font.full_name(), gname)
         self.setScene(self.viewer)
         self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
-        self.parent().parent().set_window_title()
+        self.parent().parent().set_window_title()  # type: ignore
         ed = self.preferences.top_window().source_editor
         new_glyph.set_yaml_editor(ed)
 
     @pyqtSlot()
-    def guess_cv(self):
+    def guess_cv(self) -> None:
         try:
             self.viewer.guess_cv()
         except Exception:
             self.yg_font.send_error_message(
                 {"msg": "Error while looking for a control value.", "mode": "console"}
             )
 
     @pyqtSlot(bool)
-    def switch_to_x(self, checked):
+    def switch_to_x(self, checked: bool) -> None:
         if self.viewer:
             if checked and self.viewer.yg_glyph.current_axis() != "x":
-                self.viewer.axis = "x"
+                # self.viewer.axis = "x"
                 self.viewer.yg_glyph.switch_to_axis("x")
-                self.parent().parent().set_window_title()
+                win = self.parent().parent()
+                win.set_window_title()  # type: ignore
 
     @pyqtSlot(bool)
-    def switch_to_y(self, checked):
+    def switch_to_y(self, checked: bool) -> None:
         if self.viewer:
             if checked and self.viewer.yg_glyph.current_axis() != "y":
-                self.viewer.axis = "y"
+                # self.viewer.axis = "y"
                 self.viewer.yg_glyph.switch_to_axis("y")
-                self.parent().parent().set_window_title()
+                win = self.parent().parent()
+                win.set_window_title()  # type: ignore
 
     @pyqtSlot()
-    def cleanup_yaml_code(self):
+    def cleanup_yaml_code(self) -> None:
         self.viewer.yg_glyph.rebuild_current_block()
 
     @pyqtSlot()
-    def make_hint_from_selection(self):
+    def make_hint_from_selection(self) -> None:
         menu_to_hint_type = {
             "Anchor (A)": "anchor",
             "Align (L)": "align",
-            "Shift (S)": "shift",
+            "Shift (H)": "shift",
             "Interpolate (I)": "interpolate",
-            "White Distance (W)": "whitedist",
-            "Black Distance (B)": "blackdist",
-            "Gray Distance (G)": "graydist",
+            "Stem (T)": "graydist",
         }
         with_ctrl = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ControlModifier
         ) == Qt.KeyboardModifier.ControlModifier
         with_shift = (
             QApplication.keyboardModifiers() & Qt.KeyboardModifier.ShiftModifier
         ) == Qt.KeyboardModifier.ShiftModifier
         self.viewer.make_hint_from_selection(
-            menu_to_hint_type[self.sender().text()], ctrl=with_ctrl, shift=with_shift
+            menu_to_hint_type[self.sender().text()], ctrl=with_ctrl, shift=with_shift  # type: ignore
         )
 
     @pyqtSlot()
-    def make_set(self):
+    def make_set(self) -> None:
         self.viewer.make_set()
 
     # Why does sender return None when we use the decorator? What's best in this
-    # situation?
+    # situation? Here are problems: sender_text param is not consulted. Should it be
+    # omitted? Make sure params match, esp. if we change them.
     # @pyqtSlot(object)
-    def zoom(self, sender_text):
-        sender_text = self.sender().text()
+    def zoom(self, sender_text: str) -> None:
+        sender_text = self.sender().text()  # type: ignore
         if sender_text == "Original Size":
             self.viewer.set_zoom_factor(1)
         elif sender_text == "Zoom In":
             if self.viewer.zoom_factor <= 5.75:
                 self.viewer.set_zoom_factor(self.viewer.zoom_factor + 0.25)
         elif sender_text == "Zoom Out":
             if self.viewer.zoom_factor >= 0.5:
@@ -2841,13 +2952,13 @@
 
         # v = self.viewport().geometry()
         # qp = QPoint(round(v.x() + (v.width() / 2)), round(v.y() + (v.height() / 2)))
         # self.centerOn(self.mapToScene(qp))
 
         self.centerOn(self.viewer.center_x, self.sceneRect().center().y())
 
-    def keyPressEvent(self, event):
+    def keyPressEvent(self, event) -> None:
         if event.key() in [16777219, 16777223]:
             self.viewer.delete_selected_hints()
 
-    def focusInEvent(self, event):
+    def focusInEvent(self, event) -> None:
         self.viewer.yg_glyph.undo_stack.setActive(True)
```

### Comparing `ygt-0.1.2/src/ygt/ygModel.py` & `ygt-0.1.3/src/ygt/ygModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # import traceback
-from typing import Any, TypeVar, Union, Optional, List, Callable, overload
+from typing import Any, TypeVar, Union, Optional, List, Callable, overload, Iterable
 from PyQt6.QtCore import (
     Qt,
     QObject,
     QModelIndex,
     pyqtSignal,
     pyqtSlot,
     QAbstractTableModel,
 )
 from PyQt6.QtGui import QUndoCommand, QUndoStack, QAction
-from fontTools import ttLib, ufoLib
+from fontTools import ttLib, ufoLib # type: ignore
 import yaml
 from yaml import Dumper
 import os
 import pathlib
 import uuid
 import random
 import copy
 import unicodedata
 import abc
 from .ygPreferences import ygPreferences
 from .cvGuesser import instanceChecker
 
 # from .ygSchema import error_message, set_error_message, is_cv_delta_valid
-import defcon
-from ufo2ft import compileTTF
+import defcon # type: ignore
+from ufo2ft import compileTTF # type: ignore
 
 hint_type_nums = {
     "anchor": 0,
     "align": 1,
     "shift": 1,
     "interpolate": 2,
     "stem": 3,
@@ -165,15 +165,15 @@
 #
 # saveEditBoxCommand(fontInfoEditCommand): Saves the contents of an editing dialog.
 # setDefaultCommand(fontInfoEditCommand): Sets a default value.
 # deleteDefaultCommand(fontInfoEditCommand): Delete a default key/value pair.
 # roundingDefaultCommand(fontInfoEditCommand): Set all rounding defaults.
 # editCVDeltaCommand(fontInfoEditCommand): change existing CV deltas.
 # addCVDeltaCommand(fontInfoEditCommand): add a CV delta.
-# deleteCVDeltaCommanddeleteCVDeltaCommand Delete a CV delta key/value pair.
+# deleteCVDeltaCommand(fontInfoEditCommand): Delete a CV delta key/value pair.
 # addMasterCommand(fontInfoEditCommand): Add a master.
 # deleteMasterCommand(fontInfoEditCommand): Delete a master.
 # setMasterNameCommand(fontInfoEditCommand): Change a master's display name.
 # setMasterAxisValueCommand(fontInfoEditCommand): Change value in master def.
 # deleteMasterAxisCommand(fontInfoEditCommand): Delete a master axis.
 # addCVCommand(fontInfoEditCommand): Add a control value.
 # setCVPropertyCommand(fontInfoEditCommand): set a CV property.
@@ -282,15 +282,15 @@
         if self.source_type == "yaml":
             f = open(self.filename, "w")
             f.write(yy)
             f.close()
         else:
             if os.path.exists(self.filename):
                 f = ufoLib.UFOWriter(self.filename)
-                f.writeData("org.ygthinter/source.yaml", yy.encode())
+                f.writeData("org.ygthinter/source.yaml", yy.encode()) # type: ignore
                 f.close()
             else:
                 if top_window:
                     msg = "To save to a UFO, you must select an existing UFO."
                     top_window.show_error_message(["Error", "Error", msg])
 
 
@@ -369,15 +369,16 @@
                 self.ft_font = ttLib.TTFont(fontfile)
             except FileNotFoundError as ferr:
                 ft_open_error = True
         elif extension == ".ufo":
             try:
                 ufo = defcon.Font(fontfile)
                 self.ft_font = compileTTF(ufo)
-            except Exception:
+            except Exception as e:
+                print(e)
                 ft_open_error = True
         if ft_open_error:
             raise Exception("Can't find font file " + str(fontfile))
             # Fix this! Need a dialog box and a chance to try again for a valid font.
 
         # Making a deepcopy so we can always have a clean copy of the font to work with.
         self.preview_font = copy.deepcopy(self.ft_font)
@@ -641,15 +642,15 @@
         if u != 65535:
             try:
                 c = unicodedata.category(chr(u))
             except Exception:
                 pass
         return c
 
-    def extreme_points(self, glyph_name: str) -> tuple[int, int]:
+    def extreme_points(self, glyph_name: str) -> tuple[tuple, tuple]:
         """Helper for setting up an initial cvt."""
         g = ygGlyph(ygPreferences(), self, glyph_name)
         last_highest = highest = -10000
         last_lowest = lowest = 10000
         highest_point = -1
         lowest_point = -1
         plist = g.point_list
@@ -905,15 +906,15 @@
         self.on_curve = on_curve
         self.end_of_contour = False
         self.label_pref = label_pref
         self.preferred_name = ""
 
     def preferred_label(
         self, normalized: bool = False, name_allowed: bool = True
-    ) -> Union[int, str]:
+    ) -> str | int:
         if name_allowed:
             if len(self.preferred_name) > 0:
                 return self.preferred_name
         if self.label_pref == "coord":
             if normalized:
                 t = self.coord.replace("{", "")
                 t = t.replace("}", "")
@@ -927,14 +928,17 @@
         self.preferred_name = n
 
     def __eq__(self, other) -> bool:
         try:
             return self.id == other.id
         except AttributeError:
             return False
+        
+    def __str__(self):
+        return str(self.index)
 
 
 class ygParams:
     """Parameters to be sent to a macro or function. There are two sets of
     these: one consisting of points, the other anything else (e.g. cvt
     indexes).
 
@@ -1032,15 +1036,23 @@
         if type(tester) is not ygSet:
             return result
         pts = tester.point_list()
         for pt in pts:
             if pt in self:
                 result.append(pt)
         return result
-
+    
+    def __str__(self):
+        result = "["
+        for count, p in enumerate(self._point_list):
+            if count > 0:
+                result += ", "
+            result += str(p.index)
+        result += "]"
+        return result
 
 #
 # Undo / Redo
 #
 # One helper class(glyphSaver) and several subclasses of QUndoCommand. Each glyph has its
 # own QUndoStack, and these are coordinated at the app level by one QUndoGroup.
 #
@@ -1191,25 +1203,23 @@
 
 class saveEditBoxCommand(fontInfoEditCommand):
     def __init__(
         self, yg_font: ygFont, sourceable: "ygSourceable", c: dict, text: str
     ) -> None:
         self.sourceable = sourceable
         self.c = c
-        self.text = text
+        # self.text = text
         super().__init__(yg_font)
         self.setText(text)
 
     def redo(self):
-        print("Running redo: " + self.text)
         if self.redo_state:
             self.redo_state.restore()
             self.cv_delta.dataChanged.emit(self.index, self.index)
         else:
-            print("Running first")
             self.sourceable._save(self.c)
         self.send_signal()
 
 
 class setDefaultCommand(fontInfoEditCommand):
     def __init__(self, yg_font, yg_defaults, d: dict) -> None:
         self.yg_defaults = yg_defaults
@@ -1727,14 +1737,15 @@
         glyphSourceTester(self.yg_glyph, "swapMacFuncPointsCommand").test()
         self.send_signal()
 
 
 class cleanupGlyphCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph") -> None:
         super().__init__(glyph)
+        self.setText("Clean up code")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             self.yg_glyph._rebuild_current_block()
             self.redo_state = glyphSaver(self.yg_glyph)
@@ -1743,14 +1754,15 @@
 
 
 class changeDistanceTypeCommand(glyphEditCommand):
     def __init__(self, glyph: "ygGlyph", hint: "ygHint", new_color: str) -> None:
         super().__init__(glyph)
         self.hint = hint
         self.new_color = new_color
+        self.setText("Change distance type")
 
     def redo(self) -> None:
         if self.redo_state:
             self.redo_state.restore()
         else:
             self.hint._source["rel"] = self.new_color
             self.redo_state = glyphSaver(self.yg_glyph)
@@ -2072,37 +2084,44 @@
         top_window = self.preferences.top_window()
         if top_window != None:
             self.undo_stack = QUndoStack()
             self.preferences.top_window().add_undo_stack(self.undo_stack)
             self.undo_stack.setActive(True)
         self.yaml_editor = None
         self.yg_font = yg_font
-        self.gsource = yg_font.get_glyph(gname)
+        # The next few lines have to come *after* loading the ft_font (below)
         self.gname = gname
+
+        # Work with the glyph from the fontTools representation of the font.
+
+        try:
+            self.ft_glyph = yg_font.ft_font["glyf"][self.gname]
+        except KeyError:
+            l = list(yg_font.ft_font.getGlyphSet())
+            if "A" in l:
+                self.gname = "A"
+            elif len(l) >= 2:
+                self.gname = l[1]
+            else:
+                raise Exception("Tried to load nonexistent glyph " + self.gname)
+            self.ft_glyph = yg_font.ft_font["glyf"][self.gname]
+
+        # Initialize the source for this glyph.
+
+        self.gsource = yg_font.get_glyph(self.gname)
         self.props = ygGlyphProperties(self)
         self.error = 0
 
-        # Initialize:
-
         if not "y" in self.gsource:
             self.gsource["y"] = {"points": []}
         if not "x" in self.gsource:
             self.gsource["x"] = {"points": []}
 
         self.set_clean()
 
-        # Work with the glyph from the fontTools representation of the font.
-
-        try:
-            self.ft_glyph = yg_font.ft_font["glyf"][gname]
-        except KeyError:
-            # This shouldn't happen: we should intercept bad gnames before we
-            # get here.
-            raise Exception("Tried to load nonexistent glyph " + gname)
-
         # Going to run several indexes for this glyph's points. This is because
         # Xgridfit is permissive about naming, so we need several ways to look
         # up points. (Check later to make sure all these are being used.)
 
         # Extract points from the fontTools Glyph object and store them in a list.
         self.point_list = self._make_point_list()
 
@@ -2121,14 +2140,23 @@
 
         # Decide the initial axis.
         if self.preferences and self.preferences.top_window() != None:
             self._current_axis = self.preferences.top_window().current_axis
         else:
             self._current_axis = "y"
 
+        # A little fix
+
+        backup_axis = self._current_axis
+        self._current_axis = "y"
+        self.fix_hint_types(self.current_block())
+        self._current_axis = "x"
+        self.fix_hint_types(self.current_block())
+        self._current_axis = backup_axis
+
         # Fix up the source to make it more usable.
         self._yaml_add_parents(self.current_block())
         self._yaml_supply_refs(self.current_block())
 
         # This is the QGraphicsScene wrapper for this glyph object. But
         # do we need a reference here in the __init__? It's only used once,
         # in setting up a signal, and there are other ways to do that.
@@ -2349,14 +2377,21 @@
         """Change coordinates in current block to point indices."""
         self.undo_stack.push(changePointNumbersCommand(self, True))
 
     def coords_to_indices(self) -> None:
         """Change point indices in current block to coordinates."""
         self.undo_stack.push(changePointNumbersCommand(self, False))
 
+    def fix_hint_types(self, block):
+        for ppt in block:
+            if "rel" in ppt and "space" in ppt["rel"]:
+                ppt["rel"] = ppt["rel"].replace("space", "dist")
+            if "points" in ppt:
+                self.fix_hint_types(ppt["points"])
+
     def sub_coords(self, block: list, to_coords: bool = True) -> None:
         """Helper for indices_to_coords and coords_to_indices"""
         for ppt in block:
             ppt["ptid"] = self._sub_coords(ppt["ptid"], to_coords)
             if "ref" in ppt:
                 ppt["ref"] = self._sub_coords(ppt["ref"], to_coords)
             if "points" in ppt:
@@ -2911,15 +2946,15 @@
         ...
 
     def _mk_point_list(self, obj: dict, key: str) -> list:
         """Helper for comparison functions. For target points, this will
         recurse into dependent hints to build a complete list.
 
         """
-        hint = ygHint(None, obj)
+        hint = ygHint(None, obj) # type: ignore
         if key == "ptid":
             p = hint.target()
         else:
             p = hint.ref()
         result = []
         if type(p) is dict:
             k = p.keys()
@@ -3471,19 +3506,19 @@
 
     def del_default(self, k):
         self.font.undo_stack.push(deleteDefaultCommand(self.font, self, k))
 
     def _save(self, c: dict):
         k = c.keys()
         for kk in k:
-            self.font_source["defaults"][kk] = c[kk]
+            self.font.source["defaults"][kk] = c[kk]
 
     def save(self, c: dict) -> None:
-        self.yg_font.undo_stack.push(
-            saveEditBoxCommand(self.yg_font, self, c, "Edit Font Defaults")
+        self.font.undo_stack.push(
+            saveEditBoxCommand(self.font, self, c, "Edit Font Defaults")
         )
         # k = c.keys()
         # for kk in k:
         #    self.data[kk] = c[kk]
         # self._save(c)
         self.set_clean(True)
 
@@ -3600,36 +3635,36 @@
         if index.isValid() and role == Qt.ItemDataRole.EditRole:
             self.cvt.yg_font.undo_stack.push(
                 editCVDeltaCommand(self.cvt.yg_font, self, index, value)
             )
             return True
         return False
 
-    def insertRows(self, row, count, parent=QModelIndex()):
+    def insertRows(self, row, count, parent = QModelIndex()):
         """Actually just appends a new row to the existing structure. We never
         insert multiple rows, and we always append rather than insert.
 
         """
         self.cvt.yg_font.undo_stack.push(addCVDeltaCommand(self.cvt.yg_font, self))
         return True
 
     @pyqtSlot()
     def new_row(self):
         self.insertRows(0, 0)
 
-    def deleteRows(self, row, count, parent=QModelIndex()):
+    def deleteRows(self, row, count, parent = QModelIndex()) -> bool:
         c = self.cvt.get_cv(self.name)
-        if "deltas" in c and row < len(c["deltas"]):
+        if "deltas" in c and row < len(c["deltas"]): # type: ignore
             self.cvt.yg_font.undo_stack.push(
                 deleteCVDeltaCommand(self.cvt.yg_font, self, c, row)
             )
             return True
         return False
 
-    def flags(self, index):
+    def flags(self, index: QModelIndex) -> Qt.ItemFlag:
         return super().flags(index) | Qt.ItemFlag.ItemIsEditable
 
     def headerData(self, section, orientation, role):
         if (
             role == Qt.ItemDataRole.DisplayRole
             and orientation == Qt.Orientation.Horizontal
         ):
@@ -3642,30 +3677,30 @@
         self.font_source = source
         self.top_window = top_window
         if not "cvt" in self.font_source:
             self.font_source["cvt"] = {}
         self.data = self.font_source["cvt"]
         super().__init__(self.yg_font, source["cvt"])
 
-    def source(self):
+    def source(self) -> dict:
         return self.font_source["cvt"]
 
-    def _save(self, c: dict):
+    def _save(self, c: dict) -> None:
         self.font_source["cvt"].clear()
         k = c.keys()
         for kk in k:
             self.font_source["cvt"][kk] = c[kk]
 
     def save(self, c: dict) -> None:
         self.yg_font.undo_stack.push(
             saveEditBoxCommand(self.yg_font, self, c, "Edit Control Values")
         )
         self.set_clean(True)
 
-    def keys(self):
+    def keys(self) -> Iterable:
         return self.font_source["cvt"].keys()
 
     def get_cvs(self, glyph: ygGlyph, filters: dict) -> dict:
         """Get a list of control values filtered to match a particular
         environment.
 
         Parameters:
@@ -3777,81 +3812,81 @@
         rather than just a number.
 
         """
         if name in self.font_source["cvt"]:
             return self.font_source["cvt"][name]
         return None
 
-    def get_deltas(self, name: str):
+    def get_deltas(self, name: str) -> ygCVDeltas:
         return ygCVDeltas(self, name)
 
     def add_cv(self, name: str, props: Union[int, dict]) -> None:
         self.yg_font.undo_stack.push(addCVCommand(self.yg_font, name, props))
 
-    def set_cv_property(self, cv_name, prop_name, val):
+    def set_cv_property(self, cv_name: str, prop_name: str, val: Any) -> None:
         self.yg_font.undo_stack.push(
             setCVPropertyCommand(self.yg_font, cv_name, prop_name, val)
         )
 
-    def del_cv_property(self, cv_name, prop_name):
+    def del_cv_property(self, cv_name: str, prop_name: str) -> None:
         self.yg_font.undo_stack.push(
             delCVPropertyCommand(self.yg_font, cv_name, prop_name)
         )
 
-    def del_cv(self, name):
+    def del_cv(self, name: str) -> None:
         self.yg_font.undo_stack.push(deleteCVCommand(self.yg_font, name))
 
-    def rename(self, old_name, new_name):
+    def rename(self, old_name: str, new_name: str) -> None:
         self.yg_font.undo_stack.push(renameCVCommand(self.yg_font, old_name, new_name))
 
     def __len__(self):
         return len(self.font_source["cvt"])
 
 
 class ygFunctions(ygSourceable):
     def __init__(self, font: ygFont, source: dict) -> None:
         super().__init__(font, source)
 
-    def _save(self, c: dict):
+    def _save(self, c: dict) -> None:
         try:
             self.font.source["functions"].clear()
         except KeyError:
             pass
         if not "functions" in self.font.source:
             self.font.source["functions"] = {}
         k = c.keys()
         for kk in k:
             self.font.source["functions"][kk] = c[kk]
 
     def save(self, c: dict) -> None:
-        self.yg_font.undo_stack.push(
-            saveEditBoxCommand(self.yg_font, self, c, "Edit Functions")
+        self.font.undo_stack.push(
+            saveEditBoxCommand(self.font, self, c, "Edit Functions")
         )
         # self._save(c)
         self.set_clean(True)
 
 
 class ygMacros(ygSourceable):
     def __init__(self, font: ygFont, source: dict) -> None:
         super().__init__(font, source)
 
-    def _save(self, c: dict):
+    def _save(self, c: dict) -> None:
         try:
             self.font.source["macros"].clear()
         except KeyError:
             pass
         if not "macros" in self.font.source:
             self.font.source["macros"] = {}
         k = c.keys()
         for kk in k:
             self.font.source["macros"][kk] = c[kk]
 
     def save(self, c: dict) -> None:
-        self.yg_font.undo_stack.push(
-            saveEditBoxCommand(self.yg_font, self, c, "Edit Macros")
+        self.font.undo_stack.push(
+            saveEditBoxCommand(self.font, self, c, "Edit Macros")
         )
         # self._save(c)
         self.set_clean(True)
 
 
 class ygcvar(ygSourceable):
     """This structure is now obsolete. If the more recent way of constructing
@@ -3910,18 +3945,18 @@
 
 class ygGlyphNames(ygSourceable):
     """The collection of glyph and set names."""
 
     def __init__(self, glyph: ygGlyph) -> None:
         self.yg_glyph = glyph
         super().__init__(glyph.yg_font, self.yg_glyph.gsource)
-        self.inverse_dict = {}
+        self.inverse_dict: dict = {}
         self.update_point_names()
 
-    def update_inverse_dict(self):
+    def update_inverse_dict(self) -> dict:
         if "names" in self.yg_glyph.gsource:
             new_dict = {}
             original_dict = self.yg_glyph.gsource["names"]
             for key, value in original_dict.items():
                 if (type(value) is str or type(value) is int) and not value in new_dict:
                     new_dict[value] = key
             return new_dict
@@ -3941,15 +3976,15 @@
         except Exception:
             pass
         try:
             return self.inverse_dict[yg_point.coord]
         except Exception:
             return ""
 
-    def update_point_names(self):
+    def update_point_names(self) -> None:
         self.inverse_dict = self.update_inverse_dict()
         for p in self.yg_glyph.point_list:
             p.preferred_name = self.get_point_name(p)
 
     def has_name(self, n: str) -> bool:
         if "names" in self.yg_glyph.gsource:
             return n in self.yg_glyph.gsource["names"]
```

### Comparing `ygt-0.1.2/src/ygt/ygPreferences.py` & `ygt-0.1.3/src/ygt/ygPreferences.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from typing import Optional, Any
 import yaml
 import platform
 
 try:
     import winreg
 except ModuleNotFoundError:
     pass
 import os
 from yaml import Loader, Dumper
 
 
 class ygPreferences(dict):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super(ygPreferences, self).__init__(*args, **kwargs)
         self["top_window"] = None
         self["show_off_curve_points"] = True
         self["show_point_numbers"] = False
         self["current_glyph"] = {}
         self["current_axis"] = "y"
         self["save_points_as"] = "coord"  # "coord" or "name" or "index"
@@ -43,88 +44,88 @@
             int(self["top_window_pos_y"])
             int(self["top_window_height"])
             int(self["top_window_height"])
             return True
         except Exception:
             return False
 
-    def current_axis(self):
+    def current_axis(self) -> str:
         return self["current_axis"]
 
-    def set_current_axis(self, a):
+    def set_current_axis(self, a: str) -> None:
         self["current_axis"] = a
 
-    def points_as_coords(self):
+    def points_as_coords(self) -> bool:
         return self["points_as_coords"]
 
-    def set_points_as_coords(self, b):
+    def set_points_as_coords(self, b: bool) -> None:
         self["points_as_coords"] = b
 
-    def auto_preview(self):
+    def auto_preview(self) -> bool:
         return self["auto_preview"]
 
-    def set_auto_preview(self, p):
+    def set_auto_preview(self, p: bool) -> None:
         self["auto_preview"] = p
 
-    def zoom_factor(self):
+    def zoom_factor(self) -> float:
         return self["zoom_factor"]
 
-    def set_zoom_factor(self, z):
+    def set_zoom_factor(self, z: float) -> None:
         self["zoom_factor"] = z
 
-    def recents(self):
+    def recents(self) -> dict:
         return self["recents"]
 
-    def add_recent(self, f):
+    def add_recent(self, f: str) -> None:
         if os.path.splitext(f)[1] in [".yaml", ".ufo"]:
             fl = self["recents"]
             if not f in fl:
                 fl = [f] + fl
             if len(fl) > 5:
                 fl.pop()
             self["recents"] = fl
 
-    def top_window(self):
+    def top_window(self) -> Any:
         return self["top_window"]
 
-    def show_off_curve_points(self):
+    def show_off_curve_points(self) -> bool:
         return self["show_off_curve_points"]
 
-    def set_show_off_curve_points(self, b):
+    def set_show_off_curve_points(self, b: bool): # type: ignore
         self["show_off_curve_points"] = b
 
-    def show_point_numbers(self):
+    def show_point_numbers(self) -> bool:
         return self["show_point_numbers"]
 
-    def set_show_point_numbers(self, b):
+    def set_show_point_numbers(self, b: bool) -> None:
         self["show_point_numbers"] = b
 
-    def current_glyph(self, fontfile):
+    def current_glyph(self, fontfile: str) -> str:
         try:
             return self["current_glyph"][fontfile]
         except Exception:
             return "A"
 
-    def set_current_glyph(self, k, gname):
+    def set_current_glyph(self, k: str, gname: str) -> None:
         self["current_glyph"][k] = gname
 
-    def current_font(self):
+    def current_font(self) -> str:
         return self["current_font"]
 
-    def set_current_font(self, f):
+    def set_current_font(self, f: str) -> None:
         self["current_font"] = f
 
-    def points_as(self):
+    def points_as(self) -> str:
         return self["save_points_as"]
 
-    def set_points_as(self, val):
+    def set_points_as(self, val: str) -> None:
         if val in ["indices", "coordinates"]:
             self["points_as"] = val
 
-    def save_config(self):
+    def save_config(self) -> None:
         if platform.system() == "Windows":
             write_win_registry(self)
         config_dir = os.path.expanduser("~/.ygt/")
         if not os.path.isdir(config_dir):
             try:
                 os.mkdir(config_dir)
             except Exception as e:
@@ -137,15 +138,15 @@
         for kk in k:
             if not kk in ["top_window", "current_font"]:
                 save_dict[kk] = self[kk]
         with open(config_file, "w") as f:
             f.write(yaml.dump(save_dict, sort_keys=False, Dumper=Dumper))
 
 
-def open_config(top_window):
+def open_config(top_window: Any) -> ygPreferences:
     if platform.system() == "Windows":
         return read_win_registry(top_window)
     try:
         config_path = os.path.expanduser("~/.ygt/ygt_config.yaml")
         with open(config_path, "r") as pstream:
             pref_dict = yaml.safe_load(pstream)
         p = ygPreferences()
@@ -159,16 +160,19 @@
         print("Exception in open_config:")
         print(e)
         p = ygPreferences()
         p["top_window"] = top_window
         return p
 
 
+# Not doing types for the winreg functions because the winreg module
+# can't be imported on the Mac, where checking is being done.
+
 def read_win_registry(top_window):
-    path = winreg.HKEY_CURRENT_USER
+    path = winreg.HKEY_CURRENT_USER # type: ignore
     p = ygPreferences()
     try:
         key = winreg.OpenKeyEx(path, r"SOFTWARE\\ygt\\")
     except Exception as e:
         print("Can't open registry")
         p["top_window"] = top_window
         return p
```

### Comparing `ygt-0.1.2/src/ygt/ygPreview.py` & `ygt-0.1.3/src/ygt/ygPreview.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,47 @@
+from typing import Callable, List, Optional
 from .freetypeFont import freetypeFont, RENDER_GRAYSCALE, RENDER_LCD_1, RENDER_LCD_2
 from PyQt6.QtWidgets import (
     QWidget,
     QLabel,
     QLineEdit,
     QPushButton,
     QHBoxLayout,
     QVBoxLayout,
 )
-from PyQt6.QtGui import QPainter, QBrush, QColor
+from PyQt6.QtGui import QPainter, QBrush, QColor, QPalette
 from PyQt6.QtCore import Qt, QRect, pyqtSignal, pyqtSlot, QLine
 
 
 PREVIEW_WIDTH = 450
 PREVIEW_HEIGHT = 700
 STRING_PREVIEW_HEIGHT = 150
 PREVIEW_HORI_MARGIN = 25
 PREVIEW_VERT_MARGIN = 50
 
 
 class ygPreviewContainer(QWidget):
     def __init__(self, preview, string_preview):
         super().__init__()
-        self.layout = QVBoxLayout()
-        self.layout.setSpacing(0)
-        self.layout.setContentsMargins(0, 0, 0, 0)
-        self.layout.addWidget(preview)
-        self.layout.addWidget(string_preview)
-        self.setLayout(self.layout)
+        self._layout = QVBoxLayout()
+        self._layout.setSpacing(0)
+        self._layout.setContentsMargins(0, 0, 0, 0)
+        self._layout.addWidget(preview)
+        self._layout.addWidget(string_preview)
+        self.setLayout(self._layout)
 
 
 class ygPreview(QWidget):
+
     sig_preview_paint_done = pyqtSignal(object)
 
-    def __init__(self, top_window):
+    def __init__(self, top_window) -> None:
         super().__init__()
         self.top_window = top_window
-        self.face = None
+        self.face: Optional[freetypeFont] = None
         self.hinting = "on"
         self.glyph_index = 0
         self.char_size = 30
         self.label = QLabel()
         self.label.setStyleSheet("QLabel {background-color: transparent; color: red;}")
         self.label.setText(str(self.char_size) + "ppem")
         self.label.setParent(self)
@@ -67,31 +69,39 @@
         # self.baseline_position = 0
         # The top of the grid should be offset this far from self.vertical_margin
         self.top_grid_offset = 0
         # The pixels of the glyph start this far down.
         self.top_char_margin = 0
         self.show_grid = True
         # Two- or three-dimensional array shaped by numpy.
-        self.Z = []
-        self.instance_dict = None
-        self.instance = None
+        self.Z: list = []
+        self.instance_dict: Optional[dict] = None
+        self.instance: Optional[str] = None
+        text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
+        bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+        self.dark_theme = text_hsv_value > bg_hsv_value
+        print(self.dark_theme)
         self.colors = self.mk_color_list()
         self.render_mode = RENDER_LCD_1
         self.hinting_on = True
-        self.paintEvent = self.paintEvent_b
+        self.paintEvent = self.paintEvent_b # type: ignore
 
-    def set_up_signal(self, func):
+    def set_up_signal(self, func: Callable) -> None:
         self.sig_preview_paint_done.connect(func)
 
-    def mk_color_list(self):
+    def mk_color_list(self) -> List[QColor]:
         """Pre-build a list of grayscale colors--for the big preview."""
         l = [0] * 256
         for count, c in enumerate(l):
-            l[count] = QColor(101, 53, 15, count)
-        return l
+            # Mypy complains about this, and I have no idea what is actually wrong.
+            if self.dark_theme:
+                l[count] = QColor(255, 255, 255, count) # type: ignore
+            else:
+                l[count] = QColor(101, 53, 15, count) # type: ignore
+        return l # type: ignore
 
     def fetch_glyph(self, font, glyph_index):
         """Get a temporary FreeType font, then build the specified glyph.
 
         params:
 
         font: see freetypeFont for details.
@@ -99,15 +109,15 @@
         glyph_index: Index in the font of the glyph to build.
 
         """
         self.glyph_index = glyph_index
         self.face = freetypeFont(font)
         self._build_glyph()
 
-    def _build_glyph(self):
+    def _build_glyph(self) -> bool:
         """Shape the point array and figure some key values."""
         if self.face == None:
             return False
         self.face.set_render_mode(self.render_mode)
         self.face.set_hinting_on(self.hinting_on)
         self.face.set_size(self.char_size)
         self.face.set_instance(self.instance)
@@ -154,145 +164,145 @@
         else:
             if self.pixel_size < 1:
                 self.pixel_size = 1
         self.Z = self.face.mk_array(gdata, self.render_mode)
         return True
 
     @pyqtSlot()
-    def toggle_show_hints(self):
+    def toggle_show_hints(self) -> None:
         self.hinting_on = not self.hinting_on
         self.face.set_hinting_on(self.hinting_on)
         # self._build_glyph()
         self.update()
 
     @pyqtSlot()
-    def toggle_grid(self):
+    def toggle_grid(self) -> None:
         self.show_grid = not self.show_grid
         # self._build_glyph()
         self.update()
 
     @pyqtSlot()
-    def render1(self):
+    def render1(self) -> None:
         self.set_render_mode(RENDER_GRAYSCALE)
 
     @pyqtSlot()
-    def render2(self):
+    def render2(self) -> None:
         self.set_render_mode(RENDER_LCD_1)
 
     @pyqtSlot()
-    def render3(self):
+    def render3(self) -> None:
         self.set_render_mode(RENDER_LCD_2)
 
-    def set_render_mode(self, m):
+    def set_render_mode(self, m: int) -> None:
         self.render_mode = m
         if self.render_mode == RENDER_GRAYSCALE:
-            self.paintEvent = self.paintEvent_a
+            self.paintEvent = self.paintEvent_a # type: ignore
         elif self.render_mode == RENDER_LCD_1:
-            self.paintEvent = self.paintEvent_b
+            self.paintEvent = self.paintEvent_b # type: ignore
         else:
-            self.paintEvent = self.paintEvent_c
+            self.paintEvent = self.paintEvent_c # type: ignore
         # self._build_glyph()
         self.update()
 
-    def set_size(self, n):
+    def set_size(self, n: str | int) -> None:
         n = int(n)
         if self.face != None:
             try:
                 self.char_size = n
                 if self.char_size < 10:
                     self.char_size = 10
                 self.face.set_size(self.char_size)
             except Exception as e:
                 return
             # self.label.setText(str(self.char_size) + "ppem")
             self.set_label_text()
             # self._build_glyph()
             self.update()
 
-    def resize_by(self, n):
+    def resize_by(self, n: int) -> None:
         if self.face != None and self.glyph_index != 0:
             # self.char_size += n
             # self.set_label_text()
             self.set_size(self.char_size + n)
             self.update()
 
-    def set_label_text(self):
+    def set_label_text(self) -> None:
         t = str(self.char_size) + "ppem"
         if self.instance != None:
             t += " — " + self.instance
         self.label.setText(t)
         self.label.adjustSize()
 
-    def add_instances(self, instances):
+    def add_instances(self, instances: dict) -> None:
         self.instance_dict = instances
 
-    def instance_list(self):
+    def instance_list(self) -> list:
         l = []
         if self.instance_dict:
             kk = self.instance_dict.keys()
             for k in kk:
                 l.append(k)
         return l
 
     @pyqtSlot()
-    def next_instance(self):
+    def next_instance(self) -> None:
         if self.instance and self.instance_dict:
             kk = self.instance_dict.keys()
             il = self.instance_list()
             i = il.index(self.instance)
             try:
                 k = il[i + 1]
             except Exception:
                 k = il[0]
             self.instance = k
             self._set_instance()
 
     @pyqtSlot()
-    def prev_instance(self):
+    def prev_instance(self) -> None:
         if self.instance and self.instance_dict:
             kk = self.instance_dict.keys()
             il = self.instance_list()
             i = il.index(self.instance)
             try:
                 k = il[i - 1]
             except Exception:
                 k = il[-1]
             self.instance = k
             self._set_instance()
 
     @pyqtSlot()
-    def set_instance(self):
-        self.instance = self.sender().text()
+    def set_instance(self) -> None:
+        self.instance = self.sender().text() # type: ignore
         self._set_instance()
 
-    def _set_instance(self):
+    def _set_instance(self) -> None:
         self.face.set_instance(self.instance)
         self.set_label_text()
         # self._build_glyph()
         self.update()
 
     @pyqtSlot()
-    def bigger_one(self):
+    def bigger_one(self) -> None:
         self.resize_by(1)
 
     @pyqtSlot()
-    def bigger_ten(self):
+    def bigger_ten(self) -> None:
         self.resize_by(10)
 
     @pyqtSlot()
-    def smaller_one(self):
+    def smaller_one(self) -> None:
         if self.char_size > 10:
             self.resize_by(-1)
 
     @pyqtSlot()
-    def smaller_ten(self):
+    def smaller_ten(self) -> None:
         if self.char_size > 20:
             self.resize_by(-10)
 
-    def draw_grid(self, painter):
+    def draw_grid(self, painter: QPainter) -> None:
         if self.pixel_size < 5:
             return
         top = self.vertical_margin + (self.top_grid_offset * self.pixel_size)
         left = self.horizontal_margin
         height = self.grid_height
         baseline = self.face.ascender
 
@@ -302,36 +312,48 @@
         if self.render_mode != RENDER_GRAYSCALE:
             line_length = int(line_length / 3)
 
         for i, r in enumerate(range(height)):
             if i == baseline:
                 pen.setColor(QColor("red"))
             else:
-                pen.setColor(QColor(50, 50, 50, 50))
+                if self.dark_theme:
+                    pen.setColor(QColor(200, 200, 200, 50))
+                else:
+                    pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             painter.drawLine(QLine(left, top, left + line_length, top))
             top += self.pixel_size
 
         if self.render_mode in [RENDER_GRAYSCALE, RENDER_LCD_1]:
             grid_width = self.face.glyph_slot.bitmap.width + 1
             if self.render_mode == RENDER_LCD_1:
                 grid_width = round(grid_width / 3) + 1
             y_top = self.vertical_margin + (self.top_grid_offset * self.pixel_size)
             y_bot = top - self.pixel_size
-            pen.setColor(QColor(50, 50, 50, 50))
+            if self.dark_theme:
+                pen.setColor(QColor(200, 200, 200, 50))
+            else:
+                pen.setColor(QColor(50, 50, 50, 50))
             painter.setPen(pen)
             for i, r in enumerate(range(grid_width)):
                 painter.drawLine(QLine(left, y_top, left, y_bot))
                 left += self.pixel_size
 
-    def paintEvent_a(self, event):
+    def paintEvent_a(self, event) -> None:
         """Paint grayscale glyph."""
         painter = QPainter(self)
         brush = QBrush()
-        brush.setColor(QColor("white"))
+        #text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
+        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+        #self.dark_theme = text_hsv_value > bg_hsv_value
+        if self.dark_theme:
+            brush.setColor(QColor("black"))
+        else:
+            brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
@@ -348,19 +370,25 @@
             yposition += self.pixel_size
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
-    def paintEvent_b(self, event):
+    def paintEvent_b(self, event) -> None:
         """Paint subpixel rendering with solid pixels."""
         painter = QPainter(self)
         brush = QBrush()
-        brush.setColor(QColor("white"))
+        #text_hsv_value = self.palette().color(QPalette.ColorRole.WindowText).value()
+        #bg_hsv_value = self.palette().color(QPalette.ColorRole.Base).value()
+        #self.dark_theme = text_hsv_value > bg_hsv_value
+        if self.dark_theme:
+            brush.setColor(QColor("black"))
+        else:
+            brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
@@ -369,110 +397,127 @@
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
         for row in self.Z:
             for col in row:
                 rgb = []
                 for elem in col:
                     rgb.append(elem)
-                qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
+                if self.dark_theme:
+                    qc = QColor(rgb[0], rgb[1], rgb[2])
+                else:
+                    qc = QColor(255 - rgb[0], 255 - rgb[1], 255 - rgb[2])
                 qr = QRect(xposition, yposition, self.pixel_size, self.pixel_size)
                 painter.fillRect(qr, qc)
                 xposition += self.pixel_size
             yposition += self.pixel_size
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
-    def paintEvent_c(self, event):
+    def paintEvent_c(self, event) -> None:
         """Paint subpixel rendering with rgb pixel trios."""
         painter = QPainter(self)
         brush = QBrush()
-        brush.setColor(QColor("white"))
+        if self.dark_theme:
+            brush.setColor(QColor("black"))
+        else:
+            brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
         if not self._build_glyph():
             painter.end()
             return
         if len(self.Z) == 0:
             painter.end()
             return
         xposition = self.horizontal_margin
         yposition = self.vertical_margin + (self.top_char_margin * self.pixel_size)
         for row in self.Z:
             for col in row:
                 for n, elem in enumerate(col):
-                    if n == 0:
-                        qc = QColor(255 - elem, 0, 0)
-                    elif n == 1:
-                        qc = QColor(0, 255 - elem, 0)
-                    elif n == 2:
-                        qc = QColor(0, 0, 255 - elem)
+                    if self.dark_theme:
+                        if n == 0:
+                            qc = QColor(elem, 0, 0)
+                        elif n == 1:
+                            qc = QColor(0, elem, 0)
+                        elif n == 2:
+                            qc = QColor(0, 0, elem)
+                    else:
+                        if n == 0:
+                            qc = QColor(255 - elem, 0, 0)
+                        elif n == 1:
+                            qc = QColor(0, 255 - elem, 0)
+                        elif n == 2:
+                            qc = QColor(0, 0, 255 - elem)
                     qr = QRect(
                         int(xposition),
                         int(yposition),
                         int(self.pixel_size / 3),
                         int(self.pixel_size),
                     )
                     painter.fillRect(qr, qc)
-                    xposition += self.pixel_size / 3
+                    xposition += int(self.pixel_size / 3)
             yposition += self.pixel_size
             xposition = self.horizontal_margin
         if self.show_grid:
             self.draw_grid(painter)
         painter.end()
         self.sig_preview_paint_done.emit(None)
 
 
 class ygStringPreviewPanel(QWidget):
     sig_go_to_glyph = pyqtSignal(object)
 
-    def __init__(self, yg_preview, top_window):
+    def __init__(self, yg_preview: ygPreview, top_window) -> None:
         super().__init__()
         self.yg_preview = yg_preview
         self.top_window = top_window
         self.face = self.yg_preview.face
         self._text = ""
         self.minimum_x = PREVIEW_WIDTH
         self.minimum_y = 200
         self.setMinimumSize(self.minimum_x, self.minimum_y)
-        self.paintEvent = self.paintEvent_a
-        self.rect_list = []
+        self.paintEvent = self.paintEvent_a # type: ignore
+        self.rect_list: list = []
 
-    def set_go_to_signal(self, func):
+    def set_go_to_signal(self, func: Callable) -> None:
         self.sig_go_to_glyph.connect(func)
 
-    def set_face(self, face):
+    def set_face(self, face) -> None:
         self.face = face
 
-    def set_text(self, t):
+    def set_text(self, t: str) -> None:
         self._text = t
 
-    def string_to_glyph_list(self, s):
+    def string_to_glyph_list(self, s: str) -> list:
         """Get a list of glyph names needed for string s."""
         yg_font = self.top_window.glyph_pane.viewer.yg_glyph.yg_font
         result = []
         for c in s:
             try:
                 if not c in result:
                     result.append(yg_font.unicode_to_name[ord(c)])
             except Exception:
                 result.append(".notdef")
         return result
 
-    def _fill_background(self, painter):
+    def _fill_background(self, painter: QPainter) -> None:
         brush = QBrush()
-        brush.setColor(QColor("white"))
+        if self.yg_preview.dark_theme:
+            brush.setColor(QColor("black"))
+        else:
+            brush.setColor(QColor("white"))
         brush.setStyle(Qt.BrushStyle.SolidPattern)
         rect = QRect(0, 0, self.width(), self.height())
         painter.fillRect(rect, brush)
 
-    def paintEvent_a(self, event):
+    def paintEvent_a(self, event) -> None:
         painter = QPainter(self)
         self._fill_background(painter)
         if self.face == None:
             painter.end()
             return
         if not self.yg_preview:
             return
@@ -484,40 +529,49 @@
                 glyph=self.yg_preview.glyph_index,
                 render_mode=self.yg_preview.render_mode,
                 hinting_on=self.yg_preview.hinting_on,
                 size=s,
                 instance=self.yg_preview.instance,
             )
             advance = self.face.draw_char(
-                painter, xposition, yposition, spacing_mark=True
+                painter,
+                xposition,
+                yposition,
+                spacing_mark=True,
+                dark_theme=self.yg_preview.dark_theme
             )
             xposition += advance
             if xposition + advance > (PREVIEW_WIDTH - 50):
                 if yposition == 66:
                     xposition = 25
                     yposition = 133
                 else:
                     break
         self.rect_list = self.face.rect_list
         painter.end()
 
-    def paintEvent_b(self, event):
+    def paintEvent_b(self, event) -> None:
         painter = QPainter(self)
         self._fill_background(painter)
         if not self.yg_preview:
             return
         xposition = 25
         yposition = 66
         self.face = self.yg_preview.face
         self.rect_list = self.face.draw_string(
-            painter, self._text, xposition, yposition, x_limit=PREVIEW_WIDTH - 50
+            painter,
+            self._text,
+            xposition,
+            yposition,
+            x_limit = PREVIEW_WIDTH - 50,
+            dark_theme = self.yg_preview.dark_theme
         )
         painter.end()
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event) -> None:
         qp = event.position()
         x = int(qp.x())
         y = int(qp.y())
         rr = None
         for r in self.rect_list:
             if r.contains(x, y):
                 rr = r
@@ -526,17 +580,18 @@
             if self.paintEvent == self.paintEvent_a:
                 self.yg_preview.set_size(rr.size)
             else:
                 self.sig_go_to_glyph.emit(rr.gname.decode())
 
 
 class ygStringPreview(QWidget):
+
     sig_string_changed = pyqtSignal(object)
 
-    def __init__(self, yg_preview, top_window):
+    def __init__(self, yg_preview: ygPreview, top_window) -> None:
         super().__init__()
         self.yg_preview = yg_preview
         self.top_window = top_window
 
         self._layout = QVBoxLayout()
 
         self.panel = ygStringPreviewPanel(yg_preview, top_window)
@@ -555,23 +610,23 @@
         self.qle.editingFinished.connect(self.got_string)
 
         self._layout.addWidget(self.panel)
         self._layout.addWidget(self.button_widget)
 
         self.setLayout(self._layout)
 
-    def set_go_to_signal(self, func):
+    def set_go_to_signal(self, func: Callable) -> None:
         self.panel.set_go_to_signal(func)
 
-    def set_string_preview(self):
-        self.panel.paintEvent = self.panel.paintEvent_b
+    def set_string_preview(self) -> None:
+        self.panel.paintEvent = self.panel.paintEvent_b # type: ignore
 
-    def set_size_array(self):
-        self.panel.paintEvent = self.panel.paintEvent_a
+    def set_size_array(self) -> None:
+        self.panel.paintEvent = self.panel.paintEvent_a # type: ignore
 
-    def set_face(self, f):
+    def set_face(self, f: freetypeFont) -> None:
         if self.panel != None:
             self.panel.face = f
 
-    def got_string(self):
+    def got_string(self) -> None:
         self.panel.set_text(self.qle.text())
         self.sig_string_changed.emit(self.panel._text)
```

### Comparing `ygt-0.1.2/src/ygt/ygSchema.py` & `ygt-0.1.3/src/ygt/ygSchema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-from schema import Or, Optional, Schema, SchemaError, Use, And
+from typing import Any
+from schema import Or, Optional, Schema, SchemaError, Use, And # type: ignore
 
 # from .ygModel import unicode_categories
 import re
 
 _error_message = ""
 
 DELTA_DIST = [-8, -7, -6, -5, -4, -3, -2, -1, 1, 2, 3, 4, 5, 6, 7, 8]
 DELTA_SHIFT = [2, 4, 8, 16, 32, 64]
 
 
-def set_error_message(t):
+def set_error_message(t: str) -> None:
     global _error_message
     if not _error_message:
         _error_message = t
 
 
 def error_message(reset: bool = True) -> str:
     global _error_message
     r = _error_message
     if reset:
         _error_message = ""
     return r
 
 
-def have_error_message():
+def have_error_message() -> bool:
     return bool(_error_message)
 
 
-def is_cv_distance_valid(s):
+def is_cv_distance_valid(s: Any) -> bool:
     try:
         sss = float(s)
     except Exception:
         sss = s
     if type(sss) is float or type(sss) is int:
         f = float(sss)
         return f >= -4.0 and f <= 4.0
     if type(sss) is str:
-        ss = sss.split("/", 1)
+        ss = sss.split("/", 1) # type: ignore
         try:
             left = int(ss[0])
             right = int(ss[1])
         except Exception:
             return False
         return left in DELTA_DIST and right in DELTA_SHIFT
     return False
 
 
-def is_point_valid_1(pt):
+def is_point_valid_1(pt: int | str | list | dict) -> bool:
     if type(pt) is int:
         return True
     if type(pt) is str:
         if re.match("^[a-zA-Z][0-9A-Za-z-_]*", pt):
             return True
         if re.search("\{[\d\-][\d]{0,3};[\d\-][\d]{0,3}\}", pt):
             return True
@@ -68,15 +69,15 @@
                 err = True
         if not err:
             return True
     set_error_message("point " + str(pt) + " is not valid")
     return False
 
 
-def is_point_valid_2(pt):
+def is_point_valid_2(pt: int | str | list) -> bool:
     if type(pt) is int:
         return True
     if type(pt) is str:
         if re.match("^[a-zA-Z][0-9A-Za-z-_]*", pt):
             return True
         if re.search("\{[\d\-][\d]{0,3};[\d\-][\d]{0,3}\}", pt):
             return True
@@ -87,25 +88,25 @@
                 err = True
         if not err:
             return True
     set_error_message("point " + str(pt) + " is not valid")
     return False
 
 
-def validate_points(pt):
+def validate_points(pt: list) -> bool:
     try:
         for p in pt:
             nested_point_schema.validate(p)
         return True
     except Exception as e:
         set_error_message("point " + str(pt) + " is not valid.")
     return False
 
 
-def is_round_valid(r):
+def is_round_valid(r: bool | str) -> bool:
     if type(r) is bool:
         return True
     return r in [
         "to-grid",
         "to-half-grid",
         "to-double-grid",
         "down-to-grid",
@@ -309,19 +310,19 @@
     Optional("init-graphics"): bool,
     Optional("compact"): bool,
 }
 
 names_struct = {str: is_point_valid_2}
 
 
-def tag_checker(s):
+def tag_checker(s: str) -> bool:
     return bool(re.match("^[A-Za-z]{4}$", s))
 
 
-def name_checker(s):
+def name_checker(s: str) -> bool:
     return bool(re.match("^[a-zA-Z][0-9A-Za-z-_]*$", s))
 
 
 cvar_entry_struct = [
     {
         "regions": [{"tag": tag_checker, "val": float}],
         "vals": [{"nm": name_checker, "val": int}],
@@ -329,15 +330,15 @@
 ]
 
 point_schema = Schema(point_struct)
 nested_point_schema = Schema(nested_point_struct)
 defaults_schema = Schema(defaults_struct)
 
 
-def is_valid(t):
+def is_valid(t: Any) -> bool:
     try:
         point_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in YAML source: " + str(s))
     return False
 
@@ -348,93 +349,94 @@
 prep_schema = Schema({"code": str})
 function_schema = Schema(function_entry_struct)
 macro_schema = Schema(macro_entry_struct)
 props_schema = Schema(properties_struct)
 names_schema = Schema(names_struct)
 
 
-def is_cv_delta_valid(c):
+def is_cv_delta_valid(c: dict) -> bool:
     try:
         cv_delta_schema.validate(c)
         return True
     except SchemaError as s:
         set_error_message("Illegal value in Control Value Delta: " + str(s))
     return False
 
 
-def is_cvt_valid(t):
+def is_cvt_valid(t: dict) -> bool:
     try:
         k = t.keys()
         for kk in k:
             cvt_schema.validate(t[kk])
         return True
     except SchemaError as s:
         set_error_message("Error in Control Value Table: " + str(s))
     return False
 
 
-def is_cvar_valid(t):
+def is_cvar_valid(t: dict) -> bool:
     try:
         cvar_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in cvar: " + str(s))
     return False
 
 
-def is_prep_valid(t):
+def is_prep_valid(t: dict) -> bool:
     try:
         prep_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in prep: " + str(s))
     return False
 
 
-def are_functions_valid(t):
+def are_functions_valid(t: dict) -> bool:
     try:
         for k in t.keys():
             function_schema.validate(t[k])
         return True
     except SchemaError as s:
         set_error_message("Error in functions: " + str(s))
     return False
 
 
-def are_macros_valid(t):
+def are_macros_valid(t: dict) -> bool:
     try:
         for k in t.keys():
             macro_schema.validate(t[k])
         return True
     except SchemaError as s:
         set_error_message("Error in macros: " + str(s))
     return False
 
 
-def are_defaults_valid(t):
+def are_defaults_valid(t: dict) -> bool:
     try:
         defaults_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in defaults: " + str(s))
     return False
 
 
-def are_names_valid(t):
+def are_names_valid(t: dict) -> bool:
     try:
         names_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in point names: " + str(s))
     return False
 
 
-def are_properties_valid(t):
+def are_properties_valid(t: dict) -> bool:
     try:
         props_schema.validate(t)
         return True
     except SchemaError as s:
         set_error_message("Error in glyph properties: " + str(s))
+    return False
 
 
-def always_valid(t):
+def always_valid(t) -> bool:
     return True
```

### Comparing `ygt-0.1.2/src/ygt/ygYAMLEditor.py` & `ygt-0.1.3/src/ygt/ygYAMLEditor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from typing import Optional, Callable, Any
 from PyQt6.QtCore import pyqtSignal, Qt, QTimer, pyqtSlot
 from PyQt6.QtWidgets import QDialog, QVBoxLayout, QPlainTextEdit, QDialogButtonBox
 from PyQt6.QtGui import QSyntaxHighlighter, QTextCharFormat, QColor
 import yaml
 import re
 from yaml import Dumper
 import copy
-from schema import SchemaError
+from schema import SchemaError # type: ignore
 from .ygSchema import is_valid, set_error_message, error_message, have_error_message
+from .ygModel import ygSourceable
+from .ygPreferences import ygPreferences
 
 
 # From https://stackoverflow.com/questions/8640959/
 # how-can-i-control-what-scalar-form-pyyaml-uses-for-my-data
 # Presumed public domain, since it was posted in a public forum.
 def str_presenter(dumper, data):
     if len(data.splitlines()) > 1:  # check for multiline string
@@ -32,75 +35,77 @@
     preferences (ygPreferences): The preferences object for the current file.
     """
 
     sig_source_from_editor = pyqtSignal(object)
     sig_status = pyqtSignal(object)
     sig_error = pyqtSignal(object)
 
-    def __init__(self, preferences, parent=None):
+    def __init__(self, preferences, parent = None) -> None:
         super().__init__()
         self.setAttribute(Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.setStyleSheet(
-            "ygYAMLEditor {font-family: Source Code Pro, monospace; background-color: white; }"
+            "ygYAMLEditor {font-family: Source Code Pro, monospace; }"
         )
+        # ; background-color: white
         self.setLineWrapMode(QPlainTextEdit.LineWrapMode.NoWrap)
         self.preferences = preferences
         self.textChanged.connect(self.text_changed)
         self._highlighter = ygGlyphHighlighter()
         self._timer = QTimer()
         self._timer.timeout.connect(self.check_valid)
         self.code_valid = True
         self.setup_editor()
 
-    def setup_error_signal(self, f):
+    def setup_error_signal(self, f: Callable) -> None:
         self.sig_error.connect(f)
 
     @pyqtSlot(object)
-    def install_source(self, text):
+    def install_source(self, text: str) -> None:
         self.setPlainText(text)
 
     @pyqtSlot()
-    def yaml_source(self):
+    def yaml_source(self) -> None:
         err = False
-        msg = ""
+        # msg = ""
+        s = ""
         try:
             s = yaml.safe_load(self.toPlainText())
         except Exception as e:
             err = True
             set_error_message("Source can't be parsed.")
             msg = str(e)
         if not err:
             try:
                 err = not is_valid({"points": s})
-            except SchemaError as s:
+            except SchemaError as se:
                 err = True
         if err:
             self.sig_error.emit({"msg": error_message(), "mode": "console"})
         else:
             self.sig_source_from_editor.emit(s)
 
-    def setup_status_indicator(self, o):
+    def setup_status_indicator(self, o: Callable) -> None:
         self.sig_status.connect(o)
 
-    def setup_editor_signals(self, f):
+    def setup_editor_signals(self, f: Callable) -> None:
         self.sig_source_from_editor.connect(f)
 
-    def disconnect_editor_signals(self, f):
+    def disconnect_editor_signals(self, f: Callable) -> None:
         self.sig_source_from_editor.disconnect(f)
 
     @pyqtSlot()
-    def check_valid(self):
+    def check_valid(self) -> None:
         if not self.code_valid:
             if not have_error_message():
                 set_error_message("Source can't be parsed.")
             self.sig_error.emit({"msg": error_message(), "mode": "console"})
             self.sig_status.emit(self.code_valid)
 
     @pyqtSlot()
-    def text_changed(self):
+    def text_changed(self) -> None:
         self.code_valid = True
         y = self.toPlainText()
         if len(y) == 0:
             self.setPlainText("[]\n")
         else:
             try:
                 y = yaml.safe_load(y)
@@ -117,29 +122,29 @@
                 self._timer.stop()
             except Exception:
                 pass
             self.sig_status.emit(self.code_valid)
         else:
             self._timer.start(2000)
 
-    def setup_editor(self):
+    def setup_editor(self) -> None:
         tags = r"\b(ptid|ref|rel|macro|function|pos|dist|points|round|min)\:"
         twospace = r"(  |\- )"
         fourspace = r"(    |  \- )"
         sixspace = r"(      |    \- )"
         eightspace = r"(        |      \- )"
         tenspace = r"(          |        \- )"
 
         keytwo_format = QTextCharFormat()
-        keytwo_format.setForeground(QColor(122, 6, 70, 255))
+        keytwo_format.setForeground(QColor(182, 6, 70, 255))
         pattern = twospace + tags
         self._highlighter.add_mapping(pattern, keytwo_format)
 
         keyfour_format = QTextCharFormat()
-        keyfour_format.setForeground(QColor("blue"))
+        keyfour_format.setForeground(QColor(75, 75, 255, 255))
         pattern = fourspace + tags
         self._highlighter.add_mapping(pattern, keyfour_format)
 
         keysix_format = QTextCharFormat()
         keysix_format.setForeground(QColor(201, 91, 12, 255))
         pattern = sixspace + tags
         self._highlighter.add_mapping(pattern, keysix_format)
@@ -151,15 +156,15 @@
 
         keyten_format = QTextCharFormat()
         keyten_format.setForeground(QColor("brown"))
         pattern = tenspace + tags
         self._highlighter.add_mapping(pattern, keyten_format)
 
         list_format = QTextCharFormat()
-        list_format.setForeground(QColor("red"))
+        list_format.setForeground(QColor(255, 75, 75, 255))
         pattern = r"^(\- |  \- |    \- |      \- |        \- |          \- )"
         self._highlighter.add_mapping(pattern, list_format)
 
         self._highlighter.setDocument(self.document())
 
 
 class editorPane(QPlainTextEdit):
@@ -180,15 +185,21 @@
     save_on_focus_out (bool): Whether to auto-save if user leaves this
     editor.
 
     """
 
     sig_error = pyqtSignal(object)
 
-    def __init__(self, owner, sourceable, validator, save_on_focus_out=False):
+    def __init__(
+            self,
+            owner: "editorDialog",
+            sourceable: ygSourceable,
+            validator: Callable,
+            save_on_focus_out: bool = False
+        ) -> None:
         super().__init__()
         self.save_on_focus_out = save_on_focus_out
         self.owner = owner
         self.textChanged.connect(self.text_changed)
         # error_state is true if the code in this editor is invalid.
         self.error_state = False
         self.set_style()
@@ -196,60 +207,61 @@
         self.is_valid = validator
         self.sourceable = sourceable
         self.install_yaml(copy.copy(self.sourceable.source()))
         self.dirty = False
         self._timer = QTimer()
         self._timer.timeout.connect(self.check_valid)
 
-    def setup_error_signal(self, f):
+    def setup_error_signal(self, f: Callable):
         self.sig_error.connect(f)
 
-    def install_text(self, text):
+    def install_text(self, text: str) -> None:
         self.setPlainText(text)
         self.watching_for_changes = True
 
-    def install_yaml(self, y):
+    def install_yaml(self, y: Any) -> None:
         try:
             t = yaml.dump(y, sort_keys=False, Dumper=Dumper)
         except Exception as e:
             print(e)
             t = self.owner._empty_string
         self.install_text(t)
 
-    def set_style(self):
+    def set_style(self) -> None:
         if self.error_state:
             self.setStyleSheet(
-                "QPlainTextEdit {font-family: Source Code Pro, monospace; background-color: rgb(252,227,242);  }"
+                "QPlainTextEdit {font-family: Source Code Pro, monospace; color: black; background-color: rgb(252,227,242);  }"
             )
         else:
             self.setStyleSheet(
-                "QPlainTextEdit {font-family: Source Code Pro, monospace; background-color: white;  }"
+                "QPlainTextEdit {font-family: Source Code Pro, monospace; color: black; background-color: white;  }"
             )
 
-    def set_error_state(self, b):
+    def set_error_state(self, b: bool) -> None:
         if self.error_state != b:
             self.error_state = b
             self.set_style()
 
-    def yaml_source(self):
+    def yaml_source(self) -> Any:
         try:
             t = yaml.safe_load(self.toPlainText())
             self.set_error_state(False)
-            return t
         except Exception as e:
             self.set_error_state(True)
             self.sig_error.emit({"msg": "Source can't be parsed.", "mode": "console"})
+            t = self.owner._empty_string
+        return t
 
     @pyqtSlot()
-    def check_valid(self):
+    def check_valid(self) -> None:
         self.set_error_state(True)
         self.sig_error.emit({"msg": error_message(), "mode": "console"})
 
     @pyqtSlot()
-    def text_changed(self):
+    def text_changed(self) -> None:
         if not self.watching_for_changes:
             return
         self.sourceable.set_clean(False)
         if len(self.toPlainText()) == 0:
             self.setPlainText(self.owner._empty_string)
         v = False
         try:
@@ -261,74 +273,81 @@
             self.set_error_state(not v)
             self.owner.set_dialog_title(True)
         else:
             self._timer.start(2000)
             self.owner.set_dialog_title(False)
         self.dirty = True
 
-    def focusOutEvent(self, event):
+    def focusOutEvent(self, event) -> None:
         if self.save_on_focus_out and self.dirty:
             c = self.yaml_source()
             if c != None:
                 if self.is_valid(c):
                     self.sourceable.save(c)
                     self.set_error_state(False)
                 else:
                     self.set_error_state(True)
             else:
                 self.set_error_state(True)
                 set_error_message("Source can't be parsed.")
             if self.error_state:
                 self.sig_error.emit({"msg": error_message(), "mode": "console"})
 
-    def showEvent(self, event):
+    def showEvent(self, event) -> None:
         self.install_yaml(copy.copy(self.sourceable.source()))
 
-    def refresh(self):
+    def refresh(self) -> None:
         self.install_yaml(copy.copy(self.sourceable.source()))
 
 
 class editorDialog(QDialog):
-    def __init__(self, preferences, sourceable, title, validator, top_structure="dict"):
+    def __init__(
+            self,
+            preferences: ygPreferences,
+            sourceable: ygSourceable,
+            title: str,
+            validator: Callable,
+            top_structure: str = "dict"
+        ) -> None:
         super().__init__()
         self.title = title
         self.set_dialog_title(True)
         self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
         self.preferences = preferences
         self.sourceable = sourceable
         if top_structure == "dict":
             self._empty_string = "{}\n"
         else:
             self._empty_string = "[]\n"
         self.setMinimumSize(500, 500)
-        self.layout = QVBoxLayout()
-        self.setLayout(self.layout)
+        self._layout = QVBoxLayout()
+        self.setLayout(self._layout)
         self.edit_pane = editorPane(self, sourceable, validator)
         self.edit_pane.setup_error_signal(
             self.preferences.top_window().error_manager.new_message
         )
-        self.layout.addWidget(self.edit_pane)
+        self._layout.addWidget(self.edit_pane)
         QBtn = (
             QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
         )
         self.buttonBox = QDialogButtonBox(QBtn)
         self.buttonBox.accepted.connect(self.accept)
         self.buttonBox.rejected.connect(self.reject)
-        self.layout.addWidget(self.buttonBox)
+        self._layout.addWidget(self.buttonBox)
 
-    def set_dialog_title(self, is_valid):
+    def set_dialog_title(self, is_valid: bool) -> None:
         v = " (Invalid)"
         if is_valid:
             v = " (Valid)"
         self.setWindowTitle(self.title + v)
 
-    def reject(self):
+    def reject(self) -> None:
         self.done(QDialog.DialogCode.Rejected)
 
-    def accept(self):
+    def accept(self) -> None:
         err = False
         c = self.edit_pane.yaml_source()
         if c != None:
             if self.edit_pane.is_valid(c):
                 self.sourceable.save(c)
             else:
                 err = True
@@ -337,22 +356,22 @@
         if err:
             self.reject()
             return
         self.done(QDialog.DialogCode.Accepted)
 
 
 class ygGlyphHighlighter(QSyntaxHighlighter):
-    def __init__(self, parent=None):
+    def __init__(self, parent = None) -> None:
         QSyntaxHighlighter.__init__(self, parent)
-        self._mappings = {}
+        self._mappings: dict = {}
 
-    def add_mapping(self, pattern, format):
+    def add_mapping(self, pattern: str, format: QTextCharFormat) -> None:
         self._mappings[pattern] = format
 
-    def highlightBlock(self, text):
+    def highlightBlock(self, text: str) -> None:
         for pattern, format in self._mappings.items():
             matches = re.finditer(pattern, text)
             for match in matches:
                 s = match.group(0)
                 start = match.start()
                 end = match.end()
                 self.setFormat(start, end - start, format)
```

### Comparing `ygt-0.1.2/src/ygt.egg-info/PKG-INFO` & `ygt-0.1.3/src/ygt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: ygt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A graphical hint editor for TrueType fonts
 Author-email: "Peter S. Baker" <b.tarde@mail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ygt
 
 **Ygt** is a Python app for hinting TrueType fonts. It is built to be fast, flexible, and free:
 
 - it will run equally well under Windows, Mac OS, and Linux;
-- it emphasizes modern requirements for TrueType hinting while backgrounding the obsolete;
+- it emphasizes modern requirements for TrueType hinting while deemphasizing the obsolete;
 - the most common commands use unmodified shortcut keys so you can work quickly with one hand on the keyboard and one on the mouse;
 - it will read either a TrueType font or a UFO;
 - it can save hints in an easily understood and edited YAML file,
 - which can be compiled to a hinted font either from inside the program or from the command line,
 - or it can save compiled hints to a UFO (from which fontmake can produce a hinted font)
 
 Ygt is in an alpha state, with features yet to be added (especially auto-hinting). But it is already a workable program, which the developer has used to hint thousands of glyphs in several large fonts.
 
 For the time being, Ygt must be launched from a command line. To install, make sure you are running Python 3.10.4 or later and type `pip install ygt` on the command line. Alternatively, download the files from GitHub, navigate to the directory with the file pyproject.toml, and type `pip install .` (don't forget the period!). Then type `ygt` on the command line to start the program.
 
 For more information, see the [documentation](https://github.com/psb1558/ygt/tree/main/docs) or watch a brief [introductory video](https://psb1558.github.io/ygt/index.html).
+
+## Changes
+
+Version 0.1.23 (2023-4-17) changes three keywords in Ygt’s YAML-based hinting language: `blackspace`, `whitespace`, and `grayspace` become `blackdist`, `whitedist`, and `graydist`. If you have created a hinting file for earlier versions, run this sed script:
+```
+s/blackspace/blackdist/g
+s/whitesapce/whitedist/g
+s/grayspace/graydist/g
+```
+Among other changes intended to improve stability, this version consolidates various font-level edits in a “Font Info” dialog, summoned with Ctrl-I or Cmd-I, and honors “dark themes” on various platforms.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ygt-0.1.2/src/ygt.egg-info/SOURCES.txt` & `ygt-0.1.3/src/ygt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/ygt.py
 src/ygt/__init__.py
 src/ygt/__main__.py
-src/ygt/autohint.py
+src/ygt/autohint_trash.py
 src/ygt/cvGuesser.py
 src/ygt/fontViewDialog.py
 src/ygt/freetypeFont.py
 src/ygt/macfuncDialog.py
 src/ygt/makeCVDialog.py
 src/ygt/window.py
 src/ygt/ygError.py
 src/ygt/ygHintEditor.py
 src/ygt/ygModel.py
 src/ygt/ygPreferences.py
 src/ygt/ygPreview.py
 src/ygt/ygSchema.py
+src/ygt/ygStems.py
 src/ygt/ygYAMLEditor.py
 src/ygt.egg-info/PKG-INFO
 src/ygt.egg-info/SOURCES.txt
 src/ygt.egg-info/dependency_links.txt
 src/ygt.egg-info/entry_points.txt
 src/ygt.egg-info/requires.txt
 src/ygt.egg-info/top_level.txt
+src/ygt/fonts/SourceCodePro-Regular.ttf
 src/ygt/icons/align.png
 src/ygt/icons/anchor.png
 src/ygt/icons/black_distance.png
 src/ygt/icons/cursor-icon-off.png
 src/ygt/icons/cursor-icon-on.png
 src/ygt/icons/cv.png
 src/ygt/icons/cv_guess.png
@@ -38,10 +40,11 @@
 src/ygt/icons/hand-icon-on.png
 src/ygt/icons/horizontal-off.png
 src/ygt/icons/horizontal-on.png
 src/ygt/icons/interpolate.png
 src/ygt/icons/make_set.png
 src/ygt/icons/program.png
 src/ygt/icons/shift.png
+src/ygt/icons/stem_distance.png
 src/ygt/icons/vertical-off.png
 src/ygt/icons/vertical-on.png
 src/ygt/icons/white_distance.png
```

