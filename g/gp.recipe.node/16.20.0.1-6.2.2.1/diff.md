# Comparing `tmp/gp.recipe.node-16.20.0.1.tar.gz` & `tmp/gp.recipe.node-6.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp.recipe.node-16.20.0.1.tar", last modified: Tue Apr 18 10:04:26 2023, max compression
+gzip compressed data, was "dist/gp.recipe.node-6.2.2.1.tar", last modified: Tue Jun 28 18:30:54 2016, max compression
```

## Comparing `gp.recipe.node-16.20.0.1.tar` & `gp.recipe.node-6.2.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/
--rw-r--r--   0 sallner   (1000) users      (100)      459 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/.coveragerc
--rw-r--r--   0 sallner   (1000) users      (100)     2395 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/CHANGES.rst
--rw-r--r--   0 sallner   (1000) users      (100)       40 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/CONTRIBUTORS.txt
--rw-r--r--   0 sallner   (1000) users      (100)      142 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/MANIFEST.in
--rw-r--r--   0 sallner   (1000) users      (100)     5837 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/PKG-INFO
--rw-r--r--   0 sallner   (1000) users      (100)      514 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/README.rst
--rw-r--r--   0 sallner   (1000) users      (100)     6501 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/bootstrap.py
--rw-r--r--   0 sallner   (1000) users      (100)      348 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/buildout.cfg
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/gp/
--rw-r--r--   0 sallner   (1000) users      (100)      244 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/gp/__init__.py
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/gp/recipe/
--rw-r--r--   0 sallner   (1000) users      (100)      244 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/gp/recipe/__init__.py
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/gp/recipe/node/
--rw-r--r--   0 sallner   (1000) users      (100)     1976 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/gp/recipe/node/README.rst
--rw-r--r--   0 sallner   (1000) users      (100)    11154 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/gp/recipe/node/__init__.py
--rw-r--r--   0 sallner   (1000) users      (100)     1416 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/gp/recipe/node/script.py
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/
--rw-r--r--   0 sallner   (1000) users      (100)     5837 2023-04-18 10:04:25.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/PKG-INFO
--rw-r--r--   0 sallner   (1000) users      (100)      577 2023-04-18 10:04:26.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/SOURCES.txt
--rw-r--r--   0 sallner   (1000) users      (100)        1 2023-04-18 10:04:25.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/dependency_links.txt
--rw-r--r--   0 sallner   (1000) users      (100)       46 2023-04-18 10:04:25.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/entry_points.txt
--rw-r--r--   0 sallner   (1000) users      (100)       13 2023-04-18 10:04:26.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/namespace_packages.txt
--rw-r--r--   0 sallner   (1000) users      (100)        1 2023-04-18 10:04:25.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/not-zip-safe
--rw-r--r--   0 sallner   (1000) users      (100)       86 2023-04-18 10:04:26.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/requires.txt
--rw-r--r--   0 sallner   (1000) users      (100)        3 2023-04-18 10:04:26.000000 gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/top_level.txt
--rw-r--r--   0 sallner   (1000) users      (100)       81 2023-04-18 10:04:26.318403 gp.recipe.node-16.20.0.1/setup.cfg
--rw-r--r--   0 sallner   (1000) users      (100)     2365 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/setup.py
--rw-r--r--   0 sallner   (1000) users      (100)     6218 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/tests.py
--rw-r--r--   0 sallner   (1000) users      (100)      403 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/tox.ini
--rwxr-xr-x   0 sallner   (1000) users      (100)      645 2023-04-18 10:04:24.000000 gp.recipe.node-16.20.0.1/update_node_version.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      459 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/.coveragerc
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6673 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/PKG-INFO
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      142 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/MANIFEST.in
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2002 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/CHANGES.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6501 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/bootstrap.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      102 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/setup.cfg
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2102 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/setup.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6299 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/tests.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      420 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/README.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      269 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/tox.ini
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/dependency_links.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6673 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/PKG-INFO
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      577 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/SOURCES.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      101 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/requires.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/not-zip-safe
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       47 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/entry_points.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       13 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/namespace_packages.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        3 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/top_level.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      348 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/buildout.cfg
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      244 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/__init__.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      244 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/__init__.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/node/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1825 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/node/README.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    10983 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/node/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1416 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/gp/recipe/node/script.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       40 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/CONTRIBUTORS.txt
+-rwxr-xr-x   0 gawel     (1000) gawel     (1000)      623 2016-06-28 18:30:54.000000 gp.recipe.node-6.2.2.1/update_node_version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gp.recipe.node-16.20.0.1/CHANGES.rst` & `gp.recipe.node-6.2.2.1/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-16.20.0.1 (2023-04-18)
-======================
-
-- update to 16.20.0
-
-- Stop testing for Python 3.6.
-
-- Claim support for Python 3.11.
-
-
-16.13.2.1 (2022-02-09)
-======================
-
-- update to 16.13.2
-
-- claim support for Python 3.6, 3.7, 3.8, 3.9, 3.10
-
-- Load 'arm64' version of node.js on M1/arm apple machines and others.
-
-
-13.3.0.1 (2019-12-12)
-=====================
-
-- update to 13.x
-
-
 6.2.2.1 (2016-06-28)
 ====================
 
 - Add support for offline mode in Buildout (`-o`)
 
 - Quote $PATH variable in order to fix problem when $PATH contains space
   characters.
```

### Comparing `gp.recipe.node-16.20.0.1/bootstrap.py` & `gp.recipe.node-6.2.2.1/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gp.recipe.node-16.20.0.1/gp/recipe/node/README.rst` & `gp.recipe.node-6.2.2.1/gp/recipe/node/README.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     node.js version. Ignored if url is set, or if binary-url is set that
     doesn't use the ``{v}`` placeholder. Default to recipe version.  Mean
     that using ``recipe=gp.recipe.node==0.10.22.X`` will install ``node
     0.10.22``
 
 npms
     a list of package to install with npm. You can specify a package version by
-    using ``npmname@version``. In case you want to specify a ``package.json``
-    generated after a successfull first installation or update, you can 
-    add ``.`` to the list.
+    using ``npmname@version``
 
 scripts
     a list of scripts (optional)
 
 node-path
     a list of extra directory to add to ``NODE_PATH``
 
@@ -52,15 +50,15 @@
     >>> write('buildout.cfg',
     ... """
     ... [buildout]
     ... parts = test1
     ...
     ... [test1]
     ... recipe = gp.recipe.node
-    ... npms = coffee-script less . 
+    ... npms = coffee-script less
     ... scripts = coffee lessc
     ... """)
 
 Running the buildout gives us::
 
     >>> print 'start', system(buildout)
     start...
```

### Comparing `gp.recipe.node-16.20.0.1/gp/recipe/node/__init__.py` & `gp.recipe.node-6.2.2.1/gp/recipe/node/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 """Recipe node"""
-import glob
-import json
-import logging
-import os
-import shutil
 import subprocess
+import logging
+import glob
 import sys
+import os
+import json
 from pipes import quote as shell_quote
 
 
 class Recipe(object):
     """zc.buildout recipe"""
 
     binary_format = 'https://nodejs.org/dist/v{v}/node-v{v}-{p}-{a}.tar.gz'
@@ -65,36 +64,30 @@
             os.makedirs(node_dir)
 
         node_binary = self.get_binary(options)
 
         if node_binary is None:
             args = {}
             if 'url' not in options:
-                uname = os.uname()
-                if 'x86_64' in uname:
-                    a = 'x64'
-                elif 'arm64' in uname:
-                    a = 'arm64'
-                else:
-                    a = 'x86'
                 args = dict(
                     v=self.get_version(options),
-                    a=a,
+                    a='x86_64' in os.uname() and 'x64' or 'x86',
                 )
                 if sys.platform.startswith('linux'):
                     args['p'] = 'linux'
                 elif sys.platform == 'darwin':
                     args['p'] = 'darwin'
 
             if 'p' in args:
                 binary_url = options.get('binary-url', self.binary_format)
                 options['url'] = url = binary_url.format(**args)
                 logger.info('Using binary distribution at %s', url)
 
                 from zc.buildout.download import Download
+                from archive import extract
 
                 # Use the buildout download infrastructure
                 manager = Download(options=self.buildout['buildout'],
                                    offline=self.buildout['buildout'].get('offline') == 'true')
 
                 # The buildout download utility expects us to know whether or
                 # not we have a download cache, which causes fun errors.  This
@@ -106,15 +99,15 @@
 
                 destination = self.get_node_directory(options)
 
                 # Finally, extract the archive.  The binary distribution urls
                 # are defined in this file, so we can safely assume they're
                 # gzipped tarballs.  This prevents an error when downloaded
                 # into a temporary file.
-                shutil.unpack_archive(filename, destination, format="gztar")
+                extract(filename, destination, ext=".tar.gz")
 
             else:
                 if 'url' not in options:
                     options['url'] = url = self.source_format.format(**args)
                 logger.info('Using source distribution at %s', options['url'])
                 import zc.recipe.cmmi
                 options['environment'] = (
```

### Comparing `gp.recipe.node-16.20.0.1/gp/recipe/node/script.py` & `gp.recipe.node-6.2.2.1/gp/recipe/node/script.py`

 * *Files identical despite different names*

### Comparing `gp.recipe.node-16.20.0.1/gp.recipe.node.egg-info/SOURCES.txt` & `gp.recipe.node-6.2.2.1/gp.recipe.node.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .coveragerc
-CHANGES.rst
+CHANGES.txt
 CONTRIBUTORS.txt
 MANIFEST.in
-README.rst
+README.txt
 bootstrap.py
 buildout.cfg
 setup.cfg
 setup.py
 tests.py
 tox.ini
 update_node_version.py
@@ -16,10 +16,10 @@
 gp.recipe.node.egg-info/dependency_links.txt
 gp.recipe.node.egg-info/entry_points.txt
 gp.recipe.node.egg-info/namespace_packages.txt
 gp.recipe.node.egg-info/not-zip-safe
 gp.recipe.node.egg-info/requires.txt
 gp.recipe.node.egg-info/top_level.txt
 gp/recipe/__init__.py
-gp/recipe/node/README.rst
+gp/recipe/node/README.txt
 gp/recipe/node/__init__.py
 gp/recipe/node/script.py
```

### Comparing `gp.recipe.node-16.20.0.1/setup.py` & `gp.recipe.node-6.2.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 
 def read(*rnames):
     try:
         return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
     except:
         return ''
 
-version = '16.20.0.1'
+version = '6.2.2.1'
 
 long_description = (
-    read('README.rst')
+    read('README.txt')
     + '\n' +
     'Detailed Documentation\n'
     '**********************\n'
     + '\n' +
-    read('gp', 'recipe', 'node', 'README.rst')
+    read('gp', 'recipe', 'node', 'README.txt')
     + '\n' +
     'Contributors\n'
     '************\n'
     + '\n' +
     read('CONTRIBUTORS.txt')
     + '\n' +
     'Change history\n'
     '**************\n'
     + '\n' +
-    read('CHANGES.rst')
+    read('CHANGES.txt')
     + '\n' +
     'Download\n'
     '********\n')
 
 entry_point = 'gp.recipe.node:Recipe'
 entry_points = {"zc.buildout": ["default = %s" % entry_point]}
 
@@ -47,33 +47,28 @@
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
       classifiers=[
           'Framework :: Buildout',
           'Intended Audience :: Developers',
           'Topic :: Software Development :: Build Tools',
           'License :: OSI Approved :: Zope Public License',
-          'Development Status :: 6 - Mature',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Programming Language :: Python :: 3.11',
       ],
       keywords='buildout node.js node',
       author='Gael Pasgrimaud',
       author_email='gael@gawel.org',
       url='https://github.com/gawel/gp.recipe.node',
       license='ZPL',
       packages=find_packages(exclude=['ez_setup', 'update_node_version']),
       namespace_packages=['gp', 'gp.recipe'],
       include_package_data=True,
       zip_safe=False,
       install_requires=['setuptools',
                         'zc.buildout',
                         'zc.recipe.egg',
                         'zc.recipe.cmmi',
+                        'python-archive',
                         ],
       tests_require=tests_require,
       extras_require=dict(tests=tests_require),
       test_suite='gp.recipe.node.tests.test_docs.test_suite',
       entry_points=entry_points,
       )
```

### Comparing `gp.recipe.node-16.20.0.1/tests.py` & `gp.recipe.node-6.2.2.1/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import shutil
 import tempfile
 import subprocess
 import zc.buildout.configparser
 from unittest import TestCase
 from unittest import skipIf
 from gp.recipe.node import Recipe
-from io import StringIO
+try:
+    # python 2
+    from StringIO import StringIO
+except:
+    # python 3
+    from io import StringIO
 
 TRAVIS = os.path.isdir('/home/travis')
 PY3 = bool(sys.version_info[0] == 3)
 
 BUILDOUT = """
 [buildout]
 develop = %s
```

### Comparing `gp.recipe.node-16.20.0.1/update_node_version.py` & `gp.recipe.node-6.2.2.1/update_node_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-from urllib.request import urlopen
+import urllib
 import re
 
 
 def main():
-    page = urlopen('https://nodejs.org/en/download/releases/').read().decode()
-    version = re.search(r'v([0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2})',
+    page = urllib.urlopen('https://nodejs.org/en/download/releases/').read()
+    version = re.search('v([0-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2})',
                         page).groups()[0]
 
     updated = ''
     with open('setup.py') as fd:
         for line in fd:
             if line.startswith('version ='):
                 if version not in line:
-                    line = f"version = '{version}.1.dev0'\n"
+                    line = "version = '%s.1.dev0'\n" % version
             updated += line
 
     with open('setup.py', 'w') as fd:
         fd.write(updated)
 
 if __name__ == '__main__':
     main()
```

