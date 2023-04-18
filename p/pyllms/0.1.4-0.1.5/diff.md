# Comparing `tmp/pyllms-0.1.4.tar.gz` & `tmp/pyllms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.4.tar", last modified: Thu Apr 13 22:14:21 2023, max compression
+gzip compressed data, was "pyllms-0.1.5.tar", last modified: Tue Apr 18 04:18:14 2023, max compression
```

## Comparing `pyllms-0.1.4.tar` & `pyllms-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.413453 pyllms-0.1.4/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.4/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    13651 2023-04-13 22:14:21.413151 pyllms-0.1.4/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    12410 2023-04-13 22:10:16.000000 pyllms-0.1.4/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.410615 pyllms-0.1.4/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.4/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    16855 2023-04-13 22:03:17.000000 pyllms-0.1.4/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.411758 pyllms-0.1.4/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.4/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.4/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4084 2023-04-13 22:10:49.000000 pyllms-0.1.4/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3569 2023-04-13 21:35:11.000000 pyllms-0.1.4/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.412820 pyllms-0.1.4/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    13651 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-13 22:14:21.413544 pyllms-0.1.4/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1760 2023-04-13 22:13:55.000000 pyllms-0.1.4/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.371912 pyllms-0.1.5/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.5/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    14437 2023-04-18 04:18:14.371638 pyllms-0.1.5/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    13196 2023-04-18 04:17:49.000000 pyllms-0.1.5/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.368809 pyllms-0.1.5/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.5/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    17070 2023-04-18 01:40:10.000000 pyllms-0.1.5/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.370067 pyllms-0.1.5/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.5/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.5/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4087 2023-04-17 15:37:12.000000 pyllms-0.1.5/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3569 2023-04-13 21:35:11.000000 pyllms-0.1.5/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 04:18:14.371301 pyllms-0.1.5/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    14437 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-18 04:18:14.000000 pyllms-0.1.5/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-18 04:18:14.371986 pyllms-0.1.5/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1760 2023-04-18 04:18:04.000000 pyllms-0.1.5/setup.py
```

### Comparing `pyllms-0.1.4/LICENSE` & `pyllms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.4/PKG-INFO` & `pyllms-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -20,17 +20,28 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # PyLLMs
 
-A lightweight Python that strives to enable dead-simple interaction with popular language models from OpenAI, Anthropic, AI21 and others.
+[![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
+
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+
+It is ideal for fast prototyping and evaluationg different models thanks to:
+- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+- Response meta includes tokens processed, cost and latency standardized across the models
+- Multi-model support: Get completitions from different models at the same time
+- LLM benchmark: Eevaluate models on quality, speed and cost
+
+Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
 pip3 install pyllms
@@ -78,15 +89,15 @@
     temperature=0.1,
     max_tokens=200
 )
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
+The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 ## Multi-model usage
@@ -106,17 +117,17 @@
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
 >>> model= llms.init('claude-v1')
 >>> result = model.complete_stream("write an essay on civil war")
->>> for chunks in result:
-...        if content is not None:
-...          print(chunks, end='')   
+>>> for chunk in result:
+...        if chunk is not None:
+...          print(chunk, end='')   
 ... 
 
 Here is a paragraph about civil rights:
 
 
 Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
 
@@ -131,26 +142,26 @@
 
 ```
 python3 -u
 ```
 
 ## Benchmarks
 
-Models are appearing like mushrooms after rain and we are interested in:
+Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
-We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
-gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
```

### Comparing `pyllms-0.1.4/README.md` & `pyllms-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,21 @@
+
 # PyLLMs
 
-A lightweight Python that strives to enable dead-simple interaction with popular language models from OpenAI, Anthropic, AI21 and others.
+[![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
+
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+
+It is ideal for fast prototyping and evaluationg different models thanks to:
+- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+- Response meta includes tokens processed, cost and latency standardized across the models
+- Multi-model support: Get completitions from different models at the same time
+- LLM benchmark: Eevaluate models on quality, speed and cost
+
+Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
 pip3 install pyllms
@@ -52,15 +63,15 @@
     temperature=0.1,
     max_tokens=200
 )
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
+The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 ## Multi-model usage
@@ -80,17 +91,17 @@
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
 >>> model= llms.init('claude-v1')
 >>> result = model.complete_stream("write an essay on civil war")
->>> for chunks in result:
-...        if content is not None:
-...          print(chunks, end='')   
+>>> for chunk in result:
+...        if chunk is not None:
+...          print(chunk, end='')   
 ... 
 
 Here is a paragraph about civil rights:
 
 
 Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
 
@@ -105,26 +116,26 @@
 
 ```
 python3 -u
 ```
 
 ## Benchmarks
 
-Models are appearing like mushrooms after rain and we are interested in:
+Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
-We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
-gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
```

### Comparing `pyllms-0.1.4/llms/llms.py` & `pyllms-0.1.5/llms/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 model_info_list.append(model_info)
 
         sorted_list = sorted(
             model_info_list, key=lambda x: x["cost"]["prompt"] + x["cost"]["completion"]
         )
         return sorted_list
 
-    def complete(self, prompt, history=None, **kwargs):
+    def complete(self, prompt, history=None, system_message=None, **kwargs):
         def _generate(provider):
            
             response = provider.complete(prompt, history, **kwargs)
     
             formatted_cost = format(response["meta"]["cost"], '.5f')
             formatted_latency = round(response["meta"]["latency"], 2)
             
@@ -124,15 +124,15 @@
                 for provider in self._providers
             }
             for future in as_completed(futures):
                 results.append(future.result())
 
         return Result(results)
 
-    def complete_stream(self, prompt, history=None, **kwargs):
+    def complete_stream(self, prompt, history=None, system_message=None, **kwargs):
                  
         if len(self._providers)>1:
             raise ValueError(
                 "Streaming is possible only with a single model"
             )
         if isinstance(self._providers[0], AI21Provider):
             raise ValueError(
@@ -147,14 +147,15 @@
             prompts = [
                 "What is the capital of the country where Christopher Columbus was born?",
                 "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
                 "Solve the quadratic equation: x^2 - 5x + 6 = 0",
                 "How much is 7! * 3! -1234.5 ?",
                 'translate this sentence by alternating words in gemran and french "it was a beautiful day that thursday and I want skiing outside. it started raining soon although they said it won\'t be until friday, so I went to the pool instead"',
                 "Convert December 21 · 1:00 – 1:50pm pacific to asia/taipei time",
+                "Explain the plot of Cinderella in a sentence where each word has to begin with the next letter in the alphabet from A to Z, without repeating any letters",
                 "In my kitchen there's a table with a cup with a ball inside. I moved the cup to my bed in my bedroom and turned the cup upside down. I grabbed the cup again and moved to the main room. Where's the ball now?",
                 'Capture the essence of this in exactly 7 words: "There’s much that divides us in Northern Ireland though one thing is guaranteed to bring us together: local phrases. Call it slang, call it colloquialisms, we all know only too well how important words are to where we’re from . . . and when it comes to the phrases that make us ‘us,’ we’ve got a lot to say. While you don’t need advance knowledge of the words to fit in, well, it helps. How else will you know where ‘foundered’ sits on the scale of warm to freezing? Or deciding whether that new car purchase is more ‘clinker’ than ‘beezer’? Or appreciating that ‘grand’ can mean exactly that or anything but? If the best way to get to know a nation is to understand their language, then surely tourists must be at times confused about what comes out of our mouths. Throughout the island of Ireland, we have utterly brilliant ways to verbally express ourselves.“I think it’s really important,” says Dr Frank Ferguson, research director for English Language and Literature at Ulster University, about the vitality of slang as part of language."',
                 "Write a Python function that takes a list of integers as input and returns the length of the longest increasing subsequence. An increasing subsequence is a subsequence of the given list where the elements are in strictly increasing order. Your function should have an efficient solution with a time complexity better than O(n^2), where n is the length of the input list. Output only code with no explainations and provide example usage.",
                 "Write a Python function that takes a list of integers as input and returns the maximum sum of non-adjacent elements in the list. The function should return 0 if the input list is empty. Your function should have an efficient solution with a time complexity of O(n), where n is the length of the input list. Output only code with no explainations and provide example usage.",
                 "You are given a 2D binary matrix filled with 0's and 1's. Your task is to write a JavaScript function that finds the largest rectangle containing only 1's and returns its area. Your function should have an efficient solution with a time complexity better than O(n^3), where n is the total number of elements in the input matrix. Output only code with no explainations and provide example usage.",
                 "Given the following messy and unstructured data, extract the names, email addresses, and phone numbers of the individuals listed:\
 John Doe - johndoe (at) email.com (five-five-five) one-two-three-four-five-six-seven\
```

### Comparing `pyllms-0.1.4/llms/providers/ai21.py` & `pyllms-0.1.5/llms/providers/ai21.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.4/llms/providers/anthropic.py` & `pyllms-0.1.5/llms/providers/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import time
 
 from typing import List, Optional
 
 
 class AnthropicProvider:
     MODEL_INFO = {
-        "claude-instant-v1": {"prompt": 0.43, "completion": 1.45, "token_limit": 8000},
-        "claude-v1": {"prompt": 2.9, "completion": 8.6, "token_limit": 8_000},
+        "claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
+        "claude-v1": {"prompt": 11.02, "completion": 32.68, "token_limit": 9000},
     }
 
     def __init__(self, api_key=None, model=None):
         if api_key is None:
             api_key = os.getenv("ANTHROPIC_API_KEY")
         self.client = anthropic.Client(api_key)
```

### Comparing `pyllms-0.1.4/llms/providers/openai.py` & `pyllms-0.1.5/llms/providers/openai.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.4/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.5/pyllms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.4
+Version: 0.1.5
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -20,17 +20,28 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # PyLLMs
 
-A lightweight Python that strives to enable dead-simple interaction with popular language models from OpenAI, Anthropic, AI21 and others.
+[![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
+
+PyLLMs is a minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark. 
+
+It is ideal for fast prototyping and evaluationg different models thanks to:
+- Connect to top LLMs in few lines of code (currenly OpenAI, Anthropic and AI21 are supported)
+- Response meta includes tokens processed, cost and latency standardized across the models
+- Multi-model support: Get completitions from different models at the same time
+- LLM benchmark: Eevaluate models on quality, speed and cost
+
+Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
 pip3 install pyllms
@@ -78,15 +89,15 @@
     temperature=0.1,
     max_tokens=200
 )
 ```
 
 Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
+The result meta will contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 ## Multi-model usage
@@ -106,17 +117,17 @@
 ## Streaming support
 
 PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
 
 ```
 >>> model= llms.init('claude-v1')
 >>> result = model.complete_stream("write an essay on civil war")
->>> for chunks in result:
-...        if content is not None:
-...          print(chunks, end='')   
+>>> for chunk in result:
+...        if chunk is not None:
+...          print(chunk, end='')   
 ... 
 
 Here is a paragraph about civil rights:
 
 
 Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
 
@@ -131,26 +142,26 @@
 
 ```
 python3 -u
 ```
 
 ## Benchmarks
 
-Models are appearing like mushrooms after rain and we are interested in:
+Models are appearing like mushrooms after rain and everyone is interested in three things:
 
 1) Quality
 2) Speed
 3) Cost
 
-We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+PyLLMs icludes an automated benchmark system. The quality of models is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
 
 
 ```
 models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
-gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in that case only speed and cost will be evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
```

### Comparing `pyllms-0.1.4/setup.py` & `pyllms-0.1.5/setup.py`

 * *Files identical despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.4",
+    version="0.1.5",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

