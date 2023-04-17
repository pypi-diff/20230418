# Comparing `tmp/autoplugin-0.1.2.tar.gz` & `tmp/autoplugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplugin-0.1.2.tar", last modified: Mon Apr 17 21:10:46 2023, max compression
+gzip compressed data, was "autoplugin-0.1.3.tar", last modified: Mon Apr 17 22:42:28 2023, max compression
```

## Comparing `autoplugin-0.1.2.tar` & `autoplugin-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.201649 autoplugin-0.1.2/
--rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.2/LICENSE
--rw-r--r--   0 suvansh    (501) staff       (20)     5405 2023-04-17 21:10:46.201474 autoplugin-0.1.2/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)     4552 2023-04-17 21:07:05.000000 autoplugin-0.1.2/README.md
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.200250 autoplugin-0.1.2/autoplugin/
--rw-r--r--   0 suvansh    (501) staff       (20)       50 2023-04-17 18:44:53.000000 autoplugin-0.1.2/autoplugin/__init__.py
--rw-r--r--   0 suvansh    (501) staff       (20)     8789 2023-04-17 20:59:08.000000 autoplugin-0.1.2/autoplugin/autoplugin.py
--rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-04-14 20:36:12.000000 autoplugin-0.1.2/autoplugin/testing.py
-drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 21:10:46.201199 autoplugin-0.1.2/autoplugin.egg-info/
--rw-r--r--   0 suvansh    (501) staff       (20)     5405 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/PKG-INFO
--rw-r--r--   0 suvansh    (501) staff       (20)      265 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/SOURCES.txt
--rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/dependency_links.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/requires.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-04-17 21:10:46.000000 autoplugin-0.1.2/autoplugin.egg-info/top_level.txt
--rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-04-17 21:10:46.201703 autoplugin-0.1.2/setup.cfg
--rw-r--r--   0 suvansh    (501) staff       (20)     1200 2023-04-17 21:10:25.000000 autoplugin-0.1.2/setup.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.476311 autoplugin-0.1.3/
+-rw-r--r--   0 suvansh    (501) staff       (20)     1492 2023-04-17 18:30:44.000000 autoplugin-0.1.3/LICENSE
+-rw-r--r--   0 suvansh    (501) staff       (20)     7334 2023-04-17 22:42:28.476128 autoplugin-0.1.3/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)     6481 2023-04-17 22:37:50.000000 autoplugin-0.1.3/README.md
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.474535 autoplugin-0.1.3/autoplugin/
+-rw-r--r--   0 suvansh    (501) staff       (20)       81 2023-04-17 22:27:43.000000 autoplugin-0.1.3/autoplugin/__init__.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     9781 2023-04-17 22:30:01.000000 autoplugin-0.1.3/autoplugin/autoplugin.py
+-rw-r--r--   0 suvansh    (501) staff       (20)      546 2023-04-17 22:27:27.000000 autoplugin-0.1.3/autoplugin/basic_app.py
+-rw-r--r--   0 suvansh    (501) staff       (20)     1179 2023-04-14 20:36:12.000000 autoplugin-0.1.3/autoplugin/testing.py
+drwxr-xr-x   0 suvansh    (501) staff       (20)        0 2023-04-17 22:42:28.475822 autoplugin-0.1.3/autoplugin.egg-info/
+-rw-r--r--   0 suvansh    (501) staff       (20)     7334 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/PKG-INFO
+-rw-r--r--   0 suvansh    (501) staff       (20)      289 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)        1 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       58 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/requires.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       11 2023-04-17 22:42:28.000000 autoplugin-0.1.3/autoplugin.egg-info/top_level.txt
+-rw-r--r--   0 suvansh    (501) staff       (20)       38 2023-04-17 22:42:28.476367 autoplugin-0.1.3/setup.cfg
+-rw-r--r--   0 suvansh    (501) staff       (20)     1200 2023-04-17 22:42:21.000000 autoplugin-0.1.3/setup.py
```

### Comparing `autoplugin-0.1.2/LICENSE` & `autoplugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.2/PKG-INFO` & `autoplugin-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
@@ -33,85 +33,115 @@
 ```bash
 pip install autoplugin
 ```
 
 To install with the ability to generate endpoint descriptions for the OpenAPI specification automatically from source code, install with
 
 ```bash
-pip install autoplugin[gen]
+pip install 'autoplugin[gen]'
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
-1. Import the necessary functions from AutoPlugin and FastAPI:
+1. Import the necessary functions from AutoPlugin:
 ```python
-from autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin import register, generate, launch, get_app
 ```
 
-2. Create a FastAPI app instance:
+2. Create an app instance, backed by FastAPI:
 ```python
-app = FastAPI()
+app = get_app()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
+AutoPlugin will automatically generate descriptions if needed.
 ```python
 @register(app, methods=["GET"])
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
-generate(app)  # generated files saved to `.well-known/` directory
+# generated files saved to `.well-known/` directory
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
 launch(app)  # API hosted at localhost:8000
 ```
 
+6. Follow the [instructions](https://platform.openai.com/docs/plugins/getting-started/running-a-plugin) to run a custom plugin:
+- On ChatGPT, make a new chat.
+- Under "Models" select "Plugins"
+- In the Plugins dropdown, select "Plugin store"
+- Click "Develop your own plugin"
+- Enter the URL you're running the server at ("localhost:8000" by default) and hit enter.
+- Click "Install localhost plugin" 
+
 
 ## Example
 
 Here's a complete example that demonstrates how to use AutoPlugin to create API endpoints for two functions, `hello` and `add`.
 It also generates the `openapi.yaml` and `ai-plugin.json` files, by default in the `.well-known` directory. :
 ```python
-from autoplugin.autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin.autoplugin import register, generate, launch, get_app
 
-app = FastAPI()
+app = get_app()
 
 @register(app, methods=["GET", "POST"])
 async def hello(name: str, age: int = 5) -> str:
     return f"Hello, {name}! Age {age}."
 
 @register(app, methods=["GET"])
 async def add(a: int, b: int) -> int:
     """ Adds two numbers """
     return a + b
 
 
 # Generate the necessary files
-generate(app)
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
+## The `@register` Decorator
+The `@register` decorator is used as follows:
+```python
+@register(app: FastAPI,
+            methods: List[str],                     # which HTTP methods to support
+            description: Optional[str],             # if provided, used as is
+            generate_description: Optional[bool])   # whether to autogenerate a description
+def my_func(...):
+    ...
+```
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
+By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
+
+
+## The `generate` Function
+The `generate` function has the following signature:
+```python
+def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+```
+The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
+
+All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+
 
 ## Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
```

### Comparing `autoplugin-0.1.2/README.md` & `autoplugin-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,85 +12,115 @@
 ```bash
 pip install autoplugin
 ```
 
 To install with the ability to generate endpoint descriptions for the OpenAPI specification automatically from source code, install with
 
 ```bash
-pip install autoplugin[gen]
+pip install 'autoplugin[gen]'
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
-1. Import the necessary functions from AutoPlugin and FastAPI:
+1. Import the necessary functions from AutoPlugin:
 ```python
-from autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin import register, generate, launch, get_app
 ```
 
-2. Create a FastAPI app instance:
+2. Create an app instance, backed by FastAPI:
 ```python
-app = FastAPI()
+app = get_app()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
+AutoPlugin will automatically generate descriptions if needed.
 ```python
 @register(app, methods=["GET"])
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
-generate(app)  # generated files saved to `.well-known/` directory
+# generated files saved to `.well-known/` directory
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
 launch(app)  # API hosted at localhost:8000
 ```
 
+6. Follow the [instructions](https://platform.openai.com/docs/plugins/getting-started/running-a-plugin) to run a custom plugin:
+- On ChatGPT, make a new chat.
+- Under "Models" select "Plugins"
+- In the Plugins dropdown, select "Plugin store"
+- Click "Develop your own plugin"
+- Enter the URL you're running the server at ("localhost:8000" by default) and hit enter.
+- Click "Install localhost plugin" 
+
 
 ## Example
 
 Here's a complete example that demonstrates how to use AutoPlugin to create API endpoints for two functions, `hello` and `add`.
 It also generates the `openapi.yaml` and `ai-plugin.json` files, by default in the `.well-known` directory. :
 ```python
-from autoplugin.autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin.autoplugin import register, generate, launch, get_app
 
-app = FastAPI()
+app = get_app()
 
 @register(app, methods=["GET", "POST"])
 async def hello(name: str, age: int = 5) -> str:
     return f"Hello, {name}! Age {age}."
 
 @register(app, methods=["GET"])
 async def add(a: int, b: int) -> int:
     """ Adds two numbers """
     return a + b
 
 
 # Generate the necessary files
-generate(app)
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
+## The `@register` Decorator
+The `@register` decorator is used as follows:
+```python
+@register(app: FastAPI,
+            methods: List[str],                     # which HTTP methods to support
+            description: Optional[str],             # if provided, used as is
+            generate_description: Optional[bool])   # whether to autogenerate a description
+def my_func(...):
+    ...
+```
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
+By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
+
+
+## The `generate` Function
+The `generate` function has the following signature:
+```python
+def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+```
+The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
+
+All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+
 
 ## Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
```

### Comparing `autoplugin-0.1.2/autoplugin/autoplugin.py` & `autoplugin-0.1.3/autoplugin/autoplugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 import functools
 import os
 from os.path import join
 import inspect
 from typing import Callable, List, Dict, Any, Optional
 from fastapi import FastAPI, Depends
+from fastapi.middleware.cors import CORSMiddleware
+from fastapi.responses import PlainTextResponse
 import uvicorn
 from pydantic import BaseModel, create_model
 from fastapi.openapi.utils import get_openapi
 import yaml
 import json
 
 
@@ -24,23 +26,32 @@
 def launch(app: FastAPI, host="127.0.0.1", port=8000):
     uvicorn.run(app, host=host, port=port)
 
 
 def generate(app: FastAPI, out_dir=".well-known", **kwargs):
     """ kwargs should be key-value pairs for the plugin_spec json """
     os.makedirs(out_dir, exist_ok=True)
+
+    """ OpenAPI spec """
     openapi = get_openapi(
         title="Custom ChatGPT Plugin",
         version="1.0.0",
         routes=app.routes,
     )
 
     with open(join(out_dir, "openapi.yaml"), "w") as openapi_yaml:
         yaml.dump(openapi, openapi_yaml, sort_keys=False)
+    
+    @app.get("/openapi.yaml", response_class=PlainTextResponse)
+    async def get_openapi_yaml():
+        with open(join(out_dir, "openapi.yaml"), "r") as f:
+            content = f.read()
+        return content
 
+    """ Plugin manifest file """
     plugin_spec = {
         "name_for_human": "Custom Plugin",
         "name_for_model": "Custom Plugin",
         "description_for_human": "Unspecified custom plugin. Add behavior here.",
         "description_for_model": "Unspecified custom plugin. Add behavior here.",
         "schema_version": "v1",
         "auth": {
@@ -51,26 +62,40 @@
             "url": "http://localhost:8000/openapi.yaml",
             "is_user_authenticated": False
         },
         "logo_url": "http://example.com/logo.png",
         "contact_email": "support@example.com",
         "legal_info_url": "http://www.example.com/legal"
     }
+    if "name" in kwargs:
+        plugin_name = kwargs.pop("name")
+        plugin_spec["name_for_human"] = plugin_name
+        plugin_spec["name_for_model"] = plugin_name
+    if "description" in kwargs:
+        plugin_description = kwargs.pop("description")
+        plugin_spec["description_for_human"] = plugin_description
+        plugin_spec["description_for_model"] = plugin_description
     plugin_spec.update(kwargs)
 
     # character limit checks
     _plugin_check_limit(plugin_spec, "name_for_human", 50)
     _plugin_check_limit(plugin_spec, "name_for_model", 50)
     _plugin_check_limit(plugin_spec, "description_for_human", 120)
     _plugin_check_limit(plugin_spec, "description_for_model",
                        8000)  # will decrease over time
 
     with open(join(out_dir, "ai-plugin.json"), "w") as plugin_json:
         json.dump(plugin_spec, plugin_json, indent=4)
 
+    @app.get("/.well-known/ai-plugin.json", response_class=PlainTextResponse)
+    async def get_plugin_json():
+        with open(join(out_dir, "ai-plugin.json"), "r") as f:
+            content = f.read()
+        return content
+
 
 def register(app: FastAPI,
              func: Callable = None,
              *,
              methods: List[str] = None,
              description: Optional[str] = None,
              generate_description: Optional[bool] = None,
```

### Comparing `autoplugin-0.1.2/autoplugin/testing.py` & `autoplugin-0.1.3/autoplugin/testing.py`

 * *Files identical despite different names*

### Comparing `autoplugin-0.1.2/autoplugin.egg-info/PKG-INFO` & `autoplugin-0.1.3/autoplugin.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create ChatGPT plugins from Python code
 Home-page: https://github.com/suvansh/autoplugin
 Author: Suvansh Sanjeev
 Author-email: suvansh@brilliantly.ai
 Project-URL: Tracker, https://github.com/suvansh/autoplugin/issues
 Project-URL: Source, https://github.com/suvansh/autoplugin/
 Project-URL: Documentation, https://github.com/suvansh/AutoPlugin/blob/main/README.md
@@ -33,85 +33,115 @@
 ```bash
 pip install autoplugin
 ```
 
 To install with the ability to generate endpoint descriptions for the OpenAPI specification automatically from source code, install with
 
 ```bash
-pip install autoplugin[gen]
+pip install 'autoplugin[gen]'
 ```
 
 ## Basic Usage
 To get started with AutoPlugin, follow these steps:
 
-1. Import the necessary functions from AutoPlugin and FastAPI:
+1. Import the necessary functions from AutoPlugin:
 ```python
-from autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin import register, generate, launch, get_app
 ```
 
-2. Create a FastAPI app instance:
+2. Create an app instance, backed by FastAPI:
 ```python
-app = FastAPI()
+app = get_app()
 ```
 
 3. Use the register decorator to register your functions as API endpoints.
-AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints.
-By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires setting the `OPENAI_API_KEY` environment variable).
-Finally, you can specify a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) by passing the `description` keyword argument.
+AutoPlugin will automatically generate descriptions if needed.
 ```python
 @register(app, methods=["GET"])
 async def get_order(name: str) -> str:
     order = await get_order_from_db(name)
     return f"Order for {name}: {order}"
 # Generated description: "Retrieves an order from the database for a given name."
 ```
 
 4. Generate the necessary files (`openapi.yaml` and `ai-plugin.json`) for your ChatGPT plugin.
 Optionally, specify `out_dir` to change where they're saved to:
 ```python
-generate(app)  # generated files saved to `.well-known/` directory
+# generated files saved to `.well-known/` directory
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 ```
 
 5. Launch the server. Optionally, specify `host` and `port`:
 ```python
 launch(app)  # API hosted at localhost:8000
 ```
 
+6. Follow the [instructions](https://platform.openai.com/docs/plugins/getting-started/running-a-plugin) to run a custom plugin:
+- On ChatGPT, make a new chat.
+- Under "Models" select "Plugins"
+- In the Plugins dropdown, select "Plugin store"
+- Click "Develop your own plugin"
+- Enter the URL you're running the server at ("localhost:8000" by default) and hit enter.
+- Click "Install localhost plugin" 
+
 
 ## Example
 
 Here's a complete example that demonstrates how to use AutoPlugin to create API endpoints for two functions, `hello` and `add`.
 It also generates the `openapi.yaml` and `ai-plugin.json` files, by default in the `.well-known` directory. :
 ```python
-from autoplugin.autoplugin import register, generate, launch
-from fastapi import FastAPI
+from autoplugin.autoplugin import register, generate, launch, get_app
 
-app = FastAPI()
+app = get_app()
 
 @register(app, methods=["GET", "POST"])
 async def hello(name: str, age: int = 5) -> str:
     return f"Hello, {name}! Age {age}."
 
 @register(app, methods=["GET"])
 async def add(a: int, b: int) -> int:
     """ Adds two numbers """
     return a + b
 
 
 # Generate the necessary files
-generate(app)
+generate(app, name="Example", description="Plugin to add numbers or greet users")
 
 # Launch the server
 launch(app)
 ```
 
 This example creates a FastAPI server with two endpoints, `/hello` and `/add`, that can be accessed using GET or POST requests.
 AutoPlugin will use the docstring for the OpenAPI description of `/add` and generate an automatic description for `/hello` by passing the source code of the function to OpenAI's API.
 
+## The `@register` Decorator
+The `@register` decorator is used as follows:
+```python
+@register(app: FastAPI,
+            methods: List[str],                     # which HTTP methods to support
+            description: Optional[str],             # if provided, used as is
+            generate_description: Optional[bool])   # whether to autogenerate a description
+def my_func(...):
+    ...
+```
+AutoPlugin generates function descriptions in the OpenAPI spec so that ChatGPT knows how to use your endpoints. There are a few keyword arguments to customize the behavior of this generation
+By default, the description is fetched from the docstring. If there's no docstring, or if you specify `generate_description=True`, AutoPlugin will generate one automatically from OpenAI's API (requires the LangChain package and setting the `OPENAI_API_KEY` environment variable).
+Finally, you can override the description generation behavior by specifying a description (e.g. if the docstring contains extra information not needed in the OpenAPI description) in the `description` keyword argument.
+
+
+## The `generate` Function
+The `generate` function has the following signature:
+```python
+def generate(app: FastAPI, out_dir: str=".well-known", **kwargs):
+```
+The `out_dir` keyword argument determines where the `ai-plugin.json` and `openapi.yaml` files are saved upon generation.
+
+All other keyword arguments are used to customize fields of the [plugin manifest file](https://platform.openai.com/docs/plugins/getting-started/plugin-manifest).
+The `name` keyword argument can be used for convenience to update both `name_for_human` and `name_for_model` at once. Same for `description`. In a future update, these can be automatically generated to further streamline the deployment process. Keep in mind the [best practices](https://platform.openai.com/docs/plugins/getting-started/writing-descriptions) for descriptions.
+
 
 ## Testing
 AutoPlugin also provides a `testing_server` utility (courtesy of [florimondmanca](https://github.com/encode/uvicorn/issues/742#issuecomment-674411676)) for testing your endpoints. Here's an example of how you can use it to test the `/hello` and `/add` endpoints from the example above:
 ```python
 from autoplugin.testing import testing_server
 from os.path import join
 import requests
```

### Comparing `autoplugin-0.1.2/setup.py` & `autoplugin-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autoplugin",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "fastapi",
         "pydantic",
         "uvicorn",
         "requests",
         "PyYAML",
```

