# Comparing `tmp/todonotifier-1.2.2.tar.gz` & `tmp/todonotifier-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todonotifier-1.2.2.tar", last modified: Sun Dec 18 04:40:38 2022, max compression
+gzip compressed data, was "todonotifier-1.2.3.tar", last modified: Tue Apr 18 16:53:21 2023, max compression
```

## Comparing `todonotifier-1.2.2.tar` & `todonotifier-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2022-12-18 04:40:38.821322 todonotifier-1.2.2/
--rw-r--r--   0 ashutosh   (501) staff       (20)     9546 2022-12-18 04:40:38.821392 todonotifier-1.2.2/PKG-INFO
--rw-r--r--   0 ashutosh   (501) staff       (20)     9213 2022-11-19 11:15:02.000000 todonotifier-1.2.2/README.md
--rw-r--r--   0 ashutosh   (501) staff       (20)      199 2022-11-09 19:58:39.000000 todonotifier-1.2.2/pyproject.toml
--rw-r--r--   0 ashutosh   (501) staff       (20)      107 2022-12-18 04:40:38.821915 todonotifier-1.2.2/setup.cfg
--rw-r--r--   0 ashutosh   (501) staff       (20)      705 2022-12-18 04:40:33.000000 todonotifier-1.2.2/setup.py
-drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2022-12-18 04:40:38.820689 todonotifier-1.2.2/todonotifier/
--rw-r--r--   0 ashutosh   (501) staff       (20)        0 2022-12-18 04:40:33.000000 todonotifier-1.2.2/todonotifier/__init__.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     7848 2022-11-19 10:46:25.000000 todonotifier-1.2.2/todonotifier/config.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     5855 2022-11-12 09:38:11.000000 todonotifier-1.2.2/todonotifier/connect.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     3563 2022-11-12 09:38:11.000000 todonotifier-1.2.2/todonotifier/constants.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     2549 2022-11-19 11:05:35.000000 todonotifier-1.2.2/todonotifier/driver.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     4360 2022-11-19 10:46:25.000000 todonotifier-1.2.2/todonotifier/models.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     3276 2022-11-19 11:05:35.000000 todonotifier-1.2.2/todonotifier/notifier.py
--rw-r--r--   0 ashutosh   (501) staff       (20)    12267 2022-11-19 10:46:25.000000 todonotifier-1.2.2/todonotifier/summary_generators.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     3530 2022-11-12 09:38:11.000000 todonotifier-1.2.2/todonotifier/todo_notifier.py
--rw-r--r--   0 ashutosh   (501) staff       (20)     7693 2022-11-12 09:38:11.000000 todonotifier-1.2.2/todonotifier/utils.py
-drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2022-12-18 04:40:38.821222 todonotifier-1.2.2/todonotifier.egg-info/
--rw-r--r--   0 ashutosh   (501) staff       (20)     9546 2022-12-18 04:40:38.000000 todonotifier-1.2.2/todonotifier.egg-info/PKG-INFO
--rw-r--r--   0 ashutosh   (501) staff       (20)      478 2022-12-18 04:40:38.000000 todonotifier-1.2.2/todonotifier.egg-info/SOURCES.txt
--rw-r--r--   0 ashutosh   (501) staff       (20)        1 2022-12-18 04:40:38.000000 todonotifier-1.2.2/todonotifier.egg-info/dependency_links.txt
--rw-r--r--   0 ashutosh   (501) staff       (20)       41 2022-12-18 04:40:38.000000 todonotifier-1.2.2/todonotifier.egg-info/requires.txt
--rw-r--r--   0 ashutosh   (501) staff       (20)       13 2022-12-18 04:40:38.000000 todonotifier-1.2.2/todonotifier.egg-info/top_level.txt
+drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2023-04-18 16:53:21.585257 todonotifier-1.2.3/
+-rw-r--r--   0 ashutosh   (501) staff       (20)     9742 2023-04-18 16:53:21.585373 todonotifier-1.2.3/PKG-INFO
+-rw-r--r--   0 ashutosh   (501) staff       (20)     9409 2023-04-18 16:47:37.000000 todonotifier-1.2.3/README.md
+-rw-r--r--   0 ashutosh   (501) staff       (20)      199 2022-11-09 19:58:39.000000 todonotifier-1.2.3/pyproject.toml
+-rw-r--r--   0 ashutosh   (501) staff       (20)      107 2023-04-18 16:53:21.585806 todonotifier-1.2.3/setup.cfg
+-rw-r--r--   0 ashutosh   (501) staff       (20)      705 2023-04-18 16:47:37.000000 todonotifier-1.2.3/setup.py
+drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2023-04-18 16:53:21.581344 todonotifier-1.2.3/tests/
+-rw-r--r--   0 ashutosh   (501) staff       (20)     5290 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_config.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     7218 2022-11-12 09:38:11.000000 todonotifier-1.2.3/tests/test_connect.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     1357 2022-11-12 09:38:11.000000 todonotifier-1.2.3/tests/test_constants.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     4122 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_driver.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     3057 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_models.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     2816 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_notifier.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     8443 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_summary_generators.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)    13792 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_todo_notifier.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)    12638 2023-01-16 06:23:00.000000 todonotifier-1.2.3/tests/test_utils.py
+drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2023-04-18 16:53:21.584030 todonotifier-1.2.3/todonotifier/
+-rw-r--r--   0 ashutosh   (501) staff       (20)        0 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/__init__.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     7848 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/config.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     5855 2022-11-12 09:38:11.000000 todonotifier-1.2.3/todonotifier/connect.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     3563 2022-11-12 09:38:11.000000 todonotifier-1.2.3/todonotifier/constants.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     2549 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/driver.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     4360 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/models.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     3276 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/notifier.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)    12267 2023-01-16 06:23:00.000000 todonotifier-1.2.3/todonotifier/summary_generators.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     3530 2022-11-12 09:38:11.000000 todonotifier-1.2.3/todonotifier/todo_notifier.py
+-rw-r--r--   0 ashutosh   (501) staff       (20)     7693 2022-11-12 09:38:11.000000 todonotifier-1.2.3/todonotifier/utils.py
+drwxr-xr-x   0 ashutosh   (501) staff       (20)        0 2023-04-18 16:53:21.585083 todonotifier-1.2.3/todonotifier.egg-info/
+-rw-r--r--   0 ashutosh   (501) staff       (20)     9742 2023-04-18 16:53:21.000000 todonotifier-1.2.3/todonotifier.egg-info/PKG-INFO
+-rw-r--r--   0 ashutosh   (501) staff       (20)      691 2023-04-18 16:53:21.000000 todonotifier-1.2.3/todonotifier.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutosh   (501) staff       (20)        1 2023-04-18 16:53:21.000000 todonotifier-1.2.3/todonotifier.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutosh   (501) staff       (20)       41 2023-04-18 16:53:21.000000 todonotifier-1.2.3/todonotifier.egg-info/requires.txt
+-rw-r--r--   0 ashutosh   (501) staff       (20)       13 2023-04-18 16:53:21.000000 todonotifier-1.2.3/todonotifier.egg-info/top_level.txt
```

### Comparing `todonotifier-1.2.2/PKG-INFO` & `todonotifier-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todonotifier
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to setup automatic TODO Notifications in code
 Home-page: https://github.com/ashu-tosh-kumar/todo_notifier
 Download-URL: https://pypi.org/project/todonotifier/
 Author: Ashutosh Kumar
 License: MIT
 Keywords: todo,notifier
 Description-Content-Type: text/markdown
@@ -21,14 +21,15 @@
     - [Working](#working)
     - [Salient Features](#salient-features)
     - [Other Salient Features](#other-salient-features)
 
 ## Description
 
 > Find project on [GitHub](https://github.com/ashu-tosh-kumar/todo_notifier), [PyPi](https://pypi.org/project/todonotifier/)
+> Medium Article detailing about TODO Notifier and how to use it (complements README): [Medium](https://medium.com/@at-k/streamline-your-todos-with-todo-notifier-for-python-projects-6f95c03a2d34)
 
 More often than not, we put some TODO items in code and forget about them. Sometimes, we think of coming back to a TODO item by some date but miss it being too busy with some other development.
 
 TODO Notifier aims to solve this problem. It parses through any project, collects all the todo items, generates automated summaries and send automated reminders about them.
 
 Recommended format to write TODO items**
```

### Comparing `todonotifier-1.2.2/README.md` & `todonotifier-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     - [Working](#working)
     - [Salient Features](#salient-features)
     - [Other Salient Features](#other-salient-features)
 
 ## Description
 
 > Find project on [GitHub](https://github.com/ashu-tosh-kumar/todo_notifier), [PyPi](https://pypi.org/project/todonotifier/)
+> Medium Article detailing about TODO Notifier and how to use it (complements README): [Medium](https://medium.com/@at-k/streamline-your-todos-with-todo-notifier-for-python-projects-6f95c03a2d34)
 
 More often than not, we put some TODO items in code and forget about them. Sometimes, we think of coming back to a TODO item by some date but miss it being too busy with some other development.
 
 TODO Notifier aims to solve this problem. It parses through any project, collects all the todo items, generates automated summaries and send automated reminders about them.
 
 Recommended format to write TODO items**
```

### Comparing `todonotifier-1.2.2/setup.py` & `todonotifier-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/ashu-tosh-kumar/todo_notifier",
     author="Ashutosh Kumar",
     download_url="https://pypi.org/project/todonotifier/",
     license="MIT",
     test_suite="unittest",
-    version="1.2.2",
+    version="1.2.3",
     keywords=["todo", "notifier"],
     packages=find_packages(exclude=["tests", "sample_reports"]),
     install_requires=[
-        "GitPython==3.1.29",
+        "GitPython==3.1.31",
         "python-dateutil==2.8.2",
     ],
 )
```

### Comparing `todonotifier-1.2.2/todonotifier/config.py` & `todonotifier-1.2.3/todonotifier/config.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/connect.py` & `todonotifier-1.2.3/todonotifier/connect.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/constants.py` & `todonotifier-1.2.3/todonotifier/constants.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/driver.py` & `todonotifier-1.2.3/todonotifier/driver.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/models.py` & `todonotifier-1.2.3/todonotifier/models.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/notifier.py` & `todonotifier-1.2.3/todonotifier/notifier.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/summary_generators.py` & `todonotifier-1.2.3/todonotifier/summary_generators.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/todo_notifier.py` & `todonotifier-1.2.3/todonotifier/todo_notifier.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier/utils.py` & `todonotifier-1.2.3/todonotifier/utils.py`

 * *Files identical despite different names*

### Comparing `todonotifier-1.2.2/todonotifier.egg-info/PKG-INFO` & `todonotifier-1.2.3/todonotifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todonotifier
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to setup automatic TODO Notifications in code
 Home-page: https://github.com/ashu-tosh-kumar/todo_notifier
 Download-URL: https://pypi.org/project/todonotifier/
 Author: Ashutosh Kumar
 License: MIT
 Keywords: todo,notifier
 Description-Content-Type: text/markdown
@@ -21,14 +21,15 @@
     - [Working](#working)
     - [Salient Features](#salient-features)
     - [Other Salient Features](#other-salient-features)
 
 ## Description
 
 > Find project on [GitHub](https://github.com/ashu-tosh-kumar/todo_notifier), [PyPi](https://pypi.org/project/todonotifier/)
+> Medium Article detailing about TODO Notifier and how to use it (complements README): [Medium](https://medium.com/@at-k/streamline-your-todos-with-todo-notifier-for-python-projects-6f95c03a2d34)
 
 More often than not, we put some TODO items in code and forget about them. Sometimes, we think of coming back to a TODO item by some date but miss it being too busy with some other development.
 
 TODO Notifier aims to solve this problem. It parses through any project, collects all the todo items, generates automated summaries and send automated reminders about them.
 
 Recommended format to write TODO items**
```

