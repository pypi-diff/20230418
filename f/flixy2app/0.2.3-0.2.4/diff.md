# Comparing `tmp/flixy2app-0.2.3.tar.gz` & `tmp/flixy2app-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixy2app-0.2.3.tar", last modified: Tue Apr 18 18:31:24 2023, max compression
+gzip compressed data, was "flixy2app-0.2.4.tar", last modified: Tue Apr 18 18:57:37 2023, max compression
```

## Comparing `flixy2app-0.2.3.tar` & `flixy2app-0.2.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.907037 flixy2app-0.2.3/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.2.3/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.2.3/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:31:24.906874 flixy2app-0.2.3/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      399 2023-04-11 20:13:36.000000 flixy2app-0.2.3/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897489 flixy2app-0.2.3/flixy/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897746 flixy2app-0.2.3/flixy/Demo/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Demo/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Demo/demo.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.897960 flixy2app-0.2.3/flixy/Learn/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:44:57.000000 flixy2app-0.2.3/flixy/Learn/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2859 2023-04-10 05:36:37.000000 flixy2app-0.2.3/flixy/Learn/learn.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.899412 flixy2app-0.2.3/flixy/Learn/lessons/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1381 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/Text.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:32:01.000000 flixy2app-0.2.3/flixy/Learn/lessons/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1187 2023-04-10 05:37:44.000000 flixy2app-0.2.3/flixy/Learn/lessons/app.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2235 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1908 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/column.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1755 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/navigate.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3088 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1843 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1598 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/sheet.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2872 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/textfield.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2079 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/Learn/lessons/webview.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.2.3/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.900232 flixy2app-0.2.3/flixy/flixy/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      191 2023-04-18 18:30:17.000000 flixy2app-0.2.3/flixy/flixy/APP.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3137 2023-04-18 16:14:48.000000 flixy2app-0.2.3/flixy/flixy/PAGE.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.901455 flixy2app-0.2.3/flixy/flixy/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/Haptics.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/action.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/convert_rgb_to_hex.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/error_handle.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      448 2023-04-11 20:01:41.000000 flixy2app-0.2.3/flixy/flixy/Tools/expander.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/get_parent.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/sounds.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.901875 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/call_on_change.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/Tools/subscribers/text_subscribe.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      815 2023-04-18 16:12:24.000000 flixy2app-0.2.3/flixy/flixy/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.903959 flixy2app-0.2.3/flixy/flixy/controls/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.2.3/flixy/flixy/controls/APPBAR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.2.3/flixy/flixy/controls/BUTTON.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.2.3/flixy/flixy/controls/COLUMN.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/CONTAINER.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.2.3/flixy/flixy/controls/NAVIGATOR.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.2.3/flixy/flixy/controls/ROW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.2.3/flixy/flixy/controls/SHEET.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1503 2023-04-11 20:11:55.000000 flixy2app-0.2.3/flixy/flixy/controls/SLIDER.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1412 2023-04-11 20:12:23.000000 flixy2app-0.2.3/flixy/flixy/controls/SWITCH.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1741 2023-04-10 14:48:01.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXT.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXTFIELD.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.2.3/flixy/flixy/controls/TEXTVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/WEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/controls/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      759 2023-04-18 16:19:15.000000 flixy2app-0.2.3/flixy/flixy/controls/audio.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/installer.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904416 flixy2app-0.2.3/flixy/flixy/pythonista_ui/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/VIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/WKWEBVIEW.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904680 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/__init__.py
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/gestures.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/update.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.904955 flixy2app-0.2.3/flixy/flixy/widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/flixy/widgets/on_top.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.2.3/flixy/info.txt
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.905696 flixy2app-0.2.3/flixy2app/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.2.3/flixy2app/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.2.3/flixy2app/converter.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.2.3/flixy2app/generate.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:31:24.906615 flixy2app-0.2.3/flixy2app.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1963 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-18 18:31:24.000000 flixy2app-0.2.3/flixy2app.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.2.3/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-18 18:31:24.907088 flixy2app-0.2.3/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      626 2023-04-18 18:31:09.000000 flixy2app-0.2.3/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.814925 flixy2app-0.2.4/
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 flixy2app-0.2.4/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       36 2023-04-10 11:52:11.000000 flixy2app-0.2.4/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:57:37.814777 flixy2app-0.2.4/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      399 2023-04-11 20:13:36.000000 flixy2app-0.2.4/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.804986 flixy2app-0.2.4/flixy/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.805403 flixy2app-0.2.4/flixy/Demo/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       29 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Demo/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      909 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Demo/demo.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.805824 flixy2app-0.2.4/flixy/Learn/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 12:44:57.000000 flixy2app-0.2.4/flixy/Learn/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2859 2023-04-10 05:36:37.000000 flixy2app-0.2.4/flixy/Learn/learn.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.807481 flixy2app-0.2.4/flixy/Learn/lessons/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1381 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/Text.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:32:01.000000 flixy2app-0.2.4/flixy/Learn/lessons/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1187 2023-04-10 05:37:44.000000 flixy2app-0.2.4/flixy/Learn/lessons/app.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2235 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1908 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/column.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1755 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/navigate.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3088 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1843 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1598 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/sheet.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2872 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2079 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/Learn/lessons/webview.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       57 2023-04-10 05:31:19.000000 flixy2app-0.2.4/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.808480 flixy2app-0.2.4/flixy/flixy/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      200 2023-04-18 18:57:13.000000 flixy2app-0.2.4/flixy/flixy/APP.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3137 2023-04-18 16:14:48.000000 flixy2app-0.2.4/flixy/flixy/PAGE.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.809635 flixy2app-0.2.4/flixy/flixy/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1944 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/Haptics.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      149 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/action.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      753 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/convert_rgb_to_hex.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       98 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/error_handle.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      448 2023-04-11 20:01:41.000000 flixy2app-0.2.4/flixy/flixy/Tools/expander.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      242 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/get_parent.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1340 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/sounds.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.810058 flixy2app-0.2.4/flixy/flixy/Tools/subscribers/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:40.000000 flixy2app-0.2.4/flixy/flixy/Tools/subscribers/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      355 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/subscribers/call_on_change.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1534 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/Tools/subscribers/text_subscribe.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      815 2023-04-18 16:12:24.000000 flixy2app-0.2.4/flixy/flixy/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.812233 flixy2app-0.2.4/flixy/flixy/controls/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1470 2023-04-09 22:12:43.000000 flixy2app-0.2.4/flixy/flixy/controls/APPBAR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1942 2023-04-09 21:43:35.000000 flixy2app-0.2.4/flixy/flixy/controls/BUTTON.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2879 2023-04-09 23:13:59.000000 flixy2app-0.2.4/flixy/flixy/controls/COLUMN.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       91 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/controls/CONTAINER.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2221 2023-04-09 23:28:15.000000 flixy2app-0.2.4/flixy/flixy/controls/NAVIGATOR.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2912 2023-04-09 23:11:48.000000 flixy2app-0.2.4/flixy/flixy/controls/ROW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1957 2023-04-09 23:11:34.000000 flixy2app-0.2.4/flixy/flixy/controls/SHEET.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1503 2023-04-11 20:11:55.000000 flixy2app-0.2.4/flixy/flixy/controls/SLIDER.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1412 2023-04-11 20:12:23.000000 flixy2app-0.2.4/flixy/flixy/controls/SWITCH.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1741 2023-04-10 14:48:01.000000 flixy2app-0.2.4/flixy/flixy/controls/TEXT.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3240 2023-04-09 22:54:23.000000 flixy2app-0.2.4/flixy/flixy/controls/TEXTFIELD.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1835 2023-04-09 22:54:56.000000 flixy2app-0.2.4/flixy/flixy/controls/TEXTVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3613 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/controls/WEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/controls/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      759 2023-04-18 16:19:15.000000 flixy2app-0.2.4/flixy/flixy/controls/audio.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8385 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/installer.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.812745 flixy2app-0.2.4/flixy/flixy/pythonista_ui/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1509 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/pythonista_ui/VIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    26900 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/pythonista_ui/WKWEBVIEW.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/pythonista_ui/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.813032 flixy2app-0.2.4/flixy/flixy/pythonista_ui/tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:30:50.000000 flixy2app-0.2.4/flixy/flixy/pythonista_ui/tools/__init__.py
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)    39335 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/pythonista_ui/tools/gestures.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5593 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/update.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.813345 flixy2app-0.2.4/flixy/flixy/widgets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/widgets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      196 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/flixy/widgets/on_top.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      131 2023-04-09 19:33:37.000000 flixy2app-0.2.4/flixy/info.txt
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.813777 flixy2app-0.2.4/flixy2app/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-10 11:59:37.000000 flixy2app-0.2.4/flixy2app/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-10 12:21:28.000000 flixy2app-0.2.4/flixy2app/converter.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      651 2023-04-10 12:23:39.000000 flixy2app-0.2.4/flixy2app/generate.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-18 18:57:37.814559 flixy2app-0.2.4/flixy2app.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      773 2023-04-18 18:57:37.000000 flixy2app-0.2.4/flixy2app.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1963 2023-04-18 18:57:37.000000 flixy2app-0.2.4/flixy2app.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-18 18:57:37.000000 flixy2app-0.2.4/flixy2app.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       26 2023-04-18 18:57:37.000000 flixy2app-0.2.4/flixy2app.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-18 18:57:37.000000 flixy2app-0.2.4/flixy2app.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 flixy2app-0.2.4/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-18 18:57:37.814973 flixy2app-0.2.4/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      626 2023-04-18 18:57:29.000000 flixy2app-0.2.4/setup.py
```

### Comparing `flixy2app-0.2.3/LICENSE` & `flixy2app-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/PKG-INFO` & `flixy2app-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.2.3
+Version: 0.2.4
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.2.3/flixy/Demo/demo.py` & `flixy2app-0.2.4/flixy/Demo/demo.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/learn.py` & `flixy2app-0.2.4/flixy/Learn/learn.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/Text.py` & `flixy2app-0.2.4/flixy/Learn/lessons/Text.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/app.py` & `flixy2app-0.2.4/flixy/Learn/lessons/app.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/button.py` & `flixy2app-0.2.4/flixy/Learn/lessons/button.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/column.py` & `flixy2app-0.2.4/flixy/Learn/lessons/column.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/navigate.py` & `flixy2app-0.2.4/flixy/Learn/lessons/navigate.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/page.py` & `flixy2app-0.2.4/flixy/Learn/lessons/page.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/row.py` & `flixy2app-0.2.4/flixy/Learn/lessons/row.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/sheet.py` & `flixy2app-0.2.4/flixy/Learn/lessons/sheet.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/textfield.py` & `flixy2app-0.2.4/flixy/Learn/lessons/textfield.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/Learn/lessons/webview.py` & `flixy2app-0.2.4/flixy/Learn/lessons/webview.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/PAGE.py` & `flixy2app-0.2.4/flixy/flixy/PAGE.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/Tools/Haptics.py` & `flixy2app-0.2.4/flixy/flixy/Tools/Haptics.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/Tools/convert_rgb_to_hex.py` & `flixy2app-0.2.4/flixy/flixy/Tools/convert_rgb_to_hex.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/Tools/sounds.py` & `flixy2app-0.2.4/flixy/flixy/Tools/sounds.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/Tools/subscribers/text_subscribe.py` & `flixy2app-0.2.4/flixy/flixy/Tools/subscribers/text_subscribe.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/__init__.py` & `flixy2app-0.2.4/flixy/flixy/__init__.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/APPBAR.py` & `flixy2app-0.2.4/flixy/flixy/controls/APPBAR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/BUTTON.py` & `flixy2app-0.2.4/flixy/flixy/controls/BUTTON.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/COLUMN.py` & `flixy2app-0.2.4/flixy/flixy/controls/COLUMN.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/NAVIGATOR.py` & `flixy2app-0.2.4/flixy/flixy/controls/NAVIGATOR.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/ROW.py` & `flixy2app-0.2.4/flixy/flixy/controls/ROW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/SHEET.py` & `flixy2app-0.2.4/flixy/flixy/controls/SHEET.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/SLIDER.py` & `flixy2app-0.2.4/flixy/flixy/controls/SLIDER.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/SWITCH.py` & `flixy2app-0.2.4/flixy/flixy/controls/SWITCH.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/TEXT.py` & `flixy2app-0.2.4/flixy/flixy/controls/TEXT.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/TEXTFIELD.py` & `flixy2app-0.2.4/flixy/flixy/controls/TEXTFIELD.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/TEXTVIEW.py` & `flixy2app-0.2.4/flixy/flixy/controls/TEXTVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/WEBVIEW.py` & `flixy2app-0.2.4/flixy/flixy/controls/WEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/controls/audio.py` & `flixy2app-0.2.4/flixy/flixy/controls/audio.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/installer.py` & `flixy2app-0.2.4/flixy/flixy/installer.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/pythonista_ui/VIEW.py` & `flixy2app-0.2.4/flixy/flixy/pythonista_ui/VIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/pythonista_ui/WKWEBVIEW.py` & `flixy2app-0.2.4/flixy/flixy/pythonista_ui/WKWEBVIEW.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/pythonista_ui/tools/gestures.py` & `flixy2app-0.2.4/flixy/flixy/pythonista_ui/tools/gestures.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy/flixy/update.py` & `flixy2app-0.2.4/flixy/flixy/update.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy2app/converter.py` & `flixy2app-0.2.4/flixy2app/converter.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy2app/generate.py` & `flixy2app-0.2.4/flixy2app/generate.py`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/flixy2app.egg-info/PKG-INFO` & `flixy2app-0.2.4/flixy2app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flixy2app
-Version: 0.2.3
+Version: 0.2.4
 Summary: A UI-Builder that helps programmers build the front-end without codding it.
 Home-page: https://github.com/SKbarbon/flixy
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE
```

### Comparing `flixy2app-0.2.3/flixy2app.egg-info/SOURCES.txt` & `flixy2app-0.2.4/flixy2app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flixy2app-0.2.3/setup.py` & `flixy2app-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='flixy2app',
-    version='0.2.3',
+    version='0.2.4',
     author='SKbarbon',
     description='A UI-Builder that helps programmers build the front-end without codding it.',
     long_description=long_description,
     url='https://github.com/SKbarbon/flixy',
     install_requires=["flet", "requests", "PyInstaller"],
     packages=find_packages(),
     classifiers=[
```

