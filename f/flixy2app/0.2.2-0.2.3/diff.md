# Comparing `tmp/flixy2app-0.2.2.tar.gz` & `tmp/flixy2app-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixy2app-0.2.2.tar", last modified: Tue Apr 11 20:14:51 2023, max compression
+gzip compressed data, was "flixy2app-0.2.3.tar", last modified: Tue Apr 18 18:31:24 2023, max compression
```

## Comparing `flixy2app-0.2.2.tar` & `flixy2app-0.2.3.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.070604 flixy2app-0.2.2/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.2.2/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.2.2/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-11 20:14:51.070414 flixy2app-0.2.2/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      399 2023-04-11 20:13:36.000000 flixy2app-0.2.2/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.061596 flixy2app-0.2.2/flixy/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.061940 flixy2app-0.2.2/flixy/Demo/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Demo/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Demo/demo.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.062213 flixy2app-0.2.2/flixy/Learn/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:44:57.000000 flixy2app-0.2.2/flixy/Learn/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2859 2023-04-10 05:36:37.000000 flixy2app-0.2.2/flixy/Learn/learn.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.063697 flixy2app-0.2.2/flixy/Learn/lessons/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1381 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/Text.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:32:01.000000 flixy2app-0.2.2/flixy/Learn/lessons/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1187 2023-04-10 05:37:44.000000 flixy2app-0.2.2/flixy/Learn/lessons/app.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2235 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1908 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/column.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1755 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/navigate.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3088 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1843 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1598 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/sheet.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2872 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/textfield.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2079 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/Learn/lessons/webview.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.2.2/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.064363 flixy2app-0.2.2/flixy/flixy/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      161 2023-04-09 19:45:54.000000 flixy2app-0.2.2/flixy/flixy/APP.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3026 2023-04-11 20:05:48.000000 flixy2app-0.2.2/flixy/flixy/PAGE.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.065507 flixy2app-0.2.2/flixy/flixy/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/Haptics.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/action.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/convert_rgb_to_hex.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/error_handle.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      448 2023-04-11 20:01:41.000000 flixy2app-0.2.2/flixy/flixy/Tools/expander.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/get_parent.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/sounds.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.065874 flixy2app-0.2.2/flixy/flixy/Tools/subscribers/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.2.2/flixy/flixy/Tools/subscribers/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/subscribers/call_on_change.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/Tools/subscribers/text_subscribe.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      781 2023-04-11 20:08:49.000000 flixy2app-0.2.2/flixy/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.067650 flixy2app-0.2.2/flixy/flixy/controls/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.2.2/flixy/flixy/controls/APPBAR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.2.2/flixy/flixy/controls/BUTTON.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.2.2/flixy/flixy/controls/COLUMN.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/controls/CONTAINER.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.2.2/flixy/flixy/controls/NAVIGATOR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.2.2/flixy/flixy/controls/ROW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.2.2/flixy/flixy/controls/SHEET.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1503 2023-04-11 20:11:55.000000 flixy2app-0.2.2/flixy/flixy/controls/SLIDER.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1412 2023-04-11 20:12:23.000000 flixy2app-0.2.2/flixy/flixy/controls/SWITCH.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1741 2023-04-10 14:48:01.000000 flixy2app-0.2.2/flixy/flixy/controls/TEXT.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.2.2/flixy/flixy/controls/TEXTFIELD.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.2.2/flixy/flixy/controls/TEXTVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/controls/WEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/controls/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/installer.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.068025 flixy2app-0.2.2/flixy/flixy/pythonista_ui/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/pythonista_ui/VIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/pythonista_ui/WKWEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/pythonista_ui/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.068281 flixy2app-0.2.2/flixy/flixy/pythonista_ui/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.2.2/flixy/flixy/pythonista_ui/tools/__init__.py
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/pythonista_ui/tools/gestures.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/update.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.068572 flixy2app-0.2.2/flixy/flixy/widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/flixy/widgets/on_top.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.2.2/flixy/info.txt
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.068994 flixy2app-0.2.2/flixy2app/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.2.2/flixy2app/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.2.2/flixy2app/converter.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.2.2/flixy2app/generate.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-11 20:14:51.069805 flixy2app-0.2.2/flixy2app.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-11 20:14:51.000000 flixy2app-0.2.2/flixy2app.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1933 2023-04-11 20:14:51.000000 flixy2app-0.2.2/flixy2app.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-11 20:14:51.000000 flixy2app-0.2.2/flixy2app.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-11 20:14:51.000000 flixy2app-0.2.2/flixy2app.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-11 20:14:51.000000 flixy2app-0.2.2/flixy2app.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.2.2/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-11 20:14:51.070658 flixy2app-0.2.2/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      626 2023-04-11 20:14:35.000000 flixy2app-0.2.2/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.907037 flixy2app-0.2.3/
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.2.3/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.2.3/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:31:24.906874 flixy2app-0.2.3/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      399 2023-04-11 20:13:36.000000 flixy2app-0.2.3/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897489 flixy2app-0.2.3/flixy/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897746 flixy2app-0.2.3/flixy/Demo/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Demo/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Demo/demo.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897960 flixy2app-0.2.3/flixy/Learn/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:44:57.000000 flixy2app-0.2.3/flixy/Learn/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2859 2023-04-10 05:36:37.000000 flixy2app-0.2.3/flixy/Learn/learn.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.899412 flixy2app-0.2.3/flixy/Learn/lessons/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1381 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/Text.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:32:01.000000 flixy2app-0.2.3/flixy/Learn/lessons/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1187 2023-04-10 05:37:44.000000 flixy2app-0.2.3/flixy/Learn/lessons/app.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2235 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1908 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/column.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1755 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/navigate.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3088 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1843 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1598 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/sheet.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2872 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2079 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/webview.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.2.3/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.900232 flixy2app-0.2.3/flixy/flixy/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      191 2023-04-18 18:30:17.000000 flixy2app-0.2.3/flixy/flixy/APP.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3137 2023-04-18 16:14:48.000000 flixy2app-0.2.3/flixy/flixy/PAGE.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.901455 flixy2app-0.2.3/flixy/flixy/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/Haptics.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/action.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/convert_rgb_to_hex.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/error_handle.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      448 2023-04-11 20:01:41.000000 flixy2app-0.2.3/flixy/flixy/Tools/expander.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/get_parent.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/sounds.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.901875 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/call_on_change.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/text_subscribe.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      815 2023-04-18 16:12:24.000000 flixy2app-0.2.3/flixy/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.903959 flixy2app-0.2.3/flixy/flixy/controls/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.2.3/flixy/flixy/controls/APPBAR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.2.3/flixy/flixy/controls/BUTTON.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.2.3/flixy/flixy/controls/COLUMN.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/CONTAINER.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.2.3/flixy/flixy/controls/NAVIGATOR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.2.3/flixy/flixy/controls/ROW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.2.3/flixy/flixy/controls/SHEET.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1503 2023-04-11 20:11:55.000000 flixy2app-0.2.3/flixy/flixy/controls/SLIDER.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1412 2023-04-11 20:12:23.000000 flixy2app-0.2.3/flixy/flixy/controls/SWITCH.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1741 2023-04-10 14:48:01.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXT.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXTFIELD.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXTVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/WEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      759 2023-04-18 16:19:15.000000 flixy2app-0.2.3/flixy/flixy/controls/audio.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/installer.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904416 flixy2app-0.2.3/flixy/flixy/pythonista_ui/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/VIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/WKWEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904680 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/__init__.py
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/gestures.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/update.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904955 flixy2app-0.2.3/flixy/flixy/widgets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/widgets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/widgets/on_top.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/info.txt
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.905696 flixy2app-0.2.3/flixy2app/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.2.3/flixy2app/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.2.3/flixy2app/converter.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.2.3/flixy2app/generate.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.906615 flixy2app-0.2.3/flixy2app.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1963 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.2.3/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-18 18:31:24.907088 flixy2app-0.2.3/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      626 2023-04-18 18:31:09.000000 flixy2app-0.2.3/setup.py
```

### Comparing `flixy2app-0.2.2/LICENSE` & `flixy2app-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/PKG-INFO` & `flixy2app-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.2.2
+Version: 0.2.3
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.2.2/flixy/Demo/demo.py` & `flixy2app-0.2.3/flixy/Demo/demo.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/learn.py` & `flixy2app-0.2.3/flixy/Learn/learn.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/Text.py` & `flixy2app-0.2.3/flixy/Learn/lessons/Text.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/app.py` & `flixy2app-0.2.3/flixy/Learn/lessons/app.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/button.py` & `flixy2app-0.2.3/flixy/Learn/lessons/button.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/column.py` & `flixy2app-0.2.3/flixy/Learn/lessons/column.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/navigate.py` & `flixy2app-0.2.3/flixy/Learn/lessons/navigate.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/page.py` & `flixy2app-0.2.3/flixy/Learn/lessons/page.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/row.py` & `flixy2app-0.2.3/flixy/Learn/lessons/row.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/sheet.py` & `flixy2app-0.2.3/flixy/Learn/lessons/sheet.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/textfield.py` & `flixy2app-0.2.3/flixy/Learn/lessons/textfield.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/Learn/lessons/webview.py` & `flixy2app-0.2.3/flixy/Learn/lessons/webview.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/PAGE.py` & `flixy2app-0.2.3/flixy/flixy/PAGE.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class Page (object):
 	def __init__ (self, run_as="app"):
 		self.__ui_view = None
 		self.__is_on_screen = True
 		
 		self.controls = []
+		self.overlay = []
 		self.bgcolor = "black"
 		self.title = ""
 		self.__appbar = None
 		self.font_family = "Avenir"
 		self.width = 0
 		self.height = 0
 		self.spacing = 15
@@ -50,14 +51,18 @@
 		flixy_control.respown(self, self)
 		flet_control = flixy_control.self_ui
 		self.controls.append(flixy_control)
 		cont = flet.Row([flet_control], alignment="center")
 		self.self_ui.add(cont)
 
 		self.update()
+	
+	def add_overlay (self, control):
+		self.overlay.append(control)
+		control.respown(self)
 		
 	
 	def clear (self):
 		self.controls = []
 		self.self_ui.clean()
 		self.update()
```

### Comparing `flixy2app-0.2.2/flixy/flixy/Tools/Haptics.py` & `flixy2app-0.2.3/flixy/flixy/Tools/Haptics.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/Tools/convert_rgb_to_hex.py` & `flixy2app-0.2.3/flixy/flixy/Tools/convert_rgb_to_hex.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/Tools/sounds.py` & `flixy2app-0.2.3/flixy/flixy/Tools/sounds.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/Tools/subscribers/text_subscribe.py` & `flixy2app-0.2.3/flixy/flixy/Tools/subscribers/text_subscribe.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/__init__.py` & `flixy2app-0.2.3/flixy/flixy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 from .controls.TEXTVIEW import TextView
 # from .controls.WEBVIEW import WebView
 from .controls.TEXTFIELD import TextField
 from .controls.NAVIGATOR import Navigate
 from .controls.SHEET import Sheet
 from .controls.SWITCH import Switch
 from .controls.SLIDER import Slider
+from .controls.audio import Audio
 
 # from .Tools.subscribers.text_subscribe import textSubscribe
 # from .Tools.subscribers.call_on_change import callOnChange
 # from .Tools.Haptics import selectionChanged, impactOccured, notificationOccured, vibrate, single_haptic, impact_haptic, warning_haptic
 # from .Tools.sounds import Sound
```

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/APPBAR.py` & `flixy2app-0.2.3/flixy/flixy/controls/APPBAR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/BUTTON.py` & `flixy2app-0.2.3/flixy/flixy/controls/BUTTON.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/COLUMN.py` & `flixy2app-0.2.3/flixy/flixy/controls/COLUMN.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/NAVIGATOR.py` & `flixy2app-0.2.3/flixy/flixy/controls/NAVIGATOR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/ROW.py` & `flixy2app-0.2.3/flixy/flixy/controls/ROW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/SHEET.py` & `flixy2app-0.2.3/flixy/flixy/controls/SHEET.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/SLIDER.py` & `flixy2app-0.2.3/flixy/flixy/controls/SLIDER.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/SWITCH.py` & `flixy2app-0.2.3/flixy/flixy/controls/SWITCH.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/TEXT.py` & `flixy2app-0.2.3/flixy/flixy/controls/TEXT.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/TEXTFIELD.py` & `flixy2app-0.2.3/flixy/flixy/controls/TEXTFIELD.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/TEXTVIEW.py` & `flixy2app-0.2.3/flixy/flixy/controls/TEXTVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/controls/WEBVIEW.py` & `flixy2app-0.2.3/flixy/flixy/controls/WEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/installer.py` & `flixy2app-0.2.3/flixy/flixy/installer.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/pythonista_ui/VIEW.py` & `flixy2app-0.2.3/flixy/flixy/pythonista_ui/VIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/pythonista_ui/WKWEBVIEW.py` & `flixy2app-0.2.3/flixy/flixy/pythonista_ui/WKWEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/pythonista_ui/tools/gestures.py` & `flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/gestures.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy/flixy/update.py` & `flixy2app-0.2.3/flixy/flixy/update.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy2app/converter.py` & `flixy2app-0.2.3/flixy2app/converter.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy2app/generate.py` & `flixy2app-0.2.3/flixy2app/generate.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.2/flixy2app.egg-info/PKG-INFO` & `flixy2app-0.2.3/flixy2app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.2.2
+Version: 0.2.3
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.2.2/flixy2app.egg-info/SOURCES.txt` & `flixy2app-0.2.3/flixy2app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 flixy/flixy/controls/SLIDER.py
 flixy/flixy/controls/SWITCH.py
 flixy/flixy/controls/TEXT.py
 flixy/flixy/controls/TEXTFIELD.py
 flixy/flixy/controls/TEXTVIEW.py
 flixy/flixy/controls/WEBVIEW.py
 flixy/flixy/controls/__init__.py
+flixy/flixy/controls/audio.py
 flixy/flixy/pythonista_ui/VIEW.py
 flixy/flixy/pythonista_ui/WKWEBVIEW.py
 flixy/flixy/pythonista_ui/__init__.py
 flixy/flixy/pythonista_ui/tools/__init__.py
 flixy/flixy/pythonista_ui/tools/gestures.py
 flixy/flixy/widgets/__init__.py
 flixy/flixy/widgets/on_top.py
```

### Comparing `flixy2app-0.2.2/setup.py` & `flixy2app-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='flixy2app',
-    version='0.2.2',
+    version='0.2.3',
     author='SKbarbon',
     description='A UI-Builder that helps programmers build the front-end without codding it.',
     long_description=long_description,
     url='https://github.com/SKbarbon/flixy',
     install_requires=["flet", "requests", "PyInstaller"],
     packages=find_packages(),
     classifiers=[
```

