# Comparing `tmp/chatgpt-proxy-0.2.0.tar.gz` & `tmp/chatgpt-proxy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.2.0.tar", last modified: Sun Apr 16 05:27:04 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.2.1.tar", last modified: Tue Apr 18 14:52:54 2023, max compression
```

## Comparing `chatgpt-proxy-0.2.0.tar` & `chatgpt-proxy-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 05:27:04.000000 chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-16 05:26:53.000000 chatgpt-proxy-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:27:04.424574 chatgpt-proxy-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.844480 chatgpt-proxy-0.2.1/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/setup.cfg
```

### Comparing `chatgpt-proxy-0.2.0/LICENSE` & `chatgpt-proxy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.0/PKG-INFO` & `chatgpt-proxy-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-Metadata-Version: 2.1
-Name: chatgpt-proxy
-Version: 0.2.0
-Summary: Reverse proxy for OpenAI chatgpt website API
-Author: 18870
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChatGPT-Proxy
 Python version of OpenAI's ChatGPT web API proxy  
 Python alternative of [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
 Use cookie `cf_clearance` to pass Cloudflare browser check  
 
 **`_puid` no longer works**
 
 ## Requirements
 - Access to chat.openai.com
 
 ## Install
 `pip install chatgpt-proxy`
 
 ## Usage
+
+For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
+
 ### Run as a service
 Set these environment variables:
 - `CF_CLEARANCE`: Cookie `cf_clearance`
 - `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
+- `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
+    requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
+mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
 
 Then run: `python -m chatgpt_proxy`  
 
 #### Success
@@ -86,8 +82,8 @@
 ## License
 This work is licensed under the [GNU Affero General Public License v3.0](/LICENSE) or later, with the "CHATGPT-PROXY" exception.
 
 > **"CHATGPT-PROXY" EXCEPTION TO THE AGPL**
 >
 > As a special exception, using this work in the following ways does not cause your program to be covered by the AGPL:
 > 1. Bundling the unaltered code or binary of this work in your program; or
-> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
+> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
```

### Comparing `chatgpt-proxy-0.2.0/README.md` & `chatgpt-proxy-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,56 @@
+Metadata-Version: 2.1
+Name: chatgpt-proxy
+Version: 0.2.1
+Summary: Reverse proxy for OpenAI chatgpt website API
+Author: 18870
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ChatGPT-Proxy
 Python version of OpenAI's ChatGPT web API proxy  
 Python alternative of [ChatGPT-Proxy-V4](https://github.com/acheong08/ChatGPT-Proxy-V4)  
 Use cookie `cf_clearance` to pass Cloudflare browser check  
 
 **`_puid` no longer works**
 
 ## Requirements
 - Access to chat.openai.com
 
 ## Install
 `pip install chatgpt-proxy`
 
 ## Usage
+
+For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
+
 ### Run as a service
 Set these environment variables:
 - `CF_CLEARANCE`: Cookie `cf_clearance`
 - `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
+- `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
+    requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
+mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
 
 Then run: `python -m chatgpt_proxy`  
 
 #### Success
@@ -76,8 +92,8 @@
 ## License
 This work is licensed under the [GNU Affero General Public License v3.0](/LICENSE) or later, with the "CHATGPT-PROXY" exception.
 
 > **"CHATGPT-PROXY" EXCEPTION TO THE AGPL**
 >
 > As a special exception, using this work in the following ways does not cause your program to be covered by the AGPL:
 > 1. Bundling the unaltered code or binary of this work in your program; or
-> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
+> 2. Interacting with this work through the provided inter-process communication interface, such as the HTTP API.
```

### Comparing `chatgpt-proxy-0.2.0/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.2.1/chatgpt_proxy/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import asyncio
 import logging
-import os
 from contextlib import asynccontextmanager
 
 import uvicorn
-from fastapi import FastAPI
-from pydantic import BaseSettings, Field
+from fastapi import FastAPI, Header
+from pydantic import BaseModel, BaseSettings, Field
 
 from chatgpt_proxy.proxy import WebChatGPTProxy
 
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     handlers=[logging.StreamHandler()],
 )
 
+logger = logging.getLogger(__name__)
+
 
 class Settings(BaseSettings):
     cf_clearance: str
     user_agent: str
 
     access_token: str = None
     host: str = "127.0.0.1"
     port: int = 7800
     trust: bool = Field(default=False, env="proxy_trust_client")
+    mod_access_token: str = None
 
     class Config:
         env_file = '.env'
 
 
 if __name__ == "__main__":
     env = Settings()
@@ -42,8 +44,30 @@
     async def lifespan(app: FastAPI):
         refresh_puid_task = asyncio.create_task(proxy._refresh_task())
         yield
 
     app = FastAPI(lifespan=lifespan)
     proxy.attach(app, path="/backend-api")
 
+    if env.mod_access_token:
+        logger.info("Mod access token found, enable /moderation/update_info endpoint")
+
+        class Info(BaseModel):
+            cf_clearance: str = None
+            access_token: str = None
+
+        @app.post("/moderation/update_info", status_code=200)
+        async def update_info(info: Info, authorization: str = Header(...)):
+            if authorization == env.mod_access_token:
+                if info.access_token:
+                    logger.info("New access token found")
+                    proxy.access_token = info.access_token
+                if info.cf_clearance:
+                    logger.info(f"New cf_clearance: {info.cf_clearance}")
+                    proxy.cf_clearance = info.cf_clearance
+            if await proxy._refresh_puid():
+                logger.info("New info is validated")
+            else:
+                logger.error("Failed to validate new info")
+            return {"status": "ok"}
+
     uvicorn.run(app, host=env.host, port=env.port)
```

### Comparing `chatgpt-proxy-0.2.0/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.2.1/chatgpt_proxy/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 from typing import Optional
 from urllib.parse import urlparse, urlunparse, ParseResult
 
 import httpx
 from fastapi import FastAPI
 from starlette.requests import Request
@@ -56,14 +55,15 @@
         headers["host"] = self._domain
         headers["origin"] = self._origin
         headers["referer"] = self.base_url
         return headers
 
     async def proxy(self, request: Request, path: str):
         # https://github.com/tiangolo/fastapi/discussions/7382#discussioncomment-5136454
+        logger.info(f"Proxying {request.method} {request.url}")
         rp_resp = await self._send_request(
             path=path,
             query=request.url.query.encode("utf-8"),
             method=request.method,
             headers=await self._prepare_headers(request),
             cookies=await self._prepare_cookies(request),
             content=request.stream(),
@@ -125,21 +125,21 @@
         cookies = await super()._prepare_cookies(request)
         cookies.setdefault("cf_clearance", self.cf_clearance)
         return cookies
 
     async def _prepare_headers(self, request: Request):
         headers = await super()._prepare_headers(request)
         headers["origin"] = "https://chat.openai.com"
-        headers["referer"] = "https://chat.openai.com/chat"
+        headers["referer"] = "https://chat.openai.com"
         headers["user-agent"] = self.ua
         if self.trust and self.access_token:
             headers.setdefault("authorization", f"Bearer {self.access_token}")
         return headers
 
-    async def _refresh_puid(self) -> None:
+    async def _refresh_puid(self) -> bool:
         """
         Send requests to /models through reverse proxy (current FastAPI app) to get a new puid
         
         Use to see if you pass cloudflare
         """
         if self._app is None:
             logger.info("Not attached to any FastAPI app, skip")
@@ -147,20 +147,22 @@
             app=self._app, base_url=f"https://chat.openai.com{self._path}"
         ) as client:
             resp = await client.get(
                 "/models", headers={"authorization": f"Bearer {self.access_token}"}
             )
             puid = resp.cookies.get("_puid")
             if puid:
-                logger.info(f"puid: {puid}")
+                logger.info(f"puid: {puid[:15]}...{puid[30:40]}...")
                 self.puid = puid
+                return True
             else:
                 logger.error("Failed to get puid")
                 logger.error(f"Cookies: {resp.cookies}")
                 logger.error(f"Response: \n{resp.text}")
+                return False
 
     async def _refresh_task(self) -> None:
         if self.access_token is None:
             logger.info("access_token not found, skip")
             return
 
         try:
```

### Comparing `chatgpt-proxy-0.2.0/chatgpt_proxy.egg-info/PKG-INFO` & `chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,33 +18,39 @@
 ## Requirements
 - Access to chat.openai.com
 
 ## Install
 `pip install chatgpt-proxy`
 
 ## Usage
+
+For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
+
 ### Run as a service
 Set these environment variables:
 - `CF_CLEARANCE`: Cookie `cf_clearance`
 - `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
+- `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
+    requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
+mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
 
 Then run: `python -m chatgpt_proxy`  
 
 #### Success
```

