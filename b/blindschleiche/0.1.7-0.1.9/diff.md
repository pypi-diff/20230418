# Comparing `tmp/blindschleiche-0.1.7.tar.gz` & `tmp/blindschleiche-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blindschleiche-0.1.7.tar", last modified: Wed Nov 30 13:20:52 2022, max compression
+gzip compressed data, was "blindschleiche-0.1.9.tar", last modified: Tue Apr 18 19:39:06 2023, max compression
```

## Comparing `blindschleiche-0.1.7.tar` & `blindschleiche-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0      951 2022-07-03 18:31:46.616503 blindschleiche-0.1.7/README.md
--rw-r--r--   0        0        0     1365 2022-11-30 13:19:45.687422 blindschleiche-0.1.7/blsl/__init__.py
--rw-r--r--   0        0        0      317 2022-07-02 07:55:13.963614 blindschleiche-0.1.7/blsl/__main__.py
--rw-r--r--   0        0        0      848 2022-07-10 17:54:36.042039 blindschleiche-0.1.7/blsl/falen.py
--rw-r--r--   0        0        0     3197 2022-11-30 13:19:17.711262 blindschleiche-0.1.7/blsl/genigvjs.py
--rw-r--r--   0        0        0     3882 2022-11-30 12:55:05.202936 blindschleiche-0.1.7/blsl/liftoff_gff3.py
--rw-r--r--   0        0        0     1953 2022-07-14 14:39:28.130724 blindschleiche-0.1.7/blsl/mask2bed.py
--rw-r--r--   0        0        0     1170 2022-07-05 19:31:42.400945 blindschleiche-0.1.7/blsl/n50.py
--rw-r--r--   0        0        0     4384 2022-11-30 12:55:05.202936 blindschleiche-0.1.7/blsl/pansn_rename.py
--rw-r--r--   0        0        0     3189 2022-07-05 19:34:03.373877 blindschleiche-0.1.7/blsl/telogrep.py
--rw-r--r--   0        0        0      427 2022-11-30 13:16:35.070334 blindschleiche-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      193 1970-01-01 00:00:00.000000 blindschleiche-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2142 2023-04-18 19:37:51.093886 blindschleiche-0.1.9/README.md
+-rw-r--r--   0        0        0     1773 2023-04-18 19:35:26.476534 blindschleiche-0.1.9/blsl/__init__.py
+-rw-r--r--   0        0        0      317 2022-07-02 07:55:13.963614 blindschleiche-0.1.9/blsl/__main__.py
+-rw-r--r--   0        0        0      848 2022-07-10 17:54:36.042039 blindschleiche-0.1.9/blsl/falen.py
+-rw-r--r--   0        0        0     5274 2023-04-13 08:46:56.999174 blindschleiche-0.1.9/blsl/genigvjs.py
+-rw-r--r--   0        0        0     6547 2023-04-18 19:35:26.476534 blindschleiche-0.1.9/blsl/ildemux.py
+-rw-r--r--   0        0        0     1324 2023-04-18 19:35:26.476534 blindschleiche-0.1.9/blsl/ilsample.py
+-rw-r--r--   0        0        0     3882 2022-11-30 12:55:05.202936 blindschleiche-0.1.9/blsl/liftoff_gff3.py
+-rw-r--r--   0        0        0     1953 2022-07-14 14:39:28.130724 blindschleiche-0.1.9/blsl/mask2bed.py
+-rw-r--r--   0        0        0     1170 2022-07-05 19:31:42.400945 blindschleiche-0.1.9/blsl/n50.py
+-rw-r--r--   0        0        0     4842 2022-12-14 13:40:48.624492 blindschleiche-0.1.9/blsl/pansn_rename.py
+-rw-r--r--   0        0        0     1338 2023-04-13 09:11:23.397960 blindschleiche-0.1.9/blsl/regionbed.py
+-rw-r--r--   0        0        0     3189 2022-07-05 19:34:03.373877 blindschleiche-0.1.9/blsl/telogrep.py
+-rw-r--r--   0        0        0     1227 2023-04-18 19:35:24.624638 blindschleiche-0.1.9/blsl/uniref_accessionmap.py
+-rw-r--r--   0        0        0      427 2022-11-30 13:16:35.070334 blindschleiche-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      193 1970-01-01 00:00:00.000000 blindschleiche-0.1.9/PKG-INFO
```

### Comparing `blindschleiche-0.1.7/blsl/__init__.py` & `blindschleiche-0.1.9/blsl/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from sys import argv, exit
 
-__version__ = "0.1.7"
+__version__ = "0.1.9"
 
 cmds = {}
 
 from .telogrep import telogrep_main
 cmds["telogrep"] = telogrep_main
 
 from .n50 import n50_main
@@ -27,22 +27,36 @@
 
 from .liftoff_gff3 import liftoff_gff3_main
 cmds["liftoff-gff3"] = liftoff_gff3_main
 
 from .pansn_rename import main as pansn_rename_main
 cmds["pansn-rename"] = pansn_rename_main
 
+from .ildemux import main as ildemux_main
+cmds["ildemux"] = ildemux_main
 
-def mainhelp():
+from .ilsample import main as ilsample_main
+cmds["ilsample"] = ilsample_main
+
+from .regionbed import main as regionbed_main
+cmds["regionbed"] = regionbed_main
+
+from .uniref_accessionmap import main as uniref_main
+cmds["uniref-acc2taxid"] = uniref_main
+
+
+def mainhelp(argv=None):
+    """Print this help message"""
     print("USAGE: blsl <subtool> [options...]\n\n")
     print("Where <subtool> is one of:\n")
     for tool, func in cmds.items():
-        print("  {:<12}".format(tool + ":"), "  ", func.__doc__)
+        print("  {:<19}".format(tool + ":"), " ", func.__doc__.split("\n")[0])
     print("\n\nUse blsl subtool --help to get help about a specific tool")
 
+cmds["help"] = mainhelp
 
 def main():
     if len(argv) < 2:
         mainhelp()
         exit(0)
     if argv[1] not in cmds:
         print("ERROR:", argv[1], "is not a known subtool. See help below")
```

### Comparing `blindschleiche-0.1.7/blsl/falen.py` & `blindschleiche-0.1.9/blsl/falen.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.1.7/blsl/liftoff_gff3.py` & `blindschleiche-0.1.9/blsl/liftoff_gff3.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.1.7/blsl/mask2bed.py` & `blindschleiche-0.1.9/blsl/mask2bed.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.1.7/blsl/n50.py` & `blindschleiche-0.1.9/blsl/n50.py`

 * *Files identical despite different names*

### Comparing `blindschleiche-0.1.7/blsl/pansn_rename.py` & `blindschleiche-0.1.9/blsl/pansn_rename.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 except ImportError:
     def tqdm(*args, **kwargs):
         return args[0]
 
 import argparse
 import re
 from pathlib import Path
-from sys import stderr
+from sys import stderr, exit
 
 
-def make_replacer(reffa, mode, delim="~", outdelim="~", refdelim="~"):
+def make_replacer(mode, reffa=None, org_name=None, delim="~", outdelim="~", refdelim="~"):
     names = []
     if not reffa.endswith(".fai"):
         reffa += ".fai"
     with open(reffa) as fh:
         for line in fh:
             names.append(line.split()[0])
     fromto = {}
     for name in names:
-        splitname = name.strip().split(refdelim)
-        fromname = delim.join(splitname)
+        if org_name is not None:
+            splitname = [org_name, "0", name]
+        else:
+            splitname = name.strip().split(refdelim)
+        pansn_name = delim.join(splitname)
         if mode == "cat": 
-            fromto[fromname] = outdelim.join(splitname)
+            fromto[pansn_name] = outdelim.join(splitname)
         elif mode == "add":
             fromto[splitname[2]] = outdelim.join(splitname)
         elif mode == "rm":
-            fromto[fromname] = splitname[2]
+            fromto[pansn_name] = splitname[2]
     return fromto
 
 
 def do_tsv(infh, outfh, cols, replacer, coldelim="\t"):
     for line in tqdm(infh):
         if line.startswith("#"):
             outfh.write(line)
@@ -74,35 +77,39 @@
         help="Delimiter between fields in PanSN names in <INPUT> (the # in indiv#1#chr1)")
     ap.add_argument("-D", "--out-delim",
         help="--delim for the output. Defaults to the same as --delim.")
     ap.add_argument("-r", "--reference-fasta", required=True,
         help="Reference fasta file with PanSN names.")
     ap.add_argument("-R", "--ref-delim",
         help="Delimiter between fields in PanSN names in the --reference-fasta file (default: same as --delim)")
+    ap.add_argument("-n", "--org-name",
+        help="Organism name (or similar) to prepend to current identifiers (separated by --out-delim).")
     ap.add_argument("-c", "--colidx", action="append", type=int,
         help="Which column in TSV should be sub'd? (default depends on input "
              "filetype, normally 0, use more than once for multiple columns "
              "e.g. -c 0 -c 3 for 1st & 4th cols).")
     ap.add_argument("-m", "--mode", choices=["cat", "rm", "add"],
         help="What should I do? (see below)")
     ap.add_argument("-o", "--output", default="-", type=argparse.FileType("w"),
         help="output filename, default: stdout")
     ap.add_argument("input", type=argparse.FileType("r"))
     args = ap.parse_args(argv)
 
+    if args.reference_fasta is None and args.org_name is None:
+        print("ERROR: must give either --reference-file or --org-name as source of new names")
+        exit(1)
     if args.colidx is None:
         args.colidx = [0, ]
     args.colidx = list(sorted(set(args.colidx)))
     if args.out_delim is None:
         args.out_delim = args.delim
     if args.ref_delim is None:
         args.ref_delim = args.delim
         
-    
-    replacer = make_replacer(args.reference_fasta, args.mode, args.delim, args.out_delim, args.ref_delim)
+    replacer = make_replacer(args.mode, args.reference_fasta, args.org_name, args.delim, args.out_delim, args.ref_delim)
     
     input_ftype = "tsv"
     try:
         input_filename = Path(args.input.name)
         if input_filename.suffix in fasta_exts:
             input_ftype = "fasta"
         elif input_filename.suffix in tsv_exts:
```

### Comparing `blindschleiche-0.1.7/blsl/telogrep.py` & `blindschleiche-0.1.9/blsl/telogrep.py`

 * *Files identical despite different names*

