# Comparing `tmp/sqapi-0.1.tar.gz` & `tmp/sqapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqapi-0.1.tar", last modified: Mon Apr 17 06:47:57 2023, max compression
+gzip compressed data, was "sqapi-0.2.tar", last modified: Tue Apr 18 00:18:39 2023, max compression
```

## Comparing `sqapi-0.1.tar` & `sqapi-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-17 06:47:57.166658 sqapi-0.1/
--rw-r--r--   0 ariell     (501) staff       (20)      860 2023-04-17 06:47:57.166716 sqapi-0.1/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)     6211 2023-04-17 02:32:12.000000 sqapi-0.1/README.md
--rw-r--r--   0 ariell     (501) staff       (20)       79 2023-04-17 06:47:57.166942 sqapi-0.1/setup.cfg
--rw-r--r--   0 ariell     (501) staff       (20)     1590 2023-04-17 06:41:39.000000 sqapi-0.1/setup.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-17 06:47:57.165997 sqapi-0.1/sqapi/
--rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.1/sqapi/__init__.py
--rw-r--r--   0 ariell     (501) staff       (20)    12682 2023-04-07 10:49:09.000000 sqapi-0.1/sqapi/annotate.py
--rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.1/sqapi/api.py
--rw-r--r--   0 ariell     (501) staff       (20)     4926 2023-04-07 05:24:54.000000 sqapi-0.1/sqapi/helpers.py
--rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.1/sqapi/media.py
--rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.1/sqapi/request.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-17 06:47:57.166557 sqapi-0.1/sqapi.egg-info/
--rw-r--r--   0 ariell     (501) staff       (20)      860 2023-04-17 06:47:57.000000 sqapi-0.1/sqapi.egg-info/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)      270 2023-04-17 06:47:57.000000 sqapi-0.1/sqapi.egg-info/SOURCES.txt
--rw-r--r--   0 ariell     (501) staff       (20)        1 2023-04-17 06:47:57.000000 sqapi-0.1/sqapi.egg-info/dependency_links.txt
--rw-r--r--   0 ariell     (501) staff       (20)       29 2023-04-17 06:47:57.000000 sqapi-0.1/sqapi.egg-info/requires.txt
--rw-r--r--   0 ariell     (501) staff       (20)        6 2023-04-17 06:47:57.000000 sqapi-0.1/sqapi.egg-info/top_level.txt
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.105114 sqapi-0.2/
+-rw-r--r--   0 ariell     (501) staff       (20)     8606 2023-04-18 00:18:39.105195 sqapi-0.2/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)     7705 2023-04-18 00:15:58.000000 sqapi-0.2/README.md
+-rw-r--r--   0 ariell     (501) staff       (20)       79 2023-04-18 00:18:39.105479 sqapi-0.2/setup.cfg
+-rw-r--r--   0 ariell     (501) staff       (20)     1688 2023-04-18 00:18:11.000000 sqapi-0.2/setup.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.104467 sqapi-0.2/sqapi/
+-rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.2/sqapi/__init__.py
+-rw-r--r--   0 ariell     (501) staff       (20)    12682 2023-04-07 10:49:09.000000 sqapi-0.2/sqapi/annotate.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.2/sqapi/api.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4926 2023-04-07 05:24:54.000000 sqapi-0.2/sqapi/helpers.py
+-rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.2/sqapi/media.py
+-rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.2/sqapi/request.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 00:18:39.105021 sqapi-0.2/sqapi.egg-info/
+-rw-r--r--   0 ariell     (501) staff       (20)     8606 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)      270 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        1 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ariell     (501) staff       (20)       29 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/requires.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        6 2023-04-18 00:18:39.000000 sqapi-0.2/sqapi.egg-info/top_level.txt
```

### Comparing `sqapi-0.1/README.md` & `sqapi-0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 `sqapi` is a python package that simplifies interactions with the 
 [SQUIDLE+ API](https://squidle.org/api/help?template=api_help_page.html).
 It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 
 ### Installation
 To install the `sqapi` module, you can use `pip`
 ```shell
-pip install git+https://ariell@bitbucket.org/ariell/pysq.git 
+pip install sqapi 
 ```
 
 ### Why & how
 The `sqapi` module helps to build the `HTTP` requests that are sent to the `API`. These are 
 `GET`, `POST`, `PATCH` or `DELETE` requests. Setting `verbosity=2` on the `sqapi` module will print the `HTTP` 
 requests that are being made.
 
@@ -37,26 +37,33 @@
 r.template(<TEMPLATE>)               # format the output of the request using an inbuilt HTML template
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
 
-## Example of AUTO Annotate Bot
+## Examples
+### Random annotation BOT
+This is an example of an automated labelling bot that selects random class labels to assign to points.
+It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
+Machine Learning algorithm for label suggestions.
+
 Set up the environment and a mini project
 ```shell
 mkdir sqbot_demo && cd sqbot_demo   # make a directory
 virtualenv -p python3 env           # create a virtual environment
 source env/bin/activate             # activate it
-pip install git+https://ariell@bitbucket.org/ariell/pysq.git  # install sqapi
+pip install sqapi  # install sqapi
 ```
 
-In your project directory, create a file named `run_bot.py` with the following content:
+#### 1. Create a bot class
+In your project directory, create a file named `run_bot.py`:
 
 ```python
+# run_bot.py
 import random
 from sqapi.annotate import Annotator
 from sqapi.request import query_filter as qf
 from sqapi.helpers import cli_init, create_parser
 from sqapi.media import SQMediaObject
 
 
@@ -77,58 +84,79 @@
         classifier_code = random.sample(self.possible_codes, 1)[0]  # get a random code
         prob = round(random.random(), 2)  # generate a random probability
         # TODO: use the image_data, x and y point position to generate a real label and prob
         return classifier_code, prob
 
 
 if __name__ == '__main__':
-    bot = cli_init(RandoBOT)  # convenience method that initialises the class from command line arguments
-
-    # Initialise the list of annotation_set that you want classified
+    # Get the cli arguments from the Class __init__ function signatures
+    parser = create_parser(RandoBOT)  # convenient method to build a parser from the bot class
+    
+    # Add an extra argument to the parser to get an annotation_set id to classify
+    parser.add_argument('--annotation_set_id', help="Process annotation_set with specific ID", type=int)
+    
+    # Instantiate the bot class
+    args = parser.parse_args()
+    bot = RandoBOT(**vars(args))
+    
+    # Initialise the request for the list of annotation_sets that you want classified
     # only consider annotation_sets that do not already have suggestions from this user
     r = bot.sqapi.get("/api/annotation_set")
-        .filter_not(qf("children", "any", val=qf("user_id", "eq", bot.sqapi.current_user.get("id"))))
+    r.filter_not(qf("children", "any", val=qf("user_id", "eq", bot.sqapi.current_user.get("id"))))
 
     # filter annotation_sets within a nominated user_group 
     # as specified by the extra parameter added to RandoBot.__init__
-    r.filter(name="usergroups", op="any", val=dict(name="id", op="eq", val=bot.user_group_id))
+    r.filter(name="id", op="in", val=args.annotation_set_id)
 
     bot.start(r)
 ```
 
-The `cli_init` method is a convenience tool that allows you to initialise the Class from the command line based on the 
-signature of the `__init__` methods for that class and all base classes.
+The `create_parser` method is a convenience tool that allows you to build a command line parser from the  
+signature of the `__init__` methods for the RandoBot class and all inherited base classes (eg: Annotator).
 
-To see the parameters and how to use it from the command line, run the following:
+This allows you to pass arguments from the command line, and to use help on how to use it:
 ```shell
 python run_bot.py --help
 ```
 
 It will show you all the required parameters from the base class `Annotator` as well as any extra arguments added to the 
-`__init__` method of the `RandoBot` class.
+`__init__` method of the `RandoBot` class. Parameter descriptions come from the comment block.
 
-You also need to create a label map file to pass into the `--label_map_file` argument. 
+#### 2. Create a Label Mapper File
+Before you run it, you also need to create a label map file to pass into the `--label_map_file` argument. 
 This maps the outputs from your classifier to real class labels in the system.
 
 In your project directory, create a file named `rando_bot_label_map.json` 
 with the following content:
 ```json
 {
   "ECK": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"214344"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"54079009"}}]}],
   "ASC": [{"or":[{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"1839"}},{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"35000000"}}]}],
   "SUB": [{"name":"vocab_elements","op":"any","val":{"name":"key","op":"eq","val":"82001000"}}]
 }
 ```
 
+#### 3. Run your bot
 Now you're ready to run your classifier RandoBot, by simply executing this from the command line:
 ```shell
-python run_bot.py --label_map_file rando_bot_label_map.json --user_group_id=55 --poll_delay 5 --email_results
+python run_bot.py --label_map_file rando_bot_label_map.json --annotation_set_id=55 --poll_delay 5 --email_results
 ```
 
 This will get the list of annotation_sets contained in the user_group with the id of `55`
 and attempt to provide automated suggestions on the labels it contains using random class allocations and probabilities. 
 It will continue this indefinitely in a loop every 5s ( as defined by the `--poll_delay` parameter) until canceled. 
 It will send an email to the owner of every annotation_set that it completes.
 
 Now all that's left is for you to make the labels and probabilities real, and bob's your uncle,
 you've made an automated classifier.
 
+The [examples](examples) directory has some examples that you can use and/or adapt for 
+your purposes. Specifically with regard to classifiers:
+
+1. **[demo_randobot.py](examples/bots/demo_randobot.py)**: same as example above, but with additional command line 
+   arguments for filtering annotation_sets
+2. **[keras_cnn_bot.py](examples/bots/keras_cnn_bot.py)**: a real classifier that uses a tensor_flow/keras model for 
+   classifying points in images. The class received a number of additional parameters that can all be passed in as 
+   command line arguments. Run `python keras_cnn_bot.py --help` for more information. This shows an example of how to 
+   include additional model-specific arguments along with other parameters, as well as how to process the images and 
+   for a real classifier.
+
```

### Comparing `sqapi-0.1/setup.py` & `sqapi-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup
 
 setup(
     name='sqapi',
-    version='0.1',
+    version='0.2',
     packages=['sqapi'],
     install_requires=['requests', 'numpy', 'opencv-python'],
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.',   # Give a short description about your library
     author='Greybits Engineering',                   # Type in your name
     url='https://bitbucket.org/ariell/pysq',   # Provide either the link to your github or to your website
     download_url='https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz',    # I explain this later on
     keywords=['SQUIDLE+', 'API', 'SQ', 'Machine Learning'],   # Keywords that define your package best
     classifiers=[
```

### Comparing `sqapi-0.1/sqapi/annotate.py` & `sqapi-0.2/sqapi/annotate.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.1/sqapi/api.py` & `sqapi-0.2/sqapi/api.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.1/sqapi/helpers.py` & `sqapi-0.2/sqapi/helpers.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.1/sqapi/media.py` & `sqapi-0.2/sqapi/media.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.1/sqapi/request.py` & `sqapi-0.2/sqapi/request.py`

 * *Files identical despite different names*

