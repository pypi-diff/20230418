# Comparing `tmp/synthdid-0.9.1.tar.gz` & `tmp/synthdid-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.9.1.tar", last modified: Tue Apr 18 01:37:06 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.2.tar", last modified: Tue Apr 18 02:20:34 2023, max compression
```

## Comparing `synthdid-0.9.1.tar` & `synthdid-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:37:06.364772 synthdid-0.9.1/
--rw-rw-rw-   0        0        0      432 2023-04-18 01:37:06.364772 synthdid-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-18 01:37:06.364772 synthdid-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-18 01:36:54.000000 synthdid-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:37:06.356771 synthdid-0.9.1/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6064 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/plots.py
--rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/solver.py
--rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.1/synthdid/summary.py
--rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.1/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.1/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:37:06.363771 synthdid-0.9.1/synthdid.egg-info/
--rw-rw-rw-   0        0        0      432 2023-04-18 01:37:06.000000 synthdid-0.9.1/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-18 01:37:06.000000 synthdid-0.9.1/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:37:06.000000 synthdid-0.9.1/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-18 01:37:06.000000 synthdid-0.9.1/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 01:37:06.000000 synthdid-0.9.1/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.979720 synthdid-0.9.2/
+-rw-rw-rw-   0        0        0      432 2023-04-18 02:20:34.979720 synthdid-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:20:34.979720 synthdid-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-18 02:20:24.000000 synthdid-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.969722 synthdid-0.9.2/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6127 2023-04-18 02:08:10.000000 synthdid-0.9.2/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/solver.py
+-rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.2/synthdid/summary.py
+-rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.2/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.2/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:20:34.978721 synthdid-0.9.2/synthdid.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 02:20:34.000000 synthdid-0.9.2/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.9.1/setup.py` & `synthdid-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
     author="D2CML",
-    version="0.9.1",
+    version="0.9.2",
     packages=find_packages(),
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `synthdid-0.9.1/synthdid/get_data.py` & `synthdid-0.9.2/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/placebo_simulations.py` & `synthdid-0.9.2/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/plots.py` & `synthdid-0.9.2/synthdid/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             ax.axvline(x=times[i], label="", color='k', linestyle="--", lw=.8)
 
             ax.set_xlabel("Time")
             ax.set_title("Adoption: " + str(time_title_cb(time)));
 
             # plots[f"t_{time}"] = fig
             plots.append(fig)
-
+        self.plot_outcomes = []
         self.plot_outcomes = plots
         return self
 
     def plot_weights(self, unit_filter=None, times=None, time_title_cb=int):
         weights = self.weights
         table_result = self.att_info
         lambda_wg = weights["lambda"]
@@ -142,9 +142,10 @@
             ax.legend(fontsize = 9)
             if weights_dots.difs.max() > 0 and weights_dots.difs.min() < 0:
                 ax.axhline(y=0, lw = .5, c = "#0D3276")
             plots.append(fig)
 
         for i, time in enumerate(times):
             plot_times(i)
+        self.plot_weights = []
         self.plot_weights = plots
         return self
```

### Comparing `synthdid-0.9.1/synthdid/sdid.py` & `synthdid-0.9.2/synthdid/sdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/solver.py` & `synthdid-0.9.2/synthdid/solver.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/synthdid.py` & `synthdid-0.9.2/synthdid/synthdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/utils.py` & `synthdid-0.9.2/synthdid/utils.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid/vcov.py` & `synthdid-0.9.2/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.1/synthdid.egg-info/requires.txt` & `synthdid-0.9.2/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*

