# Comparing `tmp/spacy_chapas-0.9.1-py3-none-any.whl.zip` & `tmp/spacy_chapas-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13787 bytes, number of entries: 10
+Zip file size: 13827 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       83 b- defN 20-Oct-17 14:49 spacy_chapas/__init__.py
--rw-r--r--  2.0 unx     6778 b- defN 22-Apr-24 15:03 spacy_chapas/chapas.py
+-rw-r--r--  2.0 unx     6815 b- defN 23-Apr-17 23:45 spacy_chapas/chapas.py
 -rwxr-xr-x  2.0 unx     7708 b- defN 21-Jan-09 07:47 spacy_chapas/chapas2ud
 -rwxr-xr-x  2.0 unx     3976 b- defN 21-Jan-01 04:37 spacy_chapas/unidic2ipadic
--rwxr-xr-x  2.0 unx     7708 b- defN 21-Jan-09 07:47 spacy_chapas-0.9.1.data/data/bin/chapas2ud
--rw-r--r--  2.0 unx     1071 b- defN 22-Apr-24 15:40 spacy_chapas-0.9.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8625 b- defN 22-Apr-24 15:40 spacy_chapas-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-24 15:40 spacy_chapas-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Apr-24 15:40 spacy_chapas-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      834 b- defN 22-Apr-24 15:40 spacy_chapas-0.9.1.dist-info/RECORD
-10 files, 36888 bytes uncompressed, 12357 bytes compressed:  66.5%
+-rwxr-xr-x  2.0 unx     7708 b- defN 21-Jan-09 07:47 spacy_chapas-0.9.2.data/data/bin/chapas2ud
+-rw-r--r--  2.0 unx     1071 b- defN 23-Apr-17 23:46 spacy_chapas-0.9.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8745 b- defN 23-Apr-17 23:46 spacy_chapas-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 23:46 spacy_chapas-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-17 23:46 spacy_chapas-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      834 b- defN 23-Apr-17 23:46 spacy_chapas-0.9.2.dist-info/RECORD
+10 files, 37045 bytes uncompressed, 12397 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: spacy_chapas/chapas2ud
 Comment: 
 
 Filename: spacy_chapas/unidic2ipadic
 Comment: 
 
-Filename: spacy_chapas-0.9.1.data/data/bin/chapas2ud
+Filename: spacy_chapas-0.9.2.data/data/bin/chapas2ud
 Comment: 
 
-Filename: spacy_chapas-0.9.1.dist-info/LICENSE.txt
+Filename: spacy_chapas-0.9.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: spacy_chapas-0.9.1.dist-info/METADATA
+Filename: spacy_chapas-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: spacy_chapas-0.9.1.dist-info/WHEEL
+Filename: spacy_chapas-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: spacy_chapas-0.9.1.dist-info/top_level.txt
+Filename: spacy_chapas-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spacy_chapas-0.9.1.dist-info/RECORD
+Filename: spacy_chapas-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spacy_chapas/chapas.py

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
-      d={ "spoken":"unidic-spoken", "qkana":"60b_qkana", "kindai":"60a_kindai-bungo", "kinsei":"50c_kinsei-edo", "kyogen":"40_chusei-kougo", "wakan":"30_chusei-bungo", "wabun":"20_chuko", "manyo":"10_jodai" }
+      d={ "spoken":"unidic-spoken", "novel":"65_novel", "qkana":"60b_qkana", "kindai":"60a_kindai-bungo", "kinsei":"50c_kinsei-edo", "kyogen":"40_chusei-kougo", "wakan":"30_chusei-bungo", "wabun":"20_chuko", "manyo":"10_jodai" }
       self.dictvalue=d[UniDic] if UniDic in d else UniDic
       self.model=self.ChamameWeb2ChaPASUD
       try:
         import unidic2ud
         if os.path.isdir(os.path.join(unidic2ud.DOWNLOAD_DIR,UniDic)):
           self.mecab=unidic2ud.load(UniDic,None).mecab
           self.model=self.UniDic2ChaPASUD
```

## Comparing `spacy_chapas-0.9.1.data/data/bin/chapas2ud` & `spacy_chapas-0.9.2.data/data/bin/chapas2ud`

 * *Files identical despite different names*

## Comparing `spacy_chapas-0.9.1.dist-info/LICENSE.txt` & `spacy_chapas-0.9.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `spacy_chapas-0.9.1.dist-info/METADATA` & `spacy_chapas-0.9.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-chapas
-Version: 0.9.1
+Version: 0.9.2
 Summary: ChaPAS-CaboCha-MeCab wrapper for spaCy
 Home-page: https://github.com/KoichiYasuoka/spaCy-ChaPAS
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: ChaPAS, https://sites.google.com/site/yotarow/chapas
 Project-URL: CaboCha, https://taku910.github.io/cabocha/
@@ -80,14 +80,15 @@
 次郎に -> 渡した (斜格補語)
 ```
 
 `spacy_chapas.load(UniDic)` loads spaCy Language pipeline for ChaPAS-CaboCha-MeCab. Available `UniDic` options are:
 
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

## Comparing `spacy_chapas-0.9.1.dist-info/RECORD` & `spacy_chapas-0.9.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spacy_chapas/__init__.py,sha256=LYtxHdIiHxXUWumpwZwAj1T5GD5xB_yIF_Fa7-vwWa4,83
-spacy_chapas/chapas.py,sha256=-DeB6Z5ZiKGr6pMkfNGOuSLbyS8naHnEiCe9A-G1e4g,6778
+spacy_chapas/chapas.py,sha256=1bEJi4ozpaiwPp4p-_wfWHwBevvFX4zxdzPF_LJuXnA,6815
 spacy_chapas/chapas2ud,sha256=7EpxBaJCgfjeohjQTRaq0cmkdrPnAT6i1db_K1h9Pts,7708
 spacy_chapas/unidic2ipadic,sha256=3S7GfPpjI2-53K8q9lGUqVXR4wYiwsaGTnE0694V6ps,3976
-spacy_chapas-0.9.1.data/data/bin/chapas2ud,sha256=7EpxBaJCgfjeohjQTRaq0cmkdrPnAT6i1db_K1h9Pts,7708
-spacy_chapas-0.9.1.dist-info/LICENSE.txt,sha256=CggQrBg6lOnsxk5fbwerDPop26rAOqIGJ2W8tXxXQKw,1071
-spacy_chapas-0.9.1.dist-info/METADATA,sha256=-nM5gQA9unfT7-gFCGhpA-lC3hyDIhAfHsy98wimGPc,8625
-spacy_chapas-0.9.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-spacy_chapas-0.9.1.dist-info/top_level.txt,sha256=uzwlFrX5hUgmxCctrKkNKvsvrvLjovEpF91iIJrNtJ8,13
-spacy_chapas-0.9.1.dist-info/RECORD,,
+spacy_chapas-0.9.2.data/data/bin/chapas2ud,sha256=7EpxBaJCgfjeohjQTRaq0cmkdrPnAT6i1db_K1h9Pts,7708
+spacy_chapas-0.9.2.dist-info/LICENSE.txt,sha256=CggQrBg6lOnsxk5fbwerDPop26rAOqIGJ2W8tXxXQKw,1071
+spacy_chapas-0.9.2.dist-info/METADATA,sha256=Atr6DL0Vm3VLsLNNT7Do6CridkNrzbebOFqM0avjIGM,8745
+spacy_chapas-0.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+spacy_chapas-0.9.2.dist-info/top_level.txt,sha256=uzwlFrX5hUgmxCctrKkNKvsvrvLjovEpF91iIJrNtJ8,13
+spacy_chapas-0.9.2.dist-info/RECORD,,
```

