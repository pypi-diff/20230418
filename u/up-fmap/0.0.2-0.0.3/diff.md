# Comparing `tmp/up_fmap-0.0.2.tar.gz` & `tmp/up_fmap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_fmap-0.0.2.tar", last modified: Mon Feb 13 19:06:47 2023, max compression
+gzip compressed data, was "up_fmap-0.0.3.tar", last modified: Tue Apr 18 10:39:17 2023, max compression
```

## Comparing `up_fmap-0.0.2.tar` & `up_fmap-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 19:06:47.472422 up_fmap-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-13 19:06:38.000000 up_fmap-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-13 19:06:47.472422 up_fmap-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-13 19:06:38.000000 up_fmap-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 19:06:47.472422 up_fmap-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-13 19:06:38.000000 up_fmap-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 19:06:47.472422 up_fmap-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-02-13 19:06:38.000000 up_fmap-0.0.2/test/test_up_fmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 19:06:47.472422 up_fmap-0.0.2/up_fmap/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-13 19:06:38.000000 up_fmap-0.0.2/up_fmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-02-13 19:06:38.000000 up_fmap-0.0.2/up_fmap/fmap_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 19:06:47.472422 up_fmap-0.0.2/up_fmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-13 19:06:47.000000 up_fmap-0.0.2/up_fmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-13 19:06:47.000000 up_fmap-0.0.2/up_fmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 19:06:47.000000 up_fmap-0.0.2/up_fmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-13 19:06:47.000000 up_fmap-0.0.2/up_fmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 10:39:05.000000 up_fmap-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:39:17.111011 up_fmap-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-18 10:39:05.000000 up_fmap-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:39:17.111011 up_fmap-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-18 10:39:05.000000 up_fmap-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-04-18 10:39:05.000000 up_fmap-0.0.3/test/test_up_fmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/up_fmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 10:39:05.000000 up_fmap-0.0.3/up_fmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-18 10:39:05.000000 up_fmap-0.0.3/up_fmap/fmap_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:39:17.111011 up_fmap-0.0.3/up_fmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 10:39:17.000000 up_fmap-0.0.3/up_fmap.egg-info/top_level.txt
```

### Comparing `up_fmap-0.0.2/LICENSE` & `up_fmap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.2/README.md` & `up_fmap-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `up_fmap-0.0.2/setup.py` & `up_fmap-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def run(self):
         install_FMAP()
         develop.run(self)
 
 
 setup(
     name="up_fmap",
-    version="0.0.2",
+    version="0.0.3",
     description="up_fmap",
     author="Alejandro Torreño, Eva Onaindia and Oscar Sapena",
     author_email="onaindia@dsic.upv.es",
     packages=["up_fmap"],
     package_data={"": ["FMAP/FMAP.jar"]},
     cmdclass={"build_py": InstallFMAP, "develop": InstallFMAPdevelop},
     license="APACHE",
```

### Comparing `up_fmap-0.0.2/test/test_up_fmap.py` & `up_fmap-0.0.3/test/test_up_fmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unified_planning.shortcuts import *  # type: ignore
 from unified_planning.model.multi_agent import *  # type: ignore
 from collections import namedtuple  # type: ignore
 from unified_planning.io.ma_pddl_writer import MAPDDLWriter  # type: ignore
+from unified_planning.plans import PlanKind  # type: ignore
 from unittest import TestCase, main
 import pkg_resources
 from up_fmap import FMAPsolver
 
 # from ma_depot import get_example_problems  # type: ignore
 
 # Example = namedtuple("Example", ["problem", "plan"])
@@ -233,13 +234,13 @@
         problem.add_goal(on(crate1, pallet1))
 
         with OneshotPlanner(name="fmap") as planner:
             result = planner.solve(problem)
             print("%s returned: %s" % (planner.name, result))
             print(
                 "%s returned Sequential Plan: %s"
-                % (planner.name, result.plan.to_sequential_plan())
+                % (planner.name, result.plan.convert_to(PlanKind.SEQUENTIAL_PLAN, problem))
             )
 
         with OneshotPlanner(name="fmap") as planner:
             result = planner.solve(problem)
             self.assertEqual(result.status.name, "SOLVED_SATISFICING")
```

### Comparing `up_fmap-0.0.2/up_fmap/fmap_planner.py` & `up_fmap-0.0.3/up_fmap/fmap_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pkg_resources  # type: ignore
 import unified_planning as up  # type: ignore
 from unified_planning.model import ProblemKind  # type: ignore
-from unified_planning.engines import PDDLPlanner, Credits, LogMessage  # type: ignore
+from unified_planning.engines import Engine, Credits, LogMessage  # type: ignore
+from unified_planning.engines.mixins import OneshotPlannerMixin  # type: ignore
 from typing import Callable, Dict, IO, List, Optional, Set, Union, cast  # type: ignore
 from unified_planning.io.ma_pddl_writer import MAPDDLWriter  # type: ignore
 import tempfile
 import os
 import subprocess
 import sys
 import asyncio
@@ -32,19 +33,20 @@
     "https://bitbucket.org/altorler/fmap/src/master/",
     "GPL",
     "FMAP: A Platform for the Development of Distributed Multi-Agent Planning Systems.",
     "FMAP uses a distributed heuristic search strategy. Each planning agent in the platform features an embedded search engine based on a forward partial-order planning scheme. ",
 )
 
 
-class FMAPsolver(PDDLPlanner):
+class FMAPsolver(Engine, OneshotPlannerMixin):
     def __init__(
         self, search_algorithm: Optional[str] = None, heuristic: Optional[str] = None
     ):
-        super().__init__(needs_requirements=False)
+        Engine.__init__(self)
+        OneshotPlannerMixin.__init__(self)
         self.search_algorithm = search_algorithm
         self.heuristic = heuristic
 
     @property
     def name(self) -> str:
         return "FMAP"
```

