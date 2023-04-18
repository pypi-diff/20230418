# Comparing `tmp/varvamp-0.6.tar.gz` & `tmp/varvamp-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.6.tar", last modified: Mon Apr 17 14:41:46 2023, max compression
+gzip compressed data, was "varvamp-0.7.tar", last modified: Tue Apr 18 14:46:09 2023, max compression
```

## Comparing `varvamp-0.6.tar` & `varvamp-0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:46.381536 varvamp-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-17 14:41:46.381536 varvamp-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-17 14:41:29.000000 varvamp-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:41:46.381536 varvamp-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 14:41:29.000000 varvamp-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:46.377536 varvamp-0.6/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:46.381536 varvamp-0.6/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/conserved.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-17 14:41:29.000000 varvamp-0.6/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:46.381536 varvamp-0.6/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 14:41:46.000000 varvamp-0.6/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-18 14:46:09.310270 varvamp-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 14:45:49.000000 varvamp-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:46:09.310270 varvamp-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-18 14:45:49.000000 varvamp-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/conserved.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-18 14:45:49.000000 varvamp-0.7/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:46:09.310270 varvamp-0.7/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 14:46:09.000000 varvamp-0.7/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.6/PKG-INFO` & `varvamp-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.6
+Version: 0.7
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.6/README.md` & `varvamp-0.7/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/setup.py` & `varvamp-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/command.py` & `varvamp-0.7/varvamp/command.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/alignment.py` & `varvamp-0.7/varvamp/scripts/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,18 +162,18 @@
     """
     cleaned_alignment = []
 
     for sequence in alignment:
         start = 0
         masked_seq = str()
         for region in gaps_to_mask:
-            # check if it is three bases or more and mark with 2 Ns
+            # check if it is three bases or more and mask with 2 Ns
             if region[1]-region[0] >= config.QAMPLICON_DEL_CUTOFF:
                 mask = "NN"
-            # or mask
+            # or mask with one N (small deletion)
             else:
                 mask = "N"
             stop = region[0]
             masked_seq_temp = sequence[1][start:stop]
             # check if the deletion is at the start
             if len(masked_seq_temp) == 0:
                 masked_seq = mask
```

### Comparing `varvamp-0.6/varvamp/scripts/config.py` & `varvamp-0.7/varvamp/scripts/config.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/consensus.py` & `varvamp-0.7/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/conserved.py` & `varvamp-0.7/varvamp/scripts/conserved.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,85 +15,74 @@
     # init the variables
     current_window = []
     writable = False
     in_ambiguous_region = True
     last_amb = 0
     conserved_regions = []
 
-    seq = str(consensus_amb) + 2*'N'
+    # append enough Ns to ensure that last window is closed
+    seq = str(consensus_amb) + allowed_ambiguous*'N'
+
     for idx, nuc in enumerate(seq):
         if in_ambiguous_region and nuc in config.NUCS:
             in_ambiguous_region = False
             # just entered a new stretch of non-ambiguous bases
             # may be time to open a new window
             if not current_window:
+                # track window start and ambiguous chars so far
                 current_window = [idx, 0]
-                amb_pos = []
-                # create new window if none is there. First element
-                # keeps track of start of the window, second element is
-                # a counter that resets if two ambiguous chars are longer
-                # than specified apart and last one counts all ambiguous
-                # chars. also track all amb chars after a window has opened
+                all_previous_ambiguous_pos = []
             continue
         if nuc not in config.NUCS:
             if current_window:
                 in_ambiguous_region = True
                 amb_to_amb_len = idx - last_amb
-                if nuc != "N":
-                    # track previous amb pos only if current pos is not a N as this
-                    # region is witeable
-                    amb_pos.append(idx)
-                if current_window[1] >= allowed_ambiguous or nuc == "N":
-                    # check if there were too many previous amb char in subwindow
-                    # and make it writable. Always make it writeable if N is
-                    # reached
+                all_previous_ambiguous_pos.append(idx)
+                # check if there were too many previous amb char in subwindow
+                # or if N is reached -> writeable
+                if current_window[1] == allowed_ambiguous or nuc == "N":
                     writable = True
+                    # are the current and last ambig char sufficiently far?
                     if amb_to_amb_len >= config.PRIMER_SIZES[0] and nuc != "N":
-                        # check if the last amb is sufficiently far, if yes keep
-                        # window open and set amb counter to 0, reset also the
-                        # list of amb positions and track only the current pos
                         current_window[1] = 0
+                        all_previous_ambiguous_pos = [idx]
                         writable = False
-                        amb_pos = [idx]
 
                 current_window[1] += 1
 
                 if writable:
                     writable = False
+                    # check if the writable window has a sufficient length.
                     window_length = idx-current_window[0]
                     if window_length >= config.PRIMER_SIZES[0]:
-                        # check if the writable window has a sufficient length.
                         conserved_regions.append([current_window[0], idx])
-                        # reset the window and the list of amb positions
-                        # after it was written
-                        current_window = []
-                    elif nuc == "N":
-                        # if nuc was a N and region was not written also open a
-                        # new window
-                        current_window = []
+                    # reset the window start to the last ambig char
+                    if nuc != "N":
+                        current_window[0] = all_previous_ambiguous_pos[0]+1
+                        current_window[1] = current_window[1] - 1
+                        all_previous_ambiguous_pos.pop(0)
+                    # or open a new window
                     else:
-                        # else set the start pos to the next amb pos and
-                        # check again if the new window matches the criteria
-                        current_window[0] = amb_pos[0]+1
-                        current_window[1] = current_window[1]-1
-                        amb_pos.pop(0)
+                        current_window = []
+
             last_amb = idx
 
     return conserved_regions
 
 
 def mean(conserved_regions, consensus):
     """
     calculate the percentage of regions
     that are conserved
     """
-    sum = 0
+    covered_set = set()
     for region in conserved_regions:
-        sum += region[1]-region[0]
-    return round(sum/len(consensus)*100, 1)
+        pos_list = list(range(region[0], region[1]))
+        [covered_set.add(x) for x in pos_list]
+    return round(len(covered_set)/len(consensus)*100, 1)
 
 
 def digest_seq(seq, kmer_size):
     """
     digest the sequence into kmers
     """
     return[[seq[i:i+kmer_size], i, i+len(seq[i:i+kmer_size])] for i in range(len(seq)-kmer_size+1)]
@@ -109,10 +98,12 @@
         sliced_seq = consensus[region[0]:region[1]]
         for kmer_size in range(sizes[0], sizes[1]+1):
             kmers_temp = digest_seq(sliced_seq, kmer_size)
             # adjust the start and stop position of the kmers
             for kmer_temp in kmers_temp:
                 kmer_temp[1] = kmer_temp[1]+region[0]
                 kmer_temp[2] = kmer_temp[2]+region[0]
-            kmers += kmers_temp
+                if kmer_temp in kmers:
+                    continue
+                kmers.append(kmer_temp)
 
     return kmers
```

### Comparing `varvamp-0.6/varvamp/scripts/logging.py` & `varvamp-0.7/varvamp/scripts/logging.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/primers.py` & `varvamp-0.7/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/qpcr.py` & `varvamp-0.7/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/reporting.py` & `varvamp-0.7/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp/scripts/scheme.py` & `varvamp-0.7/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.6/varvamp.egg-info/PKG-INFO` & `varvamp-0.7/varvamp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.6
+Version: 0.7
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.6/varvamp.egg-info/SOURCES.txt` & `varvamp-0.7/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

