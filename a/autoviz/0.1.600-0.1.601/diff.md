# Comparing `tmp/autoviz-0.1.600.tar.gz` & `tmp/autoviz-0.1.601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.600.tar", last modified: Mon Apr 17 00:33:02 2023, max compression
+gzip compressed data, was "autoviz-0.1.601.tar", last modified: Tue Apr 18 13:24:18 2023, max compression
```

## Comparing `autoviz-0.1.600.tar` & `autoviz-0.1.601.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.204645 autoviz-0.1.600/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14022 2023-04-17 00:33:02.204645 autoviz-0.1.600/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12210 2023-04-17 00:30:21.000000 autoviz-0.1.600/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.064021 autoviz-0.1.600/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    29545 2023-04-17 00:09:26.000000 autoviz-0.1.600/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   116997 2023-04-17 00:20:44.000000 autoviz-0.1.600/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.600/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-04-17 00:23:53.000000 autoviz-0.1.600/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24238 2022-10-02 22:52:36.000000 autoviz-0.1.600/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-17 00:33:02.173395 autoviz-0.1.600/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14022 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-04-17 00:33:01.000000 autoviz-0.1.600/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-17 00:33:02.204645 autoviz-0.1.600/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-04-17 00:22:39.000000 autoviz-0.1.600/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.485915 autoviz-0.1.601/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14161 2023-04-18 13:24:18.470300 autoviz-0.1.601/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12342 2023-04-18 13:22:22.000000 autoviz-0.1.601/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.338756 autoviz-0.1.601/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    30554 2023-04-18 12:33:51.000000 autoviz-0.1.601/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117576 2023-04-18 13:15:24.000000 autoviz-0.1.601/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-04-18 11:01:32.000000 autoviz-0.1.601/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.601/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.454671 autoviz-0.1.601/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    14161 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-18 13:24:18.485915 autoviz-0.1.601/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-04-18 13:18:30.000000 autoviz-0.1.601/setup.py
```

### Comparing `autoviz-0.1.600/PKG-INFO` & `autoviz-0.1.601/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.600
+Version: 0.1.601
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz
         
         Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
@@ -65,26 +65,27 @@
         pip install -r requirements.txt
         ```
         
         ## Usage
         
         Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
         
-        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the library
+        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
+        <b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
+        Instead, you can simply do<br>
         
         ```py
-        from autoviz.AutoViz_Class import AutoViz_Class
-        
+        from autoviz import AutoViz_Class
         AV = AutoViz_Class()
         ```
         
         Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
         If you don't have a filename, you can simply assign the filename argument `""` (empty string).
         
-        Call AutoViz using the filename (or dataframe) along with the separator and the name of the target variable in the input.
+        Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
         
         ```py
         filename = ""
         sep = ","
         dft = AV.AutoViz(
             filename,
             sep=",",
```

### Comparing `autoviz-0.1.600/README.md` & `autoviz-0.1.601/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,27 @@
 pip install -r requirements.txt
 ```
 
 ## Usage
 
 Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
 
-In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the library
+In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
+<b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
+Instead, you can simply do<br>
 
 ```py
-from autoviz.AutoViz_Class import AutoViz_Class
-
+from autoviz import AutoViz_Class
 AV = AutoViz_Class()
 ```
 
 Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
 If you don't have a filename, you can simply assign the filename argument `""` (empty string).
 
-Call AutoViz using the filename (or dataframe) along with the separator and the name of the target variable in the input.
+Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
 
 ```py
 filename = ""
 sep = ","
 dft = AV.AutoViz(
     filename,
     sep=",",
```

### Comparing `autoviz-0.1.600/autoviz/AutoViz_Class.py` & `autoviz-0.1.601/autoviz/AutoViz_Class.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,33 +315,38 @@
                                                 depVar,dfte,header,verbose)
         except:
             print('Not able to read or load file. Please check your inputs and try again...')
             return None
         ##### This is where we start plotting different kinds of charts depending on dependent variables
         if depVar == None or depVar == '':
          ##### This is when No dependent Variable is given #######
-            try:
-                svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
-                                                depVar,classes,lowess, mk_dir)
-                self.add_plots('pair_scatter',svg_data)
-            except Exception as e:
-                print(e)
-                print('Could not draw Pair Scatter Plots')
+            if len(continuous_vars) > 1:
+                try:
+                    svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
+                                                    depVar,classes,lowess, mk_dir)
+                    self.add_plots('pair_scatter',svg_data)
+                except Exception as e:
+                    print(e)
+                    print('Could not draw Pair Scatter Plots')
             try:
                 svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,problem_type,
                                     depVar,classes, mk_dir)
                 self.add_plots('dist_plot',svg_data)
             except:
                 print('Could not draw Distribution Plot')
             try:
                 if len(continuous_vars) > 0:
                     svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
                     self.add_plots('violin_plot',svg_data)
+                else:
+                    svg_data = draw_pivot_tables(dft, problem_type, verbose,
+                        chart_format,depVar,classes, mk_dir)
+                    self.add_plots('pivot_plot',svg_data)
             except:
-                print('Could not draw Violin Plot')
+                print('Could not draw Distribution Plots')
             try:
                 #### Since there is no depependent variable in this dataset, you can leave it as-is
                 numeric_cols = dft.select_dtypes(include='number').columns.tolist()
                 numeric_cols = list_difference(numeric_cols, date_vars)
                 svg_data = draw_heatmap(dft, numeric_cols, verbose,chart_format, date_vars, depVar,
                                     problem_type,classes, mk_dir)
                 self.add_plots('heat_map',svg_data)
@@ -350,57 +355,58 @@
             if date_vars != [] and len(continuous_vars) > 0:
                 try:
                     svg_data = draw_date_vars(dft,depVar,date_vars,
                                               continuous_vars,verbose,chart_format,problem_type, mk_dir)
                     self.add_plots('date_plot',svg_data)
                 except:
                     print('Could not draw Date Vars')
-            if len(continuous_vars) > 0:
+            if len(continuous_vars) > 0 and len(cats) > 0:
                 try:
                     svg_data = draw_barplots(dft,cats,continuous_vars, problem_type,
                                     verbose,chart_format,depVar,classes, mk_dir)
                     self.add_plots('bar_plot',svg_data)
                 except:
                     print('Could not draw Bar Plots')
             else:
-                try:
-                    svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                chart_format, mk_dir=None)
-                    self.add_plots('catscatter_plot',svg_data)
-                except:
-                    print ('Could not draw catscatter plots...')
+                if len(cats) > 1:
+                    try:
+                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                    chart_format, mk_dir=None)
+                        self.add_plots('catscatter_plot',svg_data)
+                    except:
+                        print ('Could not draw catscatter plots...')
         else:
             if problem_type=='Regression':
                 ############## This is a Regression Problem #################
-                try:
-                    svg_data = draw_scatters(dft,
-                                    continuous_vars,verbose,chart_format,problem_type,depVar,classes,lowess, mk_dir)
-                    self.add_plots('scatter_plot',svg_data)
-                except Exception as e:
-                    print("Exception Drawing Scatter Plots")
-                    print(e)
-                    traceback.print_exc()
-                    print('Could not draw Scatter Plots')
-                try:
-                    svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
-                                                    depVar,classes,lowess, mk_dir)
-                    self.add_plots('pair_scatter',svg_data)
-                except:
-                    print('Could not draw Pair Scatter Plots')
+                if len(continuous_vars) > 0:
+                    try:
+                        svg_data = draw_scatters(dft,
+                                        continuous_vars,verbose,chart_format,problem_type,depVar,classes,lowess, mk_dir)
+                        self.add_plots('scatter_plot',svg_data)
+                    except Exception as e:
+                        print("Exception Drawing Scatter Plots")
+                        print(e)
+                        traceback.print_exc()
+                        print('Could not draw Scatter Plots')
+                if len(continuous_vars) > 1:
+                    try:
+                        svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
+                                                        depVar,classes,lowess, mk_dir)
+                        self.add_plots('pair_scatter',svg_data)
+                    except:
+                        print('Could not draw Pair Scatter Plots')
                 try:
                     if type(depVar) == str:
                         othernums = [x for x in continuous_vars if x not in [depVar]]
                     else:
                         othernums = [x for x in continuous_vars if x not in depVar]
                     if len(othernums) >= 1:
                         svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,
                                             problem_type, depVar, classes, mk_dir)
                         self.add_plots('dist_plot',svg_data)
-                    else:
-                        print('No continuous var in data set: hence no distribution plots')
                 except:
                     print('Could not draw some Distribution Plots')
                 try:
                     if len(continuous_vars) > 0:
                         svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('violin_plot',svg_data)
                 except:
@@ -417,64 +423,68 @@
                 if date_vars != [] and len(continuous_vars) > 0:
                     try:
                         svg_data = draw_date_vars(
                             dft,depVar,date_vars,continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('date_plot',svg_data)
                     except:
                         print('Could not draw some Time Series plots')
-                if len(continuous_vars) > 0:
-
+                if len(cats) > 0 and len(continuous_vars) == 0:
+                    ### This is somewhat duplicative with distplot (above) - hence do it only minimally!
                     try:
                         svg_data = draw_pivot_tables(dft, problem_type, verbose,
                             chart_format,depVar,classes, mk_dir)
                         self.add_plots('pivot_plot',svg_data)
                     except:
                         print('Could not draw some Pivot Charts against Dependent Variable')
+                if len(continuous_vars) > 0 and len(cats) > 0:
                     try:
                         svg_data = draw_barplots(dft, find_remove_duplicates(cats+bool_vars),continuous_vars,
                                                     problem_type, verbose,chart_format,depVar,classes, mk_dir)
                         self.add_plots('bar_plot',svg_data)
                         #self.add_plots('bar_plot',None)
                     except:
                         print('Could not draw some Bar Charts')
                 else:
-                    try:
-                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                    chart_format, mk_dir=None)
-                        self.add_plots('catscatter_plot',svg_data)
-                    except:
-                        print ('Could not draw catscatter plots...')
+                    if len(cats) > 1:
+                        try:
+                            svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                        chart_format, mk_dir=None)
+                            self.add_plots('catscatter_plot',svg_data)
+                        except:
+                            print ('Could not draw catscatter plots...')
             else :
                 ############ This is a Classification Problem ##################
-                try:
-                    svg_data = draw_scatters(dft,continuous_vars,
-                                             verbose,chart_format,problem_type,depVar, classes,lowess, mk_dir)
-                    self.add_plots('scatter_plot',svg_data)
-                except Exception as e:
-                    print(e)
-                    traceback.print_exc()
-                    print("Exception Drawing Scatter Plots")
-                    print('Could not draw some Scatter Plots')
-                try:
-                    svg_data = draw_pair_scatters(dft,continuous_vars,
-                                                  problem_type,verbose,chart_format,depVar,classes,lowess, mk_dir)
-                    self.add_plots('pair_scatter',svg_data)
-                except:
-                    print('Could not draw some Pair Scatter Plots')
+                if len(continuous_vars) > 0:
+                    try:
+                        svg_data = draw_scatters(dft,continuous_vars,
+                                                 verbose,chart_format,problem_type,depVar, classes,lowess, mk_dir)
+                        self.add_plots('scatter_plot',svg_data)
+                    except Exception as e:
+                        print(e)
+                        traceback.print_exc()
+                        print('Could not draw some Scatter Plots')
+                if len(continuous_vars) > 1:
+                    try:
+                        svg_data = draw_pair_scatters(dft,continuous_vars,
+                                                      problem_type,verbose,chart_format,depVar,classes,lowess, mk_dir)
+                        self.add_plots('pair_scatter',svg_data)
+                    except:
+                        print('Could not draw some Pair Scatter Plots')
                 try:
                     if type(depVar) == str:
                         othernums = [x for x in continuous_vars if x not in [depVar]]
                     else:
                         othernums = [x for x in continuous_vars if x not in depVar]
+
                     if len(othernums) >= 1:
                         svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,
                                                 problem_type,depVar,classes, mk_dir)
                         self.add_plots('dist_plot',svg_data)
                     else:
-                        print('No continuous var in data set: hence no distribution plots')
+                        print('No continuous var in data set: drawing categorical distribution plots')
                 except:
                     print('Could not draw some Distribution Plots')
                 try:
                     if len(continuous_vars) > 0:
                         svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('violin_plot',svg_data)
                 except:
@@ -491,37 +501,40 @@
                 if date_vars != [] and len(continuous_vars) > 0:
                     try:
                         svg_data = draw_date_vars(dft,depVar,date_vars,
                                                   continuous_vars,verbose,chart_format,problem_type, mk_dir)
                         self.add_plots('date_plot',svg_data)
                     except:
                         print('Could not draw some Time Series plots')
-                if len(continuous_vars) > 0:
+                if len(cats) > 0 and len(continuous_vars) == 0:
+                    ### This is somewhat duplicative with distplot (above) - hence do it only minimally!
                     try:
                         svg_data = draw_pivot_tables(dft, problem_type, verbose,
                                         chart_format,depVar,classes, mk_dir)
                         self.add_plots('pivot_plot',svg_data)
                     except:
                         print('Could not draw some Pivot Charts against Dependent Variable')
+                if len(continuous_vars) > 0 and len(cats) > 0:
                     try:
                         svg_data = draw_barplots(dft,find_remove_duplicates(cats+bool_vars),continuous_vars,problem_type,
                                         verbose,chart_format, depVar, classes, mk_dir)
                         self.add_plots('bar_plot',svg_data)
                         pass
                     except:
                         if verbose <= 1:
                             print('Could not draw some Bar Charts')
                         pass
                 else:
-                    try:
-                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                    chart_format, mk_dir=None)
-                        self.add_plots('catscatter_plot',svg_data)
-                    except:
-                        print ('Could not draw catscatter plots...')
+                    if len(cats) > 1:
+                        try:
+                            svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
+                                        chart_format, mk_dir=None)
+                            self.add_plots('catscatter_plot',svg_data)
+                        except:
+                            print ('Could not draw catscatter plots...')
         ###### Now you can check for NLP vars or discrete_string_vars to do wordcloud #######
         if len(discrete_string_vars) > 0:
             plotname = 'wordcloud'
             import nltk
             nltk.download('popular')
             for each_string_var in discrete_string_vars:
                 try:
```

### Comparing `autoviz-0.1.600/autoviz/AutoViz_Holo.py` & `autoviz-0.1.601/autoviz/AutoViz_Holo.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.600/autoviz/AutoViz_NLP.py` & `autoviz-0.1.601/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.600/autoviz/AutoViz_Utils.py` & `autoviz-0.1.601/autoviz/AutoViz_Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,20 @@
 # Pivot Tables are generally meant for Categorical Variables on the axes
 # and a Numeric Column (typically the Dep Var) as the "Value" aggregated by Sum.
 # Let's do some pivot tables to capture some meaningful insights
 import random
 def draw_pivot_tables(dft, problem_type, verbose, chart_format, depVar='', classes=None, mk_dir=None):
     #### Finally I have fixed the bugs in pivot tables due to "category" dtypes in data ##############
     plot_name = 'Bar_Plots_Cats'
+    imgdata_list = []
     cats = [i for i in dft.loc[:,dft.nunique()<=15]]
+    if isinstance(depVar, str):
+        cats = [x for x in cats if x not in [depVar]]
+    else:
+        cats = [x for x in cats if x not in depVar]
     dft = copy.deepcopy(dft)
     cols = 2
     cmap = plt.get_cmap('jet')
     #### For some reason, the cmap colors are not working #########################
     colors = cmap(np.linspace(0, 1, len(cats)))
     colors = cycle('byrcmgkbyrcmgkbyrcmgkbyrcmgkbyr')
     #colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
@@ -167,15 +172,14 @@
     if N==0:
         print('No categorical or boolean vars in data set. Hence no pivot plots...')
         return None
     noplots = copy.deepcopy(N)
     #### You can set the number of subplots per row and the number of categories to display here cols = 2
     displaylimit = 20
     categorylimit = 5
-    imgdata_list = []
     width_size = 15
     height_size = 5
     stringlimit = 20
     N = len(cats)
     sns.set_palette("Set1")
     ###########  This works equally well for classification as well as Regression ###
     lst=[]
@@ -214,22 +218,23 @@
             data = dft[var1].value_counts()
             if problem_type != 'Binary_Classification' or problem_type != 'Multi_Classification':
                 sns.countplot(x=var1,
                                 data=dft,
                                 ax=ax1,
                                 order=dft[var1].value_counts().index,
                                 hue = depVar)
+                ax1.set_title('Distribution of %s by %s' %(var1, depVar),fontsize=12)
             else:
                 sns.countplot(x=var1,
                                 data=dft,
                                 ax=ax1,
                                 order=dft[var1].value_counts().index,)
+                ax1.set_title('Distribution of %s' %var1,fontsize=12)
             ax1.set_xlabel(var1)
             ax1.set_xticklabels(dft[var1].value_counts().index, rotation=30, ha='right', fontsize=9)
-            ax1.set_title('Distribution of %s' %var1,fontsize=12)
             counter += 1
         fig.tight_layout()
         fig.suptitle('Distribution of Variables (with <=15 categories)', fontsize=15,y=1.01);
     image_count = 0
     if verbose == 2:
         imgdata_list.append(save_image_data(fig, chart_format,
                             plot_name, depVar, mk_dir))
@@ -454,16 +459,14 @@
 # PAIR SCATTER PLOTS ARE NEEDED ONLY FOR CLASSIFICATION PROBLEMS IN NUMERIC VARIABLES
 def draw_pair_scatters(dfin,nums,problem_type, verbose,chart_format, dep=None, classes=None, lowess=False, mk_dir=None):
     """
     ### This is where you plot a pair-wise scatter plot of Independent Variables against each other####
     """
     plot_name = 'Pair_Scatter_Plots'
     dft = dfin[:]
-    if len(nums) <= 1:
-        return
     classes = copy.deepcopy(classes)
     cols = 2
     colortext = 'brymcgkbyrcmgkbyrcmgkbyrcmgkbyr'
     colors = cycle(colortext)
     imgdata_list = list()
     width_size = 15
     height_size = 4
@@ -688,15 +691,15 @@
         image_count = 0
         N = len(conti)
         target_vars = dft[dep].unique()
         fig = plt.figure(figsize=(min(N*width_size,20),min(N*height_size,20)))
         if timeseries_flag:
             fig.suptitle('Time Series: Heatmap of all Differenced Continuous vars for target = %s' %dep, fontsize=15,y=1.01)
         else:
-            fig.suptitle('Heatmap of all Continuous Variables for target = %s' %dep, fontsize=15,y=1.01)
+            fig.suptitle('Heatmap of all Numeric Variables with target: %s' %dep, fontsize=15,y=1.01)
         plotc = 1
         #rows = len(target_vars)
         rows = 1
         cols = 1
         if timeseries_flag:
             dft_target = dft[[dep]+conti].diff()
         else:
@@ -729,15 +732,15 @@
         N = len(conti)
         fig = plt.figure(figsize=(min(20,N*width_size),min(20,N*height_size)))
         corr = dft_target.corr()
         sns.heatmap(corr, annot=True)
         if timeseries_flag:
             fig.suptitle('Time Series Data: Heatmap of Differenced Continuous vars including target = %s' %dep, fontsize=15,y=1.01)
         else:
-            fig.suptitle('Heatmap of all Continuous Variables including target = %s' %dep,fontsize=15,y=1.01)
+            fig.suptitle('Heatmap of all Numeric Variables including target: %s' %dep,fontsize=15,y=1.01)
         fig.tight_layout();
         if verbose <= 1:
             plt.show();
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
                             plot_name, dep, mk_dir))
             image_count += 1
@@ -812,40 +815,42 @@
         #####  Now draw each of the categorical variable distributions in each subplot ####
         if not len(cats) == 0:
             cols = 2
             noplots = len(cats)
             rows = int((noplots/cols)+0.99 )
             k = 0
             fig = plt.figure(figsize=(width_size,rows*height_size))
-            fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
+            fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
             for each_cat in copy_cats:
                 color2 = next(colors)
                 ax1 = plt.subplot(rows, cols, k+1)
                 kwds = {"rotation": 45, "ha":"right"}
                 ### In some small datasets, we get floats as categories since there are so few categories.
                 if dft[each_cat].dtype in ['float16','float32','float64']:
                     ### In those cases, we must remove the width_size since it thinks they are an index and errors.
-                    dft[each_cat].value_counts().plot(kind='bar', 
-                                            #color=color2,
+                    dft[each_cat].value_counts(normalize=True, dropna=False).plot(kind='bar', 
+                                            color=color2,
                                             ax=ax1,label='%s' %each_cat)
-                    labels = dft[each_cat].value_counts().index.tolist()
+                    labels = dft[each_cat].value_counts(dropna=False).index.tolist()
                 else:
-                    dft[each_cat].value_counts()[:width_size].plot(kind='bar', 
-                                            #color=color2,
+                    dft[each_cat].value_counts(normalize=True, dropna=False)[:width_size].plot(kind='bar', 
+                                            color=color2,
                                             ax=ax1,label='%s' %each_cat)
-                    labels = dft[each_cat].value_counts()[:width_size].index.tolist()
+                    labels = dft[each_cat].value_counts(dropna=False)[:width_size].index.tolist()
+                k += 1
                 ax1.set_xticklabels(labels,**kwds);
-                ax1.set_title('Distribution of %s (top %d categories only)' %(each_cat,width_size))
+                ax1.set_title('Normalized distribution of %s (top %d categories only)' %(each_cat,width_size))
             fig.tight_layout();
+            
             ########## This is where you end the logic for distplots ################
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
                                 plot_name+'_Cats', dep, mk_dir))
                 image_count += 1
-            fig.suptitle('Histograms (KDE plots) of all Continuous Variables', fontsize=12,y=1.01)
+            fig.suptitle('Histograms and Normalized distribitions of all variables', fontsize=12,y=1.01)
             if verbose <= 1:
                 plt.show();
     else:
         ######### This is for Classification problems only ########
         #### Now you can draw both object and numeric variables using same conti variable
         #sns.color_palette("Set1")
         sns.set_palette("Set1")
@@ -880,41 +885,45 @@
                 elif dft[each_conti].dtype == 'object':
                     ### Remember that fillna only works at dataframe level! ###
                     dft[[each_conti]] = dft[[each_conti]].fillna("nan")
                 else:
                     dft[[each_conti]] = dft[[each_conti]].fillna(0)
             plt.subplot(rows, cols, k+1)
             ax1 = plt.gca()
+            
             if dft[each_conti].dtype==object:
                 kwds = {"rotation": 45, "ha":"right"}
                 labels = dft[each_conti].value_counts()[:width_size].index.tolist()
                 conti_df = dft[[dep,each_conti]].groupby([dep,each_conti]).size().nlargest(width_size).reset_index(name='Values')
                 pivot_df = conti_df.pivot(index=each_conti, columns=dep, values='Values')
-                #print('color list = %s' %color_list)
+                ### row_ticks must be modified since some values of dep are missing in conti_df
+                row_ticks = conti_df[dep].unique().tolist()
                 pivot_df.loc[:,row_ticks].plot.bar(stacked=True, 
                     color=color_list, 
                     ax=ax1)
                 #dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
                 #                    label=class_label)
                 #ax1.set_xticklabels(labels,**kwds);
                 ax1.set_title('Distribution of %s (top %d categories only)' %(each_conti,width_size))
             elif str(dft[each_conti].dtype) in ['category']:
                 kwds = {"rotation": 45, "ha":"right"}
                 labels = dft[each_conti].value_counts()[:width_size].index.tolist()
                 conti_df = dft[[dep,each_conti]].groupby([dep,each_conti]).size().nlargest(width_size).reset_index(name='Values')
                 pivot_df = conti_df.pivot(index=each_conti, columns=dep, values='Values')
-                #print('color list = %s' %color_list)
+                ### row_ticks must be modified since some values of dep are missing in conti_df
+                row_ticks = conti_df[dep].unique().tolist()
                 pivot_df.loc[:,row_ticks].plot.bar(stacked=True, 
                     color=color_list,
                     ax=ax1)
                 #dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
                 #                    label=class_label)
                 #ax1.set_xticklabels(labels,**kwds);
                 ax1.set_title('Distribution of %s (top %d categories only)' %(each_conti,width_size))
             else:
+                
                 for target_var, color2, class_label in zip(target_vars,color_list,classes):
                     try:
                         if legend_flag <= label_limit:
                             sns.histplot(dft.loc[dft[dep]==target_var][each_conti],
                                 #hist=False, 
                                 kde=True, stat="density",
                             #dft.loc[dft[dep]==target_var][each_conti].hist(
```

### Comparing `autoviz-0.1.600/autoviz/__init__.py` & `autoviz-0.1.601/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.600/autoviz/classify_method.py` & `autoviz-0.1.601/autoviz/classify_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -348,38 +348,38 @@
             minn.append(data[i].value_counts().min())
     length = len(data)
     nunik = data.nunique()
     nulls = data.isna().sum()
     df = pd.DataFrame(
         {
          #'column': list(data),
-        'Nuniques': nunik,
+         'Nullpercent' : 100*(nulls/length),
          'NuniquePercent': (100*(nunik/length)),
          'dtype': data.dtypes,
+        'Nuniques': nunik,
          'Nulls' : nulls,
-         'Nullpercent' : 100*(nulls/length),
-         'Value counts Min':minn
+         'Least num. of categories':minn
         },
-        columns = ['Nuniques', 'dtype','Nulls','Nullpercent', 'NuniquePercent',
-                       'Value counts Min']).sort_values(by ='Nuniques',ascending = False)
+        columns = ['Nullpercent', 'NuniquePercent','dtype','Nuniques', 'Nulls',
+                       'Least num. of categories']).sort_values(by = 'Nullpercent',ascending = False)
     newcol = 'Data cleaning improvement suggestions'
     print('%s. Complete them before proceeding to ML modeling.' %newcol)
     mixed_cols = [col for col in data.columns if len(data[col].apply(type).value_counts()) > 1]
     df[newcol] = ''
     df['first_comma'] = ''
     if len(cat_cols) > 0:
         mask0 = df['dtype'] == 'object'
-        mask1 = df['Value counts Min']/df['Nuniques'] <= 0.05
+        mask1 = df['Least num. of categories']/df['Nuniques'] <= 0.05
         mask4 = df['dtype'] == 'category'
         df.loc[mask0&mask1,newcol] += df.loc[mask0&mask1,'first_comma'] + 'combine rare categories'
         df.loc[mask4&mask1,newcol] += df.loc[mask4&mask1,'first_comma'] + 'combine rare categories'
         df.loc[mask0&mask1,'first_comma'] = ', '
         df.loc[mask4&mask1,'first_comma'] = ', '
     mask2 = df['Nulls'] > 0
-    df.loc[mask2,newcol] += df.loc[mask2,'first_comma'] + 'fill missing'
+    df.loc[mask2,newcol] += df.loc[mask2,'first_comma'] + 'fill missing values'
     df.loc[mask2,'first_comma'] = ", "
     mask3 = df['Nuniques'] == 1
     df.loc[mask3,newcol] += df.loc[mask3,'first_comma'] + 'invariant values: drop'
     df.loc[mask3,'first_comma'] = ", "
     if len(non_num_cols) > 0:
         for x in non_num_cols:
             if df.loc[x, 'NuniquePercent'] == 100:
@@ -394,26 +394,32 @@
     inf_cols = list(set(inf_cols1+inf_cols2))
     ### Check for infinite values in columns #####
     if len(inf_cols) > 0:
         for x in inf_cols:
             df.loc[x,newcol] += df.loc[x,'first_comma'] + 'infinite values: drop'
             df.loc[x,'first_comma'] = ", "
     #### Check for skewed float columns #######
-    skew_cols1 = np.array(num_cols)[[(np.abs(np.round(data[col].skew(), 1)) > 1
+    skew_cols1 = np.array(num_cols)[[(np.abs(np.round(data[col].skew(), 1)) >= 1
                     ) & (np.abs(np.round(data[col].skew(), 1)) <= 5) for col in num_cols]].tolist()
     skew_cols2 = np.array(num_cols)[[(np.abs(np.round(data[col].skew(), 1)) > 5) for col in num_cols]].tolist()
     skew_cols = list(set(skew_cols1+skew_cols2))
     ### Check for skewed values in columns #####
     if len(skew_cols1) > 0:
         for x in skew_cols1:
-            df.loc[x,newcol] += df.loc[x,'first_comma'] + 'skewed: cap or drop outliers'
+            if data[x].skew() < 0:
+                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'left skewed distribution: cap or drop outliers'
+            else:
+                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'right skewed distribution: cap or drop outliers'
             df.loc[x,'first_comma'] = ", "
     if len(skew_cols2) > 0:
         for x in skew_cols2:
-            df.loc[x,newcol] += df.loc[x,'first_comma'] + 'highly skewed: drop outliers or do box-cox transform'
+            if data[x].skew() < 0:
+                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'highly left skewed distribution: drop outliers or do box-cox transform'
+            else:
+                df.loc[x,newcol] += df.loc[x,'first_comma'] + 'highly right skewed distribution: drop outliers or do box-cox transform'
             df.loc[x,'first_comma'] = ", "
     ##### Do the same for mixed dtype columns - they must be fixed! ##
     if len(mixed_cols) > 0:
         for x in mixed_cols:
             df.loc[x,newcol] += df.loc[x,'first_comma'] + 'fix mixed data types'
             df.loc[x,'first_comma'] = ", "
     df.drop('first_comma', axis=1, inplace=True)
```

### Comparing `autoviz-0.1.600/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.601/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.600
+Version: 0.1.601
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz
         
         Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
@@ -65,26 +65,27 @@
         pip install -r requirements.txt
         ```
         
         ## Usage
         
         Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
         
-        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the library
+        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
+        <b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
+        Instead, you can simply do<br>
         
         ```py
-        from autoviz.AutoViz_Class import AutoViz_Class
-        
+        from autoviz import AutoViz_Class
         AV = AutoViz_Class()
         ```
         
         Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
         If you don't have a filename, you can simply assign the filename argument `""` (empty string).
         
-        Call AutoViz using the filename (or dataframe) along with the separator and the name of the target variable in the input.
+        Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
         
         ```py
         filename = ""
         sep = ","
         dft = AV.AutoViz(
             filename,
             sep=",",
```

### Comparing `autoviz-0.1.600/setup.py` & `autoviz-0.1.601/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.600",
+    version="0.1.601",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
```

