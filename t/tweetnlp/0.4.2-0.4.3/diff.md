# Comparing `tmp/tweetnlp-0.4.2.tar.gz` & `tmp/tweetnlp-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweetnlp-0.4.2.tar", last modified: Sat Jan 28 20:38:56 2023, max compression
+gzip compressed data, was "tweetnlp-0.4.3.tar", last modified: Tue Apr 18 17:07:34 2023, max compression
```

## Comparing `tweetnlp-0.4.2.tar` & `tweetnlp-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.163858 tweetnlp-0.4.2/
--rw-r--r--   0 asahi      (501) staff       (20)     1066 2022-05-24 10:28:20.000000 tweetnlp-0.4.2/LICENSE
--rw-r--r--   0 asahi      (501) staff       (20)    35701 2023-01-28 20:38:56.164330 tweetnlp-0.4.2/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)    34998 2023-01-28 20:38:29.000000 tweetnlp-0.4.2/README.md
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-01-28 20:38:56.165163 tweetnlp-0.4.2/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1626 2023-01-28 20:38:38.000000 tweetnlp-0.4.2/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.147251 tweetnlp-0.4.2/tweetnlp/
--rw-r--r--   0 asahi      (501) staff       (20)      537 2022-11-30 22:45:03.000000 tweetnlp-0.4.2/tweetnlp/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3699 2022-12-04 19:32:28.000000 tweetnlp-0.4.2/tweetnlp/loader.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.149852 tweetnlp-0.4.2/tweetnlp/mlm/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:37:45.000000 tweetnlp-0.4.2/tweetnlp/mlm/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     4095 2022-11-28 13:37:18.000000 tweetnlp-0.4.2/tweetnlp/mlm/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.154259 tweetnlp-0.4.2/tweetnlp/ner/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-22 15:10:27.000000 tweetnlp-0.4.2/tweetnlp/ner/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    28930 2022-11-26 19:43:35.000000 tweetnlp-0.4.2/tweetnlp/ner/allennlp_crf.py
--rw-r--r--   0 asahi      (501) staff       (20)      878 2022-11-30 22:45:03.000000 tweetnlp-0.4.2/tweetnlp/ner/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     7056 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/ner/model.py
--rw-r--r--   0 asahi      (501) staff       (20)        6 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/ner/trainer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.156075 tweetnlp-0.4.2/tweetnlp/question_answer_generation/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answer_generation/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)      626 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answer_generation/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     2861 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answer_generation/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.157695 tweetnlp-0.4.2/tweetnlp/question_answering/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answering/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)      598 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answering/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     1651 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/question_answering/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.158536 tweetnlp-0.4.2/tweetnlp/sentence_embedding/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:34:58.000000 tweetnlp-0.4.2/tweetnlp/sentence_embedding/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     1874 2022-11-28 13:42:40.000000 tweetnlp-0.4.2/tweetnlp/sentence_embedding/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.162474 tweetnlp-0.4.2/tweetnlp/text_classification/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-23 17:46:06.000000 tweetnlp-0.4.2/tweetnlp/text_classification/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2435 2022-11-30 22:45:03.000000 tweetnlp-0.4.2/tweetnlp/text_classification/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)    10083 2022-12-04 19:13:00.000000 tweetnlp-0.4.2/tweetnlp/text_classification/model.py
--rw-r--r--   0 asahi      (501) staff       (20)     5051 2022-12-02 18:24:51.000000 tweetnlp-0.4.2/tweetnlp/text_classification/readme_template.py
--rw-r--r--   0 asahi      (501) staff       (20)    15101 2022-12-02 18:24:51.000000 tweetnlp-0.4.2/tweetnlp/text_classification/trainer.py
--rw-r--r--   0 asahi      (501) staff       (20)     3986 2022-11-30 22:45:03.000000 tweetnlp-0.4.2/tweetnlp/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-01-28 20:38:56.149384 tweetnlp-0.4.2/tweetnlp.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)    35701 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      998 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       20 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/entry_points.txt
--rw-r--r--   0 asahi      (501) staff       (20)      112 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        9 2023-01-28 20:38:56.000000 tweetnlp-0.4.2/tweetnlp.egg-info/top_level.txt
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.936249 tweetnlp-0.4.3/
+-rw-r--r--   0 asahi      (501) staff       (20)     1066 2022-05-24 10:28:20.000000 tweetnlp-0.4.3/LICENSE
+-rw-r--r--   0 asahi      (501) staff       (20)    37239 2023-04-18 17:07:34.936549 tweetnlp-0.4.3/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)    36536 2023-04-18 17:07:13.000000 tweetnlp-0.4.3/README.md
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-04-18 17:07:34.937342 tweetnlp-0.4.3/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1626 2023-04-18 16:55:23.000000 tweetnlp-0.4.3/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.919638 tweetnlp-0.4.3/tweetnlp/
+-rw-r--r--   0 asahi      (501) staff       (20)      537 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3699 2022-12-04 19:32:28.000000 tweetnlp-0.4.3/tweetnlp/loader.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.922871 tweetnlp-0.4.3/tweetnlp/mlm/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:37:45.000000 tweetnlp-0.4.3/tweetnlp/mlm/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4095 2022-11-28 13:37:18.000000 tweetnlp-0.4.3/tweetnlp/mlm/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.926859 tweetnlp-0.4.3/tweetnlp/ner/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-22 15:10:27.000000 tweetnlp-0.4.3/tweetnlp/ner/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    28930 2022-11-26 19:43:35.000000 tweetnlp-0.4.3/tweetnlp/ner/allennlp_crf.py
+-rw-r--r--   0 asahi      (501) staff       (20)      878 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/ner/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7056 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/ner/model.py
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/ner/trainer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.928380 tweetnlp-0.4.3/tweetnlp/question_answer_generation/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)      626 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2861 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.930590 tweetnlp-0.4.3/tweetnlp/question_answering/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)      598 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1651 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.931831 tweetnlp-0.4.3/tweetnlp/sentence_embedding/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:34:58.000000 tweetnlp-0.4.3/tweetnlp/sentence_embedding/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1874 2022-11-28 13:42:40.000000 tweetnlp-0.4.3/tweetnlp/sentence_embedding/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.935444 tweetnlp-0.4.3/tweetnlp/text_classification/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-23 17:46:06.000000 tweetnlp-0.4.3/tweetnlp/text_classification/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2435 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/text_classification/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)    10261 2023-04-18 16:58:10.000000 tweetnlp-0.4.3/tweetnlp/text_classification/model.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5051 2022-12-02 18:24:51.000000 tweetnlp-0.4.3/tweetnlp/text_classification/readme_template.py
+-rw-r--r--   0 asahi      (501) staff       (20)    15101 2022-12-02 18:24:51.000000 tweetnlp-0.4.3/tweetnlp/text_classification/trainer.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3986 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.922433 tweetnlp-0.4.3/tweetnlp.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)    37239 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      998 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       20 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/entry_points.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      112 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        9 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/top_level.txt
```

### Comparing `tweetnlp-0.4.2/LICENSE` & `tweetnlp-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/PKG-INFO` & `tweetnlp-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tweetnlp
-Version: 0.4.2
+Version: 0.4.3
 Summary: NLP library for Twitter.
 Home-page: https://github.com/cardiffnlp/tweetnlp
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT
-Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.2.tar.gz
+Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.3.tar.gz
 Keywords: tweet,nlp,language-model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -223,25 +223,48 @@
 ```
 
 - ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
 
 ```python
 import tweetnlp
 
-# MODEL
+# MULTI-LABEL MODEL 
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
 >>> {'label': 'joy'}
+# Note: the probability of the multi-label model is the output of sigmoid function on binary prediction whether each topic is positive or negative.
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
+>>> {'label': 'joy',
+ 'probability': {'anger': 0.00025800734874792397,
+  'anticipation': 0.0005329723935574293,
+  'disgust': 0.00026112011983059347,
+  'fear': 0.00027552215033210814,
+  'joy': 0.7721399068832397,
+  'love': 0.1806265264749527,
+  'optimism': 0.04208092764019966,
+  'pessimism': 0.00025325192837044597,
+  'sadness': 0.0006160663324408233,
+  'surprise': 0.0005619609728455544,
+  'trust': 0.002393839880824089}}
+
+# SINGLE-LABEL MODEL
+model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
+>>> {'label': 'joy'}
+# NOTE: the probability of the sinlge-label model the softmax over the label.
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
 >>> {'label': 'optimism', 'probability': {'joy': 0.01367587223649025, 'optimism': 0.7345258593559265, 'anger': 0.1770714670419693, 'sadness': 0.07472680509090424}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emotion')
 ```
 
+WARNING: The single-label and multi-label emotion model have diiferent label set (single-label has four classes of 'joy'/'optimism'/'anger'/'sadness', 
+while multi-label has eleven classes of 'joy'/'optimism'/'anger'/'sadness'/'love'/'trust'/'fear'/'surprise'/'anticipation'/'disgust'/'pessimism').
+
 ### Named Entity Recognition
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp#scrollTo=WeREiLEjBlrj)
 
 This module consists of a named-entity recognition (NER) model specifically trained for tweets. The model is instantiated by `tweetnlp.load_model("ner")`, and runs the prediction by giving a text or a list of texts as argument to the `ner` function (check the paper [here](https://arxiv.org/abs/2210.03797), or the [huggingface dataset page](https://huggingface.co/datasets/tner/tweetner7)). 
 
 ```python3
 import tweetnlp
@@ -393,19 +416,20 @@
 | Task                              | Model                                                                                                                                                   | Dataset |
 |-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
 |Topic Classification (single-label)| [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all) | [cardiffnlp/tweet_topic_single](https://huggingface.co/datasets/cardiffnlp/tweet_topic_single) |
 |Topic Classification (multi-label) | [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all)   | [cardiffnlp/tweet_topic_multi](https://huggingface.co/datasets/cardiffnlp/tweet_topic_multi) |
 |Sentiment Analysis (Multilingual)  | [cardiffnlp/twitter-xlm-roberta-base-sentiment](https://huggingface.co/cardiffnlp/twitter-xlm-roberta-base-sentiment)                                   | [cardiffnlp/tweet_sentiment_multilingual](https://huggingface.co/datasets/cardiffnlp/tweet_sentiment_multilingual) |
 |Sentiment Analysis                 | [cardiffnlp/twitter-roberta-base-sentiment-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment-latest)                             | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Irony Detection                    | [cardiffnlp/twitter-roberta-base-irony](https://huggingface.co/cardiffnlp/twitter-roberta-base-irony)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate)                                                     | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate-latest)                                       | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Offensive Detection                | [cardiffnlp/twitter-roberta-base-offensive](https://huggingface.co/cardiffnlp/twitter-roberta-base-offensive)                                           | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Emoji Prediction                   | [cardiffnlp/twitter-roberta-base-emoji](https://huggingface.co/cardiffnlp/twitter-roberta-base-emoji)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Emotion Analysis                   | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                        | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
+|Emotion Analysis (single-label)    | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Emotion Analysis (multi-label)     | [cardiffnlp/twitter-roberta-base-emotion-multilabel-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion-multilabel-latest)           | TBA |
+|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                             | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
 |Question Answering                 | [lmqg/t5-small-tweetqa-qa](https://huggingface.co/lmqg/t5-small-tweetqa-qa)                                                                             | [lmqg/qg_tweetqa](https://huggingface.co/datasets/lmqg/qg_tweetqa) |
 |Question Answer Generation         | [lmqg/t5-base-tweetqa-qag](https://huggingface.co/lmqg/t5-base-tweetqa-qag)                                                                             | [lmqg/qag_tweetqa](https://huggingface.co/datasets/lmqg/qag_tweetqa) |
 |Language Modeling                  | [cardiffnlp/twitter-roberta-base-2021-124m](https://huggingface.co/cardiffnlp/twitter-roberta-base-2021-124m)                                           | TBA |
 |Tweet Embedding                    | [cambridgeltl/tweet-roberta-base-embeddings-v1](https://huggingface.co/cambridgeltl/tweet-roberta-base-embeddings-v1)                                   | TBA |
 
 
 To use an other model from local/huggingface modelhub, one can simply provide the model path/alias to the `load_model` function.
```

### Comparing `tweetnlp-0.4.2/README.md` & `tweetnlp-0.4.3/tweetnlp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: tweetnlp
+Version: 0.4.3
+Summary: NLP library for Twitter.
+Home-page: https://github.com/cardiffnlp/tweetnlp
+Author: Asahi Ushio
+Author-email: asahi1992ushio@gmail.com
+License: MIT
+Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.3.tar.gz
+Keywords: tweet,nlp,language-model
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/tweetnlp/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/tweetnlp.svg)](https://badge.fury.io/py/tweetnlp)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 [![PyPI status](https://img.shields.io/pypi/status/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 
 # TweetNLP
 TweetNLP for all the NLP enthusiasts working on Twitter! 
@@ -202,25 +223,48 @@
 ```
 
 - ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
 
 ```python
 import tweetnlp
 
-# MODEL
+# MULTI-LABEL MODEL 
+model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
+>>> {'label': 'joy'}
+# Note: the probability of the multi-label model is the output of sigmoid function on binary prediction whether each topic is positive or negative.
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
+>>> {'label': 'joy',
+ 'probability': {'anger': 0.00025800734874792397,
+  'anticipation': 0.0005329723935574293,
+  'disgust': 0.00026112011983059347,
+  'fear': 0.00027552215033210814,
+  'joy': 0.7721399068832397,
+  'love': 0.1806265264749527,
+  'optimism': 0.04208092764019966,
+  'pessimism': 0.00025325192837044597,
+  'sadness': 0.0006160663324408233,
+  'surprise': 0.0005619609728455544,
+  'trust': 0.002393839880824089}}
+
+# SINGLE-LABEL MODEL
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
 >>> {'label': 'joy'}
+# NOTE: the probability of the sinlge-label model the softmax over the label.
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
 >>> {'label': 'optimism', 'probability': {'joy': 0.01367587223649025, 'optimism': 0.7345258593559265, 'anger': 0.1770714670419693, 'sadness': 0.07472680509090424}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emotion')
 ```
 
+WARNING: The single-label and multi-label emotion model have diiferent label set (single-label has four classes of 'joy'/'optimism'/'anger'/'sadness', 
+while multi-label has eleven classes of 'joy'/'optimism'/'anger'/'sadness'/'love'/'trust'/'fear'/'surprise'/'anticipation'/'disgust'/'pessimism').
+
 ### Named Entity Recognition
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp#scrollTo=WeREiLEjBlrj)
 
 This module consists of a named-entity recognition (NER) model specifically trained for tweets. The model is instantiated by `tweetnlp.load_model("ner")`, and runs the prediction by giving a text or a list of texts as argument to the `ner` function (check the paper [here](https://arxiv.org/abs/2210.03797), or the [huggingface dataset page](https://huggingface.co/datasets/tner/tweetner7)). 
 
 ```python3
 import tweetnlp
@@ -372,19 +416,20 @@
 | Task                              | Model                                                                                                                                                   | Dataset |
 |-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
 |Topic Classification (single-label)| [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all) | [cardiffnlp/tweet_topic_single](https://huggingface.co/datasets/cardiffnlp/tweet_topic_single) |
 |Topic Classification (multi-label) | [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all)   | [cardiffnlp/tweet_topic_multi](https://huggingface.co/datasets/cardiffnlp/tweet_topic_multi) |
 |Sentiment Analysis (Multilingual)  | [cardiffnlp/twitter-xlm-roberta-base-sentiment](https://huggingface.co/cardiffnlp/twitter-xlm-roberta-base-sentiment)                                   | [cardiffnlp/tweet_sentiment_multilingual](https://huggingface.co/datasets/cardiffnlp/tweet_sentiment_multilingual) |
 |Sentiment Analysis                 | [cardiffnlp/twitter-roberta-base-sentiment-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment-latest)                             | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Irony Detection                    | [cardiffnlp/twitter-roberta-base-irony](https://huggingface.co/cardiffnlp/twitter-roberta-base-irony)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate)                                                     | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate-latest)                                       | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Offensive Detection                | [cardiffnlp/twitter-roberta-base-offensive](https://huggingface.co/cardiffnlp/twitter-roberta-base-offensive)                                           | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Emoji Prediction                   | [cardiffnlp/twitter-roberta-base-emoji](https://huggingface.co/cardiffnlp/twitter-roberta-base-emoji)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Emotion Analysis                   | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                        | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
+|Emotion Analysis (single-label)    | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Emotion Analysis (multi-label)     | [cardiffnlp/twitter-roberta-base-emotion-multilabel-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion-multilabel-latest)           | TBA |
+|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                             | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
 |Question Answering                 | [lmqg/t5-small-tweetqa-qa](https://huggingface.co/lmqg/t5-small-tweetqa-qa)                                                                             | [lmqg/qg_tweetqa](https://huggingface.co/datasets/lmqg/qg_tweetqa) |
 |Question Answer Generation         | [lmqg/t5-base-tweetqa-qag](https://huggingface.co/lmqg/t5-base-tweetqa-qag)                                                                             | [lmqg/qag_tweetqa](https://huggingface.co/datasets/lmqg/qag_tweetqa) |
 |Language Modeling                  | [cardiffnlp/twitter-roberta-base-2021-124m](https://huggingface.co/cardiffnlp/twitter-roberta-base-2021-124m)                                           | TBA |
 |Tweet Embedding                    | [cambridgeltl/tweet-roberta-base-embeddings-v1](https://huggingface.co/cambridgeltl/tweet-roberta-base-embeddings-v1)                                   | TBA |
 
 
 To use an other model from local/huggingface modelhub, one can simply provide the model path/alias to the `load_model` function.
@@ -489,7 +534,9 @@
     booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
     month = nov,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
+
+
```

### Comparing `tweetnlp-0.4.2/setup.py` & `tweetnlp-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding="utf-8") as f:
     readme = f.read()
 
-version = '0.4.2'
+version = '0.4.3'
 setup(
     name='tweetnlp',
     packages=find_packages(exclude=["assets", "tests"]),
     version=version,
     license='MIT',
     description='NLP library for Twitter.',
     url='https://github.com/cardiffnlp/tweetnlp',
```

### Comparing `tweetnlp-0.4.2/tweetnlp/__init__.py` & `tweetnlp-0.4.3/tweetnlp/__init__.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/loader.py` & `tweetnlp-0.4.3/tweetnlp/loader.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/mlm/model.py` & `tweetnlp-0.4.3/tweetnlp/mlm/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/ner/allennlp_crf.py` & `tweetnlp-0.4.3/tweetnlp/ner/allennlp_crf.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/ner/dataset.py` & `tweetnlp-0.4.3/tweetnlp/ner/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/ner/model.py` & `tweetnlp-0.4.3/tweetnlp/ner/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/question_answer_generation/dataset.py` & `tweetnlp-0.4.3/tweetnlp/question_answer_generation/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/question_answer_generation/model.py` & `tweetnlp-0.4.3/tweetnlp/question_answer_generation/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/question_answering/dataset.py` & `tweetnlp-0.4.3/tweetnlp/question_answering/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/question_answering/model.py` & `tweetnlp-0.4.3/tweetnlp/question_answering/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/sentence_embedding/model.py` & `tweetnlp-0.4.3/tweetnlp/sentence_embedding/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/text_classification/dataset.py` & `tweetnlp-0.4.3/tweetnlp/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/text_classification/model.py` & `tweetnlp-0.4.3/tweetnlp/text_classification/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 import torch
 
 from ..util import load_model, get_preprocessor
 
 DEFAULT_CACHE_DIR = f"{os.path.expanduser('~')}/.cache/tweetnlp/classification"
 MODEL_LIST = {
     'emotion': {
-        "default": "cardiffnlp/twitter-roberta-base-emotion"
+        "single_label": "cardiffnlp/twitter-roberta-base-emotion",
+        "multi_label": "cardiffnlp/twitter-roberta-base-emotion-multilabel-latest"
     },
     'emoji': {
         "default": "cardiffnlp/twitter-roberta-base-emoji"
     },
     'hate': {
-        "default": "cardiffnlp/twitter-roberta-base-hate"
+        "default": "cardiffnlp/twitter-roberta-base-hate-latest"
     },
     'irony': {
         "default": "cardiffnlp/twitter-roberta-base-irony"
     },
     'offensive': {
         "default": "cardiffnlp/twitter-roberta-base-offensive"
     },
@@ -194,17 +195,18 @@
 
 
 class Emotion(Classifier):
 
     def __init__(self,
                  model_name: str = None,
                  max_length: int = 128,
+                 multi_label: bool = True,
                  use_auth_token: bool = False):
         if model_name is None:
-            model_name = MODEL_LIST['emotion']['default']
+            model_name = MODEL_LIST['emotion']['multi_label' if multi_label else 'single_label']
         super().__init__(model_name, max_length=max_length, use_auth_token=use_auth_token)
         self.emotion = self.predict
 
 
 class Emoji(Classifier):
 
     def __init__(self,
```

### Comparing `tweetnlp-0.4.2/tweetnlp/text_classification/readme_template.py` & `tweetnlp-0.4.3/tweetnlp/text_classification/readme_template.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/text_classification/trainer.py` & `tweetnlp-0.4.3/tweetnlp/text_classification/trainer.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp/util.py` & `tweetnlp-0.4.3/tweetnlp/util.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.2/tweetnlp.egg-info/PKG-INFO` & `tweetnlp-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: tweetnlp
-Version: 0.4.2
-Summary: NLP library for Twitter.
-Home-page: https://github.com/cardiffnlp/tweetnlp
-Author: Asahi Ushio
-Author-email: asahi1992ushio@gmail.com
-License: MIT
-Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.2.tar.gz
-Keywords: tweet,nlp,language-model
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/tweetnlp/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/tweetnlp.svg)](https://badge.fury.io/py/tweetnlp)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 [![PyPI status](https://img.shields.io/pypi/status/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 
 # TweetNLP
 TweetNLP for all the NLP enthusiasts working on Twitter! 
@@ -223,25 +202,48 @@
 ```
 
 - ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
 
 ```python
 import tweetnlp
 
-# MODEL
+# MULTI-LABEL MODEL 
+model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
+>>> {'label': 'joy'}
+# Note: the probability of the multi-label model is the output of sigmoid function on binary prediction whether each topic is positive or negative.
+model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
+>>> {'label': 'joy',
+ 'probability': {'anger': 0.00025800734874792397,
+  'anticipation': 0.0005329723935574293,
+  'disgust': 0.00026112011983059347,
+  'fear': 0.00027552215033210814,
+  'joy': 0.7721399068832397,
+  'love': 0.1806265264749527,
+  'optimism': 0.04208092764019966,
+  'pessimism': 0.00025325192837044597,
+  'sadness': 0.0006160663324408233,
+  'surprise': 0.0005619609728455544,
+  'trust': 0.002393839880824089}}
+
+# SINGLE-LABEL MODEL
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
 >>> {'label': 'joy'}
+# NOTE: the probability of the sinlge-label model the softmax over the label.
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.', return_probability=True)
 >>> {'label': 'optimism', 'probability': {'joy': 0.01367587223649025, 'optimism': 0.7345258593559265, 'anger': 0.1770714670419693, 'sadness': 0.07472680509090424}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emotion')
 ```
 
+WARNING: The single-label and multi-label emotion model have diiferent label set (single-label has four classes of 'joy'/'optimism'/'anger'/'sadness', 
+while multi-label has eleven classes of 'joy'/'optimism'/'anger'/'sadness'/'love'/'trust'/'fear'/'surprise'/'anticipation'/'disgust'/'pessimism').
+
 ### Named Entity Recognition
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp#scrollTo=WeREiLEjBlrj)
 
 This module consists of a named-entity recognition (NER) model specifically trained for tweets. The model is instantiated by `tweetnlp.load_model("ner")`, and runs the prediction by giving a text or a list of texts as argument to the `ner` function (check the paper [here](https://arxiv.org/abs/2210.03797), or the [huggingface dataset page](https://huggingface.co/datasets/tner/tweetner7)). 
 
 ```python3
 import tweetnlp
@@ -393,19 +395,20 @@
 | Task                              | Model                                                                                                                                                   | Dataset |
 |-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
 |Topic Classification (single-label)| [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-single-all) | [cardiffnlp/tweet_topic_single](https://huggingface.co/datasets/cardiffnlp/tweet_topic_single) |
 |Topic Classification (multi-label) | [cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all](https://huggingface.co/cardiffnlp/twitter-roberta-base-dec2021-tweet-topic-multi-all)   | [cardiffnlp/tweet_topic_multi](https://huggingface.co/datasets/cardiffnlp/tweet_topic_multi) |
 |Sentiment Analysis (Multilingual)  | [cardiffnlp/twitter-xlm-roberta-base-sentiment](https://huggingface.co/cardiffnlp/twitter-xlm-roberta-base-sentiment)                                   | [cardiffnlp/tweet_sentiment_multilingual](https://huggingface.co/datasets/cardiffnlp/tweet_sentiment_multilingual) |
 |Sentiment Analysis                 | [cardiffnlp/twitter-roberta-base-sentiment-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment-latest)                             | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Irony Detection                    | [cardiffnlp/twitter-roberta-base-irony](https://huggingface.co/cardiffnlp/twitter-roberta-base-irony)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate)                                                     | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Hate Detection                     | [cardiffnlp/twitter-roberta-base-hate-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-hate-latest)                                       | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Offensive Detection                | [cardiffnlp/twitter-roberta-base-offensive](https://huggingface.co/cardiffnlp/twitter-roberta-base-offensive)                                           | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
 |Emoji Prediction                   | [cardiffnlp/twitter-roberta-base-emoji](https://huggingface.co/cardiffnlp/twitter-roberta-base-emoji)                                                   | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Emotion Analysis                   | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
-|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                        | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
+|Emotion Analysis (single-label)    | [cardiffnlp/twitter-roberta-base-emotion](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion)                                               | [tweet_eval](https://huggingface.co/datasets/tweet_eval) |
+|Emotion Analysis (multi-label)     | [cardiffnlp/twitter-roberta-base-emotion-multilabel-latest](https://huggingface.co/cardiffnlp/twitter-roberta-base-emotion-multilabel-latest)           | TBA |
+|Named Entity Recognition           | [tner/roberta-large-tweetner7-all](https://huggingface.co/tner/roberta-large-tweetner7-all)                                                             | [tner/tweetner7](https://huggingface.co/datasets/tner/tweetner7) |
 |Question Answering                 | [lmqg/t5-small-tweetqa-qa](https://huggingface.co/lmqg/t5-small-tweetqa-qa)                                                                             | [lmqg/qg_tweetqa](https://huggingface.co/datasets/lmqg/qg_tweetqa) |
 |Question Answer Generation         | [lmqg/t5-base-tweetqa-qag](https://huggingface.co/lmqg/t5-base-tweetqa-qag)                                                                             | [lmqg/qag_tweetqa](https://huggingface.co/datasets/lmqg/qag_tweetqa) |
 |Language Modeling                  | [cardiffnlp/twitter-roberta-base-2021-124m](https://huggingface.co/cardiffnlp/twitter-roberta-base-2021-124m)                                           | TBA |
 |Tweet Embedding                    | [cambridgeltl/tweet-roberta-base-embeddings-v1](https://huggingface.co/cambridgeltl/tweet-roberta-base-embeddings-v1)                                   | TBA |
 
 
 To use an other model from local/huggingface modelhub, one can simply provide the model path/alias to the `load_model` function.
@@ -510,9 +513,7 @@
     booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
     month = nov,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
-
-
```

### Comparing `tweetnlp-0.4.2/tweetnlp.egg-info/SOURCES.txt` & `tweetnlp-0.4.3/tweetnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

