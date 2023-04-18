# Comparing `tmp/sdypy-EMA-0.26.tar.gz` & `tmp/sdypy-EMA-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy-EMA-0.26.tar", last modified: Tue Jan 31 10:38:41 2023, max compression
+gzip compressed data, was "sdypy-EMA-0.27.tar", last modified: Tue Apr 18 13:00:35 2023, max compression
```

## Comparing `sdypy-EMA-0.26.tar` & `sdypy-EMA-0.27.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 10:38:41.181724 sdypy-EMA-0.26/
--rw-rw-rw-   0        0        0     1091 2022-02-15 12:50:00.000000 sdypy-EMA-0.26/LICENSE
--rw-rw-rw-   0        0        0     2878 2023-01-31 10:38:41.180718 sdypy-EMA-0.26/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2022-10-13 05:33:44.000000 sdypy-EMA-0.26/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-31 10:38:41.121012 sdypy-EMA-0.26/sdypy/
-drwxrwxrwx   0        0        0        0 2023-01-31 10:38:41.156888 sdypy-EMA-0.26/sdypy/EMA/
--rw-rw-rw-   0        0        0    35215 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/EMA.py
--rw-rw-rw-   0        0        0      174 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/__init__.py
--rw-rw-rw-   0        0        0     4779 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/normal_modes.py
--rw-rw-rw-   0        0        0    17154 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/pole_picking.py
--rw-rw-rw-   0        0        0     3376 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/stabilization.py
--rw-rw-rw-   0        0        0     4620 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/sdypy/EMA/tools.py
-drwxrwxrwx   0        0        0        0 2023-01-31 10:38:41.179709 sdypy-EMA-0.26/sdypy_EMA.egg-info/
--rw-rw-rw-   0        0        0     2878 2023-01-31 10:38:41.000000 sdypy-EMA-0.26/sdypy_EMA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-01-31 10:38:41.000000 sdypy-EMA-0.26/sdypy_EMA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 10:38:41.000000 sdypy-EMA-0.26/sdypy_EMA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-01-31 10:38:41.000000 sdypy-EMA-0.26/sdypy_EMA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-31 10:38:41.000000 sdypy-EMA-0.26/sdypy_EMA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 10:38:41.181724 sdypy-EMA-0.26/setup.cfg
--rw-rw-rw-   0        0        0     1474 2023-01-31 10:09:05.000000 sdypy-EMA-0.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/LICENSE
+-rw-rw-rw-   0        0        0     2873 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     2489 2023-04-18 12:59:27.000000 sdypy-EMA-0.27/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.837794 sdypy-EMA-0.27/sdypy/
+drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.845804 sdypy-EMA-0.27/sdypy/EMA/
+-rw-rw-rw-   0        0        0    40478 2023-04-18 09:40:09.000000 sdypy-EMA-0.27/sdypy/EMA/EMA.py
+-rw-rw-rw-   0        0        0      174 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/__init__.py
+-rw-rw-rw-   0        0        0     4779 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/normal_modes.py
+-rw-rw-rw-   0        0        0    18198 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/pole_picking.py
+-rw-rw-rw-   0        0        0     3376 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/stabilization.py
+-rw-rw-rw-   0        0        0     4620 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/sdypy/EMA/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/sdypy_EMA.egg-info/
+-rw-rw-rw-   0        0        0     2873 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 13:00:35.000000 sdypy-EMA-0.27/sdypy_EMA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:00:35.861803 sdypy-EMA-0.27/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2023-04-18 09:31:04.000000 sdypy-EMA-0.27/setup.py
```

### Comparing `sdypy-EMA-0.26/LICENSE` & `sdypy-EMA-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.26/PKG-INFO` & `sdypy-EMA-0.27/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.26
+Version: 0.27
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
 
-pyEMA
-=====
+sdypy-EMA
+=========
 
 Experimental and operational modal analysis
 
 Check out the `documentation`_.
 
-New in version 0.26
+This project is successor of the `pyEMA`_ project. pyEMA is no longer developed after version 0.26.
+
+New in version 0.27
 -------------------
-- include (or exclude) upper and lower residuals
-- driving point implementation (scaling modal constants to modal shapes)
-- implementation of the LSFD method that assumes proportional damping (modal constants are real-valued)
-- FRF type implementation (enables the use of accelerance, mobility or receptance)
+- UFF support: Import FRFs directly from UFF files. The `pyUFF`_ package is used to read the UFF files.
+- Stability chart upgrade: Show/hide unstable poles to improve the clarity of the chart.
+- Documentation update.
 
 
 Basic usage
 -----------
 
+Import ``EMA`` module:
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from sdypy import EMA
+
+
 Make an instance of ``Model`` class:
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
-   a = pyema.Model(
+   a = EMA.Model(
        frf_matrix,
        frequency_array,
        lower=50,
        upper=10000,
        pol_order_high=60
        )
 
@@ -88,29 +97,24 @@
 
 where **H** is reconstructed FRF matrix and **A** is a matrix of modal constants.
 
 2. Reconstruction on **c** using poles from **a**:
 
 .. code:: python
 
-    c = pyema.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
+    c = EMA.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
 
     H, A = c.get_constants(whose_poles=a)
 
 |DOI|
-|Build Status|
 
-.. _documentation: https://pyema.readthedocs.io/en/latest/index.html
+.. _documentation: https://sdypy-ema.readthedocs.io/en/latest/
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4016671.svg?
    :target: https://doi.org/10.5281/zenodo.4016671
 
-.. |Build Status| image:: https://travis-ci.com/ladisk/pyEMA.svg?branch=master
-   :target: https://travis-ci.com/ladisk/pyEMA
-
 .. _sdypy: https://github.com/sdypy/sdypy
 
-.. _sdypy-EMA: https://github.com/ladisk/sdypy-EMA
-
-
+.. _pyEMA: https://github.com/ladisk/pyEMA
 
+.. _pyUFF: https://pypi.org/project/pyuff/
```

### Comparing `sdypy-EMA-0.26/README.rst` & `sdypy-EMA-0.27/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-pyEMA
-=====
+sdypy-EMA
+=========
 
 Experimental and operational modal analysis
 
 Check out the `documentation`_.
 
-New in version 0.26
+This project is successor of the `pyEMA`_ project. pyEMA is no longer developed after version 0.26.
+
+New in version 0.27
 -------------------
-- include (or exclude) upper and lower residuals
-- driving point implementation (scaling modal constants to modal shapes)
-- implementation of the LSFD method that assumes proportional damping (modal constants are real-valued)
-- FRF type implementation (enables the use of accelerance, mobility or receptance)
+- UFF support: Import FRFs directly from UFF files. The `pyUFF`_ package is used to read the UFF files.
+- Stability chart upgrade: Show/hide unstable poles to improve the clarity of the chart.
+- Documentation update.
 
 
 Basic usage
 -----------
 
+Import ``EMA`` module:
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from sdypy import EMA
+
+
 Make an instance of ``Model`` class:
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
-   a = pyema.Model(
+   a = EMA.Model(
        frf_matrix,
        frequency_array,
        lower=50,
        upper=10000,
        pol_order_high=60
        )
 
@@ -76,27 +85,23 @@
 
 where **H** is reconstructed FRF matrix and **A** is a matrix of modal constants.
 
 2. Reconstruction on **c** using poles from **a**:
 
 .. code:: python
 
-    c = pyema.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
+    c = EMA.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
 
     H, A = c.get_constants(whose_poles=a)
 
 |DOI|
-|Build Status|
 
-.. _documentation: https://pyema.readthedocs.io/en/latest/index.html
+.. _documentation: https://sdypy-ema.readthedocs.io/en/latest/
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4016671.svg?
    :target: https://doi.org/10.5281/zenodo.4016671
 
-.. |Build Status| image:: https://travis-ci.com/ladisk/pyEMA.svg?branch=master
-   :target: https://travis-ci.com/ladisk/pyEMA
-
 .. _sdypy: https://github.com/sdypy/sdypy
 
-.. _sdypy-EMA: https://github.com/ladisk/sdypy-EMA
-
+.. _pyEMA: https://github.com/ladisk/pyEMA
 
+.. _pyUFF: https://pypi.org/project/pyuff/
```

### Comparing `sdypy-EMA-0.26/sdypy/EMA/EMA.py` & `sdypy-EMA-0.27/sdypy/EMA/EMA.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
+from matplotlib.figure import Figure
 import time
 import scipy.linalg
 from tqdm import tqdm
 from scipy.linalg import toeplitz, companion
 from scipy.optimize import least_squares, leastsq
 
 import warnings
 
 try:
     import tkinter as tk
 except:
     print('WARNING: tkinter is not istalled or not accessible. Stability chart is not available.')
 
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
-from matplotlib.figure import Figure
-
 
 warnings.filterwarnings('ignore', category=RuntimeWarning)
 
+import pyuff
+
 from .pole_picking import SelectPoles
 from . import tools
 from . import stabilization
 from . import normal_modes
 
 class Model():
     """
@@ -88,48 +89,47 @@
                 self.frf = np.array([self.frf])
 
             try:
                 self.freq = np.asarray(freq)
             except:
                 raise Exception('cannot convert freq to a numpy array')
             if self.freq.ndim != 1:
-                raise Exception(
-                    f'ndim of freq is not equal to 1 ({self.freq.ndim})')
+                raise Exception(f'ndim of freq is not equal to 1 ({self.freq.ndim})')
 
             # Cut off the frequencies above 'upper' argument
             cutoff_ind = np.argmin(np.abs(self.freq - self.upper))
             self.frf = self.frf[:, :cutoff_ind]
             self.freq = self.freq[:cutoff_ind]
         else:
-            raise Exception('input arguments are not defined')
+            # The FRFs will be added from UFF
+            pass
+
+        if not isinstance(pol_order_high, int):
+            raise Exception('pol_order_high must be an integer')
+        self.pol_order_high = pol_order_high
 
-        try:
-            self.pol_order_high = int(pol_order_high)
-        except:
-            raise Exception('cannot convert pol_order_high to an integer')
         if self.pol_order_high <= 0:
             raise Exception('pol_order_high must be more than zero')
 
-        if not pyfrf:
+        if not pyfrf and frf is not None and freq is not None:
             self.omega = 2 * np.pi * self.freq
             if dt is None:
                 self.sampling_time = 1/(2*self.freq[-1])
             else:
                 self.sampling_time = dt
 
-        if driving_point is None:
-            self.driving_point = driving_point
-        else:
-            if type(driving_point) != int:
-                raise('"driving_point" must be an integer')
-            else:
-                self.driving_point = driving_point
+        if not isinstance(driving_point, int) and driving_point is not None:
+            raise Exception('"driving_point" must be an integer')
+        if driving_point is not None:
+            if driving_point > self.frf.shape[0]:
+                raise Exception('"driving_point" must be an index of the FRF matrix. "driving_point" too large.')
+        self.driving_point = driving_point
 
         if frf_type not in ['receptance', 'mobility', 'accelerance']:
-            raise('"frf_type" must be "receptance", "mobility" or "accelerance".')
+            raise Exception('"frf_type" must be "receptance", "mobility" or "accelerance".')
         else:
             self.frf_type = frf_type
        
         self.get_participation_factors = get_partfactors
 
     def add_frf(self, pyfrf_object):
         """
@@ -137,27 +137,67 @@
 
         This method can be used in relation to pyFRF from Open Modal (https://github.com/openmodal)
 
         :param pyfrf_object: FRF object from pyFRF
         :type pyfrf_object: object
         """
         freq = pyfrf_object.get_f_axis()
-        sel = (freq >= 1.0e-1)
 
-        self.freq = freq[sel]
+        self.freq = freq
         self.omega = 2 * np.pi * self.freq
         self.sampling_time = 1/(2*self.freq[-1])
 
-        new_frf = np.vstack(pyfrf_object.get_FRF(form='receptance')[sel])
+        new_frf = np.vstack(pyfrf_object.get_FRF(form='receptance'))
 
         if isinstance(self.frf, int):
             self.frf = new_frf.T
         else:
             self.frf = np.concatenate((self.frf, new_frf.T), axis=0)
 
+    def read_uff(self, uff_filename):
+        """
+        Add FRFs from a UFF file.
+
+        :param uff_filename: The file to read.
+        :type uff_filename: str
+        """
+        try:
+            uff_file = pyuff.UFF(uff_filename)
+        except:
+            raise Exception('cannot open uff file')
+        
+        set_types = uff_file.get_set_types()
+        if 58 not in set_types:
+            raise Exception('no FRFs in uff file')
+        
+        ind58 = np.argwhere(set_types==58)[:, 0]
+        
+        uff_data = uff_file.read_sets()
+        uffFRF = np.asarray([uff_data[ind]['data'] for ind in ind58 if uff_data[ind]['func_type'] == 4])
+        ufffreq = np.asarray([uff_data[ind]['x'] for ind in ind58 if uff_data[ind]['func_type'] == 4])[0]
+
+        cutoff_ind = np.argmin(np.abs(ufffreq - self.upper))
+
+        self.freq = ufffreq
+        self.freq = self.freq[:cutoff_ind]
+        self.omega = 2 * np.pi * self.freq
+        self.sampling_time = 1/(2*self.freq[-1])
+
+        self.frf = uffFRF[:, :cutoff_ind]
+
+        if uff_data[ind58[0]]['ordinate_spec_data_type'] == 8:
+            self.frf_type = 'receptance'
+        elif uff_data[ind58[0]]['ordinate_spec_data_type'] == 11:
+            self.frf_type = 'mobility'
+        elif uff_data[ind58[0]]['ordinate_spec_data_type'] == 12:
+            self.frf_type = 'accelerance'
+        else:
+            print('Warning: frf_type cannot be obtained from the uff file. Assuming "receptance".')
+            self.frf_type = 'receptance'
+
     def get_poles(self, method='lscf', show_progress=True):
         """Compute poles based on polynomial approximation of FRF.
 
         Source: https://github.com/openmodal/OpenModal/blob/master/OpenModal/analysis/lscf.py
 
         The LSCF method is an frequency-domain Linear Least Squares
         estimator optimized for modal parameter estimation. The choice of
@@ -224,14 +264,20 @@
             def tqdm_range(x): return x
 
         self.all_poles = []
         self.pole_freq = []
         self.pole_xi = []
         self.partfactors = []
 
+        if self.freq[0] != 0:
+            df = self.freq[1] - self.freq[0]
+            freq_start = np.arange(0, self.freq[0], df)
+            self.freq = np.hstack((freq_start, self.freq))
+            self.frf = np.column_stack((np.zeros((len(freq_start), self.frf.shape[0])).T, self.frf))
+
         lower_ind = np.argmin(np.abs(self.freq - self.lower))
         n = self.pol_order_high * 2
         nf = 2 * (self.frf.shape[1] - 1)
         nr = self.frf.shape[0]
 
         indices_s = np.arange(-n, n+1)
         indices_t = np.arange(n+1)
@@ -489,14 +535,90 @@
         """
         Show modal data in a table-like structure.
         """
         print('   Nat. f.      Damping')
         print(23*'-')
         for i, f in enumerate(self.nat_freq):
             print(f'{i+1}) {f:6.1f}\t{self.nat_xi[i]:5.4f}')
+    
+    def write_uff(self, filename, name, rsp_dir, ref_dir):
+        """
+        Export modal data to a UFF file.
+
+        :param filename: The file to write to (.uff)
+        :type filename: str
+        :param name: Response and reference entity name
+        :param rsp_dir: Response direction:
+             1 - +X Translation       4 - +X Rotation
+            -1 - -X Translation      -4 - -X Rotation
+             2 - +Y Translation       5 - +Y Rotation
+            -2 - -Y Translation      -5 - -Y Rotation
+             3 - +Z Translation       6 - +Z Rotation
+            -3 - -Z Translation      -6 - -Z Rotation
+        :param ref_dir: Reference direction:
+             same options as for parameter rsp_dir  
+        """
+        print('Warning: This is an experimental feature and will be further developed.')
+
+        uffwrite = pyuff.UFF(filename)
+
+        eigval_data_to_write = {'type':58,
+                'func_type': 1, #0 - general; 22 - eigenvalue
+                'rsp_node': 1, #
+                'rsp_dir': rsp_dir,  #0 - scalar
+                'ref_dir': ref_dir,  #0 - scalar
+                'ref_node': 1, #
+                'data': self.nat_freq,
+                'x': np.arange(np.shape(self.nat_freq)[0]) + 1,
+                'id1': 'id1', 
+                'rsp_ent_name': name,
+                'ref_ent_name': name,
+                'abscissa_spacing':1,
+                'abscissa_spec_data_type':1, #general
+                'ordinate_spec_data_type':18, #frequency
+                'orddenom_spec_data_type':13 #
+                }
+        uffwrite.write_sets(eigval_data_to_write, 'add')
+
+        damp_data_to_write = {'type':58,
+                'func_type': 1, #0 - general;
+                'rsp_node': 1, #
+                'rsp_dir': rsp_dir,  #0 - scalar
+                'ref_dir': ref_dir,  #0 - scalar
+                'ref_node': 1, #
+                'data': self.nat_xi,
+                'x': np.arange(np.shape(self.nat_xi)[0]) + 1,
+                'id1': 'id1', 
+                'rsp_ent_name': name,
+                'ref_ent_name': name,
+                'abscissa_spacing':1,
+                'abscissa_spec_data_type':1, #general
+                'ordinate_spec_data_type':1, #general
+                'orddenom_spec_data_type':13 #
+                }
+        uffwrite.write_sets(damp_data_to_write, 'add')
+
+        for i in range(np.shape(self.normal_mode())[1]):
+            eigvec_data_to_write = {'type':58,
+                    'func_type': 1, #0 - general; 23 = eigenvector
+                    'rsp_node': 1, #
+                    'rsp_dir': rsp_dir,  #0 - scalar
+                    'ref_dir': ref_dir,  #0 - scalar
+                    'ref_node':1, # 
+                    'data': self.normal_mode()[:, i],
+                    'x': np.arange(np.shape(self.normal_mode())[0]),
+                    'id1': 'id1', 
+                    'rsp_ent_name': name,
+                    'ref_ent_name': name,
+                    'abscissa_spacing':1,
+                    'abscissa_spec_data_type':1, #general
+                    'ordinate_spec_data_type':1, #general
+                    'orddenom_spec_data_type':13 #
+                    }
+            uffwrite.write_sets(eigvec_data_to_write, 'add')
 
 
 def _irfft_adjusted_lower_limit(x, low_lim, indices):
     """
     Compute the ifft of real matrix x with adjusted summation limits:
     ::
         y(j) = sum[k=-n-2, ... , -low_lim-1, low_lim, low_lim+1, ... n-2, n-1] x[k] * exp(sqrt(-1)*j*k* 2*pi/n),
```

### Comparing `sdypy-EMA-0.26/sdypy/EMA/normal_modes.py` & `sdypy-EMA-0.27/sdypy/EMA/normal_modes.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.26/sdypy/EMA/pole_picking.py` & `sdypy-EMA-0.27/sdypy/EMA/pole_picking.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
         param model: object of pyEMA.Model
         """
         self.Model = Model
         self.shift_is_held = False
         self.chart_type = 0 # 0 - stability chart, 1 - cluster diagram
         self.show_legend = 0
+        self.hide_poles = 1
         self.frf_plot_type = 'abs'
 
         self.Model.nat_freq = []
         self.Model.nat_xi = []
         self.Model.pole_ind = []
         
     
@@ -53,25 +54,25 @@
         filemenu = tk.Menu(menubar, tearoff=0)
         filemenu.add_command(label='Save figure', command=self.save_this_figure)
         menubar.add_cascade(label='File', menu=filemenu)
 
         chartmenu = tk.Menu(menubar, tearoff=0)
         chartmenu.add_command(label='Stability chart', command=lambda: self.toggle_chart_type(0))
         chartmenu.add_command(label='Cluster diagram', command=lambda: self.toggle_chart_type(1))
-        menubar.add_cascade(label="Chart type", menu=chartmenu)
+        menubar.add_cascade(label="Chart Type", menu=chartmenu)
 
         mifmenu = tk.Menu(menubar, tearoff=0)
         mifmenu.add_command(label='Plot mean abs', command=lambda: self.toggle_mif_frf('abs'))
         mifmenu.add_command(label='Plot all FRFs', command=lambda: self.toggle_mif_frf('all'))
-        menubar.add_cascade(label="FRF plot type", menu=mifmenu)
+        menubar.add_cascade(label="FRF Plot Type", menu=mifmenu)
 
-        legendmenu = tk.Menu(menubar, tearoff=0)
-        legendmenu.add_command(label='Show legend', command=lambda: self.toggle_legend(1))
-        legendmenu.add_command(label='Hide legend', command=lambda: self.toggle_legend(0))
-        menubar.add_cascade(label="Legend", menu=legendmenu)
+        hidepolesmenu = tk.Menu(menubar, tearoff=0)
+        hidepolesmenu.add_command(label='Show unstable poles', command=lambda: (self.toggle_hide_poles(0), self.toggle_legend(1)))
+        hidepolesmenu.add_command(label='Hide unstable poles', command=lambda: (self.toggle_hide_poles(1), self.toggle_legend(0)))
+        menubar.add_cascade(label="Show/Hide Unstable Poles", menu=hidepolesmenu)
 
         helpmenu = tk.Menu(menubar, tearoff=0)
         helpmenu.add_command(label='Help', command=self.show_help)
         menubar.add_cascade(label='Help', menu=helpmenu)
 
         self.root.config(menu=menubar)
 
@@ -127,14 +128,16 @@
                 'Unselect a pole: SHIFT + RIGHT mouse button'
             ]
             self.ax2.text(x_position, y_position, '\n'.join(message), 
                 fontsize=12, verticalalignment='top', horizontalalignment='center',
                 bbox=dict(facecolor='lightgreen', edgecolor='lightgreen'))
         
         self.ax1.set_xlim([self.Model.lower, self.Model.upper])
+        self.ax2.set_xlabel('Frequency [Hz]')
+        self.ax2.set_ylabel('Magnitude')
         self.fig.canvas.draw()
     
 
     def get_stability(self, fn_temp=0.001, xi_temp=0.05):
         """Get the stability matrix.
         
         :param fn_temp: Natural frequency stability criterion.
@@ -155,32 +158,37 @@
             # stable eigenfrequencies, stable damping ratios
             b = np.argwhere((self.test_fn > 0) & ((self.test_xi > 0) & (self.xi_temp > 0)))
             # unstable eigenfrequencies, unstable damping ratios
             c = np.argwhere((self.test_fn == 0) & ((self.test_xi == 0) | (self.xi_temp <= 0)))
             # unstable eigenfrequencies, stable damping ratios
             d = np.argwhere((self.test_fn == 0) & ((self.test_xi > 0) & (self.xi_temp > 0)))
 
-            p1 = self.ax1.plot(self.fn_temp[a[:, 0], a[:, 1]], 1+a[:, 1], 'bx',
-                        markersize=4, label="stable frequency, unstable damping")
-            p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], 1+b[:, 1], 'gx',
-                        markersize=7, label="stable frequency, stable damping")
-            p3 = self.ax1.plot(self.fn_temp[c[:, 0], c[:, 1]], 1+c[:, 1], 'r.',
-                        markersize=4, label="unstable frequency, unstable damping")
-            p4 = self.ax1.plot(self.fn_temp[d[:, 0], d[:, 1]], 1+d[:, 1], 'r*',
-                        markersize=4, label="unstable frequency, stable damping")
+            if self.hide_poles:
+                p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], 1+b[:, 1], 'gx',
+                            markersize=7, label="Stable frequency, stable damping")
+
+            else:
+                p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], 1+b[:, 1], 'gx',
+                            markersize=7, label="Stable frequency, stable damping")
+                p1 = self.ax1.plot(self.fn_temp[a[:, 0], a[:, 1]], 1+a[:, 1], 'bx',
+                            markersize=4, label="Stable frequency, unstable damping")
+                p4 = self.ax1.plot(self.fn_temp[d[:, 0], d[:, 1]], 1+d[:, 1], 'r*',
+                            markersize=4, label="Unstable frequency, stable damping")
+                p3 = self.ax1.plot(self.fn_temp[c[:, 0], c[:, 1]], 1+c[:, 1], 'r.',
+                            markersize=4, label="Unstable frequency, unstable damping")
             
             self.line, = self.ax1.plot(self.Model.nat_freq, np.repeat(
                     self.Model.pol_order_high, len(self.Model.nat_freq)), 'kv', markersize=8)
             self.selected, = self.ax1.plot([self.Model.pole_freq[p[0]][p[1]] for p in self.Model.pole_ind], 
                                             [p[0] for p in self.Model.pole_ind], 'ko')
             
             if self.show_legend:
-                self.pole_legend = self.ax1.legend(loc='upper center', ncol=2, frameon=True)
+                self.pole_legend = self.ax1.legend(loc='lower center', ncol=4, frameon=True)
 
-            self.ax1.set_title('Stability chart')
+            self.ax1.set_title('Stability Chart')
 
             
             self.ax1.set_ylabel('Polynomial order')
 
             plt.tight_layout()
         else:
             self.line.set_xdata(np.asarray(self.Model.nat_freq))  # update data
@@ -212,32 +220,37 @@
             # stable eigenfrequencies, stable damping ratios
             b = np.argwhere((self.test_fn > 0) & ((self.test_xi > 0) & (self.xi_temp > 0)))
             # unstable eigenfrequencies, unstable damping ratios
             c = np.argwhere((self.test_fn == 0) & ((self.test_xi == 0) | (self.xi_temp <= 0)))
             # unstable eigenfrequencies, stable damping ratios
             d = np.argwhere((self.test_fn == 0) & ((self.test_xi > 0) & (self.xi_temp > 0)))
 
-            p1 = self.ax1.plot(self.fn_temp[a[:, 0], a[:, 1]], self.xi_temp[a[:, 0], a[:, 1]], 'bx',
-                        markersize=4, label="stable frequency, unstable damping")
-            p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], self.xi_temp[b[:, 0], b[:, 1]], 'gx',
-                        markersize=7, label="stable frequency, stable damping")
-            p3 = self.ax1.plot(self.fn_temp[c[:, 0], c[:, 1]], self.xi_temp[c[:, 0], c[:, 1]], 'r.',
-                        markersize=4, label="unstable frequency, unstable damping")
-            p4 = self.ax1.plot(self.fn_temp[d[:, 0], d[:, 1]], self.xi_temp[d[:, 0], d[:, 1]], 'r*',
-                        markersize=4, label="unstable frequency, stable damping")
+            if self.hide_poles:
+                p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], self.xi_temp[b[:, 0], b[:, 1]], 'gx',
+                            markersize=7, label="Stable frequency, stable damping")
+            
+            else:
+                p2 = self.ax1.plot(self.fn_temp[b[:, 0], b[:, 1]], self.xi_temp[b[:, 0], b[:, 1]], 'gx',
+                            markersize=7, label="Stable frequency, stable damping")
+                p1 = self.ax1.plot(self.fn_temp[a[:, 0], a[:, 1]], self.xi_temp[a[:, 0], a[:, 1]], 'bx',
+                            markersize=4, label="Stable frequency, unstable damping")
+                p4 = self.ax1.plot(self.fn_temp[d[:, 0], d[:, 1]], self.xi_temp[d[:, 0], d[:, 1]], 'r*',
+                            markersize=4, label="Unstable frequency, stable damping")
+                p3 = self.ax1.plot(self.fn_temp[c[:, 0], c[:, 1]], self.xi_temp[c[:, 0], c[:, 1]], 'r.',
+                            markersize=4, label="Unstable frequency, unstable damping")
             
             self.line, = self.ax1.plot(self.Model.nat_freq, np.repeat(
                     1.05*np.max(self.xi_temp[b1[:, 0], b1[:, 1]]), len(self.Model.nat_freq)), 'kv', markersize=8)
             self.selected, = self.ax1.plot([self.Model.pole_freq[p[0]][p[1]] for p in self.Model.pole_ind], 
                                             [self.Model.pole_xi[p[0]][p[1]] for p in self.Model.pole_ind], 'ko')
             
             if self.show_legend:
-                self.pole_legend = self.ax1.legend(loc='upper center', ncol=2, frameon=True)
+                self.pole_legend = self.ax1.legend(loc='lower center', ncol=4, frameon=True)
 
-            self.ax1.set_title('Cluster diagram')
+            self.ax1.set_title('Cluster Diagram')
 
             self.ax1.set_ylabel('Damping ratio')
             plt.tight_layout()
         else:
             self.line.set_xdata(np.asarray(self.Model.nat_freq))  # update data
             self.line.set_ydata(np.repeat(1.05*np.max(self.xi_temp[b1[:, 0], b1[:, 1]]), len(self.Model.nat_freq)))
 
@@ -352,14 +365,26 @@
 
         if self.chart_type == 0:
             self.plot_stability()
         elif self.chart_type == 1:
             self.plot_cluster()
     
     
+    def toggle_hide_poles(self, x):
+        if x:
+            self.hide_poles = 1
+        else:
+            self.hide_poles = 0
+
+        if self.chart_type == 0:
+            self.plot_stability()
+        elif self.chart_type == 1:
+            self.plot_cluster()
+
+
     def toggle_chart_type(self, x):
         if x == 0:
             self.chart_type = 0
             self.plot_stability()
         elif x == 1:
             self.chart_type = 1
             self.plot_cluster()
```

### Comparing `sdypy-EMA-0.26/sdypy/EMA/stabilization.py` & `sdypy-EMA-0.27/sdypy/EMA/stabilization.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.26/sdypy/EMA/tools.py` & `sdypy-EMA-0.27/sdypy/EMA/tools.py`

 * *Files identical despite different names*

### Comparing `sdypy-EMA-0.26/sdypy_EMA.egg-info/PKG-INFO` & `sdypy-EMA-0.27/sdypy_EMA.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 Metadata-Version: 2.1
 Name: sdypy-EMA
-Version: 0.26
+Version: 0.27
 Summary: Experimental and operational modal analysis.
 Home-page: https://github.com/ladisk/pyEMA
 Author: Klemen Zaletelj, Domen Gorjup, Janko Slavič, Tomaž Bregar, Miha Pogačar, et al.
 Maintainer: Janko Slavič
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
 
-pyEMA
-=====
+sdypy-EMA
+=========
 
 Experimental and operational modal analysis
 
 Check out the `documentation`_.
 
-New in version 0.26
+This project is successor of the `pyEMA`_ project. pyEMA is no longer developed after version 0.26.
+
+New in version 0.27
 -------------------
-- include (or exclude) upper and lower residuals
-- driving point implementation (scaling modal constants to modal shapes)
-- implementation of the LSFD method that assumes proportional damping (modal constants are real-valued)
-- FRF type implementation (enables the use of accelerance, mobility or receptance)
+- UFF support: Import FRFs directly from UFF files. The `pyUFF`_ package is used to read the UFF files.
+- Stability chart upgrade: Show/hide unstable poles to improve the clarity of the chart.
+- Documentation update.
 
 
 Basic usage
 -----------
 
+Import ``EMA`` module:
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from sdypy import EMA
+
+
 Make an instance of ``Model`` class:
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: python
 
-   a = pyema.Model(
+   a = EMA.Model(
        frf_matrix,
        frequency_array,
        lower=50,
        upper=10000,
        pol_order_high=60
        )
 
@@ -88,29 +97,24 @@
 
 where **H** is reconstructed FRF matrix and **A** is a matrix of modal constants.
 
 2. Reconstruction on **c** using poles from **a**:
 
 .. code:: python
 
-    c = pyema.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
+    c = EMA.Model(frf_matrix, frequency_array, lower=50, upper=10000, pol_order_high=60)
 
     H, A = c.get_constants(whose_poles=a)
 
 |DOI|
-|Build Status|
 
-.. _documentation: https://pyema.readthedocs.io/en/latest/index.html
+.. _documentation: https://sdypy-ema.readthedocs.io/en/latest/
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4016671.svg?
    :target: https://doi.org/10.5281/zenodo.4016671
 
-.. |Build Status| image:: https://travis-ci.com/ladisk/pyEMA.svg?branch=master
-   :target: https://travis-ci.com/ladisk/pyEMA
-
 .. _sdypy: https://github.com/sdypy/sdypy
 
-.. _sdypy-EMA: https://github.com/ladisk/sdypy-EMA
-
-
+.. _pyEMA: https://github.com/ladisk/pyEMA
 
+.. _pyUFF: https://pypi.org/project/pyuff/
```

### Comparing `sdypy-EMA-0.26/setup.py` & `sdypy-EMA-0.27/setup.py`

 * *Files identical despite different names*

