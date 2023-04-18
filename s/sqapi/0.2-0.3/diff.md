# Comparing `tmp/sqapi-0.2.tar.gz` & `tmp/sqapi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqapi-0.2.tar", last modified: Tue Apr 18 00:18:39 2023, max compression
+gzip compressed data, was "sqapi-0.3.tar", last modified: Tue Apr 18 02:01:41 2023, max compression
```

## Comparing `sqapi-0.2.tar` & `sqapi-0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.105114 sqapi-0.2/
--rw-r--r--   0 ariell     (501) staff       (20)     8606 2023-04-18 00:18:39.105195 sqapi-0.2/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)     7705 2023-04-18 00:15:58.000000 sqapi-0.2/README.md
--rw-r--r--   0 ariell     (501) staff       (20)       79 2023-04-18 00:18:39.105479 sqapi-0.2/setup.cfg
--rw-r--r--   0 ariell     (501) staff       (20)     1688 2023-04-18 00:18:11.000000 sqapi-0.2/setup.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.104467 sqapi-0.2/sqapi/
--rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.2/sqapi/__init__.py
--rw-r--r--   0 ariell     (501) staff       (20)    12682 2023-04-07 10:49:09.000000 sqapi-0.2/sqapi/annotate.py
--rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.2/sqapi/api.py
--rw-r--r--   0 ariell     (501) staff       (20)     4926 2023-04-07 05:24:54.000000 sqapi-0.2/sqapi/helpers.py
--rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.2/sqapi/media.py
--rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.2/sqapi/request.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.105021 sqapi-0.2/sqapi.egg-info/
--rw-r--r--   0 ariell     (501) staff       (20)     8606 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)      270 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/SOURCES.txt
--rw-r--r--   0 ariell     (501) staff       (20)        1 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/dependency_links.txt
--rw-r--r--   0 ariell     (501) staff       (20)       29 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/requires.txt
--rw-r--r--   0 ariell     (501) staff       (20)        6 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/top_level.txt
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982992 sqapi-0.3/
+-rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-04-17 06:42:47.000000 sqapi-0.3/LICENSE.txt
+-rw-r--r--   0 ariell     (501) staff       (20)     9086 2023-04-18 02:01:41.983075 sqapi-0.3/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)     8059 2023-04-18 01:38:47.000000 sqapi-0.3/README.md
+-rw-r--r--   0 ariell     (501) staff       (20)       79 2023-04-18 02:01:41.983360 sqapi-0.3/setup.cfg
+-rw-r--r--   0 ariell     (501) staff       (20)     1786 2023-04-18 02:00:20.000000 sqapi-0.3/setup.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982159 sqapi-0.3/sqapi/
+-rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.3/sqapi/__init__.py
+-rw-r--r--   0 ariell     (501) staff       (20)    12681 2023-04-18 01:48:28.000000 sqapi-0.3/sqapi/annotate.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.3/sqapi/api.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4902 2023-04-18 01:29:24.000000 sqapi-0.3/sqapi/helpers.py
+-rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.3/sqapi/media.py
+-rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.3/sqapi/request.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982895 sqapi-0.3/sqapi.egg-info/
+-rw-r--r--   0 ariell     (501) staff       (20)     9086 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)      282 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        1 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ariell     (501) staff       (20)       29 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/requires.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        6 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/top_level.txt
```

### Comparing `sqapi-0.2/PKG-INFO` & `sqapi-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.2
+Version: 0.3
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # SQAPI
 
 `sqapi` is a python package that simplifies interactions with the 
 [SQUIDLE+ API](https://squidle.org/api/help?template=api_help_page.html).
 It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 
 ### Installation
 To install the `sqapi` module, you can use `pip`
 ```shell
 pip install sqapi 
 ```
 
-### Why & how
-The `sqapi` module helps to build the `HTTP` requests that are sent to the `API`. These are 
+### What is this?
+The `sqapi` module helps to build the `HTTP` requests that are sent to the [SQUIDLE+](squidle.org) `API`. These are 
 `GET`, `POST`, `PATCH` or `DELETE` requests. Setting `verbosity=2` on the `sqapi` module will print the `HTTP` 
 requests that are being made.
 
 `sqapi` takes care of authentication, and simplifies the creation of API queries. 
 For example:
 
 ```python
@@ -42,20 +45,23 @@
 
 sqapi = SQAPI(host=<HOST>,api_key=<API_KEY>, verbosity=2)  # instantiate the sqapi module
 r=sqapi.get(<ENDPOINT>)              # define a get request using a specific endpoint
 r.filter(<NAME>,<OPERATORE>,<VALUE>) # define a filter to compare a property with a value using an operator
 data = r.execute().json()            # perform the request & return result as JSON dict (don't set template)
 ```
 
+For more information about structuring queries, check out the [Making API queries](https://squidle.org/api/help?template=api_help_page.html#api_query)
+section of the SQ+ API documentation page.
+
 Instantiating `sqapi` without an API key argument will prompt for a user login, i.e.:
 ```python
 sqapi = SQAPI(host=<HOST>, verbosity=2)  # instantiate the sqapi module
 ```
 
-You can also use it to apply templates to the data that comes out of the API:
+You can also use it to apply built-in templates to the data that comes out of the API:
 ```python
 r.template(<TEMPLATE>)               # format the output of the request using an inbuilt HTML template
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
@@ -71,14 +77,17 @@
 mkdir sqbot_demo && cd sqbot_demo   # make a directory
 virtualenv -p python3 env           # create a virtual environment
 source env/bin/activate             # activate it
 pip install sqapi  # install sqapi
 ```
 
 #### 1. Create a bot class
+In this example, we'll create an automated classifier that suggests random label suggestions for an annotation_set. 
+It uses the `Annotator` class from the `sqapi.annotate` module, which does most of the heavy-lifting. The implementation
+of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
 from sqapi.request import query_filter as qf
@@ -113,31 +122,27 @@
     # Add an extra argument to the parser to get an annotation_set id to classify
     parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
     
     # Instantiate the bot class
     args = parser.parse_args()
     bot = RandoBOT(**vars(args))
     
-    # Initialise the request for the list of annotation_sets that you want classified
-    # only consider annotation_sets that do not already have suggestions from this user
-    r = bot.sqapi.get("/api/annotation_set")
-    r.filter_not(qf("children", "any", val=qf("user_id", "eq", bot.sqapi.current_user.get("id"))))
-
-    # filter annotation_sets within a nominated user_group 
-    # as specified by the extra parameter added to RandoBot.__init__
-    r.filter(name="id", op="in", val=args.annotation_set_id)
+    # Initialise the request for the annotation_set that you want classified
+    # update the ID to the ID you want
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
 
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
-This allows you to pass arguments from the command line, and to use help on how to use it:
+This allows you to pass arguments from the command line, and helps to show how to use it:
 ```shell
+# from the command line, run:
 python run_bot.py --help
 ```
 
 It will show you all the required parameters from the base class `Annotator` as well as any extra arguments added to the 
 `__init__` method of the `RandoBot` class. Parameter descriptions come from the comment block.
 
 #### 2. Create a Label Mapper File
@@ -151,31 +156,31 @@
   "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
   "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
   "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
 }
 ```
 
 #### 3. Run your bot
-Now you're ready to run your classifier RandoBot, by simply executing this from the command line:
+Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay 5 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
 ```
 
-This will get the list of annotation_sets contained in the user_group with the id of `55`
+This will run the classifier once on the annotation_set with an `ID=55`
 and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will continue this indefinitely in a loop every 5s ( as defined by the `--poll_delay` parameter) until canceled. 
-It will send an email to the owner of every annotation_set that it completes.
+It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
+annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
-The [examples](examples) directory has some examples that you can use and/or adapt for 
+The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
-   arguments for filtering annotation_sets
-2. **[keras_cnn_bot.py](examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+   arguments for filtering annotation_sets and to keep running as a service.
+2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

### Comparing `sqapi-0.2/README.md` & `sqapi-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 ### Installation
 To install the `sqapi` module, you can use `pip`
 ```shell
 pip install sqapi 
 ```
 
-### Why & how
-The `sqapi` module helps to build the `HTTP` requests that are sent to the `API`. These are 
+### What is this?
+The `sqapi` module helps to build the `HTTP` requests that are sent to the [SQUIDLE+](squidle.org) `API`. These are 
 `GET`, `POST`, `PATCH` or `DELETE` requests. Setting `verbosity=2` on the `sqapi` module will print the `HTTP` 
 requests that are being made.
 
 `sqapi` takes care of authentication, and simplifies the creation of API queries. 
 For example:
 
 ```python
@@ -23,20 +23,23 @@
 
 sqapi = SQAPI(host=<HOST>,api_key=<API_KEY>, verbosity=2)  # instantiate the sqapi module
 r=sqapi.get(<ENDPOINT>)              # define a get request using a specific endpoint
 r.filter(<NAME>,<OPERATORE>,<VALUE>) # define a filter to compare a property with a value using an operator
 data = r.execute().json()            # perform the request & return result as JSON dict (don't set template)
 ```
 
+For more information about structuring queries, check out the [Making API queries](https://squidle.org/api/help?template=api_help_page.html#api_query)
+section of the SQ+ API documentation page.
+
 Instantiating `sqapi` without an API key argument will prompt for a user login, i.e.:
 ```python
 sqapi = SQAPI(host=<HOST>, verbosity=2)  # instantiate the sqapi module
 ```
 
-You can also use it to apply templates to the data that comes out of the API:
+You can also use it to apply built-in templates to the data that comes out of the API:
 ```python
 r.template(<TEMPLATE>)               # format the output of the request using an inbuilt HTML template
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
@@ -52,14 +55,17 @@
 mkdir sqbot_demo && cd sqbot_demo   # make a directory
 virtualenv -p python3 env           # create a virtual environment
 source env/bin/activate             # activate it
 pip install sqapi  # install sqapi
 ```
 
 #### 1. Create a bot class
+In this example, we'll create an automated classifier that suggests random label suggestions for an annotation_set. 
+It uses the `Annotator` class from the `sqapi.annotate` module, which does most of the heavy-lifting. The implementation
+of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
 from sqapi.request import query_filter as qf
@@ -94,31 +100,27 @@
     # Add an extra argument to the parser to get an annotation_set id to classify
     parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
     
     # Instantiate the bot class
     args = parser.parse_args()
     bot = RandoBOT(**vars(args))
     
-    # Initialise the request for the list of annotation_sets that you want classified
-    # only consider annotation_sets that do not already have suggestions from this user
-    r = bot.sqapi.get("/api/annotation_set")
-    r.filter_not(qf("children", "any", val=qf("user_id", "eq", bot.sqapi.current_user.get("id"))))
-
-    # filter annotation_sets within a nominated user_group 
-    # as specified by the extra parameter added to RandoBot.__init__
-    r.filter(name="id", op="in", val=args.annotation_set_id)
+    # Initialise the request for the annotation_set that you want classified
+    # update the ID to the ID you want
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
 
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
-This allows you to pass arguments from the command line, and to use help on how to use it:
+This allows you to pass arguments from the command line, and helps to show how to use it:
 ```shell
+# from the command line, run:
 python run_bot.py --help
 ```
 
 It will show you all the required parameters from the base class `Annotator` as well as any extra arguments added to the 
 `__init__` method of the `RandoBot` class. Parameter descriptions come from the comment block.
 
 #### 2. Create a Label Mapper File
@@ -132,31 +134,31 @@
   "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
   "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
   "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
 }
 ```
 
 #### 3. Run your bot
-Now you're ready to run your classifier RandoBot, by simply executing this from the command line:
+Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay 5 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
 ```
 
-This will get the list of annotation_sets contained in the user_group with the id of `55`
+This will run the classifier once on the annotation_set with an `ID=55`
 and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will continue this indefinitely in a loop every 5s ( as defined by the `--poll_delay` parameter) until canceled. 
-It will send an email to the owner of every annotation_set that it completes.
+It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
+annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
-The [examples](examples) directory has some examples that you can use and/or adapt for 
+The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
-   arguments for filtering annotation_sets
-2. **[keras_cnn_bot.py](examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+   arguments for filtering annotation_sets and to keep running as a service.
+2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

### Comparing `sqapi-0.2/setup.py` & `sqapi-0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sqapi',
-    version='0.2',
+    version='0.3',
     packages=['sqapi'],
     install_requires=['requests', 'numpy', 'opencv-python'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.',   # Give a short description about your library
     author='Greybits Engineering',                   # Type in your name
@@ -18,9 +18,11 @@
         'Intended Audience :: Developers',      # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
         'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 )
```

### Comparing `sqapi-0.2/sqapi/annotate.py` & `sqapi-0.3/sqapi/annotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :param label_map_file: path to a local file that contains the label mappings
         :param prob_thresh: probability threshold for submitted labels, only submitted if p > prob_thresh
         :param poll_delay: the poll delay for running the loop. To run once, set poll_delay = -1
         :param annotation_set_id: if supplied, will create suggested labels to the specific annotation_set with that ID
         :param affiliation_group_id: if supplied, will attempt to annotate all annotation_sets within an affiliation group
         :param user_group_id: if supplied, will attempt to annotate all annotation_sets within a user_group
         :param after_date: filter annotation_sets that were created after a specific date
-        :param host: the Squidle+ insrtance hostname
+        :param host: the Squidle+ instance hostname
         :param api_key: the API key for the user on that `host`. If omitted, you'll be asked to log in.
         :param verbosity: the verbosity of the output (0,1,2,3)
         :param email_results: flag to optionally send an email upon completion
         """
         annotator_info = annotator_info or self.__class__.__name__
         self.sqapi = SQAPI(host=host, api_key=api_key, verbosity=verbosity)
         self.annotator_info = annotator_info.format(user=self.sqapi.current_user)  #(annotator_name or self.sqapi.cliargs.annotator_name).format(user=self.sqapi.current_user)
```

### Comparing `sqapi-0.2/sqapi/api.py` & `sqapi-0.3/sqapi/api.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.2/sqapi/helpers.py` & `sqapi-0.3/sqapi/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             helptxt = f"{desc}\ndefault: {default}"
             parser.add_argument(f"--{name}", default=default, dest=param.name, type=type_, help=helptxt)
         # helptxt = f"{desc}\ntype: {txttype}  | default: {default}"
         # print(action)
         # parser.add_argument(f"--{name}", default=default, dest=param.name, type=type_, help=helptxt, action=action)
 
     for base in cls.__bases__:
-        parser = create_parser(base, parser=parser, create_subparser=False)
+        parser = create_parser(base, parser=parser)
     return parser
 
 
 def cli_init(cls, parser=None):
     params = create_parser(cls, parser=parser)
     args = params.parse_args()
     return cls(**vars(args))
```

### Comparing `sqapi-0.2/sqapi/media.py` & `sqapi-0.3/sqapi/media.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.2/sqapi/request.py` & `sqapi-0.3/sqapi/request.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.2/sqapi.egg-info/PKG-INFO` & `sqapi-0.3/sqapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.2
+Version: 0.3
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # SQAPI
 
 `sqapi` is a python package that simplifies interactions with the 
 [SQUIDLE+ API](https://squidle.org/api/help?template=api_help_page.html).
 It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 
 ### Installation
 To install the `sqapi` module, you can use `pip`
 ```shell
 pip install sqapi 
 ```
 
-### Why & how
-The `sqapi` module helps to build the `HTTP` requests that are sent to the `API`. These are 
+### What is this?
+The `sqapi` module helps to build the `HTTP` requests that are sent to the [SQUIDLE+](squidle.org) `API`. These are 
 `GET`, `POST`, `PATCH` or `DELETE` requests. Setting `verbosity=2` on the `sqapi` module will print the `HTTP` 
 requests that are being made.
 
 `sqapi` takes care of authentication, and simplifies the creation of API queries. 
 For example:
 
 ```python
@@ -42,20 +45,23 @@
 
 sqapi = SQAPI(host=<HOST>,api_key=<API_KEY>, verbosity=2)  # instantiate the sqapi module
 r=sqapi.get(<ENDPOINT>)              # define a get request using a specific endpoint
 r.filter(<NAME>,<OPERATORE>,<VALUE>) # define a filter to compare a property with a value using an operator
 data = r.execute().json()            # perform the request & return result as JSON dict (don't set template)
 ```
 
+For more information about structuring queries, check out the [Making API queries](https://squidle.org/api/help?template=api_help_page.html#api_query)
+section of the SQ+ API documentation page.
+
 Instantiating `sqapi` without an API key argument will prompt for a user login, i.e.:
 ```python
 sqapi = SQAPI(host=<HOST>, verbosity=2)  # instantiate the sqapi module
 ```
 
-You can also use it to apply templates to the data that comes out of the API:
+You can also use it to apply built-in templates to the data that comes out of the API:
 ```python
 r.template(<TEMPLATE>)               # format the output of the request using an inbuilt HTML template
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
@@ -71,14 +77,17 @@
 mkdir sqbot_demo && cd sqbot_demo   # make a directory
 virtualenv -p python3 env           # create a virtual environment
 source env/bin/activate             # activate it
 pip install sqapi  # install sqapi
 ```
 
 #### 1. Create a bot class
+In this example, we'll create an automated classifier that suggests random label suggestions for an annotation_set. 
+It uses the `Annotator` class from the `sqapi.annotate` module, which does most of the heavy-lifting. The implementation
+of the classifier is relatively straight forward.
 In your project directory, create a file named `run_bot.py`:
 
 ```python
 # run_bot.py
 import random
 from sqapi.annotate import Annotator
 from sqapi.request import query_filter as qf
@@ -113,31 +122,27 @@
     # Add an extra argument to the parser to get an annotation_set id to classify
     parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
     
     # Instantiate the bot class
     args = parser.parse_args()
     bot = RandoBOT(**vars(args))
     
-    # Initialise the request for the list of annotation_sets that you want classified
-    # only consider annotation_sets that do not already have suggestions from this user
-    r = bot.sqapi.get("/api/annotation_set")
-    r.filter_not(qf("children", "any", val=qf("user_id", "eq", bot.sqapi.current_user.get("id"))))
-
-    # filter annotation_sets within a nominated user_group 
-    # as specified by the extra parameter added to RandoBot.__init__
-    r.filter(name="id", op="in", val=args.annotation_set_id)
+    # Initialise the request for the annotation_set that you want classified
+    # update the ID to the ID you want
+    r = bot.sqapi.get("/api/annotation_set").filter(name="id", op="in", val=args.annotation_set_id)
 
     bot.start(r)
 ```
 
 The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
 signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
-This allows you to pass arguments from the command line, and to use help on how to use it:
+This allows you to pass arguments from the command line, and helps to show how to use it:
 ```shell
+# from the command line, run:
 python run_bot.py --help
 ```
 
 It will show you all the required parameters from the base class `Annotator` as well as any extra arguments added to the 
 `__init__` method of the `RandoBot` class. Parameter descriptions come from the comment block.
 
 #### 2. Create a Label Mapper File
@@ -151,31 +156,31 @@
   "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
   "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
   "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
 }
 ```
 
 #### 3. Run your bot
-Now you're ready to run your classifier RandoBot, by simply executing this from the command line:
+Now you're ready to run your classifier `RandoBot`, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay 5 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay -1 --email_results
 ```
 
-This will get the list of annotation_sets contained in the user_group with the id of `55`
+This will run the classifier once on the annotation_set with an `ID=55`
 and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
-It will continue this indefinitely in a loop every 5s ( as defined by the `--poll_delay` parameter) until canceled. 
-It will send an email to the owner of every annotation_set that it completes.
+It will run once (as defined by the `--poll_delay=-1` parameter) and it will send an email to the owner the
+annotation_set once complete.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
-The [examples](examples) directory has some examples that you can use and/or adapt for 
+The [examples](https://bitbucket.org/ariell/pysq/src/master/examples/) directory has some examples that you can use and/or adapt for 
 your purposes. Specifically with regard to classifiers:
 
-1. **[demo_randobot.py](examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
-   arguments for filtering annotation_sets
-2. **[keras_cnn_bot.py](examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
+1. **[demo_randobot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+   arguments for filtering annotation_sets and to keep running as a service.
+2. **[keras_cnn_bot.py](https://bitbucket.org/ariell/pysq/src/master/examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
    classifying points in images. The class received a number of additional parameters that can all be passed in as 
    command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
    include additional model-specific arguments along with other parameters, as well as how to process the images and 
    for a real classifier.
```

