# Comparing `tmp/pyxattr-0.8.0.tar.gz` & `tmp/pyxattr-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxattr-0.8.0.tar", last modified: Mon Dec 12 21:37:12 2022, max compression
+gzip compressed data, was "pyxattr-0.8.1.tar", last modified: Mon Apr 17 21:59:18 2023, max compression
```

## Comparing `pyxattr-0.8.0.tar` & `pyxattr-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 21:37:12.956730 pyxattr-0.8.0/
--rw-r--r--   0 root         (0) root         (0)    26527 2008-06-30 20:09:19.000000 pyxattr-0.8.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      259 2022-12-12 21:29:09.000000 pyxattr-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2611 2022-12-12 21:21:18.000000 pyxattr-0.8.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     7930 2022-12-12 21:36:41.000000 pyxattr-0.8.0/NEWS
--rw-r--r--   0 root         (0) root         (0)     1137 2022-12-12 21:37:12.956730 pyxattr-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3646 2022-12-12 21:20:40.000000 pyxattr-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 21:37:12.956730 pyxattr-0.8.0/doc/
--rw-r--r--   0 root         (0) root         (0)     8023 2022-12-12 21:21:30.000000 pyxattr-0.8.0/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      328 2021-06-05 15:50:39.000000 pyxattr-0.8.0/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1178 2021-06-05 15:50:39.000000 pyxattr-0.8.0/doc/module.rst
--rw-r--r--   0 root         (0) root         (0)     7930 2022-12-12 21:36:41.000000 pyxattr-0.8.0/doc/news.rst
--rw-r--r--   0 root         (0) root         (0)     3646 2022-12-12 21:20:40.000000 pyxattr-0.8.0/doc/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 21:37:12.956730 pyxattr-0.8.0/pyxattr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1137 2022-12-12 21:37:12.000000 pyxattr-0.8.0/pyxattr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      300 2022-12-12 21:37:12.000000 pyxattr-0.8.0/pyxattr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-12 21:37:12.000000 pyxattr-0.8.0/pyxattr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-12-12 21:37:12.000000 pyxattr-0.8.0/pyxattr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       82 2022-12-12 21:37:12.956730 pyxattr-0.8.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1963 2022-12-12 21:27:31.000000 pyxattr-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 21:37:12.956730 pyxattr-0.8.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2012-05-14 21:45:17.000000 pyxattr-0.8.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16366 2021-06-05 17:30:45.000000 pyxattr-0.8.0/tests/test_xattr.py
--rw-r--r--   0 root         (0) root         (0)    37574 2022-10-13 21:35:31.000000 pyxattr-0.8.0/xattr.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 21:59:18.128160 pyxattr-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)    26527 2008-06-30 20:09:19.000000 pyxattr-0.8.1/COPYING
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-17 21:47:59.000000 pyxattr-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-17 21:56:00.000000 pyxattr-0.8.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     7887 2023-04-17 21:50:36.000000 pyxattr-0.8.1/NEWS.md
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-17 21:59:18.128160 pyxattr-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-04-17 21:34:16.000000 pyxattr-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 21:59:18.128160 pyxattr-0.8.1/doc/
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-04-17 21:56:08.000000 pyxattr-0.8.1/doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-17 21:53:19.000000 pyxattr-0.8.1/doc/contributing.md
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-17 21:47:20.000000 pyxattr-0.8.1/doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1178 2021-06-05 15:50:39.000000 pyxattr-0.8.1/doc/module.rst
+-rw-r--r--   0 root         (0) root         (0)     7887 2023-04-17 21:50:36.000000 pyxattr-0.8.1/doc/news.md
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-04-17 21:34:16.000000 pyxattr-0.8.1/doc/readme.md
+-rw-r--r--   0 root         (0) root         (0)      648 2023-04-16 15:38:50.000000 pyxattr-0.8.1/doc/security.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 21:59:18.128160 pyxattr-0.8.1/pyxattr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-17 21:59:18.000000 pyxattr-0.8.1/pyxattr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-17 21:59:18.000000 pyxattr-0.8.1/pyxattr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 21:59:18.000000 pyxattr-0.8.1/pyxattr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-17 21:59:18.000000 pyxattr-0.8.1/pyxattr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-17 21:59:18.128160 pyxattr-0.8.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1965 2023-04-17 21:56:17.000000 pyxattr-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 21:59:18.128160 pyxattr-0.8.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2012-05-14 21:45:17.000000 pyxattr-0.8.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16366 2021-06-05 17:30:45.000000 pyxattr-0.8.1/tests/test_xattr.py
+-rw-r--r--   0 root         (0) root         (0)    37574 2022-10-13 21:35:31.000000 pyxattr-0.8.1/xattr.c
```

### Comparing `pyxattr-0.8.0/COPYING` & `pyxattr-0.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyxattr-0.8.0/Makefile` & `pyxattr-0.8.1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 PYTHON        = python3
 SPHINXOPTS    = -W
 SPHINXBUILD   = $(PYTHON) -m sphinx
 DOCDIR        = doc
 DOCHTML       = $(DOCDIR)/html
 DOCTREES      = $(DOCDIR)/doctrees
 ALLSPHINXOPTS = -d $(DOCTREES) $(SPHINXOPTS) $(DOCDIR)
-VERSION       = 0.8.0
+VERSION       = 0.8.1
 FULLVER       = pyxattr-$(VERSION)
 DISTFILE      = $(FULLVER).tar.gz
 
 MODNAME = xattr.so
-RSTFILES = doc/index.rst doc/module.rst doc/news.rst doc/readme.md doc/conf.py
-PYVERS = 3.7 3.8 3.9 3.10
+RSTFILES = doc/index.rst doc/module.rst doc/news.md doc/readme.md doc/conf.py
+PYVERS = 3.7 3.8 3.9 3.10 3.11
 REPS = 5
 
 all: doc test
 
 $(MODNAME): xattr.c
 	$(PYTHON) ./setup.py build_ext --inplace
```

### Comparing `pyxattr-0.8.0/NEWS` & `pyxattr-0.8.1/NEWS.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-News
-====
+# News
 
-Version 0.8.0
--------------
+## Version 0.8.1
+
+*Mon, 17 Apr 2023*
+
+Very minor release:
+
+* Fix the pypi declared python versions
+* Add some more documentation - a security policy, and a contributing
+  guide.
+* Restore yet again the CI environment :/
+
+## Version 0.8.0
 
 *Mon, 12 Dec 2022*
 
 Minor bugfix release, but due to lack of CI environments supporting old
 Python versions, only Python 3.7+ is supported. Otherwise:
 
 * Snape3058@ found some refcount issues (see issue #35), these have been
   fixed.
 * Tested and enabled Python 3.10 support, dropped < 3.7.
 * Various improvements to the CI environments.
 * Move fully to `setuptools` (where available), in preparation for 3.12
   dropping `distutils` support.
 
-Version 0.7.2
--------------
+## Version 0.7.2
 
 *Sun, 29 Nov 2020*
 
 Minor release:
 
 * Expand testing by adding better mixed-access checks (e.g. set via
   symlink and read on file) and by not leaking resources during tests.
 * Enable testing with Python 3.9 and confirm compatibility with it.
 * Fix documentation building with Sphinx 3.0+.
 
-Version 0.7.1
--------------
+## Version 0.7.1
 
 *released Tue, 26 Nov 2019*
 
 Typo fix release in the bug tracker link :/
 
-Version 0.7.0
--------------
+## Version 0.7.0
 
 *released Tue, 26 Nov 2019*
 
 Major change: drop compatibility with Python 2, which allows significant
 code cleanups.
 
 Other changes:
@@ -50,16 +56,15 @@
   path-like objects in Python 3.6+ (#20), and also a more uniform
   handling of Unicode path arguments with respect to other Python code.
 * Fix missing error check in list operations in `get_all` (#17).
 * Switch test library to pytest; not that a reasonable recent version is
   needed. Additionally, expand test coverage, although not directly
   visible in actual coverage reports…
 
-Version 0.6.1
--------------
+## Version 0.6.1
 
 *released Tue, 24 Jul 2018*
 
 Minor bugfix, performance and compatibility release.
 
 * Minor compatibility fix: on Linux, drop the use of the `attr` library,
   and instead switch to the glibc header `sys/xattr.h`, which is
@@ -72,16 +77,15 @@
   downsides are minor (between 0 and 5%, in many cases negligible). For
   remote or slow filesystems, this should allow much increased
   parallelism.
 * Fix symlink set operation on MacOS X; bugfix provided by adamlin, much
   appreciated! This also uncovered testing problems related to symlinks,
   which are now fixed (the bug would be caught by the updated tests).
 
-Version 0.6.0
--------------
+## Version 0.6.0
 
 *released Mon, 23 Jan 2017*
 
 Bugfix and feature release (hence the version bump).
 
 The main change is to the implementation of how attributes are listed
 and read. This was done due to existing race issues when attributes are
@@ -93,29 +97,27 @@
 might change the trade-off between number of syscalls done and memory
 usage.
 
 As feature release, OSX support was contributed by Adam Knight
 <adam@movq.us>, thanks a lot! I don't have access to OSX so the testing
 for it is done via Travis builds; please report any issues.
 
-Version 0.5.6
--------------
+## Version 0.5.6
 
 *released Sat, 09 Apr 2016*
 
 Small bugfix release:
 
 * Fixes some sign-compare warnings
 * Fixes potential name truncation in merge_ns()
 * Fixes building on systems which don't have ENODATA
 
 Tested with Python 2.7.11, Python 3.5.1 and PyPy 5.0.1.
 
-Version 0.5.5
--------------
+## Version 0.5.5
 
 *released Fri, 01 May 2015*
 
 Bugfix release:
 
 * fixes some more memory leaks when handling out-of-memory in get_all()
   function
@@ -124,24 +126,22 @@
 * fix int/size_t issues found by RedHat/Fedora,
   https://bugzilla.redhat.com/show_bug.cgi?id=1127310; the fix is
   different than their fix, but it should accomplish the same thing
 * convert all code to only do explicit casts after checking boundaries,
   making the code `-Wconversion`-clean (although that warning is not
   enabled by default)
 
-Version 0.5.4
--------------
+## Version 0.5.4
 
 *released Thu, 30 Apr 2015*
 
 Fix memory leaks on some of the error-handling paths of the `get()`
 function.
 
-Version 0.5.3
--------------
+## Version 0.5.3
 
 *released Fri, 23 May 2014*
 
 Small optimisations release:
 
 * ari edelkind contributed a speed-up optimisation for handling of files
   without xattrs (which is, in general, the expected case)
@@ -151,27 +151,25 @@
   can hide encoding errors, it mirrors what Python libraries do
   (e.g. see os.fsencode/fsdecode)
 * Sean Patrick Santos contributed improvements to the test suite so that
   it can be used even on files systems which have built-in attributes
   (e.g. when using SELinux, or NFSv4); to enable this, define the
   attributes in the TEST_IGNORE_XATTRS environment variable
 
-Version 0.5.2
--------------
+## Version 0.5.2
 
 *released Thu, 03 Jan 2013*
 
 Bug-fix release. Thanks to Michał Górny, it looked like the library had
 problem running under pypy, but actually there was a bug in the
 PyArg_ParseTuple use of et# (signed vs. unsigned, and lack of compiler
 warnings). This was fixed, and now the test suite passed with many
 CPython versions and PyPy (version 1.9).
 
-Version 0.5.1
--------------
+## Version 0.5.1
 
 *released Wed, 16 May 2012*
 
 Bug-fix release. Thanks to Dave Malcolm and his cpychecker tool, a
 number of significant bugs (refcount leaks and potential NULL-pointer
 dereferences) have been fixed.
 
@@ -181,77 +179,63 @@
 string if (due to the structure of your program) you have to pass this
 argument but want to specify no namespace.
 
 Also, the project home page has changed from SourceForge to GitHub, and
 the documentation has been converted from epydoc-based to sphinx.
 
 
-Version 0.5
------------
+## Version 0.5
 
 *released Sun, 27 Dec 2009*
 
 Implemented support for Python 3. This required a significant change to
 the C module, hence the new version number.
 
-Version 0.4
------------
+## Version 0.4
 
 *released Mon, 30 Jun 2008*
 
-API
-~~~
+### API
 
 The old functions ({get,set,list,remove}xattr) are deprecated and replaced with
 a new API that is namespace-aware and hopefully will allow other OSes (e.g.
 FreeBSD) to be supported more naturally.
 
 Both the old and the new API are supported in the 0.4 versions, however users
 are encouraged to migrate to the new API.
 
-New features
-~~~~~~~~~~~~
+### New features
 
 A new bulk get function called get_all() has been added that should be somewhat
 faster in case of querying files which have many attributes.
 
-License
-~~~~~~~
+### License
 
 Since LGPLv3 is not compatible with GPLv2 (which unfortunately I didn't realize
 before), the license was changed to LGPLv2.1 or later.
 
-Internals
-~~~~~~~~~
+### Internals
 
 Unittest coverage was improved.
 
-Version 0.3
------------
+## Version 0.3
 
 *released Sun, 09 Mar 2008*
 
 * changed licence from GPL to LGPL (3 or later)
 * changed listxattr return type from tuple to a list
 * developer-related: added unittests
 
-Version 0.2.2
--------------
+## Version 0.2.2
 
 *released Sun, 01 Jul 2007*
 
 * fixed listing symlink xattrs
 
-Version 0.2.1
--------------
+## Version 0.2.1
 
 *released Sat, 11 Feb 2006*
 
 * fixed a bug when reading symlink EAs (you weren't able to
   do it, actually)
 * fixed a possible memory leak when the actual read of the EA
   failed but the call to get the length of the EA didn't
-
-.. Local Variables:
-.. mode: rst
-.. fill-column: 72
-.. End:
```

### Comparing `pyxattr-0.8.0/PKG-INFO` & `pyxattr-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxattr
-Version: 0.8.0
+Version: 0.8.1
 Summary: Filesystem extended attributes for python
-Home-page: http://pyxattr.k1024.org/
-Download-URL: http://pyxattr.k1024.org/downloads/
+Home-page: https://pyxattr.k1024.org/
+Download-URL: https://pyxattr.k1024.org/downloads/
 Author: Iustin Pop
 Author-email: iustin@k1024.org
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/iustin/pyxattr/issues
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,13 +15,13 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 License-File: COPYING
 
 This is a C extension module for Python which
 implements extended attributes manipulation. It is a wrapper on top
 of the attr C library - see attr(5).
```

### Comparing `pyxattr-0.8.0/README.md` & `pyxattr-0.8.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # pyxattr
 
 This is the pyxattr module, a Python extension module which gives access
 to the extended attributes for filesystem objects available in some
 operating systems.
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/iustin/pyxattr/CI)](https://github.com/iustin/pyxattr/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iustin/pyxattr/ci.yml?branch=main)](https://github.com/iustin/pyxattr/actions/workflows/ci.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/iustin/pyxattr)](https://codecov.io/gh/iustin/pyxattr)
-[![Read the Docs](https://img.shields.io/readthedocs/pyxattr)](http://pyxattr.readthedocs.io/en/latest/?badge=latest)
+[![Read the Docs](https://img.shields.io/readthedocs/pyxattr)](https://pyxattr.readthedocs.io/en/latest/?badge=latest)
 [![GitHub issues](https://img.shields.io/github/issues/iustin/pyxattr)](https://github.com/iustin/pyxattr/issues)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/iustin/pyxattr)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/iustin/pyxattr)](https://github.com/iustin/pyxattr/releases)
 [![PyPI](https://img.shields.io/pypi/v/pyxattr)](https://pypi.org/project/pyxattr/)
 ![Debian package](https://img.shields.io/debian/v/python-pyxattr)
 ![Ubuntu package](https://img.shields.io/ubuntu/v/python-pyxattr)
 ![GitHub Release Date](https://img.shields.io/github/release-date/iustin/pyxattr)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/iustin/pyxattr/latest)
 ![GitHub last commit](https://img.shields.io/github/last-commit/iustin/pyxattr)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7236/badge)](https://bestpractices.coreinfrastructure.org/projects/7236)
 
 Downloads: go to <https://pyxattr.k1024.org/downloads/>. The source
-repository is either at <http://git.k1024.org/pyxattr.git> or at
+repository is either at <https://git.k1024.org/pyxattr.git> or at
 <https://github.com/iustin/pyxattr>.
 
+See the `CONTRIBUTING.md` file for details on how to contribute.
+
 ## Requirements
 
 The current supported Python versions are 3.7+ (tested up to 3.10), or
 PyPy versions 3.7+ (tested up to 3.9). The code should currently be
 compatible down to Python 3.4, but such versions are no longer tested.
 
 The library has been written and tested on Linux, kernel v2.4 or
@@ -45,14 +48,18 @@
     pip install pyxattr
 
 Or you can install already compiled versions from your distribution,
 e.g. in Debian:
 
     sudo apt install python3-pyxattr
 
+## Security
+
+For reporting security vulnerabilities, please see `SECURITY.md`.
+
 ## Basic example
 
     >>> import xattr
     >>> xattr.listxattr("file.txt")
     ['user.mime_type']
     >>> xattr.getxattr("file.txt", "user.mime_type")
     'text/plain'
```

### Comparing `pyxattr-0.8.0/doc/conf.py` & `pyxattr-0.8.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 copyright = u'2002, 2003, 2006, 2008, 2012, 2013, 2014, 2015, Iustin Pop'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.8.0'
+version = '0.8.1'
 # The full version, including alpha/beta/rc tags.
-release = '0.8.0'
+release = '0.8.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `pyxattr-0.8.0/doc/module.rst` & `pyxattr-0.8.1/doc/module.rst`

 * *Files identical despite different names*

### Comparing `pyxattr-0.8.0/doc/news.rst` & `pyxattr-0.8.1/doc/news.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-News
-====
+# News
 
-Version 0.8.0
--------------
+## Version 0.8.1
+
+*Mon, 17 Apr 2023*
+
+Very minor release:
+
+* Fix the pypi declared python versions
+* Add some more documentation - a security policy, and a contributing
+  guide.
+* Restore yet again the CI environment :/
+
+## Version 0.8.0
 
 *Mon, 12 Dec 2022*
 
 Minor bugfix release, but due to lack of CI environments supporting old
 Python versions, only Python 3.7+ is supported. Otherwise:
 
 * Snape3058@ found some refcount issues (see issue #35), these have been
   fixed.
 * Tested and enabled Python 3.10 support, dropped < 3.7.
 * Various improvements to the CI environments.
 * Move fully to `setuptools` (where available), in preparation for 3.12
   dropping `distutils` support.
 
-Version 0.7.2
--------------
+## Version 0.7.2
 
 *Sun, 29 Nov 2020*
 
 Minor release:
 
 * Expand testing by adding better mixed-access checks (e.g. set via
   symlink and read on file) and by not leaking resources during tests.
 * Enable testing with Python 3.9 and confirm compatibility with it.
 * Fix documentation building with Sphinx 3.0+.
 
-Version 0.7.1
--------------
+## Version 0.7.1
 
 *released Tue, 26 Nov 2019*
 
 Typo fix release in the bug tracker link :/
 
-Version 0.7.0
--------------
+## Version 0.7.0
 
 *released Tue, 26 Nov 2019*
 
 Major change: drop compatibility with Python 2, which allows significant
 code cleanups.
 
 Other changes:
@@ -50,16 +56,15 @@
   path-like objects in Python 3.6+ (#20), and also a more uniform
   handling of Unicode path arguments with respect to other Python code.
 * Fix missing error check in list operations in `get_all` (#17).
 * Switch test library to pytest; not that a reasonable recent version is
   needed. Additionally, expand test coverage, although not directly
   visible in actual coverage reports…
 
-Version 0.6.1
--------------
+## Version 0.6.1
 
 *released Tue, 24 Jul 2018*
 
 Minor bugfix, performance and compatibility release.
 
 * Minor compatibility fix: on Linux, drop the use of the `attr` library,
   and instead switch to the glibc header `sys/xattr.h`, which is
@@ -72,16 +77,15 @@
   downsides are minor (between 0 and 5%, in many cases negligible). For
   remote or slow filesystems, this should allow much increased
   parallelism.
 * Fix symlink set operation on MacOS X; bugfix provided by adamlin, much
   appreciated! This also uncovered testing problems related to symlinks,
   which are now fixed (the bug would be caught by the updated tests).
 
-Version 0.6.0
--------------
+## Version 0.6.0
 
 *released Mon, 23 Jan 2017*
 
 Bugfix and feature release (hence the version bump).
 
 The main change is to the implementation of how attributes are listed
 and read. This was done due to existing race issues when attributes are
@@ -93,29 +97,27 @@
 might change the trade-off between number of syscalls done and memory
 usage.
 
 As feature release, OSX support was contributed by Adam Knight
 <adam@movq.us>, thanks a lot! I don't have access to OSX so the testing
 for it is done via Travis builds; please report any issues.
 
-Version 0.5.6
--------------
+## Version 0.5.6
 
 *released Sat, 09 Apr 2016*
 
 Small bugfix release:
 
 * Fixes some sign-compare warnings
 * Fixes potential name truncation in merge_ns()
 * Fixes building on systems which don't have ENODATA
 
 Tested with Python 2.7.11, Python 3.5.1 and PyPy 5.0.1.
 
-Version 0.5.5
--------------
+## Version 0.5.5
 
 *released Fri, 01 May 2015*
 
 Bugfix release:
 
 * fixes some more memory leaks when handling out-of-memory in get_all()
   function
@@ -124,24 +126,22 @@
 * fix int/size_t issues found by RedHat/Fedora,
   https://bugzilla.redhat.com/show_bug.cgi?id=1127310; the fix is
   different than their fix, but it should accomplish the same thing
 * convert all code to only do explicit casts after checking boundaries,
   making the code `-Wconversion`-clean (although that warning is not
   enabled by default)
 
-Version 0.5.4
--------------
+## Version 0.5.4
 
 *released Thu, 30 Apr 2015*
 
 Fix memory leaks on some of the error-handling paths of the `get()`
 function.
 
-Version 0.5.3
--------------
+## Version 0.5.3
 
 *released Fri, 23 May 2014*
 
 Small optimisations release:
 
 * ari edelkind contributed a speed-up optimisation for handling of files
   without xattrs (which is, in general, the expected case)
@@ -151,27 +151,25 @@
   can hide encoding errors, it mirrors what Python libraries do
   (e.g. see os.fsencode/fsdecode)
 * Sean Patrick Santos contributed improvements to the test suite so that
   it can be used even on files systems which have built-in attributes
   (e.g. when using SELinux, or NFSv4); to enable this, define the
   attributes in the TEST_IGNORE_XATTRS environment variable
 
-Version 0.5.2
--------------
+## Version 0.5.2
 
 *released Thu, 03 Jan 2013*
 
 Bug-fix release. Thanks to Michał Górny, it looked like the library had
 problem running under pypy, but actually there was a bug in the
 PyArg_ParseTuple use of et# (signed vs. unsigned, and lack of compiler
 warnings). This was fixed, and now the test suite passed with many
 CPython versions and PyPy (version 1.9).
 
-Version 0.5.1
--------------
+## Version 0.5.1
 
 *released Wed, 16 May 2012*
 
 Bug-fix release. Thanks to Dave Malcolm and his cpychecker tool, a
 number of significant bugs (refcount leaks and potential NULL-pointer
 dereferences) have been fixed.
 
@@ -181,77 +179,63 @@
 string if (due to the structure of your program) you have to pass this
 argument but want to specify no namespace.
 
 Also, the project home page has changed from SourceForge to GitHub, and
 the documentation has been converted from epydoc-based to sphinx.
 
 
-Version 0.5
------------
+## Version 0.5
 
 *released Sun, 27 Dec 2009*
 
 Implemented support for Python 3. This required a significant change to
 the C module, hence the new version number.
 
-Version 0.4
------------
+## Version 0.4
 
 *released Mon, 30 Jun 2008*
 
-API
-~~~
+### API
 
 The old functions ({get,set,list,remove}xattr) are deprecated and replaced with
 a new API that is namespace-aware and hopefully will allow other OSes (e.g.
 FreeBSD) to be supported more naturally.
 
 Both the old and the new API are supported in the 0.4 versions, however users
 are encouraged to migrate to the new API.
 
-New features
-~~~~~~~~~~~~
+### New features
 
 A new bulk get function called get_all() has been added that should be somewhat
 faster in case of querying files which have many attributes.
 
-License
-~~~~~~~
+### License
 
 Since LGPLv3 is not compatible with GPLv2 (which unfortunately I didn't realize
 before), the license was changed to LGPLv2.1 or later.
 
-Internals
-~~~~~~~~~
+### Internals
 
 Unittest coverage was improved.
 
-Version 0.3
------------
+## Version 0.3
 
 *released Sun, 09 Mar 2008*
 
 * changed licence from GPL to LGPL (3 or later)
 * changed listxattr return type from tuple to a list
 * developer-related: added unittests
 
-Version 0.2.2
--------------
+## Version 0.2.2
 
 *released Sun, 01 Jul 2007*
 
 * fixed listing symlink xattrs
 
-Version 0.2.1
--------------
+## Version 0.2.1
 
 *released Sat, 11 Feb 2006*
 
 * fixed a bug when reading symlink EAs (you weren't able to
   do it, actually)
 * fixed a possible memory leak when the actual read of the EA
   failed but the call to get the length of the EA didn't
-
-.. Local Variables:
-.. mode: rst
-.. fill-column: 72
-.. End:
```

### Comparing `pyxattr-0.8.0/doc/readme.md` & `pyxattr-0.8.1/doc/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # pyxattr
 
 This is the pyxattr module, a Python extension module which gives access
 to the extended attributes for filesystem objects available in some
 operating systems.
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/iustin/pyxattr/CI)](https://github.com/iustin/pyxattr/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iustin/pyxattr/ci.yml?branch=main)](https://github.com/iustin/pyxattr/actions/workflows/ci.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/iustin/pyxattr)](https://codecov.io/gh/iustin/pyxattr)
-[![Read the Docs](https://img.shields.io/readthedocs/pyxattr)](http://pyxattr.readthedocs.io/en/latest/?badge=latest)
+[![Read the Docs](https://img.shields.io/readthedocs/pyxattr)](https://pyxattr.readthedocs.io/en/latest/?badge=latest)
 [![GitHub issues](https://img.shields.io/github/issues/iustin/pyxattr)](https://github.com/iustin/pyxattr/issues)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/iustin/pyxattr)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/iustin/pyxattr)](https://github.com/iustin/pyxattr/releases)
 [![PyPI](https://img.shields.io/pypi/v/pyxattr)](https://pypi.org/project/pyxattr/)
 ![Debian package](https://img.shields.io/debian/v/python-pyxattr)
 ![Ubuntu package](https://img.shields.io/ubuntu/v/python-pyxattr)
 ![GitHub Release Date](https://img.shields.io/github/release-date/iustin/pyxattr)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/iustin/pyxattr/latest)
 ![GitHub last commit](https://img.shields.io/github/last-commit/iustin/pyxattr)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7236/badge)](https://bestpractices.coreinfrastructure.org/projects/7236)
 
 Downloads: go to <https://pyxattr.k1024.org/downloads/>. The source
-repository is either at <http://git.k1024.org/pyxattr.git> or at
+repository is either at <https://git.k1024.org/pyxattr.git> or at
 <https://github.com/iustin/pyxattr>.
 
+See the `CONTRIBUTING.md` file for details on how to contribute.
+
 ## Requirements
 
 The current supported Python versions are 3.7+ (tested up to 3.10), or
 PyPy versions 3.7+ (tested up to 3.9). The code should currently be
 compatible down to Python 3.4, but such versions are no longer tested.
 
 The library has been written and tested on Linux, kernel v2.4 or
@@ -45,14 +48,18 @@
     pip install pyxattr
 
 Or you can install already compiled versions from your distribution,
 e.g. in Debian:
 
     sudo apt install python3-pyxattr
 
+## Security
+
+For reporting security vulnerabilities, please see `SECURITY.md`.
+
 ## Basic example
 
     >>> import xattr
     >>> xattr.listxattr("file.txt")
     ['user.mime_type']
     >>> xattr.getxattr("file.txt", "user.mime_type")
     'text/plain'
```

### Comparing `pyxattr-0.8.0/pyxattr.egg-info/PKG-INFO` & `pyxattr-0.8.1/pyxattr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyxattr
-Version: 0.8.0
+Version: 0.8.1
 Summary: Filesystem extended attributes for python
-Home-page: http://pyxattr.k1024.org/
-Download-URL: http://pyxattr.k1024.org/downloads/
+Home-page: https://pyxattr.k1024.org/
+Download-URL: https://pyxattr.k1024.org/downloads/
 Author: Iustin Pop
 Author-email: iustin@k1024.org
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/iustin/pyxattr/issues
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,13 +15,13 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 License-File: COPYING
 
 This is a C extension module for Python which
 implements extended attributes manipulation. It is a wrapper on top
 of the attr C library - see attr(5).
```

### Comparing `pyxattr-0.8.0/setup.py` & `pyxattr-0.8.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,39 +5,39 @@
   from setuptools import setup, Extension
 except ImportError:
   from distutils.core import setup, Extension
 
 long_desc = """This is a C extension module for Python which
 implements extended attributes manipulation. It is a wrapper on top
 of the attr C library - see attr(5)."""
-version = "0.8.0"
+version = "0.8.1"
 author = "Iustin Pop"
 author_email = "iustin@k1024.org"
 libraries = []
 macros = [
     ("_XATTR_VERSION", '"%s"' % version),
     ("_XATTR_AUTHOR", '"%s"' % author),
     ("_XATTR_EMAIL", '"%s"' % author_email),
     ]
 setup(name = "pyxattr",
       version = version,
       description = "Filesystem extended attributes for python",
       long_description = long_desc,
       author = author,
       author_email = author_email,
-      url = "http://pyxattr.k1024.org/",
-      download_url = "http://pyxattr.k1024.org/downloads/",
+      url = "https://pyxattr.k1024.org/",
+      download_url = "https://pyxattr.k1024.org/downloads/",
       license = "LGPL",
       ext_modules = [Extension("xattr", ["xattr.c"],
                                libraries=libraries,
                                define_macros=macros,
                                extra_compile_args=["-Wall", "-Werror", "-Wsign-compare"],
                                )],
       platforms = ["Linux"],
-      python_requires = ">=3.4",
+      python_requires = ">=3.7",
       project_urls={
         "Bug Tracker": "https://github.com/iustin/pyxattr/issues",
       },
       classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
```

### Comparing `pyxattr-0.8.0/tests/test_xattr.py` & `pyxattr-0.8.1/tests/test_xattr.py`

 * *Files identical despite different names*

### Comparing `pyxattr-0.8.0/xattr.c` & `pyxattr-0.8.1/xattr.c`

 * *Files identical despite different names*

