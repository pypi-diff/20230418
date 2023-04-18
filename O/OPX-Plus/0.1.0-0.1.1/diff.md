# Comparing `tmp/opx_plus-0.1.0.tar.gz` & `tmp/opx_plus-0.1.1.tar.gz`

## Comparing `opx_plus-0.1.0.tar` & `opx_plus-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/.name
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/OPX_Plus.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.0/src/OPX_Plus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 opx_plus-0.1.0/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 opx_plus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 opx_plus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/.name
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/OPX_Plus.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opx_plus-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 opx_plus-0.1.1/src/OPX_Plus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opx_plus-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 opx_plus-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 opx_plus-0.1.1/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 opx_plus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 opx_plus-0.1.1/PKG-INFO
```

### Comparing `opx_plus-0.1.0/.DS_Store` & `opx_plus-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.0/.idea/workspace.xml` & `opx_plus-0.1.1/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `opx_plus-0.1.0/.idea/workspace.xml` & `opx_plus-0.1.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment="List dependencies in README">
+    <list default="true" id="e970cb05-7d56-441a-b2e6-7549de815664" name="Changes" comment="Missed a function in the README.">
       <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -22,14 +23,15 @@
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
+    &quot;ASKED_ADD_EXTERNAL_FILES&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;
   }
 }</component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
@@ -77,15 +79,22 @@
     <task id="LOCAL-00006" summary="List dependencies in README">
       <created>1681827924064</created>
       <option name="number" value="00006"/>
       <option name="presentableId" value="LOCAL-00006"/>
       <option name="project" value="LOCAL"/>
       <updated>1681827924064</updated>
     </task>
-    <option name="localTasksCounter" value="7"/>
+    <task id="LOCAL-00007" summary="Missed a function in the README.">
+      <created>1681828151662</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1681828151662</updated>
+    </task>
+    <option name="localTasksCounter" value="8"/>
     <servers/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
       <map>
         <entry key="MAIN">
           <value>
@@ -97,10 +106,11 @@
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="git commit"/>
     <MESSAGE value="git commit test 2"/>
     <MESSAGE value="Write README"/>
     <MESSAGE value="I accidentally pasted over a function (copy_over_and_down_formulas -&gt; paste_csv_vals_to_sheet) definition... Fixed!"/>
     <MESSAGE value="List dependencies in README"/>
-    <option name="LAST_COMMIT_MESSAGE" value="List dependencies in README"/>
+    <MESSAGE value="Missed a function in the README."/>
+    <option name="LAST_COMMIT_MESSAGE" value="Missed a function in the README."/>
   </component>
 </project>
```

### Comparing `opx_plus-0.1.0/src/OPX_Plus.py` & `opx_plus-0.1.1/src/OPX_Plus.py`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.0/LICENSE.txt` & `opx_plus-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opx_plus-0.1.0/README.md` & `opx_plus-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,32 +7,40 @@
 import openpyxl, glob, webbrowser, warnings, csv, datetime, os, time
 from copy import copy
 from openpyxl.formula.translate import Translator
 ```
 
 ## Additional Functions
 ### Files
-- get_file_path(file_path, name_search, *if_missing_urls)
-- check_mandatory_files(f_list)
-- 0pen_template(template_path: object, *date_cells: str)
-- open_vals_only_sheet(from_wb_path, sheet_id=0)
-- save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
-- remove(file_path)
+```
+get_file_path(file_path, name_search, *if_missing_urls)
+check_mandatory_files(f_list)
+
+0pen_template(template_path: object, *date_cells: str)
+open_vals_only_sheet(from_wb_path, sheet_id=0)
+
+save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
+remove(file_path)
+```
 ### Move Data
-- paste_sheet_to_sheet(from_ws, to_ws, cell_range)
-- paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
-- 
-- copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
-- paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+```
+paste_sheet_to_sheet(from_ws, to_ws, cell_range)
+paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
+
+copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
+paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+```
 
 ### Sub-Functions
-- count_rows(worksheet)
-- num_to_excel_col(n)
-- excel_col_to_num(a)
-- to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
+```
+count_rows(worksheet)
+num_to_excel_col(n)
+excel_col_to_num(a)
+
+to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
                  day=datetime.datetime.now().day, hour=datetime.datetime.now().hour,
                  minute=datetime.datetime.now().minute, second=datetime.datetime.now().second, add_3_zeros=False,
                  subtract=datetime.timedelta(0))
-- date_ranger()
-- worksheet_reset(sheet_nam, wb)
-
+date_ranger()
+worksheet_reset(sheet_nam, wb)
+```
```

### Comparing `opx_plus-0.1.0/pyproject.toml` & `opx_plus-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "OPX_Plus"
-version = "0.1.0"
+name = "OPX-Plus"
+version = "0.1.1"
 authors = [
   { name="Steven Wilson", github="https://github.com/StevenWilson9" },
 ]
 description = "Adds additional functionality on top of OpenPyXL"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `opx_plus-0.1.0/PKG-INFO` & `opx_plus-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OPX_Plus
-Version: 0.1.0
+Name: OPX-Plus
+Version: 0.1.1
 Summary: Adds additional functionality on top of OpenPyXL
 Project-URL: Homepage, https://github.com/StevenWilson9/OPX_Plus
 Project-URL: Bug Tracker, https://github.com/StevenWilson9/OPX_Plus/issues
 Author: Steven Wilson
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,32 +21,40 @@
 import openpyxl, glob, webbrowser, warnings, csv, datetime, os, time
 from copy import copy
 from openpyxl.formula.translate import Translator
 ```
 
 ## Additional Functions
 ### Files
-- get_file_path(file_path, name_search, *if_missing_urls)
-- check_mandatory_files(f_list)
-- 0pen_template(template_path: object, *date_cells: str)
-- open_vals_only_sheet(from_wb_path, sheet_id=0)
-- save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
-- remove(file_path)
+```
+get_file_path(file_path, name_search, *if_missing_urls)
+check_mandatory_files(f_list)
+
+0pen_template(template_path: object, *date_cells: str)
+open_vals_only_sheet(from_wb_path, sheet_id=0)
+
+save_file(new_file_location, file_name, workbook, afterdatetext="", previousday=False)
+remove(file_path)
+```
 ### Move Data
-- paste_sheet_to_sheet(from_ws, to_ws, cell_range)
-- paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
-- 
-- copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
-- paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+```
+paste_sheet_to_sheet(from_ws, to_ws, cell_range)
+paste_csv_vals_to_sheet(csv_path, to_sheet, include_header=False)
+
+copy_over_and_down_formulas(from_ws, to_ws, formula_cells)
+paste_cells_to_cells(from_ws, to_ws, from_cell_range, offset=(0, 0))
+```
 
 ### Sub-Functions
-- count_rows(worksheet)
-- num_to_excel_col(n)
-- excel_col_to_num(a)
-- to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
+```
+count_rows(worksheet)
+num_to_excel_col(n)
+excel_col_to_num(a)
+
+to_unix_time(year=datetime.datetime.now().year, month=datetime.datetime.now().month,
                  day=datetime.datetime.now().day, hour=datetime.datetime.now().hour,
                  minute=datetime.datetime.now().minute, second=datetime.datetime.now().second, add_3_zeros=False,
                  subtract=datetime.timedelta(0))
-- date_ranger()
-- worksheet_reset(sheet_nam, wb)
-
+date_ranger()
+worksheet_reset(sheet_nam, wb)
+```
```

