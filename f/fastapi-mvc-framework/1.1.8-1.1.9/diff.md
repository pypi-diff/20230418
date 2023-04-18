# Comparing `tmp/fastapi_mvc_framework-1.1.8.tar.gz` & `tmp/fastapi_mvc_framework-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.8.tar", last modified: Wed Apr 12 11:48:39 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.9.tar", last modified: Tue Apr 18 06:29:44 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.8.tar` & `fastapi_mvc_framework-1.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.408079 fastapi_mvc_framework-1.1.8/
--rw-rw-rw-   0        0        0     7266 2023-04-12 11:48:39.407080 fastapi_mvc_framework-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.399123 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      994 2023-04-11 14:13:14.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0    10309 2023-04-11 12:22:29.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     9090 2023-04-10 14:04:09.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     4120 2023-04-12 11:44:55.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3716 2023-04-11 05:08:30.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    13007 2023-04-11 14:01:29.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    11897 2023-04-12 11:38:53.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     2764 2023-04-12 10:01:06.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     5413 2023-04-11 11:47:05.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-12 11:48:39.406085 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     7266 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      273 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-12 11:48:39.000000 fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 11:48:39.408079 fastapi_mvc_framework-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-04-12 11:48:13.000000 fastapi_mvc_framework-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:29:44.831984 fastapi_mvc_framework-1.1.9/
+-rw-rw-rw-   0        0        0     7266 2023-04-18 06:29:44.830487 fastapi_mvc_framework-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4959 2023-04-10 07:40:40.000000 fastapi_mvc_framework-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:29:44.822516 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0     1751 2023-04-13 05:28:34.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0    10362 2023-04-18 05:30:28.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     9090 2023-04-18 05:03:21.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     4120 2023-04-12 11:44:55.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     4182 2023-04-18 06:15:50.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    13005 2023-04-18 06:02:31.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    11961 2023-04-18 06:07:32.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     5731 2023-04-15 08:21:35.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     5673 2023-04-17 07:19:49.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:29:44.829501 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     7266 2023-04-18 06:29:44.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-04-18 06:29:44.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:29:44.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      273 2023-04-18 06:29:44.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-18 06:29:44.000000 fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:29:44.831984 fastapi_mvc_framework-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-04-18 06:29:29.000000 fastapi_mvc_framework-1.1.9/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.8/PKG-INFO` & `fastapi_mvc_framework-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_mvc_framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.8 Summary:
+Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.9 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.8/README.md` & `fastapi_mvc_framework-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,18 +167,20 @@
         if  auth_type.lower()=='public': 
             if userobj:
                 if hasattr(userobj,'token') or token or payload:
                     if payload and token:
                         request.scope['user'] = JWTUser(username=payload[self.username_field], token=token,
                                                         payload=payload)  
                         return True, request.scope['user']
-                else:
-                    return True,None
-            else:
-                return True, None
+            
+            return False,None
+            #     else:
+            #         return True,None
+            # else:
+            #     return True, None
         if  payload:
             user = JWTUser(username=payload[self.username_field], token=token,
                                                         payload=payload) 
             request.scope['user'] = user
             result = _casbin_auth._auth(request=request,username=payload[self.username_field])
             
             return result, user
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,19 +73,29 @@
     setattr(GeneratedController, VER_KEY, version)
 
     return GeneratedController
 
 
 class MvcRouter: 
     """ """
+    @classmethod
+    def init(cls,app):
+        cls.app = app
+
     @staticmethod
     def http(path,methods=['GET'],*args,**kwargs):
         return _route_method(path,method=methods,*args,**kwargs)
     @staticmethod
     def get(path: str, *args, **kwargs): 
+        """if path eq application._public_auth_url,the auth agr must set to 'none' """
+        if MvcRouter.app and path == MvcRouter.app._public_auth_url:
+            if 'auth' in kwargs and kwargs['auth']!='none':
+                raise RuntimeError('the public auth path must set to "none" on auth arguments') 
+            elif not 'auth' in kwargs:
+                 kwargs['auth'] = 'none'
         return _route_method(path, "get", *args, **kwargs)
 
     @staticmethod
     def post(path: str, *args, **kwargs): 
         return _route_method(path, "post", *args, **kwargs)
 
     @staticmethod
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/controller_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         setattr(decorator, METHOD_KEY, method)
         setattr(decorator, ARGS_KEY, args)
         if '__auth_url__' in mwargs: 
             setattr(func,'__auth_url__',mwargs['__auth_url__'])
             del mwargs['__auth_url__']
 
         if not 'auth' in mwargs:
-            mwargs["auth"] = 'public'
+            mwargs["auth"] = 'none'
         setattr(func,AUTH_KEY,mwargs['auth'])
         del mwargs['auth']
         setattr(decorator, KWARGS_KEY, mwargs)
         # setattr(decorator,'__doc__',getattr(func,'__doc__'))
         setattr(decorator, "__signature__", inspect.signature(func))
         return decorator
     return wrapper
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,24 +48,25 @@
 
 __app = MvcApp( ) 
 
 __app_views_dirs = {} 
 __all_controller__ = []
 
 application = __app
+api.init(application)
 
 def __init_database(): 
     db_cfg = config.get("database")
     db_uri:str = db_cfg.get("uri")
     alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
     if db_uri:
         if db_uri.startswith('sqlite'):
             db_directory = os.path.dirname(db_uri.split(':///')[1])
             os.makedirs(db_directory, exist_ok=True) 
-        application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini)
+        application.data_engine=database.init_database(db_uri,__is_debug, alembic_ini,cfg=db_cfg)
 
 def __init_auth(app,auth_type:str):
     __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
     casbin_adapter =  auth._adapters[__type_casbin_adapter] if __type_casbin_adapter in auth._adapters else None
     if not casbin_adapter:
         raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
     
@@ -217,16 +218,18 @@
     ret = func
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
 
 def generate_mvc_app( ):
     global __is_debug
+    _log.disabled = False
+    
     if __is_debug:
-        _log.debug("\n\n=================================generating mvc app===========================================")
+        _log.info("\n\n=================================generating mvc app===========================================")
     if not len(__all_controller__)>0:
         raise "must use @api_route to define a controller class"
     all_routers = []
     all_routers_map = {}
     for ctrl in __all_controller__:
         all_routers.append(register_controllers_to_app(application, ctrl))
     for router in all_routers:
@@ -236,27 +239,27 @@
             auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
             if __is_debug:  
-                _log.debug('{:20}-->{:50}-->{}'.format(str(methods),r.path,funcname) )
+                _log.info('{:20}-->{:50}-->{}'.format(str(methods),r.path,funcname) )
             all_routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
     application.routers_map = all_routers_map  
     midware.init(app=application,debug=__is_debug)
     
     auth_type = config.get("auth",None)
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             application.authObj = __init_auth(application,auth_type)
     __init_database()
     if __is_debug:
-        _log.debug("=================================generating mvc app end===========================================")
+        _log.info("=================================generating mvc app end===========================================")
     return application
 
 def run(app,*args,**kwargs): 
     import uvicorn
     global __is_debug
     host =  "host" in kwargs  and kwargs["host"]  or '0.0.0.0' 
     port = "port" in kwargs  and kwargs["port"] or 8000
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,35 @@
     http_exception_handler,
     request_validation_exception_handler,
 )
 from fastapi.exceptions import RequestValidationError
 from starlette.exceptions import HTTPException as StarletteHTTPException
 import traceback
 from .config import _log,config
-from .midware_session import SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES
-from .view import _View
+from .midware_session import (SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES)
+from fastapi.middleware.cors import CORSMiddleware
 
+from .view import _View
+from .config import config
 
 def init(app :FastAPI,debug:bool = False):
     async def on_startup():
         pass
     app.router.on_startup = [on_startup]
-    # if debug:
-        # from fastapi_utils.timing import add_timing_middleware 
-         
-        # add_timing_middleware(app, record=_log.info, prefix="app", exclude="untimed")
+    
+    cors_cfg = config.get("cors")
+    if cors_cfg:
+        app.add_middleware(
+        CORSMiddleware,
+        allow_origins=cors_cfg.get('allow_origins'),
+        allow_credentials=cors_cfg.get("allow_credentials"),
+        allow_methods=cors_cfg.get("allow_methods",["*"]),
+        allow_headers=cors_cfg.get("allow_headers",["*"]),
+        )
+
 
     #session midware
     _session_cfg:typing.Dict = config.get("session")
     _session_options = {}
     if _session_cfg:
         _storageType=_session_cfg.get("type","")
         if _storageType!="":
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc-framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Description: # fastapi_framework
         A mvc framework used FastApi
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.8 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.9 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: Apache License 2.0 Description: # fastapi_framework A mvc framework
 used FastApi Simple and elegant use of FastApi in MVC mode ## usage: install:
 ```bash pip install fastapi-mvc-framework ``` controller: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
```

### Comparing `fastapi_mvc_framework-1.1.8/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.9/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.8/setup.py` & `fastapi_mvc_framework-1.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     long_description = fh.read()
 with open('requirements.txt', encoding="utf-8-sig") as f:
     requirements = f.readlines()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.8',
+    version='1.1.9',
     license='Apache License 2.0',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
```

