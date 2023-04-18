# Comparing `tmp/robotframework-robocop-3.0.0.tar.gz` & `tmp/robotframework-robocop-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-3.0.0.tar", last modified: Wed Mar 29 09:13:04 2023, max compression
+gzip compressed data, was "robotframework-robocop-3.1.0.tar", last modified: Tue Apr 18 11:05:52 2023, max compression
```

## Comparing `robotframework-robocop-3.0.0.tar` & `robotframework-robocop-3.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:13:04.717790 robotframework-robocop-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-03-29 09:13:04.717790 robotframework-robocop-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:13:04.709790 robotframework-robocop-3.0.0/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:13:04.713790 robotframework-robocop-3.0.0/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    21057 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    23787 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30700 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    33042 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:13:04.713790 robotframework-robocop-3.0.0/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:13:04.717790 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-29 09:13:04.000000 robotframework-robocop-3.0.0/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:13:04.717790 robotframework-robocop-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-29 09:12:51.000000 robotframework-robocop-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.062965 robotframework-robocop-3.1.0/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.062965 robotframework-robocop-3.1.0/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31744 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33520 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 11:05:52.000000 robotframework-robocop-3.1.0/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:05:52.066964 robotframework-robocop-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-18 11:05:39.000000 robotframework-robocop-3.1.0/setup.py
```

### Comparing `robotframework-robocop-3.0.0/LICENSE` & `robotframework-robocop-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/PKG-INFO` & `robotframework-robocop-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.0.0
+Version: 3.1.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.0.0/README.md` & `robotframework-robocop-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/__init__.py` & `robotframework-robocop-3.1.0/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/comments.py` & `robotframework-robocop-3.1.0/robocop/checkers/comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
     def check_line(self, line, lineno):
         if line.startswith(self.SECTION_HEADER):
             return True
         if line.startswith(self.ROBOCOP_HEADER):
             return False
         if lineno == 1:
-            if line.startswith(self.LANGUAGE_HEADER):
+            if line.lower().startswith(self.LANGUAGE_HEADER):
                 self.has_language_header = True
                 return False
             elif self.is_bom:
                 # if it's BOM encoded file, first line can be ignored
                 return "***" in line
         if self.has_language_header and not line.strip():
             # empty lines after language: header can be ignored
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/documentation.py` & `robotframework-robocop-3.1.0/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/duplications.py` & `robotframework-robocop-3.1.0/robocop/checkers/duplications.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/errors.py` & `robotframework-robocop-3.1.0/robocop/checkers/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     from robot.api.parsing import If
 except ImportError:
     If = None
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleSeverity
-from robocop.utils import ROBOT_VERSION, find_robot_vars, token_col
+from robocop.utils import ROBOT_VERSION, find_robot_vars
 
 rules = {
     "0401": Rule(
         rule_id="0401",
         name="parsing-error",
         msg="Robot Framework syntax error: {{ error_msg }}",
         severity=RuleSeverity.ERROR,
@@ -213,14 +213,24 @@
     "0414": Rule(
         rule_id="0414",
         name="return-in-test-case",
         msg="RETURN can only be used inside a user keyword",
         severity=RuleSeverity.ERROR,
         version=">=5.0",
     ),
+    "0415": Rule(
+        rule_id="0415",
+        name="invalid-section-in-resource",
+        msg="Resource file can't contain '{{ section_name }}' section",
+        docs="""
+        The higher-level structure of resource files is the same as that of test case files,
+        but they can't contain Test Cases or Tasks sections.
+        """,
+        severity=RuleSeverity.ERROR,
+    ),
 }
 
 
 class ParsingErrorChecker(VisitorChecker):
     """Checker that parses Robot Framework DataErrors."""
 
     reports = (
@@ -231,14 +241,15 @@
         "non-existing-setting",
         "setting-not-supported",
         "not-enough-whitespace-after-variable",
         "not-enough-whitespace-after-suite-setting",
         "invalid-for-loop",
         "invalid-if",
         "return-in-test-case",
+        "invalid-section-in-resource",
     )
 
     keyword_only_settings = {"Arguments", "Return"}
     keyword_settings = [
         "[Documentation]",
         "[Tags]",
         "[Arguments]",
@@ -324,14 +335,16 @@
             self.handle_invalid_block(node, error, "invalid-if")
         elif "FOR loop" in error:
             self.handle_invalid_block(node, error, "invalid-for-loop")
         elif "Non-default argument after default arguments" in error or "Only last argument can be kwargs" in error:
             self.handle_positional_after_named(node, error_index)
         elif "is allowed only once. Only the first value is used" in error:
             return
+        elif "Resource file with" in error:
+            self.handle_invalid_section_in_resource(node, error)
         else:
             error = error.replace("\n   ", "")
             token = node.header if hasattr(node, "header") else node
             end_col = token.col_offset + len(node.name) + 1 if hasattr(node, "name") else token.end_col_offset + 1
             # TODO: 'col' location here can be specified more precisely
             self.report("parsing-error", error_msg=error, node=node, col=token.col_offset + 1, end_col=end_col)
 
@@ -513,14 +526,24 @@
             "parsing-error",
             error_msg=f"Positional argument '{token.value}' follows named argument",
             node=token,
             col=token.col_offset + 1,
             end_col=token.end_col_offset + 1,
         )
 
+    def handle_invalid_section_in_resource(self, node, error):
+        error_token = node.tokens[0]
+        section_name = error_token.value
+        self.report(
+            "invalid-section-in-resource",
+            section_name=section_name,
+            node=node,
+            end_col=node.col_offset + len(section_name) + 1,
+        )
+
 
 class TwoSpacesAfterSettingsChecker(VisitorChecker):
     """Checker for not enough whitespaces after [Setting] header."""
 
     reports = ("not-enough-whitespace-after-setting",)
 
     def __init__(self):
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/lengths.py` & `robotframework-robocop-3.1.0/robocop/checkers/lengths.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,14 +223,50 @@
             Test case
                 [Tags]    smoke
                 Skip    Test case draft
 
         """,
         severity=RuleSeverity.ERROR,
     ),
+    "0529": Rule(
+        rule_id="0529",
+        name="empty-test-template",
+        msg="Test Template is empty",
+        docs="""
+        ``Test Template`` sets the template to all tests in a suite. Empty value is considered an error
+        because it leads the users to wrong impression on how the suite operates.
+        Without value, the setting is ignored and the tests are not templated.
+        """,
+        severity=RuleSeverity.ERROR,
+    ),
+    "0530": Rule(
+        rule_id="0530",
+        name="empty-template",
+        msg="Template of {{ block_name }} is empty. "
+        "To overwrite suite Test Template use more explicit [Template]  NONE",
+        docs="""
+        The ``[Template]`` setting overrides the possible template set in the Setting section, and an empty value for 
+        ``[Template]`` means that the test has no template even when Test Template is used.
+        
+        If it is intended behaviour, use more explicit ``NONE`` value to indicate that you want to overwrite suite 
+        Test Template::
+        
+            *** Settings ***
+            Test Template    Template Keyword
+            
+            *** Test Cases ***
+            Templated test
+                argument
+            
+            Not templated test
+                [Template]    NONE
+
+        """,
+        severity=RuleSeverity.WARNING,
+    ),
 }
 
 
 def is_data_statement(node):
     return not isinstance(node, (EmptyLine, Comment))
 
 
@@ -501,14 +537,16 @@
         "empty-suite-setup",
         "empty-test-setup",
         "empty-teardown",
         "empty-suite-teardown",
         "empty-test-teardown",
         "empty-timeout",
         "empty-test-timeout",
+        "empty-template",
+        "empty-test-template",
         "empty-arguments",
     )
 
     def __init__(self):
         self.parent_node_name = ""
         super().__init__()
 
@@ -596,14 +634,28 @@
         if not node.name:
             self.report("empty-suite-teardown", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
 
     def visit_TestTeardown(self, node):  # noqa
         if not node.name:
             self.report("empty-test-teardown", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
 
+    def visit_TestTemplate(self, node):  # noqa
+        if not node.value:
+            self.report("empty-test-template", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
+
+    def visit_Template(self, node):  # noqa
+        if len(node.data_tokens) < 2:
+            self.report(
+                "empty-template",
+                block_name=self.parent_node_name,
+                node=node,
+                col=node.data_tokens[0].col_offset + 1,
+                end_col=node.end_col_offset,
+            )
+
     def visit_Timeout(self, node):  # noqa
         if not node.value:
             self.report(
                 "empty-timeout",
                 block_name=self.parent_node_name,
                 node=node,
                 col=node.data_tokens[0].col_offset + 1,
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/misc.py` & `robotframework-robocop-3.1.0/robocop/checkers/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "0901": Rule(
         rule_id="0901",
         name="keyword-after-return",
         msg="{{ error_msg }}",
         severity=RuleSeverity.WARNING,
         docs="""
         To improve readability use ``[Return]`` setting at the end of the keyword. If you want to return immediately
-        from the keyword use ``RETURN`` statement instead. ``[Return]`` does not return from the keyword but only
+        from the keyword, use ``RETURN`` statement instead. ``[Return]`` does not return from the keyword but only
         sets the values that will be returned at the end of the keyword.
 
         Bad::
 
             Keyword
                 Step
                 [Return]    ${variable}
@@ -284,14 +284,65 @@
 
         can be replaced with::
 
             IF    $condition    BREAK
 
         """,
     ),
+    "0917": Rule(
+        rule_id="0917",
+        name="unreachable-code",
+        msg="Unreachable code after {{ statement }} statement",
+        severity=RuleSeverity.WARNING,
+        version=">=5.0",
+        docs="""
+        Detect the unreachable code after RETURN, BREAK or CONTINUE statements.
+
+        For example::
+
+        Example Keyword
+            FOR    ${animal}    IN    cat    dog
+                IF    '${animal}' == 'cat'
+                    CONTINUE
+                    Log  ${animal}  # unreachable log
+                END
+                BREAK
+                Log    Unreachable log
+            END
+            RETURN
+            Log    Unreachable log
+        """,
+    ),
+    "0918": Rule(
+        rule_id="0918",
+        name="multiline-inline-if",
+        msg="Avoid splitting inline IF to multiple lines",
+        severity=RuleSeverity.WARNING,
+        version=">=5.0",
+        docs="""
+        It's allowed to create inline IF that spans multiple lines, but it should be avoided,
+        since it decreases readability. Try to use normal IF/ELSE instead.
+
+        Bad::
+
+            IF  ${condition}  Log  hello
+            ...    ELSE       Log  hi!
+
+        Good::
+
+            IF  ${condition}    Log  hello     ELSE    Log  hi!
+        or::
+
+            IF  ${condition}
+                Log  hello
+            ELSE
+                Log  hi!
+            END
+        """,
+    ),
 }
 
 
 class ReturnChecker(VisitorChecker):
     """Checker for [Return] and Return From Keyword violations."""
 
     reports = (
@@ -315,31 +366,63 @@
                     token = child.data_tokens[0]
                     self.report(
                         "empty-return",
                         node=child,
                         col=token.col_offset + 1,
                         end_col=token.col_offset + len(token.value),
                     )
-            elif ReturnStatement and isinstance(child, ReturnStatement):  # type: ignore[arg-type]
-                return_setting_node = child
-                error = "RETURN is not defined at the end of keyword"
             elif not isinstance(child, (EmptyLine, Comment, Teardown)):
                 if return_setting_node is not None:
                     keyword_after_return = True
 
             if isinstance(child, KeywordCall):
                 if return_from:
                     keyword_after_return = True
                     return_setting_node = child
                     error = "Keyword call after 'Return From Keyword'"
                 elif normalize_robot_name(child.keyword, remove_prefix="builtin.") == "returnfromkeyword":
                     return_from = True
         if keyword_after_return:
             token = return_setting_node.data_tokens[0]
-            self.report("keyword-after-return", error_msg=error, node=token, col=token.col_offset + 1)
+            self.report(
+                "keyword-after-return",
+                error_msg=error,
+                node=token,
+                col=token.col_offset + 1,
+                end_col=token.end_col_offset + 1,
+            )
+        self.generic_visit(node)
+
+    visit_If = visit_For = visit_While = visit_Try = visit_Keyword
+
+
+class UnreachableCodeChecker(VisitorChecker):
+    """Checker for unreachable code after RETURN, BREAK or CONTINUE statements."""
+
+    reports = ("unreachable-code",)
+
+    def visit_Keyword(self, node):  # noqa
+        statement_node = None
+
+        for child in node.body:
+            if ReturnStatement and isinstance(child, (ReturnStatement, Break, Continue)):  # type: ignore[arg-type]
+                statement_node = child
+            elif not isinstance(child, (EmptyLine, Comment, Teardown)):
+                if statement_node is not None:
+                    token = statement_node.data_tokens[0]
+                    code_after_statement = child.data_tokens[0] if hasattr(child, "data_tokens") else child
+                    self.report(
+                        "unreachable-code",
+                        statement=token.value,
+                        node=child,
+                        col=code_after_statement.col_offset + 1,
+                        end_col=child.end_col_offset + 1,
+                    )
+                    statement_node = None
+
         self.generic_visit(node)
 
     visit_If = visit_For = visit_While = visit_Try = visit_Keyword
 
 
 class NestedForLoopsChecker(VisitorChecker):
     """Checker for not supported nested FOR loops.
@@ -541,25 +624,26 @@
 
 class IfChecker(VisitorChecker):
     """Checker for IF blocks"""
 
     reports = (
         "if-can-be-merged",
         "inline-if-can-be-used",
+        "multiline-inline-if",
     )
 
     def visit_TestCase(self, node):  # noqa
         if get_errors(node):
             return
         self.check_adjacent_ifs(node)
 
     visit_For = visit_If = visit_Keyword = visit_TestCase  # TODO  While, Try Except?
 
     @staticmethod
-    def is_if_inline(node):
+    def is_inline_if(node):
         return isinstance(node.header, InlineIfHeader)
 
     def check_adjacent_ifs(self, node):
         previous_if = None
         for child in node.body:
             if isinstance(child, If):
                 if child.header.errors:
@@ -602,15 +686,24 @@
     @staticmethod
     def tokens_length(tokens):
         return sum(len(token.value) for token in tokens)
 
     def check_whether_if_should_be_inline(self, node):
         if ROBOT_VERSION.major < 5:
             return
-        if self.is_if_inline(node):
+        if self.is_inline_if(node):
+            if node.lineno != node.end_lineno:
+                if_header = node.header.data_tokens[0]
+                self.report(
+                    "multiline-inline-if",
+                    node=node,
+                    col=if_header.col_offset + 1,
+                    end_lineno=node.end_lineno,
+                    end_col=node.end_col_offset + 1,
+                )
             return
         if (
             len(node.body) != 1
             or node.orelse
             or not isinstance(node.body[0], (KeywordCall, ReturnStatement, Break, Continue))  # type: ignore[arg-type]
         ):
             return
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/naming.py` & `robotframework-robocop-3.1.0/robocop/checkers/naming.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import string
 from collections import defaultdict
 from pathlib import Path
 
 from robot.api import Token
 from robot.parsing.model.blocks import Keyword
 from robot.parsing.model.statements import Arguments, KeywordCall
+from robot.variables.search import search_variable
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleParam, RuleSeverity
 from robocop.utils import (
     ROBOT_VERSION,
     find_robot_vars,
     keyword_col,
     normalize_robot_name,
     normalize_robot_var_name,
     pattern_type,
     remove_robot_vars,
     token_col,
 )
+from robocop.utils.misc import remove_nested_variables
 from robocop.utils.run_keywords import iterate_keyword_names
 
 rules = {
     "0301": Rule(
         RuleParam(
             name="pattern",
             default=re.compile(r"[\.\?]"),
@@ -161,14 +163,30 @@
         severity=RuleSeverity.WARNING,
     ),
     "0310": Rule(
         rule_id="0310",
         name="non-local-variables-should-be-uppercase",
         msg="Test, suite and global variables should be uppercase",
         severity=RuleSeverity.WARNING,
+        docs="""
+        Good::
+
+            Set Task Variable    ${MY_VAR}           1
+            Set Suite Variable   ${MY VAR}           1
+            Set Test Variable    ${MY_VAR}           1
+            Set Global Variable  ${MY VAR${nested}}  1
+
+        Bad::
+
+            Set Task Variable    ${my_var}           1
+            Set Suite Variable   ${My Var}           1
+            Set Test Variable    ${myvar}            1
+            Set Global Variable  ${my_var${NESTED}}  1
+
+        """,
     ),
     "0311": Rule(
         rule_id="0311",
         name="else-not-upper-case",
         msg="ELSE and ELSE IF should be upper case",
         severity=RuleSeverity.ERROR,
     ),
@@ -644,27 +662,29 @@
             "settaskvariable",
             "settestvariable",
             "setsuitevariable",
             "setglobalvariable",
         }
         super().__init__()
 
-    def visit_VariableSection(self, node):  # noqa
-        for child in node.body:
-            if not child.data_tokens:
-                continue
-            token = child.data_tokens[0]
-            if token.type == Token.VARIABLE and token.value and not token.value.isupper():
-                self.report(
-                    "section-variable-not-uppercase",
-                    variable_name=token.value,
-                    lineno=token.lineno,
-                    col=token.col_offset + 1,
-                    end_col=token.col_offset + len(token.value) + 1,
-                )
+    def visit_Variable(self, node):  # noqa
+        token = node.data_tokens[0]
+        var_name = search_variable(token.value).base
+        if var_name is None:
+            return  # in RF<=5, a continuation mark ` ...` is wrongly considered a variable
+        # in Variables section, everything needs to be in uppercase
+        # because even when the variable is nested, it needs to be global
+        if not var_name.isupper():
+            self.report(
+                "section-variable-not-uppercase",
+                variable_name=token.value.strip(),
+                lineno=token.lineno,
+                col=token.col_offset + 1,
+                end_col=token.col_offset + len(token.value) + 1,
+            )
 
     def visit_KeywordCall(self, node):  # noqa
         for token in node.get_tokens(Token.ASSIGN):
             if "-" in token.value:
                 self.report(
                     "hyphen-in-variable-name",
                     variable_name=token.value,
@@ -675,15 +695,21 @@
 
         if not node.keyword:
             return
         if normalize_robot_name(node.keyword, remove_prefix="builtin.") in self.set_variable_variants:
             if len(node.data_tokens) < 2:
                 return
             token = node.data_tokens[1]
-            if token.type == Token.ARGUMENT and not token.value.isupper():
+            if not token.value:
+                return
+            var_name = search_variable(token.value).base
+            normalized_var_name = remove_nested_variables(var_name)
+            # a variable as a keyword argument can contain lowercase nested variable
+            # because the actual value of it may be uppercase
+            if not normalized_var_name.isupper():
                 self.report(
                     "non-local-variables-should-be-uppercase",
                     node=node,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/spacing.py` & `robotframework-robocop-3.1.0/robocop/checkers/spacing.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from contextlib import contextmanager
 
 from robot.api import Token
 from robot.parsing.model.blocks import Keyword, TestCase
 from robot.parsing.model.statements import Comment, EmptyLine
 from robot.parsing.model.visitor import ModelVisitor
 
+from robocop.utils.misc import ROBOT_VERSION
+
 try:
     from robot.api.parsing import InlineIfHeader
 except ImportError:
     InlineIfHeader = None
 
 from robocop.checkers import RawFileChecker, VisitorChecker
 from robocop.rules import Rule, RuleParam, RuleSeverity, SeverityThreshold
@@ -771,14 +773,23 @@
     """Checker for misaligned continuation line markers."""
 
     reports = (
         "misaligned-continuation",
         "misaligned-continuation-row",
     )
 
+    @staticmethod
+    def is_inline_if(node):
+        return isinstance(node.header, InlineIfHeader)
+
+    def visit_If(self, node):
+        # suppress the rules if the multiline-inline-if is already reported
+        if ROBOT_VERSION.major >= 5 and self.is_inline_if(node):
+            return
+
     def visit_Statement(self, node):  # noqa
         if not node.data_tokens:
             return
         starting_row = self.get_indent(node.tokens)
         first_column, indent = 0, 0
         for index, line in enumerate(node.lines):
             if index == 0:
@@ -802,23 +813,26 @@
                     indent = 0
                 elif token.type != Token.EOL and token.value.strip():  # ignore trailing whitespace
                     ignore_docs = self.param("misaligned-continuation-row", "ignore_docs")
                     if node.type == Token.DOCUMENTATION and ignore_docs:
                         break
                     if first_column:
                         if indent != first_column:
-                            cont = [token for token in line if token.type == "CONTINUATION"][0]
+                            cont = [token for token in line if token.type == "CONTINUATION"]
+                            if not cont:
+                                break
                             self.report(
                                 "misaligned-continuation-row",
                                 node=token,
                                 end_col=token.col_offset + 1,
-                                col=cont.end_col_offset + 1,
+                                col=cont[0].end_col_offset + 1,
                             )
                     else:
-                        first_column = indent
+                        if token.type != Token.COMMENT:
+                            first_column = indent
                     break  # check only first value
 
     @staticmethod
     def get_indent(tokens):
         indent_len = 0
         for token in tokens:
             if token.type != Token.SEPARATOR:
```

### Comparing `robotframework-robocop-3.0.0/robocop/checkers/tags.py` & `robotframework-robocop-3.1.0/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/config.py` & `robotframework-robocop-3.1.0/robocop/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,19 +500,25 @@
 
     def check_deprecations(self, rules):
         renamed = {
             # "old-name": "new-name"
         }
         deprecated = {
             # "rule-name": "deprecation message"
-            "bad-indent": "`strict` and `ignore_uneven` parameters are no longer available for this rule. Take a look at new E1017 bad-block-indent rule that replaces them."  # warning added in v.3.0.0
+            "bad-indent": "'strict' and 'ignore_uneven' parameters are no longer available for this rule. Take a look at new E1017 bad-block-indent rule that replaces them."  # warning added in v.3.0.0
         }
         deprecation_header = "### DEPRECATION WARNING ###"
         deprecation_footer = "This information will disappear in the next version.\n\n"
-        for rule in chain(self.include, self.exclude):
+        # get all rules mentioned in include and exclude CLI options
+        mentioned_rules = self.include.union(self.exclude)
+        # add the rules mentioned in configure CLI option
+        mentioned_rules.update(configured.split(":", 1)[0] for configured in self.configure)
+        for rule in mentioned_rules:
+            if rule not in rules:  # reports can also be configured, but we only want rules here
+                continue
             rule_name = rules[rule].name
             if rule_name in renamed:  # update warning description to specific case
                 print(
                     f"{deprecation_header}\n"
                     f"Rule '{rule_name}' is renamed to '{renamed[rule_name]}'.\n"
                     f"Update your configuration if you're using the old name. "
                     f"{deprecation_footer}"
```

### Comparing `robotframework-robocop-3.0.0/robocop/exceptions.py` & `robotframework-robocop-3.1.0/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/files.py` & `robotframework-robocop-3.1.0/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/reports.py` & `robotframework-robocop-3.1.0/robocop/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     Example::
 
         Issues by ID:
         W0502 (too-little-calls-in-keyword) : 5
         W0201 (missing-doc-keyword)         : 4
         E0401 (parsing-error)               : 3
         W0301 (not-allowed-char-in-name)    : 2
-        E0901 (keyword-after-return)        : 1
+        W0901 (keyword-after-return)        : 1
     """
 
     def __init__(self):
         self.name = "rules_by_id"
         self.description = "Groups detected issues by rule id and prints it ordered by most common"
         self.message_counter = defaultdict(int)
```

### Comparing `robotframework-robocop-3.0.0/robocop/rules.py` & `robotframework-robocop-3.1.0/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/run.py` & `robotframework-robocop-3.1.0/robocop/run.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/utils/__init__.py` & `robotframework-robocop-3.1.0/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/utils/disablers.py` & `robotframework-robocop-3.1.0/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/utils/file_types.py` & `robotframework-robocop-3.1.0/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/utils/misc.py` & `robotframework-robocop-3.1.0/robocop/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from robot.api import Token
 
 try:
     from robot.api.parsing import Variable
 except ImportError:
     from robot.parsing.model.statements import Variable
 
+from robot.variables.search import VariableIterator
 from robot.version import VERSION as RF_VERSION
 
 from robocop.exceptions import InvalidExternalCheckerError
 from robocop.utils.version_matching import Version
 from robocop.version import __version__
 
 ROBOT_VERSION = Version(RF_VERSION)
@@ -80,14 +81,23 @@
     return name
 
 
 def normalize_robot_var_name(name: str) -> str:
     return normalize_robot_name(name)[2:-1] if name else ""
 
 
+def remove_nested_variables(var_name):
+    for prefix, match, suffix in VariableIterator(var_name, ignore_errors=True):
+        if match:  # if nested variable exists
+            # take what surrounds it and run the check again
+            var_name = remove_nested_variables(prefix + suffix)
+            break
+    return var_name.strip()
+
+
 def keyword_col(node) -> int:
     return token_col(node, Token.KEYWORD)
 
 
 def token_col(node, *token_type) -> int:
     if ROBOT_VERSION.major == 3:
         for tok_type in token_type:
```

### Comparing `robotframework-robocop-3.0.0/robocop/utils/run_keywords.py` & `robotframework-robocop-3.1.0/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robocop/utils/version_matching.py` & `robotframework-robocop-3.1.0/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-3.1.0/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.0.0
+Version: 3.1.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.0.0/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-3.1.0/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.0.0/setup.py` & `robotframework-robocop-3.1.0/setup.py`

 * *Files identical despite different names*

