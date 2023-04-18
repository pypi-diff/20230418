# Comparing `tmp/decodanda-0.6.0.tar.gz` & `tmp/decodanda-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.0.tar", last modified: Tue Apr 18 20:21:06 2023, max compression
+gzip compressed data, was "decodanda-0.6.1.tar", last modified: Tue Apr 18 20:41:05 2023, max compression
```

## Comparing `decodanda-0.6.0.tar` & `decodanda-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.437799 decodanda-0.6.0/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.0/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:21:06.437451 decodanda-0.6.0/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.0/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.434348 decodanda-0.6.0/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.0/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.0/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.0/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.0/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.0/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    19659 2023-02-16 22:56:04.000000 decodanda-0.6.0/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.436972 decodanda-0.6.0/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:21:06.437924 decodanda-0.6.0/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:19:01.000000 decodanda-0.6.0/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.642897 decodanda-0.6.1/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.1/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:41:05.642450 decodanda-0.6.1/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.1/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.638515 decodanda-0.6.1/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.1/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.1/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.1/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.1/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.1/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    22076 2023-04-18 20:39:00.000000 decodanda-0.6.1/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:41:05.641756 decodanda-0.6.1/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:41:05.000000 decodanda-0.6.1/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:41:05.643039 decodanda-0.6.1/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:40:47.000000 decodanda-0.6.1/setup.py
```

### Comparing `decodanda-0.6.0/LICENSE.md` & `decodanda-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/PKG-INFO` & `decodanda-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.0/README.md` & `decodanda-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/decodanda/classes.py` & `decodanda-0.6.1/decodanda/classes.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/decodanda/imports.py` & `decodanda-0.6.1/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/decodanda/in_time.py` & `decodanda-0.6.1/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/decodanda/utilities.py` & `decodanda-0.6.1/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.0/decodanda/visualize.py` & `decodanda-0.6.1/decodanda/visualize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 from .imports import *
 from .utilities import *
 
 
 # Viz utilities
 
 def corrfunc(x, y, ax=None, **kws):
@@ -442,14 +444,88 @@
         equalize_ax(ax)
 
         ax.set_xticklabels([])
         ax.set_yticklabels([])
         ax.set_zticklabels([])
         return fig,
 
+    def animate(i):
+        ax.view_init(elev=10., azim=i * 2)
+        return fig,
+
+    if savename:
+        anim = animation.FuncAnimation(fig, animate, init_func=init,
+                                       frames=360, interval=20, blit=True)
+        mywriter = animation.PillowWriter(fps=30)
+        anim.save(savename, writer=mywriter)
+    else:
+        init()
+    mpl.rcParams.update({'figure.autolayout': True})
+    return fig
+
+
+def visualize_balanced_MDS(dec, dim=3, savename=None, title='', data=None, null=None, names=None, axs=None):
+    # performance and CCGP
+
+    mpl.rcParams.update({'figure.autolayout': False})
+    rasters = []
+    labels = []
+    ndata =  dec._max_conditioned_data
+    for key in dec.conditioned_rasters:
+        X = sample_from_rasters(dec.conditioned_rasters[key], ndata)
+        rasters.append(X)
+        y = np.repeat(key, ndata)
+        labels.append(y)
+    X = np.vstack(rasters)
+    y = np.hstack(labels)
+    C = sklearn.decomposition.PCA(n_components=dim)
+    components = C.fit_transform(X, y)
+
+    if names is None:
+        names = list(dec._semantic_vectors.keys())
+
+    if data is not None and null is not None:
+        if axs is None:
+            fig = plt.figure(figsize=(12, 5))
+            G = GridSpec(12, 12)
+            ax = fig.add_subplot(G[:, 0:6], projection='3d')
+            ax_dec = fig.add_subplot(G[1:9, 6:9])
+            ax_ccgp = fig.add_subplot(G[1:9, 10:])
+        else:
+            ax = axs[0]
+            ax_dec = axs[1]
+            ax_ccgp = axs[2]
+            fig = ax.get_figure()
+
+        ax_dec.set_title(title)
+
+        plot_perfs_null_model(data['Decoding'], null['Decoding'], ax=ax_dec, marker='o')
+        plot_perfs_null_model(data['CCGP'], null['CCGP'], ax=ax_ccgp, ylabel='CCGP', marker='s')
+    else:
+        if axs is None:
+            fig = plt.figure(figsize=(6, 5))
+            ax = fig.add_subplot(projection='3d')
+        else:
+            ax = axs
+            fig = ax.get_figure()
+
+    plt.subplots_adjust(left=0, right=0.95, top=1, bottom=0)
+
+    def init():
+        for i in range(len(names)):
+            mask = (y == names[i])
+            ax.scatter(components[mask, 0], components[mask, 1], components[mask, 2], alpha=0.05, marker='o',
+                       s=20)
+        equalize_ax(ax)
+
+        ax.set_xticklabels([])
+        ax.set_yticklabels([])
+        ax.set_zticklabels([])
+        return fig,
+
     def animate(i):
         ax.view_init(elev=10., azim=i * 2)
         return fig,
 
     if savename:
         anim = animation.FuncAnimation(fig, animate, init_func=init,
                                        frames=360, interval=20, blit=True)
```

### Comparing `decodanda-0.6.0/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.1/decodanda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.0/setup.py` & `decodanda-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.0'
+VERSION = '0.6.1'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

