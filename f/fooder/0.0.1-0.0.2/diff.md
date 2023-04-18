# Comparing `tmp/fooder-0.0.1.tar.gz` & `tmp/fooder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fooder-0.0.1.tar", last modified: Sat Apr 15 10:38:08 2023, max compression
+gzip compressed data, was "fooder-0.0.2.tar", last modified: Tue Apr 18 10:08:23 2023, max compression
```

## Comparing `fooder-0.0.1.tar` & `fooder-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-15 10:38:08.312709 fooder-0.0.1/
--rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-15 10:16:11.000000 fooder-0.0.1/LICENSE
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-15 10:38:08.312771 fooder-0.0.1/PKG-INFO
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-15 10:38:08.311579 fooder-0.0.1/fooder.egg-info/
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/PKG-INFO
--rw-r--r--   0 doman      (501) staff       (20)      396 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/SOURCES.txt
--rw-r--r--   0 doman      (501) staff       (20)        1 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/dependency_links.txt
--rw-r--r--   0 doman      (501) staff       (20)       49 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/entry_points.txt
--rw-r--r--   0 doman      (501) staff       (20)       40 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/requires.txt
--rw-r--r--   0 doman      (501) staff       (20)       11 2023-04-15 10:38:08.000000 fooder-0.0.1/fooder.egg-info/top_level.txt
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-15 10:38:08.312578 fooder-0.0.1/fooder_cli/
--rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-03 12:14:34.000000 fooder-0.0.1/fooder_cli/__init__.py
--rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-15 10:36:08.000000 fooder-0.0.1/fooder_cli/__main__.py
--rw-r--r--   0 doman      (501) staff       (20)    11822 2023-04-10 09:32:01.000000 fooder-0.0.1/fooder_cli/client.py
--rw-r--r--   0 doman      (501) staff       (20)     1872 2023-04-10 09:12:23.000000 fooder-0.0.1/fooder_cli/diary.py
--rw-r--r--   0 doman      (501) staff       (20)      882 2023-04-15 10:19:46.000000 fooder-0.0.1/fooder_cli/entry.py
--rw-r--r--   0 doman      (501) staff       (20)     2992 2023-04-15 10:38:06.000000 fooder-0.0.1/fooder_cli/main.py
--rw-r--r--   0 doman      (501) staff       (20)      912 2023-04-10 08:59:36.000000 fooder-0.0.1/fooder_cli/meal.py
--rw-r--r--   0 doman      (501) staff       (20)      304 2023-04-03 13:10:19.000000 fooder-0.0.1/fooder_cli/parser.py
--rw-r--r--   0 doman      (501) staff       (20)     2812 2023-04-03 15:02:33.000000 fooder-0.0.1/fooder_cli/product.py
--rw-r--r--   0 doman      (501) staff       (20)      100 2023-04-15 10:38:08.312964 fooder-0.0.1/setup.cfg
--rw-r--r--   0 doman      (501) staff       (20)      973 2023-04-15 10:37:19.000000 fooder-0.0.1/setup.py
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.731690 fooder-0.0.2/
+-rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-17 21:36:03.000000 fooder-0.0.2/LICENSE
+-rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-18 10:08:23.731737 fooder-0.0.2/PKG-INFO
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.730249 fooder-0.0.2/fooder.egg-info/
+-rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/PKG-INFO
+-rw-r--r--   0 doman      (501) staff       (20)      375 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/SOURCES.txt
+-rw-r--r--   0 doman      (501) staff       (20)        1 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/dependency_links.txt
+-rw-r--r--   0 doman      (501) staff       (20)       49 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/entry_points.txt
+-rw-r--r--   0 doman      (501) staff       (20)       40 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/requires.txt
+-rw-r--r--   0 doman      (501) staff       (20)       11 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/top_level.txt
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.731463 fooder-0.0.2/fooder_cli/
+-rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/__init__.py
+-rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/__main__.py
+-rw-r--r--   0 doman      (501) staff       (20)     9704 2023-04-18 10:04:23.000000 fooder-0.0.2/fooder_cli/client.py
+-rw-r--r--   0 doman      (501) staff       (20)     1626 2023-04-18 10:06:34.000000 fooder-0.0.2/fooder_cli/diary.py
+-rw-r--r--   0 doman      (501) staff       (20)      675 2023-04-18 10:04:11.000000 fooder-0.0.2/fooder_cli/entry.py
+-rw-r--r--   0 doman      (501) staff       (20)     2992 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/main.py
+-rw-r--r--   0 doman      (501) staff       (20)      719 2023-04-18 10:04:56.000000 fooder-0.0.2/fooder_cli/meal.py
+-rw-r--r--   0 doman      (501) staff       (20)     2717 2023-04-18 10:05:40.000000 fooder-0.0.2/fooder_cli/product.py
+-rw-r--r--   0 doman      (501) staff       (20)      100 2023-04-18 10:08:23.731930 fooder-0.0.2/setup.cfg
+-rw-r--r--   0 doman      (501) staff       (20)      973 2023-04-18 10:07:57.000000 fooder-0.0.2/setup.py
```

### Comparing `fooder-0.0.1/LICENSE` & `fooder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fooder-0.0.1/PKG-INFO` & `fooder-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fooder-0.0.1/fooder.egg-info/PKG-INFO` & `fooder-0.0.2/fooder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fooder-0.0.1/fooder_cli/client.py` & `fooder-0.0.2/fooder_cli/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import requests
 import os
 from datetime import date
 from typing import Optional, Dict
-import json
-from getpass import getpass
 from pydantic import validate_arguments
 from pathlib import Path
 
 
 class UnathorizedError(Exception):
     pass
 
@@ -351,89 +349,7 @@
     @validate_arguments
     def delete_entry(
         self,
         entry: int,
     ) -> None:
         """delete_entry."""
         self.delete(f"/entry/{entry}")
-
-
-def get_client() -> FooderClient:
-    client = FooderClient()
-    return client
-
-
-def pprint(response: str) -> None:
-    print(json.dumps(response, indent=2))
-
-
-if __name__ == "__main__":
-    from argparse import ArgumentParser
-
-    parser = ArgumentParser()
-    parser.add_argument("ARGS", nargs="*")
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument("-l", "--login", action="store_true", help="login to fooder")
-    group.add_argument(
-        "-p",
-        "--products",
-        action="store_true",
-        help="list products with params: q limit offset",
-    )
-    group.add_argument(
-        "-a",
-        "--add-product",
-        action="store_true",
-        help="add product with params: name protein carb fat",
-    )
-    group.add_argument(
-        "-d", "--diary", action="store_true", help="get diary with params: date"
-    )
-    group.add_argument(
-        "-e",
-        "--entry",
-        action="store_true",
-        help="create entry with params: product quantity meal",
-    )
-    group.add_argument(
-        "--delete-entry", action="store_true", help="delete entry with param: entry"
-    )
-    group.add_argument(
-        "--edit-entry",
-        action="store_true",
-        help="edit entry with params: entry grams product meal",
-    )
-    group.add_argument(
-        "-m",
-        "--meal",
-        action="store_true",
-        help="create meal with params: diary name order",
-    )
-    args = parser.parse_args()
-
-    c = FooderClient()
-
-    if args.login:
-        username = input("Username: ")
-        password = getpass("Password: ")
-        c.login(username, password)
-
-    if args.products:
-        pprint(c.list_products(*args.ARGS))
-
-    if args.add_product:
-        pprint(c.create_product(*args.ARGS))
-
-    if args.diary:
-        pprint(c.get_diary(*args.ARGS))
-
-    if args.entry:
-        pprint(c.add_entry(*args.ARGS))
-
-    if args.delete_entry:
-        pprint(c.delete_entry(*args.ARGS))
-
-    if args.edit_entry:
-        pprint(c.edit_entry(*args.ARGS))
-
-    if args.meal:
-        pprint(c.create_meal(*args.ARGS))
```

### Comparing `fooder-0.0.1/fooder_cli/main.py` & `fooder-0.0.2/fooder_cli/main.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.1/fooder_cli/product.py` & `fooder-0.0.2/fooder_cli/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,13 +83,7 @@
         protein=protein,
         carb=carb,
         fat=fat,
     )
 
     console.print(Text("Product added", style="bold green"))
     return product
-
-
-if __name__ == "__main__":
-    from .client import get_client
-
-    add_product(get_client())
```

### Comparing `fooder-0.0.1/setup.py` & `fooder-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 
 setup(
     name="fooder",
-    version="0.0.1",
+    version="0.0.2",
     author="Piotr Domanski",
     author_email="pi.domanski@gmail.com",
     description="Minimalistic cli diary for tracking calories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ickyicky/fooder-cli-client",
     classifiers=[
```

