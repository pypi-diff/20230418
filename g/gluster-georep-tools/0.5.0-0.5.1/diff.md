# Comparing `tmp/gluster-georep-tools-0.5.0.tar.gz` & `tmp/gluster-georep-tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluster-georep-tools-0.5.0.tar", last modified: Tue Apr 18 08:31:08 2023, max compression
+gzip compressed data, was "gluster-georep-tools-0.5.1.tar", last modified: Tue Apr 18 16:12:01 2023, max compression
```

## Comparing `gluster-georep-tools-0.5.0.tar` & `gluster-georep-tools-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/.github/workflows/on-release-tag.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 08:31:07.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/status/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/screenshots/gluster-georep-setup.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/.github/workflows/on-release-tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/gluster_georep_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/gluster_georep_tools/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/setup/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/gluster_georep_tools/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/gluster_georep_tools/status/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 16:12:01.000000 gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/screenshots/gluster-georep-setup.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:12:01.420158 gluster-georep-tools-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 16:11:52.000000 gluster-georep-tools-0.5.1/setup.py
```

### Comparing `gluster-georep-tools-0.5.0/.github/workflows/on-release-tag.yml` & `gluster-georep-tools-0.5.1/.github/workflows/on-release-tag.yml`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/.gitignore` & `gluster-georep-tools-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/LICENSE` & `gluster-georep-tools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/PKG-INFO` & `gluster-georep-tools-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluster-georep-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Gluster Geo-replication tools
 Home-page: https://github.com/aravindavk/gluster-georep-tools
 Author: Aravinda Vishwanathapura
 Author-email: mail@aravindavk.in
 License: MIT
 Keywords: gluster,tool,geo-replication
 Platform: linux
```

### Comparing `gluster-georep-tools-0.5.0/README.md` & `gluster-georep-tools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/gluster_georep_tools/setup/cli.py` & `gluster-georep-tools-0.5.1/gluster_georep_tools/setup/cli.py`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/gluster_georep_tools/status/cli.py` & `gluster-georep-tools-0.5.1/gluster_georep_tools/status/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 def apply_filters(status_data, args):
     session_rows = []
     for session in status_data:
         # Collect the Session name and apply filter
         # Session name will be present even though filters don't match
         session_name = "{0} ==> {1}".format(
-            session[0]["mastervol"],
-            session[0]["slave"].replace("ssh://", ""))
+            session[0]["primary_volume"],
+            session[0]["secondary"].replace("ssh://", ""))
         session_rows.append([session_name, {}, []])
 
         summary = {
             "active": 0,
             "passive": 0,
             "created": 0,
             "stopped": 0,
@@ -60,17 +60,17 @@
         print("SESSION: " + session[0])
         table = PrettyTable([
             "PRIMARY", "STATUS",
             "CRAWL STATUS", "SECONDARY NODE", "LAST SYNCED"
         ])
         for row in session[2]:
             table.add_row([
-                row["master_node"] + ":" + row["master_brick"],
+                row["primary_node"] + ":" + row["primary_brick"],
                 row["status"], row["crawl_status"],
-                row["slave_node"], row["last_synced"]
+                row["secondary_node"], row["last_synced"]
             ])
 
         # If Table has data
         if session[2]:
             print(table)
         else:
             # When no filters match
@@ -103,18 +103,18 @@
         secondary_host_tmp, secondary_vol = args.secondary.split("::")
 
         secondary_host_data = secondary_host_tmp.split("@")
         secondary_host = secondary_host_data[-1]
         if len(secondary_host_data) > 1:
             secondary_user = secondary_host_data[0]
 
-    status_data = georep.status(volname=volname,
-                                slave_host=secondary_host,
-                                slave_vol=secondary_vol,
-                                slave_user=secondary_user)
+    status_data = georep.status(primary_volume=volname,
+                                secondary_host=secondary_host,
+                                secondary_volume=secondary_vol,
+                                secondary_user=secondary_user)
 
     if not status_data:
         if args.secondary is not None:
             sys.stderr.write("No active Geo-replication "
                              "sessions between {0} and {1}\n".format(
                                  args.primary_vol,
                                  args.secondary))
```

### Comparing `gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/PKG-INFO` & `gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluster-georep-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Gluster Geo-replication tools
 Home-page: https://github.com/aravindavk/gluster-georep-tools
 Author: Aravinda Vishwanathapura
 Author-email: mail@aravindavk.in
 License: MIT
 Keywords: gluster,tool,geo-replication
 Platform: linux
```

### Comparing `gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/SOURCES.txt` & `gluster-georep-tools-0.5.1/gluster_georep_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/screenshots/gluster-georep-setup.png` & `gluster-georep-tools-0.5.1/screenshots/gluster-georep-setup.png`

 * *Files identical despite different names*

### Comparing `gluster-georep-tools-0.5.0/setup.py` & `gluster-georep-tools-0.5.1/setup.py`

 * *Files identical despite different names*

