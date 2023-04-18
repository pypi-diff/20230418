# Comparing `tmp/genepattern-notebook-23.1.0.tar.gz` & `tmp/genepattern-notebook-23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepattern-notebook-23.1.0.tar", last modified: Mon Feb  6 20:52:56 2023, max compression
+gzip compressed data, was "genepattern-notebook-23.4.tar", last modified: Tue Apr 18 15:52:54 2023, max compression
```

## Comparing `genepattern-notebook-23.1.0.tar` & `genepattern-notebook-23.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 20:52:56.247385 genepattern-notebook-23.1.0/
--rw-r--r--   0 tmtabor    (501) staff       (20)     1562 2022-01-03 20:10:07.000000 genepattern-notebook-23.1.0/LICENSE.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       67 2022-01-03 20:10:07.000000 genepattern-notebook-23.1.0/MANIFEST.in
--rw-r--r--   0 tmtabor    (501) staff       (20)     7987 2023-02-06 20:52:56.247569 genepattern-notebook-23.1.0/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)     7019 2022-04-20 16:34:45.000000 genepattern-notebook-23.1.0/README.md
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 20:52:56.245647 genepattern-notebook-23.1.0/genepattern/
--rw-r--r--   0 tmtabor    (501) staff       (20)      529 2023-02-06 20:51:48.000000 genepattern-notebook-23.1.0/genepattern/__init__.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     7509 2022-10-05 17:00:59.000000 genepattern-notebook-23.1.0/genepattern/authwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)      859 2022-09-12 21:39:43.000000 genepattern-notebook-23.1.0/genepattern/display.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    13696 2022-10-27 20:54:28.000000 genepattern-notebook-23.1.0/genepattern/jobwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     3294 2022-04-25 16:13:37.000000 genepattern-notebook-23.1.0/genepattern/sessions.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     5103 2022-04-20 16:34:37.000000 genepattern-notebook-23.1.0/genepattern/shim.py
--rw-r--r--   0 tmtabor    (501) staff       (20)    15956 2022-09-22 21:16:50.000000 genepattern-notebook-23.1.0/genepattern/taskwidget.py
--rw-r--r--   0 tmtabor    (501) staff       (20)     9476 2022-10-27 20:20:12.000000 genepattern-notebook-23.1.0/genepattern/utils.py
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 20:52:56.246813 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/
--rw-r--r--   0 tmtabor    (501) staff       (20)     7987 2023-02-06 20:52:55.000000 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/PKG-INFO
--rw-r--r--   0 tmtabor    (501) staff       (20)      485 2023-02-06 20:52:56.000000 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-02-06 20:52:55.000000 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       79 2023-02-06 20:52:55.000000 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/requires.txt
--rw-r--r--   0 tmtabor    (501) staff       (20)       12 2023-02-06 20:52:56.000000 genepattern-notebook-23.1.0/genepattern_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-02-06 20:52:56.247107 genepattern-notebook-23.1.0/nbtools/
--rw-r--r--   0 tmtabor    (501) staff       (20)       29 2022-04-20 16:34:37.000000 genepattern-notebook-23.1.0/nbtools/genepattern.json
--rw-r--r--   0 tmtabor    (501) staff       (20)       79 2023-02-06 20:52:56.248015 genepattern-notebook-23.1.0/setup.cfg
--rwxr-xr-x   0 tmtabor    (501) staff       (20)     1556 2023-02-06 20:51:56.000000 genepattern-notebook-23.1.0/setup.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.492458 genepattern-notebook-23.4/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     1562 2022-01-03 20:10:07.000000 genepattern-notebook-23.4/LICENSE.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       67 2022-01-03 20:10:07.000000 genepattern-notebook-23.4/MANIFEST.in
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7983 2023-04-18 15:52:54.492571 genepattern-notebook-23.4/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7019 2022-04-20 16:34:45.000000 genepattern-notebook-23.4/README.md
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.490228 genepattern-notebook-23.4/genepattern/
+-rw-r--r--   0 tmtabor    (501) staff       (20)      534 2023-04-17 17:48:15.000000 genepattern-notebook-23.4/genepattern/__init__.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7752 2023-04-17 17:43:14.000000 genepattern-notebook-23.4/genepattern/authwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)      859 2022-09-12 21:39:43.000000 genepattern-notebook-23.4/genepattern/display.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)    13696 2022-10-27 20:54:28.000000 genepattern-notebook-23.4/genepattern/jobwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     3294 2022-04-25 16:13:37.000000 genepattern-notebook-23.4/genepattern/sessions.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     5103 2022-04-20 16:34:37.000000 genepattern-notebook-23.4/genepattern/shim.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)    15956 2022-09-22 21:16:50.000000 genepattern-notebook-23.4/genepattern/taskwidget.py
+-rw-r--r--   0 tmtabor    (501) staff       (20)     9476 2022-10-27 20:20:12.000000 genepattern-notebook-23.4/genepattern/utils.py
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.491763 genepattern-notebook-23.4/genepattern_notebook.egg-info/
+-rw-r--r--   0 tmtabor    (501) staff       (20)     7983 2023-04-18 15:52:53.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 tmtabor    (501) staff       (20)      485 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)        1 2023-04-18 15:52:53.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       81 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/requires.txt
+-rw-r--r--   0 tmtabor    (501) staff       (20)       12 2023-04-18 15:52:54.000000 genepattern-notebook-23.4/genepattern_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 tmtabor    (501) staff       (20)        0 2023-04-18 15:52:54.491998 genepattern-notebook-23.4/nbtools/
+-rw-r--r--   0 tmtabor    (501) staff       (20)       29 2022-04-20 16:34:37.000000 genepattern-notebook-23.4/nbtools/genepattern.json
+-rw-r--r--   0 tmtabor    (501) staff       (20)       79 2023-04-18 15:52:54.492970 genepattern-notebook-23.4/setup.cfg
+-rwxr-xr-x   0 tmtabor    (501) staff       (20)     1556 2023-04-17 19:06:30.000000 genepattern-notebook-23.4/setup.py
```

### Comparing `genepattern-notebook-23.1.0/LICENSE.txt` & `genepattern-notebook-23.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/PKG-INFO` & `genepattern-notebook-23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: genepattern-notebook
-Version: 23.1.0
+Version: 23.4
 Summary: GenePattern Notebook extension for JupyterLab
 Home-page: https://github.com/genepattern/genepattern-notebook
-Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.1.0.tar.gz
+Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.4.tar.gz
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD
 Keywords: genepattern,genomics,bioinformatics,ipython,jupyter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `genepattern-notebook-23.1.0/README.md` & `genepattern-notebook-23.4/README.md`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/__init__.py` & `genepattern-notebook-23.4/genepattern/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,11 +2,11 @@
 from .taskwidget import GPTaskWidget, reproduce_job, load_task
 from .jobwidget import GPJobWidget
 from .sessions import session, get_session, register_session
 from .display import display
 from nbtools import UIBuilder as GPUIBuilder, UIOutput as GPUIOutput, build_ui, open
 
 __author__ = 'Thorin Tabor'
-__copyright__ = 'Copyright 2014-2022, Regents of the University of California & Broad Institute'
-__version__ = '23.1.0'
-__status__ = 'Beta'
+__copyright__ = 'Copyright 2014-2023, Regents of the University of California & Broad Institute'
+__version__ = '23.04'
+__status__ = 'Production'
 __license__ = 'BSD-3-Clause'
```

### Comparing `genepattern-notebook-23.1.0/genepattern/authwidget.py` & `genepattern-notebook-23.4/genepattern/authwidget.py`

 * *Files 15% similar despite different names*

```diff
@@ -87,42 +87,47 @@
         else: self.session = session
 
         # Set blank token
         self.token = None
 
         # Check to see if the provided session has valid credentials
         if self.has_credentials() and self.validate_credentials():
-            self.register_session()     # Register the session with the SessionList
-            self.register_modules()     # Register the modules with the ToolManager
-            self.system_message()       # Display the system message
-            self.trigger_login()        # Trigger login callbacks of job and task widgets
+            self.prepare_session()
 
             # Display the widget with the system message and no form
             UIBuilder.__init__(self, lambda: None, name=self.session.username, subtitle=self.session.url,
                                display_header=False, display_footer=False, color=session_color(self.session.url),
                                collapsed=True, logo=GENEPATTERN_LOGO, **kwargs)
 
         # If not, prompt the user to login
         else:
             # Apply the display spec
             for key, value in self.login_spec.items(): kwargs[key] = value
 
             # Call the superclass constructor with the spec
             UIBuilder.__init__(self, self.login, **kwargs)
 
+    def prepare_session(self):
+        """Prepare a valid session by registering the session and modules"""
+        self.register_session()     # Register the session with the SessionList
+        self.register_modules()     # Register the modules with the ToolManager
+        self.system_message()       # Display the system message
+        self.trigger_login()        # Trigger login callbacks of job and task widgets
+
     def login(self, server, username, password):
         """Login to the GenePattern server"""
         # Assign login values to session
         self.session.url = server
         self.session.username = username
         self.session.password = password
 
         # Validate the provided credentials
         if self.validate_credentials():
             self.replace_widget()
+            self.prepare_session()
 
     def has_credentials(self):
         """Test whether the session object is instantiated and whether a username and password have been provided"""
         if type(self.session) is not gp.GPServer: return False  # Test type
         if not self.session.url: return False                   # Test server url
         if not self.session.username: return False              # Test username
         if not self.session.password: return False              # Test password
@@ -140,18 +145,22 @@
             self.error = 'Invalid username or password. Please try again.'
             return False
         except BaseException as e:
             self.error = str(e)
             return False
 
     def replace_widget(self):
-        """Replace the unauthenticated widget with the authenticated widget"""
-        self.form.children[2].value = ''        # Blank password so it doesn't get serialized
-        display(GPAuthWidget(self.session))     # Display the authenticated widget
-        self.close()                            # Close the unauthenticated widget
+        """Replace the unauthenticated widget with the authenticated mode"""
+        self.form.form.children[2].value = ''        # Blank password so it doesn't get serialized
+        self.form.collapsed = True
+        self.form.name = self.session.username
+        self.form.subtitle = self.session.url
+        self.form.display_header=False
+        self.form.display_footer=False
+        self.form.form.children = []
 
     def register_session(self):
         """Register the validated credentials with the SessionList"""
         self.session = session.register(self.session.url, self.session.username, self.session.password)
 
     def register_modules(self):
         """Get the list available modules and register widgets for them with the tool manager"""
```

### Comparing `genepattern-notebook-23.1.0/genepattern/display.py` & `genepattern-notebook-23.4/genepattern/display.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/jobwidget.py` & `genepattern-notebook-23.4/genepattern/jobwidget.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/sessions.py` & `genepattern-notebook-23.4/genepattern/sessions.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/shim.py` & `genepattern-notebook-23.4/genepattern/shim.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/taskwidget.py` & `genepattern-notebook-23.4/genepattern/taskwidget.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern/utils.py` & `genepattern-notebook-23.4/genepattern/utils.py`

 * *Files identical despite different names*

### Comparing `genepattern-notebook-23.1.0/genepattern_notebook.egg-info/PKG-INFO` & `genepattern-notebook-23.4/genepattern_notebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: genepattern-notebook
-Version: 23.1.0
+Version: 23.4
 Summary: GenePattern Notebook extension for JupyterLab
 Home-page: https://github.com/genepattern/genepattern-notebook
-Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.1.0.tar.gz
+Download-URL: https://github.com/genepattern/genepattern-notebook/archive/23.4.tar.gz
 Author: Thorin Tabor
 Author-email: tmtabor@cloud.ucsd.edu
 License: BSD
 Keywords: genepattern,genomics,bioinformatics,ipython,jupyter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `genepattern-notebook-23.1.0/setup.py` & `genepattern-notebook-23.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 
-__version__ = '23.1.0'
+__version__ = '23.4'
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(name='genepattern-notebook',
@@ -30,15 +30,15 @@
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Framework :: Jupyter',
       ],
       install_requires=[
           'genepattern-python>=1.4.2',
-          'nbtools>=20',
+          'nbtools>=23.4',
           'notebook>=5.0.0',
           'ipywidgets>=7.0.0',
           'pandas',
       ],
       data_files=[("share/jupyter/nbtools", ["nbtools/genepattern.json"])],
       normalize_version=False,
       )
```

