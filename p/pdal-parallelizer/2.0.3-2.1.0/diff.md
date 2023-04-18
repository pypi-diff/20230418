# Comparing `tmp/pdal-parallelizer-2.0.3.tar.gz` & `tmp/pdal-parallelizer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdal-parallelizer-2.0.3.tar", last modified: Fri Feb  3 10:57:03 2023, max compression
+gzip compressed data, was "pdal-parallelizer-2.1.0.tar", last modified: Tue Apr 18 09:23:14 2023, max compression
```

## Comparing `pdal-parallelizer-2.0.3.tar` & `pdal-parallelizer-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/
--rw-rw-rw-   0        0        0     1553 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3202 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/README.rst
--rw-rw-rw-   0        0        0       82 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      672 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-03 10:57:03.002787 pdal-parallelizer-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/src/pdal_parallelizer/
--rw-rw-rw-   0        0        0     8522 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/__init__.py
--rw-rw-rw-   0        0        0     1546 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/bounds.py
--rw-rw-rw-   0        0        0     3176 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/cloud.py
--rw-rw-rw-   0        0        0     3281 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/do.py
--rw-rw-rw-   0        0        0     3196 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/file_manager.py
-drwxrwxrwx   0        0        0        0 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/src/pdal_parallelizer/pdal_parallelizer_cli/
--rw-rw-rw-   0        0        0        0 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/pdal_parallelizer_cli/__init__.py
--rw-rw-rw-   0        0        0     2376 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/pdal_parallelizer_cli/__main__.py
--rw-rw-rw-   0        0        0     6603 2023-02-03 10:56:26.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer/tile.py
-drwxrwxrwx   0        0        0        0 2023-02-03 10:57:03.018411 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/
--rw-rw-rw-   0        0        0     3202 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-02-03 10:57:02.000000 pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:23:14.364780 pdal-parallelizer-2.1.0/
+-rw-rw-rw-   0        0        0     1553 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3202 2023-04-18 09:23:14.364780 pdal-parallelizer-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/README.rst
+-rw-rw-rw-   0        0        0       82 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      723 2023-04-18 09:23:14.364780 pdal-parallelizer-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:23:14.349258 pdal-parallelizer-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:23:14.349258 pdal-parallelizer-2.1.0/src/pdal_parallelizer/
+-rw-rw-rw-   0        0        0     6696 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/bounds.py
+-rw-rw-rw-   0        0        0     4859 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/cloud.py
+-rw-rw-rw-   0        0        0     3252 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/do.py
+-rw-rw-rw-   0        0        0     2015 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/file_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:23:14.364780 pdal-parallelizer-2.1.0/src/pdal_parallelizer/pdal_parallelizer_cli/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/pdal_parallelizer_cli/__init__.py
+-rw-rw-rw-   0        0        0     2376 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/pdal_parallelizer_cli/__main__.py
+-rw-rw-rw-   0        0        0     1373 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/pipeline_wrapper.py
+-rw-rw-rw-   0        0        0     2006 2023-04-18 09:22:30.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer/tile.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:23:14.364780 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/
+-rw-rw-rw-   0        0        0     3202 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-18 09:23:14.000000 pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/top_level.txt
```

### Comparing `pdal-parallelizer-2.0.3/LICENSE.txt` & `pdal-parallelizer-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdal-parallelizer-2.0.3/PKG-INFO` & `pdal-parallelizer-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdal-parallelizer
-Version: 2.0.3
+Version: 2.1.0
 Summary: A simple tool for use pdal with parallel execution
 License: BSD 3-Clause License
 Keywords: pdal,parallelizer,dask
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 ================================================
```

### Comparing `pdal-parallelizer-2.0.3/README.rst` & `pdal-parallelizer-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pdal-parallelizer-2.0.3/setup.cfg` & `pdal-parallelizer-2.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6461 6c2d 7061 7261 6c6c 656c   = pdal-parallel
 00000020: 697a 6572 0d0a 7665 7273 696f 6e20 3d20  izer..version = 
-00000030: 322e 302e 330d 0a64 6573 6372 6970 7469  2.0.3..descripti
+00000030: 322e 312e 300d 0a64 6573 6372 6970 7469  2.1.0..descripti
 00000040: 6f6e 203d 2041 2073 696d 706c 6520 746f  on = A simple to
 00000050: 6f6c 2066 6f72 2075 7365 2070 6461 6c20  ol for use pdal 
 00000060: 7769 7468 2070 6172 616c 6c65 6c20 6578  with parallel ex
 00000070: 6563 7574 696f 6e0d 0a6c 6f6e 675f 6465  ecution..long_de
 00000080: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000090: 3a20 5245 4144 4d45 2e72 7374 2c20 4348  : README.rst, CH
 000000a0: 414e 4745 4c4f 472e 7273 742c 204c 4943  ANGELOG.rst, LIC
@@ -18,25 +18,29 @@
 00000110: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000120: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 00000130: 3a20 330d 0a0d 0a5b 6f70 7469 6f6e 735d  : 3....[options]
 00000140: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
 00000150: 0d0a 093d 7372 630d 0a70 6163 6b61 6765  ...=src..package
 00000160: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
 00000170: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000180: 0963 6c69 636b 0d0a 0970 6461 6c0d 0a09  .click...pdal...
-00000190: 5044 414c 0d0a 0964 6173 6b0d 0a09 6469  PDAL...dask...di
-000001a0: 7374 7269 6275 7465 640d 0a09 7477 696e  stributed...twin
-000001b0: 650d 0a09 7061 6e64 6173 0d0a 096d 6174  e...pandas...mat
-000001c0: 706c 6f74 6c69 620d 0a09 7079 7072 6f6a  plotlib...pyproj
-000001d0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-000001e0: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-000001f0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-00000200: 0970 6461 6c2d 7061 7261 6c6c 656c 697a  .pdal-paralleliz
-00000210: 6572 203d 2070 6461 6c5f 7061 7261 6c6c  er = pdal_parall
-00000220: 656c 697a 6572 2e70 6461 6c5f 7061 7261  elizer.pdal_para
-00000230: 6c6c 656c 697a 6572 5f63 6c69 2e5f 5f6d  llelizer_cli.__m
-00000240: 6169 6e5f 5f3a 6d61 696e 0d0a 0d0a 5b6f  ain__:main....[o
-00000250: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000260: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-00000270: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
-00000280: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000290: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000180: 0963 6c69 636b 3c3d 382e 312e 330d 0a09  .click<=8.1.3...
+00000190: 7064 616c 3c3d 332e 322e 320d 0a09 6461  pdal<=3.2.2...da
+000001a0: 736b 3c3d 3230 3233 2e31 2e31 0d0a 0964  sk<=2023.1.1...d
+000001b0: 6973 7472 6962 7574 6564 3c3d 3230 3233  istributed<=2023
+000001c0: 2e31 2e31 0d0a 0974 7769 6e65 3c3d 342e  .1.1...twine<=4.
+000001d0: 302e 320d 0a09 7061 6e64 6173 3c3d 312e  0.2...pandas<=1.
+000001e0: 352e 330d 0a09 7079 7072 6f6a 3c3d 332e  5.3...pyproj<=3.
+000001f0: 342e 310d 0a09 6e75 6d70 793c 3d31 2e32  4.1...numpy<=1.2
+00000200: 342e 320d 0a0d 0a5b 6f70 7469 6f6e 732e  4.2....[options.
+00000210: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+00000220: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+00000230: 200d 0a09 7064 616c 2d70 6172 616c 6c65   ...pdal-paralle
+00000240: 6c69 7a65 7220 3d20 7064 616c 5f70 6172  lizer = pdal_par
+00000250: 616c 6c65 6c69 7a65 722e 7064 616c 5f70  allelizer.pdal_p
+00000260: 6172 616c 6c65 6c69 7a65 725f 636c 692e  arallelizer_cli.
+00000270: 5f5f 6d61 696e 5f5f 3a6d 6169 6e0d 0a0d  __main__:main...
+00000280: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000290: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000002a0: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
+000002b0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000002c0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000002d0: 0a0d 0a                                  ...
```

### Comparing `pdal-parallelizer-2.0.3/src/pdal_parallelizer/__init__.py` & `pdal-parallelizer-2.1.0/src/pdal_parallelizer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import json
 import logging
-import os
 import os.path
-import click
-import pdal
+import sys
+from os.path import join
+import numpy as np
+import matplotlib.pyplot as plt
+from . import file_manager
+from . import do
+from .cloud import Cloud
 from dask import config as cfg
 from dask.distributed import LocalCluster, Client, progress
 from distributed.diagnostics import MemorySampler
-from os import listdir
-from . import do
-from . import file_manager
-from . import cloud
-from . import tile
-from matplotlib import pyplot as plt
-import sys
-import ntpath
-from os.path import join
-from math import ceil
 
 
 def query_yes_no(question, default='no'):
     valid = {'yes': True, 'y': True, 'ye': True, 'no': False, 'n': False}
     if default is None:
         prompt = ' [y/n] '
     elif default == 'yes':
@@ -38,178 +32,150 @@
         elif choice in valid:
             return valid[choice]
         else:
             sys.stdout.write('Please respond with "yes" or "no" (or "y" or "n").\n')
 
 
 def config_dask(n_workers, threads_per_worker, timeout):
-    """Make some configuration to avoid workers errors due to heartbeat or timeout problems. Set the number of cores
-    to process the pipelines """
     if not timeout:
         timeout = input('After how long of inactivity do you want to kill your worker (timeout)\n')
 
     cfg.set({'interface': 'lo'})
     cfg.set({'distributed.scheduler.worker-ttl': None})
     cfg.set({'distributed.comm.timeouts.connect': timeout})
-    cluster = LocalCluster(n_workers=n_workers, threads_per_worker=threads_per_worker, silence_logs=logging.ERROR)
+    cluster = LocalCluster(n_workers=n_workers, threads_per_worker=threads_per_worker, memory_limit=None,
+                           silence_logs=logging.ERROR)
     client = Client(cluster)
     return client
 
 
-def process_pipelines(
-        config,
-        input_type,
-        timeout=None,
-        n_workers=3,
-        threads_per_worker=1,
-        dry_run=None,
-        diagnostic=False,
-        tile_size=(256, 256),
-        buffer=None,
-        remove_buffer=None,
-        bounding_box=None,
-        merge_tiles=False,
-        remove_tiles=False
-):
-    # Assertions
-    assert type(config) is str
-    assert input_type == "single" or input_type == "dir"
-    if timeout:
-        assert type(timeout) is int
-    assert type(n_workers) is int
-    assert type(threads_per_worker) is int
-    if dry_run:
-        assert type(dry_run) is int
-    assert type(diagnostic) is bool
-    assert type(tile_size) is tuple and len(tile_size) == 2
-    if buffer:
-        assert type(buffer) is int
-    if remove_buffer:
-        assert type(remove_buffer) is bool
-    if bounding_box:
-        assert type(bounding_box) is tuple
-        assert len(bounding_box) == 4
-    assert type(merge_tiles) is bool
-    assert type(remove_tiles) is bool
-
-    with open(config, 'r') as c:
-        config_file = json.load(c)
-        input_dir = config_file.get('input')
-        output = config_file.get('output')
-        temp = config_file.get('temp')
-        pipeline = config_file.get('pipeline')
-
+def trigger_warnings(n_workers, input_type, input, output, temp, tile_size):
     if n_workers >= os.cpu_count():
         answer = query_yes_no(
             f'\nWARNING - You choose to launch {n_workers} workers but your machine has only {os.cpu_count()}'
             f' CPUs, please reduce the number of workers.\nDo you want to continue ?'
         )
         if not answer:
             return
 
     if input_type == 'single':
+        c = Cloud(input)
         if tile_size == (256, 256):
             answer = query_yes_no(
                 f'WARNING - You are using the default value of the tile_size option (256 by 256 meters). Please '
                 f'check if your points cloud\'s dimensions are greater than this value.\nDo you want to continue ? '
             )
             if not answer:
                 return
 
-        infos = cloud.compute_quickinfo(input_dir)
-        bounds = infos['summary']['bounds']
-        distX, distY = (
-            int(bounds['maxx'] - bounds['minx']),
-            int(bounds['maxy'] - bounds['miny'])
-        )
-
-        nTilesX = ceil(distX / tile_size[0])
-        nTilesY = ceil(distY / tile_size[0])
-
-        if nTilesX * nTilesY > n_workers:
+    if input_type == 'dir':
+        if input == output or input == temp:
             answer = query_yes_no(
-                f'WARNING - With this size of tiles and this number of workers, each worker will have more than one task'
-                f' and it can blow up the distributed memory. Please choose a larger size for your tiles or increase '
-                f'your number of workers.\nDo you want to continue ?'
+                f'WARNING - Your input folder is the same as your output or temp folder. This could be a problem. '
+                f'Please choose three separate directories.\n Do you want to continue ? '
             )
             if not answer:
                 return
 
+    if len(os.listdir(output)) > 0:
+        answer = query_yes_no(
+            f'WARNING - Your output directory is not empty.\n Do you want to continue ? '
+        )
+        if not answer:
+            return
+
+
+def process_pipelines(
+        config,
+        input_type,
+        timeout=None,
+        n_workers=3,
+        threads_per_worker=1,
+        dry_run=None,
+        diagnostic=None,
+        tile_size=(256, 256),
+        buffer=None,
+        remove_buffer=None,
+        bounding_box=None,
+        merge_tiles=None,
+        remove_tiles=None
+):
+    with open(config, 'r') as c:
+        config_file = json.load(c)
+        input = config_file.get('input')
+        output = config_file.get('output')
+        temp = config_file.get('temp')
+        pipeline = config_file.get('pipeline')
+
+    trigger_warnings(n_workers, input_type, input, output, temp, tile_size)
+
     if not os.path.exists(temp):
         os.mkdir(temp)
 
     if not os.path.exists(output):
         os.mkdir(output)
 
-    # If there is some temp file in the temp directory, these are processed
-    if len(listdir(temp)) != 0:
-        click.echo(
-            f'Something went wrong during previous execution, there is some temp files in your temp '
-            f'directory.\nBeginning of the execution\n')
-        # Get all the deserialized pipelines
-        pipeline_iterator = file_manager.getSerializedPipelines(temp_directory=temp)
-        # Process pipelines
-        delayed = do.process_serialized_pipelines(temp_dir=temp, iterator=pipeline_iterator)
-    else:
-        click.echo('Beginning of the execution\n')
-        # If the user don't specify the dry_run option
-        if not dry_run:
-            # If the user wants to process a single file, it is split. Else, get all the files of the input directory
-            iterator = do.splitCloud(filepath=input_dir,
-                                     output_dir=output,
-                                     json_pipeline=pipeline,
-                                     tile_bounds=tile_size,
-                                     buffer=buffer,
-                                     remove_buffer=remove_buffer,
-                                     bounding_box=bounding_box) if input_type == 'single' \
-                else file_manager.getFiles(input_directory=input_dir)
-            # Process pipelines
-            delayed = do.process_pipelines(output_dir=output, json_pipeline=pipeline, temp_dir=temp, iterator=iterator,
-                                           is_single=(input_type == 'single'))
-        else:
-            # If the user wants to process a single file, it is split and get the number of tiles given by the user.
-            # Else, get the number of files we want to do the test execution (not serialized)
-            iterator = do.splitCloud(filepath=input_dir,
-                                     output_dir=output,
-                                     json_pipeline=pipeline,
-                                     tile_bounds=tile_size,
-                                     nTiles=dry_run,
-                                     buffer=buffer,
-                                     remove_buffer=remove_buffer,
-                                     bounding_box=bounding_box) if input_type == 'single' \
-                else file_manager.getFiles(input_directory=input_dir, nFiles=dry_run)
-            # Process pipelines
-            delayed = do.process_pipelines(output_dir=output, json_pipeline=pipeline, iterator=iterator,
-                                           dry_run=dry_run, is_single=(input_type == 'single'))
-
-    client = config_dask(n_workers=n_workers, threads_per_worker=threads_per_worker, timeout=timeout)
+    client = config_dask(n_workers, threads_per_worker, timeout)
+    ms = MemorySampler()
 
-    click.echo('Parallelization started.\n')
+    if input_type == "single":
+        futures = []
+        c = Cloud(input, bounding_box)
+        if len(os.listdir(temp)) != 0:
+            print("Something went wrong during previous execution, there is some temp files in your temp " +
+                  "directory.\nBeginning of the execution\n")
+            tiles = file_manager.get_serialized_tiles(temp)
+        else:
+            tiles = c.split(tile_size, pipeline, output, buffer, dry_run)
 
-    if diagnostic:
-        ms = MemorySampler()
-        with ms.sample(label='execution', client=client):
-            delayed = client.compute(delayed)
-            progress(delayed)
-        ms.plot()
-    else:
-        delayed = client.compute(delayed)
-        progress(delayed)
+        print("Opening the cloud.\n")
+        image_array = c.load_image_array(pipeline)
 
-    del delayed
+        if bounding_box:
+            image_array = image_array[np.where((image_array["X"] > bounding_box[0]) &
+                                               (image_array["X"] < bounding_box[2]) &
+                                               (image_array["Y"] > bounding_box[1]) &
+                                               (image_array["Y"] < bounding_box[3]))]
+
+        data = do.cut_image_array(tiles, image_array, temp, dry_run)
+
+        print(f"Starting parallelization, visit the dashboard ({client.dashboard_link}) to follow the execution.\n")
+
+        with ms.sample("Execution"):
+            for (array, stages, tile) in data:
+                if len(array) > 0:
+                    big_future = client.scatter(array)
+                    futures.append(
+                        client.submit(do.execute_stages_streaming, big_future, stages, tile, temp, remove_buffer, dry_run))
+                else:
+                    if not dry_run:
+                        os.remove(temp + "/" + tile.name + ".pickle")
 
-    file_manager.getEmptyWeight(output_directory=output)
+            client.gather(futures)
 
-    if merge_tiles and len(listdir(output)) > 1:
-        input_filename = ntpath.basename(input_dir).split('.')[0]
-        writers = tile.get_writers(tile.load_pipeline(pipeline))
-        merge = cloud.merge(output, input_filename, writers)
-        if merge is not None:
-            merge_ppln = pdal.Pipeline(merge)
-            merge_ppln.execute()
+        if merge_tiles:
+            c.merge(output, pipeline)
 
         if remove_tiles:
             for f in os.listdir(output):
-                if f.split('.')[0] != input_filename:
+                if f != os.path.basename(c.filepath) and f.split(".")[1] != "png":
                     os.remove(join(output, f))
+    else:
+        if len(os.listdir(temp)) != 0:
+            print("Something went wrong during previous execution, there is some temp files in your temp " +
+                  "directory.\nBeginning of the execution\n")
+            serialized_data = file_manager.get_serialized_tiles(temp)
+            tasks = do.process_serialized_tiles(serialized_data, temp)
+        else:
+            print("Beginning of the execution.\n")
+            files = file_manager.get_files(input, dry_run)
+            tasks = do.process_several_clouds(files, pipeline, output, temp, buffer, dry_run)
+
+        print("Starting parallelization.\n")
+
+        with ms.sample("Execution"):
+            future = client.persist(tasks)
+            progress(future)
 
-    plt.savefig(output + '/memory-usage.png') if diagnostic else None
+    if diagnostic:
+        ms.plot()
+        plt.savefig(output + "/diagnostic.png")
```

### Comparing `pdal-parallelizer-2.0.3/src/pdal_parallelizer/pdal_parallelizer_cli/__main__.py` & `pdal-parallelizer-2.1.0/src/pdal_parallelizer/pdal_parallelizer_cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import sys
 import click
 from pdal_parallelizer import process_pipelines as process
 
 
 @click.group()
-@click.version_option('2.0.3')
+@click.version_option('2.1.0')
 def main():
     """A simple parallelization tool for 3d point clouds treatment"""
     pass
 
 
 @main.command()
 @click.option('-c', '--config', required=True, type=click.Path(exists=True))
```

### Comparing `pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/PKG-INFO` & `pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdal-parallelizer
-Version: 2.0.3
+Version: 2.1.0
 Summary: A simple tool for use pdal with parallel execution
 License: BSD 3-Clause License
 Keywords: pdal,parallelizer,dask
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 ================================================
```

### Comparing `pdal-parallelizer-2.0.3/src/pdal_parallelizer.egg-info/SOURCES.txt` & `pdal-parallelizer-2.1.0/src/pdal_parallelizer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 src/pdal_parallelizer/__init__.py
 src/pdal_parallelizer/bounds.py
 src/pdal_parallelizer/cloud.py
 src/pdal_parallelizer/do.py
 src/pdal_parallelizer/file_manager.py
+src/pdal_parallelizer/pipeline_wrapper.py
 src/pdal_parallelizer/tile.py
 src/pdal_parallelizer.egg-info/PKG-INFO
 src/pdal_parallelizer.egg-info/SOURCES.txt
 src/pdal_parallelizer.egg-info/dependency_links.txt
 src/pdal_parallelizer.egg-info/entry_points.txt
 src/pdal_parallelizer.egg-info/requires.txt
 src/pdal_parallelizer.egg-info/top_level.txt
```

