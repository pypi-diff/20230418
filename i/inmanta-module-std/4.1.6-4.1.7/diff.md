# Comparing `tmp/inmanta_module_std-4.1.6-py3-none-any.whl.zip` & `tmp/inmanta_module_std-4.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21107 bytes, number of entries: 9
--rw-rw-r--  2.0 unx    31585 b- defN 23-Apr-04 12:39 inmanta_plugins/std/__init__.py
--rw-rw-r--  2.0 unx    21719 b- defN 23-Apr-04 12:39 inmanta_plugins/std/resources.py
--rw-rw-r--  2.0 unx      881 b- defN 23-Apr-04 12:39 inmanta_plugins/std/setup.cfg
--rw-rw-r--  2.0 unx    18184 b- defN 23-Apr-04 12:39 inmanta_plugins/std/model/_init.cf
--rw-rw-r--  2.0 unx     1173 b- defN 23-Apr-04 12:39 inmanta_plugins/std/model/testing.cf
--rw-rw-r--  2.0 unx      245 b- defN 23-Apr-04 12:39 inmanta_module_std-4.1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 12:39 inmanta_module_std-4.1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Apr-04 12:39 inmanta_module_std-4.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      790 b- defN 23-Apr-04 12:39 inmanta_module_std-4.1.6.dist-info/RECORD
-9 files, 74685 bytes uncompressed, 19733 bytes compressed:  73.6%
+Zip file size: 21066 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx    31585 b- defN 23-Apr-18 10:12 inmanta_plugins/std/__init__.py
+-rw-rw-r--  2.0 unx    21719 b- defN 23-Apr-18 10:12 inmanta_plugins/std/resources.py
+-rw-rw-r--  2.0 unx      851 b- defN 23-Apr-18 10:12 inmanta_plugins/std/setup.cfg
+-rw-rw-r--  2.0 unx    18184 b- defN 23-Apr-18 10:12 inmanta_plugins/std/model/_init.cf
+-rw-rw-r--  2.0 unx     1173 b- defN 23-Apr-18 10:12 inmanta_plugins/std/model/testing.cf
+-rw-rw-r--  2.0 unx      194 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      790 b- defN 23-Apr-18 10:12 inmanta_module_std-4.1.7.dist-info/RECORD
+9 files, 74604 bytes uncompressed, 19692 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: inmanta_plugins/std/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/std/model/testing.cf
 Comment: 
 
-Filename: inmanta_module_std-4.1.6.dist-info/METADATA
+Filename: inmanta_module_std-4.1.7.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_std-4.1.6.dist-info/WHEEL
+Filename: inmanta_module_std-4.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_std-4.1.6.dist-info/top_level.txt
+Filename: inmanta_module_std-4.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_std-4.1.6.dist-info/RECORD
+Filename: inmanta_module_std-4.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/std/setup.cfg

```diff
@@ -23,23 +23,22 @@
 [irt]
 skip_tests = False
 
 [metadata]
 name = inmanta-module-std
 freeze_recursive = False
 freeze_operator = ~=
-version = 4.1.6
+version = 4.1.7
 license = Apache 2.0
 version_tag = 
 
 [options]
-install_requires = Jinja2~=3.1
-	email_validator~=1.3
-	pydantic~=1.10
-	dataclasses~=0.7;python_version<'3.7'
+install_requires = Jinja2>=3.1,<4
+	email_validator>=1.3,<3
+	pydantic>=1.10,<2
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
 
 [options.packages.find]
 include = inmanta_plugins*
```

