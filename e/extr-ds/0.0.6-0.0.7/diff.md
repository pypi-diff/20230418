# Comparing `tmp/extr-ds-0.0.6.tar.gz` & `tmp/extr-ds-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.6.tar", last modified: Sun Apr 16 19:36:44 2023, max compression
+gzip compressed data, was "extr-ds-0.0.7.tar", last modified: Tue Apr 18 10:03:31 2023, max compression
```

## Comparing `extr-ds-0.0.6.tar` & `extr-ds-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.257335 extr-ds-0.0.6/
--rw-rw-rw-   0        0        0     3883 2023-04-16 19:36:44.250979 extr-ds-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2728 2023-04-16 19:30:04.000000 extr-ds-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 19:36:44.263367 extr-ds-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-16 19:36:23.000000 extr-ds-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.056114 extr-ds-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.103126 extr-ds-0.0.6/src/extr_ds/
--rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.6/src/extr_ds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.246066 extr-ds-0.0.6/src/extr_ds/labelers/
--rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.6/src/extr_ds/labelers/__init__.py
--rw-rw-rw-   0        0        0     1604 2023-04-16 09:37:06.000000 extr-ds-0.0.6/src/extr_ds/labelers/iob.py
--rw-rw-rw-   0        0        0     3879 2023-04-16 19:35:58.000000 extr-ds-0.0.6/src/extr_ds/labelers/relation.py
--rw-rw-rw-   0        0        0     1145 2023-04-16 10:21:54.000000 extr-ds-0.0.6/src/extr_ds/models.py
--rw-rw-rw-   0        0        0     1059 2023-04-16 18:37:33.000000 extr-ds-0.0.6/src/extr_ds/tokenizer.py
--rw-rw-rw-   0        0        0     1561 2023-04-15 12:51:08.000000 extr-ds-0.0.6/src/extr_ds/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:36:44.225006 extr-ds-0.0.6/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     3883 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 19:36:43.000000 extr-ds-0.0.6/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.438516 extr-ds-0.0.7/
+-rw-rw-rw-   0        0        0     4025 2023-04-18 10:03:31.436303 extr-ds-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-04-18 10:02:42.000000 extr-ds-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:03:31.443818 extr-ds-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-18 09:58:31.000000 extr-ds-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.266364 extr-ds-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.304103 extr-ds-0.0.7/src/extr_ds/
+-rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.7/src/extr_ds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.425333 extr-ds-0.0.7/src/extr_ds/labelers/
+-rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.7/src/extr_ds/labelers/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-04-18 10:03:06.000000 extr-ds-0.0.7/src/extr_ds/labelers/iob.py
+-rw-rw-rw-   0        0        0     3885 2023-04-18 10:00:03.000000 extr-ds-0.0.7/src/extr_ds/labelers/relation.py
+-rw-rw-rw-   0        0        0      461 2023-04-18 09:59:18.000000 extr-ds-0.0.7/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0     1718 2023-04-17 21:01:45.000000 extr-ds-0.0.7/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.392208 extr-ds-0.0.7/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     4025 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-18 10:03:31.000000 extr-ds-0.0.7/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.6/PKG-INFO` & `extr-ds-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -20,16 +20,17 @@
         ```python
         text = 'Ted Johnson is a pitcher. Ted went to my school.'
         ```
         
         ### 1. Label Entities for Named-Entity Recognition Task (NER)
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
-        from extr_ds import IOB
+        from extr import RegEx, RegExLabel
+        from extr.entities import EntityExtactor
+        from extr_ds.labelers import IOB
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -44,15 +45,17 @@
         ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
         ## ]
         ```
         
         ### 2. Annotate for Relation Extraction Task (RE)
         
         ```python
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr.entities import EntityExtractor
+        from extr.relations import RegExRelationLabelBuilder, \
+                                   RelationExtractor
         from extr_ds.labelers import RelationClassification
         
         person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON',
                 [
                     r'\s+is\s+a\s+',
```

### Comparing `extr-ds-0.0.6/README.md` & `extr-ds-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 ```python
 text = 'Ted Johnson is a pitcher. Ted went to my school.'
 ```
 
 ### 1. Label Entities for Named-Entity Recognition Task (NER)
 
 ```python
-from extr import RegEx, RegExLabel, EntityExtactor
-from extr_ds import IOB
+from extr import RegEx, RegExLabel
+from extr.entities import EntityExtactor
+from extr_ds.labelers import IOB
 
 entity_extractor = EntityExtactor([
     RegExLabel('PERSON', [
         RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
@@ -38,15 +39,17 @@
 ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
 ## ]
 ```
 
 ### 2. Annotate for Relation Extraction Task (RE)
 
 ```python
-from extr import RegExRelationLabelBuilder, RelationExtractor
+from extr.entities import EntityExtractor
+from extr.relations import RegExRelationLabelBuilder, \
+                           RelationExtractor
 from extr_ds.labelers import RelationClassification
 
 person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
     .add_e1_to_e2(
         'PERSON',
         [
             r'\s+is\s+a\s+',
```

### Comparing `extr-ds-0.0.6/setup.py` & `extr-ds-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.6',
+    version='0.0.7',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
-        'extr==0.0.7'
+        'extr==0.0.8'
     ],
     url='https://github.com/dpasse/extr-ds',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

### Comparing `extr-ds-0.0.6/src/extr_ds/labelers/iob.py` & `extr-ds-0.0.7/src/extr_ds/labelers/iob.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Callable, Generator, Iterator, cast
-from extr import Entity, EntityExtractor
-from ..models import TokenGroup, Label
-from ..tokenizer import tokenizer
+from extr import Entity, TokenGroup
+from extr.entities import EntityExtractor
+from extr.tokenizers import tokenizer
+from ..models import Label
 
 
 class IOB():
     def __init__(self, sentence_tokenizer: Callable[[str], List[List[str]]], entity_extractor: EntityExtractor) -> None:
         self._sentence_tokenizer = sentence_tokenizer
         self._entity_extractor = entity_extractor
```

### Comparing `extr-ds-0.0.6/src/extr_ds/labelers/relation.py` & `extr-ds-0.0.7/src/extr_ds/labelers/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Callable, Dict, List, Tuple
-from extr import EntityExtractor, \
-                 EntityAnnotator, \
-                 RelationExtractor, \
-                 Relation, \
-                 Entity
-
+from extr import Relation, Entity
+from extr.entities import EntityExtractor, \
+                          EntityAnnotator
+from extr.relations import RelationExtractor
+from extr.tokenizers import tokenizer
 from ..models import RelationLabel
-from ..tokenizer import tokenizer
+
 
 class RelationClassification:
     def __init__(self,
                  sentence_tokenizer: Callable[[str], List[List[str]]],
                  entity_extractor: EntityExtractor,
                  relation_extractor: RelationExtractor,
                  no_relations: List[Tuple[str, str, str]]):
```

### Comparing `extr-ds-0.0.6/src/extr_ds/validators.py` & `extr-ds-0.0.7/src/extr_ds/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import List
+from typing import List, Union
 from dataclasses import dataclass
 from enum import Enum
 
 
-# class syntax
 class DifferenceTypes(Enum):
     NONE = 0
     MISMATCH = 1
     S1_MISSING = 2
     S2_MISSING = 3
 
 @dataclass
@@ -24,26 +23,31 @@
     sentence_labels_2: List[str]
     diffs_between_labels: List[Difference]
 
     @property
     def has_diffs(self) -> bool:
         return len(self.diffs_between_labels) > 0
 
-def check_for_differences(labels_1: List[str], labels_2: List[str]) -> Differences:
+EMPTY_SET = ['O', 'NO-RELATION']
+
+def check_for_differences(l1: Union[List[str], str], l2: Union[List[str], str]) -> Differences:
     def get_difference_type(label_1: str, label_2: str) -> DifferenceTypes:
         diff_type = DifferenceTypes.NONE
-        if label_2 == 'O' or len(label_2) == 0:
+        if label_2 in EMPTY_SET or len(label_2) == 0:
             diff_type = DifferenceTypes.S2_MISSING
-        elif label_1 == 'O' or len(label_1) == 0:
+        elif label_1 in EMPTY_SET or len(label_1) == 0:
             diff_type = DifferenceTypes.S1_MISSING
         else:
             diff_type = DifferenceTypes.MISMATCH
 
         return diff_type
 
+    labels_1 = [l1] if isinstance(l1, str) else l1
+    labels_2 = [l2] if isinstance(l2, str) else l2
+
     assert len(labels_1) == len(labels_2)
 
     diffs_between_labels = []
     for i, [label_1, label_2] in enumerate(zip(labels_1, labels_2)):
         if label_1 != label_2:
             diff_type = get_difference_type(label_1, label_2)
             diffs_between_labels.append(Difference(i, diff_type))
```

### Comparing `extr-ds-0.0.6/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.7/src/extr_ds.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -20,16 +20,17 @@
         ```python
         text = 'Ted Johnson is a pitcher. Ted went to my school.'
         ```
         
         ### 1. Label Entities for Named-Entity Recognition Task (NER)
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
-        from extr_ds import IOB
+        from extr import RegEx, RegExLabel
+        from extr.entities import EntityExtactor
+        from extr_ds.labelers import IOB
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -44,15 +45,17 @@
         ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
         ## ]
         ```
         
         ### 2. Annotate for Relation Extraction Task (RE)
         
         ```python
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr.entities import EntityExtractor
+        from extr.relations import RegExRelationLabelBuilder, \
+                                   RelationExtractor
         from extr_ds.labelers import RelationClassification
         
         person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON',
                 [
                     r'\s+is\s+a\s+',
```

