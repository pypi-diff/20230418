# Comparing `tmp/calendar_widget-1.0.2.tar.gz` & `tmp/calendar_widget-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.2.tar", last modified: Mon Apr 17 00:57:39 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.3.tar", last modified: Tue Apr 18 21:26:51 2023, max compression
```

## Comparing `calendar_widget-1.0.2.tar` & `calendar_widget-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     7068 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6215 2023-04-17 00:49:26.000000 calendar_widget-1.0.2/README.md
--rw-rw-rw-   0        0        0      763 2023-04-17 00:56:24.000000 calendar_widget-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 00:57:39.949842 calendar_widget-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.793580 calendar_widget-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.856085 calendar_widget-1.0.2/src/calendar_widget/
--rw-rw-rw-   0        0        0    32475 2023-04-17 00:56:16.000000 calendar_widget-1.0.2/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.2/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 00:57:39.934221 calendar_widget-1.0.2/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     7068 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-17 00:57:39.000000 calendar_widget-1.0.2/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     7606 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6730 2023-04-18 15:04:08.000000 calendar_widget-1.0.3/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-18 21:25:17.000000 calendar_widget-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.281569 calendar_widget-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.328447 calendar_widget-1.0.3/src/calendar_widget/
+-rw-rw-rw-   0        0        0   127009 2023-04-18 21:22:19.000000 calendar_widget-1.0.3/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.3/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.344073 calendar_widget-1.0.3/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0     7606 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/tests/
+-rw-rw-rw-   0        0        0      246 2023-04-18 21:21:20.000000 calendar_widget-1.0.3/tests/test.py
```

### Comparing `calendar_widget-1.0.2/LICENSE.md` & `calendar_widget-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.2/PKG-INFO` & `calendar_widget-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar_widget
-Version: 1.0.2
+Version: 1.0.3
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -116,14 +116,37 @@
 root.mainloop()
 ```
 
 Note: if no 'pos_x' or 'pos_y' parameters are given, the Calendar widget will default to using the standard pack function.
 
 -----
 
+## Example 2 - Binding a command to the calendar
+
+-----
+
+```
+# the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
+def Calendar_Click():
+	print(Calendar.getdate())
+
+# create the calendar widget
+Calendar = Calendar(root,
+	size = 250,
+	pos_x = 0,
+	pos_y = 0, 
+	background = 'lightblue', 
+	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
+	)
+```
+
+Note: Only a single command can be linked to the calendar widget.
+
+-----
+
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
```

### Comparing `calendar_widget-1.0.2/README.md` & `calendar_widget-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,37 @@
 root.mainloop()
 ```
 
 Note: if no 'pos_x' or 'pos_y' parameters are given, the Calendar widget will default to using the standard pack function.
 
 -----
 
+## Example 2 - Binding a command to the calendar
+
+-----
+
+```
+# the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
+def Calendar_Click():
+	print(Calendar.getdate())
+
+# create the calendar widget
+Calendar = Calendar(root,
+	size = 250,
+	pos_x = 0,
+	pos_y = 0, 
+	background = 'lightblue', 
+	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
+	)
+```
+
+Note: Only a single command can be linked to the calendar widget.
+
+-----
+
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
```

### Comparing `calendar_widget-1.0.2/pyproject.toml` & `calendar_widget-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.2/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.3/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-widget
-Version: 1.0.2
+Version: 1.0.3
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -116,14 +116,37 @@
 root.mainloop()
 ```
 
 Note: if no 'pos_x' or 'pos_y' parameters are given, the Calendar widget will default to using the standard pack function.
 
 -----
 
+## Example 2 - Binding a command to the calendar
+
+-----
+
+```
+# the 'Calendar_Click' function retrives the date selected on the Calendar by the user, and prints the date to the console
+def Calendar_Click():
+	print(Calendar.getdate())
+
+# create the calendar widget
+Calendar = Calendar(root,
+	size = 250,
+	pos_x = 0,
+	pos_y = 0, 
+	background = 'lightblue', 
+	command = Calendar_Click  # link the 'Calendar_Click' function to the widget
+	)
+```
+
+Note: Only a single command can be linked to the calendar widget.
+
+-----
+
 # Widget Parameters - functionality and styling
 
 The table below specifies opitons availiable for styling and other operations associated with the calendar widget
 
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
```

