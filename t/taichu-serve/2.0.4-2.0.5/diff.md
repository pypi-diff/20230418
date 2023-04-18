# Comparing `tmp/taichu-serve-2.0.4.tar.gz` & `tmp/taichu-serve-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.4.tar", last modified: Tue Apr 18 03:03:30 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.5.tar", last modified: Tue Apr 18 09:08:31 2023, max compression
```

## Comparing `taichu-serve-2.0.4.tar` & `taichu-serve-2.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 03:03:30.748773 taichu-serve-2.0.4/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-18 03:03:30.748615 taichu-serve-2.0.4/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-18 03:03:30.748818 taichu-serve-2.0.4/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-18 03:03:15.000000 taichu-serve-2.0.4/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 03:03:30.745313 taichu-serve-2.0.4/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.4/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.4/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     2572 2023-04-18 02:59:42.000000 taichu-serve-2.0.4/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.4/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.4/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.4/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.4/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.4/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.4/taichu_serve/log.py
--rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.4/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.4/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     2079 2023-04-18 01:38:35.000000 taichu-serve-2.0.4/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 03:03:30.747377 taichu-serve-2.0.4/taichu_serve/template/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.4/taichu_serve/template/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 03:02:30.000000 taichu-serve-2.0.4/taichu_serve/template/config.ini
--rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.4/taichu_serve/template/customize_service.py
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.4/taichu_serve/template/requirements.txt
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 03:03:30.748305 taichu-serve-2.0.4/taichu_serve/template/test/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.4/taichu_serve/template/test/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)      665 2023-04-18 03:02:30.000000 taichu-serve-2.0.4/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 chen       (501) staff       (20)      255 2023-04-18 03:02:30.000000 taichu-serve-2.0.4/taichu_serve/template/test/http_client.py
--rw-r--r--   0 chen       (501) staff       (20)      906 2023-04-18 01:38:35.000000 taichu-serve-2.0.4/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 03:03:30.746509 taichu-serve-2.0.4/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      873 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:03:30.000000 taichu-serve-2.0.4/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 09:08:31.995336 taichu-serve-2.0.5/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-18 09:08:31.995179 taichu-serve-2.0.5/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-18 09:08:31.995378 taichu-serve-2.0.5/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-18 09:06:17.000000 taichu-serve-2.0.5/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 09:08:31.991982 taichu-serve-2.0.5/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.5/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.5/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     2729 2023-04-18 03:30:42.000000 taichu-serve-2.0.5/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.5/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.5/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.5/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.5/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.5/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.5/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.5/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.5/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2079 2023-04-18 08:48:18.000000 taichu-serve-2.0.5/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 09:08:31.993976 taichu-serve-2.0.5/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.5/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.5/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.5/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.5/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 09:08:31.994961 taichu-serve-2.0.5/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.5/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.5/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.5/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.5/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-18 09:08:31.993170 taichu-serve-2.0.5/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      873 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 09:08:31.000000 taichu-serve-2.0.5/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.4/setup.py` & `taichu-serve-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name = 'taichu-serve'
 
     requirements = ['grpcio', 'grpcio-tools', 'protobuf',
                     'Flask', 'gunicorn', 'requests']
 
     setup(
         name=name,
-        version='2.0.4',
+        version='2.0.5',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
```

### Comparing `taichu-serve-2.0.4/taichu_serve/__init__.py` & `taichu-serve-2.0.5/taichu_serve/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/app.py` & `taichu-serve-2.0.5/taichu_serve/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/command.py` & `taichu-serve-2.0.5/taichu_serve/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,18 @@
             continue
 
         with open(os.path.join(template_path, file), "r") as f:
             content = f.read()
         print("create file: ", os.path.join(name, file))
         with open(os.path.join(name, file), "w") as f:
             f.write(content)
+
+    with open(os.path.join(name, "dependencies.txt"), "w") as f:
+        f.write("curl")
+    print("create file: ", os.path.join(name, "dependencies.txt"))
     print("init project done!")
 
 
 def cli():
     args = parse_args()
     if args.action == "init":
         init_project()
```

### Comparing `taichu-serve-2.0.4/taichu_serve/common.py` & `taichu-serve-2.0.5/taichu_serve/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 logger = logging.getLogger(__name__)
 
 
 def grpc_interceptor(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         Local.request_id = str(uuid.uuid4())
-        context = kwargs.get('context')
+        context = args[2]
         start_time = time.time()
         try:
             ret = func(*args, **kwargs)
         except ModelPredictError as e:
             logger.error('[grpc_interceptor] error: %s', e.message)
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(e.message)
```

### Comparing `taichu-serve-2.0.4/taichu_serve/error_code.py` & `taichu-serve-2.0.5/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.5/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.5/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/grpc_server.py` & `taichu-serve-2.0.5/taichu_serve/grpc_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/log.py` & `taichu-serve-2.0.5/taichu_serve/log.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/model_server.py` & `taichu-serve-2.0.5/taichu_serve/model_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/settings.py` & `taichu-serve-2.0.5/taichu_serve/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Taichu Model Server')
     parser.add_argument('action', action="store", choices=['init', 'run'])
     # parser.add_argument('name', action="store", default='default', type=str)
 
-    parser.add_argument('--grpc_port', action="store", default=8889, type=int)
-    parser.add_argument('--http_port', action="store", default=8888, type=int)
+    parser.add_argument('--grpc_port', action="store", default=8080, type=int)
+    parser.add_argument('--http_port', action="store", default=8081, type=int)
     parser.add_argument('--grpc_only', action="store", default=False, type=bool)
     parser.add_argument('--model_path', action="store", default='./', type=str)
     parser.add_argument('--service_file', action="store", default='customize_service.py', type=str)
     parser.add_argument('--max_concurrent_requests', action="store", default=1, type=int)
     parser.add_argument('--instances_num', action="store", default=1, type=int)
 
     args = parser.parse_args()
```

### Comparing `taichu-serve-2.0.4/taichu_serve/template/customize_service.py` & `taichu-serve-2.0.5/taichu_serve/template/customize_service.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.4/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.5/taichu_serve/template/test/grpc_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
+model_name = "TestService"
+
 
 def run():
-    conn = grpc.insecure_channel('localhost:8889')
+    conn = grpc.insecure_channel('localhost:8080')
     client = grpc_predict_v2_pb2_grpc.GRPCInferenceServiceStub(channel=conn)
 
     req = grpc_predict_v2_pb2.ModelInferRequest()
-    req.model_name = 'testservice'
+    req.model_name = model_name
     req.model_version = '1'
     req.parameters['boo_var'].bool_param = True
     req.parameters['float_var'].float_param = 12.3432
     req.parameters['str_var'].string_param = 'str'
 
     respnse = client.ModelInfer(req)
     print("received:", respnse)
```

### Comparing `taichu-serve-2.0.4/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.5/taichu_serve/template/test/stream_grpc_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import logging
 
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
+model_name = "TestService"
+
 
 def guide_list_features(stub):
     num = 5
 
     while True:
 
         def generator():
             for i in range(num):
                 req = grpc_predict_v2_pb2.ModelInferRequest()
-                req.model_name = 'testservice'
+                req.model_name = model_name
                 req.model_version = '1'
 
                 req.parameters['input'].bool_param = True
                 yield req
 
                 # time.sleep(1)
 
         resp = stub.ModelStreamInfer(generator())
         for feature in resp:
             print(feature)
 
 
 def run():
-    with grpc.insecure_channel('localhost:8889') as channel:
+    with grpc.insecure_channel('localhost:8080') as channel:
         stub = grpc_predict_v2_pb2_grpc.GRPCInferenceServiceStub(channel)
         guide_list_features(stub)
 
 
 if __name__ == '__main__':
     logging.basicConfig()
     run()
```

### Comparing `taichu-serve-2.0.4/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.5/taichu_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

