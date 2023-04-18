# Comparing `tmp/auxly-0.8.2.tar.gz` & `tmp/auxly-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\auxly-0.8.2.tar", last modified: Sun Jan 31 16:43:58 2021, max compression
+gzip compressed data, was "dist\auxly-0.9.0.tar", last modified: Tue Apr 18 02:47:22 2023, max compression
```

## Comparing `auxly-0.8.2.tar` & `auxly-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-01-31 16:43:57.993309 auxly-0.8.2/
--rw-rw-rw-   0        0        0     4510 2021-01-31 16:43:57.992311 auxly-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     3160 2021-01-31 16:43:56.000000 auxly-0.8.2/README.rst
-drwxrwxrwx   0        0        0        0 2021-01-31 16:43:57.970370 auxly-0.8.2/auxly/
--rw-rw-rw-   0        0        0     5458 2021-01-31 16:34:47.000000 auxly-0.8.2/auxly/__init__.py
--rw-rw-rw-   0        0        0    19758 2021-01-31 16:35:33.000000 auxly-0.8.2/auxly/filesys.py
--rw-rw-rw-   0        0        0     1267 2018-11-03 03:11:30.000000 auxly-0.8.2/auxly/listy.py
--rw-rw-rw-   0        0        0     7336 2020-12-12 04:50:52.000000 auxly-0.8.2/auxly/shell.py
--rw-rw-rw-   0        0        0     1726 2020-11-14 20:23:39.000000 auxly-0.8.2/auxly/stringy.py
-drwxrwxrwx   0        0        0        0 2021-01-31 16:43:57.990318 auxly-0.8.2/auxly.egg-info/
--rw-rw-rw-   0        0        0     4510 2021-01-31 16:43:57.000000 auxly-0.8.2/auxly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2021-01-31 16:43:57.000000 auxly-0.8.2/auxly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-31 16:43:57.000000 auxly-0.8.2/auxly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2021-01-31 16:43:57.000000 auxly-0.8.2/auxly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-31 16:43:57.993309 auxly-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2021-01-31 16:34:47.000000 auxly-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:22.767397 auxly-0.9.0/
+-rw-rw-rw-   0        0        0     4686 2023-04-18 02:47:22.767397 auxly-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3282 2023-04-18 02:47:21.000000 auxly-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:22.742497 auxly-0.9.0/auxly/
+-rw-rw-rw-   0        0        0     1100 2023-04-18 02:45:54.000000 auxly-0.9.0/auxly/__init__.py
+-rw-rw-rw-   0        0        0    23471 2023-04-18 02:37:13.000000 auxly-0.9.0/auxly/filesys.py
+-rw-rw-rw-   0        0        0     2191 2023-04-18 02:31:47.000000 auxly-0.9.0/auxly/listy.py
+-rw-rw-rw-   0        0        0     7343 2023-04-18 02:31:47.000000 auxly-0.9.0/auxly/shell.py
+-rw-rw-rw-   0        0        0     2564 2023-04-18 02:31:47.000000 auxly-0.9.0/auxly/stringy.py
+-rw-rw-rw-   0        0        0     6287 2023-04-18 02:31:47.000000 auxly-0.9.0/auxly/top.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:22.767397 auxly-0.9.0/auxly.egg-info/
+-rw-rw-rw-   0        0        0     4686 2023-04-18 02:47:22.000000 auxly-0.9.0/auxly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-18 02:47:22.000000 auxly-0.9.0/auxly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:47:22.000000 auxly-0.9.0/auxly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 02:47:22.000000 auxly-0.9.0/auxly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:47:22.767397 auxly-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-04-18 02:45:54.000000 auxly-0.9.0/setup.py
```

### Comparing `auxly-0.8.2/PKG-INFO` & `auxly-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 1.1
 Name: auxly
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python library for common shell-like script tasks.
 Home-page: https://github.com/jeffrimko/Auxly
 Author: Jeff Rimko
 Author-email: jeffrimko@gmail.com
 License: MIT
 Description: |License| |Build Status|
         
+        .. _`_introduction`:
         
         Introduction
         ============
         
         This project provides a Python 2.7/3.x library for common tasks
         especially when writing shell-like scripts. Some of the functionality
         overlaps with the standard library but the API is slightly modified.
@@ -54,49 +55,54 @@
         -  `examples/guess_os.py <https://github.com/jeffrimko/Auxly/blob/master/examples/guess_os.py>`__
            - Attempts to guess the host OS based on available shell commands.
         
         Refer to the unit tests
         `here <https://github.com/jeffrimko/Auxly/tree/master/tests>`__ for
         additional examples.
         
+        .. _`_status`:
         
         Status
         ======
         
         Currently, this project is in the **development release** stage. While
         this project is suitable for use, please note that there may be
         incompatibilities in new releases.
         
         Release notes are maintained in the project
         `changelog <https://github.com/jeffrimko/Auxly/blob/master/CHANGELOG.adoc>`__.
         
+        .. _`_requirements`:
         
         Requirements
         ============
         
         Auxly should run on any Python 2.7/3.x interpreter without additional
         dependencies.
         
+        .. _`_installation`:
         
         Installation
         ============
         
         Auxly can be installed with pip using the following command:
         ``pip install auxly``
         
         Additionally, Auxly can be installed from source by running:
         ``python setup.py install``
         
+        .. _`_documentation`:
         
         Documentation
         =============
         
         The full documentation for this project can be found `here on Read the
         Docs <http://auxly.readthedocs.io>`__.
         
+        .. _`_similar`:
         
         Similar
         =======
         
         The following projects are similar and may be worth checking out:
         
         -  `Reusables <https://github.com/cdgriffith/Reusables>`__
```

### Comparing `auxly-0.8.2/README.rst` & `auxly-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 |License| |Build Status|
 
+.. _`_introduction`:
 
 Introduction
 ============
 
 This project provides a Python 2.7/3.x library for common tasks
 especially when writing shell-like scripts. Some of the functionality
 overlaps with the standard library but the API is slightly modified.
@@ -46,49 +47,54 @@
 -  `examples/guess_os.py <https://github.com/jeffrimko/Auxly/blob/master/examples/guess_os.py>`__
    - Attempts to guess the host OS based on available shell commands.
 
 Refer to the unit tests
 `here <https://github.com/jeffrimko/Auxly/tree/master/tests>`__ for
 additional examples.
 
+.. _`_status`:
 
 Status
 ======
 
 Currently, this project is in the **development release** stage. While
 this project is suitable for use, please note that there may be
 incompatibilities in new releases.
 
 Release notes are maintained in the project
 `changelog <https://github.com/jeffrimko/Auxly/blob/master/CHANGELOG.adoc>`__.
 
+.. _`_requirements`:
 
 Requirements
 ============
 
 Auxly should run on any Python 2.7/3.x interpreter without additional
 dependencies.
 
+.. _`_installation`:
 
 Installation
 ============
 
 Auxly can be installed with pip using the following command:
 ``pip install auxly``
 
 Additionally, Auxly can be installed from source by running:
 ``python setup.py install``
 
+.. _`_documentation`:
 
 Documentation
 =============
 
 The full documentation for this project can be found `here on Read the
 Docs <http://auxly.readthedocs.io>`__.
 
+.. _`_similar`:
 
 Similar
 =======
 
 The following projects are similar and may be worth checking out:
 
 -  `Reusables <https://github.com/cdgriffith/Reusables>`__
```

### Comparing `auxly-0.8.2/auxly/__init__.py` & `auxly-0.9.0/auxly/top.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,61 @@
 ##==============================================================#
 ## SECTION: Imports                                             #
 ##==============================================================#
 
 from __future__ import print_function
+
 import ctypes
 import os
 import os.path as op
 import platform
 import subprocess
-
-import auxly.filesys
-import auxly.shell
-import auxly.stringy
-import auxly.listy
-
-##==============================================================#
-## SECTION: Global Definitions                                  #
-##==============================================================#
-
-#: Library version string.
-__version__ = "0.8.2"
+import sys
+import traceback
 
 ##==============================================================#
 ## SECTION: Class Definitions                                   #
 ##==============================================================#
 
 class AuxlyError(Exception):
     """Default Auxly error."""
-    pass
+    def __init__(self, ex=None):
+        self.exc_name = ""
+        self.traceback = ""
+        self.ex = ex
+        if isinstance(ex, Exception):
+            try:
+                raise ex
+            except:
+                self.ex = ""
+                self._trycollect()
+        else:
+            self._trycollect()
+        super(AuxlyError, self).__init__(ex)
+    def _trycollect(self):
+        try:
+            self.exc_name = sys.exc_info()[0].__name__
+            self.traceback = traceback.format_exc() or ""
+        except:
+            pass
+    def __bool__(self):
+        return False
+    def __str__(self):
+        output = self.__class__.__name__
+        if self.ex or self.traceback:
+            output += ": "
+        if self.ex:
+            output += str(self.ex)
+        if self.exc_name:
+            output += str(self.exc_name)
+        if self.traceback:
+            output += os.linesep + str(self.traceback)
+        return output
+    def __repr__(self):
+        return str(self)
 
 ##==============================================================#
 ## SECTION: Function Definitions                                #
 ##==============================================================#
 
 def iswindows():
     """Returns true if host OS is Windows."""
@@ -72,15 +96,15 @@
     ::
         throw()
         throw("error message")
         throw(ValueError)
         throw(ValueError, "error message")
     """
     exception = AuxlyError
-    if len(args) > 0 and isinstance(args[0], type(Exception)):
+    if len(args) > 0 and isinstance(args[0], type) and issubclass(args[0], Exception):
         exception = args[0]
         args = args[1:]
     raise exception(*args, **kwargs)
 
 def isadmin():
     """Returns true if the script is being run in admin mode, otherwise
     false."""
@@ -93,14 +117,19 @@
     function is returned which will suppress output."""
     def _vprint(msg, **kwargs):
         print(msg, **kwargs)
     def _nprint(msg, **kwargs):
         pass
     return _vprint if enabled else _nprint
 
+def trythrow(arg):
+    if isinstance(arg, Exception):
+        raise arg
+    return arg
+
 def trycatch(*args, **kwargs):
     """Wraps a function in a try/catch block. Can be used as a function
     decorator or as a function that accepts another function.
 
     **Params**:
       - func (func) - Function to call. Only available when used as a function.
       - oncatch (str) [kwargs] - Function to call if an exception is caught.
```

### Comparing `auxly-0.8.2/auxly/filesys.py` & `auxly-0.9.0/auxly/filesys.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Library of functions related to file system contents and manipulation."""
 
 ##==============================================================#
 ## SECTION: Imports                                             #
 ##==============================================================#
 
+from datetime import datetime
 import atexit
 import codecs
 import hashlib
 import os
 import os.path as op
-import re
 import shutil
 import sys
-from datetime import datetime
+
+import top as auxly
+from stringy import haspattern, subtract
 
 ##==============================================================#
 ## SECTION: Global Definitions                                  #
 ##==============================================================#
 
 #: Default file encoding.
 ENCODING = "utf-8"
@@ -56,146 +58,208 @@
     def __exit__(self, type, value, traceback):
         os.chdir(self.original)
     def __getattr__(self, name):
         return getattr(self.path, name)
     def __repr__(self):
         return self.path
 
-class _FileSysObject(object):
-    def __init__(self, path, *extrapath):
-        self._fspath = op.join(path, *extrapath)
-    def isfile(self):
-        """Returns true if object is file, otherwise false."""
-        return op.isfile(self._fspath)
-    def isdir(self):
-        """Returns true if object is directory, otherwise false."""
-        return op.isdir(self._fspath)
-    def dirpath(self):
-        """Returns a ``Path`` object for the directory associated with this
-        object."""
-        try:
-            if self.isfile():
-                return Path(op.dirname(self._fspath))
-            else:
-                return Path(self)
-        except:
-            return None
+class Path(str):
+    """Object representing a file system path."""
+    def __new__(cls, path, *extrapath, **kwargs):
+        return super(Path, cls).__new__(cls, op.abspath(op.join(path, *extrapath)))
+    def __init__(self, *path):
+        self._fspath = op.abspath(op.join(*path))
+    def __add__(self, value):
+        return Path(self._fspath + value)
+    def __sub__(self, value):
+        return Path(subtract(self._fspath, value))
+    def __repr__(self):
+        return self._fspath
+    @property
+    def path(self):
+        """Returns the path as a string."""
+        return self._fspath
     @property
     def name(self):
+        """Returns the base name of the path."""
         return op.basename(self._fspath)
+    @property
+    def parent(self):
+        """Returns a ``Dir`` for the parent directory of this object."""
+        return Dir(op.dirname(self._fspath))
+    def join(self, relpath):
+        """Returns a ``Path`` of the given relative path joined with this
+        object."""
+        return Path(self, relpath)
     def exists(self):
         """Returns true if object exists, otherwise false."""
         return op.exists(self._fspath)
+    def isdir(self):
+        """Returns true if path is for an existing directory, otherwise false."""
+        return op.isdir(self._fspath)
+    def isfile(self):
+        """Returns true if path is for an existing file, otherwise false."""
+        return op.isfile(self._fspath)
     def isempty(self):
         """Returns true if object is empty, otherwise false."""
         return isempty(self._fspath)
     def created(self):
         """Returns the object created date/time."""
+        if not self.exists():
+            return None
         try:
             return datetime.fromtimestamp(op.getctime(self._fspath))
-        except:
-            return None
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
     def modified(self):
         """Returns the object modified date/time."""
+        if not self.exists():
+            return None
         try:
             return datetime.fromtimestamp(op.getmtime(self._fspath))
-        except:
-            return None
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
     def size(self):
         """Returns the size of the object in bytes."""
-        try:
-            return getsize(self._fspath, recurse=True)
-        except:
+        if not self.exists():
             return None
+        try:
+            return getsize(self._fspath, recurse=False)
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
+    def delete(self):
+        """Deletes the file. Returns true if successful, otherwise false."""
+        return delete(self)
+    def copy(self, dstpath):
+        return copy(self._fspath, dstpath)
+    def move(self, dstpath):
+        return move(self._fspath, dstpath)
 
-class Path(_FileSysObject, str):
-    """Object representing a file system path."""
-    def __new__(cls, path, *extrapath):
-        return super(Path, cls).__new__(cls, op.abspath(op.join(path, *extrapath)))
-    def __init__(self, *path):
-        super(Path, self).__init__(self)
-        #: The directory path.
-        self.dir = None
-        #: The file name with extension, e.g. "myfile.txt".
-        self.filename = None
-        #: The file name without extension, e.g. "myfile".
-        self.file = None
-        #: The file extension, e.g. ".txt".
-        self.ext = None
-        self.parse()
-    def parse(self):
-        if op.isdir(self):
-            self.dir = self
-        elif op.isfile(self):
-            base = op.basename(self)
-            self.dir = op.dirname(self)
-            self.filename = base
-            self.file = op.splitext(base)[0]
-            self.ext = op.splitext(base)[1]
-    def join(self, relpath):
-        """Joins the given relative path with this path."""
-        return Path(self, relpath)
+class Dir(Path):
+    """Object representing a file system directory."""
+    def __init__(self, path, *extrapath, **kwargs):
+        """Dir object for the given path.
 
-class File(_FileSysObject):
+        **Params:**
+          - path (str) - Path to the directory. Multiple values will be passed to
+            `os.path.join()`.
+          - make (bool) [kwargs] - If true, the directory will be created if it
+            does not exist.
+          - del_at_exit (bool) [kwargs] - If true, the directory will be
+            deleted when the script exits.
+        """
+        if not path:
+            raise ValueError("no path provided")
+        if isinstance(path, Path):
+            path = path._fspath
+        super(Dir, self).__init__(path, *extrapath)
+        if self.exists() and self.isfile():
+            raise TypeError("dir cannot be file")
+        if kwargs.get('make'):
+            self.make()
+        if kwargs.get('del_at_exit'):
+            atexit.register(self.delete)
+    def countall(self, **kwargs):
+        return countall(self, **kwargs)
+    def countfiles(self, **kwargs):
+        return countfiles(self, **kwargs)
+    def countdirs(self, **kwargs):
+        return countdirs(self, **kwargs)
+    def walkall(self, **kwargs):
+        for i in walkall(self, **kwargs):
+            yield i
+    def walkfiles(self, **kwargs):
+        for i in walkfiles(self, **kwargs):
+            yield i
+    def walkdirs(self, **kwargs):
+        for i in walkdirs(self, **kwargs):
+            yield i
+    def make(self):
+        """Creates the directory if it does not already exist. No effect if the
+        directory already exists."""
+        return makedirs(self, ignore_extsep=True)
+
+class File(Path):
     """Object representing a file system file. The ENCODING variable defines the
     default encoding."""
     def __init__(self, path, *extrapath, **kwargs):
-        """Creates a file object for the given path.
+        """File object for the given path.
 
         **Params:**
           - path (str) - Path to the file. Multiple values will be passed to
             `os.path.join()`.
+          - make (bool) [kwargs] - If true, the file will be created if it does
+            not exist.
           - del_at_exit (bool) [kwargs] - If true, the file will be deleted when the
             script exits.
         """
         if not path:
             raise ValueError("no path provided")
-        #: The file path as a ``Path`` object.
-        self.path = Path(path, *extrapath)
-        if self.path.exists() and self.path.isdir():
+        if isinstance(path, Path):
+            path = path._fspath
+        super(File, self).__init__(path, *extrapath)
+        if self.exists() and self.isdir():
             raise TypeError("file cannot be dir")
-        super(File, self).__init__(self.path)
-        del_at_exit = kwargs.get('del_at_exit')
-        if del_at_exit:
+        if kwargs.get('make'):
+            self.make()
+        if kwargs.get('del_at_exit'):
             atexit.register(self.delete)
-    def __repr__(self):
-        return self.path
+    @property
+    def stem(self):
+        """Returns the file stem, i.e. the file name without the extension."""
+        toks = op.basename(self._fspath)
+        return op.splitext(toks)[0]
+    @property
+    def ext(self):
+        """Returns the file extension including the period (e.g. `.txt`)."""
+        toks = op.basename(self._fspath)
+        return op.splitext(toks)[1]
     def read(self, encoding=None):
         """Reads from the file and returns result as a string."""
         encoding = encoding or ENCODING
+        if not self.exists():
+            return None
         try:
-            with codecs.open(self.path, encoding=encoding) as fi:
+            with codecs.open(self, encoding=encoding) as fi:
                 return fi.read()
-        except:
-            return None
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
+    def splitlines(self, encoding=None):
+        """Reads from the file and returns result as a list of lines with endings removed."""
+        try:
+            return (self.read(encoding=encoding) or "").splitlines()
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
     def readlines(self, encoding=None):
-        """Reads from the file and returns result as a list of lines."""
+        """Reads from the file and returns result as a list of lines with endings included."""
+        if not self.exists():
+            return []
         try:
             encoding = encoding or ENCODING
-            with codecs.open(self.path, encoding=encoding) as fi:
+            with codecs.open(self, encoding=encoding) as fi:
                 return fi.readlines()
-        except:
-            return []
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
     def _write(self, content, mode, encoding=None, linesep=False):
         """Handles file writes."""
-        makedirs(self.path)
+        makedirs(self)
         try:
             encoding = encoding or ENCODING
             if "b" not in mode:
                 try:
                     content = str(content)
-                except:
+                except Exception:
                     pass
                 if linesep:
                     content += os.linesep
-            with codecs.open(self.path, mode, encoding=encoding) as fo:
+            with codecs.open(self, mode, encoding=encoding) as fo:
                 fo.write(content)
                 return True
-        except:
-            return False
+        except Exception as ex:
+            return auxly.AuxlyError(ex)
     def append(self, content, binary=False, encoding=None):
         """Appends the given content to the file. Existing content is
         preserved. Returns true if successful, otherwise false."""
         mode = "ab" if binary else "a"
         return self._write(content, mode, encoding=encoding, linesep=False)
     def appendline(self, content, binary=False, encoding=None):
         """Same as `append()` but adds a line break after the content."""
@@ -209,32 +273,28 @@
     def writeline(self, content, binary=False, encoding=None):
         """Same as `write()` but adds a line break after the content."""
         mode = "wb" if binary else "w"
         return self._write(content, mode, encoding=encoding, linesep=True)
     def empty(self):
         """Erases/empties the content in a file but does not delete it."""
         return self.write("")
-    def delete(self):
-        """Deletes the file. Returns true if successful, otherwise false."""
-        return delete(self.path)
     def checksum(self, **kwargs):
         """Returns the checksum of the file."""
-        return checksum(self.path, **kwargs)
+        return checksum(self, **kwargs)
+    def make(self):
+        """Creates an empty file If the file does not already exist. No effect
+        if the file already exist."""
+        if self.isfile():
+            return True
+        return self.empty()
 
 ##==============================================================#
 ## SECTION: Function Definitions                                #
 ##==============================================================#
 
-def _is_match(regex, text):
-    """Returns true if the given text matches the given regex pattern."""
-    try:
-        return re.compile(regex).search(text) != None
-    except:
-        return False
-
 def abspath(relpath, root=None):
     """Returns an absolute path based on the given root and relative path."""
     root = root or cwd()
     if op.isfile(root):
         root = op.dirname(root)
     return op.abspath(op.join(root, relpath))
 
@@ -249,26 +309,28 @@
         print(auxly.filesys.cwd())  # Get the CWD.
         auxly.filesys.cwd("foo")  # Set the CWD to `foo`.
     """
     return Cwd(path, root=root).path
 
 def makedirs(path, ignore_extsep=False):
     """Makes all directories required for given path; returns true if successful
-    otherwise false.
+    otherwise false. Returns true if directories already exist.
 
     **Examples**:
     ::
         auxly.filesys.makedirs("bar/baz")
     """
+    if op.isdir(path):
+       return True
     if not ignore_extsep and op.basename(path).find(os.extsep) > -1:
         path = op.dirname(path)
     try:
         os.makedirs(path)
-    except:
-        return False
+    except Exception as ex:
+        return auxly.AuxlyError(ex)
     return True
 
 def delete(path, regex=None, recurse=False, test=False):
     """Deletes the file or directory at `path`. If `path` is a directory and
     `regex` is provided, matching files will be deleted; `recurse` controls
     whether subdirectories are recursed. A list of deleted items is returned.
     If `test` is true, nothing will be deleted and a list of items that would
@@ -279,85 +341,106 @@
         if not test: os.remove(path)
         else: return [path]
         return [] if op.exists(path) else [path]
     elif op.isdir(path):
         if regex:
             for r,ds,fs in os.walk(path):
                 for i in fs:
-                    if _is_match(regex, i):
+                    if haspattern(regex, i):
                         deleted += delete(op.join(r,i), test=test)
                 if not recurse:
                     break
         else:
             if not test: shutil.rmtree(path)
             else: return [path]
             return [] if op.exists(path) else [path]
     return deleted
 
-def walkfiles(startdir, regex=None, recurse=True, regex_entire=True):
-    """Yields Path object for files found within the given start
+def walkall(startdir, regex=None, regex_entire=True, recurse=False):
+    """Yields a ``File`` or ``Dir`` for all found files and directories within
+    the given start directory. Can optionally filter paths using a regex
+    pattern, either on the entire path if regex_entire is true otherwise on the
+    file name only."""
+    if not op.isdir(startdir):
+        return
+    for i in walkdirs(startdir, regex, regex_entire, recurse):
+        yield i
+    for i in walkfiles(startdir, regex, regex_entire, recurse):
+        yield i
+
+def walkfiles(startdir, regex=None, regex_entire=True, recurse=False):
+    """Yields a ``File`` for files found within the given start
     directory. Can optionally filter paths using a regex pattern, either on the
     entire path if regex_entire is true otherwise on the file name only."""
+    if not op.isdir(startdir):
+        return
     if sys.version_info >= (3, 6):
         startdir = op.abspath(startdir)
         with os.scandir(startdir) as it:
             for i in it:
                 if i.is_file():
                     if regex:
                         path = op.join(startdir, i.name)
                         n = path if regex_entire else i.name
-                        if _is_match(regex, n):
-                            yield Path(path)
+                        if haspattern(regex, n):
+                            yield File(path)
                     else:
-                        yield op.join(startdir, i.name)
+                        yield File(op.join(startdir, i.name))
                 elif recurse:
                     for j in walkfiles(op.join(startdir, i.name), regex, recurse, regex_entire):
-                        yield Path(j)
+                        yield File(j)
     else:
         for r,_,fs in os.walk(startdir):
             if not recurse and startdir != r:
                 return
             for f in fs:
                 path = op.abspath(op.join(r,f))
                 n = path if regex_entire else f
-                if regex and not _is_match(regex, n):
+                if regex and not haspattern(regex, n):
                     continue
                 if op.isfile(path):
-                    yield Path(path)
+                    yield File(path)
 
-def walkdirs(startdir, regex=None, recurse=True, regex_entire=True):
+def walkdirs(startdir, regex=None, regex_entire=True, recurse=False):
     """Yields Path object for directories found within the given start
     directory. Can optionally filter paths using a regex pattern, either on the
     entire path if regex_entire is true otherwise on the directory name only."""
+    if not op.isdir(startdir):
+        return
     if sys.version_info >= (3, 6):
         startdir = op.abspath(startdir)
         with os.scandir(startdir) as it:
             for i in it:
                 if i.is_dir():
                     if regex:
                         path = op.join(startdir, i.name)
                         n = path if regex_entire else op.basename(i.name)
-                        if _is_match(regex, n):
-                            yield Path(path)
+                        if haspattern(regex, n):
+                            yield Dir(path)
                     else:
-                        yield Path(startdir, i.name)
+                        yield Dir(startdir, i.name)
                     if recurse:
                         for j in walkdirs(op.join(startdir, i.name), regex, recurse, regex_entire):
-                            yield Path(j)
+                            yield Dir(j)
     else:
         for r,ds,_ in os.walk(startdir):
             if not recurse and startdir != r:
                 return
             for d in ds:
                 path = op.abspath(op.join(r,d))
                 n = path if regex_entire else d
-                if regex and not _is_match(regex, n):
+                if regex and not haspattern(regex, n):
                     continue
                 if op.isfile(path):
-                    yield Path(path)
+                    yield Dir(path)
+
+def countall(path, recurse=False):
+    """Returns the number of directories and files under the given directory
+    path."""
+    return countfiles(path, recurse) + countdirs(path, recurse)
 
 def countfiles(path, recurse=False):
     """Returns the number of files under the given directory path."""
     if not op.isdir(path):
         return 0
     count = 0
     for r,ds,fs in os.walk(path):
@@ -449,15 +532,16 @@
         shutil.copy2(srcpath, dstpath)
 
     return op.exists(dstpath)
 
 def move(srcpath, dstpath, overwrite=True):
     """Moves the file or directory at `srcpath` to `dstpath`. Returns true if
     successful, otherwise false."""
-    # TODO: (JRR@201612230924) Consider adding smarter checks to prevent files ending up with directory names; e.g. if dstpath directory does not exist.
+    # TODO: Consider adding smarter checks to prevent files ending up with
+    # directory names; e.g. if dstpath directory does not exist.
     srcpath = op.abspath(srcpath)
     dstpath = op.abspath(dstpath)
     if not op.exists(srcpath):
         return False
     if srcpath == dstpath:
         return True
     if op.isfile(srcpath) and op.isdir(dstpath):
@@ -483,16 +567,16 @@
             # prevent unintentionally deleting the srcpath before moving.
             if "nt" == os.name and srcpath.lower() == dstpath.lower():
                 pass
             elif not delete(verpath):
                 return False
     try:
         shutil.move(srcpath, dstpath)
-    except:
-        return False
+    except Exception as ex:
+        return auxly.AuxlyError(ex)
     return verfunc(verpath)
 
 def checksum(fpath, hasher=None, asbytes=False):
     """Returns the checksum of the file at the given path as a hex string
     (default) or as a bytes literal. Uses MD5 by default.
 
     **Attribution**:
@@ -500,25 +584,28 @@
     `Stack Overflow <https://stackoverflow.com/a/3431835/789078>`_."""
     def blockiter(fpath, blocksize=0x1000):
         with open(fpath, "rb") as afile:
             block = afile.read(blocksize)
             while len(block) > 0:
                 yield block
                 block = afile.read(blocksize)
+    if not op.exists(fpath):
+        return None
     try:
         hasher = hasher or hashlib.md5()
         for block in blockiter(fpath):
             hasher.update(block)
         return (hasher.digest() if asbytes else hasher.hexdigest())
-    except:
-        return None
+    except Exception as ex:
+        return auxly.AuxlyError(ex)
 
 def rootdir():
     """Returns the system root directory."""
     return os.path.abspath(os.sep)
 
 ##==============================================================#
 ## SECTION: Main Body                                           #
 ##==============================================================#
 
 if __name__ == '__main__':
-    pass
+    print(makedirs("foo"))
+    print("OK")
```

### Comparing `auxly-0.8.2/auxly/listy.py` & `auxly-0.9.0/auxly/listy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,71 @@
 ##==============================================================#
+## SECTION: Imports                                             #
+##==============================================================#
+
+import top as auxly
+
+##==============================================================#
 ## SECTION: Function Definitions                                #
 ##==============================================================#
 
-def chunk(l, n):
-    """Yields a generator which groups the given list into successive n-size
-    chunks.
+def chunk(items, size):
+    """Yields a generator which groups the given list items into successive chunks of
+    the given size.
 
     **Attribution**:
     Written by Ned Batchelder and originally posted on
     `Stack Overflow <https://stackoverflow.com/a/312464/789078>`_.
 
     **Examples**:
     ::
         list(auxly.listy.chunk([1,2,3,4,5,6,7,8], 3))
         # [[1, 2, 3], [4, 5, 6], [7, 8]]
     """
-    for i in range(0, len(l), n):
-        yield l[i:i + n]
+    for i in range(0, len(items), size):
+        yield items[i:i + size]
 
-def smooth(l):
-    """Yields a generator which smooths all elements as if the given list
+def smooth(items):
+    """Yields a generator which smooths all items as if the given list
     was of depth 1.
 
     **Examples**:
     ::
         list(auxly.listy.smooth([1,[2,[3,[4]]]]))
         # [1, 2, 3, 4]
     """
-    if type(l) in [list, tuple]:
-        for i in l:
+    if type(items) in [list, tuple]:
+        for i in items:
             for j in smooth(i):
                 yield j
     else:
-        yield l
+        yield items
+
+def isiterable(item):
+    """Returns true if the given item is iterable."""
+    try:
+        [i for i in item]
+        return True
+    except TypeError:
+        return False
+
+def iterate(items):
+    """Iterates over the given items, whether they are iterable or not. Strings
+    are not iterated per character."""
+    if isinstance(items, str) or not isiterable(items):
+        items = [items]
+    for i in items:
+        yield i
+
+def index(items, num):
+    """Returns the item at the given index, otherwise AuxlyError."""
+    try:
+        return items[num]
+    except IndexError as ex:
+        return auxly.AuxlyError(ex)
 
 ##==============================================================#
 ## SECTION: Main Body                                           #
 ##==============================================================#
 
 if __name__ == '__main__':
     pass
```

### Comparing `auxly-0.8.2/auxly/shell.py` & `auxly-0.9.0/auxly/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import os.path as op
 import subprocess
 import sys
 import signal
 import tempfile
 
-import auxly
+import top as auxly
 
 ##==============================================================#
 ## SECTION: Global Definitions                                  #
 ##==============================================================#
 
 #: Null device.
 NULL = open(os.devnull, "w")
```

### Comparing `auxly-0.8.2/auxly/stringy.py` & `auxly-0.9.0/auxly/stringy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ##==============================================================#
 ## SECTION: Imports                                             #
 ##==============================================================#
 
 from random import choice
 from string import ascii_lowercase
+import re
+
+import top as auxly
+from listy import iterate
 
 ##==============================================================#
 ## SECTION: Function Definitions                                #
 ##==============================================================#
 
 def subat(orig, index, replace):
     """Substitutes the replacement string/character at the given index in the
@@ -22,29 +26,51 @@
 def randomize(length=6, choices=None):
     """Returns a random string of the given length."""
     if type(choices) == str:
         choices = list(choices)
     choices = choices or ascii_lowercase
     return "".join(choice(choices) for _ in range(length))
 
-def between(full, start, end):
+def between(orig, start, end):
     """Returns the substring of the given string that occurs between the start
     and end strings."""
     try:
-        if not start:
-            parse = full
-        else:
-            parse = full.split(start, 1)[1]
-        if end:
-            result = parse.split(end, 1)[0]
-        else:
-            result = parse
-        return result
+        parse = orig
+        if start and start in parse:
+            parse = parse.split(start, 1)[1]
+        if end and end in parse:
+            parse = parse.split(end, 1)[0]
+        return parse
+    except:
+        return auxly.AuxlyError()
+
+def remove(orig, subs):
+    """Removes the given substrings from the given string, returns the modified
+    string."""
+    output = orig
+    try:
+        for s in iterate(subs):
+            output = output.replace(s, "")
+        return output
     except:
-        return full
+        return auxly.AuxlyError()
+
+def haspattern(pattern, search):
+    """Returns true if the given text contains the given regex pattern."""
+    try:
+        return re.compile(pattern).search(search) != None
+    except:
+        return auxly.AuxlyError()
+
+def subtract(orig, tosub):
+    """Returns the original string with the given substring removed if it is
+    found at the end, otherwise returns just the original string."""
+    if orig.endswith(tosub):
+        return orig[:-1 * len(tosub)]
+    return orig
 
 ##==============================================================#
 ## SECTION: Main Body                                           #
 ##==============================================================#
 
 if __name__ == '__main__':
     pass
```

### Comparing `auxly-0.8.2/auxly.egg-info/PKG-INFO` & `auxly-0.9.0/auxly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 1.1
 Name: auxly
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python library for common shell-like script tasks.
 Home-page: https://github.com/jeffrimko/Auxly
 Author: Jeff Rimko
 Author-email: jeffrimko@gmail.com
 License: MIT
 Description: |License| |Build Status|
         
+        .. _`_introduction`:
         
         Introduction
         ============
         
         This project provides a Python 2.7/3.x library for common tasks
         especially when writing shell-like scripts. Some of the functionality
         overlaps with the standard library but the API is slightly modified.
@@ -54,49 +55,54 @@
         -  `examples/guess_os.py <https://github.com/jeffrimko/Auxly/blob/master/examples/guess_os.py>`__
            - Attempts to guess the host OS based on available shell commands.
         
         Refer to the unit tests
         `here <https://github.com/jeffrimko/Auxly/tree/master/tests>`__ for
         additional examples.
         
+        .. _`_status`:
         
         Status
         ======
         
         Currently, this project is in the **development release** stage. While
         this project is suitable for use, please note that there may be
         incompatibilities in new releases.
         
         Release notes are maintained in the project
         `changelog <https://github.com/jeffrimko/Auxly/blob/master/CHANGELOG.adoc>`__.
         
+        .. _`_requirements`:
         
         Requirements
         ============
         
         Auxly should run on any Python 2.7/3.x interpreter without additional
         dependencies.
         
+        .. _`_installation`:
         
         Installation
         ============
         
         Auxly can be installed with pip using the following command:
         ``pip install auxly``
         
         Additionally, Auxly can be installed from source by running:
         ``python setup.py install``
         
+        .. _`_documentation`:
         
         Documentation
         =============
         
         The full documentation for this project can be found `here on Read the
         Docs <http://auxly.readthedocs.io>`__.
         
+        .. _`_similar`:
         
         Similar
         =======
         
         The following projects are similar and may be worth checking out:
         
         -  `Reusables <https://github.com/cdgriffith/Reusables>`__
```

### Comparing `auxly-0.8.2/setup.py` & `auxly-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from auxly.filesys import File
 
 setup(
     name = "auxly",
-    version = "0.8.2",
+    version = "0.9.0",
     author = "Jeff Rimko",
     author_email = "jeffrimko@gmail.com",
     description = "Python library for common shell-like script tasks.",
     license = "MIT",
     keywords = "cli script utility library",
     url = "https://github.com/jeffrimko/Auxly",
     packages=["auxly"],
```

