# Comparing `tmp/toggl-track-0.4.0.tar.gz` & `tmp/toggl-track-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggl-track-0.4.0.tar", last modified: Sat Mar 11 12:24:37 2023, max compression
+gzip compressed data, was "toggl-track-0.5.0.tar", last modified: Mon Apr 17 22:49:47 2023, max compression
```

## Comparing `toggl-track-0.4.0.tar` & `toggl-track-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:24:37.100764 toggl-track-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-11 12:24:20.000000 toggl-track-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-11 12:24:37.100764 toggl-track-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-03-11 12:24:20.000000 toggl-track-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:24:37.100764 toggl-track-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-11 12:24:20.000000 toggl-track-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:24:37.100764 toggl-track-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-03-11 12:24:20.000000 toggl-track-0.4.0/tests/test_entries_group_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-03-11 12:24:20.000000 toggl-track-0.4.0/tests/test_entries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-11 12:24:20.000000 toggl-track-0.4.0/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-11 12:24:20.000000 toggl-track-0.4.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:24:37.100764 toggl-track-0.4.0/toggl_track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:24:20.000000 toggl-track-0.4.0/toggl_track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-11 12:24:20.000000 toggl-track-0.4.0/toggl_track/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-11 12:24:20.000000 toggl-track-0.4.0/toggl_track/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-11 12:24:20.000000 toggl-track-0.4.0/toggl_track/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-11 12:24:20.000000 toggl-track-0.4.0/toggl_track/toggl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:24:37.100764 toggl-track-0.4.0/toggl_track.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-11 12:24:37.000000 toggl-track-0.4.0/toggl_track.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 22:49:27.000000 toggl-track-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-17 22:49:47.029955 toggl-track-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-17 22:49:27.000000 toggl-track-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:49:47.029955 toggl-track-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-17 22:49:27.000000 toggl-track-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.025954 toggl-track-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_entries_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19564 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_entries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 22:49:27.000000 toggl-track-0.5.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/toggl_track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-17 22:49:27.000000 toggl-track-0.5.0/toggl_track/toggl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:49:47.029955 toggl-track-0.5.0/toggl_track.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 22:49:47.000000 toggl-track-0.5.0/toggl_track.egg-info/top_level.txt
```

### Comparing `toggl-track-0.4.0/LICENSE` & `toggl-track-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toggl-track-0.4.0/PKG-INFO` & `toggl-track-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggl-track
-Version: 0.4.0
+Version: 0.5.0
 Summary: CLI tool and Python library to access Toggl Track https://toggl.com/track/
 Home-page: https://github.com/zmoog/toggl-track
 Author: Maurizio Branca
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/zmoog/toggl-track/issues
 Project-URL: CI, https://github.com/zmoog/toggl-track/actions
 Project-URL: Changelog, https://github.com/zmoog/toggl-track/releases
@@ -48,15 +48,15 @@
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       02:37 PM   03:15 PM   0:38       type:support
     2023-02-03   Rosanna                                                                      11:06 AM   02:37 PM   3:31
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       09:25 AM   11:06 AM   1:41       type:support
     2023-02-03   sync                                                                         08:37 AM   09:25 AM   0:48       type:sync
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
                                                                                                         Total      13:08
 
-Now you can also filter time entries by project ID:
+Now you can also filter time entries by project ID or description:
 
     $ tgl entries --project-id 178435728 list
                                                                 Time Entries
 
     At           Description                                                                  Start      Stop       Duration   Tags
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
     2023-02-03   Community: Allow parsing of IPv6 addresses in ingest pipeline                08:18 PM   10:09 PM   1:51       type:support
@@ -66,14 +66,40 @@
     2023-02-03   Community: Fix parsing error client port is blank and adjust for timeStamp   03:15 PM   04:21 PM   1:05       type:support
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       02:37 PM   03:15 PM   0:38       type:support
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       09:25 AM   11:06 AM   1:41       type:support
     2023-02-03   sync                                                                         08:37 AM   09:25 AM   0:48       type:sync
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
                                                                                                         Total      7:05
 
+    $ tgl entries --description SDH list
+
+                                Time Entries                                
+                                                                                
+    At           Description   Start      Stop       Duration   Tags          
+    ────────────────────────────────────────────────────────────────────────── 
+    2023-04-01   SDH 3256      05:56 AM   07:01 AM   1:04       type:support  
+    2023-03-31   SDH 3256      03:01 PM   04:18 PM   1:17       type:support  
+    2023-03-31   SDH 3247      09:45 AM   12:04 PM   2:18       type:support  
+    2023-03-31   SDH 3253      08:49 AM   09:45 AM   0:56       type:support  
+    2023-03-31   SDH 3237      07:22 AM   08:30 AM   1:08       type:support  
+    2023-03-30   SDH 3229      01:16 PM   05:35 PM   4:18       type:support  
+    2023-03-30   SDH 3229      09:36 AM   11:31 AM   1:55       type:support  
+    2023-04-03   SDH 3140      08:11 AM   09:19 AM   1:07       type:support  
+    2023-03-29   SDH 3149      01:36 PM   05:04 PM   3:27       type:support  
+    2023-03-28   SDH 3237      05:04 PM   06:03 PM   0:58       type:support  
+    2023-03-28   SDH 3237      02:40 PM   03:01 PM   0:20       type:support  
+    2023-03-28   SDH 3237      01:43 PM   02:21 PM   0:38       type:support  
+    2023-03-28   SDH 3237      10:31 AM   12:17 PM   1:46       type:support  
+    2023-03-27   SDH 3069      08:50 PM   09:29 PM   0:39       type:support  
+    2023-03-27   SDH 3069      05:51 PM   06:56 PM   1:05       type:support  
+    2023-03-27   SDH 3069      04:59 PM   05:21 PM   0:21       type:support  
+    2023-03-27   SDH 3069      01:11 PM   03:09 PM   1:57       type:support  
+    ──────────────────────────────────────────────────────────────────────────
+                                            Total      25:22
+
 Supports JSON and NDJSON as alternative output format using the  `--format` option:
 
     # format result as a list of objects
     $ tgl --format ndjson entries --project-id 178435728 list
 
     [{"id": 2848841800, "workspace_id": 1815018, "user_id": 2621333, "project_id": 178435728, "task_id": null, "billable": false, "at": "2023-02-16T15:54:40+00:00", "description": "Observability Demo Day",  ... "stop": "2023-02-16T06:59:01+00:00", "duration": 314, "tags": ["type:goal"]}]
```

### Comparing `toggl-track-0.4.0/README.md` & `toggl-track-0.5.0/toggl_track.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: toggl-track
+Version: 0.5.0
+Summary: CLI tool and Python library to access Toggl Track https://toggl.com/track/
+Home-page: https://github.com/zmoog/toggl-track
+Author: Maurizio Branca
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/zmoog/toggl-track/issues
+Project-URL: CI, https://github.com/zmoog/toggl-track/actions
+Project-URL: Changelog, https://github.com/zmoog/toggl-track/releases
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # toggl-track
 
 [![PyPI](https://img.shields.io/pypi/v/toggl-track.svg)](https://pypi.org/project/toggl-track/)
 [![Changelog](https://img.shields.io/github/v/release/zmoog/toggl-track?include_prereleases&label=changelog)](https://github.com/zmoog/toggl-track/releases)
 [![Tests](https://github.com/zmoog/toggl-track/workflows/Test/badge.svg)](https://github.com/zmoog/toggl-track/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/zmoog/toggl-track/blob/master/LICENSE)
 
@@ -33,15 +48,15 @@
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       02:37 PM   03:15 PM   0:38       type:support
     2023-02-03   Rosanna                                                                      11:06 AM   02:37 PM   3:31
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       09:25 AM   11:06 AM   1:41       type:support
     2023-02-03   sync                                                                         08:37 AM   09:25 AM   0:48       type:sync
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
                                                                                                         Total      13:08
 
-Now you can also filter time entries by project ID:
+Now you can also filter time entries by project ID or description:
 
     $ tgl entries --project-id 178435728 list
                                                                 Time Entries
 
     At           Description                                                                  Start      Stop       Duration   Tags
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
     2023-02-03   Community: Allow parsing of IPv6 addresses in ingest pipeline                08:18 PM   10:09 PM   1:51       type:support
@@ -51,14 +66,40 @@
     2023-02-03   Community: Fix parsing error client port is blank and adjust for timeStamp   03:15 PM   04:21 PM   1:05       type:support
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       02:37 PM   03:15 PM   0:38       type:support
     2023-02-03   Community: Azure Signin Module authentication_processing_details Issue       09:25 AM   11:06 AM   1:41       type:support
     2023-02-03   sync                                                                         08:37 AM   09:25 AM   0:48       type:sync
     ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
                                                                                                         Total      7:05
 
+    $ tgl entries --description SDH list
+
+                                Time Entries                                
+                                                                                
+    At           Description   Start      Stop       Duration   Tags          
+    ────────────────────────────────────────────────────────────────────────── 
+    2023-04-01   SDH 3256      05:56 AM   07:01 AM   1:04       type:support  
+    2023-03-31   SDH 3256      03:01 PM   04:18 PM   1:17       type:support  
+    2023-03-31   SDH 3247      09:45 AM   12:04 PM   2:18       type:support  
+    2023-03-31   SDH 3253      08:49 AM   09:45 AM   0:56       type:support  
+    2023-03-31   SDH 3237      07:22 AM   08:30 AM   1:08       type:support  
+    2023-03-30   SDH 3229      01:16 PM   05:35 PM   4:18       type:support  
+    2023-03-30   SDH 3229      09:36 AM   11:31 AM   1:55       type:support  
+    2023-04-03   SDH 3140      08:11 AM   09:19 AM   1:07       type:support  
+    2023-03-29   SDH 3149      01:36 PM   05:04 PM   3:27       type:support  
+    2023-03-28   SDH 3237      05:04 PM   06:03 PM   0:58       type:support  
+    2023-03-28   SDH 3237      02:40 PM   03:01 PM   0:20       type:support  
+    2023-03-28   SDH 3237      01:43 PM   02:21 PM   0:38       type:support  
+    2023-03-28   SDH 3237      10:31 AM   12:17 PM   1:46       type:support  
+    2023-03-27   SDH 3069      08:50 PM   09:29 PM   0:39       type:support  
+    2023-03-27   SDH 3069      05:51 PM   06:56 PM   1:05       type:support  
+    2023-03-27   SDH 3069      04:59 PM   05:21 PM   0:21       type:support  
+    2023-03-27   SDH 3069      01:11 PM   03:09 PM   1:57       type:support  
+    ──────────────────────────────────────────────────────────────────────────
+                                            Total      25:22
+
 Supports JSON and NDJSON as alternative output format using the  `--format` option:
 
     # format result as a list of objects
     $ tgl --format ndjson entries --project-id 178435728 list
 
     [{"id": 2848841800, "workspace_id": 1815018, "user_id": 2621333, "project_id": 178435728, "task_id": null, "billable": false, "at": "2023-02-16T15:54:40+00:00", "description": "Observability Demo Day",  ... "stop": "2023-02-16T06:59:01+00:00", "duration": 314, "tags": ["type:goal"]}]
```

### Comparing `toggl-track-0.4.0/setup.py` & `toggl-track-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4.0"
+VERSION = "0.5.0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `toggl-track-0.4.0/tests/test_entries_group_by.py` & `toggl-track-0.5.0/tests/test_entries_group_by.py`

 * *Files identical despite different names*

### Comparing `toggl-track-0.4.0/tests/test_entries_list.py` & `toggl-track-0.5.0/tests/test_entries_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,46 @@
 env = {
     "TOGGL_API_TOKEN": "1234567890abcdef1234567890abcdef", # fake token for testing
 }
 
 
 @pytest.mark.vcr
 @pytest.mark.block_network
+def test_list_filter_by_description(save_to_tmp):
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        result = runner.invoke(
+            cli,
+            ["entries", "--description", "toggl-track", "list", "--start-date", "2023-01-26", "--end-date", "2023-01-27"],
+            env=env,
+        )
+        save_to_tmp(result.output, name="test_list_filter_by_description")
+        assert result.exit_code == 0
+        assert (
+            result.output
+            == """                                  Time Entries                                  
+                                                                                
+  At           Description               Start      Stop       Duration   Tags  
+ ────────────────────────────────────────────────────────────────────────────── 
+  2023-01-26   toggl-track: list time    07:28 AM   08:08 AM   0:39             
+               entries                                                          
+  2023-01-26   toggl-track: list time    06:48 AM   07:17 AM   0:28             
+               entries                                                          
+  2023-01-26   toggl-track: list time    05:11 AM   06:06 AM   0:54             
+               entries                                                          
+ ────────────────────────────────────────────────────────────────────────────── 
+                                                    Total      2:02             
+                                                                                
+
+"""
+        )
+        
+
+@pytest.mark.vcr
+@pytest.mark.block_network
 def test_list(save_to_tmp):
     runner = CliRunner()
     with runner.isolated_filesystem():
         result = runner.invoke(
             cli,
             ["entries", "list", "--start-date", "2023-01-26", "--end-date", "2023-01-27"],
             env=env,
```

### Comparing `toggl-track-0.4.0/tests/test_result.py` & `toggl-track-0.5.0/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `toggl-track-0.4.0/toggl_track/cli.py` & `toggl-track-0.5.0/toggl_track/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,22 +36,28 @@
     "CLI tool and Python library to access Toggl Track https://toggl.com/track/"
     ctx.ensure_object(dict)
     ctx.obj['format'] = format
     ctx.obj['json_root'] = json_root
 
 @cli.group()
 @click.option(
+    '--description',
+    '-d',
+    type=click.STRING,
+    multiple=False)
+@click.option(
     '--project-id',
     '-p',
     type=click.INT,
     multiple=True)
 @click.pass_context
-def entries(ctx: click.Context, project_id: List[int]):
+def entries(ctx: click.Context, description: List[str], project_id: List[int]):
     "Time entries commands"
     ctx.ensure_object(dict)
+    ctx.obj['description'] = description
     ctx.obj['project_id'] = project_id
 
 
 @entries.command(name="list")
 @click.option(
     "--start-date",
     type=click.DateTime(),
@@ -68,15 +74,15 @@
     """Returns a list of the latest time entries (default: last 24 hours)"""
 
     client = TimeEntries.from_environment()
 
     click.echo(
         render(
             TimeEntriesListResult(
-                client.list(start_date, end_date, project_ids=ctx.obj['project_id'])
+                client.list(start_date, end_date, project_ids=ctx.obj['project_id'], description=ctx.obj['description'])
             ),
             format=ctx.obj['format'],
             json_root=ctx.obj['json_root'],
         )
     )
 
 
@@ -101,15 +107,15 @@
     """Returns a list of time entries grouped by a field"""
 
     client = TimeEntries.from_environment()
 
     click.echo(
         render(
             TimeEntriesGroupByResult(
-                client.list(start_date, end_date, project_ids=ctx.obj['project_id']),
+                client.list(start_date, end_date, project_ids=ctx.obj['project_id'], description=ctx.obj['description']),
                 key_func=GroupByCriterion(field)
             ),
             format=ctx.obj['format'],
             json_root=ctx.obj['json_root'],
         ),
         nl=True,  # add a newline at the end of the output
     )
```

### Comparing `toggl-track-0.4.0/toggl_track/result.py` & `toggl-track-0.5.0/toggl_track/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import io
 import json
 import datetime as dt
 from itertools import groupby
-from typing import Any, List
+from typing import Any, Iterator, List
 
 from pydantic.json import pydantic_encoder
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from .toggl import TimeEntry
 
 
 class TimeEntriesListResult(object):
-    """Turns a list of TimeEntry objects into a rich table"""
+    """Turns a TimeEntry iterator into a rich table"""
 
-    def __init__(self, entries: List[TimeEntry]) -> None:
-        self.entries = entries
+    def __init__(self, entries: Iterator[TimeEntry]) -> None:
+        self.entries = list(entries)  # we iterate over the entries twice
 
     def __str__(self) -> str:
         """Returns a rich table as a string."""
         
         if not self.entries:
             return "No time entries found."
 
@@ -78,17 +78,17 @@
     def __call__(self, time_entry: TimeEntry) -> Any:
         v = getattr(time_entry, self.name)
         if isinstance(v, List):
             return "".join(v)
         return v
 
 class TimeEntriesGroupByResult(object):
-    """Turns a list of TimeEntry objects into a rich table grouped by a criterion."""
+    """Turns a TimeEntry iterator into a rich table grouped by a criterion."""
 
-    def __init__(self, entries: List[TimeEntry], key_func: GroupByCriterion) -> None:
+    def __init__(self, entries: Iterator[TimeEntry], key_func: GroupByCriterion) -> None:
         self.key_func = key_func
 
         # group entries by key_func
         grouped_entries = groupby(
             sorted(  # sort before grouping
                 entries,
                 key=key_func,
```

### Comparing `toggl-track-0.4.0/toggl_track/toggl.py` & `toggl-track-0.5.0/toggl_track/toggl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import urllib
 from datetime import datetime
-from typing import Optional, List
+from typing import Optional, Iterator, List
 
 import requests
 from pydantic import BaseModel, parse_raw_as
-from typing import List
 
 
 class TimeEntry(BaseModel):
     """TimeEntry model."""
     id: int
     workspace_id: int
     user_id: int
@@ -40,15 +39,15 @@
         if "TOGGL_API_TOKEN" not in os.environ:
             raise Exception(
                 "TOGGL_API_TOKEN environment variable not found. "
                 "Please set it to your Toggl Track API token."
             )
         return cls(api_token=os.environ["TOGGL_API_TOKEN"])
 
-    def list(self, start_date: datetime, end_date: datetime, project_ids: List[int] = ()) -> List[TimeEntry]:
+    def list(self, start_date: datetime, end_date: datetime, description: str = None, project_ids: List[int] = []) -> Iterator[TimeEntry]:
         """Fetches the time entries between `start_date` and `end_date` dates.
         
         Time Entries API v9
         https://developers.track.toggl.com/docs/api/time_entries
         """
         params = dict(
             start_date=start_date.isoformat() + "Z",
@@ -63,12 +62,15 @@
         resp = requests.get(url, auth=(self.api_token, "api_token"))
         if resp.status_code != 200:
             raise Exception(resp.text)
 
         # it looks like the API doesn't support filtering, so I suppose
         # we have to do it ourselves
         entries = parse_raw_as(List[TimeEntry], resp.text)
-        
+
+        if description:
+            entries = filter(lambda entry: description in entry.initiative, entries)
+
         if project_ids:
-            return list(filter(lambda entry: entry.project_id in project_ids, entries))
+            entries = filter(lambda entry: entry.project_id in project_ids, entries)
         
         return entries
```

