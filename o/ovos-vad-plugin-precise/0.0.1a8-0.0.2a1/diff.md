# Comparing `tmp/ovos-vad-plugin-precise-0.0.1a8.tar.gz` & `tmp/ovos-vad-plugin-precise-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-vad-plugin-precise-0.0.1a8.tar", last modified: Tue Apr 18 03:54:57 2023, max compression
+gzip compressed data, was "ovos-vad-plugin-precise-0.0.2a1.tar", last modified: Tue Apr 18 15:49:48 2023, max compression
```

## Comparing `ovos-vad-plugin-precise-0.0.1a8.tar` & `ovos-vad-plugin-precise-0.0.2a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:54:57.250213 ovos-vad-plugin-precise-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 03:54:57.246213 ovos-vad-plugin-precise-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:54:57.246213 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/vad.tflite
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 03:54:51.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:54:57.246213 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 03:54:57.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:54:56.000000 ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:54:57.250213 ovos-vad-plugin-precise-0.0.1a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-04-18 03:54:48.000000 ovos-vad-plugin-precise-0.0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:49:48.121241 ovos-vad-plugin-precise-0.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 15:49:48.121241 ovos-vad-plugin-precise-0.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:49:48.121241 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/vad.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 15:49:42.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:49:48.121241 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 15:49:48.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:49:47.000000 ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:49:48.121241 ovos-vad-plugin-precise-0.0.2a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-04-18 15:49:38.000000 ovos-vad-plugin-precise-0.0.2a1/setup.py
```

### Comparing `ovos-vad-plugin-precise-0.0.1a8/LICENSE.md` & `ovos-vad-plugin-precise-0.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a8/PKG-INFO` & `ovos-vad-plugin-precise-0.0.2a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-precise
-Version: 0.0.1a8
+Version: 0.0.2a1
 Summary: precise VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-precise
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-precise-0.0.1a8/README.md` & `ovos-vad-plugin-precise-0.0.2a1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,61 +6,96 @@
 
 see scripts in ./training folder
 
 `Data: <TrainData wake_words=87243 not_wake_words=26209 test_wake_words=62258 test_not_wake_words=17654>`
 
 datasets used:
 - https://www.kaggle.com/datasets/mozillaorg/common-voice
+- https://www.kaggle.com/datasets/ogechukwu/voice
 - https://github.com/karolpiczak/ESC-50
 - https://urbansounddataset.weebly.com/urbansound8k.html
 - FSD50K (eval) - https://zenodo.org/record/4060432
 - https://pdsounds.tuxfamily.org/
 - https://paperswithcode.com/dataset/nar
 - https://www.csc.kth.se/~jastork/downloads/building_106_kitchen.zip
 - https://ai.googleblog.com/2017/08/launching-speech-commands-dataset.html
 - https://github.com/OpenVoiceOS/ovos-ww-community-dataset
 - https://www.kaggle.com/datasets/aanhari/alexa-dataset
 - https://www.kaggle.com/datasets/mohamedhamadacs/khwarizmi-wake-word
 - https://research.google.com/audioset/dataset/index.html (via https://github.com/Jeremias-V/audioset-processing/tree/fix-downloads)
 - some private wake word data
 
-test set
+
+test set (threshold of 0.5)
+
+```
+=== Counts ===
+False Positives: 223
+True Negatives: 17430
+False Negatives: 6847
+True Positives: 55411
+
+=== Summary ===
+72841 out of 79911
+91.15%
+
+1.26% false positives
+11.00% false negatives
+```
+
+test set (threshold of 0.3)
 
 ```
 === Counts ===
-False Positives: 512
-True Negatives: 13035
-False Negatives: 2512
-True Positives: 59541
+False Positives: 745
+True Negatives: 16908
+False Negatives: 3429
+True Positives: 58829
 
 === Summary ===
-72576 out of 75600
-96.00%
+75737 out of 79911
+94.78%
 
-3.78% false positives
-4.05% false negatives
+4.22% false positives
+5.51% false negatives
 ```
 
-train set
+train set (threshold of 0.5)
 
 ```
 === Counts ===
-False Positives: 533
-True Negatives: 19791
-False Negatives: 3372
-True Positives: 83206
+False Positives: 164
+True Negatives: 26044
+False Negatives: 9424
+True Positives: 77819
 
 === Summary ===
-102997 out of 106902
-96.35%
+103863 out of 113451
+91.55%
+
+0.63% false positives
+10.80% false negatives
+```
+
+train set (threshold of 0.3)
 
-2.62% false positives
-3.89% false negatives
 ```
+=== Counts ===
+False Positives: 932
+True Negatives: 25276
+False Negatives: 4467
+True Positives: 82776
+
+=== Summary ===
+108052 out of 113451
+95.24%
 
+3.56% false positives
+5.12% false negatives
+```
 
 # Logs
 
 some quick logs taken with ovos-dinkum-listener, threshold can be tuned for your microphone
 
 a usb pseye mic was used for testing
```

### Comparing `ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/__init__.py` & `ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from precise_lite_runner.runner import Listener
 
 
 class PreciseVAD(VADEngine):
     def __init__(self, config=None, sample_rate=None):
         super().__init__(config, sample_rate)
         model = self.config.get("model") or join(dirname(__file__), "vad.tflite")
-        self.vad_threshold = self.config.get("threshold", 0.5)
+        self.vad_threshold = self.config.get("threshold", 0.35)
         self.debug = self.config.get("debug", False)
         self.vad = Listener(model)
 
     def is_silence(self, chunk):
         # return True or False
         prob = self.vad.get_prediction(chunk)
         if self.debug:
```

### Comparing `ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise/vad.tflite` & `ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise/vad.tflite`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a8/ovos_vad_plugin_precise.egg-info/PKG-INFO` & `ovos-vad-plugin-precise-0.0.2a1/ovos_vad_plugin_precise.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-precise
-Version: 0.0.1a8
+Version: 0.0.2a1
 Summary: precise VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-precise
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-precise-0.0.1a8/setup.py` & `ovos-vad-plugin-precise-0.0.2a1/setup.py`

 * *Files identical despite different names*

