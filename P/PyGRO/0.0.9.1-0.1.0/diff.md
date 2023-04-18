# Comparing `tmp/PyGRO-0.0.9.1.tar.gz` & `tmp/PyGRO-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRO-0.0.9.1.tar", last modified: Tue Nov 30 15:44:29 2021, max compression
+gzip compressed data, was "PyGRO-0.1.0.tar", last modified: Tue Apr 18 07:07:26 2023, max compression
```

## Comparing `PyGRO-0.0.9.1.tar` & `PyGRO-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2021-11-30 15:44:29.929579 PyGRO-0.0.9.1/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2595 2021-11-30 15:44:29.929358 PyGRO-0.0.9.1/PKG-INFO
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2021-11-30 15:44:29.908546 PyGRO-0.0.9.1/PyGRO.egg-info/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2595 2021-11-30 15:44:29.000000 PyGRO-0.0.9.1/PyGRO.egg-info/PKG-INFO
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      422 2021-11-30 15:44:29.000000 PyGRO-0.0.9.1/PyGRO.egg-info/SOURCES.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        1 2021-11-30 15:44:29.000000 PyGRO-0.0.9.1/PyGRO.egg-info/dependency_links.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)       25 2021-11-30 15:44:29.000000 PyGRO-0.0.9.1/PyGRO.egg-info/requires.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        6 2021-11-30 15:44:29.000000 PyGRO-0.0.9.1/PyGRO.egg-info/top_level.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1645 2021-06-10 12:30:16.000000 PyGRO-0.0.9.1/README.md
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2021-11-30 15:44:29.913262 PyGRO-0.0.9.1/pygro/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      159 2021-02-08 10:52:48.000000 PyGRO-0.0.9.1/pygro/__init__.py
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2021-11-30 15:44:29.927621 PyGRO-0.0.9.1/pygro/default_metrics/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    11199 2021-04-04 11:28:03.000000 PyGRO-0.0.9.1/pygro/default_metrics/KerrBL.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    49866 2021-05-08 10:28:38.000000 PyGRO-0.0.9.1/pygro/default_metrics/KerrSTVG.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2657 2021-04-04 11:28:07.000000 PyGRO-0.0.9.1/pygro/default_metrics/Yukawa.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      130 2021-05-08 10:28:55.000000 PyGRO-0.0.9.1/pygro/default_metrics/__init__.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     3753 2021-11-16 21:36:58.000000 PyGRO-0.0.9.1/pygro/geodesic.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     5503 2021-11-30 15:43:08.000000 PyGRO-0.0.9.1/pygro/geodesic_engine.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    15149 2021-06-10 12:31:19.000000 PyGRO-0.0.9.1/pygro/integrators.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        0 2021-02-08 17:04:03.000000 PyGRO-0.0.9.1/pygro/interpolators.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    22828 2021-11-30 15:43:03.000000 PyGRO-0.0.9.1/pygro/metric_engine.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)       38 2021-11-30 15:44:29.929645 PyGRO-0.0.9.1/setup.cfg
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      739 2021-11-30 15:44:16.000000 PyGRO-0.0.9.1/setup.py
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.212633 PyGRO-0.1.0/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1065 2021-01-29 22:40:37.000000 PyGRO-0.1.0/LICENSE.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-04-18 07:07:26.212458 PyGRO-0.1.0/PKG-INFO
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.206441 PyGRO-0.1.0/PyGRO.egg-info/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/PKG-INFO
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      452 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        1 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)       25 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/requires.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        6 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/top_level.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      925 2022-02-10 10:18:41.000000 PyGRO-0.1.0/README.md
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.209246 PyGRO-0.1.0/pygro/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      195 2022-03-11 17:21:23.000000 PyGRO-0.1.0/pygro/__init__.py
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.212059 PyGRO-0.1.0/pygro/default_metrics/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    11199 2021-04-04 11:28:03.000000 PyGRO-0.1.0/pygro/default_metrics/KerrBL.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    49866 2021-05-08 10:28:38.000000 PyGRO-0.1.0/pygro/default_metrics/KerrSTVG.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2657 2021-04-04 11:28:07.000000 PyGRO-0.1.0/pygro/default_metrics/Yukawa.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      130 2021-05-08 10:28:55.000000 PyGRO-0.1.0/pygro/default_metrics/__init__.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     3753 2023-04-18 06:57:57.000000 PyGRO-0.1.0/pygro/geodesic.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     8386 2023-04-18 06:58:01.000000 PyGRO-0.1.0/pygro/geodesic_engine.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    17450 2023-04-18 06:57:43.000000 PyGRO-0.1.0/pygro/integrators.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        0 2021-02-08 17:04:03.000000 PyGRO-0.1.0/pygro/interpolators.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    33634 2023-04-18 06:57:42.000000 PyGRO-0.1.0/pygro/metric_engine.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     4228 2022-03-24 17:38:30.000000 PyGRO-0.1.0/pygro/observer.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)       38 2023-04-18 07:07:26.212672 PyGRO-0.1.0/setup.cfg
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      737 2023-04-18 07:06:41.000000 PyGRO-0.1.0/setup.py
```

### Comparing `PyGRO-0.0.9.1/README.md` & `PyGRO-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,40 @@
+Metadata-Version: 2.1
+Name: PyGRO
+Version: 0.1.0
+Summary: A Python Integrator for General Relativistic Orbits
+Author: Riccardo Della Monica
+Author-email: dellamonicariccardo@gmail.com
+License: LICENSE.txt
+Keywords: python,first package
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # PyGRO
 ### A Python integrator for General Relativistic Orbits
 
-[PyGRO](https://github.com/rdellamonica/pigro/tree/master) is a Python library that provides methods and functions to perform the numerical integration of the geodesic equations describing a particle or photon orbit in any metric theory of gravity, given an alaytic expression of the metric tensor.
+[PyGRO](https://github.com/rdellamonica/pigro/tree/master) is a Python library that provides methods and functions to perform the numerical integration of the geodesic equations describing a particle or photon orbit in any metric theory of gravity, given an analytic expression of the metric tensor.
 
 ***
 
 ## Installation
 PyGRO is distributed as a Python package that can be installed through the PyPi package mangaer via:
 
 ```bash
 pip install pygro
 ```
 
-or by cloning this GitHub repository.
+or by cloning [PyGRO GitHub repository](https://github.com/rdellamonica/pigro/tree/master).
 
 ## Documentation
-The complete documentation for PyGRO is available on [docs](https://github.com/rdellamonica/pigro/tree/master).
-
-***
-## Minimal example
-
-PyGRO comes with several built-in spacetimes that can be used to study the motion of test massive and mass-less particles undergoing geodesic motion.
-
-This is an example of time-like geodesic around a Kerr black hole in Boyer-Lindquist coordinates (`default_metrics.KerrBL()`)
-
-```python
-import pygro
-import numpy as np
+The complete documentation for PyGRO is available on [docs](https://rdellamonica.github.io/pygro/build/html/index.html) (still work in progress).
 
-metric = pygro.default_metrics.KerrBL(m = 1, a = 0.95)
-geo_engine = pygro.GeodesicEngine(metric)
-
-geo = pygro.Geodesic("time-like", geo_engine)
-geo.set_starting_point(0, 50, np.pi/2, 0)
-geo.set_starting_velocity_direction(0, 90, v = 0.1, angles = "deg")
-
-geo_engine.integrate(geo, 10000, initial_step = 1)
-```
-Which returns integrated coordinates in the `Geodesic` object.
-
-![alt text](img/example1.png "Integrated time-like geodesic in the Kerr spacetime.")
-
-***
 ## Copyright
 
 Copyright 2020 Riccardo Della Monica
 
-PyGRO is a free software made available under the MIT License. For details see the LICENSE file.
+PyGRO is a free software made available under the MIT License. For details see the LICENSE file.
```

### Comparing `PyGRO-0.0.9.1/pygro/default_metrics/KerrBL.py` & `PyGRO-0.1.0/pygro/default_metrics/KerrBL.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.0.9.1/pygro/default_metrics/KerrSTVG.py` & `PyGRO-0.1.0/pygro/default_metrics/KerrSTVG.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.0.9.1/pygro/default_metrics/Yukawa.py` & `PyGRO-0.1.0/pygro/default_metrics/Yukawa.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.0.9.1/pygro/geodesic.py` & `PyGRO-0.1.0/pygro/geodesic.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.0.9.1/pygro/integrators.py` & `PyGRO-0.1.0/pygro/integrators.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,28 +61,38 @@
 
         h = initial_step
         twiddle1 = self.twiddle1
         twiddle2 = self.twiddle2
         quit1 = self.quit1
         quit2 = self.quit2
 
-        while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+        try:
+            while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+                if self.verbose:
+                    print("{:.4f}".format(x[-1]), end= "\r")
+                next = self.next_step(x[-1], y[-1], h, twiddle1, twiddle2, quit1, quit2)
+                x.append(next[0])
+                y.append(next[1])
+                h = next[2]
+                twiddle1 = next[3]
+                twiddle2 = next[4]
+                quit1 = next[5]
+                quit2 = next[6]
+            
+            if not self.stopping_criterion(*y[-1]):
+                exit = self.stopping_criterion.exit
+            else:
+                exit = "done"
+        except KeyboardInterrupt:
             if self.verbose:
-                print("{:.4f}".format(x[-1]), end= "\r")
-            next = self.next_step(x[-1], y[-1], h, twiddle1, twiddle2, quit1, quit2)
-            x.append(next[0])
-            y.append(next[1])
-            h = next[2]
-            twiddle1 = next[3]
-            twiddle2 = next[4]
-            quit1 = next[5]
-            quit2 = next[6]
+                print("Integration stopped.")
+            exit = "stopped"
         
         if not self.interpolate:
-            return np.array(x), np.array(y)
+            return np.array(x), np.array(y), exit
         else:
             return sp_int.interp1d(np.array(x), np.array(y), kind = 'cubic')
 
     def next_step(self, x, y, h, TWIDDLE1, TWIDDLE2, QUIT1, QUIT2):
         k = np.zeros(6, dtype = object)
         h1 = h
         while True:
@@ -179,24 +189,25 @@
             w = v/(self.Atol+self.Rtol*y1)
             return np.linalg.norm(w)**(1/(1+i))
         else:
             v = y1-y2
             return abs(v/(self.Atol+self.Rtol*y1))**(1/(1+i))
 
 class RungeKuttaFehlberg78():
-    def __init__(self, f, initial_step = 1, AccuracyGoal = 10, PrecisionGoal = 0, SF = 0.9, interpolate = False, stopping_criterion = "none", verbose = False):
+    def __init__(self, f, initial_step = 1, AccuracyGoal = 10, PrecisionGoal = 0, SF = 0.9, interpolate = False, stopping_criterion = "none", verbose = False, hmax = np.inf):
 
         self.f = f
         self.tolerance = 1
         self.Atol = 10**(-AccuracyGoal)
         self.Rtol = 10**(-PrecisionGoal)
         self.initial_step = initial_step
         self.interpolate = interpolate
         self.verbose = verbose
         self.SF = SF
+        self.hmax = hmax
 
         self.c = [0, 2/27,  1/9, 1/6, 5/12, 1/2, 5/6, 1/6, 2/3, 1/3, 1, 0, 1]
         
         self.a = np.array(
         [
             [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
             [2/27, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
@@ -211,16 +222,16 @@
             [2383/4100, 0, 0, -341/164, 4496/1025, -301/82, 2133/4100, 45/82, 45/164, 18/41, 0, 0, 0],
             [3/205, 0, 0, 0, 0, -6/41, -3/205, -3/41, 3/41, 6/41, 0, 0, 0],
             [-1777/4100, 0, 0, -341/164, 4496/1025, -289/82, 2193/4100, 51/82, 33/164, 12/41, 0, 1, 0]
         ])
 
         self.b = np.array(
             [
-                [41/840, 0, 0, 0, 0, 34/105, 9/35, 9/35, 9/280, 9/280, 41/180, 0, 0],
-                [0, 0, 0, 0, 0, 34/105, 9/35, 9/35, 9/280, 9/280, 0, 41/180, 41/180]
+                [41/840, 0, 0, 0, 0, 34/105, 9/35, 9/35, 9/280, 9/280, 41/840, 0, 0],
+                [0, 0, 0, 0, 0, 34/105, 9/35, 9/35, 9/280, 9/280, 0, 41/840, 41/840]
             ]
         )
 
         if stopping_criterion == "none":
             self.stopping_criterion = lambda geo: True
         else:
             self.stopping_criterion = stopping_criterion
@@ -228,54 +239,81 @@
     def integrate(self, x_start, x_end, y_start, initial_step):
 
         x = [x_start]
         y = [y_start]
 
         h = initial_step
 
-        while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+        try:
+            while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+                if self.verbose:
+                    print("{:.4f}".format(x[-1]), end= "\r")
+                next = self.next_step(x[-1], y[-1], h)
+                x.append(next[0])
+                y.append(next[1])
+                h = next[2]
+
+            if not self.stopping_criterion(*y[-1]):
+                exit = self.stopping_criterion.exit
+            else:
+                exit = "done"
+        except KeyboardInterrupt:
             if self.verbose:
-                print("{:.4f}".format(x[-1]), end= "\r")
-            next = self.next_step(x[-1], y[-1], h)
-            x.append(next[0])
-            y.append(next[1])
-            h = next[2]
+                print("Integration stopped.")
+            exit = "stopped"
         
         if not self.interpolate:
-            return np.array(x), np.array(y)
+            return np.array(x), np.array(y), exit
         else:
             return sp_int.interp1d(np.array(x), np.array(y), kind = 'cubic')
 
     def next_step(self, x, y, h):
         k = np.zeros(13, dtype = object)
-        h1 = h
+        h1 = h*1
+        ATTEMPTS = 1000
+
         while True:
-            
             for i in range(13):
-                k[i] = h1*self.f(x+self.c[i]*h1, y + np.dot(k, self.a[i]))
+                k[i] = self.f(x+self.c[i]*h1, y + h1*np.dot(k, self.a[i]))
             
-            y7 = y + np.dot(self.b[0], k)
-            y8 = y + np.dot(self.b[1], k)
+            y7 = y + h1*np.dot(self.b[0], k)
+            y8 = y + h1*np.dot(self.b[1], k)
             
-            v = y8-y7
-            w = abs(v)/(self.Atol+self.Rtol*abs(y7))
+            v = y7-y8
+            w = abs(v)/(self.Atol+self.Rtol*abs(np.maximum(y7,y8)))
 
-            err = max(w)
-            print(err)
-            if err > 1:
-                h1 *= self.SF*err**(-1/7)
+            err = np.linalg.norm(w) / w.size ** 0.5
+
+            #print(err, end = "\r")
+
+            scale_min = 0.125
+            scale_max = 4
+
+            if err == 0:
+                scale = scale_max
+                h1 *= scale
+                h1 = np.min([h1, self.hmax])
+            else:                
+
+                scale = 0.8*(1/err)**(1/7)
+                scale = min(max(scale, scale_min), scale_max)
+                
+                h1 *= scale
+                h1 = np.min([h1, self.hmax])
+                if err <= 1:
+                    break
                 continue
-            else:
-                h1 *= self.SF*err**(-1/8)
-                break
+        
+        #print("------------------  Step done")
+            
         x1 = x + h1
-        return x1, y8, h1
+        return x1, y7, h1
 
 class RungeKuttaFehlberg45():
-    def __init__(self, f, initial_step = 1, AccuracyGoal = 10, PrecisionGoal = 0, SF = 0.9, interpolate = False, stopping_criterion = "none", verbose = False, hmax = 1e+16):
+    def __init__(self, f, initial_step = 1, AccuracyGoal = 10, PrecisionGoal = 0, SF = 0.84, interpolate = False, stopping_criterion = "none", verbose = False, hmax = 1e+16):
 
         self.f = f
         self.tolerance = 1
         self.Atol = 10**(-AccuracyGoal)
         self.Rtol = 10**(-PrecisionGoal)
         self.initial_step = initial_step
         self.interpolate = interpolate
@@ -285,15 +323,15 @@
 
         self.a = np.array([
             [0, 0, 0, 0, 0, 0],
             [1/4, 0, 0, 0, 0, 0],
             [3/32, 9/32, 0, 0, 0, 0],
             [1932/2197, -7200/2197, 7296/2197, 0, 0, 0],
             [439/216, -8, 3680/513, -845/4104, 0, 0],
-            [-8/27, 2, -3544/2565, 1859/4104, -11/40, 0]
+            [-8/27, 2, -3544/2565, 1859/4104, -11/40, 0],
         ])
 
         self.b = np.array([
             [16/135,  0, 6656/12825, 28561/56430, -9/50, 2/55],
             [25/216, 0, 1408/2565, 2197/4104, -1/5, 0]
         ])
 
@@ -309,24 +347,34 @@
     def integrate(self, x_start, x_end, y_start, initial_step):
 
         x = [x_start]
         y = [y_start]
 
         h = initial_step
 
-        while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+        try:
+            while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+                if self.verbose:
+                    print("{:.4f}".format(x[-1]), end= "\r")
+                next = self.next_step(x[-1], y[-1], h)
+                x.append(next[0])
+                y.append(next[1])
+                h = next[2]
+
+            if not self.stopping_criterion(*y[-1]):
+                exit = self.stopping_criterion.exit
+            else:
+                exit = "done"
+        except KeyboardInterrupt:
             if self.verbose:
-                print("{:.4f}".format(x[-1]), end= "\r")
-            next = self.next_step(x[-1], y[-1], h)
-            x.append(next[0])
-            y.append(next[1])
-            h = next[2]
+                print("Integration stopped.")
+            exit = "stopped"
         
         if not self.interpolate:
-            return np.array(x), np.array(y)
+            return np.array(x), np.array(y), exit
         else:
             return sp_int.interp1d(np.array(x), np.array(y), kind = 'cubic')
 
     def next_step(self, x, y, h):
         k = np.zeros(6, dtype = object)
         h1 = h
         while True:
@@ -334,28 +382,41 @@
             for i in range(6):
                 k[i] = h1*self.f(x+self.c[i]*h1, y + np.dot(k, self.a[i]))
             
             y4 = y + np.dot(self.b[1], k)
             y5 = y + np.dot(self.b[0], k)
             
             v = y4-y5
-            w = abs(v)/(self.Atol+self.Rtol*abs(y4))
 
-            err = max(w)
+            err = np.linalg.norm(v)/h1/self.Atol
+
             if err > 1:
-                h1 *= self.SF*err**(-0.25)
+                delta = self.SF*err**(-0.2)
+                if delta <= 0.1:
+                    h1 *= 0.1
+                elif delta >= 4:
+                    h1 *= 4
+                else:
+                    h1 *= delta
                 continue
             else:
                 if err == 0:
-                    h2 = min(self.hmax, 2*h1)
+                    if self.hmax > 0:
+                        h2 = min(self.hmax, 2*h1)
+                    else:
+                        h2 = max(self.hmax, 2*h1)
                     break
-                h2 = min(self.hmax, h1*self.SF*err**(-0.2))
+                if self.hmax > 0:
+                    h2 = min(self.hmax, h1*self.SF*err**(-0.2))
+                else:
+                    h2 = max(self.hmax, h1*self.SF*err**(-0.2))
                 break
+            
         x1 = x + h1
-        return x1, y5, h2
+        return x1, y4, h2
 
 
 class DormandPrince45():
     def __init__(self, f, initial_step = 1, AccuracyGoal = 10, PrecisionGoal = 10, SF = 0.9, interpolate = False, stopping_criterion = "none", verbose = False, hmax = 1e+16):
 
         self.f = f
         self.tolerance = 1
@@ -394,24 +455,34 @@
     def integrate(self, x_start, x_end, y_start, initial_step):
 
         x = [x_start]
         y = [y_start]
 
         h = initial_step
 
-        while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+        try:
+            while abs(x[-1]) <= abs(x_end) and self.stopping_criterion(*y[-1]):
+                if self.verbose:
+                    print("{:.4f}".format(x[-1]), end= "\r")
+                next = self.next_step(x[-1], y[-1], h)
+                x.append(next[0])
+                y.append(next[1])
+                h = next[2]
+
+            if not self.stopping_criterion(*y[-1]):
+                exit = self.stopping_criterion.exit
+            else:
+                exit = "done"
+        except KeyboardInterrupt:
             if self.verbose:
-                print("{:.4f}".format(x[-1]), end= "\r")
-            next = self.next_step(x[-1], y[-1], h)
-            x.append(next[0])
-            y.append(next[1])
-            h = next[2]
+                print("Integration stopped.")
+            exit = "stopped"
         
         if not self.interpolate:
-            return np.array(x), np.array(y)
+            return np.array(x), np.array(y), exit
         else:
             return sp_int.interp1d(np.array(x), np.array(y), kind = 'cubic')
 
     def next_step(self, x, y, h):
         k = np.zeros(7, dtype = object)
         h1 = h
         while True:
```

### Comparing `PyGRO-0.0.9.1/pygro/metric_engine.py` & `PyGRO-0.1.0/pygro/metric_engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,86 +17,197 @@
 #    -  x: an array of coordinates;                                                     #
 #    -  u: an array of derivatives of x w.r.t. to the affine parameter;                 #
 #                                                                                       #   
 #   g and x are user inputs.                                                            #
 #                                                                                       #
 #########################################################################################
 
+def parse_expr(expr):
+    return sp.parse_expr(expr)
+
 class Metric():
-    def __init__(self):
+    instances = []
+    r"""This is the main symbolic tool within PyGRO to perform tensorial calculations
+    starting from the spacetime metric. The ``Metric`` object can be initialized in two separate ways:
+
+    .. rubric:: Interactive mode
+    
+    In this case the ``Metric`` has to be initialized without any additional argument.
+    Later the :py:func:`Metric.initialize_metric` method should be called without additional arguments in order to enter the interactive mode.
+    During this phase the user will be asked to input:
+
+    * The ``name`` of the spacetime.
+    * The symbolic ``coordinates`` in which the metric is expressed.
+    * The symbolic expression of the spacetime metric which can be either expressed as a line elemnt :math:`ds^2 = g_{\mu\nu}dx^\mu dx^\nu` or as the single components :math:`g_{\mu\nu}` of the metric tensor.
+    * The symbolix expression of ``transformation functions`` to pseudo-cartesian coordinates which can be useful to :doc:`visualize`.
+
+    After the insertion of all the required information the metric is initialized.
+
+    .. rubric:: Functional mode
+
+    In this case the ``Metric`` object is initialized without interactive input by the user. The arguments to build the metric can be either passed to the ``Metric`` constructor upon class initialization,
+    
+    >>> spacetime_metric = pygro.Metric(**kwargs)
+
+    or as arguments to the  :py:func:`Metric.initialize_metric` method:
+
+    >>> spacetime_metric = pygro.Metric()
+    >>> spacetime_metric.initialize_metric(**kwargs)
+
+    The ``**kwargs`` that can be passed to initialize a ``Metric`` object are the following:
+
+    :param name: The name of the metric to initialize.
+    :type name: str
+    :param coordinates: Four-dimensional list containing the symbolic expression of the space-time coordinates in which the `line_element` argument is written.
+    :type coordinates: list of str
+    :param line_element: A string containing the symbolic expression of the line element (that will be parsed using `sympy`) expressed in the space-time coordinates defined in the `coordinates` argument.
+    :type line_element: str
+
+    .. note::
+        Test
+    
+    After successful initialization, the ``Metric`` instance has the following attributes:
+
+    :ivar g: The symbolic representation of the metric tensor. It is a :math:`4\times4` ``sympy.Matrix`` object.
+    :type g: sympy.Matric
+
+    """
+    def __init__(self, **kwargs):
         self.initialized = 0
         self.initialized_metric = 0
         self.geodesic_engine_linked = False
-    
-    def initialize_metric(self):
-        self.name = input("Insert the name of the spacetime (e.g. 'Kerr metric'): ")
 
-        print("Initialazing {}".format(self.name))
+        if len(kwargs) > 0:
+            if "load" in kwargs:
+                self.load_metric(kwargs["load"])
+            self.initialize_metric(**kwargs)
         
-        print("Define coordinates symbols:")
+        Metric.instances.append(self)
+    
+    def initialize_metric(self, **kwargs):
+        """Initializes the `Metric` either in *Interactive* or *Functional* mode. 
+
+        :param \**kwargs:
+            to pass only to access *Functional* mode. In this case, required parameters are ``name``, ``coordinates`` and ``line_element``,
+            but additional parameters can and *must* be passed on occasions (see :doc:`create_metric` to see examples). 
+        """
+
         self.x = []
         self.dx = []
         self.x_str = []
         self.u = []
-        for i in range(4):
-            coordinate = input("Coordinate {}: ".format(i))
-            setattr(self, coordinate, sp.symbols(coordinate))
-            self.x.append(self.__dict__[coordinate])
-            self.x_str.append(coordinate)
 
-            velocity = "u_" + coordinate
-            setattr(self, velocity, sp.symbols(velocity))
-            self.u.append(self.__dict__[velocity])
+        interactive_metric_insertion = len(kwargs) == 0        
 
-            differential = "d" + coordinate
-            setattr(self, differential, sp.symbols(differential))
-            self.dx.append(self.__dict__[differential])
-        
+        if not interactive_metric_insertion:
 
-        case = input("From? [tensor/line element]: ")
+            minimal_kwargs = ["name", "coordinates", "line_element"]
 
-        if case == "tensor":
-            print("Define metric tensor components:")
-            self.g = sp.zeros(4, 4)
-            self.g_str = np.zeros([4,4], dtype = object)
+            for kwarg in minimal_kwargs:
+                if not kwarg in kwargs:
+                    raise ValueError('initialize_metric in non-interactive mode should have "name", "coordinates", "line_element" as minimal arguments')
 
-            for i in range(4):
-                for j in range(4):
-                    while True:
-                        try:
-                            component = input("g[{},{}]: ".format(i, j))
-                            component_symb = sp.parse_expr(component)
-                        except:
-                            print("Please insert a valid expression for the component.")
-                            continue
-                        else:
-                            self.g[i,j] = component_symb
-                            self.g_str[i,j] = component
-                            break
-                    
-        elif case == "line element":
+            self.name = kwargs['name']
+
+            coordinates_input = kwargs["coordinates"]
+            
+            if len(coordinates_input) != 4:
+                raise ValueError('coordinates should be a 4-dimensional list of strings')
+            
+            for coordinate in coordinates_input:
+                setattr(self, coordinate, sp.symbols(coordinate))
+                self.x.append(self.__dict__[coordinate])
+                self.x_str.append(coordinate)
+
+                velocity = "u_" + coordinate
+                setattr(self, velocity, sp.symbols(velocity))
+                self.u.append(self.__dict__[velocity])
+
+                differential = "d" + coordinate
+                setattr(self, differential, sp.symbols(differential))
+                self.dx.append(self.__dict__[differential])
+            
             self.g = sp.zeros(4, 4)
             self.g_str = np.zeros([4,4], dtype = object)
-            while True:
-                try:
-                    ds2_str = input("ds^2 = ")
-                    ds2_sym = sp.expand(sp.parse_expr(ds2_str))
-                except:
-                    print("Please insert a valid expression for the line element.")
-                    continue
-                else:
-                    self.ds2 = ds2_sym
-                    for i, dx1 in enumerate(self.dx):
-                        for j, dx2 in enumerate(self.dx):
-                            self.g[i,j] = self.ds2.coeff(dx1*dx2,1)
-                            self.g_str[i,j] = str(self.g[i,j])
-                    break
+
+            try:
+                ds2_str = kwargs["line_element"]
+                ds2_sym = sp.expand(sp.parse_expr(ds2_str))
+            except:
+                raise ValueError("Please insert a valid expression for the line element.")
+            else:
+                self.ds2 = ds2_sym
+                for i, dx1 in enumerate(self.dx):
+                    for j, dx2 in enumerate(self.dx):
+                        self.g[i,j] = self.ds2.coeff(dx1*dx2,1)
+                        self.g_str[i,j] = str(self.g[i,j])
+
         else:
-            raise("Only 'tensor' or 'line element' are accepted method for parsing the metric.")
-        
+            self.name = input("Insert the name of the spacetime (e.g. 'Kerr metric'): ")
+
+            print("Initialazing {}".format(self.name))
+            
+            print("Define coordinates symbols:")
+            
+            for i in range(4):
+                coordinate = input("Coordinate {}: ".format(i))
+                setattr(self, coordinate, sp.symbols(coordinate))
+                self.x.append(self.__dict__[coordinate])
+                self.x_str.append(coordinate)
+
+                velocity = "u_" + coordinate
+                setattr(self, velocity, sp.symbols(velocity))
+                self.u.append(self.__dict__[velocity])
+
+                differential = "d" + coordinate
+                setattr(self, differential, sp.symbols(differential))
+                self.dx.append(self.__dict__[differential])
+            
+
+            case = input("From? [tensor/line element]: ")
+
+            if case == "tensor":
+                print("Define metric tensor components:")
+                self.g = sp.zeros(4, 4)
+                self.g_str = np.zeros([4,4], dtype = object)
+
+                for i in range(4):
+                    for j in range(4):
+                        while True:
+                            try:
+                                component = input("g[{},{}]: ".format(i, j))
+                                component_symb = sp.parse_expr(component)
+                            except:
+                                print("Please insert a valid expression for the component.")
+                                continue
+                            else:
+                                self.g[i,j] = component_symb
+                                self.g_str[i,j] = component
+                                break
+                        
+            elif case == "line element":
+                self.g = sp.zeros(4, 4)
+                self.g_str = np.zeros([4,4], dtype = object)
+                while True:
+                    try:
+                        ds2_str = input("ds^2 = ")
+                        ds2_sym = sp.expand(sp.parse_expr(ds2_str))
+                    except:
+                        print("Please insert a valid expression for the line element.")
+                        continue
+                    else:
+                        self.ds2 = ds2_sym
+                        for i, dx1 in enumerate(self.dx):
+                            for j, dx2 in enumerate(self.dx):
+                                self.g[i,j] = self.ds2.coeff(dx1*dx2,1)
+                                self.g_str[i,j] = str(self.g[i,j])
+                        break
+            else:
+                raise("Only 'tensor' or 'line element' are accepted method for parsing the metric.")
+            
         print("Calculating inverse metric...")
         self.g_inv = self.g.inv()
         self.g_inv_str = np.zeros([4,4], dtype = object)
         
         for i in range(4):
             for j in range(4):
                 self.g_inv_str[i,j] = str(self.g_inv[i,j])
@@ -143,83 +254,139 @@
         
         free_sym = list(self.g.free_symbols-set(self.x))
         free_func = list(self.g.atoms(AppliedUndef))
 
         if len(free_sym) > 0:
             for sym in free_sym:
                 self.add_parameter(str(sym))
-                value = float(input("Insert value for {}: ".format(str(sym))))
-                self.set_constant(**{str(sym): value})
+                if str(sym) in kwargs:
+                    self.set_constant(**{str(sym): kwargs.get(str(sym))})
+                else:
+                    value = float(input("Insert value for {}: ".format(str(sym))))
+                    self.set_constant(**{str(sym): value})
 
         if len(free_func) > 0:
             for func in free_func:
                 self.add_parameter(str(func))
-                kind = input("Define kind for function {} [expr/py]: ".format(str(func)))
+                
+                if interactive_metric_insertion:
+                    kind = input("Define kind for function {} [expr/py]: ".format(str(func)))
+                else:
+                    if not str(func.func) in kwargs:
+                        raise ValueError("Auxiliary functions shoudld be passed as arguments, either as strings (expression mode) or as python methods (functional mode).")
+                    
+                    if isinstance(kwargs[str(func.func)], str):
+                        kind = "expr"
+                    elif callable(kwargs[str(func.func)]):
+                        kind = "py"
 
                 if kind == "expr":
                     self.parameters[str(func)]['kind'] = "expression"
-                    expr_str = input("{} = ".format(str(func)))
+                    if interactive_metric_insertion:
+                        expr_str = input("{} = ".format(str(func)))
+                    else:
+                        expr_str = kwargs[str(func.func)]
+
                     expr_sym = sp.expand(sp.parse_expr(expr_str))
 
                     self.parameters[str(func)]['value'] = expr_sym
 
                     expr_free_sym = expr_sym.free_symbols-set([self.parameters[parameter]["symbolic"] for parameter in self.parameters])-set(self.x)
 
                     for sym in expr_free_sym:
                         self.add_parameter(str(sym))
-                        value = float(input("Insert value for {}: ".format(str(sym))))
-                        self.set_constant(**{str(sym): value})
-
+                        if str(sym) in kwargs:
+                            self.set_constant(**{str(sym): kwargs.get(str(sym))})
+                        else:
+                            value = float(input("Insert value for {}: ".format(str(sym))))
+                            self.set_constant(**{str(sym): value})
 
                     for arg in list(func.args):
                         self.parameters[str(func)][f"d{str(func.func)}d{str(arg)}"] = expr_sym.diff(arg)
 
-
                 elif kind == "py":
 
                     self.parameters[str(func)]['kind'] = "pyfunc"
 
-                    print(f"Remember to set the Python function for {str(func)} and its derivatives with")
+                    if interactive_metric_insertion:
+                        print(f"Remember to set the Python function for {str(func)} and its derivatives with")
                     
-                    derlist = ""
-                    for arg in list(func.args):
-                        derlist += f", d{str(func.func)}d{str(arg)} = func"
-                    
-                    print(f"set_function_to_parameter({str(func)}, f = func{derlist})")
+                        derlist = ""
+                        for arg in list(func.args):
+                            derlist += f", d{str(func.func)}d{str(arg)} = func"
+                        
+                        print(f"set_function_to_parameter({str(func)}, f = func{derlist})")
 
-        while True:
-            case = input("Want to insert transform functions to pseudo-cartesian coordiantes? [y/n] ")
+                    else:
+                        args = list(func.args)
+                        derlist = [f"d{str(func.func)}d{str(arg)}" for arg in args]
 
-            if case == "y":
-                for x in ["t", "x", "y", "z"]:
-                    while True:
-                        try:
-                            x_inpt = input(f"{x} = ")
-                            x_symb = sp.parse_expr(x_inpt)
-                        except KeyboardInterrupt:
-                            raise SystemExit
-                        except:
-                            print("Insert a valid expression.")
-                            continue
-                        else:
-                            self.transform_s.append(x_symb)
-                            self.transform_functions_str.append(x_inpt)
-                            self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(x_symb), 'numpy'))
-                            break
-                break
-                            
-            elif case == "n":
-                break
-            else:
-                print("Not a valid input.")
-                continue
+                        arg_derlist = {}
+
+                        for der in derlist:
+                            if not der in kwargs:
+                                raise ValueError(f"In functional mode pass as arguments functional derivatives  of auxiliary functions. In this case '{der}' is missing.")
+                            else:
+                                arg_derlist[der] = kwargs[der]
+
+                        self.set_function_to_parameter(str(func), kwargs[str(func.func)], **arg_derlist)
+
+        if interactive_metric_insertion:
+            while True:
+                case = input("Want to insert transform functions to pseudo-cartesian coordiantes? [y/n] ")
+
+                if case == "y":
+                    for x in ["t", "x", "y", "z"]:
+                        while True:
+                            try:
+                                x_inpt = input(f"{x} = ")
+                                x_symb = sp.parse_expr(x_inpt)
+                            except KeyboardInterrupt:
+                                raise SystemExit
+                            except:
+                                print("Insert a valid expression.")
+                                continue
+                            else:
+                                self.transform_s.append(x_symb)
+                                self.transform_functions_str.append(x_inpt)
+                                self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(x_symb), 'numpy'))
+                                break
+                    break
+                                
+                elif case == "n":
+                    break
+                else:
+                    print("Not a valid input.")
+                    continue
+        else:
+            if "transform" in kwargs:
+                transform = kwargs["transform"]
+                if len(transform) != 4:
+                    raise ValueError('"transform" should be a 4-dimensional list of strings')
+                
+                for i, x in enumerate(["t", "x", "y", "z"]):
+                    try:
+                        x_inpt = transform[i]
+                        x_symb = sp.parse_expr(x_inpt)
+                    except:
+                        raise ValueError(f"Insert a valid expression for transform function {x}")
+                    else:
+                        self.transform_s.append(x_symb)
+                        self.transform_functions_str.append(x_inpt)
+                        self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(x_symb), 'numpy'))
+                    
 
         print("The metric_engine has been initialized.")
 
     def save_metric(self, filename):
+        r"""Saves the metric into a *.metric* file which can later be loaded with the :py:func:`Metric.load_metric` method.
+
+        :param filename: The name of the *.metric* file in which to save the metric.
+        :type filename: str
+        """
         if self.initialized:
             with open(filename, "w+") as file:
                 output = {}
                 
                 output['name'] = self.name
                 output['g'] = self.g_str.tolist()
                 output['x'] = self.x_str
@@ -248,15 +415,19 @@
                 
                 json.dump(output, file)
 
         else:
             print("Initialize (initialize_metric) or load (load_metric) a metric before saving.")
     
     def load_metric(self, filename, verbose = True, **params):
+        r"""Loads the metric from a *.metric* file which has been saved through the :py:func:`Metric.save_metric` method.
 
+        :param filename: The name of the *.metric* file from which to load the metric.
+        :type filename: str
+        """
         f = open(filename, "r")
 
         load = json.load(f)
 
         self.load_metric_from_json(load, verbose, **params)
 
         
@@ -398,21 +569,24 @@
                 transform_function = sp.parse_expr(transf)
                 self.transform_s.append(transform_function)
                 self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(transform_function), 'numpy'))
 
         if verbose:
             print("The metric_engine has been initialized.")
 
-    def add_parameter(self, symbol):
+    def add_parameter(self, symbol, value = None):
         if self.initialized:
             self.parameters[symbol] = {}
             self.parameters[symbol]['symbol'] = symbol
             self.parameters[symbol]['symbolic'] = sp.parse_expr(symbol)
-            self.parameters[symbol]['value'] = None
-            self.parameters[symbol]['kind'] = None
+            self.parameters[symbol]['value'] = value
+            if value != None:
+                self.parameters[symbol]['kind'] = "constant"
+            else:
+                self.parameters[symbol]['kind'] = None
         else:
             print("Initialize (initialize_metric) or load (load_metric) a metric before adding parameters.")
     
     def set_constant(self, **params):
         if self.initialized:
             for param in params:
                 try:
@@ -421,14 +595,22 @@
                 except:
                     print(f"No parameter named '{str(param)}' in the metric_engine.")
                     break
         else:
             print("Initialize (initialize_metric) or load (load_metric) a metric before adding parameters.")
     
     def set_expression_to_parameter(self, param, expr_str):
+        r"""Selects the ``param`` element from the ``metric.parameters`` dictionary, sets its kind to ``"expr"`` and assignes to it a value which is the sybolic parsed
+        espresion in the `expr_str` argument.
+        
+        :param param: The symbolic name of the parameter to modify.
+        :type param: str
+        :param expr_str: The symbolic expresison to assign to this parameter.
+        :type expr_str: str
+        """
         if self.initialized:
             if param in self.parameters:
                 self.parameters[str(param)]['value'] = sp.parse_expr(expr_str)
                 self.parameters[str(param)]['kind'] = "expression"
                 func = self.parameters[str(param)]['symbolic']
 
                 expr_sym = sp.expand(sp.parse_expr(expr_str))
@@ -449,14 +631,30 @@
             else:
                 raise TypeError(f"No parameter named '{str(param)}' in the metric_engine.")
         else:
             print("Initialize (initialize_metric) or load (load_metric) a metric before adding parameters.")
 
 
     def set_function_to_parameter(self, param, function, **derivatives):
+        r"""Selects the ``param`` element from the ``metric.parameters`` dictionary, sets its kind to ``"py"`` and assignes as its value
+        the ``function`` method that is passed as argument. 
+
+        .. note::
+            The ``function`` argument **must** be a method which admits four floats and returns a single float as results.
+            However, in the ``line_element`` argument, upon initialization of the ``Metric``, only explicit coordinate dependences of the
+            functional parameter must be indicated. Moreover, for each of the explicit coordinate dependence of the function its derivative should also
+            be passed in argument
+
+            :Example:
+        
+        :param param: The symbolic name of the parameter to modify.
+        :type param: str
+        :param expr_str: The symbolic expresison to assign to this parameter.
+        :type expr_str: str
+        """
         if self.initialized:
             
             args = list(self.parameters[str(param)]['symbolic'].args)
             func = self.parameters[str(param)]['symbolic'].func
             self.parameters[str(param)]['kind'] = "pyfunc"
 
             self.parameters[str(param)]['value'] = implemented_function(f"{func}_func", function)
@@ -466,28 +664,40 @@
                 if not der in derivatives:
                     raise KeyError(f"Specify a meethod for the derivative of the function with respect to {arg}")
                 else:
                     self.parameters[str(param)][der] = implemented_function(f"d{func}d{arg}_func", derivatives[der])
         else:
             print("Initialize (initialize_metric) or load (load_metric) a metric before adding parameters.")
 
+    # Getters
+
     def get_parameters_symb(self):
         return [self.parameters[constant]['symbolic'] for constant in self.parameters if self.parameters[constant]['kind'] == "constant"]
 
     def get_parameters_val(self):
         return [self.parameters[constant]['value'] for constant in self.parameters if self.parameters[constant]['kind'] == "constant"]
 
     def get_parameters_constants(self):
         return {self.parameters[constant]['symbol']: self.parameters[constant] for constant in self.parameters if self.parameters[constant]["kind"] == "constant"}
     
     def get_parameters_expressions(self):
         return {self.parameters[constant]['symbol']: self.parameters[constant] for constant in self.parameters if self.parameters[constant]["kind"] == "expression"}
 
     def get_parameters_functions(self):
         return {self.parameters[constant]['symbol']: self.parameters[constant] for constant in self.parameters if self.parameters[constant]["kind"] == "pyfunc"}
+    
+    def get_constant(self, parameter):
+        """Returns the value of the constant ``parameter``, if defined.
+        """
+        if self.parameters[parameter]["kind"] == "constant":
+            return self.parameters[parameter]["value"]
+        else:
+            raise TypeError(f"Unknown constant {parameter}")
+
+    # Auxiliary functions
 
     def subs_functions(self, expr):
         functions = self.get_parameters_expressions()
 
         if len(functions) > 0:
             for func in functions:
 
@@ -495,30 +705,30 @@
                 f = functions[func]['symbolic']
 
                 for arg in f.args:
                     subs.append((sp.Derivative(f, arg), functions[func][f"d{f.func}d{arg}"]))
                 
                 expr = expr.subs(subs)
             
-            expr = expr.subs(f, functions[func]['value'])
+                expr = expr.subs(f, functions[func]['value'])
         
         functions = self.get_parameters_functions()
 
         if len(functions) > 0:
             for func in functions:
 
                 subs = []
                 f = functions[func]['symbolic']
 
                 for arg in f.args:
                     subs.append((sp.Derivative(f, arg), functions[func][f"d{f.func}d{arg}"](*self.x)))
                 
                 expr = expr.subs(subs)
             
-            expr = expr.subs(f, functions[func]['value'](*self.x))
+                expr = expr.subs(f, functions[func]['value'](*self.x))
         
         return expr
 
 
     def evaluate_parameters(self, expr):
         if any(x['value'] == None for x in self.parameters.values()):
             print("You must set_constant for every constant value in your metric, before evaluating.")
@@ -544,14 +754,17 @@
                     except:
                         print("Insert a valid expression.")
                         continue
                     else:
                         self.transform_s.append(x_symb)
                         self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(x_symb), 'numpy'))
                         break
+    
+    def parse_expr(self, expr):
+        return sp.parse_expr(expr)
 
     def transform(self, X):
         if self.transform_functions:
             return self.transform_functions[0](X), self.transform_functions[1](X), self.transform_functions[2](X), self.transform_functions[3](X)
         else:
             raise TypeError("Coordinate transformations not set. Consider using .set_coordinate_transformation method in Metric class.")
 
@@ -564,11 +777,29 @@
         
         return norm'''
     
     def g_f(self, x):
         return lambdify([*self.x, *self.get_parameters_symb()], self.subs_functions(self.g))(*x, *self.get_parameters_val())
 
     def Christoffel(self, mu, nu, rho):
+        """The mu-nu-rho Christoffel symbol, :math:`\Gamma^{\mu}_{\nu\rho}` related to the metric tensor.
+        """
         ch = 0
         for sigma in range(4):
             ch += self.g_inv[rho,sigma]*(self.g[sigma, nu].diff(self.x[mu])+self.g[mu, sigma].diff(self.x[nu])-self.g[mu, nu].diff(self.x[sigma]))/2
-        return ch
+        return ch
+    
+    def Lagrangian(self):
+        lagrangian = 0
+
+        for i in range(4):
+            for j in range(4):
+                lagrangian += self.g[i,j]*self.u[i]*self.u[j]/2
+        
+        return lagrangian
+    
+    def norm(self, x, vec):
+        n = 0
+        for i in range(4):
+            for j in range(4):
+                n += self.g_f(x)[i,j]*vec[i]*vec[j]
+        return n
```

### Comparing `PyGRO-0.0.9.1/setup.py` & `PyGRO-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='PyGRO',
-  version='0.0.9.1',
+  version='0.1.0',
   author='Riccardo Della Monica',
   author_email='dellamonicariccardo@gmail.com',
   packages=find_packages(),
   license='LICENSE.txt',
   description='A Python Integrator for General Relativistic Orbits',
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
```

