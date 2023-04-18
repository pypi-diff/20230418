# Comparing `tmp/rosbag_merge-0.1.2.tar.gz` & `tmp/rosbag_merge-0.1.3.tar.gz`

## Comparing `rosbag_merge-0.1.2.tar` & `rosbag_merge-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/INSTALL.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/requirements.txt
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/.github/workflows/publish-to-pypi-and-test-pypi.yml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/examples/main_direct.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/__init__.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/bag_stream.py
--rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/main.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/csv_merge.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/merge_bags.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/src/rosbag_merge/deprecated/rosbag_to_csv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/topic_list.txt
--rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
--rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
--rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/LICENSE
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 rosbag_merge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/INSTALL.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/.github/workflows/publish-to-pypi-and-test-pypi.yml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/examples/main_direct.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/__init__.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/bag_stream.py
+-rwxr-xr-x   0        0        0     5625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/main.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/deprecated/csv_merge.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/deprecated/merge_bags.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/src/rosbag_merge/deprecated/rosbag_to_csv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/tests/topic_list.txt
+-rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
+-rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
+-rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 rosbag_merge-0.1.3/PKG-INFO
```

### Comparing `rosbag_merge-0.1.2/.github/workflows/publish-to-pypi-and-test-pypi.yml` & `rosbag_merge-0.1.3/.github/workflows/publish-to-pypi-and-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/examples/main_direct.py` & `rosbag_merge-0.1.3/examples/main_direct.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/src/rosbag_merge/bag_stream.py` & `rosbag_merge-0.1.3/src/rosbag_merge/bag_stream.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 
 Helps stream bag data and apply bag writing capabilities.
 
 """
 
-from argparse import Namespace
-from tqdm import tqdm
+import heapq
 import os
-from rosbags.rosbag1 import Reader, Writer, ReaderError, WriterError
-from rosbags.typesys import get_types_from_msg
+from argparse import Namespace
 from contextlib import ExitStack, contextmanager
-import heapq
+
+from rosbags.rosbag1 import Reader, ReaderError, Writer, WriterError
+from rosbags.typesys import get_types_from_msg
+from tqdm import tqdm
 
 """
 Copyright open_rosbag1 and read_messages comes from marv_robotics
 https://gitlab.com/ternaris/marv-robotics/-/blob/master/code/marv-robotics/marv_robotics/bag.py#L360
 # Copyright 2016 - 2018  Ternaris.
 # SPDX-License-Identifier: AGPL-3.0-only
 """
+
+
 @contextmanager
 def open_rosbag1(path):
     try:
         with Reader(path) as bag:
             yield bag
     except ReaderError:
         raise ReaderError(
@@ -29,68 +32,64 @@
                 f'Unindexed bag file: {path}\n'
                 '  File was not copied in full or recording did not finish properly\n'
                 '  Use `rosbag reindex` to index what is there.'
             ),
         ) from None
 
 
-def read_messages(paths, topics=None, start_time=None, end_time=None, wipe_typesys=False):
+def read_messages(paths, topics=None, start_time=None, end_time=None):
     """Iterate chronologically raw BagMessage for topic from paths."""
     # pylint: disable=too-many-locals
-
-    if wipe_typesys:
-        backup = types.FIELDDEFS.copy()
-        for key in list(types.FIELDDEFS.keys()):
-            if key not in [
-                'builtin_interfaces/msg/Time',
-                'builtin_interfaces/msg/Duration',
-                'std_msgs/msg/Header',
-            ]:
-                types.FIELDDEFS.pop(key)
-        MSGDEFCACHE.clear()
-
     with ExitStack() as stack:
-        if wipe_typesys:
-            stack.callback(
-                lambda:
-                (types.FIELDDEFS.clear() or types.FIELDDEFS.update(backup) or MSGDEFCACHE.clear()),
-            )
         bags = [stack.enter_context(open_rosbag1(path)) for path in paths]
-        if wipe_typesys:
-            typs = {}
-            for bag in bags:
-                for rconn in bag.connections:
-                    typs.update(get_types_from_msg(rconn.msgdef, rconn.msgtype))
-            register_types(typs)
-        gens = [
-            bag.messages(
-                connections=[x for x in bag.connections if x.topic in topics],
-                start=start_time,
-                stop=end_time,
-            ) for bag in bags
-        ]
+        gens = []
+        for bag in bags:
+            valid_connections = []
+            if (topics is None):
+                # connect to all topics
+                valid_connections = [x for x in bag.connections]
+            else:
+                valid_connections = [
+                    x for x in bag.connections if x.topic in topics]
+            gens.append(
+                bag.messages(
+                    connections=valid_connections,
+                    start=start_time,
+                    stop=end_time,
+                )
+            )
         prev_time = 0
         for connection, time, data in heapq.merge(*gens, key=lambda x: x[1]):
             assert time >= prev_time, (repr(time), repr(prev_time))
             yield connection, time, data
             prev_time = time
 
-def main(input_bags : 'list[str]', topics : 'list[str]', output_path : str, outbag_name : str):
+
+def main(input_bags: 'list[str]', topics: 'list[str]', output_path: str, outbag_name: str, exists_ok: bool):
     try:
-        full_bag_path = os.path.join(output_path,outbag_name+".bag")
+        full_bag_path = os.path.join(output_path, outbag_name+".bag")
+        # clean up the preexisting bag when the exists_okay flag is present
+        if (exists_ok and os.path.exists(full_bag_path)):
+            os.remove(full_bag_path)
+            for bag_name in input_bags:
+                if (os.path.basename(bag_name) == outbag_name+".bag"):
+                    input_bags.remove(bag_name)
+
         # open the output bag in an automatically closing context
         with Writer(full_bag_path) as output_bag:
             conn_map = {}
             # process messages across input bag(s)
             for connection, timestamp, rawdata in read_messages(input_bags, topics=topics):
                 try:
                     # we're saving by topic, may cause an error if the md5sum changes
-                    conn_map[connection.topic] = output_bag.add_connection(connection.topic, connection.msgtype, connection.msgdef, connection.md5sum, connection.ext.callerid, connection.ext.latching)
+                    conn_map[connection.topic] = output_bag.add_connection(
+                        connection.topic, connection.msgtype, connection.msgdef, connection.md5sum, connection.ext.callerid, connection.ext.latching)
                 except WriterError:
-                     pass
+                    pass
             for connection, timestamp, rawdata in read_messages(input_bags, topics=topics):
                 # write this message to the output bag
-                output_bag.write(conn_map[connection.topic], timestamp, rawdata)    
+                output_bag.write(
+                    conn_map[connection.topic], timestamp, rawdata)
     except KeyboardInterrupt:
         pass
     finally:
         print("Done.")
```

### Comparing `rosbag_merge-0.1.2/src/rosbag_merge/main.py` & `rosbag_merge-0.1.3/src/rosbag_merge/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,140 @@
 #! /usr/bin/env python3
 import argparse
-
-from . import bag_stream
+import glob
 import os
 import sys
-import glob 
 
 from icecream import ic
+
+from . import bag_stream
+
 ic.configureOutput(includeContext=True)
 
 """
 This main file is meant to help interface users with the python package.
 
 """
 
-def refine_args(args:argparse.Namespace)-> argparse.Namespace:
+
+def refine_args(args: argparse.Namespace) -> argparse.Namespace:
     # Refine the arguments to handle simplified inputs such as directories, files with lists of topics, etc.
     retval = args
 
     # make sequence of topics from a topic file
-    if args.topic_file :
+    if args.topic_file:
         if ("topics" not in args) or (not args.topics):
             args.topics = []
         with open(args.topic_file) as f:
             lines = [line.strip() for line in f]
         args.topics.extend(lines)
         ic(args.topics)
     # input files into the respective args Namespace
     if len(args.input_paths):
         for path in args.input_paths:
             for f in os.listdir(path):
-                full_file_path = os.path.join(path,f)
+                full_file_path = os.path.join(path, f)
                 if (f.endswith(".csv")):
                     if "input_csvs" not in args:
                         args.input_csvs = []
                     args.input_csvs.append(full_file_path)
                 elif (f.endswith(".bag")):
                     if "input_bags" not in args:
                         args.input_bags = []
                     args.input_bags.append(full_file_path)
     # TODO, if outpath, then join outpath with out file paths, must also do with the csv writer
-    no_outbag_actions = (not args.outbag_name) and (args.write_bag) 
+    no_outbag_actions = (not args.outbag_name) and (args.write_bag)
     if (no_outbag_actions):
         ic("Writing bags requires an outbag suffix.")
     no_input_files = (("input_bags" not in args) or (not len(args.input_bags)))
     args.write_bag = True if args.output_path and args.outbag_name else False
-    requesting_write_without_output_path =  not args.output_path and (args.merge_csvs or args.write_csvs or args.write_bag)
+    requesting_write_without_output_path = not args.output_path and (
+        args.merge_csvs or args.write_csvs or args.write_bag)
     if (no_outbag_actions or no_input_files or requesting_write_without_output_path):
-        if no_outbag_actions : 
+        if no_outbag_actions:
             ic(no_outbag_actions)
-        if no_input_files : 
+        if no_input_files:
             ic(no_input_files)
-        if requesting_write_without_output_path : 
+        if requesting_write_without_output_path:
             ic(requesting_write_without_output_path)
-        
+
         create_parser().print_help()
         retval = None  # Invalid args, so make it clear
     return retval
 
 
-def create_parser()-> argparse.ArgumentParser:
+def create_parser() -> argparse.ArgumentParser:
     # Creates the appropriate argument parser (separated out to enable printing helps, etc.)
     # create an argument parser to read arguments from the command line
     parser = argparse.ArgumentParser(description=__doc__)
     # add an argument for the output bag to create
     parser.add_argument('--output_path', '-op',
-        type=str,
-        help='The output path for all outputted files. (global paths)',
-        default="./",
-    )
+                        type=str,
+                        help='The output path for all outputted files. (global paths)',
+                        default="./",
+                        )
     parser.add_argument('--outbag_name', '-obn',
-        type=str,
-        help='The output bag name ( file to write to )',
-        default=None,
-    )
+                        type=str,
+                        help='The output bag name ( file to write to )',
+                        default=None,
+                        )
     parser.add_argument('--write_bag', action='store_true')
     # add an argument for the sequence of input bags
     parser.add_argument('--input_bags', '-ib',
-        type=str,
-        nargs='+',
-        help='A list of input bag files. (global paths)',
-        default=[],
-    )
+                        type=str,
+                        nargs='+',
+                        help='A list of input bag files. (global paths)',
+                        default=[],
+                        )
     parser.add_argument('--input_paths', '-ip',
-        type=str,
-        nargs='+',
-        help='A list of input directories with bag files. (global paths)',
-        default="./",
-    )
+                        type=str,
+                        nargs='+',
+                        help='A list of input directories with bag files. (global paths)',
+                        default="./",
+                        )
     # add an argument for the topics to filter
     parser.add_argument('--topics', '-t',
-        type=str,
-        nargs='*',
-        help='A sequence of topics to include from the input bags.',
-        default=None, # or list of strings ['*'],
-        required=False,
-    )
+                        type=str,
+                        nargs='*',
+                        help='A sequence of topics to include from the input bags.',
+                        default=None,  # or list of strings ['*'],
+                        required=False,
+                        )
     parser.add_argument('--topic-file', '-f',
-        type=str,
-        help='A file representing a list of topics. One topic per line.',
-        default=None,
-        required=False,
-    )
+                        type=str,
+                        help='A file representing a list of topics. One topic per line.',
+                        default=None,
+                        required=False,
+                        )
+    parser.add_argument('--exists-ok', '-eo',
+                        type=bool,
+                        help='A true value will remove the file and prevent rosbags exception if the file exists.',
+                        default=True,
+                        required=False,
+                        )
     return parser
 
 
-def parse_args(args)-> argparse.Namespace:
+def parse_args(args) -> argparse.Namespace:
     parser = create_parser()
     # Get the arguments from the argument parser and return
     return parser.parse_args(args)
-    
 
-def main(args:argparse.Namespace=None):
+
+def main(args: argparse.Namespace = None):
     if not args:
         args = parse_args(sys.argv[1:])
     # Refine arguments here so simplified args can be used.
     args = refine_args(args)
     if args is None:
         return  # Invalid arguments, return
-    bag_stream.main(input_bags=args.input_bags 
-                    ,output_path=args.output_path
-                    ,outbag_name=args.outbag_name
-                    ,topics=args.topics
-                    ) 
+    bag_stream.main(input_bags=args.input_bags, output_path=args.output_path, outbag_name=args.outbag_name, topics=args.topics, exists_ok=args.exists_ok
+                    )
+
 
 if __name__ == "__main__":
     # Load command line arguments here so that the main function can be called directly from import
     args = parse_args(sys.argv[1:])
     main(args)
 
 # explicitly define the outward facing API of this module (either command line or direct call to the main function)
-__all__ = [ main.__name__, main ]
+__all__ = [main.__name__, main]
```

### Comparing `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/csv_merge.py` & `rosbag_merge-0.1.3/src/rosbag_merge/deprecated/csv_merge.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/merge_bags.py` & `rosbag_merge-0.1.3/src/rosbag_merge/deprecated/merge_bags.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/src/rosbag_merge/deprecated/rosbag_to_csv.py` & `rosbag_merge-0.1.3/src/rosbag_merge/deprecated/rosbag_to_csv.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag` & `rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag` & `rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag` & `rosbag_merge-0.1.3/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/LICENSE` & `rosbag_merge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/README.md` & `rosbag_merge-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.1.2/pyproject.toml` & `rosbag_merge-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project]
 # add the distribution name of the package, the tar ball and python wheel use this name, this name goes the /home/$USER/.local/lib/python3.8/site-packages/
 name = "rosbag_merge"
 
 # version is the package version. See the version specifier specification
 # for more details on versions. Some build backends allow it to be 
 # specified another way, such as from a file or a git tag.
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Jonathan Sanabria", email="jonsanria@gmail.com" },
 ]
 description = "A gathering of tools for merging rosbags and saving their topic information to csv."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `rosbag_merge-0.1.2/PKG-INFO` & `rosbag_merge-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag_merge
-Version: 0.1.2
+Version: 0.1.3
 Summary: A gathering of tools for merging rosbags and saving their topic information to csv.
 Project-URL: Homepage, https://github.com/1hada/rosbag-merge/
 Project-URL: Bug Tracker, https://github.com/1hada/rosbag-merge/issues/
 Author-email: Jonathan Sanabria <jonsanria@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

