# Comparing `tmp/langcorn-0.0.4.tar.gz` & `tmp/langcorn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.4.tar", max compression
+gzip compressed data, was "langcorn-0.0.5.tar", max compression
```

## Comparing `langcorn-0.0.4.tar` & `langcorn-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-04-15 10:21:27.252307 langcorn-0.0.4/LICENSE
--rw-r--r--   0        0        0     4011 2023-04-15 10:21:27.252307 langcorn-0.0.4/Readme.md
--rw-r--r--   0        0        0       77 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/__init__.py
--rw-r--r--   0        0        0      417 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/__init__.py
--rw-r--r--   0        0        0     2267 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/api.py
--rw-r--r--   0        0        0      825 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/test_api.py
--rw-r--r--   0        0        0      944 2023-04-15 10:21:27.252307 langcorn-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4993 1970-01-01 00:00:00.000000 langcorn-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-18 11:39:47.784152 langcorn-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4847 2023-04-18 11:39:47.784152 langcorn-0.0.5/Readme.md
+-rw-r--r--   0        0        0       77 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     3156 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/api.py
+-rw-r--r--   0        0        0      825 2023-04-18 11:39:47.784152 langcorn-0.0.5/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      944 2023-04-18 11:39:47.784152 langcorn-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 langcorn-0.0.5/PKG-INFO
```

### Comparing `langcorn-0.0.4/LICENSE` & `langcorn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.4/Readme.md` & `langcorn-0.0.5/Readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -48,17 +48,20 @@
 
 Run your LangCorn FastAPI server:
 
 ```shell
 langcorn server examples.ex1:chain
 
 
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
-INFO:     Started server process [87033]
+[INFO] 2023-04-18 14:34:56.32 | api:create_service:75 | Creating service
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:85 | lang_app='examples.ex1:chain':LLMChain(['product'])
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:104 | Serving
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:106 | Endpoint: /docs
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:106 | Endpoint: /examples.ex1/run
+INFO:     Started server process [27843]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 or as an alternative
 
@@ -69,19 +72,22 @@
 
 Run multiple chains
 
 ```shell
 python -m langcorn server examples.ex1:chain examples.ex2:chain
 
 
-
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex2/run
-INFO:     Started server process [87033]
+[INFO] 2023-04-18 14:35:21.11 | api:create_service:75 | Creating service
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:85 | lang_app='examples.ex1:chain':LLMChain(['product'])
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:85 | lang_app='examples.ex2:chain':SimpleSequentialChain(['input'])
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:104 | Serving
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /docs
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /examples.ex1/run
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /examples.ex2/run
+INFO:     Started server process [27863]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 Import the necessary packages and create your FastAPI app:
 
@@ -108,14 +114,19 @@
 ```shell
 
 uvicorn main:app --host 0.0.0.0 --port 8000
 ```
 
 Now, your LangChain models and pipelines are accessible via the LangCorn API server.
 
+## Docs
+
+Automatically served FastAPI doc
+![](https://res.cloudinary.com/dq0w2rtm9/image/upload/c_pad,b_auto:predominant,fl_preserve_transparency/v1681817836/Screen_Shot_2023-04-18_at_14.36.00_ms2thb.jpg?_s=public-apps)
+
 ## Auth
 
 It possible to add a static api token auth by specifying `auth_token`
 
 ```shell
 python langcorn server examples.ex1:chain examples.ex2:chain --auth_token=api-secret-value
 ```
```

### Comparing `langcorn-0.0.4/langcorn/server/api.py` & `langcorn-0.0.5/langcorn/server/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,41 +40,66 @@
             logger.info("Authorized using integration token")
             return
         raise HTTPException(status_code=401, detail="Token verification failed")
 
     return verify_auth
 
 
+def derive_fields(language_app) -> (list[str], list[str]):
+    if hasattr(language_app, "input_variables"):
+        return language_app.input_variables, language_app.output_variables
+    elif hasattr(language_app, "prompt"):
+        return language_app.prompt.input_variables, [language_app.output_key]
+    return [language_app.input_key], ["output"]
+
+
+def derive_class(name, fields):
+    return type(
+        f"Lang{name}", (BaseModel,), {"__annotations__": {f: str for f in fields}}
+    )
+
+
+def make_handler(request_cls, chain):
+    async def handler(
+        request: request_cls,
+    ):
+        output = chain.run(request.dict())
+        # add error handling
+        return LangResponse(output=output, error="")
+
+    return handler
+
+
 def create_service(*lc_apps, auth_token: str = ""):
     # Make local modules discoverable
     sys.path.append(os.path.dirname(__file__))
     logger.info("Creating service")
     app = FastAPI()
     endpoints = ["/docs"]
 
     _authenticate_or_401 = Depends(authenticate_or_401(auth_token=auth_token))
 
     for lang_app in lc_apps:
         chain = import_from_string(lang_app)
-        logger.info(f"{lang_app=}")
-        logger.info(f"{chain=}")
+        inn, out = derive_fields(chain)
+        logger.debug(f"inputs:{inn=}")
+        logger.info(f"{lang_app=}:{chain.__class__.__name__}({inn})")
         endpoint_prefix = lang_app.split(":")[0]
-        endpoints.append(f"/{endpoint_prefix}/run")
+        cls_name = "".join([c.capitalize() for c in endpoint_prefix.split(".")])
+        request_cls = derive_class(cls_name, inn)
+        logger.debug(f"{request_cls=}")
 
-        @app.post(
+        endpoints.append(f"/{endpoint_prefix}/run")
+        # avoid hoisting issues with handler(request)
+        app.post(
             f"/{endpoint_prefix}/run",
             response_model=LangResponse,
             dependencies=[_authenticate_or_401],
-        )
-        async def predict_sync(
-            request: LangRequest,
-        ):
-            output = chain.run(request.prompt)
-            # add error handling
-            return LangResponse(output=output, error="")
+            name=lang_app,
+        )(make_handler(request_cls, chain))
 
     @app.get("/ht")
     async def health_check():
         return dict(functions=[*lc_apps])
 
     logger.info("Serving")
     for endpoint in endpoints:
```

### Comparing `langcorn-0.0.4/langcorn/server/test_api.py` & `langcorn-0.0.5/langcorn/server/test_api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.4/pyproject.toml` & `langcorn-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
@@ -16,15 +16,15 @@
 [tool.poetry.scripts]
 langcorn = "langcorn.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0.92.0"
 uvicorn = "^0.20.0"
-langchain = "^0.0.131"
+langchain = "^0.0.139"
 openai = "^0.27.2"
 fire = "^0.5.0"
 loguru = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
```

### Comparing `langcorn-0.0.4/PKG-INFO` & `langcorn-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: langchain (>=0.0.131,<0.0.132)
+Requires-Dist: langchain (>=0.0.139,<0.0.140)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Project-URL: Repository, https://github.com/msoedov/langcorn
 Description-Content-Type: text/markdown
 
 # Langcorn
@@ -74,17 +74,20 @@
 
 Run your LangCorn FastAPI server:
 
 ```shell
 langcorn server examples.ex1:chain
 
 
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
-INFO:     Started server process [87033]
+[INFO] 2023-04-18 14:34:56.32 | api:create_service:75 | Creating service
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:85 | lang_app='examples.ex1:chain':LLMChain(['product'])
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:104 | Serving
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:106 | Endpoint: /docs
+[INFO] 2023-04-18 14:34:57.51 | api:create_service:106 | Endpoint: /examples.ex1/run
+INFO:     Started server process [27843]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 or as an alternative
 
@@ -95,19 +98,22 @@
 
 Run multiple chains
 
 ```shell
 python -m langcorn server examples.ex1:chain examples.ex2:chain
 
 
-
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
-[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex2/run
-INFO:     Started server process [87033]
+[INFO] 2023-04-18 14:35:21.11 | api:create_service:75 | Creating service
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:85 | lang_app='examples.ex1:chain':LLMChain(['product'])
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:85 | lang_app='examples.ex2:chain':SimpleSequentialChain(['input'])
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:104 | Serving
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /docs
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /examples.ex1/run
+[INFO] 2023-04-18 14:35:21.82 | api:create_service:106 | Endpoint: /examples.ex2/run
+INFO:     Started server process [27863]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 Import the necessary packages and create your FastAPI app:
 
@@ -134,14 +140,19 @@
 ```shell
 
 uvicorn main:app --host 0.0.0.0 --port 8000
 ```
 
 Now, your LangChain models and pipelines are accessible via the LangCorn API server.
 
+## Docs
+
+Automatically served FastAPI doc
+![](https://res.cloudinary.com/dq0w2rtm9/image/upload/c_pad,b_auto:predominant,fl_preserve_transparency/v1681817836/Screen_Shot_2023-04-18_at_14.36.00_ms2thb.jpg?_s=public-apps)
+
 ## Auth
 
 It possible to add a static api token auth by specifying `auth_token`
 
 ```shell
 python langcorn server examples.ex1:chain examples.ex2:chain --auth_token=api-secret-value
 ```
```

