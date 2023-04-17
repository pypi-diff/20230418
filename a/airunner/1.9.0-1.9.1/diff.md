# Comparing `tmp/airunner-1.9.0.tar.gz` & `tmp/airunner-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.0.tar", last modified: Sat Apr 15 20:46:32 2023, max compression
+gzip compressed data, was "airunner-1.9.1.tar", last modified: Mon Apr 17 23:20:49 2023, max compression
```

## Comparing `airunner-1.9.0.tar` & `airunner-1.9.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 20:46:20.000000 airunner-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-15 20:46:32.199985 airunner-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-15 20:46:20.000000 airunner-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:46:32.199985 airunner-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 20:46:20.000000 airunner-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.195985 airunner-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16605 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    62388 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-15 20:46:20.000000 airunner-1.9.0/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-15 20:46:21.000000 airunner-1.9.0/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:46:32.199985 airunner-1.9.0/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 20:46:32.000000 airunner-1.9.0/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 23:20:37.000000 airunner-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:20:49.084199 airunner-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 23:20:37.000000 airunner-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:20:49.084199 airunner-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-17 23:20:37.000000 airunner-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-17 23:20:38.000000 airunner-1.9.1/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.0/LICENSE` & `airunner-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.0/setup.py` & `airunner-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.0",
+    version="1.9.1",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.9.0",
+        "aihandler==1.9.5",
     ]
 )
```

### Comparing `airunner-1.9.0/src/airunner/extensions.py` & `airunner-1.9.1/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.0/src/airunner/filters.py` & `airunner-1.9.1/src/airunner/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 class SaturationFilter(Filter):
     name = "Saturation"
 
     def __init__(self, factor=1.0):
         self.factor = factor
 
     def filter(self, image):
-        print(image)
         return ImageEnhance.Color(image).enhance(1.0 + self.factor)
 
 
 class FilterBase:
     ui_name = ""
     window_title = ""
```

### Comparing `airunner-1.9.0/src/airunner/main.py` & `airunner-1.9.1/src/airunner/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import requests
 import torch
 from PIL import Image
 from PyQt6 import uic, QtCore, QtGui
 from PyQt6.QtWidgets import QApplication, QLabel, QWidget, QColorDialog, QFileDialog, QVBoxLayout, QDialog, QSpacerItem, \
     QSizePolicy
-from PyQt6.QtCore import QPoint, pyqtSlot, QRect
+from PyQt6.QtCore import QPoint, pyqtSlot, QRect, QPointF
 from PyQt6.QtGui import QPainter, QIcon, QColor, QGuiApplication
 from aihandler.qtvar import TQDMVar, ImageVar, MessageHandlerVar, ErrorHandlerVar
 from aihandler.settings import MAX_SEED, AVAILABLE_SCHEDULERS_BY_ACTION, MODELS, LOG_LEVEL
 from aihandler.util import get_extensions_from_path, import_extension_class
 from airunner.history import History
 from airunner.windows.about import AboutWindow
 from airunner.windows.advanced_settings import AdvancedSettings
@@ -27,14 +27,15 @@
 from airunner.windows.preferences import PreferencesWindow
 from airunner.windows.video import VideoPopup
 from airunner.qtcanvas import Canvas
 from airunner.settingsmanager import SettingsManager
 from airunner.runai_client import OfflineClient
 from airunner.filters import FilterGaussianBlur, FilterBoxBlur, FilterUnsharpMask, FilterSaturation, \
     FilterColorBalance, FilterPixelArt
+from airunner.balloon import Balloon
 import qdarktheme
 
 
 class MainWindow(QApplication):
     progress_bar_started = False
     use_pixels = False
     action = "txt2img"
@@ -53,14 +54,22 @@
     tqdm_callback_triggered = False
     _document_name = "Untitled"
     _is_dirty = False
     is_saved = False
     _embedding_names = []
 
     @property
+    def layer_highlight_style(self):
+        return f"background-color: #c7f6fc; border: 1px solid #000000; color: #000000;"
+
+    @property
+    def layer_normal_style(self):
+        return "background-color: #ffffff; border: 1px solid #333333; color: #333;"
+
+    @property
     def current_index(self):
         return self.window.tabWidget.currentIndex()
 
     @property
     def current_section(self):
         return self.sections[self.current_index]
 
@@ -599,17 +608,17 @@
             # onclick of layer_obj set as the current layer index on self.canvas
             layer_obj.mousePressEvent = lambda event, _layer=layer: self.set_current_layer(
                 self.canvas.layers.index(_layer)
             )
 
             # show a border around layer_obj if it is the selected index
             if self.canvas.current_layer_index == index:
-                layer_obj.frame.setStyleSheet("background-color: #c7f6fc; border: 1px solid #000000;")
+                layer_obj.frame.setStyleSheet(self.layer_highlight_style)
             else:
-                layer_obj.frame.setStyleSheet("background-color: #ffffff; border: 1px solid #333333;")
+                layer_obj.frame.setStyleSheet(self.layer_normal_style)
 
             # enable delete button in layer_obj
             layer_obj.visible_button.setIcon(QIcon("src/icons/eye.png" if layer.visible else "src/icons/eye-off.png"))
             #layer_obj.delete_button.clicked.connect(lambda _, _index=index: self.canvas.delete_layer(_index))
             layer_obj.visible_button.clicked.connect(lambda _, _layer=layer, _layer_obj=layer_obj: self.toggle_layer_visibility(_layer, _layer_obj))
             # layer_obj.up_button.clicked.connect(lambda _, _layer=layer: self.canvas.move_layer_up(_layer))
             # layer_obj.down_button.clicked.connect(lambda _, _layer=layer: self.canvas.move_layer_down(_layer))
@@ -625,20 +634,20 @@
         # change the eye icon of the visible_button on the layer
         self.canvas.toggle_layer_visibility(layer)
         layer_obj.visible_button.setIcon(QIcon("src/icons/eye.png" if layer.visible else "src/icons/eye-off.png"))
 
     def set_current_layer(self, index):
         item = self.container.layout().itemAt(self.canvas.current_layer_index)
         if item:
-            item.widget().frame.setStyleSheet("background-color: #ffffff; border: 1px solid #333333;")
+            item.widget().frame.setStyleSheet(self.layer_normal_style)
         self.canvas.current_layer_index = index
         # green border should only be on the outter frame not all elements
         item = self.container.layout().itemAt(self.canvas.current_layer_index)
         if item:
-            item.widget().frame.setStyleSheet("background-color: #c7f6fc; border: 1px solid #000000;")
+            item.widget().frame.setStyleSheet(self.layer_highlight_style)
 
     def new_document(self):
         self.canvas = Canvas(self)
         self.is_saved = False
         self.is_dirty = False
         self._document_name = "Untitled"
         self.set_window_title()
@@ -760,173 +769,220 @@
             for layer in self.canvas.layers:
                 if layer.uuid == uuid:
                     sorted_layers.append(layer)
                     break
         self.canvas.layers = sorted_layers
 
     def undo_draw(self, previous_event):
-        start_line_index = previous_event["start_line_index"]
-        end_line_index = previous_event["end_line_index"]
-        # delete all lines in range start_line_index to end_line_index
-        previous_event["lines"] = self.canvas.layers[previous_event["layer_index"]].lines[start_line_index:end_line_index]
-        self.history.undone_history.append(previous_event)
-        del self.canvas.layers[previous_event["layer_index"]].lines[start_line_index:end_line_index]
-        self.canvas.update()
+        index = previous_event["layer_index"]
+        lines = previous_event["lines"]
+        previous_event["lines"] = self.canvas.layers[index].lines.copy()
+        self.canvas.layers[index].lines = lines
+        return previous_event
 
     def undo_erase(self, previous_event):
         # add lines to layer
-        lines = self.canvas.layers[previous_event["layer_index"]].lines
-        self.canvas.layers[previous_event["layer_index"]].lines = previous_event["lines"]
-        previous_event["lines"] = lines
-        self.history.undone_history.append(previous_event)
-        self.canvas.update()
+        lines = previous_event["lines"]
+        images = previous_event["images"]
+        index = previous_event["layer_index"]
+        previous_event["lines"] = self.canvas.layers[index].lines
+        previous_event["images"] = self.canvas.get_image_copy(index)
+        self.canvas.layers[index].lines = lines
+        self.canvas.layers[index].images = images
+        return previous_event
 
-    def undo_delete(self, previous_event):
-        # delete layer
-        layer = previous_event["layer"]
-        self.canvas.layers = [l for l in self.canvas.layers if l != layer]
-        self.history.undone_history.append(previous_event)
+    def undo_new_layer(self, previous_event):
+        layers = self.canvas.get_layers_copy()
+        self.canvas.layers = previous_event["layers"]
         self.canvas.current_layer_index = previous_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        previous_event["layers"] = layers
+        return previous_event
 
     def undo_move_layer(self, previous_event):
         layer_order = []
         for layer in self.canvas.layers:
             layer_order.append(layer.uuid)
         self.resort_layers(previous_event)
         previous_event["layer_order"] = layer_order
         self.history.undone_history.append(previous_event)
         self.canvas.current_layer_index = previous_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        return previous_event
 
     def undo_delete_layer(self, previous_event):
-        layers = self.canvas.layers
+        layers = self.canvas.get_layers_copy()
         self.canvas.layers = previous_event["layers"]
-        previous_event["layers"] = layers
-        self.history.undone_history.append(previous_event)
         self.canvas.current_layer_index = previous_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        previous_event["layers"] = layers
+        return previous_event
 
     def undo_set_image(self, previous_event):
         # replace layer images with original images
         images = previous_event["images"]
+        layer_index = previous_event["layer_index"]
         current_image_root_point = QPoint(self.canvas.image_root_point.x(), self.canvas.image_root_point.y())
         current_image_pivot_point = QPoint(self.canvas.image_pivot_point.x(), self.canvas.image_pivot_point.y())
         self.canvas.image_root_point = previous_event["previous_image_root_point"]
         self.canvas.image_pivot_point = previous_event["previous_image_pivot_point"]
-        previous_event["images"] = self.canvas.layers[previous_event["layer_index"]].images
+        previous_event["images"] = self.canvas.get_image_copy(layer_index)
         previous_event["previous_image_root_point"] = current_image_root_point
         previous_event["previous_image_pivot_point"] = current_image_pivot_point
         self.canvas.layers[previous_event["layer_index"]].images = images
-        self.history.undone_history.append(previous_event)
-        self.canvas.update()
+        return previous_event
+
+    def undo_add_widget(self, previous_event):
+        widets = previous_event["widgets"]
+        previous_event["widgets"] = self.canvas.layers[previous_event["layer_index"]].widgets
+        self.canvas.layers[previous_event["layer_index"]].widgets = widets
+        return previous_event
 
     def undo(self):
         if len(self.history.event_history) == 0:
             return
         previous_event = self.history.event_history.pop()
         event_name = previous_event["event"]
         if event_name == "draw":
-            self.undo_draw(previous_event)
+            previous_event = self.undo_draw(previous_event)
         elif event_name == "erase":
-            self.undo_erase(previous_event)
+            previous_event = self.undo_erase(previous_event)
         elif event_name == "new_layer":
-            self.undo_delete(previous_event)
+            if len(self.canvas.layers) == 1:
+                self.history.event_history.append(previous_event)
+                return
+            previous_event = self.undo_new_layer(previous_event)
         elif event_name == "move_layer":
             self.undo_move_layer(previous_event)
         elif event_name == "delete_layer":
             self.undo_delete_layer(previous_event)
         elif event_name == "set_image":
             self.undo_set_image(previous_event)
+        elif event_name == "add_widget":
+            self.undo_add_widget(previous_event)
+        self.history.undone_history.append(previous_event)
+        self.show_layers()
+        self.canvas.update()
 
     def redo_draw(self, undone_event):
         lines = undone_event["lines"]
-        self.canvas.layers[undone_event["layer_index"]].lines.extend(lines)
+        undone_event["lines"] = self.canvas.layers[undone_event["layer_index"]].lines
+        self.canvas.layers[undone_event["layer_index"]].lines = lines
+        return undone_event
 
     def redo_erase(self, undone_event):
-        lines = self.canvas.layers[undone_event["layer_index"]].lines
-        self.canvas.layers[undone_event["layer_index"]].lines = undone_event["lines"]
-        undone_event["lines"] = lines
+        lines = undone_event["lines"]
+        images = undone_event["images"]
+        layer_index = undone_event["layer_index"]
+        undone_event["lines"] = self.canvas.layers[layer_index].lines.copy()
+        undone_event["images"] = self.canvas.get_image_copy(layer_index)
+        self.canvas.layers[undone_event["layer_index"]].lines = lines
+        self.canvas.layers[undone_event["layer_index"]].images = images
+        return undone_event
 
     def redo_new_layer(self, undone_event):
-        self.canvas.layers.insert(0, undone_event["layer"])
+        layers = self.canvas.get_layers_copy()
+        self.canvas.layers = undone_event["layers"]
         self.canvas.current_layer_index = undone_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        undone_event["layers"] = layers
+        return undone_event
 
     def redo_move_layer(self, undone_event):
         layer_order = []
         for layer in self.canvas.layers:
             layer_order.append(layer.uuid)
         self.resort_layers(undone_event)
         undone_event["layer_order"] = layer_order
         self.canvas.current_layer_index = undone_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        return undone_event
 
     def redo_delete_layer(self, undone_event):
-        layers = self.canvas.layers
+        layers = self.canvas.get_layers_copy()
         self.canvas.layers = undone_event["layers"]
-        undone_event["layers"] = layers
         self.canvas.current_layer_index = undone_event["layer_index"]
-        self.canvas.update()
-        self.show_layers()
+        undone_event["layers"] = layers
+        return undone_event
 
     def redo_set_image(self, undone_event):
         layers = self.canvas.layers
         images = undone_event["images"]
+        layer_index = undone_event["layer_index"]
         current_image_root_point = QPoint(self.canvas.image_root_point.x(), self.canvas.image_root_point.y())
         current_image_pivot_point = QPoint(self.canvas.image_pivot_point.x(), self.canvas.image_pivot_point.y())
         self.canvas.image_root_point = undone_event["previous_image_root_point"]
         self.canvas.image_pivot_point = undone_event["previous_image_pivot_point"]
-        undone_event["images"] = layers[undone_event["layer_index"]].images
+        undone_event["images"] = self.canvas.get_image_copy(layer_index)
         undone_event["previous_image_root_point"] = current_image_root_point
         undone_event["previous_image_pivot_point"] = current_image_pivot_point
         self.canvas.layers[undone_event["layer_index"]].images = images
-        self.canvas.update()
+        return undone_event
+
+    def redo_add_widget(self, undone_event):
+        # add widget
+        widgets = undone_event["widgets"]
+        undone_event["widgets"] = self.canvas.layers[undone_event["layer_index"]].widgets
+        self.canvas.layers[undone_event["layer_index"]].widgets = widgets
+        return undone_event
 
     def redo(self):
         if len(self.history.undone_history) == 0:
             return
         undone_event = self.history.undone_history.pop()
         event_name = undone_event["event"]
         if event_name == "draw":
-            self.redo_draw(undone_event)
+            undone_event = self.redo_draw(undone_event)
         elif event_name == "erase":
-            self.redo_erase(undone_event)
+            undone_event = self.redo_erase(undone_event)
         elif event_name == "new_layer":
-            self.redo_new_layer(undone_event)
+            undone_event = self.redo_new_layer(undone_event)
         elif event_name == "move_layer":
-            self.redo_move_layer(undone_event)
+            undone_event = self.redo_move_layer(undone_event)
         elif event_name == "delete_layer":
-            self.redo_delete_layer(undone_event)
+            undone_event = self.redo_delete_layer(undone_event)
         elif event_name == "set_image":
-            self.redo_set_image(undone_event)
-        self.canvas.update()
+            undone_event = self.redo_set_image(undone_event)
+        elif event_name == "add_widget":
+            undone_event = self.redo_add_widget(undone_event)
         self.history.event_history.append(undone_event)
+        self.show_layers()
+        self.canvas.update()
 
     def focus_button_clicked(self):
         self.canvas.recenter()
 
+    def word_balloon_button_clicked(self):
+        """
+        Create and add a word balloon to the canvas.
+        :return:
+        """
+        # create a word balloon
+        word_balloon = Balloon()
+        word_balloon.setGeometry(100, 100, 200, 100)
+        word_balloon.set_tail_pos(QPointF(50, 100))
+        # add the widget to the canvas
+        self.history.add_event({
+            "event": "add_widget",
+            "layer_index": self.canvas.current_layer_index,
+            "widgets": self.canvas.current_layer.widgets.copy(),
+        })
+        self.canvas.current_layer.widgets.append(word_balloon)
+        self.show_layers()
+        self.canvas.update()
+
     def show_initialize_buttons(self):
         self.window.eraser_button.clicked.connect(lambda: self.set_tool("eraser"))
         self.window.brush_button.clicked.connect(lambda: self.set_tool("brush"))
         self.window.active_grid_area_button.clicked.connect(lambda: self.set_tool("active_grid_area"))
         self.window.move_button.clicked.connect(lambda: self.set_tool("move"))
         #self.window.select_button.clicked.connect(lambda: self.set_tool("select"))
         self.window.primary_color_button.clicked.connect(self.set_primary_color)
         self.window.secondary_color_button.clicked.connect(self.set_secondary_color)
         self.window.grid_button.clicked.connect(self.toggle_grid)
         self.window.undo_button.clicked.connect(self.undo)
         self.window.redo_button.clicked.connect(self.redo)
         self.window.nsfw_button.clicked.connect(self.toggle_nsfw_filter)
         self.window.focus_button.clicked.connect(self.focus_button_clicked)
+        self.window.wordballoon_button.clicked.connect(self.word_balloon_button_clicked)
         self.set_button_colors()
         self.window.grid_button.setChecked(
             self.settings_manager.settings.show_grid.get() == True
         )
         self.window.nsfw_button.setChecked(
             self.settings_manager.settings.nsfw_filter.get() == True
         )
@@ -1012,16 +1068,18 @@
         if data["action"] == "txt2vid":
             return self.video_handler(data)
 
         self.stop_progress_bar(data["action"])
         if nsfw_content_detected and self.settings_manager.settings.nsfw_filter.get():
             self.message_handler("NSFW content detected, try again.", error=True)
         else:
+            self.canvas.add_layer()
             self.canvas.image_handler(image, data)
             self.message_handler("")
+            self.show_layers()
 
     def update_canvas_color(self, color):
         self.window.canvas_container.setStyleSheet(f"background-color: {color};")
         self.window.canvas_container.setAutoFillBackground(True)
 
     def initialize_tabs(self):
         # load all the forms
```

### Comparing `airunner-1.9.0/src/airunner/qtcanvas.py` & `airunner-1.9.1/src/airunner/qtcanvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,93 +65,32 @@
         self.index = index
         self.name = name
         self.visible = visible
         self.opacity = opacity
         self.offset = offset
         self.lines = []
         self.images = []
+        self.widgets = []
         self.uuid = uuid.uuid4()
 
     def clear(self, index):
         self.index = index
         self.lines = []
         self.images = []
+        self.widgets = []
         self.visible = True
         self.opacity = 1.0
         self.name = f"Layer {self.index + 1}"
 
 
 class Canvas:
     saving = False
     select_start = None
     select_end = None
 
-    def set_current_layer(self, index):
-        self.current_layer_index = index
-
-    def apply_filter(self):
-        index = 0
-        for image in self.current_layer.images:
-            self.current_layer.images[index].image = image.image.filter(self.parent.current_filter)
-            index += 1
-
-    def delete_layer(self, index):
-        self.parent.history.add_event({
-            "event": "delete_layer",
-            "layers": [layer for layer in self.layers],
-            "layer_index": self.current_layer_index
-        })
-
-        if len(self.layers) == 1:
-            self.layers = [LayerData(0, "Layer 1")]
-        else:
-            try:
-                self.layers.pop(index)
-            except IndexError:
-                pass
-        self.parent.show_layers()
-        self.update()
-
-    def toggle_layer_visibility(self, layer):
-        layer.visible = not layer.visible
-        self.update()
-
-    def track_layer_move_history(self):
-        layer_order = []
-        for layer in self.layers:
-            layer_order.append(layer.uuid)
-        self.parent.history.add_event({
-            "event": "move_layer",
-            "layer_order": layer_order,
-            "layer_index": self.current_layer_index
-        })
-
-    def move_layer_up(self, layer):
-        index = self.layers.index(layer)
-        if index == 0:
-            return
-        # track the current layer order
-        self.track_layer_move_history()
-        self.layers.remove(layer)
-        self.layers.insert(index - 1, layer)
-        self.current_layer_index = index - 1
-        self.parent.show_layers()
-        self.update()
-
-    def move_layer_down(self, layer):
-        index = self.layers.index(layer)
-        if index == len(self.layers) - 1:
-            return
-        self.track_layer_move_history()
-        self.layers.remove(layer)
-        self.layers.insert(index + 1, layer)
-        self.current_layer_index = index + 1
-        self.parent.show_layers()
-        self.update()
-
     @property
     def current_active_image(self):
         try:
             return self.current_layer.images[self.current_layer_index]
         except IndexError:
             return None
 
@@ -218,25 +157,108 @@
     def grid_size(self):
         return self.settings_manager.settings.size.get()
 
     @property
     def mouse_pos(self):
         return self.canvas_container.mapFromGlobal(QCursor.pos())
 
+    @property
+    def active_grid_area_color(self):
+        if self.parent.current_section == "txt2img":
+            brush_color = QColor(0, 255, 0)
+        elif self.parent.current_section == "img2img":
+            brush_color = QColor(255, 0, 0)
+        elif self.parent.current_section == "depth2img":
+            brush_color = QColor(0, 0, 255)
+        elif self.parent.current_section == "pix2pix":
+            brush_color = QColor(255, 255, 0)
+        elif self.parent.current_section == "outpaint":
+            brush_color = QColor(0, 255, 255)
+        elif self.parent.current_section == "superresolution":
+            brush_color = QColor(255, 0, 255)
+        elif self.parent.current_section == "controlnet":
+            brush_color = QColor(255, 255, 255)
+        else:
+            brush_color = QColor(0, 0, 0)
+        return brush_color
+
+    def set_current_layer(self, index):
+        self.current_layer_index = index
+
+    def apply_filter(self):
+        index = 0
+        for image in self.current_layer.images:
+            self.current_layer.images[index].image = image.image.filter(self.parent.current_filter)
+            index += 1
+
+    def get_layers_copy(self):
+        return [layer for layer in self.layers]
+
+    def delete_layer(self, index):
+        self.parent.history.add_event({
+            "event": "delete_layer",
+            "layers": self.get_layers_copy(),
+            "layer_index": self.current_layer_index
+        })
+
+        if len(self.layers) == 1:
+            self.layers = [LayerData(0, "Layer 1")]
+        else:
+            try:
+                self.layers.pop(index)
+            except IndexError:
+                pass
+        self.parent.show_layers()
+        self.update()
+
+    def toggle_layer_visibility(self, layer):
+        layer.visible = not layer.visible
+        self.update()
+
+    def track_layer_move_history(self):
+        layer_order = []
+        for layer in self.layers:
+            layer_order.append(layer.uuid)
+        self.parent.history.add_event({
+            "event": "move_layer",
+            "layer_order": layer_order,
+            "layer_index": self.current_layer_index
+        })
+
+    def move_layer_up(self, layer):
+        index = self.layers.index(layer)
+        if index == 0:
+            return
+        # track the current layer order
+        self.track_layer_move_history()
+        self.layers.remove(layer)
+        self.layers.insert(index - 1, layer)
+        self.current_layer_index = index - 1
+        self.parent.show_layers()
+        self.update()
+
+    def move_layer_down(self, layer):
+        index = self.layers.index(layer)
+        if index == len(self.layers) - 1:
+            return
+        self.track_layer_move_history()
+        self.layers.remove(layer)
+        self.layers.insert(index + 1, layer)
+        self.current_layer_index = index + 1
+        self.parent.show_layers()
+        self.update()
+
     def add_layer(self):
+        self.parent.history.add_event({
+            "event": "new_layer",
+            "layers": self.get_layers_copy(),
+            "layer_index": self.current_layer_index
+        })
         layer_name = f"Layer {len(self.layers) + 1}"
         self.layers.insert(0, LayerData(len(self.layers), layer_name))
-
-        if len(self.layers) > 1:
-            self.parent.history.add_event({
-                "event": "new_layer",
-                "layer": self.layers[0],
-                "layer_index": self.current_layer_index
-            })
-
         self.set_current_layer(0)
 
     def __init__(
         self,
         parent=None
     ):
         self.canvas_rect = QRect(0, 0, 0, 0)
@@ -426,19 +448,28 @@
         # Draw the grid and any lines that have been drawn by the user
         painter = QPainter(self.canvas_container)
 
         # draw grid
         if not self.saving:
             self.draw_grid(painter)
 
-        # draw image
-        self.draw_images(painter)
+        layers = self.layers.copy()
+        layers.reverse()
+        for index in range(len(layers)):
+            layer = layers[index]
+            if not layer.visible:
+                continue
+            # draw image
+            self.draw_images(layer, index, painter)
 
-        # draw user lines
-        self.draw_user_lines(painter)
+            # draw user lines
+            self.draw_user_lines(layer, index, painter)
+
+            # draw widgets
+            self.draw_widgets(layer, index, painter)
 
         self.draw_selection_box(painter)
 
         if not self.saving:
             self.draw_active_grid_area_container(painter)
 
     def enter_event(self, event):
@@ -482,34 +513,14 @@
         # Draw vertical grid lines
         x = start_x
         while x < end_x:
             painter.setPen(self.grid_pen)
             painter.drawLine(x, 0, x, self.canvas_container.height())
             x += self.grid_size
 
-    @property
-    def active_grid_area_color(self):
-        if self.parent.current_section == "txt2img":
-            brush_color = QColor(0, 255, 0)
-        elif self.parent.current_section == "img2img":
-            brush_color = QColor(255, 0, 0)
-        elif self.parent.current_section == "depth2img":
-            brush_color = QColor(0, 0, 255)
-        elif self.parent.current_section == "pix2pix":
-            brush_color = QColor(255, 255, 0)
-        elif self.parent.current_section == "outpaint":
-            brush_color = QColor(0, 255, 255)
-        elif self.parent.current_section == "superresolution":
-            brush_color = QColor(255, 0, 255)
-        elif self.parent.current_section == "controlnet":
-            brush_color = QColor(255, 255, 255)
-        else:
-            brush_color = QColor(0, 0, 0)
-        return brush_color
-
     def draw_active_grid_area_container(self, painter):
         """
         Draw a rectangle around the active grid area of
         """
         painter.setPen(self.grid_pen)
         painter.setBrush(QBrush(QColor(0, 0, 0, 0)))
         pen = QPen(
@@ -529,84 +540,81 @@
         """
         Create a new image object and add it to the current layer
         """
         # convert image to RGBA
         image = image.convert("RGBA")
         self.current_layer.images.append(ImageData(location, image))
 
-    def draw_images(self, painter):
-        index = 0
-        layers = self.layers.copy()
-        layers.reverse()
-        for layer in layers:
-            if not layer.visible:
-                continue
-            for image in layer.images:
-                # display PIL.image as QPixmap
-                img = image.image
-                if self.parent.current_filter and index == self.current_layer_index:
-                    img = img.filter(self.parent.current_filter)
-                qimage = ImageQt(img)
-                pixmap = QPixmap.fromImage(qimage)
-
-                # apply the layer offset
-                x = image.position.x() + self.pos_x
-                y = image.position.y() + self.pos_y
-                location = QPoint(int(x), int(y)) + self.current_layer.offset
+    ######
+    # Drawing functions: render images, widgets and lines to canvas
+    ######
+    def draw_images(self, layer, index, painter):
+        for image in layer.images:
+            # display PIL.image as QPixmap
+            img = image.image
+            if self.parent.current_filter and index == self.current_layer_index:
+                img = img.filter(self.parent.current_filter)
+            qimage = ImageQt(img)
+            pixmap = QPixmap.fromImage(qimage)
+
+            # apply the layer offset
+            x = image.position.x() + self.pos_x
+            y = image.position.y() + self.pos_y
+            location = QPoint(int(x), int(y)) + self.current_layer.offset
+
+            # draw the image
+            painter.drawPixmap(location, pixmap)
+
+    def draw_widgets(self, layer, index, painter):
+        for widget in layer.widgets:
+            widget.draw(painter)
 
-                # draw the image
-                painter.drawPixmap(location, pixmap)
-            index += 1
+    def draw_user_lines(self, layer, index, painter):
+        painter.setBrush(self.brush)
+        for line in layer.lines:
+            pen = line.pen
+            pen.setCapStyle(Qt.PenCapStyle.RoundCap)
+            painter.setPen(pen)
+            start = QPointF(line.start_point.x() + self.pos_x, line.start_point.y() + self.pos_y)
+            end = QPointF(line.end_point.x() + self.pos_x, line.end_point.y() + self.pos_y)
+
+            # also apply the layer offset
+            offset = QPointF(self.current_layer.offset.x(), self.current_layer.offset.y())
+            start += offset
+            end += offset
+
+            # create a QPainterPath to hold the curve
+            path = QPainterPath()
+            path.moveTo(QPointF(start.x(), start.y()))
+
+            # calculate control points for the Bezier curve
+            dx = end.x() - start.x()
+            dy = end.y() - start.y()
+            ctrl1 = QPointF(start.x() + dx / 3, start.y() + dy / 3)
+            ctrl2 = QPointF(end.x() - dx / 3, end.y() - dy / 3)
+
+            # add the curve to the path
+            path.cubicTo(ctrl1, ctrl2, end)
+
+            # create a QPolygonF from the path to draw the curve
+            polygons = path.toSubpathPolygons()
+            if len(polygons) > 0:
+                curve = QPolygonF(polygons[0])
+                painter.drawPolyline(curve)
+    ######
+    # End Drawing functions
+    ######
 
     def invert_image(self):
         # convert image mode to RGBA
         for image in self.current_layer.images:
             image.image = image.image.convert("RGB")
             image.image = ImageOps.invert(image.image)
             image.image = image.image.convert("RGBA")
 
-    def draw_user_lines(self, painter):
-        painter.setBrush(self.brush)
-        layers = self.layers.copy()
-        layers.reverse()
-        for layer in layers:
-            if not layer.visible:
-                continue
-            for line in layer.lines:
-                pen = line.pen
-                pen.setCapStyle(Qt.PenCapStyle.RoundCap)
-                painter.setPen(pen)
-                start = QPointF(line.start_point.x() + self.pos_x, line.start_point.y() + self.pos_y)
-                end = QPointF(line.end_point.x() + self.pos_x, line.end_point.y() + self.pos_y)
-
-                # also apply the layer offset
-                offset = QPointF(self.current_layer.offset.x(), self.current_layer.offset.y())
-                start += offset
-                end += offset
-
-                # create a QPainterPath to hold the curve
-                path = QPainterPath()
-                path.moveTo(QPointF(start.x(), start.y()))
-
-                # calculate control points for the Bezier curve
-                dx = end.x() - start.x()
-                dy = end.y() - start.y()
-                ctrl1 = QPointF(start.x() + dx / 3, start.y() + dy / 3)
-                ctrl2 = QPointF(end.x() - dx / 3, end.y() - dy / 3)
-
-                # add the curve to the path
-                path.cubicTo(ctrl1, ctrl2, end)
-
-                # create a QPolygonF from the path to draw the curve
-                polygons = path.toSubpathPolygons()
-                if len(polygons) > 0:
-                    curve = QPolygonF(polygons[0])
-                    painter.drawPolyline(curve)
-        # convert to QImage and combine with self.current_layer.image
-
     def draw_selection_box(self, painter):
         if self.select_start is not None and self.select_end is not None:
             # the rectangle should have a dashed line border
             painter.setPen(QPen(Qt.GlobalColor.red, 1))
             painter.setBrush(Qt.GlobalColor.transparent)
             painter.drawRect(QRect(self.select_start, self.select_end))
 
@@ -634,27 +642,21 @@
 
     def recenter(self):
         self.pos_x = 0
         self.pos_y = 0
         self.update()
 
     def handle_erase(self, event):
+        self.is_erasing = True
         # Erase any line segments that intersect with the current position of the mouse
         brush_size = self.settings_manager.settings.mask_brush_size.get()
         start = event.pos() - QPoint(self.pos_x, self.pos_y) - self.image_pivot_point
         for i, line in enumerate(self.current_layer.lines):
             # check if line intersects with start using brush size radius
             if line.intersects(start, brush_size):
-                if not self.is_erasing:
-                    self.is_erasing = True
-                    self.parent.history.add_event({
-                        "event": "erase",
-                        "layer_index": self.current_layer_index,
-                        "lines": self.current_layer.lines.copy()
-                    })
                 self.current_layer.lines.pop(i)
                 self.update()
 
         # erase pixels from image
         if len(self.current_layer.images) > 0:
             image = self.current_layer.images[0].image
             if image:
@@ -796,14 +798,19 @@
         self.layers[self.current_layer_index].offset = point
 
     def mouse_press_event(self, event):
         if event.button() == Qt.MouseButton.LeftButton:
             self.select_start = event.pos()
         if event.button() in (Qt.MouseButton.LeftButton, Qt.MouseButton.RightButton):
             if self.brush_selected:
+                self.parent.history.add_event({
+                    "event": "draw",
+                    "layer_index": self.current_layer_index,
+                    "lines": self.current_layer.lines.copy()
+                })
                 self.start_drawing_line_index = len(self.current_layer.lines)
                 start = event.pos() - QPoint(self.pos_x, self.pos_y)
                 end = event.pos() - QPoint(self.pos_x, self.pos_y)
                 pen = self.pen(event)
                 line = LineData(start, end, pen, self.current_layer_index)
                 start += self.layers[self.current_layer_index].offset
                 end += self.layers[self.current_layer_index].offset
@@ -835,16 +842,26 @@
             self.select_start.setX(self.select_start.x() - (self.select_start.x() % grid_size))
             self.select_start.setY(self.select_start.y() - (self.select_start.y() % grid_size))
             self.select_end.setX(self.select_end.x() - (self.select_end.x() % grid_size))
             self.select_end.setY(self.select_end.y() - (self.select_end.y() % grid_size))
 
         self.update()
 
+    def get_image_copy(self, index):
+        return [ImageData(imageData.position, imageData.image.copy()) for imageData in self.layers[index].images]
+
     def handle_tool(self, event):
         if self.eraser_selected:
+            if not self.is_erasing:
+                self.parent.history.add_event({
+                    "event": "erase",
+                    "layer_index": self.current_layer_index,
+                    "lines": self.current_layer.lines.copy(),
+                    "images": self.get_image_copy(self.current_layer_index)
+                })
             self.handle_erase(event)
             self.parent.is_dirty = True
         elif self.brush_selected:
             self.handle_draw(event)
             self.parent.is_dirty = True
         elif self.move_selected:
             self.handle_move_layer(event)
@@ -880,19 +897,13 @@
         # trigger draw event
         self.update()
 
     def mouse_release_event(self, event):
         if event.button() in (Qt.MouseButton.LeftButton, Qt.MouseButton.RightButton):
             if self.brush_selected:
                 self.stop_drawing_line_index = len(self.current_layer.lines)
-                self.parent.history.add_event({
-                    "event": "draw",
-                    "layer_index": self.current_layer_index,
-                    "start_line_index": self.start_drawing_line_index,
-                    "end_line_index": self.stop_drawing_line_index
-                })
                 self.update()
             elif self.eraser_selected:
-                is_erasing = False
+                self.is_erasing = False
         elif event.button() == Qt.MouseButton.MiddleButton:
             # Start dragging the canvas when the middle or right mouse button is pressed
             self.drag_pos = event.pos()
```

### Comparing `airunner-1.9.0/src/airunner/runai_client.py` & `airunner-1.9.1/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.0/src/airunner/settingsmanager.py` & `airunner-1.9.1/src/airunner/settingsmanager.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.0/src/airunner/utils.py` & `airunner-1.9.1/src/airunner/utils.py`

 * *Files identical despite different names*

