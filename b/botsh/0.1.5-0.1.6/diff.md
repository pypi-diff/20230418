# Comparing `tmp/botsh-0.1.5.tar.gz` & `tmp/botsh-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.5.tar", last modified: Tue Apr 18 16:31:11 2023, max compression
+gzip compressed data, was "botsh-0.1.6.tar", last modified: Tue Apr 18 16:38:16 2023, max compression
```

## Comparing `botsh-0.1.5.tar` & `botsh-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:31:11.034042 botsh-0.1.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2023-04-18 14:41:00.000000 botsh-0.1.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-04-18 14:41:00.000000 botsh-0.1.5/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:31:11.034042 botsh-0.1.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-04-18 16:17:51.000000 botsh-0.1.5/Pipfile
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    64876 2023-04-18 14:41:00.000000 botsh-0.1.5/Pipfile.lock
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3901 2023-04-18 14:41:00.000000 botsh-0.1.5/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-18 16:31:11.034042 botsh-0.1.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1597 2023-04-18 16:30:46.000000 botsh-0.1.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:31:11.030042 botsh-0.1.5/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:31:11.034042 botsh-0.1.5/src/botsh/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-18 14:41:00.000000 botsh-0.1.5/src/botsh/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3601 2023-04-18 15:21:53.000000 botsh-0.1.5/src/botsh/docker_exec.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      317 2023-04-18 14:41:00.000000 botsh-0.1.5/src/botsh/history.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1581 2023-04-18 16:30:29.000000 botsh-0.1.5/src/botsh/llm.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2023-04-18 14:41:00.000000 botsh-0.1.5/src/botsh/logging.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2718 2023-04-18 14:41:00.000000 botsh-0.1.5/src/botsh/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1204 2023-04-18 16:28:51.000000 botsh-0.1.5/src/botsh/prompt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-04-18 15:01:04.000000 botsh-0.1.5/src/botsh/task_driver.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:31:11.034042 botsh-0.1.5/src/botsh/templates/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1099 2023-04-18 16:29:47.000000 botsh-0.1.5/src/botsh/templates/prompt.jinja2
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:31:11.034042 botsh-0.1.5/src/botsh.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      881 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-04-18 16:31:10.000000 botsh-0.1.5/src/botsh.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2023-04-18 14:41:00.000000 botsh-0.1.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-04-18 14:41:00.000000 botsh-0.1.6/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:38:16.532794 botsh-0.1.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-04-18 16:17:51.000000 botsh-0.1.6/Pipfile
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    64876 2023-04-18 14:41:00.000000 botsh-0.1.6/Pipfile.lock
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3901 2023-04-18 14:41:00.000000 botsh-0.1.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-18 16:38:16.532794 botsh-0.1.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1597 2023-04-18 16:37:45.000000 botsh-0.1.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.528794 botsh-0.1.6/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.528794 botsh-0.1.6/src/botsh/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3601 2023-04-18 15:21:53.000000 botsh-0.1.6/src/botsh/docker_exec.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      317 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/history.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1581 2023-04-18 16:30:29.000000 botsh-0.1.6/src/botsh/llm.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/logging.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2718 2023-04-18 14:41:00.000000 botsh-0.1.6/src/botsh/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1204 2023-04-18 16:28:51.000000 botsh-0.1.6/src/botsh/prompt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-04-18 16:37:34.000000 botsh-0.1.6/src/botsh/task_driver.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/src/botsh/templates/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1099 2023-04-18 16:29:47.000000 botsh-0.1.6/src/botsh/templates/prompt.jinja2
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:38:16.532794 botsh-0.1.6/src/botsh.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      881 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-04-18 16:38:16.000000 botsh-0.1.6/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.5/LICENSE` & `botsh-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/PKG-INFO` & `botsh-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.5
+Version: 0.1.6
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botsh-0.1.5/Pipfile.lock` & `botsh-0.1.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/README.md` & `botsh-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/setup.py` & `botsh-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.5",
+    version="0.1.6",
     description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Paul Butler",
     author_email="paul@driftingin.space",
     url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
```

### Comparing `botsh-0.1.5/src/botsh/docker_exec.py` & `botsh-0.1.6/src/botsh/docker_exec.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/src/botsh/llm.py` & `botsh-0.1.6/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/src/botsh/main.py` & `botsh-0.1.6/src/botsh/main.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/src/botsh/prompt.py` & `botsh-0.1.6/src/botsh/prompt.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/src/botsh/task_driver.py` & `botsh-0.1.6/src/botsh/task_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 explanation=result.explanation,
             )
 
         exit_code, output = self.container.run_command(result.command)
         lines = output.splitlines()
         if len(lines) > 10:
             truncated = len(lines) - 10
-            result = (
+            output = (
                 f"[ {truncated} lines truncated ]"
                 + "\n".join(lines[-10:])
                 + "\n[...]\n"
             )
 
         self.history.append(
             CommandExecution(result.explanation, result.command, output, exit_code)
```

### Comparing `botsh-0.1.5/src/botsh/templates/prompt.jinja2` & `botsh-0.1.6/src/botsh/templates/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `botsh-0.1.5/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.6/src/botsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.5
+Version: 0.1.6
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botsh-0.1.5/src/botsh.egg-info/requires.txt` & `botsh-0.1.6/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

