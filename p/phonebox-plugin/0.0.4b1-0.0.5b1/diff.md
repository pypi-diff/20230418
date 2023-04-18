# Comparing `tmp/phonebox_plugin-0.0.4b1.tar.gz` & `tmp/phonebox_plugin-0.0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonebox_plugin-0.0.4b1.tar", last modified: Thu Jun  9 10:46:38 2022, max compression
+gzip compressed data, was "phonebox_plugin-0.0.5b1.tar", last modified: Tue Apr 18 18:52:08 2023, max compression
```

## Comparing `phonebox_plugin-0.0.4b1.tar` & `phonebox_plugin-0.0.5b1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.066380 phonebox_plugin-0.0.4b1/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1066 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/LICENSE
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      123 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/MANIFEST.in
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     5569 2022-06-09 10:46:38.065718 phonebox_plugin-0.0.4b1/PKG-INFO
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4870 2021-11-29 21:23:12.000000 phonebox_plugin-0.0.4b1/README.md
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.003274 phonebox_plugin-0.0.4b1/phonebox_plugin/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      493 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      205 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/admin.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.014484 phonebox_plugin-0.0.4b1/phonebox_plugin/api/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       35 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/api/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      546 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/api/nested_serializers.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1148 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/api/serializers.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      256 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/api/urls.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      780 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/api/views.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      556 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/choices.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     3293 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/filters.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)    10187 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/forms.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.028375 phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1982 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/0001_initial.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      376 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/0002_alter_number_id.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2337 2022-02-09 07:26:36.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/0003_voicecircuit.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)        0 2021-09-21 14:31:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/__init__.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4882 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/models.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      331 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/navigation.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1402 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/tables.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.031569 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6148 2021-11-22 16:21:02.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/.DS_Store
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.063572 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      588 2021-11-25 15:49:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_number.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      588 2022-06-08 18:09:55.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4360 2021-11-29 08:57:28.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     5176 2022-06-08 18:16:15.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      734 2022-06-09 10:06:12.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/list_view.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1910 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4327 2021-10-01 18:47:55.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/number.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4466 2022-02-06 20:40:53.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     3263 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      254 2022-02-06 20:40:07.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/tags_panel.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6570 2021-11-30 11:25:05.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     6980 2022-02-06 20:40:32.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)      775 2021-11-29 21:06:14.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     2035 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1595 2022-06-08 14:24:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/urls.py
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     4157 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/phonebox_plugin/views.py
-drwxr-xr-x   0 IKorotchenkov   (501) staff       (20)        0 2022-06-09 10:46:38.007603 phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     5569 2022-06-09 10:46:37.000000 phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/PKG-INFO
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1711 2022-06-09 10:46:37.000000 phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)        1 2022-06-09 10:46:37.000000 phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       16 2022-06-09 10:46:37.000000 phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/top_level.txt
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)       38 2022-06-09 10:46:38.066592 phonebox_plugin-0.0.4b1/setup.cfg
--rw-r--r--   0 IKorotchenkov   (501) staff       (20)     1107 2022-06-09 10:46:13.000000 phonebox_plugin-0.0.4b1/setup.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.091702 phonebox_plugin-0.0.5b1/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1066 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/LICENSE
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      123 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/MANIFEST.in
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-04-18 18:52:08.091521 phonebox_plugin-0.0.5b1/PKG-INFO
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4870 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/README.md
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.085919 phonebox_plugin-0.0.5b1/phonebox_plugin/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      493 2023-04-18 18:35:42.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      205 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/admin.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.087617 phonebox_plugin-0.0.5b1/phonebox_plugin/api/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       35 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      707 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/nested_serializers.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1148 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/serializers.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      256 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/urls.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      780 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/api/views.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      556 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/choices.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3293 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/filters.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)    10187 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/forms.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.088544 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1982 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0001_initial.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      376 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0002_alter_number_id.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2337 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0003_voicecircuit.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/__init__.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4882 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/models.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      331 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/navigation.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1402 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/tables.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.082665 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.091305 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      588 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4360 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5176 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      734 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1913 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1910 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4327 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4466 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     3263 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      254 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/tags_panel.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6570 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     6980 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)      775 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2038 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     2035 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1595 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/urls.py
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     4507 2023-04-18 17:33:00.000000 phonebox_plugin-0.0.5b1/phonebox_plugin/views.py
+drwxr-xr-x   0 igorkorotchenkov   (501) staff       (20)        0 2023-04-18 18:52:08.086585 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     5549 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1811 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)        1 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       16 2023-04-18 18:52:08.000000 phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/top_level.txt
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)       38 2023-04-18 18:52:08.091748 phonebox_plugin-0.0.5b1/setup.cfg
+-rw-r--r--   0 igorkorotchenkov   (501) staff       (20)     1107 2023-04-18 18:35:25.000000 phonebox_plugin-0.0.5b1/setup.py
```

### Comparing `phonebox_plugin-0.0.4b1/LICENSE` & `phonebox_plugin-0.0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/PKG-INFO` & `phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: phonebox_plugin
-Version: 0.0.4b1
+Name: phonebox-plugin
+Version: 0.0.5b1
 Summary: A phone numbers management plugin for NetBox.
 Home-page: https://github.com/iDebugAll/phonebox-plugin.git
+Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
-Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.4-beta.1.tar.gz
 Keywords: netbox,netbox-plugin,plugin
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -80,15 +79,15 @@
 General installation steps and considerations follow the [official guidelines](https://netbox.readthedocs.io/en/stable/plugins/).
 
 ### Package Installation from PyPi
 
 Assuming you use a Virtual Environment for Netbox:
 ```
 $ source /opt/netbox/venv/bin/activate
-(venv) $ pip3 install phonebox_plugin
+(venv) $ pip3 install phonebox-plugin
 ```
 
 ### Package Installation from Source Code
 The source code is available on [GitHub](https://github.com/iDebugAll/phonebox_plugin).<br/>
 Download and install the package. Assuming you use a Virtual Environment for Netbox:
 ```
 $ git clone https://github.com/iDebugAll/phonebox_plugin
@@ -151,9 +150,7 @@
 Rebuild the running docker containers:
 ```
 $ cd netbox-docker
 $ docker-compose down
 $ docker-compose up -d
 ```
 Netbox Community Docker setup performs static files collection on every startup. No manual actions required.
-
-
```

### Comparing `phonebox_plugin-0.0.4b1/README.md` & `phonebox_plugin-0.0.5b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 General installation steps and considerations follow the [official guidelines](https://netbox.readthedocs.io/en/stable/plugins/).
 
 ### Package Installation from PyPi
 
 Assuming you use a Virtual Environment for Netbox:
 ```
 $ source /opt/netbox/venv/bin/activate
-(venv) $ pip3 install phonebox_plugin
+(venv) $ pip3 install phonebox-plugin
 ```
 
 ### Package Installation from Source Code
 The source code is available on [GitHub](https://github.com/iDebugAll/phonebox_plugin).<br/>
 Download and install the package. Assuming you use a Virtual Environment for Netbox:
 ```
 $ git clone https://github.com/iDebugAll/phonebox_plugin
```

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/api/nested_serializers.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/api/nested_serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from rest_framework import serializers
 from phonebox_plugin import models
-from netbox.api import WritableNestedSerializer
+
+try:
+    from netbox.api import ChoiceField, WritableNestedSerializer
+except ImportError:
+    from netbox.api.fields import ChoiceField
+    from netbox.api.serializers.nested import WritableNestedSerializer
+
 from tenancy.api.nested_serializers import NestedTenantSerializer
 
 __all__ = ["NestedNumberSerializer", ]
 
 
 class NestedNumberSerializer(WritableNestedSerializer):
```

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/api/serializers.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/api/views.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/choices.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/choices.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/filters.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/filters.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/forms.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/0001_initial.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/migrations/0003_voicecircuit.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/migrations/0003_voicecircuit.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/models.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/models.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/tables.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_number.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/list_view.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/number.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/number_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/obj_table.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html` & `phonebox_plugin-0.0.5b1/phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/urls.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin/views.py` & `phonebox_plugin-0.0.5b1/phonebox_plugin/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 
 class NumberListView(generic.ObjectListView):
     queryset = Number.objects.all()
     filterset = filters.NumberFilterSet
     filterset_form = forms.NumberFilterForm
     table = tables.NumberTable
-    if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
+    if NETBOX_CURRENT_VERSION >= version.parse("3.0") and NETBOX_CURRENT_VERSION < version.parse("3.4"):
         template_name = "phonebox_plugin/list_view_3.x.html"
+    elif NETBOX_CURRENT_VERSION >= version.parse("3.4"):
+        template_name = "phonebox_plugin/list_view_3.4.html"
     else:
         template_name = "phonebox_plugin/list_view.html"
 
 
 class NumberView(generic.ObjectView):
     queryset = Number.objects.prefetch_related('tenant')
     if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
@@ -72,16 +74,18 @@
 
 
 class VoiceCircuitListView(generic.ObjectListView):
     queryset = VoiceCircuit.objects.all()
     filterset = filters.VoiceCircuitFilterSet
     filterset_form = forms.VoiceCircuitFilterForm
     table = tables.VoiceCircuitTable
-    if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
+    if NETBOX_CURRENT_VERSION >= version.parse("3.0") and NETBOX_CURRENT_VERSION < version.parse("3.4"):
         template_name = "phonebox_plugin/voice_circuit_list_view_3.x.html"
+    elif NETBOX_CURRENT_VERSION >= version.parse("3.4"):
+        template_name = "phonebox_plugin/voice_circuit_list_view_3.4.html"
     else:
         template_name = "phonebox_plugin/voice_circuit_list_view.html"
 
 
 class VoiceCircuitView(generic.ObjectView):
     queryset = VoiceCircuit.objects.prefetch_related('tenant')
     if NETBOX_CURRENT_VERSION >= version.parse("3.0"):
```

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/PKG-INFO` & `phonebox_plugin-0.0.5b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: phonebox-plugin
-Version: 0.0.4b1
+Name: phonebox_plugin
+Version: 0.0.5b1
 Summary: A phone numbers management plugin for NetBox.
 Home-page: https://github.com/iDebugAll/phonebox-plugin.git
+Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz
 Author: Igor Korotchenkov
 Author-email: iDebugAll@gmail.com
 License: MIT
-Download-URL: https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.4-beta.1.tar.gz
 Keywords: netbox,netbox-plugin,plugin
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -80,15 +79,15 @@
 General installation steps and considerations follow the [official guidelines](https://netbox.readthedocs.io/en/stable/plugins/).
 
 ### Package Installation from PyPi
 
 Assuming you use a Virtual Environment for Netbox:
 ```
 $ source /opt/netbox/venv/bin/activate
-(venv) $ pip3 install phonebox_plugin
+(venv) $ pip3 install phonebox-plugin
 ```
 
 ### Package Installation from Source Code
 The source code is available on [GitHub](https://github.com/iDebugAll/phonebox_plugin).<br/>
 Download and install the package. Assuming you use a Virtual Environment for Netbox:
 ```
 $ git clone https://github.com/iDebugAll/phonebox_plugin
@@ -151,9 +150,7 @@
 Rebuild the running docker containers:
 ```
 $ cd netbox-docker
 $ docker-compose down
 $ docker-compose up -d
 ```
 Netbox Community Docker setup performs static files collection on every startup. No manual actions required.
-
-
```

### Comparing `phonebox_plugin-0.0.4b1/phonebox_plugin.egg-info/SOURCES.txt` & `phonebox_plugin-0.0.5b1/phonebox_plugin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 phonebox_plugin/api/serializers.py
 phonebox_plugin/api/urls.py
 phonebox_plugin/api/views.py
 phonebox_plugin/migrations/0001_initial.py
 phonebox_plugin/migrations/0002_alter_number_id.py
 phonebox_plugin/migrations/0003_voicecircuit.py
 phonebox_plugin/migrations/__init__.py
-phonebox_plugin/templates/.DS_Store
 phonebox_plugin/templates/phonebox_plugin/add_number.html
 phonebox_plugin/templates/phonebox_plugin/add_number_3.x.html
 phonebox_plugin/templates/phonebox_plugin/add_voice_circuit.html
 phonebox_plugin/templates/phonebox_plugin/add_voice_circuit_3.x.html
 phonebox_plugin/templates/phonebox_plugin/list_view.html
+phonebox_plugin/templates/phonebox_plugin/list_view_3.4.html
 phonebox_plugin/templates/phonebox_plugin/list_view_3.x.html
 phonebox_plugin/templates/phonebox_plugin/number.html
 phonebox_plugin/templates/phonebox_plugin/number_3.x.html
 phonebox_plugin/templates/phonebox_plugin/obj_table.html
 phonebox_plugin/templates/phonebox_plugin/tags_panel.html
 phonebox_plugin/templates/phonebox_plugin/voice_circuit.html
 phonebox_plugin/templates/phonebox_plugin/voice_circuit_3.x.html
 phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view.html
+phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.4.html
 phonebox_plugin/templates/phonebox_plugin/voice_circuit_list_view_3.x.html
```

### Comparing `phonebox_plugin-0.0.4b1/setup.py` & `phonebox_plugin-0.0.5b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from os import path
 top_level_directory = path.abspath(path.dirname(__file__))
 with open(path.join(top_level_directory, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='phonebox_plugin',
-    version='v0.0.4-beta.1',
+    version='v0.0.5-beta.1',
     url='https://github.com/iDebugAll/phonebox-plugin.git',
-    download_url='https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.4-beta.1.tar.gz',
+    download_url='https://github.com/iDebugAll/phonebox-plugin/archive/v0.0.5-beta.1.tar.gz',
     description='A phone numbers management plugin for NetBox.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Igor Korotchenkov',
     author_email='iDebugAll@gmail.com',
     install_requires=[],
     packages=find_packages(),
```

