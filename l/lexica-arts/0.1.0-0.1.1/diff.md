# Comparing `tmp/lexica_arts-0.1.0.tar.gz` & `tmp/lexica_arts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexica_arts-0.1.0.tar", last modified: Tue Apr 18 04:26:58 2023, max compression
+gzip compressed data, was "lexica_arts-0.1.1.tar", last modified: Tue Apr 18 04:30:40 2023, max compression
```

## Comparing `lexica_arts-0.1.0.tar` & `lexica_arts-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-18 04:26:58.486678 lexica_arts-0.1.0/
--rw-rw----   0 root         (0) everybody  (9997)     1251 2023-04-18 04:26:58.478679 lexica_arts-0.1.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1045 2023-04-18 04:26:01.000000 lexica_arts-0.1.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-18 04:26:58.462679 lexica_arts-0.1.0/lexica_arts.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1251 2023-04-18 04:26:58.000000 lexica_arts-0.1.0/lexica_arts.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      173 2023-04-18 04:26:58.000000 lexica_arts-0.1.0/lexica_arts.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-18 04:26:58.000000 lexica_arts-0.1.0/lexica_arts.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       12 2023-04-18 04:26:58.000000 lexica_arts-0.1.0/lexica_arts.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      960 2023-04-18 04:22:38.000000 lexica_arts-0.1.0/lexica_arts.py
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-18 04:26:58.486678 lexica_arts-0.1.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      279 2023-04-18 04:21:42.000000 lexica_arts-0.1.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-18 04:30:40.022678 lexica_arts-0.1.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1021 2023-04-18 04:30:40.018678 lexica_arts-0.1.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      815 2023-04-18 04:30:24.000000 lexica_arts-0.1.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-18 04:30:40.010678 lexica_arts-0.1.1/lexica_arts.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1021 2023-04-18 04:30:39.000000 lexica_arts-0.1.1/lexica_arts.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      173 2023-04-18 04:30:39.000000 lexica_arts-0.1.1/lexica_arts.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-18 04:30:39.000000 lexica_arts-0.1.1/lexica_arts.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       12 2023-04-18 04:30:39.000000 lexica_arts-0.1.1/lexica_arts.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      960 2023-04-18 04:22:38.000000 lexica_arts-0.1.1/lexica_arts.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-18 04:30:40.026678 lexica_arts-0.1.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      279 2023-04-18 04:29:43.000000 lexica_arts-0.1.1/setup.py
```

### Comparing `lexica_arts-0.1.0/PKG-INFO` & `lexica_arts-0.1.1/lexica_arts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 Metadata-Version: 2.1
-Name: lexica_arts
-Version: 0.1.0
+Name: lexica-arts
+Version: 0.1.1
 Summary: A module for generating image in Lexica.arts
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Модуль `lexica_arts` предоставляет класс `Image`, который используется для генерации изображений с помощью API-сервиса Lexica. Для использования модуля необходимо установить библиотеки aiohttp и Pillow (библиотека для работы с изображениями).
 
 Класс Image содержит метод generate, который принимает два параметра: `prompt` и `negative`. Параметр `prompt` содержит описание изображения, которое необходимо сгенерировать, а параметр `negative` содержит негативное описание (необязательно).
 
-Пример использования модуля:
-
-```import lexica_arts
-
-api_key = 'your_api_key'
-
-image = lexica_arts.Image(api_key)
-
-generated_image = await image.generate(prompt="beautiful sunset", negative="cloudy sky")
-
```

### Comparing `lexica_arts-0.1.0/README.md` & `lexica_arts-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+Metadata-Version: 2.1
+Name: lexica_arts
+Version: 0.1.1
+Summary: A module for generating image in Lexica.arts
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 Модуль `lexica_arts` предоставляет класс `Image`, который используется для генерации изображений с помощью API-сервиса Lexica. Для использования модуля необходимо установить библиотеки aiohttp и Pillow (библиотека для работы с изображениями).
 
 Класс Image содержит метод generate, который принимает два параметра: `prompt` и `negative`. Параметр `prompt` содержит описание изображения, которое необходимо сгенерировать, а параметр `negative` содержит негативное описание (необязательно).
 
-Пример использования модуля:
-
-```import lexica_arts
-
-api_key = 'your_api_key'
-
-image = lexica_arts.Image(api_key)
 
-generated_image = await image.generate(prompt="beautiful sunset", negative="cloudy sky")
```

### Comparing `lexica_arts-0.1.0/lexica_arts.py` & `lexica_arts-0.1.1/lexica_arts.py`

 * *Files identical despite different names*

