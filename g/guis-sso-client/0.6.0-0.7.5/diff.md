# Comparing `tmp/guis_sso_client-0.6.0.tar.gz` & `tmp/guis_sso_client-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guis_sso_client-0.6.0.tar", last modified: Tue Apr 18 09:54:12 2023, max compression
+gzip compressed data, was "guis_sso_client-0.7.5.tar", last modified: Tue Apr 18 09:58:19 2023, max compression
```

## Comparing `guis_sso_client-0.6.0.tar` & `guis_sso_client-0.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.385132 guis_sso_client-0.6.0/
--rw-r--r--   0 mpilia     (501) staff       (20)      190 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/MANIFEST.in
--rw-r--r--   0 mpilia     (501) staff       (20)       59 2023-04-18 09:54:12.385217 guis_sso_client-0.6.0/PKG-INFO
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.383162 guis_sso_client-0.6.0/guis_sso_client/
--rw-r--r--   0 mpilia     (501) staff       (20)      171 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/__init__.py
--rw-r--r--   0 mpilia     (501) staff       (20)     2678 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/admin.py
--rw-r--r--   0 mpilia     (501) staff       (20)     2699 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/apps.py
--rw-r--r--   0 mpilia     (501) staff       (20)     1854 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/backends.py
--rw-r--r--   0 mpilia     (501) staff       (20)      514 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/context_processors.py
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384046 guis_sso_client-0.6.0/guis_sso_client/management/
--rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/management/__init__.py
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384253 guis_sso_client-0.6.0/guis_sso_client/management/commands/
--rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/management/commands/__init__.py
--rw-r--r--   0 mpilia     (501) staff       (20)     1167 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/management/commands/pushgroups.py
--rw-r--r--   0 mpilia     (501) staff       (20)     3750 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/middleware.py
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384406 guis_sso_client-0.6.0/guis_sso_client/migrations/
--rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/migrations/__init__.py
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.380786 guis_sso_client-0.6.0/guis_sso_client/static/
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384514 guis_sso_client-0.6.0/guis_sso_client/static/js/
--rw-r--r--   0 mpilia     (501) staff       (20)     1011 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/static/js/guis_sso_smartcheck.js
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.380984 guis_sso_client-0.6.0/guis_sso_client/templates/
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384749 guis_sso_client-0.6.0/guis_sso_client/templates/applications/
--rw-r--r--   0 mpilia     (501) staff       (20)      455 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/templates/applications/guis_applications.html
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.384930 guis_sso_client-0.6.0/guis_sso_client/templates/sso/
--rw-r--r--   0 mpilia     (501) staff       (20)      432 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/templates/sso/guis_sso_smartcheck.html
--rw-r--r--   0 mpilia     (501) staff       (20)       60 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/tests.py
--rw-r--r--   0 mpilia     (501) staff       (20)      315 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/urls.py
--rw-r--r--   0 mpilia     (501) staff       (20)     3763 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/utils.py
--rw-r--r--   0 mpilia     (501) staff       (20)     2808 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/guis_sso_client/views.py
-drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:54:12.383926 guis_sso_client-0.6.0/guis_sso_client.egg-info/
--rw-r--r--   0 mpilia     (501) staff       (20)       59 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/PKG-INFO
--rw-r--r--   0 mpilia     (501) staff       (20)      876 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpilia     (501) staff       (20)        1 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpilia     (501) staff       (20)        1 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/not-zip-safe
--rw-r--r--   0 mpilia     (501) staff       (20)       80 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/requires.txt
--rw-r--r--   0 mpilia     (501) staff       (20)       16 2023-04-18 09:54:12.000000 guis_sso_client-0.6.0/guis_sso_client.egg-info/top_level.txt
--rw-r--r--   0 mpilia     (501) staff       (20)       67 2023-04-18 09:54:12.385440 guis_sso_client-0.6.0/setup.cfg
--rw-r--r--   0 mpilia     (501) staff       (20)      475 2023-04-18 09:45:19.000000 guis_sso_client-0.6.0/setup.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.553189 guis_sso_client-0.7.5/
+-rw-r--r--   0 mpilia     (501) staff       (20)      190 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/MANIFEST.in
+-rw-r--r--   0 mpilia     (501) staff       (20)       59 2023-04-18 09:58:19.553233 guis_sso_client-0.7.5/PKG-INFO
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.551333 guis_sso_client-0.7.5/guis_sso_client/
+-rw-r--r--   0 mpilia     (501) staff       (20)      171 2023-04-18 09:58:08.000000 guis_sso_client-0.7.5/guis_sso_client/__init__.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     2678 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/admin.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     2699 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/apps.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     2307 2023-04-18 09:58:08.000000 guis_sso_client-0.7.5/guis_sso_client/backends.py
+-rw-r--r--   0 mpilia     (501) staff       (20)      514 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/context_processors.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552419 guis_sso_client-0.7.5/guis_sso_client/management/
+-rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/management/__init__.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552623 guis_sso_client-0.7.5/guis_sso_client/management/commands/
+-rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/management/commands/__init__.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     1167 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/management/commands/pushgroups.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     3750 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/middleware.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552745 guis_sso_client-0.7.5/guis_sso_client/migrations/
+-rw-r--r--   0 mpilia     (501) staff       (20)        0 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/migrations/__init__.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.549575 guis_sso_client-0.7.5/guis_sso_client/static/
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552844 guis_sso_client-0.7.5/guis_sso_client/static/js/
+-rw-r--r--   0 mpilia     (501) staff       (20)     1011 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/static/js/guis_sso_smartcheck.js
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.549749 guis_sso_client-0.7.5/guis_sso_client/templates/
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552962 guis_sso_client-0.7.5/guis_sso_client/templates/applications/
+-rw-r--r--   0 mpilia     (501) staff       (20)      455 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/templates/applications/guis_applications.html
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.553080 guis_sso_client-0.7.5/guis_sso_client/templates/sso/
+-rw-r--r--   0 mpilia     (501) staff       (20)      432 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/templates/sso/guis_sso_smartcheck.html
+-rw-r--r--   0 mpilia     (501) staff       (20)       60 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/tests.py
+-rw-r--r--   0 mpilia     (501) staff       (20)      333 2023-04-18 09:58:08.000000 guis_sso_client-0.7.5/guis_sso_client/urls.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     3763 2023-04-18 09:45:19.000000 guis_sso_client-0.7.5/guis_sso_client/utils.py
+-rw-r--r--   0 mpilia     (501) staff       (20)     2900 2023-04-18 09:58:08.000000 guis_sso_client-0.7.5/guis_sso_client/views.py
+drwxr-xr-x   0 mpilia     (501) staff       (20)        0 2023-04-18 09:58:19.552285 guis_sso_client-0.7.5/guis_sso_client.egg-info/
+-rw-r--r--   0 mpilia     (501) staff       (20)       59 2023-04-18 09:58:19.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpilia     (501) staff       (20)      876 2023-04-18 09:58:19.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)        1 2023-04-18 09:58:19.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)        1 2023-04-18 09:54:12.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/not-zip-safe
+-rw-r--r--   0 mpilia     (501) staff       (20)       80 2023-04-18 09:58:19.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/requires.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)       16 2023-04-18 09:58:19.000000 guis_sso_client-0.7.5/guis_sso_client.egg-info/top_level.txt
+-rw-r--r--   0 mpilia     (501) staff       (20)       67 2023-04-18 09:58:19.553414 guis_sso_client-0.7.5/setup.cfg
+-rw-r--r--   0 mpilia     (501) staff       (20)      475 2023-04-18 09:58:08.000000 guis_sso_client-0.7.5/setup.py
```

### Comparing `guis_sso_client-0.6.0/guis_sso_client/admin.py` & `guis_sso_client-0.7.5/guis_sso_client/admin.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/apps.py` & `guis_sso_client-0.7.5/guis_sso_client/apps.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/backends.py` & `guis_sso_client-0.7.5/guis_sso_client/backends.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 import logging
 
+from django import VERSION
+
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.contrib.auth.models import Group
 
 from .utils import get_sso_login_data
 
 
 logger = logging.getLogger('guis_sso_client')
 
 
 class SSOAuthenticationBackend(ModelBackend):
 
+    if VERSION[0] < 2 and VERSION[1] < 11:
+        def authenticate(self, claim=None):
+            sso_session_key = claim['sso_session_key']
+            logger.debug('sso_session_key: %s', sso_session_key)
+            login_data = get_sso_login_data(sso_session_key)
+            if login_data:
+                return self.login_data_to_user(login_data)
+            return None
+    else:
+        def authenticate(self, request, claim=None):
+            sso_session_key = claim['sso_session_key']
+            logger.debug('sso_session_key: %s', sso_session_key)
+            login_data = get_sso_login_data(sso_session_key)
+            if login_data:
+                return self.login_data_to_user(login_data)
+            return None
+
     UserModel = get_user_model()
 
     def login_data_to_user(self, login_data):
         logger.debug('received login data: {}'.format(login_data))
         if login_data and 'user' in login_data:
             json_user = login_data['user']
             group_list = login_data['groups']
@@ -36,15 +55,7 @@
             user.groups.clear()
             for group in groups:
                 user.groups.add(group)
             logger.info('user successfully authenticated: {}'.format(
                 user.get_full_name()))
             return user
         return None
-
-    def authenticate(self, claim=None):
-        sso_session_key = claim['sso_session_key']
-        logger.debug('sso_session_key: %s', sso_session_key)
-        login_data = get_sso_login_data(sso_session_key)
-        if login_data:
-            return self.login_data_to_user(login_data)
-        return None
```

### Comparing `guis_sso_client-0.6.0/guis_sso_client/context_processors.py` & `guis_sso_client-0.7.5/guis_sso_client/context_processors.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/management/commands/pushgroups.py` & `guis_sso_client-0.7.5/guis_sso_client/management/commands/pushgroups.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/middleware.py` & `guis_sso_client-0.7.5/guis_sso_client/middleware.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/static/js/guis_sso_smartcheck.js` & `guis_sso_client-0.7.5/guis_sso_client/static/js/guis_sso_smartcheck.js`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/utils.py` & `guis_sso_client-0.7.5/guis_sso_client/utils.py`

 * *Files identical despite different names*

### Comparing `guis_sso_client-0.6.0/guis_sso_client/views.py` & `guis_sso_client-0.7.5/guis_sso_client/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
 import time
 import json
 
 from django.conf import settings
 from django.contrib.auth import authenticate, login, logout
 from django.contrib.auth.decorators import login_required
-from django.core.urlresolvers import reverse
+from django import VERSION
+if VERSION[0] < 2:
+    from django.core.urlresolvers import reverse
+else:
+    from django.urls import reverse
 from django.http import HttpResponse, HttpResponseRedirect
 
 from furl import furl
 from jose.jwt import decode, encode
 
 from .utils import get_applications
```

### Comparing `guis_sso_client-0.6.0/guis_sso_client.egg-info/SOURCES.txt` & `guis_sso_client-0.7.5/guis_sso_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

