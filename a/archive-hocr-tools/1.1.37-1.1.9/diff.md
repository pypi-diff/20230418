# Comparing `tmp/archive-hocr-tools-1.1.37.tar.gz` & `tmp/archive-hocr-tools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archive-hocr-tools-1.1.37.tar", last modified: Mon Apr 17 22:15:35 2023, max compression
+gzip compressed data, was "/home/merlijn/archive/archive-hocr-tools/dist/tmpulyt8lyw/archive-hocr-tools-1.1.9.tar", last modified: Mon Oct  4 21:06:27 2021, max compression
```

## Comparing `archive-hocr-tools-1.1.37.tar` & `archive-hocr-tools-1.1.9.tar`

### file list

```diff
@@ -1,55 +1,34 @@
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.604009 archive-hocr-tools-1.1.37/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.37/COPYING
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.37/LICENSE.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      733 2023-04-17 22:15:35.604009 archive-hocr-tools-1.1.37/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      657 2023-04-17 22:14:32.000000 archive-hocr-tools-1.1.37/README
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      657 2023-04-17 22:14:32.000000 archive-hocr-tools-1.1.37/README.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.597342 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      733 2023-04-17 22:15:35.000000 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      946 2023-04-17 22:15:35.000000 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2023-04-17 22:15:35.000000 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      126 2023-04-17 22:15:35.000000 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/requires.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2023-04-17 22:15:35.000000 archive-hocr-tools-1.1.37/archive_hocr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.600676 archive-hocr-tools-1.1.37/bin/
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    23974 2021-10-11 22:41:03.000000 archive-hocr-tools-1.1.37/bin/abbyy-to-hocr
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1305 2021-02-03 13:57:49.000000 archive-hocr-tools-1.1.37/bin/fts-text-annotate
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1544 2021-10-15 18:16:54.000000 archive-hocr-tools-1.1.37/bin/fts-text-match
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3018 2023-03-03 00:51:23.000000 archive-hocr-tools-1.1.37/bin/hocr-combine-stream
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    10480 2023-04-17 22:14:32.000000 archive-hocr-tools-1.1.37/bin/hocr-confidence-filter
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1565 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.37/bin/hocr-extract-page
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1424 2023-01-09 20:19:20.000000 archive-hocr-tools-1.1.37/bin/hocr-flatten-pages
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1831 2022-03-16 09:42:59.000000 archive-hocr-tools-1.1.37/bin/hocr-fold-chars
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2409 2022-08-12 00:45:40.000000 archive-hocr-tools-1.1.37/bin/hocr-lookup-check
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      551 2021-01-07 22:43:12.000000 archive-hocr-tools-1.1.37/bin/hocr-lookup-create
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      888 2021-01-08 12:38:34.000000 archive-hocr-tools-1.1.37/bin/hocr-lookup-reconstruct
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1182 2022-08-12 00:45:40.000000 archive-hocr-tools-1.1.37/bin/hocr-split-pages
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      594 2021-10-15 21:39:26.000000 archive-hocr-tools-1.1.37/bin/hocr-text
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      826 2021-01-08 13:40:53.000000 archive-hocr-tools-1.1.37/bin/hocr-text-paragraphs
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    27998 2023-04-17 22:14:32.000000 archive-hocr-tools-1.1.37/bin/hocr-to-epub
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    13436 2022-09-05 10:24:23.000000 archive-hocr-tools-1.1.37/bin/pdf-to-hocr
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      686 2021-02-02 19:43:59.000000 archive-hocr-tools-1.1.37/conftest.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.600676 archive-hocr-tools-1.1.37/docs/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      638 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.37/docs/Makefile
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.600676 archive-hocr-tools-1.1.37/docs/source/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1961 2022-04-16 05:05:04.000000 archive-hocr-tools-1.1.37/docs/source/conf.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4126 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.37/docs/source/index.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.37/docs/source/parse.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       83 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.37/docs/source/searching.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      100 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.37/docs/source/text.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.604009 archive-hocr-tools-1.1.37/hocr/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2021-06-28 13:26:24.000000 archive-hocr-tools-1.1.37/hocr/__init__.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.604009 archive-hocr-tools-1.1.37/hocr/data/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     6951 2023-01-30 22:06:33.000000 archive-hocr-tools-1.1.37/hocr/data/abbyy-lang-map.csv
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10570 2022-08-12 09:48:56.000000 archive-hocr-tools-1.1.37/hocr/fts.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    11425 2023-04-17 22:14:29.000000 archive-hocr-tools-1.1.37/hocr/parse.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3908 2021-06-28 13:54:43.000000 archive-hocr-tools-1.1.37/hocr/searching.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4886 2022-08-12 00:45:40.000000 archive-hocr-tools-1.1.37/hocr/text.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2915 2022-11-19 12:19:24.000000 archive-hocr-tools-1.1.37/hocr/util.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       23 2023-04-17 22:14:33.000000 archive-hocr-tools-1.1.37/hocr/version.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       61 2021-10-04 20:43:57.000000 archive-hocr-tools-1.1.37/pyproject.toml
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       12 2023-04-17 22:14:29.000000 archive-hocr-tools-1.1.37/requirements.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2023-04-17 22:15:35.607342 archive-hocr-tools-1.1.37/setup.cfg
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1792 2023-03-03 01:01:57.000000 archive-hocr-tools-1.1.37/setup.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-04-17 22:15:35.604009 archive-hocr-tools-1.1.37/tests/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    44515 2021-02-02 22:09:21.000000 archive-hocr-tools-1.1.37/tests/hocr_res.json
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1472 2021-02-02 22:12:31.000000 archive-hocr-tools-1.1.37/tests/test_hocr.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      690 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      609 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/requires.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/bin/
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    23972 2021-08-06 18:07:47.000000 archive-hocr-tools-1.1.9/bin/abbyy-to-hocr
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1305 2021-02-03 13:57:49.000000 archive-hocr-tools-1.1.9/bin/fts-text-annotate
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1254 2021-06-28 13:26:24.000000 archive-hocr-tools-1.1.9/bin/fts-text-match
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3037 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-combine-stream
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1565 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-extract-page
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1831 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-fold-chars
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2420 2021-01-08 15:17:51.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-check
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      551 2021-01-07 22:43:12.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-create
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      888 2021-01-08 12:38:34.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-reconstruct
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2562 2021-10-04 20:51:43.000000 archive-hocr-tools-1.1.9/bin/hocr-text
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      826 2021-01-08 13:40:53.000000 archive-hocr-tools-1.1.9/bin/hocr-text-paragraphs
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/hocr/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2021-06-28 13:26:24.000000 archive-hocr-tools-1.1.9/hocr/__init__.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7765 2021-06-28 13:54:43.000000 archive-hocr-tools-1.1.9/hocr/fts.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8288 2021-10-04 20:51:43.000000 archive-hocr-tools-1.1.9/hocr/parse.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3908 2021-06-28 13:54:43.000000 archive-hocr-tools-1.1.9/hocr/searching.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4946 2021-06-28 13:12:11.000000 archive-hocr-tools-1.1.9/hocr/text.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2211 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/hocr/util.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       22 2021-10-04 21:05:07.000000 archive-hocr-tools-1.1.9/hocr/version.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/COPYING
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/LICENSE.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      483 2020-10-31 10:07:13.000000 archive-hocr-tools-1.1.9/README
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       61 2021-10-04 20:43:57.000000 archive-hocr-tools-1.1.9/pyproject.toml
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/setup.cfg
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1451 2021-10-04 21:05:30.000000 archive-hocr-tools-1.1.9/setup.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      690 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `archive-hocr-tools-1.1.37/COPYING` & `archive-hocr-tools-1.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/LICENSE.txt` & `archive-hocr-tools-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/bin/abbyy-to-hocr` & `archive-hocr-tools-1.1.9/bin/abbyy-to-hocr`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # X Parse exact abbyy software version, other attributes, move those to hOCR files
 # / Test with different abbyy xml versions
 # X Test with unicode languages - also for writing direction and such -> maybe charParams.wordLeftMost can be used (if the first char is not wordLeftMost...)
 # X use <line fs="8.5" ...> (etc) for x_fsize for words?
 # X Add scan_res (from image or item metadata? meh)
 # X word confidence wordFromDictionary (?) + char confs?, 'suspicious' attribute
 # - Add lots of (strict) assertions to prevent silent bugs (unknown areas/types, etc)
-# - ocr_page image property - point to the some url for convenience (where do we
+# - ocr_page image property - point to the some url for convience (where do we
 #   get it from?)
 
 # Tested versions:
 #
 # - 'ABBYY FineReader 11.0 (Extended OCR)'
 # - 'ABBYY FineReader 11.0'
 # - 'ABBYY FineReader 9.0'
```

### Comparing `archive-hocr-tools-1.1.37/bin/fts-text-annotate` & `archive-hocr-tools-1.1.9/bin/fts-text-annotate`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/bin/fts-text-match` & `archive-hocr-tools-1.1.9/bin/hocr-extract-page`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
 
-import json
+from lxml import etree
 
-from hocr.searching import hocr_load_lookup_table
-from hocr.util import open_if_required
-from hocr.fts import find_matches
+from hocr.searching import hocr_load_lookup_table, hocr_lookup_page_by_dat
+from hocr.parse import hocr_page_iterator
+from hocr.util import open_if_required, get_header_footer
 
+def process_file(filepath, pageno, tablepath):
+    fd = open_if_required(filepath)
+    top, bottom = get_header_footer(fd)
 
-def process_file(hocrfile, textfile, tablepath, es_workaround):
-    lookup_table = hocr_load_lookup_table(tablepath)
+    sys.stdout.buffer.write(top)
 
-    hocrfp = open_if_required(hocrfile)
-    textfp = open_if_required(textfile)
-    text = textfp.read().decode('utf-8')
+    if tablepath:
+        lookup_table = hocr_load_lookup_table(tablepath)
+        fp = open_if_required(filepath)
 
-    for word_results in find_matches(lookup_table, hocrfp, text,
-            es_whitespace_fixup_required=es_workaround):
-        json.dump(word_results, sys.stdout)
-        sys.stdout.write('\n')
+        dat = lookup_table[pageno]
+        page = hocr_lookup_page_by_dat(fp, dat)
+    else:
+        for idx, page in enumerate(hocr_page_iterator(fd)):
+            if idx == pageno:
+                break
+
+    s = etree.tostring(page, pretty_print=True, method='xml',
+                       encoding='utf-8').decode('utf-8')
+
+    s = ' ' + s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
+    s = s.encode('utf-8')
+    sys.stdout.buffer.write(s)
+
+    sys.stdout.buffer.write(bottom)
 
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='hOCR lookup table '
-                                                 'paragraph-level validator')
-    parser.add_argument('--hocr', help='hOCR Filename to read',
+    parser = argparse.ArgumentParser(description='hOCR single page extractor')
+    parser.add_argument('-f', '--infile', help='Filename to read',
                         type=str, default=None)
-    parser.add_argument('--annotated-text', help='Annotated fulltext filename '
-                                                 'to read', type=str,
-                                                 default=None)
-    parser.add_argument('--table', help='Table to use',
+    parser.add_argument('-t', '--table', help='Table to use',
                         type=str, default=None)
-    parser.add_argument('--es-workaround', help='Flag to enable working around'
-                        'ES stripping leading whitespace',
-                        default=False, action='store_true')
+    parser.add_argument('-p', '--page', help='Page number to extract (zero based)',
+                        type=int, default=None)
     args = parser.parse_args()
 
-    process_file(args.hocr, args.annotated_text, args.table, args.es_workaround)
+    process_file(args.infile, args.page, args.table)
+
```

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-combine-stream` & `archive-hocr-tools-1.1.9/bin/hocr-combine-stream`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             page_no += 1
 
             s = etree.tostring(page, pretty_print=True, method='xml',
                                encoding='utf-8').decode('utf-8')
             # Let's Remove the xmlns in the div.
             # Yes, this is horrible, but cleanup_namespaces doesn't help
             # since as far as tostring knows, this is the root.
-            # Let's also add two spaces for indentation for the first
+            # Let's also add two spaces for indendation for the first
             # page, and one for all the other pages.
             if page_no == 1:
                 s = '  ' + \
                     s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
             else:
                 s = ' ' + \
                     s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
@@ -81,13 +81,14 @@
     parser.add_argument('-g', '--glob', help='Glob of files to parse',
                         type=str, default=None)
     args = parser.parse_args()
 
     files_to_process = glob(args.glob)
 
     if not len(files_to_process):
+        import sys
         print('No files to process!', file=sys.stderr)
         sys.exit(1)
 
     files_to_process = sorted(files_to_process)
 
     process_files(files_to_process)
```

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-extract-page` & `archive-hocr-tools-1.1.9/bin/fts-text-match`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
 
-from lxml import etree
+import json
 
-from hocr.searching import hocr_load_lookup_table, hocr_lookup_page_by_dat
-from hocr.parse import hocr_page_iterator
-from hocr.util import open_if_required, get_header_footer
+from hocr.searching import hocr_load_lookup_table
+from hocr.util import open_if_required
+from hocr.fts import find_matches
 
-def process_file(filepath, pageno, tablepath):
-    fd = open_if_required(filepath)
-    top, bottom = get_header_footer(fd)
 
-    sys.stdout.buffer.write(top)
+def process_file(hocrfile, textfile, tablepath):
+    lookup_table = hocr_load_lookup_table(tablepath)
 
-    if tablepath:
-        lookup_table = hocr_load_lookup_table(tablepath)
-        fp = open_if_required(filepath)
+    hocrfp = open_if_required(hocrfile)
+    textfp = open_if_required(textfile)
+    text = textfp.read().decode('utf-8')
 
-        dat = lookup_table[pageno]
-        page = hocr_lookup_page_by_dat(fp, dat)
-    else:
-        for idx, page in enumerate(hocr_page_iterator(fd)):
-            if idx == pageno:
-                break
-
-    s = etree.tostring(page, pretty_print=True, method='xml',
-                       encoding='utf-8').decode('utf-8')
-
-    s = ' ' + s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
-    s = s.encode('utf-8')
-    sys.stdout.buffer.write(s)
-
-    sys.stdout.buffer.write(bottom)
+    for word_results in find_matches(lookup_table, hocrfp, text):
+        json.dump(word_results, sys.stdout)
+        sys.stdout.write('\n')
 
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='hOCR single page extractor')
-    parser.add_argument('-f', '--infile', help='Filename to read',
+    parser = argparse.ArgumentParser(description='hOCR lookup table '
+                                                 'paragraph-level validator')
+    parser.add_argument('--hocr', help='hOCR Filename to read',
                         type=str, default=None)
-    parser.add_argument('-t', '--table', help='Table to use',
+    parser.add_argument('--annotated-text', help='Annotated fulltext filename '
+                                                 'to read', type=str,
+                                                 default=None)
+    parser.add_argument('--table', help='Table to use',
                         type=str, default=None)
-    parser.add_argument('-p', '--page', help='Page number to extract (zero based)',
-                        type=int, default=None)
     args = parser.parse_args()
 
-    process_file(args.infile, args.page, args.table)
-
+    process_file(args.hocr, args.annotated_text, args.table)
```

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-flatten-pages` & `archive-hocr-tools-1.1.9/bin/hocr-fold-chars`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 #!/usr/bin/env python
 
 import sys
-import re
-
 import argparse
 
 from lxml import etree
 
 from hocr.parse import hocr_page_iterator
 from hocr.util import open_if_required, get_header_footer
 
-rem = re.compile("<div class=['\"]ocr_page['\"].*>")
 
-def process_file(filepath):
-    fd = open_if_required(filepath)
+def process_files(infile):
+    fd = open_if_required(infile)
     top, bottom = get_header_footer(fd)
 
-    # Idea: strip ending for first page, add ending to last page?
+    sys.stdout.buffer.write(top)
 
-    first = True
+    page_no = 0
 
-    print(top.decode('utf-8'))
-    for pageno, page in enumerate(hocr_page_iterator(fd)):
+    fd.seek(0)
+    for page in hocr_page_iterator(fd):
+        words = page.xpath(".//*[@class='ocrx_word']")
+        for word in words:
+            chars = word.xpath("*[@class='ocrx_cinfo']")
+            txt = ''
+            for char in chars:
+                txt += char.text
+
+            ch = word.getchildren()
+            for c in ch:
+                word.remove(c)
+            word.text = txt
 
         s = etree.tostring(page, pretty_print=True, method='xml',
                            encoding='utf-8').decode('utf-8')
-
-        s = ' ' + s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
-
-        if first:
-            # Remove the last </div> of the first page
-            idx = s.rindex('</div>')
-            s = s[:idx]
-            first = False
+        # Let's Remove the xmlns in the div.
+        # Yes, this is horrible, but cleanup_namespaces doesn't help
+        # since as far as tostring knows, this is the root.
+        # Let's also add two spaces for indendation for the first
+        # page, and one for all the other pages.
+        if page_no == 1:
+            s = '  ' + \
+                s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
         else:
-            # XXX: This assumes that <div class="ocr_page"> is the only html
-            # element on the line (!)
-            s = re.sub(rem, '', s, count=1)
-
-        print(s)
+            s = ' ' + \
+                s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
 
-    print(bottom.decode('utf-8'))
+        s = s.encode('utf-8')
+        sys.stdout.buffer.write(s)
 
+    sys.stdout.buffer.write(bottom)
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='hOCR page flatten (combine several pages into one page)')
-    parser.add_argument('-f', '--infile', help='Filename to read',
+    parser = argparse.ArgumentParser(description='Fold character-based hOCR '
+                                                 'into word-based hOCR')
+    parser.add_argument('-f', '--infile', help='Input file',
                         type=str, default=None)
     args = parser.parse_args()
 
-    process_file(args.infile)
+    process_files(args.infile)
```

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-lookup-check` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-check`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 
+import sys
 import argparse
 
 from hocr.parse import hocr_page_to_word_data_fast
 from hocr.searching import hocr_load_lookup_table, hocr_lookup_page_by_dat, \
         hocr_lookup_by_plaintext_offset
 from hocr.util import open_if_required
 from hocr.text import hocr_paragraph_text
```

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-lookup-create` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-create`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-lookup-reconstruct` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-reconstruct`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/bin/hocr-text-paragraphs` & `archive-hocr-tools-1.1.9/bin/hocr-text-paragraphs`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/hocr/parse.py` & `archive-hocr-tools-1.1.9/hocr/parse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gzip
 import re
 
 from lxml import etree
 
-from .util import open_if_required, HOCR_SCHEMA
+from .util import open_if_required
 
 
 WRITING_DIRECTION_UNSPECIFIED = 0
 WRITING_DIRECTION_LEFT_TO_RIGHT = 1
 WRITING_DIRECTION_RIGHT_TO_LEFT = 2
 WRITING_DIRECTION_TOP_TO_BOTTOM = 3
 
@@ -35,19 +35,22 @@
     Returns:
 
     * Iterator returning a etree.Element hOCR page.
     """
     fp = open_if_required(fd_or_path)
 
     # Seek to start
-    fp.seek(0)
+    # TODO: We should make tools call seek if they should, rather than having
+    # this function call seek()
+    # Do not remove this for now
+    #fp.seek(0)
 
     # TODO: Add gzip loading, specify what file_like should be (I suggest just
     # file descriptor or just path)
-    doc = etree.iterparse(fp, tag=(HOCR_SCHEMA + 'div', 'div'))
+    doc = etree.iterparse(fp, tag='{http://www.w3.org/1999/xhtml}div')
     for act, elem in doc:
         if elem.tag[-3:] == 'div' and elem.attrib['class'] == 'ocr_page':
             page = elem
             yield page
 
             elem.clear()
 
@@ -103,15 +106,15 @@
     Args:
 
     * hocr_page: a single hocr_page as returned by hocr_page_iterator
     * (optional) scaler: a scalar to scale font sizes by
 
     Returns:
 
-    A list of paragraphs, each paragraph containing a list of lines, and each
+    A list of paragraph, each paragraph containing a list of lines, and each
     line containing a list of words, plus properties.
 
     Paragraphs have the following attributes:
 
     * `'lines'`: the lines that form this paragraph
 
     Lines have the following attributes:
@@ -126,22 +129,21 @@
     * `'bbox'`: bounding box (tuple of 4 floats)
     * `'fontsize'`: fontsize as a float, or 0.
     * `'writing_direction'`: See WRITING_DIRECTION_* constants
     * `'confidence'`: word confidence, 0 - 100
     """
     paragraphs = []
 
-    for par in hocr_page.xpath('.//*[@class="ocrx_block" or @class="ocr_par"]'):
+    for par in hocr_page.xpath('.//*[@class="ocr_par"]'):
         paragraph_data = {'lines': []}
 
         paragraph_writing_direction = WRITING_DIRECTION_UNSPECIFIED
         if 'dir' in par.attrib:
             paragraph_writing_direction = wdmap[par.attrib['dir']]
 
-        # We assume that the direct children are all the lines
         for line in par.getchildren():
             line_data = {}
 
             linebox = BBOX_REGEX.search(line.attrib['title']).group(1).split()
             baseline = BASELINE_REGEX.search(line.attrib['title'])
             if baseline is not None:
                 baseline = baseline.group(1).split()
@@ -159,38 +161,20 @@
                 rawtext = ''
                 wordbased = True
                 for char in word.xpath('.//*[@class="ocrx_cinfo"]'):
                     rawtext += char.text
                     wordbased = False
 
                 if wordbased:
-                    wword = word
-                    # Words may contains additional nodes like <em>
-                    while True:
-                        children = wword.getchildren()
-                        if len(children) == 0:
-                            break
-
-                        if len(children) > 1:
-                            raise ValueError('Not character based but word has multiple children?')
-
-                        wword = children[0]
-
-                    rawtext = wword.text
-
-                    if wword.text is None:
-                        raise ValueError('Word with no text value?')
+                    rawtext = word.text
 
                 box = BBOX_REGEX.search(word.attrib['title']).group(1).split()
                 box = [float(i) for i in box]
 
-                conf = None
-                m = X_WCONF_REGEX.search(word.attrib['title'])
-                if m:
-                    conf = int(m.group(1).split()[0])
+                conf = int(X_WCONF_REGEX.search(word.attrib['title']).group(1).split()[0])
 
                 f_sizeraw = X_FSIZE_REGEX.search(word.attrib['title'])
                 if f_sizeraw:
                     x_fsize = float(f_sizeraw.group(1))
                     x_fsize *= scaler
                 else:
                     x_fsize = 0. # Will get fixed later on, in pdfrenderer at least
@@ -210,67 +194,14 @@
             #print('Line words:', word_data)
             paragraph_data['lines'].append(line_data)
 
         paragraphs.append(paragraph_data)
 
     return paragraphs
 
-def hocr_page_to_photo_data(hocr_page, minimum_page_area_pct=10):
-    """
-    Parses a single hocr_page into photo data.
-
-    Args:
-
-    * hocr_page: a single hocr_page as returned by hocr_page_iterator
-    * (optional) minimum_page_area_pct: a minimum percentage of the page area the picture should inhabit
-
-    Returns:
-
-    A list of bounding boxes where photos were found
-    """
-
-    # Get the actual boxes from the page
-    photo_boxes = []
-    for photo in hocr_page.xpath('.//*[@class="ocr_photo"]'):
-        box = BBOX_REGEX.search(photo.attrib['title']).group(1).split()
-        box = [float(i) for i in box]
-        photo_boxes.append(box)
-
-    # Helper function to determine if there are nested boxes
-    def box_contains_box(box_a, box_b):
-        return box_a[0] <= box_b[0] and box_a[1] <= box_b[1] \
-           and box_a[2] >= box_b[2] and box_a[3] >= box_b[3]
-
-    # Clean up the box data a bit
-    cleaned_photo_boxes = list(photo_boxes)
-    dim = hocr_page_get_dimensions(hocr_page)
-    area_page = dim[0]*dim[1]
-    for box_a in photo_boxes:
-        # Image must cover at least minimum_page_area_pct of page
-        width, height = box_a[2]-box_a[0], box_a[3]-box_a[1]
-        area_box = width*height
-        if area_box < area_page*(minimum_page_area_pct/100.):
-            try:
-                cleaned_photo_boxes.remove(box_a)
-                #print("Box %s is too small, removing" % (box_a))
-            except: # Already removed
-                pass
-
-        # Nested boxes are redundant
-        for box_b in photo_boxes:
-            if box_a == box_b:
-                continue
-            if box_contains_box(box_a, box_b):
-                try:
-                    cleaned_photo_boxes.remove(box_b)
-                    #print("Box %s is fully inside box %s, removing" % (box_b, box_a))
-                except: # Already removed
-                    pass
-
-    return cleaned_photo_boxes
 
 def get_title_attrs(title):
     # Assume Tesseract generated hOCR, where every ';' has a space after it
     sub_title = title.split('; ')
     box = None
     conf = None
 
@@ -313,18 +244,17 @@
     * `'bbox'`: bounding box (tuple of 4 floats)
     * `'confidence'`: word confidence, 0 - 100
     """
     paragraphs = []
 
     has_ocrx_cinfo = 0
 
-    for par in hocr_page.xpath('.//*[@class="ocrx_block" or @class="ocr_par"]'):
+    for par in hocr_page.xpath('.//*[@class="ocr_par"]'):
         paragraph_data = {'lines': []}
 
-        # We assume that the direct children are all the lines
         for line in par.getchildren():
             line_data = {}
 
             word_data = []
             for word in line.xpath('.//*[@class="ocrx_word"]'):
                 title = word.attrib['title']
 
@@ -338,30 +268,16 @@
                         wordbased = False
                         has_ocrx_cinfo = 1
 
                 if has_ocrx_cinfo == 0:
                     has_ocrx_cinfo = 2
 
                 if wordbased:
-                    # Words may contains additional nodes like <em>
-                    while True:
-                        children = word.getchildren()
-                        if len(children) == 0:
-                            break
-
-                        if len(children) > 1:
-                            raise ValueError('Not character based but word has multiple children?')
-
-                        word = children[0]
-
                     rawtext = word.text
 
-                    if word.text is None:
-                        raise ValueError('Word with no text value?')
-
                 word_data.append({'bbox': box, 'text': rawtext,
                                   'confidence': conf})
 
 
             line_data['words'] = word_data
             paragraph_data['lines'].append(line_data)
```

### Comparing `archive-hocr-tools-1.1.37/hocr/searching.py` & `archive-hocr-tools-1.1.9/hocr/searching.py`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.37/hocr/text.py` & `archive-hocr-tools-1.1.9/hocr/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import xml.parsers.expat
 
 from .util import open_if_required
-from .parse import hocr_page_to_word_data_fast, hocr_page_iterator
+from .parse import hocr_page_to_word_data, hocr_page_to_word_data_fast, \
+        hocr_page_iterator, hocr_page_get_dimensions
 
 
 def hocr_paragraph_text(paragraph):
     """
     Reconstruct text that matches the FTS text from a hOCR paragraph.
     Returns a tuple, first item in the tuple is the text, the second is a
     boolean, indicating if this paragraph is to be merged into the next one, see
```

### Comparing `archive-hocr-tools-1.1.37/hocr/util.py` & `archive-hocr-tools-1.1.9/hocr/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import gzip
-import io
 
 from lxml import etree
 
 #: Contains the HOCR schema
 HOCR_SCHEMA = '{http://www.w3.org/1999/xhtml}'
 
 
@@ -19,42 +18,14 @@
             xml_file = open(fd_or_path, 'rb')
     else:
         xml_file = fd_or_path
 
     return xml_file
 
 
-def get_ocr_system(fd):
-    """
-    Read the ocr-system meta tag from a new file descriptor containing a hOCR
-    document. If you want to use an existing file descriptor, ensure to seek to
-    the start first.
-
-    Args:
-
-    * fd: Open file descriptor
-
-    Return:
-
-    * string of the content system or None if none is specified
-    """
-    header, footer = get_header_footer(fd)
-
-    bio = io.BytesIO()
-    bio.write(header + footer)
-    bio.seek(0)
-
-    parse = etree.iterparse(bio, tag=(HOCR_SCHEMA+'meta',), events=('end',))
-    for (start_end, element) in parse:
-        if element.attrib.get('name') == 'ocr-system':
-            return element.attrib.get('content')
-
-    return None
-
-
 def get_header_footer(fd):
     """
     Extract the parts before and after the body elements from a given XML file
 
     Args:
 
     * fd: Open file descriptor
```

### Comparing `archive-hocr-tools-1.1.37/setup.py` & `archive-hocr-tools-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,18 @@
       keywords=['hOCR', 'Internet Archive'],
       license='AGPL-3.0',
       scripts=['bin/hocr-combine-stream', 'bin/hocr-fold-chars',
                'bin/hocr-text', 'bin/fts-text-annotate',
                'bin/fts-text-match', 'bin/hocr-lookup-check',
                'bin/hocr-lookup-create', 'bin/hocr-lookup-reconstruct',
                'bin/hocr-text-paragraphs', 'bin/hocr-extract-page',
-               'bin/abbyy-to-hocr', 'bin/hocr-split-pages',
-               'bin/hocr-flatten-pages', 'bin/hocr-confidence-filter',
-               'bin/hocr-to-epub', 'bin/pdf-to-hocr'],
+               'bin/abbyy-to-hocr'],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Programming Language :: Python :: 3',
       ],
       python_requires='>=3.6',
       include_package_data=True,
-      install_requires=['lxml==4.6.5'],
-      extras_require={
-          'epub': ['ebooklib==0.17.1', 'internetarchive-deriver-module==1.0.1', 'iso639==0.1.4'],
-          'pdf': ['PyMuPDF==1.19.2', 'numpy==1.21.3'],
-      },
+      install_requires=['lxml'],
       package_data={'hocr': ['data/*']})
```

