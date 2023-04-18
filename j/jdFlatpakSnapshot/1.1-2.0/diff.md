# Comparing `tmp/jdFlatpakSnapshot-1.1.tar.gz` & `tmp/jdFlatpakSnapshot-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdFlatpakSnapshot-1.1.tar", last modified: Mon Apr 10 15:06:34 2023, max compression
+gzip compressed data, was "jdFlatpakSnapshot-2.0.tar", last modified: Tue Apr 18 16:24:17 2023, max compression
```

## Comparing `jdFlatpakSnapshot-1.1.tar` & `jdFlatpakSnapshot-2.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/
--rw-r--r--   0 root         (0) root         (0)     2879 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35075 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/AboutDialog.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Constants.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Environment.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/FlatpakHandler.py
--rw-r--r--   0 root         (0) root         (0)     2756 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Functions.py
--rw-r--r--   0 root         (0) root         (0)     5611 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ImportExport.py
--rw-r--r--   0 root         (0) root         (0)    13658 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ProgressDialog.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Settings.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/SettingsDialog.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Types.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/WelcomeDialog.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__init__.py
--rw-r--r--   0 root         (0) root         (0)        2 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/
--rw-r--r--   0 root         (0) root         (0)     3101 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/app-icon.svg
--rw-r--r--   0 root         (0) root         (0)     1181 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/default-icon.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/
--rw-r--r--   0 root         (0) root         (0)    19882 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
--rw-r--r--   0 root         (0) root         (0)    19670 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
--rw-r--r--   0 root         (0) root         (0)    19804 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/
--rw-r--r--   0 root         (0) root         (0)     2287 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/AboutDialog.ui
--rw-r--r--   0 root         (0) root         (0)     5626 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/ProgressDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3221 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/SettingsDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3642 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:06:34.807073 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1222 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-10 15:06:34.000000 jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-10 15:05:48.000000 jdFlatpakSnapshot-1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 15:06:34.811073 jdFlatpakSnapshot-1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35075 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4277 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Constants.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/FlatpakHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     5509 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ImportExport.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Languages.py
+-rw-r--r--   0 root         (0) root         (0)    17027 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ProgressDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/SnapshotCollection.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Types.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/WelcomeDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/app-icon.svg
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/default-icon.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/
+-rw-r--r--   0 root         (0) root         (0)    27319 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts
+-rw-r--r--   0 root         (0) root         (0)    27635 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts
+-rw-r--r--   0 root         (0) root         (0)    25664 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/ProgressDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:24:17.196058 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 16:24:17.000000 jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-18 16:18:16.000000 jdFlatpakSnapshot-2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 16:24:17.200058 jdFlatpakSnapshot-2.0/setup.cfg
```

### Comparing `jdFlatpakSnapshot-1.1/BuildBackend.py` & `jdFlatpakSnapshot-2.0/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/LICENSE` & `jdFlatpakSnapshot-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Environment.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from .SnapshotCollection import	SnapshotCollection
 from .FlatpakHandler import FlatpakHandler
-from .Types import SnapshotDictEntry
 from .Settings import Settings
 from PyQt6.QtGui import QIcon
 from pathlib import Path
 import json
 import sys
 import os
 
@@ -19,30 +19,20 @@
         self.icon = QIcon(os.path.join(self.program_dir, "icons", "app-icon.svg"))
 
         try:
             os.makedirs(self.data_dir)
         except FileExistsError:
             pass
 
-        self.snapshot_dict: dict[str, list[SnapshotDictEntry]] = {}
-        try:
-            with open(os.path.join(self.data_dir, "snapshots.json"), "r", encoding="utf-8") as f:
-                self.snapshot_dict = json.load(f)
-        except FileNotFoundError:
-            pass
-        except Exception:
-            print("Error opening " + os.path.join(self.data_dir, "snapshots.json"), file=sys.stderr)
+        self.snapshot_collection = SnapshotCollection(self)
+        self.snapshot_collection.load_snapshots()
 
         self.settings = Settings()
         self.settings.load(os.path.join(self.data_dir, "settings.json"))
 
         self.flatpak_handler = FlatpakHandler(self)
 
-    def save_snapshot_dict(self) -> None:
-        with open(os.path.join(self.data_dir, "snapshots.json"), "w", encoding="utf-8") as f:
-            json.dump(self.snapshot_dict, f, ensure_ascii=False, indent=4)
-
     def _get_data_path(self) -> str:
         if os.getenv("XDG_DATA_HOME"):
             return os.path.join(os.getenv("XDG_DATA_HOME"), "JakobDev", "jdFlatpakSnapshot")
         else:
             return os.path.join(str(Path.home()), ".local", "share", "JakobDev", "jdFlatpakSnapshot")
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/FlatpakHandler.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/FlatpakHandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,14 @@
             return None
 
 
     def is_running(self, app_id: str) -> bool:
         """
         Checks if the given App is running
         """
-        print("HHH")
         try:
             for app in subprocess.run(self._get_flatpak_command() + ["ps", "--columns=application"], capture_output=True, check=True).stdout.decode("utf-8").splitlines():
-                print(app)
                 if app == app_id:
                     return True
             return False
         except Exception:
             return False
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Functions.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,14 @@
         if os.path.isfile(full_path):
             file_list.append(os.path.join(start_path, i))
         elif os.path.isdir(full_path):
             file_list += list_files_recursive(full_path, os.path.join(start_path, i))
     return file_list
 
 
-def generate_snapshot_filename(directory: str) -> str:
-    while True:
-        filename = str(uuid.uuid4()) + ".tar"
-        path = os.path.join(directory, filename)
-
-        if os.path.exists(path):
-            continue
-
-        return path
-
-
 def human_readable_size(size: int) -> str:
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(size) < 1024.0:
             return f"{size:3.1f}{unit}B"
         size /= 1024.0
     return f"{size:.1f}YiB"
 
@@ -74,30 +63,20 @@
         pass
 
     with handler.open(zip_path, "r") as f:
         with open(extract_path, "wb") as w:
             w.write(f.read())
 
 
-def snapshot_name_exists(env: "Environment", app_id: str, name: str) -> bool:
-    """
-    Checks if a Snapshot with the given Name exists for this Flatpak
-    """
-    for i in env.snapshot_dict.get(app_id, []):
-        if i["name"] == name:
-            return True
-    return False
-
-
 def is_flatpak_installed(app_id: str) -> bool:
     """
     Checks if the given Flatpak is installed
     """
     for i in FLATPAK_DIRS:
-        if os.path.isdir(os.path.join(i, "apps", app_id)):
+        if os.path.isdir(os.path.join(i, "app", app_id)):
             return True
     return False
 
 
 def is_run_as_flatpak() -> bool:
     """
     Checks if the App is run as Flatpak
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ImportExport.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ImportExport.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,67 @@
-from .Functions import human_readable_size, format_datetime, generate_snapshot_filename, snapshot_name_exists, extract_file_from_zip, is_flatpak_installed
-from .Types import ExportedFileManifest, SnapshotDictEntry
+from .Functions import human_readable_size, format_datetime, extract_file_from_zip, is_flatpak_installed
 from PyQt6.QtWidgets import QWidget, QMessageBox, QInputDialog
-from .Constants import COMPRESSION_METHODS
 from PyQt6.QtCore import QCoreApplication
+from .Types import ExportedFileManifest
 from typing import TYPE_CHECKING
+from .Snapshot import Snapshot
 import traceback
 import datetime
 import zipfile
 import json
 import sys
 import os
 
 
 if TYPE_CHECKING:
     from .Environment import Environment
 
 
 def _import_single_snapshot(env: "Environment", app_id: str, parent: QWidget, zf: zipfile.ZipFile):
+    new_snapshot = env.snapshot_collection.generate_new_snapshot()
+    new_snapshot.app_id = app_id
+
     with zf.open("metadata.json", "r") as f:
-        snapshot_info: SnapshotDictEntry = json.loads(f.read())
+        new_snapshot.load_dict(json.load(f))
 
-    for method in reversed(COMPRESSION_METHODS):
-        if "data.tar" + method.suffix in zf.namelist():
-            file_name = "data.tar" + method.suffix
-            compression = method.name
+    new_snapshot.regenerate_filename()
+    file_name = "data.tar" + new_snapshot.get_compression_method().suffix
 
     text = QCoreApplication.translate("ImportExport", "This includes the following Snapshot:") + "<br>"
-    text += QCoreApplication.translate("ImportExport", "App: {{app}}").replace("{{app}}", app_id) + "<br>"
-    text += QCoreApplication.translate("ImportExport", "Name: {{name}}").replace("{{name}}", snapshot_info["name"]) + "<br>"
-    text += QCoreApplication.translate("ImportExport", "Compression: {{compression}}").replace("{{compression}}", compression) + "<br>"
+    text += QCoreApplication.translate("ImportExport", "App: {{app}}").replace("{{app}}", new_snapshot.app_id) + "<br>"
+    text += QCoreApplication.translate("ImportExport", "Name: {{name}}").replace("{{name}}", new_snapshot.name) + "<br>"
+    text += QCoreApplication.translate("ImportExport", "Compression: {{compression}}").replace("{{compression}}", new_snapshot.get_compression_method().name) + "<br>"
     text += QCoreApplication.translate("ImportExport", "Size on disk: {{size}}").replace("{{size}}", human_readable_size(zf.getinfo(file_name).file_size)) + "<br>"
-    text += QCoreApplication.translate("ImportExport", "Created on: {{datetime}}").replace("{{datetime}}", format_datetime(datetime.datetime.fromtimestamp(snapshot_info["timestamp"]), env.settings.get("datetimeFormat"))) + "<br><br>"
+    text += QCoreApplication.translate("ImportExport", "Created on: {{datetime}}").replace("{{datetime}}", format_datetime(datetime.datetime.fromtimestamp(new_snapshot.timestamp), env.settings.get("datetimeFormat"))) + "<br><br>"
     text += QCoreApplication.translate("ImportExport", "Do you want to import it?")
 
     if QMessageBox.question(parent, QCoreApplication.translate("ImportExport", "Import"), text, QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No) != QMessageBox.StandardButton.Yes:
         return
 
-    if not is_flatpak_installed(app_id):
-        if QMessageBox.question(parent, QCoreApplication.translate("ImportExport", "App not installed"), QCoreApplication.translate("ImportExport", "It looks like {{app}} is not installed. Are you really want to import the data?").replace("{{app}}", app_id), QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No) != QMessageBox.StandardButton.Yes:
+    if not is_flatpak_installed(new_snapshot.app_id):
+        if QMessageBox.question(parent, QCoreApplication.translate("ImportExport", "App not installed"), QCoreApplication.translate("ImportExport", "It looks like {{app}} is not installed. Are you really want to import the data?").replace("{{app}}", new_snapshot.app_id), QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No) != QMessageBox.StandardButton.Yes:
             return
 
-    if snapshot_name_exists(env, app_id, snapshot_info["name"]):
+    if env.snapshot_collection.do_snapshot_name_exists(new_snapshot.app_id, new_snapshot.name):
         while True:
             new_name = QInputDialog.getText(parent, QCoreApplication.translate("ImportExport", "New name"), QCoreApplication.translate("ImportExport", "There is already a Snapshot with this Name for this App. Please enter a new one."))[0].strip()
 
             if new_name == "":
                 return
 
-            if snapshot_name_exists(env, app_id, new_name):
+            if env.snapshot_collection.do_snapshot_name_exists(new_snapshot.app_id, new_name):
                 QMessageBox.information(parent,  QCoreApplication.translate("ImportExport", "Name exists"),  QCoreApplication.translate("ImportExport", "This Name also exists. Please enter a new one."))
             else:
-                snapshot_info["name"] = new_name
+                new_snapshot.name = new_name
                 break
 
-    snapshot_path = generate_snapshot_filename(os.path.join(env.data_dir, "snapshots", app_id))
-
-    extract_file_from_zip(zf, file_name, snapshot_path)
+    extract_file_from_zip(zf, file_name, new_snapshot.get_full_tar_path())
 
-    if app_id not in env.snapshot_dict:
-        env.snapshot_dict[app_id] = []
-
-    snapshot_info["filename"] = os.path.basename(snapshot_path)
-    env.snapshot_dict[app_id].append(snapshot_info)
-    env.save_snapshot_dict()
+    env.snapshot_collection.add_snapshot(new_snapshot)
+    env.snapshot_collection.save_snapshots()
 
 
 def import_file(env: "Environment", path: str, parent: QWidget) -> None:
     try:
         zf = zipfile.ZipFile(path, "r")
 
         with zf.open("manifest.json", "r") as f:
@@ -83,21 +78,26 @@
     finally:
         try:
             zf.close()
         except Exception:
             pass
 
 
-def export_single_snapshot(env: "Environment", path: str, app_id: str, snapshot_info: SnapshotDictEntry,  parent: QWidget) -> None:
+def export_single_snapshot(env: "Environment", current_snapshot: Snapshot, path: str, parent: QWidget) -> None:
     try:
         with zipfile.ZipFile(path, "w") as zf:
-            zf.write(os.path.join(env.data_dir, "snapshots", app_id, snapshot_info["filename"]), "data." + snapshot_info["filename"].split(".", 1)[1])
-            zf.writestr("metadata.json", json.dumps(snapshot_info, ensure_ascii=False, indent=4))
+            zf.write(current_snapshot.get_full_tar_path(), "data." + current_snapshot.filename.split(".", 1)[1])
+            zf.writestr("metadata.json", json.dumps(current_snapshot.to_dict(), ensure_ascii=False, indent=4))
             zf.writestr("manifest.json", json.dumps({
                 "version": 1,
                 "app_version": env.version,
                 "type": "single_snapshot",
-                "app_id": app_id
+                "app_id": current_snapshot.app_id
             }, ensure_ascii=False, indent=4))
     except Exception:
+        try:
+            os.remove(path)
+        except Exception:
+            pass
+
         print(traceback.format_exc(),end="",file=sys.stderr)
-        QMessageBox.critical(parent, QCoreApplication.translate("ImportExport", "Export failed"), QCoreApplication.translate("ImportExport", "Cound not export {{name}}"). replace("{{name}}", snapshot_info["name"]))
+        QMessageBox.critical(parent, QCoreApplication.translate("ImportExport", "Export failed"), QCoreApplication.translate("ImportExport", "Cound not export {{name}}"). replace("{{name}}", current_snapshot.name))
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/MainWindow.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/MainWindow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt6.QtWidgets import QMainWindow, QListWidgetItem, QMessageBox, QInputDialog, QFileDialog, QApplication
-from.Functions import generate_snapshot_filename, human_readable_size, format_datetime
 from .ImportExport import import_file, export_single_snapshot
+from.Functions import human_readable_size, format_datetime
 from .Constants import FLATPAK_DIRS, COMPRESSION_METHODS
 from .ui_compiled.MainWindow import Ui_MainWindow
 from PyQt6.QtCore import Qt, QCoreApplication
 from .SettingsDialog import SettingsDialog
 from typing import Optional, TYPE_CHECKING
 from .ProgressDialog import ProgressDialog
 from .WelcomeDialog import WelcomeDialog
@@ -16,77 +16,89 @@
 import shutil
 import sys
 import os
 
 
 if TYPE_CHECKING:
     from .Environment import Environment
+    from .Snapshot import Snapshot
 
 
-def _get_name_from_desktop_entry(desktop_file: str, app_id: str) -> Optional[str]:
+def _get_name_from_desktop_entry(desktop_file: str, app_id: str, language: str) -> Optional[str]:
     try:
         entry = desktop_entry_lib.DesktopEntry.from_file(desktop_file)
     except Exception:
         return None
 
     if not entry.should_show():
         return None
 
     if entry.Name.default_text != "":
-        return entry.Name.default_text
+        if language == "default":
+            return entry.Name.get_translated_text()
+        else:
+            return entry.Name.translations.get(language, entry.Name.default_text)
     else:
         return app_id
 
 
 class MainWindow(QMainWindow, Ui_MainWindow):
     def __init__(self, env: "Environment"):
         super().__init__()
         self._env = env
 
         self.setupUi(self)
 
         self._default_icon = QIcon(os.path.join(env.program_dir, "icons", "default-icon.svg"))
-        self._settings_dialog = SettingsDialog(env)
-        self._progress_dialog = ProgressDialog()
+        self._settings_dialog = SettingsDialog(env, self)
+        self._progress_dialog = ProgressDialog(env, self)
         self.welcome_dialog = WelcomeDialog(env)
         self._about_dialog = AboutDialog(env)
 
         self._fill_app_list()
+        self._update_snapshot_buttons_enabled()
 
-        self.list_apps.currentItemChanged.connect(self._update_snapshot_list)
-        self.snapshot_list.currentItemChanged.connect(self._enable_snapshot_buttons)
+        self.list_apps.currentItemChanged.connect(self._list_apps_item_changed)
+        self.snapshot_list.currentItemChanged.connect(self._update_snapshot_buttons_enabled)
 
         self.create_snapshot_button.clicked.connect(self._create_snapshot_button_clicked)
         self.restore_snapshot_button.clicked.connect(self._restore_snapshot_button_clicked)
         self.rename_snapshot_button.clicked.connect(self._rename_snapshot_button_clicked)
         self.delete_snapshot_button.clicked.connect(self._delete_snapshot_button_clicked)
         self.export_snapshot_button.clicked.connect(self._export_snapshot_button_clicked)
         self.about_snapshot_button.clicked.connect(self._about_snapshot_button_clicked)
 
         self.import_action.triggered.connect(self._import_action_clicked)
         self.exit_action.triggered.connect(lambda: sys.exit(0))
 
         self.settings_action.triggered.connect(self._settings_dialog.open_dialog)
 
+        self.uninstalled_apps_snapshot_delete_action.triggered.connect(self._uninstalled_apps_snapshot_delete_action_clicked)
+        self.delete_broken_snapshots_action.triggered.connect(self._delete_broken_snapshots_action_clicked)
+
         self.welcome_dialog_action.triggered.connect(self.welcome_dialog.open_dialog)
         self.view_source_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdFlatpakSnapshot"))
         self.report_bug_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdFlatpakSnapshot/issues"))
         self.translate_action.triggered.connect(lambda: webbrowser.open("https://translate.codeberg.org/projects/jdFlatpakSnapshot"))
         self.donate_action.triggered.connect(lambda: webbrowser.open("https://ko-fi.com/jakobdev"))
         self.about_action.triggered.connect(self._about_dialog.exec)
         self.about_qt_action.triggered.connect(QApplication.instance().aboutQt)
 
+        if self.list_apps.count() == 0:
+            QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "No Flatpaks found"), QCoreApplication.translate("MainWindow", "No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu."))
+
     def _fill_app_list(self) -> None:
         self.list_apps.clear()
 
         known_ids = []
         for i in FLATPAK_DIRS:
             self._load_apps(i, known_ids)
 
         self.list_apps.sortItems(Qt.SortOrder.AscendingOrder)
+        self.update_app_list_visible()
 
     def _load_apps(self, flatpak_path: str, known_ids: list[str]) -> None:
         if not os.path.isdir(flatpak_path):
             return
 
         if not os.path.isdir(os.path.join(flatpak_path, "app")):
             return
@@ -95,15 +107,15 @@
             app_id = i.removesuffix(".desktop")
 
             if app_id in known_ids:
                 continue
 
             known_ids.append(app_id)
 
-            name = _get_name_from_desktop_entry(os.path.join(flatpak_path,  "exports", "share" , "applications", i + ".desktop"), app_id)
+            name = _get_name_from_desktop_entry(os.path.join(flatpak_path,  "exports", "share" , "applications", i + ".desktop"), app_id, self._env.settings.get("language"))
 
             icon = None
             if os.path.isfile(os.path.join(flatpak_path, "exports", "share" , "icons", "hicolor", "scalable", "apps", app_id + ".svg")):
                 icon = QIcon(os.path.join(flatpak_path, "exports", "share" , "icons", "hicolor", "scalable","apps",  app_id + ".svg"))
             else:
                 for size in ("512x512", "256x256", "128x128", "96x96", "64x64", "48x48", "32x32", "24x24", "22x22", "16x16"):
                     if os.path.isfile(os.path.join(flatpak_path, "exports", "share" , "icons", "hicolor", size, "apps",  app_id + ".png")):
@@ -112,170 +124,210 @@
             if icon is None:
                 item = QListWidgetItem(self._default_icon, name or app_id)
             else:
                  item = QListWidgetItem(icon, name or app_id)
             item.setData(42, i)
             self.list_apps.addItem(item)
 
-    def _update_snapshot_list(self) -> None:
+    def _get_selected_snapshot(self) -> Optional["Snapshot"]:
+        return self._env.snapshot_collection.get_snapshot_by_id(self.snapshot_list.currentItem().data(42))
+
+    def update_app_list_visible(self) -> None:
+        for i in range(self.list_apps.count()):
+            item = self.list_apps.item(i)
+            app_id = item.data(42)
+
+            if item.text() == app_id and not self._env.settings.get("showSystemApps"):
+                item.setHidden(True)
+                continue
+
+            if not os.path.isdir(os.path.join(os.path.expanduser("~/.var/app"), app_id)) and not self._env.settings.get("showAppsWithNoData"):
+                item.setHidden(True)
+                continue
+
+            item.setHidden(False)
+
+        self.list_apps.setCurrentRow(-1)
+        self._list_apps_item_changed()
+
+    def _list_apps_item_changed(self) -> None:
+        self.create_snapshot_button.setEnabled(self.list_apps.currentRow() != -1)
+        self.update_snapshot_list()
+
+    def update_snapshot_list(self) -> None:
         self.snapshot_list.clear()
 
         self.restore_snapshot_button.setEnabled(False)
         self.rename_snapshot_button.setEnabled(False)
         self.delete_snapshot_button.setEnabled(False)
         self.export_snapshot_button.setEnabled(False)
         self.about_snapshot_button.setEnabled(False)
 
-        if self.list_apps.currentItem().data(42) not in self._env.snapshot_dict:
+        if self.list_apps.currentItem() is None:
+            return
+
+        if self.list_apps.currentItem().data(42) not in self._env.snapshot_collection.snapshots:
             return
 
-        for i in self._env.snapshot_dict[self.list_apps.currentItem().data(42)]:
-            self.snapshot_list.addItem(i["name"])
+        for i in self._env.snapshot_collection.snapshots[self.list_apps.currentItem().data(42)]:
+            if i.is_valid():
+                item = QListWidgetItem(i.name)
+                item.setData(42, i.id)
+                self.snapshot_list.addItem(item)
 
-    def _enable_snapshot_buttons(self) -> None:
-        self.restore_snapshot_button.setEnabled(True)
-        self.rename_snapshot_button.setEnabled(True)
-        self.delete_snapshot_button.setEnabled(True)
-        self.export_snapshot_button.setEnabled(True)
-        self.about_snapshot_button.setEnabled(True)
+    def _update_snapshot_buttons_enabled(self) -> None:
+        enabled = self.snapshot_list.currentRow() != -1
+        self.restore_snapshot_button.setEnabled(enabled)
+        self.rename_snapshot_button.setEnabled(enabled)
+        self.delete_snapshot_button.setEnabled(enabled)
+        self.export_snapshot_button.setEnabled(enabled)
+        self.about_snapshot_button.setEnabled(enabled)
 
     def _import_action_clicked(self) -> None:
         filter = QCoreApplication.translate("MainWindow", "Exported Snapshots") + " (*.flatpaksnapshot);;" +   QCoreApplication.translate("MainWindow", "All Files") + " (*)"
         path = QFileDialog.getOpenFileName(self, filter=filter)[0]
 
         if path == "":
             return
 
         import_file(self._env, path, self)
 
-        self._update_snapshot_list()
+        self.update_snapshot_list()
+
+    def _uninstalled_apps_snapshot_delete_action_clicked(self) -> None:
+        if QMessageBox.question(self, QCoreApplication.translate("MainWindow", "Delete Snapshot of uninstalled Apps"), QCoreApplication.translate("MainWindow", "This will delete all Snapshots of apps that are no longer installed. Do you want to continue?")) != QMessageBox.StandardButton.Yes:
+           return
+
+        self._env.snapshot_collection.delete_snapshots_of_uninstalled_apps()
+        self._env.snapshot_collection.save_snapshots()
+
+        self.update_snapshot_list()
+
+        QMessageBox.information(self, QCoreApplication.translate("MainWindow", "Snapshots deleted"), QCoreApplication.translate("MainWindow", "The Snapshots were successfully deleted"))
+
+    def _delete_broken_snapshots_action_clicked(self) -> None:
+        if QMessageBox.question(self, QCoreApplication.translate("MainWindow", "Delete broken Snapshots"), QCoreApplication.translate("MainWindow", "This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?")) != QMessageBox.StandardButton.Yes:
+           return
+
+        self._env.snapshot_collection.delete_broken_snapshots()
+        self._env.snapshot_collection.save_snapshots()
+
+        self.update_snapshot_list()
+
+        QMessageBox.information(self, QCoreApplication.translate("MainWindow", "Snapshots deleted"), QCoreApplication.translate("MainWindow", "The Snapshots were successfully deleted"))
 
     def _create_snapshot_button_clicked(self) -> None:
         app_id = self.list_apps.currentItem().data(42)
 
         if not os.path.isdir(os.path.join(os.path.expanduser("~/.var/app"), app_id)):
             QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "No data"), QCoreApplication.translate("MainWindow", "This Flatpak has no Data"))
             return
 
+        if self._env.flatpak_handler.is_running(app_id) and not self._env.settings.get("allowCreatingWhileRunning"):
+            QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Flatpak running"), QCoreApplication.translate("MainWindow", "This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running."))
+            return
+
         commit = self._env.flatpak_handler.get_installed_commit(app_id)
         if not commit:
             QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Could not get Commit"), QCoreApplication.translate("MainWindow", "Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs."))
 
         name, ok = QInputDialog.getText(self, QCoreApplication.translate("MainWindow", "Enter Name"), QCoreApplication.translate("MainWindow", "Please enter a Name for your Snapshot"))
 
         if not ok or name == "":
             return
 
-        for i in self._env.snapshot_dict.get(app_id, []):
-            if i["name"] == name:
-                QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Name exists"), QCoreApplication.translate("MainWindow", "This Name already exists"))
-                return
+        if self._env.snapshot_collection.do_snapshot_name_exists(app_id, name):
+            QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Name exists"), QCoreApplication.translate("MainWindow", "This Name already exists"))
+            return
 
-        snapshot_path = generate_snapshot_filename(os.path.join(self._env.data_dir, "snapshots", app_id))
+        new_snapshot = self._env.snapshot_collection.generate_new_snapshot()
+        snapshot_path = os.path.join(self._env.data_dir, "snapshots", app_id, new_snapshot.id + ".tar")
+        new_snapshot.app_id = app_id
 
-        comp_method, ok, = QInputDialog.getItem(self, QCoreApplication.translate("MainWindow", "Compression method"), QCoreApplication.translate("MainWindow", "Please choose a compression method"), [i[0] for i in COMPRESSION_METHODS], editable=False)
+        comp_method, ok, = QInputDialog.getItem(self, QCoreApplication.translate("MainWindow", "Compression method"), QCoreApplication.translate("MainWindow", "Please choose a compression method"), [i.name for i in COMPRESSION_METHODS], editable=False)
 
         if not ok:
             return
 
         for comp in COMPRESSION_METHODS:
-            if comp[0] == comp_method:
+            if comp.name == comp_method:
                 compression_method_data = comp
                 break
 
         save_path = snapshot_path + compression_method_data.suffix
 
-        self._progress_dialog.create_tar_archive(save_path, os.path.join(os.path.expanduser("~/.var/app"), app_id), compression_method_data.mode)
-
-        if app_id not in self._env.snapshot_dict:
-            self._env.snapshot_dict[app_id] = []
+        new_snapshot.name = name
+        new_snapshot.filename = os.path.basename(save_path)
+        new_snapshot.timestamp = int(datetime.datetime.now().timestamp())
+        new_snapshot.commit = commit
 
-        self._env.snapshot_dict[app_id].append({
-            "name": name,
-            "filename": os.path.basename(save_path),
-            "timestamp": int(datetime.datetime.now().timestamp()),
-            "commit": commit
-        })
-
-        self._env.save_snapshot_dict()
-        self._update_snapshot_list()
+        self._progress_dialog.create_tar_archive(new_snapshot)
 
     def _restore_snapshot_button_clicked(self) -> None:
-        app_id = self.list_apps.currentItem().data(42)
+        current_snapshot = self._get_selected_snapshot()
 
-        if self._env.flatpak_handler.is_running(app_id):
+        if self._env.flatpak_handler.is_running(current_snapshot.app_id) and not self._env.settings.get("allowRestoringWhileRunning"):
             QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Flatpak running"), QCoreApplication.translate("MainWindow", "This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running."))
             return
 
         if QMessageBox.question(self, QCoreApplication.translate("MainWindow", "Restore Snapshot"), QCoreApplication.translate("MainWindow", "Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.")) != QMessageBox.StandardButton.Yes:
             return
 
-        data_dir = os.path.join(os.path.expanduser("~/.var/app"), app_id)
+        data_dir = os.path.join(os.path.expanduser("~/.var/app"), current_snapshot.app_id)
 
         try:
             shutil.rmtree(data_dir)
         except FileNotFoundError:
             pass
         except Exception:
             QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Error"), QCoreApplication.translate("MainWindow", "An error occurred while deleting {{path}}").replace("{{path}}", data_dir))
             return
 
-        self._progress_dialog.extract_tar_archive(os.path.join(self._env.data_dir, "snapshots", app_id, self._env.snapshot_dict[app_id][self.snapshot_list.currentRow()]["filename"]), data_dir)
+        self._progress_dialog.extract_tar_archive(current_snapshot)
 
     def _rename_snapshot_button_clicked(self) -> None:
         name, ok = QInputDialog.getText(self, QCoreApplication.translate("MainWindow", "New name"), QCoreApplication.translate("MainWindow", "Please enter a new name"))
 
         if not ok or name == "":
             return
 
-        for i in self._env.snapshot_dict[self.list_apps.currentItem().data(42)]:
-            if i["name"] == name:
-                QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Name exists"), QCoreApplication.translate("MainWindow", "This name already exists"))
-                return
+        current_snapshot = self._get_selected_snapshot()
 
-        self._env.snapshot_dict[self.list_apps.currentItem().data(42)][self.snapshot_list.currentRow()]["name"] = name
+        if self._env.snapshot_collection.do_snapshot_name_exists(current_snapshot.app_id,name):
+            QMessageBox.critical(self, QCoreApplication.translate("MainWindow", "Name exists"), QCoreApplication.translate("MainWindow", "This name already exists"))
+            return
+
+        current_snapshot.name = name
 
-        self._update_snapshot_list()
+        self.update_snapshot_list()
 
     def _delete_snapshot_button_clicked(self) -> None:
         if QMessageBox.question(self, QCoreApplication.translate("MainWindow", "Delete snapshot"), QCoreApplication.translate("MainWindow", "Are you sure you want to delete this snapshot?")) != QMessageBox.StandardButton.Yes:
            return
 
-        app_id = self.list_apps.currentItem().data(42)
+        current_snapshot = self._get_selected_snapshot()
 
-        os.remove(os.path.join(self._env.data_dir, "snapshots", app_id, self._env.snapshot_dict[app_id][self.snapshot_list.currentRow()]["filename"]))
-        del self._env.snapshot_dict[app_id][self.snapshot_list.currentRow()]
+        self._env.snapshot_collection.delete_snapshot(current_snapshot)
 
-        self._env.save_snapshot_dict()
-        self._update_snapshot_list()
+        self._env.snapshot_collection.save_snapshots()
+        self.update_snapshot_list()
 
         QMessageBox.information(self, QCoreApplication.translate("MainWindow", "Snapshot deleted"), QCoreApplication.translate("MainWindow", "The snapshot was successfully deleted"))
 
     def _export_snapshot_button_clicked(self) -> None:
         filter = QCoreApplication.translate("MainWindow", "Exported Snapshots") + " (*.flatpaksnapshot);;" +   QCoreApplication.translate("MainWindow", "All Files") + " (*)"
         path = QFileDialog.getSaveFileName(self, filter=filter)[0]
 
         if path == "":
             return
 
-        app_id = self.list_apps.currentItem().data(42)
-        data = self._env.snapshot_dict[app_id][self.snapshot_list.currentRow()]
-
-        export_single_snapshot(self._env, path, app_id, data, self)
+        export_single_snapshot(self._env, self._get_selected_snapshot(), path, self)
 
     def _about_snapshot_button_clicked(self) -> None:
-        app_id = self.list_apps.currentItem().data(42)
-        data = self._env.snapshot_dict[app_id][self.snapshot_list.currentRow()]
-
-        for method in reversed(COMPRESSION_METHODS):
-            if data["filename"].endswith(method.suffix):
-                compression = method.name
-                break
-
-        text =  QCoreApplication.translate("MainWindow", "Compression: {{compression}}").replace("{{compression}}", compression) + "<br>"
-        text += QCoreApplication.translate("MainWindow", "Size on disk: {{size}}").replace("{{size}}", human_readable_size(os.path.getsize(os.path.join(self._env.data_dir, "snapshots", app_id, data["filename"])))) + "<br>"
-        text += QCoreApplication.translate("MainWindow", "Created on: {{datetime}}").replace("{{datetime}}", format_datetime(datetime.datetime.fromtimestamp(data["timestamp"]), self._env.settings.get("datetimeFormat"))) + "<br>"
-        text += QCoreApplication.translate("MainWindow", "Commit: {{commit}}").replace("{{commit}}", data.get("commit") or QCoreApplication.translate("MainWindow", "Unknown"))
-
+        snapshot = self._get_selected_snapshot()
 
+        text =  QCoreApplication.translate("MainWindow", "Compression: {{compression}}").replace("{{compression}}", snapshot.get_compression_method().name) + "<br>"
+        text += QCoreApplication.translate("MainWindow", "Size on disk: {{size}}").replace("{{size}}", human_readable_size(os.path.getsize(os.path.join(self._env.data_dir, "snapshots", snapshot.app_id, snapshot.filename)))) + "<br>"
+        text += QCoreApplication.translate("MainWindow", "Created on: {{datetime}}").replace("{{datetime}}", format_datetime(datetime.datetime.fromtimestamp(snapshot.timestamp), self._env.settings.get("datetimeFormat"))) + "<br>"
+        text += QCoreApplication.translate("MainWindow", "Commit: {{commit}}").replace("{{commit}}", snapshot.commit or QCoreApplication.translate("MainWindow", "Unknown"))
 
         QMessageBox.information(self, QCoreApplication.translate("MainWindow", "About {{name}}").replace("{{name}}", self.snapshot_list.currentItem().text()), text)
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/Settings.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/Settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 
 class Settings():
     def __init__(self):
         self._default_settings = {
             "language": "default",
             "datetimeFormat": DEFAULT_DATETIME_FORMAT,
+            "showSystemApps": True,
+            "showAppsWithNoData": True,
+            "allowCreatingWhileRunning": False,
+            "allowRestoringWhileRunning": False,
             "flatpakCommand": "flatpak",
             "showWelcomeDialog": True
         }
 
         self._user_settings = {}
 
     def get(self, key: str) -> Any:
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/WelcomeDialog.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/__init__.py` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/app-icon.svg` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/app-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/icons/default-icon.svg` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/icons/default-icon.svg`

 * *Files identical despite different names*

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts`

 * *Files 13% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts`

```diff
@@ -1,498 +1,650 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="de">
+<TS version="2.1" language="nl">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>A Program to create Snapshots of Flatpak Apps</source>
-      <translation>Ein Programm zum erstellen von Snapshowts von Flatpak Apps</translation>
+      <translation>Een programma om momentopnamen van flatpakapps te maken</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
+      <translation>Dit programma is uitgebracht onder de GPL3-licentie</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Translators</source>
+      <translation>Vertalers</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>The following people translated jdFlatpakSnapshot:</source>
+      <translation>Deze mensen hebben jdFlatpakSnapshot vertaald:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Changelog</source>
+      <translation>Wijzigingslog</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Schließen</translation>
+      <translation>Sluiten</translation>
     </message>
   </context>
   <context>
     <name>Constants</name>
     <message>
-      <location filename="../Constants.py" line="13"/>
+      <location filename="../Constants.py" line="12"/>
       <source>None</source>
-      <translation>Keine</translation>
+      <translation>Geen</translation>
     </message>
   </context>
   <context>
     <name>ImportExport</name>
     <message>
-      <location filename="../ImportExport.py" line="28"/>
+      <location filename="../ImportExport.py" line="29"/>
       <source>This includes the following Snapshot:</source>
-      <translation>Dies enthält den folgenden Snapshot:</translation>
+      <translation>Dit bevat de volgende momentopname:</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="29"/>
+      <location filename="../ImportExport.py" line="30"/>
       <source>App: {{app}}</source>
       <translation>App: {{app}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="30"/>
+      <location filename="../ImportExport.py" line="31"/>
       <source>Name: {{name}}</source>
-      <translation>Name: {{name}}</translation>
+      <translation>Naam: {{name}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="31"/>
+      <location filename="../ImportExport.py" line="32"/>
       <source>Compression: {{compression}}</source>
-      <translation>Komprimierungsverfahren: {{compression}}</translation>
+      <translation>Compressie: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="32"/>
+      <location filename="../ImportExport.py" line="33"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Größe auf dem Datenträger: {{size}}</translation>
+      <translation>Grootte op schijf: {{size}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="33"/>
+      <location filename="../ImportExport.py" line="34"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Erstellt am: {{datetime}}</translation>
+      <translation>Gemaakt op: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="34"/>
+      <location filename="../ImportExport.py" line="35"/>
       <source>Do you want to import it?</source>
-      <translation>Möchtest du ihn importieren?</translation>
+      <translation>Wilt u deze momentopname importeren?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="36"/>
+      <location filename="../ImportExport.py" line="37"/>
       <source>Import</source>
-      <translation>Importieren</translation>
+      <translation>Importeren</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>App not installed</source>
-      <translation>App nicht installiert</translation>
+      <translation>App niet geïnstalleerd</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>It looks like {{app}} is not installed. Are you really want to import the data?</source>
-      <translation>Es sieht so aus, als sei {{app}} nicht intstalliert. Mächtest du die Daten trotzdem importieren?</translation>
+      <translation>Het lijkt er op dan {{app}} niet geïnstalleerd is. Weet u zeker dat u de gegevens wilt importeren?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>New name</source>
-      <translation>Neuer Name</translation>
+      <translation>Nieuwe naam</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>There is already a Snapshot with this Name for this App. Please enter a new one.</source>
-      <translation>Es existiert bereits ein Snapshot mt diesem Namen für diese App. Bitte gib einen neuen ein.</translation>
+      <translation>Er is al een momentopname van deze app onder deze naam. Kies een andere naam.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Naam in gebruik</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>This Name also exists. Please enter a new one.</source>
-      <translation>Diser Name existiert auch. Bitte gib einen neuen ein.</translation>
+      <translation>Deze naam is ook in gebruik. Kies een andere naam.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>Error</source>
-      <translation>Fehler</translation>
+      <translation>Foutmelding</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>An error occurred during import. Maybe the File is not valid.</source>
-      <translation>Während des Importierens ist ein Fehler aufgetreten. Möglicherweise ist die Datei ungültig.</translation>
+      <translation>Er is een fout opgetreden tijdens het importeren. Mogelijk is het bestand beschadigd.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Export failed</source>
-      <translation>Export fehlgeschlagen</translation>
+      <translation>Exporteren mislukt</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Cound not export {{name}}</source>
-      <translation>Konnte {{name}} nicht exportieren</translation>
+      <translation>{{name}} kan niet worden geëxporteerd</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
-      <location filename="../SettingsDialog.py" line="17"/>
+      <location filename="../Languages.py" line="6"/>
       <source>English</source>
-      <translation>Englisch</translation>
+      <translation>Engels</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="18"/>
+      <location filename="../Languages.py" line="7"/>
       <source>German</source>
-      <translation>Deutsch</translation>
+      <translation>Duits</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="8"/>
+      <source>Dutch</source>
+      <translation>Nederlands</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="9"/>
+      <source>Turkish</source>
+      <translation>Turks</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No Flatpaks found</source>
+      <translation>Geen flatpaks aangetroffen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu.</source>
+      <translation>Er zijn geen flatpaks aangetroffen op uw systeem. Zorg dat er flatplaks geïnstalleerd zijn en dat jdFlatpakSnapshot over de juiste rechten beschikt. Als het probleem blijft optreden, maak hier dan melding van. U kunt de meldingspagina openen via het ?-menu.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>Exported Snapshots</source>
-      <translation>Exportierte Snapshots</translation>
+      <translation>Geëxporteerde momentopnamen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>All Files</source>
-      <translation>Alle Dateien</translation>
+      <translation>Alle bestanden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>Delete Snapshot of uninstalled Apps</source>
+      <translation>Momentopname van verwijderde apps wissen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>This will delete all Snapshots of apps that are no longer installed. Do you want to continue?</source>
+      <translation>Hierdoor worden alle momentopnamen van verwijderde apps gewist. Weet u zeker dat u wilt doorgaan?</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>Snapshots deleted</source>
+      <translation>Momentopnamen gewist</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>The Snapshots were successfully deleted</source>
+      <translation>De momentopnamen zijn gewist</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>Delete broken Snapshots</source>
+      <translation>Beschadigde momentopnamen wissen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?</source>
+      <translation>Hierdoor worden alle beschadigde momentopnamen gewist. Dit kan nodig zijn als er bijvoorbeeld een bug optreedt tijdens het maken van een momentopname of als de gegevens niet kloppen. Weet u zeker dat u wilt doorgaan?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>No data</source>
-      <translation>Keine Daten</translation>
+      <translation>Geen gegevens</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>This Flatpak has no Data</source>
-      <translation>Dieses Flatpak hat keine Daten</translation>
+      <translation>Deze flatpak bevat geen gegevens</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>Flatpak running</source>
+      <translation>Flatpak in gebruik</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
+      <translation>Deze flatpak is momenteel in gebruik. U kunt de momentopname van een flatpak niet herstellen zolang deze in gebruik is.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get Commit</source>
-      <translation>Kontte Commit nicht auslesen</translation>
+      <translation>Kan commit niet opvragen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs.</source>
-      <translation>Der Commit dieses Flatpaks konnte nicht ausgelesen werden. Du kannst trotzdem einen Snapshot erstellen, weisst aber nacher nicht mehr, zu welcher Version er gehört.</translation>
+      <translation>De commit van deze flatpak kan niet worden opgevraagd. U kunt wel een momentopname maken, maar er wordt geen versienummer toegekend.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Enter Name</source>
-      <translation>Namen eingeben</translation>
+      <translation>Naam invoeren</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Please enter a Name for your Snapshot</source>
-      <translation>Bitte gib einen Namen für diesen Snapshot ein</translation>
+      <translation>Geef de momentopname een naam</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="296"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>Name exists</source>
-      <translation>Name existiert</translation>
+      <translation>Naam in gebruik</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>This Name already exists</source>
-      <translation>Dieser Name existiert bereits</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Compression method</source>
-      <translation>Komprimierungsverfahren</translation>
+      <translation>Compressiemethode</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Please choose a compression method</source>
-      <translation>Bitte wähle ein Komprimierungsverfahren aus</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>Flatpak running</source>
-      <translation>Flatpak läuft</translation>
+      <translation>Kies een compressiemethode</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
-      <translation>Dieses Flatpak wird gerade ausgeführt. Du kannst keinen Snapshot wiederherstellen, während das Flatpak gerade ausgeführt wird.</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Restore Snapshot</source>
-      <translation>Snapshot wiederherstellen</translation>
+      <translation>Momentopname herstellen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.</source>
-      <translation>Bist du sicher, dass du diesen Snapshot wiederherstellen möchtest? Vorhandene Daten werden dabei überschrieben.</translation>
+      <translation>Weet u zeker dat u deze momentopname wilt herstellen? Hierdoor worden alle flatpakgegevens overschreven.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>Error</source>
-      <translation>fehler</translation>
+      <translation>Foutmelding</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>An error occurred while deleting {{path}}</source>
-      <translation>Während des Löschens von {{path}} ist ein Fehler aufgetreten</translation>
+      <translation>Er is een fout opgetreden tijdens het verwijderen van {{path}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>New name</source>
-      <translation>Neuer Name</translation>
+      <translation>Nieuwe naam</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>Please enter a new name</source>
-      <translation>Bitte gib einen neuen Namen ein</translation>
+      <translation>Voer een nieuwe naam in</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
+      <location filename="../MainWindow.py" line="296"/>
       <source>This name already exists</source>
-      <translation>Dieser Name existiert bereits</translation>
+      <translation>Deze naam is al in gebruik</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Delete snapshot</source>
-      <translation>Snapshot löschen</translation>
+      <translation>Momentopname verwijderen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Are you sure you want to delete this snapshot?</source>
-      <translation>Bist du sicher, dass du diesen Snapshot löschen willst?</translation>
+      <translation>Weet u zeker dat u deze momentopname wilt verwijderen?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>Snapshot deleted</source>
-      <translation>Snapshot gelöscht</translation>
+      <translation>Momentopname verwijderd</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>The snapshot was successfully deleted</source>
-      <translation>Der Snapshot wurde erfolgreich gelöscht</translation>
+      <translation>De momentopname is verwijderd</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="274"/>
+      <location filename="../MainWindow.py" line="328"/>
       <source>Compression: {{compression}}</source>
-      <translation>Komprimierungsverfahren: {{compression}}</translation>
+      <translation>Compressie: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="275"/>
+      <location filename="../MainWindow.py" line="329"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Größe auf dem Datenträger: {{size}}</translation>
+      <translation>Grootte op schijf: {{size}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="276"/>
+      <location filename="../MainWindow.py" line="330"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Erstellt am: {{datetime}}</translation>
+      <translation>Gemaakt op: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Commit: {{commit}}</source>
       <translation>Commit: {{commit}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Unknown</source>
-      <translation>Unbekannt</translation>
+      <translation>Onbekend</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="281"/>
+      <location filename="../MainWindow.py" line="333"/>
       <source>About {{name}}</source>
-      <translation>Über {{name}}</translation>
+      <translation>Over {{name}}</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Flatpaks</source>
       <translation>Flatpaks</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Create Snapshot</source>
-      <translation>Snapshot erstellen</translation>
+      <translation>Momentopname maken</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Snapshots</source>
-      <translation>Snapshots</translation>
+      <translation>Momentopnamen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Restore</source>
-      <translation>Wiederherstellen</translation>
+      <translation>Herstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Umbennenen</translation>
+      <translation>Naam wijzigen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Löschen</translation>
+      <translation>Verwijderen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Export</source>
-      <translation>Exportieren</translation>
+      <translation>Exporteren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Über</translation>
+      <translation>Over</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Datei</translation>
+      <translation>Bestand</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Maintenance</source>
+      <translation>Onderhoud</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Über Qt</translation>
+      <translation>Over Qt</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Beenden</translation>
+      <translation>Afsluiten</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Import</source>
-      <translation>Import</translation>
+      <translation>Importeren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Willkommensdialog zeigen</translation>
+      <translation>Welkomstvenster tonen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Quelltext ansehen</translation>
+      <translation>Broncode bekijken</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Fehler melden</translation>
+      <translation>Bug melden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Übersetzen</translation>
+      <translation>Vertalen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Spenden</translation>
+      <translation>Doneren</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Delete Snapshots of uninstalled Apps</source>
+      <translation>Momentopnamen van verwijderde apps wissen</translation>
     </message>
   </context>
   <context>
     <name>ProgressDialog</name>
     <message>
+      <location filename="../ProgressDialog.py" line="32"/>
+      <source>Scanning files. Please wait...</source>
+      <translation>Bezig met doorzoeken van bestanden…</translation>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="42"/>
+      <source>Compressing {{path}}</source>
+      <translation>Bezig met comprimeren van {{path}}…</translation>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="58"/>
+      <source>Extracting {{path}}</source>
+      <translation>Bezig met extraheren van {{path}}…</translation>
+    </message>
+    <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Progress</source>
-      <translation>Fortschritt</translation>
+      <translation>Voortgang</translation>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</source>
+      <translation>Let op: de voortgangsbalk toont alléén hoeveel bestanden er verwerkt zijn, dus níet de voortgang van losse bestanden. Bij het verwerken van grotere bestanden kan het daardoor lijken of het programma bevroren is.</translation>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>Cancel</source>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../SettingsDialog.py" line="30"/>
+      <location filename="../SettingsDialog.py" line="27"/>
       <source>System language</source>
-      <translation>Systemsprache</translation>
+      <translation>Systeemtaal</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="53"/>
+      <location filename="../SettingsDialog.py" line="57"/>
       <source>(Preview: {{preview}})</source>
-      <translation>(Vorschau: {{preview}})</translation>
+      <translation>(Voorbeeld: {{preview}})</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="55"/>
+      <location filename="../SettingsDialog.py" line="59"/>
       <source>(Invalid)</source>
-      <translation>(Ungültig)</translation>
+      <translation>(Ongeldig)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Einstellungen</translation>
+      <translation>Instellingen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>General</source>
+      <translation>Algemeen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>(needs restart)</source>
+      <translation>(herstart vereist)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Datetime Format:</source>
-      <translation>Datumszeitformat:</translation>
+      <translation>Datum- en tijdopmaak:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Sprache:</translation>
+      <translation>Taal:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
-      <source>(needs restart)</source>
-      <translation>(benötigt Neustart)</translation>
+      <source>Show system Apps</source>
+      <translation>Systeemapps tonen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Show Apps with no Data</source>
+      <translation>Gegevensloze apps tonen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow creating Snapshots while the App is running</source>
+      <translation>Ook momentopnamen maken terwijl apps actief zijn</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow restoring Snapshots while the App is running</source>
+      <translation>Ook momentopnamen herstellen terwijl apps actief zijn</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Advanced</source>
+      <translation>Geavanceerd</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Flatpak Command</source>
+      <translation>Flatpakopdracht</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>You can specify the command to call Flatpak here. This is only needed if Flatpak is not present in the PATH due to an own installation.</source>
+      <comment>Don't translate PATH, as it's the name of a Environment Variable</comment>
+      <translation>Hier kunt u aangeven welke flatpakopdracht er dient te worden aangeroepen. Dit is alléén nodig als Flatpak niet op een door PATH opgenomen locatie geïnstalleerd is.</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command:</source>
-      <translation>Flatpakbefehl:</translation>
+      <translation>Flatpakopdracht:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Zurücksetzen</translation>
+      <translation>Standaardwaarden</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Ok</translation>
+      <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Abbrechen</translation>
+      <translation>Annuleren</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Willkommen</translation>
+      <translation>Welkom</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdFlatpakSnapshot!</source>
-      <translation>Willkommen bei jdFlatpakSnapshot!</translation>
+      <translation>Welkom in jdFlatpakSnapshot!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to create a Snapshot of the Data of a Flatpak.</source>
-      <translation>Dieses Programm erlaubt dir, Snapshots von den Daten eines Flatpaks zu erstellen.</translation>
+      <translation>Met dit programma kunt u een momentopname van de gegevens van een flatpak maken.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</source>
-      <translation>Du kannst das z.B. nutzen um mit den Einstellungen eines Programms herumzuspielen und falls etwas nicht funktioniert, einfach den alten Stand wiederherstellen.</translation>
+      <translation>Dit is bijvoorbeeld handig als u met de instellingen van een programma wilt spelen en ze nadien wilt herstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</source>
-      <translation>Dieses Programm speichert nur die Daten eines Flatpaks sowie die Version, aber nicht das Flatpak selber.</translation>
+      <translation>Let op: dit programma maakt alleen een momentopname van de gegevens en versie van een flatpak, maar niet van de flatpak zelf.</translation>
+    </message>
+    <message>
+      <location filename="../ui/WelcomeDialog.ui" line="0"/>
+      <source>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</source>
+      <translation>Als u een bug tegenkomt, meld deze dan. U kunt de bugpagina openen via ? → Bug melden. U kunt op die manier tevens ideeën delen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</source>
-      <translation>Um loszulegen, wähle ein Flatpak aus und klicke auf &quot;Snapshot erstellen&quot;.</translation>
+      <translation>Kies een flatpak en klik op ‘Momentopname maken’ om aan de slag te gaan.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Diesen Dialog beim Programmstart anzeigen</translation>
+      <translation>Venster altijd tonen na opstarten</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts`

 * *Files 10% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_nl.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts`

```diff
@@ -1,498 +1,650 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="nl">
+<TS version="2.1" language="tr">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Hakkında</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>A Program to create Snapshots of Flatpak Apps</source>
-      <translation>Een programma om momentopnamen van flatpakapps te maken</translation>
+      <translation>Flatpak Uygulamalarının Anlık Görüntülerini oluşturmak için Bir Program</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Dit programma is uitgebracht onder de GPL3-licentie</translation>
+      <translation>Bu program GPL 3 ile lisanslanmıştır</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Translators</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>The following people translated jdFlatpakSnapshot:</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Changelog</source>
+      <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Sluiten</translation>
+      <translation>Kapat</translation>
     </message>
   </context>
   <context>
     <name>Constants</name>
     <message>
-      <location filename="../Constants.py" line="13"/>
+      <location filename="../Constants.py" line="12"/>
       <source>None</source>
-      <translation>Geen</translation>
+      <translation>Hiçbiri</translation>
     </message>
   </context>
   <context>
     <name>ImportExport</name>
     <message>
-      <location filename="../ImportExport.py" line="28"/>
+      <location filename="../ImportExport.py" line="29"/>
       <source>This includes the following Snapshot:</source>
-      <translation>Dit bevat de volgende momentopname:</translation>
+      <translation>Bu, aşağıdaki Anlık Görüntüyü içerir:</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="29"/>
+      <location filename="../ImportExport.py" line="30"/>
       <source>App: {{app}}</source>
-      <translation>App: {{app}}</translation>
+      <translation>Uygulama: {{app}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="30"/>
+      <location filename="../ImportExport.py" line="31"/>
       <source>Name: {{name}}</source>
-      <translation>Naam: {{name}}</translation>
+      <translation>Ad: {{name}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="31"/>
+      <location filename="../ImportExport.py" line="32"/>
       <source>Compression: {{compression}}</source>
-      <translation>Compressie: {{compression}}</translation>
+      <translation>Sıkıştırma: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="32"/>
+      <location filename="../ImportExport.py" line="33"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Grootte op schijf: {{size}}</translation>
+      <translation>Diskteki boyutu: {{size}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="33"/>
+      <location filename="../ImportExport.py" line="34"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Gemaakt op: {{datetime}}</translation>
+      <translation>Oluşturulma tarihi: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="34"/>
+      <location filename="../ImportExport.py" line="35"/>
       <source>Do you want to import it?</source>
-      <translation>Wilt u deze momentopname importeren?</translation>
+      <translation>İçe aktarmak istiyor musun?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="36"/>
+      <location filename="../ImportExport.py" line="37"/>
       <source>Import</source>
-      <translation>Importeren</translation>
+      <translation>İçe aktar</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>App not installed</source>
-      <translation>App niet geïnstalleerd</translation>
+      <translation>Uygulama kurulmamış</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>It looks like {{app}} is not installed. Are you really want to import the data?</source>
-      <translation>Het lijkt er op dan {{app}} niet geïnstalleerd is. Weet u zeker dat u de gegevens wilt importeren?</translation>
+      <translation>{{app}} kurulmamış görünüyor. Veriyi gerçekten içe aktarmak istiyor musun?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>New name</source>
-      <translation>Nieuwe naam</translation>
+      <translation>Yeni ad</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>There is already a Snapshot with this Name for this App. Please enter a new one.</source>
-      <translation>Er is al een momentopname van deze app onder deze naam. Kies een andere naam.</translation>
+      <translation>Bu Uygulama için bu Ada sahip bir Anlık Görüntü zaten var. Lütfen yeni bir ad girin.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>Name exists</source>
-      <translation>Naam in gebruik</translation>
+      <translation>Ad zaten var</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>This Name also exists. Please enter a new one.</source>
-      <translation>Deze naam is ook in gebruik. Kies een andere naam.</translation>
+      <translation>Bu ad da var. Lütfen yeni bir tane girin.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>Error</source>
-      <translation>Foutmelding</translation>
+      <translation>Hata</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>An error occurred during import. Maybe the File is not valid.</source>
-      <translation>Er is een fout opgetreden tijdens het importeren. Mogelijk is het bestand beschadigd.</translation>
+      <translation>İçe aktarma sırasında hata oluştu. Dosya geçersiz olabilir.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Export failed</source>
-      <translation>Exporteren mislukt</translation>
+      <translation>Dışa aktarılamadı</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Cound not export {{name}}</source>
-      <translation>{{name}} kan niet worden geëxporteerd</translation>
+      <translation>{{name}} dışa aktarılamadı</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
-      <location filename="../SettingsDialog.py" line="17"/>
+      <location filename="../Languages.py" line="6"/>
       <source>English</source>
-      <translation>Engels</translation>
+      <translation>İngilizce</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="18"/>
+      <location filename="../Languages.py" line="7"/>
       <source>German</source>
-      <translation>Duits</translation>
+      <translation>Almanca</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="8"/>
+      <source>Dutch</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="9"/>
+      <source>Turkish</source>
+      <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No Flatpaks found</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>Exported Snapshots</source>
-      <translation>Geëxporteerde momentopnamen</translation>
+      <translation>Dışa Aktarılan Anlık Görüntüler</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>All Files</source>
-      <translation>Alle bestanden</translation>
+      <translation>Tüm Dosyalar</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>Delete Snapshot of uninstalled Apps</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>This will delete all Snapshots of apps that are no longer installed. Do you want to continue?</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>Snapshots deleted</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>The Snapshots were successfully deleted</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>Delete broken Snapshots</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?</source>
+      <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>No data</source>
-      <translation>Geen gegevens</translation>
+      <translation>Veri yok</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>This Flatpak has no Data</source>
-      <translation>Deze flatpak bevat geen gegevens</translation>
+      <translation>Bu Flatpakʼın Verisi yok</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>Flatpak running</source>
+      <translation>Flatpak çalışıyor</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
+      <translation>Bu Flatpak şu anda çalışıyor. Çalışırken bir Flatpakʼın Anlık Görüntüsünü geri yükleyemezsiniz.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get Commit</source>
-      <translation>Kan commit niet opvragen</translation>
+      <translation>İşleme getirilemedi</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs.</source>
-      <translation>De commit van deze flatpak kan niet worden opgevraagd. U kunt wel een momentopname maken, maar er wordt geen versienummer toegekend.</translation>
+      <translation>Bu Flatpak için işleme alınamadı. Yine de bir Anlık Görüntü oluşturabilirsiniz, ancak bunun hangi Sürüme ait olduğunu bilemezsiniz.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Enter Name</source>
-      <translation>Naam invoeren</translation>
+      <translation>Ad Gir</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Please enter a Name for your Snapshot</source>
-      <translation>Geef de momentopname een naam</translation>
+      <translation>Anlık Görüntü için bir Ad girin</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="296"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>Name exists</source>
-      <translation>Naam in gebruik</translation>
+      <translation>Ad var</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>This Name already exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Bu Ad zaten var</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Compression method</source>
-      <translation>Compressiemethode</translation>
+      <translation>Sıkıştırma yöntemi</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Please choose a compression method</source>
-      <translation>Kies een compressiemethode</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>Flatpak running</source>
-      <translation>Flatpak in gebruik</translation>
+      <translation>Lütfen sıkıştırma yöntemi seçin</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
-      <translation>Deze flatpak is momenteel in gebruik. U kunt de momentopname van een flatpak niet herstellen zolang deze in gebruik is.</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Restore Snapshot</source>
-      <translation>Momentopname herstellen</translation>
+      <translation>Anlık Görüntüyü Geri Yükle</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.</source>
-      <translation>Weet u zeker dat u deze momentopname wilt herstellen? Hierdoor worden alle flatpakgegevens overschreven.</translation>
+      <translation>Bu Anlık Görüntüyü geri yüklemek istediğinizden emin misiniz? Bu, Flatpakʼın tüm Verilerinin üzerine yazacak.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>Error</source>
-      <translation>Foutmelding</translation>
+      <translation>Hata</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>An error occurred while deleting {{path}}</source>
-      <translation>Er is een fout opgetreden tijdens het verwijderen van {{path}}</translation>
+      <translation>{{path}} silinirken hata oluştur</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>New name</source>
-      <translation>Nieuwe naam</translation>
+      <translation>Yeni ad</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>Please enter a new name</source>
-      <translation>Voer een nieuwe naam in</translation>
+      <translation>Lütfen yeni ad girin</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
+      <location filename="../MainWindow.py" line="296"/>
       <source>This name already exists</source>
-      <translation>Deze naam is al in gebruik</translation>
+      <translation>Bu ad zaten var</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Delete snapshot</source>
-      <translation>Momentopname verwijderen</translation>
+      <translation>Anlık görüntüyü sil</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Are you sure you want to delete this snapshot?</source>
-      <translation>Weet u zeker dat u deze momentopname wilt verwijderen?</translation>
+      <translation>Bu anlık görüntüyü silmek istediğinden emin misin?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>Snapshot deleted</source>
-      <translation>Momentopname verwijderd</translation>
+      <translation>Anlık görüntü silindi</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>The snapshot was successfully deleted</source>
-      <translation>De momentopname is verwijderd</translation>
+      <translation>Anlık görüntü başarıyla silindi</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="274"/>
+      <location filename="../MainWindow.py" line="328"/>
       <source>Compression: {{compression}}</source>
-      <translation>Compressie: {{compression}}</translation>
+      <translation>Sıkıştırma: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="275"/>
+      <location filename="../MainWindow.py" line="329"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Grootte op schijf: {{size}}</translation>
+      <translation>Diskteki boyut: {{size}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="276"/>
+      <location filename="../MainWindow.py" line="330"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Gemaakt op: {{datetime}}</translation>
+      <translation>Oluşturulma tarihi: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Commit: {{commit}}</source>
-      <translation>Commit: {{commit}}</translation>
+      <translation>İşleme: {{commit}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Unknown</source>
-      <translation>Onbekend</translation>
+      <translation>Bilinmiyor</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="281"/>
+      <location filename="../MainWindow.py" line="333"/>
       <source>About {{name}}</source>
-      <translation>Over {{name}}</translation>
+      <translation>{{name}} Hakkında</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Flatpaks</source>
-      <translation>Flatpaks</translation>
+      <translation>Flatpakler</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Create Snapshot</source>
-      <translation>Momentopname maken</translation>
+      <translation>Anlık Görüntü Oluştur</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Snapshots</source>
-      <translation>Momentopnamen</translation>
+      <translation>Anlık Görüntüler</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Restore</source>
-      <translation>Herstellen</translation>
+      <translation>Geri Yükle</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Naam wijzigen</translation>
+      <translation>Yeniden Adlandır</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <translation>Sil</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Export</source>
-      <translation>Exporteren</translation>
+      <translation>Dışa Aktar</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Over</translation>
+      <translation>Hakkında</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Bestand</translation>
+      <translation>Dosya</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Ayarlar</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Maintenance</source>
+      <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Over Qt</translation>
+      <translation>Qt Hakkında</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Afsluiten</translation>
+      <translation>Çıkış</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Import</source>
-      <translation>Importeren</translation>
+      <translation>İçe Aktar</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Welkomstvenster tonen</translation>
+      <translation>Hoşgeldin iletişim kutusunu göster</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Broncode bekijken</translation>
+      <translation>Kaynağı Göster</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Bug melden</translation>
+      <translation>Hata Raporla</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Vertalen</translation>
+      <translation>Çevir</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Doneren</translation>
+      <translation>Bağış Yap</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Delete Snapshots of uninstalled Apps</source>
+      <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>ProgressDialog</name>
     <message>
+      <location filename="../ProgressDialog.py" line="32"/>
+      <source>Scanning files. Please wait...</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="42"/>
+      <source>Compressing {{path}}</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="58"/>
+      <source>Extracting {{path}}</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Progress</source>
-      <translation>Voortgang</translation>
+      <translation>İlerleme</translation>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>Cancel</source>
+      <translation type="unfinished">İptal</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../SettingsDialog.py" line="30"/>
+      <location filename="../SettingsDialog.py" line="27"/>
       <source>System language</source>
-      <translation>Systeemtaal</translation>
+      <translation>Sistem dili</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="53"/>
+      <location filename="../SettingsDialog.py" line="57"/>
       <source>(Preview: {{preview}})</source>
-      <translation>(Voorbeeld: {{preview}})</translation>
+      <translation>(Önizleme: {{preview}})</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="55"/>
+      <location filename="../SettingsDialog.py" line="59"/>
       <source>(Invalid)</source>
-      <translation>(Ongeldig)</translation>
+      <translation>(Geçersiz)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Instellingen</translation>
+      <translation>Ayarlar</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>General</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>(needs restart)</source>
+      <translation>(yeniden başlatma gerekli)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Datetime Format:</source>
-      <translation>Datum- en tijdopmaak:</translation>
+      <translation>Tarih Biçimi:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Taal:</translation>
+      <translation>Dil:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
-      <source>(needs restart)</source>
-      <translation>(herstart vereist)</translation>
+      <source>Show system Apps</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Show Apps with no Data</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow creating Snapshots while the App is running</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow restoring Snapshots while the App is running</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Advanced</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Flatpak Command</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>You can specify the command to call Flatpak here. This is only needed if Flatpak is not present in the PATH due to an own installation.</source>
+      <comment>Don't translate PATH, as it's the name of a Environment Variable</comment>
+      <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command:</source>
-      <translation>Flatpakopdracht:</translation>
+      <translation>Flatpak Komutu:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Standaardwaarden</translation>
+      <translation>Sıfırla</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Oké</translation>
+      <translation>Tamam</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>Annuleren</translation>
+      <translation>İptal</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Welkom</translation>
+      <translation>Hoşgeldiniz</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdFlatpakSnapshot!</source>
-      <translation>Welkom in jdFlatpakSnapshot!</translation>
+      <translation>jdFlatpakSnapshotʼa Hoşgeldiniz!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to create a Snapshot of the Data of a Flatpak.</source>
-      <translation>Met dit programma kunt u een momentopname van de gegevens van een flatpak maken.</translation>
+      <translation>Bu Program, bir Flatpak'ın Verilerinin Anlık Görüntüsünü oluşturmanızı sağlar.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</source>
-      <translation>Dit is bijvoorbeeld handig als u met de instellingen van een programma wilt spelen en ze nadien wilt herstellen.</translation>
+      <translation>Bu uygulamayı, örneğin bir Programın Ayarlarını değiştirmek ve bazı şeyler çalışmadığında, Anlık Görüntüyü geri yüklemek için kullanabilirsiniz.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</source>
-      <translation>Let op: dit programma maakt alleen een momentopname van de gegevens en versie van een flatpak, maar niet van de flatpak zelf.</translation>
+      <translation>Bu Program yalnızca bir Flatpakʼın Verilerini ve Flatpakʼın Sürümünü kaydeder, Flatpakʼın kendisini kaydetmez.</translation>
+    </message>
+    <message>
+      <location filename="../ui/WelcomeDialog.ui" line="0"/>
+      <source>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</source>
+      <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</source>
-      <translation>Kies een flatpak en klik op ‘Momentopname maken’ om aan de slag te gaan.</translation>
+      <translation>Başlamak için bir Flatpak seçin ve &quot;Anlık Görüntü Oluştur&quot; düğmesine tıklayın.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Venster altijd tonen na opstarten</translation>
+      <translation>Bu iletişim kutusunu başlangıçta göster</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts`

 * *Files 22% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_tr.ts` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/translations/jdFlatpakSnapshot_de.ts`

```diff
@@ -1,498 +1,650 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1" language="tr">
+<TS version="2.1" language="de">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>About</source>
-      <translation>Hakkında</translation>
+      <translation>Über</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>A Program to create Snapshots of Flatpak Apps</source>
-      <translation>Flatpak Uygulamalarının Anlık Görüntülerini oluşturmak için Bir Program</translation>
+      <translation>Ein Programm zum erstellen von Snapshots von Flatpak Apps</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
-      <translation>Bu program GPL 3 ile lisanslanmıştır</translation>
+      <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Translators</source>
+      <translation>Übersetzer</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>The following people translated jdFlatpakSnapshot:</source>
+      <translation>Die folgenden Personen haben jdFlatpakSnapshot übersetzt:</translation>
+    </message>
+    <message>
+      <location filename="../ui/AboutDialog.ui" line="0"/>
+      <source>Changelog</source>
+      <translation>Änderungsprotokoll</translation>
     </message>
     <message>
       <location filename="../ui/AboutDialog.ui" line="0"/>
       <source>Close</source>
-      <translation>Kapat</translation>
+      <translation>Schließen</translation>
     </message>
   </context>
   <context>
     <name>Constants</name>
     <message>
-      <location filename="../Constants.py" line="13"/>
+      <location filename="../Constants.py" line="12"/>
       <source>None</source>
-      <translation>Hiçbiri</translation>
+      <translation>Keine</translation>
     </message>
   </context>
   <context>
     <name>ImportExport</name>
     <message>
-      <location filename="../ImportExport.py" line="28"/>
+      <location filename="../ImportExport.py" line="29"/>
       <source>This includes the following Snapshot:</source>
-      <translation>Bu, aşağıdaki Anlık Görüntüyü içerir:</translation>
+      <translation>Dies enthält den folgenden Snapshot:</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="29"/>
+      <location filename="../ImportExport.py" line="30"/>
       <source>App: {{app}}</source>
-      <translation>Uygulama: {{app}}</translation>
+      <translation>App: {{app}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="30"/>
+      <location filename="../ImportExport.py" line="31"/>
       <source>Name: {{name}}</source>
-      <translation>Ad: {{name}}</translation>
+      <translation>Name: {{name}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="31"/>
+      <location filename="../ImportExport.py" line="32"/>
       <source>Compression: {{compression}}</source>
-      <translation>Sıkıştırma: {{compression}}</translation>
+      <translation>Komprimierungsverfahren: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="32"/>
+      <location filename="../ImportExport.py" line="33"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Diskteki boyutu: {{size}}</translation>
+      <translation>Größe auf dem Datenträger: {{size}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="33"/>
+      <location filename="../ImportExport.py" line="34"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Oluşturulma tarihi: {{datetime}}</translation>
+      <translation>Erstellt am: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="34"/>
+      <location filename="../ImportExport.py" line="35"/>
       <source>Do you want to import it?</source>
-      <translation>İçe aktarmak istiyor musun?</translation>
+      <translation>Möchtest du ihn importieren?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="36"/>
+      <location filename="../ImportExport.py" line="37"/>
       <source>Import</source>
-      <translation>İçe aktar</translation>
+      <translation>Importieren</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>App not installed</source>
-      <translation>Uygulama kurulmamış</translation>
+      <translation>App nicht installiert</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="40"/>
+      <location filename="../ImportExport.py" line="41"/>
       <source>It looks like {{app}} is not installed. Are you really want to import the data?</source>
-      <translation>{{app}} kurulmamış görünüyor. Veriyi gerçekten içe aktarmak istiyor musun?</translation>
+      <translation>Es sieht so aus, als sei {{app}} nicht intstalliert. Mächtest du die Daten trotzdem importieren?</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>New name</source>
-      <translation>Yeni ad</translation>
+      <translation>Neuer Name</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="45"/>
+      <location filename="../ImportExport.py" line="46"/>
       <source>There is already a Snapshot with this Name for this App. Please enter a new one.</source>
-      <translation>Bu Uygulama için bu Ada sahip bir Anlık Görüntü zaten var. Lütfen yeni bir ad girin.</translation>
+      <translation>Es existiert bereits ein Snapshot mt diesem Namen für diese App. Bitte gib einen neuen ein.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>Name exists</source>
-      <translation>Ad zaten var</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="51"/>
+      <location filename="../ImportExport.py" line="52"/>
       <source>This Name also exists. Please enter a new one.</source>
-      <translation>Bu ad da var. Lütfen yeni bir tane girin.</translation>
+      <translation>Diser Name existiert auch. Bitte gib einen neuen ein.</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>Error</source>
-      <translation>Hata</translation>
+      <translation>Fehler</translation>
     </message>
     <message>
-      <location filename="../ImportExport.py" line="82"/>
+      <location filename="../ImportExport.py" line="77"/>
       <source>An error occurred during import. Maybe the File is not valid.</source>
-      <translation>İçe aktarma sırasında hata oluştu. Dosya geçersiz olabilir.</translation>
+      <translation>Während des Importierens ist ein Fehler aufgetreten. Möglicherweise ist die Datei ungültig.</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Export failed</source>
-      <translation>Dışa aktarılamadı</translation>
+      <translation>Export fehlgeschlagen</translation>
     </message>
     <message>
       <location filename="../ImportExport.py" line="103"/>
       <source>Cound not export {{name}}</source>
-      <translation>{{name}} dışa aktarılamadı</translation>
+      <translation>Konnte {{name}} nicht exportieren</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
-      <location filename="../SettingsDialog.py" line="17"/>
+      <location filename="../Languages.py" line="6"/>
       <source>English</source>
-      <translation>İngilizce</translation>
+      <translation>Englisch</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="18"/>
+      <location filename="../Languages.py" line="7"/>
       <source>German</source>
-      <translation>Almanca</translation>
+      <translation>Deutsch</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="8"/>
+      <source>Dutch</source>
+      <translation>Niederländisch</translation>
+    </message>
+    <message>
+      <location filename="../Languages.py" line="9"/>
+      <source>Turkish</source>
+      <translation>Türkisch</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No Flatpaks found</source>
+      <translation>Keine Flatpaks gefunden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="87"/>
+      <source>No flatpaks were found on your system. Make sure that some are installed and jdFlatpakSnapshot has the necessary permissions. If the problem persists, please report it. You can access the bug reporting page from the ? menu.</source>
+      <translation>Es wurden keine Flatpaks auf deinem System gefunden. Stelle sicher, dass welche installiert sind und jdFlatpakSnapshot die notwendigen Berechtigungen hat. Sollte der Fehler bestehen bleiben, melde ihn bitte. Du kannst die Seite zum Melden von Fehlern über das ? Menü aufrufen.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>Exported Snapshots</source>
-      <translation>Dışa Aktarılan Anlık Görüntüler</translation>
+      <translation>Exportierte Snapshots</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="254"/>
-      <location filename="../MainWindow.py" line="142"/>
+      <location filename="../MainWindow.py" line="317"/>
+      <location filename="../MainWindow.py" line="186"/>
       <source>All Files</source>
-      <translation>Tüm Dosyalar</translation>
+      <translation>Alle Dateien</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>Delete Snapshot of uninstalled Apps</source>
+      <translation>Snapshots von deinstallierten Apps löschen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="197"/>
+      <source>This will delete all Snapshots of apps that are no longer installed. Do you want to continue?</source>
+      <translation>Dies wird alle Snapshots von Apps löschen, die nicht mehr installiert sind. Möchtest du fortfahren?</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>Snapshots deleted</source>
+      <translation>Snapshots gelöscht</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="216"/>
+      <location filename="../MainWindow.py" line="205"/>
+      <source>The Snapshots were successfully deleted</source>
+      <translation>Die Snapshots wurden erfolgreich gelöscht</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>Delete broken Snapshots</source>
+      <translation>Kaputte Snapshots löschen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="208"/>
+      <source>This will delete all broken Snaphots. This might be needed, when a Bug occurs during the creation of a Snaphot or the data is messed up. Do you want to continue?</source>
+      <translation>Dies wird alle kaputten Snapshots löschen.Das wird eventuell benötigt, wenn während des Erstellens eines Snapshots ein Bug aufgetreten ist oder Dateien zerstört sind. Möchtest du fortfahren?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>No data</source>
-      <translation>Veri yok</translation>
+      <translation>Keine Daten</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="156"/>
+      <location filename="../MainWindow.py" line="222"/>
       <source>This Flatpak has no Data</source>
-      <translation>Bu Flatpakʼın Verisi yok</translation>
+      <translation>Dieses Flatpak hat keine Daten</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>Flatpak running</source>
+      <translation>Flatpak läuft</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="269"/>
+      <location filename="../MainWindow.py" line="226"/>
+      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
+      <translation>Dieses Flatpak wird gerade ausgeführt. Du kannst keinen Snapshot wiederherstellen, während das Flatpak gerade ausgeführt wird.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get Commit</source>
-      <translation>İşleme getirilemedi</translation>
+      <translation>Kontte Commit nicht auslesen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="161"/>
+      <location filename="../MainWindow.py" line="231"/>
       <source>Could not get the commit for this Flatpak. You still can craete a Snapshot, but you will not know, to which Version it belongs.</source>
-      <translation>Bu Flatpak için işleme alınamadı. Yine de bir Anlık Görüntü oluşturabilirsiniz, ancak bunun hangi Sürüme ait olduğunu bilemezsiniz.</translation>
+      <translation>Der Commit dieses Flatpaks konnte nicht ausgelesen werden. Du kannst trotzdem einen Snapshot erstellen, weisst aber nacher nicht mehr, zu welcher Version er gehört.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Enter Name</source>
-      <translation>Ad Gir</translation>
+      <translation>Namen eingeben</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="163"/>
+      <location filename="../MainWindow.py" line="233"/>
       <source>Please enter a Name for your Snapshot</source>
-      <translation>Anlık Görüntü için bir Ad girin</translation>
+      <translation>Bitte gib einen Namen für diesen Snapshot ein</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="296"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>Name exists</source>
-      <translation>Ad var</translation>
+      <translation>Name existiert</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="170"/>
+      <location filename="../MainWindow.py" line="239"/>
       <source>This Name already exists</source>
-      <translation>Bu Ad zaten var</translation>
+      <translation>Dieser Name existiert bereits</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Compression method</source>
-      <translation>Sıkıştırma yöntemi</translation>
+      <translation>Komprimierungsverfahren</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="175"/>
+      <location filename="../MainWindow.py" line="246"/>
       <source>Please choose a compression method</source>
-      <translation>Lütfen sıkıştırma yöntemi seçin</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>Flatpak running</source>
-      <translation>Flatpak çalışıyor</translation>
+      <translation>Bitte wähle ein Komprimierungsverfahren aus</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="206"/>
-      <source>This Flatpak ts currently running. You can't restore the Snapshot of a Flatpak while it's running.</source>
-      <translation>Bu Flatpak şu anda çalışıyor. Çalışırken bir Flatpakʼın Anlık Görüntüsünü geri yükleyemezsiniz.</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Restore Snapshot</source>
-      <translation>Anlık Görüntüyü Geri Yükle</translation>
+      <translation>Snapshot wiederherstellen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="209"/>
+      <location filename="../MainWindow.py" line="272"/>
       <source>Are you sure you want to restore this Snapshot? This will overwrite all Data of this Flatpak.</source>
-      <translation>Bu Anlık Görüntüyü geri yüklemek istediğinizden emin misiniz? Bu, Flatpakʼın tüm Verilerinin üzerine yazacak.</translation>
+      <translation>Bist du sicher, dass du diesen Snapshot wiederherstellen möchtest? Vorhandene Daten werden dabei überschrieben.</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>Error</source>
-      <translation>Hata</translation>
+      <translation>fehler</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="219"/>
+      <location filename="../MainWindow.py" line="282"/>
       <source>An error occurred while deleting {{path}}</source>
-      <translation>{{path}} silinirken hata oluştur</translation>
+      <translation>Während des Löschens von {{path}} ist ein Fehler aufgetreten</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>New name</source>
-      <translation>Yeni ad</translation>
+      <translation>Neuer Name</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="225"/>
+      <location filename="../MainWindow.py" line="288"/>
       <source>Please enter a new name</source>
-      <translation>Lütfen yeni ad girin</translation>
+      <translation>Bitte gib einen neuen Namen ein</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="232"/>
+      <location filename="../MainWindow.py" line="296"/>
       <source>This name already exists</source>
-      <translation>Bu ad zaten var</translation>
+      <translation>Dieser Name existiert bereits</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Delete snapshot</source>
-      <translation>Anlık görüntüyü sil</translation>
+      <translation>Snapshot löschen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="240"/>
+      <location filename="../MainWindow.py" line="304"/>
       <source>Are you sure you want to delete this snapshot?</source>
-      <translation>Bu anlık görüntüyü silmek istediğinden emin misin?</translation>
+      <translation>Bist du sicher, dass du diesen Snapshot löschen willst?</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>Snapshot deleted</source>
-      <translation>Anlık görüntü silindi</translation>
+      <translation>Snapshot gelöscht</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="251"/>
+      <location filename="../MainWindow.py" line="314"/>
       <source>The snapshot was successfully deleted</source>
-      <translation>Anlık görüntü başarıyla silindi</translation>
+      <translation>Der Snapshot wurde erfolgreich gelöscht</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="274"/>
+      <location filename="../MainWindow.py" line="328"/>
       <source>Compression: {{compression}}</source>
-      <translation>Sıkıştırma: {{compression}}</translation>
+      <translation>Komprimierungsverfahren: {{compression}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="275"/>
+      <location filename="../MainWindow.py" line="329"/>
       <source>Size on disk: {{size}}</source>
-      <translation>Diskteki boyut: {{size}}</translation>
+      <translation>Größe auf dem Datenträger: {{size}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="276"/>
+      <location filename="../MainWindow.py" line="330"/>
       <source>Created on: {{datetime}}</source>
-      <translation>Oluşturulma tarihi: {{datetime}}</translation>
+      <translation>Erstellt am: {{datetime}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Commit: {{commit}}</source>
-      <translation>İşleme: {{commit}}</translation>
+      <translation>Commit: {{commit}}</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="277"/>
+      <location filename="../MainWindow.py" line="331"/>
       <source>Unknown</source>
-      <translation>Bilinmiyor</translation>
+      <translation>Unbekannt</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="281"/>
+      <location filename="../MainWindow.py" line="333"/>
       <source>About {{name}}</source>
-      <translation>{{name}} Hakkında</translation>
+      <translation>Über {{name}}</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Flatpaks</source>
-      <translation>Flatpakler</translation>
+      <translation>Flatpaks</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Create Snapshot</source>
-      <translation>Anlık Görüntü Oluştur</translation>
+      <translation>Snapshot erstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Snapshots</source>
-      <translation>Anlık Görüntüler</translation>
+      <translation>Snapshots</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Restore</source>
-      <translation>Geri Yükle</translation>
+      <translation>Wiederherstellen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Rename</source>
-      <translation>Yeniden Adlandır</translation>
+      <translation>Umbennenen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Delete</source>
-      <translation>Sil</translation>
+      <translation>Löschen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Export</source>
-      <translation>Dışa Aktar</translation>
+      <translation>Exportieren</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About</source>
-      <translation>Hakkında</translation>
+      <translation>Über</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
-      <translation>Dosya</translation>
+      <translation>Datei</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Settings</source>
-      <translation>Ayarlar</translation>
+      <translation>Einstellungen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Maintenance</source>
+      <translation>Wartung</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>About Qt</source>
-      <translation>Qt Hakkında</translation>
+      <translation>Über Qt</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Exit</source>
-      <translation>Çıkış</translation>
+      <translation>Beenden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Import</source>
-      <translation>İçe Aktar</translation>
+      <translation>Import</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Show welcome dialog</source>
-      <translation>Hoşgeldin iletişim kutusunu göster</translation>
+      <translation>Willkommensdialog zeigen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>View Source</source>
-      <translation>Kaynağı Göster</translation>
+      <translation>Quelltext ansehen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Report Bug</source>
-      <translation>Hata Raporla</translation>
+      <translation>Fehler melden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Translate</source>
-      <translation>Çevir</translation>
+      <translation>Übersetzen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Donate</source>
-      <translation>Bağış Yap</translation>
+      <translation>Spenden</translation>
+    </message>
+    <message>
+      <location filename="../ui/MainWindow.ui" line="0"/>
+      <source>Delete Snapshots of uninstalled Apps</source>
+      <translation>Snapshots von deinstallierten Apps löschen</translation>
     </message>
   </context>
   <context>
     <name>ProgressDialog</name>
     <message>
+      <location filename="../ProgressDialog.py" line="32"/>
+      <source>Scanning files. Please wait...</source>
+      <translation>Durchsuche Dateien. bite warten...</translation>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="42"/>
+      <source>Compressing {{path}}</source>
+      <translation>Komprimiere {{path}}</translation>
+    </message>
+    <message>
+      <location filename="../ProgressDialog.py" line="58"/>
+      <source>Extracting {{path}}</source>
+      <translation>Extrahiere {{path}}</translation>
+    </message>
+    <message>
       <location filename="../ui/ProgressDialog.ui" line="0"/>
       <source>Progress</source>
-      <translation>İlerleme</translation>
+      <translation>Fortschritt</translation>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</source>
+      <translation>Der Fortschrittsbalken zeigt nur an, wie viele Dateien bereits verarbeitet wurden. Er zeigt nicht an, den Fortschritt innerhalb einer einzigen Datei an, Wenn gerade eine größere Datei verarbeitet wird, kann es also so aussehen, als würde das Programm gerade hängen.</translation>
+    </message>
+    <message>
+      <location filename="../ui/ProgressDialog.ui" line="0"/>
+      <source>Cancel</source>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../SettingsDialog.py" line="30"/>
+      <location filename="../SettingsDialog.py" line="27"/>
       <source>System language</source>
-      <translation>Sistem dili</translation>
+      <translation>Systemsprache</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="53"/>
+      <location filename="../SettingsDialog.py" line="57"/>
       <source>(Preview: {{preview}})</source>
-      <translation>(Önizleme: {{preview}})</translation>
+      <translation>(Vorschau: {{preview}})</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="55"/>
+      <location filename="../SettingsDialog.py" line="59"/>
       <source>(Invalid)</source>
-      <translation>(Geçersiz)</translation>
+      <translation>(Ungültig)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
-      <translation>Ayarlar</translation>
+      <translation>Einstellungen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>General</source>
+      <translation>Allgemein</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>(needs restart)</source>
+      <translation>(benötigt Neustart)</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Datetime Format:</source>
-      <translation>Tarih Biçimi:</translation>
+      <translation>Datumszeitformat:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
-      <translation>Dil:</translation>
+      <translation>Sprache:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
-      <source>(needs restart)</source>
-      <translation>(yeniden başlatma gerekli)</translation>
+      <source>Show system Apps</source>
+      <translation>Systemapps anzeigen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Show Apps with no Data</source>
+      <translation>Apps ohne Daten anzeigen</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow creating Snapshots while the App is running</source>
+      <translation>Erstellen von Snapshots während die App läuft erlauben</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Allow restoring Snapshots while the App is running</source>
+      <translation>Wiederherstellen von Snapshots während die App läuft erlauben</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Advanced</source>
+      <translation>Erweitert</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>Flatpak Command</source>
+      <translation>Flatpakbefehl</translation>
+    </message>
+    <message>
+      <location filename="../ui/SettingsDialog.ui" line="0"/>
+      <source>You can specify the command to call Flatpak here. This is only needed if Flatpak is not present in the PATH due to an own installation.</source>
+      <comment>Don't translate PATH, as it's the name of a Environment Variable</comment>
+      <translation>Du kannst hier den Befehl zum aufrufen von Flatpak festlegen. Dies wird nur benötigt, wenn Flatpak aufgrund eine eigenen Installation nicht im PATH vorhanden sein sollte.</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Flatpak Command:</source>
-      <translation>Flatpak Komutu:</translation>
+      <translation>Flatpakbefehl:</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Reset</source>
-      <translation>Sıfırla</translation>
+      <translation>Zurücksetzen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>OK</source>
-      <translation>Tamam</translation>
+      <translation>Ok</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
-      <translation>İptal</translation>
+      <translation>Abbrechen</translation>
     </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
-      <translation>Hoşgeldiniz</translation>
+      <translation>Willkommen</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Welcome to jdFlatpakSnapshot!</source>
-      <translation>jdFlatpakSnapshotʼa Hoşgeldiniz!</translation>
+      <translation>Willkommen bei jdFlatpakSnapshot!</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program allows you to create a Snapshot of the Data of a Flatpak.</source>
-      <translation>Bu Program, bir Flatpak'ın Verilerinin Anlık Görüntüsünü oluşturmanızı sağlar.</translation>
+      <translation>Dieses Programm erlaubt dir, Snapshots von den Daten eines Flatpaks zu erstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</source>
-      <translation>Bu uygulamayı, örneğin bir Programın Ayarlarını değiştirmek ve bazı şeyler çalışmadığında, Anlık Görüntüyü geri yüklemek için kullanabilirsiniz.</translation>
+      <translation>Du kannst das z.B. nutzen um mit den Einstellungen eines Programms herumzuspielen und falls etwas nicht funktioniert, einfach den alten Stand wiederherstellen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</source>
-      <translation>Bu Program yalnızca bir Flatpakʼın Verilerini ve Flatpakʼın Sürümünü kaydeder, Flatpakʼın kendisini kaydetmez.</translation>
+      <translation>Dieses Programm speichert nur die Daten eines Flatpaks sowie die Version, aber nicht das Flatpak selber.</translation>
+    </message>
+    <message>
+      <location filename="../ui/WelcomeDialog.ui" line="0"/>
+      <source>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</source>
+      <translation>Solltest du auf einen Fehler stoßen, melde ihn bitte. Du kannst den Bugtracker über ?&gt;Fehler melden aufrufen. Verbesserungsvorschläge sind auch willkommen.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</source>
-      <translation>Başlamak için bir Flatpak seçin ve &quot;Anlık Görüntü Oluştur&quot; düğmesine tıklayın.</translation>
+      <translation>Um loszulegen, wähle ein Flatpak aus und klicke auf &quot;Snapshot erstellen&quot;.</translation>
     </message>
     <message>
       <location filename="../ui/WelcomeDialog.ui" line="0"/>
       <source>Show this Dialog on Startup</source>
-      <translation>Bu iletişim kutusunu başlangıçta göster</translation>
+      <translation>Diesen Dialog beim Programmstart anzeigen</translation>
     </message>
   </context>
 </TS>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/AboutDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/ProgressDialog.ui`

 * *Files 14% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/AboutDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/ProgressDialog.ui`

```diff
@@ -1,90 +1,88 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>AboutDialog</class>
-  <widget class="QDialog" name="AboutDialog">
+  <class>ProgressDialog</class>
+  <widget class="QDialog" name="ProgressDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
-        <height>300</height>
+        <height>179</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>About</string>
+      <string>Progress</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <widget class="QLabel" name="icon_label">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="minimumSize">
-            <size>
-              <width>64</width>
-              <height>64</height>
-            </size>
-          </property>
+        <widget class="QLabel" name="progress_label">
           <property name="text">
-            <string notr="true">icon_label</string>
+            <string notr="true">{Progress}</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="version_label">
-          <property name="text">
-            <string notr="true">jdFlatpakSnapshot {{version}}</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+        <widget class="QProgressBar" name="progress_bar">
+          <property name="value">
+            <number>24</number>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="label">
           <property name="text">
-            <string>A Program to create Snapshots of Flatpak Apps</string>
+            <string>The progress bar only shows how many files have been processed. It does not show the progress within a single file, so if a larger file is being processed, it may look like the program is hanging.</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_2">
-          <property name="text">
-            <string>This Program is licensed under GPL 3</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="wordWrap">
+            <bool>true</bool>
           </property>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="label_3">
-          <property name="text">
-            <string notr="true">Copyright © 2023 JakobDev</string>
+        <spacer name="verticalSpacer">
+          <property name="orientation">
+            <enum>Qt::Vertical</enum>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>40</height>
+            </size>
           </property>
-        </widget>
+        </spacer>
       </item>
       <item>
-        <widget class="QPushButton" name="close_button">
-          <property name="text">
-            <string>Close</string>
-          </property>
-        </widget>
+        <layout class="QHBoxLayout" name="horizontalLayout">
+          <item>
+            <spacer name="horizontalSpacer">
+              <property name="orientation">
+                <enum>Qt::Horizontal</enum>
+              </property>
+              <property name="sizeHint" stdset="0">
+                <size>
+                  <width>40</width>
+                  <height>20</height>
+                </size>
+              </property>
+            </spacer>
+          </item>
+          <item>
+            <widget class="QPushButton" name="cancel_button">
+              <property name="text">
+                <string>Cancel</string>
+              </property>
+            </widget>
+          </item>
+        </layout>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/MainWindow.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/MainWindow.ui`

 * *Files 6% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/MainWindow.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/MainWindow.ui`

```diff
@@ -142,16 +142,24 @@
         <addaction name="report_bug_action"/>
         <addaction name="translate_action"/>
         <addaction name="donate_action"/>
         <addaction name="separator"/>
         <addaction name="about_action"/>
         <addaction name="about_qt_action"/>
       </widget>
+      <widget class="QMenu" name="menuMaintenance">
+        <property name="title">
+          <string>Maintenance</string>
+        </property>
+        <addaction name="uninstalled_apps_snapshot_delete_action"/>
+        <addaction name="delete_broken_snapshots_action"/>
+      </widget>
       <addaction name="menuFile"/>
       <addaction name="menuSettings"/>
+      <addaction name="menuMaintenance"/>
       <addaction name="menu"/>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
     <action name="about_action">
       <property name="text">
         <string>About</string>
       </property>
@@ -197,11 +205,21 @@
       </property>
     </action>
     <action name="donate_action">
       <property name="text">
         <string>Donate</string>
       </property>
     </action>
+    <action name="uninstalled_apps_snapshot_delete_action">
+      <property name="text">
+        <string>Delete Snapshots of uninstalled Apps</string>
+      </property>
+    </action>
+    <action name="delete_broken_snapshots_action">
+      <property name="text">
+        <string>Delete broken Snapshots</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/SettingsDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui`

 * *Files 23% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/SettingsDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/WelcomeDialog.ui`

```diff
@@ -1,120 +1,149 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>SettingsDialog</class>
-  <widget class="QDialog" name="SettingsDialog">
+  <class>WelcomeDialog</class>
+  <widget class="QDialog" name="WelcomeDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
-        <height>138</height>
+        <height>271</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Settings</string>
+      <string>Welcome</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <layout class="QGridLayout" name="gridLayout">
-          <item row="1" column="0">
-            <widget class="QLabel" name="label_2">
-              <property name="text">
-                <string>Datetime Format:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="1">
-            <widget class="QLineEdit" name="datetime_format_edit"/>
-          </item>
-          <item row="0" column="0">
-            <widget class="QLabel" name="label">
-              <property name="text">
-                <string>Language:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="0" column="1">
-            <widget class="QComboBox" name="language_box"/>
-          </item>
-          <item row="0" column="2">
-            <widget class="QLabel" name="label_3">
-              <property name="text">
-                <string>(needs restart)</string>
-              </property>
-            </widget>
-          </item>
-          <item row="1" column="2">
-            <widget class="QLabel" name="datetime_format_preview_label">
-              <property name="text">
-                <string notr="true">valid-label</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="0">
-            <widget class="QLabel" name="label_4">
-              <property name="text">
-                <string>Flatpak Command:</string>
-              </property>
-            </widget>
-          </item>
-          <item row="2" column="1" colspan="2">
-            <widget class="QLineEdit" name="flatpak_command_edit"/>
-          </item>
-        </layout>
+        <widget class="QLabel" name="label">
+          <property name="text">
+            <string>Welcome to jdFlatpakSnapshot!</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QLabel" name="label_2">
+          <property name="text">
+            <string>This Program allows you to create a Snapshot of the Data of a Flatpak.</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QLabel" name="label_3">
+          <property name="text">
+            <string>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QLabel" name="label_5">
+          <property name="text">
+            <string>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QLabel" name="label_6">
+          <property name="text">
+            <string>If you encounter a bug, please report it. You can access the Bug Tracker via ?&gt;Report Bug. Suggestions for improvement are also welcome.</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QLabel" name="label_4">
+          <property name="text">
+            <string>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
+          </property>
+          <property name="wordWrap">
+            <bool>true</bool>
+          </property>
+        </widget>
       </item>
       <item>
-        <spacer name="verticalSpacer">
+        <widget class="QCheckBox" name="show_startup_check_box">
+          <property name="text">
+            <string>Show this Dialog on Startup</string>
+          </property>
+        </widget>
+      </item>
+      <item>
+        <widget class="QDialogButtonBox" name="button_box">
           <property name="orientation">
-            <enum>Qt::Vertical</enum>
+            <enum>Qt::Horizontal</enum>
+          </property>
+          <property name="standardButtons">
+            <set>QDialogButtonBox::Ok</set>
           </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>40</height>
-            </size>
-          </property>
-        </spacer>
-      </item>
-      <item>
-        <layout class="QHBoxLayout" name="horizontalLayout">
-          <item>
-            <widget class="QPushButton" name="reset_button">
-              <property name="text">
-                <string>Reset</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <spacer name="horizontalSpacer">
-              <property name="orientation">
-                <enum>Qt::Horizontal</enum>
-              </property>
-              <property name="sizeHint" stdset="0">
-                <size>
-                  <width>40</width>
-                  <height>20</height>
-                </size>
-              </property>
-            </spacer>
-          </item>
-          <item>
-            <widget class="QPushButton" name="ok_button">
-              <property name="text">
-                <string>OK</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="cancel_button">
-              <property name="text">
-                <string>Cancel</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
+        </widget>
       </item>
     </layout>
   </widget>
   <resources/>
-  <connections/>
+  <connections>
+    <connection>
+      <sender>button_box</sender>
+      <signal>accepted()</signal>
+      <receiver>WelcomeDialog</receiver>
+      <slot>accept()</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>248</x>
+          <y>254</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>157</x>
+          <y>274</y>
+        </hint>
+      </hints>
+    </connection>
+    <connection>
+      <sender>button_box</sender>
+      <signal>rejected()</signal>
+      <receiver>WelcomeDialog</receiver>
+      <slot>reject()</slot>
+      <hints>
+        <hint type="sourcelabel">
+          <x>316</x>
+          <y>260</y>
+        </hint>
+        <hint type="destinationlabel">
+          <x>286</x>
+          <y>274</y>
+        </hint>
+      </hints>
+    </connection>
+  </connections>
 </ui>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/AboutDialog.ui`

 * *Files 22% similar despite different names*

#### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot/ui/WelcomeDialog.ui` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot/ui/AboutDialog.ui`

```diff
@@ -1,136 +1,145 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WelcomeDialog</class>
-  <widget class="QDialog" name="WelcomeDialog">
+  <class>AboutDialog</class>
+  <widget class="QDialog" name="AboutDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
-        <height>271</height>
+        <height>312</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Welcome</string>
+      <string>About</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <widget class="QLabel" name="label">
-          <property name="text">
-            <string>Welcome to jdFlatpakSnapshot!</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+        <widget class="QLabel" name="icon_label">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="minimumSize">
+            <size>
+              <width>64</width>
+              <height>64</height>
+            </size>
           </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_2">
-          <property name="text">
-            <string>This Program allows you to create a Snapshot of the Data of a Flatpak.</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_3">
           <property name="text">
-            <string>You can use this e.g. to play a with the Settings of a Program and when something doesn't work, restore the Snapshot.</string>
+            <string notr="true">icon_label</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="label_5">
+        <widget class="QLabel" name="version_label">
           <property name="text">
-            <string>This Program only saves the Data of a Flatpak and the Version of the Flatpak, but not the Flatpak itself.</string>
+            <string notr="true">jdFlatpakSnapshot {{version}}</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="label_4">
-          <property name="text">
-            <string>To get started, select a Flatpak and click &quot;Create Snapshot&quot;.</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-          <property name="wordWrap">
-            <bool>true</bool>
-          </property>
+        <widget class="QTabWidget" name="tab_widget">
+          <property name="currentIndex">
+            <number>0</number>
+          </property>
+          <widget class="QWidget" name="tab">
+            <attribute name="title">
+              <string>About</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_2">
+              <item>
+                <widget class="QLabel" name="label">
+                  <property name="text">
+                    <string>A Program to create Snapshots of Flatpak Apps</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_2">
+                  <property name="text">
+                    <string>This Program is licensed under GPL 3</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_3">
+                  <property name="text">
+                    <string notr="true">Copyright © 2023 JakobDev</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_2">
+            <attribute name="title">
+              <string>Translators</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_3">
+              <item>
+                <widget class="QLabel" name="label_4">
+                  <property name="text">
+                    <string>The following people translated jdFlatpakSnapshot:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                  <property name="wordWrap">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QTextEdit" name="translators_edit">
+                  <property name="readOnly">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_3">
+            <attribute name="title">
+              <string>Changelog</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_4">
+              <item>
+                <widget class="QTextEdit" name="changelog_edit">
+                  <property name="readOnly">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
         </widget>
       </item>
       <item>
-        <widget class="QCheckBox" name="show_startup_check_box">
+        <widget class="QPushButton" name="close_button">
           <property name="text">
-            <string>Show this Dialog on Startup</string>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QDialogButtonBox" name="button_box">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Ok</set>
+            <string>Close</string>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
-  <connections>
-    <connection>
-      <sender>button_box</sender>
-      <signal>accepted()</signal>
-      <receiver>WelcomeDialog</receiver>
-      <slot>accept()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>248</x>
-          <y>254</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>157</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>button_box</sender>
-      <signal>rejected()</signal>
-      <receiver>WelcomeDialog</receiver>
-      <slot>reject()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>316</x>
-          <y>260</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>286</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-  </connections>
+  <connections/>
 </ui>
```

### Comparing `jdFlatpakSnapshot-1.1/jdFlatpakSnapshot.egg-info/SOURCES.txt` & `jdFlatpakSnapshot-2.0/jdFlatpakSnapshot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 pyproject.toml
 jdFlatpakSnapshot/AboutDialog.py
 jdFlatpakSnapshot/Constants.py
 jdFlatpakSnapshot/Environment.py
 jdFlatpakSnapshot/FlatpakHandler.py
 jdFlatpakSnapshot/Functions.py
 jdFlatpakSnapshot/ImportExport.py
+jdFlatpakSnapshot/Languages.py
 jdFlatpakSnapshot/MainWindow.py
 jdFlatpakSnapshot/ProgressDialog.py
 jdFlatpakSnapshot/Settings.py
 jdFlatpakSnapshot/SettingsDialog.py
+jdFlatpakSnapshot/Snapshot.py
+jdFlatpakSnapshot/SnapshotCollection.py
 jdFlatpakSnapshot/Types.py
 jdFlatpakSnapshot/WelcomeDialog.py
 jdFlatpakSnapshot/__init__.py
 jdFlatpakSnapshot/__main__.py
 jdFlatpakSnapshot/version.txt
 jdFlatpakSnapshot.egg-info/PKG-INFO
 jdFlatpakSnapshot.egg-info/SOURCES.txt
```

### Comparing `jdFlatpakSnapshot-1.1/pyproject.toml` & `jdFlatpakSnapshot-2.0/pyproject.toml`

 * *Files identical despite different names*

