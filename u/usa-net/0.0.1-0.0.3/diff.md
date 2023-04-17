# Comparing `tmp/usa-net-0.0.1.tar.gz` & `tmp/usa-net-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usa-net-0.0.1.tar", last modified: Thu Apr 13 03:18:49 2023, max compression
+gzip compressed data, was "usa-net-0.0.3.tar", last modified: Mon Apr 17 22:08:46 2023, max compression
```

## Comparing `usa-net-0.0.1.tar` & `usa-net-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.039946 usa-net-0.0.1/
--rw-r--r--   0 bbolte     (501) staff       (20)      100 2023-04-13 03:15:19.000000 usa-net-0.0.1/MANIFEST.in
--rw-r--r--   0 bbolte     (501) staff       (20)      266 2023-04-13 03:18:49.040052 usa-net-0.0.1/PKG-INFO
--rw-r--r--   0 bbolte     (501) staff       (20)       33 2023-04-13 00:38:27.000000 usa-net-0.0.1/README.md
--rw-r--r--   0 bbolte     (501) staff       (20)     1435 2023-04-13 02:04:20.000000 usa-net-0.0.1/pyproject.toml
--rw-r--r--   0 bbolte     (501) staff       (20)       90 2023-04-13 02:28:04.000000 usa-net-0.0.1/requirements-dev.txt
--rw-r--r--   0 bbolte     (501) staff       (20)      220 2023-04-13 03:18:36.000000 usa-net-0.0.1/requirements.txt
--rw-r--r--   0 bbolte     (501) staff       (20)      195 2023-04-13 03:18:49.040612 usa-net-0.0.1/setup.cfg
--rw-r--r--   0 bbolte     (501) staff       (20)      878 2023-04-13 03:15:54.000000 usa-net-0.0.1/setup.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.007326 usa-net-0.0.1/tests/
--rw-r--r--   0 bbolte     (501) staff       (20)       42 2023-04-13 00:37:55.000000 usa-net-0.0.1/tests/test_dummy.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.008605 usa-net-0.0.1/usa/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 00:34:42.000000 usa-net-0.0.1/usa/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)        6 2023-04-13 03:15:23.000000 usa-net-0.0.1/usa/__version__.txt
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.013557 usa-net-0.0.1/usa/evaluation/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 02:20:52.000000 usa-net-0.0.1/usa/evaluation/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)    11015 2023-04-13 02:30:13.000000 usa-net-0.0.1/usa/evaluation/path_length.py
--rw-r--r--   0 bbolte     (501) staff       (20)    13031 2023-04-13 02:30:07.000000 usa-net-0.0.1/usa/evaluation/semantics.py
--rw-r--r--   0 bbolte     (501) staff       (20)     9959 2023-04-13 02:57:07.000000 usa-net-0.0.1/usa/evaluation/trajectories.py
--rw-r--r--   0 bbolte     (501) staff       (20)     9730 2023-04-13 02:51:00.000000 usa-net-0.0.1/usa/evaluation/utils.py
--rw-r--r--   0 bbolte     (501) staff       (20)     5023 2023-04-13 02:40:12.000000 usa-net-0.0.1/usa/evaluation/visualize_semantics.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.017779 usa-net-0.0.1/usa/models/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 00:34:42.000000 usa-net-0.0.1/usa/models/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)    37431 2023-04-13 02:03:02.000000 usa-net-0.0.1/usa/models/clip.py
--rw-r--r--   0 bbolte     (501) staff       (20)     2916 2023-04-13 02:59:38.000000 usa-net-0.0.1/usa/models/point2emb.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.024395 usa-net-0.0.1/usa/planners/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 02:20:52.000000 usa-net-0.0.1/usa/planners/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)     6750 2023-04-13 02:24:02.000000 usa-net-0.0.1/usa/planners/base.py
--rw-r--r--   0 bbolte     (501) staff       (20)    16759 2023-04-13 02:56:35.000000 usa-net-0.0.1/usa/planners/clip_sdf.py
--rw-r--r--   0 bbolte     (501) staff       (20)     8553 2023-04-13 02:54:14.000000 usa-net-0.0.1/usa/planners/common.py
--rw-r--r--   0 bbolte     (501) staff       (20)     4101 2023-04-13 02:54:23.000000 usa-net-0.0.1/usa/planners/occupancy_map.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.025640 usa-net-0.0.1/usa/scripts/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 00:34:42.000000 usa-net-0.0.1/usa/scripts/__init__.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.027041 usa-net-0.0.1/usa/scripts/adhoc/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 00:41:36.000000 usa-net-0.0.1/usa/scripts/adhoc/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)     1602 2023-04-13 00:40:59.000000 usa-net-0.0.1/usa/scripts/adhoc/distribution_estimates.py
--rw-r--r--   0 bbolte     (501) staff       (20)      222 2023-04-13 00:34:42.000000 usa-net-0.0.1/usa/scripts/cli.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.028076 usa-net-0.0.1/usa/tasks/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 00:34:42.000000 usa-net-0.0.1/usa/tasks/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)    12857 2023-04-13 02:09:03.000000 usa-net-0.0.1/usa/tasks/clip_sdf.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.034457 usa-net-0.0.1/usa/tasks/datasets/
--rw-r--r--   0 bbolte     (501) staff       (20)        0 2023-04-13 02:03:37.000000 usa-net-0.0.1/usa/tasks/datasets/__init__.py
--rw-r--r--   0 bbolte     (501) staff       (20)     3400 2023-04-13 02:08:19.000000 usa-net-0.0.1/usa/tasks/datasets/home_robot.py
--rw-r--r--   0 bbolte     (501) staff       (20)     8636 2023-04-13 02:57:06.000000 usa-net-0.0.1/usa/tasks/datasets/posed_rgbd.py
--rw-r--r--   0 bbolte     (501) staff       (20)    11368 2023-04-13 02:16:03.000000 usa-net-0.0.1/usa/tasks/datasets/r3d.py
--rw-r--r--   0 bbolte     (501) staff       (20)     5825 2023-04-13 02:16:05.000000 usa-net-0.0.1/usa/tasks/datasets/replica_cad.py
--rw-r--r--   0 bbolte     (501) staff       (20)     7203 2023-04-13 02:10:26.000000 usa-net-0.0.1/usa/tasks/datasets/stretch.py
--rw-r--r--   0 bbolte     (501) staff       (20)     1992 2023-04-13 02:05:34.000000 usa-net-0.0.1/usa/tasks/datasets/types.py
--rw-r--r--   0 bbolte     (501) staff       (20)    13394 2023-04-13 02:09:56.000000 usa-net-0.0.1/usa/tasks/datasets/utils.py
-drwxr-xr-x   0 bbolte     (501) staff       (20)        0 2023-04-13 03:18:49.039241 usa-net-0.0.1/usa_net.egg-info/
--rw-r--r--   0 bbolte     (501) staff       (20)      266 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/PKG-INFO
--rw-r--r--   0 bbolte     (501) staff       (20)     1109 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/SOURCES.txt
--rw-r--r--   0 bbolte     (501) staff       (20)        1 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/dependency_links.txt
--rw-r--r--   0 bbolte     (501) staff       (20)       51 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/entry_points.txt
--rw-r--r--   0 bbolte     (501) staff       (20)      273 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/requires.txt
--rw-r--r--   0 bbolte     (501) staff       (20)        4 2023-04-13 03:18:48.000000 usa-net-0.0.1/usa_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 22:08:34.000000 usa-net-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 22:08:46.440763 usa-net-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 22:08:34.000000 usa-net-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-17 22:08:34.000000 usa-net-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:08:34.000000 usa-net-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 22:08:34.000000 usa-net-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 22:08:46.440763 usa-net-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-17 22:08:34.000000 usa-net-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 22:08:34.000000 usa-net-0.0.3/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/__version__.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/evaluation/visualize_semantics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/models/point2emb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/planners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/clip_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/planners/occupancy_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/scripts/adhoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/adhoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/adhoc/distribution_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.436763 usa-net-0.0.3/usa/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/clip_sdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/usa/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/home_robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/posed_rgbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/r3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/replica_cad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-04-17 22:08:34.000000 usa-net-0.0.3/usa/tasks/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:08:46.440763 usa-net-0.0.3/usa_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 22:08:46.000000 usa-net-0.0.3/usa_net.egg-info/top_level.txt
```

### Comparing `usa-net-0.0.1/pyproject.toml` & `usa-net-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "liblzfse.*",
     "matplotlib.*",
     "open3d.*",
     "pandas.*",
     "PIL.*",
     "pytest.*",
     "quaternion.*",
-    "scipy.*",
     "seaborn.*",
     "torchvision.*",
     "tqdm.*",
 ]
 
 ignore_missing_imports = true
```

### Comparing `usa-net-0.0.1/setup.py` & `usa-net-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.1/usa/evaluation/path_length.py` & `usa-net-0.0.3/usa/evaluation/path_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import argparse
 import bdb
 import csv
 import logging
 import math
 import os
 from pathlib import Path
-from typing import List, Tuple
 
 import matplotlib.pyplot as plt
 import ml.api as ml
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 from usa.evaluation.utils import EvalSet, get_planners, plot_map, plot_paths
 from usa.planners.base import Map
 
 logger = logging.getLogger(__name__)
 
-PathStartEndCoords = List[Tuple[Tuple[float, float], Tuple[float, float]]]
+PathStartEndCoords = list[tuple[tuple[float, float], tuple[float, float]]]
 
 
-def not_in_line_of_sight(planner_map: Map, xy: np.ndarray, start_xy: Tuple[float, float]) -> np.ndarray:
+def not_in_line_of_sight(planner_map: Map, xy: np.ndarray, start_xy: tuple[float, float]) -> np.ndarray:
     """Gets a mask of the points which aren't in line-of-sight from the start.
 
     Args:
         planner_map: The occupancy map
         xy: The XZ coordinates of the points
         start_xy: The XZ coordinates of the start point
 
     Returns:
         A mask of the points which aren't in line-of-sight from the start.
     """
 
-    def is_line_of_sight(start_xy: Tuple[float, float], end_xy: Tuple[float, float]) -> bool:
+    def is_line_of_sight(start_xy: tuple[float, float], end_xy: tuple[float, float]) -> bool:
         start_pt = planner_map.to_pt(start_xy)
         end_pt = planner_map.to_pt(end_xy)
 
         if start_pt == end_pt:
             return True
 
         dx = end_pt[0] - start_pt[0]
@@ -74,15 +73,15 @@
 
 def get_eval_set(
     name: str,
     save_dir: Path,
     num_paths: int = 100,
     min_path_euclid_mul: float = 0.1,
     filter_line_of_sight_points: bool = True,
-) -> Tuple[EvalSet, PathStartEndCoords]:
+) -> tuple[EvalSet, PathStartEndCoords]:
     """Gets the evaluation set for a clip recorded with the Stretch robot.
 
     Args:
         name: The name of the evaluation set.
         save_dir: The directory to save the evaluation set to.
         num_paths: The number of paths to evaluate
         min_path_euclid_mul: The minimum euclidean distance between the start
@@ -195,15 +194,15 @@
         path_dir.mkdir(parents=True, exist_ok=True)
 
         with open(path_dir / "lengths.csv", "w", encoding="utf-8") as f:
             lengths_writer = csv.writer(f, delimiter=",")
             lengths_writer.writerow(["start_x", "start_y", "end_x", "end_y", "path_length"])
 
             planner_map = planner.get_map()
-            paths: List[List[Tuple[float, float]]] = []
+            paths: list[list[tuple[float, float]]] = []
 
             for i, (start, end) in enumerate(path_coords):
                 try:
                     path = planner.plan(start, end)
 
                     # Checks that path start and end are correct.
                     assert np.allclose(path[0], start, atol=1e-3), f"Path start is incorrect: {path[0]} != {start}"
```

### Comparing `usa-net-0.0.1/usa/evaluation/semantics.py` & `usa-net-0.0.3/usa/evaluation/semantics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 import argparse
 import bdb
 import csv
 import logging
 import os
 from pathlib import Path
-from typing import Iterator, List, Tuple
+from typing import Iterator
 
+import ml.api as ml
 import numpy as np
 import open3d as o3d
 import pandas as pd
 import torch
-from ml.utils.logging import configure_logging
-from ml.utils.random import set_random_seed
 
 from usa.evaluation.utils import EvalSet, get_planners, plot_paths
 from usa.planners.clip_sdf import ClipSdfPlanner
 from usa.tasks.datasets.utils import (
     make_point_cloud_from_dataset,
     make_video_from_dataset,
 )
 
 logger = logging.getLogger(__name__)
 
-PathStartCoordsAndGoal = List[Tuple[Tuple[float, float], str]]
+PathStartCoordsAndGoal = list[tuple[tuple[float, float], str]]
 
 
 def get_eval_set(
     name: str,
-    queries: List[str],
+    queries: list[str],
     rotate: bool = False,
     concat_horizontal: bool = False,
-) -> Tuple[EvalSet, PathStartCoordsAndGoal]:
+) -> tuple[EvalSet, PathStartCoordsAndGoal]:
     """Gets the evaluation set for a clip recorded with the Stretch robot.
 
     Args:
         name: The name of the evaluation set.
         queries: The queries to use for the.
         rotate: If the video should be rotated.
         concat_horizontal: If the video should be concatenated horizontally.
 
     Returns:
         The evaluation set for evaluating the path length, along with the
         start coordinates and goal.
     """
 
     # Seed everything for reproducibility.
-    set_random_seed(1337)
+    ml.set_random_seed(1337)
 
     planners, dataset, poses = get_planners(name, False)
 
     # Gets the XZ coordinates (remember, using the camera frame, so Z is
     # forward while X is right).
     xs, ys = poses[:, 0, 3], poses[:, 1, 3]
     xy = np.stack([xs, ys], axis=1)
@@ -77,15 +76,15 @@
         concat_horizontal=concat_horizontal,
     )
 
     return eval_set, start_xy_list
 
 
 def evaluate(eval_set: EvalSet, path_coords: PathStartCoordsAndGoal, eval_set_dir: Path) -> None:
-    configure_logging(use_tqdm=True)
+    ml.configure_logging(use_tqdm=True)
 
     # Setting this for the optimizer.
     os.environ["USE_FP64"] = "1"
 
     logger.info("Evaluating %s on %d paths", eval_set.name, len(path_coords))
 
     # Makes a new directory for running the evaluation.
@@ -137,15 +136,15 @@
         o3d.io.write_point_cloud(str(path_point_cloud_path), path_point_cloud)
     logger.info("Path point cloud path: %s", path_point_cloud_path)
 
     def clean_goal(goal: str) -> str:
         # Converts a generic goal string into a string to use as a file name.
         return goal.replace(" ", "_").replace("/", "_").lower()
 
-    def interpolate_path(path: List[Tuple[float, float]], resolution: float) -> Iterator[Tuple[float, float]]:
+    def interpolate_path(path: list[tuple[float, float]], resolution: float) -> Iterator[tuple[float, float]]:
         for i in range(len(path) - 1):
             start = path[i]
             end = path[i + 1]
             num_points = int(np.linalg.norm(np.array(start) - np.array(end)) / resolution) + 1
             for t in np.linspace(0, 1, num_points):
                 yield (1 - t) * start[0] + t * end[0], (1 - t) * start[1] + t * end[1]
 
@@ -163,15 +162,15 @@
             path_dir.mkdir(parents=True, exist_ok=True)
 
             with open(path_dir / "lengths.csv", "w", encoding="utf-8") as f:
                 lengths_writer = csv.writer(f, delimiter=",")
                 lengths_writer.writerow(["start_x", "start_y", "goal", "path_length"])
 
                 planner_map = planner.get_map()
-                paths: List[List[Tuple[float, float]]] = []
+                paths: list[list[tuple[float, float]]] = []
 
                 for start, goal in path_coords:
                     try:
                         path = planner.plan(start, end_goal=goal)
 
                         # Checks that path start and end are correct.
                         assert np.allclose(path[0], start, atol=1e-3), f"Path start is incorrect: {path[0]} != {start}"
@@ -246,15 +245,15 @@
     Usage:
         python -m ml.evaluation.evaluations.semantics
 
     Raises:
         KeyError: If the evaluation set is not found.
     """
 
-    configure_logging(use_tqdm=True)
+    ml.configure_logging(use_tqdm=True)
 
     parser = argparse.ArgumentParser(description="Runs semantic evaluation.")
     parser.add_argument("key", help="The evaluation key to use")
     parser.add_argument("save_dir", help="Where to save results")
     parser.add_argument("-n", "--num-paths", type=int, default=100, help="Maximum number of paths to evaluate")
     parser.add_argument("-e", "--min-euclid-mul", type=float, default=0.1, help="Minimum path distance multipler")
     args = parser.parse_args()
```

### Comparing `usa-net-0.0.1/usa/evaluation/trajectories.py` & `usa-net-0.0.3/usa/evaluation/trajectories.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import argparse
 import logging
 import os
 from pathlib import Path
-from typing import List, Literal, Optional, Tuple, Type, cast, get_args
+from typing import Literal, Type, cast, get_args
 
+import ml.api as ml
 import numpy as np
 import open3d as o3d
-from ml.trainers.mixins.device.auto import AutoDevice
-from ml.trainers.mixins.device.base import BaseDevice
-from ml.utils.logging import configure_logging
 from torch.utils.data.dataset import Dataset
 
 from usa.evaluation.utils import load_clip_sdf_model_from_ckpt_and_config, plot_paths
 from usa.models.point2emb import Point2EmbModel
 from usa.planners.base import Planner
 from usa.planners.clip_sdf import (
     AStarPlanner as AStarClipSDFPlanner,
@@ -27,17 +25,17 @@
 PlannerType = Literal["a_star", "gradient"]
 
 
 def get_planner(
     model: Point2EmbModel,
     task: ClipSdfTask,
     planner_key: PlannerType,
-    floor_ceil_heights: Tuple[float, float],
-    device: Type[BaseDevice],
-    dataset: Optional[Dataset[PosedRGBDItem]] = None,
+    floor_ceil_heights: tuple[float, float],
+    device: Type[ml.BaseDevice],
+    dataset: Dataset[PosedRGBDItem] | None = None,
 ) -> Planner:
     if dataset is None:
         dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
     floor_height, ceil_height = floor_ceil_heights
 
     if planner_key == "a_star":
         return AStarClipSDFPlanner(
@@ -63,27 +61,27 @@
             ceil_height=ceil_height,
         )
 
     raise NotImplementedError(f"Planner {planner_key} is not implemented.")
 
 
 def print_trajectories(
-    start_xy: Tuple[float, float],
-    goals: List[str],
+    start_xy: tuple[float, float],
+    goals: list[str],
     planner: Planner,
-    floor_ceil_heights: Tuple[float, float],
-    artifacts_dir: Optional[Path] = None,
-    dataset: Optional[Dataset[PosedRGBDItem]] = None,
+    floor_ceil_heights: tuple[float, float],
+    artifacts_dir: Path | None = None,
+    dataset: Dataset[PosedRGBDItem] | None = None,
     save_goals: bool = True,
 ) -> None:
     start_x, start_y = start_xy
     if not planner.is_valid_starting_point((start_x, start_y)):
         logger.warning("Starting point %s is not valid!", start_xy)
 
-    all_trajectories: List[List[Tuple[float, float]]] = []
+    all_trajectories: list[list[tuple[float, float]]] = []
     for goal in goals:
         trajectory = planner.plan(start_xy, end_goal=goal)
         start_xy = trajectory[-1]
         all_trajectories.append(trajectory)
         logger.info("Goal: %s", goal)
         logger.info("Trajectory: %s", trajectory)
 
@@ -150,15 +148,15 @@
             flat_trajectories = [point for trajectory in all_trajectories for point in trajectory]
             traj_point_cloud = o3d.geometry.PointCloud()
             traj_point_cloud.points = o3d.utility.Vector3dVector([(x, y, halfh) for x, y in flat_trajectories])
             traj_point_cloud.colors = o3d.utility.Vector3dVector([[1, 0, 0] for _ in flat_trajectories])
             point_cloud += traj_point_cloud
 
             # Adds the map.
-            planner_map_occupied: List[Tuple[float, float]] = []
+            planner_map_occupied: list[tuple[float, float]] = []
             ymax, xmax = planner_map.grid.shape[:2]
             for x in range(xmax):
                 for y in range(ymax):
                     if planner_map.is_occupied((x, y)):
                         xy = planner_map.to_xy((x, y))
                         planner_map_occupied.append(xy)
             map_point_cloud = o3d.geometry.PointCloud()
@@ -177,15 +175,15 @@
     Note that the goal locations need to be separated by a semicolon because
     of how argparse interprets strings.
 
     See `scripts/get_trajectories_demo.sh` for an example of how to use this
     script.
     """
 
-    configure_logging(use_tqdm=True)
+    ml.configure_logging(use_tqdm=True)
 
     parser = argparse.ArgumentParser(description="Get trajectories for a trained model.")
     parser.add_argument(
         "--planner",
         type=str,
         choices=get_args(PlannerType),
         default="gradient",
@@ -236,28 +234,28 @@
         help="The path to the directory to save artifacts to.",
         required=False,
     )
     args = parser.parse_args()
 
     # Gets the device (GPU, CPU, Metal...)
     os.environ["USE_FP64"] = "1"
-    device = AutoDevice.detect_device()
+    device = ml.AutoDevice.detect_device()
 
     # Loads the model from the model root.
     ckpt_path, config_path = Path(args.ckpt_path), Path(args.config_path)
     model, task = load_clip_sdf_model_from_ckpt_and_config(ckpt_path, config_path, device)
 
     # Gets the dataset and planner from the given model.
     floor_ceil_heights = float(args.floor_height), float(args.ceil_height)
     dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
     planner = get_planner(model, task, cast(PlannerType, args.planner), floor_ceil_heights, device, dataset)
 
     # Gets the starting XY coordinates, the goal locations and the artifacts directory from arguments.
     start_xy = float(args.xy[0]), float(args.xy[1])
-    goals = cast(List[str], args.goals.split(";"))
+    goals = cast(list[str], args.goals.split(";"))
     artifacts_dir = Path(args.artifacts_dir) if args.artifacts_dir else None
 
     print_trajectories(start_xy, goals, planner, floor_ceil_heights, artifacts_dir, dataset)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `usa-net-0.0.1/usa/evaluation/utils.py` & `usa-net-0.0.3/usa/evaluation/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, List, Tuple, Type, cast
+from typing import Type, cast
 
 import matplotlib.pyplot as plt
 import ml.api as ml
 import numpy as np
 import torch
-from ml.trainers.mixins.device.base import BaseDevice
 from omegaconf import OmegaConf
 from torch.utils.data.dataset import Dataset
 
 from usa.models.point2emb import Point2EmbModel
 from usa.planners.base import Map, Planner
 from usa.planners.clip_sdf import (
     AStarPlanner as AStarClipSDFPlanner,
@@ -25,30 +24,30 @@
 from usa.tasks.datasets.types import PosedRGBDItem
 
 
 @dataclass
 class EvalSet:
     name: str
     dataset: Dataset[PosedRGBDItem]
-    planners: Dict[str, Planner]
+    planners: dict[str, Planner]
     rotate: bool = False
     concat_horizontal: bool = False
 
 
 def get_eval_root_dir() -> Path:
     root_dir = ml.get_eval_run_dir() / "usa"
     root_dir.mkdir(parents=True, exist_ok=True)
     return root_dir
 
 
 def load_clip_sdf_model_from_ckpt_and_config(
     ckpt_path: Path,
     config_path: Path,
-    device: Type[BaseDevice],
-) -> Tuple[Point2EmbModel, ClipSdfTask]:
+    device: Type[ml.BaseDevice],
+) -> tuple[Point2EmbModel, ClipSdfTask]:
     """Loads the CLIP SDF model from the experiment path.
 
     Args:
         ckpt_path: The path to the checkpoint file.
         config_path: The path to the config file.
         device: The device to load the model on.
 
@@ -68,15 +67,15 @@
 
     device.module_to(model)
     device.module_to(task)
 
     return model, task
 
 
-def load_clip_sdf_model(exp_path: Path, device: Type[BaseDevice]) -> Tuple[Point2EmbModel, ClipSdfTask]:
+def load_clip_sdf_model(exp_path: Path, device: Type[ml.BaseDevice]) -> tuple[Point2EmbModel, ClipSdfTask]:
     """Loads the CLIP SDF model from the experiment path.
 
     Args:
         exp_path: The path to the experiment path (probably ending in something
             like "run_0/")
         device: The device to load the model on.
 
@@ -103,15 +102,15 @@
 
 
 def get_planners(
     name: str,
     use_occ_grid_planners: bool,
     floor_height: float = 0.1,
     ceil_height: float = 1.3,
-) -> Tuple[Dict[str, Planner], Dataset[PosedRGBDItem], np.ndarray]:
+) -> tuple[dict[str, Planner], Dataset[PosedRGBDItem], np.ndarray]:
     """Returns the planners for a given evaluation set.
 
     Args:
         name: The name of the evaluation set.
         use_occ_grid_planners: If the occupancy grid planners should be used.
         floor_height: The height of the floor.
         ceil_height: The height of the ceiling.
@@ -145,15 +144,15 @@
 
     model, task = load_clip_sdf_model(clip_sdf_exp_path, device)
     dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
 
     # Cache to the experiment directory.
     base_cache_dir = clip_sdf_exp_path / "eval_cache" / "semantics" / name
 
-    planners: Dict[str, Planner] = {
+    planners: dict[str, Planner] = {
         "a_star_10_cm_clip_sdf": AStarClipSDFPlanner(
             dataset,
             model,
             task,
             device,
             "euclidean",
             resolution=0.1,
@@ -246,15 +245,15 @@
     poses = get_poses(dataset, base_cache_dir)
 
     return planners, dataset, poses
 
 
 def plot_paths(
     planner_map: Map,
-    paths: List[List[Tuple[float, float]]],
+    paths: list[list[tuple[float, float]]],
     output_path: Path,
 ) -> None:
     """Plots a planner path and saves it to the output directory.
 
     Args:
         planner_map: The planner map.
         paths: The paths.
```

### Comparing `usa-net-0.0.1/usa/evaluation/visualize_semantics.py` & `usa-net-0.0.3/usa/evaluation/visualize_semantics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import logging
 import os
 from pathlib import Path
-from typing import List, Tuple, Type, cast
+from typing import Type, cast
 
 import ml.api as ml
 import numpy as np
 import open3d as o3d
 from torch.utils.data.dataset import Dataset
 
 from usa.evaluation.utils import load_clip_sdf_model_from_ckpt_and_config
@@ -19,17 +19,17 @@
 logger = logging.getLogger(__name__)
 
 
 def visualize_semantics(
     model: Point2EmbModel,
     task: ClipSdfTask,
     device: Type[ml.BaseDevice],
-    floor_ceil_heights: Tuple[float, float],
+    floor_ceil_heights: tuple[float, float],
     dataset: Dataset[PosedRGBDItem],
-    goals: List[str],
+    goals: list[str],
     artifacts_dir: Path,
     resolution: float,
 ) -> None:
     floor_height, ceil_height = floor_ceil_heights
 
     planner = GradientClipSDFPlanner(
         dataset,
@@ -143,15 +143,15 @@
 
     # Gets the dataset.
     floor_ceil_heights = float(args.floor_height), float(args.ceil_height)
     dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
 
     # Gets the resolution, goal locations and artifacts directory from arguments.
     resolution = float(args.resolution)
-    goals = cast(List[str], args.goals.split(";"))
+    goals = cast(list[str], args.goals.split(";"))
     artifacts_dir = Path(args.artifacts_dir)
 
     visualize_semantics(model, task, device, floor_ceil_heights, dataset, goals, artifacts_dir, resolution)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `usa-net-0.0.1/usa/models/clip.py` & `usa-net-0.0.3/usa/models/clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,15 @@
 import functools
 import gzip
 import html
 import os
 import re
 from collections import OrderedDict
 from pathlib import Path
-from typing import (
-    Any,
-    Dict,
-    List,
-    Literal,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-    cast,
-    get_args,
-    overload,
-)
+from typing import Any, Literal, cast, get_args, overload
 
 import ftfy
 import ml.api as ml
 import numpy as np
 import torch
 import torch.nn.functional as F
 import torchvision
@@ -54,15 +42,15 @@
 
 def cast_pretrained_model_key(s: str) -> PretrainedModel:
     args = get_args(PretrainedModel)
     assert s in args, f"Invalid pretraiend model key: '{s}' Valid options are {args}"
     return cast(PretrainedModel, s)
 
 
-PRETRAINED_MODELS: Dict[PretrainedModel, str] = {
+PRETRAINED_MODELS: dict[PretrainedModel, str] = {
     "RN50": f"{URL_PREFIX}/afeb0e10f9e5a86da6080e35cf09123aca3b358a0c3e3b6c78a7b63bc04b6762/RN50.pt",
     "RN101": f"{URL_PREFIX}/8fa8567bab74a42d41c5915025a8e4538c3bdbe8804a470a72f30b0d94fab599/RN101.pt",
     "RN50x4": f"{URL_PREFIX}/7e526bd135e493cef0776de27d5f42653e6b4c8bf9e0f653bb11773263205fdd/RN50x4.pt",
     "RN50x16": f"{URL_PREFIX}/52378b407f34354e150460fe41077663dd5b39c54cd0bfd2b27167a4a06ec9aa/RN50x16.pt",
     "RN50x64": f"{URL_PREFIX}/be1cfb55d75a9666199fb2206c106743da0f6468c9d327f3e0d0a543a9919d9c/RN50x64.pt",
     "ViT_B_32": f"{URL_PREFIX}/40d365715913c9da98579312b702a82c18be219cc2a73407c4526f58eba950af/ViT-B-32.pt",
     "ViT_B_16": f"{URL_PREFIX}/5806e77cd80f8b59890b7e101eabd078d9fb84e6937f9e85e4ecb61988df416f/ViT-B-16.pt",
@@ -92,15 +80,15 @@
 
 @functools.lru_cache()
 def default_bpe() -> str:
     return os.path.join(os.path.dirname(os.path.abspath(__file__)), "bpe_simple_vocab_16e6.txt.gz")
 
 
 @functools.lru_cache()
-def bytes_to_unicode() -> Dict[int, str]:
+def bytes_to_unicode() -> dict[int, str]:
     """Returns list of utf-8 byte and a corresponding list of unicode strings.
 
     The reversible bpe codes work on unicode strings. This means you need a
     large # of unicode characters in your vocab if you want to avoid UNKs.
     When you're at something like a 10B token dataset you end up needing around
     5K for decent coverage. This is a signficant percentage of your normal,
     say, 32K bpe vocab. To avoid that, we want lookup tables between utf-8
@@ -121,15 +109,15 @@
             bs.append(b)
             cs.append(2**8 + n)
             n += 1
     css = [chr(n) for n in cs]
     return dict(zip(bs, css))
 
 
-def get_pairs(word: Tuple[str, ...]) -> Set[Tuple[str, str]]:
+def get_pairs(word: tuple[str, ...]) -> set[tuple[str, str]]:
     pairs = set()
     prev_char = word[0]
     for char in word[1:]:
         pairs.add((prev_char, char))
         prev_char = char
     return pairs
 
@@ -181,15 +169,15 @@
             return token + "</w>"
 
         while True:
             bigram = min(pairs, key=lambda pair: self.bpe_ranks.get(pair, float("inf")))
             if bigram not in self.bpe_ranks:
                 break
             first, second = bigram
-            new_word_list: List[str] = []
+            new_word_list: list[str] = []
             i = 0
             while i < len(word):
                 try:
                     j = word.index(first, i)
                     new_word_list.extend(word[i:j])
                     i = j
                 except Exception:
@@ -207,30 +195,30 @@
             if len(word) == 1:
                 break
             pairs = get_pairs(word)
         word_str = " ".join(word)
         self.cache[token] = word_str
         return word_str
 
-    def encode(self, text: str) -> List[int]:
-        bpe_tokens: List[int] = []
+    def encode(self, text: str) -> list[int]:
+        bpe_tokens: list[int] = []
         text = whitespace_clean(basic_clean(text)).lower()
         for token in re.findall(self.pat, text):
             token = "".join(self.byte_encoder[b] for b in token.encode("utf-8"))
             bpe_tokens.extend(self.encoder[bpe_token] for bpe_token in self.bpe(token).split(" "))
         return bpe_tokens
 
-    def decode(self, tokens: List[int]) -> str:
+    def decode(self, tokens: list[int]) -> str:
         text = "".join([self.decoder[token] for token in tokens])
         text = bytearray([self.byte_decoder[c] for c in text]).decode("utf-8", errors="replace").replace("</w>", " ")
         return text
 
     def tokenize(
         self,
-        texts: Union[str, List[str]],
+        texts: str | list[str],
         context_length: int = 77,
         truncate: bool = False,
     ) -> Tensor:
         if isinstance(texts, str):
             texts = [texts]
 
         sot_token = self.encoder["<|startoftext|>"]
@@ -258,16 +246,16 @@
 
     def __init__(
         self,
         inplanes: int,
         planes: int,
         stride: int = 1,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         # all conv layers have stride 1. an avgpool is performed after the second convolution when stride > 1
         self.conv1 = nn.Conv2d(inplanes, planes, 1, bias=False, device=device, dtype=dtype)
         self.bn1 = nn.BatchNorm2d(planes, device=device, dtype=dtype)
         self.relu1 = nn.ReLU(inplace=True)
@@ -310,18 +298,18 @@
 
 class AttentionPool2d(nn.Module):
     def __init__(
         self,
         spacial_dim: int,
         embed_dim: int,
         num_heads: int,
-        output_dim: Optional[int] = None,
+        output_dim: int | None = None,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         if dtype is None:
             pos_emb = torch.randn(spacial_dim**2 + 1, embed_dim, device=device) / embed_dim**0.5
         else:
             pos_emb = torch.randn(spacial_dim**2 + 1, embed_dim, device=device, dtype=dtype) / embed_dim**0.5
@@ -361,22 +349,22 @@
 
 
 class ModifiedResNet(nn.Module):
     __constants__ = ["input_resolution", "output_dim"]
 
     def __init__(
         self,
-        layers: Tuple[int, int, int, int],
+        layers: tuple[int, int, int, int],
         output_dim: int,
         heads: int,
         input_resolution: int = 224,
         width: int = 64,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         """ResNet class that is similar to TorchVision's but with some changes.
 
         - There are now 3 "stem" convolutions as opposed to 1, with an average
           pool instead of a max pool.
         - Performs anti-aliasing strided convolutions, where an avgpool is
           prepended to convolutions with stride > 1
@@ -490,18 +478,18 @@
 
 
 class ResidualAttentionBlock(nn.Module):
     def __init__(
         self,
         d_model: int,
         n_head: int,
-        attn_mask: Optional[Tensor] = None,
+        attn_mask: Tensor | None = None,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         self.attn = nn.MultiheadAttention(d_model, n_head, device=device, dtype=dtype)
         self.ln_1 = nn.LayerNorm(d_model, device=device, dtype=dtype)
         self.mlp = nn.Sequential(
             OrderedDict(
@@ -527,18 +515,18 @@
 
 class Transformer(nn.Module):
     def __init__(
         self,
         width: int,
         layers: int,
         heads: int,
-        attn_mask: Optional[Tensor] = None,
+        attn_mask: Tensor | None = None,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ):
         super().__init__()
         self.width = width
         self.layers = layers
         blocks = [ResidualAttentionBlock(width, heads, attn_mask, device=device, dtype=dtype) for _ in range(layers)]
         self.resblocks = nn.Sequential(*blocks)
 
@@ -554,16 +542,16 @@
         input_resolution: int,
         patch_size: int,
         width: int,
         layers: int,
         heads: int,
         output_dim: int,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         self.input_resolution = input_resolution
         self.output_dim = output_dim
         self.conv1 = nn.Conv2d(
             in_channels=3,
@@ -626,16 +614,16 @@
         embed_dim: int,
         context_length: int,
         vocab_size: int,
         transformer_width: int,
         transformer_heads: int,
         transformer_layers: int,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         self.context_length = context_length
 
         self.transformer = Transformer(
             width=transformer_width,
@@ -701,32 +689,32 @@
 
 class CLIP(nn.Module):
     def __init__(
         self,
         embed_dim: int,
         # vision
         image_resolution: int,
-        vision_layers: Union[Tuple[int, int, int, int], int],
+        vision_layers: tuple[int, int, int, int] | int,
         vision_width: int,
         vision_patch_size: int,
         # text
         context_length: int,
         vocab_size: int,
         transformer_width: int,
         transformer_heads: int,
         transformer_layers: int,
         *,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | None = None,
+        dtype: torch.dtype | None = None,
     ) -> None:
         super().__init__()
 
         self.context_length = context_length
 
-        self.visual: Union[ModifiedResNet, VisionTransformer]
+        self.visual: ModifiedResNet | VisionTransformer
         if isinstance(vision_layers, (tuple, list)):
             vision_heads = vision_width * 32 // 64
             self.visual = ModifiedResNet(
                 layers=vision_layers,
                 output_dim=embed_dim,
                 heads=vision_heads,
                 input_resolution=image_resolution,
@@ -786,15 +774,15 @@
 
     def encode_image(self, image: Tensor) -> Tensor:
         return self.visual(image)
 
     def encode_text(self, text: Tensor) -> Tensor:
         return self.linguistic(text)
 
-    def forward(self, image: Tensor, text: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(self, image: Tensor, text: Tensor) -> tuple[Tensor, Tensor]:
         image_features = self.encode_image(image)
         text_features = self.encode_text(text)
 
         # normalized features
         image_features = image_features / image_features.norm(dim=1, keepdim=True)
         text_features = text_features / text_features.norm(dim=1, keepdim=True)
 
@@ -833,52 +821,52 @@
                     attr.data = attr.data.half()
 
     model.apply(_convert_weights_to_fp16)
 
 
 @overload
 def load_pretrained(
-    key: Union[PretrainedModel, nn.Module],
+    key: PretrainedModel | nn.Module,
     mode: Literal["visual"],
     *,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
-) -> Union[ModifiedResNet, VisionTransformer]:
+    device: torch.device | None = None,
+    dtype: torch.dtype | None = None,
+) -> ModifiedResNet | VisionTransformer:
     ...
 
 
 @overload
 def load_pretrained(
-    key: Union[PretrainedModel, nn.Module],
+    key: PretrainedModel | nn.Module,
     mode: Literal["linguistic"],
     *,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
+    device: torch.device | None = None,
+    dtype: torch.dtype | None = None,
 ) -> TextModel:
     ...
 
 
 @overload
 def load_pretrained(
-    key: Union[PretrainedModel, nn.Module],
+    key: PretrainedModel | nn.Module,
     mode: Literal["all"],
     *,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
+    device: torch.device | None = None,
+    dtype: torch.dtype | None = None,
 ) -> CLIP:
     ...
 
 
 def load_pretrained(
-    key: Union[PretrainedModel, nn.Module],
+    key: PretrainedModel | nn.Module,
     mode: str,
     *,
-    device: Optional[torch.device] = None,
-    dtype: Optional[torch.dtype] = None,
-) -> Union[CLIP, ModifiedResNet, VisionTransformer, TextModel]:
+    device: torch.device | None = None,
+    dtype: torch.dtype | None = None,
+) -> CLIP | ModifiedResNet | VisionTransformer | TextModel:
     """Builds the CLIP model from a state dictionary.
 
     Args:
         key: The model key to load, or another model to load weights from
         mode: Default is to return all models, but can optionally return just
             the visual or linguistic part of the model
         device: The device for the model
@@ -894,24 +882,24 @@
         ckpt = key.state_dict()
     else:
         filepath = get_pretrained_path(key)
         ckpt = torch.jit.load(filepath, map_location="cpu").state_dict()
 
     vit = "visual.proj" in ckpt
 
-    vision_layers: Union[Tuple[int, int, int, int], int]
+    vision_layers: tuple[int, int, int, int] | int
     if vit:
         vision_width = ckpt["visual.conv1.weight"].shape[0]
         vision_layers = sum(1 for k in ckpt.keys() if k.startswith("visual.") and k.endswith(".attn.in_proj_weight"))
         vision_patch_size = ckpt["visual.conv1.weight"].shape[-1]
         grid_size = round((ckpt["visual.positional_embedding"].shape[0] - 1) ** 0.5)
         image_resolution = vision_patch_size * grid_size
     else:
         vision_layers = cast(
-            Tuple[int, int, int, int],
+            tuple[int, int, int, int],
             tuple(len(set(k.split(".")[2] for k in ckpt if k.startswith(f"visual.layer{b}"))) for b in [1, 2, 3, 4]),
         )
         vision_width = ckpt["visual.layer1.0.conv1.weight"].shape[0]
         output_width = round((ckpt["visual.attnpool.positional_embedding"].shape[0] - 1) ** 0.5)
         vision_patch_size = None
         assert output_width**2 + 1 == ckpt["visual.attnpool.positional_embedding"].shape[0]
         image_resolution = output_width * 32
@@ -947,15 +935,15 @@
     non_visual_keys.pop("logit_scale")
     for k, v in non_visual_keys.items():
         del ckpt[k]
         ckpt[f"linguistic.{k}"] = v
 
     convert_weights(model)
 
-    def get_ckpt_part(ckpt: Dict[str, Any], prefix: str) -> Dict[str, Any]:
+    def get_ckpt_part(ckpt: dict[str, Any], prefix: str) -> dict[str, Any]:
         return {k[len(prefix) :]: v for k, v in ckpt.items() if k.startswith(prefix)}
 
     if mode == "visual":
         model.visual.load_state_dict(get_ckpt_part(ckpt, "visual."))
         return model.visual
     elif mode == "linguistic":
         model.linguistic.load_state_dict(get_ckpt_part(ckpt, "linguistic."))
```

### Comparing `usa-net-0.0.1/usa/models/point2emb.py` & `usa-net-0.0.3/usa/models/point2emb.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,31 +44,48 @@
 
 @dataclass
 class Point2EmbModelConfig(ml.BaseModelConfig):
     num_layers: int = ml.conf_field(MISSING, help="Number of MLP layers for encoding position")
     hidden_dims: int = ml.conf_field(MISSING, help="Number of hidden layer dimensions")
     num_pos_embs: int = ml.conf_field(6, help="Number of positional embedding frequencies")
     output_dims: int = ml.conf_field(MISSING, help="Number of output dimensions")
+    norm: str = ml.conf_field("no_norm", help="Per-layer normalization to apply")
+    act: str = ml.conf_field("relu", help="Activation function to use")
 
 
 @ml.register_model("point2emb", Point2EmbModelConfig)
 class Point2EmbModel(ml.BaseModel[Point2EmbModelConfig]):
     def __init__(self, config: Point2EmbModelConfig) -> None:
         super().__init__(config)
 
+        assert config.num_layers > 0
+
         # Gets the position embedding MLP.
         self.pos_embs = SinusoidalPositionalEmbeddings(config.num_pos_embs)
         pos_mlp_in_dims = POSITION_INPUT_DIMS * self.pos_embs.out_dims
+        norm_type = ml.cast_norm_type(config.norm)
+        act_type = ml.cast_activation_type(config.act)
         layers: list[nn.Module] = []
-        layers += [nn.Sequential(nn.Linear(pos_mlp_in_dims, config.hidden_dims), nn.ReLU())]
         layers += [
-            nn.Sequential(nn.Linear(config.hidden_dims, config.hidden_dims), nn.ReLU())
-            for _ in range(config.num_layers - 1)
+            nn.Sequential(
+                nn.Linear(
+                    pos_mlp_in_dims if i == 0 else config.hidden_dims,
+                    config.output_dims if i == config.num_layers - 1 else config.hidden_dims,
+                ),
+                ml.get_norm_linear(
+                    "no_norm" if i == config.num_layers - 1 else norm_type,
+                    dim=config.output_dims if i == config.num_layers - 1 else config.hidden_dims,
+                ),
+                ml.get_activation(
+                    "no_act" if i == config.num_layers - 1 else act_type,
+                    inplace=True,
+                ),
+            )
+            for i in range(config.num_layers)
         ]
-        layers += [nn.Linear(config.hidden_dims, config.output_dims)]
         self.position_mlp = nn.Sequential(*layers)
 
         self.apply(init_weights)
 
     def forward(self, points: Tensor) -> Tensor:
         """Simple model mapping a viewing angle to an embedding vector.
```

### Comparing `usa-net-0.0.1/usa/planners/base.py` & `usa-net-0.0.3/usa/planners/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 from torch import Tensor, nn
 from torch.utils.data.dataset import Dataset
 
 from usa.tasks.datasets.posed_rgbd import get_bounds, get_poses, iter_xyz
 from usa.tasks.datasets.types import PosedRGBDItem
 
 
 @dataclass
 class Map:
     grid: np.ndarray
     resolution: float
-    origin: Tuple[float, float]
+    origin: tuple[float, float]
 
-    def to_pt(self, xy: Tuple[float, float]) -> Tuple[int, int]:
+    def to_pt(self, xy: tuple[float, float]) -> tuple[int, int]:
         return (
             int((xy[0] - self.origin[0]) / self.resolution + 0.5),
             int((xy[1] - self.origin[1]) / self.resolution + 0.5),
         )
 
-    def to_xy(self, pt: Tuple[int, int]) -> Tuple[float, float]:
+    def to_xy(self, pt: tuple[int, int]) -> tuple[float, float]:
         return (
             pt[0] * self.resolution + self.origin[0],
             pt[1] * self.resolution + self.origin[1],
         )
 
-    def is_occupied(self, pt: Tuple[int, int]) -> bool:
+    def is_occupied(self, pt: tuple[int, int]) -> bool:
         return bool(self.grid[pt[1], pt[0]])
 
 
 def get_occupancy_map_from_dataset(
     ds: Dataset[PosedRGBDItem],
     cell_size: float,
-    occ_height_range: Tuple[float, float],
+    occ_height_range: tuple[float, float],
     occ_threshold: int = 100,
     clear_around_bot_radius: float = 0.0,
-    cache_dir: Optional[Path] = None,
+    cache_dir: Path | None = None,
     ignore_cached: bool = True,
 ) -> Map:
     """Gets the occupancy map from the given dataset.
 
     This employs a voting strategy to smooth out noisy points. We detect if
     there are points in some height range, and if so, we add one vote to the
     cell. We then threshold the votes to get the occupancy map.
@@ -74,28 +73,29 @@
     cache_loc = None if cache_dir is None else cache_dir / f"occ_map_{args_str}.npy"
 
     if not ignore_cached and cache_loc is not None and cache_loc.is_file():
         occ_map = np.load(cache_loc)
 
     else:
         xbins, ybins = int(bounds.xdiff / resolution) + 1, int(bounds.ydiff / resolution) + 1
-        counts: Optional[Tensor] = None
-        any_counts: Optional[Tensor] = None
+        counts: Tensor | None = None
+        any_counts: Tensor | None = None
 
         # Counts the number of points in each cell.
         with torch.no_grad():
             for xyz, mask_tensor in iter_xyz(ds, "Occupancy Map"):
                 xyz = xyz[~mask_tensor]
                 xy = xyz[:, :2]
 
                 xs = ((xy[:, 0] - origin[0]) / resolution).floor().long()
                 ys = ((xy[:, 1] - origin[1]) / resolution).floor().long()
 
-                if counts is None or any_counts is None:
+                if counts is None:
                     counts = xy.new_zeros((ybins, xbins), dtype=torch.long).flatten()
+                if any_counts is None:
                     any_counts = xy.new_zeros((ybins, xbins), dtype=torch.bool).flatten()
 
                 # Counts the number of occupying points in each cell.
                 occ_xys = (xyz[:, 2] >= min_height) & (xyz[:, 2] <= max_height)
 
                 if len(occ_xys) != 0:
                     occ_inds = ys[occ_xys] * xbins + xs[occ_xys]
@@ -130,15 +130,15 @@
                 np.save(cache_loc, occ_map)
 
     return Map(occ_map, resolution, origin)
 
 
 class Planner(nn.Module, ABC):
     @abstractmethod
-    def is_valid_starting_point(self, xy: Tuple[float, float]) -> bool:
+    def is_valid_starting_point(self, xy: tuple[float, float]) -> bool:
         """Checks if the starting point is valid.
 
         Args:
             xy: The starting point.
 
         Returns:
             True if the starting point is valid.
@@ -151,33 +151,33 @@
         Returns:
             The map.
         """
 
     @abstractmethod
     def plan(
         self,
-        start_xy: Tuple[float, float],
-        end_xy: Optional[Tuple[float, float]] = None,
-        end_goal: Optional[str] = None,
-    ) -> List[Tuple[float, float]]:
+        start_xy: tuple[float, float],
+        end_xy: tuple[float, float] | None = None,
+        end_goal: str | None = None,
+    ) -> list[tuple[float, float]]:
         """Plan a path from start_xy to an ending location.
 
         Note that either `end_xy` or `end_goal` must be specified, but not both.
 
         Args:
             start_xy: The start position.
             end_xy: The end position.
             end_goal: The end goal, specified as a string.
 
         Returns:
             A list of waypoints from start_xy to end_xy.
         """
 
     @abstractmethod
-    def score_locations(self, end_goal: str, xyzs: List[Tuple[float, float, float]]) -> List[float]:
+    def score_locations(self, end_goal: str, xyzs: list[tuple[float, float, float]]) -> list[float]:
         """Scores the locations by their semantic similarity to the goal.
 
         Args:
             end_goal: The end goal, specified as a string.
             xyzs: The positions to score.
 
         Returns:
```

### Comparing `usa-net-0.0.1/usa/planners/clip_sdf.py` & `usa-net-0.0.3/usa/planners/clip_sdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 import logging
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Type, cast
+from typing import Type, cast
 
+import ml.api as ml
 import numpy as np
 import torch
 import tqdm
-from ml.trainers.mixins.device.base import BaseDevice
 from torch import Tensor
 from torch.utils.data.dataset import Dataset
 
 from usa.models.point2emb import Point2EmbModel
 from usa.planners.base import Map, Planner, get_occupancy_map_from_dataset
 from usa.planners.common import AStarPlanner as AStarPlannerBase, Heuristic
 from usa.tasks.clip_sdf import ClipSdfTask
@@ -21,20 +21,20 @@
 
 class ClipSdfPlanner(Planner):
     def __init__(
         self,
         dataset: Dataset[PosedRGBDItem],
         model: Point2EmbModel,
         task: ClipSdfTask,
-        device: Type[BaseDevice],
+        device: Type[ml.BaseDevice],
         resolution: float,
         occ_avoid_radius: float = 0.3,
         floor_height: float = 0.1,
         ceil_height: float = 1.3,
-        cache_dir: Optional[Path] = None,
+        cache_dir: Path | None = None,
     ) -> None:
         """Initializes the ClipSdfPlanner.
 
         Args:
             dataset: The dataset to use for planning.
             model: The model to use for planning.
             task: The task for training the model.
@@ -66,26 +66,26 @@
             (self.min_z, self.max_z),
             cache_dir=cache_dir,
         )
 
         # Don't train the model.
         self.model.eval().requires_grad_(False)
 
-    def get_clip_and_sdf(self, xyz: List[Tuple[float, float, float]]) -> Tuple[Tensor, List[float]]:
+    def get_clip_and_sdf(self, xyz: list[tuple[float, float, float]]) -> tuple[Tensor, list[float]]:
         xyz_tensor = torch.tensor(xyz)
         xyz_tensor = self.device.tensor_to(xyz_tensor)
         preds = self.model(xyz_tensor)
         clip_emb_size = preds.size(-1) - 1
         clip_preds, sdf_preds = torch.split(preds, [clip_emb_size, 1], dim=-1)
         return clip_preds.cpu(), [s.item() for s in sdf_preds.cpu()]
 
-    def get_grid_xyzs(self) -> Tuple[Tensor, Tensor, Tensor]:
+    def get_grid_xyzs(self) -> tuple[Tensor, Tensor, Tensor]:
         y_pixels, x_pixels = self.occ_map.grid.shape
 
-        def occ_map_pt_to_xy(pt: Tuple[int, int]) -> Tuple[float, float]:
+        def occ_map_pt_to_xy(pt: tuple[int, int]) -> tuple[float, float]:
             return (
                 pt[0] * self.occ_map.resolution + self.occ_map.origin[0],
                 pt[1] * self.occ_map.resolution + self.occ_map.origin[1],
             )
 
         x_min, y_min = occ_map_pt_to_xy((0, 0))
         x_max, y_max = occ_map_pt_to_xy((x_pixels, y_pixels))
@@ -142,38 +142,38 @@
 
         return Map(
             grid=is_occ,
             origin=origin,
             resolution=self.occ_map.resolution,
         )
 
-    def score_locations(self, end_goal: str, xyzs: List[Tuple[float, float, float]]) -> List[float]:
+    def score_locations(self, end_goal: str, xyzs: list[tuple[float, float, float]]) -> list[float]:
         with torch.no_grad():
             tokens = self.device.tensor_to(self.task.clip.tokenizer.tokenize(end_goal))
             goal_embs = self.task.clip.linguistic(tokens)
             xyzs_tensor = torch.tensor(xyzs)
-            scores: List[float] = []
+            scores: list[float] = []
             for xyz_chunk in xyzs_tensor.split(256):
                 xyz_chunk = self.device.tensor_to(xyz_chunk)
                 clip_preds = self.model(xyz_chunk)[:, :-1]
                 clip_scores = goal_embs @ clip_preds.T
                 scores.extend(clip_scores.squeeze(0).cpu().tolist())
             return scores
 
 
 class AStarPlanner(ClipSdfPlanner):
     def __init__(
         self,
         dataset: Dataset[PosedRGBDItem],
         model: Point2EmbModel,
         task: ClipSdfTask,
-        device: Type[BaseDevice],
+        device: Type[ml.BaseDevice],
         heuristic: Heuristic,
         resolution: float,
-        cache_dir: Optional[Path] = None,
+        cache_dir: Path | None = None,
         floor_height: float = 0.1,
         ceil_height: float = 1.3,
     ) -> None:
         super().__init__(
             dataset=dataset,
             model=model,
             task=task,
@@ -193,19 +193,19 @@
             is_occ=clip_sdf_map.grid,
             origin=clip_sdf_map.origin,
             resolution=clip_sdf_map.resolution,
         )
 
     def plan(
         self,
-        start_xy: Tuple[float, float],
-        end_xy: Optional[Tuple[float, float]] = None,
-        end_goal: Optional[str] = None,
+        start_xy: tuple[float, float],
+        end_xy: tuple[float, float] | None = None,
+        end_goal: str | None = None,
         remove_line_of_sight_points: bool = True,
-    ) -> List[Tuple[float, float]]:
+    ) -> list[tuple[float, float]]:
         if end_goal is not None:
             assert end_xy is None, "Cannot specify both end_xy and end_goal"
             end_xy = self.get_end_xy(start_xy, end_goal)
 
         return self.a_star_planner.plan(
             start_xy=start_xy,
             end_xy=end_xy,
@@ -229,15 +229,15 @@
         for xyz_chunk in tqdm.tqdm(torch.split(xyzs, 64)):
             clip_embs = self.model(xyz_chunk)[:, :-1]
             tok_scores = embs @ clip_embs.T
             all_clip_sims.append(tok_scores.flatten(0).detach().cpu())
 
         return torch.cat(all_clip_sims, dim=0).view(xs.shape).max(dim=-1, keepdim=True).values.numpy()
 
-    def get_end_xy(self, start_xy: Tuple[float, float], end_goal: str) -> Tuple[float, float]:
+    def get_end_xy(self, start_xy: tuple[float, float], end_goal: str) -> tuple[float, float]:
         score_map = self.get_score_map(end_goal)
         start_pt = self.a_star_planner.to_pt(start_xy)
         reachable_pts = self.a_star_planner.get_reachable_points(start_pt)
         xs, ys = zip(*reachable_pts)
         reachable_map = np.zeros_like(score_map, dtype=bool)
         reachable_map[ys, xs] = True
 
@@ -247,37 +247,37 @@
         y, x, _ = unocc_points[best_point_index]
 
         assert not self.a_star_planner.point_is_occupied(x, y), "Best point is occupied"
 
         # Converts to (X, Y) coordinates.
         return self.a_star_planner.to_xy((x, y))
 
-    def is_valid_starting_point(self, xy: Tuple[float, float]) -> bool:
+    def is_valid_starting_point(self, xy: tuple[float, float]) -> bool:
         return self.a_star_planner.is_valid_starting_point(xy)
 
     @functools.lru_cache
     def get_map(self) -> Map:
         return self.a_star_planner.get_map()
 
 
 class GradientPlanner(ClipSdfPlanner):
     def __init__(
         self,
         dataset: Dataset[PosedRGBDItem],
         model: Point2EmbModel,
         task: ClipSdfTask,
-        device: Type[BaseDevice],
+        device: Type[ml.BaseDevice],
         lr: float = 1e-2,
         dist_loss_weight: float = 1.0,
         spacing_loss_weight: float = 1.0,
         occ_loss_weight: float = 25.0,
         sim_loss_weight: float = 15.0,
         num_optimization_steps: int = 1000,
         min_distance: float = 1e-5,
-        cache_dir: Optional[Path] = None,
+        cache_dir: Path | None = None,
         floor_height: float = 0.1,
         ceil_height: float = 1.3,
     ) -> None:
         # Constant resolution.
         visualization_resolution = 0.025
         planner_resolution = 0.1
 
@@ -317,30 +317,30 @@
     def get_target_query_emb(self, end_goal: str) -> Tensor:
         tokens = self.device.tensor_to(self.task.clip.tokenizer.tokenize(end_goal))
         embs = self.task.clip.linguistic(tokens)
         return embs
 
     def plan(
         self,
-        start_xy: Tuple[float, float],
-        end_xy: Optional[Tuple[float, float]] = None,
-        end_goal: Optional[str] = None,
-    ) -> List[Tuple[float, float]]:
+        start_xy: tuple[float, float],
+        end_xy: tuple[float, float] | None = None,
+        end_goal: str | None = None,
+    ) -> list[tuple[float, float]]:
         assert end_xy is not None or end_goal is not None, "Must specify either end_xy or end_goal"
         assert end_xy is None or end_goal is None, "Must specify either end_xy or end_goal, not both"
 
         # Gets the end goal embedding.
         target_emb = None if end_goal is None else self.get_target_query_emb(end_goal)
 
         # Gets a seed path from the base planner.
         seed_path = self.base_planner.plan(start_xy, end_xy, end_goal, remove_line_of_sight_points=False)
         xys = self.device.tensor_to(torch.tensor(seed_path))
         xys.requires_grad_(True)
 
-        def get_losses(xys: Tensor) -> Dict[str, Tensor]:
+        def get_losses(xys: Tensor) -> dict[str, Tensor]:
             # Loss for avoiding obstacles.
             waypoint_xyz_min = torch.cat([xys[1:], torch.full_like(xys[1:, :1], self.min_z)], dim=-1)
             waypoint_xyz_max = torch.cat([xys[1:], torch.full_like(xys[1:, :1], self.max_z)], dim=-1)
             preds_min = self.model(waypoint_xyz_min)
             preds_max = self.model(waypoint_xyz_max)
             clip_preds_min, sdf_preds_min = preds_min[-1:, :-1], preds_min[..., -1]
             clip_preds_max, sdf_preds_max = preds_max[-1:, :-1], preds_max[..., -1]
@@ -354,15 +354,15 @@
             dist_loss = norms.sum()
 
             # Spacing loss, to try to make the waypoints spaced evenly.
             # The idea here is that the norms on either side of any given
             # point should be roughly equal.
             spacing_loss = ((norms[1:] - norms[:-1]) ** 2).sum()
 
-            losses: Dict[str, Tensor] = {
+            losses: dict[str, Tensor] = {
                 "dist": dist_loss * self.dist_loss_weight,
                 "spacing": spacing_loss * self.spacing_loss_weight,
                 "occ": occ_loss * self.occ_loss_weight,
             }
 
             # Embedding loss for the final waypoint; try to maximize the
             # similarity between it's clip embedding and the target embedding.
@@ -373,15 +373,15 @@
                 # sim_score = torch.where(is_inside_obs[-1], torch.zeros_like(sim_score), sim_score)
                 sim_loss = -sim_score
                 losses["sim"] = sim_loss * self.sim_loss_weight
 
             return losses
 
         # Optimization loop, just using gradient descent.
-        prev_xys: Optional[Tensor] = None
+        prev_xys: Tensor | None = None
 
         opt = torch.optim.Adam([xys], lr=self.lr)
         # opt = torch.optim.SGD([xys], lr=self.lr, momentum=0.9)
 
         for _ in tqdm.trange(self.num_optimization_steps):
             opt.zero_grad()
             losses = get_losses(xys)
@@ -414,11 +414,11 @@
         points = [(x, y) for x, y in xys.detach().cpu().numpy().tolist()]  # pylint: disable=unnecessary-comprehension
 
         # Explicitly delete the optimizer and points.
         del opt, xys
 
         return points
 
-    def is_valid_starting_point(self, xy: Tuple[float, float]) -> bool:
+    def is_valid_starting_point(self, xy: tuple[float, float]) -> bool:
         min_xyz, max_xyz = (xy[0], xy[1], self.min_z), (xy[0], xy[1], self.max_z)
         _, sdfs = self.get_clip_and_sdf([min_xyz, max_xyz])
         return all(sdf > self.occ_avoid_radius for sdf in sdfs)
```

### Comparing `usa-net-0.0.1/usa/planners/common.py` & `usa-net-0.0.3/usa/planners/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import functools
 import heapq
 import math
-from typing import Dict, List, Literal, Optional, Set, Tuple
+from typing import Literal
 
 import numpy as np
 
 from usa.planners.base import Map, Planner
 
 Heuristic = Literal["manhattan", "euclidean", "octile", "chebyshev"]
 
 
-def neighbors(pt: Tuple[int, int]) -> List[Tuple[int, int]]:
+def neighbors(pt: tuple[int, int]) -> list[tuple[int, int]]:
     return [(pt[0] + dx, pt[1] + dy) for dx in range(-1, 2) for dy in range(-1, 2) if (dx, dy) != (0, 0)]
 
 
 class AStarPlanner(Planner):
     def __init__(
         self,
         heuristic: Heuristic,
         is_occ: np.ndarray,
-        origin: Tuple[float, float],
+        origin: tuple[float, float],
         resolution: float,
     ) -> None:
         super().__init__()
 
         self.heuristic = heuristic
         self.is_occ = is_occ
         self.origin = origin
@@ -34,34 +34,34 @@
         if x < 0 or y < 0 or x >= occ_map.grid.shape[1] or y >= occ_map.grid.shape[0]:
             return True
         return bool(occ_map.grid[y][x])
 
     def xy_is_occupied(self, x: float, y: float) -> bool:
         return self.point_is_occupied(*self.to_pt((x, y)))
 
-    def to_pt(self, xy: Tuple[float, float]) -> Tuple[int, int]:
+    def to_pt(self, xy: tuple[float, float]) -> tuple[int, int]:
         return self.get_map().to_pt(xy)
 
-    def to_xy(self, pt: Tuple[int, int]) -> Tuple[float, float]:
+    def to_xy(self, pt: tuple[int, int]) -> tuple[float, float]:
         return self.get_map().to_xy(pt)
 
-    def compute_heuristic(self, a: Tuple[int, int], b: Tuple[int, int]) -> float:
+    def compute_heuristic(self, a: tuple[int, int], b: tuple[int, int]) -> float:
         if self.heuristic == "manhattan":
             return abs(a[0] - b[0]) + abs(a[1] - b[1])
         if self.heuristic == "euclidean":
             return ((a[0] - b[0]) ** 2 + (a[1] - b[1]) ** 2) ** 0.5
         if self.heuristic == "octile":
             dx = abs(a[0] - b[0])
             dy = abs(a[1] - b[1])
             return (dx + dy) + (1 - 2) * min(dx, dy)
         if self.heuristic == "chebyshev":
             return max(abs(a[0] - b[0]), abs(a[1] - b[1]))
         raise ValueError(f"Unknown heuristic: {self.heuristic}")
 
-    def is_in_line_of_sight(self, start_pt: Tuple[int, int], end_pt: Tuple[int, int]) -> bool:
+    def is_in_line_of_sight(self, start_pt: tuple[int, int], end_pt: tuple[int, int]) -> bool:
         """Checks if there is a line-of-sight between two points.
 
         Implements using Bresenham's line algorithm.
 
         Args:
             start_pt: The starting point.
             end_pt: The ending point.
@@ -93,15 +93,15 @@
                 #     return False
                 for x in list({math.floor(xf), math.ceil(xf)}):
                     if self.point_is_occupied(x, y):
                         return False
 
         return True
 
-    def clean_path(self, path: List[Tuple[int, int]]) -> List[Tuple[int, int]]:
+    def clean_path(self, path: list[tuple[int, int]]) -> list[tuple[int, int]]:
         """Cleans up the final path.
 
         This implements a simple algorithm where, given some current position,
         we find the last point in the path that is in line-of-sight, and then
         we set the current position to that point. This is repeated until we
         reach the end of the path. This is not particularly efficient, but
         it's simple and works well enough.
@@ -121,17 +121,15 @@
                     break
             else:
                 j = i + 1
             cleaned_path.append(path[j])
             i = j
         return cleaned_path
 
-    def get_unoccupied_neighbor(
-        self, pt: Tuple[int, int], goal_pt: Optional[Tuple[int, int]] = None
-    ) -> Tuple[int, int]:
+    def get_unoccupied_neighbor(self, pt: tuple[int, int], goal_pt: tuple[int, int] | None = None) -> tuple[int, int]:
         if not self.point_is_occupied(*pt):
             return pt
 
         # This is a sort of hack to deal with points that are close to an edge.
         # If the start point is occupied, we check adjacent points until we get
         # one which is unoccupied. If we can't find one, we throw an error.
         neighbor_pts = neighbors(pt)
@@ -140,27 +138,27 @@
             neighbor_pts.sort(key=lambda n: self.compute_heuristic(n, goal_pt_non_null))
         for neighbor_pt in neighbor_pts:
             if not self.point_is_occupied(*neighbor_pt):
                 return neighbor_pt
 
         raise ValueError("No reachable points")
 
-    def get_reachable_points(self, start_pt: Tuple[int, int]) -> Set[Tuple[int, int]]:
+    def get_reachable_points(self, start_pt: tuple[int, int]) -> set[tuple[int, int]]:
         """Gets all reachable points from a given starting point.
 
         Args:
             start_pt: The starting point
 
         Returns:
             The set of all reachable points
         """
 
         start_pt = self.get_unoccupied_neighbor(start_pt)
 
-        reachable_points: Set[Tuple[int, int]] = set()
+        reachable_points: set[tuple[int, int]] = set()
         to_visit = [start_pt]
         while to_visit:
             pt = to_visit.pop()
             if pt in reachable_points:
                 continue
             reachable_points.add(pt)
             for new_pt in neighbors(pt):
@@ -169,31 +167,31 @@
                 if self.point_is_occupied(new_pt[0], new_pt[1]):
                     continue
                 to_visit.append(new_pt)
         return reachable_points
 
     def plan(
         self,
-        start_xy: Tuple[float, float],
-        end_xy: Optional[Tuple[float, float]] = None,
-        end_goal: Optional[str] = None,
+        start_xy: tuple[float, float],
+        end_xy: tuple[float, float] | None = None,
+        end_goal: str | None = None,
         remove_line_of_sight_points: bool = True,
-    ) -> List[Tuple[float, float]]:
+    ) -> list[tuple[float, float]]:
         assert end_goal is None and end_xy is not None, "AStarPlanner doesn't implement location queries"
 
         start_pt, end_pt = self.to_pt(start_xy), self.to_pt(end_xy)
 
         # Checks that both points are unoccupied.
         start_pt = self.get_unoccupied_neighbor(start_pt, end_pt)
         end_pt = self.get_unoccupied_neighbor(end_pt, start_pt)
 
         # Implements A* search.
         q = [(0, start_pt)]
-        came_from: Dict[Tuple[int, int], Optional[Tuple[int, int]]] = {start_pt: None}
-        cost_so_far: Dict[Tuple[int, int], float] = {start_pt: 0.0}
+        came_from: dict[tuple[int, int], tuple[int, int] | None] = {start_pt: None}
+        cost_so_far: dict[tuple[int, int], float] = {start_pt: 0.0}
         while q:
             _, current = heapq.heappop(q)
 
             if current == end_pt:
                 break
 
             for nxt in neighbors(current):
@@ -223,20 +221,20 @@
 
         # Clean up the path.
         if remove_line_of_sight_points:
             path = self.clean_path(path)
 
         return [start_xy] + [self.to_xy(pt) for pt in path[1:-1]] + [end_xy]
 
-    def is_valid_starting_point(self, xy: Tuple[float, float]) -> bool:
+    def is_valid_starting_point(self, xy: tuple[float, float]) -> bool:
         return not self.point_is_occupied(*self.to_pt(xy))
 
     @functools.lru_cache
     def get_map(self) -> Map:
         return Map(
             grid=self.is_occ,
             resolution=self.resolution,
             origin=self.origin,
         )
 
-    def score_locations(self, end_goal: str, xyzs: List[Tuple[float, float, float]]) -> List[float]:
+    def score_locations(self, end_goal: str, xyzs: list[tuple[float, float, float]]) -> list[float]:
         raise NotImplementedError("AStarPlanner doesn't implement location queries")
```

### Comparing `usa-net-0.0.1/usa/planners/occupancy_map.py` & `usa-net-0.0.3/usa/planners/occupancy_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from typing import List, Optional, Tuple
 
 import cv2
 import numpy as np
 from torch.utils.data.dataset import Dataset
 
 from usa.planners.base import Map, Planner, get_occupancy_map_from_dataset
 from usa.planners.common import AStarPlanner as AStarPlannerBase, Heuristic
@@ -15,15 +14,15 @@
         self,
         dataset: Dataset[PosedRGBDItem],
         resolution: float,
         floor_height: float = 0.1,
         ceil_height: float = 1.3,
         occ_avoid_radius: float = 0.5,
         clear_around_bot_radius: float = 0.3,
-        cache_dir: Optional[Path] = None,
+        cache_dir: Path | None = None,
     ) -> None:
         """Initializes the OccupancyMapPlanner.
 
         Args:
             dataset: The dataset to use for planning.
             resolution: The resolution of the occupancy map.
             floor_height: The height of the floor.
@@ -54,25 +53,25 @@
 
         # The array of occupied positions.
         is_occ = occupancy_map.grid.astype(np.float32)
         radius = int(np.round(self.occ_avoid_radius / self.resolution))
         is_occ = cv2.dilate(is_occ, cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (radius, radius)))
         self.is_occ = is_occ
 
-    def score_locations(self, end_goal: str, xyzs: List[Tuple[float, float, float]]) -> List[float]:
+    def score_locations(self, end_goal: str, xyzs: list[tuple[float, float, float]]) -> list[float]:
         raise NotImplementedError("OccupancyMapPlanner doesn't implement location queries")
 
 
 class AStarPlanner(OccupancyMapPlanner):
     def __init__(
         self,
         dataset: Dataset[PosedRGBDItem],
         heuristic: Heuristic,
         resolution: float,
-        cache_dir: Optional[Path] = None,
+        cache_dir: Path | None = None,
         floor_height: float = 0.1,
         ceil_height: float = 1.3,
     ) -> None:
         """Initializes the AStarPlanner.
 
         Args:
             dataset: The dataset to use for planning.
@@ -99,18 +98,18 @@
             is_occ=self.is_occ,
             origin=self.origin,
             resolution=resolution,
         )
 
     def plan(
         self,
-        start_xy: Tuple[float, float],
-        end_xy: Optional[Tuple[float, float]] = None,
-        end_goal: Optional[str] = None,
-    ) -> List[Tuple[float, float]]:
+        start_xy: tuple[float, float],
+        end_xy: tuple[float, float] | None = None,
+        end_goal: str | None = None,
+    ) -> list[tuple[float, float]]:
         return self.a_star_planner.plan(start_xy, end_xy, end_goal)
 
-    def is_valid_starting_point(self, xy: Tuple[float, float]) -> bool:
+    def is_valid_starting_point(self, xy: tuple[float, float]) -> bool:
         return self.a_star_planner.is_valid_starting_point(xy)
 
     def get_map(self) -> Map:
         return self.a_star_planner.get_map()
```

### Comparing `usa-net-0.0.1/usa/scripts/adhoc/distribution_estimates.py` & `usa-net-0.0.3/usa/scripts/adhoc/distribution_estimates.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.1/usa/tasks/clip_sdf.py` & `usa-net-0.0.3/usa/tasks/clip_sdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import itertools
 import logging
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable
 
 import ml.api as ml
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 import tqdm
 from omegaconf import MISSING
@@ -14,38 +14,46 @@
 from torch.utils.data.dataset import Dataset
 
 from usa.models.clip import (
     CLIPTokenizer,
     cast_pretrained_model_key as cast_pretrained_clip_model_key,
     load_pretrained as load_pretrained_clip,
 )
+from usa.models.point2emb import Point2EmbModel
 from usa.tasks.datasets.posed_rgbd import Bounds, get_posed_rgbd_dataset
 from usa.tasks.datasets.types import PosedRGBDItem
 from usa.tasks.datasets.utils import (
     get_nearest_xyz,
     get_xy_pixel_from_xyz,
     get_xyz_coordinates,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def aminmax(x: Tensor) -> tuple[Tensor, Tensor]:
+    if x.device.type == "mps":
+        return x.min(), x.max()
+    xmin, xmax = torch.aminmax(x)
+    return xmin, xmax
+
+
 def clip_sim(a: Tensor, b: Tensor) -> Tensor:
     assert a.dim() == 2 and b.dim() == 2
     a, b = a / (a.norm(dim=1, keepdim=True) + 1e-3), b / (b.norm(dim=1, keepdim=True) + 1e-3)
     return a @ b.t()
 
 
 def get_image_crop_around(
     xy: Tensor,
     image: Tensor,
-    trg_shape: Tuple[int, int],
+    trg_shape: tuple[int, int],
     min_crop: float = 0.2,
     max_crop: float = 0.4,
-) -> Optional[Tuple[Tensor, Tensor]]:
+) -> tuple[Tensor, Tensor] | None:
     trg_w, trg_h = trg_shape
     npts, _, img_h, img_w = image.shape
 
     # Gets the crop shapes.
     crop_width = (((torch.rand(npts, device=xy.device) * (max_crop - min_crop)) + min_crop) * img_w).int()
     crop_height = (crop_width * trg_h / trg_w).int()
 
@@ -72,23 +80,24 @@
         dim=0,
     )
 
     return cropped, mask
 
 
 @dataclass
-class ClipSdfTaskConfig(ml.BaseTaskConfig):
+class ClipSdfTaskConfig(ml.SupervisedLearningTaskConfig):
     dataset: str = ml.conf_field(MISSING, help="Dataset key to use")
+    dataset_path: str | None = ml.conf_field(None, help="Path to the dataset")
     clip_model: str = ml.conf_field(MISSING, help="The CLIP model to load")
-    queries: List[str] = ml.conf_field(MISSING, help="Queries to evaluate against")
+    queries: list[str] = ml.conf_field(MISSING, help="Queries to evaluate against")
     rotate_image: bool = ml.conf_field(False, help="If set, rotate image when getting CLIP scores")
     pts_per_frame: int = ml.conf_field(100, help="Number of points to sample per frame")
     min_depth_prct: float = ml.conf_field(0.1, help="Minimum depth percentage to sample")
     points_to_sample: int = ml.conf_field(50, help="XYZ points to sample (per frame) during model inference")
-    image_shape: Tuple[int, int] = ml.conf_field(lambda: (224, 224), help="Size of the SDF image to log")
+    image_shape: tuple[int, int] = ml.conf_field(lambda: (224, 224), help="Size of the SDF image to log")
 
 
 class ClipModel:
     def __init__(self, key: str) -> None:
         """Wrapper for the CLIP model which isn't an nn.Module.
 
         This is useful because we don't want to save the CLIP model weights
@@ -107,16 +116,22 @@
         # Disables gradients for CLIP model.
         self.visual.requires_grad_(False)
         self.linguistic.requires_grad_(False)
 
         self.tokenizer = CLIPTokenizer()
 
 
+Model = Point2EmbModel
+Batch = PosedRGBDItem
+Output = tuple[Tensor, Tensor]
+Loss = dict[str, Tensor]
+
+
 @ml.register_task("clip_sdf", ClipSdfTaskConfig)
-class ClipSdfTask(ml.BaseTask):
+class ClipSdfTask(ml.SupervisedLearningTask[ClipSdfTaskConfig, Model, Batch, Output, Loss]):
     bounds: Tensor
     pose_bounds: Tensor
     clip_text_embs: Tensor
     clip: ClipModel
 
     def __init__(self, config: ClipSdfTaskConfig) -> None:
         super().__init__(config)
@@ -133,15 +148,15 @@
 
     def apply(self, fn: Callable[["torch.nn.Module"], None]) -> Any:
         self.clip.visual.apply(fn)
         self.clip.linguistic.apply(fn)
         return super().apply(fn)
 
     def _get_posed_rgb_dataset(self) -> Dataset[PosedRGBDItem]:
-        return get_posed_rgbd_dataset(self.config.dataset)
+        return get_posed_rgbd_dataset(self.config.dataset, path=self.config.dataset_path)
 
     @functools.cached_property
     def _dataset(self) -> Dataset[PosedRGBDItem]:
         return self._get_posed_rgb_dataset()
 
     @functools.lru_cache
     def text_clip_embs(self, device: torch.device) -> Tensor:
@@ -150,43 +165,35 @@
             embs = self.clip.linguistic(tokens)
             return embs
 
     @property
     def slice_height(self) -> float:
         return (self.pose_bounds[1, 0] + self.pose_bounds[1, 1]).item() / 2
 
-    def run_model(
-        self,
-        model: ml.BaseModel,
-        batch: PosedRGBDItem,
-        state: ml.State,
-    ) -> Tuple[Tensor, Tensor]:
+    def run_model(self, model: Model, batch: Batch, state: ml.State) -> tuple[Tensor, Tensor]:
         _, depth, mask, intrinsics, pose = batch
         depth_frac = torch.rand_like(depth) * (1 - self.config.min_depth_prct) + self.config.min_depth_prct
 
         # Sample XYZ points to run through the model.
         sample_mask = torch.rand_like(mask, dtype=depth.dtype)
-        q = torch.quantile(sample_mask.float(), self.config.points_to_sample / sample_mask.numel()).to(sample_mask)
+        q = torch.quantile(
+            (sample_mask.cpu() if mask.device.type == "mps" else sample_mask).float(),
+            self.config.points_to_sample / sample_mask.numel(),
+        ).to(sample_mask)
         mask = mask | (sample_mask > q)
         sampled_xyz = get_xyz_coordinates(depth_frac * depth, mask, pose, intrinsics).to(depth)
 
         preds = model(sampled_xyz)
 
         return preds, sampled_xyz
 
-    def compute_loss(
-        self,
-        model: ml.BaseModel,
-        batch: PosedRGBDItem,
-        state: ml.State,
-        output: Tuple[Tensor, Tensor],
-    ) -> Dict[str, Tensor]:
+    def compute_loss(self, model: Model, batch: Batch, state: ml.State, output: Output) -> Loss:
         rgb, depth, mask, intrinsics, pose = batch
         preds, xyz = output
-        device, dtype = preds.device, preds.dtype
+        device = preds.device
 
         # Splits into CLIP and SDF predictions.
         clip_preds, sdf_preds = torch.split(preds, [self.clip.visual.output_dim, 1], dim=-1)
 
         with torch.no_grad():
             # Gets the nearest neighbor to the sampled points.
             batch_xyz = get_xyz_coordinates(depth.to(pose), mask, pose, intrinsics)
@@ -198,16 +205,16 @@
 
             # Gets the pixel closest to the nearest XYZ point.
             nearest_xy = get_xy_pixel_from_xyz(nearest_xyz, pose[batch_inds], intrinsics[batch_inds])
             nearest_xy = nearest_xy.round().int()
             crop_result = get_image_crop_around(nearest_xy, rgb[batch_inds], (224, 224))
 
             # If there was a cropped image, get the CLIP embeddings for it.
-            crop_image: Optional[Tensor] = None
-            clip: Optional[Tensor] = None
+            crop_image: Tensor | None = None
+            clip: Tensor | None = None
             if crop_result is not None:
                 crop_image = crop_result[0]
                 if self.config.rotate_image:
                     crop_image = V.rotate(crop_image, -90)
                 clip = self.clip.visual(crop_image)
 
             # Gets the CLIP embeddings for the cropped images.
@@ -231,46 +238,37 @@
             # Weight the CLIP loss by the softmax of the SDF.
             clip_sdfs = sdf[crop_result[1]]
             clip_loss = clip_loss * F.softmax(clip_sdfs, dim=0)
 
             losses["clip"] = clip_loss
 
         # Logs the prediction ranges.
-        pmin, pmax = preds.aminmax()
+        pmin, pmax = aminmax(preds)
         self.logger.log_scalar("pmin", pmin)
         self.logger.log_scalar("pmax", pmax)
 
         if state.phase == "valid":
-            clip_image, sdf_image = self.get_clip_and_sdf_images(model, device, dtype)
-            self.logger.log_image("sdf", sdf_image)
+            # clip_image, sdf_image = self.get_clip_and_sdf_images(model, device, preds.dtype)
+            # self.logger.log_image("sdf", sdf_image)
             self.logger.log_point_cloud("xyz", torch.stack([xyz, nearest_xyz.to(xyz)]))
             self.logger.log_point_cloud("surface", batch_xyz.to(xyz))
-            self.logger.log_labeled_images("query_sims", (clip_image, self.config.queries))
+            # self.logger.log_labeled_images("query_sims", (clip_image, self.config.queries))
 
-            if crop_image is not None:
-                self.logger.log_images("cropped", crop_image)
+            # if crop_image is not None:
+            #     self.logger.log_images("cropped", crop_image)
 
         return losses
 
-    def get_single_loss(self, loss: Tensor | Dict[str, Tensor]) -> Tuple[Tensor, List[str]]:
-        assert isinstance(loss, dict)
-        losses: List[Tensor] = [loss["sdf"].mean()]
-        keys: List[str] = ["sdf"]
-        if "clip" in loss:
-            losses += [loss["clip"].mean()]
-            keys += ["clip"]
-        return torch.stack(losses), keys
-
     def get_clip_and_sdf_images(
         self,
         model: ml.BaseModel,
         device: torch.device,
         dtype: torch.dtype,
         image_chunk_size: int = 128,
-    ) -> Tuple[Tensor, Tensor]:
+    ) -> tuple[Tensor, Tensor]:
         with torch.no_grad():
             bounds = Bounds.from_arr(self.bounds)
             pose_bounds = Bounds.from_arr(self.pose_bounds)
             slice_z = (pose_bounds.zmax + pose_bounds.zmin) / 2
 
             # Gets the XYZ points for the SDF image.
             width, height = self.config.image_shape
@@ -281,29 +279,29 @@
             xyz = torch.stack((xs, ys, torch.full_like(xs, slice_z)), dim=-1).flatten(0, -2)
             num_chunks = xyz.shape[0] // image_chunk_size
 
             # Compute CLIP similarity with the text embeddings.
             text_embs = self.text_clip_embs(device)
 
             # Runs all XYZ points through the model to get predictions.
-            all_clip_preds: List[Tensor] = []
-            all_sdf_preds: List[Tensor] = []
+            all_clip_preds: list[Tensor] = []
+            all_sdf_preds: list[Tensor] = []
             for xyz_chunk in tqdm.tqdm(torch.chunk(xyz, num_chunks), disable=ml.is_distributed()):
                 preds = model(xyz_chunk)
                 clip_preds, sdf_preds = torch.split(preds, [self.clip.visual.output_dim, 1], dim=-1)
                 all_clip_preds.append(clip_sim(clip_preds, text_embs))
                 all_sdf_preds.append(sdf_preds)
 
             # Concatenates the predictions and converts them to image shapes.
             sdf_preds = torch.cat(all_sdf_preds, dim=0).view(width, height)
             clip_preds = torch.cat(all_clip_preds, dim=0).view(width, height, text_embs.shape[0])
 
             # Normalizes CLIP similarity image to range (0, 1).
             clip_preds = clip_preds.softmax(dim=-1)
-            clip_min, clip_max = clip_preds.aminmax()
+            clip_min, clip_max = aminmax(clip_preds)
             clip_preds = (clip_preds - clip_min) / (clip_max - clip_min + 1e-3)
 
             # CLIP image has shape (num_embs, width, height)
             # SDF image has shape (width, height)
             return clip_preds.permute(2, 0, 1), sdf_preds
 
     def get_dataset(self, phase: ml.Phase) -> Dataset:
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/home_robot.py` & `usa-net-0.0.3/usa/tasks/datasets/home_robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from torchvision.datasets.utils import download_url
 
 from usa.tasks.datasets.types import PosedRGBDItem
 from usa.tasks.datasets.utils import visualize_posed_rgbd_dataset
 
 logger = logging.getLogger(__name__)
 
-CHRIS_LAB_URL = "https://github.com/codekansas/usa/releases/download/v1.0.0/chris_lab.pkl"
+CHRIS_LAB_URL = "https://github.com/codekansas/usa/releases/download/v0.0.2/chris_lab.pkl"
 
 
 @dataclass
 class Data:
     color_imgs: np.ndarray
     depth_imgs: np.ndarray
     poses: np.ndarray
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/posed_rgbd.py` & `usa-net-0.0.3/usa/tasks/datasets/posed_rgbd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterator, List, Optional, Tuple
+from typing import Iterator
 
 import ml.api as ml
 import more_itertools
 import numpy as np
 import torch
 import tqdm
 from torch import Tensor
 from torch.utils.data.dataset import Dataset
 
 from usa.tasks.datasets.home_robot import (
     HomeRobotDataset,
     chris_lab_home_robot_dataset,
 )
-from usa.tasks.datasets.r3d import LabR3DDataset, StudioR3DDataset
+from usa.tasks.datasets.r3d import LabR3DDataset, R3DDataset, StudioR3DDataset
 from usa.tasks.datasets.replica_cad import ReplicaCADDataset
 from usa.tasks.datasets.stretch import (
     chess_stretch_dataset,
     kitchen_stretch_dataset,
     lab_stretch_dataset,
 )
 from usa.tasks.datasets.types import PosedRGBDItem
@@ -36,14 +36,19 @@
     random_crop: bool = True,
 ) -> Dataset[PosedRGBDItem]:
     if key == "home_robot":
         if path is None:
             path = os.environ.get("HOME_ROBOT_DS_PATH")
         assert path is not None, "Path must be specified for `home_robot` dataset; set `HOME_ROBOT_DS_PATH` env var"
         return HomeRobotDataset(path)
+    if key == "r3d":
+        if path is None:
+            path = os.environ.get("R3D_DS_PATH")
+        assert path is not None, "Path must be specified for `r3d` dataset; set `R3D_DS_PATH` env var"
+        return R3DDataset(path, img_dim=img_dim, random_crop=random_crop)
     if key == "chris_lab":
         return chris_lab_home_robot_dataset()
     if key == "lab_r3d":
         return LabR3DDataset(img_dim=img_dim, random_crop=random_crop)
     if key == "studio_r3d":
         return StudioR3DDataset(img_dim=img_dim, random_crop=random_crop)
     if key == "lab_stretch":
@@ -104,17 +109,20 @@
             dim=1,
         )
 
     @classmethod
     def from_xyz(cls, xyz: Tensor) -> Tensor:
         assert xyz.shape[-1] == 3
 
-        xmin, xmax = torch.aminmax(xyz[..., 0])
-        ymin, ymax = torch.aminmax(xyz[..., 1])
-        zmin, zmax = torch.aminmax(xyz[..., 2])
+        # Supports MPS tensors.
+        aminmax = lambda x: (x.min(), x.max()) if x.device.type == "mps" else tuple(torch.aminmax(x))
+
+        xmin, xmax = aminmax(xyz[..., 0])
+        ymin, ymax = aminmax(xyz[..., 1])
+        zmin, zmax = aminmax(xyz[..., 2])
 
         return torch.tensor([[xmin, xmax], [ymin, ymax], [zmin, zmax]], device=xyz.device, dtype=xyz.dtype)
 
 
 def get_xyz(depth: Tensor, mask: Tensor, pose: Tensor, intrinsics: Tensor) -> Tensor:
     """Returns the XYZ coordinates for a set of points.
 
@@ -147,15 +155,15 @@
     # Mask out bad depth points.
     xyz = xyz.unflatten(1, (height, width))
     xyz[mask.squeeze(1)] = 0.0
 
     return xyz
 
 
-def iter_xyz(ds: Dataset[PosedRGBDItem], desc: str, chunk_size: int = 16) -> Iterator[Tuple[Tensor, Tensor]]:
+def iter_xyz(ds: Dataset[PosedRGBDItem], desc: str, chunk_size: int = 16) -> Iterator[tuple[Tensor, Tensor]]:
     """Iterates XYZ points from the dataset.
 
     Args:
         ds: The dataset to iterate points from
         desc: TQDM bar description
         chunk_size: Process this many frames from the dataset at a time
 
@@ -175,38 +183,38 @@
                 *((device.tensor_to(t) for t in (i.depth, i.mask, i.pose, i.intrinsics)) for i in (ds[i] for i in inds))
             )
         )
         xyz = get_xyz(depth, mask, pose, intrinsics)
         yield xyz, mask.squeeze(1)
 
 
-def get_poses(ds: Dataset[PosedRGBDItem], cache_dir: Optional[Path] = None) -> np.ndarray:
+def get_poses(ds: Dataset[PosedRGBDItem], cache_dir: Path | None = None) -> np.ndarray:
     # pylint: disable=unsupported-assignment-operation,unsubscriptable-object
     cache_loc = None if cache_dir is None else cache_dir / "poses.npy"
 
     if cache_loc is not None and cache_loc.is_file():
         return np.load(cache_loc)
 
-    all_poses: List[np.ndarray] = []
+    all_poses: list[np.ndarray] = []
     for item in tqdm.tqdm(ds, desc="Poses"):
         all_poses.append(item.pose.cpu().numpy())
 
     poses = np.stack(all_poses)
     if cache_loc is not None:
         cache_loc.parent.mkdir(exist_ok=True, parents=True)
         np.save(cache_loc, poses)
 
     return poses
 
 
-def get_pose_bounds(ds: Dataset[PosedRGBDItem], cache_dir: Optional[Path] = None) -> Bounds:
+def get_pose_bounds(ds: Dataset[PosedRGBDItem], cache_dir: Path | None = None) -> Bounds:
     # pylint: disable=unsupported-assignment-operation,unsubscriptable-object
     cache_loc = None if cache_dir is None else cache_dir / "pose_bounds.npy"
 
-    bounds: Optional[np.ndarray] = None
+    bounds: np.ndarray | None = None
 
     if cache_loc is not None and cache_loc.is_file():
         bounds = np.load(cache_loc)
     else:
         for item in tqdm.tqdm(ds, desc="Pose bounds"):
             xyz = item.pose[..., :3, 3].cpu().numpy()
             if bounds is None:
@@ -219,19 +227,19 @@
             cache_loc.parent.mkdir(exist_ok=True, parents=True)
             np.save(cache_loc, bounds)
 
     assert bounds is not None, "No samples found"
     return Bounds.from_arr(bounds)
 
 
-def get_bounds(ds: Dataset[PosedRGBDItem], cache_dir: Optional[Path] = None) -> Bounds:
+def get_bounds(ds: Dataset[PosedRGBDItem], cache_dir: Path | None = None) -> Bounds:
     # pylint: disable=unsupported-assignment-operation,unsubscriptable-object
     cache_loc = None if cache_dir is None else cache_dir / "bounds.npy"
 
-    bounds: Optional[np.ndarray] = None
+    bounds: np.ndarray | None = None
 
     if cache_loc is not None and cache_loc.is_file():
         bounds = np.load(cache_loc)
     else:
         for xyz, mask in iter_xyz(ds, "Bounds"):
             xyz_flat = xyz[~mask]
             minv_torch, maxv_torch = xyz_flat.aminmax(dim=0)
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/r3d.py` & `usa-net-0.0.3/usa/tasks/datasets/r3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import logging
 import re
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Tuple
 from zipfile import ZipFile
 
 import cv2
 import liblzfse
 import ml.api as ml
 import numpy as np
 import torch
@@ -19,30 +18,30 @@
 from tqdm import tqdm
 
 from usa.tasks.datasets.types import PosedRGBDItem
 from usa.tasks.datasets.utils import visualize_posed_rgbd_dataset
 
 logger = logging.getLogger(__name__)
 
-LAB_DATASET_URL = "https://github.com/codekansas/usa/releases/download/v1.0.0/lab.r3d"
-STUDIO_DATASET_URL = "https://github.com/codekansas/usa/releases/download/v1.0.0/studio.r3d"
+LAB_DATASET_URL = "https://github.com/codekansas/usa/releases/download/v0.0.2/lab.r3d"
+STUDIO_DATASET_URL = "https://github.com/codekansas/usa/releases/download/v0.0.2/studio.r3d"
 
 
 @dataclass(frozen=True)
 class Metadata:
-    rgb_shape: Tuple[int, int]
-    depth_shape: Tuple[int, int]
+    rgb_shape: tuple[int, int]
+    depth_shape: tuple[int, int]
     fps: int
     timestamps: np.ndarray  # (T) the camera frame timestamps
     intrinsics: np.ndarray  # (3, 3) intrinsics matrix
     poses: np.ndarray  # (T, 4, 4) camera pose matrices
     start_pose: np.ndarray  # (4, 4) initial camera pose matrix
 
 
-def as_pose_matrix(pose: List[float]) -> np.ndarray:
+def as_pose_matrix(pose: list[float]) -> np.ndarray:
     """Converts a list of pose parameters to a pose matrix.
 
     Args:
         pose: The list of pose parametres, (qx, qy, qz, qw, px, py, pz)
 
     Returns:
         A (4, 4) pose matrix
@@ -55,15 +54,15 @@
     return mat
 
 
 def get_arrs(
     r3d_file: ZipFile,
     meta: Metadata,
     use_depth_shape: bool = True,
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Loads the arrays from the .r3d file.
 
     Args:
         r3d_file: The open .r3d file
         meta: The metadata loaded from the file
         use_depth_shape: If True, the image array will be resized to the depth
             shape; otherwise, the depth array will be resized to the image
@@ -82,15 +81,15 @@
     depth_re_expr = re.compile(r"^rgbd/(\d+).depth$")
     conf_re_expr = re.compile(r"^rgbd/(\d+).conf$")
 
     tsz = meta.timestamps.shape[0]
     rgb_h, rgb_w = meta.rgb_shape
     depth_h, depth_w = meta.depth_shape
 
-    def get_filenames(expr: re.Pattern) -> List[str]:
+    def get_filenames(expr: re.Pattern) -> list[str]:
         re_matches = sorted(
             [re_match for re_match in (expr.match(f.filename) for f in r3d_file.filelist) if re_match is not None],
             key=lambda m: int(m.group(1)),
         )
         return [m.group() for m in re_matches]
 
     def to_img_shape(arr: np.ndarray) -> np.ndarray:
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/replica_cad.py` & `usa-net-0.0.3/usa/tasks/datasets/replica_cad.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # From the Google Drive folder here: https://drive.google.com/drive/folders/1nzAVDInjDwt_GFehyhkOZvXrRJ33FCaR
 # EVAL_PTS_URL = "https://drive.google.com/file/d/1ECNbnf9FBCxfWr_IZK_WRwybLKfYyuyE/view?usp=sharing"
 # GT_SDFS_URL = "https://drive.google.com/file/d/1qFI2Pd9td8CaRKpSarvOlqdB3b-FRoKw/view?usp=sharing"
 # SEQS_URL = "https://drive.google.com/file/d/1IUCymFSKFOno9CRGo6gNnZieb1jDpzoi/view?usp=sharing"
 
 # From the project repo (original ZIP was corrupted for some reason).
-SEQS_URL = "https://github.com/codekansas/usa/releases/download/v1.0.0/replica.zip"
+SEQS_URL = "https://github.com/codekansas/usa/releases/download/v0.0.2/replica.zip"
 
 
 def intrinsics_matrix(fx: float, fy: float, cx: float, cy: float) -> Tensor:
     intr = np.eye(3, dtype=np.float64)
     intr[0, 0] = fx
     intr[1, 1] = fy
     intr[0, 2] = cx
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/stretch.py` & `usa-net-0.0.3/usa/tasks/datasets/stretch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle as pkl
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Dict, Iterator, List, Tuple
+from typing import Any, Iterator
 
 import ml.api as ml
 import numpy as np
 import torch
 import torchvision.transforms.functional as V
 import tqdm
 from quaternion import as_rotation_matrix, quaternion
@@ -17,46 +17,46 @@
 
 # Pre-recorded clips used in paper.
 LAB_CLIP_URL = "https://drive.google.com/file/d/1-bJ08bSnMFqz82OolCSbiyY430UstNzL/view?usp=share_link"
 KITCHEN_CLIP_URL = "https://drive.google.com/file/d/133D0ydVu2I3ddS69qdoJ-5HtcRgyrvgf/view?usp=share_link"
 CHESS_CLIP_URL = "https://drive.google.com/file/d/1ElpXCMclP9xocU1Kd5OyrtkO3UNSbzf8/view?usp=share_link"
 
 
-def iter_raw(path: Path) -> Iterator[Dict[str, Any]]:
+def iter_raw(path: Path) -> Iterator[dict[str, Any]]:
     with open(path, "rb") as f:
         while True:
             try:
                 yield pkl.load(f)
             except EOFError:
                 break
 
 
 @dataclass
 class OccupancyMap:
     image: np.ndarray
-    shape: Tuple[int, int]
-    origin: Tuple[float, float]
+    shape: tuple[int, int]
+    origin: tuple[float, float]
     resolution: float
 
 
 @dataclass
 class Data:
     color_imgs: np.ndarray
     depth_imgs: np.ndarray
     poses: np.ndarray
     intrinsics: np.ndarray
-    occupancy_maps: List[OccupancyMap]
+    occupancy_maps: list[OccupancyMap]
 
 
 def load_data(path: Path) -> Data:
-    color_imgs: List[np.ndarray] = []
-    depth_imgs: List[np.ndarray] = []
-    poses: List[np.ndarray] = []
-    intrinsics: List[np.ndarray] = []
-    occupancy_maps: List[OccupancyMap] = []
+    color_imgs: list[np.ndarray] = []
+    depth_imgs: list[np.ndarray] = []
+    poses: list[np.ndarray] = []
+    intrinsics: list[np.ndarray] = []
+    occupancy_maps: list[OccupancyMap] = []
     for data in tqdm.tqdm(iter_raw(path), disable=ml.is_distributed(), desc="Loading data"):
         color_img = data["color"]["image"]
         depth_img = data["depth"]["image"]
 
         # Gets the occupancy map for the current frame.
         occ_map_data = data["occupancy_map"]
         occupancy_map = OccupancyMap(
@@ -107,15 +107,15 @@
         depth_imgs=np.stack(depth_imgs, axis=0),
         poses=np.stack(poses, axis=0),
         intrinsics=np.stack(intrinsics, axis=0),
         occupancy_maps=occupancy_maps,
     )
 
 
-def load_pose(path: Path) -> Tuple[np.ndarray, List[Tuple[int, int]]]:
+def load_pose(path: Path) -> tuple[np.ndarray, list[tuple[int, int]]]:
     inds = np.genfromtxt(path, delimiter=",", skip_header=True, usecols=[2, 3], dtype=np.int64)
     poses = np.genfromtxt(path, delimiter=",", skip_header=True, usecols=[4, 5, 6, 7, 8, 9, 10])
     mat = np.eye(4, dtype=np.float64)[None, :, :].repeat(poses.shape[0], axis=0)
     mat[:, :3, :3] = np.stack([as_rotation_matrix(quaternion(qw, qx, qy, qz)) for qw, qx, qy, qz in poses[:, 3:]])
     mat[:, :3, 3] = poses[:, :3]
     ids = list((a, b) for a, b in zip(inds[:, 0].tolist(), inds[:, 1].tolist()))
     return mat, ids
```

### Comparing `usa-net-0.0.1/usa/tasks/datasets/utils.py` & `usa-net-0.0.3/usa/tasks/datasets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import logging
 import os
 import time
 from pathlib import Path
-from typing import Iterator, Tuple
+from typing import Iterator
 
 import ml.api as ml
 import numpy as np
 import open3d as o3d
 import torch
 import tqdm
 from torch import Tensor
@@ -138,22 +138,26 @@
     intrinsics = intrinsics[batch_inds]
     pose = pose[batch_inds]
 
     # Gets the depths for each coordinate.
     depth = depth[flipped_mask]
 
     # Gets the pixel grid.
-    xs, ys = torch.meshgrid(torch.arange(width), torch.arange(height), indexing="xy")
+    xs, ys = torch.meshgrid(
+        torch.arange(width, device=depth.device),
+        torch.arange(height, device=depth.device),
+        indexing="xy",
+    )
     xy = torch.stack([xs, ys], dim=-1)[None, :, :].repeat_interleave(bsz, dim=0)
     xy = xy[flipped_mask.squeeze(1)]
 
     return get_xyz_coordinates_from_xy(depth, xy, pose, intrinsics)
 
 
-def get_nearest_xyz(all_xyz: Tensor, xyz: Tensor) -> Tuple[Tensor, Tensor]:
+def get_nearest_xyz(all_xyz: Tensor, xyz: Tensor) -> tuple[Tensor, Tensor]:
     """Gets nearest neighbor coordinates.
 
     Args:
         all_xyz: The points to compare to, with shape (B, 3)
         xyz: The points to get nearest neighbors to, with shape (N, 3)
 
     Returns:
```

### Comparing `usa-net-0.0.1/usa_net.egg-info/SOURCES.txt` & `usa-net-0.0.3/usa_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

