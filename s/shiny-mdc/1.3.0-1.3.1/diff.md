# Comparing `tmp/shiny_mdc-1.3.0.tar.gz` & `tmp/shiny_mdc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.3.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.3.1.tar", max compression
```

## Comparing `shiny_mdc-1.3.0.tar` & `shiny_mdc-1.3.1.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0     2641 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/LICENSE
--rw-r--r--   0        0        0       78 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/README.md
--rw-r--r--   0        0        0     2297 2023-04-15 15:54:00.737400 shiny_mdc-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-15 15:53:36.712693 shiny_mdc-1.3.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     4713 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-15 15:54:00.737400 shiny_mdc-1.3.0/shinymdc/_version.py
--rw-r--r--   0        0        0      337 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      853 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      290 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0     3359 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1041 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      426 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19149 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      977 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1443 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1440 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2187 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      897 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     2099 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      511 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2343 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-15 15:53:36.716693 shiny_mdc-1.3.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/figures/lines.png
--rw-r--r--   0        0        0     2971 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/references.bib
--rw-r--r--   0        0        0   678733 2023-04-15 15:53:36.720693 shiny_mdc-1.3.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   411241 2023-04-15 15:53:36.724693 shiny_mdc-1.3.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   404508 2023-04-15 15:53:36.724693 shiny_mdc-1.3.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   443714 2023-04-15 15:53:36.728693 shiny_mdc-1.3.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   449285 2023-04-15 15:53:36.728693 shiny_mdc-1.3.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   599001 2023-04-15 15:53:36.732693 shiny_mdc-1.3.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   548590 2023-04-15 15:53:36.732693 shiny_mdc-1.3.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   421381 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1619 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/empty.md
--rw-r--r--   0        0        0     1356 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-15 15:53:36.736693 shiny_mdc-1.3.0/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2895 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/README.md
+-rw-r--r--   0        0        0     2297 2023-04-18 08:26:05.426183 shiny_mdc-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     4936 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-18 08:26:05.430183 shiny_mdc-1.3.1/shinymdc/_version.py
+-rw-r--r--   0        0        0      337 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      853 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      290 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      426 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0     2503 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-18 08:25:42.701568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0      848 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19149 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      935 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1397 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2144 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      890 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     2057 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      469 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2255 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/figures/lines.png
+-rw-r--r--   0        0        0     2972 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-18 08:25:42.705568 shiny_mdc-1.3.1/test/references.bib
+-rw-r--r--   0        0        0   682300 2023-04-18 08:25:42.709568 shiny_mdc-1.3.1/test/samples/basic.pdf
+-rw-r--r--   0        0        0   412224 2023-04-18 08:25:42.713568 shiny_mdc-1.3.1/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   405928 2023-04-18 08:25:42.713568 shiny_mdc-1.3.1/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   445680 2023-04-18 08:25:42.717568 shiny_mdc-1.3.1/test/samples/icml.pdf
+-rw-r--r--   0        0        0   450203 2023-04-18 08:25:42.717568 shiny_mdc-1.3.1/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600967 2023-04-18 08:25:42.721568 shiny_mdc-1.3.1/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   551977 2023-04-18 08:25:42.721568 shiny_mdc-1.3.1/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   423226 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1625 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/empty.md
+-rw-r--r--   0        0        0     1837 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/main1.md
+-rw-r--r--   0        0        0     1353 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-18 08:25:42.725568 shiny_mdc-1.3.1/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.3.1/PKG-INFO
```

### Comparing `shiny_mdc-1.3.0/CHANGELOG.md` & `shiny_mdc-1.3.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [1.3.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.3.0...v1.3.1) (2023-04-18)
+
+
+### Bug Fixes
+
+* fix handling of notes in citations ([9a272a6](https://github.com/jayanthkoushik/shiny-mdc/commit/9a272a661971a25dc78703a2889dcadf00c429ed))
+
 ## [1.3.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.2.0...v1.3.0) (2023-04-15)
 
 
 ### Features
 
 * improve clean up of tex files directory ([d5b1822](https://github.com/jayanthkoushik/shiny-mdc/commit/d5b182265fbd3884ebc59ca618bd2302df400647))
 * improve command line interface ([58fb232](https://github.com/jayanthkoushik/shiny-mdc/commit/58fb2328e5c59bab3970ee7ff6beea1d4a9af252))
```

### Comparing `shiny_mdc-1.3.0/LICENSE` & `shiny_mdc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/pyproject.toml` & `shiny_mdc-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.3.0"  # managed by `poetry-dynamic-versioning`
+version = "1.3.1"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.3.0/shinymdc/_latexmk.py` & `shiny_mdc-1.3.1/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/_liquid.py` & `shiny_mdc-1.3.1/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/_pandoc.py` & `shiny_mdc-1.3.1/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/_templates.py` & `shiny_mdc-1.3.1/shinymdc/_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,19 +40,24 @@
 
     _static_resources = defaultdict(
         list,
         {
             # These are per-template static resources. The '*' key if for resources
             # that are common to all templates.
             "*": ["reqsetup.tex", "floatsetup.tex", "mathsetup.tex", "miscsetup.tex"],
+            "basic": ["bibsupersetup.tex"],
+            "stylish": ["bibsupersetup.tex"],
+            "standalone": ["bibsupersetup.tex"],
+            "spacious": ["bibsupersetup.tex"],
             "iccv": [
                 "iccv/iccv.sty",
                 "iccv/esopic.sty",
                 "iccv/everyshi.sty",
                 "iccv/bibstyle.bst",
+                "bibnonatsetup.tex",
             ],
             "iclr": ["iclr/iclr.sty", "iclr/bibstyle.bst", "iclr/mathcommands.tex"],
             "icml": ["icml/icml.sty", "icml/bibstyle.bst"],
             "neurips": ["neurips/neurips.sty"],
         },
     )
     _dynamic_resources = defaultdict(
```

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.3.1/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.3.1/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.3.1/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.3.1/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.3.1/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.3.1/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.3.1/shinymdc/resources/static/miscsetup.tex`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,14 @@
 \usepackage{acronym}
 \usepackage{relsize}
 \usepackage{xcolor}
 \usepackage{tikz}
 \usepackage{fancyvrb}
 \usepackage{pgf}
 
-% Put year in citet.
-\newcommand*{\nolink}[1]{{\protect\NoHyper#1\protect\endNoHyper}}
-\let\origcitet\citet
-\renewcommand{\citet}[1]{%
-  \nolink{\citeauthor{#1} (\citeyear{#1})}~\citep{#1}%
-}
-
 % Handle footnotes inside tables, figures.
 \makesavenoteenv{table}
 \makesavenoteenv{table*}
 \makesavenoteenv{figure}
 \makesavenoteenv{figure*}
 
 % Add small space after footnote label.
```

### Comparing `shiny_mdc-1.3.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.3.1/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/shinymdc.py` & `shiny_mdc-1.3.1/shinymdc/shinymdc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.3.1/shinymdc/templates/basic.tex`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 \PassOptionsToPackage{hidelinks=true}{hyperref}
-\PassOptionsToPackage{square,numbers,super,sort&compress}{natbib}
 
 \documentclass[%
   letterpaper,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
 \usepackage[margin=1.5in,footskip=0.75in]{geometry}
 \usepackage{parskip}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
+\input{$bibsupersetup$}
 \input{$miscsetup$}
 
 % Increase maximum figure/table widths.
 \renewcommand{\maxfigwidth}{6.5in}
 \renewcommand{\maxtabwidth}{6.5in}
 
 \title{\vspace{-5ex} $title$}
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.3.1/shinymdc/templates/iccv.tex`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 $if(submission)$
 \PassOptionsToPackage{pagebackref=true,breaklinks=true,letterpaper=true,colorlinks,bookmarks=false}{hyperref}
 $else$
 \PassOptionsToPackage{breaklinks=true,bookmarks=false}{hyperref}
 $endif$
 
-\PassOptionsToPackage{square,numbers,sort&compress}{natbib}
-
 \documentclass[10pt,twocolumn,letterpaper]{article}
 
 \usepackage{$everyshi$}
 \usepackage{$esopic$}
 \usepackage{$iccv$}
 \usepackage{newtxtext}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
+\input{$bibnonatsetup$}
 
 $if(submission)$$else$\iccvfinalcopy$endif$
 
 \def\iccvPaperID{$paperid$}
 \def\httilde{\mbox{\tt\raisebox{-.5ex}{\symbol{126}}}}
 
 % Pages are numbered in submission mode, and unnumbered in camera-ready.
 \ificcvfinal\pagestyle{empty}\fi
 
-% Make citet equal to citep since author names are not available.
-\renewcommand{\citet}[1]{\citep{#1}}
-
 $for(includes)$
 $it$
 $endfor$
 
 \raggedbottom
 
 \begin{document}
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.3.1/shinymdc/templates/iclr.tex`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 \usepackage{url}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
 
-% Restore old citet.
-\let\citet\origcitet
-
 % Optional math commands from https://github.com/goodfeli/dlbook_notation.
 % \input{$mathcommands$.tex}
 
 \title{$title$}
 
 % The \author macro works with any number of authors. There are two commands
 % used to separate the names and addresses of multiple authors: \And and \AND.
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.3.1/shinymdc/templates/icml.tex`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 \usepackage$if(submission)$$else$[accepted]$endif${$icml$}
 
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
 
-% Restore old citet.
-\let\citet\origcitet
-
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % THEOREMS
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 \theoremstyle{plain}
 \newtheorem{theorem}{Theorem}[section]
 \newtheorem{proposition}[theorem]{Proposition}
 \newtheorem{lemma}[theorem]{Lemma}
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.3.1/shinymdc/templates/neurips.tex`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 \RequirePackage{scrlfile}
 \PreventPackageFromLoading{babel}
 \PreventPackageFromLoading{microtype}
 $endif$
 
 \documentclass{article}
 
-\PassOptionsToPackage{square,numbers,sort&compress}{natbib}
+\PassOptionsToPackage{numbers,sort&compress}{natbib}
 \usepackage$if(submission)$$else$$if(preprint)$[preprint]$else$[final]$endif$$endif${$neurips$}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
 \input{$miscsetup$}
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.3.1/shinymdc/templates/spacious.tex`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 \PassOptionsToPackage{hidelinks=true}{hyperref}
-\PassOptionsToPackage{square,numbers,super,sort&compress}{natbib}
 
 \documentclass[%
   letterpaper,%
   12pt,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
@@ -12,14 +11,15 @@
 \usepackage{fancyhdr}
 \usepackage{cfr-lm}
 % \usepackage{ebgaramond}
 
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$mathsetup$}
+\input{$bibsupersetup$}
 \input{$miscsetup$}
 
 % Increase maximum figure/table sizes.
 \renewcommand{\maxfigwidth}{6.5in}
 \renewcommand{\maxfigheight}{10in}
 \renewcommand{\maxtabwidth}{6.5in}
 \renewcommand{\maxtabheight}{10in}
```

### Comparing `shiny_mdc-1.3.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.3.1/shinymdc/templates/stylish.tex`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 \PassOptionsToPackage{hidelinks=true}{hyperref}
-% \PassOptionsToPackage{square,comma,numbers,super,sort&compress}{natbib}
-\PassOptionsToPackage{square,comma,numbers,super,sort}{natbib}
 
 \documentclass[%
   letterpaper,%
   twocolumn,%
   $if(lang)$$lang$$else$english$endif$%
 ]{article}
 
@@ -16,18 +14,20 @@
   footnotesep=50pt%
 ]{geometry}
 \usepackage[sf,big,raggedright,compact]{titlesec}
 \usepackage{fancyhdr}
 \usepackage{newtxtext}
 \usepackage{etoolbox}
 
+\def\nobibcompress{TRUE}
 \input{$reqsetup$}
 \input{$floatsetup$}
 \input{$dblfloatsetup$}
 \input{$mathsetup$}
+\input{$bibsupersetup$}
 \input{$miscsetup$}
 
 % Use small font for tables.
 \AtBeginEnvironment{tabular}{\smaller}
 
 % Configure caption font.
 \captionsetup{justification=raggedright,font={sf,small}}
```

### Comparing `shiny_mdc-1.3.0/test/figures/anscombe.pdf` & `shiny_mdc-1.3.1/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/figures/densities.pdf` & `shiny_mdc-1.3.1/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/figures/diamonds.pdf` & `shiny_mdc-1.3.1/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.3.1/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/figures/lines.png` & `shiny_mdc-1.3.1/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/main.md` & `shiny_mdc-1.3.1/test/main.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   affiliation:
   - 2
 institute:
 - id: 1
   name: Institute One
 - id: 2
   name: Institute Two at City, State
-abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference[@texbook].
+abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference [@texbook].
 bibliography: references.bib
 sections:
 - sections/main1.md
 - sections/main2.md
 - sections/empty.md
 appendices:
 - sections/appendix1.md
```

### Comparing `shiny_mdc-1.3.0/test/references.bib` & `shiny_mdc-1.3.1/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/samples/basic.pdf` & `shiny_mdc-1.3.1/test/samples/basic.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -172,71 +172,41 @@
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Short citation [2]
-• Long citation: Mittelbach et al. (2004) [2] , Lesk and Kernighan (1977) [3]
-• Multi citation [2–4]
-• Pointer to footnote1
+• Pointer to footnote 1
 
 7
 
-Tables
-• Table 1
-• Table 2
-
-8
-
-Figures
-• Figure 2
+Citations
+• Short citation [2]
+• Short citation with pre note [see 2]
+• Short citation with post note [2, p. 1]
+• Short citation with pre/post notes [see 2, p. 1]
+• Long citation: Lesk and Kernighan (1977) [3]
+• Long citation with note: Lesk and Kernighan (1977) [3, p. 1]
+• Multi citation [2–4]
+• Multi citation with pre note [see 2–4]
+• Multi citation with post note [2–4, for more]
+• Multi citation with pre/post notes [see 2–4, for more]
 1 Example footnote text.
 
 3
 
 (2)
 
-Figure 2: Narrow figure
-
-A
-B
-C
-D
-E
-F
-G
-H
-I
-J
-
-62
-
-64
-
-66
-
-68
-
-x
-
-70
-
-Figure 3: Wide figure
-
-4
-
-72
-
-74
-
-76
+8
 
-Col1
+Tables
+• Table 1
+• Table 2
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -253,14 +223,15 @@
 333
 
 4
 44
 444
 
 Table 1: Short table
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -325,30 +296,70 @@
 4
 
 5
 
 6
 
 Table 2: Wide table
+
+9
+
+Figures
+• Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
-9
+10
 
 Includes
+
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
-
 Content added through include statement.
 
 2 Footnote in sub-figure caption.
 3 Footnote in figure caption.
 
+4
+
+Figure 2: Narrow figure
+
+A
+B
+C
+D
+E
+F
+G
+H
+I
+J
+
+62
+
+64
+
+66
+
+68
+
+x
+
+70
+
+Figure 3: Wide figure
+
 5
 
+72
+
+74
+
+76
+
 dataset = I
 
 dataset = II
 
 dataset = III
 
 dataset = IV
@@ -378,19 +389,19 @@
 
 15
 
 5
 
 10
 
-(b) Figure with ‘width=3.5in’2
+(b) Figure with ‘width=3.5in’ 2
 
 (a) Figure with ‘width=2.5in’
 
-Figure 4: Sub-figures3
+Figure 4: Sub-figures 3
 
 6
 
 x
 
 15
 
@@ -644,15 +655,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table3
+Table B1: Extra wide table 3
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum
 non neque sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed
```

### Comparing `shiny_mdc-1.3.0/test/samples/iccv.pdf` & `shiny_mdc-1.3.1/test/samples/iccv.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -23,15 +23,15 @@
 
 sem quis urna vulputate aliquet.
 
 Abstract
 
 1.1. Subsection 1
 
-Markdown in abstract. x + 2. Section 1. Reference[2].
+Markdown in abstract. x + 2. Section 1. Reference [2].
 
 1. Section
 Integer at enim eu tellus malesuada scelerisque. Ut sed
 rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
 pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 Nunc faucibus pellentesque elit, non ornare risus suscipit sed.
 Maecenas vel blandit ex.
@@ -102,87 +102,15 @@
 
 x
 
 15
 
 (c) Sub-figure with ‘width=2in’
 
-Col1
-
-Col2
-
-Col3
-
-Col4
-
-Col5
-
-Col6
-
-Col7
-
-Col8
-
-Col9
-
-Col10
-
-a
-b
-
-1
-11
-
-2
-22
-
-3
-33
-
-123
-456
-
-abcd
-efgh
-
-1234
-567
-
-444
-44
-
-555
-55
-
-666
-66
-
-Mid
-c
-
-111
-
-222
-
-333
-
-789
-
-ijkl
-
-89
-
-4
-
-5
-
-6
-
-Table 2: Wide table
-Aliquam at ultrices libero. Nulla facilisi. Fusce sed est
+Aliquam at ultrices libero. Nulla facilisi. Fusce sed est
 placerat, fringilla augue at, pretium nisl.
 1.2.2
 
 Subsubsection 2
 
 In ut nunc libero. Duis eu elementum purus. Etiam dictum,
 ipsum nec aliquam lobortis, magna magna pellentesque
@@ -192,41 +120,39 @@
 molestie, eget varius eros ultrices.
 Subsubsubsection Proin eleifend lorem semper, commodo
 tellus nec, porta purus. Nullam commodo lectus nibh,
 consequat maximus lorem faucibus in. Nam purus eros,
 rutrum in sapien et, condimentum lacinia nibh.
 
 2. Typography
-
-R∞
-2
-• Inline: 0 exp−x dx
-• Block: Equation 1, Equation 2
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
-x=1
-x + y = 10
+• Bold
+• Italic
+• Bold italic.
 
 6. Links
-
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Short citation[4]
-• Long citation: [4], [3]
-• Multi citation[1, 3, 4]
-• Pointer to footnote¹
+• Pointer to footnote ¹
 
-• Bold
-• Italic
-• Bold italic.
+7. Citations
+• Short citation [4]
+• Short citation with pre note [4]
+• Short citation with post note [4, p. 1]
+• Short citation with pre/post notes [4, p. 1]
+• Long citation: [3]
+• Long citation with note: [3, p. 1]
+• Multi citation [3, 1, 4]
+• Multi citation with pre note [3, 1, 4]
+• Multi citation with post note [3, 1, 4, for more]
+• Multi citation with pre/post notes [3, 1, 4, for more]
 
-7. Tables
+8. Tables
 
 3. Numbers
 
 • Table 1
 • Table 2
 
 • Normal: 0123456789
@@ -238,23 +164,14 @@
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
 5. Math
-Z ∞
-
-2
-
-exp−x dx
-
-(1)
-
-x + y + z = 100
 
 Col1
 
 Col2
 
 Col3
 
@@ -274,23 +191,49 @@
 
 4
 44
 444
 
 Table 1: Short table
 
-8. Figures
+9. Figures
+Z ∞
+
+2
+
+exp−x dx
+
+0
+
+(1)
+
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
-0
-
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 (2)
+10. Includes
+R∞
+2
+• Commands from metadata include: arg min R
+• Inline: 0 exp−x dx
+• Include command in body (there should be text after
+• Block: Equation 1, Equation 2
+this):
+• Commands defined in body (P[x in X]): P[x ∈ X ]
+• Aligned:
+Content added through include statement.
+x=1
+x + y = 10
+x + y + z = 100
+
+¹ Example footnote text.
+² Footnote in sub-figure caption.
+³ Footnote in figure caption.
 
 A
 B
 C
 D
 E
 F
@@ -351,29 +294,96 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’²
+(b) Figure with ‘width=3.5in’ ²
 
-Figure 4: Sub-figures³
+Figure 4: Sub-figures ³
 
 10
 
 x
 
 15
 
-9. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
+Col1
+
+Col2
+
+Col3
+
+Col4
+
+Col5
+
+Col6
+
+Col7
+
+Col8
+
+Col9
+
+Col10
+
+a
+b
+
+1
+11
+
+2
+22
+
+3
+33
+
+123
+456
+
+abcd
+efgh
+
+1234
+567
+
+444
+44
+
+555
+55
+
+666
+66
+
+Mid
+c
+
+111
+
+222
+
+333
+
+789
+
+ijkl
+
+89
+
+4
+
+5
+
+6
+
+Table 2: Wide table
 
 References
 [1] Donald E. Knuth. Literate programming. The Computer
 Journal, 27(2):97–111, 1984.
 [2] Donald E. Knuth. The TEX Book. Addison-Wesley Professional,
 1986.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting
@@ -435,30 +445,24 @@
 Proin eleifend lorem semper, commodo tellus nec, porta
 purus. Nullam commodo lectus nibh, consequat maximus
 lorem faucibus in. Nam purus eros, rutrum in sapien et,
 condimentum lacinia nibh.
 
 A.2. Appendix figures
 • Figure A1
-
 • Figure A2
 
 A.3. Appendix includes
 • Commands from metadata include (argmin R):
 • Include command in body (there should be text after
 this):
 Content added through include statement.
 
 A.4. Appendix links
 • Appendix section: Section A.1.1, Section B
-• Main body section: Section 1
-• Main body figure: Figure 2
-• Main body table: Table 1
-• Main body equation: Equation 1
-• Citation: [1]
 
 (a) Figure with non-default extension
 
 (b) Sub-figure
 
 dataset = I
 
@@ -501,14 +505,20 @@
 
 (c) Sub-figure
 
 Figure A2: Sub-figures with large combined size.
 
 15
 
+• Main body section: Section 1
+• Main body figure: Figure 2
+• Main body table: Table 1
+• Main body equation: Equation 1
+• Citation: [1]
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -609,15 +619,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table³
+Table B1: Extra wide table ³
 
 Appendix B. Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed
 sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum
```

### Comparing `shiny_mdc-1.3.0/test/samples/iclr.pdf` & `shiny_mdc-1.3.1/test/samples/iclr.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 9% similar despite different names*

#### pdftotext {} -

```diff
@@ -18,15 +18,15 @@
 author4@author4.com
 
 Author Number Five
 Institute Two at City, State
 authornumberfive@institutetwo.edu
 
 Abstract
-Markdown in abstract. x + 2. Section 1. Reference(Knuth, 1986).
+Markdown in abstract. x + 2. Section 1. Reference (Knuth, 1986).
 
 1
 
 Section
 
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus
 vitae pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar. Nunc faucibus
@@ -149,42 +149,61 @@
 0
 
 2
 
 (1)
 
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+
+(2)
+
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
+
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Short citation(Mittelbach et al., 2004)
-• Long citation: Mittelbach et al. (2004), Lesk & Kernighan (1977)
-• Multi citation(Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004)
-• Pointer to footnote¹
+• Pointer to footnote ¹
 
 7
 
+Citations
+• Short citation (Mittelbach et al., 2004)
+• Short citation with pre note (see Mittelbach et al., 2004)
+• Short citation with post note (Mittelbach et al., 2004, p. 1)
+• Short citation with pre/post notes (see Mittelbach et al., 2004, p. 1)
+• Long citation: Lesk & Kernighan (1977)
+• Long citation with note: Lesk & Kernighan (1977, p. 1)
+• Multi citation (Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004)
+• Multi citation with pre note (see Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al.,
+2004)
+• Multi citation with post note (Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004,
+for more)
+• Multi citation with pre/post notes (see Lesk & Kernighan, 1977; Knuth, 1984; Mittelbach
+et al., 2004, for more)
+
+8
+
 Tables
 • Table 1
 • Table 2
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -203,15 +222,17 @@
 
 4
 44
 444
 
 Table 1: Short table
 
-Col1
+3
+
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -276,51 +297,17 @@
 
 5
 
 6
 
 Table 2: Wide table
 
-8
-
-Figures
-• Figure 2
-¹ Example footnote text.
-
-3
-
-(2)
-
-Figure 2: Narrow figure
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-9
-
-Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-
-Content added through include statement.
-
-References
-Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
-Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
-Proceedings of American Federation of Information Processing Societies: 1977 National Computer
-Conference, pp. 879–888, Dallas, Texas, 1977.
-Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
-Companion. Addison-Wesley Professional, 2 edition, 2004.
-
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
-
-4
+Figure 2: Narrow figure
 
-A
+A
 B
 C
 D
 E
 F
 G
 H
@@ -337,15 +324,15 @@
 
 x
 
 70
 
 Figure 3: Wide figure
 
-5
+4
 
 72
 
 74
 
 76
 
@@ -382,26 +369,56 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’²
+(b) Figure with ‘width=3.5in’ ²
 
-Figure 4: Sub-figures³
+Figure 4: Sub-figures ³
 
-6
+9
+
+Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
+¹ Example footnote text.
+² Footnote in sub-figure caption.
+³ Footnote in figure caption.
+
+5
 
 10
 
 x
 
 15
 
+10
+
+Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+
+Content added through include statement.
+
+References
+Donald E. Knuth. Literate programming. The Computer Journal, 27(2):97–111, 1984.
+Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
+Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX. In
+Proceedings of American Federation of Information Processing Societies: 1977 National Computer
+Conference, pp. 879–888, Dallas, Texas, 1977.
+Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The LATEX
+Companion. Addison-Wesley Professional, 2 edition, 2004.
+
+6
+
 A
 B
 C
 D
 E
 F
 G
@@ -629,15 +646,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table³
+Table B1: Extra wide table ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
```

### Comparing `shiny_mdc-1.3.0/test/samples/icml.pdf` & `shiny_mdc-1.3.1/test/samples/icml.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,16 +1,14 @@
 shinymdc-test
 
 Author One * 1 Author MiddleName Two * 1 2 Author * Author Four Author Number Five 2
 
 Abstract
-Markdown in abstract.
-Reference(Knuth, 1986).
-
-x + 2.
+Markdown in abstract. x + 2.
+Reference (Knuth, 1986).
 
 1.1. Subsection 1
 Section 1.
 
 1. Section
 
 In mollis tortor vel ante cursus, ac consectetur nibh
@@ -106,127 +104,73 @@
 
 x
 
 15
 
 (c) Sub-figure with ‘width=2in’
 
-Col1
-
-Col2
-
-Col3
-
-Col4
-
-Col5
-
-Col6
-
-Col7
-
-Col8
-
-Col9
-
-Col10
-
-a
-b
-
-1
-11
-
-2
-22
-
-3
-33
-
-123
-456
-
-abcd
-efgh
-
-1234
-567
-
-444
-44
-
-555
-55
-
-666
-66
-
-Mid
-c
-
-111
-
-222
-
-333
-
-789
-
-ijkl
-
-89
-
-4
-
-5
-
-6
-
-Table 2. Wide table
-
-Subsubsubsection Proin eleifend lorem semper,
+Subsubsubsection Proin eleifend lorem semper,
 commodo tellus nec, porta purus. Nullam commodo lectus
 nibh, consequat maximus lorem faucibus in. Nam purus
 eros, rutrum in sapien et, condimentum lacinia nibh.
 
 2. Typography
 • Bold
 • Italic
 • Bold italic.
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
-6. Links
-• Section: Section 1, Section 1.2
-• Appendix section: Section B, Section A.1.1
-• Appendix figure: Figure A1
-• Appendix table: Table B1
-• Appendix math: Equation 4
-• Short citation(Mittelbach et al., 2004)
-• Long citation: Mittelbach et al. (2004), Lesk &
-Kernighan (1977)
-• Multi citation(Lesk & Kernighan, 1977; Knuth, 1984;
-Mittelbach et al., 2004)
-• Pointer to footnote1
-
-7. Tables
-• Table 1
-• Table 2
-
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (C M U )
 • Repeated (short): C M U
 • Forced short: U S A
 • Repeated after forced short (short+long): United States
 of America ( U S A )
 • Plural: social security numbers ( S S N S )
 
+• Pointer to footnote 1
+
+7. Citations
+• Short citation (Mittelbach et al., 2004)
+• Short citation with pre note (see Mittelbach et al., 2004)
+• Short citation with post note (Mittelbach et al., 2004,
+p. 1)
+• Short citation with pre/post notes (see Mittelbach et al.,
+2004, p. 1)
+• Long citation: Lesk & Kernighan (1977)
+• Long citation with note: Lesk & Kernighan (1977, p. 1)
+• Multi citation (Lesk & Kernighan, 1977; Knuth, 1984;
+Mittelbach et al., 2004)
+• Multi citation with pre note (see Lesk & Kernighan,
+1977; Knuth, 1984; Mittelbach et al., 2004)
+• Multi citation with post note (Lesk & Kernighan, 1977;
+Knuth, 1984; Mittelbach et al., 2004, for more)
+• Multi citation with pre/post notes (see Lesk &
+Kernighan, 1977; Knuth, 1984; Mittelbach et al., 2004,
+for more)
+
+8. Tables
+• Table 1
+• Table 2
+
+5. Math
+Z ∞
+
+2
+
+exp−x dx
+
+(1)
+
+0
+
 Col1
 
 Col2
 
 Col3
 
 Col4
@@ -243,51 +187,52 @@
 33
 333
 
 4
 44
 444
 
-Table 1. Short table
-
-5. Math
-Z ∞
-
-2
-
-exp−x dx
-
-(1)
-
-8. Figures
-
-0
-
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9Table 1. Short table
 (2)
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
 
-9. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
+9. Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
 
 x=1
 x + y = 10
 x + y + z = 100
 
+10. Includes
+• Commands from metadata include: arg min R
+
+6. Links
+• Section: Section 1, Section 1.2
+• Appendix section: Section B, Section A.1.1
+• Appendix figure: Figure A1
+• Appendix table: Table B1
+• Appendix math: Equation 4
+
+1
+
+Example footnote text.
+Footnote in sub-figure caption.
+3
+Footnote in figure caption.
+4
+Footnote in figure caption.
+2
+
 A
 B
 C
 D
 E
 F
 G
@@ -347,25 +292,102 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’2
+(b) Figure with ‘width=3.5in’ 2
 
-Figure 4. Sub-figures4
+Figure 4. Sub-figures 4
 
 10
 
 x
 
 15
 
-Figure 2. Narrow figure
+Col1
+
+Col2
+
+Col3
+
+Col4
+
+Col5
+
+Col6
+
+Col7
+
+Col8
+
+Col9
+
+Col10
+
+a
+b
+
+1
+11
+
+2
+22
+
+3
+33
+
+123
+456
+
+abcd
+efgh
+
+1234
+567
+
+444
+44
+
+555
+55
+
+666
+66
+
+Mid
+c
+
+111
+
+222
+
+333
+
+789
+
+ijkl
+
+89
+
+4
+
+5
+
+6
+
+Table 2. Wide table
+
+• Include command in body (there should be text after
+this):
+Content added through include statement.
+
+Figure 2. Narrow figure
 
 References
 Knuth, D. E. Literate programming. The Computer Journal,
 27(2):97–111, 1984.
 Knuth, D. E. The TEX Book. Addison-Wesley Professional,
 1986.
 Lesk, M. and Kernighan, B. Computer typesetting of
@@ -594,15 +616,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1. Extra wide table4
+Table B1. Extra wide table 4
 
 B. Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit.
 Aliquam nisi purus, bibendum non neque sed, lacinia
 tristique tortor. Vestibulum eu lectus sed velit luctus varius.
 Sed sollicitudin ligula ante. Integer porta a erat commodo
 dignissim. Duis et lectus diam. Nulla id erat vestibulum nisi
```

### Comparing `shiny_mdc-1.3.0/test/samples/neurips.pdf` & `shiny_mdc-1.3.1/test/samples/neurips.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 9% similar despite different names*

#### pdftotext {} -

```diff
@@ -17,15 +17,15 @@
 author4@author4.com
 
 Author Number Five
 Institute Two at City, State
 authornumberfive@institutetwo.edu
 
 Abstract
-Markdown in abstract. x + 2. Section 1. Reference[1].
+Markdown in abstract. x + 2. Section 1. Reference [1].
 
 1
 
 Section
 
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus
 vitae pulvinar leo, at pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar. Nunc faucibus
@@ -155,33 +155,45 @@
 a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
 R∞
 2
 • Inline: 0 exp−x dx
 • Block: Equation 1, Equation 2
 • Commands defined in body (P[x in X]): P[x ∈ X ]
 • Aligned:
+
 x=1
 x + y = 10
 x + y + z = 100
 
 6
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Short citation[2]
-• Long citation: Mittelbach et al. (2004) [2], Lesk and Kernighan (1977) [3]
-• Multi citation[2–4]
-• Pointer to footnote1
+• Pointer to footnote 1
 
 7
 
+Citations
+• Short citation [2]
+• Short citation with pre note [see 2]
+• Short citation with post note [2, p. 1]
+• Short citation with pre/post notes [see 2, p. 1]
+• Long citation: Lesk and Kernighan [3]
+• Long citation with note: Lesk and Kernighan [3, p. 1]
+• Multi citation [2–4]
+• Multi citation with pre note [see 2–4]
+• Multi citation with post note [2–4, for more]
+• Multi citation with pre/post notes [see 2–4, for more]
+
+8
+
 Tables
 • Table 1
 • Table 2
 
 Col1
 1
 11
@@ -198,15 +210,19 @@
 4
 22
 33
 44
 222 333 444
 Table 1: Short table
 
-Col1
+3
+
+(2)
+
+Col1
 
 Col2
 
 Col3
 
 Col4
 
@@ -268,46 +284,17 @@
 
 4
 
 5
 
 6
 
-3
-
-(2)
-
-Figure 2: Narrow figure
-
-8
-
-Figures
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-9
-
-Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-
-Content added through include statement.
-
-1
-
-Example footnote text.
-Footnote in sub-figure caption.
-3
-Footnote in figure caption.
-2
-
-4
+Figure 2: Narrow figure
 
-A
+A
 B
 C
 D
 E
 F
 G
 H
@@ -324,15 +311,15 @@
 
 x
 
 70
 
 Figure 3: Wide figure
 
-5
+4
 
 72
 
 74
 
 76
 
@@ -369,26 +356,51 @@
 
 x
 
 15
 
 5
 
-(b) Figure with ‘width=3.5in’2
+(b) Figure with ‘width=3.5in’ 2
 
-Figure 4: Sub-figures3
+Figure 4: Sub-figures 3
 
-6
+9
+
+Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
+1
+
+Example footnote text.
+Footnote in sub-figure caption.
+3
+Footnote in figure caption.
+2
+
+5
 
 10
 
 x
 
 15
 
+10
+
+Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+
+Content added through include statement.
+
+6
+
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris Rowley. The
 LATEX Companion. Addison-Wesley Professional, 2 edition, 2004.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting of technical journals on UNIX.
 In Proceedings of American Federation of Information Processing Societies: 1977 National
 Computer Conference, pages 879–888, Dallas, Texas, 1977.
@@ -515,15 +527,15 @@
 
 15
 
 • Main body section: Section 1
 • Main body figure: Figure 2
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984) [4]
+• Citation: Knuth [4]
 
 10
 
 Col1
 
 Col2
 
@@ -627,15 +639,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table3
+Table B1: Extra wide table 3
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque
 sed, lacinia tristique tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante.
```

### Comparing `shiny_mdc-1.3.0/test/samples/spacious.pdf` & `shiny_mdc-1.3.1/test/samples/spacious.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -150,24 +150,38 @@
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
 • Appendix table: Table B1
 • Appendix math: Equation 4
+• Pointer to footnote 1
+
+7. Citations
 • Short citation [2]
-• Long citation: Mittelbach et al. (2004) [2] , Lesk and Kernighan
-(1977) [3]
+• Short citation with pre note [see 2]
+• Short citation with post note [2, p. 1]
+• Short citation with pre/post notes [see 2, p. 1]
+• Long citation: Lesk and Kernighan (1977) [3]
+• Long citation with note: Lesk and Kernighan (1977) [3, p. 1]
 • Multi citation [2–4]
-• Pointer to footnote1
+• Multi citation with pre note [see 2–4]
+• Multi citation with post note [2–4, for more]
+• Multi citation with pre/post notes [see 2–4, for more]
 
-7. Tables
+8. Tables
 • Table 1
 • Table 2
 
+1
+
+Example footnote text.
+
+5
+
 Col1
 
 Col2
 
 Col3 Col4
 
 1
@@ -184,20 +198,14 @@
 
 4
 44
 444
 
 Table 1: Short table
 
-1
-
-Example footnote text.
-
-5
-
 Col1 Col2
 
 Col3
 
 Col4 Col5
 
 Col6
@@ -249,30 +257,34 @@
 
 6
 
 ijkl
 
 Table 2: Wide table
 
-8. Figures
-
-Figure 2: Narrow figure
-
+9. Figures
 • Figure 2
 • Figure 3
 • Figure 4, Figure 4a, Figure 4b
 
+10. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after this):
+Content added through include statement.
+
 2
 3
 
 Footnote in sub-figure caption.
 Footnote in figure caption.
 
 6
 
+Figure 2: Narrow figure
+
 A
 B
 C
 D
 E
 F
 G
@@ -290,19 +302,21 @@
 
 x
 
 70
 
 72
 
+Figure 3: Wide figure
+
 74
 
 76
 
-Figure 3: Wide figure
+7
 
 dataset = I
 
 dataset = II
 
 dataset = III
 
@@ -335,29 +349,22 @@
 
 15
 
 5
 
 10
 
-(b) Figure with ‘width=3.5in’2
+(b) Figure with ‘width=3.5in’ 2
 
-Figure 4: Sub-figures3
+Figure 4: Sub-figures 3
 
 x
 
 15
 
-7
-
-9. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after this):
-Content added through include statement.
-
 8
 
 References
 [1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
 [2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and Chris
 Rowley. The LATEX Companion. Addison-Wesley Professional, 2 edition, 2004.
 [3] Michael Lesk and Brian Kernighan. Computer typesetting of technical journals
@@ -569,15 +576,15 @@
 efgh
 ijkl
 
 1234 9876
 567 543
 89 21
 
-Table B1: Extra wide table3
+Table B1: Extra wide table 3
 
 Appendix B Appendix 2
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi
 purus, bibendum non neque sed, lacinia tristique tortor. Vestibulum
 eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer
 porta a erat commodo dignissim. Duis et lectus diam. Nulla id erat
 vestibulum nisi placerat efficitur. Nulla a semper libero.
```

### Comparing `shiny_mdc-1.3.0/test/samples/standalone.pdf` & `shiny_mdc-1.3.1/test/samples/standalone.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -148,20 +148,31 @@
 
 Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section ??, Section ??
 • Appendix figure: Figure ??
 • Appendix table: Table ??
 • Appendix math: Equation ??
+• Pointer to footnote a
+
+7
+
+Citations
 • Short citation [1]
-• Long citation: Mittelbach et al. (2004) [1] , Lesk and Kernighan (1977) [2]
+• Short citation with pre note [see 1]
+• Short citation with post note [1, p. 1]
+• Short citation with pre/post notes [see 1, p. 1]
+• Long citation: Lesk and Kernighan (1977) [2]
+• Long citation with note: Lesk and Kernighan (1977) [2, p. 1]
 • Multi citation [1–3]
-• Pointer to footnotea
+• Multi citation with pre note [see 1–3]
+• Multi citation with post note [1–3, for more]
+• Multi citation with pre/post notes [see 1–3, for more]
 
-7
+8
 
 Tables
 • Table 1
 • Table 2
 Col1
 
 Col2
@@ -260,15 +271,15 @@
 
 70
 
 72
 
 Table 2: Wide table
 
-8
+9
 
 Figures
 
 a Example footnote text.
 
 Figure 2: Narrow figure
 
@@ -341,23 +352,23 @@
 
 10
 
 x
 
 15
 
-b: Figure with ‘width=3.5in’a
-Figure 4: Sub-figuresb
+b: Figure with ‘width=3.5in’ a
+Figure 4: Sub-figures b
 
-9
+10
 
 Includes
+
 • Commands from metadata include: arg min R
 • Include command in body (there should be text after this):
-
 Content added through include statement.
 
 References
 
 [1] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle, and
 Chris Rowley. The LATEX Companion. Addison-Wesley Professional, 2 edition,
 2004.
```

### Comparing `shiny_mdc-1.3.0/test/samples/stylish.pdf` & `shiny_mdc-1.3.1/test/samples/stylish.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -11,17 +11,19 @@
 
 Author Four
 author4@author4.com
 
 Author Number Five2
 authornumberfive@institutetwo.edu
 
+Markdown in abstract. x + 2. Section 1. Reference
+
 [1]
 
-Markdown in abstract. x + 2. Section 1. Reference .
+.
 
 1. Section
 Integer at enim eu tellus malesuada scelerisque. Ut sed rhoncus ipsum, at tempor nisl. Vivamus vitae pulvinar leo, at
 pharetra massa. Ut lobortis odio non nulla tincidunt pulvinar.
 Nunc faucibus pellentesque elit, non ornare risus suscipit sed.
 Maecenas vel blandit ex.
 Phasellus ultrices mi non nulla hendrerit, at rhoncus augue suscipit. Pellentesque a lectus eget felis maximus feugiat
@@ -182,99 +184,118 @@
 
 Table 2: Wide table
 
 2. Typography
 
 • Appendix table: Table B1
 • Appendix math: Equation 4
-• Short citation [²]
-• Long citation: Mittelbach et al. (2004) [²], Lesk and
-Kernighan (1977)[³]
-• Multi citation [²𝄒³𝄒⁴]
-• Pointer to footnote¹
+• Pointer to footnote ¹
 
 • Bold
 • Italic
 • Bold italic.
 
 3. Numbers
 • Normal: 0123456789
 • Math: 0123456789
 
-7. Tables
-• Table 1
-• Table 2
+¹ Example footnote text.
+
+7. Citations
 
 4. Acronyms
 • Default (short+long): Carnegie Mellon University
 (CMU)
 • Repeated (short): CMU
 • Forced short: USA
 • Repeated after forced short (short+long): United States
 of America (USA)
 • Plural: social security numbers (SSNs)
 
-Col1
+5. Math
+Z ∞
 
-Col2
+2
 
-Col3
+exp−x dx
 
-Col4
+0
+
+(1)
 
+• Short citation[²]
+• Short citation with pre note[ˢᵉᵉ ²]
+• Short citation with post note[²𝄒 ᵖ⋅ ¹]
+• Short citation with pre/post notes[ˢᵉᵉ ²𝄒 ᵖ⋅ ¹]
+• Long citation: Lesk and Kernighan (1977)[³]
+• Long citation with note: Lesk and Kernighan
+(1977)[³𝄒 ᵖ⋅ ¹]
+• Multi citation[²𝄒 ³𝄒 ⁴]
+• Multi citation with pre note[ˢᵉᵉ ²𝄒 ³𝄒 ⁴]
+• Multi citation with post note[²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+• Multi citation with pre/post notes[ˢᵉᵉ ²𝄒 ³𝄒 ⁴𝄒 ᶠᵒʳ ᵐᵒʳᵉ]
+
+8. Tables
+
+1 6, 7, 8, 9
+a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1,•2,Table
+3, 4, 5,
+•
+Table
+2
+(2)
+R∞
+2
+• Inline: 0 exp−x dx
+• Block: Equation 1, Equation 2
+Col1
+• Commands defined in body (P[x in X]): P[x ∈ X ]
 1
+• Aligned:
 11
 111
 
+Col2
+
+Col3
+
+Col4
+
 2
 22
 222
 
 3
 33
 333
 
 4
 44
 444
 
 Table 1: Short table
 
-5. Math
-Z ∞
-
-2
-
-exp−x dx
-
-0
-
-(1)
-
-8. Figures
-
-a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
-(2)
-R∞
-2
-• Inline: 0 exp−x dx
-• Block: Equation 1, Equation 2
-• Commands defined in body (P[x in X]): P[x ∈ X ]
-• Aligned:
 x=1
 x + y = 10
 x + y + z = 100
 
 6. Links
 • Section: Section 1, Section 1.2
 • Appendix section: Section B, Section A.1.1
 • Appendix figure: Figure A1
-Figure 2: Narrow figure
+
+9. Figures
+• Figure 2
+• Figure 3
+• Figure 4, Figure 4a, Figure 4b
+
 2
 
+² Footnote in sub-figure caption.
+
 A
 B
 C
 D
 E
 F
 G
@@ -298,41 +319,15 @@
 
 74
 
 76
 
 Figure 3: Wide figure
 
-• Figure 2
-• Figure 3
-• Figure 4, Figure 4a, Figure 4b
-
-9. Includes
-• Commands from metadata include: arg min R
-• Include command in body (there should be text after
-this):
-Content added through include statement.
-
-References
-[1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
-[2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
-and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
-2 edition, 2004.
-[3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
-journals on UNIX. In Proceedings of American Federation of Information Processing Societies: 1977 National Computer Conference, pages
-879–888, Dallas, Texas, 1977.
-[4] Donald E. Knuth. Literate programming. The Computer Journal, 27(2):
-97–111, 1984.
-
-² Footnote in sub-figure caption.
-³ Footnote in figure caption.
-
-3
-
-dataset = I
+dataset = I
 
 dataset = II
 
 dataset = III
 
 dataset = IV
 
@@ -366,17 +361,38 @@
 
 10
 
 x
 
 15
 
-(b) Figure with ‘width=3.5in’²
+(b) Figure with ‘width=3.5in’ ²
+
+Figure 4: Sub-figures ³
+
+3
+
+10. Includes
+• Commands from metadata include: arg min R
+• Include command in body (there should be text after
+this):
+Content added through include statement.
 
-Figure 4: Sub-figures³
+References
+[1] Donald E. Knuth. The TEX Book. Addison-Wesley Professional, 1986.
+[2] Frank Mittelbach, Michel Gossens, Johannes Braams, David Carlisle,
+and Chris Rowley. The LATEX Companion. Addison-Wesley Professional,
+2 edition, 2004.
+[3] Michael Lesk and Brian Kernighan. Computer typesetting of technical
+journals on UNIX. In Proceedings of American Federation of Information Processing Societies: 1977 National Computer Conference, pages
+879–888, Dallas, Texas, 1977.
+[4] Donald E. Knuth. Literate programming. The Computer Journal, 27(2):
+97–111, 1984.
+
+Figure 2: Narrow figure
 
 4
 
 A
 B
 C
 D
@@ -439,15 +455,15 @@
 
 A.4 Appendix links
 • Appendix section: Section A.1.1, Section B
 • Main body section: Section 1
 • Main body figure: Figure 2
 • Main body table: Table 1
 • Main body equation: Equation 1
-• Citation: Knuth (1984) [⁴]
+• Citation: Knuth (1984)[⁴]
 
 5
 
 (a) Figure with non-default extension
 
 (b) Sub-figure
 
@@ -602,15 +618,15 @@
 567
 89
 
 9876
 543
 21
 
-Table B1: Extra wide table³
+Table B1: Extra wide table ³
 
 Appendix B
 
 Appendix 2
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam nisi purus, bibendum non neque sed, lacinia tristique
 tortor. Vestibulum eu lectus sed velit luctus varius. Sed sollicitudin ligula ante. Integer porta a erat commodo dignissim.
```

### Comparing `shiny_mdc-1.3.0/test/sections/appendix1.md` & `shiny_mdc-1.3.1/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/test/sections/appendix2.md` & `shiny_mdc-1.3.1/test/sections/appendix2.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 dignissim. Duis et lectus diam. Nulla id erat vestibulum nisi placerat
 efficitur. Nulla a semper libero.
 
 ## Appendix tables
 
 * @tbl:app2ex1
 
-Col1       Col2     Col3     Col4     Col5     Col6     Col7     Col8     Col9     Col10     Col11     Col12     Col13     Col14     Col15     Col16     Col17   Col17
-------   ------   ------   ------   ------   ------   ------   ------   ------   -------   -------   -------   -------   -------   -------   -------   -------   -------
-a             1        2        3      123     abcd     1234      444        a       bbb      cccc       ddd      eeee       fff      gggg      abcd      1234   9876
-b            11       22       33      456     efgh      567       44       aa        bb      cccc        dd      eeee        ff      gggg      efgh       567   543
-c           111      222      333      789     ijkl       89    4[^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
+Col1       Col2     Col3     Col4     Col5     Col6     Col7      Col8     Col9     Col10     Col11     Col12     Col13     Col14     Col15     Col16     Col17   Col17
+------   ------   ------   ------   ------   ------   ------   -------   ------   -------   -------   -------   -------   -------   -------   -------   -------   -------
+a             1        2        3      123     abcd     1234       444        a       bbb      cccc       ddd      eeee       fff      gggg      abcd      1234   9876
+b            11       22       33      456     efgh      567        44       aa        bb      cccc        dd      eeee        ff      gggg      efgh       567   543
+c           111      222      333      789     ijkl       89    4 [^t]      aaa         b      cccc         d      eeee         f      gggg      ijkl        89   21
 
-: Extra wide table[^u] {#tbl:app2ex1}
+: Extra wide table [^u] {#tbl:app2ex1}
 
 [^t]: Footnote in table.
 [^u]: Footnote in table caption.
 
 ## Appendix math
 
 $$
```

### Comparing `shiny_mdc-1.3.0/test/sections/main1.md` & `shiny_mdc-1.3.1/test/sections/main1.md`

 * *Files 20% similar despite different names*

```diff
@@ -56,13 +56,23 @@
 # Links
 
 * Section: @sec:ex1, @sec:ex1.2
 * Appendix section: @sec:app2ex1, @sec:app1ex1.1.1
 * Appendix figure: @fig:app1ex1
 * Appendix table: @tbl:app2ex1
 * Appendix math: @eq:app2ex2
-* Short citation[@latex:companion]
-* Long citation: @latex:companion, @lesk:1977
-* Multi citation[@lesk:1977; @knuth:1984; @latex:companion]
-* Pointer to footnote[^1]
+* Pointer to footnote [^1]
 
 [^1]: Example footnote text.
+
+# Citations
+
+* Short citation [@latex:companion]
+* Short citation with pre note [see @latex:companion]
+* Short citation with post note [@latex:companion, p. 1]
+* Short citation with pre/post notes [see @latex:companion, p. 1]
+* Long citation: @lesk:1977
+* Long citation with note: @lesk:1977 [p. 1]
+* Multi citation [@lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with pre note [see @lesk:1977; @knuth:1984; @latex:companion]
+* Multi citation with post note [@lesk:1977; @knuth:1984; @latex:companion, for more]
+* Multi citation with pre/post notes [see @lesk:1977; @knuth:1984; @latex:companion, for more]
```

### Comparing `shiny_mdc-1.3.0/test/sections/main2.md` & `shiny_mdc-1.3.1/test/sections/main2.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 * @fig:ex2
 * @fig:ex3, @fig:ex3a, @fig:ex3b
 
 <div id="fig:ex3">
 
 ![Figure with 'width=2.5in'](figures/gaussian2d){#fig:ex3a width=2.5in}
 
-![Figure with 'width=3.5in'[^f]](figures/anscombe){#fig:ex3b width=3.5in}
+![Figure with 'width=3.5in' [^f]](figures/anscombe){#fig:ex3b width=3.5in}
 
-Sub-figures[^g]
+Sub-figures [^g]
 </div>
 
 [^f]: Footnote in sub-figure caption.
 [^g]: Footnote in figure caption.
 
 
 # Includes {#sec:includes}
```

### Comparing `shiny_mdc-1.3.0/test/utils/commands.md` & `shiny_mdc-1.3.1/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.3.0/PKG-INFO` & `shiny_mdc-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

