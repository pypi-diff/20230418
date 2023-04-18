# Comparing `tmp/plotguy-1.0.3.tar.gz` & `tmp/plotguy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.3.tar", last modified: Mon Mar 13 21:18:54 2023, max compression
+gzip compressed data, was "plotguy-1.0.4.tar", last modified: Tue Apr 18 03:36:32 2023, max compression
```

## Comparing `plotguy-1.0.3.tar` & `plotguy-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-03-13 21:18:54.407707 plotguy-1.0.3/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-03-13 21:18:54.407432 plotguy-1.0.3/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.3/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-03-13 21:18:54.406423 plotguy-1.0.3/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25546 2023-03-13 21:02:36.000000 plotguy-1.0.3/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.3/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    63306 2023-02-28 02:27:43.000000 plotguy-1.0.3/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37786 2023-02-24 01:25:02.000000 plotguy-1.0.3/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11340 2022-10-16 03:24:02.000000 plotguy-1.0.3/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-03-13 21:18:54.407229 plotguy-1.0.3/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-03-13 21:18:54.000000 plotguy-1.0.3/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-03-13 21:18:54.000000 plotguy-1.0.3/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-03-13 21:18:54.000000 plotguy-1.0.3/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      124 2023-03-13 21:18:54.000000 plotguy-1.0.3/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-03-13 21:18:54.000000 plotguy-1.0.3/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-03-13 21:18:54.407754 plotguy-1.0.3/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      814 2023-03-13 21:17:32.000000 plotguy-1.0.3/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.909128 plotguy-1.0.4/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-18 03:36:32.908974 plotguy-1.0.4/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.4/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.908011 plotguy-1.0.4/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25562 2023-04-18 03:28:10.000000 plotguy-1.0.4/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.4/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.4/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.4/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.4/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-18 03:36:32.908776 plotguy-1.0.4/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-18 03:36:32.000000 plotguy-1.0.4/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-18 03:36:32.909177 plotguy-1.0.4/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-18 03:34:27.000000 plotguy-1.0.4/setup.py
```

### Comparing `plotguy-1.0.3/plotguy/__init__.py` & `plotguy-1.0.4/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,17 @@
     return save_name
 
 
 def path_reference_code(save_name):
     reference_code = str(zlib.crc32(bytes(save_name, 'UTF-8')))[:6]
     return reference_code
 
-def generate_filepath(para_combination,folder='',file_format='parquet'):
+def generate_filepath(para_combination, folder=''):
+
+    file_format = para_combination['file_format']
 
     if not file_format == 'parquet':
         file_format = 'csv'
 
     save_name = filename_only(para_combination)
 
     reference_code = path_reference_code(save_name)
@@ -74,16 +76,14 @@
 
     result = cal_performance(para_combination)
     index = para_combination['reference_index']
     manager_list.append((index,result))
 
 
 def generate_backtest_result(all_para_combination, number_of_core=8, risk_free_rate='geometric_mean'):
-
-
     ## Get / Calculate risk free rate
     start_date = all_para_combination[0]['start_date']
     end_date = all_para_combination[0]['end_date']
 
     if isinstance(risk_free_rate, str):
         try:
             if risk_free_rate == 'geometric_mean':
@@ -94,14 +94,15 @@
                 risk_free_rate = plotguy.get_latest_fed_fund_rate()
         except:
             risk_free_rate = 2  # if network error, set rate to 2 %
             print('Network error. Risk free rate: {:.2f} %'.format(risk_free_rate))
     else:
         print('Risk free rate: {:.2f} %'.format(risk_free_rate))
 
+    print('Backtest result is loading. Please wait patiently.')
 
 
     manager_list = mp.Manager().list()# To save the result with index number
 
     cal_performance_list = []
     for para_combination in all_para_combination:
         para_combination['risk_free_rate'] = risk_free_rate
@@ -289,15 +290,15 @@
     freq = para_combination['freq']
     file_format = para_combination['file_format']
     sec_profile = para_combination['sec_profile']
     margin_req = sec_profile['margin_req']
     multiplier = sec_profile['multiplier']
 
     # Read backtest data
-    save_path = generate_filepath(para_combination=para_combination,folder=folder,file_format=file_format)
+    save_path = generate_filepath(para_combination=para_combination,folder=folder)
     if file_format == 'parquet':
         df_backtest = pd.read_parquet(save_path) # Daraframe that may not be daily
         ### parquet specific, All backtest force to treart as summary, # ie filter action only
         # df_backtest = df_backtest.loc[df_backtest['action'] != ''].copy()
         # df_backtest = df_backtest.loc[df_backtest['action'].isnull() == False].copy()
     else:
         df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
@@ -470,29 +471,28 @@
 
     return df_daily
 
 
 
 
 def cal_performance(para_combination):
-
     start_date = para_combination['start_date']
     end_date = para_combination['end_date']
 
     risk_free_rate = para_combination['risk_free_rate']
 
     intraday = para_combination['intraday']
     summary_mode = para_combination['summary_mode']
 
     file_format = para_combination['file_format']
 
     if (intraday or summary_mode):
         df_daily = resample_summary_to_daily(para_combination=para_combination)
     else:
-        save_path = generate_filepath(para_combination=para_combination, file_format=file_format)
+        save_path = generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
         df_backtest['date'] = pd.to_datetime(df_backtest['date'], format='%Y-%m-%d')
         df_backtest = df_backtest.loc[(df_backtest['date'] >= start_date) & (df_backtest['date'] <= end_date)]
@@ -547,15 +547,15 @@
         net_profit, holding_period_day, return_on_capital, annualized_return, annualized_std, annualized_sr = calculate_sharp_ratio(df, 'equity_value', risk_free_rate)
         mdd_pct, mdd_dollar = calculate_mdd(df, 'equity_value')
         mdd_pct = mdd_pct * -100
         mdd_dollar = mdd_dollar * -1
 
         # Win Rate (need to use df_backtest directly)
 
-        save_path = generate_filepath(para_combination=para_combination, file_format=file_format)
+        save_path = generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
         win_rate_dict = calculate_win_rate(df_backtest)
         num_of_trade, num_of_loss, num_of_win, win_rate, loss_rate = win_rate_dict['Overall']
@@ -644,10 +644,9 @@
     result_dict['bah_annualized_std'] = bah_annualized_std
     result_dict['bah_annualized_sr'] = bah_annualized_sr
     result_dict['bah_mdd_dollar'] = bah_mdd_dollar
     result_dict['bah_mdd_pct'] = bah_mdd_pct
     result_dict['return_to_bah'] = return_on_capital - bah_return
 
 
-
     return result_dict
```

### Comparing `plotguy-1.0.3/plotguy/aggregate.py` & `plotguy-1.0.4/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.3/plotguy/components.py` & `plotguy-1.0.4/plotguy/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,15 @@
         # grab first and last observations from df.date and make a continuous date range from that
         dt_all = pd.date_range(start=df['datetime'].iloc[0], end=df['datetime'].iloc[-1], freq=freq)
         # check which dates from your source that also accur in the continuous date range
         dt_obs = [d.strftime("%Y-%m-%d %H:%M:%S") for d in df['datetime']]
         # isolate missing timestamps
         dt_breaks = [d for d in dt_all.strftime("%Y-%m-%d %H:%M:%S").tolist() if not d in dt_obs]
 
-        save_path = plotguy.generate_filepath(para_combination=para_combination, file_format=file_format)
+        save_path = plotguy.generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_signal_list = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_signal_list = pd.read_csv(save_path, index_col=0)
 
         df_signal_list['date'] = pd.to_datetime(df_signal_list['date'], format='%Y-%m-%d')
         df_signal_list['datetime'] = pd.to_datetime(df_signal_list['datetime'], format='%Y-%m-%d %H:%M:%S')
@@ -603,15 +603,15 @@
 
             # df = pd.read_csv(save_path)
             # df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
 
             if (intraday or summary_mode):
                 df_daily = plotguy.resample_summary_to_daily(para_combination=para_combination)
             else:
-                save_path = plotguy.generate_filepath(para_combination=para_combination, file_format=file_format)
+                save_path = plotguy.generate_filepath(para_combination=para_combination)
                 if file_format == 'parquet':
                     df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
                 else:
                     df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
                 df_daily = df_backtest.copy()
 
@@ -733,15 +733,15 @@
 
         pass
 
 
     def generate_chart_2_full(self, para_combination, line_colour, settings):
         file_format = para_combination['file_format']
 
-        save_path = plotguy.generate_filepath(para_combination=para_combination, file_format=file_format)
+        save_path = plotguy.generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
         df_csv = df_backtest.copy()
         df_chart = self.prepare_df_chart(df_csv)
```

### Comparing `plotguy-1.0.3/plotguy/equity_curves.py` & `plotguy-1.0.4/plotguy/equity_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,16 +579,15 @@
 
                     reference_index = self.graph_df.iloc[i].reference_index
                     df_all_para_combination = pd.DataFrame(all_para_combination)
                     para_combination = \
                     df_all_para_combination.loc[df_all_para_combination['reference_index'] == reference_index].to_dict(
                         'records')[0]
 
-                    file_format = para_combination['file_format']
-                    save_path = plotguy.generate_filepath(para_combination=para_combination, file_format=file_format)
+                    save_path = plotguy.generate_filepath(para_combination=para_combination)
                     ref_code = self.graph_df.iloc[i].reference_code
                     risk_free_rate = self.graph_df.iloc[i].risk_free_rate
 
                     performance_matrix = components.update_performance_matrix(start_date, end_date,
                                                                               self.graph_df.iloc[i].copy(), para_dict,
                                                                               risk_free_rate, ref_code)
```

### Comparing `plotguy-1.0.3/plotguy/signals.py` & `plotguy-1.0.4/plotguy/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,21 +126,15 @@
         )
         def display_output(title_area, stat_area, line_chart, hist_area, para_radioitems):
 
             # if not complete selection
             if None in para_radioitems:
                 return title_area, stat_area, line_chart, hist_area
 
-            save_path = generate_filepath(
-                py_filename=filename,
-                output_folder=output_folder,
-                start_date=start_date,
-                end_date=end_date,
-                para_dict=para_dict,
-                para_combination=para_radioitems)
+            save_path = generate_filepath(para_combination=para_radioitems)
 
             df = pd.read_csv(save_path)
 
             # Count number of subchart
             subchart_count = 0
             try:
                 fig = settings['subchart_1']
```

### Comparing `plotguy-1.0.3/setup.py` & `plotguy-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.3",
+    version="1.0.4",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

