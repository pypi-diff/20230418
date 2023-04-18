# Comparing `tmp/TransLiter-0.2.4.tar.gz` & `tmp/TransLiter-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TransLiter-0.2.4.tar", last modified: Fri Apr 14 18:42:38 2023, max compression
+gzip compressed data, was "TransLiter-0.2.5.tar", last modified: Tue Apr 18 18:16:02 2023, max compression
```

## Comparing `TransLiter-0.2.4.tar` & `TransLiter-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.866818 TransLiter-0.2.4/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.2.4/LICENSE
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4438 2023-04-14 18:42:38.866702 TransLiter-0.2.4/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4088 2023-04-13 18:14:28.000000 TransLiter-0.2.4/README.md
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.865837 TransLiter-0.2.4/TransLiter/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      110 2023-04-12 17:26:39.000000 TransLiter-0.2.4/TransLiter/__init__.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     3374 2023-04-12 19:11:15.000000 TransLiter-0.2.4/TransLiter/jp_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1116 2023-04-12 00:32:24.000000 TransLiter-0.2.4/TransLiter/ko_jamo.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-04-12 17:31:03.000000 TransLiter-0.2.4/TransLiter/spacing.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2082 2023-04-14 18:40:59.000000 TransLiter-0.2.4/TransLiter/transliter_jp.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2382 2023-04-14 18:31:29.000000 TransLiter-0.2.4/TransLiter/transliter_ko.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.866510 TransLiter-0.2.4/TransLiter.egg-info/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4438 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      373 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/SOURCES.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/dependency_links.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/not-zip-safe
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/requires.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/top_level.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-14 18:42:38.866855 TransLiter-0.2.4/setup.cfg
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      647 2023-04-14 04:08:10.000000 TransLiter-0.2.4/setup.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-18 18:16:02.399041 TransLiter-0.2.5/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.2.5/LICENSE
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4451 2023-04-18 18:16:02.398933 TransLiter-0.2.5/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4101 2023-04-18 17:41:29.000000 TransLiter-0.2.5/README.md
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-18 18:16:02.398116 TransLiter-0.2.5/TransLiter/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      110 2023-04-12 17:26:39.000000 TransLiter-0.2.5/TransLiter/__init__.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3414 2023-04-18 18:13:28.000000 TransLiter-0.2.5/TransLiter/jp_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1832 2023-04-18 17:11:04.000000 TransLiter-0.2.5/TransLiter/ko_jamo.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-04-12 17:31:03.000000 TransLiter-0.2.5/TransLiter/spacing.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1920 2023-04-18 18:14:28.000000 TransLiter-0.2.5/TransLiter/transliter_jp.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2990 2023-04-18 17:40:57.000000 TransLiter-0.2.5/TransLiter/transliter_ko.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-18 18:16:02.398775 TransLiter-0.2.5/TransLiter.egg-info/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4451 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      373 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/not-zip-safe
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/requires.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-18 18:16:02.000000 TransLiter-0.2.5/TransLiter.egg-info/top_level.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-18 18:16:02.399078 TransLiter-0.2.5/setup.cfg
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      647 2023-04-18 17:37:02.000000 TransLiter-0.2.5/setup.py
```

### Comparing `TransLiter-0.2.4/LICENSE` & `TransLiter-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TransLiter-0.2.4/PKG-INFO` & `TransLiter-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.2.4
+Version: 0.2.5
 Summary: TransLiter transliterates multilingual text into English.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -41,63 +41,63 @@
 
 ## 1. Korean
 
 ### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
-annyeohaseyo. narssiga johneyo!
+'annyeonghaseyo. nalssiga jotneyo!'
 ```
 
 If you want to use the transliteration function several times in a row:
 
 ```
 > tl.transliter_ko()
 
 > Please enter Korean text: 안녕하세요. 날씨가 좋네요!
-annyeohaseyo. narssiga johneyo!
+annyeonghaseyo. nalssiga jotneyo!
 
 > Please enter Korean text: 우리나라 만세!
 urinara manse!
 ```
 
 To exit TransLiter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
 The output is saved as `output_ko.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
-annyeohaseyo.
+annyeonghaseyo.
 오늘 날씨 좋네요!
-oneur narssi johneyo!
+oneul nalssi jotneyo!
 행복한 하루 되세요.
-haeboghan haru doeseyo.
+haengbokhan haru doeseyo.
 저는 독서가 취미입니다.
-jeoneun dogseoga chwimiibnida.
+jeoneun dokseoga chwimiibnida.
 하루하루 재미있게 살아요.
-haruharu jaemiissge sarayo.
-가족들과 저녁을 먹어요.gajogdeurgwa jeonyeogeur meogeoyo.
+haruharu jaemiitge salayo.
+가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
 The output is saved as `output_ko.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
-0          안녕하세요.                       annyeohaseyo.
-1      오늘 날씨 좋네요!               oneur narssi johneyo!
-2     행복한 하루 되세요.             haeboghan haru doeseyo.
-3   저는 독서가 취미입니다.      jeoneun dogseoga chwimiibnida.
-4  하루하루 재미있게 살아요.         haruharu jaemiissge sarayo.
-5   가족들과 저녁을 먹어요.  gajogdeurgwa jeonyeogeur meogeoyo.
+0          안녕하세요.                     annyeonghaseyo.
+1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
+2     행복한 하루 되세요.           haengbokhan haru doeseyo.
+3   저는 독서가 취미입니다.      jeoneun dokseoga chwimiibnida.
+4  하루하루 재미있게 살아요.          haruharu jaemiitge salayo.
+5   가족들과 저녁을 먹어요.  gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ## 2. Japanese
 
 ### 2-1. Simple functions
 
 ```
@@ -142,33 +142,33 @@
 ```
 
 ### 2-3. File Export (txt -> csv)
 
 The output is saved as `output_jp.csv` in your current directory.
 
 ```
->>> tl.csv_jp("test_jp.txt")
+> tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
 3      おねがいします。         onegaishimasu。
 4    気をつけてください。    kiwotsuketekudasai。
 5   それはいい考えですね。  sorehaiikangaedesune。
 ```
 
 ## 3. Spacing
 
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
-> spacing("良 い ニ ュ ー ス で す。")
+> tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
 If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
 
 ```
-> spacing_file("test.txt")
+> tl.spacing_file("test.txt")
 ```
```

### Comparing `TransLiter-0.2.4/README.md` & `TransLiter-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,63 +28,63 @@
 
 ## 1. Korean
 
 ### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
-annyeohaseyo. narssiga johneyo!
+'annyeonghaseyo. nalssiga jotneyo!'
 ```
 
 If you want to use the transliteration function several times in a row:
 
 ```
 > tl.transliter_ko()
 
 > Please enter Korean text: 안녕하세요. 날씨가 좋네요!
-annyeohaseyo. narssiga johneyo!
+annyeonghaseyo. nalssiga jotneyo!
 
 > Please enter Korean text: 우리나라 만세!
 urinara manse!
 ```
 
 To exit TransLiter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
 The output is saved as `output_ko.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
-annyeohaseyo.
+annyeonghaseyo.
 오늘 날씨 좋네요!
-oneur narssi johneyo!
+oneul nalssi jotneyo!
 행복한 하루 되세요.
-haeboghan haru doeseyo.
+haengbokhan haru doeseyo.
 저는 독서가 취미입니다.
-jeoneun dogseoga chwimiibnida.
+jeoneun dokseoga chwimiibnida.
 하루하루 재미있게 살아요.
-haruharu jaemiissge sarayo.
-가족들과 저녁을 먹어요.gajogdeurgwa jeonyeogeur meogeoyo.
+haruharu jaemiitge salayo.
+가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
 The output is saved as `output_ko.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
-0          안녕하세요.                       annyeohaseyo.
-1      오늘 날씨 좋네요!               oneur narssi johneyo!
-2     행복한 하루 되세요.             haeboghan haru doeseyo.
-3   저는 독서가 취미입니다.      jeoneun dogseoga chwimiibnida.
-4  하루하루 재미있게 살아요.         haruharu jaemiissge sarayo.
-5   가족들과 저녁을 먹어요.  gajogdeurgwa jeonyeogeur meogeoyo.
+0          안녕하세요.                     annyeonghaseyo.
+1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
+2     행복한 하루 되세요.           haengbokhan haru doeseyo.
+3   저는 독서가 취미입니다.      jeoneun dokseoga chwimiibnida.
+4  하루하루 재미있게 살아요.          haruharu jaemiitge salayo.
+5   가족들과 저녁을 먹어요.  gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ## 2. Japanese
 
 ### 2-1. Simple functions
 
 ```
@@ -129,31 +129,31 @@
 ```
 
 ### 2-3. File Export (txt -> csv)
 
 The output is saved as `output_jp.csv` in your current directory.
 
 ```
->>> tl.csv_jp("test_jp.txt")
+> tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
 3      おねがいします。         onegaishimasu。
 4    気をつけてください。    kiwotsuketekudasai。
 5   それはいい考えですね。  sorehaiikangaedesune。
 ```
 
 ## 3. Spacing
 
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
-> spacing("良 い ニ ュ ー ス で す。")
+> tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
 If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
 
 ```
-> spacing_file("test.txt")
+> tl.spacing_file("test.txt")
 ```
```

### Comparing `TransLiter-0.2.4/TransLiter/jp_list.py` & `TransLiter-0.2.5/TransLiter/jp_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "ひゃ": "hya", "ひゅ": "hyu", "ひょ": "hyo",
     "みゃ": "mya", "みゅ": "myu", "みょ": "myo",
     "りゃ": "rya", "りゅ": "ryu", "りょ": "ryo",
     "ぎゃ": "gya", "ぎゅ": "gyu", "ぎょ": "gyo",
     "じゃ": "ja", "じゅ": "ju", "じょ": "jo",
     "ぢゃ": "ja", "ぢゅ": "ju", "ぢょ": "jo",
     "びゃ": "bya", "びゅ": "byu", "びょ": "byo",
-    "ぴゃ": "pya", "ぴゅ": "pyu", "ぴょ": "pyo"
+    "ぴゃ": "pya", "ぴゅ": "pyu", "ぴょ": "pyo", "っ": "k", "ッ": "t"
 }
 
 katakana_to_english = {
         "ア": "a", "イ": "i", "ウ": "u", "エ": "e", "オ": "o",
         "カ": "ka", "キ": "ki", "ク": "ku", "ケ": "ke", "コ": "ko",
         "サ": "sa", "シ": "shi", "ス": "su", "セ": "se", "ソ": "so",
         "タ": "ta", "チ": "chi", "ツ": "tsu", "テ": "te", "ト": "to",
@@ -44,15 +44,15 @@
         "ダ": "da", "ヂ": "ji", "ヅ": "zu", "デ": "de", "ド": "do",
         "バ": "ba", "ビ": "bi", "ブ": "bu", "ベ": "be", "ボ": "bo",
         "パ": "pa", "ピ": "pi", "プ": "pu", "ペ": "pe", "ポ": "po",
         "キャ": "kya", "キュ": "kyu", "キョ": "kyo",
         "シャ": "sha", "シュ": "shu", "ショ": "sho",
         "チャ": "cha", "チュ": "chu", "チョ": "cho",
         "ニャ": "nya", "ニュ": "nyu", "ニョ": "nyo",
-        "ヒャ": "hya", "ヒュ": "hyu", "ヒョ": "hyo",
+        "ヒャ": "hya", "ヒュ": "hyu", "ヒョ": "hyo", "フォ": "fo",
         "ミャ": "mya", "ミュ": "myu", "ミョ": "myo",
         "リャ": "rya", "リュ": "ryu", "リョ": "ryo",
         "ギャ": "gya", "ギュ": "gyu", "ギョ": "gyo",
         "ジャ": "ja", "ジュ": "ju", "ジョ": "jo",
         "ビャ": "bya", "ビュ": "byu", "ビョ": "byo",
         "ピャ": "pya", "ピュ": "pyu", "ピョ": "pyo"
     }
```

### Comparing `TransLiter-0.2.4/TransLiter/transliter_jp.py` & `TransLiter-0.2.5/TransLiter/transliter_jp.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 def jp(text):
     text = kanji_to_hiragana(text)
     hiragana_to_english.update(katakana_to_english)
     transliterated_text = ""
     i = 0
     while i < len(text):
         try:
-            if i < len(text) - 1 and text[i+1] in ['ッ', 'っ']:
-                transliterated_text += hiragana_to_english[text[i]][0]
-                i += 1
-            elif i < len(text) - 1 and text[i+1] in ['ゃ', 'ゅ', 'ょ']:
+            if i < len(text) - 1 and text[i+1] in ['ゃ', 'ゅ', 'ょ']:
                 transliterated_text += hiragana_to_english[text[i]+text[i+1]]
                 i += 1
             else:
                 transliterated_text += hiragana_to_english.get(text[i], text[i])
         except KeyError:
             pass
         i += 1
```

### Comparing `TransLiter-0.2.4/TransLiter/transliter_ko.py` & `TransLiter-0.2.5/TransLiter/transliter_ko.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,27 +19,39 @@
                 jamo_result.append(JONGSUNG_LIST[char3])
         else:
             jamo_result.append(keyword)
     return "".join(jamo_result)
 
 def ko(text):
     text = convert(text)
-    syllables = list(text)
-    transliterated_syllables = []
-    for syllable in syllables:
-        transliterated_syllable = ''
-        for letter in syllable:
-            if letter in KOREAN_ALPHABET:
-                transliterated_syllable += KOREAN_ALPHABET[letter]
+    letter = list(text)
+    transliterated_letters = []
+    for i in range(len(letter)-1):
+        transliterated_letter = ''
+        try:
+            if letter[i] in JONGSUNG_LIST2 and letter[i+1] in CHOSUNG_LIST2:
+                transliterated_letter += JONGSUNG_ALPHABET[letter[i]]
+            elif letter[i] in CHOSUNG_LIST or JUNGSUNG_LIST:
+                transliterated_letter += KOREAN_ALPHABET[letter[i]]
             else:
-                transliterated_syllable += letter
-        transliterated_syllables.append(transliterated_syllable)
-    transliterated_word = ''.join(transliterated_syllables)
+                transliterated_letter += letter[i]
+            transliterated_letters.append(transliterated_letter)
+        except KeyError:
+            transliterated_letter += letter[i]
+            transliterated_letters.append(transliterated_letter)
+    if len(letter) > 1:
+        if letter[-1] in JONGSUNG_LIST2:
+            transliterated_letters.append(JONGSUNG_ALPHABET[letter[-1]])
+        elif letter[-1] in JUNGSUNG_LIST:
+            transliterated_letters.append(KOREAN_ALPHABET[letter[-1]])
+        else:
+            transliterated_letters.append(letter[-1])
+    transliterated_word = ''.join(transliterated_letters)
     return transliterated_word
-
+        
 def transliter_ko():
     while True:
         input_text = input("Please enter Korean text: ")
         print(ko(input_text))
         if input_text == "": 
             break
```

### Comparing `TransLiter-0.2.4/TransLiter.egg-info/PKG-INFO` & `TransLiter-0.2.5/TransLiter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.2.4
+Version: 0.2.5
 Summary: TransLiter transliterates multilingual text into English.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -41,63 +41,63 @@
 
 ## 1. Korean
 
 ### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
-annyeohaseyo. narssiga johneyo!
+'annyeonghaseyo. nalssiga jotneyo!'
 ```
 
 If you want to use the transliteration function several times in a row:
 
 ```
 > tl.transliter_ko()
 
 > Please enter Korean text: 안녕하세요. 날씨가 좋네요!
-annyeohaseyo. narssiga johneyo!
+annyeonghaseyo. nalssiga jotneyo!
 
 > Please enter Korean text: 우리나라 만세!
 urinara manse!
 ```
 
 To exit TransLiter, please press enter without any text.
 
 ### 1-2. File Export (txt -> txt)
 
 The output is saved as `output_ko.txt` in your current directory.
 
 ```
 > tl.txt_ko("test_ko.txt")
 안녕하세요.
-annyeohaseyo.
+annyeonghaseyo.
 오늘 날씨 좋네요!
-oneur narssi johneyo!
+oneul nalssi jotneyo!
 행복한 하루 되세요.
-haeboghan haru doeseyo.
+haengbokhan haru doeseyo.
 저는 독서가 취미입니다.
-jeoneun dogseoga chwimiibnida.
+jeoneun dokseoga chwimiibnida.
 하루하루 재미있게 살아요.
-haruharu jaemiissge sarayo.
-가족들과 저녁을 먹어요.gajogdeurgwa jeonyeogeur meogeoyo.
+haruharu jaemiitge salayo.
+가족들과 저녁을 먹어요.gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ### 1-3. File Export (txt -> csv)
 
 The output is saved as `output_ko.csv` in your current directory.
 
 ```
 > tl.csv_ko("test_ko.txt")
     Original Text                 Transliterated Text
-0          안녕하세요.                       annyeohaseyo.
-1      오늘 날씨 좋네요!               oneur narssi johneyo!
-2     행복한 하루 되세요.             haeboghan haru doeseyo.
-3   저는 독서가 취미입니다.      jeoneun dogseoga chwimiibnida.
-4  하루하루 재미있게 살아요.         haruharu jaemiissge sarayo.
-5   가족들과 저녁을 먹어요.  gajogdeurgwa jeonyeogeur meogeoyo.
+0          안녕하세요.                     annyeonghaseyo.
+1      오늘 날씨 좋네요!               oneul nalssi jotneyo!
+2     행복한 하루 되세요.           haengbokhan haru doeseyo.
+3   저는 독서가 취미입니다.      jeoneun dokseoga chwimiibnida.
+4  하루하루 재미있게 살아요.          haruharu jaemiitge salayo.
+5   가족들과 저녁을 먹어요.  gajokdeulgwa jeonyeokeul meokeoyo.
 ```
 
 ## 2. Japanese
 
 ### 2-1. Simple functions
 
 ```
@@ -142,33 +142,33 @@
 ```
 
 ### 2-3. File Export (txt -> csv)
 
 The output is saved as `output_jp.csv` in your current directory.
 
 ```
->>> tl.csv_jp("test_jp.txt")
+> tl.csv_jp("test_jp.txt")
   Original Text    Transliterated Text
 0        気を付けて。           kiwotsukete。
 1     良いニュースです。         yoinyuーsudesu。
 2      おやすみなさい。          oyasuminasai。
 3      おねがいします。         onegaishimasu。
 4    気をつけてください。    kiwotsuketekudasai。
 5   それはいい考えですね。  sorehaiikangaedesune。
 ```
 
 ## 3. Spacing
 
 Some languages such as Japanese don't have spacing between words. If there is spacing between the characters or words for text in those languages, you might bump into errors. To avoid the errors, the spacing needs to be removed.
 
 ```
-> spacing("良 い ニ ュ ー ス で す。")
+> tl.spacing("良 い ニ ュ ー ス で す。")
 良いニュースです。
 ```
 
 If you want to remove all spacing from a file, use `spacing_file("filename")`. The result is saved as `spacing_removed.txt`.
 
 ```
-> spacing_file("test.txt")
+> tl.spacing_file("test.txt")
 ```
```

### Comparing `TransLiter-0.2.4/setup.py` & `TransLiter-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='TransLiter',
     python_requires='>=3.6',
-    version='0.2.4',
+    version='0.2.5',
     url='https://github.com/elibooklover/TransLiter',
     license='MIT',
     author='Hoyeol Kim',
     author_email='elibooklover@gmail.com',
     description='TransLiter transliterates multilingual text into English.',
     packages=['TransLiter', ],
     long_description=long_description,
```

