# Comparing `tmp/dokos-1.0.4.tar.gz` & `tmp/dokos-1.0.5.tar.gz`

## Comparing `dokos-1.0.4.tar` & `dokos-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.4/10-million-password-list-top-1000.txt
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dokos-1.0.4/pyproject.tmpl
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.4/requirements.txt
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.4/.vscode/launch.json
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/VERSION
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/__init__.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 dokos-1.0.4/src/dokos/__main__.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.4/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.4/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dokos-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 dokos-1.0.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dokos-1.0.5/10-million-password-list-top-1000.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 dokos-1.0.5/pyproject.tmpl
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dokos-1.0.5/requirements.txt
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 dokos-1.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/VERSION
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/__init__.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 dokos-1.0.5/src/dokos/__main__.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 dokos-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 dokos-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dokos-1.0.5/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dokos-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 dokos-1.0.5/PKG-INFO
```

### Comparing `dokos-1.0.4/.gitlab-ci.yml` & `dokos-1.0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/10-million-password-list-top-1000.txt` & `dokos-1.0.5/10-million-password-list-top-1000.txt`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/pyproject.tmpl` & `dokos-1.0.5/pyproject.tmpl`

 * *Files 20% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.cylab.be/cylab/dokos"
 "Bug Tracker" = "https://gitlab.cylab.be/cylab/dokos/-/issues"
 
 [project.scripts]
-dokos = "dokos.dokos:main"
+dokos = "dokos.__main__:main"
```

### Comparing `dokos-1.0.4/.vscode/launch.json` & `dokos-1.0.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/src/dokos/__main__.py` & `dokos-1.0.5/src/dokos/__main__.py`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/.gitignore` & `dokos-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/LICENSE` & `dokos-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/README.md` & `dokos-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dokos-1.0.4/pyproject.toml` & `dokos-1.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Dokos"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Thibault Debatty", email="t.debatty@cylab.be" },
 ]
 description = "HTTP login cracker"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -22,8 +22,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.cylab.be/cylab/dokos"
 "Bug Tracker" = "https://gitlab.cylab.be/cylab/dokos/-/issues"
 
 [project.scripts]
-dokos = "dokos.dokos:main"
+dokos = "dokos.__main__:main"
```

### Comparing `dokos-1.0.4/PKG-INFO` & `dokos-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dokos
-Version: 1.0.4
+Version: 1.0.5
 Summary: HTTP login cracker
 Project-URL: Homepage, https://gitlab.cylab.be/cylab/dokos
 Project-URL: Bug Tracker, https://gitlab.cylab.be/cylab/dokos/-/issues
 Author-email: Thibault Debatty <t.debatty@cylab.be>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

