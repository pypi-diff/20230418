# Comparing `tmp/pysigma_backend_microsoft365defender-0.1.0.tar.gz` & `tmp/pysigma_backend_microsoft365defender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_microsoft365defender-0.1.0.tar", max compression
+gzip compressed data, was "pysigma_backend_microsoft365defender-0.1.2.tar", max compression
```

## Comparing `pysigma_backend_microsoft365defender-0.1.0.tar` & `pysigma_backend_microsoft365defender-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7653 2023-03-28 13:18:46.880193 pysigma_backend_microsoft365defender-0.1.0/LICENSE
--rw-r--r--   0        0        0      626 2023-03-28 13:18:46.880193 pysigma_backend_microsoft365defender-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      407 2023-03-28 13:18:46.880193 pysigma_backend_microsoft365defender-0.1.0/sigma/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    11533 2023-03-28 13:18:46.884193 pysigma_backend_microsoft365defender-0.1.0/sigma/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      315 2023-03-28 13:18:46.884193 pysigma_backend_microsoft365defender-0.1.0/sigma/pipelines/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    29088 2023-03-28 13:18:46.884193 pysigma_backend_microsoft365defender-0.1.0/sigma/pipelines/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/LICENSE
+-rw-r--r--   0        0        0      626 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    11533 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      315 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    29236 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.1.2/PKG-INFO
```

### Comparing `pysigma_backend_microsoft365defender-0.1.0/LICENSE` & `pysigma_backend_microsoft365defender-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.1.0/pyproject.toml` & `pysigma_backend_microsoft365defender-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-microsoft365defender"
-version = "0.1.0"
+version = "0.1.2"
 description = "pySigma Microsoft 365 Defender backend"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/AttackIQ/pySigma-backend-microsoft365defender"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_microsoft365defender-0.1.0/sigma/backends/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/microsoft365defender.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.1.0/sigma/pipelines/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/microsoft365defender.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     logsource_windows_file_change, logsource_windows_file_access, logsource_windows_file_rename, \
     logsource_windows_registry_set, logsource_windows_registry_add, logsource_windows_registry_delete, \
     logsource_windows_registry_event, logsource_windows_network_connection
 from sigma.processing.transformations import FieldMappingTransformation, \
     RuleFailureTransformation, ReplaceStringTransformation, SetStateTransformation, DetectionItemTransformation, \
     ValueTransformation, DetectionItemFailureTransformation
 from sigma.processing.conditions import IncludeFieldCondition, \
-    RuleProcessingItemAppliedCondition, ExcludeFieldCondition
+    RuleProcessingItemAppliedCondition, ExcludeFieldCondition, DetectionItemProcessingItemAppliedCondition
 from sigma.conditions import ConditionOR
 from sigma.types import SigmaString, SigmaType
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
 from sigma.rule import SigmaDetectionItem, SigmaDetection
 from collections import defaultdict
 
 
@@ -395,50 +395,50 @@
 ## Exclude any fields already mapped. For example, if process_creation events ProcessId has already
 ## been mapped to the same field name (ProcessId), we don't to remap it to InitiatingProcessId
 generic_field_mappings_proc_item = [ProcessingItem(
     identifier="microsoft_365_defender_fieldmappings_generic",
     transformation=FieldMappingTransformation(
         generic_field_mappings
     ),
-    rule_conditions=[
-        RuleProcessingItemAppliedCondition(f"microsoft_365_defender_fieldmappings_{table_name}")
+    detection_item_conditions=[
+        DetectionItemProcessingItemAppliedCondition(f"microsoft_365_defender_fieldmappings_{table_name}")
         for table_name in table_to_category_mappings.keys()
     ],
-    rule_condition_linking=any,
-    rule_condition_negation=True,
+    detection_item_condition_linking=any,
+    detection_item_condition_negation=True,
 )
 ]
 ## Field Value Replacements ProcessingItems
 replacement_proc_items = [
     # Sysmon uses abbreviations in RegistryKey values, replace with full key names as the DeviceRegistryEvents schema
     # expects them to be
     # Note: Ensure this comes AFTER field mapping renames, as we're specifying DeviceRegistryEvent fields
     #
     # Do this one first, or else the HKLM only one will replace HKLM and mess up the regex
     ProcessingItem(
         identifier="microsoft_365_defender_registry_key_replace_currentcontrolset",
-        transformation=ReplaceStringTransformation(regex=r"((?i)^HKLM\\SYSTEM\\CurrentControlSet)",
+        transformation=ReplaceStringTransformation(regex=r"(?i)(^HKLM\\SYSTEM\\CurrentControlSet)",
                                                    replacement=r"HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet001"),
         field_name_conditions=[IncludeFieldCondition(['RegistryKey', 'PreviousRegistryKey'])]
     ),
     ProcessingItem(
         identifier="microsoft_365_defender_registry_key_replace_hklm",
-        transformation=ReplaceStringTransformation(regex=r"((?i)^HKLM)",
+        transformation=ReplaceStringTransformation(regex=r"(?i)(^HKLM)",
                                                    replacement=r"HKEY_LOCAL_MACHINE"),
         field_name_conditions=[IncludeFieldCondition(['RegistryKey', 'PreviousRegistryKey'])]
     ),
     ProcessingItem(
         identifier="microsoft_365_defender_registry_key_replace_hku",
-        transformation=ReplaceStringTransformation(regex=r"((?i)^HKU)",
+        transformation=ReplaceStringTransformation(regex=r"(?i)(^HKU)",
                                                    replacement=r"HKEY_USERS"),
         field_name_conditions=[IncludeFieldCondition(['RegistryKey', 'PreviousRegistryKey'])]
     ),
     ProcessingItem(
         identifier="microsoft_365_defender_registry_key_replace_hkcr",
-        transformation=ReplaceStringTransformation(regex=r"((?i)^HKCR)",
+        transformation=ReplaceStringTransformation(regex=r"(?i)(^HKCR)",
                                                    replacement=r"HKEY_LOCAL_MACHINE\\CLASSES"),
         field_name_conditions=[IncludeFieldCondition(['RegistryKey', 'PreviousRegistryKey'])]
     ),
     ProcessingItem(
         identifier="microsoft_365_defender_registry_actiontype_value",
         transformation=RegistryActionTypeValueTransformation(),
         field_name_conditions=[IncludeFieldCondition(['ActionType'])]
@@ -475,15 +475,16 @@
         identifier=f"microsoft_365_defender_unsupported_fields_{table_name}",
         transformation=InvalidFieldTransformation(
             f"Please use valid fields for the {table_name} table, or the following fields that have keymappings in this "
             f"pipeline:\n"
             # Combine field mappings for table and generic field mappings dicts, get the unique keys, add the Hashes field, sort it
             f"{', '.join(sorted(set({**query_table_field_mappings[table_name], **generic_field_mappings}.keys()).union({'Hashes'})))}"
         ),
-        field_name_conditions=[ExcludeFieldCondition(fields=table_fields)],
+        field_name_conditions=[
+            ExcludeFieldCondition(fields=table_fields + list(generic_field_mappings.keys()) + ['Hashes'])],
         rule_conditions=[
             category_to_conditions_mappings[rule_category]
             for rule_category in table_to_category_mappings[table_name]
         ],
         rule_condition_linking=any,
     )
     for table_name, table_fields in valid_fields_per_table.items()
```

### Comparing `pysigma_backend_microsoft365defender-0.1.0/PKG-INFO` & `pysigma_backend_microsoft365defender-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-microsoft365defender
-Version: 0.1.0
+Version: 0.1.2
 Summary: pySigma Microsoft 365 Defender backend
 Home-page: https://github.com/AttackIQ/pySigma-backend-microsoft365defender
 License: LGPL-3.0-only
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

