# Comparing `tmp/analysis-runner-2.40.7.tar.gz` & `tmp/analysis-runner-2.40.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-runner-2.40.7.tar", last modified: Thu Apr  6 07:40:25 2023, max compression
+gzip compressed data, was "analysis-runner-2.40.8.tar", last modified: Tue Apr 18 08:15:49 2023, max compression
```

## Comparing `analysis-runner-2.40.7.tar` & `analysis-runner-2.40.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:40:25.099449 analysis-runner-2.40.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-06 07:40:25.099449 analysis-runner-2.40.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:40:25.095449 analysis-runner-2.40.7/analysis_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cli_analysisrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cli_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/analysis_runner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:40:25.095449 analysis-runner-2.40.7/analysis_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 07:40:25.000000 analysis-runner-2.40.7/analysis_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 07:40:25.099449 analysis-runner-2.40.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:40:25.095449 analysis-runner-2.40.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-06 07:40:23.000000 analysis-runner-2.40.7/test/test_analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/analysis_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_analysisrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/analysis_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/test/test_analysis_runner.py
```

### Comparing `analysis-runner-2.40.7/LICENSE` & `analysis-runner-2.40.8/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/PKG-INFO` & `analysis-runner-2.40.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.7
+Version: 2.40.8
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.7/README.md` & `analysis-runner-2.40.8/README.md`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cli.py` & `analysis-runner-2.40.8/analysis_runner/cli.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cli_analysisrunner.py` & `analysis-runner-2.40.8/analysis_runner/cli_analysisrunner.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cli_config.py` & `analysis-runner-2.40.8/analysis_runner/cli_config.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cli_cromwell.py` & `analysis-runner-2.40.8/analysis_runner/cli_cromwell.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/constants.py` & `analysis-runner-2.40.8/analysis_runner/constants.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cromwell.py` & `analysis-runner-2.40.8/analysis_runner/cromwell.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/cromwell_model.py` & `analysis-runner-2.40.8/analysis_runner/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/dataproc.py` & `analysis-runner-2.40.8/analysis_runner/dataproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     get_git_commit_ref_of_current_repository,
     get_repo_name_from_remote,
     prepare_git_job,
     get_relative_path_from_git_root,
 )
 
 
-HAIL_VERSION = '0.2.110'
+HAIL_VERSION = '0.2.105'
 DATAPROC_IMAGE = (
     f'australia-southeast1-docker.pkg.dev/analysis-runner/images/'
     f'dataproc:hail-{HAIL_VERSION}'
 )
 # Wheel built from https://github.com/populationgenomics/hail
 # The difference from the official build is the version of ElasticSearch:
 # We use 8.x.x, and Hail is built for 7.x.x by default.
```

### Comparing `analysis-runner-2.40.7/analysis_runner/git.py` & `analysis-runner-2.40.8/analysis_runner/git.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner/util.py` & `analysis-runner-2.40.8/analysis_runner/util.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/analysis_runner.egg-info/PKG-INFO` & `analysis-runner-2.40.8/analysis_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.7
+Version: 2.40.8
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.7/analysis_runner.egg-info/SOURCES.txt` & `analysis-runner-2.40.8/analysis_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.7/setup.py` & `analysis-runner-2.40.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='2.40.7',
+    version='2.40.8',
     description='Analysis runner to help make analysis results reproducible',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/{PKG}',
     license='MIT',
     packages=['analysis_runner'],
     include_package_data=True,
```

### Comparing `analysis-runner-2.40.7/test/test_analysis_runner.py` & `analysis-runner-2.40.8/test/test_analysis_runner.py`

 * *Files identical despite different names*

