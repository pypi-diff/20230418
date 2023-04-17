# Comparing `tmp/unexpected_isaves-2.1.1.tar.gz` & `tmp/unexpected_isaves-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unexpected_isaves-2.1.1.tar", last modified: Tue Apr  4 20:26:25 2023, max compression
+gzip compressed data, was "unexpected_isaves-2.1.2.tar", last modified: Mon Apr 17 22:15:15 2023, max compression
```

## Comparing `unexpected_isaves-2.1.1.tar` & `unexpected_isaves-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:26:25.052474 unexpected_isaves-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-04 20:26:25.052474 unexpected_isaves-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 20:26:25.052474 unexpected_isaves-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:26:25.048473 unexpected_isaves-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:26:25.052474 unexpected_isaves-2.1.1/src/unexpected_isaves/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/src/unexpected_isaves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24265 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/src/unexpected_isaves/blocks.json
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-04-04 20:26:09.000000 unexpected_isaves-2.1.1/src/unexpected_isaves/save_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:26:25.052474 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-04 20:26:25.000000 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-04 20:26:25.000000 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:26:25.000000 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 20:26:25.000000 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 20:26:25.000000 unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/unexpected_isaves/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/top_level.txt
```

### Comparing `unexpected_isaves-2.1.1/LICENSE` & `unexpected_isaves-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unexpected_isaves-2.1.1/PKG-INFO` & `unexpected_isaves-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unexpected_isaves
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it.
-Author-email: Eric Mendes <ericvelasco.2000@gmail.com>
+Author-email: Eric Mendes <ericvelasco.2000@gmail.com>, Henrique Souza <henriquesoliveira05@gmail.com>
 Maintainer-email: Eric Mendes <ericvelasco.2000@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Eric Mendes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: unexpected_isaves Version: 2.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: unexpected_isaves Version: 2.1.2 Summary: A Python
 library that paints an image on a spreadsheet, builds its pixel art in
 Minecraft, makes its ascii art, or makes a rubik's cube art out of it. Author-
 email: Eric Mendes
-2000@gmail.com> Maintainer-email: Eric Mendes
+2000@gmail.com>, Henrique Souza
+gmail.com> Maintainer-email: Eric Mendes
 2000@gmail.com> License: MIT License Copyright (c) 2022 Eric Mendes Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `unexpected_isaves-2.1.1/README.md` & `unexpected_isaves-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unexpected_isaves-2.1.1/pyproject.toml` & `unexpected_isaves-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "unexpected_isaves"
-version = "2.1.1"
+version = "2.1.2"
 description = "A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["minecraft", "pixel", "art", "excel", "spreadsheet", "ascii", "rubiks"]
 authors = [
-  {name = "Eric Mendes", email = "ericvelasco.2000@gmail.com" }
+  {name = "Eric Mendes", email = "ericvelasco.2000@gmail.com" },
+  {name = "Henrique Souza", email = "henriquesoliveira05@gmail.com" }
 ]
 maintainers = [
   {name = "Eric Mendes", email = "ericvelasco.2000@gmail.com" }
 ]
 classifiers = [  
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Other Audience",
```

### Comparing `unexpected_isaves-2.1.1/src/unexpected_isaves/blocks.json` & `unexpected_isaves-2.1.2/src/unexpected_isaves/blocks.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9262295081967213%*

 * *Differences: {'31': "{'blocks': ['lapis_lazuli_block']}",*

 * * '32': "{'blocks': ['emerald_block']}",*

 * * '36': "{'blocks': ['orange_terracotta']}",*

 * * '37': "{'blocks': ['magenta_terracotta']}",*

 * * '38': "{'blocks': ['light_blue_terracotta']}",*

 * * '39': "{'blocks': ['yellow_terracotta']}",*

 * * '40': "{'blocks': ['lime_terracotta']}",*

 * * '41': "{'blocks': ['pink_terracotta']}",*

 * * '44': "{'blocks': ['cyan_terracotta']}",*

 * * '46': "{'blocks': ['blue_terracotta']}",*

 * * '48': "{'blocks': ['green_terracotta']}",*

 * * '49': "{'blocks': ['red_terracotta […]*

```diff
@@ -753,23 +753,27 @@
         "rgb": [
             92,
             219,
             213
         ]
     },
     {
-        "blocks": "lapis_lazuli_block",
+        "blocks": [
+            "lapis_lazuli_block"
+        ],
         "rgb": [
             74,
             128,
             255
         ]
     },
     {
-        "blocks": "emerald_block",
+        "blocks": [
+            "emerald_block"
+        ],
         "rgb": [
             0,
             217,
             58
         ]
     },
     {
@@ -832,55 +836,67 @@
         "rgb": [
             209,
             177,
             161
         ]
     },
     {
-        "blocks": "orange_terracotta",
+        "blocks": [
+            "orange_terracotta"
+        ],
         "rgb": [
             159,
             82,
             36
         ]
     },
     {
-        "blocks": "magenta_terracotta",
+        "blocks": [
+            "magenta_terracotta"
+        ],
         "rgb": [
             149,
             87,
             108
         ]
     },
     {
-        "blocks": "light_blue_terracotta",
+        "blocks": [
+            "light_blue_terracotta"
+        ],
         "rgb": [
             112,
             108,
             138
         ]
     },
     {
-        "blocks": "yellow_terracotta",
+        "blocks": [
+            "yellow_terracotta"
+        ],
         "rgb": [
             186,
             133,
             36
         ]
     },
     {
-        "blocks": "lime_terracotta",
+        "blocks": [
+            "lime_terracotta"
+        ],
         "rgb": [
             103,
             117,
             53
         ]
     },
     {
-        "blocks": "pink_terracotta",
+        "blocks": [
+            "pink_terracotta"
+        ],
         "rgb": [
             160,
             77,
             78
         ]
     },
     {
@@ -902,15 +918,17 @@
         "rgb": [
             135,
             107,
             98
         ]
     },
     {
-        "blocks": "cyan_terracotta",
+        "blocks": [
+            "cyan_terracotta"
+        ],
         "rgb": [
             87,
             92,
             92
         ]
     },
     {
@@ -921,15 +939,17 @@
         "rgb": [
             122,
             73,
             88
         ]
     },
     {
-        "blocks": "blue_terracotta",
+        "blocks": [
+            "blue_terracotta"
+        ],
         "rgb": [
             76,
             62,
             92
         ]
     },
     {
@@ -941,39 +961,47 @@
         "rgb": [
             76,
             50,
             35
         ]
     },
     {
-        "blocks": "green_terracotta",
+        "blocks": [
+            "green_terracotta"
+        ],
         "rgb": [
             76,
             82,
             42
         ]
     },
     {
-        "blocks": "red_terracotta",
+        "blocks": [
+            "red_terracotta"
+        ],
         "rgb": [
             142,
             60,
             46
         ]
     },
     {
-        "blocks": "black_terracotta",
+        "blocks": [
+            "black_terracotta"
+        ],
         "rgb": [
             37,
             22,
             16
         ]
     },
     {
-        "blocks": "crimson_nylium",
+        "blocks": [
+            "crimson_nylium"
+        ],
         "rgb": [
             189,
             48,
             49
         ]
     },
     {
@@ -1051,39 +1079,47 @@
         "rgb": [
             86,
             44,
             62
         ]
     },
     {
-        "blocks": "warped_wart_block",
+        "blocks": [
+            "warped_wart_block"
+        ],
         "rgb": [
             20,
             180,
             133
         ]
     },
     {
-        "blocks": "deepslate",
+        "blocks": [
+            "deepslate"
+        ],
         "rgb": [
             100,
             100,
             100
         ]
     },
     {
-        "blocks": "raw_iron_block",
+        "blocks": [
+            "raw_iron_block"
+        ],
         "rgb": [
             216,
             175,
             147
         ]
     },
     {
-        "blocks": "glow_lichen",
+        "blocks": [
+            "glow_lichen"
+        ],
         "rgb": [
             127,
             167,
             150
         ]
     }
 ]
```

### Comparing `unexpected_isaves-2.1.1/src/unexpected_isaves/save_image.py` & `unexpected_isaves-2.1.2/src/unexpected_isaves/save_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,28 +106,32 @@
     res: List[str],
     path: str,
     minecraft_version: str = "1.18.2",
 ) -> None:
     # Getting the name that the image should have via the given path
     image_name = os.path.splitext(os.path.split(path)[1])[0]
 
+    # Minecraft version to data pack version relation can be found at https://minecraft.fandom.com/wiki/Data_pack.
+    # Feel free to help us keep updated by contributing.
     if minecraft_version >= "1.13.0" and minecraft_version <= "1.14.4":
         datapack_version = 4
     elif minecraft_version >= "1.15.0" and minecraft_version <= "1.16.1":
         datapack_version = 5
     elif minecraft_version >= "1.16.2" and minecraft_version <= "1.16.5":
         datapack_version = 6
     elif minecraft_version >= "1.17.0" and minecraft_version <= "1.17.1":
         datapack_version = 7
     elif minecraft_version >= "1.18.0" and minecraft_version <= "1.18.1":
         datapack_version = 8
     elif minecraft_version == "1.18.2":
         datapack_version = 9
-    elif minecraft_version == "1.19.0":
+    elif minecraft_version >= "1.19.0" and minecraft_version <= "1.19.3":
         datapack_version = 10
+    elif minecraft_version == "1.19.4":
+        datapack_version = 12
     else:
         raise ValueError(
             "Unsupported minecraft_version. If you feel like this is a mistake, open an issue at https://github.com/Eric-Mendes/unexpected-isaves/issues to let us know."
         )
 
     pack_mcmeta = {
         "pack": {
```

### Comparing `unexpected_isaves-2.1.1/src/unexpected_isaves.egg-info/PKG-INFO` & `unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: unexpected-isaves
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it.
-Author-email: Eric Mendes <ericvelasco.2000@gmail.com>
+Author-email: Eric Mendes <ericvelasco.2000@gmail.com>, Henrique Souza <henriquesoliveira05@gmail.com>
 Maintainer-email: Eric Mendes <ericvelasco.2000@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Eric Mendes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: unexpected-isaves Version: 2.1.1 Summary: A Python
+Metadata-Version: 2.1 Name: unexpected-isaves Version: 2.1.2 Summary: A Python
 library that paints an image on a spreadsheet, builds its pixel art in
 Minecraft, makes its ascii art, or makes a rubik's cube art out of it. Author-
 email: Eric Mendes
-2000@gmail.com> Maintainer-email: Eric Mendes
+2000@gmail.com>, Henrique Souza
+gmail.com> Maintainer-email: Eric Mendes
 2000@gmail.com> License: MIT License Copyright (c) 2022 Eric Mendes Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

