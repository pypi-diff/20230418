# Comparing `tmp/xflib-0.1.10.tar.gz` & `tmp/xflib-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflib-0.1.10.tar", last modified: Sun Apr 16 23:16:30 2023, max compression
+gzip compressed data, was "xflib-0.1.11.tar", last modified: Tue Apr 18 17:45:03 2023, max compression
```

## Comparing `xflib-0.1.10.tar` & `xflib-0.1.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-16 23:16:30.807289 xflib-0.1.10/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1062 2023-03-29 22:02:05.000000 xflib-0.1.10/LICENSE
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      426 2023-04-16 23:16:30.807158 xflib-0.1.10/PKG-INFO
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      137 2023-04-02 13:17:47.000000 xflib-0.1.10/README.md
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       38 2023-04-16 23:16:30.807337 xflib-0.1.10/setup.cfg
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      606 2023-04-16 23:01:35.000000 xflib-0.1.10/setup.py
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-16 23:16:30.804938 xflib-0.1.10/src/
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-16 23:16:30.806309 xflib-0.1.10/src/xflib/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       58 2023-04-16 23:12:35.000000 xflib-0.1.10/src/xflib/__init__.py
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     9946 2023-04-16 23:16:01.000000 xflib-0.1.10/src/xflib/ps.py
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-16 21:57:03.000000 xflib-0.1.10/src/xflib/ui.py
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1311 2023-04-16 23:15:50.000000 xflib-0.1.10/src/xflib/utils.py
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-16 23:16:30.806967 xflib-0.1.10/src/xflib.egg-info/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      426 2023-04-16 23:16:30.000000 xflib-0.1.10/src/xflib.egg-info/PKG-INFO
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      263 2023-04-16 23:16:30.000000 xflib-0.1.10/src/xflib.egg-info/SOURCES.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        1 2023-04-16 23:16:30.000000 xflib-0.1.10/src/xflib.egg-info/dependency_links.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       10 2023-04-16 23:16:30.000000 xflib-0.1.10/src/xflib.egg-info/requires.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        6 2023-04-16 23:16:30.000000 xflib-0.1.10/src/xflib.egg-info/top_level.txt
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-18 17:45:03.476393 xflib-0.1.11/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1062 2023-04-18 12:40:11.000000 xflib-0.1.11/LICENSE
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      426 2023-04-18 17:45:03.476257 xflib-0.1.11/PKG-INFO
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     3825 2023-04-18 14:25:49.000000 xflib-0.1.11/README.md
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       38 2023-04-18 17:45:03.476435 xflib-0.1.11/setup.cfg
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      606 2023-04-18 17:44:38.000000 xflib-0.1.11/setup.py
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-18 17:45:03.473802 xflib-0.1.11/src/
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-18 17:45:03.475264 xflib-0.1.11/src/xflib/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       58 2023-04-18 12:40:11.000000 xflib-0.1.11/src/xflib/__init__.py
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)    10038 2023-04-18 17:42:31.000000 xflib-0.1.11/src/xflib/ps.py
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     7727 2023-04-18 17:38:21.000000 xflib-0.1.11/src/xflib/ui.py
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     2243 2023-04-18 12:54:30.000000 xflib-0.1.11/src/xflib/utils.py
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-18 17:45:03.476073 xflib-0.1.11/src/xflib.egg-info/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      426 2023-04-18 17:45:03.000000 xflib-0.1.11/src/xflib.egg-info/PKG-INFO
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      263 2023-04-18 17:45:03.000000 xflib-0.1.11/src/xflib.egg-info/SOURCES.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        1 2023-04-18 17:45:03.000000 xflib-0.1.11/src/xflib.egg-info/dependency_links.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       10 2023-04-18 17:45:03.000000 xflib-0.1.11/src/xflib.egg-info/requires.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        6 2023-04-18 17:45:03.000000 xflib-0.1.11/src/xflib.egg-info/top_level.txt
```

### Comparing `xflib-0.1.10/LICENSE` & `xflib-0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `xflib-0.1.10/setup.py` & `xflib-0.1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xflib',
-    version='0.1.10',
+    version='0.1.11',
     description='A particle system, effects and UI library for Pygame',
     author='XFajk',
     author_email='ertyperty24@gmail.com',
     url='https://github.com/XFajk/xflib/tree/main',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `xflib-0.1.10/src/xflib/ps.py` & `xflib-0.1.11/src/xflib/ps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pygame
 import math
+from typing import Callable
 from .utils import surf_circle, surf_rect, surf_polygon
 
 
 class ShapeParticles:
     def __init__(self, shape_type: str, gravity: float = 0.0):
         self.shape_type = shape_type
         self.gravity = gravity
@@ -18,15 +19,15 @@
                 "vel": vel,
                 "size": size,
                 "color": color,
                 "dis_amount": dis_amount,
             }
         )
 
-    def use(self, surf: pygame.Surface, dt: float = 1.0, operation=lambda x, dt: x):
+    def use(self, surf: pygame.Surface, dt: float, operation: Callable[[dict, float], any]):
         if self.shape_type == "circle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
                 p["loc"][0] += p["vel"][0] * dt
                 p["loc"][1] += p["vel"][1] * dt
                 p["size"] -= p["dis_amount"] * dt
                 p["vel"][1] += self.gravity * dt
                 operation(p, dt)
@@ -43,15 +44,15 @@
                 operation(p, dt)
                 pygame.draw.rect(surf, p["color"], (p["loc"][0]-p["size"]/2, p["loc"][1]-p["size"]/2, p["size"], p["size"]))
                 if p["size"] <= 0:
                     self.objects.pop(i)
         else:
             raise TypeError(f"{self.shape_type} is an invalid shape type you can use circle or rectangle")
 
-    def use_with_light(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
+    def use_with_light(self, surf: pygame.Surface, dt: float, operation: Callable[[dict, float], any]):
         if self.shape_type == "circle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
                 p["loc"][0] += p["vel"][0] * dt
                 p["loc"][1] += p["vel"][1] * dt
                 p["size"] -= p["dis_amount"] * dt
                 p["vel"][1] += self.gravity * dt
                 operation(p, dt)
@@ -86,23 +87,23 @@
         self.gravity = gravity
         self.objects = []
 
     def add(self, loc: list | pygame.Vector2, angle: float, speed: float, scale: float, color: tuple | pygame.Color,
             dis_amount: float):
         self.objects.append(Spark(loc, math.radians(angle), speed, color, scale, dis_amount))
 
-    def use(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
+    def use(self, surf: pygame.Surface, dt: float, operation: Callable[[dict, float], any]):
         for i, s in sorted(enumerate(self.objects), reverse=True):
             s.move(dt, self.gravity)
             operation(s, dt)
             s.draw(surf)
             if not s.alive:
                 self.objects.pop(i)
 
-    def use_with_light(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
+    def use_with_light(self, surf: pygame.Surface, dt: float, operation: Callable[[dict, float], any]):
         for i, s in sorted(enumerate(self.objects), reverse=True):
             s.move(dt, self.gravity)
             operation(s, dt)
             s.draw(surf)
             scale = s.scale * 3
             points = [
                 [s.loc[0] + math.cos(s.angle) * s.speed * scale,
@@ -145,15 +146,15 @@
                 "color": color,
                 "dis_amount": dis_amount,
                 "rot_amount_deg": rot_amount_deg,
                 "rotation": 0
             }
         )
 
-    def use(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
+    def use(self, surf: pygame.Surface, dt: float, operation: Callable[[dict, float], any]):
         for i, p in sorted(enumerate(self.objects), reverse=True):
             p["loc"][0] += p["vel"][0] * dt
             p["loc"][1] += p["vel"][1] * dt
             p["size"] -= p["dis_amount"] * dt
             p["vel"][1] += self.gravity * dt
             operation(p, dt)
             p_img = pygame.transform.scale(self.img, (p["size"], p["size"]))
```

