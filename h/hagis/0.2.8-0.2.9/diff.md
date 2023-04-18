# Comparing `tmp/hagis-0.2.8.tar.gz` & `tmp/hagis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.8.tar", last modified: Tue Apr 18 09:29:46 2023, max compression
+gzip compressed data, was "hagis-0.2.9.tar", last modified: Tue Apr 18 09:40:37 2023, max compression
```

## Comparing `hagis-0.2.8.tar` & `hagis-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.291689 hagis-0.2.8/
--rw-rw-rw-   0        0        0      941 2023-04-18 09:29:46.283691 hagis-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.243684 hagis-0.2.8/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.8/hagis/__init__.py
--rw-rw-rw-   0        0        0     9887 2023-04-18 09:25:23.000000 hagis-0.2.8/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:29:46.275695 hagis-0.2.8/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 09:29:46.000000 hagis-0.2.8/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-18 09:29:20.000000 hagis-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 09:29:46.291689 hagis-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.196305 hagis-0.2.9/
+-rw-rw-rw-   0        0        0      941 2023-04-18 09:40:37.196305 hagis-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.156885 hagis-0.2.9/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.9/hagis/__init__.py
+-rw-rw-rw-   0        0        0     9790 2023-04-18 09:37:19.000000 hagis-0.2.9/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:40:37.187409 hagis-0.2.9/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 09:40:37.000000 hagis-0.2.9/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-18 09:40:11.000000 hagis-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:40:37.196305 hagis-0.2.9/setup.cfg
```

### Comparing `hagis-0.2.8/PKG-INFO` & `hagis-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.8
+Version: 0.2.9
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.8/hagis/hagis.py` & `hagis-0.2.9/hagis/hagis.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,21 +56,15 @@
 
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
     def set_token_generator(self, username: str, password: str, referer: str = "", generate_token_url: str = "https://www.arcgis.com/sharing/generateToken", **kwargs: Any) -> None:
         kwargs["username"] = username
         kwargs["password"] = password
         kwargs["referer"] = referer
-
-        if referer:
-            kwargs["client"] = "referer"
-        elif "ip" in kwargs:
-            kwargs["client"] = "ip"
-        else:
-            kwargs["client"] = "requestip"
+        kwargs["client"] = "referer" if referer else "ip" if "ip" in kwargs else "requestip"
 
         key = generate_token_url, md5(dumps(kwargs).encode("utf-8")).hexdigest()
 
         def generate_token() -> str:
             if key not in Layer._token_cache:
                 Layer._token_cache[key] = "", 0
```

### Comparing `hagis-0.2.8/hagis.egg-info/PKG-INFO` & `hagis-0.2.9/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.8
+Version: 0.2.9
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.8/pyproject.toml` & `hagis-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

