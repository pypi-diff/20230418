# Comparing `tmp/zenoml-0.4.6.tar.gz` & `tmp/zenoml-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenoml-0.4.6.tar", max compression
+gzip compressed data, was "zenoml-0.4.7.tar", max compression
```

## Comparing `zenoml-0.4.6.tar` & `zenoml-0.4.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1081 2022-02-24 19:12:18.966638 zenoml-0.4.6/LICENSE.md
--rw-r--r--   0        0        0     3934 2023-03-29 10:51:34.882987 zenoml-0.4.6/README.md
--rw-r--r--   0        0        0     1321 2023-04-16 15:13:54.593984 zenoml-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      427 2023-04-16 15:12:31.649606 zenoml-0.4.6/zeno/__init__.py
--rw-r--r--   0        0        0       53 2023-04-16 15:12:31.655723 zenoml-0.4.6/zeno/__main__.py
--rwxr-xr-x   0        0        0     5943 2023-04-16 15:12:31.814437 zenoml-0.4.6/zeno/api.py
--rw-r--r--   0        0        0    21519 2023-04-16 15:12:31.891037 zenoml-0.4.6/zeno/backend.py
--rw-r--r--   0        0        0     1543 2023-04-16 15:12:31.667539 zenoml-0.4.6/zeno/classes/base.py
--rw-r--r--   0        0        0     1340 2023-04-16 15:12:31.756077 zenoml-0.4.6/zeno/classes/classes.py
--rw-r--r--   0        0        0      821 2023-04-16 15:12:31.639350 zenoml-0.4.6/zeno/classes/metadata.py
--rw-r--r--   0        0        0      487 2023-04-16 15:12:31.638895 zenoml-0.4.6/zeno/classes/projection.py
--rw-r--r--   0        0        0      692 2023-04-16 15:12:31.736743 zenoml-0.4.6/zeno/classes/report.py
--rw-r--r--   0        0        0      650 2023-04-16 15:12:31.677226 zenoml-0.4.6/zeno/classes/slice.py
--rw-r--r--   0        0        0     6148 2023-02-07 21:13:15.301646 zenoml-0.4.6/zeno/frontend/.DS_Store
--rw-r--r--   0        0        0  1844175 2023-04-16 15:14:19.147192 zenoml-0.4.6/zeno/frontend/build/assets/main.5a7a7111.js
--rw-r--r--   0        0        0    57544 2023-04-16 15:14:19.137821 zenoml-0.4.6/zeno/frontend/build/assets/main.6757dad9.css
--rw-r--r--   0        0        0     1173 2023-04-16 15:14:17.851374 zenoml-0.4.6/zeno/frontend/build/favicon.png
--rw-r--r--   0        0        0     1016 2023-04-16 15:14:17.852054 zenoml-0.4.6/zeno/frontend/build/global.css
--rw-r--r--   0        0        0      255 2023-04-16 15:14:19.136469 zenoml-0.4.6/zeno/frontend/build/manifest.json
--rw-r--r--   0        0        0   370831 2023-04-16 15:14:17.854859 zenoml-0.4.6/zeno/frontend/build/smui.css
--rw-r--r--   0        0        0    17353 2023-04-16 15:14:17.855845 zenoml-0.4.6/zeno/frontend/build/zeno.png
--rw-r--r--   0        0        0      863 2023-04-16 15:14:19.758717 zenoml-0.4.6/zeno/frontend/index.html
--rw-r--r--   0        0        0      881 2023-03-08 02:24:41.317296 zenoml-0.4.6/zeno/frontend/index_og.html
--rw-r--r--   0        0        0     6519 2023-04-16 15:12:31.752207 zenoml-0.4.6/zeno/processing/data_processing.py
--rw-r--r--   0        0        0     2980 2023-04-16 15:12:31.700099 zenoml-0.4.6/zeno/processing/filtering.py
--rw-r--r--   0        0        0     6985 2023-04-16 15:12:31.830529 zenoml-0.4.6/zeno/processing/histogram_processing.py
--rw-r--r--   0        0        0     3585 2023-04-16 15:12:31.727047 zenoml-0.4.6/zeno/processing/projection_processing.py
--rwxr-xr-x   0        0        0     2945 2023-04-16 15:12:31.676618 zenoml-0.4.6/zeno/runner.py
--rw-r--r--   0        0        0     8672 2023-04-16 15:12:31.796712 zenoml-0.4.6/zeno/server.py
--rw-r--r--   0        0        0     2834 2023-04-16 15:12:31.713471 zenoml-0.4.6/zeno/setup.py
--rw-r--r--   0        0        0     7275 2023-04-16 15:12:31.824953 zenoml-0.4.6/zeno/util.py
--rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 zenoml-0.4.6/setup.py
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 zenoml-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-02-24 19:12:18.966638 zenoml-0.4.7/LICENSE.md
+-rw-r--r--   0        0        0     4488 2023-04-17 23:18:23.305935 zenoml-0.4.7/README.md
+-rw-r--r--   0        0        0     1321 2023-04-17 23:18:35.286697 zenoml-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-17 23:18:23.328202 zenoml-0.4.7/zeno/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-16 15:12:31.655723 zenoml-0.4.7/zeno/__main__.py
+-rwxr-xr-x   0        0        0     5943 2023-04-16 15:12:31.814437 zenoml-0.4.7/zeno/api.py
+-rw-r--r--   0        0        0    21519 2023-04-16 15:12:31.891037 zenoml-0.4.7/zeno/backend.py
+-rw-r--r--   0        0        0     1543 2023-04-16 15:12:31.667539 zenoml-0.4.7/zeno/classes/base.py
+-rw-r--r--   0        0        0     1340 2023-04-16 15:12:31.756077 zenoml-0.4.7/zeno/classes/classes.py
+-rw-r--r--   0        0        0      821 2023-04-16 15:12:31.639350 zenoml-0.4.7/zeno/classes/metadata.py
+-rw-r--r--   0        0        0      487 2023-04-16 15:12:31.638895 zenoml-0.4.7/zeno/classes/projection.py
+-rw-r--r--   0        0        0      692 2023-04-16 15:12:31.736743 zenoml-0.4.7/zeno/classes/report.py
+-rw-r--r--   0        0        0      650 2023-04-16 15:12:31.677226 zenoml-0.4.7/zeno/classes/slice.py
+-rw-r--r--   0        0        0     6148 2023-02-07 21:13:15.301646 zenoml-0.4.7/zeno/frontend/.DS_Store
+-rw-r--r--   0        0        0  1844175 2023-04-17 23:19:05.657730 zenoml-0.4.7/zeno/frontend/build/assets/main.5a7a7111.js
+-rw-r--r--   0        0        0    57544 2023-04-17 23:19:05.657204 zenoml-0.4.7/zeno/frontend/build/assets/main.6757dad9.css
+-rw-r--r--   0        0        0     1173 2023-04-17 23:19:04.384539 zenoml-0.4.7/zeno/frontend/build/favicon.png
+-rw-r--r--   0        0        0     1016 2023-04-17 23:19:04.385260 zenoml-0.4.7/zeno/frontend/build/global.css
+-rw-r--r--   0        0        0      255 2023-04-17 23:19:05.657268 zenoml-0.4.7/zeno/frontend/build/manifest.json
+-rw-r--r--   0        0        0   370831 2023-04-17 23:19:04.388186 zenoml-0.4.7/zeno/frontend/build/smui.css
+-rw-r--r--   0        0        0    17353 2023-04-17 23:19:04.389588 zenoml-0.4.7/zeno/frontend/build/zeno.png
+-rw-r--r--   0        0        0      863 2023-04-17 23:19:06.058249 zenoml-0.4.7/zeno/frontend/index.html
+-rw-r--r--   0        0        0      881 2023-03-08 02:24:41.317296 zenoml-0.4.7/zeno/frontend/index_og.html
+-rw-r--r--   0        0        0     6519 2023-04-16 15:12:31.752207 zenoml-0.4.7/zeno/processing/data_processing.py
+-rw-r--r--   0        0        0     2980 2023-04-16 15:12:31.700099 zenoml-0.4.7/zeno/processing/filtering.py
+-rw-r--r--   0        0        0     6985 2023-04-16 15:12:31.830529 zenoml-0.4.7/zeno/processing/histogram_processing.py
+-rw-r--r--   0        0        0     3585 2023-04-16 15:12:31.727047 zenoml-0.4.7/zeno/processing/projection_processing.py
+-rwxr-xr-x   0        0        0     2946 2023-04-17 23:18:23.328661 zenoml-0.4.7/zeno/runner.py
+-rw-r--r--   0        0        0     8672 2023-04-16 15:12:31.796712 zenoml-0.4.7/zeno/server.py
+-rw-r--r--   0        0        0     2834 2023-04-16 15:12:31.713471 zenoml-0.4.7/zeno/setup.py
+-rw-r--r--   0        0        0     7275 2023-04-16 15:12:31.824953 zenoml-0.4.7/zeno/util.py
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 zenoml-0.4.7/setup.py
+-rw-r--r--   0        0        0     5701 1970-01-01 00:00:00.000000 zenoml-0.4.7/PKG-INFO
```

### Comparing `zenoml-0.4.6/LICENSE.md` & `zenoml-0.4.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/README.md` & `zenoml-0.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 It combines a **Python API** with an **interactive UI** to allow users to discover, explore, and analyze the performance of their models across diverse use cases.
 Zeno can be used for any data type or task with [modular views](https://zenoml.com/docs/views/) for everything from object detection to audio transcription.
 
 
 ### Demos
 
 
-| **Image Classification**  | **Audio Transcription** | **Image Generation** | **Sensor Data Exploration** |
-|:-------------:|:-------------:|:-------------:|:-------------:|
-| CIFAR-10  | Speech Accent Archive | DiffusionDB | MotionSense |
-|[![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://image-example.zenoml.com/)| [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://audio-example.zenoml.com/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-diffusiondb.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://imu-example.zenoml.com/) |
+| **Image Classification**  | **Audio Transcription** | **Image Generation** | **Dataset Chatbot** | **Sensor Classification**
+|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
+| Imagenette  | Speech Accent Archive | DiffusionDB | LangChain + Notion | MotionSense
+|[![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imagenette.hf.space/)| [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-audio-transcription.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-diffusiondb.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-langchain-qa.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imu-classification.hf.space)
+| [code](https://huggingface.co/spaces/zeno-ml/imagenette/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/diffusiondb/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/imu-classification/tree/main) |
 
 <br /> 
 
 https://user-images.githubusercontent.com/4563691/220689691-1ad7c184-02db-4615-b5ac-f52b8d5b8ea3.mp4
 
 ## Quickstart
```

### Comparing `zenoml-0.4.6/pyproject.toml` & `zenoml-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zenoml"
-version = "0.4.6"
+version = "0.4.7"
 description = "Interactive Evaluation Framework for Machine Learning"
 license = "MIT"
 authors = ["Ángel Alexander Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/zeno-ml/zeno"
 homepage = "https://zenoml.com"
 keywords = ["ml", "testing", "evaluation", "machine learning", "ai"]
```

### Comparing `zenoml-0.4.6/zeno/api.py` & `zenoml-0.4.7/zeno/api.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/backend.py` & `zenoml-0.4.7/zeno/backend.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/classes/base.py` & `zenoml-0.4.7/zeno/classes/base.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/classes/classes.py` & `zenoml-0.4.7/zeno/classes/classes.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/classes/metadata.py` & `zenoml-0.4.7/zeno/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/classes/report.py` & `zenoml-0.4.7/zeno/classes/report.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/classes/slice.py` & `zenoml-0.4.7/zeno/classes/slice.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/.DS_Store` & `zenoml-0.4.7/zeno/frontend/.DS_Store`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/assets/main.5a7a7111.js` & `zenoml-0.4.7/zeno/frontend/build/assets/main.5a7a7111.js`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/assets/main.6757dad9.css` & `zenoml-0.4.7/zeno/frontend/build/assets/main.6757dad9.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/favicon.png` & `zenoml-0.4.7/zeno/frontend/build/favicon.png`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/global.css` & `zenoml-0.4.7/zeno/frontend/build/global.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/smui.css` & `zenoml-0.4.7/zeno/frontend/build/smui.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/build/zeno.png` & `zenoml-0.4.7/zeno/frontend/build/zeno.png`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/index.html` & `zenoml-0.4.7/zeno/frontend/index.html`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/frontend/index_og.html` & `zenoml-0.4.7/zeno/frontend/index_og.html`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/processing/data_processing.py` & `zenoml-0.4.7/zeno/processing/data_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/processing/filtering.py` & `zenoml-0.4.7/zeno/processing/filtering.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/processing/histogram_processing.py` & `zenoml-0.4.7/zeno/processing/histogram_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/processing/projection_processing.py` & `zenoml-0.4.7/zeno/processing/projection_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/runner.py` & `zenoml-0.4.7/zeno/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     else:
         zeno(sys.argv[1])
 
 
 def run_zeno(params: ZenoParameters):
     zeno = ZenoBackend(params)
     app = get_server(zeno)
+
     zeno.start_processing()
 
     print(
         "\n\033[1mZeno\033[0m running on http://{}:{}\n".format(
             params.host, params.port
         )
     )
```

### Comparing `zenoml-0.4.6/zeno/server.py` & `zenoml-0.4.7/zeno/server.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/setup.py` & `zenoml-0.4.7/zeno/setup.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/zeno/util.py` & `zenoml-0.4.7/zeno/util.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.6/PKG-INFO` & `zenoml-0.4.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenoml
-Version: 0.4.6
+Version: 0.4.7
 Summary: Interactive Evaluation Framework for Machine Learning
 Home-page: https://zenoml.com
 License: MIT
 Keywords: ml,testing,evaluation,machine learning,ai
 Author: Ángel Alexander Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.8.1,<=3.11
@@ -42,18 +42,19 @@
 It combines a **Python API** with an **interactive UI** to allow users to discover, explore, and analyze the performance of their models across diverse use cases.
 Zeno can be used for any data type or task with [modular views](https://zenoml.com/docs/views/) for everything from object detection to audio transcription.
 
 
 ### Demos
 
 
-| **Image Classification**  | **Audio Transcription** | **Image Generation** | **Sensor Data Exploration** |
-|:-------------:|:-------------:|:-------------:|:-------------:|
-| CIFAR-10  | Speech Accent Archive | DiffusionDB | MotionSense |
-|[![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://image-example.zenoml.com/)| [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://audio-example.zenoml.com/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-diffusiondb.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://imu-example.zenoml.com/) |
+| **Image Classification**  | **Audio Transcription** | **Image Generation** | **Dataset Chatbot** | **Sensor Classification**
+|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
+| Imagenette  | Speech Accent Archive | DiffusionDB | LangChain + Notion | MotionSense
+|[![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imagenette.hf.space/)| [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-audio-transcription.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-diffusiondb.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-langchain-qa.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imu-classification.hf.space)
+| [code](https://huggingface.co/spaces/zeno-ml/imagenette/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/diffusiondb/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/imu-classification/tree/main) |
 
 <br /> 
 
 https://user-images.githubusercontent.com/4563691/220689691-1ad7c184-02db-4615-b5ac-f52b8d5b8ea3.mp4
 
 ## Quickstart
```

