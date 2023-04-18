# Comparing `tmp/zirconium-1.1.1.tar.gz` & `tmp/zirconium-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\erina\PycharmProjects\zirconium\dist\.tmp-vket62k6\zirconium-1.1.1.tar", last modified: Thu Apr  6 21:25:24 2023, max compression
+gzip compressed data, was "zirconium-1.1.2.tar", last modified: Tue Apr 18 11:57:41 2023, max compression
```

## Comparing `zirconium-1.1.1.tar` & `zirconium-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 21:25:24.000000 zirconium-1.1.1/
--rw-rw-rw-   0        0        0     1058 2022-05-07 10:41:49.000000 zirconium-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5115 2023-04-06 21:25:24.000000 zirconium-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4570 2023-04-06 21:22:07.000000 zirconium-1.1.1/README.md
--rw-rw-rw-   0        0        0       88 2022-05-07 10:39:24.000000 zirconium-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      684 2023-04-06 21:25:24.000000 zirconium-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium/
--rw-rw-rw-   0        0        0      240 2023-04-06 21:24:54.000000 zirconium-1.1.1/src/zirconium/__init__.py
--rw-rw-rw-   0        0        0    15986 2023-04-06 21:17:59.000000 zirconium-1.1.1/src/zirconium/config.py
--rw-rw-rw-   0        0        0     5155 2023-04-06 21:19:22.000000 zirconium-1.1.1/src/zirconium/parsers.py
--rw-rw-rw-   0        0        0     1148 2023-03-23 03:43:23.000000 zirconium-1.1.1/src/zirconium/sproviders.py
--rw-rw-rw-   0        0        0     5350 2023-03-23 03:07:39.000000 zirconium-1.1.1/src/zirconium/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium.egg-info/
--rw-rw-rw-   0        0        0     5115 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 21:25:24.000000 zirconium-1.1.1/src/zirconium.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 21:25:24.000000 zirconium-1.1.1/tests/
--rw-rw-rw-   0        0        0    14440 2022-06-14 20:53:44.000000 zirconium-1.1.1/tests/test_config.py
--rw-rw-rw-   0        0        0    12057 2023-04-06 21:19:51.000000 zirconium-1.1.1/tests/test_handlers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/
+-rw-rw-rw-   0        0        0     1058 2023-04-18 11:50:52.000000 zirconium-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5115 2023-04-18 11:57:41.146935 zirconium-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4570 2023-04-18 11:50:54.000000 zirconium-1.1.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-23 19:45:58.000000 zirconium-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      684 2023-04-18 11:57:41.146935 zirconium-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.115708 zirconium-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.131286 zirconium-1.1.2/src/zirconium/
+-rw-rw-rw-   0        0        0      240 2023-04-18 11:57:30.000000 zirconium-1.1.2/src/zirconium/__init__.py
+-rw-rw-rw-   0        0        0    16476 2023-04-18 11:55:45.000000 zirconium-1.1.2/src/zirconium/config.py
+-rw-rw-rw-   0        0        0     5155 2023-04-18 11:50:54.000000 zirconium-1.1.2/src/zirconium/parsers.py
+-rw-rw-rw-   0        0        0     1148 2023-04-18 11:50:54.000000 zirconium-1.1.2/src/zirconium/sproviders.py
+-rw-rw-rw-   0        0        0     5447 2023-01-30 20:11:22.000000 zirconium-1.1.2/src/zirconium/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/src/zirconium.egg-info/
+-rw-rw-rw-   0        0        0     5115 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 11:57:41.000000 zirconium-1.1.2/src/zirconium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 11:57:41.146935 zirconium-1.1.2/tests/
+-rw-rw-rw-   0        0        0    15708 2023-04-18 11:54:13.000000 zirconium-1.1.2/tests/test_config.py
+-rw-rw-rw-   0        0        0    12057 2023-04-18 11:50:54.000000 zirconium-1.1.2/tests/test_handlers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zirconium-1.1.1/LICENSE` & `zirconium-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.1/PKG-INFO` & `zirconium-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.1.1
+Version: 1.1.2
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zirconium-1.1.1/README.md` & `zirconium-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.1/setup.cfg` & `zirconium-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 207a 6972 636f 6e69 756d 0d0a 7665   = zirconium..ve
-00000020: 7273 696f 6e20 3d20 312e 312e 310d 0a61  rsion = 1.1.1..a
+00000020: 7273 696f 6e20 3d20 312e 312e 320d 0a61  rsion = 1.1.2..a
 00000030: 7574 686f 7220 3d20 4572 696e 2054 7572  uthor = Erin Tur
 00000040: 6e62 756c 6c0d 0a61 7574 686f 725f 656d  nbull..author_em
 00000050: 6169 6c20 3d20 6572 696e 2e61 2e74 7572  ail = erin.a.tur
 00000060: 6e62 756c 6c40 676d 6169 6c2e 636f 6d0d  nbull@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
 00000080: 7863 656c 6c65 6e74 2063 6f6e 6669 6775  xcellent configu
 00000090: 7261 7469 6f6e 206d 616e 6167 656d 656e  ration managemen
```

### Comparing `zirconium-1.1.1/src/zirconium/config.py` & `zirconium-1.1.2/src/zirconium/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 registrar_func = ep.load()
                 registrar_func(self)
             self.ach.execute_hooks(self)
             self.init()
 
     def get(self, *key, default=None, coerce=None, blank_to_none=False, raw=False, raise_error=False):
         key = self._expand_key(key)
-        full_key = ".".join([str(x) for x in key])
+        full_key = ".".join([str(x) for x in key]) + (str(coerce) if coerce else "")
         if full_key in self._cached_gets:
             return self._cached_gets[full_key]
         with self.cache_lock:
             if full_key not in self._cached_gets:
                 value = super().get(*key, default=default, raise_error=raise_error)
                 if blank_to_none and value == "":
                     value = None
@@ -298,14 +298,24 @@
         if self.file_registry[key]:
             return max(x[1] for x in self.file_registry[key]) + 1
         return 0
 
     def register_environ_var(self, env_var_name, *target_config):
         self.environment_map[env_var_name] = target_config
 
+    def reload_config(self):
+        # We take all three locks to prevent any weird multi-threaded behaviour from happening. All writes are blocked until we are done the re-load except our own.
+        with self.lock:
+            with self.registry_lock:
+                with self.cache_lock:
+                    self._cached_gets = {}
+                    self._init_flag = False
+                    self.clear()
+                    self.init()
+
     def register_secret_as_environ_var(self, secret_path, secret_provider, env_var_name):
         self.secrets_env_map[env_var_name] = (secret_path, secret_provider)
 
     def register_secret_config(self, secret_path, secret_provider, *target_config):
         secret_provider = secret_provider.lower()
         self.secrets_map[f"{secret_path}{secret_provider}"] = (secret_path, secret_provider, target_config)
```

### Comparing `zirconium-1.1.1/src/zirconium/parsers.py` & `zirconium-1.1.2/src/zirconium/parsers.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.1/src/zirconium/sproviders.py` & `zirconium-1.1.2/src/zirconium/sproviders.py`

 * *Files identical despite different names*

### Comparing `zirconium-1.1.1/src/zirconium/utils.py` & `zirconium-1.1.2/src/zirconium/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
         """ __len__ implementation """
         return len(self.d)
 
     def __iter__(self):
         """ __iter__ implementation """
         return iter(self.d)
 
+    def clear(self):
+        """Clear the dictionary of all entries."""
+        self.d = {}
+
     def deep_update(self, d):
         """ Similar to update(), but will merge dictionaries at depth. Thread-safe. """
         with self.lock:
             for key in d.keys():
                 if key in self.d and MutableDeepDict.is_dict_like(d[key]) and MutableDeepDict.is_dict_like(self.d[key]):
                     mut = MutableDeepDict(self.d[key])
                     mut.deep_update(d[key])
```

### Comparing `zirconium-1.1.1/src/zirconium.egg-info/PKG-INFO` & `zirconium-1.1.2/src/zirconium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zirconium
-Version: 1.1.1
+Version: 1.1.2
 Summary: Excellent configuration management for Python
 Home-page: https://github.com/turnbullerin/zirconium
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/zirconium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zirconium-1.1.1/tests/test_handlers.py` & `zirconium-1.1.2/tests/test_handlers.py`

 * *Files identical despite different names*

