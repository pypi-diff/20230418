# Comparing `tmp/iris_pex_embedded_python-2.0.2.tar.gz` & `tmp/iris_pex_embedded_python-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.0.2.tar", last modified: Mon Apr 17 12:59:31 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.0.3.tar", last modified: Tue Apr 18 12:22:09 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.0.2.tar` & `iris_pex_embedded_python-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.821010 iris_pex_embedded_python-2.0.2/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.0.2/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-17 12:59:31.820076 iris_pex_embedded_python-2.0.2/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.2/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.2/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-17 12:59:31.821247 iris_pex_embedded_python-2.0.2/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-17 12:54:41.000000 iris_pex_embedded_python-2.0.2/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.777791 iris_pex_embedded_python-2.0.2/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.777261 iris_pex_embedded_python-2.0.2/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.784283 iris_pex_embedded_python-2.0.2/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.806054 iris_pex_embedded_python-2.0.2/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1138 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112    19811 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112    14889 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     6228 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.814906 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112      845 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/top_level.txt
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.817317 iris_pex_embedded_python-2.0.2/test/
--rw-r--r--   0 grongier (902446405) 1252422112      273 2023-01-06 14:56:27.000000 iris_pex_embedded_python-2.0.2/test/test_selectt.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.649999 iris_pex_embedded_python-2.0.3/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.0.3/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-18 12:22:09.649116 iris_pex_embedded_python-2.0.3/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.3/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.3/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-18 12:22:09.650279 iris_pex_embedded_python-2.0.3/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-18 12:20:55.000000 iris_pex_embedded_python-2.0.3/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.596010 iris_pex_embedded_python-2.0.3/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.595276 iris_pex_embedded_python-2.0.3/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.604141 iris_pex_embedded_python-2.0.3/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.633472 iris_pex_embedded_python-2.0.3/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    19811 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112    14889 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     6966 2023-04-18 10:16:42.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.644975 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112      845 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.646683 iris_pex_embedded_python-2.0.3/test/
+-rw-r--r--   0 grongier (902446405) 1252422112      273 2023-01-06 14:56:27.000000 iris_pex_embedded_python-2.0.3/test/test_selectt.py
```

### Comparing `iris_pex_embedded_python-2.0.2/LICENSE` & `iris_pex_embedded_python-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/PKG-INFO` & `iris_pex_embedded_python-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.0.2
+Version: 2.0.3
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.0.2/README.md` & `iris_pex_embedded_python-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/setup.py` & `iris_pex_embedded_python-2.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.0.2',
+        version='2.0.3',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from grongier.pex._private_session_process import _PrivateSessionProcess
 from grongier.pex._business_operation import _BusinessOperation
 from grongier.pex._inbound_adapter import _InboundAdapter
 from grongier.pex._outbound_adapter import _OutboundAdapter
 from grongier.pex._message import _Message
 from grongier.pex._pickle_message import _PickleMessage
 from grongier.pex._director import _Director
+from grongier.pex._utils import _Utils
 
-import grongier.pex._utils as Utils
-
+class Utils(_Utils): pass
 class InboundAdapter(_InboundAdapter): pass
 class OutboundAdapter(_OutboundAdapter): pass
 class BusinessService(_BusinessService): pass
 class BusinessOperation(_BusinessOperation): pass
 class BusinessProcess(_BusinessProcess): pass
 class DuplexService(_PrivateSessionDuplex): pass
 class DuplexOperation(_PrivateSessionDuplex): pass
```

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.2/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.0.3/src/grongier/pex/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,150 +1,159 @@
-import iris
 import os
 import ast
+import iris
 
-def raise_on_error(sc):
-    """
-    If the status code is an error, raise an exception
-    
-    :param sc: The status code returned by the Iris API
-    """
-    if iris.system.Status.IsError(sc):
-        raise RuntimeError(iris.system.Status.GetOneStatusText(sc))
-
-def setup(path:str = None):
-
-    if path is None:
-        # get the parent directory of the current module
-        # and append 'iris/Grongier/PEX' to it
-        path = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'iris/Grongier/PEX')
-
-    raise_on_error(iris.cls('%SYSTEM.OBJ').LoadDir(path,'cubk',"*.cls",1))
-
-def register_component(module:str,classname:str,path:str,overwrite:int,iris_classname:str):
-    """
-    It registers a component in the Iris database.
-    
-    :param module: The name of the module that contains the class
-    :type module: str
-    :param classname: The name of the class you want to register
-    :type classname: str
-    :param path: The path to the component
-    :type path: str
-    :param overwrite: 0 = no, 1 = yes
-    :type overwrite: int
-    :param iris_classname: The name of the class in the Iris class hierarchy
-    :type iris_classname: str
-    :return: The return value is a string.
-    """
-
-    return iris.cls('Grongier.PEX.Utils').dispatchRegisterComponent(module,classname,path,overwrite,iris_classname)
-
-def register_folder(path:str,overwrite:int,iris_package_name:str):
-    """
-    > This function takes a path to a folder, and registers all the Python files in that folder as IRIS
-    classes
-    
-    :param path: the path to the folder containing the files you want to register
-    :type path: str
-    :param overwrite: 
-    :type overwrite: int
-    :param iris_package_name: The name of the iris package you want to register the file to
-    :type iris_package_name: str
-    """
-    path = os.path.normpath(path)
-    for filename in os.listdir(path):
-        if filename.endswith(".py"): 
-            _register_file(filename, path, overwrite, iris_package_name)
-        else:
-            continue
-
-def register_file(file:str,overwrite:int,iris_package_name:str):
-    """
-    It takes a file name, a boolean to overwrite existing components, and the name of the Iris
-    package that the file is in. It then opens the file, parses it, and looks for classes that extend
-    BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
-    with the module name, class name, path, overwrite boolean, and the full Iris package name
-    
-    :param file: the name of the file containing the component
-    :type file: str
-    :param overwrite: if the component already exists, overwrite it
-    :type overwrite: int
-    :param iris_package_name: the name of the iris package that you want to register the components to
-    :type iris_package_name: str
-    """
-    head_tail = os.path.split(file)
-    return _register_file(head_tail[1],head_tail[0],overwrite,iris_package_name)
-
-def _register_file(filename:str,path:str,overwrite:int,iris_package_name:str):
-    """
-    It takes a file name, a path, a boolean to overwrite existing components, and the name of the Iris
-    package that the file is in. It then opens the file, parses it, and looks for classes that extend
-    BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
-    with the module name, class name, path, overwrite boolean, and the full Iris package name
-    
-    :param filename: the name of the file containing the component
-    :type filename: str
-    :param path: the path to the directory containing the files to be registered
-    :type path: str
-    :param overwrite: if the component already exists, overwrite it
-    :type overwrite: int
-    :param iris_package_name: the name of the iris package that you want to register the components to
-    :type iris_package_name: str
-    """
-    #pour chaque classe dans le module, appeler register_component
-    f =  os.path.join(path,filename)
-    with open(f) as file:
-        node = ast.parse(file.read())
-        #list of class in the file
-        classes = [n for n in node.body if isinstance(n, ast.ClassDef)]
-        for klass in classes:
-            extend = ''
-            if len(klass.bases) == 1:
-                if hasattr(klass.bases[0],'id'):
-                    extend = klass.bases[0].id
-                else:
-                    extend = klass.bases[0].attr
-            #if extends BusinessOperation,BusinessProcess,BusinessService
-            if  extend in ('BusinessOperation','BusinessProcess','BusinessService','DuplexService','DuplexProcess','DuplexOperation','InboundAdapter','OutboundAdapter'):
-                module = filename_to_module(filename)
-                register_component(module, klass.name, path, overwrite, f"{iris_package_name}.{module}.{klass.name}")
-
-def register_package(package:str,path:str,overwrite:int,iris_package_name:str):
-    """
-    It takes a package name, a path to the package, a flag to overwrite existing files, and the name of
-    the iris package to register the files to. It then loops through all the files in the package and
-    registers them to the iris package
-    
-    :param package: the name of the package you want to register
-    :type package: str
-    :param path: the path to the directory containing the package
-    :type path: str
-    :param overwrite: 0 = don't overwrite, 1 = overwrite
-    :type overwrite: int
-    :param iris_package_name: The name of the package in the Iris package manager
-    :type iris_package_name: str
-    """
-    for filename in os.listdir(os.path.join(path,package)):
-        if filename.endswith(".py"): 
-            _register_file(os.path.join(package,filename), path, overwrite, iris_package_name)
+class _Utils():
+    @staticmethod
+    def raise_on_error(sc):
+        """
+        If the status code is an error, raise an exception
+        
+        :param sc: The status code returned by the Iris API
+        """
+        if iris.system.Status.IsError(sc):
+            raise RuntimeError(iris.system.Status.GetOneStatusText(sc))
+
+    @staticmethod
+    def setup(path:str = None):
+
+        if path is None:
+            # get the parent directory of the current module
+            # and append 'iris/Grongier/PEX' to it
+            path = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'iris/Grongier/PEX')
+
+        _Utils.raise_on_error(iris.cls('%SYSTEM.OBJ').LoadDir(path,'cubk',"*.cls",1))
+
+    @staticmethod
+    def register_component(module:str,classname:str,path:str,overwrite:int,iris_classname:str):
+        """
+        It registers a component in the Iris database.
+        
+        :param module: The name of the module that contains the class
+        :type module: str
+        :param classname: The name of the class you want to register
+        :type classname: str
+        :param path: The path to the component
+        :type path: str
+        :param overwrite: 0 = no, 1 = yes
+        :type overwrite: int
+        :param iris_classname: The name of the class in the Iris class hierarchy
+        :type iris_classname: str
+        :return: The return value is a string.
+        """
+
+        return iris.cls('Grongier.PEX.Utils').dispatchRegisterComponent(module,classname,path,overwrite,iris_classname)
+
+    @staticmethod
+    def register_folder(path:str,overwrite:int,iris_package_name:str):
+        """
+        > This function takes a path to a folder, and registers all the Python files in that folder as IRIS
+        classes
+        
+        :param path: the path to the folder containing the files you want to register
+        :type path: str
+        :param overwrite: 
+        :type overwrite: int
+        :param iris_package_name: The name of the iris package you want to register the file to
+        :type iris_package_name: str
+        """
+        path = os.path.normpath(path)
+        for filename in os.listdir(path):
+            if filename.endswith(".py"): 
+                _Utils._register_file(filename, path, overwrite, iris_package_name)
+            else:
+                continue
+
+    @staticmethod
+    def register_file(file:str,overwrite:int,iris_package_name:str):
+        """
+        It takes a file name, a boolean to overwrite existing components, and the name of the Iris
+        package that the file is in. It then opens the file, parses it, and looks for classes that extend
+        BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
+        with the module name, class name, path, overwrite boolean, and the full Iris package name
+        
+        :param file: the name of the file containing the component
+        :type file: str
+        :param overwrite: if the component already exists, overwrite it
+        :type overwrite: int
+        :param iris_package_name: the name of the iris package that you want to register the components to
+        :type iris_package_name: str
+        """
+        head_tail = os.path.split(file)
+        return _Utils._register_file(head_tail[1],head_tail[0],overwrite,iris_package_name)
+
+    @staticmethod
+    def _register_file(filename:str,path:str,overwrite:int,iris_package_name:str):
+        """
+        It takes a file name, a path, a boolean to overwrite existing components, and the name of the Iris
+        package that the file is in. It then opens the file, parses it, and looks for classes that extend
+        BusinessOperation, BusinessProcess, or BusinessService. If it finds one, it calls register_component
+        with the module name, class name, path, overwrite boolean, and the full Iris package name
+        
+        :param filename: the name of the file containing the component
+        :type filename: str
+        :param path: the path to the directory containing the files to be registered
+        :type path: str
+        :param overwrite: if the component already exists, overwrite it
+        :type overwrite: int
+        :param iris_package_name: the name of the iris package that you want to register the components to
+        :type iris_package_name: str
+        """
+        #pour chaque classe dans le module, appeler register_component
+        f =  os.path.join(path,filename)
+        with open(f) as file:
+            node = ast.parse(file.read())
+            #list of class in the file
+            classes = [n for n in node.body if isinstance(n, ast.ClassDef)]
+            for klass in classes:
+                extend = ''
+                if len(klass.bases) == 1:
+                    if hasattr(klass.bases[0],'id'):
+                        extend = klass.bases[0].id
+                    else:
+                        extend = klass.bases[0].attr
+                #if extends BusinessOperation,BusinessProcess,BusinessService
+                if  extend in ('BusinessOperation','BusinessProcess','BusinessService','DuplexService','DuplexProcess','DuplexOperation','InboundAdapter','OutboundAdapter'):
+                    module = _Utils.filename_to_module(filename)
+                    _Utils.register_component(module, klass.name, path, overwrite, f"{iris_package_name}.{module}.{klass.name}")
+
+    @staticmethod
+    def register_package(package:str,path:str,overwrite:int,iris_package_name:str):
+        """
+        It takes a package name, a path to the package, a flag to overwrite existing files, and the name of
+        the iris package to register the files to. It then loops through all the files in the package and
+        registers them to the iris package
+        
+        :param package: the name of the package you want to register
+        :type package: str
+        :param path: the path to the directory containing the package
+        :type path: str
+        :param overwrite: 0 = don't overwrite, 1 = overwrite
+        :type overwrite: int
+        :param iris_package_name: The name of the package in the Iris package manager
+        :type iris_package_name: str
+        """
+        for filename in os.listdir(os.path.join(path,package)):
+            if filename.endswith(".py"): 
+                _Utils._register_file(os.path.join(package,filename), path, overwrite, iris_package_name)
+            else:
+                continue
+
+    @staticmethod
+    def filename_to_module(filename) -> str:
+        """
+        It takes a filename and returns the module name
+        
+        :param filename: The name of the file to be imported
+        :return: The module name
+        """
+        module = ''
+
+        path,file = os.path.split(filename)
+        mod = file.split('.')[0]
+        packages = path.replace(os.sep, ('.'))
+        if len(packages) >1:
+            module = packages+'.'+mod
         else:
-            continue
-
-def filename_to_module(filename) -> str:
-    """
-    It takes a filename and returns the module name
-    
-    :param filename: The name of the file to be imported
-    :return: The module name
-    """
-    module = ''
-
-    path,file = os.path.split(filename)
-    mod = file.split('.')[0]
-    packages = path.replace(os.sep, ('.'))
-    if len(packages) >1:
-        module = packages+'.'+mod
-    else:
-        module = mod
+            module = mod
 
-    return module
+        return module
```

### Comparing `iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.0.2
+Version: 2.0.3
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

