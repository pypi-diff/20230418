# Comparing `tmp/conllup-0.4.5.tar.gz` & `tmp/conllup-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conllup-0.4.5.tar", last modified: Fri Apr 14 16:26:49 2023, max compression
+gzip compressed data, was "conllup-0.4.6.tar", last modified: Tue Apr 18 13:20:14 2023, max compression
```

## Comparing `conllup-0.4.5.tar` & `conllup-0.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-14 16:26:49.305427 conllup-0.4.5/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)     3385 2023-04-14 16:24:50.000000 conllup-0.4.5/README.md
--rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.5/long_description.rst
--rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-04-14 16:23:44.000000 conllup-0.4.5/pyproject.toml
--rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-04-14 16:26:49.305427 conllup-0.4.5/setup.cfg
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/conllup/
--rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.5/src/conllup/__init__.py
--rw-rw-r--   0 wran      (1000) wran      (1000)    11695 2023-04-14 16:23:44.000000 conllup-0.4.5/src/conllup/conllup.py
--rw-rw-r--   0 wran      (1000) wran      (1000)     6803 2023-02-07 18:51:16.000000 conllup-0.4.5/src/conllup/processing.py
--rw-rw-r--   0 wran      (1000) wran      (1000)      552 2023-02-02 18:44:41.000000 conllup-0.4.5/src/conllup/types.py
-drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-14 16:26:49.305427 conllup-0.4.5/src/conllup.egg-info/
--rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/PKG-INFO
--rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/SOURCES.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/dependency_links.txt
--rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-04-14 16:26:49.000000 conllup-0.4.5/src/conllup.egg-info/top_level.txt
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.257676 conllup-0.4.6/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-18 13:20:14.257676 conllup-0.4.6/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)     3499 2023-04-18 13:19:26.000000 conllup-0.4.6/README.md
+-rw-rw-r--   0 wran      (1000) wran      (1000)       24 2023-02-01 16:20:21.000000 conllup-0.4.6/long_description.rst
+-rw-rw-r--   0 wran      (1000) wran      (1000)      246 2023-04-18 13:19:26.000000 conllup-0.4.6/pyproject.toml
+-rw-rw-r--   0 wran      (1000) wran      (1000)      482 2023-04-18 13:20:14.257676 conllup-0.4.6/setup.cfg
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.253676 conllup-0.4.6/src/
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.253676 conllup-0.4.6/src/conllup/
+-rw-rw-r--   0 wran      (1000) wran      (1000)        0 2023-01-30 16:14:25.000000 conllup-0.4.6/src/conllup/__init__.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)    12044 2023-04-18 13:10:04.000000 conllup-0.4.6/src/conllup/conllup.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)     6856 2023-04-18 13:11:48.000000 conllup-0.4.6/src/conllup/processing.py
+-rw-rw-r--   0 wran      (1000) wran      (1000)      570 2023-04-18 13:10:04.000000 conllup-0.4.6/src/conllup/types.py
+drwxrwxr-x   0 wran      (1000) wran      (1000)        0 2023-04-18 13:20:14.257676 conllup-0.4.6/src/conllup.egg-info/
+-rw-rw-r--   0 wran      (1000) wran      (1000)      335 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/PKG-INFO
+-rw-rw-r--   0 wran      (1000) wran      (1000)      289 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/SOURCES.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        1 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/dependency_links.txt
+-rw-rw-r--   0 wran      (1000) wran      (1000)        8 2023-04-18 13:20:14.000000 conllup-0.4.6/src/conllup.egg-info/top_level.txt
```

### Comparing `conllup-0.4.5/README.md` & `conllup-0.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 1. change versions in pyproject.toml
 2. build new package `python3 -m build`
 3. upload to pypi `python3 -m twine upload --repository pypi dist/*`
 4. Optional : if you want to try the testpypi version of the package `pip install --index-url https://test.pypi.org/simple/ --no-deps conllup`
 
 ## Changelog
+### 0.4.6
+- add order in place in replaceArrayOfTokens() outputted treeJson (thanks to the new _sortTokensJson())
 ### 0.4.4:
 - minor fix
 ### 0.4.3:
 - optimized for speed (reduced by half the time of loading and serializing conllus)
 ### 0.4.2:
 - add optional parameter `keepEmptyTrees` in `readConlluFile()`. If True, Empty trees in conll will be discarded (some malformed conll trees could have some empty tokens)
 ### 0.4.0:
```

### Comparing `conllup-0.4.5/src/conllup/conllup.py` & `conllup-0.4.6/src/conllup/conllup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path
 from typing import Dict, List, TypedDict, Union, Literal
 
-from .types import featuresJson_T, tokenJson_T, metaJson_T, treeJson_T, sentenceJson_T
+from .types import featuresJson_T, tokenJson_T, metaJson_T, treeJson_T, sentenceJson_T, tokensJson_T
 
 tabLabel_T = Literal[
     "ID", "FORM", "LEMMA", "UPOS", "XPOS", "FEATS", "HEAD", "DEPREL", "DEPS", "MISC"
 ]
 tabType_T = Literal["str", "int", "dict"]
 
 
@@ -250,14 +250,21 @@
 
 import functools
 
 
 def _sortTokenIndexes(tokenIndexes: List[str]) -> List[str]:
     return sorted(tokenIndexes, key=functools.cmp_to_key(_compareTokenIndexes))
 
+def _sortTokensJson(tokensJson: tokensJson_T) -> tokensJson_T:
+    sortedTokensJson: tokensJson_T = {}
+    tokenIndexes = list(tokensJson.keys())
+    sortedTokenIndexes = _sortTokenIndexes(tokenIndexes)
+    for tokenIndex in sortedTokenIndexes:
+        sortedTokensJson[tokenIndex] = tokensJson[tokenIndex]
+    return sortedTokensJson
 
 def _treeJsonToConll(treeJson: treeJson_T) -> str:
     treeConllLines: List[str] = []
     tokensJson = {**treeJson["nodesJson"], **treeJson["groupsJson"]}
     tokenIndexes = [token["ID"] for token in tokensJson.values()]
     sortedTokenIndexes = _sortTokenIndexes(tokenIndexes)
     for tokenIndex in sortedTokenIndexes:
```

### Comparing `conllup-0.4.5/src/conllup/processing.py` & `conllup-0.4.6/src/conllup/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List, Tuple, Literal
 
-from .conllup import _isGroupToken, emptyNodesOrGroupsJson, emptyNodeJson
+from .conllup import _isGroupToken, emptyNodesOrGroupsJson, emptyNodeJson, _sortTokensJson
 from .types import treeJson_T, tokenJson_T
 
 mappingSpacesAfter: List[Tuple[str, str]] = [
     ("\\s", "s"),
     ("\\\\t", "\t"),
     ("\\\\n", "\n"),
     ("\\\\v", "\v"),
@@ -159,15 +159,15 @@
     if len(oldTokensIndexes) == 1:
         if len(newTokensForms) == 0:
             replaceAction = 'DELETE_ONE_TOKEN'
         elif len(newTokensForms) == 1:
             replaceAction = 'RENAME_ONE_TOKEN'
         elif len(newTokensForms) >= 1:
             replaceAction = 'SPLIT_ONE_TOKEN_INTO_MANY'
-    print(f"replaceArrayOfTokens() : detected action = {replaceAction}")
+    # print(f"replaceArrayOfTokens() : detected action = {replaceAction}")
 
     startBefore = oldTokensIndexes[0]
     endBefore = oldTokensIndexes[-1]
     endAfter = endBefore + len(newTokensForms) - len(oldTokensIndexes)
 
     # add new tokens to new tree
     newTokenIndex = oldTokensIndexes[0]
@@ -204,9 +204,9 @@
         if newTokenJson["ID"] != '-1':
             if _isGroupToken(newTokenJson):
                 # the token is a group token
                 newGroupsJson[newTokenJson["ID"]] = newTokenJson
             else:
                 # the token is a normal token
                 newNodesJson[newTokenJson["ID"]] = newTokenJson
-    newTreeJson: treeJson_T = {"nodesJson": newNodesJson, "groupsJson": newGroupsJson}
+    newTreeJson: treeJson_T = {"nodesJson": _sortTokensJson(newNodesJson), "groupsJson": _sortTokensJson(newGroupsJson)}
     return newTreeJson
```

### Comparing `conllup-0.4.5/src/conllup/types.py` & `conllup-0.4.6/src/conllup/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     XPOS: str
     FEATS: featuresJson_T
     HEAD: int
     DEPREL: str
     DEPS: featuresJson_T
     MISC: featuresJson_T
 
-nodesJson_T = Dict[str, tokenJson_T]
-groupsJson_T = Dict[str, tokenJson_T]
+tokensJson_T = Dict[str, tokenJson_T]
+nodesJson_T = tokensJson_T
+groupsJson_T = tokensJson_T
 
 class treeJson_T(TypedDict):
     nodesJson: nodesJson_T
     groupsJson: groupsJson_T
 
 
 metaJson_T = Dict[str, str]
```

