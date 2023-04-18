# Comparing `tmp/bcligpt-1.0.0.tar.gz` & `tmp/bcligpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcligpt-1.0.0.tar", last modified: Tue Apr 11 12:31:42 2023, max compression
+gzip compressed data, was "bcligpt-1.0.1.tar", last modified: Tue Apr 18 12:50:31 2023, max compression
```

## Comparing `bcligpt-1.0.0.tar` & `bcligpt-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.114300 bcligpt-1.0.0/
--rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-11 12:31:42.114300 bcligpt-1.0.0/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-04-03 14:53:27.000000 bcligpt-1.0.0/README.md
--rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-04-11 12:31:38.000000 bcligpt-1.0.0/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-11 12:31:42.114300 bcligpt-1.0.0/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.106300 bcligpt-1.0.0/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.110300 bcligpt-1.0.0/src/bcligpt/
--rw-r--r--   0 marco     (1000) marco     (1000)       48 2023-04-03 15:22:45.000000 bcligpt-1.0.0/src/bcligpt/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2953 2023-04-11 12:28:20.000000 bcligpt-1.0.0/src/bcligpt/app.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-11 12:31:42.114300 bcligpt-1.0.0/src/bcligpt.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      279 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        8 2023-04-11 12:31:42.000000 bcligpt-1.0.0/src/bcligpt.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 12:50:31.093027 bcligpt-1.0.1/
+-rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-18 12:50:31.089027 bcligpt-1.0.1/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      133 2023-04-03 14:53:27.000000 bcligpt-1.0.1/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)      374 2023-04-18 12:50:27.000000 bcligpt-1.0.1/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-18 12:50:31.093027 bcligpt-1.0.1/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 12:50:31.085027 bcligpt-1.0.1/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 12:50:31.089027 bcligpt-1.0.1/src/bcligpt/
+-rw-r--r--   0 marco     (1000) marco     (1000)       48 2023-04-03 15:22:45.000000 bcligpt-1.0.1/src/bcligpt/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2954 2023-04-18 12:46:55.000000 bcligpt-1.0.1/src/bcligpt/app.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 12:50:31.089027 bcligpt-1.0.1/src/bcligpt.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)      319 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      279 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       42 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        8 2023-04-18 12:50:31.000000 bcligpt-1.0.1/src/bcligpt.egg-info/top_level.txt
```

### Comparing `bcligpt-1.0.0/src/bcligpt/app.py` & `bcligpt-1.0.1/src/bcligpt/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,13 +57,13 @@
                         content = chunk['choices'][0]['delta']['content']
                         full_content += content
                         md = Markdown(full_content, code_theme=code_theme)
                         live.update(md)
             message_token_count = len(encoding.encode(full_content))
             tokens += message_token_count
             messages.append({"role": "assistant", "content": full_content})
-            cost = tokens * 0.002 / 1000
+            cost += tokens * 0.002 / 1000
         except InvalidRequestError as e:
             print("Error: ", e)
             while tokens > 3500:
                 popped_message = messages.pop(1)
                 tokens -= len(encoding.encode(popped_message["content"]))
```

