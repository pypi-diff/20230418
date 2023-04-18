# Comparing `tmp/sd-parsers-0.1.0.tar.gz` & `tmp/sd-parsers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-parsers-0.1.0.tar", last modified: Fri Apr 14 21:36:40 2023, max compression
+gzip compressed data, was "sd-parsers-0.2.0.tar", last modified: Tue Apr 18 01:00:48 2023, max compression
```

## Comparing `sd-parsers-0.1.0.tar` & `sd-parsers-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:40.003651 sd-parsers-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.995651 sd-parsers-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.995651 sd-parsers-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/.github/workflows/publish-to.pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-14 21:36:40.003651 sd-parsers-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.995651 sd-parsers-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/examples/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/examples/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:36:40.003651 sd-parsers-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.995651 sd-parsers-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.999651 sd-parsers-0.1.0/src/sd_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-14 21:36:39.000000 sd-parsers-0.1.0/src/sd_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 21:36:39.000000 sd-parsers-0.1.0/src/sd_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:36:39.000000 sd-parsers-0.1.0/src/sd_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 21:36:39.000000 sd-parsers-0.1.0/src/sd_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 21:36:39.000000 sd-parsers-0.1.0/src/sd_parsers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:39.999651 sd-parsers-0.1.0/src/sdparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:40.003651 sd-parsers-0.1.0/src/sdparsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parsers/automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parsers/automatic1111_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parsers/comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/parsers/invokeai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-14 21:36:30.000000 sd-parsers-0.1.0/src/sdparsers/prompt_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/.github/workflows/publish-to.pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:00:48.479963 sd-parsers-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sd_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sdparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sdparsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111_stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/prompt_info.py
```

### Comparing `sd-parsers-0.1.0/.github/workflows/publish-to.pypi.yml` & `sd-parsers-0.2.0/.github/workflows/publish-to.pypi.yml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/LICENSE.txt` & `sd-parsers-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/PKG-INFO` & `sd-parsers-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.1.0
+Version: 0.2.0
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,28 +31,29 @@
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI
 * Invoke AI
+* NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
 
 The ```ParserManager()``` constructor takes two arguments:
 * `config_file`: If you want to provide alternate processing instructions. (absolute path to config file)
-* `process_items`: If the parser should try to make the output across the different
+* `process_items`: If the parser should try to normalize the output across the different image sources. (defaults to `True`)
 
 ### Basic usage:
 
 Read prompt information from a given filename:
 ```python
 from sdparsers import ParserManager
 
@@ -86,47 +87,52 @@
 from sdparsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info = parser.parse(image)
 ```
 
-Directly using a specific parser, the configuration file is not read automatically. (see ```ParserManager.__init__()```)
+Directly using a specific parser, the configuration file is not read automatically. (see `ParserManager.__init__()`)
 
-Also, when not called via ```ParserManager```, the ```parse()``` method now requires a Pillow Image object as argument. (see ```ParserManager.parse()```)
+Also, when not called via `ParserManager`, the `parse()` method now requires a Pillow Image object as argument. (see `ParserManager.parse()`)
 
 
 ### Output
-The ```parse()``` method returns a ```PromptInfo``` type with the following properties (or ```None``` if no metadata was found):
-* ```generator```: A simple string, specifying the parsing module that was used.
+The `parse()` method returns a `PromptInfo` type with the following properties (or `None` if no metadata was found):
+* `generator`: A simple string, specifying the parsing module that was used.
 
   ("AUTOMATIC1111" | "AUTOMATICStealth" | "ComfyUI" | "InvokeAI")
 
-* ```prompts```: A list of tuples of prompts as found in the parsed metadata.
+* `prompts`: A list of tuples of prompts as found in the parsed metadata.
 
-  In the form of ```(prompt, negative_prompt)```.
+  In the form of `(prompt, negative_prompt)`.
 
-* `samplers`: An unordered list of found samplers (and parameters)
+* `samplers`: An unordered list of found samplers (and parameters).
 
-* `models`: An unordered list of models used in the generation process
+  The key values of the parameters dictionary will be normalized to be more consistent across image generators if `ParserManager` is used with `process_items` set to `True`.
 
-* ```metadata```: A dictionary of metadata besides the prompt information.
+* `models`: An unordered list of models used in the generation process.
+
+* `metadata`: A dictionary of metadata besides the prompt information.
 
   Contains additional parameters which are found in the image metadata.
 
   Highly dependent on the provided data structure of the respective image generator.
 
-  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True``` (the default).
+  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True```.
  
 * ```raw_params```: A dictionary of the unmodified metadata entries found in the parsed image (if present).
 
   * Automatic1111: ```"parameters"```
   * InvokeAI: ```"sd-metadata"``` and ```"Dream"```
   * ComfyUI: ```"prompt"``` and ```"workflow"```
 
 
 ## Credits
 Idea and motivation using AUTOMATIC1111's stable diffusion webui
 - https://github.com/AUTOMATIC1111/stable-diffusion-webui
 
 Stealth PNGInfo code adopted from ashen-sensored's sd webui extension
 - https://github.com/ashen-sensored/sd_webui_stealth_pnginfo
+
+Example workflows for testing the ComfyUI parser
+- https://github.com/comfyanonymous/ComfyUI_examples
```

### Comparing `sd-parsers-0.1.0/README.md` & `sd-parsers-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI
 * Invoke AI
+* NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
 
 The ```ParserManager()``` constructor takes two arguments:
 * `config_file`: If you want to provide alternate processing instructions. (absolute path to config file)
-* `process_items`: If the parser should try to make the output across the different
+* `process_items`: If the parser should try to normalize the output across the different image sources. (defaults to `True`)
 
 ### Basic usage:
 
 Read prompt information from a given filename:
 ```python
 from sdparsers import ParserManager
 
@@ -56,47 +57,52 @@
 from sdparsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info = parser.parse(image)
 ```
 
-Directly using a specific parser, the configuration file is not read automatically. (see ```ParserManager.__init__()```)
+Directly using a specific parser, the configuration file is not read automatically. (see `ParserManager.__init__()`)
 
-Also, when not called via ```ParserManager```, the ```parse()``` method now requires a Pillow Image object as argument. (see ```ParserManager.parse()```)
+Also, when not called via `ParserManager`, the `parse()` method now requires a Pillow Image object as argument. (see `ParserManager.parse()`)
 
 
 ### Output
-The ```parse()``` method returns a ```PromptInfo``` type with the following properties (or ```None``` if no metadata was found):
-* ```generator```: A simple string, specifying the parsing module that was used.
+The `parse()` method returns a `PromptInfo` type with the following properties (or `None` if no metadata was found):
+* `generator`: A simple string, specifying the parsing module that was used.
 
   ("AUTOMATIC1111" | "AUTOMATICStealth" | "ComfyUI" | "InvokeAI")
 
-* ```prompts```: A list of tuples of prompts as found in the parsed metadata.
+* `prompts`: A list of tuples of prompts as found in the parsed metadata.
 
-  In the form of ```(prompt, negative_prompt)```.
+  In the form of `(prompt, negative_prompt)`.
 
-* `samplers`: An unordered list of found samplers (and parameters)
+* `samplers`: An unordered list of found samplers (and parameters).
 
-* `models`: An unordered list of models used in the generation process
+  The key values of the parameters dictionary will be normalized to be more consistent across image generators if `ParserManager` is used with `process_items` set to `True`.
 
-* ```metadata```: A dictionary of metadata besides the prompt information.
+* `models`: An unordered list of models used in the generation process.
+
+* `metadata`: A dictionary of metadata besides the prompt information.
 
   Contains additional parameters which are found in the image metadata.
 
   Highly dependent on the provided data structure of the respective image generator.
 
-  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True``` (the default).
+  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True```.
  
 * ```raw_params```: A dictionary of the unmodified metadata entries found in the parsed image (if present).
 
   * Automatic1111: ```"parameters"```
   * InvokeAI: ```"sd-metadata"``` and ```"Dream"```
   * ComfyUI: ```"prompt"``` and ```"workflow"```
 
 
 ## Credits
 Idea and motivation using AUTOMATIC1111's stable diffusion webui
 - https://github.com/AUTOMATIC1111/stable-diffusion-webui
 
 Stealth PNGInfo code adopted from ashen-sensored's sd webui extension
-- https://github.com/ashen-sensored/sd_webui_stealth_pnginfo
+- https://github.com/ashen-sensored/sd_webui_stealth_pnginfo
+
+Example workflows for testing the ComfyUI parser
+- https://github.com/comfyanonymous/ComfyUI_examples
```

### Comparing `sd-parsers-0.1.0/examples/cmdline.py` & `sd-parsers-0.2.0/examples/cmdline.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/examples/fast_api.py` & `sd-parsers-0.2.0/examples/fast_api.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/src/sd_parsers.egg-info/PKG-INFO` & `sd-parsers-0.2.0/src/sd_parsers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.1.0
+Version: 0.2.0
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,28 +31,29 @@
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI
 * Invoke AI
+* NovelAI
 
 Provides a list of prompts used in the generation of the image, as well as generator-specific metadata.
 
 ## Installation
 ```
 pip install sd-parsers
 ```
 
 ## Usage
 For a simple query, import ```ParserManager``` from ```sdparsers``` and use its ```parse()``` method to parse an image. (see [examples](https://github.com/d3x-at/sd-parsers/tree/master/examples))
 
 The ```ParserManager()``` constructor takes two arguments:
 * `config_file`: If you want to provide alternate processing instructions. (absolute path to config file)
-* `process_items`: If the parser should try to make the output across the different
+* `process_items`: If the parser should try to normalize the output across the different image sources. (defaults to `True`)
 
 ### Basic usage:
 
 Read prompt information from a given filename:
 ```python
 from sdparsers import ParserManager
 
@@ -86,47 +87,52 @@
 from sdparsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info = parser.parse(image)
 ```
 
-Directly using a specific parser, the configuration file is not read automatically. (see ```ParserManager.__init__()```)
+Directly using a specific parser, the configuration file is not read automatically. (see `ParserManager.__init__()`)
 
-Also, when not called via ```ParserManager```, the ```parse()``` method now requires a Pillow Image object as argument. (see ```ParserManager.parse()```)
+Also, when not called via `ParserManager`, the `parse()` method now requires a Pillow Image object as argument. (see `ParserManager.parse()`)
 
 
 ### Output
-The ```parse()``` method returns a ```PromptInfo``` type with the following properties (or ```None``` if no metadata was found):
-* ```generator```: A simple string, specifying the parsing module that was used.
+The `parse()` method returns a `PromptInfo` type with the following properties (or `None` if no metadata was found):
+* `generator`: A simple string, specifying the parsing module that was used.
 
   ("AUTOMATIC1111" | "AUTOMATICStealth" | "ComfyUI" | "InvokeAI")
 
-* ```prompts```: A list of tuples of prompts as found in the parsed metadata.
+* `prompts`: A list of tuples of prompts as found in the parsed metadata.
 
-  In the form of ```(prompt, negative_prompt)```.
+  In the form of `(prompt, negative_prompt)`.
 
-* `samplers`: An unordered list of found samplers (and parameters)
+* `samplers`: An unordered list of found samplers (and parameters).
 
-* `models`: An unordered list of models used in the generation process
+  The key values of the parameters dictionary will be normalized to be more consistent across image generators if `ParserManager` is used with `process_items` set to `True`.
 
-* ```metadata```: A dictionary of metadata besides the prompt information.
+* `models`: An unordered list of models used in the generation process.
+
+* `metadata`: A dictionary of metadata besides the prompt information.
 
   Contains additional parameters which are found in the image metadata.
 
   Highly dependent on the provided data structure of the respective image generator.
 
-  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True``` (the default).
+  The key values of this dictionary will be normalized to be more consistent across image generators if ```ParserManager``` is used with ```process_items``` set to ```True```.
  
 * ```raw_params```: A dictionary of the unmodified metadata entries found in the parsed image (if present).
 
   * Automatic1111: ```"parameters"```
   * InvokeAI: ```"sd-metadata"``` and ```"Dream"```
   * ComfyUI: ```"prompt"``` and ```"workflow"```
 
 
 ## Credits
 Idea and motivation using AUTOMATIC1111's stable diffusion webui
 - https://github.com/AUTOMATIC1111/stable-diffusion-webui
 
 Stealth PNGInfo code adopted from ashen-sensored's sd webui extension
 - https://github.com/ashen-sensored/sd_webui_stealth_pnginfo
+
+Example workflows for testing the ComfyUI parser
+- https://github.com/comfyanonymous/ComfyUI_examples
```

### Comparing `sd-parsers-0.1.0/src/sd_parsers.egg-info/SOURCES.txt` & `sd-parsers-0.2.0/src/sd_parsers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 LICENSE.txt
 README.md
 pyproject.toml
 .github/workflows/publish-to.pypi.yml
+examples/README.md
 examples/cmdline.py
 examples/fast_api.py
 src/sd_parsers.egg-info/PKG-INFO
 src/sd_parsers.egg-info/SOURCES.txt
 src/sd_parsers.egg-info/dependency_links.txt
 src/sd_parsers.egg-info/requires.txt
 src/sd_parsers.egg-info/top_level.txt
@@ -15,8 +16,9 @@
 src/sdparsers/parser.py
 src/sdparsers/parser_manager.py
 src/sdparsers/prompt_info.py
 src/sdparsers/parsers/__init__.py
 src/sdparsers/parsers/automatic1111.py
 src/sdparsers/parsers/automatic1111_stealth.py
 src/sdparsers/parsers/comfyui.py
-src/sdparsers/parsers/invokeai.py
+src/sdparsers/parsers/invokeai.py
+src/sdparsers/parsers/novelai.py
```

### Comparing `sd-parsers-0.1.0/src/sdparsers/parser.py` & `sd-parsers-0.2.0/src/sdparsers/parser.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/src/sdparsers/parser_manager.py` & `sd-parsers-0.2.0/src/sdparsers/parser_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,23 @@
         self.parsers = sorted((parser(get_config(parser), process_items)
                                for parser in _get_parsers()),
                               key=lambda p: p.PRIORITY, reverse=True)
 
     def parse(self, image: Union[str, bytes, Path,
                                  SupportsRead[bytes],
                                  Image.Image]) -> Optional[PromptInfo]:
-        '''try available parsers to get image information'''
+        '''try available parsers to get image information
+
+        The following exceptions can be thrown by the underlying `Image.open()`
+        function:
+        :exception FileNotFoundError: If the file cannot be found.
+        :exception PIL.UnidentifiedImageError: If the image cannot be opened
+        and identified.
+        :exception ValueError: If a StringIO instance is used for fp.
+        '''
         if isinstance(image, Image.Image):
             return self._parse(image)
         else:
             with Image.open(image) as image_data:
                 return self._parse(image_data)
 
     def _parse(self, image: Image.Image) -> Optional[PromptInfo]:
```

### Comparing `sd-parsers-0.1.0/src/sdparsers/parsers/automatic1111.py` & `sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,37 +68,43 @@
 
 def split_parameters(parameters: str) -> Tuple[str, str, dict]:
     '''split an A1111 parameters string into prompt, negative prompt and metadata'''
     lines = parameters.split("\n")
     if not lines:
         return None, None, None
 
-    metadata_raw = lines[-1].split(',')
-    if len(metadata_raw) < 3:
+    def split_meta(item: str):
+        key, value = map(str.strip, item.split(':'))
+        return key, value
+
+    metadata = None
+    try:
+        metadata = [split_meta(item) for item in lines[-1].split(',')]
+    except ValueError:
+        pass
+
+    if not metadata or len(metadata) < 3:
         # actually a bit stricter than in the webui itself
         # grants some protection against "non-a1111" parameters
         return None, None, None
 
-    metadata = (map(str.strip, item.split(':')) for item in metadata_raw)
     prompt_lines = lines[:-1]
 
     # prompt
     prompt = []
     i = 0
     for line in prompt_lines:
         line = line.strip()
         if line.startswith("Negative prompt:"):
             prompt_lines[i] = line[16:]
             break
         prompt.append(line)
         i += 1
 
     # negative prompt
-    negative_prompt = []
-    for line in prompt_lines[i:]:
-        negative_prompt.append(line.strip())
+    negative_prompt = [line.strip() for line in prompt_lines[i:]]
 
     return (
         "\n".join(prompt),
         "\n".join(negative_prompt),
         dict(metadata)
     )
```

### Comparing `sd-parsers-0.1.0/src/sdparsers/parsers/automatic1111_stealth.py` & `sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111_stealth.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/src/sdparsers/parsers/comfyui.py` & `sd-parsers-0.2.0/src/sdparsers/parsers/comfyui.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/src/sdparsers/parsers/invokeai.py` & `sd-parsers-0.2.0/src/sdparsers/parsers/invokeai.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.1.0/src/sdparsers/prompt_info.py` & `sd-parsers-0.2.0/src/sdparsers/prompt_info.py`

 * *Files identical despite different names*

