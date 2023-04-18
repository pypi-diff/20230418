# Comparing `tmp/fastpathplanning-0.1.0.tar.gz` & `tmp/fastpathplanning-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastpathplanning-0.1.0.tar", last modified: Mon Apr 17 23:27:39 2023, max compression
+gzip compressed data, was "fastpathplanning-0.1.1.tar", last modified: Tue Apr 18 15:56:33 2023, max compression
```

## Comparing `fastpathplanning-0.1.0.tar` & `fastpathplanning-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:27:39.685389 fastpathplanning-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-17 23:27:39.685389 fastpathplanning-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:27:39.685389 fastpathplanning-0.1.0/fastpathplanning/
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6176 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/boxes.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/fastpathplanning.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/graph.py
--rw-r--r--   0 root         (0) root         (0)     5361 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/polygonal.py
--rw-r--r--   0 root         (0) root         (0)    10220 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/fastpathplanning/smooth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 23:27:39.685389 fastpathplanning-0.1.0/fastpathplanning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-17 23:27:39.000000 fastpathplanning-0.1.0/fastpathplanning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-17 23:27:39.000000 fastpathplanning-0.1.0/fastpathplanning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 23:27:39.000000 fastpathplanning-0.1.0/fastpathplanning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-17 23:27:39.000000 fastpathplanning-0.1.0/fastpathplanning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 23:27:39.000000 fastpathplanning-0.1.0/fastpathplanning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 23:27:39.685389 fastpathplanning-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1294 2023-04-17 23:27:35.000000 fastpathplanning-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/fastpathplanning/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6176 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/boxes.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/fastpathplanning.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/graph.py
+-rw-r--r--   0 root         (0) root         (0)     5361 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/polygonal.py
+-rw-r--r--   0 root         (0) root         (0)    10920 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/smooth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/fastpathplanning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/setup.py
```

### Comparing `fastpathplanning-0.1.0/LICENSE` & `fastpathplanning-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.0/PKG-INFO` & `fastpathplanning-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpathplanning
-Version: 0.1.0
+Version: 0.1.1
 Summary: An algorithm for path planning in sequences of safe boxes
 Home-page: https://github.com/cvxgrp/fpp.py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fastpathplanning-0.1.0/fastpathplanning/boxes.py` & `fastpathplanning-0.1.1/fastpathplanning/boxes.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.0/fastpathplanning/fastpathplanning.py` & `fastpathplanning-0.1.1/fastpathplanning/fastpathplanning.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.0/fastpathplanning/graph.py` & `fastpathplanning-0.1.1/fastpathplanning/graph.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.0/fastpathplanning/polygonal.py` & `fastpathplanning-0.1.1/fastpathplanning/polygonal.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.0/fastpathplanning/smooth.py` & `fastpathplanning-0.1.1/fastpathplanning/smooth.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,15 +171,17 @@
     for i, value in initial.items():
         constraints.append(points[0][i][0] == value)
     for i, value in final.items():
         constraints.append(points[n_boxes - 1][i][-1] == value)
 
     # Loop through boxes.
     cost = 0
+    continuity = {}
     for k in range(n_boxes):
+        continuity[k] = {}
 
         # Box containment.
         Lk = np.array([L[k]] * n_points)
         Uk = np.array([U[k]] * n_points)
         constraints.append(points[k][0] >= Lk)
         constraints.append(points[k][0] <= Uk)
 
@@ -189,14 +191,16 @@
             ci = durations[k] / h
             constraints.append(points[k][i][1:] - points[k][i][:-1] == ci * points[k][i + 1])
 
         # Continuity and differentiability.
         if k < n_boxes - 1:
             for i in range(D + 1):
                 constraints.append(points[k][i][-1] == points[k + 1][i][0])
+                if i > 0:
+                    continuity[k][i] = constraints[-1]
 
         # Cost function.
         for i, ai in alpha.items():
             h = n_points - 1 - i
             A = np.zeros((h + 1, h + 1))
             for m in range(h + 1):
                 for n in range(h + 1):
@@ -215,14 +219,22 @@
     a = 0
     for k in range(n_boxes):
         b = a + durations[k]
         beziers.append(BezierCurve(points[k][0].value, a, b))
         a = b
     path = CompositeBezierCurve(beziers)
 
+    retiming_weights = {}
+    for k in range(n_boxes - 1):
+        retiming_weights[k] = {}
+        for i in range(1, D + 1):
+            primal = points[k][i][-1].value
+            dual = continuity[k][i].dual_value
+            retiming_weights[k][i] = primal.dot(dual)
+
     # Reconstruct costs.
     cost_breakdown = {}
     for k in range(n_boxes):
         cost_breakdown[k] = {}
         bez = beziers[k]
         for i in range(1, D + 1):
             bez = bez.derivative()
@@ -230,32 +242,37 @@
                 cost_breakdown[k][i] = alpha[i] * bez.l2_squared()
 
     # Solution statistics.
     sol_stats = {}
     sol_stats['cost'] = prob.value
     sol_stats['runtime'] = prob.solver_stats.solve_time
     sol_stats['cost_breakdown'] = cost_breakdown
+    sol_stats['retiming_weights'] = retiming_weights
 
     return path, sol_stats
 
 
-def retiming(kappa, costs, durations, **kwargs):
+def retiming(kappa, costs, durations, retiming_weights, **kwargs):
 
     # Decision variables.
     n_boxes = max(costs) + 1
     eta = cp.Variable(n_boxes)
     eta.value = np.ones(n_boxes)
     constr = [durations @ eta == sum(durations)]
 
     # Scale costs from previous trajectory.
     cost = 0
     for i, ci in costs.items():
         for j, cij in ci.items():
-            power = 2 * j - 1
-            cost += cij * cp.power(eta[i], - power)
+            cost += cij * cp.power(eta[i], 1 - 2 * j)
+
+    # Retiming weights.
+    for k in range(n_boxes - 1):
+        for i, w in retiming_weights[k].items():
+            cost += i * retiming_weights[k][i] * (eta[k + 1] - eta[k])
 
     # Trust region.
     if not np.isinf(kappa):
         constr.append(eta[1:] - eta[:-1] <= kappa)
         constr.append(eta[:-1] - eta[1:] <= kappa)
         
     # Solve SOCP and get new durarations.
@@ -292,59 +309,60 @@
 def optimize_bezier_with_retiming(L, U, durations, alpha, initial, final,
     omega=3, kappa_min=1e-2, verbose=False, **kwargs):
 
     # Solve initial Bezier problem.
     path, sol_stats = optimize_bezier(L, U, durations, alpha, initial, final, **kwargs)
     cost = sol_stats['cost']
     cost_breakdown = sol_stats['cost_breakdown']
+    retiming_weights = sol_stats['retiming_weights']
 
     if verbose:
         init_log()
         update_log(0, cost, np.nan, np.inf, True)
 
     # Lists to populate.
     costs = [cost]
     paths = [path]
     durations_iter = [durations]
     bez_runtimes = [sol_stats['runtime']]
     retiming_runtimes = []
 
     # Iterate retiming and Bezier.
-    kappa = np.inf
+    kappa = 1
     n_iters = 0
     i = 1
     while True:
         n_iters += 1
 
         # Retime.
         new_durations, runtime, kappa_max = retiming(kappa, cost_breakdown,
-            durations, **kwargs)
+            durations, retiming_weights, **kwargs)
         durations_iter.append(new_durations)
         retiming_runtimes.append(runtime)
 
         # Improve Bezier curves.
         path_new, sol_stats = optimize_bezier(L, U, new_durations,
             alpha, initial, final, **kwargs)
         cost_new = sol_stats['cost']
-        cost_breakdown_new = sol_stats['cost_breakdown']
         costs.append(cost_new)
         paths.append(path_new)
         bez_runtimes.append(sol_stats['runtime'])
 
         decr = cost_new - cost
         accept = decr < 0
         if verbose:
             update_log(i, cost_new, decr, kappa, accept)
 
         # If retiming improved the trajectory.
         if accept:
             durations = new_durations
             path = path_new
             cost = cost_new
-            cost_breakdown = cost_breakdown_new
+            cost_breakdown = sol_stats['cost_breakdown']
+            retiming_weights = sol_stats['retiming_weights']
 
         if kappa < kappa_min:
             break
         kappa = kappa_max / omega
         i += 1
 
     runtime = sum(bez_runtimes) + sum(retiming_runtimes)
```

### Comparing `fastpathplanning-0.1.0/fastpathplanning.egg-info/PKG-INFO` & `fastpathplanning-0.1.1/fastpathplanning.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpathplanning
-Version: 0.1.0
+Version: 0.1.1
 Summary: An algorithm for path planning in sequences of safe boxes
 Home-page: https://github.com/cvxgrp/fpp.py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fastpathplanning-0.1.0/setup.py` & `fastpathplanning-0.1.1/setup.py`

 * *Files identical despite different names*

