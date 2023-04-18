# Comparing `tmp/unidic_combo-1.4.0-py3-none-any.whl.zip` & `tmp/unidic_combo-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 72211 bytes, number of entries: 45
+Zip file size: 72233 bytes, number of entries: 45
 -rw-r--r--  2.0 unx      126 b- defN 21-Jan-21 01:54 unidic_combo/__init__.py
 -rw-r--r--  2.0 unx    15539 b- defN 21-Jan-03 00:24 unidic_combo/config.template.jsonnet
 -rw-r--r--  2.0 unx     9852 b- defN 21-Jan-21 03:28 unidic_combo/main.py
 -rw-r--r--  2.0 unx    11255 b- defN 21-Jan-24 03:31 unidic_combo/predict.py
 -rw-r--r--  2.0 unx     4742 b- defN 21-Feb-18 12:16 unidic_combo/unidic_combo.py
 -rw-r--r--  2.0 unx       79 b- defN 21-Jan-21 02:13 unidic_combo/commands/__init__.py
 -rw-r--r--  2.0 unx     9186 b- defN 21-Jan-21 02:13 unidic_combo/commands/train.py
@@ -35,13 +35,13 @@
 -rw-r--r--  2.0 unx     3257 b- defN 21-Jan-28 04:49 unidic_combo/training/tensorboard_writer.py
 -rw-r--r--  2.0 unx    13786 b- defN 21-Mar-28 12:17 unidic_combo/training/trainer.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Jan-21 02:13 unidic_combo/utils/__init__.py
 -rw-r--r--  2.0 unx      786 b- defN 21-Jan-21 02:13 unidic_combo/utils/checks.py
 -rw-r--r--  2.0 unx     2235 b- defN 21-Jan-21 02:13 unidic_combo/utils/download.py
 -rw-r--r--  2.0 unx     4619 b- defN 21-Jan-21 02:13 unidic_combo/utils/graph.py
 -rw-r--r--  2.0 unx    13278 b- defN 21-Jan-21 02:13 unidic_combo/utils/metrics.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Jun-16 15:46 unidic_combo-1.4.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     7327 b- defN 22-Jun-16 15:46 unidic_combo-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-16 15:46 unidic_combo-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 22-Jun-16 15:46 unidic_combo-1.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4052 b- defN 22-Jun-16 15:46 unidic_combo-1.4.0.dist-info/RECORD
-45 files, 225962 bytes uncompressed, 65657 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-18 00:09 unidic_combo-1.4.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     7447 b- defN 23-Apr-18 00:09 unidic_combo-1.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 00:09 unidic_combo-1.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-18 00:09 unidic_combo-1.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4052 b- defN 23-Apr-18 00:09 unidic_combo-1.4.1.dist-info/RECORD
+45 files, 226082 bytes uncompressed, 65679 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -114,23 +114,23 @@
 
 Filename: unidic_combo/utils/graph.py
 Comment: 
 
 Filename: unidic_combo/utils/metrics.py
 Comment: 
 
-Filename: unidic_combo-1.4.0.dist-info/LICENSE.txt
+Filename: unidic_combo-1.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: unidic_combo-1.4.0.dist-info/METADATA
+Filename: unidic_combo-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: unidic_combo-1.4.0.dist-info/WHEEL
+Filename: unidic_combo-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: unidic_combo-1.4.0.dist-info/top_level.txt
+Filename: unidic_combo-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: unidic_combo-1.4.0.dist-info/RECORD
+Filename: unidic_combo-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `unidic_combo-1.4.0.dist-info/LICENSE.txt` & `unidic_combo-1.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `unidic_combo-1.4.0.dist-info/METADATA` & `unidic_combo-1.4.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidic-combo
-Version: 1.4.0
+Version: 1.4.1
 Summary: UniDic2UD + COMBO-pytorch wrapper for spaCy
 Home-page: https://github.com/KoichiYasuoka/UniDic-COMBO
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: GPL
 Project-URL: COMBO-pytorch, https://gitlab.clarin-pl.eu/syntactic-tools/combo
 Project-URL: Source, https://github.com/KoichiYasuoka/UniDic-COMBO
@@ -27,15 +27,15 @@
 Requires-Dist: ipadic (>=1.0.0)
 Requires-Dist: overrides (<5,>=3.1.0)
 Requires-Dist: protobuf (>=3.14.0)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: spacy (>=2.2.2)
 Requires-Dist: torch (>=1.6.0)
 Requires-Dist: unidic-lite (>=1.0.8)
-Requires-Dist: unidic2ud (>=2.9.6)
+Requires-Dist: unidic2ud (>=2.9.9)
 
 [![Current PyPI packages](https://badge.fury.io/py/unidic-combo.svg)](https://pypi.org/project/unidic-combo/)
 
 # UniDic-COMBO
 
 [UniDic2UD](https://github.com/KoichiYasuoka/UniDic2UD) + [COMBO-pytorch](https://gitlab.clarin-pl.eu/syntactic-tools/combo) wrapper for [spaCy](https://spacy.io)
 
@@ -82,14 +82,15 @@
 一疋も -> 見えぬ (斜格補語)
 ```
 
 `unidic_combo.load(UniDic,BERT=True)` loads spaCy Language pipeline for UniDic2UD + COMBO-pytorch. Available `UniDic` options are:
 
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

## Comparing `unidic_combo-1.4.0.dist-info/RECORD` & `unidic_combo-1.4.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -34,12 +34,12 @@
 unidic_combo/training/tensorboard_writer.py,sha256=ayUXPB1SXOmouLlnRcesDcfde5sQshWLIDn773wyVhM,3257
 unidic_combo/training/trainer.py,sha256=Y8ZM8W0xzJRlvmhWDpMKISILjX7cTxXbnyqvY1nc1CE,13786
 unidic_combo/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unidic_combo/utils/checks.py,sha256=ddhk3oeZtyFb3ujBdWU2wODPoHiH2a2NTnTllgYolmI,786
 unidic_combo/utils/download.py,sha256=BuM0cJtDh7DOv0kR5K7SVZY0O8FdOsQJ9IN6mkXCFm0,2235
 unidic_combo/utils/graph.py,sha256=zPx-LXGapnkx0rneHwgKYbIhLSnBbMTwGf6LwCNJRR0,4619
 unidic_combo/utils/metrics.py,sha256=BOA8SijrZVdAx4QJ2HL9HPsGcMv3GqhPh0btoLMOAaw,13278
-unidic_combo-1.4.0.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-unidic_combo-1.4.0.dist-info/METADATA,sha256=pMbewQ6ZlR2mUJ5mFmdYkX1oXUcufMQe_L-XeQinLOw,7327
-unidic_combo-1.4.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-unidic_combo-1.4.0.dist-info/top_level.txt,sha256=tieqixOsaBMJpNTB5u4KONLIAqgdWYoafUc5AYpCbcc,13
-unidic_combo-1.4.0.dist-info/RECORD,,
+unidic_combo-1.4.1.dist-info/LICENSE.txt,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+unidic_combo-1.4.1.dist-info/METADATA,sha256=JlMcfd5Zm33X-wtSPbxm4PMJMlOMcvhycbmACUzB2TM,7447
+unidic_combo-1.4.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+unidic_combo-1.4.1.dist-info/top_level.txt,sha256=tieqixOsaBMJpNTB5u4KONLIAqgdWYoafUc5AYpCbcc,13
+unidic_combo-1.4.1.dist-info/RECORD,,
```

