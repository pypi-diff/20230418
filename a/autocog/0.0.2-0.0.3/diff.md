# Comparing `tmp/autocog-0.0.2.tar.gz` & `tmp/autocog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocog-0.0.2.tar", last modified: Tue Apr 18 20:04:19 2023, max compression
+gzip compressed data, was "autocog-0.0.3.tar", last modified: Tue Apr 18 20:09:29 2023, max compression
```

## Comparing `autocog-0.0.2.tar` & `autocog-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.795281 autocog-0.0.2/
--rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.2/.gitignore
--rw-r--r--   0 andreas    (501) staff       (20)     1227 2023-04-18 20:04:19.795093 autocog-0.0.2/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)     1135 2023-04-18 20:03:23.000000 autocog-0.0.2/README.md
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.753303 autocog-0.0.2/autocog/
--rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.2/autocog/autocog.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.794854 autocog-0.0.2/autocog.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)     1227 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)      236 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/entry_points.txt
--rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-18 20:04:19.795328 autocog-0.0.2/setup.cfg
--rw-r--r--   0 andreas    (501) staff       (20)      540 2023-04-18 20:03:37.000000 autocog-0.0.2/setup.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.965244 autocog-0.0.3/
+-rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.3/.gitignore
+-rw-r--r--   0 andreas    (501) staff       (20)     1180 2023-04-18 20:09:29.965087 autocog-0.0.3/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)     1135 2023-04-18 20:03:23.000000 autocog-0.0.3/README.md
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.935119 autocog-0.0.3/autocog/
+-rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.3/autocog/autocog.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:09:29.964861 autocog-0.0.3/autocog.egg-info/
+-rw-r--r--   0 andreas    (501) staff       (20)     1180 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)      236 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/entry_points.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/requires.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:09:29.000000 autocog-0.0.3/autocog.egg-info/top_level.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-18 20:09:29.965287 autocog-0.0.3/setup.cfg
+-rw-r--r--   0 andreas    (501) staff       (20)      746 2023-04-18 20:09:12.000000 autocog-0.0.3/setup.py
```

### Comparing `autocog-0.0.2/PKG-INFO` & `autocog-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.2
+Version: 0.0.3
+Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
-![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
```

### Comparing `autocog-0.0.2/README.md` & `autocog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autocog-0.0.2/autocog/autocog.py` & `autocog-0.0.3/autocog/autocog.py`

 * *Files identical despite different names*

### Comparing `autocog-0.0.2/autocog.egg-info/PKG-INFO` & `autocog-0.0.3/autocog.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.2
+Version: 0.0.3
+Home-page: https://github.com/andreasjansson/AutoCog
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
-![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
```

