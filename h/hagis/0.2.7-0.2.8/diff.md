# Comparing `tmp/hagis-0.2.7.tar.gz` & `tmp/hagis-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.7.tar", last modified: Tue Apr 18 01:41:59 2023, max compression
+gzip compressed data, was "hagis-0.2.8.tar", last modified: Tue Apr 18 09:29:46 2023, max compression
```

## Comparing `hagis-0.2.7.tar` & `hagis-0.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:41:59.558708 hagis-0.2.7/
--rw-rw-rw-   0        0        0      941 2023-04-18 01:41:59.550805 hagis-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 01:41:59.514313 hagis-0.2.7/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.7/hagis/__init__.py
--rw-rw-rw-   0        0        0     9574 2023-04-18 01:38:28.000000 hagis-0.2.7/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:41:59.550805 hagis-0.2.7/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-18 01:41:59.000000 hagis-0.2.7/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-18 01:41:59.000000 hagis-0.2.7/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:41:59.000000 hagis-0.2.7/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 01:41:59.000000 hagis-0.2.7/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-18 01:39:36.000000 hagis-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 01:41:59.558708 hagis-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.291689 hagis-0.2.8/
+-rw-rw-rw-   0        0        0      941 2023-04-18 09:29:46.283691 hagis-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.243684 hagis-0.2.8/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.8/hagis/__init__.py
+-rw-rw-rw-   0        0        0     9887 2023-04-18 09:25:23.000000 hagis-0.2.8/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.275695 hagis-0.2.8/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-18 09:29:20.000000 hagis-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:29:46.291689 hagis-0.2.8/setup.cfg
```

### Comparing `hagis-0.2.7/PKG-INFO` & `hagis-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.7
+Version: 0.2.8
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.7/hagis/hagis.py` & `hagis-0.2.8/hagis/hagis.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,44 +52,55 @@
         # Add custom properties that have not been handled as dynamically handled propeties.
         for property, field in mapping.items():
             if property not in mapped:
                 self._fields[property.lower()] = field
 
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
-    def set_token_generator(self, generate_token_url: str = "https://www.arcgis.com/sharing/generateToken", **parameters: Any) -> None:
-        parameters["f"] = "json"
+    def set_token_generator(self, username: str, password: str, referer: str = "", generate_token_url: str = "https://www.arcgis.com/sharing/generateToken", **kwargs: Any) -> None:
+        kwargs["username"] = username
+        kwargs["password"] = password
+        kwargs["referer"] = referer
+
+        if referer:
+            kwargs["client"] = "referer"
+        elif "ip" in kwargs:
+            kwargs["client"] = "ip"
+        else:
+            kwargs["client"] = "requestip"
 
-        key = generate_token_url, md5(dumps(parameters).encode("utf-8")).hexdigest()
+        key = generate_token_url, md5(dumps(kwargs).encode("utf-8")).hexdigest()
 
         def generate_token() -> str:
             if key not in Layer._token_cache:
                 Layer._token_cache[key] = "", 0
 
             # Get the cached token and its expiry.
-            token, expiration_seconds = Layer._token_cache[key];
+            token, expiration_seconds = Layer._token_cache[key]
 
             # Renew if less than a minute left.
             if expiration_seconds - time() < 60:
-                obj = self._post(generate_token_url, **parameters)
+                obj = self._post(generate_token_url, **kwargs)
                 token, expiration_seconds = obj.token, obj.expires / 1000
                 Layer._token_cache[key] = token, expiration_seconds
 
             return token
 
-        self._generate_token = generate_token;
+        self._generate_token = generate_token
+
+    def set_token(self, token: str) -> None:
+        self._generate_token = lambda: token
 
     def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterable[T]:
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
             fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
-
             if not self._shape_property_name:
                 kwargs["returnGeometry"] = False
 
         for row in self._query(where_clause, fields, **kwargs):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
@@ -101,37 +112,37 @@
                     # Normal classes require the parameterless constructor.
                     item = self._model()
                     for property_name, property_value in dictionary.items():
                         setattr(item, property_name, property_value)
                 yield item
 
     def count(self, where_clause: str = "1=1") -> int:
-        obj = self._post_with_token("query", where=where_clause, returnCountOnly=True, f="json")
+        obj = self._call("query", where=where_clause, returnCountOnly=True)
         return obj.count
 
     def find(self, oid: int, **kwargs: Any) -> Optional[T]:
         items = [item for item in self.query(f"{self._oid_field}={oid}", **kwargs)]
         if items:
             return items[0]
 
     def apply_edits(self, adds: Optional[List[T]] = None, updates: Optional[List[T]] = None, deletes: Union[List[int], List[str], None] = None, **kwargs: Any) -> SimpleNamespace:
         adds_json = "" if adds is None else dumps([self._to_dict(x) for x in adds])
         updates_json = "" if updates is None else dumps([self._to_dict(x) for x in updates])
         deletes_json = "" if deletes is None else dumps([x for x in deletes])
-        return self._post_with_token("applyEdits", adds=adds_json, updates=updates_json, deletes=deletes_json, f="json", **kwargs)
+        return self._call("applyEdits", adds=adds_json, updates=updates_json, deletes=deletes_json, **kwargs)
 
     def insert(self, items: List[T], **kwargs: Any) -> List[int]:
         result = self.apply_edits(adds=items, **kwargs)
         return [x.objectId for x in result.addResults]
 
     def update(self, items: List[T], **kwargs: Any) -> None:
         self.apply_edits(updates=items, **kwargs)
 
     def delete(self, where_clause: str, **kwargs: Any) -> None:
-        self._post_with_token("deleteFeatures", where=where_clause, f="json", **kwargs)
+        self._call("deleteFeatures", where=where_clause, **kwargs)
 
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
@@ -144,40 +155,41 @@
                 attributes[field] = int((value - datetime.utcfromtimestamp(0)).total_seconds() * 1000)
             else:
                 attributes[field] = value
 
         return dictionary
 
     def _post(self, url: str, **kwargs: Any) -> SimpleNamespace:
+        kwargs["f"] = "json"
         response = post(url, kwargs)
         obj = loads(response.text, object_hook=lambda x: SimpleNamespace(**x))
 
         if hasattr(obj, "error"):
             raise Exception(obj.error.message)
 
         return obj
 
-    def _post_with_token(self, method: str, **kwargs: Any) -> SimpleNamespace:
+    def _call(self, method: str, **kwargs: Any) -> SimpleNamespace:
         kwargs["token"] = self._generate_token()
         return self._post(f"{self._layer_url}/{method}", **kwargs)
 
     def _get_rows(self, where_clause: str, fields: str, **kwargs: Any) -> Tuple[List[SimpleNamespace], bool]:
-        obj = self._post_with_token("query", where=where_clause, outFields=fields, f="json", **kwargs)
+        obj = self._call("query", where=where_clause, outFields=fields, **kwargs)
         date_fields = [f.name for f in obj.fields if f.type == "esriFieldTypeDate"] if hasattr(obj, "fields") else []
 
         if date_fields:
             for f in obj.features:
                 for key, value in f.attributes.__dict__.items():
                     if key in date_fields and value:
                         f.attributes.__dict__[key] = datetime.fromtimestamp(value / 1000)
 
         return (obj.features, obj.exceededTransferLimit if hasattr(obj, "exceededTransferLimit") else False)
 
     def _get_oids(self, where_clause: str) -> List[int]:
-        obj = self._post_with_token("query", where=where_clause, returnIdsOnly="true", f="json")
+        obj = self._call("query", where=where_clause, returnIdsOnly="true")
         return obj.objectIds
 
     def _map(self, row: SimpleNamespace) -> SimpleNamespace:
         if not hasattr(row, "geometry"):
             return row.attributes
 
         if self._shape_property_type is None or self._shape_property_type in self._unknown_shape_types:
```

### Comparing `hagis-0.2.7/hagis.egg-info/PKG-INFO` & `hagis-0.2.8/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.7
+Version: 0.2.8
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.7/pyproject.toml` & `hagis-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

