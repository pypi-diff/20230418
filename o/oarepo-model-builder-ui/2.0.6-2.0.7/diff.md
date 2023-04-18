# Comparing `tmp/oarepo-model-builder-ui-2.0.6.tar.gz` & `tmp/oarepo-model-builder-ui-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-2.0.6.tar", last modified: Mon Apr 10 12:04:04 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-2.0.7.tar", last modified: Tue Apr 18 13:57:43 2023, max compression
```

## Comparing `oarepo-model-builder-ui-2.0.6.tar` & `oarepo-model-builder-ui-2.0.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/layout_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 12:04:04.000000 oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:04:04.924389 oarepo-model-builder-ui-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-10 12:01:58.000000 oarepo-model-builder-ui-2.0.6/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.299518 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/layout_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/tests/test_translation.py
```

### Comparing `oarepo-model-builder-ui-2.0.6/PKG-INFO` & `oarepo-model-builder-ui-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.6
+Version: 2.0.7
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.6/README.md` & `oarepo-model-builder-ui-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 import inflect
 
 from oarepo_model_builder.builder import ModelBuilder
 from oarepo_model_builder.builders import process
 from oarepo_model_builder.builders.json_base import JSONBaseBuilder
 from oarepo_model_builder.property_preprocessors import PropertyPreprocessor
+from oarepo_model_builder.invenio.invenio_record_search import get_facet_details
 from oarepo_model_builder.utils.verbose import log
 
 from oarepo_model_builder_ui.config import UI_ITEMS
 
 """
 Will generate:
 metadata: {
@@ -19,15 +20,15 @@
   help: <help.key>
   children: {
     k: child_def
   }, // or 
   child: {
     ...
   }
-}
+
 // invenio_stuff_here
 
 it will be saved to package/model/ui.json
 """
 
 
 class InvenioLayoutBuilder(JSONBaseBuilder):
@@ -65,14 +66,21 @@
                         x.key
                         for x in self.stack
                         if x.schema_element_type == "property" and x.key
                     )
                     + f".{fld}",
                 )
 
+            facets = get_facet_details(
+                self.stack, self.current_model, self.schema, set()
+            )
+
+            if len(facets):
+                ui["facet"] = facets[0]["path"]
+
             self.output.enter(self.stack.top.key, {})
         elif schema_element_type == "properties":
             self.output.enter("children", {})
         elif schema_element_type == "items":
             self.output.enter("child", {})
         else:
             leave = False
```

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/invenio/layout_setup_cfg.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/model_preprocessors/layout_settings.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/layout_settings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui/validation/__init__.py` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.6
+Version: 2.0.7
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 oarepo_model_builder_ui/invenio/layout.py
 oarepo_model_builder_ui/invenio/layout_setup_cfg.py
 oarepo_model_builder_ui/model_preprocessors/__init__.py
 oarepo_model_builder_ui/model_preprocessors/layout_settings.py
 oarepo_model_builder_ui/outputs/i18n.py
 oarepo_model_builder_ui/outputs/layout.py
 oarepo_model_builder_ui/validation/__init__.py
+tests/test_facets.py
 tests/test_translation.py
```

### Comparing `oarepo-model-builder-ui-2.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.6/setup.cfg` & `oarepo-model-builder-ui-2.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 2.0.6
+version = 2.0.7
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

