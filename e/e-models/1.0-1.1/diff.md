# Comparing `tmp/e-models-1.0.tar.gz` & `tmp/e-models-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.0.tar", last modified: Thu Apr  6 13:24:57 2023, max compression
+gzip compressed data, was "e-models-1.1.tar", last modified: Tue Apr 18 18:43:32 2023, max compression
```

## Comparing `e-models-1.0.tar` & `e-models-1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-06 13:24:57.329274 e-models-1.0/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.0/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3023 2023-04-06 13:24:57.329274 e-models-1.0/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2485 2023-04-06 13:23:40.000000 e-models-1.0/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-06 13:24:57.329274 e-models-1.0/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3023 2023-04-06 13:24:57.000000 e-models-1.0/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      447 2023-04-06 13:24:57.000000 e-models-1.0/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-06 13:24:57.000000 e-models-1.0/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       17 2023-04-06 13:24:57.000000 e-models-1.0/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-04-06 13:24:57.000000 e-models-1.0/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-06 13:24:57.329274 e-models-1.0/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-04-06 13:24:15.000000 e-models-1.0/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.0/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-06 13:24:57.329274 e-models-1.0/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34179 2023-04-05 19:57:01.000000 e-models-1.0/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.0/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.0/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.0/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.0/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.0/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6564 2023-04-05 19:51:44.000000 e-models-1.0/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.0/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-06 13:24:57.329274 e-models-1.0/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      926 2023-04-06 13:24:05.000000 e-models-1.0/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-06 13:24:57.329274 e-models-1.0/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7860 2023-04-05 19:54:34.000000 e-models-1.0/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3550 2023-04-18 18:43:32.362634 e-models-1.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3012 2023-04-18 18:35:24.000000 e-models-1.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.358634 e-models-1.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3550 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      447 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       17 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.358634 e-models-1.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-04-18 18:42:20.000000 e-models-1.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34179 2023-04-05 19:57:01.000000 e-models-1.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.1/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6870 2023-04-18 18:32:52.000000 e-models-1.1/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-18 18:43:32.362634 e-models-1.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      926 2023-04-18 18:42:11.000000 e-models-1.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7875 2023-04-18 18:32:24.000000 e-models-1.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.0/LICENSE` & `e-models-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.0/PKG-INFO` & `e-models-1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: e-models
-Version: 1.0
-Summary: Tools for helping build of extraction models with scrapy spiders.
-Home-page: https://github.com/kalessin/emodels
-Author: Martin Olveyra
-Author-email: molveyra@gmail.com
-License: BSD
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 e-models
 ========
 
 
 Suite of tools to assist in the build of extraction models with scrapy spiders
 
 Installation:
@@ -36,18 +20,27 @@
 2. The main purpose of this approach is the generation of datasets suitable for training transformer models for text extraction (aka extractive question answering, EQA)
 3. As a secondary objective, it provides an alternative approach to xpath and css selectors for extraction of data from the html source, that may be more suitable and readable for humans.
 
 Usage:
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the properties just
 described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
-extraction data will be incrementally stored at `<user home folder>/.datasets/items/<item class name>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
+extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_DIR`.
 
-So, in order to maintain dataset well ordered you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
-schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers generalize better. At
+So, in order to maintain a clean dataset well ordered, only enable extract items saving when you are sure you have the correct extraction selectors. Then run locally:
+
+```
+EMODELS_SAVE_EXTRACT_ITEMS=1 scrapy crawl myspider
+```
+
+In addition, in order to have your dataset well ordered, you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
+schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. At
 the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
 So, even if you didn't train the transformer to extract a specific item class, it will do great if you trained it to extract its fields, if it already learned to extract same fields from
 other item classes. You only need to ask the correct question. For example, given an html page as a context, you can ask the model: `which is the phone number?`. You don't need to specify
 which kind of data (a business? a person? an organization?) you expect to find there.
 
+**Important Note**: Usage of the methods introduced by ExtractItemLoader (`add_text_re()` and `add_text_re_as_html()`) will have an impact in the performance of the spiders you use it, so the
+recommendation is to use them in spiders that don't extract more than few hundred items.
+
 (WIP...)
```

### Comparing `e-models-1.0/e_models.egg-info/PKG-INFO` & `e-models-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.0
+Version: 1.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -36,18 +36,27 @@
 2. The main purpose of this approach is the generation of datasets suitable for training transformer models for text extraction (aka extractive question answering, EQA)
 3. As a secondary objective, it provides an alternative approach to xpath and css selectors for extraction of data from the html source, that may be more suitable and readable for humans.
 
 Usage:
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the properties just
 described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
-extraction data will be incrementally stored at `<user home folder>/.datasets/items/<item class name>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
+extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_DIR`.
 
-So, in order to maintain dataset well ordered you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
-schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers generalize better. At
+So, in order to maintain a clean dataset well ordered, only enable extract items saving when you are sure you have the correct extraction selectors. Then run locally:
+
+```
+EMODELS_SAVE_EXTRACT_ITEMS=1 scrapy crawl myspider
+```
+
+In addition, in order to have your dataset well ordered, you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
+schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. At
 the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
 So, even if you didn't train the transformer to extract a specific item class, it will do great if you trained it to extract its fields, if it already learned to extract same fields from
 other item classes. You only need to ask the correct question. For example, given an html page as a context, you can ask the model: `which is the phone number?`. You don't need to specify
 which kind of data (a business? a person? an organization?) you expect to find there.
 
+**Important Note**: Usage of the methods introduced by ExtractItemLoader (`add_text_re()` and `add_text_re_as_html()`) will have an impact in the performance of the spiders you use it, so the
+recommendation is to use them in spiders that don't extract more than few hundred items.
+
 (WIP...)
```

### Comparing `e-models-1.0/emodels/html2text/__init__.py` & `e-models-1.1/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.0/emodels/html2text/config.py` & `e-models-1.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.0/emodels/html2text/utils.py` & `e-models-1.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.0/emodels/scrapyutils.py` & `e-models-1.1/emodels/scrapyutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,14 +125,24 @@
         return result
 
 
 ExtractDict = NewType("ExtractDict", Dict[str, Tuple[int, int]])
 
 
 class ExtractItemLoader(ItemLoader):
+
+    def __new__(cls, *args, **kwargs):
+        obj = super().__new__(cls)
+        if not hasattr(cls, "savefile"):
+            folder = os.path.join(EMODELS_ITEMS_DIR, obj.default_item_class.__name__)
+            os.makedirs(folder, exist_ok=True)
+            findex = len(os.listdir(folder))
+            cls.savefile = os.path.join(folder, f"{findex}.jl.gz")
+        return obj
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         assert "response" in self.context, '"response" is required.'
         if not isinstance(self.context["response"], ExtractTextResponse):
             self.context["response"] = self.context["response"].replace(cls=ExtractTextResponse)
         self.extract_indexes: ExtractDict = ExtractDict({})
         self._mconverter = Markdown()
@@ -164,18 +174,18 @@
             if attr not in self.extract_indexes:
                 cleaned = self._mconverter.convert(t).strip()
                 self.add_value(attr, cleaned, *processors, **kw)
                 self.extract_indexes[attr] = (s, e)
 
     def load_item(self) -> Item:
         item = super().load_item()
-        self._save_extract_sample(item.__class__.__name__)
+        self._save_extract_sample()
         return item
 
-    def _save_extract_sample(self, clsname: str):
+    def _save_extract_sample(self):
         if EMODELS_SAVE_EXTRACT_ITEMS and self.extract_indexes:
             sample = {
                 "indexes": self.extract_indexes,
                 "markdown": self.context["response"].markdown,
             }
-            with gzip.open(os.path.join(EMODELS_ITEMS_DIR, f"{clsname}.jl.gz"), "at") as fz:
+            with gzip.open(self.savefile, "at") as fz:
                 print(json.dumps(sample), file=fz)
```

### Comparing `e-models-1.0/setup.py` & `e-models-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.0',
+    version      = '1.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.0/tests/test_scrapyutils.py` & `e-models-1.1/tests/test_scrapyutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 class BusinessSearchItemLoader(ExtractItemLoader):
     default_item_class = BusinessSearchItem
     default_output_processor = TakeFirst()
 
 
 class ScrapyUtilsTests(TestCase):
-    jobs_result_file = os.path.join(config.EMODELS_DIR, "items/JobItem.jl.gz")
-    business_result_file = os.path.join(config.EMODELS_DIR, "items/BusinessSearchItem.jl.gz")
+    jobs_result_file = os.path.join(config.EMODELS_DIR, "items/JobItem/0.jl.gz")
+    business_result_file = os.path.join(config.EMODELS_DIR, "items/BusinessSearchItem/0.jl.gz")
 
     def tearDown(self):
         for col in "jobs", "business":
             fname = getattr(self, f"{col}_result_file")
             if os.path.isfile(fname):
                 os.remove(fname)
 
@@ -127,17 +127,17 @@
         sample_file = os.path.join(SAMPLES_DIR, "yell.html")
         body = open(sample_file).read().encode("utf8")
         response = ExtractTextResponse(url="https://yell.com/result.html", body=body, status=200)
 
         for r in response.css_split(".businessCapsule--mainRow"):
             loader = BusinessSearchItemLoader(response=r)
             loader.add_text_re("name", r"##(.+)")
-            loader.add_text_re("phone", r"Tel([\s\d]+)")
+            loader.add_text_re("phone", r"Tel([\s\d]+)", tid="#telephone")
             loader.add_text_re("website", r"Website\]\((.+?)\)")
-            loader.add_text_re("address", r"\[.+\|(.+)\]\(.+view=map", flags=re.S)
+            loader.add_text_re("address", r"\[(?:.+\|)?(.+)\]\(.+view=map")
             loader.add_text_re("profile_url", r"\[More info .+\]\((http.+?\d+/)")
             loader.add_text_re(
                 "category",
                 tid=".businessCapsule--classification",
             )
             loader.add_text_re("locality", tid="#addressLocality", strict_tid=True)
             loader.add_text_re("address_alt", reg=r"(?:.+\|)?(.+?),?", tid="#addressLocality")
```

