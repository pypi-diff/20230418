# Comparing `tmp/security-util-0.0.1.tar.gz` & `tmp/security-util-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security-util-0.0.1.tar", last modified: Tue Apr 18 12:59:40 2023, max compression
+gzip compressed data, was "security-util-0.0.2.tar", last modified: Tue Apr 18 14:11:06 2023, max compression
```

## Comparing `security-util-0.0.1.tar` & `security-util-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:59:40.753874 security-util-0.0.1/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      144 2023-04-18 12:59:40.753637 security-util-0.0.1/PKG-INFO
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:47:24.000000 security-util-0.0.1/README.md
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      358 2023-04-18 12:48:52.000000 security-util-0.0.1/pyproject.toml
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:59:40.750664 security-util-0.0.1/security_util/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       50 2023-04-18 12:50:34.000000 security-util-0.0.1/security_util/__init__.py
-drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:59:40.753194 security-util-0.0.1/security_util.egg-info/
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      144 2023-04-18 12:59:40.000000 security-util-0.0.1/security_util.egg-info/PKG-INFO
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      243 2023-04-18 12:59:40.000000 security-util-0.0.1/security_util.egg-info/SOURCES.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-04-18 12:59:40.000000 security-util-0.0.1/security_util.egg-info/dependency_links.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-04-18 12:57:13.000000 security-util-0.0.1/security_util.egg-info/not-zip-safe
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       14 2023-04-18 12:59:40.000000 security-util-0.0.1/security_util.egg-info/top_level.txt
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       38 2023-04-18 12:59:40.753926 security-util-0.0.1/setup.cfg
--rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)     1381 2023-04-18 12:57:34.000000 security-util-0.0.1/setup.py
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 14:11:06.463746 security-util-0.0.2/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      194 2023-04-18 14:11:06.463849 security-util-0.0.2/PKG-INFO
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:47:24.000000 security-util-0.0.2/README.md
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      354 2023-04-18 14:02:10.000000 security-util-0.0.2/pyproject.toml
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 14:11:06.460245 security-util-0.0.2/security_util/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       50 2023-04-18 12:50:34.000000 security-util-0.0.2/security_util/__init__.py
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 14:11:06.462606 security-util-0.0.2/security_util.egg-info/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      194 2023-04-18 14:11:06.000000 security-util-0.0.2/security_util.egg-info/PKG-INFO
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      267 2023-04-18 14:11:06.000000 security-util-0.0.2/security_util.egg-info/SOURCES.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-04-18 14:11:06.000000 security-util-0.0.2/security_util.egg-info/dependency_links.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)       20 2023-04-18 14:11:06.000000 security-util-0.0.2/security_util.egg-info/top_level.txt
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        1 2023-04-18 14:05:11.000000 security-util-0.0.2/security_util.egg-info/zip-safe
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)      276 2023-04-18 14:11:06.464249 security-util-0.0.2/setup.cfg
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)     1381 2023-04-18 14:10:00.000000 security-util-0.0.2/setup.py
+drwxr-xr-x   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 14:11:06.463319 security-util-0.0.2/tests/
+-rw-r--r--   0 Zakhar.Fedotkin   (502) staff       (20)        0 2023-04-18 12:47:24.000000 security-util-0.0.2/tests/__init__.py
```

### Comparing `security-util-0.0.1/setup.py` & `security-util-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
             pass
 
         
 
 
 
 setup(name='security-util',
-      version='0.0.1',
+      version='0.0.2',
       description='Security util for python',
       author='Battle Furry <btlfry@gmail.com>',
       license='MIT',
       zip_safe=False,
       cmdclass={'install': CustomInstall})
```

