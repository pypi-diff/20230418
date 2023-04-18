# Comparing `tmp/MailToolsBox-0.1.0.1.tar.gz` & `tmp/MailToolsBox-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailToolsBox-0.1.0.1.tar", last modified: Mon Apr 17 11:40:50 2023, max compression
+gzip compressed data, was "MailToolsBox-0.1.0.2.tar", last modified: Tue Apr 18 07:15:12 2023, max compression
```

## Comparing `MailToolsBox-0.1.0.1.tar` & `MailToolsBox-0.1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.966057 MailToolsBox-0.1.0.1/
--rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.954059 MailToolsBox-0.1.0.1/MailToolsBox/
--rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.1/MailToolsBox/__init__.py
--rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.1/MailToolsBox/imapClient.py
--rw-rw-rw-   0        0        0     3853 2023-04-17 09:46:24.000000 MailToolsBox-0.1.0.1/MailToolsBox/mailSender.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.964056 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3489 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3489 2023-04-17 11:40:50.966057 MailToolsBox-0.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-04-17 11:23:42.000000 MailToolsBox-0.1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 11:40:50.967055 MailToolsBox-0.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-04-17 11:32:27.000000 MailToolsBox-0.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.112032 MailToolsBox-0.1.0.2/MailToolsBox/
+-rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.2/MailToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.2/MailToolsBox/imapClient.py
+-rw-rw-rw-   0        0        0     3853 2023-04-17 09:46:24.000000 MailToolsBox-0.1.0.2/MailToolsBox/mailSender.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.138023 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3496 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-18 07:15:12.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3496 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-04-17 11:23:42.000000 MailToolsBox-0.1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-04-18 07:08:46.000000 MailToolsBox-0.1.0.2/setup.py
```

### Comparing `MailToolsBox-0.1.0.1/LICENSE.txt` & `MailToolsBox-0.1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.1/MailToolsBox/imapClient.py` & `MailToolsBox-0.1.0.2/MailToolsBox/imapClient.py`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.1/MailToolsBox/mailSender.py` & `MailToolsBox-0.1.0.2/MailToolsBox/mailSender.py`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.1/MailToolsBox.egg-info/PKG-INFO` & `MailToolsBox-0.1.0.2/MailToolsBox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: MailToolsBox
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Mail tools simplify mail server and sender development for developers.
-Home-page: https://www.ramai.io
+Home-page: https://www.rambod.net
 Download-URL: https://github.com/rambod/MailToolsBox/archive/0.0.4.6.tar.gz
 Author: Rambod Ghashghai
-Author-email: rambod@ramai.io
+Author-email: gh.rambod@gmail.com
 License: MIT
 Keywords: Mail,Server,smtp,send,email,tools,box
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MailToolsBox
 
 MailToolsBox is a Python package that provides two classes to help you
 interact with emails.
```

### Comparing `MailToolsBox-0.1.0.1/PKG-INFO` & `MailToolsBox-0.1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: MailToolsBox
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Mail tools simplify mail server and sender development for developers.
-Home-page: https://www.ramai.io
+Home-page: https://www.rambod.net
 Download-URL: https://github.com/rambod/MailToolsBox/archive/0.0.4.6.tar.gz
 Author: Rambod Ghashghai
-Author-email: rambod@ramai.io
+Author-email: gh.rambod@gmail.com
 License: MIT
 Keywords: Mail,Server,smtp,send,email,tools,box
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MailToolsBox
 
 MailToolsBox is a Python package that provides two classes to help you
 interact with emails.
```

### Comparing `MailToolsBox-0.1.0.1/README.md` & `MailToolsBox-0.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.1/setup.py` & `MailToolsBox-0.1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from distutils.core import setup
 
 
 setup(
     name='MailToolsBox',
     packages=['MailToolsBox'],
-    version='0.1.0.1',
+    version='0.1.0.2',
     license='MIT',
     # Give a short description about your library
     description='Mail tools simplify mail server and sender development for developers.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Rambod Ghashghai',                   # Type in your name
-    author_email='rambod@ramai.io',      # Type in your E-Mail
+    author_email='gh.rambod@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
-    url='https://www.ramai.io',
+    url='https://www.rambod.net',
     # I explain this later on
     download_url='https://github.com/rambod/MailToolsBox/archive/0.0.4.6.tar.gz',
     keywords=['Mail', 'Server', 'smtp',  'send', 'email', 'tools',
               'box'],   # Keywords that define your package best
     install_requires=[
         "Jinja2==3.0.2",
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 4 - Beta',
         # Define that your audience are developers
         'Intended Audience :: Developers',
         'Topic :: Communications :: Email',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

