# Comparing `tmp/IMGTgeneDL-0.5.1.tar.gz` & `tmp/IMGTgeneDL-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMGTgeneDL-0.5.1.tar", last modified: Sun Apr 16 23:33:40 2023, max compression
+gzip compressed data, was "IMGTgeneDL-0.5.2.tar", last modified: Tue Apr 18 18:30:50 2023, max compression
```

## Comparing `IMGTgeneDL-0.5.1.tar` & `IMGTgeneDL-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/LICENSE
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12125 2023-04-16 23:07:58.000000 IMGTgeneDL-0.5.1/README.md
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/pyproject.toml
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      846 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/setup.cfg
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.117405 IMGTgeneDL-0.5.1/src/
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/src/IMGTgeneDL/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    36683 2023-04-16 23:27:06.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/IMGTgeneDL.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      524 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/c-region-variant-configs.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      527 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/species.tsv
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      399 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/SOURCES.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/dependency_links.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       58 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/entry_points.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       36 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/requires.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       11 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/top_level.txt
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 18:30:50.835914 IMGTgeneDL-0.5.2/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.2/LICENSE
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-18 18:30:50.835914 IMGTgeneDL-0.5.2/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12125 2023-04-18 18:26:48.000000 IMGTgeneDL-0.5.2/README.md
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.2/pyproject.toml
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      846 2023-04-18 18:30:50.835914 IMGTgeneDL-0.5.2/setup.cfg
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 18:30:50.723914 IMGTgeneDL-0.5.2/src/
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 18:30:50.755914 IMGTgeneDL-0.5.2/src/IMGTgeneDL/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    36751 2023-04-18 18:26:48.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL/IMGTgeneDL.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      524 2023-04-18 03:49:08.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL/c-region-variant-configs.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      527 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL/species.tsv
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-18 18:30:50.831914 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      399 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/SOURCES.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/dependency_links.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       58 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/entry_points.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       36 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/requires.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       11 2023-04-18 18:30:50.000000 IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/top_level.txt
```

### Comparing `IMGTgeneDL-0.5.1/LICENSE` & `IMGTgeneDL-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.1/PKG-INFO` & `IMGTgeneDL-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: IMGTgeneDL
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python script to download data from IMGT/GENE-DB
 Home-page: https://github.com/JamieHeather/IMGTgeneDL
 Author: Jamie Heather
 Author-email: jheather@mgh.harvard.edu
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IMGTgeneDL
 
-## 0.5.1
+## 0.5.2
 ##### Jamie Heather | CCR @ MGH | 2023
 
 This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
```

### Comparing `IMGTgeneDL-0.5.1/README.md` & `IMGTgeneDL-0.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # IMGTgeneDL
 
-## 0.5.1
+## 0.5.2
 ##### Jamie Heather | CCR @ MGH | 2023
 
 This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
```

### Comparing `IMGTgeneDL-0.5.1/setup.cfg` & `IMGTgeneDL-0.5.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = IMGTgeneDL
-version = 0.5.1
+version = 0.5.2
 author = Jamie Heather
 author_email = jheather@mgh.harvard.edu
 description = Python script to download data from IMGT/GENE-DB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JamieHeather/IMGTgeneDL
 project_urls = 
-Bug Tracker = https://github.com/JamieHeather/IMGTgeneDL/issues
+bug tracker = https://github.com/JamieHeather/IMGTgeneDL/issues
 classifiers = 
-Programming Language = : Python :: 3
-License = : OSI Approved :: MIT License
-Operating System = : OS Independent
+programming language = : Python :: 3
+license = : OSI Approved :: MIT License
+operating system = : OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires =
```

### Comparing `IMGTgeneDL-0.5.1/src/IMGTgeneDL/IMGTgeneDL.py` & `IMGTgeneDL-0.5.2/src/IMGTgeneDL/IMGTgeneDL.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Ensure correct importlib-resources function imported
 if sys.version_info < (3, 9):
     import importlib_resources                              # PyPI
 else:
     import importlib.resources as importlib_resources       # importlib.resources
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
 warnings.filterwarnings('ignore', message='Unverified HTTPS request')
 
 
 def args():
@@ -325,25 +325,25 @@
 
                         except:
                             warnings.warn("Failed to download individual exon IMGT/GENE-DB raw data (for " +
                                           '/'.join([full_gene, search_species, gene_type]) +
                                           ". Check connection/input options")
 
                     assembled_fasta = concat_constants(exon_fasta, gene_type)
-                    out_fasta += assembled_fasta
+                    out_fasta += assembled_fasta.replace('\r', '') + '\n'
 
                 # Otherwise try to download the full gene region
                 else:
                     dl_url = imgt_url(full_gene, search_species, gene_type)
 
                     try:
                         # ... and then download that, pulling out the FASTA sequence from amidst the HTML
                         reads = page_scrape(dl_url)
                         if reads:
-                            out_fasta += reads
+                            out_fasta += reads.replace('\r', '') + '\n'
 
                     except:
                         warnings.warn("Failed to download specific IMGT/GENE-DB raw data for " +
                                       '/'.join([search_species, full_gene, gene_type]) +
                                       ". Check connection/input options. \nURL = " + dl_url)
 
             # TODO filter out TRAV/DV duplicates (which get downloaded both from TRA and TRD loci calls) at this stage?
@@ -751,15 +751,15 @@
                 suffix = exon_arrangement
                 for substr in ['EX1', 'EX2', 'EX3', 'EX4', '+', 'UTR']:
                     suffix = suffix.replace(substr, '')
                 suffix = '_' + suffix
 
             out_header = '|'.join([accessions, g + suffix, header_bits[g]['EX1'][2], functionality, exon_arrangement,
                                    '?', len_str + ' nt', '?', ' ', ' ', ' ', ' ', len_str + '+0=' + len_str, ' ', ' '])
-            out_fasta += fastafy(out_header, gene_seq)
+            out_fasta += fastafy(out_header, gene_seq.replace('\r', ''))
 
     return out_fasta
 
 
 base_url = "https://www.imgt.org/download/GENE-DB/"
 
 # The contents of the IMGT fasta headers that users might wish to filter on
```

### Comparing `IMGTgeneDL-0.5.1/src/IMGTgeneDL/c-region-variant-configs.tsv` & `IMGTgeneDL-0.5.2/src/IMGTgeneDL/c-region-variant-configs.tsv`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.1/src/IMGTgeneDL/species.tsv` & `IMGTgeneDL-0.5.2/src/IMGTgeneDL/species.tsv`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/PKG-INFO` & `IMGTgeneDL-0.5.2/src/IMGTgeneDL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: IMGTgeneDL
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python script to download data from IMGT/GENE-DB
 Home-page: https://github.com/JamieHeather/IMGTgeneDL
 Author: Jamie Heather
 Author-email: jheather@mgh.harvard.edu
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IMGTgeneDL
 
-## 0.5.1
+## 0.5.2
 ##### Jamie Heather | CCR @ MGH | 2023
 
 This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
```

