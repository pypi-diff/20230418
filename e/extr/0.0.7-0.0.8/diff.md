# Comparing `tmp/extr-0.0.7.tar.gz` & `tmp/extr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.7.tar", last modified: Sun Apr 16 18:50:49 2023, max compression
+gzip compressed data, was "extr-0.0.8.tar", last modified: Tue Apr 18 09:55:54 2023, max compression
```

## Comparing `extr-0.0.7.tar` & `extr-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.299183 extr-0.0.7/
--rw-rw-rw-   0        0        0     2431 2023-04-16 18:50:49.299183 extr-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-15 09:22:47.000000 extr-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 18:50:49.307184 extr-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-04-16 18:50:30.000000 extr-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.061978 extr-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.122471 extr-0.0.7/src/extr/
--rw-rw-rw-   0        0        0      247 2023-04-13 10:55:50.000000 extr-0.0.7/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1693 2023-04-16 18:19:36.000000 extr-0.0.7/src/extr/entities.py
--rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.7/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     2263 2023-04-16 18:19:38.000000 extr-0.0.7/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.7/src/extr/regex.py
--rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.7/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:50:49.291180 extr-0.0.7/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2431 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 18:50:48.000000 extr-0.0.7/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.332029 extr-0.0.8/
+-rw-rw-rw-   0        0        0     2522 2023-04-18 09:55:54.329917 extr-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1655 2023-04-18 09:54:04.000000 extr-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:55:54.338972 extr-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-04-18 09:55:24.000000 extr-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.123941 extr-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.195901 extr-0.0.8/src/extr/
+-rw-rw-rw-   0        0        0      268 2023-04-18 09:50:37.000000 extr-0.0.8/src/extr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.276871 extr-0.0.8/src/extr/entities/
+-rw-rw-rw-   0        0        0       80 2023-04-18 09:41:28.000000 extr-0.0.8/src/extr/entities/__init__.py
+-rw-rw-rw-   0        0        0      612 2023-04-18 09:41:38.000000 extr-0.0.8/src/extr/entities/annotator.py
+-rw-rw-rw-   0        0        0     1144 2023-04-18 09:45:57.000000 extr-0.0.8/src/extr/entities/extractor.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.8/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     2901 2023-04-18 09:42:52.000000 extr-0.0.8/src/extr/models.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.293671 extr-0.0.8/src/extr/regexes/
+-rw-rw-rw-   0        0        0       38 2023-04-18 09:50:25.000000 extr-0.0.8/src/extr/regexes/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-04-18 09:47:44.000000 extr-0.0.8/src/extr/regexes/regex.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.311522 extr-0.0.8/src/extr/relations/
+-rw-rw-rw-   0        0        0       96 2023-04-18 09:53:11.000000 extr-0.0.8/src/extr/relations/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-04-18 09:46:03.000000 extr-0.0.8/src/extr/relations/extractor.py
+-rw-rw-rw-   0        0        0     1676 2023-04-18 09:53:02.000000 extr-0.0.8/src/extr/relations/label_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.325156 extr-0.0.8/src/extr/tokenizers/
+-rw-rw-rw-   0        0        0       34 2023-04-18 09:43:44.000000 extr-0.0.8/src/extr/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-04-18 09:43:53.000000 extr-0.0.8/src/extr/tokenizers/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:55:54.261625 extr-0.0.8/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 09:55:53.000000 extr-0.0.8/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.7/PKG-INFO` & `extr-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
@@ -21,15 +21,16 @@
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtractor
+        from extr import RegEx, RegExLabel
+        from extr.entities import EntityExtractor
         
         entity_extractor = EntityExtractor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -44,16 +45,17 @@
         ## ]
         ```
         
         ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr import EntityAnnotator
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr.entities import EntityAnnotator
+        from extr.relations import RelationExtractor, \
+                                   RegExRelationLabelBuilder
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

### Comparing `extr-0.0.7/README.md` & `extr-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 text = 'Ted is a Pitcher.'
 ```
 
 ### 1. Entity Extraction
 > Find Named Entities from text.
 
 ```python
-from extr import RegEx, RegExLabel, EntityExtractor
+from extr import RegEx, RegExLabel
+from extr.entities import EntityExtractor
 
 entity_extractor = EntityExtractor([
     RegExLabel('PERSON', [
         RegEx([r'ted'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
@@ -38,16 +39,17 @@
 ## ]
 ```
 
 ### 2. Relation Extraction
 > Annotate and Extract Relationships between Entities
 
 ```python
-from extr import EntityAnnotator
-from extr import RegExRelationLabelBuilder, RelationExtractor
+from extr.entities import EntityAnnotator
+from extr.relations import RelationExtractor, \
+                           RegExRelationLabelBuilder
 
 ## define relationship between PERSON and POSITION
 relationship = RegExRelationLabelBuilder('is_a') \
     .add_e1_to_e2(
         'PERSON', ## e1
         [
             ## define how the relationship exists in nature
```

### Comparing `extr-0.0.7/setup.py` & `extr-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr',
-    version='0.0.7',
+    version='0.0.8',
     keywords='',
     description='Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[],
     url='https://github.com/dpasse/extr',
     long_description=long_description,
```

### Comparing `extr-0.0.7/src/extr/entities.py` & `extr-0.0.8/src/extr/entities/extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, cast
 
-from .regex import RegExLabel
-from .iterutils import flatten
-from .models import Location, Entity, EntityAnnotationResults
+from ..regexes import RegExLabel
+from ..iterutils import flatten
+from ..models import Location, Entity
 
 
 class EntityExtractor:
     def __init__(self, regex_labels: List[RegExLabel]) -> None:
         self._regex_labels = regex_labels
 
     def get_entities(self, text: str) -> List[Entity]:
@@ -32,19 +32,7 @@
 
             if curr_entity.is_in(prev_entity):
                 continue
 
             entities.append(curr_entity)
 
         return entities
-
-class EntityAnnotator:
-    def annotate(self, text: str, entities: List[Entity]) -> EntityAnnotationResults:
-        def insert_entity(text: str, entity: Entity) -> str:
-            return text[:entity.start] + str(entity) + text[entity.end:]
-
-        annotated_text = text[:]
-        for identifer, entity in enumerate(entities):
-            entity.identifier = identifer + 1
-            annotated_text = insert_entity(annotated_text, entity)
-
-        return EntityAnnotationResults(text, annotated_text, entities)
```

### Comparing `extr-0.0.7/src/extr/models.py` & `extr-0.0.8/src/extr/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Any, TypeVar
+from typing import Any, Dict, List, TypeVar
 
 from dataclasses import dataclass, field
 
 
 NOT_DEFINED_FLAG: int = -1
 
 # pylint: disable=C0103
@@ -77,7 +77,32 @@
 class Relation:
     label: str
     e1: Entity
     e2: Entity
 
     def __repr__(self) -> str:
         return f'<Relation e1="{self.e1.text}" r="{self.label}" e2="{self.e2.text}">'
+
+@dataclass(frozen=True)
+class Token(ILocation):
+    text: str
+    location: Location
+    order: int
+    entities: List[Entity] = field(default_factory=lambda: [])
+
+    def add_entity(self, entity: Entity):
+        self.entities.append(entity)
+
+    def __len__(self) -> int:
+        return len(self.entities)
+
+    def __str__(self) -> str:
+        return self.text
+
+    def __repr__(self) -> str:
+        return f'<Token text="{self.text}", location={repr(self.location)}, order={self.order}>'
+
+@dataclass(frozen=True)
+class TokenGroup(ILocation):
+    location: Location
+    sentence: str
+    tokens: List[Token]
```

### Comparing `extr-0.0.7/src/extr/relations.py` & `extr-0.0.8/src/extr/relations/extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Generator, cast
 
 import re
-from .regex import RegExLabel
-from .entities import EntityAnnotationResults
-from .iterutils import flatten
-from .models import Relation
+from ..regexes import RegExLabel
+from ..models import EntityAnnotationResults, Relation
+from ..iterutils import flatten
 
 
 class RelationExtractor:
     def __init__(self, relation_labels: List[RegExLabel]) -> None:
         self._relation_labels = relation_labels
 
     def extract(self, entity_annotation_results: EntityAnnotationResults) -> List[Relation]:
```

### Comparing `extr-0.0.7/src/extr.egg-info/PKG-INFO` & `extr-0.0.8/src/extr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
 Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
@@ -21,15 +21,16 @@
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtractor
+        from extr import RegEx, RegExLabel
+        from extr.entities import EntityExtractor
         
         entity_extractor = EntityExtractor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -44,16 +45,17 @@
         ## ]
         ```
         
         ### 2. Relation Extraction
         > Annotate and Extract Relationships between Entities
         
         ```python
-        from extr import EntityAnnotator
-        from extr import RegExRelationLabelBuilder, RelationExtractor
+        from extr.entities import EntityAnnotator
+        from extr.relations import RelationExtractor, \
+                                   RegExRelationLabelBuilder
         
         ## define relationship between PERSON and POSITION
         relationship = RegExRelationLabelBuilder('is_a') \
             .add_e1_to_e2(
                 'PERSON', ## e1
                 [
                     ## define how the relationship exists in nature
```

