# Comparing `tmp/ChineseNumberUtils-1.0.3.tar.gz` & `tmp/ChineseNumberUtils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lukai\Desktop\??\chinese_number_converter\dist\tmp51s3byww\ChineseNumberUtils-1.0.3.tar", last modified: Mon Jun 27 09:06:34 2022, max compression
+gzip compressed data, was "C:\Users\lukai\Downloads\chinese-number-converter\dist\.tmp-l5oguddy\ChineseNumberUtils-1.1.1.tar", last modified: Tue Apr 18 12:24:02 2023, max compression
```

## Comparing `ChineseNumberUtils-1.0.3.tar` & `ChineseNumberUtils-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/
-drwxrwxrwx   0        0        0        0 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils/
--rw-rw-rw-   0        0        0        0 2022-05-02 13:53:06.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils/__init__.py
--rw-rw-rw-   0        0        0     6355 2022-05-05 12:53:42.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils/convert.py
-drwxrwxrwx   0        0        0        0 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/
--rw-rw-rw-   0        0        0     3937 2022-06-27 09:06:33.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-27 09:06:33.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-06-27 09:06:33.000000 ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2022-05-02 14:06:09.000000 ChineseNumberUtils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3937 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3120 2022-06-27 09:06:01.000000 ChineseNumberUtils-1.0.3/README.md
--rw-rw-rw-   0        0        0       86 2022-05-02 13:54:44.000000 ChineseNumberUtils-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      763 2022-06-27 09:06:34.000000 ChineseNumberUtils-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/
+-rw-rw-rw-   0        0        0     1075 2023-04-18 11:27:06.000000 ChineseNumberUtils-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3957 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2023-04-18 12:22:29.000000 ChineseNumberUtils-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/
+drwxrwxrwx   0        0        0        0 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/
+-rw-rw-rw-   0        0        0     3957 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 11:27:06.000000 ChineseNumberUtils-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      883 2023-04-18 12:24:02.000000 ChineseNumberUtils-1.1.1/setup.cfg
```

### Comparing `ChineseNumberUtils-1.0.3/ChineseNumberUtils.egg-info/PKG-INFO` & `ChineseNumberUtils-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,112 @@
 Metadata-Version: 2.1
 Name: ChineseNumberUtils
-Version: 1.0.3
+Version: 1.1.1
 Summary: A simple converter between Chinese and arabic number
 Home-page: https://github.com/nrchan/chinese-number-converter
 Author: NR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Utilities
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chinese-number-convertor
 
-This is a simple Chinese number converter that converts between [Chinese numberals](https://en.wikipedia.org/wiki/Chinese_numerals) and [arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
+This is a simple Chinese number converter that converts between
+[Chinese numbers](https://en.wikipedia.org/wiki/Chinese_numerals) and
+[Arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
 
 ## 👍 Quickstart
 
 ```python
-from ChineseNumberUtils import convert
+from cnc import convert
 
 print(convert.chinese2number("五十七")) #57
 print(convert.number2chinese(57)) #五十七
 ```
 
 ## 👉 chinese2number(string) -> (float|int)
 
 Returns the arabic number representation of given string.
 
 ### Notes
 
-The function uses a loosely-matching logic, so the given string doesn't need to be confined to a specific pattern.
+The function uses a loosely-matching logic, so the given string doesn't need to
+be confined to a specific pattern.
 
 ```python
 print(convert.chinese2number("兩千零一十二")) #2012
 print(convert.chinese2number("二零一二")) #will also be 2012
 print(convert.chinese2number("2012")) #will be, of course, 2012
 ```
-> That being said, please still avoid ambiguous and grammartically incorrect string such as ```一兆一``` or ```一百一千億```.
+
+> That being said, please still avoid ambiguous and grammartically incorrect
+> string such as ```一兆一``` or ```一百一千億```.
 
 ### Support character
 
 Support following characters:
+
 - **Normal number**: 一...九、十、百、千
 - **Large number** till 10<sup>52</sup>-1: 萬、億...極
 - **Zero**: 零、〇
-- **Captial version** of all characters above: 壹...玖、拾、佰、仟
+- **Capital version** of all characters above: 壹...玖、拾、佰、仟
 - **Arabic number**: 1...9、0
 - **Simplified version** off all characters above: 贰、万...
-> Arabic numbers were also supported because they will sometimes be mixed with characters, like "1億5000萬".
+
+> Arabic numbers were also supported because they will sometimes be mixed with
+> characters, like "1億5000萬".
 
 ## 👉 number2chinese(int) -> (string)
 
 Returns the chinese representation of given number.
 
 ### Arguments
 
 - **language**: string, "**T**" or "**S**".
-    - Choose between Traditional and Simplified characters.
-    - (default is "T")
+  - Choose between Traditional and Simplified characters.
+  - (default is "T")
 - **bigNumber**: bool, **True** or **False**.
-    - Output capital version of charaters.
-    - (default is False)
+  - Output capital version of charaters.
+  - (default is False)
 
 ```python
 print(convert.number2chinese(202)) #兩百零二
 print(convert.number2chinese(202, language = "S", bigNumber = True)) #贰佰零贰
 ```
 
 - **forceErLian**: string, "**auto**", "**force**" or "**forceNot**".
-    - Whether to distinguish Er(二) and Lian(兩).
-    - 1. When set to "auto", the output will follow regional convention. 
-      2. When set to "force", both Traditional and Simplified version will distinguish word usage.
-      3. When set to "forceNot", it will always output Er(二) for number "two".
-    - (default is "auto")
-> This will only effect when not using capital number (bigNumber = False). Using capital number will always output 貳/贰.
+  - Whether to distinguish Er(二) and Lian(兩).
+    1. When set to "auto", the output will follow regional convention.
+    2. When set to "force", both Traditional and Simplified version will
+       distinguish word usage.
+    3. When set to "forceNot", it will always output Er(二) for number "two".
+  - (default is "auto")
+
+> This will only effect when not using capital number (bigNumber = False).
+> Using capital number will always output 貳/贰.
 
 ```python
 print(convert.number2chinese(202, language = "T")) #兩百零二
 print(convert.number2chinese(202, language = "T", forceErLian = "forceNot")) #二百零二
 print(convert.number2chinese(202, language = "S")) #二百零二
 print(convert.number2chinese(202, language = "S", forceErLian = "force")) #两百零二
 ```
 
 ### Notes
 
-This function uses "萬進" logic when dealing with larger number (> 10<sup>8</sup>), which basically means that every 4 digits will be treated as a group.
-This is the most common logic to deal with large numbers, and can support up to 10<sup>52</sup>-1.
+This function uses "萬進" logic when dealing with larger number
+(>10<sup>8</sup>), which basically means that every 4 digits will be treated as a
+group.
+
+This is the most common logic to deal with large numbers, and can support up to
+10<sup>52</sup>-1.
```

### Comparing `ChineseNumberUtils-1.0.3/LICENSE` & `ChineseNumberUtils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ChineseNumberUtils-1.0.3/PKG-INFO` & `ChineseNumberUtils-1.1.1/cnc/ChineseNumberUtils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,112 @@
 Metadata-Version: 2.1
 Name: ChineseNumberUtils
-Version: 1.0.3
+Version: 1.1.1
 Summary: A simple converter between Chinese and arabic number
 Home-page: https://github.com/nrchan/chinese-number-converter
 Author: NR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Traditional)
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Utilities
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chinese-number-convertor
 
-This is a simple Chinese number converter that converts between [Chinese numberals](https://en.wikipedia.org/wiki/Chinese_numerals) and [arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
+This is a simple Chinese number converter that converts between
+[Chinese numbers](https://en.wikipedia.org/wiki/Chinese_numerals) and
+[Arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
 
 ## 👍 Quickstart
 
 ```python
-from ChineseNumberUtils import convert
+from cnc import convert
 
 print(convert.chinese2number("五十七")) #57
 print(convert.number2chinese(57)) #五十七
 ```
 
 ## 👉 chinese2number(string) -> (float|int)
 
 Returns the arabic number representation of given string.
 
 ### Notes
 
-The function uses a loosely-matching logic, so the given string doesn't need to be confined to a specific pattern.
+The function uses a loosely-matching logic, so the given string doesn't need to
+be confined to a specific pattern.
 
 ```python
 print(convert.chinese2number("兩千零一十二")) #2012
 print(convert.chinese2number("二零一二")) #will also be 2012
 print(convert.chinese2number("2012")) #will be, of course, 2012
 ```
-> That being said, please still avoid ambiguous and grammartically incorrect string such as ```一兆一``` or ```一百一千億```.
+
+> That being said, please still avoid ambiguous and grammartically incorrect
+> string such as ```一兆一``` or ```一百一千億```.
 
 ### Support character
 
 Support following characters:
+
 - **Normal number**: 一...九、十、百、千
 - **Large number** till 10<sup>52</sup>-1: 萬、億...極
 - **Zero**: 零、〇
-- **Captial version** of all characters above: 壹...玖、拾、佰、仟
+- **Capital version** of all characters above: 壹...玖、拾、佰、仟
 - **Arabic number**: 1...9、0
 - **Simplified version** off all characters above: 贰、万...
-> Arabic numbers were also supported because they will sometimes be mixed with characters, like "1億5000萬".
+
+> Arabic numbers were also supported because they will sometimes be mixed with
+> characters, like "1億5000萬".
 
 ## 👉 number2chinese(int) -> (string)
 
 Returns the chinese representation of given number.
 
 ### Arguments
 
 - **language**: string, "**T**" or "**S**".
-    - Choose between Traditional and Simplified characters.
-    - (default is "T")
+  - Choose between Traditional and Simplified characters.
+  - (default is "T")
 - **bigNumber**: bool, **True** or **False**.
-    - Output capital version of charaters.
-    - (default is False)
+  - Output capital version of charaters.
+  - (default is False)
 
 ```python
 print(convert.number2chinese(202)) #兩百零二
 print(convert.number2chinese(202, language = "S", bigNumber = True)) #贰佰零贰
 ```
 
 - **forceErLian**: string, "**auto**", "**force**" or "**forceNot**".
-    - Whether to distinguish Er(二) and Lian(兩).
-    - 1. When set to "auto", the output will follow regional convention. 
-      2. When set to "force", both Traditional and Simplified version will distinguish word usage.
-      3. When set to "forceNot", it will always output Er(二) for number "two".
-    - (default is "auto")
-> This will only effect when not using capital number (bigNumber = False). Using capital number will always output 貳/贰.
+  - Whether to distinguish Er(二) and Lian(兩).
+    1. When set to "auto", the output will follow regional convention.
+    2. When set to "force", both Traditional and Simplified version will
+       distinguish word usage.
+    3. When set to "forceNot", it will always output Er(二) for number "two".
+  - (default is "auto")
+
+> This will only effect when not using capital number (bigNumber = False).
+> Using capital number will always output 貳/贰.
 
 ```python
 print(convert.number2chinese(202, language = "T")) #兩百零二
 print(convert.number2chinese(202, language = "T", forceErLian = "forceNot")) #二百零二
 print(convert.number2chinese(202, language = "S")) #二百零二
 print(convert.number2chinese(202, language = "S", forceErLian = "force")) #两百零二
 ```
 
 ### Notes
 
-This function uses "萬進" logic when dealing with larger number (> 10<sup>8</sup>), which basically means that every 4 digits will be treated as a group.
-This is the most common logic to deal with large numbers, and can support up to 10<sup>52</sup>-1.
+This function uses "萬進" logic when dealing with larger number
+(>10<sup>8</sup>), which basically means that every 4 digits will be treated as a
+group.
+
+This is the most common logic to deal with large numbers, and can support up to
+10<sup>52</sup>-1.
```

### Comparing `ChineseNumberUtils-1.0.3/README.md` & `ChineseNumberUtils-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 # chinese-number-convertor
 
-This is a simple Chinese number converter that converts between [Chinese numberals](https://en.wikipedia.org/wiki/Chinese_numerals) and [arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
+This is a simple Chinese number converter that converts between
+[Chinese numbers](https://en.wikipedia.org/wiki/Chinese_numerals) and
+[Arabic numbers](https://en.wikipedia.org/wiki/Arabic_numerals).
 
 ## 👍 Quickstart
 
 ```python
-from ChineseNumberUtils import convert
+from cnc import convert
 
 print(convert.chinese2number("五十七")) #57
 print(convert.number2chinese(57)) #五十七
 ```
 
 ## 👉 chinese2number(string) -> (float|int)
 
 Returns the arabic number representation of given string.
 
 ### Notes
 
-The function uses a loosely-matching logic, so the given string doesn't need to be confined to a specific pattern.
+The function uses a loosely-matching logic, so the given string doesn't need to
+be confined to a specific pattern.
 
 ```python
 print(convert.chinese2number("兩千零一十二")) #2012
 print(convert.chinese2number("二零一二")) #will also be 2012
 print(convert.chinese2number("2012")) #will be, of course, 2012
 ```
-> That being said, please still avoid ambiguous and grammartically incorrect string such as ```一兆一``` or ```一百一千億```.
+
+> That being said, please still avoid ambiguous and grammartically incorrect
+> string such as ```一兆一``` or ```一百一千億```.
 
 ### Support character
 
 Support following characters:
+
 - **Normal number**: 一...九、十、百、千
 - **Large number** till 10<sup>52</sup>-1: 萬、億...極
 - **Zero**: 零、〇
-- **Captial version** of all characters above: 壹...玖、拾、佰、仟
+- **Capital version** of all characters above: 壹...玖、拾、佰、仟
 - **Arabic number**: 1...9、0
 - **Simplified version** off all characters above: 贰、万...
-> Arabic numbers were also supported because they will sometimes be mixed with characters, like "1億5000萬".
+
+> Arabic numbers were also supported because they will sometimes be mixed with
+> characters, like "1億5000萬".
 
 ## 👉 number2chinese(int) -> (string)
 
 Returns the chinese representation of given number.
 
 ### Arguments
 
 - **language**: string, "**T**" or "**S**".
-    - Choose between Traditional and Simplified characters.
-    - (default is "T")
+  - Choose between Traditional and Simplified characters.
+  - (default is "T")
 - **bigNumber**: bool, **True** or **False**.
-    - Output capital version of charaters.
-    - (default is False)
+  - Output capital version of charaters.
+  - (default is False)
 
 ```python
 print(convert.number2chinese(202)) #兩百零二
 print(convert.number2chinese(202, language = "S", bigNumber = True)) #贰佰零贰
 ```
 
 - **forceErLian**: string, "**auto**", "**force**" or "**forceNot**".
-    - Whether to distinguish Er(二) and Lian(兩).
-    - 1. When set to "auto", the output will follow regional convention. 
-      2. When set to "force", both Traditional and Simplified version will distinguish word usage.
-      3. When set to "forceNot", it will always output Er(二) for number "two".
-    - (default is "auto")
-> This will only effect when not using capital number (bigNumber = False). Using capital number will always output 貳/贰.
+  - Whether to distinguish Er(二) and Lian(兩).
+    1. When set to "auto", the output will follow regional convention.
+    2. When set to "force", both Traditional and Simplified version will
+       distinguish word usage.
+    3. When set to "forceNot", it will always output Er(二) for number "two".
+  - (default is "auto")
+
+> This will only effect when not using capital number (bigNumber = False).
+> Using capital number will always output 貳/贰.
 
 ```python
 print(convert.number2chinese(202, language = "T")) #兩百零二
 print(convert.number2chinese(202, language = "T", forceErLian = "forceNot")) #二百零二
 print(convert.number2chinese(202, language = "S")) #二百零二
 print(convert.number2chinese(202, language = "S", forceErLian = "force")) #两百零二
 ```
 
 ### Notes
 
-This function uses "萬進" logic when dealing with larger number (> 10<sup>8</sup>), which basically means that every 4 digits will be treated as a group.
-This is the most common logic to deal with large numbers, and can support up to 10<sup>52</sup>-1.
+This function uses "萬進" logic when dealing with larger number
+(>10<sup>8</sup>), which basically means that every 4 digits will be treated as a
+group.
+
+This is the most common logic to deal with large numbers, and can support up to
+10<sup>52</sup>-1.
```

