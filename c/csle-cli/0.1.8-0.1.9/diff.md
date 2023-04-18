# Comparing `tmp/csle_cli-0.1.8.tar.gz` & `tmp/csle_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.1.8.tar", last modified: Mon Mar 20 15:29:47 2023, max compression
+gzip compressed data, was "csle_cli-0.1.9.tar", last modified: Tue Mar 21 08:10:40 2023, max compression
```

## Comparing `csle_cli-0.1.8.tar` & `csle_cli-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:47.297964 csle_cli-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-03-20 15:29:47.298100 csle_cli-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)    22943 2023-02-12 17:03:02.000000 csle_cli-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      668 2023-02-12 08:59:32.000000 csle_cli-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1368 2023-03-20 15:29:47.299132 csle_cli-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cli-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:47.290097 csle_cli-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:47.293443 csle_cli-0.1.8/src/csle_cli/
--rw-r--r--   0 kimham     (501) staff       (20)       38 2022-11-28 13:00:49.000000 csle_cli-0.1.8/src/csle_cli/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_cli-0.1.8/src/csle_cli/__version__.py
--rwxr-xr-x   0 kimham     (501) staff       (20)   111224 2023-03-20 13:32:15.000000 csle_cli-0.1.8/src/csle_cli/cli.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:47.297725 csle_cli-0.1.8/src/csle_cli.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      629 2023-03-20 15:29:46.000000 csle_cli-0.1.8/src/csle_cli.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      369 2023-03-20 15:29:47.000000 csle_cli-0.1.8/src/csle_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:29:46.000000 csle_cli-0.1.8/src/csle_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)       47 2023-03-20 15:29:47.000000 csle_cli-0.1.8/src/csle_cli.egg-info/entry_points.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:54.000000 csle_cli-0.1.8/src/csle_cli.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      291 2023-03-20 15:29:47.000000 csle_cli-0.1.8/src/csle_cli.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)        9 2023-03-20 15:29:47.000000 csle_cli-0.1.8/src/csle_cli.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:40.833284 csle_cli-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-03-21 08:10:40.833284 csle_cli-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22943 2023-02-28 07:08:18.000000 csle_cli-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-02-11 20:28:41.000000 csle_cli-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1368 2023-03-21 08:10:40.833284 csle_cli-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_cli-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:40.829284 csle_cli-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:40.833284 csle_cli-0.1.9/src/csle_cli/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       38 2022-11-28 13:03:16.000000 csle_cli-0.1.9/src/csle_cli/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_cli-0.1.9/src/csle_cli/__version__.py
+-rwxrwxr-x   0 kim       (1000) kim       (1000)   111224 2023-03-21 06:33:58.000000 csle_cli-0.1.9/src/csle_cli/cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:40.833284 csle_cli-0.1.9/src/csle_cli.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      629 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      369 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       47 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.1.9/src/csle_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      291 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2023-03-21 08:10:40.000000 csle_cli-0.1.9/src/csle_cli.egg-info/top_level.txt
```

### Comparing `csle_cli-0.1.8/PKG-INFO` & `csle_cli-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.1.8/README.md` & `csle_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.1.8/pyproject.toml` & `csle_cli-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.1.8/setup.cfg` & `csle_cli-0.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-common>=0.1.8
-	csle-cluster>=0.1.8
-	csle-collector>=0.1.8
-	csle-attacker>=0.1.8
-	csle-defender>=0.1.8
-	csle-system-identification>=0.1.8
-	gym-csle-stopping-game>=0.1.8
-	csle-agents>=0.1.8
+	csle-common>=0.1.9
+	csle-cluster>=0.1.9
+	csle-collector>=0.1.9
+	csle-attacker>=0.1.9
+	csle-defender>=0.1.9
+	csle-system-identification>=0.1.9
+	gym-csle-stopping-game>=0.1.9
+	csle-agents>=0.1.9
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.1.8/src/csle_cli/cli.py` & `csle_cli-0.1.9/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.1.8/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.1.9/src/csle_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

