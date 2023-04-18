# Comparing `tmp/metisse-0.0.5.tar.gz` & `tmp/metisse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\metisse-0.0.5.tar", last modified: Mon Apr 17 10:41:33 2023, max compression
+gzip compressed data, was "dist\metisse-0.0.6.tar", last modified: Tue Apr 18 02:34:46 2023, max compression
```

## Comparing `metisse-0.0.5.tar` & `metisse-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.318678 metisse-0.0.5/
--rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3220 2023-04-17 10:41:33.317681 metisse-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2760 2023-04-17 10:35:51.000000 metisse-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.271803 metisse-0.0.5/metisse/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.283796 metisse-0.0.5/metisse/clients/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.285765 metisse-0.0.5/metisse/clients/android/
--rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.5/metisse/clients/android/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.5/metisse/clients/android/adb.py
--rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.287763 metisse-0.0.5/metisse/clients/ios/
--rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/clients/ios/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/clients/ios/wda.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.289755 metisse-0.0.5/metisse/example/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.257840 metisse-0.0.5/metisse/example/example_data/
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.291751 metisse-0.0.5/metisse/example/example_data/icon/
--rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/icon/example_template_face.png
--rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/icon/example_template_hand.png
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.292747 metisse-0.0.5/metisse/example/example_data/temp_image/
--rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/temp_image/tmp0.png
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.308705 metisse-0.0.5/metisse/example/example_data/ui/
--rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/ui/gui_settings.py
--rw-rw-rw-   0        0        0    16964 2023-04-17 10:34:42.000000 metisse-0.0.5/metisse/example/example_data/ui/script_gui.py
--rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_main.ui
--rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_main_ui.py
--rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub.ui
--rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub2.ui
--rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
--rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub3.ui
--rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
--rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
--rw-rw-rw-   0        0        0     7076 2023-04-17 10:04:33.000000 metisse-0.0.5/metisse/example/generate_example.py
--rw-rw-rw-   0        0        0    22532 2023-04-17 10:04:58.000000 metisse-0.0.5/metisse/metisse.py
--rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/params.py
--rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/settings.py
--rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/template_metis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.316684 metisse-0.0.5/metisse/utils/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/utils/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/utils/image_recognition.py
--rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.5/metisse/utils/metisse_log.py
--rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.5/metisse/utils/metisse_path.py
--rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/utils/opencv_utils.py
--rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.5/metisse/utils/ui_client.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:41:33.280779 metisse-0.0.5/metisse.egg-info/
--rw-rw-rw-   0        0        0     3220 2023-04-17 10:41:33.000000 metisse-0.0.5/metisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-04-17 10:41:33.000000 metisse-0.0.5/metisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:41:33.000000 metisse-0.0.5/metisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 10:41:33.000000 metisse-0.0.5/metisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:41:33.000000 metisse-0.0.5/metisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:41:33.318678 metisse-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1018 2023-04-17 10:37:30.000000 metisse-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.163861 metisse-0.0.6/
+-rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4519 2023-04-18 02:34:46.163861 metisse-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4005 2023-04-18 02:19:32.000000 metisse-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:45.982755 metisse-0.0.6/metisse/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.012673 metisse-0.0.6/metisse/clients/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.025609 metisse-0.0.6/metisse/clients/android/
+-rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/clients/android/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/clients/android/adb.py
+-rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.038604 metisse-0.0.6/metisse/clients/ios/
+-rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/ios/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/ios/wda.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.047583 metisse-0.0.6/metisse/example/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:45.943828 metisse-0.0.6/metisse/example/example_data/
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.050543 metisse-0.0.6/metisse/example/example_data/icon/
+-rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/icon/example_template_face.png
+-rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/icon/example_template_hand.png
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.053535 metisse-0.0.6/metisse/example/example_data/temp_image/
+-rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/temp_image/tmp0.png
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.126064 metisse-0.0.6/metisse/example/example_data/ui/
+-rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/gui_settings.py
+-rw-rw-rw-   0        0        0    16964 2023-04-17 10:34:42.000000 metisse-0.0.6/metisse/example/example_data/ui/script_gui.py
+-rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main.ui
+-rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main_ui.py
+-rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub.ui
+-rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2.ui
+-rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
+-rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3.ui
+-rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
+-rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
+-rw-rw-rw-   0        0        0     7076 2023-04-17 10:04:33.000000 metisse-0.0.6/metisse/example/generate_example.py
+-rw-rw-rw-   0        0        0    22532 2023-04-17 10:04:58.000000 metisse-0.0.6/metisse/metisse.py
+-rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/params.py
+-rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/settings.py
+-rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/template_metis.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.161867 metisse-0.0.6/metisse/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/image_recognition.py
+-rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/utils/metisse_log.py
+-rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.6/metisse/utils/metisse_path.py
+-rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/opencv_utils.py
+-rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/ui_client.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.005692 metisse-0.0.6/metisse.egg-info/
+-rw-rw-rw-   0        0        0     4519 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:34:46.163861 metisse-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-04-18 02:30:34.000000 metisse-0.0.6/setup.py
```

### Comparing `metisse-0.0.5/LICENSE` & `metisse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/PKG-INFO` & `metisse-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: metisse
-Version: 0.0.5
+Version: 0.0.6
 Summary: A versatile and automated testing framework for games and apps on Android and iOS platforms
 Author: Henry Chen
 Author-email: weekand7@gmail.com
 License: Apache License 2.0
+Keywords: automation,automated-test,game,android,ios
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Metisse
@@ -28,15 +29,47 @@
 ## Installation
 
 To install Metisse, run the following command in your terminal:
 
 ```bash
 pip install metisse
 ```
-Usage
+
+### Additional Requirements
+
+#### Android Devices
+
+1. Enable Developer Mode on your Android device.
+2. Turn on USB Debugging (adb) on your Android device.
+3. Install Android Debug Bridge (adb) on your computer.
+4. Add adb to your system path.
+
+#### iOS Devices
+
+1. Install Appium/WebDriverAgent on your ios device.
+
+### Enabling Developer Mode and USB Debugging (adb) on Android Devices
+
+Follow these steps to enable Developer Mode and USB Debugging on your Android device:
+
+1. Open the Settings app on your Android device.
+2. Scroll down and tap "About phone" or "About device."
+3. Find the "Build number" or "Software version" and tap it 7 times. You will see a message that you are now a developer.
+4. Go back to the main Settings menu and tap "Developer options" (it should be visible now).
+5. Enable "USB Debugging."
+
+### Android Debug Bridge (adb) Installation and Configuration
+
+Follow these steps to install and configure adb:
+
+1. Download the Android SDK Platform Tools from the following link: https://developer.android.com/studio/releases/platform-tools
+2. Extract the downloaded zip file to a location of your choice.
+3. Add the extracted folder to your system's PATH variable.
+
+### Usage
 Here's a simple example demonstrating how to use Metisse for image recognition and user interaction:
 
 python
 Copy code
 ```bash
 from metisse.metisse import MetisseClass
 from metisse.params import ImageRecognitionParams, SaveParams
@@ -47,15 +80,15 @@
             self,
             device_id=device_id,
             relatively_path=relatively_path,
             pyqt6_ui_label=pyqt6_ui_label,
             os_environment=os_environment,
         )
 
-    def __call__(self):
+    def __call__(self, *args, **kwargs):
         # Your custom script implementation goes here
 
 if __name__ == "__main__":
     script_obj = script_example("01234567(test_uid)", None, None, "android")
     script_obj()
 ```
```

### Comparing `metisse-0.0.5/metisse/clients/android/adb.py` & `metisse-0.0.6/metisse/clients/android/adb.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/clients/client.py` & `metisse-0.0.6/metisse/clients/client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/clients/ios/wda.py` & `metisse-0.0.6/metisse/clients/ios/wda.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/icon/example_template_face.png` & `metisse-0.0.6/metisse/example/example_data/icon/example_template_face.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/icon/example_template_hand.png` & `metisse-0.0.6/metisse/example/example_data/icon/example_template_hand.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/temp_image/tmp0.png` & `metisse-0.0.6/metisse/example/example_data/temp_image/tmp0.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/script_gui.py` & `metisse-0.0.6/metisse/example/example_data/ui/script_gui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_main.ui` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_main_ui.py` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub.ui` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub2.ui` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub3.ui` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/example_data/ui/universal_script_gui_sub_ui.py` & `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/example/generate_example.py` & `metisse-0.0.6/metisse/example/generate_example.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/metisse.py` & `metisse-0.0.6/metisse/metisse.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/params.py` & `metisse-0.0.6/metisse/params.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/template_metis.py` & `metisse-0.0.6/metisse/template_metis.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/utils/image_recognition.py` & `metisse-0.0.6/metisse/utils/image_recognition.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/utils/metisse_log.py` & `metisse-0.0.6/metisse/utils/metisse_log.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/utils/metisse_path.py` & `metisse-0.0.6/metisse/utils/metisse_path.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/utils/opencv_utils.py` & `metisse-0.0.6/metisse/utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse/utils/ui_client.py` & `metisse-0.0.6/metisse/utils/ui_client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/metisse.egg-info/PKG-INFO` & `metisse-0.0.6/metisse.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: metisse
-Version: 0.0.5
+Version: 0.0.6
 Summary: A versatile and automated testing framework for games and apps on Android and iOS platforms
 Author: Henry Chen
 Author-email: weekand7@gmail.com
 License: Apache License 2.0
+Keywords: automation,automated-test,game,android,ios
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Metisse
@@ -28,15 +29,47 @@
 ## Installation
 
 To install Metisse, run the following command in your terminal:
 
 ```bash
 pip install metisse
 ```
-Usage
+
+### Additional Requirements
+
+#### Android Devices
+
+1. Enable Developer Mode on your Android device.
+2. Turn on USB Debugging (adb) on your Android device.
+3. Install Android Debug Bridge (adb) on your computer.
+4. Add adb to your system path.
+
+#### iOS Devices
+
+1. Install Appium/WebDriverAgent on your ios device.
+
+### Enabling Developer Mode and USB Debugging (adb) on Android Devices
+
+Follow these steps to enable Developer Mode and USB Debugging on your Android device:
+
+1. Open the Settings app on your Android device.
+2. Scroll down and tap "About phone" or "About device."
+3. Find the "Build number" or "Software version" and tap it 7 times. You will see a message that you are now a developer.
+4. Go back to the main Settings menu and tap "Developer options" (it should be visible now).
+5. Enable "USB Debugging."
+
+### Android Debug Bridge (adb) Installation and Configuration
+
+Follow these steps to install and configure adb:
+
+1. Download the Android SDK Platform Tools from the following link: https://developer.android.com/studio/releases/platform-tools
+2. Extract the downloaded zip file to a location of your choice.
+3. Add the extracted folder to your system's PATH variable.
+
+### Usage
 Here's a simple example demonstrating how to use Metisse for image recognition and user interaction:
 
 python
 Copy code
 ```bash
 from metisse.metisse import MetisseClass
 from metisse.params import ImageRecognitionParams, SaveParams
@@ -47,15 +80,15 @@
             self,
             device_id=device_id,
             relatively_path=relatively_path,
             pyqt6_ui_label=pyqt6_ui_label,
             os_environment=os_environment,
         )
 
-    def __call__(self):
+    def __call__(self, *args, **kwargs):
         # Your custom script implementation goes here
 
 if __name__ == "__main__":
     script_obj = script_example("01234567(test_uid)", None, None, "android")
     script_obj()
 ```
```

### Comparing `metisse-0.0.5/metisse.egg-info/SOURCES.txt` & `metisse-0.0.6/metisse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metisse-0.0.5/setup.py` & `metisse-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='metisse',
-    version="0.0.5",
+    version="0.0.6",
     description="A versatile and automated testing framework for games and apps on Android and iOS platforms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Henry Chen',
     author_email='weekand7@gmail.com',
     license='Apache License 2.0',
+    keywords=['automation', 'automated-test', 'game', 'android', 'ios'],
     packages=find_packages(exclude=['unit_tests', 'unit_tests.*']),
     package_data={
         'metisse': ['example/example_data/**/*'],
     },
     install_requires=[
         'facebook_wda>=1.3.3',
         'numpy>=1.17.3',
         'opencv_python>=4.5.1.48',
         'Pillow>=3.4.0',
         'PyQt6>=6.0.0',
         'dill>=0.3.1.1',
+        'tidevice>=0.9.12',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 )
```

