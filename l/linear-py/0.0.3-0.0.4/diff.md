# Comparing `tmp/linear-py-0.0.3.tar.gz` & `tmp/linear-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear-py-0.0.3.tar", last modified: Mon Mar 27 20:58:27 2023, max compression
+gzip compressed data, was "linear-py-0.0.4.tar", last modified: Tue Apr 18 03:50:53 2023, max compression
```

## Comparing `linear-py-0.0.3.tar` & `linear-py-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ghost     (1000) ghost     (1000)        0 2023-03-27 20:58:27.185719 linear-py-0.0.3/
--rw-rw-r--   0 ghost     (1000) ghost     (1000)    34901 2023-03-27 20:04:45.000000 linear-py-0.0.3/LICENSE
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      594 2023-03-27 20:58:27.185719 linear-py-0.0.3/PKG-INFO
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      112 2023-03-27 20:15:54.000000 linear-py-0.0.3/README.md
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      104 2023-03-27 19:55:39.000000 linear-py-0.0.3/pyproject.toml
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      738 2023-03-27 20:58:27.185719 linear-py-0.0.3/setup.cfg
-drwxrwxr-x   0 ghost     (1000) ghost     (1000)        0 2023-03-27 20:58:27.185719 linear-py-0.0.3/src/
-drwxrwxr-x   0 ghost     (1000) ghost     (1000)        0 2023-03-27 20:58:27.185719 linear-py-0.0.3/src/linear/
--rw-rw-r--   0 ghost     (1000) ghost     (1000)       47 2023-03-27 20:37:12.000000 linear-py-0.0.3/src/linear/Exceptions.py
--rw-rw-r--   0 ghost     (1000) ghost     (1000)     1335 2023-03-27 20:57:47.000000 linear-py-0.0.3/src/linear/Linear.py
--rw-rw-r--   0 ghost     (1000) ghost     (1000)       26 2023-03-27 20:35:08.000000 linear-py-0.0.3/src/linear/__init__.py
-drwxrwxr-x   0 ghost     (1000) ghost     (1000)        0 2023-03-27 20:58:27.185719 linear-py-0.0.3/src/linear_py.egg-info/
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      594 2023-03-27 20:58:27.000000 linear-py-0.0.3/src/linear_py.egg-info/PKG-INFO
--rw-rw-r--   0 ghost     (1000) ghost     (1000)      295 2023-03-27 20:58:27.000000 linear-py-0.0.3/src/linear_py.egg-info/SOURCES.txt
--rw-rw-r--   0 ghost     (1000) ghost     (1000)        1 2023-03-27 20:58:27.000000 linear-py-0.0.3/src/linear_py.egg-info/dependency_links.txt
--rw-rw-r--   0 ghost     (1000) ghost     (1000)       17 2023-03-27 20:58:27.000000 linear-py-0.0.3/src/linear_py.egg-info/requires.txt
--rw-rw-r--   0 ghost     (1000) ghost     (1000)        7 2023-03-27 20:58:27.000000 linear-py-0.0.3/src/linear_py.egg-info/top_level.txt
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)    34901 2023-04-07 18:41:07.000000 linear-py-0.0.4/LICENSE
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-18 03:50:53.511351 linear-py-0.0.4/PKG-INFO
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      112 2023-04-07 18:41:07.000000 linear-py-0.0.4/README.md
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      104 2023-04-07 18:41:07.000000 linear-py-0.0.4/pyproject.toml
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      738 2023-04-18 03:50:53.511351 linear-py-0.0.4/setup.cfg
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.507351 linear-py-0.0.4/src/
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/src/linear/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       47 2023-04-07 18:41:07.000000 linear-py-0.0.4/src/linear/Exceptions.py
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)     2104 2023-04-18 03:30:27.000000 linear-py-0.0.4/src/linear/Linear.py
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       26 2023-04-07 18:41:07.000000 linear-py-0.0.4/src/linear/__init__.py
+drwxrwxr-x   0 valeness  (1000) valeness  (1000)        0 2023-04-18 03:50:53.511351 linear-py-0.0.4/src/linear_py.egg-info/
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      594 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/PKG-INFO
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)      295 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)        1 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)       17 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/requires.txt
+-rw-rw-r--   0 valeness  (1000) valeness  (1000)        7 2023-04-18 03:50:53.000000 linear-py-0.0.4/src/linear_py.egg-info/top_level.txt
```

### Comparing `linear-py-0.0.3/LICENSE` & `linear-py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linear-py-0.0.3/PKG-INFO` & `linear-py-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integrate with the linear graphQL in a pythonic way
 Home-page: https://gitlab.com/thinkhuman-public/linear-py
 Author: valeness
 Author-email: james@thinkhuman.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linear-py-0.0.3/setup.cfg` & `linear-py-0.0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = linear-py
-version = 0.0.3
+version = 0.0.4
 author = valeness
 author_email = james@thinkhuman.co
 description = Integrate with the linear graphQL in a pythonic way
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/thinkhuman-public/linear-py
 classifiers =
```

### Comparing `linear-py-0.0.3/src/linear/Linear.py` & `linear-py-0.0.4/src/linear/Linear.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,16 +35,37 @@
             """
                 query Resource {"""+resource+"""{nodes{id,name}}}
             """
         )
 
         return resource_response["data"][resource]["nodes"]
 
-    def create_issue(self, project=''):
-        pass
+    def create_issue(self, title, description='', project_id='', state_id='', team_id=''):
+        create_response = self.query_grapql(
+            """
+            mutation IssueCreate {{
+              issueCreate(
+                input: {{
+                    title: "{title}"
+                    description: "{description}"
+                    projectId: "{project_id}"
+                    stateId: "{state_id}"
+                    teamId: "{team_id}"
+                }}
+              ) {{
+                success
+                issue {{
+                  id
+                  title
+                }}
+              }}
+            }}
+            """.format(title=title, description=description, project_id=project_id, team_id=team_id, state_id=state_id)
+        )
+        return create_response['data']['issueCreate']
 
     def teams(self):
         return self.query_basic_resource('teams')
 
     def states(self):
         return self.query_basic_resource('workflowStates')
```

### Comparing `linear-py-0.0.3/src/linear_py.egg-info/PKG-INFO` & `linear-py-0.0.4/src/linear_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integrate with the linear graphQL in a pythonic way
 Home-page: https://gitlab.com/thinkhuman-public/linear-py
 Author: valeness
 Author-email: james@thinkhuman.co
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

