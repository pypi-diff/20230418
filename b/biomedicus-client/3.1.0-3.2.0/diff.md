# Comparing `tmp/biomedicus_client-3.1.0.tar.gz` & `tmp/biomedicus_client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedicus_client-3.1.0.tar", last modified: Thu Mar 16 19:53:39 2023, max compression
+gzip compressed data, was "biomedicus_client-3.2.0.tar", last modified: Mon Apr 17 22:41:04 2023, max compression
```

## Comparing `biomedicus_client-3.1.0.tar` & `biomedicus_client-3.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:39.048668 biomedicus_client-3.1.0/
--rw-r--r--   0 knol0061   (501) staff       (20)    11358 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/LICENSE.txt
--rw-r--r--   0 knol0061   (501) staff       (20)       46 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/MANIFEST.in
--rw-r--r--   0 knol0061   (501) staff       (20)    16107 2023-03-16 19:53:39.047545 biomedicus_client-3.1.0/PKG-INFO
--rw-r--r--   0 knol0061   (501) staff       (20)     1495 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/README.md
--rw-r--r--   0 knol0061   (501) staff       (20)     2096 2023-03-16 19:52:16.000000 biomedicus_client-3.1.0/pyproject.toml
--rw-r--r--   0 knol0061   (501) staff       (20)       38 2023-03-16 19:53:39.048882 biomedicus_client-3.1.0/setup.cfg
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:38.917793 biomedicus_client-3.1.0/src/
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:38.936613 biomedicus_client-3.1.0/src/biomedicus_client/
--rw-r--r--   0 knol0061   (501) staff       (20)      809 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)      691 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/__main__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1384 2023-02-16 16:51:26.000000 biomedicus_client-3.1.0/src/biomedicus_client/cli.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:38.978755 biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/
--rw-r--r--   0 knol0061   (501) staff       (20)      870 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1502 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/command.py
--rw-r--r--   0 knol0061   (501) staff       (20)     2077 2023-02-16 16:51:26.000000 biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/config_writing.py
--rw-r--r--   0 knol0061   (501) staff       (20)     1078 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/parser.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:39.045983 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/
--rw-r--r--   0 knol0061   (501) staff       (20)      717 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/__init__.py
--rw-r--r--   0 knol0061   (501) staff       (20)     3305 2023-02-01 19:42:09.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/_run.py
--rw-r--r--   0 knol0061   (501) staff       (20)      704 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     5777 2023-02-07 16:20:36.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/default_pipeline.py
--rw-r--r--   0 knol0061   (501) staff       (20)     4492 2023-02-07 16:20:36.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/rtf_to_text.py
--rw-r--r--   0 knol0061   (501) staff       (20)      242 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/rtf_to_text_pipeline.yml
--rw-r--r--   0 knol0061   (501) staff       (20)      827 2023-01-13 02:07:31.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/scaleout_pipeline_config.yml
--rw-r--r--   0 knol0061   (501) staff       (20)     4006 2023-02-07 16:20:36.000000 biomedicus_client-3.1.0/src/biomedicus_client/pipeline/sources.py
--rw-r--r--   0 knol0061   (501) staff       (20)      160 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client/version.py
-drwxr-xr-x   0 knol0061   (501) staff       (20)        0 2023-03-16 19:53:38.943353 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/
--rw-r--r--   0 knol0061   (501) staff       (20)    16107 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/PKG-INFO
--rw-r--r--   0 knol0061   (501) staff       (20)     1029 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/SOURCES.txt
--rw-r--r--   0 knol0061   (501) staff       (20)        1 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/dependency_links.txt
--rw-r--r--   0 knol0061   (501) staff       (20)       56 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/entry_points.txt
--rw-r--r--   0 knol0061   (501) staff       (20)       75 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/requires.txt
--rw-r--r--   0 knol0061   (501) staff       (20)       18 2023-03-16 19:53:38.000000 biomedicus_client-3.1.0/src/biomedicus_client.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/
+-rw-r--r--   0 ben       (1000) ben       (1000)    11358 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/LICENSE.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       46 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1495 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/README.md
+-rw-r--r--   0 ben       (1000) ben       (1000)     2140 2023-04-17 22:38:27.000000 biomedicus_client-3.2.0/pyproject.toml
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/setup.cfg
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/
+-rw-r--r--   0 ben       (1000) ben       (1000)      809 2023-04-17 15:52:14.000000 biomedicus_client-3.2.0/src/biomedicus_client/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      691 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/__main__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1328 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/
+-rw-r--r--   0 ben       (1000) ben       (1000)      870 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1502 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/command.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     2077 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/config_writing.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1078 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/parser.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/
+-rw-r--r--   0 ben       (1000) ben       (1000)      717 2023-03-13 16:38:29.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3335 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/_run.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      636 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     5789 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/default_pipeline.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     4506 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      313 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text_pipeline.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)      619 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/scaleout_pipeline_config.yml
+-rw-r--r--   0 ben       (1000) ben       (1000)     4026 2023-04-17 19:25:13.000000 biomedicus_client-3.2.0/src/biomedicus_client/pipeline/sources.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      160 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client/version.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-17 22:41:04.813477 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)    16086 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1029 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       56 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      133 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       18 2023-04-17 22:41:04.000000 biomedicus_client-3.2.0/src/biomedicus_client.egg-info/top_level.txt
```

### Comparing `biomedicus_client-3.1.0/LICENSE.txt` & `biomedicus_client-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/PKG-INFO` & `biomedicus_client-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedicus_client
-Version: 3.1.0
+Version: 3.2.0
 Summary: A biomedical and clinical natural language processing engine.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -228,15 +228,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.txt
 
 # BioMedICUS Client
 
 The BioMedical Information Collection and Understanding System (BioMedICUS) is a system for large-scale text analysis and processing of biomedical and clinical reports. The system is being developed by the Natural Language Processing and Information Extraction Program at the University of Minnesota Institute for Health Informatics.
 
 This is a collaborative project that aims to serve biomedical and clinical researchers, allowing for customization with different texts.
```

### Comparing `biomedicus_client-3.1.0/README.md` & `biomedicus_client-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/pyproject.toml` & `biomedicus_client-3.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -32,34 +32,33 @@
     'Programming Language :: Python :: Implementation :: CPython',
     'Topic :: Scientific/Engineering :: Information Analysis',
     'Topic :: Scientific/Engineering :: Medical Science Apps.',
     'Topic :: Text Processing :: General',
     'Topic :: Text Processing :: Linguistic'
 ]
 dependencies = [
-    "mtap==1.1.0",
+    "mtap==1.2.1",
+    "grpcio==1.53.0",
+    "grpcio-health-checking==1.53.0",
+    "grpcio-status==1.53.0",
+    "pyyaml==6.0",
     "tqdm==4.65.0",
     "importlib_resources==5.12.0",
 ]
 dynamic = ["version"]
 
-[project.optional-dependencies]
-test = [
-    "pytest==7.2.2"
-]
-
 [project.scripts]
 b9client = "biomedicus_client.cli:main"
 
 [project.urls]
 homepage = "https://nlpie.github.io/biomedicus"
 documentation = "https://nlpie.github.io/biomedicus/guides"
 repository = "https://github.com/nlpie/biomedicus3.git"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["biomedicus_client*"]
 
 [tool.setuptools_scm]
 write_to = "biomedicus_client/src/biomedicus_client/version.py"
-fallback_version = "3.1.0"
+fallback_version = "3.2.0"
 root = ".."
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/__init__.py` & `biomedicus_client-3.2.0/src/biomedicus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/__main__.py` & `biomedicus_client-3.2.0/src/biomedicus_client/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/cli.py` & `biomedicus_client-3.2.0/src/biomedicus_client/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 import logging
 
 from biomedicus_client.cli_tools import create_parser, WriteConfigsCommand
 from biomedicus_client.pipeline import RunCommand, default_pipeline, rtf_to_text
 
 CLIENT_CONFIGS = {
     'pipeline': default_pipeline.default_pipeline_config,
-    'run': default_pipeline.default_pipeline_config,
-    'scaleout-pipeline': default_pipeline.scaleout_pipeline_config,
-    'rtf-to-text-pipeline': rtf_to_text.default_rtf_to_text_pipeline_config
+    'scaleout_pipeline': default_pipeline.scaleout_pipeline_config,
+    'rtf_only_pipeline': rtf_to_text.default_rtf_to_text_pipeline_config
 }
 
 
 def main(args=None):
     parser = create_parser(
         WriteConfigsCommand(CLIENT_CONFIGS),
         RunCommand(),
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/__init__.py` & `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/command.py` & `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/command.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/config_writing.py` & `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/config_writing.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/cli_tools/parser.py` & `biomedicus_client-3.2.0/src/biomedicus_client/cli_tools/parser.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/__init__.py` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/_run.py` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Support for running the default pipeline by default and optionally arbitrary pipelines."""
 
 from argparse import ArgumentParser
 from typing import List
 
-from mtap.processing import FilesInDirectoryProcessingSource
+from mtap import events_client
+from mtap.pipeline import FilesInDirectoryProcessingSource
 
 from biomedicus_client.cli_tools import Command
 from biomedicus_client.pipeline import default_pipeline
 from biomedicus_client.pipeline.sources import WatcherSource, RtfHandler, rtf_source, TxtHandler
 
 
 class RunCommand(Command):
@@ -44,17 +45,17 @@
                             help="Watches the directory for new files to process.")
         parser.add_argument('--no-times', default=False, action='store_true',
                             help="Suppress printing pipeline run times after completion.")
         parser.add_argument('--log-level', default='INFO',
                             help="The log level to use.")
 
     def command_fn(self, conf):
-        with default_pipeline.from_args(conf) as pipeline:
-            input_directory = conf.input_directory
-            client = pipeline.events_client
+        pipeline = default_pipeline.from_args(conf)
+        input_directory = conf.input_directory
+        with events_client(pipeline.events_address) as client:
             if conf.rtf:
                 extension_glob = conf.extension_glob or "**/*.rtf"
                 if conf.watch:
                     source = WatcherSource(RtfHandler(input_directory, extension_glob, client))
                 else:
                     source = rtf_source(input_directory, extension_glob, client)
                 params = {'document_name': 'plaintext'}
@@ -63,10 +64,10 @@
                 if conf.watch:
                     source = WatcherSource(TxtHandler(input_directory, extension_glob, client))
                 else:
                     source = FilesInDirectoryProcessingSource(client,
                                                               input_directory,
                                                               extension_glob=extension_glob)
                 params = None
-            pipeline.run_multithread(source, params=params, log_level=conf.log_level)
-            if not conf.no_times:
-                pipeline.print_times()
+            result = pipeline.run_multithread(source, params=params, log_level=conf.log_level)
+        if not conf.no_times:
+            result.print()
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/biomedicus_default_pipeline.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 name: biomedicus-default-pipeline
 events_address: localhost:50100
 mp_config:
-  max_failures: 0
   show_progress: True
   workers: 4
   read_ahead: 4
   close_events: True
   mp_start_method: spawn
+error_handlers:
+  - name: simple
+  - name: termination
+    params:
+      max_failures: 0
 components:
   - name: biomedicus-sentences
     address: localhost:50300
   - name: biomedicus-tnt-tagger
     address: localhost:50400
   - name: biomedicus-acronyms
     address: localhost:50500
   - name: biomedicus-concepts
     address: localhost:50600
-  - name: biomedicus-negex-triggers
+  - name: biomedicus-negex
     address: localhost:50700
-  - name: biomedicus-selective-dependencies
-    address: localhost:50800
-  - name: biomedicus-deepen
-    address: localhost:50900
   - name: biomedicus-section-headers
     address: localhost:51000
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/default_pipeline.py` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/default_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Optional, Union
 
 from importlib_resources import files
 from mtap import Pipeline, LocalProcessor, RemoteProcessor
-from mtap.serialization import get_serializer, SerializationProcessor
+from mtap.serialization import SerializerRegistry, SerializationProcessor
 
 __all__ = ['default_pipeline_config', 'scaleout_pipeline_config', 'create', 'from_args', 'argument_parser']
 
 default_pipeline_config = files('biomedicus_client.pipeline').joinpath('biomedicus_default_pipeline.yml')
 scaleout_pipeline_config = files('biomedicus_client.pipeline').joinpath('scaleout_pipeline_config.yml')
 
 
@@ -62,15 +62,15 @@
     pipeline = Pipeline.from_yaml_file(config)
 
     if events_addresses is not None:
         pipeline.events_address = events_addresses
 
     serializer = None if serializer == 'None' else serializer
     if serializer is not None:
-        serialization_proc = SerializationProcessor(get_serializer(serializer),
+        serialization_proc = SerializationProcessor(SerializerRegistry.get(serializer),
                                                     output_directory,
                                                     include_label_text=include_label_text)
         ser_comp = LocalProcessor(serialization_proc, component_id='serializer')
         pipeline.append(ser_comp)
 
     if rtf:
         rtf_processor = RemoteProcessor(processor_name='biomedicus-rtf',
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/rtf_to_text.py` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/rtf_to_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from argparse import ArgumentParser, Namespace
 from os import PathLike
 
 from importlib_resources import files
 from pathlib import Path
 from typing import Union, Optional, List
 
-from mtap import Pipeline, LocalProcessor, EventProcessor, processor
+from mtap import Pipeline, LocalProcessor, EventProcessor, processor, events_client
 
 from biomedicus_client.cli_tools import Command
 from biomedicus_client.pipeline.sources import rtf_source
 
 __all__ = ['default_rtf_to_text_pipeline_config', 'create', 'from_args', 'argument_parser', 'RunRtfToTextCommand']
 
 default_rtf_to_text_pipeline_config = files('biomedicus_client.pipeline').joinpath('rtf_to_text_pipeline.yml')
@@ -111,16 +111,16 @@
         parser.add_argument('input_directory', help="The input directory of text files to process.")
         parser.add_argument('--extension-glob', default="*.rtf",
                             help="The extension glob used to find files to process.")
         parser.add_argument('--log-level', default='INFO',
                             help="The log level for the pipeline runners.")
 
     def command_fn(self, conf):
-        with from_args(conf) as pipeline:
-            input_directory = Path(conf.input_directory)
+        pipeline = from_args(conf)
+        input_directory = Path(conf.input_directory)
 
-            source = rtf_source(input_directory, conf.extension_glob,
-                                pipeline.events_client)
+        with events_client(pipeline.events_address) as client:
+            source = rtf_source(input_directory, conf.extension_glob, client)
             total = sum(1 for _ in input_directory.rglob(conf.extension_glob))
 
-            pipeline.run_multithread(source, total=total, log_level=conf.log_level)
-            pipeline.print_times()
+            times = pipeline.run_multithread(source, total=total, log_level=conf.log_level)
+        times.print()
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client/pipeline/sources.py` & `biomedicus_client-3.2.0/src/biomedicus_client/pipeline/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 #  limitations under the License.
 """Input sources for running pipelines."""
 
 import fnmatch
 import time
 from pathlib import Path
 
-from mtap import Event, EventsClient
-from mtap.processing import ProcessingSource
+from mtap import Event
+from mtap.pipeline import ProcessingSource
+from mtap.types import EventsClient
 from watchdog.events import FileSystemEventHandler, FileSystemEvent
 
 
 def rtf_source(input_directory: Path, extension_glob: str, events_client: EventsClient):
     input_directory = Path(input_directory)
     for path in input_directory.rglob(extension_glob):
         with path.open('rb', errors=None) as f:
@@ -82,15 +83,15 @@
                     self.consume(doc)
 
 
 class WatcherSource(ProcessingSource):
     def __init__(self, handler):
         self.handler = handler
 
-    def provide(self, consume):
+    def produce(self, consume):
         from watchdog.observers import Observer
 
         self.handler.consume = consume
 
         observer = Observer()
         observer.schedule(self.handler, str(self.handler.input_directory), recursive=True)
         print('Observing directory: ' + str(self.handler.input_directory))
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client.egg-info/PKG-INFO` & `biomedicus_client-3.2.0/src/biomedicus_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedicus-client
-Version: 3.1.0
+Version: 3.2.0
 Summary: A biomedical and clinical natural language processing engine.
 Author-email: University of Minnesota NLP/IE Group <nlp-ie@umn.edu>, Ben Knoll <benknoll@umn.edu>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -228,15 +228,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.txt
 
 # BioMedICUS Client
 
 The BioMedical Information Collection and Understanding System (BioMedICUS) is a system for large-scale text analysis and processing of biomedical and clinical reports. The system is being developed by the Natural Language Processing and Information Extraction Program at the University of Minnesota Institute for Health Informatics.
 
 This is a collaborative project that aims to serve biomedical and clinical researchers, allowing for customization with different texts.
```

### Comparing `biomedicus_client-3.1.0/src/biomedicus_client.egg-info/SOURCES.txt` & `biomedicus_client-3.2.0/src/biomedicus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

