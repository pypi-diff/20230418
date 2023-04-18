# Comparing `tmp/numerous html-report-generator-1.0.3.tar.gz` & `tmp/numerous html-report-generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerous html-report-generator-1.0.3.tar", last modified: Thu Feb 23 20:39:35 2023, max compression
+gzip compressed data, was "numerous html-report-generator-1.1.0.tar", last modified: Tue Apr 18 12:20:34 2023, max compression
```

## Comparing `numerous html-report-generator-1.0.3.tar` & `numerous html-report-generator-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.706099 numerous html-report-generator-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3151 2023-02-23 20:39:35.705098 numerous html-report-generator-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 20:39:35.706099 numerous html-report-generator-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.697098 numerous html-report-generator-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.695098 numerous html-report-generator-1.0.3/src/numerous/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.699098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/block.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/caption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.701098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/div.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/figure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.702098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/pandas/dataframetable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.702098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/plotly/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/plotly/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/plotly/gofigure.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/section.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/tabs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.703098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1715 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/examples/quick_start.py
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.703098 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/templates/
--rw-rw-rw-   0 root         (0) root         (0)     6319 2023-02-23 20:39:25.000000 numerous html-report-generator-1.0.3/src/numerous/html_report_generator/templates/report_template_numerous.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 20:39:35.705098 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3151 2023-02-23 20:39:35.000000 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1286 2023-02-23 20:39:35.000000 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 20:39:35.000000 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-02-23 20:39:35.000000 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-23 20:39:35.000000 numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.991454 numerous html-report-generator-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-18 12:20:34.990538 numerous html-report-generator-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:20:34.992371 numerous html-report-generator-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.981370 numerous html-report-generator-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.979537 numerous html-report-generator-1.1.0/src/numerous/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.984120 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/block.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/caption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.985954 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/div.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/figure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.986871 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/pandas/dataframetable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.986871 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/gofigure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/section.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/tabs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.987787 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/quick_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.987787 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2023-04-18 12:20:24.000000 numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/report_template_numerous.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:20:34.990538 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-18 12:20:34.000000 numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/top_level.txt
```

### Comparing `numerous html-report-generator-1.0.3/LICENSE` & `numerous html-report-generator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/PKG-INFO` & `numerous html-report-generator-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous html-report-generator
-Version: 1.0.3
+Version: 1.1.0
 Summary: Report generator for html reports
 Home-page: 
 Author: numerous - Tobias Skov Reipuert, Tobias Dokkedal Elmøe, Lasse Nyberg Thomsen, Ósk Björnsdottir
 Author-email: report-generator@numerous.com
 License: O-BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -23,15 +23,15 @@
 
 We have provided you with a first template that you can modify to your needs. Soon we will publish a guide on how to change basic things in it - for instance the logo file.
 
 ## Installation
 
 The package numerous report generator can be installed with:
 ```console
-pip install numerous-report-generator
+pip install numerous-html-report-generator
 ```
 
 ## Quick start
 
 Here is a simple example to get you started once you have installed the package:
 
 ```python
```

### Comparing `numerous html-report-generator-1.0.3/README.md` & `numerous html-report-generator-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 We have provided you with a first template that you can modify to your needs. Soon we will publish a guide on how to change basic things in it - for instance the logo file.
 
 ## Installation
 
 The package numerous report generator can be installed with:
 ```console
-pip install numerous-report-generator
+pip install numerous-html-report-generator
 ```
 
 ## Quick start
 
 Here is a simple example to get you started once you have installed the package:
 
 ```python
```

### Comparing `numerous html-report-generator-1.0.3/setup.py` & `numerous html-report-generator-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/__init__.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 This package helps you create interactive and nice looking reports, yet available in a single static html file.
 """
 from .report import Report
 from numerous.html_report_generator.components.plotly.gofigure import GoFigure
 from .components.div import Div
 from .components.tabs import Tabs
 from .components.section import Section
+from .components.cards import Card
 from numerous.html_report_generator.components.pandas.dataframetable import DataFrameTable
```

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/caption.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/caption.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/plotly/gofigure.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/plotly/gofigure.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/section.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/section.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/components/tabs.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/components/tabs.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/examples/quick_start.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/examples/quick_start.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/report.py` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/report.py`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous/html_report_generator/templates/report_template_numerous.html` & `numerous html-report-generator-1.1.0/src/numerous/html_report_generator/templates/report_template_numerous.html`

 * *Files identical despite different names*

### Comparing `numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/PKG-INFO` & `numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous-html-report-generator
-Version: 1.0.3
+Version: 1.1.0
 Summary: Report generator for html reports
 Home-page: 
 Author: numerous - Tobias Skov Reipuert, Tobias Dokkedal Elmøe, Lasse Nyberg Thomsen, Ósk Björnsdottir
 Author-email: report-generator@numerous.com
 License: O-BSD-3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -23,15 +23,15 @@
 
 We have provided you with a first template that you can modify to your needs. Soon we will publish a guide on how to change basic things in it - for instance the logo file.
 
 ## Installation
 
 The package numerous report generator can be installed with:
 ```console
-pip install numerous-report-generator
+pip install numerous-html-report-generator
 ```
 
 ## Quick start
 
 Here is a simple example to get you started once you have installed the package:
 
 ```python
```

### Comparing `numerous html-report-generator-1.0.3/src/numerous_html_report_generator.egg-info/SOURCES.txt` & `numerous html-report-generator-1.1.0/src/numerous_html_report_generator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 src/numerous/html_report_generator/__init__.py
 src/numerous/html_report_generator/block.py
 src/numerous/html_report_generator/caption.py
 src/numerous/html_report_generator/report.py
 src/numerous/html_report_generator/components/__init__.py
+src/numerous/html_report_generator/components/cards.py
 src/numerous/html_report_generator/components/div.py
 src/numerous/html_report_generator/components/figure.py
 src/numerous/html_report_generator/components/section.py
 src/numerous/html_report_generator/components/table.py
 src/numerous/html_report_generator/components/tabs.py
 src/numerous/html_report_generator/components/pandas/__init__.py
 src/numerous/html_report_generator/components/pandas/dataframetable.py
```

