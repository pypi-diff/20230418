# Comparing `tmp/spacy_syncha-0.9.1-py3-none-any.whl.zip` & `tmp/spacy_syncha-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14885 bytes, number of entries: 11
+Zip file size: 14926 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       83 b- defN 21-Mar-11 05:44 spacy_syncha/__init__.py
--rw-r--r--  2.0 unx     6777 b- defN 22-Apr-24 15:09 spacy_syncha/syncha.py
+-rw-r--r--  2.0 unx     6814 b- defN 23-Apr-17 23:49 spacy_syncha/syncha.py
 -rwxr-xr-x  2.0 unx     7389 b- defN 21-Jan-09 07:53 spacy_syncha/syncha2ud
 -rwxr-xr-x  2.0 unx     3976 b- defN 21-Jan-01 04:37 spacy_syncha/unidic2ipadic
--rwxr-xr-x  2.0 unx     7389 b- defN 21-Jan-09 07:53 spacy_syncha-0.9.1.data/data/bin/syncha2ud
--rwxr-xr-x  2.0 unx     3976 b- defN 21-Jan-01 04:37 spacy_syncha-0.9.1.data/data/bin/unidic2ipadic
--rw-r--r--  2.0 unx     1071 b- defN 22-Apr-24 15:51 spacy_syncha-0.9.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8487 b- defN 22-Apr-24 15:51 spacy_syncha-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-24 15:51 spacy_syncha-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Apr-24 15:51 spacy_syncha-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      937 b- defN 22-Apr-24 15:51 spacy_syncha-0.9.1.dist-info/RECORD
-11 files, 40190 bytes uncompressed, 13287 bytes compressed:  66.9%
+-rwxr-xr-x  2.0 unx     7389 b- defN 21-Jan-09 07:53 spacy_syncha-0.9.2.data/data/bin/syncha2ud
+-rwxr-xr-x  2.0 unx     3976 b- defN 21-Jan-01 04:37 spacy_syncha-0.9.2.data/data/bin/unidic2ipadic
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-17 23:51 spacy_syncha-0.9.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8607 b- defN 23-Apr-17 23:51 spacy_syncha-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 23:51 spacy_syncha-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-17 23:51 spacy_syncha-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      937 b- defN 23-Apr-17 23:51 spacy_syncha-0.9.2.dist-info/RECORD
+11 files, 40347 bytes uncompressed, 13328 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: spacy_syncha/syncha2ud
 Comment: 
 
 Filename: spacy_syncha/unidic2ipadic
 Comment: 
 
-Filename: spacy_syncha-0.9.1.data/data/bin/syncha2ud
+Filename: spacy_syncha-0.9.2.data/data/bin/syncha2ud
 Comment: 
 
-Filename: spacy_syncha-0.9.1.data/data/bin/unidic2ipadic
+Filename: spacy_syncha-0.9.2.data/data/bin/unidic2ipadic
 Comment: 
 
-Filename: spacy_syncha-0.9.1.dist-info/LICENSE.txt
+Filename: spacy_syncha-0.9.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: spacy_syncha-0.9.1.dist-info/METADATA
+Filename: spacy_syncha-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: spacy_syncha-0.9.1.dist-info/WHEEL
+Filename: spacy_syncha-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: spacy_syncha-0.9.1.dist-info/top_level.txt
+Filename: spacy_syncha-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spacy_syncha-0.9.1.dist-info/RECORD
+Filename: spacy_syncha-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spacy_syncha/syncha.py

```diff
@@ -42,17 +42,17 @@
   from_disk=lambda self,*args,**kwargs:None
   to_bytes=lambda self,*args,**kwargs:None
   from_bytes=lambda self,*args,**kwargs:None
   def __init__(self,vocab,UniDic):
     import subprocess
     self.UniDic=UniDic
     if UniDic:
-      d={ "gendai":"dic1", "spoken":"dic2", "qkana":"dic3", "kindai":"dic4", "kinsei":"dic5", "kyogen":"dic6", "wakan":"dic7", "wabun":"dic8", "manyo":"dic9" }
+      d={ "gendai":"dic1", "spoken":"dic2", "novel":"dic11", "qkana":"dic3", "kindai":"dic4", "kinsei":"dic5", "kyogen":"dic6", "wakan":"dic7", "wabun":"dic8", "manyo":"dic9" }
       self.dictkey=d[UniDic]
-      d={ "gendai":"gendai", "spoken":"unidic-spoken", "qkana":"60b_qkana", "kindai":"60a_kindai-bungo", "kinsei":"50c_kinsei-edo", "kyogen":"40_chusei-kougo", "wakan":"30_chusei-bungo", "wabun":"20_chuko", "manyo":"10_jodai" }
+      d={ "gendai":"gendai", "spoken":"unidic-spoken", "novel":"65_novel", "qkana":"60b_qkana", "kindai":"60a_kindai-bungo", "kinsei":"50c_kinsei-edo", "kyogen":"40_chusei-kougo", "wakan":"30_chusei-bungo", "wabun":"20_chuko", "manyo":"10_jodai" }
       self.dictvalue=d[UniDic]
       self.model=self.ChamameWeb2SynChaUD
       try:
         import unidic2ud
         if os.path.isdir(os.path.join(unidic2ud.DOWNLOAD_DIR,UniDic)):
           self.mecab=unidic2ud.load(UniDic,None).mecab
           self.model=self.UniDic2SynChaUD
```

## Comparing `spacy_syncha-0.9.1.data/data/bin/syncha2ud` & `spacy_syncha-0.9.2.data/data/bin/syncha2ud`

 * *Files identical despite different names*

## Comparing `spacy_syncha-0.9.1.data/data/bin/unidic2ipadic` & `spacy_syncha-0.9.2.data/data/bin/unidic2ipadic`

 * *Files identical despite different names*

## Comparing `spacy_syncha-0.9.1.dist-info/LICENSE.txt` & `spacy_syncha-0.9.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `spacy_syncha-0.9.1.dist-info/METADATA` & `spacy_syncha-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-syncha
-Version: 0.9.1
+Version: 0.9.2
 Summary: SynCha-CaboCha-MeCab wrapper for spaCy
 Home-page: https://github.com/KoichiYasuoka/spaCy-SynCha
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: SynCha, https://sites.google.com/site/ryuiida/syncha
 Project-URL: CaboCha, https://taku910.github.io/cabocha/
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Natural Language :: Japanese
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: deplacy (>=2.0.2)
+Requires-Dist: deplacy (>=2.0.5)
 Requires-Dist: spacy (>=2.2.2)
 
 [![Current PyPI packages](https://badge.fury.io/py/spacy-syncha.svg)](https://pypi.org/project/spacy-syncha/)
 
 # spaCy-SynCha
 
 SynCha-CaboCha-MeCab wrapper for spaCy
@@ -80,14 +80,15 @@
 次郎に -> 渡した (間接目的語)
 ```
 
 `spacy_syncha.load(UniDic)` loads spaCy Language pipeline for SynCha-CaboCha-MeCab. Available `UniDic` options are:
 
 * `UniDic="gendai"`: Use [現代書き言葉UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_bccwj).
 * `UniDic="spoken"`: Use [現代話し言葉UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_csj).
+* `UniDic="novel"`: Use [近現代口語小説UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_novel).
 * `UniDic="qkana"`: Use [旧仮名口語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_qkana).
 * `UniDic="kindai"`: Use [近代文語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_kindai).
 * `UniDic="kinsei"`: Use [近世江戸口語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_kinsei-edo).
 * `UniDic="kyogen"`: Use [中世口語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_chusei-kougo).
 * `UniDic="wakan"`: Use [中世文語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_chusei-bungo).
 * `UniDic="wabun"`: Use [中古和文UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_wabun).
 * `UniDic="manyo"`: Use [上代語UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_jodai).
```

## Comparing `spacy_syncha-0.9.1.dist-info/RECORD` & `spacy_syncha-0.9.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 spacy_syncha/__init__.py,sha256=XJw-ocSTmK2q0e_XVrgkwE7QP4ELPiXbOLXh3R7QC_I,83
-spacy_syncha/syncha.py,sha256=LDjWi5N51Gq3AKHcigBmG7yhLgMN-p_4Kr61-XHqXcU,6777
+spacy_syncha/syncha.py,sha256=5YaiAW0udsveatrEExW_y3c7AGbWp97ezWKf9v3pFwc,6814
 spacy_syncha/syncha2ud,sha256=Jc3VchRC_wqCYGxTvrxvWshOCbmGHiym3UQGFGnp1t0,7389
 spacy_syncha/unidic2ipadic,sha256=3S7GfPpjI2-53K8q9lGUqVXR4wYiwsaGTnE0694V6ps,3976
-spacy_syncha-0.9.1.data/data/bin/syncha2ud,sha256=Jc3VchRC_wqCYGxTvrxvWshOCbmGHiym3UQGFGnp1t0,7389
-spacy_syncha-0.9.1.data/data/bin/unidic2ipadic,sha256=3S7GfPpjI2-53K8q9lGUqVXR4wYiwsaGTnE0694V6ps,3976
-spacy_syncha-0.9.1.dist-info/LICENSE.txt,sha256=CggQrBg6lOnsxk5fbwerDPop26rAOqIGJ2W8tXxXQKw,1071
-spacy_syncha-0.9.1.dist-info/METADATA,sha256=2bcPWf62-pFwEutNPrXrAamtJtva1wqlsyFyFpzgRP4,8487
-spacy_syncha-0.9.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-spacy_syncha-0.9.1.dist-info/top_level.txt,sha256=qLezzteq4S7DevkwYK5DoMxzUxPCybrws4dRjr9raRE,13
-spacy_syncha-0.9.1.dist-info/RECORD,,
+spacy_syncha-0.9.2.data/data/bin/syncha2ud,sha256=Jc3VchRC_wqCYGxTvrxvWshOCbmGHiym3UQGFGnp1t0,7389
+spacy_syncha-0.9.2.data/data/bin/unidic2ipadic,sha256=3S7GfPpjI2-53K8q9lGUqVXR4wYiwsaGTnE0694V6ps,3976
+spacy_syncha-0.9.2.dist-info/LICENSE.txt,sha256=CggQrBg6lOnsxk5fbwerDPop26rAOqIGJ2W8tXxXQKw,1071
+spacy_syncha-0.9.2.dist-info/METADATA,sha256=umKnzn3Pb3l-1ZhOVfKJ3phnEA7cLjOLrD8YW341diw,8607
+spacy_syncha-0.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+spacy_syncha-0.9.2.dist-info/top_level.txt,sha256=qLezzteq4S7DevkwYK5DoMxzUxPCybrws4dRjr9raRE,13
+spacy_syncha-0.9.2.dist-info/RECORD,,
```

