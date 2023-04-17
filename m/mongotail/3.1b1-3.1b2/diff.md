# Comparing `tmp/mongotail-3.1b1.tar.gz` & `tmp/mongotail-3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongotail-3.1b1.tar", last modified: Mon Mar 28 19:49:51 2022, max compression
+gzip compressed data, was "mongotail-3.1b2.tar", last modified: Tue Mar 29 20:41:30 2022, max compression
```

## Comparing `mongotail-3.1b1.tar` & `mongotail-3.1b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-28 19:49:51.865187 mongotail-3.1b1/
--rw-rw-r--   0 user      (1000) user      (1000)      905 2022-02-11 13:47:19.000000 mongotail-3.1b1/AUTHORS.rst
--rw-rw-r--   0 user      (1000) user      (1000)     4376 2022-03-25 12:42:11.000000 mongotail-3.1b1/CHANGELOG.rst
--rw-rw----   0 user      (1000) user      (1000)    35147 2017-11-27 00:38:25.000000 mongotail-3.1b1/COPYING
--rw-rw-r--   0 user      (1000) user      (1000)      943 2022-02-11 13:47:19.000000 mongotail-3.1b1/INSTALL.rst
--rw-rw----   0 user      (1000) user      (1000)       97 2017-11-27 00:38:25.000000 mongotail-3.1b1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    11648 2022-03-28 19:49:51.865187 mongotail-3.1b1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10457 2022-03-28 19:49:23.000000 mongotail-3.1b1/README.rst
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-28 19:49:51.861186 mongotail-3.1b1/mongotail/
--rw-rw-r--   0 user      (1000) user      (1000)     1692 2022-03-24 21:32:53.000000 mongotail-3.1b1/mongotail/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3456 2022-03-27 00:45:15.000000 mongotail-3.1b1/mongotail/conn.py
--rw-rw----   0 user      (1000) user      (1000)     1889 2022-03-26 23:41:04.000000 mongotail-3.1b1/mongotail/err.py
--rw-rw-r--   0 user      (1000) user      (1000)     4029 2022-02-11 13:47:19.000000 mongotail-3.1b1/mongotail/jsondec.py
--rw-rw-r--   0 user      (1000) user      (1000)    12237 2022-03-27 00:53:51.000000 mongotail-3.1b1/mongotail/mongotail.py
--rw-rw-r--   0 user      (1000) user      (1000)    10851 2022-02-11 13:47:19.000000 mongotail-3.1b1/mongotail/out.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-28 19:49:51.865187 mongotail-3.1b1/mongotail.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    11648 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      437 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       55 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-03-28 19:38:33.000000 mongotail-3.1b1/mongotail.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       45 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2022-03-28 19:49:51.000000 mongotail-3.1b1/mongotail.egg-info/top_level.txt
--rw-rw----   0 user      (1000) user      (1000)       80 2022-03-28 19:49:51.865187 mongotail-3.1b1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2777 2022-03-27 01:15:56.000000 mongotail-3.1b1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-29 20:41:30.209119 mongotail-3.1b2/
+-rw-rw-r--   0 user      (1000) user      (1000)      905 2022-02-11 13:47:19.000000 mongotail-3.1b2/AUTHORS.rst
+-rw-rw-r--   0 user      (1000) user      (1000)     4376 2022-03-25 12:42:11.000000 mongotail-3.1b2/CHANGELOG.rst
+-rw-rw----   0 user      (1000) user      (1000)    35147 2017-11-27 00:38:25.000000 mongotail-3.1b2/COPYING
+-rw-rw-r--   0 user      (1000) user      (1000)      943 2022-02-11 13:47:19.000000 mongotail-3.1b2/INSTALL.rst
+-rw-rw----   0 user      (1000) user      (1000)       97 2017-11-27 00:38:25.000000 mongotail-3.1b2/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    12307 2022-03-29 20:41:30.209119 mongotail-3.1b2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    11116 2022-03-29 19:50:45.000000 mongotail-3.1b2/README.rst
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-29 20:41:30.209119 mongotail-3.1b2/mongotail/
+-rw-rw-r--   0 user      (1000) user      (1000)     1692 2022-03-29 20:02:02.000000 mongotail-3.1b2/mongotail/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3481 2022-03-29 12:06:52.000000 mongotail-3.1b2/mongotail/conn.py
+-rw-rw----   0 user      (1000) user      (1000)     1889 2022-03-26 23:41:04.000000 mongotail-3.1b2/mongotail/err.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4029 2022-02-11 13:47:19.000000 mongotail-3.1b2/mongotail/jsondec.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12237 2022-03-29 12:17:58.000000 mongotail-3.1b2/mongotail/mongotail.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10851 2022-02-11 13:47:19.000000 mongotail-3.1b2/mongotail/out.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-03-29 20:41:30.209119 mongotail-3.1b2/mongotail.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    12307 2022-03-29 20:41:29.000000 mongotail-3.1b2/mongotail.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      437 2022-03-29 20:41:30.000000 mongotail-3.1b2/mongotail.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-03-29 20:41:29.000000 mongotail-3.1b2/mongotail.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       55 2022-03-29 20:41:30.000000 mongotail-3.1b2/mongotail.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-03-29 20:11:47.000000 mongotail-3.1b2/mongotail.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2022-03-29 20:41:30.000000 mongotail-3.1b2/mongotail.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2022-03-29 20:41:30.000000 mongotail-3.1b2/mongotail.egg-info/top_level.txt
+-rw-rw----   0 user      (1000) user      (1000)       80 2022-03-29 20:41:30.209119 mongotail-3.1b2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2777 2022-03-29 19:50:45.000000 mongotail-3.1b2/setup.py
```

### Comparing `mongotail-3.1b1/AUTHORS.rst` & `mongotail-3.1b2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/CHANGELOG.rst` & `mongotail-3.1b2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/COPYING` & `mongotail-3.1b2/COPYING`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/INSTALL.rst` & `mongotail-3.1b2/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/PKG-INFO` & `mongotail-3.1b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongotail
-Version: 3.1b1
+Version: 3.1b2
 Summary: Mongotail, Log all MongoDB queries in a "tail"able way.
 Home-page: https://github.com/mrsarm/mongotail
-Download-URL: https://github.com/mrsarm/mongotail/tarball/3.1b1
+Download-URL: https://github.com/mrsarm/mongotail/tarball/3.1b2
 Author: Mariano Ruiz
 Author-email: mrsarm@gmail.com
 License: GPL-3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -155,21 +155,41 @@
     2015-02-24 19:17:01.195 QUERY  [User] : {"_id": ObjectId("549048806b5d3db78cf6f654")}. 1 returned.
     2015-02-24 19:17:01.196 UPDATE [Activation] : {"_id": "AB524"}, {"_id": "AB524", "code": "f2cbad0c"}. 1 updated.
     2015-02-24 19:17:10.729 COUNT  [User] : {"active": {"$exists": true}, "firstName": {"$regex": "mac"}}
     ...
 
 To Connect with SSL or a remote Mongo instance, check the options with ``mongotail --help``.
 
+Profiling considerations
+^^^^^^^^^^^^^^^^^^^^^^^^
+
 **NOTE**: The level chosen can affect performance. It also can allow the
 server to write the content of queries to the log, which might have
 information security implications for your deployment. Remember to setup your
 database profiling level to ``0`` again after debugging your data::
 
     $ mongotail MYDATABASE -l 0
 
+
+Find slow queries
+^^^^^^^^^^^^^^^^^
+
+When you activate the profiler, you can choose to so with level 1 profiling
+instead of level 2. Level 1 configure the profiler system to log only "slow" operations.
+Then you have to set the threshold in milliseconds for the profile to consider an
+operation "slow". In the following example the threshold is set to 10 milliseconds::
+
+    $ mongotail sales -l 1
+    Profiling set to level 1
+    $ mongotail sales -s 10
+    Threshold profiling set to 10 milliseconds
+
+Then when you check your databases only operations that take 10 or more milliseconds
+will be displayed.
+
 A *step-by-step* guide of how to use Mongotail and the latest features
 is `here <http://mrsarm.blogspot.com.ar/2016/08/mongotail-2-0-with-new-features-mongodb-3-2-support.html>`_.
 
 
 Installation
 ------------
```

### Comparing `mongotail-3.1b1/README.rst` & `mongotail-3.1b2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -124,21 +124,41 @@
     2015-02-24 19:17:01.195 QUERY  [User] : {"_id": ObjectId("549048806b5d3db78cf6f654")}. 1 returned.
     2015-02-24 19:17:01.196 UPDATE [Activation] : {"_id": "AB524"}, {"_id": "AB524", "code": "f2cbad0c"}. 1 updated.
     2015-02-24 19:17:10.729 COUNT  [User] : {"active": {"$exists": true}, "firstName": {"$regex": "mac"}}
     ...
 
 To Connect with SSL or a remote Mongo instance, check the options with ``mongotail --help``.
 
+Profiling considerations
+^^^^^^^^^^^^^^^^^^^^^^^^
+
 **NOTE**: The level chosen can affect performance. It also can allow the
 server to write the content of queries to the log, which might have
 information security implications for your deployment. Remember to setup your
 database profiling level to ``0`` again after debugging your data::
 
     $ mongotail MYDATABASE -l 0
 
+
+Find slow queries
+^^^^^^^^^^^^^^^^^
+
+When you activate the profiler, you can choose to so with level 1 profiling
+instead of level 2. Level 1 configure the profiler system to log only "slow" operations.
+Then you have to set the threshold in milliseconds for the profile to consider an
+operation "slow". In the following example the threshold is set to 10 milliseconds::
+
+    $ mongotail sales -l 1
+    Profiling set to level 1
+    $ mongotail sales -s 10
+    Threshold profiling set to 10 milliseconds
+
+Then when you check your databases only operations that take 10 or more milliseconds
+will be displayed.
+
 A *step-by-step* guide of how to use Mongotail and the latest features
 is `here <http://mrsarm.blogspot.com.ar/2016/08/mongotail-2-0-with-new-features-mongodb-3-2-support.html>`_.
 
 
 Installation
 ------------
```

### Comparing `mongotail-3.1b1/mongotail/__init__.py` & `mongotail-3.1b2/mongotail/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ##############################################################################
 
 
 __author__ = 'Mariano Ruiz'
-__version__ = '3.1b1'
+__version__ = '3.1b2'
 __license__ = 'GPL-3'
 __url__ = 'https://github.com/mrsarm/mongotail'
 __doc__ = """Mongotail, Log all MongoDB queries in a "tail"able way."""
 __usage__ = """%(prog)s [db address] [options]
 
 db address can be:
   foo                   foo database on local machine (IPv4 connection)
```

### Comparing `mongotail-3.1b1/mongotail/conn.py` & `mongotail-3.1b2/mongotail/conn.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             options["authSource"] = args.auth_database
         user = args.username or username
         if user:
             options["username"] = user
             passw = args.password or password
             if passw is None:
                 passw = getpass.getpass()
-            options["password"] = passw
+            options["password"] = passw if passw != '' else None
 
         if scheme:
             client = MongoClient(address, **options)
         else:
             client = MongoClient(host=host, port=port, **options)
     except Exception as e:
         error("Error trying to connect: %s" % str(e), ECONNREFUSED)
```

### Comparing `mongotail-3.1b1/mongotail/err.py` & `mongotail-3.1b2/mongotail/err.py`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/mongotail/jsondec.py` & `mongotail-3.1b2/mongotail/jsondec.py`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/mongotail/mongotail.py` & `mongotail-3.1b2/mongotail/mongotail.py`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/mongotail/out.py` & `mongotail-3.1b2/mongotail/out.py`

 * *Files identical despite different names*

### Comparing `mongotail-3.1b1/mongotail.egg-info/PKG-INFO` & `mongotail-3.1b2/mongotail.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongotail
-Version: 3.1b1
+Version: 3.1b2
 Summary: Mongotail, Log all MongoDB queries in a "tail"able way.
 Home-page: https://github.com/mrsarm/mongotail
-Download-URL: https://github.com/mrsarm/mongotail/tarball/3.1b1
+Download-URL: https://github.com/mrsarm/mongotail/tarball/3.1b2
 Author: Mariano Ruiz
 Author-email: mrsarm@gmail.com
 License: GPL-3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -155,21 +155,41 @@
     2015-02-24 19:17:01.195 QUERY  [User] : {"_id": ObjectId("549048806b5d3db78cf6f654")}. 1 returned.
     2015-02-24 19:17:01.196 UPDATE [Activation] : {"_id": "AB524"}, {"_id": "AB524", "code": "f2cbad0c"}. 1 updated.
     2015-02-24 19:17:10.729 COUNT  [User] : {"active": {"$exists": true}, "firstName": {"$regex": "mac"}}
     ...
 
 To Connect with SSL or a remote Mongo instance, check the options with ``mongotail --help``.
 
+Profiling considerations
+^^^^^^^^^^^^^^^^^^^^^^^^
+
 **NOTE**: The level chosen can affect performance. It also can allow the
 server to write the content of queries to the log, which might have
 information security implications for your deployment. Remember to setup your
 database profiling level to ``0`` again after debugging your data::
 
     $ mongotail MYDATABASE -l 0
 
+
+Find slow queries
+^^^^^^^^^^^^^^^^^
+
+When you activate the profiler, you can choose to so with level 1 profiling
+instead of level 2. Level 1 configure the profiler system to log only "slow" operations.
+Then you have to set the threshold in milliseconds for the profile to consider an
+operation "slow". In the following example the threshold is set to 10 milliseconds::
+
+    $ mongotail sales -l 1
+    Profiling set to level 1
+    $ mongotail sales -s 10
+    Threshold profiling set to 10 milliseconds
+
+Then when you check your databases only operations that take 10 or more milliseconds
+will be displayed.
+
 A *step-by-step* guide of how to use Mongotail and the latest features
 is `here <http://mrsarm.blogspot.com.ar/2016/08/mongotail-2-0-with-new-features-mongodb-3-2-support.html>`_.
 
 
 Installation
 ------------
```

### Comparing `mongotail-3.1b1/setup.py` & `mongotail-3.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     packages=[
         'mongotail',
     ],
     zip_safe=False,
     platforms='any',
     install_requires=[
         'pymongo[srv]>=3.12,<5.0.0',
-        'res-address==2.0b1',
+        'res-address==2.0b2',
     ],
     entry_points={
         'console_scripts': [
             'mongotail = mongotail.mongotail:main',
         ],
     },
     classifiers=[
```

