# Comparing `tmp/codeprompt-0.1.0.tar.gz` & `tmp/codeprompt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeprompt-0.1.0.tar", max compression
+gzip compressed data, was "codeprompt-0.2.0.tar", max compression
```

## Comparing `codeprompt-0.1.0.tar` & `codeprompt-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-04-17 18:01:52.256574 codeprompt-0.1.0/codeprompt/__init__.py
--rw-r--r--   0        0        0     1480 2023-04-18 08:09:10.960763 codeprompt-0.1.0/codeprompt/chatgpt_models.py
--rw-r--r--   0        0        0     2075 2023-04-17 18:42:30.259935 codeprompt-0.1.0/codeprompt/cli.py
--rw-r--r--   0        0        0     5407 2023-04-18 08:15:39.777199 codeprompt-0.1.0/codeprompt/codeprompt.py
--rw-r--r--   0        0        0      287 2023-04-18 08:15:10.807370 codeprompt-0.1.0/codeprompt/promptstr.py
--rw-r--r--   0        0        0     1032 2023-04-17 20:10:28.531741 codeprompt-0.1.0/codeprompt/techniques/chunk.py
--rw-r--r--   0        0        0      415 2023-04-18 08:15:10.771268 codeprompt-0.1.0/codeprompt/techniques/count_token.py
--rw-r--r--   0        0        0     4877 2023-04-17 19:36:30.189113 codeprompt-0.1.0/codeprompt/template.py
--rw-r--r--   0        0        0     1096 2023-04-17 18:00:35.293947 codeprompt-0.1.0/LICENSE
--rw-r--r--   0        0        0      610 2023-04-18 08:15:49.343113 codeprompt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2236 2023-04-18 08:13:06.162124 codeprompt-0.1.0/README.md
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 codeprompt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-17 18:01:52.256574 codeprompt-0.2.0/codeprompt/__init__.py
+-rw-r--r--   0        0        0     1480 2023-04-18 08:09:10.960763 codeprompt-0.2.0/codeprompt/chatgpt_models.py
+-rw-r--r--   0        0        0     2075 2023-04-17 18:42:30.259935 codeprompt-0.2.0/codeprompt/cli.py
+-rw-r--r--   0        0        0     5407 2023-04-18 08:15:39.777199 codeprompt-0.2.0/codeprompt/codeprompt.py
+-rw-r--r--   0        0        0      295 2023-04-18 08:19:37.721986 codeprompt-0.2.0/codeprompt/promptstr.py
+-rw-r--r--   0        0        0     1032 2023-04-17 20:10:28.531741 codeprompt-0.2.0/codeprompt/techniques/chunk.py
+-rw-r--r--   0        0        0      419 2023-04-18 08:19:37.736031 codeprompt-0.2.0/codeprompt/techniques/count_token.py
+-rw-r--r--   0        0        0     4881 2023-04-18 08:20:38.002085 codeprompt-0.2.0/codeprompt/template.py
+-rw-r--r--   0        0        0     1096 2023-04-17 18:00:35.293947 codeprompt-0.2.0/LICENSE
+-rw-r--r--   0        0        0      610 2023-04-18 08:24:07.691394 codeprompt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2242 2023-04-18 08:20:37.956518 codeprompt-0.2.0/README.md
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 codeprompt-0.2.0/PKG-INFO
```

### Comparing `codeprompt-0.1.0/codeprompt/chatgpt_models.py` & `codeprompt-0.2.0/codeprompt/chatgpt_models.py`

 * *Files identical despite different names*

### Comparing `codeprompt-0.1.0/codeprompt/cli.py` & `codeprompt-0.2.0/codeprompt/cli.py`

 * *Files identical despite different names*

### Comparing `codeprompt-0.1.0/codeprompt/codeprompt.py` & `codeprompt-0.2.0/codeprompt/codeprompt.py`

 * *Files identical despite different names*

### Comparing `codeprompt-0.1.0/codeprompt/techniques/chunk.py` & `codeprompt-0.2.0/codeprompt/techniques/chunk.py`

 * *Files identical despite different names*

### Comparing `codeprompt-0.1.0/codeprompt/template.py` & `codeprompt-0.2.0/codeprompt/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         parsed_content = self.templates_env.parse(template_source)
         variables = meta.find_undeclared_variables(parsed_content)
         return template, variables
 
 
 if __name__ == "__main__":
     template_dirs = [
-        "C:\\Users\\joe\\AppData\\Local\\pyprompt\\templates",
-        "C:\\Users\\joe\\AppData\\Local\\pyprompt\\profiles\\default\\templates",
+        "C:\\Users\\joe\\AppData\\Local\\codeprompt\\templates",
+        "C:\\Users\\joe\\AppData\\Local\\codeprompt\\profiles\\default\\templates",
     ]
     template_dirs = [Path(template_dir) for template_dir in template_dirs]
     template_manager = TemplateManager(template_dirs)
     template_manager.load_templates()
     template_name = "test_template.md"
     substitutions = {
         "name": "Joe",
```

### Comparing `codeprompt-0.1.0/LICENSE` & `codeprompt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeprompt-0.1.0/pyproject.toml` & `codeprompt-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeprompt"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Nutchanon Ninyawee <nutchanon@codustry.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 codeprompt = "codeprompt.codeprompt:main"
```

### Comparing `codeprompt-0.1.0/README.md` & `codeprompt-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# pyprompt
+# codeprompt
 ultils for prompt engineers e.g. chucking
 
 ## install
 ```bash
-pip install pyprompt
+pip install codeprompt
 ```
 
 ```bash
 $ codeprompt
 Open VSCode and Copy the paths (Shift + Alt + C) of the files you want to include in the prompt.
 Press Enter to continue.
 
@@ -28,15 +28,15 @@
 representing the repository ends when the symbols "--END--" are encountered. Meanwhile,
 Reply with "Aha" to allow me continue providing more context.
 
 Any further text beyond "--END--" should be interpreted as instructions using the aforementioned code as
 context. Instructions may include questions, requests to refactor, debug, find vulnerabilities, or make the
 code more robust. The programming language can be determined from the file extension in the file path.
 ----
-pyprompt\template.py
+codeprompt\template.py
 \`\`\`
 import os
 from pathlib import Path
 from loguru import logger
 
 import pyperclip
 import frontmatter
```

### Comparing `codeprompt-0.1.0/PKG-INFO` & `codeprompt-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeprompt
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Nutchanon Ninyawee
 Author-email: nutchanon@codustry.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,20 +15,20 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pygithub (>=1.58.1,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-frontmatter (>=1.0.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
-# pyprompt
+# codeprompt
 ultils for prompt engineers e.g. chucking
 
 ## install
 ```bash
-pip install pyprompt
+pip install codeprompt
 ```
 
 ```bash
 $ codeprompt
 Open VSCode and Copy the paths (Shift + Alt + C) of the files you want to include in the prompt.
 Press Enter to continue.
 
@@ -49,15 +49,15 @@
 representing the repository ends when the symbols "--END--" are encountered. Meanwhile,
 Reply with "Aha" to allow me continue providing more context.
 
 Any further text beyond "--END--" should be interpreted as instructions using the aforementioned code as
 context. Instructions may include questions, requests to refactor, debug, find vulnerabilities, or make the
 code more robust. The programming language can be determined from the file extension in the file path.
 ----
-pyprompt\template.py
+codeprompt\template.py
 \`\`\`
 import os
 from pathlib import Path
 from loguru import logger
 
 import pyperclip
 import frontmatter
```

