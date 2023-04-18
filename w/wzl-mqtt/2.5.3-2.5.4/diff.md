# Comparing `tmp/wzl-mqtt-2.5.3.tar.gz` & `tmp/wzl-mqtt-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wzl-mqtt-2.5.3.tar", last modified: Sat Apr 15 07:29:11 2023, max compression
+gzip compressed data, was "wzl-mqtt-2.5.4.tar", last modified: Tue Apr 18 08:19:49 2023, max compression
```

## Comparing `wzl-mqtt-2.5.3.tar` & `wzl-mqtt-2.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.938241 wzl-mqtt-2.5.3/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4274 2023-04-15 07:29:11.937241 wzl-mqtt-2.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/PyPI-README.md
--rw-rw-rw-   0 root         (0) root         (0)     4275 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 07:29:11.938241 wzl-mqtt-2.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.927241 wzl-mqtt-2.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.936241 wzl-mqtt-2.5.3/src/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17184 2023-04-15 07:26:59.000000 wzl-mqtt-2.5.3/src/mqtt/client.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3868 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.3/src/mqtt/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 07:29:11.937241 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4274 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      340 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-15 07:29:11.000000 wzl-mqtt-2.5.3/wzl_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:19:49.582964 wzl-mqtt-2.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-29 08:03:52.000000 wzl-mqtt-2.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4415 2023-04-18 08:19:49.581964 wzl-mqtt-2.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3814 2023-04-18 08:18:23.000000 wzl-mqtt-2.5.4/PyPI-README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-04-18 08:18:23.000000 wzl-mqtt-2.5.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 08:19:49.582964 wzl-mqtt-2.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-04-18 08:18:23.000000 wzl-mqtt-2.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:19:49.575964 wzl-mqtt-2.5.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:19:49.580964 wzl-mqtt-2.5.4/src/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.4/src/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17195 2023-04-18 08:18:23.000000 wzl-mqtt-2.5.4/src/mqtt/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.4/src/mqtt/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3868 2023-03-29 08:03:53.000000 wzl-mqtt-2.5.4/src/mqtt/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:19:49.581964 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4415 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 08:19:49.000000 wzl-mqtt-2.5.4/wzl_mqtt.egg-info/top_level.txt
```

### Comparing `wzl-mqtt-2.5.3/LICENSE` & `wzl-mqtt-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.3/PKG-INFO` & `wzl-mqtt-2.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-mqtt
-Version: 2.5.3
+Version: 2.5.4
 Summary: Small library containing an MQTT publisher and receiver.
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/
 Author: Matthias Bodenbenner, Benjamin Montavon
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WZL-MQTT
 
-Current stable version: 2.5.3
+Current stable version: 2.5.4
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -90,14 +90,17 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.4** - 2023-04-18
+  - fixed usage of a randomized client_id, so that the same credentials can be used for multiple clients in parallel
+
 **2.5.3** - 2023-04-15
   - if the port is specified as string it is also correctly processed now
   - improved user feedback in case of successful connection to the broker
   - improved user feedback if the combination of port, ssl and websocket is invalid
 
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
```

### Comparing `wzl-mqtt-2.5.3/PyPI-README.md` & `wzl-mqtt-2.5.4/PyPI-README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WZL-MQTT
 
-Current stable version: 2.5.3
+Current stable version: 2.5.4
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -75,14 +75,17 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.4** - 2023-04-18
+  - fixed usage of a randomized client_id, so that the same credentials can be used for multiple clients in parallel
+
 **2.5.3** - 2023-04-15
   - if the port is specified as string it is also correctly processed now
   - improved user feedback in case of successful connection to the broker
   - improved user feedback if the combination of port, ssl and websocket is invalid
 
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
```

### Comparing `wzl-mqtt-2.5.3/README.md` & `wzl-mqtt-2.5.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WZL-MQTT
 
-Current stable version: 2.5.3
+Current stable version: 2.5.4
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 For using the MQTT Broker of the chair and department specific features, refer to the [internal documention](https://iot.wzl-mq.rwth-aachen.de/documentation/mqtt.html).
 
@@ -86,17 +86,21 @@
 
 The authors acknowledge funding from the LaVA project (Large Volume Applications, contract 17IND03 of the
 European Metrology Programme for Innovation and Research EMPIR). The EMPIR initiative is co-funded by
 the European Union’s Horizon 2020 research and innovation programme and the EMPIR Participating States.
 
 ## Changelog
 
+**2.5.4** - 2023-04-18
+  - fixed usage of a randomized client_id, so that the same credentials can be used for multiple clients in parallel
+
 **2.5.3** - 2023-04-15
   - if the port is specified as string it is also correctly processed now
-  - improved logging output in case of successful connection to the broker
+  - improved user feedback in case of successful connection to the broker
+  - improved user feedback if the combination of port, ssl and websocket is invalid
 
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
 
 2.5.1
   - increased verbosity in case of errors by including the full stack trace
```

### Comparing `wzl-mqtt-2.5.3/setup.py` & `wzl-mqtt-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("PyPI-README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='wzl-mqtt',
-      version='2.5.3',
+      version='2.5.4',
       url='https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/',
       project_urls={
             "Bug Tracker": "https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues",
       },
       author='Matthias Bodenbenner, Benjamin Montavon',
       author_email='m.bodenbenner@wzl-mq.rwth-aachen.de',
       description='Small library containing an MQTT publisher and receiver.',
@@ -17,10 +17,10 @@
       long_description=long_description,
       long_description_content_type="text/markdown",
       classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
       ],
-      install_requires=['paho-mqtt==1.5.1'],
+      install_requires=['paho-mqtt~=1.5.1'],
       python_requires='>=3.6',
       zip_safe=False)
```

### Comparing `wzl-mqtt-2.5.3/src/mqtt/client.py` & `wzl-mqtt-2.5.4/src/mqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,24 @@
         Raises:
             IndexError: If there already exists a client with the given uuid.
         """
 
         self._logger = logger.get(
             'MQTTClient') if logger is not None else Logger().get('MQTTClient')
 
-        if username in MQTTClient.instances:
+        self.name = username if username is not None else str(uuid.uuid4())
+
+        if self.name in MQTTClient.instances:
             self._logger.error(
-                "MQTT Client {} already exists!".format(username))
-            raise IndexError("MQTT Client {} already exists!".format(username))
+                "MQTT Client {} already exists!".format(self.name))
+            raise IndexError("MQTT Client {} already exists!".format(self.name))
 
-        MQTTClient.instances[username] = self
-        self.name = username if username is not None else uuid.uuid4()
+        MQTTClient.instances[self.name] = self
         self.prefix = prefix
-        self._client = mqtt.Client(username, *args, **kwargs)
+        self._client = mqtt.Client(self.name, *args, **kwargs)
         self._client.on_connect = self._on_connect
         self._client.on_disconnect = self._on_disconnect
 
         self._client.loop_start()
 
         self._connected = False
```

### Comparing `wzl-mqtt-2.5.3/src/mqtt/exceptions.py` & `wzl-mqtt-2.5.4/src/mqtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.3/src/mqtt/logger.py` & `wzl-mqtt-2.5.4/src/mqtt/logger.py`

 * *Files identical despite different names*

### Comparing `wzl-mqtt-2.5.3/wzl_mqtt.egg-info/PKG-INFO` & `wzl-mqtt-2.5.4/wzl_mqtt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-mqtt
-Version: 2.5.3
+Version: 2.5.4
 Summary: Small library containing an MQTT publisher and receiver.
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/
 Author: Matthias Bodenbenner, Benjamin Montavon
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/iot/mqtt/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WZL-MQTT
 
-Current stable version: 2.5.3
+Current stable version: 2.5.4
 
 ## Documentation
 
 For the full API documentation, view [https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/](https://iot.wzl-mq.rwth-aachen.de/documentation/libs/mqtt/).
 
 ## Installation
 Requires at least Python 3.6
@@ -90,14 +90,17 @@
     except KeyboardInterrupt:
         break
 
 ```
 
 ## Changelog
 
+**2.5.4** - 2023-04-18
+  - fixed usage of a randomized client_id, so that the same credentials can be used for multiple clients in parallel
+
 **2.5.3** - 2023-04-15
   - if the port is specified as string it is also correctly processed now
   - improved user feedback in case of successful connection to the broker
   - improved user feedback if the combination of port, ssl and websocket is invalid
 
 **2.5.2** - 2023-03-29
   - client handles slash in at the end of prefix and the beginning of topic to avoid multiple consecutive slashes correctly now
```

