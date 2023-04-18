# Comparing `tmp/tcfg-0.4.4.tar.gz` & `tmp/tcfg-0.4.6.tar.gz`

## Comparing `tcfg-0.4.4.tar` & `tcfg-0.4.6.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 tcfg-0.4.4/Makefile
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tcfg-0.4.4/TODO.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/cfg.yml
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/decorator.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/inherit.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/nested.json
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/__init__.py
--rw-r--r--   0        0        0    24618 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/config.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/reserved.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tcfg-0.4.4/LICENSE
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 tcfg-0.4.4/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 tcfg-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 tcfg-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tcfg-0.4.6/Makefile
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tcfg-0.4.6/TODO.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tcfg-0.4.6/examples/cfg.yml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tcfg-0.4.6/examples/decorator.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tcfg-0.4.6/examples/inherit.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tcfg-0.4.6/examples/nested.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 tcfg-0.4.6/playground/config.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 tcfg-0.4.6/playground/sample.yml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 tcfg-0.4.6/playground/type_checking.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/__init__.py
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/config.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/type_check/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/type_check/base.py
+-rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/type_check/custom_types.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 tcfg-0.4.6/tcfg/type_check/exceptions.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tcfg-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tcfg-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 tcfg-0.4.6/README.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 tcfg-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 tcfg-0.4.6/PKG-INFO
```

### Comparing `tcfg-0.4.4/Makefile` & `tcfg-0.4.6/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,13 @@
 
 badges:
 	echo No badges to create
 	# python3 make_badges.py
 
 build:
 	python3 -m build
-	# make badges
 
 deploy:
 	python3 -m twine upload --repository pypi dist/*
 
 build_deploy:
 	make build deploy
```

### Comparing `tcfg-0.4.4/examples/decorator.py` & `tcfg-0.4.6/examples/decorator.py`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.4/examples/inherit.py` & `tcfg-0.4.6/examples/inherit.py`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.4/LICENSE` & `tcfg-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.4/README.md` & `tcfg-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.4/pyproject.toml` & `tcfg-0.4.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcfg"
-version = "0.4.4"
+version = "0.4.6"
 authors = [
     { name="Tired Fox", email="zboehm104@gmail.com"}
 ]
 description="Typed dataclass like configuration objects"
 readme = "README.md"
 license = "MIT"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "saimll",
     "pyyaml>=6",
     "toml>=0.10.2"
 ]
 
+[project.optional-dependencies]
+all = ["toml","PyYaml"]
+toml = ["toml"]
+yaml = ["PyYaml"]
+
 [project.scripts]
 # moph = "mophidian.__main__:cli"
 
 [project.urls]
 "Homepage" = "https://github.com/Tired-Fox/tcfg"
 "Documentation" = "https://tired-fox.github.io/tcfg"
```

### Comparing `tcfg-0.4.4/PKG-INFO` & `tcfg-0.4.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: tcfg
-Version: 0.4.4
+Version: 0.4.6
 Summary: Typed dataclass like configuration objects
 Project-URL: Homepage, https://github.com/Tired-Fox/tcfg
 Project-URL: Documentation, https://tired-fox.github.io/tcfg
 Author-email: Tired Fox <zboehm104@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: pyyaml>=6
 Requires-Dist: saimll
 Requires-Dist: toml>=0.10.2
+Provides-Extra: all
+Requires-Dist: pyyaml; extra == 'all'
+Requires-Dist: toml; extra == 'all'
+Provides-Extra: toml
+Requires-Dist: toml; extra == 'toml'
+Provides-Extra: yaml
+Requires-Dist: pyyaml; extra == 'yaml'
 Description-Content-Type: text/markdown
 
 # tcfg
 
 ```python
 from tcfg import cfg, Option
```

