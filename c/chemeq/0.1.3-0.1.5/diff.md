# Comparing `tmp/chemeq-0.1.3.tar.gz` & `tmp/chemeq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemeq-0.1.3.tar", last modified: Sun Apr 16 14:11:37 2023, max compression
+gzip compressed data, was "chemeq-0.1.5.tar", last modified: Tue Apr 18 09:13:08 2023, max compression
```

## Comparing `chemeq-0.1.3.tar` & `chemeq-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:37.360436 chemeq-0.1.3/
--rw-rw-rw-   0        0        0     1083 2023-04-14 23:38:40.000000 chemeq-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       41 2023-04-15 14:14:51.000000 chemeq-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4762 2023-04-16 14:11:37.360436 chemeq-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4085 2023-04-16 14:00:59.000000 chemeq-0.1.3/README.md
--rw-rw-rw-   0        0        0     3839 2023-02-24 23:54:34.000000 chemeq-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:37.320441 chemeq-0.1.3/chemeq/
--rw-rw-rw-   0        0        0     3495 2023-04-16 13:13:37.000000 chemeq-0.1.3/chemeq/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-02-24 23:54:36.000000 chemeq-0.1.3/chemeq/balanced_equations.csv
--rw-rw-rw-   0        0        0     2754 2023-04-13 09:56:06.000000 chemeq-0.1.3/chemeq/count_elements.py
--rw-rw-rw-   0        0        0    15514 2023-04-16 13:22:26.000000 chemeq-0.1.3/chemeq/equation_balancer.py
--rw-rw-rw-   0        0        0     2462 2023-04-04 10:17:48.000000 chemeq-0.1.3/chemeq/periodic_table.csv
--rw-rw-rw-   0        0        0     6522 2023-04-16 13:37:51.000000 chemeq-0.1.3/chemeq/syntax_review.py
--rw-rw-rw-   0        0        0     2182 2023-04-12 10:29:56.000000 chemeq-0.1.3/chemeq/unbalanced_equations.csv
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:37.350446 chemeq-0.1.3/chemeq.egg-info/
--rw-rw-rw-   0        0        0     4762 2023-04-16 14:11:37.000000 chemeq-0.1.3/chemeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-16 14:11:37.000000 chemeq-0.1.3/chemeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:11:37.000000 chemeq-0.1.3/chemeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-16 14:11:37.000000 chemeq-0.1.3/chemeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 14:11:37.000000 chemeq-0.1.3/chemeq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-04-13 14:13:18.000000 chemeq-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 14:11:37.360436 chemeq-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-04-16 14:09:54.000000 chemeq-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:11:37.350446 chemeq-0.1.3/tests/
--rw-rw-rw-   0        0        0     2296 2023-04-13 21:31:02.000000 chemeq-0.1.3/tests/test_base_outputs.py
--rw-rw-rw-   0        0        0     1343 2023-04-14 10:47:52.000000 chemeq-0.1.3/tests/test_syntax.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/
+-rw-rw-rw-   0        0        0     1083 2023-04-14 23:38:40.000000 chemeq-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       41 2023-04-15 14:14:51.000000 chemeq-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4859 2023-04-18 09:13:08.072329 chemeq-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4156 2023-04-17 21:28:54.000000 chemeq-0.1.5/README.md
+-rw-rw-rw-   0        0        0     3839 2023-02-24 23:54:34.000000 chemeq-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.052330 chemeq-0.1.5/chemeq/
+-rw-rw-rw-   0        0        0     3781 2023-04-17 09:13:05.000000 chemeq-0.1.5/chemeq/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-04-13 09:56:06.000000 chemeq-0.1.5/chemeq/count_elements.py
+-rw-rw-rw-   0        0        0    15300 2023-04-17 19:35:13.000000 chemeq-0.1.5/chemeq/equation_balancer.py
+-rw-rw-rw-   0        0        0     2462 2023-04-04 10:17:48.000000 chemeq-0.1.5/chemeq/periodic_table.csv
+-rw-rw-rw-   0        0        0     6512 2023-04-17 19:33:43.000000 chemeq-0.1.5/chemeq/syntax_review.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/chemeq.egg-info/
+-rw-rw-rw-   0        0        0     4859 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-04-13 14:13:18.000000 chemeq-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:13:08.072329 chemeq-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-04-17 21:27:39.000000 chemeq-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/tests/
+-rw-rw-rw-   0        0        0     2296 2023-04-13 21:31:02.000000 chemeq-0.1.5/tests/test_base_outputs.py
+-rw-rw-rw-   0        0        0     1343 2023-04-14 10:47:52.000000 chemeq-0.1.5/tests/test_syntax.py
```

### Comparing `chemeq-0.1.3/LICENSE.txt` & `chemeq-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.3/PKG-INFO` & `chemeq-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 Metadata-Version: 2.1
 Name: chemeq
-Version: 0.1.3
-Summary: Balance chemical equations, calculates molecular weights
+Version: 0.1.5
+Summary: Balance chemical equations & calculates molecular weights
 Home-page: https://github.com/elbiop/chemeq
 Author: Elbio Peña
 Author-email: elbioemilio@outlook.es
 Keywords: chemistry,chemical,chemicals,equation,equations,balance,balancer,balancing,reaction,reactions,periodic table,elements
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## USE
 ```
 pip install chemeq
 ```
 
-## PROJECT DESCRIPTION
+## PROJECT DESCRIPTION  
 
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.
-The package has two objects: **chemeq** and **periodic_table**
+Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**   
 
-### 1. chemeq
-&emsp; CLASS, Receives a string representing a chemical equation  as input.
-&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".
+### 1. chemeq   
+&emsp; CLASS, Receives a string representing a chemical equation  as input.   
+&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
-&emsp; The **chemeq CLASS** has three properties and one method.
+&emsp; The **chemeq CLASS** has three properties and one method.   
 
-&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.
+&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
-### 2. periodic_table
-&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,
-&emsp;  atomic mass error, period, group & state.
+### 2. periodic_table   
+&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
+&emsp;  atomic mass error, period, group & state.   
 
-&emsp;     Source for the periodic table of elements:
-&emsp;     IUPAC - International Union of Pure and Applied Chemistry
-&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/
+&emsp;     Source for the periodic table of elements:   
+&emsp;     IUPAC - International Union of Pure and Applied Chemistry   
+&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/   
 
-## LIMITATIONS
-- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.
-- Intermediate prefixes like those from hydrates such as Cu(SO4)â€¢5H2O
-&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.
+## LIMITATIONS   
+- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.   
+- Intermediate prefixes like those from hydrates such as Cu(SO4)â€¢5H2O   
+&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.   
 
-## EXAMPLES
+## EXAMPLES   
 ```
   >>> from chemeq import chemeq
   >>> eq = chemeq("C2H5(OH) + O2 = CO2 + H2O")
   >>> eq.is_balanced
   False
 ```
   The balance status of the equation is also visible in the equation object itself.
```

### Comparing `chemeq-0.1.3/README.md` & `chemeq-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 ## USE
 ```
 pip install chemeq
 ```
 
-## PROJECT DESCRIPTION
+## PROJECT DESCRIPTION  
 
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.
-The package has two objects: **chemeq** and **periodic_table**
+Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**   
 
-### 1. chemeq
-&emsp; CLASS, Receives a string representing a chemical equation  as input.
-&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".
+### 1. chemeq   
+&emsp; CLASS, Receives a string representing a chemical equation  as input.   
+&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
-&emsp; The **chemeq CLASS** has three properties and one method.
+&emsp; The **chemeq CLASS** has three properties and one method.   
 
-&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.
+&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
-### 2. periodic_table
-&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,
-&emsp;  atomic mass error, period, group & state.
+### 2. periodic_table   
+&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
+&emsp;  atomic mass error, period, group & state.   
 
-&emsp;     Source for the periodic table of elements:
-&emsp;     IUPAC - International Union of Pure and Applied Chemistry
-&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/
+&emsp;     Source for the periodic table of elements:   
+&emsp;     IUPAC - International Union of Pure and Applied Chemistry   
+&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/   
 
-## LIMITATIONS
-- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.
-- Intermediate prefixes like those from hydrates such as Cu(SO4)•5H2O
-&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.
+## LIMITATIONS   
+- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.   
+- Intermediate prefixes like those from hydrates such as Cu(SO4)•5H2O   
+&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.   
 
-## EXAMPLES
+## EXAMPLES   
 ```
   >>> from chemeq import chemeq
   >>> eq = chemeq("C2H5(OH) + O2 = CO2 + H2O")
   >>> eq.is_balanced
   False
 ```
   The balance status of the equation is also visible in the equation object itself.
```

### Comparing `chemeq-0.1.3/README.txt` & `chemeq-0.1.5/README.txt`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.3/chemeq/__init__.py` & `chemeq-0.1.5/chemeq/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,18 +88,26 @@
     if "periodic_table.csv" not in os.listdir():
         with open('periodic_table.csv', 'w') as pt:
             pt.write(PERIODIC_TABLE_CONTENT)
 
     # shorten import paths
     from chemeq.equation_balancer import chemeq
     from chemeq.equation_balancer import periodic_table
+    from chemeq.syntax_review import syntax_review
+    from chemeq.count_elements import count_elements
     os.chdir(CURRENT_PATH)
 else:
     # if not installed run from source location
     sys.path.insert(0, CURRENT_PATH)
     from equation_balancer import chemeq
     from equation_balancer import periodic_table
+    from syntax_review import syntax_review
+    from count_elements import count_elements
 
 
-__all__ = ["chemeq",
-           "periodic_table"]
+__all__ = [
+            "chemeq",
+            "periodic_table",
+            "count_elements",
+            "syntax_review"
+          ]
 __author__ = "Elbio Peña Almonte"
```

### Comparing `chemeq-0.1.3/chemeq/count_elements.py` & `chemeq-0.1.5/chemeq/count_elements.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.3/chemeq/equation_balancer.py` & `chemeq-0.1.5/chemeq/equation_balancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 installed = util.find_spec("chemeq")
 
 # Different imports if package is installed or in source directory
 if installed.has_location:
     # if installed run installed version
     INSTALLATION_PATH = installed.submodule_search_locations[0] + os.sep
     os.chdir(INSTALLATION_PATH)
-    # shorten import paths
-    from chemeq.syntax_review import syntax_review
-    from chemeq.count_elements import count_elements
-    periodic_table = pd.read_csv("periodic_table.csv", header=3)
-    os.chdir(CURRENT_PATH)
 else:
     # if not installed run from source location
     sys.path.insert(0, CURRENT_PATH)
-    from syntax_review import syntax_review
-    from count_elements import count_elements
-    periodic_table = pd.read_csv("periodic_table.csv", header=3)
 
+from syntax_review import syntax_review
+from count_elements import count_elements
+os.chdir(CURRENT_PATH)
+
+periodic_table = pd.read_csv("periodic_table.csv", header=3)
 
 
 class chemeq():
     '''CLASS that receives a string representing a chemical equation of the
     form:
     "reactant_1 + ... + reactant_n  = product_1 + ... + product_n"
```

### Comparing `chemeq-0.1.3/chemeq/periodic_table.csv` & `chemeq-0.1.5/chemeq/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.3/chemeq/syntax_review.py` & `chemeq-0.1.5/chemeq/syntax_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 import re
 import pandas as pd
 from importlib import util
 
 CURRENT_PATH = os.path.abspath(".")
 
 # if package is installed change to installation directory
@@ -11,14 +10,15 @@
 if installed.has_location:
     INSTALLATION_PATH = installed.submodule_search_locations[0] + os.sep
     os.chdir(INSTALLATION_PATH)
 
 periodic_table = pd.read_csv("periodic_table.csv", header=3)
 os.chdir(CURRENT_PATH)
 
+
 def syntax_review(equation):
     '''Verify the chemical equation syntax and if it is correct, returns
     the reactants and products compounds and a list of the present elements
 
     equation: type str. represents chemical equation.
     all_symbols: type list[str], symbols for all chemical elements.
     return: type list[str], reactants formulas witout prefix (molar values),
```

### Comparing `chemeq-0.1.3/chemeq.egg-info/PKG-INFO` & `chemeq-0.1.5/chemeq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 Metadata-Version: 2.1
 Name: chemeq
-Version: 0.1.3
-Summary: Balance chemical equations, calculates molecular weights
+Version: 0.1.5
+Summary: Balance chemical equations & calculates molecular weights
 Home-page: https://github.com/elbiop/chemeq
 Author: Elbio Peña
 Author-email: elbioemilio@outlook.es
 Keywords: chemistry,chemical,chemicals,equation,equations,balance,balancer,balancing,reaction,reactions,periodic table,elements
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## USE
 ```
 pip install chemeq
 ```
 
-## PROJECT DESCRIPTION
+## PROJECT DESCRIPTION  
 
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.
-The package has two objects: **chemeq** and **periodic_table**
+Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**   
 
-### 1. chemeq
-&emsp; CLASS, Receives a string representing a chemical equation  as input.
-&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".
+### 1. chemeq   
+&emsp; CLASS, Receives a string representing a chemical equation  as input.   
+&emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
-&emsp; The **chemeq CLASS** has three properties and one method.
+&emsp; The **chemeq CLASS** has three properties and one method.   
 
-&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.
-&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.
+&emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
-### 2. periodic_table
-&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,
-&emsp;  atomic mass error, period, group & state.
+### 2. periodic_table   
+&emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
+&emsp;  atomic mass error, period, group & state.   
 
-&emsp;     Source for the periodic table of elements:
-&emsp;     IUPAC - International Union of Pure and Applied Chemistry
-&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/
+&emsp;     Source for the periodic table of elements:   
+&emsp;     IUPAC - International Union of Pure and Applied Chemistry   
+&emsp;     https://iupac.org/what-we-do/periodic-table-of-elements/   
 
-## LIMITATIONS
-- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.
-- Intermediate prefixes like those from hydrates such as Cu(SO4)â€¢5H2O
-&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.
+## LIMITATIONS   
+- Does not include Rare earths, synthetic elements, Radon, Francium & Radium.   
+- Intermediate prefixes like those from hydrates such as Cu(SO4)â€¢5H2O   
+&emsp; must be represented with subindexes like Cu(SO4)(H2O)5.   
 
-## EXAMPLES
+## EXAMPLES   
 ```
   >>> from chemeq import chemeq
   >>> eq = chemeq("C2H5(OH) + O2 = CO2 + H2O")
   >>> eq.is_balanced
   False
 ```
   The balance status of the equation is also visible in the equation object itself.
```

### Comparing `chemeq-0.1.3/setup.py` & `chemeq-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import setuptools
 
 
 LONG_DESC = open("README.md", "r").read()
 
 setuptools.setup(
     name='chemeq',
-    version='0.1.3',
-    description='''Balance chemical equations, calculates molecular weights
-    of reactants and products and provides a DataFrame with the periodic table
-    of elements''',
+    version='0.1.5',
+    description="Balance chemical equations & calculates molecular weights",
     long_description=LONG_DESC,
     long_description_content_type="text/markdown",
-    readme="README.md",
     author="Elbio Peña",
     author_email="elbioemilio@outlook.es",
 
     packages=setuptools.find_packages(where="."),
     package_dir={"": "."},
     package_data={"chemeq": ["chemeq/*.csv"], "": ["README.md"]},
     include_package_data=True,
     exclude_package_data={"chemeq": [".gitignore"]},
-    requires_python=">= 3.6",
+    python_requires=">= 3.6",
     install_requires=["numpy", "pandas"],
     keywords=["chemistry", "chemical", "chemicals", "equation",
               "equations", "balance", "balancer", "balancing", "reaction",
               "reactions", "periodic table", "elements"],
 
     classifiers=["Development Status :: 5 - Production/Stable",
                  "Programming Language :: Python :: 3",
```

### Comparing `chemeq-0.1.3/tests/test_base_outputs.py` & `chemeq-0.1.5/tests/test_base_outputs.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.3/tests/test_syntax.py` & `chemeq-0.1.5/tests/test_syntax.py`

 * *Files identical despite different names*

