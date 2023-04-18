# Comparing `tmp/pypsn-0.1.0.tar.gz` & `tmp/pypsn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypsn-0.1.0.tar", last modified: Sun Apr 16 14:09:54 2023, max compression
+gzip compressed data, was "pypsn-0.1.1.tar", last modified: Tue Apr 18 12:02:00 2023, max compression
```

## Comparing `pypsn-0.1.0.tar` & `pypsn-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-16 14:09:54.124404 pypsn-0.1.0/
--rw-r--r--   0 vanous    (1000) vanous    (1000)     1063 2023-04-05 17:36:44.000000 pypsn-0.1.0/LICENSE
--rw-r--r--   0 vanous    (1000) vanous    (1000)     2569 2023-04-16 14:09:54.124404 pypsn-0.1.0/PKG-INFO
--rw-r--r--   0 vanous    (1000) vanous    (1000)     2173 2023-04-16 14:01:37.000000 pypsn-0.1.0/README.md
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-16 14:09:54.124404 pypsn-0.1.0/pypsn/
--rwxr-xr-x   0 vanous    (1000) vanous    (1000)     9626 2023-04-12 18:16:14.000000 pypsn-0.1.0/pypsn/__init__.py
-drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-16 14:09:54.124404 pypsn-0.1.0/pypsn.egg-info/
--rw-r--r--   0 vanous    (1000) vanous    (1000)     2569 2023-04-16 14:09:54.000000 pypsn-0.1.0/pypsn.egg-info/PKG-INFO
--rw-r--r--   0 vanous    (1000) vanous    (1000)      160 2023-04-16 14:09:54.000000 pypsn-0.1.0/pypsn.egg-info/SOURCES.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)        1 2023-04-16 14:09:54.000000 pypsn-0.1.0/pypsn.egg-info/dependency_links.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)        6 2023-04-16 14:09:54.000000 pypsn-0.1.0/pypsn.egg-info/top_level.txt
--rw-r--r--   0 vanous    (1000) vanous    (1000)       38 2023-04-16 14:09:54.124404 pypsn-0.1.0/setup.cfg
--rw-r--r--   0 vanous    (1000) vanous    (1000)      599 2023-04-16 13:59:25.000000 pypsn-0.1.0/setup.py
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     1063 2023-04-05 17:36:44.000000 pypsn-0.1.1/LICENSE
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     2255 2023-04-18 12:02:00.553688 pypsn-0.1.1/PKG-INFO
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     1847 2023-04-18 11:54:55.000000 pypsn-0.1.1/README.md
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/pypsn/
+-rwxr-xr-x   0 vanous    (1000) vanous    (1000)     9627 2023-04-18 11:58:57.000000 pypsn-0.1.1/pypsn/__init__.py
+drwxr-xr-x   0 vanous    (1000) vanous    (1000)        0 2023-04-18 12:02:00.553688 pypsn-0.1.1/pypsn.egg-info/
+-rw-r--r--   0 vanous    (1000) vanous    (1000)     2255 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/PKG-INFO
+-rw-r--r--   0 vanous    (1000) vanous    (1000)      160 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/SOURCES.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)        1 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/dependency_links.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)        6 2023-04-18 12:02:00.000000 pypsn-0.1.1/pypsn.egg-info/top_level.txt
+-rw-r--r--   0 vanous    (1000) vanous    (1000)       38 2023-04-18 12:02:00.553688 pypsn-0.1.1/setup.cfg
+-rw-r--r--   0 vanous    (1000) vanous    (1000)      611 2023-04-18 11:52:07.000000 pypsn-0.1.1/setup.py
```

### Comparing `pypsn-0.1.0/LICENSE` & `pypsn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypsn-0.1.0/PKG-INFO` & `pypsn-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pypsn
-Version: 0.1.0
+Version: 0.1.1
 Summary: PosiStageNet parser
 Home-page: https://github.com/open-stage/python-psn
 Author: vanous
 Author-email: noreply@nodomain.com
 License: MIT
 Project-URL: Source, https://github.com/open-stage/python-psn
-Project-URL: Changelog, https://github.com/open-stage/python-psn/CHANGELOG.md
+Project-URL: Changelog, https://github.com/open-stage/python-psn/blob/master/CHANGELOG.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-psn
 
 Pure Python parsing library for PSN V2 - [PosiStageNet](https://posistage.net/)
 
-PSN specification as per [GitHub repo](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+[Official PSN specification](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+
+[Source code](https://github.com/open-stage/python-psn)
 
 ## Installation
 
 ```bash
 pip install pypsn
 ```
 
-To install latest master from git, run pip:
+To install latest master from git via pip:
 ```bash
 python -m pip install https://codeload.github.com/open-stage/python-psn/zip/refs/heads/master
 ```
 
 ## Usage
 
 ```python
@@ -55,15 +57,15 @@
 
 ## Development, status
 
 - Supporting PSN V2
 - Parsing only, not sending
 - Using threading module
 - Linux, Windows and macOS tested
-- Typed
+- Typed, no-strict
 - Initial pytest testing provided together with CI/CD setup
 
 ### Type hints
 
 * At this point, the `--no-strict-optional` is needed for mypy tests to pass:
 
 ```bash
@@ -78,29 +80,7 @@
 - to test, use `pytest`
 - to test typing with mypy use 
 
 ```bash
 pytest --mypy -m mypy pypsn/*py
 ```
 
-## Releasing to pypi
-
-* update CHANGELOG.md
-* increment version in setup.py
-* `git tag versionCode`
-* `git push origin/versionCode`
-* generate wheel:
-
-```bash
-python3 setup.py sdist bdist_wheel
-```
-* test upload to TestPypi with twine:
-
-```bash
-python -m twine upload --repository testpypi dist/* --verbose
-```
-
-* release to official pypi:
-
-```bash
-python -m twine upload dist/*
-```
```

### Comparing `pypsn-0.1.0/README.md` & `pypsn-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # python-psn
 
 Pure Python parsing library for PSN V2 - [PosiStageNet](https://posistage.net/)
 
-PSN specification as per [GitHub repo](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+[Official PSN specification](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+
+[Source code](https://github.com/open-stage/python-psn)
 
 ## Installation
 
 ```bash
 pip install pypsn
 ```
 
-To install latest master from git, run pip:
+To install latest master from git via pip:
 ```bash
 python -m pip install https://codeload.github.com/open-stage/python-psn/zip/refs/heads/master
 ```
 
 ## Usage
 
 ```python
@@ -42,15 +44,15 @@
 
 ## Development, status
 
 - Supporting PSN V2
 - Parsing only, not sending
 - Using threading module
 - Linux, Windows and macOS tested
-- Typed
+- Typed, no-strict
 - Initial pytest testing provided together with CI/CD setup
 
 ### Type hints
 
 * At this point, the `--no-strict-optional` is needed for mypy tests to pass:
 
 ```bash
@@ -65,29 +67,7 @@
 - to test, use `pytest`
 - to test typing with mypy use 
 
 ```bash
 pytest --mypy -m mypy pypsn/*py
 ```
 
-## Releasing to pypi
-
-* update CHANGELOG.md
-* increment version in setup.py
-* `git tag versionCode`
-* `git push origin/versionCode`
-* generate wheel:
-
-```bash
-python3 setup.py sdist bdist_wheel
-```
-* test upload to TestPypi with twine:
-
-```bash
-python -m twine upload --repository testpypi dist/* --verbose
-```
-
-* release to official pypi:
-
-```bash
-python -m twine upload dist/*
-```
```

### Comparing `pypsn-0.1.0/pypsn/__init__.py` & `pypsn-0.1.1/pypsn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class psn_vector3:
     def __init__(self, x: float, y: float, z: float):
         self.x = x
         self.y = y
         self.z = z
 
     def __str__(self):
-        return f"{self.x}, {self.y} {self.z}"
+        return f"{self.x}, {self.y}, {self.z}"
 
     def __eq__(self, other) -> bool:
         return self.x == other.x and self.y == other.y and self.z == other.z
 
     def __iter__(self):
         return iter((self.x, self.y, self.z))
 
@@ -295,29 +295,29 @@
     while buffer:
         tracker_id, chunk_buffer, buffer = parse_chunk(buffer)
 
         tracker = psn_tracker(tracker_id)
 
         if len(chunk_buffer) > 0:
             while chunk_buffer:
-                chunk_id, info_buffer, chunk_buffer = parse_chunk(chunk_buffer)
+                chunk_id, data_buffer, chunk_buffer = parse_chunk(chunk_buffer)
                 if chunk_id in iter(psn_tracker_chunk):
-                    vector = psn_vector3(*unpack("<fff", info_buffer))
+                    vector = psn_vector3(*unpack("<fff", data_buffer))
                     if chunk_id == psn_tracker_chunk.PSN_DATA_TRACKER_POS:
                         tracker.pos = vector
                     elif chunk_id == psn_tracker_chunk.PSN_DATA_TRACKER_ORI:
                         tracker.ori = vector
                     elif chunk_id == psn_tracker_chunk.PSN_DATA_TRACKER_ACCEL:
                         tracker.accel = vector
                     elif chunk_id == psn_tracker_chunk.PSN_DATA_TRACKER_SPEED:
                         tracker.speed = vector
                     elif chunk_id == psn_tracker_chunk.PSN_DATA_TRACKER_TRGTPOS:
                         tracker.trgtpos = vector
 
                 elif chunk_id == psn_tracker_chunk_info.PSN_DATA_TRACKER_STATUS:
-                    status = unpack("<f", info_buffer)[0]
+                    status = unpack("<f", data_buffer)[0]
                     tracker.status = status
                 elif chunk_id == psn_tracker_chunk_info.PSN_DATA_TRACKER_TIMESTAMP:
-                    timestamp = unpack("<L", info_buffer)[0]
+                    timestamp = unpack("<L", data_buffer)[0]
                     tracker.timestamp = timestamp
         trackers.append(tracker)
     return trackers
```

### Comparing `pypsn-0.1.0/pypsn.egg-info/PKG-INFO` & `pypsn-0.1.1/pypsn.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pypsn
-Version: 0.1.0
+Version: 0.1.1
 Summary: PosiStageNet parser
 Home-page: https://github.com/open-stage/python-psn
 Author: vanous
 Author-email: noreply@nodomain.com
 License: MIT
 Project-URL: Source, https://github.com/open-stage/python-psn
-Project-URL: Changelog, https://github.com/open-stage/python-psn/CHANGELOG.md
+Project-URL: Changelog, https://github.com/open-stage/python-psn/blob/master/CHANGELOG.md
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-psn
 
 Pure Python parsing library for PSN V2 - [PosiStageNet](https://posistage.net/)
 
-PSN specification as per [GitHub repo](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+[Official PSN specification](https://github.com/vyv/psn-cpp/blob/master/doc/PosiStageNetprotocol_v2.03_2019_09_09.pdf)
+
+[Source code](https://github.com/open-stage/python-psn)
 
 ## Installation
 
 ```bash
 pip install pypsn
 ```
 
-To install latest master from git, run pip:
+To install latest master from git via pip:
 ```bash
 python -m pip install https://codeload.github.com/open-stage/python-psn/zip/refs/heads/master
 ```
 
 ## Usage
 
 ```python
@@ -55,15 +57,15 @@
 
 ## Development, status
 
 - Supporting PSN V2
 - Parsing only, not sending
 - Using threading module
 - Linux, Windows and macOS tested
-- Typed
+- Typed, no-strict
 - Initial pytest testing provided together with CI/CD setup
 
 ### Type hints
 
 * At this point, the `--no-strict-optional` is needed for mypy tests to pass:
 
 ```bash
@@ -78,29 +80,7 @@
 - to test, use `pytest`
 - to test typing with mypy use 
 
 ```bash
 pytest --mypy -m mypy pypsn/*py
 ```
 
-## Releasing to pypi
-
-* update CHANGELOG.md
-* increment version in setup.py
-* `git tag versionCode`
-* `git push origin/versionCode`
-* generate wheel:
-
-```bash
-python3 setup.py sdist bdist_wheel
-```
-* test upload to TestPypi with twine:
-
-```bash
-python -m twine upload --repository testpypi dist/* --verbose
-```
-
-* release to official pypi:
-
-```bash
-python -m twine upload dist/*
-```
```

### Comparing `pypsn-0.1.0/setup.py` & `pypsn-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pypsn",
-    version="0.1.0",
+    version="0.1.1",
     long_description=long_description,
     description="PosiStageNet parser",
     license="MIT",
     url="https://github.com/open-stage/python-psn",
     long_description_content_type="text/markdown",
     author="vanous",
     author_email="noreply@nodomain.com",
     packages=["pypsn"],
     project_urls={
         "Source": "https://github.com/open-stage/python-psn",
-        "Changelog": "https://github.com/open-stage/python-psn/CHANGELOG.md",
+        "Changelog": "https://github.com/open-stage/python-psn/blob/master/CHANGELOG.md",
     },
 )
```

