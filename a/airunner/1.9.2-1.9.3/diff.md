# Comparing `tmp/airunner-1.9.2.tar.gz` & `tmp/airunner-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.2.tar", last modified: Mon Apr 17 23:55:05 2023, max compression
+gzip compressed data, was "airunner-1.9.3.tar", last modified: Tue Apr 18 15:31:43 2023, max compression
```

## Comparing `airunner-1.9.2.tar` & `airunner-1.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 23:54:54.000000 airunner-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:55:05.946614 airunner-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 23:54:54.000000 airunner-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:55:05.946614 airunner-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-17 23:54:54.000000 airunner-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.942614 airunner-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.023322 airunner-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 15:31:28.000000 airunner-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-18 15:31:43.023322 airunner-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-18 15:31:28.000000 airunner-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:31:43.023322 airunner-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-18 15:31:28.000000 airunner-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.019322 airunner-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.019322 airunner-1.9.3/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-18 15:31:29.000000 airunner-1.9.3/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.023322 airunner-1.9.3/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.2/LICENSE` & `airunner-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/PKG-INFO` & `airunner-1.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.2
+Version: 1.9.3
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Banner](banner.png)](https://capsizegames.itch.io/ai-runner)
+[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
 [![Windows Build](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml)
 [![Linux Build](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml)
-[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
+[![PyPi](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml)
 ![GitHub](https://img.shields.io/github/license/Capsize-Games/airunner)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Capsize-Games/airunner)
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
```

### Comparing `airunner-1.9.2/README.md` & `airunner-1.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Banner](banner.png)](https://capsizegames.itch.io/ai-runner)
+[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
 [![Windows Build](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml)
 [![Linux Build](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml)
-[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
+[![PyPi](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml)
 ![GitHub](https://img.shields.io/github/license/Capsize-Games/airunner)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Capsize-Games/airunner)
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
```

### Comparing `airunner-1.9.2/setup.py` & `airunner-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.2",
+    version="1.9.3",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `airunner-1.9.2/src/airunner/balloon.py` & `airunner-1.9.3/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/extensions.py` & `airunner-1.9.3/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/filters.py` & `airunner-1.9.3/src/airunner/filters.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/main.py` & `airunner-1.9.3/src/airunner/main.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/qtcanvas.py` & `airunner-1.9.3/src/airunner/qtcanvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,16 @@
 import io
 import subprocess
-import uuid
-import PIL
 from PIL import Image, ImageOps, ImageDraw, ImageGrab
 from PIL.ImageQt import ImageQt
 from PyQt6.QtCore import Qt, QPoint, QRect, QPointF
 from PyQt6.QtGui import QColor, QPainter, QPen, QBrush, QPixmap, QCursor, QPainterPath, QPolygonF
-
-
-class ImageData:
-    def __init__(self, position: QPoint, image: Image):
-        self.position = position
-        self.image = image
-
-
-class LineData:
-    @property
-    def pen(self):
-        pen = self._pen if self._pen else {
-            "color": "#000000",
-            "width": 1,
-            "style": Qt.PenStyle.SolidLine
-        }
-        return QPen(
-            QColor(pen["color"]),
-            pen["width"],
-            pen["style"]
-        )
-
-    def __init__(self, start_point: QPoint, end_point: QPoint, pen: QPen, layer_index: int):
-        self.start_point = start_point
-        self.end_point = end_point
-        # do not store as a qpen, store as a dict
-        self._pen = {
-            "color": pen.color(),
-            "width": pen.width(),
-            "style": pen.style()
-        }
-        self.layer_index = layer_index
-
-    def intersects(self, start: QPoint, brush_size: int):
-        # check x and use brush size
-        if self.start_point.x() > start.x() - brush_size and self.start_point.x() < start.x() + brush_size:
-            if self.start_point.y() > start.y() - brush_size and self.start_point.y() < start.y() + brush_size:
-                return True
-        return False
-
-
-class LayerData:
-    @property
-    def image(self):
-        if len(self.images) > 0:
-            return self.images[0]
-        return None
-
-    def __init__(
-        self,
-        index: int,
-        name: str,
-        visible: bool = True,
-        opacity: float = 1.0,
-        offset: QPoint = QPoint(0, 0)
-    ):
-        self.index = index
-        self.name = name
-        self.visible = visible
-        self.opacity = opacity
-        self.offset = offset
-        self.lines = []
-        self.images = []
-        self.widgets = []
-        self.uuid = uuid.uuid4()
-
-    def clear(self, index):
-        self.index = index
-        self.lines = []
-        self.images = []
-        self.widgets = []
-        self.visible = True
-        self.opacity = 1.0
-        self.name = f"Layer {self.index + 1}"
-
+from airunner.models.layerdata import LayerData
+from airunner.models.imagedata import ImageData
+from airunner.models.linedata import LineData
 
 class Canvas:
     saving = False
     select_start = None
     select_end = None
 
     @property
```

### Comparing `airunner-1.9.2/src/airunner/runai_client.py` & `airunner-1.9.3/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/settingsmanager.py` & `airunner-1.9.3/src/airunner/settingsmanager.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner/utils.py` & `airunner-1.9.3/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.2/src/airunner.egg-info/PKG-INFO` & `airunner-1.9.3/src/airunner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.2
+Version: 1.9.3
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Banner](banner.png)](https://capsizegames.itch.io/ai-runner)
+[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
 [![Windows Build](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/windows-dispatch.yml)
 [![Linux Build](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/linux-dispatch.yml)
-[![Discord](https://img.shields.io/discord/839511291466219541?color=5865F2&logo=discord&logoColor=white)](https://discord.gg/PUVDDCJ7gz)
+[![PyPi](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml/badge.svg)](https://github.com/Capsize-Games/airunner/actions/workflows/pypi-dispatch.yml)
 ![GitHub](https://img.shields.io/github/license/Capsize-Games/airunner)
 ![GitHub last commit](https://img.shields.io/github/last-commit/Capsize-Games/airunner)
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
```

