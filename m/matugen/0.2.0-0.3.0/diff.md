# Comparing `tmp/matugen-0.2.0.tar.gz` & `tmp/matugen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matugen-0.2.0.tar", max compression
+gzip compressed data, was "matugen-0.3.0.tar", max compression
```

## Comparing `matugen-0.2.0.tar` & `matugen-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1362 2023-04-16 15:23:06.646495 matugen-0.2.0/README.md
--rw-r--r--   0        0        0      534 2023-04-16 15:34:23.460991 matugen-0.2.0/matugen/__main__.py
--rw-r--r--   0        0        0     5262 2023-04-16 15:33:58.799250 matugen-0.2.0/matugen/util.py
--rw-r--r--   0        0        0      375 2023-04-16 18:12:49.066705 matugen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 matugen-0.2.0/setup.py
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 matugen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1615 2023-04-17 19:24:00.227213 matugen-0.3.0/README.md
+-rw-r--r--   0        0        0      437 2023-04-17 19:08:30.540135 matugen-0.3.0/matugen/__main__.py
+-rw-r--r--   0        0        0     5623 2023-04-17 19:08:25.961097 matugen-0.3.0/matugen/util.py
+-rw-r--r--   0        0        0      375 2023-04-17 19:28:58.050912 matugen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 matugen-0.3.0/setup.py
+-rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 matugen-0.3.0/PKG-INFO
```

### Comparing `matugen-0.2.0/README.md` & `matugen-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,22 +15,40 @@
     <a href="https://github.com/InioX/matugen/wiki">Wiki</a>
 </div>
 
 ## Description
 [Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.
 
 ## Installation
-Assuming you already have [Poetry](https://python-poetry.org/) installed:
+### From Pypi
+>**Note** Assuming you have python with pip installed
+```shell
+pip install matugen
+```
+
+### Usage
+```shell
+# Dark theme
+matugen /path/to/wallpaper/
+# Light theme
+matugen /path/to/wallpaper/ -l
+```
+Example:
+```shell
+matugen ~/wall/snow.png -l
+```
+
+### From repo with poetry
+>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:
 ```shell
 git clone https://github.com/InioX/matugen && cd matugen
 poetry install
 ```
 
-## Usage
-Assuming you are in the root of this project:
+#### Usage
 ```shell
 # Dark theme
 poetry run matugen /path/to/wallpaper/
 # Light theme
 poetry run matugen /path/to/wallpaper/ -l
 ```
 Example:
```

#### html2text {}

```diff
@@ -2,16 +2,19 @@
                           4fe9-9ee5-a1a1395d70dc.png]
                              ****** Matugen ******
                 A material you color generation tool for linux
                          Installation Â· Usage Â· Wiki
 ## Description [Material Design 3](https://m3.material.io/) offers a new color
 system that allows for more flexible and dynamic use of color. The new system
 includes a wider range of colors, as well as a range of tints and shades that
-can be used to create subtle variations in color. ## Installation Assuming you
-already have [Poetry](https://python-poetry.org/) installed: ```shell git clone
-https://github.com/InioX/matugen && cd matugen poetry install ``` ## Usage
-Assuming you are in the root of this project: ```shell # Dark theme poetry run
-matugen /path/to/wallpaper/ # Light theme poetry run matugen /path/to/
-wallpaper/ -l ``` Example: ```shell poetry run matugen ~/wall/snow.png -l ```
-## Showcase Showcase with Hyprland, Waybar, kitty, and fish shell: >**Warning**
->The preview and usage may be outdated. [![](https://markdown-videos.deta.dev/
-youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)
+can be used to create subtle variations in color. ## Installation ### From Pypi
+>**Note** Assuming you have python with pip installed ```shell pip install
+matugen ``` ### Usage ```shell # Dark theme matugen /path/to/wallpaper/ # Light
+theme matugen /path/to/wallpaper/ -l ``` Example: ```shell matugen ~/wall/
+snow.png -l ``` ### From repo with poetry >**Note** Assuming you already have
+[Poetry](https://python-poetry.org/) installed: ```shell git clone https://
+github.com/InioX/matugen && cd matugen poetry install ``` #### Usage ```shell #
+Dark theme poetry run matugen /path/to/wallpaper/ # Light theme poetry run
+matugen /path/to/wallpaper/ -l ``` Example: ```shell poetry run matugen ~/wall/
+snow.png -l ``` ## Showcase Showcase with Hyprland, Waybar, kitty, and fish
+shell: >**Warning** >The preview and usage may be outdated. [![](https://
+markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)
```

### Comparing `matugen-0.2.0/matugen/util.py` & `matugen-0.3.0/matugen/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 import os
 import re
 import logging
 import pathlib
+import importlib.metadata
 from material_color_utilities_python import Image, themeFromImage
 from rich.logging import RichHandler
 from configparser import ConfigParser
 from argparse import Namespace, ArgumentParser
 from pathlib import Path
 
 
+def get_version() -> str:
+    return importlib.metadata.version('matugen')
+
+
+def get_scheme(args):
+    scheme = Scheme(Theme.get(args.wallpaper), args.lightmode)
+    return scheme.to_hex()
+
+
 def parse_arguments():
     parser = ArgumentParser()
 
     parser.add_argument(
         "wallpaper",
         help="the wallpaper that will be used",
         type=str
     )
 
     parser.add_argument(
         "-l", "--lightmode",
         help="specify whether to use light mode",
         action="store_true"
     )
+    parser.add_argument(
+        "--version",
+        help="outputs the version",
+        action="version",
+        version=get_version()
+    )
     args: Namespace = parser.parse_args()
     return args
 
 
 def setup_logging():
     FORMAT = "%(message)s"
     logging.basicConfig(
```

### Comparing `matugen-0.2.0/setup.py` & `matugen-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['material-color-utilities-python==0.1.5', 'rich>=12.5.1,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['matugen = matugen.__main__:main']}
 
 setup_kwargs = {
     'name': 'matugen',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
-    'long_description': '<div align="center">\n     <img src="https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-4fe9-9ee5-a1a1395d70dc.png" width=140>\n      <h1>Matugen</h1>\n </div>\n    \n<div align="center">\n  <b>A material you color generation tool for linux</b>\n</div>\n\n<div align="center">\n    <a href="#installation">Installation</a>\n    ·\n    <a href="#usage">Usage</a>\n    ·\n    <a href="https://github.com/InioX/matugen/wiki">Wiki</a>\n</div>\n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.\n\n## Installation\nAssuming you already have [Poetry](https://python-poetry.org/) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd matugen\npoetry install\n```\n\n## Usage\nAssuming you are in the root of this project:\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n',
+    'long_description': '<div align="center">\n     <img src="https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-4fe9-9ee5-a1a1395d70dc.png" width=140>\n      <h1>Matugen</h1>\n </div>\n    \n<div align="center">\n  <b>A material you color generation tool for linux</b>\n</div>\n\n<div align="center">\n    <a href="#installation">Installation</a>\n    ·\n    <a href="#usage">Usage</a>\n    ·\n    <a href="https://github.com/InioX/matugen/wiki">Wiki</a>\n</div>\n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.\n\n## Installation\n### From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\nmatugen ~/wall/snow.png -l\n```\n\n### From repo with poetry\n>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd matugen\npoetry install\n```\n\n#### Usage\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n',
     'author': 'InioX',
     'author_email': 'justimnix@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,31 +1,34 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['matugen']
 package_data = \ {'': ['*']} install_requires = \ ['material-color-utilities-
 python==0.1.5', 'rich>=12.5.1,<13.0.0'] entry_points = \ {'console_scripts':
 ['matugen = matugen.__main__:main']} setup_kwargs = { 'name': 'matugen',
-'version': '0.2.0', 'description': '', 'long_description': '
+'version': '0.3.0', 'description': '', 'long_description': '
 \n [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                          4fe9-9ee5-a1a1395d70dc.png]\n
                              ****** Matugen ******
                                       \n
 \n \n
               \n A material you color generation tool for linux\n
 \n\n
                   \n Installation\n Â·\n Usage\n Â·\n Wiki\n
 \n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new
 color system that allows for more flexible and dynamic use of color. The new
 system includes a wider range of colors, as well as a range of tints and shades
-that can be used to create subtle variations in color.\n\n##
-Installation\nAssuming you already have [Poetry](https://python-poetry.org/
+that can be used to create subtle variations in color.\n\n## Installation\n###
+From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip
+install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/
+wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:
+\n```shell\nmatugen ~/wall/snow.png -l\n```\n\n### From repo with
+poetry\n>**Note** Assuming you already have [Poetry](https://python-poetry.org/
 ) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd
-matugen\npoetry install\n```\n\n## Usage\nAssuming you are in the root of this
-project:\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n#
-Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:
-\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase
-with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and
-usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/
-rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n', 'author': 'InioX',
-'author_email': 'justimnix@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
+matugen\npoetry install\n```\n\n#### Usage\n```shell\n# Dark theme\npoetry run
+matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/
+wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -
+l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:
+\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://
+markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/
+rMxoORO41rs)\n', 'author': 'InioX', 'author_email': 'justimnix@gmail.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
 'entry_points': entry_points, 'python_requires': '>=3.10,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `matugen-0.2.0/PKG-INFO` & `matugen-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matugen
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: InioX
 Author-email: justimnix@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,22 +29,40 @@
     <a href="https://github.com/InioX/matugen/wiki">Wiki</a>
 </div>
 
 ## Description
 [Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.
 
 ## Installation
-Assuming you already have [Poetry](https://python-poetry.org/) installed:
+### From Pypi
+>**Note** Assuming you have python with pip installed
+```shell
+pip install matugen
+```
+
+### Usage
+```shell
+# Dark theme
+matugen /path/to/wallpaper/
+# Light theme
+matugen /path/to/wallpaper/ -l
+```
+Example:
+```shell
+matugen ~/wall/snow.png -l
+```
+
+### From repo with poetry
+>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:
 ```shell
 git clone https://github.com/InioX/matugen && cd matugen
 poetry install
 ```
 
-## Usage
-Assuming you are in the root of this project:
+#### Usage
 ```shell
 # Dark theme
 poetry run matugen /path/to/wallpaper/
 # Light theme
 poetry run matugen /path/to/wallpaper/ -l
 ```
 Example:
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: matugen Version: 0.2.0 Summary: Author: InioX
+Metadata-Version: 2.1 Name: matugen Version: 0.3.0 Summary: Author: InioX
 Author-email: justimnix@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 material-color-utilities-python (==0.1.5) Requires-Dist: rich
 (>=12.5.1,<13.0.0) Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                           4fe9-9ee5-a1a1395d70dc.png]
                              ****** Matugen ******
                 A material you color generation tool for linux
                          Installation Â· Usage Â· Wiki
 ## Description [Material Design 3](https://m3.material.io/) offers a new color
 system that allows for more flexible and dynamic use of color. The new system
 includes a wider range of colors, as well as a range of tints and shades that
-can be used to create subtle variations in color. ## Installation Assuming you
-already have [Poetry](https://python-poetry.org/) installed: ```shell git clone
-https://github.com/InioX/matugen && cd matugen poetry install ``` ## Usage
-Assuming you are in the root of this project: ```shell # Dark theme poetry run
-matugen /path/to/wallpaper/ # Light theme poetry run matugen /path/to/
-wallpaper/ -l ``` Example: ```shell poetry run matugen ~/wall/snow.png -l ```
-## Showcase Showcase with Hyprland, Waybar, kitty, and fish shell: >**Warning**
->The preview and usage may be outdated. [![](https://markdown-videos.deta.dev/
-youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)
+can be used to create subtle variations in color. ## Installation ### From Pypi
+>**Note** Assuming you have python with pip installed ```shell pip install
+matugen ``` ### Usage ```shell # Dark theme matugen /path/to/wallpaper/ # Light
+theme matugen /path/to/wallpaper/ -l ``` Example: ```shell matugen ~/wall/
+snow.png -l ``` ### From repo with poetry >**Note** Assuming you already have
+[Poetry](https://python-poetry.org/) installed: ```shell git clone https://
+github.com/InioX/matugen && cd matugen poetry install ``` #### Usage ```shell #
+Dark theme poetry run matugen /path/to/wallpaper/ # Light theme poetry run
+matugen /path/to/wallpaper/ -l ``` Example: ```shell poetry run matugen ~/wall/
+snow.png -l ``` ## Showcase Showcase with Hyprland, Waybar, kitty, and fish
+shell: >**Warning** >The preview and usage may be outdated. [![](https://
+markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)
```

