# Comparing `tmp/ja2mqtt-1.0.0.tar.gz` & `tmp/ja2mqtt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja2mqtt-1.0.0.tar", last modified: Tue Apr 18 10:51:42 2023, max compression
+gzip compressed data, was "ja2mqtt-1.0.1.tar", last modified: Tue Apr 18 11:06:54 2023, max compression
```

## Comparing `ja2mqtt-1.0.0.tar` & `ja2mqtt-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.899004 ja2mqtt-1.0.0/
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.891809 ja2mqtt-1.0.0/.github/
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.893410 ja2mqtt-1.0.0/.github/workflows/
--rw-r--r--   0 tomas      (501) staff       (20)     1265 2023-04-18 08:50:02.000000 ja2mqtt-1.0.0/.github/workflows/docker-image.yml
--rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/.gitignore
--rw-r--r--   0 tomas      (501) staff       (20)      608 2023-04-18 08:38:27.000000 ja2mqtt-1.0.0/Makefile
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 10:51:42.898851 ja2mqtt-1.0.0/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     4113 2023-04-18 09:35:34.000000 ja2mqtt-1.0.0/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.894898 ja2mqtt-1.0.0/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/bin/env.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/bin/ja2mqtt
--rw-r--r--   0 tomas      (501) staff       (20)      178 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/bin/requirements.txt
--rwxr-xr-x   0 tomas      (501) staff       (20)      193 2023-04-14 16:09:33.000000 ja2mqtt-1.0.0/bin/venv-create.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       29 2023-04-14 16:09:33.000000 ja2mqtt-1.0.0/bin/venv-freeze.sh
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.895462 ja2mqtt-1.0.0/config/
--rw-r--r--   0 tomas      (501) staff       (20)     3335 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/config/ja2mqtt.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     1174 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/config/sample-config.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.895764 ja2mqtt-1.0.0/docker/
--rw-r--r--   0 tomas      (501) staff       (20)      935 2023-04-18 08:38:57.000000 ja2mqtt-1.0.0/docker/Dockerfile
--rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 00:34:56.000000 ja2mqtt-1.0.0/docker/docker-compose.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.895995 ja2mqtt-1.0.0/docker/mqtt-config/
--rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/docker/mqtt-config/mosquitto.conf
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.896611 ja2mqtt-1.0.0/ja2mqtt/
--rwxr-xr-x   0 tomas      (501) staff       (20)      218 2023-04-18 10:51:40.000000 ja2mqtt-1.0.0/ja2mqtt/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      788 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/__main__.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.897838 ja2mqtt-1.0.0/ja2mqtt/commands/
--rw-r--r--   0 tomas      (501) staff       (20)     2539 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/commands/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      875 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/commands/config.py
--rw-r--r--   0 tomas      (501) staff       (20)      869 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/commands/run.py
--rw-r--r--   0 tomas      (501) staff       (20)     1697 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/commands/test.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.898599 ja2mqtt-1.0.0/ja2mqtt/components/
--rw-r--r--   0 tomas      (501) staff       (20)      786 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/components/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     8485 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/components/bridge.py
--rw-r--r--   0 tomas      (501) staff       (20)     5096 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/components/mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     4879 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/components/serial.py
--rw-r--r--   0 tomas      (501) staff       (20)     5255 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/components/simulator.py
--rw-r--r--   0 tomas      (501) staff       (20)    12675 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     7450 2023-04-17 22:42:29.000000 ja2mqtt-1.0.0/ja2mqtt/utils.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 10:51:42.897262 ja2mqtt-1.0.0/ja2mqtt.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 10:51:42.000000 ja2mqtt-1.0.0/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      762 2023-04-18 10:51:42.000000 ja2mqtt-1.0.0/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-18 10:51:42.000000 ja2mqtt-1.0.0/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-18 10:51:42.000000 ja2mqtt-1.0.0/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-18 10:51:42.000000 ja2mqtt-1.0.0/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-18 10:51:42.899039 ja2mqtt-1.0.0/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1454 2023-04-18 10:18:52.000000 ja2mqtt-1.0.0/setup.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.697172 ja2mqtt-1.0.1/
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.690805 ja2mqtt-1.0.1/.github/
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.692130 ja2mqtt-1.0.1/.github/workflows/
+-rw-r--r--   0 tomas      (501) staff       (20)     1288 2023-04-18 10:58:21.000000 ja2mqtt-1.0.1/.github/workflows/docker-image.yml
+-rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/.gitignore
+-rw-r--r--   0 tomas      (501) staff       (20)      631 2023-04-18 10:56:21.000000 ja2mqtt-1.0.1/Makefile
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 11:06:54.697040 ja2mqtt-1.0.1/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 10:18:37.000000 ja2mqtt-1.0.1/README-pypi.text
+-rw-r--r--   0 tomas      (501) staff       (20)     4113 2023-04-18 09:35:34.000000 ja2mqtt-1.0.1/README.md
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.693380 ja2mqtt-1.0.1/bin/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/env.sh
+-rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/ja2mqtt
+-rw-r--r--   0 tomas      (501) staff       (20)      178 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/bin/requirements.txt
+-rwxr-xr-x   0 tomas      (501) staff       (20)      193 2023-04-14 16:09:33.000000 ja2mqtt-1.0.1/bin/venv-create.sh
+-rwxr-xr-x   0 tomas      (501) staff       (20)       29 2023-04-14 16:09:33.000000 ja2mqtt-1.0.1/bin/venv-freeze.sh
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.693834 ja2mqtt-1.0.1/config/
+-rw-r--r--   0 tomas      (501) staff       (20)     3335 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/config/ja2mqtt.yaml
+-rw-r--r--   0 tomas      (501) staff       (20)     1174 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/config/sample-config.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.694098 ja2mqtt-1.0.1/docker/
+-rw-r--r--   0 tomas      (501) staff       (20)      935 2023-04-18 08:38:57.000000 ja2mqtt-1.0.1/docker/Dockerfile
+-rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 00:34:56.000000 ja2mqtt-1.0.1/docker/docker-compose.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.694460 ja2mqtt-1.0.1/docker/mqtt-config/
+-rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/docker/mqtt-config/mosquitto.conf
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.695134 ja2mqtt-1.0.1/ja2mqtt/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      218 2023-04-18 11:06:28.000000 ja2mqtt-1.0.1/ja2mqtt/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)      788 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/__main__.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.696190 ja2mqtt-1.0.1/ja2mqtt/commands/
+-rw-r--r--   0 tomas      (501) staff       (20)     2539 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)      875 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)      869 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/run.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1697 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/commands/test.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.696862 ja2mqtt-1.0.1/ja2mqtt/components/
+-rw-r--r--   0 tomas      (501) staff       (20)      786 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)     8485 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/bridge.py
+-rw-r--r--   0 tomas      (501) staff       (20)     5096 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)     4879 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/serial.py
+-rw-r--r--   0 tomas      (501) staff       (20)     5255 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/components/simulator.py
+-rw-r--r--   0 tomas      (501) staff       (20)    12675 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)     7450 2023-04-17 22:42:29.000000 ja2mqtt-1.0.1/ja2mqtt/utils.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-18 11:06:54.695687 ja2mqtt-1.0.1/ja2mqtt.egg-info/
+-rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)      779 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-18 11:06:54.000000 ja2mqtt-1.0.1/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-18 11:06:54.697201 ja2mqtt-1.0.1/setup.cfg
+-rw-r--r--   0 tomas      (501) staff       (20)     1454 2023-04-18 10:18:52.000000 ja2mqtt-1.0.1/setup.py
```

### Comparing `ja2mqtt-1.0.0/.github/workflows/docker-image.yml` & `ja2mqtt-1.0.1/.github/workflows/docker-image.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
           python-version: "3.7"
       - name: Build Python package
         run: |
           python -m pip install --upgrade pip
           if [ -f bin/requirements.txt ]; then pip install -r bin/requirements.txt; fi
           rm -fr dist/*
           python3 setup.py egg_info sdist
-          mkdir -p docker/files
+          rm -fr docker/files && mkdir -p docker/files
           cp dist/*.tar.gz docker/files
           cp config/sample-config.yaml docker/files
           cp config/ja2mqtt.yaml docker/files
       - name: Set up QEMU
         uses: docker/setup-qemu-action@v2
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v2
```

### Comparing `ja2mqtt-1.0.0/Makefile` & `ja2mqtt-1.0.1/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 check:
 	pylint ja2mqtt
 
 image:
 	rm dist/*
 	python3 setup.py egg_info sdist
-	mkdir -p docker/files
+	rm -fr docker/files && mkdir -p docker/files
 	cp dist/ja2mqtt-*.tar.gz docker/files
 	cp config/sample-config.yaml docker/files
 	cp config/ja2mqtt.yaml docker/files
 	cd docker && docker build . --platform linux/arm64 -t tomvit/ja2mqtt-dev:latest
 
 clean:
 	rm -fr build
```

### Comparing `ja2mqtt-1.0.0/PKG-INFO` & `ja2mqtt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.0/README.md` & `ja2mqtt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/config/ja2mqtt.yaml` & `ja2mqtt-1.0.1/config/ja2mqtt.yaml`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/config/sample-config.yaml` & `ja2mqtt-1.0.1/config/sample-config.yaml`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/docker/Dockerfile` & `ja2mqtt-1.0.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/docker/mqtt-config/mosquitto.conf` & `ja2mqtt-1.0.1/docker/mqtt-config/mosquitto.conf`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/__main__.py` & `ja2mqtt-1.0.1/ja2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.1/ja2mqtt/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/commands/config.py` & `ja2mqtt-1.0.1/ja2mqtt/commands/config.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.1/ja2mqtt/commands/run.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/commands/test.py` & `ja2mqtt-1.0.1/ja2mqtt/commands/test.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.1/ja2mqtt/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.1/ja2mqtt/components/bridge.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.1/ja2mqtt/components/mqtt.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/components/serial.py` & `ja2mqtt-1.0.1/ja2mqtt/components/serial.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.1/ja2mqtt/components/simulator.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/config.py` & `ja2mqtt-1.0.1/ja2mqtt/config.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt/utils.py` & `ja2mqtt-1.0.1/ja2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.0/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.1/ja2mqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ja2mqtt-1.0.0/ja2mqtt.egg-info/SOURCES.txt` & `ja2mqtt-1.0.1/ja2mqtt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 Makefile
+README-pypi.text
 README.md
 setup.py
 .github/workflows/docker-image.yml
 bin/env.sh
 bin/ja2mqtt
 bin/requirements.txt
 bin/venv-create.sh
```

### Comparing `ja2mqtt-1.0.0/setup.py` & `ja2mqtt-1.0.1/setup.py`

 * *Files identical despite different names*

