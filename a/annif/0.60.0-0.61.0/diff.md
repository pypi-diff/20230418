# Comparing `tmp/annif-0.60.0.tar.gz` & `tmp/annif-0.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annif-0.60.0.tar", max compression
+gzip compressed data, was "annif-0.61.0.tar", max compression
```

## Comparing `annif-0.60.0.tar` & `annif-0.61.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
--rw-r--r--   0        0        0      606 2023-01-20 08:31:10.784753 annif-0.60.0/LICENSE.txt
--rw-r--r--   0        0        0     7893 2023-01-20 08:31:10.784753 annif-0.60.0/README.md
--rw-r--r--   0        0        0     1271 2023-01-20 08:31:10.784753 annif-0.60.0/annif/__init__.py
--rw-r--r--   0        0        0     1245 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/__init__.py
--rw-r--r--   0        0        0     1771 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/analyzer.py
--rw-r--r--   0        0        0      322 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/simple.py
--rw-r--r--   0        0        0      376 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/simplemma.py
--rw-r--r--   0        0        0      506 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/snowball.py
--rw-r--r--   0        0        0     1174 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/spacy.py
--rw-r--r--   0        0        0      906 2023-01-20 08:31:10.784753 annif-0.60.0/annif/analyzer/voikko.py
--rw-r--r--   0        0        0     2027 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/__init__.py
--rw-r--r--   0        0        0     4008 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/backend.py
--rw-r--r--   0        0        0     1293 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/dummy.py
--rw-r--r--   0        0        0     5861 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/ensemble.py
--rw-r--r--   0        0        0     5611 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/fasttext.py
--rw-r--r--   0        0        0     2951 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/http.py
--rw-r--r--   0        0        0     3468 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/hyperopt.py
--rw-r--r--   0        0        0     2481 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/mixins.py
--rw-r--r--   0        0        0     5555 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/mllm.py
--rw-r--r--   0        0        0     9062 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/nn_ensemble.py
--rw-r--r--   0        0        0     5295 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/omikuji.py
--rw-r--r--   0        0        0     5664 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/pav.py
--rw-r--r--   0        0        0     4770 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/stwfsa.py
--rw-r--r--   0        0        0     3910 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/svc.py
--rw-r--r--   0        0        0     4383 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/tfidf.py
--rw-r--r--   0        0        0     6581 2023-01-20 08:31:10.784753 annif-0.60.0/annif/backend/yake.py
--rw-r--r--   0        0        0    23198 2023-01-20 08:31:10.784753 annif-0.60.0/annif/cli.py
--rw-r--r--   0        0        0     4313 2023-01-20 08:31:10.784753 annif-0.60.0/annif/config.py
--rw-r--r--   0        0        0      664 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/__init__.py
--rw-r--r--   0        0        0      480 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/combine.py
--rw-r--r--   0        0        0     3992 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/document.py
--rw-r--r--   0        0        0     4651 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/skos.py
--rw-r--r--   0        0        0     8671 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/subject.py
--rw-r--r--   0        0        0     1354 2023-01-20 08:31:10.784753 annif-0.60.0/annif/corpus/types.py
--rw-r--r--   0        0        0      626 2023-01-20 08:31:10.784753 annif-0.60.0/annif/datadir.py
--rw-r--r--   0        0        0     1135 2023-01-20 08:31:10.784753 annif-0.60.0/annif/default_config.py
--rw-r--r--   0        0        0     9345 2023-01-20 08:31:10.784753 annif-0.60.0/annif/eval.py
--rw-r--r--   0        0        0     1866 2023-01-20 08:31:10.784753 annif-0.60.0/annif/exception.py
--rw-r--r--   0        0        0        0 2023-01-20 08:31:10.784753 annif-0.60.0/annif/lexical/__init__.py
--rw-r--r--   0        0        0    11824 2023-01-20 08:31:10.784753 annif-0.60.0/annif/lexical/mllm.py
--rw-r--r--   0        0        0     2784 2023-01-20 08:31:10.784753 annif-0.60.0/annif/lexical/tokenset.py
--rw-r--r--   0        0        0     1466 2023-01-20 08:31:10.784753 annif-0.60.0/annif/lexical/util.py
--rw-r--r--   0        0        0     8535 2023-01-20 08:31:10.784753 annif-0.60.0/annif/openapi/annif.yaml
--rw-r--r--   0        0        0     2267 2023-01-20 08:31:10.784753 annif-0.60.0/annif/parallel.py
--rw-r--r--   0        0        0     9296 2023-01-20 08:31:10.784753 annif-0.60.0/annif/project.py
--rw-r--r--   0        0        0     5465 2023-01-20 08:31:10.784753 annif-0.60.0/annif/registry.py
--rw-r--r--   0        0        0     3812 2023-01-20 08:31:10.784753 annif-0.60.0/annif/rest.py
--rw-r--r--   0        0        0   194901 2023-01-20 08:31:10.784753 annif-0.60.0/annif/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   522721 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0      590 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/css/fonts.css
--rw-r--r--   0        0        0     2862 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/css/style.css
--rw-r--r--   0        0        0    15086 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/favicon.ico
--rw-r--r--   0        0        0    35776 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/fonts/Jost-400-Book.otf
--rw-r--r--   0        0        0    98228 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/fonts/Jost-400-Book.ttf
--rw-r--r--   0        0        0    39056 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/fonts/Jost-500-Medium.otf
--rw-r--r--   0        0        0   109760 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/fonts/Jost-500-Medium.ttf
--rw-r--r--   0        0        0     2663 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/img/annif-RGB.svg
--rw-r--r--   0        0        0      530 2023-01-20 08:31:10.788753 annif-0.60.0/annif/static/img/arrow-white.svg
--rw-r--r--   0        0        0    26580 2023-01-20 08:31:10.792753 annif-0.60.0/annif/static/js/axios.min.js
--rw-r--r--   0        0        0   124862 2023-01-20 08:31:10.792753 annif-0.60.0/annif/static/js/axios.min.js.map
--rw-r--r--   0        0        0    60480 2023-01-20 08:31:10.792753 annif-0.60.0/annif/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   217134 2023-01-20 08:31:10.792753 annif-0.60.0/annif/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    87533 2023-01-20 08:31:10.792753 annif-0.60.0/annif/static/js/vue.min.js
--rw-r--r--   0        0        0     6462 2023-01-20 08:31:10.792753 annif-0.60.0/annif/suggestion.py
--rw-r--r--   0        0        0    11064 2023-01-20 08:31:10.792753 annif-0.60.0/annif/templates/home.html
--rw-r--r--   0        0        0     1717 2023-01-20 08:31:10.792753 annif-0.60.0/annif/transform/__init__.py
--rw-r--r--   0        0        0      749 2023-01-20 08:31:10.792753 annif-0.60.0/annif/transform/inputlimiter.py
--rw-r--r--   0        0        0     1146 2023-01-20 08:31:10.792753 annif-0.60.0/annif/transform/langfilter.py
--rw-r--r--   0        0        0     1845 2023-01-20 08:31:10.792753 annif-0.60.0/annif/transform/transform.py
--rw-r--r--   0        0        0     3292 2023-01-20 08:31:10.792753 annif-0.60.0/annif/util.py
--rw-r--r--   0        0        0      147 2023-01-20 08:31:10.792753 annif-0.60.0/annif/views.py
--rw-r--r--   0        0        0     4738 2023-01-20 08:31:10.792753 annif-0.60.0/annif/vocab.py
--rw-r--r--   0        0        0     2142 2023-01-20 08:31:10.792753 annif-0.60.0/pyproject.toml
--rw-r--r--   0        0        0     9844 1970-01-01 00:00:00.000000 annif-0.60.0/setup.py
--rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 annif-0.60.0/PKG-INFO
+-rw-r--r--   0        0        0      606 2023-04-18 08:47:03.235039 annif-0.61.0/LICENSE.txt
+-rw-r--r--   0        0        0     7872 2023-04-18 08:47:03.235039 annif-0.61.0/README.md
+-rw-r--r--   0        0        0     1549 2023-04-18 08:47:03.235039 annif-0.61.0/annif/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/__init__.py
+-rw-r--r--   0        0        0     1771 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/analyzer.py
+-rw-r--r--   0        0        0      322 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/simple.py
+-rw-r--r--   0        0        0      376 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/simplemma.py
+-rw-r--r--   0        0        0      506 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/snowball.py
+-rw-r--r--   0        0        0     1174 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/spacy.py
+-rw-r--r--   0        0        0      906 2023-04-18 08:47:03.235039 annif-0.61.0/annif/analyzer/voikko.py
+-rw-r--r--   0        0        0     2027 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/__init__.py
+-rw-r--r--   0        0        0     4541 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/backend.py
+-rw-r--r--   0        0        0     1417 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/dummy.py
+-rw-r--r--   0        0        0     5271 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/ensemble.py
+-rw-r--r--   0        0        0     5567 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/fasttext.py
+-rw-r--r--   0        0        0     2841 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/http.py
+-rw-r--r--   0        0        0     3468 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/hyperopt.py
+-rw-r--r--   0        0        0     2409 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/mixins.py
+-rw-r--r--   0        0        0     5502 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/mllm.py
+-rw-r--r--   0        0        0     9364 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/nn_ensemble.py
+-rw-r--r--   0        0        0     5313 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/omikuji.py
+-rw-r--r--   0        0        0     6003 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/pav.py
+-rw-r--r--   0        0        0     4725 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/stwfsa.py
+-rw-r--r--   0        0        0     3872 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/svc.py
+-rw-r--r--   0        0        0     4289 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/tfidf.py
+-rw-r--r--   0        0        0     6537 2023-04-18 08:47:03.235039 annif-0.61.0/annif/backend/yake.py
+-rw-r--r--   0        0        0    19381 2023-04-18 08:47:03.235039 annif-0.61.0/annif/cli.py
+-rw-r--r--   0        0        0     5878 2023-04-18 08:47:03.235039 annif-0.61.0/annif/cli_util.py
+-rw-r--r--   0        0        0     4313 2023-04-18 08:47:03.235039 annif-0.61.0/annif/config.py
+-rw-r--r--   0        0        0      664 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/__init__.py
+-rw-r--r--   0        0        0      480 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/combine.py
+-rw-r--r--   0        0        0     4113 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/document.py
+-rw-r--r--   0        0        0     4651 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/skos.py
+-rw-r--r--   0        0        0     8798 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/subject.py
+-rw-r--r--   0        0        0     1756 2023-04-18 08:47:03.235039 annif-0.61.0/annif/corpus/types.py
+-rw-r--r--   0        0        0      626 2023-04-18 08:47:03.235039 annif-0.61.0/annif/datadir.py
+-rw-r--r--   0        0        0     1135 2023-04-18 08:47:03.235039 annif-0.61.0/annif/default_config.py
+-rw-r--r--   0        0        0     8906 2023-04-18 08:47:03.235039 annif-0.61.0/annif/eval.py
+-rw-r--r--   0        0        0     1866 2023-04-18 08:47:03.235039 annif-0.61.0/annif/exception.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:47:03.235039 annif-0.61.0/annif/lexical/__init__.py
+-rw-r--r--   0        0        0    11823 2023-04-18 08:47:03.235039 annif-0.61.0/annif/lexical/mllm.py
+-rw-r--r--   0        0        0     2784 2023-04-18 08:47:03.235039 annif-0.61.0/annif/lexical/tokenset.py
+-rw-r--r--   0        0        0     1466 2023-04-18 08:47:03.235039 annif-0.61.0/annif/lexical/util.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:47:03.239041 annif-0.61.0/annif/openapi/__init__.py
+-rw-r--r--   0        0        0    10845 2023-04-18 08:47:03.239041 annif-0.61.0/annif/openapi/annif.yaml
+-rw-r--r--   0        0        0     1552 2023-04-18 08:47:03.239041 annif-0.61.0/annif/openapi/validation.py
+-rw-r--r--   0        0        0     2680 2023-04-18 08:47:03.239041 annif-0.61.0/annif/parallel.py
+-rw-r--r--   0        0        0     9303 2023-04-18 08:47:03.239041 annif-0.61.0/annif/project.py
+-rw-r--r--   0        0        0     5465 2023-04-18 08:47:03.239041 annif-0.61.0/annif/registry.py
+-rw-r--r--   0        0        0     5230 2023-04-18 08:47:03.239041 annif-0.61.0/annif/rest.py
+-rw-r--r--   0        0        0   194901 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   522721 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0      590 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/css/fonts.css
+-rw-r--r--   0        0        0     2862 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/css/style.css
+-rw-r--r--   0        0        0    15086 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/favicon.ico
+-rw-r--r--   0        0        0    35776 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/fonts/Jost-400-Book.otf
+-rw-r--r--   0        0        0    98228 2023-04-18 08:47:03.239041 annif-0.61.0/annif/static/fonts/Jost-400-Book.ttf
+-rw-r--r--   0        0        0    39056 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/fonts/Jost-500-Medium.otf
+-rw-r--r--   0        0        0   109760 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/fonts/Jost-500-Medium.ttf
+-rw-r--r--   0        0        0     2663 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/img/annif-RGB.svg
+-rw-r--r--   0        0        0      530 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/img/arrow-white.svg
+-rw-r--r--   0        0        0    26580 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/js/axios.min.js
+-rw-r--r--   0        0        0   124862 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/js/axios.min.js.map
+-rw-r--r--   0        0        0    60480 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   217134 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    87533 2023-04-18 08:47:03.243042 annif-0.61.0/annif/static/js/vue.min.js
+-rw-r--r--   0        0        0     4783 2023-04-18 08:47:03.243042 annif-0.61.0/annif/suggestion.py
+-rw-r--r--   0        0        0    11064 2023-04-18 08:47:03.243042 annif-0.61.0/annif/templates/home.html
+-rw-r--r--   0        0        0     1717 2023-04-18 08:47:03.243042 annif-0.61.0/annif/transform/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-18 08:47:03.243042 annif-0.61.0/annif/transform/inputlimiter.py
+-rw-r--r--   0        0        0     1145 2023-04-18 08:47:03.243042 annif-0.61.0/annif/transform/langfilter.py
+-rw-r--r--   0        0        0     1845 2023-04-18 08:47:03.243042 annif-0.61.0/annif/transform/transform.py
+-rw-r--r--   0        0        0     3206 2023-04-18 08:47:03.243042 annif-0.61.0/annif/util.py
+-rw-r--r--   0        0        0      147 2023-04-18 08:47:03.243042 annif-0.61.0/annif/views.py
+-rw-r--r--   0        0        0     4738 2023-04-18 08:47:03.243042 annif-0.61.0/annif/vocab.py
+-rw-r--r--   0        0        0     2231 2023-04-18 08:47:03.243042 annif-0.61.0/pyproject.toml
+-rw-r--r--   0        0        0    10123 1970-01-01 00:00:00.000000 annif-0.61.0/PKG-INFO
```

### Comparing `annif-0.60.0/LICENSE.txt` & `annif-0.61.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/README.md` & `annif-0.61.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <img src="https://annif.org/static/img/annif-RGB.svg" width="150">
 
 [![DOI](https://zenodo.org/badge/100936800.svg)](https://zenodo.org/badge/latestdoi/100936800)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![CI/CD](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml)
-[![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/master/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)
+[![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/main/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)
 [![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
-[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=master)
-[![codebeat badge](https://codebeat.co/badges/e496f151-93db-4f0e-9e30-bc3339e58ca4)](https://codebeat.co/projects/github-com-natlibfi-annif-master)
+[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=main)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=main)
+[![codebeat badge](https://codebeat.co/badges/7a8ef539-0094-48b8-84c2-c413b4a50d57)](https://codebeat.co/projects/github-com-natlibfi-annif-main)
 [![CodeQL](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NatLibFi_Annif&metric=alert_status)](https://sonarcloud.io/dashboard?id=NatLibFi_Annif)
 [![docs](https://readthedocs.org/projects/annif/badge/?version=latest)](https://annif.readthedocs.io/en/latest/index.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Annif is an automated subject indexing toolkit. It was originally created as
 a statistical automated indexing tool that used metadata from the
@@ -44,15 +44,15 @@
     annif
 
 See [Getting Started](https://github.com/NatLibFi/Annif/wiki/Getting-started)
 in the wiki for more details.
 
 # Docker install
 
-You can use Annif as a pre-built Docker container. Please see the 
+You can use Annif as a pre-built Docker container. Please see the
 [wiki documentation](https://github.com/NatLibFi/Annif/wiki/Usage-with-Docker)
 for details.
 
 # Development install
 
 A development version of Annif can be installed by cloning the [GitHub
 repository](https://github.com/NatLibFi/Annif).
@@ -67,19 +67,19 @@
 Switch into the repository directory.
 
 Install [pipx](https://pypa.github.io/pipx/) and Poetry if you don't have them. First pipx:
 
     python3 -m pip install --user pipx
     python3 -m pipx ensurepath
 
-Open a new shell, and then install Poetry: 
+Open a new shell, and then install Poetry:
 
     pipx install poetry
 
-Poetry can be installed also without pipx: check the [Poetry documentation](https://python-poetry.org/docs/master/#installation). 
+Poetry can be installed also without pipx: check the [Poetry documentation](https://python-poetry.org/docs/master/#installation).
 
 Create a virtual environment and install dependencies:
 
     poetry install
 
 By default development dependencies are included. Use option `-E` to install dependencies for selected optional features (`-E "extra1 extra2"` for multiple extras), or install all of them with `--all-extras`. By default the virtual environment directory is not under the project directory, but there is a [setting for selecting this](https://python-poetry.org/docs/configuration/#virtualenvsin-project).
 
@@ -113,36 +113,36 @@
 
 ## Citing the software itself
 
 See "Cite this repository" in the details of the repository.
 
 ## Annif articles
 <ul>
-<li> 
-Suominen, O.; Inkinen, J.; Lehtinen, M., 2022. 
+<li>
+Suominen, O.; Inkinen, J.; Lehtinen, M., 2022.
 Annif and Finto AI: Developing and Implementing Automated Subject Indexing.
 JLIS.It, 13(1), pp. 265–282. URL:
 https://www.jlis.it/index.php/jlis/article/view/437
 <details>
 <summary>See BibTex</summary>
-    
+
     @article{suominen2022annif,
       title={Annif and Finto AI: Developing and Implementing Automated Subject Indexing},
       author={Suominen, Osma and Inkinen, Juho and Lehtinen, Mona},
       journal={JLIS.it},
       volume={13},
       number={1},
       pages={265--282},
       year={2022},
       doi = {10.4403/jlis.it-12740},
       url={https://www.jlis.it/index.php/jlis/article/view/437},
     }
 </details>
-</li> 
-<li> 
+</li>
+<li>
 Suominen, O.; Koskenniemi, I, 2022.
 Annif Analyzer Shootout: Comparing text lemmatization methods for automated subject indexing.
 Code4Lib Journal, (54). URL:
 https://journal.code4lib.org/articles/16719
 <details>
 <summary>See BibTex</summary>
 
@@ -151,16 +151,16 @@
       author={Suominen, Osma and Koskenniemi, Ilkka},
       journal={Code4Lib J.},
       number={54},
       year={2022},
       url={https://journal.code4lib.org/articles/16719},
     }
 </details>
-</li> 
-<li> 
+</li>
+<li>
 Suominen, O., 2019. Annif: DIY automated subject indexing using multiple
 algorithms. LIBER Quarterly, 29(1), pp.1–25. DOI:
 https://doi.org/10.18352/lq.10285
 <details>
 <summary>See BibTex</summary>
 
     @article{suominen2019annif,
```

### Comparing `annif-0.60.0/annif/__init__.py` & `annif-0.61.0/annif/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import logging
 import os
 import os.path
 
 import connexion
 from flask_cors import CORS
 
+from annif.openapi.validation import CustomRequestBodyValidator
+
+logging.basicConfig()
 logger = logging.getLogger("annif")
+logger.setLevel(level=logging.INFO)
 
 import annif.backend  # noqa
 
 
 def create_app(config_name=None):
     # 'cxapp' here is the Connexion application that has a normal Flask app
     # as a property (cxapp.app)
@@ -25,21 +29,25 @@
             config_name = "annif.default_config.Config"
         else:
             config_name = "annif.default_config.ProductionConfig"
     logger.debug("creating app with configuration %s", config_name)
     cxapp.app.config.from_object(config_name)
     cxapp.app.config.from_envvar("ANNIF_SETTINGS", silent=True)
 
-    cxapp.add_api("annif.yaml")
+    validator_map = {
+        "body": CustomRequestBodyValidator,
+    }
+    cxapp.add_api("annif.yaml", validator_map=validator_map)
 
     # add CORS support
     CORS(cxapp.app)
 
     if cxapp.app.config["INITIALIZE_PROJECTS"]:
         annif.registry.initialize_projects(cxapp.app)
+        logger.info("finished initializing projects")
 
     # register the views via blueprints
     from annif.views import bp
 
     cxapp.app.register_blueprint(bp)
 
     # return the Flask app
```

### Comparing `annif-0.60.0/annif/analyzer/__init__.py` & `annif-0.61.0/annif/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/analyzer/analyzer.py` & `annif-0.61.0/annif/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/analyzer/spacy.py` & `annif-0.61.0/annif/analyzer/spacy.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/analyzer/voikko.py` & `annif-0.61.0/annif/analyzer/voikko.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/backend/__init__.py` & `annif-0.61.0/annif/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/backend/backend.py` & `annif-0.61.0/annif/backend/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import abc
 import os.path
 from datetime import datetime, timezone
 from glob import glob
 
 from annif import logger
+from annif.suggestion import SuggestionBatch
 
 
 class AnnifBackend(metaclass=abc.ABCMeta):
     """Base class for Annif backends that perform analysis. The
     non-implemented methods should be overridden in subclasses."""
 
     name = None
@@ -69,26 +70,36 @@
     def initialize(self, parallel=False):
         """This method can be overridden by backends. It should cause the
         backend to pre-load all data it needs during operation.
         If parallel is True, the backend should expect to be used for
         parallel operation."""
         pass
 
-    @abc.abstractmethod
     def _suggest(self, text, params):
-        """This method should implemented by backends. It implements
-        the suggest functionality, with pre-processed parameters."""
+        """Either this method or _suggest_batch should be implemented by by
+        backends.  It implements the suggest functionality for a single
+        document, with pre-processed parameters."""
         pass  # pragma: no cover
 
-    def suggest(self, text, params=None):
-        """Suggest subjects for the input text and return a list of subjects
+    def _suggest_batch(self, texts, params):
+        """This method can be implemented by backends to use batching of documents in
+        their operations. This default implementation uses the regular suggest
+        functionality."""
+        return SuggestionBatch.from_sequence(
+            [self._suggest(text, params) for text in texts],
+            self.project.subjects,
+            limit=int(params.get("limit")),
+        )
+
+    def suggest(self, texts, params=None):
+        """Suggest subjects for the input documents and return a list of subject sets
         represented as a list of SubjectSuggestion objects."""
         beparams = self._get_backend_params(params)
         self.initialize()
-        return self._suggest(text, params=beparams)
+        return self._suggest_batch(texts, params=beparams)
 
     def debug(self, message):
         """Log a debug message from this backend"""
         logger.debug("Backend {}: {}".format(self.backend_id, message))
 
     def info(self, message):
         """Log an info message from this backend"""
```

### Comparing `annif-0.60.0/annif/backend/dummy.py` & `annif-0.61.0/annif/backend/dummy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Dummy backend for testing basic interaction of projects and backends"""
 
 
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion
 
 from . import backend
 
 
 class DummyBackend(backend.AnnifLearningBackend):
     name = "dummy"
     initialized = False
@@ -18,23 +18,28 @@
 
     def initialize(self, parallel=False):
         self.initialized = True
 
     def _suggest(self, text, params):
         score = float(params.get("score", 1.0))
 
+        # Ensure tests fail if "text" with wrong type ends up here
+        assert isinstance(text, str)
+
+        # Give no hits for no text
+        if len(text) == 0:
+            return []
+
         # allow overriding returned subject via uri parameter
         if "uri" in params:
             subject_id = self.project.subjects.by_uri(params["uri"])
         else:
             subject_id = self.subject_id
 
-        return ListSuggestionResult(
-            [SubjectSuggestion(subject_id=subject_id, score=score)]
-        )
+        return [SubjectSuggestion(subject_id=subject_id, score=score)]
 
     def _learn(self, corpus, params):
         # in this dummy backend we "learn" by picking up the subject ID
         # of the first subject of the first document in the learning set
         # and using that in subsequent analysis results
         for doc in corpus.documents:
             if doc.subject_set:
```

### Comparing `annif-0.60.0/annif/backend/fasttext.py` & `annif-0.61.0/annif/backend/fasttext.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import collections
 import os.path
 
 import fasttext
 
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion
 
 from . import backend, mixins
 
 
 class FastTextBackend(mixins.ChunkingBackend, backend.AnnifBackend):
     """fastText backend for Annif"""
 
@@ -159,8 +159,8 @@
         for score, label in best_labels[:limit]:
             results.append(
                 SubjectSuggestion(
                     subject_id=self._label_to_subject_id(label),
                     score=score / len(chunktexts),
                 )
             )
-        return ListSuggestionResult(results)
+        return results
```

### Comparing `annif-0.60.0/annif/backend/http.py` & `annif-0.61.0/annif/backend/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 
 import dateutil.parser
 import requests
 import requests.exceptions
 
 from annif.exception import OperationFailedException
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion
 
 from . import backend
 
 
 class HTTPBackend(backend.AnnifBackend):
     name = "http"
     _headers = None
@@ -65,21 +65,21 @@
             data["project"] = params["project"]
 
         try:
             req = requests.post(params["endpoint"], data=data, headers=self.headers)
             req.raise_for_status()
         except requests.exceptions.RequestException as err:
             self.warning("HTTP request failed: {}".format(err))
-            return ListSuggestionResult([])
+            return []
 
         try:
             response = req.json()
         except ValueError as err:
             self.warning("JSON decode failed: {}".format(err))
-            return ListSuggestionResult([])
+            return []
 
         if "results" in response:
             results = response["results"]
         else:
             results = response
 
         try:
@@ -89,10 +89,10 @@
                     score=hit["score"],
                 )
                 for hit in results
                 if hit["score"] > 0.0
             ]
         except (TypeError, ValueError) as err:
             self.warning("Problem interpreting JSON data: {}".format(err))
-            return ListSuggestionResult([])
+            return []
 
-        return ListSuggestionResult(subject_suggestions)
+        return subject_suggestions
```

### Comparing `annif-0.60.0/annif/backend/hyperopt.py` & `annif-0.61.0/annif/backend/hyperopt.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/backend/mixins.py` & `annif-0.61.0/annif/backend/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os.path
 
 import joblib
 from sklearn.feature_extraction.text import TfidfVectorizer
 
 import annif.util
 from annif.exception import NotInitializedException
-from annif.suggestion import ListSuggestionResult
 
 
 class ChunkingBackend(metaclass=abc.ABCMeta):
     """Annif backend mixin that implements chunking of input"""
 
     DEFAULT_PARAMETERS = {"chunksize": 1}
 
@@ -35,15 +34,15 @@
         self.debug("Found {} sentences".format(len(sentences)))
         chunksize = int(params["chunksize"])
         chunktexts = []
         for i in range(0, len(sentences), chunksize):
             chunktexts.append(" ".join(sentences[i : i + chunksize]))
         self.debug("Split sentences into {} chunks".format(len(chunktexts)))
         if len(chunktexts) == 0:  # no input, empty result
-            return ListSuggestionResult([])
+            return []
         return self._suggest_chunks(chunktexts, params)
 
 
 class TfidfVectorizerMixin:
     """Annif backend mixin that implements TfidfVectorizer functionality"""
 
     VECTORIZER_FILE = "vectorizer"
```

### Comparing `annif-0.60.0/annif/backend/mllm.py` & `annif-0.61.0/annif/backend/mllm.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import joblib
 import numpy as np
 
 import annif.eval
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
 from annif.lexical.mllm import MLLMModel
-from annif.suggestion import VectorSuggestionResult
+from annif.suggestion import vector_to_suggestions
 
 from . import backend, hyperopt
 
 
 class MLLMOptimizer(hyperopt.HyperparameterOptimizer):
     """Hyperparameter optimizer for the MLLM backend"""
 
@@ -44,15 +44,15 @@
             if candidates:
                 features = self._backend._model._candidates_to_features(candidates)
                 scores = model.predict_proba(features)
                 ranking = self._backend._model._prediction_to_list(scores, candidates)
             else:
                 ranking = []
             results = self._backend._prediction_to_result(ranking, params)
-            batch.evaluate(results, goldsubj)
+            batch.evaluate_many([results], [goldsubj])
         results = batch.results(metrics=[self._metric])
         return results[self._metric]
 
     def _postprocess(self, study):
         bp = study.best_params
         lines = [
             f"min_samples_leaf={bp['min_samples_leaf']}",
@@ -140,14 +140,13 @@
     def _generate_candidates(self, text):
         return self._model.generate_candidates(text, self.project.analyzer)
 
     def _prediction_to_result(self, prediction, params):
         vector = np.zeros(len(self.project.subjects), dtype=np.float32)
         for score, subject_id in prediction:
             vector[subject_id] = score
-        result = VectorSuggestionResult(vector)
-        return result.filter(self.project.subjects, limit=int(params["limit"]))
+        return vector_to_suggestions(vector, int(params["limit"]))
 
     def _suggest(self, text, params):
         candidates = self._generate_candidates(text)
         prediction = self._model.predict(candidates)
         return self._prediction_to_result(prediction, params)
```

### Comparing `annif-0.60.0/annif/backend/nn_ensemble.py` & `annif-0.61.0/annif/backend/nn_ensemble.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from tensorflow.keras.models import Model, load_model
 from tensorflow.keras.utils import Sequence
 
 import annif.corpus
 import annif.parallel
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
-from annif.suggestion import VectorSuggestionResult
+from annif.suggestion import SuggestionBatch, vector_to_suggestions
 
 from . import backend, ensemble
 
 
 def idx_to_key(idx):
     """convert an integer index to a binary key for use in LMDB"""
     return b"%08d" % idx
@@ -126,26 +126,36 @@
                 backend_id=self.backend_id,
             )
         self.debug("loading Keras model from {}".format(model_filename))
         self._model = load_model(
             model_filename, custom_objects={"MeanLayer": MeanLayer}
         )
 
-    def _merge_hits_from_sources(self, hits_from_sources, params):
-        score_vector = np.array(
+    def _merge_source_batches(self, batch_by_source, sources, params):
+        src_weight = dict(sources)
+        score_vectors = np.array(
             [
-                np.sqrt(hits.as_vector(len(subjects))) * weight * len(hits_from_sources)
-                for hits, weight, subjects in hits_from_sources
+                [
+                    np.sqrt(suggestions.as_vector())
+                    * src_weight[project_id]
+                    * len(batch_by_source)
+                    for suggestions in batch
+                ]
+                for project_id, batch in batch_by_source.items()
             ],
             dtype=np.float32,
+        ).transpose(1, 2, 0)
+        prediction = self._model(score_vectors).numpy()
+        return SuggestionBatch.from_sequence(
+            [
+                vector_to_suggestions(row, limit=int(params["limit"]))
+                for row in prediction
+            ],
+            self.project.subjects,
         )
-        results = self._model.predict(
-            np.expand_dims(score_vector.transpose(), 0), verbose=0
-        )
-        return VectorSuggestionResult(results[0])
 
     def _create_model(self, sources):
         self.info("creating NN ensemble model")
 
         inputs = Input(shape=(len(self.project.subjects), len(sources)))
 
         flat_input = Flatten()(inputs)
@@ -208,15 +218,15 @@
         self.info("Processing training documents...")
         with pool_class(jobs) as pool:
             for hits, subject_set in pool.imap_unordered(
                 psmap.suggest, corpus.documents
             ):
                 doc_scores = []
                 for project_id, p_hits in hits.items():
-                    vector = p_hits.as_vector(len(self.project.subjects))
+                    vector = p_hits.as_vector()
                     doc_scores.append(
                         np.sqrt(vector) * sources[project_id] * len(sources)
                     )
                 score_vector = np.array(doc_scores, dtype=np.float32).transpose()
                 true_vector = subject_set.as_vector(len(self.project.subjects))
                 seq.add_sample(score_vector, true_vector)
```

### Comparing `annif-0.60.0/annif/backend/omikuji.py` & `annif-0.61.0/annif/backend/omikuji.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import annif.util
 from annif.exception import (
     NotInitializedException,
     NotSupportedException,
     OperationFailedException,
 )
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion, SuggestionBatch
 
 from . import backend, mixins
 
 
 class OmikujiBackend(mixins.TfidfVectorizerMixin, backend.AnnifBackend):
     """Omikuji based backend for Annif"""
 
@@ -118,22 +118,22 @@
             }
             veccorpus = self.create_vectorizer(input, vecparams)
             self._create_train_file(veccorpus, corpus)
         else:
             self.info("Reusing cached training data from previous run.")
         self._create_model(params, jobs)
 
-    def _suggest(self, text, params):
-        self.debug(
-            'Suggesting subjects for text "{}..." (len={})'.format(text[:20], len(text))
-        )
-        vector = self.vectorizer.transform([text])
-        if vector.nnz == 0:  # All zero vector, empty result
-            return ListSuggestionResult([])
-        feature_values = [
-            (col, vector[row, col]) for row, col in zip(*vector.nonzero())
-        ]
-        results = []
+    def _suggest_batch(self, texts, params):
+        vector = self.vectorizer.transform(texts)
         limit = int(params["limit"])
-        for subj_id, score in self._model.predict(feature_values, top_k=limit):
-            results.append(SubjectSuggestion(subject_id=subj_id, score=score))
-        return ListSuggestionResult(results)
+
+        batch_results = []
+        for row in vector:
+            if row.nnz == 0:  # All zero vector, empty result
+                batch_results.append([])
+                continue
+            feature_values = [(col, row[0, col]) for col in row.nonzero()[1]]
+            results = []
+            for subj_id, score in self._model.predict(feature_values, top_k=limit):
+                results.append(SubjectSuggestion(subject_id=subj_id, score=score))
+            batch_results.append(results)
+        return SuggestionBatch.from_sequence(batch_results, self.project.subjects)
```

### Comparing `annif-0.60.0/annif/backend/pav.py` & `annif-0.61.0/annif/backend/pav.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 import joblib
 import numpy as np
 from scipy.sparse import coo_matrix, csc_matrix
 from sklearn.isotonic import IsotonicRegression
 
 import annif.corpus
-import annif.suggestion
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
+from annif.suggestion import SubjectSuggestion, SuggestionBatch
 
 from . import backend, ensemble
 
 
 class PAVBackend(ensemble.BaseEnsembleBackend):
     """PAV ensemble backend that combines results from multiple projects"""
 
@@ -53,49 +53,56 @@
                     backend_id=self.backend_id,
                 )
 
     def _get_model(self, source_project_id):
         self.initialize()
         return self._models[source_project_id]
 
-    def _normalize_hits(self, hits, source_project):
-        reg_models = self._get_model(source_project.project_id)
-        pav_result = []
-        for hit in hits.as_list():
-            if hit.subject_id in reg_models:
-                score = reg_models[hit.subject_id].predict([hit.score])[0]
-            else:  # default to raw score
-                score = hit.score
-            pav_result.append(
-                annif.suggestion.SubjectSuggestion(
-                    subject_id=hit.subject_id, score=score
-                )
+    def _merge_source_batches(self, batch_by_source, sources, params):
+        reg_batch_by_source = {}
+        for project_id, batch in batch_by_source.items():
+            reg_models = self._get_model(project_id)
+            pav_batch = [
+                [
+                    SubjectSuggestion(
+                        subject_id=sugg.subject_id,
+                        score=reg_models[sugg.subject_id].predict([sugg.score])[0],
+                    )
+                    if sugg.subject_id in reg_models
+                    else SubjectSuggestion(
+                        subject_id=sugg.subject_id, score=sugg.score
+                    )  # default to raw score
+                    for sugg in result
+                ]
+                for result in batch
+            ]
+            reg_batch_by_source[project_id] = SuggestionBatch.from_sequence(
+                pav_batch, self.project.subjects
             )
-        pav_result.sort(key=lambda hit: hit.score, reverse=True)
-        return annif.suggestion.ListSuggestionResult(pav_result)
+
+        return super()._merge_source_batches(reg_batch_by_source, sources, params)
 
     @staticmethod
     def _suggest_train_corpus(source_project, corpus):
         # lists for constructing score matrix
         data, row, col = [], [], []
         # lists for constructing true label matrix
         trow, tcol = [], []
 
         ndocs = 0
         for docid, doc in enumerate(corpus.documents):
-            hits = source_project.suggest(doc.text)
-            vector = hits.as_vector(len(source_project.subjects))
+            hits = source_project.suggest([doc.text])[0]
+            vector = hits.as_vector()
             for cid in np.flatnonzero(vector):
                 data.append(vector[cid])
                 row.append(docid)
                 col.append(cid)
             for cid in np.flatnonzero(
                 doc.subject_set.as_vector(len(source_project.subjects))
             ):
-
                 trow.append(docid)
                 tcol.append(cid)
             ndocs += 1
         scores = coo_matrix(
             (data, (row, col)),
             shape=(ndocs, len(source_project.subjects)),
             dtype=np.float32,
```

### Comparing `annif-0.60.0/annif/backend/stwfsa.py` & `annif-0.61.0/annif/backend/stwfsa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from stwfsapy.predictor import StwfsapyPredictor
 
 from annif.exception import NotInitializedException, NotSupportedException
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion
 from annif.util import atomic_save, boolean
 
 from . import backend
 
 _KEY_CONCEPT_TYPE_URI = "concept_type_uri"
 _KEY_SUBTHESAURUS_TYPE_URI = "sub_thesaurus_type_uri"
 _KEY_THESAURUS_RELATION_TYPE_URI = "thesaurus_relation_type_uri"
@@ -19,15 +19,14 @@
 _KEY_EXPAND_AMPERSAND_WITH_SPACES = "expand_ampersand_with_spaces"
 _KEY_EXPAND_ABBREVIATION_WITH_PUNCTUATION = "expand_abbreviation_with_punctuation"
 _KEY_SIMPLE_ENGLISH_PLURAL_RULES = "simple_english_plural_rules"
 _KEY_USE_TXT_VEC = "use_txt_vec"
 
 
 class StwfsaBackend(backend.AnnifBackend):
-
     name = "stwfsa"
 
     STWFSA_PARAMETERS = {
         _KEY_CONCEPT_TYPE_URI: str,
         _KEY_SUBTHESAURUS_TYPE_URI: str,
         _KEY_THESAURUS_RELATION_TYPE_URI: str,
         _KEY_THESAURUS_RELATION_IS_SPECIALISATION: boolean,
@@ -121,8 +120,8 @@
         suggestions = []
         for uri, score in result:
             subject_id = self.project.subjects.by_uri(uri)
             if subject_id is not None:
                 suggestions.append(
                     SubjectSuggestion(subject_id=subject_id, score=score)
                 )
-        return ListSuggestionResult(suggestions)
+        return suggestions
```

### Comparing `annif-0.60.0/annif/backend/svc.py` & `annif-0.61.0/annif/backend/svc.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import joblib
 import numpy as np
 import scipy.special
 from sklearn.svm import LinearSVC
 
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion, SuggestionBatch
 
 from . import backend, mixins
 
 
 class SVCBackend(mixins.TfidfVectorizerMixin, backend.AnnifBackend):
     """Support vector classifier backend for Annif"""
 
@@ -90,20 +90,21 @@
         limit = int(params["limit"])
         for class_id in np.argsort(scores)[::-1][:limit]:
             subject_id = self._model.classes_[class_id]
             if subject_id is not None:
                 results.append(
                     SubjectSuggestion(subject_id=subject_id, score=scores[class_id])
                 )
-        return ListSuggestionResult(results)
+        return results
 
-    def _suggest(self, text, params):
-        self.debug(
-            'Suggesting subjects for text "{}..." (len={})'.format(text[:20], len(text))
-        )
-        vector = self.vectorizer.transform([text])
-        if vector.nnz == 0:  # All zero vector, empty result
-            return ListSuggestionResult([])
-        confidences = self._model.decision_function(vector)[0]
+    def _suggest_batch(self, texts, params):
+        vector = self.vectorizer.transform(texts)
+        confidences = self._model.decision_function(vector)
         # convert to 0..1 score range using logistic function
-        scores = scipy.special.expit(confidences)
-        return self._scores_to_suggestions(scores, params)
+        scores_list = scipy.special.expit(confidences)
+        return SuggestionBatch.from_sequence(
+            [
+                [] if row.nnz == 0 else self._scores_to_suggestions(scores, params)
+                for scores, row in zip(scores_list, vector)
+            ],
+            self.project.subjects,
+        )
```

### Comparing `annif-0.60.0/annif/backend/tfidf.py` & `annif-0.61.0/annif/backend/tfidf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 
 import gensim.similarities
 from gensim.matutils import Sparse2Corpus
 
 import annif.util
 from annif.exception import NotInitializedException, NotSupportedException
-from annif.suggestion import VectorSuggestionResult
+from annif.suggestion import vector_to_suggestions
 
 from . import backend, mixins
 
 
 class SubjectBuffer:
     """A file-backed buffer to store and retrieve subject text."""
 
@@ -114,10 +114,8 @@
 
     def _suggest(self, text, params):
         self.debug(
             'Suggesting subjects for text "{}..." (len={})'.format(text[:20], len(text))
         )
         tokens = self.project.analyzer.tokenize_words(text)
         vectors = self.vectorizer.transform([" ".join(tokens)])
-        docsim = self._index[vectors[0]]
-        fullresult = VectorSuggestionResult(docsim)
-        return fullresult.filter(self.project.subjects, limit=int(params["limit"]))
+        return vector_to_suggestions(self._index[vectors[0]], int(params["limit"]))
```

### Comparing `annif-0.60.0/annif/backend/yake.py` & `annif-0.61.0/annif/backend/yake.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import joblib
 import yake
 from rdflib.namespace import SKOS
 
 import annif.util
 from annif.exception import ConfigurationException, NotSupportedException
-from annif.suggestion import ListSuggestionResult, SubjectSuggestion
+from annif.suggestion import SubjectSuggestion
 
 from . import backend
 
 
 class YakeBackend(backend.AnnifBackend):
     """Yake based backend for Annif"""
 
@@ -126,15 +126,15 @@
         suggestions = self._keyphrases2suggestions(keyphrases)
 
         subject_suggestions = [
             SubjectSuggestion(subject_id=self.project.subjects.by_uri(uri), score=score)
             for uri, score in suggestions[:limit]
             if score > 0.0
         ]
-        return ListSuggestionResult(subject_suggestions)
+        return subject_suggestions
 
     def _keyphrases2suggestions(self, keyphrases):
         suggestions = []
         not_matched = []
         for kp, score in keyphrases:
             uris = self._keyphrase2uris(kp)
             for uri in uris:
```

### Comparing `annif-0.60.0/annif/cli.py` & `annif-0.61.0/annif/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,156 +6,35 @@
 import json
 import os.path
 import re
 import sys
 
 import click
 import click_log
-from flask import current_app
-from flask.cli import FlaskGroup, ScriptInfo
+from flask.cli import FlaskGroup
 
 import annif
 import annif.corpus
 import annif.parallel
 import annif.project
 import annif.registry
-from annif.exception import (
-    ConfigurationException,
-    NotInitializedException,
-    NotSupportedException,
-)
+from annif import cli_util
+from annif.exception import NotInitializedException, NotSupportedException
 from annif.project import Access
-from annif.suggestion import ListSuggestionResult, SuggestionFilter
 from annif.util import metric_code
 
 logger = annif.logger
 click_log.basic_config(logger)
 
 cli = FlaskGroup(create_app=annif.create_app, add_version_option=False)
 cli = click.version_option(message="%(version)s")(cli)
 
 
-def get_project(project_id):
-    """
-    Helper function to get a project by ID and bail out if it doesn't exist"""
-    try:
-        return annif.registry.get_project(project_id, min_access=Access.private)
-    except ValueError:
-        click.echo("No projects found with id '{0}'.".format(project_id), err=True)
-        sys.exit(1)
-
-
-def get_vocab(vocab_id):
-    """
-    Helper function to get a vocabulary by ID and bail out if it doesn't
-    exist"""
-    try:
-        return annif.registry.get_vocab(vocab_id, min_access=Access.private)
-    except ValueError:
-        click.echo(f"No vocabularies found with the id '{vocab_id}'.", err=True)
-        sys.exit(1)
-
-
-def open_documents(paths, subject_index, vocab_lang, docs_limit):
-    """Helper function to open a document corpus from a list of pathnames,
-    each of which is either a TSV file or a directory of TXT files. For
-    directories with subjects in TSV files, the given vocabulary language
-    will be used to convert subject labels into URIs. The corpus will be
-    returned as an instance of DocumentCorpus or LimitingDocumentCorpus."""
-
-    def open_doc_path(path, subject_index):
-        """open a single path and return it as a DocumentCorpus"""
-        if os.path.isdir(path):
-            return annif.corpus.DocumentDirectory(
-                path, subject_index, vocab_lang, require_subjects=True
-            )
-        return annif.corpus.DocumentFile(path, subject_index)
-
-    if len(paths) == 0:
-        logger.warning("Reading empty file")
-        docs = open_doc_path(os.path.devnull, subject_index)
-    elif len(paths) == 1:
-        docs = open_doc_path(paths[0], subject_index)
-    else:
-        corpora = [open_doc_path(path, subject_index) for path in paths]
-        docs = annif.corpus.CombinedCorpus(corpora)
-    if docs_limit is not None:
-        docs = annif.corpus.LimitingDocumentCorpus(docs, docs_limit)
-    return docs
-
-
-def parse_backend_params(backend_param, project):
-    """Parse a list of backend parameters given with the --backend-param
-    option into a nested dict structure"""
-    backend_params = collections.defaultdict(dict)
-    for beparam in backend_param:
-        backend, param = beparam.split(".", 1)
-        key, val = param.split("=", 1)
-        validate_backend_params(backend, beparam, project)
-        backend_params[backend][key] = val
-    return backend_params
-
-
-def validate_backend_params(backend, beparam, project):
-    if backend != project.config["backend"]:
-        raise ConfigurationException(
-            'The backend {} in CLI option "-b {}" not matching the project'
-            " backend {}.".format(backend, beparam, project.config["backend"])
-        )
-
-
-BATCH_MAX_LIMIT = 15
-
-
-def generate_filter_batches(subjects):
-    import annif.eval
-
-    filter_batches = collections.OrderedDict()
-    for limit in range(1, BATCH_MAX_LIMIT + 1):
-        for threshold in [i * 0.05 for i in range(20)]:
-            hit_filter = SuggestionFilter(subjects, limit, threshold)
-            batch = annif.eval.EvaluationBatch(subjects)
-            filter_batches[(limit, threshold)] = (hit_filter, batch)
-    return filter_batches
-
-
-def set_project_config_file_path(ctx, param, value):
-    """Override the default path or the path given in env by CLI option"""
-    with ctx.ensure_object(ScriptInfo).load_app().app_context():
-        if value:
-            current_app.config["PROJECTS_CONFIG_PATH"] = value
-
-
-def common_options(f):
-    """Decorator to add common options for all CLI commands"""
-    f = click.option(
-        "-p",
-        "--projects",
-        help="Set path to project configuration file or directory",
-        type=click.Path(dir_okay=True, exists=True),
-        callback=set_project_config_file_path,
-        expose_value=False,
-        is_eager=True,
-    )(f)
-    return click_log.simple_verbosity_option(logger)(f)
-
-
-def backend_param_option(f):
-    """Decorator to add an option for CLI commands to override BE parameters"""
-    return click.option(
-        "--backend-param",
-        "-b",
-        multiple=True,
-        help="Override backend parameter of the config file. "
-        + "Syntax: `-b <backend>.<parameter>=<value>`.",
-    )(f)
-
-
 @cli.command("list-projects")
-@common_options
+@cli_util.common_options
 @click_log.simple_verbosity_option(logger, default="ERROR")
 def run_list_projects():
     """
     List available projects.
     \f
     Show a list of currently defined projects. Projects are defined in a
     configuration file, normally called ``projects.cfg``. See `Project
@@ -174,44 +53,44 @@
                 proj.project_id, proj.name, proj.language, str(proj.is_trained)
             )
         )
 
 
 @cli.command("show-project")
 @click.argument("project_id")
-@common_options
+@cli_util.common_options
 def run_show_project(project_id):
     """
     Show information about a project.
     """
 
-    proj = get_project(project_id)
+    proj = cli_util.get_project(project_id)
     click.echo(f"Project ID:        {proj.project_id}")
     click.echo(f"Project Name:      {proj.name}")
     click.echo(f"Language:          {proj.language}")
     click.echo(f"Vocabulary:        {proj.vocab.vocab_id}")
     click.echo(f"Vocab language:    {proj.vocab_lang}")
     click.echo(f"Access:            {proj.access.name}")
     click.echo(f"Trained:           {proj.is_trained}")
     click.echo(f"Modification time: {proj.modification_time}")
 
 
 @cli.command("clear")
 @click.argument("project_id")
-@common_options
+@cli_util.common_options
 def run_clear_project(project_id):
     """
     Initialize the project to its original, untrained state.
     """
-    proj = get_project(project_id)
+    proj = cli_util.get_project(project_id)
     proj.remove_model_data()
 
 
 @cli.command("list-vocabs")
-@common_options
+@cli_util.common_options
 @click_log.simple_verbosity_option(logger, default="ERROR")
 def run_list_vocabs():
     """
     List available vocabularies.
     """
 
     template = "{0: <20}{1: <20}{2: >10}  {3: <6}"
@@ -235,36 +114,35 @@
 @click.argument("subjectfile", type=click.Path(exists=True, dir_okay=False))
 @click.option("--language", "-L", help="Language of subject file")
 @click.option(
     "--force",
     "-f",
     default=False,
     is_flag=True,
-    help="Replace existing vocabulary completely " + "instead of updating it",
+    help="Replace existing vocabulary completely instead of updating it",
 )
-@common_options
+@cli_util.common_options
 def run_load_vocab(vocab_id, language, force, subjectfile):
     """
     Load a vocabulary from a subject file.
     """
-    vocab = get_vocab(vocab_id)
+    vocab = cli_util.get_vocab(vocab_id)
     if annif.corpus.SubjectFileSKOS.is_rdf_file(subjectfile):
         # SKOS/RDF file supported by rdflib
         subjects = annif.corpus.SubjectFileSKOS(subjectfile)
         click.echo(f"Loading vocabulary from SKOS file {subjectfile}...")
     elif annif.corpus.SubjectFileCSV.is_csv_file(subjectfile):
         # CSV file
         subjects = annif.corpus.SubjectFileCSV(subjectfile)
         click.echo(f"Loading vocabulary from CSV file {subjectfile}...")
     else:
         # probably a TSV file - we need to know its language
         if not language:
             click.echo(
-                "Please use --language option to set the language of "
-                + "a TSV vocabulary.",
+                "Please use --language option to set the language of a TSV vocabulary.",
                 err=True,
             )
             sys.exit(1)
         click.echo(f"Loading vocabulary from TSV file {subjectfile}...")
         subjects = annif.corpus.SubjectFileTSV(subjectfile, language)
     vocab.load_vocabulary(subjects, force=force)
 
@@ -275,109 +153,112 @@
 @click.option(
     "--cached/--no-cached",
     "-c/-C",
     default=False,
     help="Reuse preprocessed training data from previous run",
 )
 @click.option(
-    "--docs-limit",
-    "-d",
-    default=None,
-    type=click.IntRange(0, None),
-    help="Maximum number of documents to use",
-)
-@click.option(
     "--jobs",
     "-j",
     default=0,
     help="Number of parallel jobs (0 means choose automatically)",
 )
-@backend_param_option
-@common_options
+@cli_util.docs_limit_option
+@cli_util.backend_param_option
+@cli_util.common_options
 def run_train(project_id, paths, cached, docs_limit, jobs, backend_param):
     """
     Train a project on a collection of documents.
     \f
     This will train the project using the documents from ``PATHS`` (directories
     or possibly gzipped TSV files) in a single batch operation. If ``--cached``
     is set, preprocessed training data from the previous run is reused instead
     of documents input; see `Reusing preprocessed training data
     <https://github.com/NatLibFi/Annif/wiki/
     Reusing-preprocessed-training-data>`_.
     """
-    proj = get_project(project_id)
-    backend_params = parse_backend_params(backend_param, proj)
+    proj = cli_util.get_project(project_id)
+    backend_params = cli_util.parse_backend_params(backend_param, proj)
     if cached:
         if len(paths) > 0:
             raise click.UsageError(
                 "Corpus paths cannot be given when using --cached option."
             )
         documents = "cached"
     else:
-        documents = open_documents(paths, proj.subjects, proj.vocab_lang, docs_limit)
+        documents = cli_util.open_documents(
+            paths, proj.subjects, proj.vocab_lang, docs_limit
+        )
     proj.train(documents, backend_params, jobs)
 
 
 @cli.command("learn")
 @click.argument("project_id")
 @click.argument("paths", type=click.Path(exists=True), nargs=-1)
-@click.option(
-    "--docs-limit",
-    "-d",
-    default=None,
-    type=click.IntRange(0, None),
-    help="Maximum number of documents to use",
-)
-@backend_param_option
-@common_options
+@cli_util.docs_limit_option
+@cli_util.backend_param_option
+@cli_util.common_options
 def run_learn(project_id, paths, docs_limit, backend_param):
     """
     Further train an existing project on a collection of documents.
     \f
     Similar to the ``train`` command. This will continue training an already
     trained project using the documents given by ``PATHS`` in a single batch
     operation. Not supported by all backends.
     """
-    proj = get_project(project_id)
-    backend_params = parse_backend_params(backend_param, proj)
-    documents = open_documents(paths, proj.subjects, proj.vocab_lang, docs_limit)
+    proj = cli_util.get_project(project_id)
+    backend_params = cli_util.parse_backend_params(backend_param, proj)
+    documents = cli_util.open_documents(
+        paths, proj.subjects, proj.vocab_lang, docs_limit
+    )
     proj.learn(documents, backend_params)
 
 
 @cli.command("suggest")
 @click.argument("project_id")
+@click.argument(
+    "paths", type=click.Path(dir_okay=False, exists=True, allow_dash=True), nargs=-1
+)
 @click.option("--limit", "-l", default=10, help="Maximum number of subjects")
 @click.option("--threshold", "-t", default=0.0, help="Minimum score threshold")
 @click.option("--language", "-L", help="Language of subject labels")
-@backend_param_option
-@common_options
-def run_suggest(project_id, limit, threshold, language, backend_param):
+@cli_util.docs_limit_option
+@cli_util.backend_param_option
+@cli_util.common_options
+def run_suggest(
+    project_id, paths, limit, threshold, language, backend_param, docs_limit
+):
     """
-    Suggest subjects for a single document from standard input.
+    Suggest subjects for a single document from standard input or for one or more
+    document file(s) given its/their path(s).
     \f
     This will read a text document from standard input and suggest subjects for
-    it.
+    it, or if given path(s) to file(s), suggest subjects for it/them.
     """
-    project = get_project(project_id)
-    text = sys.stdin.read()
+    project = cli_util.get_project(project_id)
     lang = language or project.vocab_lang
     if lang not in project.vocab.languages:
         raise click.BadParameter(f'language "{lang}" not supported by vocabulary')
-    backend_params = parse_backend_params(backend_param, project)
-    hit_filter = SuggestionFilter(project.subjects, limit, threshold)
-    hits = hit_filter(project.suggest(text, backend_params))
-    for hit in hits.as_list():
-        subj = project.subjects[hit.subject_id]
-        click.echo(
-            "<{}>\t{}\t{}".format(
-                subj.uri,
-                "\t".join(filter(None, (subj.labels[lang], subj.notation))),
-                hit.score,
-            )
-        )
+    backend_params = cli_util.parse_backend_params(backend_param, project)
+
+    if paths and not (len(paths) == 1 and paths[0] == "-"):
+        docs = cli_util.open_text_documents(paths, docs_limit)
+        results = project.suggest_corpus(docs, backend_params).filter(limit, threshold)
+        for (
+            suggestions,
+            path,
+        ) in zip(results, paths):
+            click.echo(f"Suggestions for {path}")
+            cli_util.show_hits(suggestions, project, lang)
+    else:
+        text = sys.stdin.read()
+        suggestions = project.suggest([text], backend_params).filter(limit, threshold)[
+            0
+        ]
+        cli_util.show_hits(suggestions, project, lang)
 
 
 @cli.command("index")
 @click.argument("project_id")
 @click.argument("directory", type=click.Path(exists=True, file_okay=False))
 @click.option(
     "--suffix", "-s", default=".annif", help="File name suffix for result files"
@@ -387,67 +268,52 @@
     "-f/-F",
     default=False,
     help="Force overwriting of existing result files",
 )
 @click.option("--limit", "-l", default=10, help="Maximum number of subjects")
 @click.option("--threshold", "-t", default=0.0, help="Minimum score threshold")
 @click.option("--language", "-L", help="Language of subject labels")
-@backend_param_option
-@common_options
+@cli_util.backend_param_option
+@cli_util.common_options
 def run_index(
     project_id, directory, suffix, force, limit, threshold, language, backend_param
 ):
     """
     Index a directory with documents, suggesting subjects for each document.
     Write the results in TSV files with the given suffix (``.annif`` by
     default).
     """
-    project = get_project(project_id)
+    project = cli_util.get_project(project_id)
     lang = language or project.vocab_lang
     if lang not in project.vocab.languages:
         raise click.BadParameter(f'language "{lang}" not supported by vocabulary')
-    backend_params = parse_backend_params(backend_param, project)
-    hit_filter = SuggestionFilter(project.subjects, limit, threshold)
+    backend_params = cli_util.parse_backend_params(backend_param, project)
+
+    documents = annif.corpus.DocumentDirectory(
+        directory, None, None, require_subjects=False
+    )
+    results = project.suggest_corpus(documents, backend_params).filter(limit, threshold)
 
-    for docfilename, dummy_subjectfn in annif.corpus.DocumentDirectory(
-        directory, project.subjects, project.vocab_lang, require_subjects=False
-    ):
-        with open(docfilename, encoding="utf-8-sig") as docfile:
-            text = docfile.read()
+    for (docfilename, _), suggestions in zip(documents, results):
         subjectfilename = re.sub(r"\.txt$", suffix, docfilename)
         if os.path.exists(subjectfilename) and not force:
             click.echo(
                 "Not overwriting {} (use --force to override)".format(subjectfilename)
             )
             continue
         with open(subjectfilename, "w", encoding="utf-8") as subjfile:
-            results = project.suggest(text, backend_params)
-            for hit in hit_filter(results).as_list():
-                subj = project.subjects[hit.subject_id]
-                line = "<{}>\t{}\t{}".format(
-                    subj.uri,
-                    "\t".join(filter(None, (subj.labels[lang], subj.notation))),
-                    hit.score,
-                )
-                click.echo(line, file=subjfile)
+            cli_util.show_hits(suggestions, project, lang, file=subjfile)
 
 
 @cli.command("eval")
 @click.argument("project_id")
 @click.argument("paths", type=click.Path(exists=True), nargs=-1)
 @click.option("--limit", "-l", default=10, help="Maximum number of subjects")
 @click.option("--threshold", "-t", default=0.0, help="Minimum score threshold")
 @click.option(
-    "--docs-limit",
-    "-d",
-    default=None,
-    type=click.IntRange(0, None),
-    help="Maximum number of documents to use",
-)
-@click.option(
     "--metric",
     "-m",
     default=[],
     multiple=True,
     help="Metric to calculate (default: all)",
 )
 @click.option(
@@ -463,16 +329,17 @@
     type=click.File("w", encoding="utf-8", errors="ignore", lazy=True),
     help="""Specify file in order to write non-aggregated results per subject.
     File directory must exist, existing file will be overwritten.""",
 )
 @click.option(
     "--jobs", "-j", default=1, help="Number of parallel jobs (0 means all CPUs)"
 )
-@backend_param_option
-@common_options
+@cli_util.docs_limit_option
+@cli_util.backend_param_option
+@cli_util.common_options
 def run_eval(
     project_id,
     paths,
     limit,
     threshold,
     docs_limit,
     metric,
@@ -491,16 +358,16 @@
     subjects match the gold-standard subjects in the documents.
 
     Normally the output is the list of the metrics calculated across documents.
     If ``--results-file <FILENAME>`` option is given, the metrics are
     calculated separately for each subject, and written to the given file.
     """
 
-    project = get_project(project_id)
-    backend_params = parse_backend_params(backend_param, project)
+    project = cli_util.get_project(project_id)
+    backend_params = cli_util.parse_backend_params(backend_param, project)
 
     import annif.eval
 
     eval_batch = annif.eval.EvaluationBatch(project.subjects)
 
     if results_file:
         try:
@@ -510,26 +377,29 @@
                     results_file.name
                 )
             )
         except Exception as e:
             raise NotSupportedException(
                 "cannot open results-file for writing: " + str(e)
             )
-    docs = open_documents(paths, project.subjects, project.vocab_lang, docs_limit)
-
+    corpus = cli_util.open_documents(
+        paths, project.subjects, project.vocab_lang, docs_limit
+    )
     jobs, pool_class = annif.parallel.get_pool(jobs)
 
     project.initialize(parallel=True)
     psmap = annif.parallel.ProjectSuggestMap(
         project.registry, [project_id], backend_params, limit, threshold
     )
 
     with pool_class(jobs) as pool:
-        for hits, subject_set in pool.imap_unordered(psmap.suggest, docs.documents):
-            eval_batch.evaluate(hits[project_id], subject_set)
+        for hit_sets, subject_sets in pool.imap_unordered(
+            psmap.suggest_batch, corpus.doc_batches
+        ):
+            eval_batch.evaluate_many(hit_sets[project_id], subject_sets)
 
     template = "{0:<30}\t{1}"
     metrics = eval_batch.results(
         metrics=metric, results_file=results_file, language=project.vocab_lang
     )
     for metric, score in metrics.items():
         click.echo(template.format(metric + ":", score))
@@ -537,129 +407,145 @@
         json.dump(
             {metric_code(mname): val for mname, val in metrics.items()},
             metrics_file,
             indent=2,
         )
 
 
+FILTER_BATCH_MAX_LIMIT = 15
+OPTIMIZE_METRICS = ["Precision (doc avg)", "Recall (doc avg)", "F1 score (doc avg)"]
+
+
 @cli.command("optimize")
 @click.argument("project_id")
 @click.argument("paths", type=click.Path(exists=True), nargs=-1)
 @click.option(
-    "--docs-limit",
-    "-d",
-    default=None,
-    type=click.IntRange(0, None),
-    help="Maximum number of documents to use",
-)
-@backend_param_option
-@common_options
-def run_optimize(project_id, paths, docs_limit, backend_param):
+    "--jobs", "-j", default=1, help="Number of parallel jobs (0 means all CPUs)"
+)
+@cli_util.docs_limit_option
+@cli_util.backend_param_option
+@cli_util.common_options
+def run_optimize(project_id, paths, jobs, docs_limit, backend_param):
     """
     Suggest subjects for documents, testing multiple limits and thresholds.
     \f
     This command will use different limit (maximum number of subjects) and
     score threshold values when assigning subjects to each document given by
     ``PATHS`` and compare the results against the gold standard subjects in the
     documents. The output is a list of parameter combinations and their scores.
     From the output, you can determine the optimum limit and threshold
     parameters depending on which measure you want to target.
     """
-    project = get_project(project_id)
-    backend_params = parse_backend_params(backend_param, project)
+    project = cli_util.get_project(project_id)
+    backend_params = cli_util.parse_backend_params(backend_param, project)
+    filter_params = cli_util.generate_filter_params(FILTER_BATCH_MAX_LIMIT)
+
+    import annif.eval
+
+    corpus = cli_util.open_documents(
+        paths, project.subjects, project.vocab_lang, docs_limit
+    )
 
-    filter_batches = generate_filter_batches(project.subjects)
+    jobs, pool_class = annif.parallel.get_pool(jobs)
+
+    project.initialize(parallel=True)
+    psmap = annif.parallel.ProjectSuggestMap(
+        project.registry,
+        [project_id],
+        backend_params,
+        limit=FILTER_BATCH_MAX_LIMIT,
+        threshold=0.0,
+    )
 
     ndocs = 0
-    docs = open_documents(paths, project.subjects, project.vocab_lang, docs_limit)
-    for doc in docs.documents:
-        raw_hits = project.suggest(doc.text, backend_params)
-        hits = raw_hits.filter(project.subjects, limit=BATCH_MAX_LIMIT)
-        assert isinstance(hits, ListSuggestionResult), (
-            "Optimize should only be done with ListSuggestionResult "
-            + "as it would be very slow with VectorSuggestionResult."
-        )
-        for hit_filter, batch in filter_batches.values():
-            batch.evaluate(hit_filter(hits), doc.subject_set)
-        ndocs += 1
+    suggestion_batches = []
+    subject_set_batches = []
+    with pool_class(jobs) as pool:
+        for suggestion_batch, subject_sets in pool.imap_unordered(
+            psmap.suggest_batch, corpus.doc_batches
+        ):
+            ndocs += len(suggestion_batch[project_id])
+            suggestion_batches.append(suggestion_batch[project_id])
+            subject_set_batches.append(subject_sets)
+
+    from annif.suggestion import SuggestionResults
+
+    orig_suggestion_results = SuggestionResults(suggestion_batches)
 
     click.echo("\t".join(("Limit", "Thresh.", "Prec.", "Rec.", "F1")))
 
     best_scores = collections.defaultdict(float)
     best_params = {}
 
     template = "{:d}\t{:.02f}\t{:.04f}\t{:.04f}\t{:.04f}"
-    # Store the batches in a list that gets consumed along the way
-    # This way GC will have a chance to reclaim the memory
-    filter_batches = list(filter_batches.items())
-    while filter_batches:
-        params, filter_batch = filter_batches.pop(0)
-        metrics = ["Precision (doc avg)", "Recall (doc avg)", "F1 score (doc avg)"]
-        results = filter_batch[1].results(metrics=metrics)
+    import annif.eval
+
+    for limit, threshold in filter_params:
+        eval_batch = annif.eval.EvaluationBatch(project.subjects)
+        filtered_results = orig_suggestion_results.filter(limit, threshold)
+        for batch, subject_sets in zip(filtered_results.batches, subject_set_batches):
+            eval_batch.evaluate_many(batch, subject_sets)
+        results = eval_batch.results(metrics=OPTIMIZE_METRICS)
         for metric, score in results.items():
             if score >= best_scores[metric]:
                 best_scores[metric] = score
-                best_params[metric] = params
+                best_params[metric] = (limit, threshold)
         click.echo(
             template.format(
-                params[0],
-                params[1],
+                limit,
+                threshold,
                 results["Precision (doc avg)"],
                 results["Recall (doc avg)"],
                 results["F1 score (doc avg)"],
             )
         )
 
     click.echo()
     template2 = "Best {:>19}: {:.04f}\tLimit: {:d}\tThreshold: {:.02f}"
-    for metric in metrics:
+    for metric in OPTIMIZE_METRICS:
         click.echo(
             template2.format(
                 metric,
                 best_scores[metric],
                 best_params[metric][0],
                 best_params[metric][1],
             )
         )
     click.echo("Documents evaluated:\t{}".format(ndocs))
 
 
 @cli.command("hyperopt")
 @click.argument("project_id")
 @click.argument("paths", type=click.Path(exists=True), nargs=-1)
-@click.option(
-    "--docs-limit",
-    "-d",
-    default=None,
-    type=click.IntRange(0, None),
-    help="Maximum number of documents to use",
-)
 @click.option("--trials", "-T", default=10, help="Number of trials")
 @click.option(
     "--jobs", "-j", default=1, help="Number of parallel runs (0 means all CPUs)"
 )
 @click.option(
     "--metric", "-m", default="NDCG", help="Metric to optimize (default: NDCG)"
 )
 @click.option(
     "--results-file",
     "-r",
     type=click.File("w", encoding="utf-8", errors="ignore", lazy=True),
     help="""Specify file path to write trial results as CSV.
     File directory must exist, existing file will be overwritten.""",
 )
-@common_options
+@cli_util.docs_limit_option
+@cli_util.common_options
 def run_hyperopt(project_id, paths, docs_limit, trials, jobs, metric, results_file):
     """
     Optimize the hyperparameters of a project using validation documents from
     ``PATHS``. Not supported by all backends. Output is a list of trial results
     and a report of the best performing parameters.
     """
-    proj = get_project(project_id)
-    documents = open_documents(paths, proj.subjects, proj.vocab_lang, docs_limit)
+    proj = cli_util.get_project(project_id)
+    documents = cli_util.open_documents(
+        paths, proj.subjects, proj.vocab_lang, docs_limit
+    )
     click.echo(f"Looking for optimal hyperparameters using {trials} trials")
     rec = proj.hyperopt(documents, trials, jobs, metric, results_file)
     click.echo(f"Got best {metric} score {rec.score:.4f} with:")
     click.echo("---")
     for line in rec.lines:
         click.echo(line)
     click.echo("---")
```

### Comparing `annif-0.60.0/annif/config.py` & `annif-0.61.0/annif/config.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/corpus/__init__.py` & `annif-0.61.0/annif/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/corpus/document.py` & `annif-0.61.0/annif/corpus/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
                 yield (filename, None)
 
     @property
     def documents(self):
         for docfilename, keyfilename in self:
             with open(docfilename, errors="replace", encoding="utf-8-sig") as docfile:
                 text = docfile.read()
+            if keyfilename is None:
+                yield Document(text=text, subject_set=None)
+                continue
             with open(keyfilename, encoding="utf-8-sig") as keyfile:
                 subjects = SubjectSet.from_string(
                     keyfile.read(), self.subject_index, self.language
                 )
             yield Document(text=text, subject_set=subjects)
```

### Comparing `annif-0.60.0/annif/corpus/skos.py` & `annif-0.61.0/annif/corpus/skos.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/corpus/subject.py` & `annif-0.61.0/annif/corpus/subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Classes for supporting subject corpora expressed as directories or files"""
 
 import csv
 import os.path
 
 import numpy as np
 
+import annif
 import annif.util
-from annif import logger
 
 from .skos import serialize_subjects_to_skos
 from .types import Subject, SubjectCorpus
 
+logger = annif.logger.getChild("subject")
+logger.addFilter(annif.util.DuplicateFilter())
+
 
 class SubjectFileTSV(SubjectCorpus):
     """A monolingual subject vocabulary stored in a TSV file."""
 
     def __init__(self, path, language):
         """initialize the SubjectFileTSV given a path to a TSV file and the
         language of the vocabulary"""
@@ -266,12 +269,13 @@
 
     def as_vector(self, size=None, destination=None):
         """Return the hits as a one-dimensional NumPy array in sklearn
         multilabel indicator format. Use destination array if given (not
         None), otherwise create and return a new one of the given size."""
 
         if destination is None:
+            assert size is not None and size > 0
             destination = np.zeros(size, dtype=bool)
 
         destination[list(self._subject_ids)] = True
 
         return destination
```

### Comparing `annif-0.60.0/annif/datadir.py` & `annif-0.61.0/annif/datadir.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/default_config.py` & `annif-0.61.0/annif/default_config.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/eval.py` & `annif-0.61.0/annif/eval.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,152 @@
 """Evaluation metrics for Annif"""
 
-import statistics
 import warnings
 
 import numpy as np
-from scipy.sparse import csr_matrix
-from sklearn.metrics import (
-    f1_score,
-    label_ranking_average_precision_score,
-    precision_score,
-    recall_score,
-)
+import scipy.sparse
+from sklearn.metrics import f1_score, precision_score, recall_score
 
 from annif.exception import NotSupportedException
-
-
-def filter_pred_top_k(preds, limit):
-    """filter a 2D prediction vector, retaining only the top K suggestions
-    for each individual prediction; the rest will be set to zeros"""
-
-    masks = []
-    for pred in preds:
-        mask = np.zeros_like(pred, dtype=bool)
-        top_k = np.argsort(pred)[::-1][:limit]
-        mask[top_k] = True
-        masks.append(mask)
-    return preds * np.array(masks)
+from annif.suggestion import SuggestionBatch, filter_suggestion
 
 
 def true_positives(y_true, y_pred):
     """calculate the number of true positives using bitwise operations,
     emulating the way sklearn evaluation metric functions work"""
-    return int((y_true & y_pred).sum())
+    return int((y_true.multiply(y_pred)).sum())
 
 
 def false_positives(y_true, y_pred):
     """calculate the number of false positives using bitwise operations,
     emulating the way sklearn evaluation metric functions work"""
-    return int((~y_true & y_pred).sum())
+    return int((y_true < y_pred).sum())
 
 
 def false_negatives(y_true, y_pred):
     """calculate the number of false negatives using bitwise operations,
     emulating the way sklearn evaluation metric functions work"""
-    return int((y_true & ~y_pred).sum())
-
-
-def precision_at_k_score(y_true, y_pred, limit):
-    """calculate the precision at K, i.e. the number of relevant items
-    among the top K predicted ones"""
-    scores = []
-    for true, pred in zip(y_true, y_pred):
-        order = pred.argsort()[::-1]
-        orderlimit = min(limit, np.count_nonzero(pred))
-        order = order[:orderlimit]
-        gain = true[order]
-        if orderlimit > 0:
-            scores.append(gain.sum() / orderlimit)
-        else:
-            scores.append(0.0)
-    return statistics.mean(scores)
+    return int((y_true > y_pred).sum())
 
 
 def dcg_score(y_true, y_pred, limit=None):
     """return the discounted cumulative gain (DCG) score for the selected
     labels vs. relevant labels"""
-    order = y_pred.argsort()[::-1]
-    n_pred = np.count_nonzero(y_pred)
+
+    n_pred = y_pred.count_nonzero()
     if limit is not None:
         n_pred = min(limit, n_pred)
-    order = order[:n_pred]
-    gain = y_true[order]
-    discount = np.log2(np.arange(order.size) + 2)
 
+    top_k = y_pred.data.argsort()[-n_pred:][::-1]
+    order = y_pred.indices[top_k]
+    gain = y_true[:, order]
+    discount = np.log2(np.arange(1, n_pred + 1) + 1)
     return (gain / discount).sum()
 
 
 def ndcg_score(y_true, y_pred, limit=None):
     """return the normalized discounted cumulative gain (nDCG) score for the
     selected labels vs. relevant labels"""
-    scores = []
-    for true, pred in zip(y_true, y_pred):
+
+    scores = np.ones(y_true.shape[0], dtype=np.float32)
+    for i in range(y_true.shape[0]):
+        true = y_true.getrow(i)
         idcg = dcg_score(true, true, limit)
-        dcg = dcg_score(true, pred, limit)
         if idcg > 0:
-            scores.append(dcg / idcg)
-        else:
-            scores.append(1.0)  # perfect score for no relevant hits case
-    return statistics.mean(scores)
+            pred = y_pred.getrow(i)
+            dcg = dcg_score(true, pred, limit)
+            scores[i] = dcg / idcg
+
+    return float(scores.mean())
 
 
 class EvaluationBatch:
     """A class for evaluating batches of results using all available metrics.
-    The evaluate() method is called once per document in the batch.
-    Final results can be queried using the results() method."""
+    The evaluate() method is called once per document in the batch or evaluate_many()
+    for a list of documents of the batch. Final results can be queried using the
+    results() method."""
 
     def __init__(self, subject_index):
         self._subject_index = subject_index
-        self._samples = []
+        self._suggestion_arrays = []
+        self._gold_subject_arrays = []
 
-    def evaluate(self, hits, gold_subjects):
-        self._samples.append((hits, gold_subjects))
+    def evaluate_many(self, suggestion_batch, gold_subject_batch):
+        if not isinstance(suggestion_batch, SuggestionBatch):
+            suggestion_batch = SuggestionBatch.from_sequence(
+                suggestion_batch, self._subject_index
+            )
+        self._suggestion_arrays.append(suggestion_batch.array)
+
+        # convert gold_subject_batch to sparse matrix
+        ar = scipy.sparse.dok_array(
+            (len(gold_subject_batch), len(self._subject_index)), dtype=bool
+        )
+        for idx, subject_set in enumerate(gold_subject_batch):
+            for subject_id in subject_set:
+                ar[idx, subject_id] = True
+        self._gold_subject_arrays.append(ar.tocsr())
 
     def _evaluate_samples(self, y_true, y_pred, metrics=[]):
         y_pred_binary = y_pred > 0.0
-        y_true_sparse = csr_matrix(y_true)
 
         # define the available metrics as lazy lambda functions
         # so we can execute only the ones actually requested
         all_metrics = {
             "Precision (doc avg)": lambda: precision_score(
-                y_true_sparse, y_pred_binary, average="samples"
+                y_true, y_pred_binary, average="samples"
             ),
             "Recall (doc avg)": lambda: recall_score(
-                y_true_sparse, y_pred_binary, average="samples"
+                y_true, y_pred_binary, average="samples"
             ),
             "F1 score (doc avg)": lambda: f1_score(
-                y_true_sparse, y_pred_binary, average="samples"
+                y_true, y_pred_binary, average="samples"
             ),
             "Precision (subj avg)": lambda: precision_score(
-                y_true_sparse, y_pred_binary, average="macro"
+                y_true, y_pred_binary, average="macro"
             ),
             "Recall (subj avg)": lambda: recall_score(
-                y_true_sparse, y_pred_binary, average="macro"
+                y_true, y_pred_binary, average="macro"
             ),
             "F1 score (subj avg)": lambda: f1_score(
-                y_true_sparse, y_pred_binary, average="macro"
+                y_true, y_pred_binary, average="macro"
             ),
             "Precision (weighted subj avg)": lambda: precision_score(
-                y_true_sparse, y_pred_binary, average="weighted"
+                y_true, y_pred_binary, average="weighted"
             ),
             "Recall (weighted subj avg)": lambda: recall_score(
-                y_true_sparse, y_pred_binary, average="weighted"
+                y_true, y_pred_binary, average="weighted"
             ),
             "F1 score (weighted subj avg)": lambda: f1_score(
-                y_true_sparse, y_pred_binary, average="weighted"
+                y_true, y_pred_binary, average="weighted"
             ),
             "Precision (microavg)": lambda: precision_score(
-                y_true_sparse, y_pred_binary, average="micro"
+                y_true, y_pred_binary, average="micro"
             ),
             "Recall (microavg)": lambda: recall_score(
-                y_true_sparse, y_pred_binary, average="micro"
+                y_true, y_pred_binary, average="micro"
             ),
             "F1 score (microavg)": lambda: f1_score(
-                y_true_sparse, y_pred_binary, average="micro"
+                y_true, y_pred_binary, average="micro"
             ),
             "F1@5": lambda: f1_score(
-                y_true_sparse, filter_pred_top_k(y_pred, 5) > 0.0, average="samples"
+                y_true, filter_suggestion(y_pred, 5) > 0.0, average="samples"
             ),
             "NDCG": lambda: ndcg_score(y_true, y_pred),
             "NDCG@5": lambda: ndcg_score(y_true, y_pred, limit=5),
             "NDCG@10": lambda: ndcg_score(y_true, y_pred, limit=10),
-            "Precision@1": lambda: precision_at_k_score(y_true, y_pred, limit=1),
-            "Precision@3": lambda: precision_at_k_score(y_true, y_pred, limit=3),
-            "Precision@5": lambda: precision_at_k_score(y_true, y_pred, limit=5),
-            "LRAP": lambda: label_ranking_average_precision_score(y_true, y_pred),
+            "Precision@1": lambda: precision_score(
+                y_true, filter_suggestion(y_pred, 1) > 0.0, average="samples"
+            ),
+            "Precision@3": lambda: precision_score(
+                y_true, filter_suggestion(y_pred, 3) > 0.0, average="samples"
+            ),
+            "Precision@5": lambda: precision_score(
+                y_true, filter_suggestion(y_pred, 5) > 0.0, average="samples"
+            ),
             "True positives": lambda: true_positives(y_true, y_pred_binary),
             "False positives": lambda: false_positives(y_true, y_pred_binary),
             "False negatives": lambda: false_negatives(y_true, y_pred_binary),
         }
 
         if not metrics:
             metrics = all_metrics.keys()
@@ -191,56 +179,50 @@
             print("\t".join((str(e) for e in row)), file=results_file)
 
     def output_result_per_subject(self, y_true, y_pred, results_file, language):
         """Write results per subject (non-aggregated)
         to outputfile results_file, using labels in the given language"""
 
         y_pred = y_pred.T > 0.0
-        y_true = y_true.T > 0.0
-
-        true_pos = y_true & y_pred
-        false_pos = ~y_true & y_pred
-        false_neg = y_true & ~y_pred
+        y_true = y_true.T
 
-        r = len(y_true)
+        true_pos = y_true.multiply(y_pred).sum(axis=1)
+        false_pos = (y_true < y_pred).sum(axis=1)
+        false_neg = (y_true > y_pred).sum(axis=1)
+
+        with np.errstate(invalid="ignore"):
+            precision = np.nan_to_num(true_pos / (true_pos + false_pos))
+            recall = np.nan_to_num(true_pos / (true_pos + false_neg))
+            f1_score = np.nan_to_num(2 * (precision * recall) / (precision + recall))
 
         zipped = zip(
             [subj.uri for subj in self._subject_index],  # URI
             [subj.labels[language] for subj in self._subject_index],  # Label
-            np.sum((true_pos + false_neg), axis=1),  # Support
-            np.sum(true_pos, axis=1),  # True_positives
-            np.sum(false_pos, axis=1),  # False_positives
-            np.sum(false_neg, axis=1),  # False_negatives
-            [
-                precision_score(y_true[i], y_pred[i], zero_division=0) for i in range(r)
-            ],  # Precision
-            [
-                recall_score(y_true[i], y_pred[i], zero_division=0) for i in range(r)
-            ],  # Recall
-            [f1_score(y_true[i], y_pred[i], zero_division=0) for i in range(r)],
-        )  # F1
+            y_true.sum(axis=1),  # Support
+            true_pos,  # True positives
+            false_pos,  # False positives
+            false_neg,  # False negatives
+            precision,  # Precision
+            recall,  # Recall
+            f1_score,  # F1 score
+        )
         self._result_per_subject_header(results_file)
         self._result_per_subject_body(zipped, results_file)
 
     def results(self, metrics=[], results_file=None, language=None):
         """evaluate a set of selected subjects against a gold standard using
         different metrics. If metrics is empty, use all available metrics.
         If results_file (file object) given, write results per subject to it
         with labels expressed in the given language."""
 
-        if not self._samples:
+        if not self._suggestion_arrays:
             raise NotSupportedException("cannot evaluate empty corpus")
 
-        shape = (len(self._samples), len(self._subject_index))
-        y_true = np.zeros(shape, dtype=bool)
-        y_pred = np.zeros(shape, dtype=np.float32)
-
-        for idx, (hits, gold_subjects) in enumerate(self._samples):
-            gold_subjects.as_vector(destination=y_true[idx])
-            hits.as_vector(len(self._subject_index), destination=y_pred[idx])
+        y_pred = scipy.sparse.csr_array(scipy.sparse.vstack(self._suggestion_arrays))
+        y_true = scipy.sparse.csr_array(scipy.sparse.vstack(self._gold_subject_arrays))
 
         results = self._evaluate_samples(y_true, y_pred, metrics)
         results["Documents evaluated"] = int(y_true.shape[0])
 
         if results_file:
             self.output_result_per_subject(y_true, y_pred, results_file, language)
         return results
```

### Comparing `annif-0.60.0/annif/exception.py` & `annif-0.61.0/annif/exception.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/lexical/mllm.py` & `annif-0.61.0/annif/lexical/mllm.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,14 @@
         with pool_class(
             jobs, initializer=MLLMCandidateGenerator.init, initargs=(cg_args,)
         ) as pool:
             params = ((doc.subject_set, doc.text) for doc in corpus.documents)
             for doc_subject_ids, candidates in pool.starmap(
                 MLLMCandidateGenerator.generate_candidates, params, 10
             ):
-
                 self._subj_freq.update(doc_subject_ids)
                 self._doc_freq.update([c.subject_id for c in candidates])
                 train_x.append(candidates)
                 train_y += [(c.subject_id in doc_subject_ids) for c in candidates]
 
         return (train_x, train_y)
```

### Comparing `annif-0.60.0/annif/lexical/tokenset.py` & `annif-0.61.0/annif/lexical/tokenset.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/lexical/util.py` & `annif-0.61.0/annif/lexical/util.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/parallel.py` & `annif-0.61.0/annif/parallel.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,20 +38,28 @@
         self.limit = limit
         self.threshold = threshold
 
     def suggest(self, doc):
         filtered_hits = {}
         for project_id in self.project_ids:
             project = self.registry.get_project(project_id)
-            hits = project.suggest(doc.text, self.backend_params)
-            filtered_hits[project_id] = hits.filter(
-                project.subjects, self.limit, self.threshold
-            )
+            batch = project.suggest([doc.text], self.backend_params)
+            filtered_hits[project_id] = batch.filter(self.limit, self.threshold)[0]
         return (filtered_hits, doc.subject_set)
 
+    def suggest_batch(self, batch):
+        filtered_hit_sets = {}
+        texts, subject_sets = zip(*[(doc.text, doc.subject_set) for doc in batch])
+
+        for project_id in self.project_ids:
+            project = self.registry.get_project(project_id)
+            batch = project.suggest(texts, self.backend_params)
+            filtered_hit_sets[project_id] = batch.filter(self.limit, self.threshold)
+        return (filtered_hit_sets, subject_sets)
+
 
 def get_pool(n_jobs):
     """return a suitable multiprocessing pool class, and the correct jobs
     argument for its constructor, for the given amount of parallel jobs"""
 
     ctx = multiprocessing.get_context(MP_START_METHOD)
```

### Comparing `annif-0.60.0/annif/project.py` & `annif-0.61.0/annif/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os.path
 from shutil import rmtree
 
 import annif
 import annif.analyzer
 import annif.backend
 import annif.corpus
-import annif.suggestion
 import annif.transform
 from annif.datadir import DatadirMixin
 from annif.exception import (
     AnnifException,
     ConfigurationException,
     NotInitializedException,
     NotSupportedException,
@@ -105,21 +104,19 @@
 
         self._initialize_analyzer()
         self._initialize_subjects()
         self._initialize_backend(parallel)
 
         self.initialized = True
 
-    def _suggest_with_backend(self, text, backend_params):
+    def _suggest_with_backend(self, texts, backend_params):
         if backend_params is None:
             backend_params = {}
         beparams = backend_params.get(self.backend.backend_id, {})
-        hits = self.backend.suggest(text, beparams)
-        logger.debug("Got %d hits from backend %s", len(hits), self.backend.backend_id)
-        return hits
+        return self.backend.suggest(texts, beparams)
 
     @property
     def analyzer(self):
         if self._analyzer is None:
             if self.analyzer_spec:
                 self._analyzer = annif.analyzer.get_analyzer(self.analyzer_spec)
             else:
@@ -195,29 +192,33 @@
     def is_trained(self):
         return self._get_info("is_trained")
 
     @property
     def modification_time(self):
         return self._get_info("modification_time")
 
-    def suggest(self, text, backend_params=None):
-        """Suggest subjects the given text by passing it to the backend. Returns a
-        list of SubjectSuggestion objects ordered by decreasing score."""
+    def suggest_corpus(self, corpus, backend_params=None):
+        """Suggest subjects for the given documents corpus in batches of documents."""
+        suggestions = (
+            self.suggest([doc.text for doc in doc_batch], backend_params)
+            for doc_batch in corpus.doc_batches
+        )
+        import annif.suggestion
+
+        return annif.suggestion.SuggestionResults(suggestions)
+
+    def suggest(self, texts, backend_params=None):
+        """Suggest subjects for the given documents batch."""
         if not self.is_trained:
             if self.is_trained is None:
                 logger.warning("Could not get train state information.")
             else:
                 raise NotInitializedException("Project is not trained.")
-        logger.debug(
-            'Suggesting subjects for text "%s..." (len=%d)', text[:20], len(text)
-        )
-        text = self.transform.transform_text(text)
-        hits = self._suggest_with_backend(text, backend_params)
-        logger.debug("%d hits from backend", len(hits))
-        return hits
+        texts = [self.transform.transform_text(text) for text in texts]
+        return self._suggest_with_backend(texts, backend_params)
 
     def train(self, corpus, backend_params=None, jobs=0):
         """train the project using documents from a metadata source"""
         if corpus != "cached":
             corpus = self.transform.transform_corpus(corpus)
         if backend_params is None:
             backend_params = {}
```

### Comparing `annif-0.60.0/annif/registry.py` & `annif-0.61.0/annif/registry.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/css/bootstrap.min.css` & `annif-0.61.0/annif/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/css/bootstrap.min.css.map` & `annif-0.61.0/annif/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/css/fonts.css` & `annif-0.61.0/annif/static/css/fonts.css`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/css/style.css` & `annif-0.61.0/annif/static/css/style.css`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/favicon.ico` & `annif-0.61.0/annif/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/fonts/Jost-400-Book.otf` & `annif-0.61.0/annif/static/fonts/Jost-400-Book.otf`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/fonts/Jost-400-Book.ttf` & `annif-0.61.0/annif/static/fonts/Jost-400-Book.ttf`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/fonts/Jost-500-Medium.otf` & `annif-0.61.0/annif/static/fonts/Jost-500-Medium.otf`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/fonts/Jost-500-Medium.ttf` & `annif-0.61.0/annif/static/fonts/Jost-500-Medium.ttf`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/img/annif-RGB.svg` & `annif-0.61.0/annif/static/img/annif-RGB.svg`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/img/arrow-white.svg` & `annif-0.61.0/annif/static/img/arrow-white.svg`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/js/axios.min.js` & `annif-0.61.0/annif/static/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/js/axios.min.js.map` & `annif-0.61.0/annif/static/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/js/bootstrap.min.js` & `annif-0.61.0/annif/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/js/bootstrap.min.js.map` & `annif-0.61.0/annif/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/static/js/vue.min.js` & `annif-0.61.0/annif/static/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/templates/home.html` & `annif-0.61.0/annif/templates/home.html`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/transform/__init__.py` & `annif-0.61.0/annif/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/transform/inputlimiter.py` & `annif-0.61.0/annif/transform/inputlimiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from annif.exception import ConfigurationException
 
 from . import transform
 
 
 class InputLimiter(transform.BaseTransform):
-
     name = "limit"
 
     def __init__(self, project, input_limit):
         super().__init__(project)
         self.input_limit = int(input_limit)
         self._validate_value(self.input_limit)
```

### Comparing `annif-0.60.0/annif/transform/langfilter.py` & `annif-0.61.0/annif/transform/langfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from . import transform
 
 logger = annif.logger
 
 
 class LangFilter(transform.BaseTransform):
-
     name = "filter_lang"
 
     def __init__(
         self, project, text_min_length=500, sentence_min_length=50, min_ratio=0.5
     ):
         super().__init__(project)
         self.text_min_length = int(text_min_length)
```

### Comparing `annif-0.60.0/annif/transform/transform.py` & `annif-0.61.0/annif/transform/transform.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/annif/util.py` & `annif-0.61.0/annif/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 """Utility functions for Annif"""
 
 import glob
+import logging
 import os
 import os.path
 import tempfile
 
-import numpy as np
-
 from annif import logger
-from annif.suggestion import VectorSuggestionResult
+
+
+class DuplicateFilter(logging.Filter):
+    """Filter out log messages that have already been displayed."""
+
+    def __init__(self):
+        super().__init__()
+        self.logged = set()
+
+    def filter(self, record):
+        current_log = hash((record.module, record.levelno, record.msg, record.args))
+        if current_log not in self.logged:
+            self.logged.add(current_log)
+            return True
+        return False
 
 
 def atomic_save(obj, dirname, filename, method=None):
     """Save the given object (which must have a .save() method, unless the
     method parameter is given) into the given directory with the given
     filename, using a temporary file and renaming the temporary file to the
     final name."""
@@ -34,25 +47,14 @@
 def cleanup_uri(uri):
     """remove angle brackets from a URI, if any"""
     if uri.startswith("<") and uri.endswith(">"):
         return uri[1:-1]
     return uri
 
 
-def merge_hits(weighted_hits, size):
-    """Merge hits from multiple sources. Input is a sequence of WeightedSuggestion
-    objects. The size parameter determines the length of the subject vector.
-    Returns an SuggestionResult object."""
-
-    weights = [whit.weight for whit in weighted_hits]
-    scores = [whit.hits.as_vector(size) for whit in weighted_hits]
-    result = np.average(scores, axis=0, weights=weights)
-    return VectorSuggestionResult(result)
-
-
 def parse_sources(sourcedef):
     """parse a source definition such as 'src1:1.0,src2' into a sequence of
     tuples (src_id, weight)"""
 
     sources = []
     totalweight = 0.0
     for srcdef in sourcedef.strip().split(","):
```

### Comparing `annif-0.60.0/annif/vocab.py` & `annif-0.61.0/annif/vocab.py`

 * *Files identical despite different names*

### Comparing `annif-0.60.0/pyproject.toml` & `annif-0.61.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "annif"
-version = "0.60.0"
+version = "0.61.0"
 description = "Automated subject indexing and classification tool"
 authors = ["National Library of Finland <finto-posti@helsinki.fi>"]
 maintainers = [
     "Osma Suominen <osma.suominen@helsinki.fi>",
     "Juho Inkinen <juho.inkinen@helsinki.fi>",
     "Mona Lehtinen <mona.lehtinen@helsinki.fi>",
 ]
@@ -27,53 +27,53 @@
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 
 connexion = {version = "2.14.*", extras = ["swagger-ui"]}
-swagger_ui_bundle = "*"
 flask = ">=1.0.4,<3"
-flask-cors = "*"
+flask-cors = "3.0.*"
 click = "8.1.*"
-click-log = "*"
+click-log = "0.4.*"
 joblib = "1.2.*"
-nltk = "*"
+nltk = "3.8.*"
 gensim = "4.3.*"
-scikit-learn = "1.2.0"
+scikit-learn = "1.2.2"
 scipy = "1.10.*"
 rdflib = ">=4.2,<7.0"
-gunicorn = "*"
+gunicorn = "20.1.*"
 numpy = "1.24.*"
 optuna = "2.10.*"
 stwfsapy = "0.3.*"
-python-dateutil = "*"
+python-dateutil = "2.8.*"
 tomli = "2.0.*"
 simplemma = "0.9.*"
+jsonschema = "4.17.*"
 
 fasttext-wheel = {version = "0.9.2", optional = true}
-voikko = {version = "*", optional = true}
+voikko = {version = "0.5.*", optional = true}
 tensorflow-cpu = {version = "2.11.*", optional = true}
-lmdb = {version = "1.4.0", optional = true}
+lmdb = {version = "1.4.1", optional = true}
 omikuji = {version = "0.5.*", optional = true}
 yake = {version = "0.4.5", optional = true}
-spacy = {version = "3.4.*", optional = true}
+spacy = {version = "3.5.*", optional = true}
 
 [tool.poetry.dev-dependencies]
 py = "*"
 pytest = "*"
 requests = "*"
-codecov = "*"
 pytest-cov = "*"
 pytest-watch = "*"
 pytest-flask = "*"
 flake8 = "*"
 bumpversion = "*"
-black = "*"
+black = "23.*"
 isort = "*"
+schemathesis = "3.19.*"
 
 [tool.poetry.extras]
 fasttext = ["fasttext-wheel"]
 voikko = ["voikko"]
 nn = ["tensorflow-cpu", "lmdb"]
 omikuji = ["omikuji"]
 yake = ["yake"]
@@ -86,7 +86,10 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 line_length = "88"
 skip_gitignore = true
+
+[tool.pytest.ini_options]
+addopts = "-m 'not slow'"
```

### Comparing `annif-0.60.0/setup.py` & `annif-0.61.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,248 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: annif
+Version: 0.61.0
+Summary: Automated subject indexing and classification tool
+Home-page: https://annif.org
+License: Apache-2.0
+Keywords: machine-learning,text-classification,rest-api,code4lib,subject-indexing
+Author: National Library of Finland
+Author-email: finto-posti@helsinki.fi
+Maintainer: Osma Suominen
+Maintainer-email: osma.suominen@helsinki.fi
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: fasttext
+Provides-Extra: nn
+Provides-Extra: omikuji
+Provides-Extra: spacy
+Provides-Extra: voikko
+Provides-Extra: yake
+Requires-Dist: click (>=8.1.0,<8.2.0)
+Requires-Dist: click-log (>=0.4.0,<0.5.0)
+Requires-Dist: connexion[swagger-ui] (>=2.14.0,<2.15.0)
+Requires-Dist: fasttext-wheel (==0.9.2) ; extra == "fasttext"
+Requires-Dist: flask (>=1.0.4,<3)
+Requires-Dist: flask-cors (>=3.0.0,<3.1.0)
+Requires-Dist: gensim (>=4.3.0,<4.4.0)
+Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
+Requires-Dist: joblib (>=1.2.0,<1.3.0)
+Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
+Requires-Dist: lmdb (==1.4.1) ; extra == "nn"
+Requires-Dist: nltk (>=3.8.0,<3.9.0)
+Requires-Dist: numpy (>=1.24.0,<1.25.0)
+Requires-Dist: omikuji (>=0.5.0,<0.6.0) ; extra == "omikuji"
+Requires-Dist: optuna (>=2.10.0,<2.11.0)
+Requires-Dist: python-dateutil (>=2.8.0,<2.9.0)
+Requires-Dist: rdflib (>=4.2,<7.0)
+Requires-Dist: scikit-learn (==1.2.2)
+Requires-Dist: scipy (>=1.10.0,<1.11.0)
+Requires-Dist: simplemma (>=0.9.0,<0.10.0)
+Requires-Dist: spacy (>=3.5.0,<3.6.0) ; extra == "spacy"
+Requires-Dist: stwfsapy (>=0.3.0,<0.4.0)
+Requires-Dist: tensorflow-cpu (>=2.11.0,<2.12.0) ; extra == "nn"
+Requires-Dist: tomli (>=2.0.0,<2.1.0)
+Requires-Dist: voikko (>=0.5.0,<0.6.0) ; extra == "voikko"
+Requires-Dist: yake (==0.4.5) ; extra == "yake"
+Project-URL: Documentation, https://github.com/NatLibFi/Annif/wiki
+Project-URL: Repository, https://github.com/NatLibFi/Annif
+Description-Content-Type: text/markdown
+
+<img src="https://annif.org/static/img/annif-RGB.svg" width="150">
+
+[![DOI](https://zenodo.org/badge/100936800.svg)](https://zenodo.org/badge/latestdoi/100936800)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![CI/CD](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml)
+[![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/main/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)
+[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)
+[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=main)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=main)
+[![codebeat badge](https://codebeat.co/badges/7a8ef539-0094-48b8-84c2-c413b4a50d57)](https://codebeat.co/projects/github-com-natlibfi-annif-main)
+[![CodeQL](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NatLibFi_Annif&metric=alert_status)](https://sonarcloud.io/dashboard?id=NatLibFi_Annif)
+[![docs](https://readthedocs.org/projects/annif/badge/?version=latest)](https://annif.readthedocs.io/en/latest/index.html)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Annif is an automated subject indexing toolkit. It was originally created as
+a statistical automated indexing tool that used metadata from the
+[Finna.fi](https://finna.fi) discovery interface as a training corpus.
+
+This repo contains a rewritten production version of Annif based on the
+[prototype](https://github.com/osma/annif). It is a work in progress, but
+already functional for many common tasks.
+
+[Finto AI](https://ai.finto.fi/) is a service based on Annif; see the [source code for Finto AI](https://github.com/NatLibFi/FintoAI).
+
+# Basic install
+
+Annif is developed and tested on Linux. If you want to run Annif on Windows or Mac OS, the recommended way is to use Docker (see below) or a Linux virtual machine.
+
+You will need Python 3.8+ to install Annif.
+
+The recommended way is to install Annif from
+[PyPI](https://pypi.org/project/annif/) into a virtual environment.
+
+    python3 -m venv annif-venv
+    source annif-venv/bin/activate
+    pip install annif
+
+You will also need NLTK data files:
+
+    python -m nltk.downloader punkt
+
+Start up the application:
+
+    annif
+
+See [Getting Started](https://github.com/NatLibFi/Annif/wiki/Getting-started)
+in the wiki for more details.
+
+# Docker install
+
+You can use Annif as a pre-built Docker container. Please see the
+[wiki documentation](https://github.com/NatLibFi/Annif/wiki/Usage-with-Docker)
+for details.
+
+# Development install
+
+A development version of Annif can be installed by cloning the [GitHub
+repository](https://github.com/NatLibFi/Annif).
+[Poetry](https://python-poetry.org/) is used for managing dependencies and virtual environment for the development version.
+
+See [CONTRIBUTING.md](CONTRIBUTING.md) for information on [unit tests](CONTRIBUTING.md#unit-tests), [code style](CONTRIBUTING.md#code-style), [development flow](CONTRIBUTING.md#development-flow) etc. details that are useful when participating in Annif development.
+
+## Installation and setup
+
+Clone the repository.
+
+Switch into the repository directory.
+
+Install [pipx](https://pypa.github.io/pipx/) and Poetry if you don't have them. First pipx:
+
+    python3 -m pip install --user pipx
+    python3 -m pipx ensurepath
+
+Open a new shell, and then install Poetry:
+
+    pipx install poetry
+
+Poetry can be installed also without pipx: check the [Poetry documentation](https://python-poetry.org/docs/master/#installation).
+
+Create a virtual environment and install dependencies:
+
+    poetry install
+
+By default development dependencies are included. Use option `-E` to install dependencies for selected optional features (`-E "extra1 extra2"` for multiple extras), or install all of them with `--all-extras`. By default the virtual environment directory is not under the project directory, but there is a [setting for selecting this](https://python-poetry.org/docs/configuration/#virtualenvsin-project).
+
+Enter the virtual environment:
+
+    poetry shell
+
+You will also need NLTK data files:
+
+    python -m nltk.downloader punkt
+
+Start up the application:
+
+    annif
+
+# Getting help
+
+Many resources are available:
+
+ * [Usage documentation in the wiki](https://github.com/NatLibFi/Annif/wiki)
+ * [Annif tutorial](https://github.com/NatLibFi/Annif-tutorial) for learning to use Annif
+ * [annif-users](https://groups.google.com/forum/#!forum/annif-users) discussion forum
+ * [Internal API documentation](https://annif.readthedocs.io) on ReadTheDocs
+ * [annif.org](https://annif.org) project web site
+
+# Publications / How to cite
+
+Two articles about Annif have been published in peer-reviewed Open Access
+journals. The software itself is also archived on Zenodo and
+has a [citable DOI](https://doi.org/10.5281/zenodo.5654173).
+
+## Citing the software itself
+
+See "Cite this repository" in the details of the repository.
+
+## Annif articles
+<ul>
+<li>
+Suominen, O.; Inkinen, J.; Lehtinen, M., 2022.
+Annif and Finto AI: Developing and Implementing Automated Subject Indexing.
+JLIS.It, 13(1), pp. 265–282. URL:
+https://www.jlis.it/index.php/jlis/article/view/437
+<details>
+<summary>See BibTex</summary>
+
+    @article{suominen2022annif,
+      title={Annif and Finto AI: Developing and Implementing Automated Subject Indexing},
+      author={Suominen, Osma and Inkinen, Juho and Lehtinen, Mona},
+      journal={JLIS.it},
+      volume={13},
+      number={1},
+      pages={265--282},
+      year={2022},
+      doi = {10.4403/jlis.it-12740},
+      url={https://www.jlis.it/index.php/jlis/article/view/437},
+    }
+</details>
+</li>
+<li>
+Suominen, O.; Koskenniemi, I, 2022.
+Annif Analyzer Shootout: Comparing text lemmatization methods for automated subject indexing.
+Code4Lib Journal, (54). URL:
+https://journal.code4lib.org/articles/16719
+<details>
+<summary>See BibTex</summary>
+
+    @article{suominen2022analyzer,
+      title={Annif Analyzer Shootout: Comparing text lemmatization methods for automated subject indexing},
+      author={Suominen, Osma and Koskenniemi, Ilkka},
+      journal={Code4Lib J.},
+      number={54},
+      year={2022},
+      url={https://journal.code4lib.org/articles/16719},
+    }
+</details>
+</li>
+<li>
+Suominen, O., 2019. Annif: DIY automated subject indexing using multiple
+algorithms. LIBER Quarterly, 29(1), pp.1–25. DOI:
+https://doi.org/10.18352/lq.10285
+<details>
+<summary>See BibTex</summary>
+
+    @article{suominen2019annif,
+      title={Annif: DIY automated subject indexing using multiple algorithms},
+      author={Suominen, Osma},
+      journal={{LIBER} Quarterly},
+      volume={29},
+      number={1},
+      pages={1--25},
+      year={2019},
+      doi = {10.18352/lq.10285},
+      url = {https://doi.org/10.18352/lq.10285}
+    }
+</details>
+</li>
+</ul>
+
+# License
+
+The code in this repository is licensed under Apache License 2.0, except for the
+dependencies included under `annif/static/css` and `annif/static/js`,
+which have their own licenses, see the file headers for details.
+Please note that the [YAKE](https://github.com/LIAAD/yake) library is licended
+under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.txt), while Annif is
+licensed under the Apache License 2.0. The licenses are compatible, but
+depending on legal interpretation, the terms of the GPLv3 (for example the
+requirement to publish corresponding source code when publishing an executable
+application) may be considered to apply to the whole of Annif+Yake if you
+decide to install the optional Yake dependency.
 
-packages = \
-['annif',
- 'annif.analyzer',
- 'annif.backend',
- 'annif.corpus',
- 'annif.lexical',
- 'annif.transform']
-
-package_data = \
-{'': ['*'],
- 'annif': ['openapi/*',
-           'static/*',
-           'static/css/*',
-           'static/fonts/*',
-           'static/img/*',
-           'static/js/*',
-           'templates/*']}
-
-install_requires = \
-['click-log',
- 'click>=8.1.0,<8.2.0',
- 'connexion[swagger-ui]>=2.14.0,<2.15.0',
- 'flask-cors',
- 'flask>=1.0.4,<3',
- 'gensim>=4.3.0,<4.4.0',
- 'gunicorn',
- 'joblib>=1.2.0,<1.3.0',
- 'nltk',
- 'numpy>=1.24.0,<1.25.0',
- 'optuna>=2.10.0,<2.11.0',
- 'python-dateutil',
- 'rdflib>=4.2,<7.0',
- 'scikit-learn==1.2.0',
- 'scipy>=1.10.0,<1.11.0',
- 'simplemma>=0.9.0,<0.10.0',
- 'stwfsapy>=0.3.0,<0.4.0',
- 'swagger_ui_bundle',
- 'tomli>=2.0.0,<2.1.0']
-
-extras_require = \
-{'fasttext': ['fasttext-wheel==0.9.2'],
- 'nn': ['tensorflow-cpu>=2.11.0,<2.12.0', 'lmdb==1.4.0'],
- 'omikuji': ['omikuji>=0.5.0,<0.6.0'],
- 'spacy': ['spacy>=3.4.0,<3.5.0'],
- 'voikko': ['voikko'],
- 'yake': ['yake==0.4.5']}
-
-entry_points = \
-{'console_scripts': ['annif = annif.cli:cli']}
-
-setup_kwargs = {
-    'name': 'annif',
-    'version': '0.60.0',
-    'description': 'Automated subject indexing and classification tool',
-    'long_description': '<img src="https://annif.org/static/img/annif-RGB.svg" width="150">\n\n[![DOI](https://zenodo.org/badge/100936800.svg)](https://zenodo.org/badge/latestdoi/100936800)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![CI/CD](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/cicd.yml)\n[![codecov](https://codecov.io/gh/NatLibFi/Annif/branch/master/graph/badge.svg)](https://codecov.io/gh/NatLibFi/Annif)\n[![Code Climate](https://codeclimate.com/github/NatLibFi/Annif/badges/gpa.svg)](https://codeclimate.com/github/NatLibFi/Annif)\n[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/NatLibFi/Annif/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/NatLibFi/Annif/?branch=master)\n[![codebeat badge](https://codebeat.co/badges/e496f151-93db-4f0e-9e30-bc3339e58ca4)](https://codebeat.co/projects/github-com-natlibfi-annif-master)\n[![CodeQL](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml/badge.svg)](https://github.com/NatLibFi/Annif/actions/workflows/codeql.yml)\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NatLibFi_Annif&metric=alert_status)](https://sonarcloud.io/dashboard?id=NatLibFi_Annif)\n[![docs](https://readthedocs.org/projects/annif/badge/?version=latest)](https://annif.readthedocs.io/en/latest/index.html)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nAnnif is an automated subject indexing toolkit. It was originally created as\na statistical automated indexing tool that used metadata from the\n[Finna.fi](https://finna.fi) discovery interface as a training corpus.\n\nThis repo contains a rewritten production version of Annif based on the\n[prototype](https://github.com/osma/annif). It is a work in progress, but\nalready functional for many common tasks.\n\n[Finto AI](https://ai.finto.fi/) is a service based on Annif; see the [source code for Finto AI](https://github.com/NatLibFi/FintoAI).\n\n# Basic install\n\nAnnif is developed and tested on Linux. If you want to run Annif on Windows or Mac OS, the recommended way is to use Docker (see below) or a Linux virtual machine.\n\nYou will need Python 3.8+ to install Annif.\n\nThe recommended way is to install Annif from\n[PyPI](https://pypi.org/project/annif/) into a virtual environment.\n\n    python3 -m venv annif-venv\n    source annif-venv/bin/activate\n    pip install annif\n\nYou will also need NLTK data files:\n\n    python -m nltk.downloader punkt\n\nStart up the application:\n\n    annif\n\nSee [Getting Started](https://github.com/NatLibFi/Annif/wiki/Getting-started)\nin the wiki for more details.\n\n# Docker install\n\nYou can use Annif as a pre-built Docker container. Please see the \n[wiki documentation](https://github.com/NatLibFi/Annif/wiki/Usage-with-Docker)\nfor details.\n\n# Development install\n\nA development version of Annif can be installed by cloning the [GitHub\nrepository](https://github.com/NatLibFi/Annif).\n[Poetry](https://python-poetry.org/) is used for managing dependencies and virtual environment for the development version.\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information on [unit tests](CONTRIBUTING.md#unit-tests), [code style](CONTRIBUTING.md#code-style), [development flow](CONTRIBUTING.md#development-flow) etc. details that are useful when participating in Annif development.\n\n## Installation and setup\n\nClone the repository.\n\nSwitch into the repository directory.\n\nInstall [pipx](https://pypa.github.io/pipx/) and Poetry if you don\'t have them. First pipx:\n\n    python3 -m pip install --user pipx\n    python3 -m pipx ensurepath\n\nOpen a new shell, and then install Poetry: \n\n    pipx install poetry\n\nPoetry can be installed also without pipx: check the [Poetry documentation](https://python-poetry.org/docs/master/#installation). \n\nCreate a virtual environment and install dependencies:\n\n    poetry install\n\nBy default development dependencies are included. Use option `-E` to install dependencies for selected optional features (`-E "extra1 extra2"` for multiple extras), or install all of them with `--all-extras`. By default the virtual environment directory is not under the project directory, but there is a [setting for selecting this](https://python-poetry.org/docs/configuration/#virtualenvsin-project).\n\nEnter the virtual environment:\n\n    poetry shell\n\nYou will also need NLTK data files:\n\n    python -m nltk.downloader punkt\n\nStart up the application:\n\n    annif\n\n# Getting help\n\nMany resources are available:\n\n * [Usage documentation in the wiki](https://github.com/NatLibFi/Annif/wiki)\n * [Annif tutorial](https://github.com/NatLibFi/Annif-tutorial) for learning to use Annif\n * [annif-users](https://groups.google.com/forum/#!forum/annif-users) discussion forum\n * [Internal API documentation](https://annif.readthedocs.io) on ReadTheDocs\n * [annif.org](https://annif.org) project web site\n\n# Publications / How to cite\n\nTwo articles about Annif have been published in peer-reviewed Open Access\njournals. The software itself is also archived on Zenodo and\nhas a [citable DOI](https://doi.org/10.5281/zenodo.5654173).\n\n## Citing the software itself\n\nSee "Cite this repository" in the details of the repository.\n\n## Annif articles\n<ul>\n<li> \nSuominen, O.; Inkinen, J.; Lehtinen, M., 2022. \nAnnif and Finto AI: Developing and Implementing Automated Subject Indexing.\nJLIS.It, 13(1), pp. 265–282. URL:\nhttps://www.jlis.it/index.php/jlis/article/view/437\n<details>\n<summary>See BibTex</summary>\n    \n    @article{suominen2022annif,\n      title={Annif and Finto AI: Developing and Implementing Automated Subject Indexing},\n      author={Suominen, Osma and Inkinen, Juho and Lehtinen, Mona},\n      journal={JLIS.it},\n      volume={13},\n      number={1},\n      pages={265--282},\n      year={2022},\n      doi = {10.4403/jlis.it-12740},\n      url={https://www.jlis.it/index.php/jlis/article/view/437},\n    }\n</details>\n</li> \n<li> \nSuominen, O.; Koskenniemi, I, 2022.\nAnnif Analyzer Shootout: Comparing text lemmatization methods for automated subject indexing.\nCode4Lib Journal, (54). URL:\nhttps://journal.code4lib.org/articles/16719\n<details>\n<summary>See BibTex</summary>\n\n    @article{suominen2022analyzer,\n      title={Annif Analyzer Shootout: Comparing text lemmatization methods for automated subject indexing},\n      author={Suominen, Osma and Koskenniemi, Ilkka},\n      journal={Code4Lib J.},\n      number={54},\n      year={2022},\n      url={https://journal.code4lib.org/articles/16719},\n    }\n</details>\n</li> \n<li> \nSuominen, O., 2019. Annif: DIY automated subject indexing using multiple\nalgorithms. LIBER Quarterly, 29(1), pp.1–25. DOI:\nhttps://doi.org/10.18352/lq.10285\n<details>\n<summary>See BibTex</summary>\n\n    @article{suominen2019annif,\n      title={Annif: DIY automated subject indexing using multiple algorithms},\n      author={Suominen, Osma},\n      journal={{LIBER} Quarterly},\n      volume={29},\n      number={1},\n      pages={1--25},\n      year={2019},\n      doi = {10.18352/lq.10285},\n      url = {https://doi.org/10.18352/lq.10285}\n    }\n</details>\n</li>\n</ul>\n\n# License\n\nThe code in this repository is licensed under Apache License 2.0, except for the\ndependencies included under `annif/static/css` and `annif/static/js`,\nwhich have their own licenses, see the file headers for details.\nPlease note that the [YAKE](https://github.com/LIAAD/yake) library is licended\nunder [GPLv3](https://www.gnu.org/licenses/gpl-3.0.txt), while Annif is\nlicensed under the Apache License 2.0. The licenses are compatible, but\ndepending on legal interpretation, the terms of the GPLv3 (for example the\nrequirement to publish corresponding source code when publishing an executable\napplication) may be considered to apply to the whole of Annif+Yake if you\ndecide to install the optional Yake dependency.\n',
-    'author': 'National Library of Finland',
-    'author_email': 'finto-posti@helsinki.fi',
-    'maintainer': 'Osma Suominen',
-    'maintainer_email': 'osma.suominen@helsinki.fi',
-    'url': 'https://annif.org',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

