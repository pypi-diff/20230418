# Comparing `tmp/forked-authomatic-1.2.2.dev0.tar.gz` & `tmp/forked-authomatic-1.2.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forked-authomatic-1.2.2.dev0.tar", last modified: Mon Apr 17 14:39:03 2023, max compression
+gzip compressed data, was "forked-authomatic-1.2.3.dev0.tar", last modified: Tue Apr 18 02:24:33 2023, max compression
```

## Comparing `forked-authomatic-1.2.2.dev0.tar` & `forked-authomatic-1.2.3.dev0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.164437 forked-authomatic-1.2.2.dev0/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     7859 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/CHANGES.rst
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      175 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1099 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/LICENSE.txt
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      492 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/MANIFEST.in
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     4653 2023-04-17 14:39:03.164671 forked-authomatic-1.2.2.dev0/PKG-INFO
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     3173 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/README.rst
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1830 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/RELEASE.rst
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.150920 forked-authomatic-1.2.2.dev0/authomatic/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      227 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/__init__.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     6561 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/adapters.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    53269 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/core.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1224 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/exceptions.py
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.153260 forked-authomatic-1.2.2.dev0/authomatic/extras/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/extras/__init__.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1421 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/extras/flask.py
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.154291 forked-authomatic-1.2.2.dev0/authomatic/extras/gae/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     7151 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/extras/gae/__init__.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     5233 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/extras/gae/openid.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1356 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/extras/interfaces.py
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.159259 forked-authomatic-1.2.2.dev0/authomatic/providers/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    30309 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/__init__.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     3445 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/gaeopenid.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    38857 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/oauth1.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    59333 2023-04-17 14:12:29.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/oauth2.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    17262 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/openid.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      124 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/providers/persona.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    29751 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/authomatic/six.py
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1101 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/config-template.py
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.161920 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     4653 2023-04-17 14:39:03.000000 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/PKG-INFO
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      823 2023-04-17 14:39:03.000000 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/SOURCES.txt
--rw-r--r--   0 duzhiqiang   (501) staff       (20)        1 2023-04-17 14:39:03.000000 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/dependency_links.txt
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      102 2023-04-17 14:39:03.000000 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/requires.txt
--rw-r--r--   0 duzhiqiang   (501) staff       (20)       17 2023-04-17 14:39:03.000000 forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/top_level.txt
-drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:39:03.163887 forked-authomatic-1.2.2.dev0/javascript/
--rw-r--r--   0 duzhiqiang   (501) staff       (20)    16582 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/javascript/authomatic.js
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     7950 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/javascript/authomatic.map
--rw-r--r--   0 duzhiqiang   (501) staff       (20)     1502 2023-04-17 14:39:03.165782 forked-authomatic-1.2.2.dev0/setup.cfg
--rw-r--r--   0 duzhiqiang   (501) staff       (20)      334 2023-04-17 14:03:13.000000 forked-authomatic-1.2.2.dev0/setup.py
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.459320 forked-authomatic-1.2.3.dev0/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     7859 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/CHANGES.rst
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      175 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1099 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/LICENSE.txt
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      492 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/MANIFEST.in
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     4653 2023-04-18 02:24:33.459573 forked-authomatic-1.2.3.dev0/PKG-INFO
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     3173 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/README.rst
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1830 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/RELEASE.rst
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.442623 forked-authomatic-1.2.3.dev0/authomatic/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      227 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/__init__.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     6561 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/adapters.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    53269 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/core.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1224 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/exceptions.py
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.444874 forked-authomatic-1.2.3.dev0/authomatic/extras/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)        0 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/extras/__init__.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1421 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/extras/flask.py
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.445888 forked-authomatic-1.2.3.dev0/authomatic/extras/gae/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     7151 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/extras/gae/__init__.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     5233 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/extras/gae/openid.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1356 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/extras/interfaces.py
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.452326 forked-authomatic-1.2.3.dev0/authomatic/providers/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    30309 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/__init__.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     3445 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/gaeopenid.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    38857 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/oauth1.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    59410 2023-04-18 02:24:01.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/oauth2.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    17262 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/openid.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      124 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/providers/persona.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    29751 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/authomatic/six.py
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1101 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/config-template.py
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.456280 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     4653 2023-04-18 02:24:33.000000 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/PKG-INFO
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      823 2023-04-18 02:24:33.000000 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)        1 2023-04-18 02:24:33.000000 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      102 2023-04-18 02:24:33.000000 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/requires.txt
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)       17 2023-04-18 02:24:33.000000 forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/top_level.txt
+drwxr-xr-x   0 duzhiqiang   (501) staff       (20)        0 2023-04-18 02:24:33.458422 forked-authomatic-1.2.3.dev0/javascript/
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)    16582 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/javascript/authomatic.js
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     7950 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/javascript/authomatic.map
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)     1502 2023-04-18 02:24:33.460970 forked-authomatic-1.2.3.dev0/setup.cfg
+-rw-r--r--   0 duzhiqiang   (501) staff       (20)      334 2023-04-17 14:03:13.000000 forked-authomatic-1.2.3.dev0/setup.py
```

### Comparing `forked-authomatic-1.2.2.dev0/CHANGES.rst` & `forked-authomatic-1.2.3.dev0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/LICENSE.txt` & `forked-authomatic-1.2.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/PKG-INFO` & `forked-authomatic-1.2.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forked-authomatic
-Version: 1.2.2.dev0
+Version: 1.2.3.dev0
 Summary: Authorization / authentication client library for Python web applications
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
```

### Comparing `forked-authomatic-1.2.2.dev0/README.rst` & `forked-authomatic-1.2.3.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/RELEASE.rst` & `forked-authomatic-1.2.3.dev0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/adapters.py` & `forked-authomatic-1.2.3.dev0/authomatic/adapters.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/core.py` & `forked-authomatic-1.2.3.dev0/authomatic/core.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/exceptions.py` & `forked-authomatic-1.2.3.dev0/authomatic/exceptions.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/extras/flask.py` & `forked-authomatic-1.2.3.dev0/authomatic/extras/flask.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/extras/gae/__init__.py` & `forked-authomatic-1.2.3.dev0/authomatic/extras/gae/__init__.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/extras/gae/openid.py` & `forked-authomatic-1.2.3.dev0/authomatic/extras/gae/openid.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/extras/interfaces.py` & `forked-authomatic-1.2.3.dev0/authomatic/extras/interfaces.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/providers/__init__.py` & `forked-authomatic-1.2.3.dev0/authomatic/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/providers/gaeopenid.py` & `forked-authomatic-1.2.3.dev0/authomatic/providers/gaeopenid.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/providers/oauth1.py` & `forked-authomatic-1.2.3.dev0/authomatic/providers/oauth1.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/providers/oauth2.py` & `forked-authomatic-1.2.3.dev0/authomatic/providers/oauth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,41 +413,41 @@
             self.access_token_response = response
 
             access_token = response.data.get('access_token', '')
             refresh_token = response.data.get('refresh_token', '')
 
             # OAuth 2.0 credentials need access_token, refresh_token,
             # token_type and expire_in.
-            self.credentials.token = access_token
-            self.credentials.refresh_token = refresh_token
+            self.credentials.token = response.data.get('access_token', '')
+            self.credentials.refresh_token = response.data.get('refresh_token', '')
             self.credentials.expire_in = response.data.get('expires_in')
             self.credentials.token_type = response.data.get('token_type', '')
             # sWe don't need these two guys anymore.
             self.credentials.consumer_key = ''
             self.credentials.consumer_secret = ''
 
             # update credentials
             self.credentials = self._x_credentials_parser(
                 self.credentials, response.data)
 
-            if response.status != 200 or not access_token:
+            if response.status != 200 or not self.credentials.token:
                 raise FailureError(
                     'Failed to obtain OAuth 2.0 access token from {0}! '
                     'HTTP status: {1}, message: {2}.'.format(
                         self.access_token_url,
                         response.status,
                         response.content
                     ),
                     original_message=response.content,
                     status=response.status,
                     url=self.access_token_url)
 
             self._log(logging.INFO, u'Got access token.')
 
-            if refresh_token:
+            if self.credentials.refresh_token:
                 self._log(logging.INFO, u'Got refresh access token.')
 
             # create user
             self._update_or_create_user(response.data, self.credentials)
 
             # =================================================================
             # We're done!
```

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/providers/openid.py` & `forked-authomatic-1.2.3.dev0/authomatic/providers/openid.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/authomatic/six.py` & `forked-authomatic-1.2.3.dev0/authomatic/six.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/config-template.py` & `forked-authomatic-1.2.3.dev0/config-template.py`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/PKG-INFO` & `forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forked-authomatic
-Version: 1.2.2.dev0
+Version: 1.2.3.dev0
 Summary: Authorization / authentication client library for Python web applications
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
```

### Comparing `forked-authomatic-1.2.2.dev0/forked_authomatic.egg-info/SOURCES.txt` & `forked-authomatic-1.2.3.dev0/forked_authomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/javascript/authomatic.js` & `forked-authomatic-1.2.3.dev0/javascript/authomatic.js`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/javascript/authomatic.map` & `forked-authomatic-1.2.3.dev0/javascript/authomatic.map`

 * *Files identical despite different names*

### Comparing `forked-authomatic-1.2.2.dev0/setup.cfg` & `forked-authomatic-1.2.3.dev0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.2.dev
+version = 1.2.3.dev
 name = forked-authomatic
 description = Authorization / authentication client library for Python web applications
 long_description = file: README.rst
 author = Peter Hudec
 author_email = peterhudec@peterhudec.com
 maintainer = Authomatic Project Community
 maintainer_email = authomaticproject@protonmail.com
```

