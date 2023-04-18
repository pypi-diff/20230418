# Comparing `tmp/chemeq-0.1.5.tar.gz` & `tmp/chemeq-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemeq-0.1.5.tar", last modified: Tue Apr 18 09:13:08 2023, max compression
+gzip compressed data, was "chemeq-0.1.7.tar", last modified: Tue Apr 18 09:41:42 2023, max compression
```

## Comparing `chemeq-0.1.5.tar` & `chemeq-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/
--rw-rw-rw-   0        0        0     1083 2023-04-14 23:38:40.000000 chemeq-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       41 2023-04-15 14:14:51.000000 chemeq-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4859 2023-04-18 09:13:08.072329 chemeq-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4156 2023-04-17 21:28:54.000000 chemeq-0.1.5/README.md
--rw-rw-rw-   0        0        0     3839 2023-02-24 23:54:34.000000 chemeq-0.1.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.052330 chemeq-0.1.5/chemeq/
--rw-rw-rw-   0        0        0     3781 2023-04-17 09:13:05.000000 chemeq-0.1.5/chemeq/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-04-13 09:56:06.000000 chemeq-0.1.5/chemeq/count_elements.py
--rw-rw-rw-   0        0        0    15300 2023-04-17 19:35:13.000000 chemeq-0.1.5/chemeq/equation_balancer.py
--rw-rw-rw-   0        0        0     2462 2023-04-04 10:17:48.000000 chemeq-0.1.5/chemeq/periodic_table.csv
--rw-rw-rw-   0        0        0     6512 2023-04-17 19:33:43.000000 chemeq-0.1.5/chemeq/syntax_review.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/chemeq.egg-info/
--rw-rw-rw-   0        0        0     4859 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:13:08.000000 chemeq-0.1.5/chemeq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-04-13 14:13:18.000000 chemeq-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 09:13:08.072329 chemeq-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-04-17 21:27:39.000000 chemeq-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:13:08.072329 chemeq-0.1.5/tests/
--rw-rw-rw-   0        0        0     2296 2023-04-13 21:31:02.000000 chemeq-0.1.5/tests/test_base_outputs.py
--rw-rw-rw-   0        0        0     1343 2023-04-14 10:47:52.000000 chemeq-0.1.5/tests/test_syntax.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:41:42.757483 chemeq-0.1.7/
+-rw-rw-rw-   0        0        0     1083 2023-04-14 23:38:40.000000 chemeq-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       41 2023-04-15 14:14:51.000000 chemeq-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4832 2023-04-18 09:41:42.757483 chemeq-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4097 2023-04-18 09:38:01.000000 chemeq-0.1.7/README.md
+-rw-rw-rw-   0        0        0     3839 2023-02-24 23:54:34.000000 chemeq-0.1.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:41:42.747484 chemeq-0.1.7/chemeq/
+-rw-rw-rw-   0        0        0     3781 2023-04-17 09:13:05.000000 chemeq-0.1.7/chemeq/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-04-13 09:56:06.000000 chemeq-0.1.7/chemeq/count_elements.py
+-rw-rw-rw-   0        0        0    15300 2023-04-17 19:35:13.000000 chemeq-0.1.7/chemeq/equation_balancer.py
+-rw-rw-rw-   0        0        0     2462 2023-04-04 10:17:48.000000 chemeq-0.1.7/chemeq/periodic_table.csv
+-rw-rw-rw-   0        0        0     6512 2023-04-17 19:33:43.000000 chemeq-0.1.7/chemeq/syntax_review.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:41:42.757483 chemeq-0.1.7/chemeq.egg-info/
+-rw-rw-rw-   0        0        0     4832 2023-04-18 09:41:42.000000 chemeq-0.1.7/chemeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-04-18 09:41:42.000000 chemeq-0.1.7/chemeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:41:42.000000 chemeq-0.1.7/chemeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 09:41:42.000000 chemeq-0.1.7/chemeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:41:42.000000 chemeq-0.1.7/chemeq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-04-13 14:13:18.000000 chemeq-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:41:42.757483 chemeq-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-04-18 09:41:05.000000 chemeq-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:41:42.757483 chemeq-0.1.7/tests/
+-rw-rw-rw-   0        0        0     2296 2023-04-13 21:31:02.000000 chemeq-0.1.7/tests/test_base_outputs.py
+-rw-rw-rw-   0        0        0     1343 2023-04-14 10:47:52.000000 chemeq-0.1.7/tests/test_syntax.py
```

### Comparing `chemeq-0.1.5/LICENSE.txt` & `chemeq-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/PKG-INFO` & `chemeq-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 Metadata-Version: 2.1
 Name: chemeq
-Version: 0.1.5
-Summary: Balance chemical equations & calculates molecular weights
+Version: 0.1.7
+Summary: Balance chemical equations & calculates molecular weights plus periodic table of elements
 Home-page: https://github.com/elbiop/chemeq
 Author: Elbio Peña
 Author-email: elbioemilio@outlook.es
 Keywords: chemistry,chemical,chemicals,equation,equations,balance,balancer,balancing,reaction,reactions,periodic table,elements
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## USE
-```
-pip install chemeq
-```
 
-## PROJECT DESCRIPTION  
-
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
-The package has two objects: **chemeq** and **periodic_table**   
+Package capable of balance chemical equations and contains the most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**.   
 
 ### 1. chemeq   
 &emsp; CLASS, Receives a string representing a chemical equation  as input.   
 &emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
 &emsp; The **chemeq CLASS** has three properties and one method.   
 
 &emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds,  molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds, molecular weights and elements.   
 &emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
 ### 2. periodic_table   
 &emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
 &emsp;  atomic mass error, period, group & state.
```

### Comparing `chemeq-0.1.5/README.md` & `chemeq-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-## USE
-```
-pip install chemeq
-```
 
-## PROJECT DESCRIPTION  
-
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
-The package has two objects: **chemeq** and **periodic_table**   
+Package capable of balance chemical equations and contains the most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**.   
 
 ### 1. chemeq   
 &emsp; CLASS, Receives a string representing a chemical equation  as input.   
 &emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
 &emsp; The **chemeq CLASS** has three properties and one method.   
 
 &emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds,  molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds, molecular weights and elements.   
 &emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
 ### 2. periodic_table   
 &emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
 &emsp;  atomic mass error, period, group & state.
```

### Comparing `chemeq-0.1.5/README.txt` & `chemeq-0.1.7/README.txt`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq/__init__.py` & `chemeq-0.1.7/chemeq/__init__.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq/count_elements.py` & `chemeq-0.1.7/chemeq/count_elements.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq/equation_balancer.py` & `chemeq-0.1.7/chemeq/equation_balancer.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq/periodic_table.csv` & `chemeq-0.1.7/chemeq/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq/syntax_review.py` & `chemeq-0.1.7/chemeq/syntax_review.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/chemeq.egg-info/PKG-INFO` & `chemeq-0.1.7/chemeq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 Metadata-Version: 2.1
 Name: chemeq
-Version: 0.1.5
-Summary: Balance chemical equations & calculates molecular weights
+Version: 0.1.7
+Summary: Balance chemical equations & calculates molecular weights plus periodic table of elements
 Home-page: https://github.com/elbiop/chemeq
 Author: Elbio Peña
 Author-email: elbioemilio@outlook.es
 Keywords: chemistry,chemical,chemicals,equation,equations,balance,balancer,balancing,reaction,reactions,periodic table,elements
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## USE
-```
-pip install chemeq
-```
 
-## PROJECT DESCRIPTION  
-
-Package capable of balance chemical equations and containsthe most used portion of the periodic table of elements.   
-The package has two objects: **chemeq** and **periodic_table**   
+Package capable of balance chemical equations and contains the most used portion of the periodic table of elements.   
+The package has two objects: **chemeq** and **periodic_table**.   
 
 ### 1. chemeq   
 &emsp; CLASS, Receives a string representing a chemical equation  as input.   
 &emsp; In the shape: "reactant_1 + ... + reactant_n  = product_1 + ... + product_n".   
 
 &emsp; The **chemeq CLASS** has three properties and one method.   
 
 &emsp;&emsp;      **is_balanced** : Property. Boolean (True or False)   
-&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
-&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side) compounds,   
-&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; molecular weights and elements.   
+&emsp;&emsp;      **reactants** &emsp;: Property. pandas.DtataFrame where each row represents one of the reactants (left side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds,  molecular weights and elements.   
+&emsp;&emsp;      **products** &emsp; : Property. pandas.DtataFrame where each row represents one of the product (right side)   
+&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;   compounds, molecular weights and elements.   
 &emsp;&emsp;      **balance()** &emsp; : Method. Balances the equation if it is unbalanced.   
 
 
 ### 2. periodic_table   
 &emsp;  pandas.DataFrame containing a portion of the periodic table of elements contains: Z, name, symbol, atomic mass,   
 &emsp;  atomic mass error, period, group & state.
```

### Comparing `chemeq-0.1.5/setup.py` & `chemeq-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 
 LONG_DESC = open("README.md", "r").read()
 
 setuptools.setup(
     name='chemeq',
-    version='0.1.5',
-    description="Balance chemical equations & calculates molecular weights",
+    version='0.1.7',
+    description="Balance chemical equations & calculates molecular weights plus periodic table of elements",
     long_description=LONG_DESC,
     long_description_content_type="text/markdown",
     author="Elbio Peña",
     author_email="elbioemilio@outlook.es",
 
     packages=setuptools.find_packages(where="."),
     package_dir={"": "."},
```

### Comparing `chemeq-0.1.5/tests/test_base_outputs.py` & `chemeq-0.1.7/tests/test_base_outputs.py`

 * *Files identical despite different names*

### Comparing `chemeq-0.1.5/tests/test_syntax.py` & `chemeq-0.1.7/tests/test_syntax.py`

 * *Files identical despite different names*

