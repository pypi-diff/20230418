# Comparing `tmp/spiakid-drs-0.1.tar.gz` & `tmp/spiakid-drs-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid-drs-0.1.tar", last modified: Tue Feb 14 16:15:20 2023, max compression
+gzip compressed data, was "spiakid-drs-0.11.tar", last modified: Tue Apr 18 13:50:55 2023, max compression
```

## Comparing `spiakid-drs-0.1.tar` & `spiakid-drs-0.11.tar`

### file list

```diff
@@ -1,43 +1,31 @@
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.833846 spiakid-drs-0.1/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    10173 2023-02-09 09:47:58.000000 spiakid-drs-0.1/LICENSE
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1675 2023-02-14 16:15:20.833846 spiakid-drs-0.1/PKG-INFO
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     2181 2023-02-09 09:47:58.000000 spiakid-drs-0.1/README.md
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1262 2023-02-09 09:47:58.000000 spiakid-drs-0.1/README_for_pip.md
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      579 2023-02-14 16:12:49.000000 spiakid-drs-0.1/pyproject.toml
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       38 2023-02-14 16:15:20.833846 spiakid-drs-0.1/setup.cfg
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.805846 spiakid-drs-0.1/src/
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.805846 spiakid-drs-0.1/src/Functions/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1750 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/GUI.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     5466 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/IQCalibration.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     2283 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/Modelisation.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    45994 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/SinglePhotonProcess.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/__init__.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    12011 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/cmplxIQ.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    48530 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/resonator.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    23078 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/Functions/utility.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      519 2023-02-13 11:01:18.000000 spiakid-drs-0.1/src/Interface.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-02-09 09:47:58.000000 spiakid-drs-0.1/src/__init__.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1587 2023-02-13 14:49:47.000000 spiakid-drs-0.1/src/prototype.py
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.809846 spiakid-drs-0.1/src/spiakid_drs.egg-info/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1675 2023-02-14 16:15:20.000000 spiakid-drs-0.1/src/spiakid_drs.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      939 2023-02-14 16:15:20.000000 spiakid-drs-0.1/src/spiakid_drs.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        1 2023-02-14 16:15:20.000000 spiakid-drs-0.1/src/spiakid_drs.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       40 2023-02-14 16:15:20.000000 spiakid-drs-0.1/src/spiakid_drs.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       48 2023-02-14 16:15:20.000000 spiakid-drs-0.1/src/spiakid_drs.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.801846 spiakid-drs-0.1/src/venv_DRS/
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.833846 spiakid-drs-0.1/src/venv_DRS/bin/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1176 2023-02-13 12:50:26.000000 spiakid-drs-0.1/src/venv_DRS/bin/activate_this.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      619 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2html.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      741 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2html4.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)     1086 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2html5.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      818 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2latex.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      641 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2man.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      807 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2odt.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)     1745 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      626 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2pseudoxml.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      662 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2s5.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      898 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2xetex.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      627 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rst2xml.py
--rwxrwxr-x   0 sfaes     (1000) sfaes     (1000)      695 2023-02-13 12:51:37.000000 spiakid-drs-0.1/src/venv_DRS/bin/rstpep2html.py
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-02-14 16:15:20.833846 spiakid-drs-0.1/tests/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      159 2023-02-09 09:47:58.000000 spiakid-drs-0.1/tests/test_prototype.py
+drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    10173 2023-03-15 14:15:26.000000 spiakid-drs-0.11/LICENSE
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1676 2023-04-18 13:50:55.471867 spiakid-drs-0.11/PKG-INFO
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     2552 2023-03-15 14:15:26.000000 spiakid-drs-0.11/README.md
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1262 2023-03-15 14:15:26.000000 spiakid-drs-0.11/README_for_pip.md
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      580 2023-04-18 13:49:31.000000 spiakid-drs-0.11/pyproject.toml
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       38 2023-04-18 13:50:55.471867 spiakid-drs-0.11/setup.cfg
+drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.463867 spiakid-drs-0.11/src/
+drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.467867 spiakid-drs-0.11/src/Functions/
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1926 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Data.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     5329 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/IQCalibration.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     3105 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Modelisation.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     9399 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pixel.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     4915 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Plot.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     7577 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pulse_Timeline.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     3331 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pulse_average.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-03-15 14:15:26.000000 spiakid-drs-0.11/src/Functions/__init__.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    11983 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/cmplxIQ.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    48462 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/resonator.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    11933 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/utility.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1906 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Interface.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-03-15 14:15:26.000000 spiakid-drs-0.11/src/__init__.py
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1466 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/prototype.py
+drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/src/spiakid_drs.egg-info/
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1676 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      612 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        1 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       40 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       39 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/tests/
+-rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      159 2023-03-15 14:15:26.000000 spiakid-drs-0.11/tests/test_prototype.py
```

### Comparing `spiakid-drs-0.1/LICENSE` & `spiakid-drs-0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.1/PKG-INFO` & `spiakid-drs-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.1
+Version: 0.11
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `spiakid-drs-0.1/README.md` & `spiakid-drs-0.11/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,28 +22,35 @@
 virtualenv venv_DRS # Create a virtual environment for the DRS
 source venv_DRS/bin/activate # Activate the virtual environment for the DRS
 ```
 then, install the SPIAKID DRS with pip:
 ```
 pip install spiakid-drs
 ```
+or, if **virtualenvwrapper** is already installed, you can use
+```
+mkvirtualenv -i spiakid-drs -p python3 DRS 
+```
+An other way to use DRS is in a Docker container. You can find indications [here](https://spiakid.pages.obspm.fr/DRS/usage.html#docker).
 
 Latest version of DRS can be downloaded from this Gitlab with **git** command:
 ```
 git clone https://gitlab.obspm.fr/spiakid/DRS.git
 ```
 or
 
 ```
 git clone git@gitlab.obspm.fr:spiakid/DRS.git
 ```
 ### Requirements
 The SPIAKID DRS requires Python 3.8 or later.
 
+### Example
 
+You can find examples [here](https://spiakid.pages.obspm.fr/DRS/usage.html#example-1-mkid-feature-review).
 
 ## Authors
 The DRS is developped by Pasquale Panuzzo, Sebastien Faes, ...
 
 
 ## Project status and roadmap
 The DRS is in a prototyping stage
```

### Comparing `spiakid-drs-0.1/README_for_pip.md` & `spiakid-drs-0.11/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.1/src/Functions/IQCalibration.py` & `spiakid-drs-0.11/src/Functions/IQCalibration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.optimize import curve_fit
 import scipy.interpolate as interp;
-import lmfit as lm
+import Functions.utility as ut
 
 
-
-def fit_sin(t,A,phi,I0,f):
-
-    return A*np.sin(2*np.pi*f*t + phi) + I0
-
-def fit_cos(t,A,phi,I0,f):
-    
-    return A*np.cos(2*np.pi*f*t + phi) + I0
-
 def IQ_binary_old(filename):
     
     data = np.fromfile(filename,dtype=float,count = -1,sep = '')
     data_len = int((len(data)-1)/2)
     
     time = data[0]*np.arange(0,data_len)
     I = data[1:data_len+1]
@@ -34,17 +25,17 @@
     Q = data[data_len+2:]
     return time,I, Q
 
 def GetAmpPhaseError(t,I,Q,IF_freq,isplotting = False):
     
     #take the I as an reference for calibration
   
-    poptQ,pcovQ = curve_fit(lambda t,A,phi,Q0: fit_sin(t,A,phi,Q0,IF_freq),t,Q)
+    poptQ,pcovQ = curve_fit(lambda t,A,phi,Q0: ut.fit_sin(t,A,phi,Q0,IF_freq),t,Q)
 
-    poptI,pcovI = curve_fit(lambda t,A,phi,I0: fit_cos(t,A,phi,I0,IF_freq),t,I)
+    poptI,pcovI = curve_fit(lambda t,A,phi,I0: ut.fit_cos(t,A,phi,I0,IF_freq),t,I)
 
     AQ = poptQ[0]
     phiQ = poptQ[1]
     Q0 = poptQ[2]
     
     # print("AQ:",AQ)
     # print("APhi:",phiQ)
@@ -53,16 +44,16 @@
     phiI = poptI[1]
     I0 = poptI[2]
     
     delta_amp = AI/AQ
     delta_phi = phiQ-phiI
     
     if isplotting == True:
-        I_fit = fit_cos(t,AI,phiI,I0,IF_freq)
-        Q_fit = fit_sin(t,AQ,phiQ,Q0,IF_freq)
+        I_fit = ut.fit_cos(t,AI,phiI,I0,IF_freq)
+        Q_fit = ut.fit_sin(t,AQ,phiQ,Q0,IF_freq)
         
         f,(ax1,ax2) = plt.subplots(2,1,sharex = True)
         ax1.plot(t*1e6,I,label = 'I Meas')
         ax1.plot(t*1e6,I_fit,label = 'I Fit')
         
         ax1.legend()
         
@@ -81,18 +72,14 @@
         ax2.legend()
         plt.tight_layout()
         
         
     
     return delta_amp,delta_phi,I0,Q0
     
-    
-
-
-
 def IQCal(I,Q,delta_A,delta_phi,I0 = 0,Q0 = 0):
     
     #calibrate the DC offset
     #I: the raw I data
     #Q: the raw Q data
     #delta_A: the radio of the amp of Q and I
     #delta_phi: the phase imbalance between I and Q
@@ -183,24 +170,22 @@
     S21 = 10**(amp/20)*np.exp(1j*phase)
     
     I = np.real(S21)
     Q = np.imag(S21)
     
     return freq,I,Q
     
-
 def IQ_CalNoise(I,Q,freq_noise,freq,I0,Q0,IQ_caldata):
     
     indx,delta_A,delta_phase,I0_noise,Q0_noise = IQ_noiseCaldata(freq_noise,freq,I0,Q0,IQ_caldata)
     
     ICal,QCal = IQCal(I,Q,delta_A,delta_phase,I0_noise,Q0_noise)
     
     return ICal,QCal
     
-
 def IQ_noiseCaldata(freq_noise,freq,I0,Q0,IQ_caldata):
     
     
     freq_cal = IQ_caldata[:,0]
     amp_imbalance = IQ_caldata[:,1]
     phase_imbalance = IQ_caldata[:,2]
```

### Comparing `spiakid-drs-0.1/src/Functions/Modelisation.py` & `spiakid-drs-0.11/src/Functions/Modelisation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,86 @@
-import numpy as np
-import h5py
-import matplotlib.pyplot as plt
-import lmfit as lf
-import glob
-import scipy.signal as sps
-from scipy import interpolate as interp
-
 import Functions.resonator as a
-import Functions.SinglePhotonProcess as spp
 import Functions.cmplxIQ as fitmodel
+import Functions.Pulse_Timeline as PT
+import Functions.Pulse_average as PA
+import Functions.Pixel as PX
+import Functions.Data as dt
+import Functions.Plot as pl
 
-def Data_read(Data,Plot_path,Plot_Format):
-    f = h5py.File(Data,'r')
+def Data_read(Data,Plot_path,Plot_Format,Plot_List,Level,meas,IQ_number):
+    data = dt.read_hdf5(Data)
 #get the temp and readout power of the measurement
-    temp = f['header'].attrs['temp']
-    pwr = f['header'].attrs['power']
+    temp = data['temp']
+    pwr = data['pwr']
 
 #get frequency, I and Q of the resonator 
-    freq = f['resonator/freq'][...]
-    I = f['resonator/I'][...]
-    Q = f['resonator/Q'][...]
+    freq = data['freq']
+    I = data['I']
+    Q = data['Q']
 
-    I0 = f['resonator/I0'][...]
-    Q0 = f['resonator/Q0'][...]
+    I0 = data['I0']
+    Q0 = data['Q0']
 
     #get the IQ calibation data for the noise and pulse data
-    IQCaldata = f['calibration/IQCaldata'][...]
+    IQCaldata = data['IQCaldata']
 
     #create a resonator object
     res = a.Resonator('1', temp, pwr, freq, I, Q,I0 = I0,Q0 = Q0)
     #fit the resonator with S21 (transmission)
     res.load_params(fitmodel.cmplxIQ_params)
     res.do_lmfit(fitmodel.cmplxIQ_fit)
 
     t_offset = 0.001
-    binsize = 500
+    binsize_pulse = 500
+    binsize_hist = 0.1
 
     templatetime = 0.002
 
-    laserfreq = f['pulse'].attrs['laserfreq']
+    laserfreq = data['laserfreq']
     pulsetriggertime = 1/laserfreq/2 - t_offset
     savefolder = Plot_path
-    samplefreq = f['pulse'].attrs['samplefreq']
+    samplefreq = data['samplefreq']
+    #TODO Ask photonum on the interface
+    if Level == 2:
+        x = PX.Pixel(data,res,t_offset,binsize_pulse=500,binsize_hist=0.1,peakwidth=2,photonum=2)
+    
+    if Level == 1:
+        x = PA.Pulse_average(res,data,t_offset,binsize_pulse)
+
+    if Level == 0:
+        x = PT.Pulse_Timeline(data['IQ%d'%(meas)],data,res,t_offset,binsize_pulse)
+
+
+    if 0 in Plot_List:
+        pl.Energy_Resolution(x,binsize_hist,photonum=2,Format=Plot_Format,savefolder=savefolder)
+    if 1 in Plot_List:
+        pl.Pulse_Height(x, binsize_hist, Format =Plot_Format, savefolder=savefolder)
+    if 2 in Plot_List:
+        pl.Avg_pulse(x, Format =Plot_Format, savefolder=savefolder, fit=True)
+    if 3 in Plot_List:
+        pl.Avg_pulse_timeline(x,meas,Level, Format =Plot_Format, savefolder=savefolder)
+    if 4 in Plot_List:
+        pl.pulse_timeline(x,meas,IQ_number,Level, Format =Plot_Format, savefolder=savefolder)
+    
+
+
+
+
 
     #generate the averaged pulse data as the template
-    avedata = spp.GenPulseAverageWithHDF(res,f,savefolder,IQCaldata,calibrate_drift = True, t_offset = t_offset,savefig = True,Format=Plot_Format)
+    # avedata = spp.GenPulseAverageWithHDF(res,f,savefolder,IQCaldata,calibrate_drift = True, t_offset = t_offset,savefig = True,Format=Plot_Format)
 
-    #generate the psd (Power Spectral Density) of the resonator
-    psd = spp.GenPSDWithHDF(res,f,savefolder,IQCaldata,binsize = binsize,pulselaser = laserfreq,Format=Plot_Format)
+    # #generate the psd (Power Spectral Density) of the resonator
+    # psd = spp.GenPSDWithHDF(res,f,savefolder,IQCaldata,binsize = binsize,pulselaser = laserfreq,Format=Plot_Format)
 
 
-    #generate the wiener filter for both amplitude and phase
-    wifilterphase, wifilteramp,indx = spp.GenWienerFilter(avedata,psd,savefolder,binsize = binsize,pulsetriggertime = pulsetriggertime,dt = 1/samplefreq, templatetime = templatetime,Format=Plot_Format)
+    # #generate the wiener filter for both amplitude and phase
+    # wifilterphase, wifilteramp,indx = spp.GenWienerFilter(avedata,psd,savefolder,binsize = binsize,pulsetriggertime = pulsetriggertime,dt = 1/samplefreq, templatetime = templatetime,Format=Plot_Format)
 
-    #use the wiener filter to generate the pulse statistics
-    pulseheights = spp.GenPulseStatisticsHDF(res,f,wifilterphase,savefolder,IQCaldata,binsize = binsize,t_offset = t_offset,calibrate_drift = True,pulsetype = 'phase',plotbin = 0.2,Format=Plot_Format)
+    # #use the wiener filter to generate the pulse statistics
+    # pulseheights = spp.GenPulseStatisticsHDF(res,f,wifilterphase,savefolder,IQCaldata,binsize = binsize,t_offset = t_offset,calibrate_drift = True,pulsetype = 'phase',plotbin = 0.2,Format=Plot_Format)
 
-    #estimate the energy resolution
-    spp.EnergyResolution(pulseheights,savefolder,photonum = 6,Format=Plot_Format)
+    # #estimate the energy resolution
+    # spp.EnergyResolution(pulseheights,savefolder,photonum = 6,Format=Plot_Format)
```

### Comparing `spiakid-drs-0.1/src/Functions/cmplxIQ.py` & `spiakid-drs-0.11/src/Functions/cmplxIQ.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings
 import numpy as np
 import scipy.signal as sps
-import scipy.special as spc
 import lmfit as lf
 
 # def cmplxIQ_fit(paramsVec, freqs, data=None, eps=None, **kwargs):
 def cmplxIQ_fit(paramsVec, res, residual=True, **kwargs):
     """Return complex S21 resonance model or, if data is specified, a residual.
 
     Parameters
```

### Comparing `spiakid-drs-0.1/src/Functions/resonator.py` & `spiakid-drs-0.11/src/Functions/resonator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import lmfit as lf
 import glob
 import scipy.signal as sps
-from scipy import interpolate as interp
 import pandas as pd
 
 class Resonator(object):
     r"""Fit an S21 measurement of a hanger (or notch) type resonator.
 
     Parameters
     ----------
@@ -493,16 +492,14 @@
             
             
         
         
             
         return pulse_amp,pulse_phase
         
-        
-        
     def cal_pulse_outside(self,pulsedata,pulsefreqmeas,pulsewidth = 50,fs = 5e6):
         
         # if self.hasnoisedata == True:
         indx = np.argmin(np.abs(self.freq-pulsefreqmeas))
         indx = indx
         
         #the delay of the transmission 
@@ -1000,18 +997,14 @@
     
     for i, freqseg in enumerate(freqsegs):
         
         sumpoints = round(respoints[i]/df);
         
         segpoints = freqsegs
         
-    
-
-
-
 def RemoveGlich(data,sigma_level = 5):
     
     # assume that the data is normal distributed;
     
     # data_amp = np.abs(data)
     
     mean = np.mean(data)           
@@ -1267,16 +1260,14 @@
 
     block = zip(*tlists)
 
     print(repr(list(pwrs)).replace(',', ',\t'))
     for b in block:
         print(repr(b).replace(',', ',\t'))
 
-
-
 def block_check_resList(resList, sdev=0.005, prune=False, verbose=True):
     """Helper tool for preparing a resList with missing data for resSweep"""
     #Get all possible powers
     pwrs = np.unique([res.pwr for res in resList])
 
     #This will hold a list of temps at each power
     tlists = []
```

### Comparing `spiakid-drs-0.1/src/prototype.py` & `spiakid-drs-0.11/src/prototype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import h5py
-import sys
-import numpy as np
-import pandas as pd
 from Functions import Modelisation as mod
 import os
 import argparse
 from pathlib import Path
 import pathlib
 
-
+"""
+Link between Terminal and pipeline
+"""
 def parse():
     # read in command line arguments
     parser = argparse.ArgumentParser(description='MKID Pipeline CLI')
     parser.add_argument('--init', action='store_true', help='launch the interface')
-    # parser.add_argument('--dinit', action='store_true', help='launch the interface through docker')
     parser.add_argument('--outp', help='output destination', dest='out_cfg', default=None)
     parser.add_argument('--inp', help='data location', dest='in_cfg' , default=None)
     parser.add_argument('--format', help='format of the plot', default='.jpg', dest='form')
     parser.add_argument('--dir', help='create input and output folder', action='store_true')
     return parser.parse_args()
 
 
@@ -25,14 +22,15 @@
     args = parse()
 
     if args.init:
         try:
             path = str(sorted(pathlib.Path('/').glob('**/Interface.py'))[0]) #Docker version
         except:
             path = str(sorted(pathlib.Path('').glob('**/Interface.py'))[0])  #Terminal version
+
         os.system("streamlit run "+path)
     
     if args.out_cfg!=None and args.in_cfg!=None:
         mod.Data_read(args.in_cfg,args.out_cfg,args.form)
         print('Done')
 
     if args.dir:
```

### Comparing `spiakid-drs-0.1/src/spiakid_drs.egg-info/PKG-INFO` & `spiakid-drs-0.11/src/spiakid_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.1
+Version: 0.11
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

