# Comparing `tmp/pype-tensorflow-0.2.0.tar.gz` & `tmp/pype-tensorflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-tensorflow-0.2.0.tar", last modified: Fri Jan 20 12:15:28 2023, max compression
+gzip compressed data, was "pype-tensorflow-0.3.0.tar", last modified: Tue Apr 18 07:36:15 2023, max compression
```

## Comparing `pype-tensorflow-0.2.0.tar` & `pype-tensorflow-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:28.493424 pype-tensorflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-20 12:15:28.493424 pype-tensorflow-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:15:28.493424 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-20 12:15:28.000000 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-20 12:15:28.000000 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:28.000000 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-20 12:15:28.000000 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:15:28.000000 pype-tensorflow-0.2.0/pype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:15:28.493424 pype-tensorflow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-20 12:11:52.000000 pype-tensorflow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:15.290459 pype-tensorflow-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 07:36:15.290459 pype-tensorflow-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:36:15.286459 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 07:36:15.000000 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 07:36:15.000000 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:15.000000 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 07:36:15.000000 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:36:15.000000 pype-tensorflow-0.3.0/pype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:36:15.290459 pype-tensorflow-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-18 07:32:59.000000 pype-tensorflow-0.3.0/setup.py
```

### Comparing `pype-tensorflow-0.2.0/setup.py` & `pype-tensorflow-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import find_namespace_packages, setup
 
-version = "0.2.0"
+if __name__ == "__main__":
+    version = "0.3.0"
 
-deps = [
-    f"pype-base=={version}",
-    # on mac, it is recommended to use conda/mamba or source to install tensorflow
-    "tensorflow>=2.9.1",
-    "numpy>=1.23.0",
-    "protobuf>=3.19",
-]
-strict_deps = [s.replace(">=", "==") for s in deps]
+    deps = [
+        f"pype-base=={version}",
+        # on mac, it is recommended to use conda/mamba or source to install tensorflow
+        "tensorflow>=2.9.1",
+        "numpy>=1.23.0",
+        "protobuf>=3.19",
+    ]
+    strict_deps = [s.replace(">=", "==") for s in deps]
 
-setup(
-    name="pype-tensorflow",
-    install_requires=deps,
-    extras_require={"dev": strict_deps, "strict": strict_deps},
-    packages=find_namespace_packages(include=["pype.*"]),
-    version=version,
-)
+    setup(
+        name="pype-tensorflow",
+        install_requires=deps,
+        extras_require={"dev": strict_deps, "strict": strict_deps},
+        packages=find_namespace_packages(include=["pype.*"]),
+        version=version,
+    )
```

