# Comparing `tmp/griptape_core-0.9.0.tar.gz` & `tmp/griptape_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.9.0.tar", max compression
+gzip compressed data, was "griptape_core-0.9.1.tar", max compression
```

## Comparing `griptape_core-0.9.0.tar` & `griptape_core-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.9.0/LICENSE
--rw-r--r--   0        0        0     2822 2023-04-13 18:09:31.695590 griptape_core-0.9.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.9.0/griptape/__init__.py
--rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.9.0/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.9.0/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2618 2023-04-17 15:37:07.810310 griptape_core-0.9.0/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0      999 2023-04-13 18:09:31.698425 griptape_core-0.9.0/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.9.0/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.9.0/griptape/core/base_executor.py
--rw-r--r--   0        0        0     4110 2023-04-17 23:12:07.704923 griptape_core-0.9.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      529 2023-04-16 19:45:11.589553 griptape_core-0.9.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.9.0/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.9.0/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.9.0/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.9.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.9.0/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.9.0/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.9.0/griptape/core/utils/command_runner.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.9.0/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.9.0/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.9.0/griptape/core/utils/python_runner.py
--rw-r--r--   0        0        0      730 2023-04-17 23:27:20.929740 griptape_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 griptape_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2822 2023-04-13 18:09:31.695590 griptape_core-0.9.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.9.1/griptape/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-07 23:37:39.379544 griptape_core-0.9.1/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-08 22:17:54.154182 griptape_core-0.9.1/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2618 2023-04-17 15:37:07.810310 griptape_core-0.9.1/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0      999 2023-04-13 18:09:31.698425 griptape_core-0.9.1/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.9.1/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      379 2023-04-10 23:10:10.282207 griptape_core-0.9.1/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     4831 2023-04-18 15:48:38.107686 griptape_core-0.9.1/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      529 2023-04-16 19:45:11.589553 griptape_core-0.9.1/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.9.1/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-10 23:10:10.279443 griptape_core-0.9.1/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1865 2023-04-10 23:10:10.284540 griptape_core-0.9.1/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.9.1/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.9.1/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      356 2023-04-13 16:37:25.769148 griptape_core-0.9.1/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-09 19:15:55.931641 griptape_core-0.9.1/griptape/core/utils/command_runner.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.9.1/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.9.1/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape_core-0.9.1/griptape/core/utils/python_runner.py
+-rw-r--r--   0        0        0      730 2023-04-18 15:51:31.865035 griptape_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 griptape_core-0.9.1/PKG-INFO
```

### Comparing `griptape_core-0.9.0/LICENSE` & `griptape_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/README.md` & `griptape_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.9.1/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.9.1/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/base_tool.py` & `griptape_core-0.9.1/griptape/core/base_tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import logging
 import os
 from abc import ABC
 from typing import Optional
 import yaml
 from attr import define, fields, Attribute, field, Factory
+from decouple import config
 from jinja2 import Template
 
 
 @define
 class BaseTool(ABC):
     MANIFEST_FILE = "manifest.yml"
     DOCKERFILE_FILE = "Dockerfile"
@@ -22,15 +23,17 @@
 
     @property
     def env_fields(self) -> list[Attribute]:
         return [f for f in fields(self.__class__) if f.metadata.get("env")]
 
     @property
     def env(self) -> dict[str, str]:
-        return {f.metadata["env"]: str(getattr(self, f.name)) for f in self.env_fields}
+        return {
+            f.metadata["env"]: str(getattr(self, f.name)) for f in self.env_fields if getattr(self, f.name)
+        }
 
     @property
     def manifest_path(self) -> str:
         return os.path.join(self.abs_dir_path, self.MANIFEST_FILE)
 
     @property
     def dockerfile_path(self) -> str:
@@ -71,23 +74,36 @@
         for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
             if getattr(method, "is_action", False):
                 methods.append(method)
 
         return methods
 
     def env_value(self, name: str) -> Optional[any]:
-        env_var_value = os.environ.get(name, None)
+        # First, check if there is a matching field with an environment variable in the metadata
+        env_field = next(
+            (f for f in self.env_fields if f.metadata.get("env") == name),
+            None
+        )
+
+        if env_field:
+            # Try casting the environment variable value to a matching field type
+            type_hint = env_field.type.__args__[0] if hasattr(env_field.type, "__args__") else env_field.type
+            env_var_value = config(name, default=None, cast=type_hint) if config(name, default=None) else None
+        else:
+            env_var_value = config(name, default=None)
 
         if env_var_value:
+            # Return a non-None environment variable value
             return env_var_value
+        elif env_field:
+            # Read field value directly
+            return getattr(self, env_field.name)
         else:
-            return next(
-                (getattr(self, f.name) for f in self.env_fields if f.metadata.get("env") == name),
-                None
-            )
+            # If all fails, return None
+            return None
 
     def action_name(self, action: callable) -> str:
         if action is None or not getattr(action, "is_action", False):
             raise Exception("This method is not a tool action.")
         else:
             return action.config["name"]
```

### Comparing `griptape_core-0.9.0/griptape/core/decorators.py` & `griptape_core-0.9.1/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/executors/docker_executor.py` & `griptape_core-0.9.1/griptape/core/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/executors/local_executor.py` & `griptape_core-0.9.1/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/utils/j2.py` & `griptape_core-0.9.1/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/griptape/core/utils/python_runner.py` & `griptape_core-0.9.1/griptape/core/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.9.0/pyproject.toml` & `griptape_core-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.9.0/PKG-INFO` & `griptape_core-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

