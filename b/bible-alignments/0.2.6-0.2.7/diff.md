# Comparing `tmp/bible_alignments-0.2.6.tar.gz` & `tmp/bible_alignments-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_alignments-0.2.6.tar", max compression
+gzip compressed data, was "bible_alignments-0.2.7.tar", max compression
```

## Comparing `bible_alignments-0.2.6.tar` & `bible_alignments-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.6/LICENSE
--rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.6/README.md
--rw-r--r--   0        0        0     1699 2023-04-17 20:24:58.984767 bible_alignments-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.6/src/.github/actions/run-checks/action.yml
--rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.6/src/.github/actions/setup-poetry-env/action.yml
--rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529247 bible_alignments-0.2.6/src/.github/workflows/on-merge-to-main.yml
--rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529364 bible_alignments-0.2.6/src/.github/workflows/on-pull-request.yml
--rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.6/src/.github/workflows/on-release-main.yml
--rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.6/src/.github/workflows/validate-codecov-config.yml
--rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.6/src/01-Exploration.ipynb
--rw-r--r--   0        0        0        0 2023-02-24 04:25:37.140718 bible_alignments-0.2.6/src/__init__.py
--rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.6/src/catalog.py
--rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.6/src/config.py
--rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.6/src/format/__init__.py
--rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.6/src/format/grapecity.py
--rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702000 bible_alignments-0.2.6/src/gcsource.py
--rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463000 bible_alignments-0.2.6/src/gctarget.py
--rw-r--r--   0        0        0     4536 2023-04-12 23:47:40.528000 bible_alignments-0.2.6/src/grapecity.py
--rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 bible_alignments-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    20131 2023-02-22 04:20:29.147219 bible_alignments-0.2.7/LICENSE
+-rw-r--r--   0        0        0      900 2023-03-01 18:19:16.168100 bible_alignments-0.2.7/README.md
+-rw-r--r--   0        0        0     1699 2023-04-18 14:13:25.664522 bible_alignments-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      554 2023-02-22 04:20:29.528825 bible_alignments-0.2.7/src/.github/actions/run-checks/action.yml
+-rw-r--r--   0        0        0     2033 2023-02-22 04:20:29.529037 bible_alignments-0.2.7/src/.github/actions/setup-poetry-env/action.yml
+-rw-r--r--   0        0        0      975 2023-02-22 04:20:29.529247 bible_alignments-0.2.7/src/.github/workflows/on-merge-to-main.yml
+-rw-r--r--   0        0        0      949 2023-02-22 04:20:29.529364 bible_alignments-0.2.7/src/.github/workflows/on-pull-request.yml
+-rw-r--r--   0        0        0     1964 2023-02-22 04:20:29.529486 bible_alignments-0.2.7/src/.github/workflows/on-release-main.yml
+-rw-r--r--   0        0        0      351 2023-02-22 04:20:29.529608 bible_alignments-0.2.7/src/.github/workflows/validate-codecov-config.yml
+-rw-r--r--   0        0        0    16557 2023-02-28 20:36:24.715176 bible_alignments-0.2.7/src/01-Exploration.ipynb
+-rw-r--r--   0        0        0      149 2023-04-18 14:05:38.099337 bible_alignments-0.2.7/src/__init__.py
+-rw-r--r--   0        0        0     4810 2023-03-16 20:46:04.251808 bible_alignments-0.2.7/src/catalog.py
+-rw-r--r--   0        0        0      247 2023-02-24 04:25:33.130530 bible_alignments-0.2.7/src/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 04:20:29.529807 bible_alignments-0.2.7/src/format/__init__.py
+-rw-r--r--   0        0        0     5829 2023-02-22 04:20:29.529962 bible_alignments-0.2.7/src/format/grapecity.py
+-rw-r--r--   0        0        0     2134 2023-04-12 01:30:26.702000 bible_alignments-0.2.7/src/gcsource.py
+-rw-r--r--   0        0        0     2193 2023-04-12 01:30:54.463000 bible_alignments-0.2.7/src/gctarget.py
+-rw-r--r--   0        0        0     5705 2023-04-18 12:59:07.522414 bible_alignments-0.2.7/src/grapecity.py
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 bible_alignments-0.2.7/PKG-INFO
```

### Comparing `bible_alignments-0.2.6/LICENSE` & `bible_alignments-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/README.md` & `bible_alignments-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/pyproject.toml` & `bible_alignments-0.2.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bible-alignments"
-version = "0.2.6"
+version = "0.2.7"
 description = "Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments."
 authors = ["Sean Boisen <sean.boisen@clear.bible>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Bible", "alignment", "Bible alignment"]
 repository = "https://github.com/Clear-Bible/Alignments"
 #documentation = "https://sboisen.github.io/alignments/"
```

### Comparing `bible_alignments-0.2.6/src/.github/actions/run-checks/action.yml` & `bible_alignments-0.2.7/src/.github/actions/run-checks/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/.github/actions/setup-poetry-env/action.yml` & `bible_alignments-0.2.7/src/.github/actions/setup-poetry-env/action.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/.github/workflows/on-merge-to-main.yml` & `bible_alignments-0.2.7/src/.github/workflows/on-merge-to-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/.github/workflows/on-pull-request.yml` & `bible_alignments-0.2.7/src/.github/workflows/on-pull-request.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/.github/workflows/on-release-main.yml` & `bible_alignments-0.2.7/src/.github/workflows/on-release-main.yml`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/01-Exploration.ipynb` & `bible_alignments-0.2.7/src/01-Exploration.ipynb`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/catalog.py` & `bible_alignments-0.2.7/src/catalog.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/format/grapecity.py` & `bible_alignments-0.2.7/src/format/grapecity.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/gcsource.py` & `bible_alignments-0.2.7/src/gcsource.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/gctarget.py` & `bible_alignments-0.2.7/src/gctarget.py`

 * *Files identical despite different names*

### Comparing `bible_alignments-0.2.6/src/grapecity.py` & `bible_alignments-0.2.7/src/grapecity.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Note that some of the target texts were typed in by hand, so may have
 minor differences from authoritative editions.
 
 """
 
 from collections import UserDict
 from dataclasses import dataclass, field
+import itertools
 import json
 from typing import Union
 
 from src import config, gcsource, gctarget
 
 # from . import config, gcsource, gctarget
 
@@ -49,38 +50,62 @@
         return len(self.sourceitems) == 1 and self.sourceitems[0].pos == "Name"
 
     def display(self) -> None:
         """Display text for alignments."""
         print(f"{self.identifier}: {[s.token for s in self.sourceitems]}\t{[s.token for s in self.targetitems]}")
 
 
-# @dataclass
-# class AlignmentSet:
-#     """Manage all the alignment data for a verse."""
-
-#     verseid: str
-#     items: list = field(default_factory=list)
-
-#     def __repr__(self) -> str:
-#         """Return a printed representation."""
-#         return f"<AlignmentSet({self.verseid})>"
-
-#     def namesets(self, sourceattr: str = "text") -> list:
-#         """Return a list of lists pairing a source name with target term(s).
-
-#         By default, the text attribute for the source is provided, or
-#         you can specify a different sourceattr.
-
-#         """
-#         return [
-#             (getattr(ag.sourceitems[0], sourceattr), t.text)
-#             for ag in self.items
-#             if ag.issourcename
-#             for t in ag.targetitems
-#         ]
+def verseid(ag):
+    """Key function for grouping by verse.
+
+    Takes an alignment group and return the verse ID.
+    """
+    # not sure why this doesn't work
+    # assert isinstance(ag, AlignmentGroup), f"Arg must be an AlignmentGroup instance: {ag}"
+    assert ag.__class__.__name__ == "AlignmentGroup", f"Arg must be an AlignmentGroup instance: {ag}"
+    return ag.identifier.split(".")[0]
+
+
+@dataclass
+class AlignmentSet:
+    """Manage all the alignment data for a verse."""
+
+    verseid: str
+    sources: list = field(default_factory=list)
+    targets: list = field(default_factory=list)
+    items: list = field(default_factory=list)
+
+    def __repr__(self) -> str:
+        """Return a printed representation."""
+        return f"<AlignmentSet({self.verseid})>"
+
+    @staticmethod
+    def from_aglist(aglist) -> "AlignmentSet":
+        """Return an AlignmentSet for a list of AlignmentGroups."""
+        assert aglist, f"List must not be empty: {aglist}"
+        verseID = verseid(aglist[0])
+        aset = AlignmentSet(verseid=verseID)
+        aset.sources = [item for ag in aglist for item in ag.sourceitems]
+        aset.targets = [item for ag in aglist for item in ag.targetitems]
+        aset.items = aglist
+        return aset
+
+    # def namesets(self, sourceattr: str = "text") -> list:
+    #     """Return a list of lists pairing a source name with target term(s).
+
+    #     By default, the text attribute for the source is provided, or
+    #     you can specify a different sourceattr.
+
+    #     """
+    #     return [
+    #         (getattr(ag.sourceitems[0], sourceattr), t.text)
+    #         for ag in self.items
+    #         if ag.issourcename
+    #         for t in ag.targetitems
+    #     ]
 
 
 class Reader(UserDict):
     """Read alignment data and integrate source and target."""
 
     def __init__(self, sourceid: str, targetid: str, languageid: str, processid: str) -> None:
         """Initialize Reader instance."""
@@ -114,7 +139,11 @@
         print(f"Target:\t{self.targetid}\t({len(self.targetreader)} words)")
         print(f"Process:\t{self.processid}")
         print(f"{len(self)} alignments")
 
     def source_concordance(self, value: str, attr: str = "lemma") -> list[AlignmentGroup]:
         """Return alignment groups whose source attr value is value."""
         return [ag for ag in self.data.values() if value in [getattr(s, attr) for s in ag.sourceitems]]
+
+    def verse_groups(self) -> list[list[AlignmentGroup]]:
+        """Return a list of lists of AlignmentGroups, by verse."""
+        return [list(g) for k, g in itertools.groupby(self.values(), verseid)]
```

### Comparing `bible_alignments-0.2.6/PKG-INFO` & `bible_alignments-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bible-alignments
-Version: 0.2.6
+Version: 0.2.7
 Summary: Word-level alignments for Bibles, including both automatic alignments and manually corrected alignments.
 Home-page: https://github.com/Clear-Bible/Alignments
 License: MIT
 Keywords: Bible,alignment,Bible alignment
 Author: Sean Boisen
 Author-email: sean.boisen@clear.bible
 Requires-Python: >=3.7,<4.0
```

