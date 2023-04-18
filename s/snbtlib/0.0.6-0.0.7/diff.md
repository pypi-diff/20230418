# Comparing `tmp/snbtlib-0.0.6.tar.gz` & `tmp/snbtlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snbtlib-0.0.6.tar", last modified: Thu Mar  9 05:59:03 2023, max compression
+gzip compressed data, was "snbtlib-0.0.7.tar", last modified: Tue Apr 18 02:15:02 2023, max compression
```

## Comparing `snbtlib-0.0.6.tar` & `snbtlib-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 05:59:03.878266 snbtlib-0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      716 2023-03-09 05:59:03.878266 snbtlib-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-03-09 05:59:03.878266 snbtlib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-03-09 05:56:33.000000 snbtlib-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 05:59:03.875266 snbtlib-0.0.6/snbtlib/
--rw-rw-rw-   0        0        0       44 2022-05-03 16:43:47.000000 snbtlib-0.0.6/snbtlib/__init__.py
--rw-rw-rw-   0        0        0     6681 2023-03-09 05:54:31.000000 snbtlib-0.0.6/snbtlib/formatter.py
-drwxrwxrwx   0        0        0        0 2023-03-09 05:59:03.877266 snbtlib-0.0.6/snbtlib.egg-info/
--rw-rw-rw-   0        0        0      716 2023-03-09 05:59:03.000000 snbtlib-0.0.6/snbtlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-03-09 05:59:03.000000 snbtlib-0.0.6/snbtlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 05:59:03.000000 snbtlib-0.0.6/snbtlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-09 05:59:03.000000 snbtlib-0.0.6/snbtlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 05:59:03.878266 snbtlib-0.0.6/test/
--rw-rw-rw-   0        0        0      207 2023-03-09 05:52:36.000000 snbtlib-0.0.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.762783 snbtlib-0.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-04-18 02:15:02.762783 snbtlib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:15:02.763784 snbtlib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-04-18 02:13:31.000000 snbtlib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.758783 snbtlib-0.0.7/snbtlib/
+-rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-0.0.7/snbtlib/__init__.py
+-rw-rw-rw-   0        0        0     6952 2023-04-18 02:12:47.000000 snbtlib-0.0.7/snbtlib/formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.761783 snbtlib-0.0.7/snbtlib.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 02:15:02.000000 snbtlib-0.0.7/snbtlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 02:15:02.761783 snbtlib-0.0.7/test/
+-rw-rw-rw-   0        0        0      190 2023-03-15 08:59:09.000000 snbtlib-0.0.7/test/test.py
```

### Comparing `snbtlib-0.0.6/LICENSE` & `snbtlib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snbtlib-0.0.6/PKG-INFO` & `snbtlib-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

### Comparing `snbtlib-0.0.6/setup.py` & `snbtlib-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='snbtlib',
-    version='0.0.6',
+    version='0.0.7',
     keywords='minecraft',
     description='a formatter for snbt from minecraft',
     long_description=long_description,
     license='MIT License',
     url='',
     author='Tryanks',
     author_email='tryanks@outlook.com',
```

### Comparing `snbtlib-0.0.6/snbtlib/formatter.py` & `snbtlib-0.0.7/snbtlib/formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     return token_list
 
 
 def NumberBuilder(r):
     s = StringIO()
     s.write(r.get_point())
     while i := r.next():
-        if i in ',\n' or i.isspace():
+        if i in '},\n' or i.isspace():
             r.last()
             break
         s.write(i)
     return '$number$' + s.getvalue()
 
 
 def StringBuilder(r):
@@ -229,17 +229,23 @@
                 s += r.snext()
                 continue
             elif i == '"':
                 if r.snext() == ':':
                     s = f'"{s}"'
                     break
                 else:
-                    r.last()
-                    token.type = Token.STRING
-                    break
+                    if not r.get_point().isspace() and not r.get_point() in ',]}':
+                        r.last()
+                        s += '\\'
+                        s += r.get_point()
+                        continue
+                    else:
+                        r.last()
+                        token.type = Token.STRING
+                        break
         if i == ':' and not stringStatus:
             break
         s += i
         if s in ('true', 'false'):
             token.type = Token.BOOL
             s = True if s == 'true' else False
             break
```

### Comparing `snbtlib-0.0.6/snbtlib.egg-info/PKG-INFO` & `snbtlib-0.0.7/snbtlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

