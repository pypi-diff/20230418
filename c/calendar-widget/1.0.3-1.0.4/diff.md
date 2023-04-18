# Comparing `tmp/calendar_widget-1.0.3.tar.gz` & `tmp/calendar_widget-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.3.tar", last modified: Tue Apr 18 21:26:51 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.4.tar", last modified: Tue Apr 18 21:43:55 2023, max compression
```

## Comparing `calendar_widget-1.0.3.tar` & `calendar_widget-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0     7606 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6730 2023-04-18 15:04:08.000000 calendar_widget-1.0.3/README.md
--rw-rw-rw-   0        0        0      763 2023-04-18 21:25:17.000000 calendar_widget-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.281569 calendar_widget-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.328447 calendar_widget-1.0.3/src/calendar_widget/
--rw-rw-rw-   0        0        0   127009 2023-04-18 21:22:19.000000 calendar_widget-1.0.3/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.3/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.344073 calendar_widget-1.0.3/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     7606 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 21:26:51.000000 calendar_widget-1.0.3/src/calendar_widget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 21:26:51.359699 calendar_widget-1.0.3/tests/
--rw-rw-rw-   0        0        0      246 2023-04-18 21:21:20.000000 calendar_widget-1.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:43:55.555956 calendar_widget-1.0.4/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0     7499 2023-04-18 21:43:55.555956 calendar_widget-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6625 2023-04-18 21:41:15.000000 calendar_widget-1.0.4/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-18 21:43:01.000000 calendar_widget-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 21:43:55.555956 calendar_widget-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 21:43:55.399694 calendar_widget-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 21:43:55.509077 calendar_widget-1.0.4/src/calendar_widget/
+-rw-rw-rw-   0        0        0   126891 2023-04-18 21:33:29.000000 calendar_widget-1.0.4/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.4/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:43:55.540330 calendar_widget-1.0.4/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0     7499 2023-04-18 21:43:55.000000 calendar_widget-1.0.4/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-18 21:43:55.000000 calendar_widget-1.0.4/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 21:43:55.000000 calendar_widget-1.0.4/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 21:43:55.000000 calendar_widget-1.0.4/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 21:43:55.540330 calendar_widget-1.0.4/tests/
+-rw-rw-rw-   0        0        0      246 2023-04-18 21:21:20.000000 calendar_widget-1.0.4/tests/test.py
```

### Comparing `calendar_widget-1.0.3/LICENSE.md` & `calendar_widget-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.3/PKG-INFO` & `calendar_widget-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar_widget
-Version: 1.0.3
+Version: 1.0.4
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -150,20 +150,18 @@
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
 | pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
 | command= | A function to be called when the widget is clicked. |
-| background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
-| calendar_relief= | Sets the relief of the Calendar widget. |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). Example: background="blue" or background='sky.png' |
 | arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
 | arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months |
 | arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months |
-| date_box_border= | Sets the colour of the border associated with the monthly calendar grid. |
 | date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. |
 | date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. |
 | date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. |
 | arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. |
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
```

### Comparing `calendar_widget-1.0.3/README.md` & `calendar_widget-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,20 +134,18 @@
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
 | pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
 | command= | A function to be called when the widget is clicked. |
-| background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
-| calendar_relief= | Sets the relief of the Calendar widget. |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). Example: background="blue" or background='sky.png' |
 | arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
 | arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months |
 | arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months |
-| date_box_border= | Sets the colour of the border associated with the monthly calendar grid. |
 | date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. |
 | date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. |
 | date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. |
 | arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. |
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
```

### Comparing `calendar_widget-1.0.3/pyproject.toml` & `calendar_widget-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.3/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.4/src/calendar_widget/Calendar_Widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         # function are overridden by the options specified when and instance of the calendar object is created.
         if style == "Dark":
             background = "gray7"                     # colour of the calendar background
             calendar_relief = "flat"                 # relief style options associated with the canvas on which the calendar is created
             arrow_box_border = "gray25"              # colour of the box outline that contains the arrows for selecting previous and following months
             arrow_box_fill = "gray7"                 # colour inside the box that contains the arrows
             arrow_box_width = 1                      # width of the line used to create the box that contains the arrows
-            date_box_border = "gray25"               # colour of the border associated with the monthly calendar grid
             date_box_fill = "gray7"                  # colour inside the boxes that make up the monthly calendar grid
             date_box_width = 2                       # width of the line used to create the grid for the monthly calendar
             self.date_boxes_outline = "gray50"       # colour of the box outline for the boxes that make up the monthly claendar grid
             arrow_outline = "gray25"                 # colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows
             arrow_fill = "black"                     # colour of the calendar arrows
             arrow_thickness = 1                      # thickness of the calendar arrows
             arrow_active = "lime"                    # colour for the activefill associated with the calendar arrows
```

### Comparing `calendar_widget-1.0.3/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.4/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendar-widget
-Version: 1.0.3
+Version: 1.0.4
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -150,20 +150,18 @@
 | options | description |
 | ------- | ----------- |
 | size= | Sets the width of the widget in pixels. The default width is 300px. |
 | pos_x= | Sets the x coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | pos_y= | Sets the y coordinate position of the widget within the window. Note: In tkinter, this is always the top left corner. |
 | style= | Set the style="Dark" for the dark theme. If no styling is specified the Calendar will inherit its default white theme. |
 | command= | A function to be called when the widget is clicked. |
-| background= | Sets the background of the Calendar to a valid tkinter colour. Example: background="blue" |
-| calendar_relief= | Sets the relief of the Calendar widget. |
+| background= | Sets the background of the Calendar to a valid tkinter colour or image (png, gif, ppm, pgm). Example: background="blue" or background='sky.png' |
 | arrow_box_border= | Sets the border colour of the box containing the arrows for selecting previous and following months. |
 | arrow_box_fill= | Sets the background of the box containing the arrows for selecting previous and following months |
 | arrow_box_width= | Sets the line width of the box containing the arrows for selecting previous and following months |
-| date_box_border= | Sets the colour of the border associated with the monthly calendar grid. |
 | date_box_fill= | Sets the colour inside of the boxes that make up the monthly calendar grid. |
 | date_box_width= | Sets the width of the line used to create the grid for the monthly calendar. |
 | date_boxes_outline= | Sets the colour of the box outline for the boxes that make up the monthly claendar grid. |
 | arrow_outline= | Sets the colour for the outline of the polygon (i.e - triangle) that represents the calendar arrows. |
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
```

