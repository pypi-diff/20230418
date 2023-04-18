# Comparing `tmp/ozan-arslan-0.0.1.tar.gz` & `tmp/ozan-arslan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozan-arslan-0.0.1.tar", last modified: Tue Apr 18 20:20:42 2023, max compression
+gzip compressed data, was "ozan-arslan-0.0.2.tar", last modified: Tue Apr 18 20:42:31 2023, max compression
```

## Comparing `ozan-arslan-0.0.1.tar` & `ozan-arslan-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:20:42.615070 ozan-arslan-0.0.1/
--rw-r--r--   0 MTeke1     (502) staff       (20)     1074 2023-04-18 19:57:50.000000 ozan-arslan-0.0.1/LICENSE
--rw-r--r--   0 MTeke1     (502) staff       (20)      501 2023-04-18 20:20:42.614929 ozan-arslan-0.0.1/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-18 19:49:53.000000 ozan-arslan-0.0.1/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)      576 2023-04-18 20:02:31.000000 ozan-arslan-0.0.1/pyproject.toml
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-18 20:20:42.615122 ozan-arslan-0.0.1/setup.cfg
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:20:42.613083 ozan-arslan-0.0.1/src/
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:20:42.614024 ozan-arslan-0.0.1/src/ozan/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:15:23.000000 ozan-arslan-0.0.1/src/ozan/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      684 2023-04-18 20:19:04.000000 ozan-arslan-0.0.1/src/ozan/ozan.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:20:42.614733 ozan-arslan-0.0.1/src/ozan_arslan.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)      501 2023-04-18 20:20:42.000000 ozan-arslan-0.0.1/src/ozan_arslan.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      226 2023-04-18 20:20:42.000000 ozan-arslan-0.0.1/src/ozan_arslan.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-18 20:20:42.000000 ozan-arslan-0.0.1/src/ozan_arslan.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        5 2023-04-18 20:20:42.000000 ozan-arslan-0.0.1/src/ozan_arslan.egg-info/top_level.txt
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.325318 ozan-arslan-0.0.2/
+-rw-r--r--   0 MTeke1     (502) staff       (20)     1074 2023-04-18 19:57:50.000000 ozan-arslan-0.0.2/LICENSE
+-rw-r--r--   0 MTeke1     (502) staff       (20)      936 2023-04-18 20:42:31.325146 ozan-arslan-0.0.2/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      434 2023-04-18 20:42:07.000000 ozan-arslan-0.0.2/README.md
+-rw-r--r--   0 MTeke1     (502) staff       (20)      576 2023-04-18 20:38:19.000000 ozan-arslan-0.0.2/pyproject.toml
+-rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-04-18 20:42:31.325385 ozan-arslan-0.0.2/setup.cfg
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.322578 ozan-arslan-0.0.2/src/
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.323742 ozan-arslan-0.0.2/src/ozan/
+-rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:15:23.000000 ozan-arslan-0.0.2/src/ozan/__init__.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)      686 2023-04-18 20:37:03.000000 ozan-arslan-0.0.2/src/ozan/ozan.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-04-18 20:42:31.324770 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/
+-rw-r--r--   0 MTeke1     (502) staff       (20)      936 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      226 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/SOURCES.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/dependency_links.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        5 2023-04-18 20:42:31.000000 ozan-arslan-0.0.2/src/ozan_arslan.egg-info/top_level.txt
```

### Comparing `ozan-arslan-0.0.1/LICENSE` & `ozan-arslan-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ozan-arslan-0.0.1/pyproject.toml` & `ozan-arslan-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ozan-arslan"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ozan-arslan-0.0.1/src/ozan/ozan.py` & `ozan-arslan-0.0.2/src/ozan/ozan.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 
     def run(self):
         while True:
             # Clear the console screen
             os.system("cls" if os.name == "nt" else "clear")
 
             # Print the text at the current position
-            print(" " * self.x + MovingText.text)
+            print(" " * self.x + OzanArslan.text)
 
             # Wait for a short period
             time.sleep(0.1)
 
             # Move the text to the right by one character
             self.x += 1
 
             # Wrap the text back to the beginning of the screen if it reaches the end
             if self.x >= os.get_terminal_size().columns:
                 self.x = 0
+
+
```

