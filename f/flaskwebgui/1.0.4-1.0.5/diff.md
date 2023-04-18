# Comparing `tmp/flaskwebgui-1.0.4.tar.gz` & `tmp/flaskwebgui-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskwebgui-1.0.4.tar", last modified: Sat Mar 11 09:29:45 2023, max compression
+gzip compressed data, was "flaskwebgui-1.0.5.tar", last modified: Tue Apr 18 13:24:56 2023, max compression
```

## Comparing `flaskwebgui-1.0.4.tar` & `flaskwebgui-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-03-11 09:29:45.262694 flaskwebgui-1.0.4/
--rw-rw-r--   0 alin      (1000) alin      (1000)     1064 2023-03-11 07:58:47.000000 flaskwebgui-1.0.4/LICENSE
--rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-03-11 09:29:45.262694 flaskwebgui-1.0.4/PKG-INFO
--rw-rw-r--   0 alin      (1000) alin      (1000)     7616 2023-03-11 09:28:14.000000 flaskwebgui-1.0.4/README.md
--rw-rw-r--   0 alin      (1000) alin      (1000)       38 2023-03-11 09:29:45.262694 flaskwebgui-1.0.4/setup.cfg
--rw-rw-r--   0 alin      (1000) alin      (1000)      824 2023-03-11 09:29:20.000000 flaskwebgui-1.0.4/setup.py
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-03-11 09:29:45.258694 flaskwebgui-1.0.4/src/
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-03-11 09:29:45.262694 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/
--rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-03-11 09:29:45.000000 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/PKG-INFO
--rw-rw-r--   0 alin      (1000) alin      (1000)      239 2023-03-11 09:29:45.000000 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/SOURCES.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)        1 2023-03-11 09:29:45.000000 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/dependency_links.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-03-11 09:29:45.000000 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/requires.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-03-11 09:29:45.000000 flaskwebgui-1.0.4/src/flaskwebgui.egg-info/top_level.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)     7375 2023-03-11 09:15:31.000000 flaskwebgui-1.0.4/src/flaskwebgui.py
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/
+-rw-rw-r--   0 alin      (1000) alin      (1000)     1064 2023-03-11 07:58:47.000000 flaskwebgui-1.0.5/LICENSE
+-rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/PKG-INFO
+-rw-rw-r--   0 alin      (1000) alin      (1000)     7616 2023-03-11 09:28:14.000000 flaskwebgui-1.0.5/README.md
+-rw-rw-r--   0 alin      (1000) alin      (1000)       38 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/setup.cfg
+-rw-rw-r--   0 alin      (1000) alin      (1000)      824 2023-04-18 13:24:41.000000 flaskwebgui-1.0.5/setup.py
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.305650 flaskwebgui-1.0.5/src/
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.305650 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/
+-rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/PKG-INFO
+-rw-rw-r--   0 alin      (1000) alin      (1000)      239 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)        1 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/requires.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/top_level.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)     7509 2023-04-18 13:24:11.000000 flaskwebgui-1.0.5/src/flaskwebgui.py
```

### Comparing `flaskwebgui-1.0.4/LICENSE` & `flaskwebgui-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskwebgui-1.0.4/PKG-INFO` & `flaskwebgui-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.0.4
+Version: 1.0.5
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flaskwebgui-1.0.4/README.md` & `flaskwebgui-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flaskwebgui-1.0.4/setup.py` & `flaskwebgui-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt", "r") as r:
     install_requires = r.readlines()
 
 
 setup(
     name="flaskwebgui",
-    version="1.0.4",
+    version="1.0.5",
     description="Create desktop applications with Flask/Django/FastAPI!",
     url="https://github.com/ClimenteA/flaskwebgui",
     author="Climente Alin",
     author_email="climente.alin@gmail.com",
     license="MIT",
     py_modules=["flaskwebgui"],
     install_requires=install_requires,
```

### Comparing `flaskwebgui-1.0.4/src/flaskwebgui.egg-info/PKG-INFO` & `flaskwebgui-1.0.5/src/flaskwebgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.0.4
+Version: 1.0.5
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flaskwebgui-1.0.4/src/flaskwebgui.py` & `flaskwebgui-1.0.5/src/flaskwebgui.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,16 +228,20 @@
         subprocess.run(self.browser_command)
 
         if self.browser_path is None:
             while self.__keyboard_interrupt is False:
                 time.sleep(1)
 
         if isinstance(server_process, Process):
+            if self.on_shutdown is not None:
+                self.on_shutdown()
             server_process.kill()
         else:
+            if self.on_shutdown is not None:
+                self.on_shutdown()
             kill_port(self.port)
 
     def run(self):
         if self.on_startup is not None:
             self.on_startup()
 
         if OPERATING_SYSTEM == "darwin":
@@ -255,9 +259,8 @@
             browser_thread.start()
             server_process.join()
             browser_thread.join()
         except KeyboardInterrupt:
             self.__keyboard_interrupt = True
             print("Stopped")
 
-        if self.on_shutdown is not None:
-            self.on_shutdown()
+        return server_process, browser_thread
```

