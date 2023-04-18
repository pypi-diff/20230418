# Comparing `tmp/copasi-petab-importer-1.0.2.tar.gz` & `tmp/copasi-petab-importer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\copasi-petab-importer-1.0.2.tar", last modified: Tue Sep 28 11:22:45 2021, max compression
+gzip compressed data, was "copasi-petab-importer-1.0.3.tar", last modified: Tue Apr 18 05:53:43 2023, max compression
```

## Comparing `copasi-petab-importer-1.0.2.tar` & `copasi-petab-importer-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/
--rw-rw-rw-   0        0        0       66 2021-09-27 13:46:37.000000 copasi-petab-importer-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      329 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3321 2021-06-08 15:00:51.000000 copasi-petab-importer-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/
--rw-rw-rw-   0        0        0     9394 2021-09-27 14:45:08.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/PEtab.py
--rw-rw-rw-   0        0        0      324 2021-09-27 14:44:36.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/__init__.py
--rw-rw-rw-   0        0        0      518 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/_version.py
--rw-rw-rw-   0        0        0     1965 2021-09-27 13:10:20.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/convert_all_petab.py
--rw-rw-rw-   0        0        0     4715 2021-09-27 13:10:20.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/convert_benchmark.py
--rw-rw-rw-   0        0        0    33541 2021-09-28 11:11:08.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/convert_petab.py
--rw-rw-rw-   0        0        0    12717 2020-03-25 13:15:25.000000 copasi-petab-importer-1.0.2/copasi_petab_importer/petab.ui
-drwxrwxrwx   0        0        0        0 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/
--rw-rw-rw-   0        0        0      329 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      255 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      925 2021-09-27 13:50:14.000000 copasi-petab-importer-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-28 11:22:45.000000 copasi-petab-importer-1.0.2/test/
--rw-rw-rw-   0        0        0     1416 2021-09-28 11:22:23.000000 copasi-petab-importer-1.0.2/test/test_importer.py
--rw-rw-rw-   0        0        0    78254 2021-09-27 13:48:22.000000 copasi-petab-importer-1.0.2/versioneer.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816281 copasi-petab-importer-1.0.3/
+-rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-04-18 05:53:43.816325 copasi-petab-importer-1.0.3/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)     3253 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816634 copasi-petab-importer-1.0.3/copasi_petab_importer/
+-rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/PEtab.py
+-rw-r--r--   0 frank      (501) staff       (20)      311 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      497 2023-04-18 05:53:43.816667 copasi-petab-importer-1.0.3/copasi_petab_importer/_version.py
+-rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_all_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_benchmark.py
+-rw-r--r--   0 frank      (501) staff       (20)    33406 2023-04-17 21:25:19.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/convert_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/copasi_petab_importer/petab.ui
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816031 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)      279 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      603 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)      138 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)       62 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       22 2023-04-18 05:53:43.000000 copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/top_level.txt
+-rw-r--r--   0 frank      (501) staff       (20)      243 2023-04-18 05:53:43.816499 copasi-petab-importer-1.0.3/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-04-18 05:53:43.816140 copasi-petab-importer-1.0.3/test/
+-rw-r--r--   0 frank      (501) staff       (20)     1916 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/test/test_importer.py
+-rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.3/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `copasi-petab-importer-1.0.2/README.md` & `copasi-petab-importer-1.0.3/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-## PEtab Importer
-This project holds the code to import the parameter estimation benchmark problems into [COPASI](https://copasi.org). The test cases it ought to be able to deal with are from this project: 
-
-* [Benchmark-Models](https://github.com/LeonardSchmiester/Benchmark-Models)
-
-These models are encoded in the [PEtab](https://github.com/ICB-DCM/PEtab/) format with this [documentation](https://github.com/ICB-DCM/PEtab/blob/master/doc/documentation_data_format.md). The format specifies: 
-
-* an SBML file with the model definition
-* a measurement file with the experimental data
-* a condition file that specifies different initial conditions
-
-So this converter 1. reads the SBML file and converts it to the COPASI format, then converts the experimental data so we can use it in COPASI, and provides the mapping to the observables. Once the converter is done, and you run the parameter estimation you will get the current solution displayed. 
-
-The benchmarks are also added as submodule to this repo. So if you do want to use those, be sure to check it out as well, running: 
-
-	git submodule init 
-	git submodule update
-
-
-### Setup
-Create a new virtual environment, and then run `pip install -r requirements.txt`. This will install all the dependencies, these are: 
-
-- numpy
-- pandas
-- python-copasi
-- python-libsbml
-- PyQt5
-- pyyaml
-
-You can also directly install the importer in one line directly from git (including the dependencies) using: 
-
-	pip install git+https://github.com/copasi/python-petab-importer.git
-
-and you can run directly: 
-
-	copasi_petab_import  [<petab_dir>]  <model_name> <output_dir>
-
-### Usage
-Once installed, you can use the graphical user interface, specify the benchmark directory, select the test and the model, and you ought to be able to open the generated COPASI file directly. You do this by running: 
-
-    python PEtab.py
-    
-<img src="./doc/demo.gif">
-    
-Alternatively you cold convert the benchmark models directly by invoking the converter: 
-
-    python convert_petab.py <benchmark_dir> <model_name> <output_dir>
-    
-where:
-
-  * `benchmark_dir` is a directory to a pe tab dir, like `./hackathon_contributions_new_data_format/Becker_Science2010`.
-  * `model_name` is one of the model names in the directory like `Becker_Science2010__BaF3_Exp`. The program assumes, that the measurement data and condition data files are in the directory containing the model name (otherwise any measurement / condition file will be greedily taken)
-  * `output_dir` is the directory into which the output will be written. For example '/out'. In this case at the end of the run the files `Becker_Science2010__BaF3_Exp.cps` and `Becker_Science2010__BaF3_Exp.txt` would be generated. 
-
-Also added a bulk converter: 
-
-    python convert_all_petab.py <base_dir> <output_dir>
-    
-where:
-
-  * `base_dir` is the pe tab root dir, as in `./hackathon_contributions_new_data_format/`
-  * `output_dir` the directory in which the files will be saved in
-
-### License
-Just as COPASI, the packages available on this page are provided under the 
-[Artistic License 2.0](http://copasi.org/Download/License/), 
-which is an [OSI](http://www.opensource.org/) approved license. This license 
-allows non-commercial and commercial use free of charge.
+## PEtab Importer
+This project holds the code to import the parameter estimation benchmark problems into [COPASI](https://copasi.org). The test cases it ought to be able to deal with are from this project: 
+
+* [Benchmark-Models](https://github.com/LeonardSchmiester/Benchmark-Models)
+
+These models are encoded in the [PEtab](https://github.com/ICB-DCM/PEtab/) format with this [documentation](https://github.com/ICB-DCM/PEtab/blob/master/doc/documentation_data_format.md). The format specifies: 
+
+* an SBML file with the model definition
+* a measurement file with the experimental data
+* a condition file that specifies different initial conditions
+
+So this converter 1. reads the SBML file and converts it to the COPASI format, then converts the experimental data so we can use it in COPASI, and provides the mapping to the observables. Once the converter is done, and you run the parameter estimation you will get the current solution displayed. 
+
+The benchmarks are also added as submodule to this repo. So if you do want to use those, be sure to check it out as well, running: 
+
+	git submodule init 
+	git submodule update
+
+
+### Setup
+Create a new virtual environment, and then run `pip install -r requirements.txt`. This will install all the dependencies, these are: 
+
+- numpy
+- pandas
+- python-copasi
+- python-libsbml
+- PyQt5
+- pyyaml
+
+You can also directly install the importer in one line directly from git (including the dependencies) using: 
+
+	pip install git+https://github.com/copasi/python-petab-importer.git
+
+and you can run directly: 
+
+	copasi_petab_import  [<petab_dir>]  <model_name> <output_dir>
+
+### Usage
+Once installed, you can use the graphical user interface, specify the benchmark directory, select the test and the model, and you ought to be able to open the generated COPASI file directly. You do this by running: 
+
+    python PEtab.py
+    
+<img src="./doc/demo.gif">
+    
+Alternatively you cold convert the benchmark models directly by invoking the converter: 
+
+    python convert_petab.py <benchmark_dir> <model_name> <output_dir>
+    
+where:
+
+  * `benchmark_dir` is a directory to a pe tab dir, like `./hackathon_contributions_new_data_format/Becker_Science2010`.
+  * `model_name` is one of the model names in the directory like `Becker_Science2010__BaF3_Exp`. The program assumes, that the measurement data and condition data files are in the directory containing the model name (otherwise any measurement / condition file will be greedily taken)
+  * `output_dir` is the directory into which the output will be written. For example '/out'. In this case at the end of the run the files `Becker_Science2010__BaF3_Exp.cps` and `Becker_Science2010__BaF3_Exp.txt` would be generated. 
+
+Also added a bulk converter: 
+
+    python convert_all_petab.py <base_dir> <output_dir>
+    
+where:
+
+  * `base_dir` is the pe tab root dir, as in `./hackathon_contributions_new_data_format/`
+  * `output_dir` the directory in which the files will be saved in
+
+### License
+Just as COPASI, the packages available on this page are provided under the 
+[Artistic License 2.0](http://copasi.org/Download/License/), 
+which is an [OSI](http://www.opensource.org/) approved license. This license 
+allows non-commercial and commercial use free of charge.
```

### Comparing `copasi-petab-importer-1.0.2/copasi_petab_importer/PEtab.py` & `copasi-petab-importer-1.0.3/copasi_petab_importer/PEtab.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-import os
-import sys
-import traceback
-from PyQt5.QtWidgets import QMainWindow, QDesktopWidget, QApplication, \
-    QFileDialog, QMessageBox
-from PyQt5 import uic
-from PyQt5.QtCore import QUrl, QSettings, Qt
-from PyQt5.QtGui import QDesktopServices
-
-from copasi_petab_importer import convert_petab
-
-
-class PETabGui(QMainWindow):
-
-    def __init__(self):
-        # super().__init__()
-        QMainWindow.__init__(self)
-
-        self.dir = None
-        self.model_dir = None
-        self.model = None
-        self.out_dir = None
-        self.show_progress = True
-        self.show_result = True
-        self.show_result_per_experiment = False
-        self.show_result_per_dependent = False
-        self.write_report = False
-
-        self.ui = uic.loadUi(os.path.join(os.path.dirname(__file__), 'petab.ui'), self)
-
-        self.center()
-        self.load_settings()
-        self.load_model_dirs()
-        self.show()
-
-    def closeEvent(self, event):
-        self.save_settings()
-
-    @staticmethod
-    def _get_user_dir():
-        home = os.getenv("HOME")
-        if home is not None:
-            return home
-        from pathlib import Path
-        return Path.home()
-
-    def load_settings(self):
-        settings = QSettings(os.path.join(PETabGui._get_user_dir(), ".petab.ini"), QSettings.IniFormat)
-
-        benchmark_dir = '../benchmarks/hackathon_contributions_new_data_format'
-        self.dir = settings.value("dir", benchmark_dir)
-        self.model_dir = settings.value("model_dir", r'Becker_Science2010')
-        self.model = settings.value("model", 'Becker_Science2010__BaF3_Exp')
-        self.out_dir = settings.value("out_dir", './out')
-        self.show_progress = settings.value("show_progress", True, type=bool)
-        self.show_result = settings.value("show_result", True, type=bool)
-        self.show_result_per_experiment = settings.value("show_result_per_experiment", False, type=bool)
-        self.show_result_per_dependent = settings.value("show_result_per_dependent", False, type=bool)
-        self.write_report = settings.value("write_report", False, type=bool)
-
-        self.ui.txtDir.setText(self.dir)
-        self.ui.txtOutDir.setText(self.out_dir)
-        self.ui.chkPlotProgressOfFit.setChecked(self.show_progress)
-        self.ui.chkPlotResult.setChecked(self.show_result)
-        self.ui.chkPlotResultPerExperiment.setChecked(self.show_result_per_experiment)
-        self.ui.chkPlotResultPerDependent.setChecked(self.show_result_per_dependent)
-        self.ui.chkWriteReport.setChecked(self.write_report)
-
-    def save_settings(self):
-        settings = QSettings(os.path.join(PETabGui._get_user_dir(), ".petab.ini"), QSettings.IniFormat)
-        settings.setValue("dir", self.dir)
-        settings.setValue("model_dir", self.model_dir)
-        settings.setValue("model", self.model)
-        settings.setValue("out_dir", self.out_dir)
-        settings.setValue("show_progress", self.show_progress)
-        settings.setValue("show_result", self.show_result)
-        settings.setValue("show_result_per_experiment", self.show_result_per_experiment)
-        settings.setValue("show_result_per_dependent", self.show_result_per_dependent)
-        settings.setValue("write_report", self.write_report)
-
-    def slotOpenModelDir(self):
-        url = QUrl.fromLocalFile(os.path.join(self.dir, self.model_dir))
-        QDesktopServices.openUrl(url)
-
-    def slotOpenInCOPASI(self):
-        QDesktopServices.openUrl(
-            QUrl.fromLocalFile(
-                os.path.join(self.out_dir, os.path.splitext(self.model)[0] + '.cps')))
-
-    def slotSetBenchmarkDir(self, dir):
-        if not os.path.exists(dir):
-            return
-        self.dir = dir
-        self.ui.txtDir.setText(dir)
-        self.load_model_dirs()
-
-    def slotSetModelDir(self, model_dir):
-        self.model_dir = model_dir
-        items = self.ui.lstModelDirs.findItems(self.model_dir,
-                                               Qt.MatchFixedString)
-        if len(items) > 0:
-            self.ui.lstModelDirs.setCurrentItem(items[0])
-        self.load_models()
-
-    def slotSetModel(self, model):
-        self.model = model
-        self.setWindowFilePath(model)
-        items = self.ui.lstModels.findItems(self.model, Qt.MatchFixedString)
-        if len(items) > 0:
-            self.ui.lstModels.setCurrentItem(items[0])
-
-    def slotSetOutputDir(self, out_dir):
-        self.out_dir = out_dir
-        self.ui.txtOutDir.setText(out_dir)
-
-    def slotBrowseBenchmarkDir(self):
-        result = QFileDialog.getExistingDirectory(self,
-                                                  'Select Benchmark dir',
-                                                  self.dir)
-        if result is None:
-            return
-        self.slotSetBenchmarkDir(result)
-
-    def slotModelDirSelected(self):
-        selected = self.ui.lstModelDirs.currentItem()
-        if selected is None:
-            self.model_dir = None
-        else:
-            self.model_dir = selected.text()
-        self.slotSetModelDir(self.model_dir)
-
-    def load_model_dirs(self):
-        self.ui.lstModelDirs.clear()
-        if self.dir is None or not os.path.exists(self.dir):
-            return
-        for (dirpath, dirnames, filenames) in os.walk(self.dir):
-            self.ui.lstModelDirs.addItems(sorted(dirnames))
-            break  # only from top level
-        if self.model_dir is not None:
-            self.slotSetModelDir(self.model_dir)
-
-    def load_models(self):
-        self.ui.lstModels.clear()
-        self.model = None
-        full_dir = os.path.join(self.dir, self.model_dir)
-        if self.model_dir is None or not os.path.exists(full_dir):
-            self.ui.wdgDetail.setEnabled(False)
-            return
-        self.ui.wdgDetail.setEnabled(True)
-        yaml = None
-        for (dirpath, dirnames, filenames) in os.walk(full_dir):
-            for file in sorted(filenames):
-                if file.startswith('model_'):
-                    file = file[6:]
-                if file.endswith('.xml'):
-                    file = file[:-4]
-                    self.ui.lstModels.addItem(file)
-                    self.model = file
-                if file.endswith('.yaml') and not '_solution' in file:
-                    self.ui.lstModels.addItem(file)
-                    yaml = file
-            break  # skip other dirs
-        if yaml is not None:
-            self.model = yaml
-            self.slotSetModel(yaml)
-        elif self.model is not None:
-            self.slotSetModel(self.model)
-
-    def slotModelSelected(self):
-        selected = self.ui.lstModels.currentItem()
-        if selected is None:
-            return
-        self.slotSetModel(selected.text())
-
-    def slotBrowseOutputDir(self):
-        result = QFileDialog.getExistingDirectory(self,
-                                                  'Select Output Folder',
-                                                  self.out_dir)
-        if result is None:
-            return
-        self.slotSetOutputDir(result)
-
-    def slotConvert(self):
-        self.ui.cmdConvert.setEnabled(False)
-        self.ui.cmdOpenInCOPASI.setEnabled(False)
-        QApplication.processEvents()
-        try:
-            self.out_dir = self.ui.txtOutDir.text()
-            self.show_progress = self.ui.chkPlotProgressOfFit.isChecked()
-            self.show_result = self.ui.chkPlotResult.isChecked()
-            self.show_result_per_experiment = self.ui.chkPlotResultPerExperiment.isChecked()
-            self.show_result_per_dependent = self.ui.chkPlotResultPerDependent.isChecked()
-            self.write_report = self.ui.chkWriteReport.isChecked()
-
-            if not os.path.exists(self.out_dir):
-                os.makedirs(self.out_dir, exist_ok=True)
-            full_dir = os.path.join(self.dir, self.model_dir)
-            converter = convert_petab.PEtabConverter(full_dir, self.model,
-                                                     self.out_dir, os.path.splitext(self.model)[0])
-            converter.transform_data = self.ui.chkTransformData.isChecked()
-            converter.show_progress_of_fit = self.show_progress
-            converter.show_result = self.show_result
-            converter.show_result_per_experiment = self.show_result_per_experiment
-            converter.show_result_per_dependent = self.show_result_per_dependent
-            converter.save_report = self.write_report
-            converter.convert()
-            if converter.experimental_data_file is not None:
-                with open(converter.experimental_data_file, 'r') as data:
-                    text = data.read()
-                    self.ui.txtData.document().setPlainText(text)
-        except BaseException:
-            msg = traceback.format_exc()
-            QMessageBox.critical(self, 'Error converting', msg)
-        self.ui.cmdConvert.setEnabled(True)
-        self.ui.cmdOpenInCOPASI.setEnabled(True)
-
-    def center(self):
-        qr = self.frameGeometry()
-        cp = QDesktopWidget().availableGeometry().center()
-        qr.moveCenter(cp)
-        self.move(qr.topLeft())
-
-
-def petab_gui():
-    app = QApplication(sys.argv)
-    widget = PETabGui()
-    sys.exit(app.exec_())
-
-
-if __name__ == '__main__':
-    petab_gui()
+import os
+import sys
+import traceback
+from PyQt5.QtWidgets import QMainWindow, QDesktopWidget, QApplication, \
+    QFileDialog, QMessageBox
+from PyQt5 import uic
+from PyQt5.QtCore import QUrl, QSettings, Qt
+from PyQt5.QtGui import QDesktopServices
+
+from copasi_petab_importer import convert_petab
+
+
+class PETabGui(QMainWindow):
+
+    def __init__(self):
+        # super().__init__()
+        QMainWindow.__init__(self)
+
+        self.dir = None
+        self.model_dir = None
+        self.model = None
+        self.out_dir = None
+        self.show_progress = True
+        self.show_result = True
+        self.show_result_per_experiment = False
+        self.show_result_per_dependent = False
+        self.write_report = False
+
+        self.ui = uic.loadUi(os.path.join(os.path.dirname(__file__), 'petab.ui'), self)
+
+        self.center()
+        self.load_settings()
+        self.load_model_dirs()
+        self.show()
+
+    def closeEvent(self, event):
+        self.save_settings()
+
+    @staticmethod
+    def _get_user_dir():
+        home = os.getenv("HOME")
+        if home is not None:
+            return home
+        from pathlib import Path
+        return Path.home()
+
+    def load_settings(self):
+        settings = QSettings(os.path.join(PETabGui._get_user_dir(), ".petab.ini"), QSettings.IniFormat)
+
+        benchmark_dir = '../benchmarks/hackathon_contributions_new_data_format'
+        self.dir = settings.value("dir", benchmark_dir)
+        self.model_dir = settings.value("model_dir", r'Becker_Science2010')
+        self.model = settings.value("model", 'Becker_Science2010__BaF3_Exp')
+        self.out_dir = settings.value("out_dir", './out')
+        self.show_progress = settings.value("show_progress", True, type=bool)
+        self.show_result = settings.value("show_result", True, type=bool)
+        self.show_result_per_experiment = settings.value("show_result_per_experiment", False, type=bool)
+        self.show_result_per_dependent = settings.value("show_result_per_dependent", False, type=bool)
+        self.write_report = settings.value("write_report", False, type=bool)
+
+        self.ui.txtDir.setText(self.dir)
+        self.ui.txtOutDir.setText(self.out_dir)
+        self.ui.chkPlotProgressOfFit.setChecked(self.show_progress)
+        self.ui.chkPlotResult.setChecked(self.show_result)
+        self.ui.chkPlotResultPerExperiment.setChecked(self.show_result_per_experiment)
+        self.ui.chkPlotResultPerDependent.setChecked(self.show_result_per_dependent)
+        self.ui.chkWriteReport.setChecked(self.write_report)
+
+    def save_settings(self):
+        settings = QSettings(os.path.join(PETabGui._get_user_dir(), ".petab.ini"), QSettings.IniFormat)
+        settings.setValue("dir", self.dir)
+        settings.setValue("model_dir", self.model_dir)
+        settings.setValue("model", self.model)
+        settings.setValue("out_dir", self.out_dir)
+        settings.setValue("show_progress", self.show_progress)
+        settings.setValue("show_result", self.show_result)
+        settings.setValue("show_result_per_experiment", self.show_result_per_experiment)
+        settings.setValue("show_result_per_dependent", self.show_result_per_dependent)
+        settings.setValue("write_report", self.write_report)
+
+    def slotOpenModelDir(self):
+        url = QUrl.fromLocalFile(os.path.join(self.dir, self.model_dir))
+        QDesktopServices.openUrl(url)
+
+    def slotOpenInCOPASI(self):
+        QDesktopServices.openUrl(
+            QUrl.fromLocalFile(
+                os.path.join(self.out_dir, os.path.splitext(self.model)[0] + '.cps')))
+
+    def slotSetBenchmarkDir(self, dir):
+        if not os.path.exists(dir):
+            return
+        self.dir = dir
+        self.ui.txtDir.setText(dir)
+        self.load_model_dirs()
+
+    def slotSetModelDir(self, model_dir):
+        self.model_dir = model_dir
+        items = self.ui.lstModelDirs.findItems(self.model_dir,
+                                               Qt.MatchFixedString)
+        if len(items) > 0:
+            self.ui.lstModelDirs.setCurrentItem(items[0])
+        self.load_models()
+
+    def slotSetModel(self, model):
+        self.model = model
+        self.setWindowFilePath(model)
+        items = self.ui.lstModels.findItems(self.model, Qt.MatchFixedString)
+        if len(items) > 0:
+            self.ui.lstModels.setCurrentItem(items[0])
+
+    def slotSetOutputDir(self, out_dir):
+        self.out_dir = out_dir
+        self.ui.txtOutDir.setText(out_dir)
+
+    def slotBrowseBenchmarkDir(self):
+        result = QFileDialog.getExistingDirectory(self,
+                                                  'Select Benchmark dir',
+                                                  self.dir)
+        if result is None:
+            return
+        self.slotSetBenchmarkDir(result)
+
+    def slotModelDirSelected(self):
+        selected = self.ui.lstModelDirs.currentItem()
+        if selected is None:
+            self.model_dir = None
+        else:
+            self.model_dir = selected.text()
+        self.slotSetModelDir(self.model_dir)
+
+    def load_model_dirs(self):
+        self.ui.lstModelDirs.clear()
+        if self.dir is None or not os.path.exists(self.dir):
+            return
+        for (dirpath, dirnames, filenames) in os.walk(self.dir):
+            self.ui.lstModelDirs.addItems(sorted(dirnames))
+            break  # only from top level
+        if self.model_dir is not None:
+            self.slotSetModelDir(self.model_dir)
+
+    def load_models(self):
+        self.ui.lstModels.clear()
+        self.model = None
+        full_dir = os.path.join(self.dir, self.model_dir)
+        if self.model_dir is None or not os.path.exists(full_dir):
+            self.ui.wdgDetail.setEnabled(False)
+            return
+        self.ui.wdgDetail.setEnabled(True)
+        yaml = None
+        for (dirpath, dirnames, filenames) in os.walk(full_dir):
+            for file in sorted(filenames):
+                if file.startswith('model_'):
+                    file = file[6:]
+                if file.endswith('.xml'):
+                    file = file[:-4]
+                    self.ui.lstModels.addItem(file)
+                    self.model = file
+                if file.endswith('.yaml') and not '_solution' in file:
+                    self.ui.lstModels.addItem(file)
+                    yaml = file
+            break  # skip other dirs
+        if yaml is not None:
+            self.model = yaml
+            self.slotSetModel(yaml)
+        elif self.model is not None:
+            self.slotSetModel(self.model)
+
+    def slotModelSelected(self):
+        selected = self.ui.lstModels.currentItem()
+        if selected is None:
+            return
+        self.slotSetModel(selected.text())
+
+    def slotBrowseOutputDir(self):
+        result = QFileDialog.getExistingDirectory(self,
+                                                  'Select Output Folder',
+                                                  self.out_dir)
+        if result is None:
+            return
+        self.slotSetOutputDir(result)
+
+    def slotConvert(self):
+        self.ui.cmdConvert.setEnabled(False)
+        self.ui.cmdOpenInCOPASI.setEnabled(False)
+        QApplication.processEvents()
+        try:
+            self.out_dir = self.ui.txtOutDir.text()
+            self.show_progress = self.ui.chkPlotProgressOfFit.isChecked()
+            self.show_result = self.ui.chkPlotResult.isChecked()
+            self.show_result_per_experiment = self.ui.chkPlotResultPerExperiment.isChecked()
+            self.show_result_per_dependent = self.ui.chkPlotResultPerDependent.isChecked()
+            self.write_report = self.ui.chkWriteReport.isChecked()
+
+            if not os.path.exists(self.out_dir):
+                os.makedirs(self.out_dir, exist_ok=True)
+            full_dir = os.path.join(self.dir, self.model_dir)
+            converter = convert_petab.PEtabConverter(full_dir, self.model,
+                                                     self.out_dir, os.path.splitext(self.model)[0])
+            converter.transform_data = self.ui.chkTransformData.isChecked()
+            converter.show_progress_of_fit = self.show_progress
+            converter.show_result = self.show_result
+            converter.show_result_per_experiment = self.show_result_per_experiment
+            converter.show_result_per_dependent = self.show_result_per_dependent
+            converter.save_report = self.write_report
+            converter.convert()
+            if converter.experimental_data_file is not None:
+                with open(converter.experimental_data_file, 'r') as data:
+                    text = data.read()
+                    self.ui.txtData.document().setPlainText(text)
+        except BaseException:
+            msg = traceback.format_exc()
+            QMessageBox.critical(self, 'Error converting', msg)
+        self.ui.cmdConvert.setEnabled(True)
+        self.ui.cmdOpenInCOPASI.setEnabled(True)
+
+    def center(self):
+        qr = self.frameGeometry()
+        cp = QDesktopWidget().availableGeometry().center()
+        qr.moveCenter(cp)
+        self.move(qr.topLeft())
+
+
+def petab_gui():
+    app = QApplication(sys.argv)
+    widget = PETabGui()
+    sys.exit(app.exec_())
+
+
+if __name__ == '__main__':
+    petab_gui()
```

### Comparing `copasi-petab-importer-1.0.2/copasi_petab_importer/convert_all_petab.py` & `copasi-petab-importer-1.0.3/copasi_petab_importer/convert_all_petab.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from copasi_petab_importer import convert_petab
-import sys
-import os
-
-
-def convert_all_benchmarks(base_dir, out_dir):
-    dirs = None
-    for (dirpath, dirnames, filenames) in os.walk(base_dir):
-        dirs = sorted(dirnames)
-        break
-
-    for directory in dirs:
-        current_dir = os.path.join(base_dir, directory)
-        models = get_all_models(current_dir)
-        num_models = len(models)
-        if num_models == 0:
-            print("No models for %s ... skipping" % directory)
-            continue
-
-        for model in models:
-            if num_models == 1:
-                print("  Converting model {0}".format(model))
-            else:
-                print("  Converting model {0} of {1}".format(model, directory))
-
-            convert_model(current_dir, model, out_dir)
-
-    pass
-
-
-def get_all_models(current_dir):
-    models = []
-    for (dirpath, dirnames, filenames) in os.walk(current_dir):
-        for name in filenames:
-            assert (isinstance(name, str))
-            if name.endswith('.xml'):
-                name = name[:-4]
-                if name.startswith('model_'):
-                    name = name[6:]
-                models.append(name)
-        break
-    models = sorted(models)
-    return models
-
-
-def convert_model(current_dir, model, out_dir):
-    try:
-        worker = convert_petab.PEtabConverter(current_dir,
-                                              model, out_dir)
-        worker.convert()
-    except BaseException:
-        import traceback
-        print("Couldn't convert {0} due to\n\n{1}".format(
-            model, traceback.format_exc()))
-
-
-if __name__ == "__main__":
-    num_args = len(sys.argv)
-    if num_args > 2:
-        base_dir = sys.argv[1]
-        out_dir = sys.argv[2]
-    else:
-        base_dir = '../benchmarks/hackathon_contributions_new_data_format'
-        out_dir = '../out'
-
-    convert_all_benchmarks(base_dir, out_dir)
+from copasi_petab_importer import convert_petab
+import sys
+import os
+
+
+def convert_all_benchmarks(base_dir, out_dir):
+    dirs = None
+    for (dirpath, dirnames, filenames) in os.walk(base_dir):
+        dirs = sorted(dirnames)
+        break
+
+    for directory in dirs:
+        current_dir = os.path.join(base_dir, directory)
+        models = get_all_models(current_dir)
+        num_models = len(models)
+        if num_models == 0:
+            print("No models for %s ... skipping" % directory)
+            continue
+
+        for model in models:
+            if num_models == 1:
+                print("  Converting model {0}".format(model))
+            else:
+                print("  Converting model {0} of {1}".format(model, directory))
+
+            convert_model(current_dir, model, out_dir)
+
+    pass
+
+
+def get_all_models(current_dir):
+    models = []
+    for (dirpath, dirnames, filenames) in os.walk(current_dir):
+        for name in filenames:
+            assert (isinstance(name, str))
+            if name.endswith('.xml'):
+                name = name[:-4]
+                if name.startswith('model_'):
+                    name = name[6:]
+                models.append(name)
+        break
+    models = sorted(models)
+    return models
+
+
+def convert_model(current_dir, model, out_dir):
+    try:
+        worker = convert_petab.PEtabConverter(current_dir,
+                                              model, out_dir)
+        worker.convert()
+    except BaseException:
+        import traceback
+        print("Couldn't convert {0} due to\n\n{1}".format(
+            model, traceback.format_exc()))
+
+
+if __name__ == "__main__":
+    num_args = len(sys.argv)
+    if num_args > 2:
+        base_dir = sys.argv[1]
+        out_dir = sys.argv[2]
+    else:
+        base_dir = '../benchmarks/hackathon_contributions_new_data_format'
+        out_dir = '../out'
+
+    convert_all_benchmarks(base_dir, out_dir)
```

### Comparing `copasi-petab-importer-1.0.2/copasi_petab_importer.egg-info/SOURCES.txt` & `copasi-petab-importer-1.0.3/copasi_petab_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.2/setup.py` & `copasi-petab-importer-1.0.3/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
-import versioneer
-
-ENTRY_POINTS = {
-    'console_scripts': [
-        'copasi_petab_import=copasi_petab_importer.convert_petab:main',
-        'copasi_petab_gui=copasi_petab_importer.PEtab:petab_gui',
-    ]
-}
-
-setup(
-    name='copasi-petab-importer',
-    packages=['copasi_petab_importer'],
-    package_dir={'copasi_petab_importer': 'copasi_petab_importer'},
-    url='https://github.com/copasi/python-petab-importer',
-    license='Artistic-2.0',
-    author='Frank T. Bergmann',
-    author_email='frank.bergmann@bioquant.uni-heidelberg.de',
-    description='COPASI PEtab Importer',
-    entry_points=ENTRY_POINTS,
-    install_requires=['numpy', 'pandas', 'python-copasi', 'python-libsbml', 'pyyaml'],
-    extras_require={'gui': ['PyQt5']},
-    package_data={'copasi_petab_importer': ['*.ui']},
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
-)
+from setuptools import setup
+import versioneer
+
+ENTRY_POINTS = {
+    'console_scripts': [
+        'copasi_petab_import=copasi_petab_importer.convert_petab:main',
+        'copasi_petab_gui=copasi_petab_importer.PEtab:petab_gui',
+    ]
+}
+
+setup(
+    name='copasi-petab-importer',
+    packages=['copasi_petab_importer'],
+    package_dir={'copasi_petab_importer': 'copasi_petab_importer'},
+    url='https://github.com/copasi/python-petab-importer',
+    license='Artistic-2.0',
+    author='Frank T. Bergmann',
+    author_email='frank.bergmann@bioquant.uni-heidelberg.de',
+    description='COPASI PEtab Importer',
+    entry_points=ENTRY_POINTS,
+    install_requires=['numpy', 'pandas', 'python-copasi', 'python-libsbml', 'pyyaml'],
+    extras_require={'gui': ['PyQt5']},
+    package_data={'copasi_petab_importer': ['*.ui']},
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
+)
```

### Comparing `copasi-petab-importer-1.0.2/versioneer.py` & `copasi-petab-importer-1.0.3/versioneer.py`

 * *Files identical despite different names*

