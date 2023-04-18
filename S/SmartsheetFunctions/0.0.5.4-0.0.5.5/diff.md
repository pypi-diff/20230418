# Comparing `tmp/SmartsheetFunctions-0.0.5.4.tar.gz` & `tmp/SmartsheetFunctions-0.0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartsheetFunctions-0.0.5.4.tar", last modified: Mon Apr 17 21:15:06 2023, max compression
+gzip compressed data, was "SmartsheetFunctions-0.0.5.5.tar", last modified: Tue Apr 18 16:23:49 2023, max compression
```

## Comparing `SmartsheetFunctions-0.0.5.4.tar` & `SmartsheetFunctions-0.0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.169198 SmartsheetFunctions-0.0.5.4/
--rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.4/LICENSE
--rw-rw-rw-   0        0        0     5064 2023-04-17 21:15:06.168198 SmartsheetFunctions-0.0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.150201 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/
--rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/__init__.py
--rw-rw-rw-   0        0        0    23631 2023-04-17 21:14:49.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/smartsheet.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:15:06.166199 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/
--rw-rw-rw-   0        0        0     5064 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 21:15:06.000000 SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 21:15:06.170200 SmartsheetFunctions-0.0.5.4/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 21:14:48.000000 SmartsheetFunctions-0.0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:23:49.604123 SmartsheetFunctions-0.0.5.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.5/LICENSE
+-rw-rw-rw-   0        0        0     5064 2023-04-18 16:23:49.603124 SmartsheetFunctions-0.0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 16:23:49.584124 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions/
+-rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions/__init__.py
+-rw-rw-rw-   0        0        0    23799 2023-04-18 16:23:07.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions/smartsheet.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:23:49.600122 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/
+-rw-rw-rw-   0        0        0     5064 2023-04-18 16:23:49.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-18 16:23:49.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:23:49.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 16:23:49.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-18 16:23:49.000000 SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 16:23:49.604123 SmartsheetFunctions-0.0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-18 16:23:30.000000 SmartsheetFunctions-0.0.5.5/setup.py
```

### Comparing `SmartsheetFunctions-0.0.5.4/LICENSE` & `SmartsheetFunctions-0.0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.4/PKG-INFO` & `SmartsheetFunctions-0.0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.4/README.md` & `SmartsheetFunctions-0.0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.4/SmartsheetFunctions/smartsheet.py` & `SmartsheetFunctions-0.0.5.5/SmartsheetFunctions/smartsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         api_url = f"{self.api_url}sheets/{self.sheet_id}/columns"
         payload = json.dumps(payload, default=json_decode_handler)
         r = requests.post(api_url, headers=self.std_header, data=payload)
         if r.status_code != 200:
             print(r.status_code, r.text)
         return r.json()
     
-    def add_rows_payload_creator(self, data: list, column_headers: list, add_row_position: str, additional_settings: dict) -> list:
+    def add_rows_payload_creator(self, data: list, column_headers: list, add_row_position: str, additional_settings: dict, rows_to_skip: int) -> list:
             """
             Creates a payload for adding new rows to a Smartsheet.
 
             Args:
                 data (list): A list of data to be added to the sheet. Each element of the list represents a new row.
                 column_headers (list): A list of the column headers in the order they appear in the sheet.
                 add_row_position (str): A string indicating whether new rows should be added at the top or bottom of the sheet.
@@ -429,23 +429,27 @@
             # Get the IDs of the columns in the sheet, so we can map column headers to column IDs later.
             col_names = self.column_names()
             col_ids = self.sheet_column_ids()
             col_dict = self.column_dictionary(col_names, col_ids)
 
             add_payload = []
             rows_payload = []
-            counter = 0
+            counter = 1
+            
+            #set rows to skip to 0 if not specified
+            if rows_to_skip == None:
+                rows_to_skip = 0
 
             # Regular expressions for matching decimal and percentage values in cells.
             decimal_regex = re.compile(r"\d+\.\d+")
             percent_pattern = re.compile(r"\d+%")
 
             # Loop over the rows of data, creating a payload for each row.
             for row in new_data:
-                if counter != 0:
+                if counter > rows_to_skip:
                     col_counter = 0
                     for col in column_headers:
                         
                         # Check if the cell value is a decimal or percentage value, and convert it if necessary.
                         decimal_regex_test = decimal_regex.search(str(row[col_counter]))
                         datetime_test = isinstance(row[col_counter], datetime.datetime)
```

### Comparing `SmartsheetFunctions-0.0.5.4/SmartsheetFunctions.egg-info/PKG-INFO` & `SmartsheetFunctions-0.0.5.5/SmartsheetFunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.4
+Version: 0.0.5.5
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.4/setup.py` & `SmartsheetFunctions-0.0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="SmartsheetFunctions",
-    version="0.0.5.4",
+    version="0.0.5.5",
     author="Derek Bantel",
     author_email="derekbantel@outlook.com",
     description="SmartSheet Functions for development",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     packages=["SmartsheetFunctions"],
```

