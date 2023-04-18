# Comparing `tmp/dnxmy-1.0.0.tar.gz` & `tmp/dnxmy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnxmy-1.0.0.tar", last modified: Tue Apr  4 13:06:02 2023, max compression
+gzip compressed data, was "dnxmy-1.0.1.tar", last modified: Tue Apr 18 13:52:55 2023, max compression
```

## Comparing `dnxmy-1.0.0.tar` & `dnxmy-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-04 13:06:02.929756 dnxmy-1.0.0/
--rw-r--r--   0 s11528   (906015332) 1796141739     2731 2023-04-04 13:06:02.929488 dnxmy-1.0.0/PKG-INFO
--rw-r--r--   0 s11528   (906015332) 1796141739     1189 2023-04-04 07:08:27.000000 dnxmy-1.0.0/README.md
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-04 13:06:02.926199 dnxmy-1.0.0/dnxmy/
--rw-r--r--   0 s11528   (906015332) 1796141739      109 2023-04-04 11:35:11.000000 dnxmy-1.0.0/dnxmy/__init__.py
--rw-r--r--   0 s11528   (906015332) 1796141739    11470 2023-04-04 11:18:13.000000 dnxmy-1.0.0/dnxmy/config_generator.py
--rw-r--r--   0 s11528   (906015332) 1796141739     6054 2023-04-04 11:18:12.000000 dnxmy-1.0.0/dnxmy/dnxmy.py
--rw-r--r--   0 s11528   (906015332) 1796141739     7136 2023-04-04 09:54:41.000000 dnxmy-1.0.0/dnxmy/variable_generator.py
-drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-04 13:06:02.928854 dnxmy-1.0.0/dnxmy.egg-info/
--rw-r--r--   0 s11528   (906015332) 1796141739     2731 2023-04-04 13:06:02.000000 dnxmy-1.0.0/dnxmy.egg-info/PKG-INFO
--rw-r--r--   0 s11528   (906015332) 1796141739      249 2023-04-04 13:06:02.000000 dnxmy-1.0.0/dnxmy.egg-info/SOURCES.txt
--rw-r--r--   0 s11528   (906015332) 1796141739        1 2023-04-04 13:06:02.000000 dnxmy-1.0.0/dnxmy.egg-info/dependency_links.txt
--rw-r--r--   0 s11528   (906015332) 1796141739       28 2023-04-04 13:06:02.000000 dnxmy-1.0.0/dnxmy.egg-info/requires.txt
--rw-r--r--   0 s11528   (906015332) 1796141739        6 2023-04-04 13:06:02.000000 dnxmy-1.0.0/dnxmy.egg-info/top_level.txt
--rw-r--r--   0 s11528   (906015332) 1796141739       38 2023-04-04 13:06:02.929915 dnxmy-1.0.0/setup.cfg
--rw-r--r--   0 s11528   (906015332) 1796141739     1743 2023-04-02 14:55:19.000000 dnxmy-1.0.0/setup.py
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.343425 dnxmy-1.0.1/
+-rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-04-18 13:52:55.343123 dnxmy-1.0.1/PKG-INFO
+-rw-r--r--   0 s11528   (906015332) 1796141739     1487 2023-04-18 08:08:38.000000 dnxmy-1.0.1/README.md
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.339189 dnxmy-1.0.1/dnxmy/
+-rw-r--r--   0 s11528   (906015332) 1796141739      109 2023-04-18 08:08:47.000000 dnxmy-1.0.1/dnxmy/__init__.py
+-rw-r--r--   0 s11528   (906015332) 1796141739    11965 2023-04-18 07:46:21.000000 dnxmy-1.0.1/dnxmy/config_generator.py
+-rw-r--r--   0 s11528   (906015332) 1796141739     6054 2023-04-04 11:18:12.000000 dnxmy-1.0.1/dnxmy/dnxmy.py
+-rw-r--r--   0 s11528   (906015332) 1796141739     7144 2023-04-18 07:17:29.000000 dnxmy-1.0.1/dnxmy/variable_generator.py
+drwxr-xr-x   0 s11528   (906015332) 1796141739        0 2023-04-18 13:52:55.342032 dnxmy-1.0.1/dnxmy.egg-info/
+-rw-r--r--   0 s11528   (906015332) 1796141739     3037 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/PKG-INFO
+-rw-r--r--   0 s11528   (906015332) 1796141739      249 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/SOURCES.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739        1 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/dependency_links.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739       28 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/requires.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739        6 2023-04-18 13:52:55.000000 dnxmy-1.0.1/dnxmy.egg-info/top_level.txt
+-rw-r--r--   0 s11528   (906015332) 1796141739       38 2023-04-18 13:52:55.343557 dnxmy-1.0.1/setup.cfg
+-rw-r--r--   0 s11528   (906015332) 1796141739     1743 2023-04-02 14:55:19.000000 dnxmy-1.0.1/setup.py
```

### Comparing `dnxmy-1.0.0/PKG-INFO` & `dnxmy-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnxmy
-Version: 1.0.0
+Version: 1.0.1
 Summary: dnxmy: dummy data generator for machine learning and statistics
 Home-page: https://github.com/roseiricho/dnxmy
 Author: Yuki Yamamoto
 Author-email: curious.yamamon@gmail.com
 Maintainer: Yuki Yamamoto
 Maintainer-email: curious.yamamon@gmail.com
 License: MIT License
@@ -36,15 +36,16 @@
         ```python
         import dnxmy
         ```
         
         ### Example
         The following notebook is a reference case study using this library.
         
-        - [Example]()
+        - [Experiments on missing data completion](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_missing_data_completion.ipynb)
+        - [Experiments on model selection for AIC and BIC](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_model_selection_for_AIC_and_BIC.ipynb)
         
         ## Support
         Bugs may be reported at [issues](https://github.com/roseiricho/dnxmy/issues).
         
         ## License
         This project is licensed under the MIT License - see the [LICENSE](https://github.com/roseiricho/dnxmy/blob/main/LICENSE) file for details.
```

### Comparing `dnxmy-1.0.0/README.md` & `dnxmy-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 ```python
 import dnxmy
 ```
 
 ### Example
 The following notebook is a reference case study using this library.
 
-- [Example]()
+- [Experiments on missing data completion](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_missing_data_completion.ipynb)
+- [Experiments on model selection for AIC and BIC](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_model_selection_for_AIC_and_BIC.ipynb)
 
 ## Support
 Bugs may be reported at [issues](https://github.com/roseiricho/dnxmy/issues).
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/roseiricho/dnxmy/blob/main/LICENSE) file for details.
```

### Comparing `dnxmy-1.0.0/dnxmy/config_generator.py` & `dnxmy-1.0.1/dnxmy/config_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,25 +179,27 @@
         ma_shock_type (list): List of shock types for the MA part of the ARMA variable.
           Defaults to None.
         ma_shock_value (list): List of shock values for the MA part of the ARMA variable.
           Defaults to None.
     """
     # create a dictionary for the AR shocks
     ar_shock_dict = {}
-    for i, t, v in zip(ar_shock_time, ar_shock_type, ar_shock_value):
-      ar_shock_dict[i] = {}
-      ar_shock_dict[i]['type'] = t
-      ar_shock_dict[i]['value'] = v
+    if ar_shock_time is not None or ar_shock_type is not None or ar_shock_value is not None:
+      for i, t, v in zip(ar_shock_time, ar_shock_type, ar_shock_value):
+        ar_shock_dict[i] = {}
+        ar_shock_dict[i]['type'] = t
+        ar_shock_dict[i]['value'] = v
     
     # create a dictionary for the MA shocks
     ma_shock_dict = {}
-    for i, t, v in zip(ma_shock_time, ma_shock_type, ma_shock_value):
-      ma_shock_dict[i] = {}
-      ma_shock_dict[i]['type'] = t
-      ma_shock_dict[i]['value'] = v
+    if ma_shock_time is not None or ma_shock_type is not None or ma_shock_value is not None:
+      for i, t, v in zip(ma_shock_time, ma_shock_type, ma_shock_value):
+        ma_shock_dict[i] = {}
+        ma_shock_dict[i]['type'] = t
+        ma_shock_dict[i]['value'] = v
 
     # create the column configuration dictionary
     self.dataset_config.append({
       'column_name': col_name,
       'variable_type': 'time_series',
       'time_series_config': {
         'intercept': intercept,
@@ -214,15 +216,15 @@
           'params': ma_params,
           'shock': ma_shock_dict
         }
       }
     })
 
 
-  def add_dependent_colmn(self, 
+  def add_dependent_column(self, 
                           col_name: str, 
                           variables: list, 
                           beta: list, 
                           intercept: float, 
                           offset_column: str = None, 
                           offset_function: str = 'default', 
                           link_function: str = 'identity'):
@@ -252,14 +254,27 @@
         'offset': {
           'column_name': offset_column,
           'function': offset_function
         },
         'link_function': link_function
       }
     })
+  
+  
+  def delete_column_config(self, col_name: str):
+    """
+    Delete a column configuration.
+
+    Args:
+        col_name (str): Name of the column.
+    """
+    for col in self.dataset_config:
+      if col['column_name'] == col_name:
+        self.dataset_config.remove(col)
+        break
 
 
   def t_sort(self):
     """
     Optimize the order of dataset configuration using topological sorting.
     """
     sorted_list = []
```

### Comparing `dnxmy-1.0.0/dnxmy/dnxmy.py` & `dnxmy-1.0.1/dnxmy/dnxmy.py`

 * *Files identical despite different names*

### Comparing `dnxmy-1.0.0/dnxmy/variable_generator.py` & `dnxmy-1.0.1/dnxmy/variable_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,25 +96,25 @@
   arma_samples = [ar_samples[0] + ma_samples[0] + time_series_config['intercept'] + np.random.normal(0, time_series_config['sigma'])]
   
   # generate ARMA samples
   for i in range(1, n):
     ar = sum([ar_params['params'][j] * ar_samples[i - j - 1] for j in range(min(i, ar_params.get('order', 0)))])
     
     # add shock
-    if ar_params['shock'].get(i) is not None:
+    if ar_params.get('shock').get(i) is not None:
       shock_value = ar_params['shock'][i]['value']
       if ar_params['shock'][i]['type'] == 'sigma':
         shock_value *= time_series_config['sigma']
       ar += shock_value
     ar_samples.append(ar)
 
     ma = sum([ma_params['params'][j] * ma_samples[i - j - 1] for j in range(min(i, ma_params.get('order', 0)))])
 
     # add shock
-    if ma_params['shock'].get(i) is not None:
+    if ma_params.get('shock').get(i) is not None:
       shock_value = ma_params['shock'][i]['value']
       if ma_params['shock'][i]['type'] == 'sigma':
         shock_value *= time_series_config['sigma']
       ma += shock_value
     ma_samples.append(ma)
 
     arma_samples.append(ar + ma + np.random.normal(0, time_series_config['sigma']))
```

### Comparing `dnxmy-1.0.0/dnxmy.egg-info/PKG-INFO` & `dnxmy-1.0.1/dnxmy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnxmy
-Version: 1.0.0
+Version: 1.0.1
 Summary: dnxmy: dummy data generator for machine learning and statistics
 Home-page: https://github.com/roseiricho/dnxmy
 Author: Yuki Yamamoto
 Author-email: curious.yamamon@gmail.com
 Maintainer: Yuki Yamamoto
 Maintainer-email: curious.yamamon@gmail.com
 License: MIT License
@@ -36,15 +36,16 @@
         ```python
         import dnxmy
         ```
         
         ### Example
         The following notebook is a reference case study using this library.
         
-        - [Example]()
+        - [Experiments on missing data completion](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_missing_data_completion.ipynb)
+        - [Experiments on model selection for AIC and BIC](https://github.com/roseiricho/analysis-portfolio/blob/main/Experiments_on_model_selection_for_AIC_and_BIC.ipynb)
         
         ## Support
         Bugs may be reported at [issues](https://github.com/roseiricho/dnxmy/issues).
         
         ## License
         This project is licensed under the MIT License - see the [LICENSE](https://github.com/roseiricho/dnxmy/blob/main/LICENSE) file for details.
```

### Comparing `dnxmy-1.0.0/setup.py` & `dnxmy-1.0.1/setup.py`

 * *Files identical despite different names*

