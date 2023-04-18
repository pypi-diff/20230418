# Comparing `tmp/hagis-0.2.5.tar.gz` & `tmp/hagis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.5.tar", last modified: Mon Apr 17 13:26:53 2023, max compression
+gzip compressed data, was "hagis-0.2.6.tar", last modified: Mon Apr 17 15:03:55 2023, max compression
```

## Comparing `hagis-0.2.5.tar` & `hagis-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.284656 hagis-0.2.5/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:26:53.283656 hagis-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.271105 hagis-0.2.5/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.5/hagis/__init__.py
--rw-rw-rw-   0        0        0     9657 2023-04-17 13:24:45.000000 hagis-0.2.5/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.281645 hagis-0.2.5/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-17 13:24:55.000000 hagis-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 13:26:53.284656 hagis-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:55.060666 hagis-0.2.6/
+-rw-rw-rw-   0        0        0      941 2023-04-17 15:03:55.059665 hagis-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:55.049665 hagis-0.2.6/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.6/hagis/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-17 15:03:11.000000 hagis-0.2.6/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:03:55.057664 hagis-0.2.6/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-17 15:03:55.000000 hagis-0.2.6/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-17 15:03:55.000000 hagis-0.2.6/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:03:55.000000 hagis-0.2.6/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 15:03:55.000000 hagis-0.2.6/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-17 15:03:27.000000 hagis-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:03:55.060666 hagis-0.2.6/setup.cfg
```

### Comparing `hagis-0.2.5/PKG-INFO` & `hagis-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.5/hagis/hagis.py` & `hagis-0.2.6/hagis/hagis.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._layer_url = layer_url
         self._model = model
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
         self._fields: Dict[str, str] = {}
-        self.generate_token: Callable[[], str] = lambda: ""
+        self._generate_token: Callable[[], str] = lambda: ""
         self._is_dynamic = model == SimpleNamespace
 
         if self._is_dynamic:
             return
         
         # List of custom mapping properties that have been handled.
         mapped: List[str] = []
@@ -73,15 +73,15 @@
                 response = post(generate_token_url, data = parameters)
                 dictionary = loads(response.content)
                 token, expiration_seconds = dictionary["token"], dictionary["expires"] / 1000
                 Layer._token_cache[key] = token, expiration_seconds
 
             return token
         
-        self.generate_token = generate_token;
+        self._generate_token = generate_token;
 
     def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterable[T]:
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
@@ -147,15 +147,15 @@
             else:
                 attributes[field] = value
 
         return dictionary
 
     def _post(self, method: str, **kwargs: Any) -> SimpleNamespace:
         # Update the token.
-        kwargs["token"] = self.generate_token()
+        kwargs["token"] = self._generate_token()
         response = post(f"{self._layer_url}/{method}", kwargs)
 
         # Map it to a dynamic object.
         obj = loads(response.text, object_hook=lambda x: SimpleNamespace(**x))
 
         # If this is an error response, throw an exception.
         if hasattr(obj, "error"):
```

### Comparing `hagis-0.2.5/hagis.egg-info/PKG-INFO` & `hagis-0.2.6/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.5/pyproject.toml` & `hagis-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

