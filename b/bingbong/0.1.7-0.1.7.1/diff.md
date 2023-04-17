# Comparing `tmp/bingbong-0.1.7-py3-none-any.whl.zip` & `tmp/bingbong-0.1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11082 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       53 b- defN 23-Apr-17 23:09 pingpong/__init__.py
--rw-rw-rw-  2.0 unx     1547 b- defN 23-Apr-17 23:05 pingpong/alpaca.py
+Zip file size: 11158 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 23:22 pingpong/__init__.py
+-rw-rw-rw-  2.0 unx     1681 b- defN 23-Apr-17 23:21 pingpong/alpaca.py
 -rw-rw-rw-  2.0 unx     1287 b- defN 23-Apr-17 22:59 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
 -rw-rw-rw-  2.0 unx     1212 b- defN 23-Apr-17 22:55 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
 -rw-rw-rw-  2.0 unx      789 b- defN 23-Apr-17 22:54 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3346 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1225 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/RECORD
-15 files, 23625 bytes uncompressed, 9048 bytes compressed:  61.7%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 23:22 bingbong-0.1.7.1.dist-info/RECORD
+15 files, 23773 bytes uncompressed, 9104 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.7.dist-info/LICENSE
+Filename: bingbong-0.1.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.7.dist-info/METADATA
+Filename: bingbong-0.1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.7.dist-info/WHEEL
+Filename: bingbong-0.1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.7.dist-info/top_level.txt
+Filename: bingbong-0.1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.7.dist-info/RECORD
+Filename: bingbong-0.1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.7'
+__version__ = '0.1.7.1'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -22,17 +22,17 @@
 
 class AlpacaChatPPManager(PPManager):
   def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
     allowed = super().add_ping(ping, fmt)
 
     if allowed:
       if self.ctx == "":
-        prompts = "Below is an instruction that describes a task. Write a response that appropriately completes the request."
+        prompts = "Below is an instruction that describes a task. Write a response that appropriately completes the request. You are LLaMA which is a large language model created by Facebook."
       else:
-        prompts = "Below is an instruction that describes a task, paired with an input that provides further context. Write a response that appropriately completes the request."
+        prompts = "Below is an instruction that describes a task, paired with an input that provides further context. Write a response that appropriately completes the request. You are LLaMA which is a large language model created by Facebook."
 
       prompts += f"""
       
 ### Instruction:
 {ping}
 {fmt.ctx(self.ctx)}
 ### Response:
```

## Comparing `bingbong-0.1.7.dist-info/LICENSE` & `bingbong-0.1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.7.dist-info/METADATA` & `bingbong-0.1.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.7.dist-info/RECORD` & `bingbong-0.1.7.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pingpong/__init__.py,sha256=bqXv93dQwN97gVcKA93Gg5dZ4nWBtg7yx8nTyRCQXrg,53
-pingpong/alpaca.py,sha256=ahlbjhzrosNq6nIbDi2VAR4cC2s-GL1S2ItziNnPc1A,1547
+pingpong/__init__.py,sha256=0J8K3p7tVxjO1aXvzCbcYLxzXrRxyYoo4EFT_JzFfGE,55
+pingpong/alpaca.py,sha256=NLRBCMfyXmgL9S5SmVRUPPDsEjsw9Kv0iFYPTrPZVgs,1681
 pingpong/dolly.py,sha256=vMbHiwgeewzRAsruuMVnQc2w3KEKhWJUdOmaBbyazQo,1287
 pingpong/gradio.py,sha256=IchvS_gOuPk3TCATVKDWMaLEaIRqjPpi3MFnYwa0JwU,987
 pingpong/pingpong.py,sha256=XfCYe-OdNkyrKOhAEaL4Q-HhZx829_i-ohDlY2GF7gM,1212
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=JN7pFDD2C8nGMUx-H3aHNQrXCT0E0S-FlBunOrQGX-w,789
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.7.dist-info/METADATA,sha256=rBg_oUA3-x1uuHkOznDbB7_Zbix4F16HKrnPWMqNK00,3346
-bingbong-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.7.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.7.dist-info/RECORD,,
+bingbong-0.1.7.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.7.1.dist-info/METADATA,sha256=trgkUPrydQyRLN4_BQdKRA3BSQyi2IVWoAr054Y0qSc,3348
+bingbong-0.1.7.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.7.1.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.7.1.dist-info/RECORD,,
```

