# Comparing `tmp/smplotlib-0.0.5.tar.gz` & `tmp/smplotlib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-z8qlp8f0/smplotlib-0.0.5.tar", last modified: Fri Apr 14 03:22:31 2023, max compression
+gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-j3lyd1s5/smplotlib-0.0.6.tar", last modified: Tue Apr 18 01:19:12 2023, max compression
```

## Comparing `smplotlib-0.0.5.tar` & `smplotlib-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-14 01:14:04.000000 smplotlib-0.0.5/LICENSE
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       70 2023-04-14 03:22:16.000000 smplotlib-0.0.5/MANIFEST.in
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:22:31.000000 smplotlib-0.0.5/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1439 2023-04-14 02:47:08.000000 smplotlib-0.0.5/README.md
--rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-14 03:17:51.000000 smplotlib-0.0.5/pyproject.toml
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-04-14 03:22:31.000000 smplotlib-0.0.5/setup.cfg
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     3225 2023-04-14 03:12:34.000000 smplotlib-0.0.5/src/smplotlib/__init__.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     2275 2023-04-14 03:14:00.000000 smplotlib-0.0.5/src/smplotlib/demo.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    40706 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/smplot.mplstyle
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib/test_data/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/test_data/test_array.npy
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib/ttf/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-14 03:09:55.000000 smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib.egg-info/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib.egg-info/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1169 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       10 2023-04-14 03:22:31.000000 smplotlib-0.0.5/src/smplotlib.egg-info/top_level.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-14 03:09:55.000000 smplotlib-0.0.5/two_phase.png
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-14 01:14:04.000000 smplotlib-0.0.6/LICENSE
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       70 2023-04-14 03:22:16.000000 smplotlib-0.0.6/MANIFEST.in
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2057 2023-04-18 01:19:12.000000 smplotlib-0.0.6/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1531 2023-04-14 03:48:18.000000 smplotlib-0.0.6/README.md
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-18 01:18:55.000000 smplotlib-0.0.6/pyproject.toml
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-04-18 01:19:12.000000 smplotlib-0.0.6/setup.cfg
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     3225 2023-04-15 23:05:56.000000 smplotlib-0.0.6/src/smplotlib/__init__.py
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2275 2023-04-14 03:14:00.000000 smplotlib-0.0.6/src/smplotlib/demo.py
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    40688 2023-04-15 23:05:11.000000 smplotlib-0.0.6/src/smplotlib/smplot.mplstyle
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/test_data/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/test_data/test_array.npy
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/ttf/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2057 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1169 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       10 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/top_level.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-14 03:09:55.000000 smplotlib-0.0.6/two_phase.png
```

### Comparing `smplotlib-0.0.5/LICENSE` & `smplotlib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/PKG-INFO` & `smplotlib-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,18 @@
 ```bash
 git clone
 cd smplotlib
 pip install -e .
 ```
 
 ## Usage
-
 ```python
 import smplotlib
 ```
-Here's an example figure generated following `python demo.py` (scientifically it's not that correct, but it's just an example). This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html). 
+Then just use `matplotlib.pyplot` as usual. For a quick start, you can use `smplotlib.demo_plot()` to generate a figure with the default settings. This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html), but the cooling curve doesn't correspond to the actual CR rates and ISRF.
+
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
 There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
```

### Comparing `smplotlib-0.0.5/README.md` & `smplotlib-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 ```bash
 git clone
 cd smplotlib
 pip install -e .
 ```
 
 ## Usage
-
 ```python
 import smplotlib
 ```
-Here's an example figure generated following `python demo.py` (scientifically it's not that correct, but it's just an example). This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html). 
+Then just use `matplotlib.pyplot` as usual. For a quick start, you can use `smplotlib.demo_plot()` to generate a figure with the default settings. This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html), but the cooling curve doesn't correspond to the actual CR rates and ISRF.
+
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
 There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
```

### Comparing `smplotlib-0.0.5/pyproject.toml` & `smplotlib-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smplotlib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jiaxuan Li", email="jiaxuanl@princeton.edu" },
 ]
 description = "Matplotlib template for SuperMongo style"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smplotlib-0.0.5/src/smplotlib/__init__.py` & `smplotlib-0.0.6/src/smplotlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 for font in font_manager.findSystemFonts(pkg_path):
     font_manager.fontManager.addfont(font)
 assert 'Hershey' in font_manager.findfont('AVHershey Complex'), "Hershey font is not found"
 
 # Load style
 plt.style.use(os.path.join(pkg_path, 'smplot.mplstyle'))
 
-def set_style(usetex=False, fontsize=15, fontweight='normal', figsize=(6, 6), dpi=100):
+def set_style(usetex=False, fontsize=15, fontweight='normal', figsize=(6, 6), dpi=120):
     '''
     Set matplotlib parameters for SuperMongo style.
     
     Parameters
     ----------
     usetex : bool, optional.
         Whether to use LaTeX to render the text. Default is False.
```

### Comparing `smplotlib-0.0.5/src/smplotlib/demo.py` & `smplotlib-0.0.6/src/smplotlib/demo.py`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/smplot.mplstyle` & `smplotlib-0.0.6/src/smplotlib/smplot.mplstyle`

 * *Files 0% similar despite different names*

```diff
@@ -104,35 +104,35 @@
 
 
 ## ***************************************************************************
 ## * LINES                                                                   *
 ## ***************************************************************************
 ## See https://matplotlib.org/api/artist_api.html#module-matplotlib.lines
 ## for more information on line properties.
-#lines.linewidth: 1.5               # line width in points
+lines.linewidth: 1.2               # line width in points
 #lines.linestyle: -                 # solid line
 lines.color:     black                # has no affect on plot(); see axes.prop_cycle
 #lines.marker:          None        # the default marker
 #lines.markerfacecolor: auto        # the default marker face color
 #lines.markeredgecolor: auto        # the default marker edge color
 #lines.markeredgewidth: 1.0         # the line width around the marker symbol
-#lines.markersize:      6           # marker size, in points
+lines.markersize:      8           # marker size, in points
 #lines.dash_joinstyle:  round       # {miter, round, bevel}
 #lines.dash_capstyle:   butt        # {butt, round, projecting}
 #lines.solid_joinstyle: round       # {miter, round, bevel}
 #lines.solid_capstyle:  projecting  # {butt, round, projecting}
-#lines.antialiased: True            # render lines in antialiased (no jaggies)
+lines.antialiased: True            # render lines in antialiased (no jaggies)
 
 ## The three standard dash patterns.  These are scaled by the linewidth.
 lines.dashed_pattern: 6.5, 3
-#lines.dashdot_pattern: 6.4, 1.6, 1, 1.6
+lines.dashdot_pattern: 6.5, 3, 2, 3
 lines.dotted_pattern: 2, 4
 #lines.scale_dashes: True
 
-#markers.fillstyle: full  # {full, left, right, bottom, top, none}
+markers.fillstyle: none  # {full, left, right, bottom, top, none}
 
 #pcolor.shading: auto
 #pcolormesh.snap: True  # Whether to snap the mesh to pixel boundaries. This is
                         # provided solely to allow old test images to remain
                         # unchanged. Set to False to obtain the previous behavior.
 
 ## ***************************************************************************
@@ -400,15 +400,16 @@
 #axes.spines.left:   True  # display axis spines
 #axes.spines.bottom: True
 #axes.spines.top:    True
 #axes.spines.right:  True
 
 #axes.unicode_minus: True  # use Unicode for the minus symbol rather than hyphen.  See
                            # https://en.wikipedia.org/wiki/Plus_and_minus_signs#Character_codes
-#axes.prop_cycle: cycler('color', ['1f77b4', 'ff7f0e', '2ca02c', 'd62728', '9467bd', '8c564b', 'e377c2', '7f7f7f', 'bcbd22', '17becf'])
+axes.prop_cycle: cycler('color', ['k', 'e31c1c', '4200f7', '328b22', '71fcff', 'f100ff', '6bff42'])
+# r,g,b,c,m,lightgreen
                   # color cycle for plot lines as list of string color specs:
                   # single letter, long name, or web-style hex
                   # As opposed to all other parameters in this file, the color
                   # values must be enclosed in quotes for this parameter,
                   # e.g. '1f77b4', instead of 1f77b4.
                   # See also https://matplotlib.org/tutorials/intermediate/color_cycle.html
                   # for more details on prop_cycle usage.
@@ -580,15 +581,15 @@
 
 
 ## ***************************************************************************
 ## * IMAGES                                                                  *
 ## ***************************************************************************
 #image.aspect:          equal        # {equal, auto} or a number
 image.interpolation:   none  # see help(imshow) for options
-image.cmap:            turbo      # A colormap name, gray etc...
+image.cmap:            jet      # A colormap name, gray etc...
 image.lut:             256          # the size of the colormap lookup table
 image.origin:          lower        # {lower, upper}
 #image.resample:        True
 #image.composite_image: True  # When True, all the images on a set of axes are
                               # combined into a single composite image before
                               # saving a figure as a vector graphics file,
                               # such as a PDF.
@@ -603,28 +604,28 @@
                                      # widths. If set to None, it falls back to
                                      # `line.linewidth`.
 
 
 ## ***************************************************************************
 ## * ERRORBAR PLOTS                                                          *
 ## ***************************************************************************
-errorbar.capsize: 3  # length of end cap on error bars in pixels
+errorbar.capsize: 2  # length of end cap on error bars in pixels
 
 
 ## ***************************************************************************
 ## * HISTOGRAM PLOTS                                                         *
 ## ***************************************************************************
-#hist.bins: 10  # The default number of histogram bins or 'auto'.
+hist.bins: 'auto'  # The default number of histogram bins or 'auto'.
 
 
 ## ***************************************************************************
 ## * SCATTER PLOTS                                                           *
 ## ***************************************************************************
 #scatter.marker: o         # The default marker type for scatter plots.
-scatter.edgecolors: black  # The default edge colors for scatter plots.
+#scatter.edgecolors: black  # The default edge colors for scatter plots.
 
 
 ## ***************************************************************************
 ## * AGG RENDERING                                                           *
 ## ***************************************************************************
 ## Warning: experimental, 2008/10/10
 #agg.path.chunksize: 0  # 0 to disable; values in the range
@@ -670,15 +671,15 @@
 #savefig.facecolor: auto        # figure face color when saving
 #savefig.edgecolor: auto        # figure edge color when saving
 #savefig.format:    png         # {png, ps, pdf, svg}
 savefig.bbox:      tight    # {tight, standard}
                                 # 'tight' is incompatible with pipe-based animation
                                 # backends (e.g. 'ffmpeg') but will work with those
                                 # based on temporary files (e.g. 'ffmpeg_file')
-#savefig.pad_inches:   0.1      # Padding to be used when bbox is set to 'tight'
+#savefig.pad_inches:   '0.1'      # Padding to be used when bbox is set to 'tight'
 #savefig.directory:    ~        # default directory in savefig dialog box,
                                 # leave empty to always use current working directory
 #savefig.transparent: False     # setting that controls whether figures are saved with a
                                 # transparent background by default
 savefig.orientation: landscape  # Orientation of saved figure
 
 ### tk backend params
```

### Comparing `smplotlib-0.0.5/src/smplotlib/test_data/test_array.npy` & `smplotlib-0.0.6/src/smplotlib/test_data/test_array.npy`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexLight.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexMedium.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexLight.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexLight.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexMedium.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf` & `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/src/smplotlib.egg-info/PKG-INFO` & `smplotlib-0.0.6/src/smplotlib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,18 @@
 ```bash
 git clone
 cd smplotlib
 pip install -e .
 ```
 
 ## Usage
-
 ```python
 import smplotlib
 ```
-Here's an example figure generated following `python demo.py` (scientifically it's not that correct, but it's just an example). This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html). 
+Then just use `matplotlib.pyplot` as usual. For a quick start, you can use `smplotlib.demo_plot()` to generate a figure with the default settings. This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html), but the cooling curve doesn't correspond to the actual CR rates and ISRF.
+
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
 There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
```

### Comparing `smplotlib-0.0.5/src/smplotlib.egg-info/SOURCES.txt` & `smplotlib-0.0.6/src/smplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.5/two_phase.png` & `smplotlib-0.0.6/two_phase.png`

 * *Files identical despite different names*

