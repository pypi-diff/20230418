# Comparing `tmp/hugging_py_face-0.0.1.tar.gz` & `tmp/hugging_py_face-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.0.1.tar", last modified: Sun Apr 16 19:39:03 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.1.0.tar", last modified: Tue Apr 18 10:56:29 2023, max compression
```

## Comparing `hugging_py_face-0.0.1.tar` & `hugging_py_face-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/
--rw-rw-rw-   0        0        0      523 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/hugging_py_face/
--rw-rw-rw-   0        0        0      385 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0        0 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0     1419 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/computer_vision.py
--rw-rw-rw-   0        0        0      320 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0     1053 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    15820 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0      523 2023-04-16 19:39:02.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:39:02.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-16 19:39:02.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-16 19:39:02.000000 hugging_py_face-0.0.1/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 19:39:03.000000 hugging_py_face-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-04-16 19:38:38.000000 hugging_py_face-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/
+-rw-rw-rw-   0        0        0     5915 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4550 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face/
+-rw-rw-rw-   0        0        0      422 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      112 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3877 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0     2844 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/computer_vision.py
+-rw-rw-rw-   0        0        0      320 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0     1479 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    17241 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     5915 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:56:29.000000 hugging_py_face-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      940 2023-04-18 10:56:11.000000 hugging_py_face-0.1.0/setup.py
```

### Comparing `hugging_py_face-0.0.1/hugging_py_face/computer_vision.py` & `hugging_py_face-0.1.0/hugging_py_face/computer_vision.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,48 @@
-from typing import Text, List, Optional
+from pandas import DataFrame
+from typing import Text, List, Optional, Union
+
 from .multimedia_processing import MultimediaProcessing
 
 
 class ComputerVision(MultimediaProcessing):
     def __init__(self, api_token):
         super().__init__(api_token)
 
-    def image_classification(self, input: Text, model: Optional[Text] = None) -> List:
+    def image_classification(self, inputs: Union[Text, List], model: Optional[Text] = None) -> List:
         """
         Classify an image from a file path or an url.
 
-        :param input: the file path or url to the image to classify
+        :param inputs: a string or a list of strings of the file paths or urls of the images to classify.
+        :param model: the model to use for the image classification task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a list of dictionaries each containing the label and the confidence score for that label.
+        """
+        if type(inputs) == list:
+            return self._query_in_list(inputs, model=model, task="image-classification")
+        elif type(inputs) == str:
+            return self._query(inputs, model=model, task="image-classification")
+
+    def image_classification_in_df(self, df: DataFrame, column: Text, model: Optional[Text] = None) -> DataFrame:
+        """
+        Classify images from a dataframe.
+
+        :param df: a pandas DataFrame containing the images to classify.
+        :param column: the name of the column containing the file paths or urls of the images to classify.
         :param model: the model to use for the image classification task. If not provided, the recommended model from Hugging Face will be used.
-        :return: a list of dictionaries each containing the label and the confidence score for that label
+        :return: a pandas DataFrame with the label for the images. Each label added will be the one with the highest confidence score for that particular image. The label will be added as a new column called 'predictions' to the original DataFrame.
         """
-        return self._query(input, model=model, task="image-classification")
+        predictions = self._query_in_df(df, column, model=model, task="image-classification")
+        df["predictions"] = [prediction[0]['label'] for prediction in predictions]
+        return df
 
-    def object_detection(self, input: Text, model: Optional[Text] = None) -> List:
+    def object_detection(self, inputs: Union[Text, List], model: Optional[Text] = None) -> List:
         """
         Perform object detection on an image from a file path or an url.
 
-        :param input: the file path or url to the image to perform object detection on
+        :param inputs: a string or a list of strings of the file paths or urls of the images to perform object detection on.
         :param model: the model to use for the object detection task. If not provided, the recommended model from Hugging Face will be used.
-        :return: a list of dictionaries each containing the label, the confidence score for that label, and the bounding box coordinates
+        :return: a list of dictionaries each containing the label, the confidence score for that label, and the bounding box coordinates.
         """
-        return self._query(input, model=model, task="object-detection")
+        if type(inputs) == list:
+            return self._query(inputs, model=model, task="object-detection")
+        elif type(inputs) == str:
+            return self._query(inputs, model=model, task="object-detection")
```

### Comparing `hugging_py_face-0.0.1/hugging_py_face/nlp.py` & `hugging_py_face-0.1.0/hugging_py_face/nlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,19 +94,17 @@
         return df
 
     def question_answering(self, question: Text, context: Text, model: Optional[Text] = None) -> Dict:
         """
         Answer a question using the provided context.
 
         :param question: a string of the question to be answered.
-        :param context: a string of context.
+        :param context: a string of context. This field is required for the question answering task and cannot be left empty.
         :param model: the model to use for the question answering task. If not provided, the recommended model from Hugging Face will be used.
         :return: a dict of the answer.
-
-        # TODO: check if questions can be answered without context
         """
         return self._query(
             {
                 "question": question,
                 "context": context
             },
             model=model,
@@ -166,14 +164,29 @@
         :param parameters: a dict of parameters. For more information, see the `detailed parameters for the text generation task <https://huggingface.co/docs/api-inference/detailed_parameters#text-generation-task>`_.
         :param options: a dict of options. For more information, see the `detailed parameters for the text generation task <https://huggingface.co/docs/api-inference/detailed_parameters#text-generation-task>`_.
         :param model: the model to use for the text generation task. If not provided, the recommended model from Hugging Face will be used.
         :return: a dict or a list of dicts containing the generated text.
         """
         return self._query(text, parameters=parameters, options=options, model=model, task='text-generation')
 
+    def text_generation_in_df(self, df: DataFrame, column: Text, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> DataFrame:
+        """
+        Continue text from a prompt in the column of a DataFrame.
+
+        :param df: a pandas DataFrame containing the strings to be generated from.
+        :param column: the column containing the strings to be generated from.
+        :param parameters: a dict of parameters. For more information, see the `detailed parameters for the text generation task <https://huggingface.co/docs/api-inference/detailed_parameters#text-generation-task>`_.
+        :param options: a dict of options. For more information, see the `detailed parameters for the text generation task <https://huggingface.co/docs/api-inference/detailed_parameters#text-generation-task>`_.
+        :param model: the model to use for the text generation task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a pandas DataFrame with the generated text. The generated text will be added as a new column called 'predictions' to the original DataFrame.
+        """
+        predictions = self._query_in_df(df, column, parameters=parameters, options=options, model=model, task='text-generation')
+        df['predictions'] = [prediction[0]['generated_text'] for prediction in predictions]
+        return df
+
     def zero_shot_classification(self, text: Union[Text, List], candidate_labels: List, parameters: Optional[Dict] = {}, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Classify a sentence/paragraph to one of the candidate labels provided.
 
         :param text: a string or list of strings to be classified.
         :param candidate_labels: a list of strings that are potential classes for inputs.
         :param parameters: a dict of parameters excluding candidate_labels which is passed in as a separate argument. For more information, see the `detailed parameters for the zero shot classification task <https://huggingface.co/docs/api-inference/detailed_parameters#zeroshot-classification-task>`_.
@@ -187,15 +200,15 @@
             text,
             parameters=parameters,
             options=options,
             model=model,
             task='zero-shot-classification'
         )
 
-    def conversational(self, text: Union[Text, List], past_user_inputs: Optional[Text] = None, generated_responses: Optional[Text] = None, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
+    def conversational(self, text: Union[Text, List], past_user_inputs: Optional[List] = None, generated_responses: Optional[List] = None, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Corresponds to any chatbot like structure: pass in some text along with the past_user_inputs and generated_responses to receive a response.
 
         :param text: a string or list of strings representing the last input(s) from the user in the conversation.
         :param past_user_inputs: a list of strings corresponding to the earlier replies from the user. Should be of the same length of generated_responses. Each response from the bot will contain past_user_inputs previously passed into the model.
         :param generated_responses: a list of strings corresponding to the earlier replies from the model. Each response from the bot will contain generated_responses from earlier replies from the model.
         :param parameters: a dict of parameters. For more information, see the `detailed parameters for the conversational task <https://huggingface.co/docs/api-inference/detailed_parameters#conversational-task>`_.
```

### Comparing `hugging_py_face-0.0.1/setup.py` & `hugging_py_face-0.1.0/setup.py`

 * *Files identical despite different names*

