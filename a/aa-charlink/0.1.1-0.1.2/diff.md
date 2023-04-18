# Comparing `tmp/aa-charlink-0.1.1.tar.gz` & `tmp/aa-charlink-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.1.1.tar", last modified: Mon Apr 17 20:17:05 2023, max compression
+gzip compressed data, was "aa-charlink-0.1.2.tar", last modified: Tue Apr 18 07:34:50 2023, max compression
```

## Comparing `aa-charlink-0.1.1.tar` & `aa-charlink-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.664034 aa-charlink-0.1.1/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 20:17:05.000000 aa-charlink-0.1.1/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.664034 aa-charlink-0.1.1/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/app_imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/charlink/imports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/imports/corptools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/imports/memberaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/imports/miningtaxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.660034 aa-charlink-0.1.1/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/charlink/templates/charlink/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-17 20:16:52.000000 aa-charlink-0.1.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1578 2023-04-17 20:17:05.668034 aa-charlink-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.746011 aa-charlink-0.1.2/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 07:34:50.000000 aa-charlink-0.1.2/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/app_imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/corptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/memberaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/imports/miningtaxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.746011 aa-charlink-0.1.2/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/charlink/templates/charlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-18 07:34:33.000000 aa-charlink-0.1.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-18 07:34:50.750011 aa-charlink-0.1.2/setup.cfg
```

### Comparing `aa-charlink-0.1.1/LICENSE` & `aa-charlink-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/aa_charlink.egg-info/SOURCES.txt` & `aa-charlink-0.1.2/aa_charlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/app_imports.py` & `aa-charlink-0.1.2/charlink/app_imports.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/forms.py` & `aa-charlink-0.1.2/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/imports/corptools.py` & `aa-charlink-0.1.2/charlink/imports/corptools.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/imports/memberaudit.py` & `aa-charlink-0.1.2/charlink/imports/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/imports/miningtaxes.py` & `aa-charlink-0.1.2/charlink/imports/miningtaxes.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/charlink/templates/charlink/charlink.html` & `aa-charlink-0.1.2/charlink/templates/charlink/charlink.html`

 * *Files 20% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 {% block content %}
     <div class="col-lg-12">
         <h1 class="page-header text-center">Character Linking</h1>
         <div class="text-center">
             <form method="post">
                 {% csrf_token %}
                 {{ form|bootstrap }}
-                <button type="submit" class="btn btn-primary">Link</button>
+                <button type="submit" class="btn btn-primary">Login</button>
             </form>
         </div>
     </div>
 {% endblock content %}
```

### Comparing `aa-charlink-0.1.1/charlink/views.py` & `aa-charlink-0.1.2/charlink/views.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.1.1/setup.cfg` & `aa-charlink-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
@@ -17,15 +17,15 @@
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Operating System :: POSIX :: Linux
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -44,15 +44,15 @@
 	eveonline
 url = https://github.com/Maestro-Zacht/aa-charlink
 
 [options]
 packages = find:
 python_requires = ~=3.8
 install_requires = 
-	allianceauth~=3.3
+	allianceauth~=3.0
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = charlink*
 
 [bdist_wheel]
```

