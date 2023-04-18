# Comparing `tmp/scattertext-0.1.8.tar.gz` & `tmp/scattertext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scattertext-0.1.8.tar", last modified: Thu Nov  3 07:02:07 2022, max compression
+gzip compressed data, was "scattertext-0.1.9.tar", last modified: Fri Nov 11 01:06:39 2022, max compression
```

## Comparing `scattertext-0.1.8.tar` & `scattertext-0.1.9.tar`

### file list

```diff
@@ -1,340 +1,340 @@
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      293 2022-11-03 07:02:07.000000 scattertext-0.1.8/PKG-INFO
--rw-r--r--   0 jasonkessler   (501) staff       (20)    11346 2018-09-21 06:21:05.000000 scattertext-0.1.8/LICENSE
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      293 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/PKG-INFO
--rw-r--r--   0 jasonkessler   (501) staff       (20)        1 2018-09-21 06:28:35.000000 scattertext-0.1.8/scattertext.egg-info/not-zip-safe
--rw-r--r--   0 jasonkessler   (501) staff       (20)    12519 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/SOURCES.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)       54 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/entry_points.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)       77 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/requires.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)       12 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/top_level.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)        1 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext.egg-info/dependency_links.txt
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/
--rw-r--r--   0 jasonkessler   (501) staff       (20)    23837 2022-10-11 00:08:48.000000 scattertext-0.1.8/scattertext/TermDocMatrixWithoutCategories.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/representations/
--rw-r--r--   0 jasonkessler   (501) staff       (20)       19 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/representations/GensimPhraseAugmenter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6207 2021-06-27 03:28:56.000000 scattertext-0.1.8/scattertext/representations/Word2VecFromParsedCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      196 2019-10-13 00:29:27.000000 scattertext-0.1.8/scattertext/representations/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4120 2021-11-15 03:14:28.000000 scattertext-0.1.8/scattertext/representations/EmbeddingsResolver.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     9122 2021-05-08 17:49:56.000000 scattertext-0.1.8/scattertext/representations/CategoryEmbeddings.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      567 2018-10-15 05:40:59.000000 scattertext-0.1.8/scattertext/representations/CorpusSentenceIterator.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1503 2019-03-25 00:47:57.000000 scattertext-0.1.8/scattertext/representations/Doc2VecBuilder.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2420 2021-07-29 07:04:43.000000 scattertext-0.1.8/scattertext/representations/LatentSemanticScaling.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/categorygrouping/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2022-05-30 01:17:33.000000 scattertext-0.1.8/scattertext/categorygrouping/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4608 2022-06-15 02:11:38.000000 scattertext-0.1.8/scattertext/categorygrouping/CharacteristicGrouper.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/tokenizers/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2450 2021-03-14 01:28:31.000000 scattertext-0.1.8/scattertext/tokenizers/roberta.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-25 02:40:00.000000 scattertext-0.1.8/scattertext/tokenizers/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4658 2018-12-05 08:45:20.000000 scattertext-0.1.8/scattertext/SampleCorpora.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4829 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/PriorFactory.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1889 2019-11-06 06:45:38.000000 scattertext-0.1.8/scattertext/SampleLexicons.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      388 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/Formatter.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/topicmodel/
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/topicmodel/interface/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2020-04-06 00:38:07.000000 scattertext-0.1.8/scattertext/topicmodel/interface/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       64 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/topicmodel/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3519 2020-06-21 23:38:55.000000 scattertext-0.1.8/scattertext/topicmodel/SentencesForTopicModeling.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4794 2021-11-15 03:48:32.000000 scattertext-0.1.8/scattertext/CorpusFromTermFrequencies.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3999 2022-03-20 23:20:25.000000 scattertext-0.1.8/scattertext/OffsetCorpusFactory.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1887 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/CorpusFromScikit.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      385 2022-11-02 23:36:56.000000 scattertext-0.1.8/scattertext/FeatureOuput.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/characteristic/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/characteristic/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2339 2021-01-17 19:16:52.000000 scattertext-0.1.8/scattertext/characteristic/DenseRankCharacteristicness.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/test/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2804 2020-06-08 01:19:45.000000 scattertext-0.1.8/scattertext/test/test_cohensD.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1409 2019-03-06 18:28:07.000000 scattertext-0.1.8/scattertext/test/test_associationCompator.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2178 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_CornerScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      565 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_combineDocsIntoDomains.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2528 2020-02-11 05:30:21.000000 scattertext-0.1.8/scattertext/test/test_ParsedCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     8772 2019-04-18 00:14:00.000000 scattertext-0.1.8/scattertext/test/test_scatterChartExplorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4401 2020-02-11 05:34:52.000000 scattertext-0.1.8/scattertext/test/test_termCategoryFrequencies.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3176 2020-02-11 05:30:21.000000 scattertext-0.1.8/scattertext/test/test_corpusFromPandas.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2270 2019-02-21 08:21:33.000000 scattertext-0.1.8/scattertext/test/test_scaledFScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      982 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_vizDataAdapter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    49161 2020-02-11 05:30:21.000000 scattertext-0.1.8/scattertext/test/test_termDocMatrixFromPandas.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1910 2021-01-16 07:51:31.000000 scattertext-0.1.8/scattertext/test/test_Dispersion.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      713 2020-02-11 05:35:03.000000 scattertext-0.1.8/scattertext/test/test_relativeEntropy.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1231 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_domainCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    32298 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_diachronicTermMiner.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      587 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_indexStoreFromDict.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      553 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_phraseSelector.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6997 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_docsAndLabelsFromCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3142 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_indexStore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      447 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_HTMLSemioticSquareViz.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6011 2018-10-15 06:26:19.000000 scattertext-0.1.8/scattertext/test/test_featsFromSpacyDocAndEmpath.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2121 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_logOddsUninformativePriorScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3328 2019-04-19 00:53:26.000000 scattertext-0.1.8/scattertext/test/test_semioticSquareFromAxes.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1723 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_compactTerms.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1595 2018-12-11 10:17:21.000000 scattertext-0.1.8/scattertext/test/test_CategoryColorAssigner.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      845 2019-11-24 21:45:03.000000 scattertext-0.1.8/scattertext/test/test_betaPosterior.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      443 2020-03-23 04:41:28.000000 scattertext-0.1.8/scattertext/test/test_useFullDocAsFeature.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      454 2020-03-23 07:17:55.000000 scattertext-0.1.8/scattertext/test/test_useFullDocAsMetadata.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6127 2021-01-18 08:06:24.000000 scattertext-0.1.8/scattertext/test/test_CorpusFromParsedDocuments.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      847 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_autoTermSelector.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      756 2019-01-26 11:09:36.000000 scattertext-0.1.8/scattertext/test/test_Scalers.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      366 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_oneClassScatterChart.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     9316 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_corpusFromFeatureDict.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      655 2021-01-15 04:47:47.000000 scattertext-0.1.8/scattertext/test/test_CorpusWithoutCategoriesFromParsedDocuments.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4311 2020-02-11 05:33:44.000000 scattertext-0.1.8/scattertext/test/test_semioticSquare.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1064 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_logOddsRatioUninformativeDirichletPrior.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      784 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_termDocMatrixFromFrequencies.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      997 2020-02-11 05:34:02.000000 scattertext-0.1.8/scattertext/test/test_ZScores.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4714 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_FeatsFromSpacyDoc.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      438 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_unigramsFromSpacyDoc.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      492 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_denseRankCharacteristicness.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2640 2020-02-11 05:30:21.000000 scattertext-0.1.8/scattertext/test/test_termRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1892 2021-11-15 03:39:09.000000 scattertext-0.1.8/scattertext/test/test_word2VecFromParsedCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      766 2018-12-27 08:24:21.000000 scattertext-0.1.8/scattertext/test/test_classPercentageCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2367 2021-01-04 01:02:32.000000 scattertext-0.1.8/scattertext/test/test_PMIFiltering.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2636 2021-11-15 03:16:25.000000 scattertext-0.1.8/scattertext/test/test_embeddingsResolver.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1025 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_extract_emoji.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1981 2019-10-08 19:45:28.000000 scattertext-0.1.8/scattertext/test/test_WhitespaceNLP.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      867 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_featureLister.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    29944 2022-09-25 17:49:20.000000 scattertext-0.1.8/scattertext/test/test_HTMLVisualizationAssembly.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1884 2020-02-11 05:33:21.000000 scattertext-0.1.8/scattertext/test/test_featsFromScoredLexicon.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4207 2021-01-04 01:10:05.000000 scattertext-0.1.8/scattertext/test/test_PriorFactory.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      394 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_indexStoreFromList.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      692 2020-02-11 05:35:03.000000 scattertext-0.1.8/scattertext/test/test_BM25Difference.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    14504 2020-02-11 05:04:46.000000 scattertext-0.1.8/scattertext/test/test_scatterChart.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1717 2019-11-03 21:03:34.000000 scattertext-0.1.8/scattertext/test/test_CSRMatrixTools.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      907 2020-10-11 22:48:42.000000 scattertext-0.1.8/scattertext/test/test_featsFromTopicModel.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      703 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_large_int_format.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1515 2018-12-21 04:59:51.000000 scattertext-0.1.8/scattertext/test/test_corpusFromPandasWithoutCategories.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1006 2020-02-14 16:58:51.000000 scattertext-0.1.8/scattertext/test/test_credTFIDF.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1180 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_corpusFromScikit.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    26533 2022-10-06 06:08:24.000000 scattertext-0.1.8/scattertext/test/test_TermDocMat.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3819 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_fourSquareAxes.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     5535 2019-08-13 02:04:11.000000 scattertext-0.1.8/scattertext/test/test_termDocMatrixFactory.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1126 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_termDocMatrixFromScikit.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3648 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_asiannlp.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      420 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_percentile_lexicographic.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1077 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/test/test_gensimPhraseAdder.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/termranking/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1355 2020-02-23 00:28:44.000000 scattertext-0.1.8/scattertext/termranking/TermRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      286 2018-11-22 00:21:48.000000 scattertext-0.1.8/scattertext/termranking/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1691 2019-11-24 18:08:36.000000 scattertext-0.1.8/scattertext/termranking/DocLengthNormalizedFrequencyRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      529 2020-03-19 04:27:10.000000 scattertext-0.1.8/scattertext/termranking/OncePerDocFrequencyRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      468 2019-11-24 18:07:17.000000 scattertext-0.1.8/scattertext/termranking/AbsoluteFrequencyRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      340 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termranking/DocLengthDividedFrequencyRanker.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2117 2019-11-03 21:02:15.000000 scattertext-0.1.8/scattertext/CSRMatrixTools.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3870 2022-01-21 07:14:28.000000 scattertext-0.1.8/scattertext/DocsAndLabelsFromCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    29913 2022-10-14 01:51:22.000000 scattertext-0.1.8/scattertext/ScatterChart.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    12293 2022-03-20 22:37:08.000000 scattertext-0.1.8/scattertext/TermDocMatrixFromPandas.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1973 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/TermDocMatrixFromFrequencies.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6306 2021-01-18 09:44:28.000000 scattertext-0.1.8/scattertext/Scalers.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/smoothing/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      584 2021-05-31 00:20:10.000000 scattertext-0.1.8/scattertext/smoothing/lowess.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       57 2021-05-14 04:26:53.000000 scattertext-0.1.8/scattertext/smoothing/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      725 2021-02-01 07:17:36.000000 scattertext-0.1.8/scattertext/smoothing/sigmoidal.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      480 2021-04-28 04:38:57.000000 scattertext-0.1.8/scattertext/smoothing/power_law.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      684 2021-01-18 23:37:44.000000 scattertext-0.1.8/scattertext/smoothing/mean_isotonic.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/diachronic/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4911 2020-04-12 22:20:46.000000 scattertext-0.1.8/scattertext/diachronic/GanttChart.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6659 2021-05-24 00:15:15.000000 scattertext-0.1.8/scattertext/diachronic/DiachronicTermMiner.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2020-04-13 00:58:53.000000 scattertext-0.1.8/scattertext/diachronic/DiachronicPairPlot.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       58 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/diachronic/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      805 2020-04-11 22:25:24.000000 scattertext-0.1.8/scattertext/diachronic/BubbleDiachronicVisualization.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      108 2019-01-30 06:48:40.000000 scattertext-0.1.8/scattertext/diachronic/DiachronicVisualizer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1203 2021-06-06 00:24:52.000000 scattertext-0.1.8/scattertext/diachronic/TimeStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    37629 2022-10-06 06:16:30.000000 scattertext-0.1.8/scattertext/TermDocMatrix.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/categoryprojector/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3371 2019-08-17 15:49:39.000000 scattertext-0.1.8/scattertext/categoryprojector/CategoryProjectorEvaluator.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    13260 2022-10-21 06:35:38.000000 scattertext-0.1.8/scattertext/categoryprojector/pairplot.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2019-01-28 01:45:23.000000 scattertext-0.1.8/scattertext/categoryprojector/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7074 2022-06-17 04:57:42.000000 scattertext-0.1.8/scattertext/categoryprojector/CategoryProjection.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     8841 2022-10-21 06:35:29.000000 scattertext-0.1.8/scattertext/categoryprojector/CategoryProjector.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     5553 2022-07-20 22:14:11.000000 scattertext-0.1.8/scattertext/categoryprojector/OptimalProjection.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/features/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3300 2022-06-17 02:54:35.000000 scattertext-0.1.8/scattertext/features/FeatsFromSpacyDoc.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      400 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/features/UnigramsFromSpacyDoc.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2045 2021-03-08 05:39:42.000000 scattertext-0.1.8/scattertext/features/PyTextRankPhrases.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      365 2020-03-23 07:17:39.000000 scattertext-0.1.8/scattertext/features/UseFullDocAsFeature.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      432 2021-08-24 01:39:13.000000 scattertext-0.1.8/scattertext/features/PyatePhrases.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    20724 2018-12-03 17:17:11.000000 scattertext-0.1.8/scattertext/features/FeatsFromGeneralInquirer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      936 2021-04-21 07:04:27.000000 scattertext-0.1.8/scattertext/features/RegexFeatAndOffsetGetter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/features/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1860 2019-11-03 21:38:17.000000 scattertext-0.1.8/scattertext/features/FeatsFromScoredLexicon.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3167 2020-06-07 23:32:50.000000 scattertext-0.1.8/scattertext/features/FeatsFromMoralFoundationsDictionary.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      451 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/features/FeatsFromSpacyDocOnlyEmoji.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2110 2021-02-03 08:23:49.000000 scattertext-0.1.8/scattertext/features/FeatsFromSpacyDocAndEmpath.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1370 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/features/PhraseMachinePhrases.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/features/featoffsets/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2858 2022-11-03 06:49:53.000000 scattertext-0.1.8/scattertext/features/featoffsets/flexible_ngram_features.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      222 2022-03-20 23:29:02.000000 scattertext-0.1.8/scattertext/features/featoffsets/feat_and_offset_getter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-24 20:37:18.000000 scattertext-0.1.8/scattertext/features/featoffsets/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      552 2021-12-28 08:50:38.000000 scattertext-0.1.8/scattertext/features/featoffsets/token_and_feat_offset_getter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4027 2021-03-06 03:35:02.000000 scattertext-0.1.8/scattertext/features/FeatsFromTopicModel.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      430 2020-04-05 01:21:48.000000 scattertext-0.1.8/scattertext/features/UseFullDocAsMetadata.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      929 2020-07-17 03:42:17.000000 scattertext-0.1.8/scattertext/features/SpacyEntities.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      404 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/features/FeatsFromSpacyDocOnlyNounChunks.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      548 2019-12-04 08:32:02.000000 scattertext-0.1.8/scattertext/features/FeatsFromSentencePiece.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      348 2021-02-03 08:22:17.000000 scattertext-0.1.8/scattertext/features/FeatsFromOnlyEmpath.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    10371 2021-07-26 07:11:25.000000 scattertext-0.1.8/scattertext/features/CognitiveDistortionsOffsetGetter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    14114 2022-03-20 22:35:54.000000 scattertext-0.1.8/scattertext/TermDocMatrixFactory.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    99646 2022-11-03 06:26:07.000000 scattertext-0.1.8/scattertext/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7387 2022-03-23 20:23:35.000000 scattertext-0.1.8/scattertext/TermCategoryFrequencies.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/frequencyreaders/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/frequencyreaders/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2015 2022-03-24 19:19:45.000000 scattertext-0.1.8/scattertext/frequencyreaders/DefaultBackgroundFrequencies.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/semioticsquare/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7662 2019-04-18 21:50:46.000000 scattertext-0.1.8/scattertext/semioticsquare/SemioticSquare.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       42 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/semioticsquare/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2395 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/semioticsquare/FourSquare.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3797 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/semioticsquare/FourSquareAxis.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3099 2020-09-30 02:03:08.000000 scattertext-0.1.8/scattertext/semioticsquare/SemioticSquareFromAxes.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2832 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/DeployedClassifier.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4398 2022-03-21 06:27:13.000000 scattertext-0.1.8/scattertext/OffsetCorpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2044 2018-12-11 10:40:23.000000 scattertext-0.1.8/scattertext/CategoryColorAssigner.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4635 2021-01-25 02:41:00.000000 scattertext-0.1.8/scattertext/WhitespaceNLP.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      673 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/PValGetter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2821 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/TermDocMatrixFromScikit.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/viz/
--rw-r--r--   0 jasonkessler   (501) staff       (20)    21947 2022-09-25 17:50:31.000000 scattertext-0.1.8/scattertext/viz/ScatterplotStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7405 2022-11-03 06:58:35.000000 scattertext-0.1.8/scattertext/viz/PyPlotFromScattertextStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      329 2019-01-28 03:29:06.000000 scattertext-0.1.8/scattertext/viz/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6690 2022-01-01 23:28:02.000000 scattertext-0.1.8/scattertext/viz/BasicHTMLFromScatterplotStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3255 2021-11-15 01:25:21.000000 scattertext-0.1.8/scattertext/viz/HTMLSemioticSquareViz.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6050 2022-01-01 23:29:08.000000 scattertext-0.1.8/scattertext/viz/PairPlotFromScattertextStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1159 2019-01-06 09:31:16.000000 scattertext-0.1.8/scattertext/viz/VizDataAdapter.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1853 2021-02-15 02:32:51.000000 scattertext-0.1.8/scattertext/viz/TermInfo.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/termscoring/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1810 2022-07-16 20:06:40.000000 scattertext-0.1.8/scattertext/termscoring/BM25Difference.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4623 2022-07-07 01:11:22.000000 scattertext-0.1.8/scattertext/termscoring/Productivity.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2210 2022-03-26 09:20:41.000000 scattertext-0.1.8/scattertext/termscoring/CohensD.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1331 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termscoring/CornerScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3888 2019-11-24 21:29:27.000000 scattertext-0.1.8/scattertext/termscoring/BetaPosterior.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3706 2019-11-24 21:30:14.000000 scattertext-0.1.8/scattertext/termscoring/MannWhitneyU.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4622 2022-08-17 01:34:11.000000 scattertext-0.1.8/scattertext/termscoring/ScikitTermScorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     9983 2020-07-19 23:24:23.000000 scattertext-0.1.8/scattertext/termscoring/CredTFIDF.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      230 2019-01-08 05:35:22.000000 scattertext-0.1.8/scattertext/termscoring/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      442 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termscoring/RankDifference.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      641 2021-06-22 01:17:05.000000 scattertext-0.1.8/scattertext/termscoring/DeltaJSDivergence.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1457 2022-01-02 00:08:08.000000 scattertext-0.1.8/scattertext/termscoring/RankDifferenceScorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1735 2018-10-15 06:13:55.000000 scattertext-0.1.8/scattertext/termscoring/RelativeEntropy.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2040 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termscoring/LogOddsUniformativePriorScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     5351 2022-10-14 01:56:19.000000 scattertext-0.1.8/scattertext/termscoring/CorpusBasedTermScorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      854 2018-10-02 04:59:29.000000 scattertext-0.1.8/scattertext/termscoring/ZScores.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      946 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termscoring/OLSUngnarStyle.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3092 2021-06-22 06:15:15.000000 scattertext-0.1.8/scattertext/termscoring/CohensDCalculator.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2319 2022-11-03 05:59:23.000000 scattertext-0.1.8/scattertext/termscoring/BNSScorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1025 2022-01-02 00:02:26.000000 scattertext-0.1.8/scattertext/termscoring/LogOddsRatio.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      596 2019-04-30 04:58:21.000000 scattertext-0.1.8/scattertext/termscoring/test_credTFIDF.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    13605 2020-03-29 02:16:08.000000 scattertext-0.1.8/scattertext/termscoring/ScaledFScore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2360 2022-03-09 23:49:08.000000 scattertext-0.1.8/scattertext/termscoring/CraigsZeta.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6594 2021-03-08 03:23:47.000000 scattertext-0.1.8/scattertext/CLI.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3552 2020-09-30 06:49:19.000000 scattertext-0.1.8/scattertext/Common.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2838 2021-11-15 03:48:32.000000 scattertext-0.1.8/scattertext/AutoTermSelector.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4136 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/CorpusFromFeatureDict.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3137 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/AsianNLP.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2911 2022-01-21 07:08:19.000000 scattertext-0.1.8/scattertext/ScatterChartData.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/dispersion/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-15 03:07:37.000000 scattertext-0.1.8/scattertext/dispersion/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     8896 2021-05-31 01:36:55.000000 scattertext-0.1.8/scattertext/dispersion/Dispersion.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    10458 2022-10-14 06:14:12.000000 scattertext-0.1.8/scattertext/ScatterChartExplorer.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4801 2022-06-16 19:49:19.000000 scattertext-0.1.8/scattertext/ParsedCorpus.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/graphs/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3682 2021-11-15 01:34:55.000000 scattertext-0.1.8/scattertext/graphs/GraphStructure.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      202 2020-04-07 03:09:55.000000 scattertext-0.1.8/scattertext/graphs/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2554 2020-05-18 01:26:51.000000 scattertext-0.1.8/scattertext/graphs/SimpleDiGraph.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2891 2020-05-18 01:24:44.000000 scattertext-0.1.8/scattertext/graphs/ComponentDiGraph.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     5977 2020-05-18 02:25:17.000000 scattertext-0.1.8/scattertext/graphs/ComponentDiGraphHTMLRenderer.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/external/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/external/__init__.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/external/phrasemachine/
--rw-r--r--   0 jasonkessler   (501) staff       (20)    11067 2021-03-08 03:23:59.000000 scattertext-0.1.8/scattertext/external/phrasemachine/phrasemachine.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/external/phrasemachine/__init__.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/emojis/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/emojis/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1977 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/emojis/EmojiExtractor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)    68316 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/emojis/ProcessedEmojiStructure.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/categorytable/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7208 2022-08-11 01:27:36.000000 scattertext-0.1.8/scattertext/categorytable/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      161 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/OneClassScatterChart.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/indexstore/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      392 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/indexstore/IndexStoreFromList.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      137 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/indexstore/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2347 2022-07-07 00:21:34.000000 scattertext-0.1.8/scattertext/indexstore/IndexStore.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      508 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/indexstore/IndexStoreFromDict.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2761 2021-01-02 01:38:25.000000 scattertext-0.1.8/scattertext/CorpusDF.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2886 2021-04-28 10:03:10.000000 scattertext-0.1.8/scattertext/CorpusFromParsedDocuments.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/distancemeasures/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      333 2019-04-18 22:11:50.000000 scattertext-0.1.8/scattertext/distancemeasures/DistanceMeasureBase.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      102 2019-04-18 22:16:17.000000 scattertext-0.1.8/scattertext/distancemeasures/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      304 2019-04-18 22:12:12.000000 scattertext-0.1.8/scattertext/distancemeasures/EuclideanDistance.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/data/
--rw-r--r--   0 jasonkessler   (501) staff       (20)    59085 2020-06-07 23:19:29.000000 scattertext-0.1.8/scattertext/data/mfd2.0.csv
--rw-r--r--   0 jasonkessler   (501) staff       (20)   205970 2019-11-06 04:02:51.000000 scattertext-0.1.8/scattertext/data/whissells_df.csv
--rw-r--r--   0 jasonkessler   (501) staff       (20)  2906024 2020-06-07 23:07:24.000000 scattertext-0.1.8/scattertext/data/inqtabs.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)   767471 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/political_data.csv
--rw-r--r--   0 jasonkessler   (501) staff       (20)   224203 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/rotten_tomatoes_corpus.csv.bz2
--rw-r--r--   0 jasonkessler   (501) staff       (20)    12316 2021-04-26 15:14:49.000000 scattertext-0.1.8/scattertext/data/arglex_Somasundaran07.json
--rw-r--r--   0 jasonkessler   (501) staff       (20)  4956327 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/count_1w.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)   994217 2020-12-31 08:08:26.000000 scattertext-0.1.8/scattertext/data/political_data.json
--rw-r--r--   0 jasonkessler   (501) staff       (20)   433305 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/punkt.english.pickle
--rw-r--r--   0 jasonkessler   (501) staff       (20)  5566017 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/count_2w.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)   681736 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/rotten_tomatoes_corpus_full.csv.bz2
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/data/viz/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6387 2021-08-11 08:14:44.000000 scattertext-0.1.8/scattertext/data/viz/pairplot_without_halo.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6436 2021-06-06 00:15:53.000000 scattertext-0.1.8/scattertext/data/viz/graph_plot.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     9163 2021-11-15 03:05:40.000000 scattertext-0.1.8/scattertext/data/viz/semiotic_new.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)    12770 2019-01-30 06:33:53.000000 scattertext-0.1.8/scattertext/data/viz/timeline.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1035 2020-03-29 06:00:32.000000 scattertext-0.1.8/scattertext/data/viz/autocomplete.css
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/data/viz/scripts/
--rw-r--r--   0 jasonkessler   (501) staff       (20)   105987 2019-01-15 08:16:37.000000 scattertext-0.1.8/scattertext/data/viz/scripts/main_bk.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)   214693 2018-11-18 19:14:19.000000 scattertext-0.1.8/scattertext/data/viz/scripts/d3.min.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)      131 2020-03-29 04:17:17.000000 scattertext-0.1.8/scattertext/data/viz/scripts/autocomplete_call.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6230 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/viz/scripts/range-tree.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)   152434 2022-09-26 06:14:36.000000 scattertext-0.1.8/scattertext/data/viz/scripts/main.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)   334370 2020-04-18 01:24:42.000000 scattertext-0.1.8/scattertext/data/viz/scripts/timelines-chart.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)   195294 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/viz/scripts/rectangle-holder.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)     4739 2020-12-18 09:05:24.000000 scattertext-0.1.8/scattertext/data/viz/scripts/autocomplete_definition.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)    18948 2018-11-18 19:14:41.000000 scattertext-0.1.8/scattertext/data/viz/scripts/d3-scale-chromatic.v1.min.js
--rw-r--r--   0 jasonkessler   (501) staff       (20)     6520 2021-06-14 01:28:19.000000 scattertext-0.1.8/scattertext/data/viz/table_plot.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)      204 2020-03-29 05:03:48.000000 scattertext-0.1.8/scattertext/data/viz/search_form.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     9307 2022-01-01 23:30:24.000000 scattertext-0.1.8/scattertext/data/viz/pairplot.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1779 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/viz/semiotic.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7014 2021-06-13 23:45:31.000000 scattertext-0.1.8/scattertext/data/viz/time_plot.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)     5218 2021-01-17 07:44:44.000000 scattertext-0.1.8/scattertext/data/viz/scattertext.html
--rw-r--r--   0 jasonkessler   (501) staff       (20)   234366 2020-08-20 07:11:06.000000 scattertext-0.1.8/scattertext/data/republican_convention_2016.csv
--rw-r--r--   0 jasonkessler   (501) staff       (20)   214434 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/chinese.csv
--rw-r--r--   0 jasonkessler   (501) staff       (20)   175176 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/hamlet.txt
--rw-r--r--   0 jasonkessler   (501) staff       (20)    99979 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/data/presidential_debates_2016.csv.gz
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/domain/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/domain/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1050 2020-02-23 05:35:23.000000 scattertext-0.1.8/scattertext/domain/CombineDocsIntoDomains.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:06.000000 scattertext-0.1.8/scattertext/continuous/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-03-30 06:09:40.000000 scattertext-0.1.8/scattertext/continuous/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1229 2021-04-01 23:45:01.000000 scattertext-0.1.8/scattertext/continuous/sklearnpipeline.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      354 2021-03-30 06:38:16.000000 scattertext-0.1.8/scattertext/continuous/coefficientbase.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-04-01 23:47:54.000000 scattertext-0.1.8/scattertext/continuous/correlations.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1621 2021-04-01 23:01:22.000000 scattertext-0.1.8/scattertext/continuous/ungar.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2629 2022-06-16 19:49:19.000000 scattertext-0.1.8/scattertext/DataFrameCorpus.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/termsignificance/
--rw-r--r--   0 jasonkessler   (501) staff       (20)      148 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termsignificance/TermSignificance.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3145 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioInformativeDirichletPiror.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       93 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termsignificance/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3121 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioUninformativeDirichletPrior.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2601 2021-12-29 04:51:14.000000 scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioSmoothed.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1348 2018-12-27 07:09:54.000000 scattertext-0.1.8/scattertext/termsignificance/ScaledFScoreSignificance.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/helpers/
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-01 08:40:25.000000 scattertext-0.1.8/scattertext/helpers/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      259 2021-01-01 08:59:53.000000 scattertext-0.1.8/scattertext/helpers/MakeUnique.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1966 2020-04-13 06:20:24.000000 scattertext-0.1.8/scattertext/CorpusFromPandas.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2871 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/TermDocMatrixFilter.py
-drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-03 07:02:07.000000 scattertext-0.1.8/scattertext/termcompaction/
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1106 2020-02-23 06:03:48.000000 scattertext-0.1.8/scattertext/termcompaction/ClassPercentageCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.8/scattertext/termcompaction/__init__.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     7974 2022-10-21 06:18:58.000000 scattertext-0.1.8/scattertext/termcompaction/AssociationCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     2839 2020-02-23 05:31:10.000000 scattertext-0.1.8/scattertext/termcompaction/CompactTerms.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1917 2020-02-23 05:37:20.000000 scattertext-0.1.8/scattertext/termcompaction/DomainCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)      623 2022-08-17 01:27:55.000000 scattertext-0.1.8/scattertext/termcompaction/ScikitCompactor.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1623 2020-02-23 05:42:15.000000 scattertext-0.1.8/scattertext/termcompaction/PhraseSelector.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1276 2021-01-24 20:14:58.000000 scattertext-0.1.8/scattertext/CorpusWithoutCategoriesFromParsedDocuments.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)     3140 2021-01-02 00:55:36.000000 scattertext-0.1.8/scattertext/Corpus.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       16 2020-10-08 00:54:24.000000 scattertext-0.1.8/MANIFEST.in
--rw-r--r--   0 jasonkessler   (501) staff       (20)   140237 2022-11-03 06:58:35.000000 scattertext-0.1.8/README.md
--rw-r--r--   0 jasonkessler   (501) staff       (20)     1128 2022-11-03 06:59:15.000000 scattertext-0.1.8/setup.py
--rw-r--r--   0 jasonkessler   (501) staff       (20)       38 2022-11-03 07:02:07.000000 scattertext-0.1.8/setup.cfg
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.682264 scattertext-0.1.9/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    11346 2018-09-21 06:21:05.000000 scattertext-0.1.9/LICENSE
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       16 2020-10-08 00:54:24.000000 scattertext-0.1.9/MANIFEST.in
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      276 2022-11-11 01:06:39.681994 scattertext-0.1.9/PKG-INFO
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   142991 2022-11-11 00:56:09.000000 scattertext-0.1.9/README.md
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.458334 scattertext-0.1.9/scattertext/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3137 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/AsianNLP.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2838 2021-11-15 03:48:32.000000 scattertext-0.1.9/scattertext/AutoTermSelector.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6594 2021-03-08 03:23:47.000000 scattertext-0.1.9/scattertext/CLI.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2117 2019-11-03 21:02:15.000000 scattertext-0.1.9/scattertext/CSRMatrixTools.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2044 2018-12-11 10:40:23.000000 scattertext-0.1.9/scattertext/CategoryColorAssigner.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3552 2020-09-30 06:49:19.000000 scattertext-0.1.9/scattertext/Common.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3140 2021-01-02 00:55:36.000000 scattertext-0.1.9/scattertext/Corpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2761 2021-01-02 01:38:25.000000 scattertext-0.1.9/scattertext/CorpusDF.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4136 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/CorpusFromFeatureDict.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1966 2020-04-13 06:20:24.000000 scattertext-0.1.9/scattertext/CorpusFromPandas.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2886 2021-04-28 10:03:10.000000 scattertext-0.1.9/scattertext/CorpusFromParsedDocuments.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1887 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/CorpusFromScikit.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4794 2021-11-15 03:48:32.000000 scattertext-0.1.9/scattertext/CorpusFromTermFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1276 2021-01-24 20:14:58.000000 scattertext-0.1.9/scattertext/CorpusWithoutCategoriesFromParsedDocuments.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2629 2022-06-16 19:49:19.000000 scattertext-0.1.9/scattertext/DataFrameCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2832 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/DeployedClassifier.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3870 2022-01-21 07:14:28.000000 scattertext-0.1.9/scattertext/DocsAndLabelsFromCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      385 2022-11-02 23:36:56.000000 scattertext-0.1.9/scattertext/FeatureOuput.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      388 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/Formatter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4398 2022-03-21 06:27:13.000000 scattertext-0.1.9/scattertext/OffsetCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3999 2022-03-20 23:20:25.000000 scattertext-0.1.9/scattertext/OffsetCorpusFactory.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      161 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/OneClassScatterChart.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      673 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/PValGetter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4801 2022-06-16 19:49:19.000000 scattertext-0.1.9/scattertext/ParsedCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4829 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/PriorFactory.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4658 2018-12-05 08:45:20.000000 scattertext-0.1.9/scattertext/SampleCorpora.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1889 2019-11-06 06:45:38.000000 scattertext-0.1.9/scattertext/SampleLexicons.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6618 2022-11-08 01:12:53.000000 scattertext-0.1.9/scattertext/Scalers.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    29913 2022-10-14 01:51:22.000000 scattertext-0.1.9/scattertext/ScatterChart.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2911 2022-01-21 07:08:19.000000 scattertext-0.1.9/scattertext/ScatterChartData.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    10458 2022-10-14 06:14:12.000000 scattertext-0.1.9/scattertext/ScatterChartExplorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7387 2022-03-23 20:23:35.000000 scattertext-0.1.9/scattertext/TermCategoryFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    37629 2022-10-06 06:16:30.000000 scattertext-0.1.9/scattertext/TermDocMatrix.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    14114 2022-03-20 22:35:54.000000 scattertext-0.1.9/scattertext/TermDocMatrixFactory.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2871 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/TermDocMatrixFilter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1973 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/TermDocMatrixFromFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    12293 2022-03-20 22:37:08.000000 scattertext-0.1.9/scattertext/TermDocMatrixFromPandas.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2821 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/TermDocMatrixFromScikit.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    23837 2022-10-11 00:08:48.000000 scattertext-0.1.9/scattertext/TermDocMatrixWithoutCategories.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4635 2021-01-25 02:41:00.000000 scattertext-0.1.9/scattertext/WhitespaceNLP.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    99483 2022-11-08 00:51:51.000000 scattertext-0.1.9/scattertext/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.463479 scattertext-0.1.9/scattertext/categorygrouping/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4608 2022-06-15 02:11:38.000000 scattertext-0.1.9/scattertext/categorygrouping/CharacteristicGrouper.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2022-05-30 01:17:33.000000 scattertext-0.1.9/scattertext/categorygrouping/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.467259 scattertext-0.1.9/scattertext/categoryprojector/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7074 2022-06-17 04:57:42.000000 scattertext-0.1.9/scattertext/categoryprojector/CategoryProjection.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     8841 2022-10-21 06:35:29.000000 scattertext-0.1.9/scattertext/categoryprojector/CategoryProjector.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3371 2019-08-17 15:49:39.000000 scattertext-0.1.9/scattertext/categoryprojector/CategoryProjectorEvaluator.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     5553 2022-07-20 22:14:11.000000 scattertext-0.1.9/scattertext/categoryprojector/OptimalProjection.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2019-01-28 01:45:23.000000 scattertext-0.1.9/scattertext/categoryprojector/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    13260 2022-10-21 06:35:38.000000 scattertext-0.1.9/scattertext/categoryprojector/pairplot.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.468197 scattertext-0.1.9/scattertext/categorytable/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7208 2022-08-11 01:27:36.000000 scattertext-0.1.9/scattertext/categorytable/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.469664 scattertext-0.1.9/scattertext/characteristic/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2339 2021-01-17 19:16:52.000000 scattertext-0.1.9/scattertext/characteristic/DenseRankCharacteristicness.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/characteristic/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.472103 scattertext-0.1.9/scattertext/continuous/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-03-30 06:09:40.000000 scattertext-0.1.9/scattertext/continuous/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      354 2021-03-30 06:38:16.000000 scattertext-0.1.9/scattertext/continuous/coefficientbase.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1802 2022-11-10 23:35:27.000000 scattertext-0.1.9/scattertext/continuous/correlations.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1229 2021-04-01 23:45:01.000000 scattertext-0.1.9/scattertext/continuous/sklearnpipeline.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1621 2021-04-01 23:01:22.000000 scattertext-0.1.9/scattertext/continuous/ungar.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.534804 scattertext-0.1.9/scattertext/data/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    12316 2021-04-26 15:14:49.000000 scattertext-0.1.9/scattertext/data/arglex_Somasundaran07.json
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   214434 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/chinese.csv
+-rw-r--r--   0 jasonkessler   (501) staff       (20)  4956327 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/count_1w.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)  5566017 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/count_2w.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   175176 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/hamlet.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)  2906024 2020-06-07 23:07:24.000000 scattertext-0.1.9/scattertext/data/inqtabs.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    59085 2020-06-07 23:19:29.000000 scattertext-0.1.9/scattertext/data/mfd2.0.csv
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   767471 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/political_data.csv
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   994217 2020-12-31 08:08:26.000000 scattertext-0.1.9/scattertext/data/political_data.json
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    99979 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/presidential_debates_2016.csv.gz
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   433305 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/punkt.english.pickle
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   234366 2020-08-20 07:11:06.000000 scattertext-0.1.9/scattertext/data/republican_convention_2016.csv
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   224203 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/rotten_tomatoes_corpus.csv.bz2
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   681736 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/rotten_tomatoes_corpus_full.csv.bz2
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.540847 scattertext-0.1.9/scattertext/data/viz/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1035 2020-03-29 06:00:32.000000 scattertext-0.1.9/scattertext/data/viz/autocomplete.css
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6436 2021-06-06 00:15:53.000000 scattertext-0.1.9/scattertext/data/viz/graph_plot.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     9307 2022-01-01 23:30:24.000000 scattertext-0.1.9/scattertext/data/viz/pairplot.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6387 2021-08-11 08:14:44.000000 scattertext-0.1.9/scattertext/data/viz/pairplot_without_halo.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     5218 2021-01-17 07:44:44.000000 scattertext-0.1.9/scattertext/data/viz/scattertext.html
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.548143 scattertext-0.1.9/scattertext/data/viz/scripts/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      131 2020-03-29 04:17:17.000000 scattertext-0.1.9/scattertext/data/viz/scripts/autocomplete_call.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4739 2020-12-18 09:05:24.000000 scattertext-0.1.9/scattertext/data/viz/scripts/autocomplete_definition.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    18948 2018-11-18 19:14:41.000000 scattertext-0.1.9/scattertext/data/viz/scripts/d3-scale-chromatic.v1.min.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   214693 2018-11-18 19:14:19.000000 scattertext-0.1.9/scattertext/data/viz/scripts/d3.min.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   152434 2022-09-26 06:14:36.000000 scattertext-0.1.9/scattertext/data/viz/scripts/main.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   105987 2019-01-15 08:16:37.000000 scattertext-0.1.9/scattertext/data/viz/scripts/main_bk.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6230 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/viz/scripts/range-tree.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   195294 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/viz/scripts/rectangle-holder.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   334370 2020-04-18 01:24:42.000000 scattertext-0.1.9/scattertext/data/viz/scripts/timelines-chart.js
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      204 2020-03-29 05:03:48.000000 scattertext-0.1.9/scattertext/data/viz/search_form.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1779 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/data/viz/semiotic.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     9163 2021-11-15 03:05:40.000000 scattertext-0.1.9/scattertext/data/viz/semiotic_new.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6520 2021-06-14 01:28:19.000000 scattertext-0.1.9/scattertext/data/viz/table_plot.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7014 2021-06-13 23:45:31.000000 scattertext-0.1.9/scattertext/data/viz/time_plot.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    12770 2019-01-30 06:33:53.000000 scattertext-0.1.9/scattertext/data/viz/timeline.html
+-rw-r--r--   0 jasonkessler   (501) staff       (20)   205970 2019-11-06 04:02:51.000000 scattertext-0.1.9/scattertext/data/whissells_df.csv
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.555470 scattertext-0.1.9/scattertext/diachronic/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      805 2020-04-11 22:25:24.000000 scattertext-0.1.9/scattertext/diachronic/BubbleDiachronicVisualization.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2020-04-13 00:58:53.000000 scattertext-0.1.9/scattertext/diachronic/DiachronicPairPlot.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6659 2021-05-24 00:15:15.000000 scattertext-0.1.9/scattertext/diachronic/DiachronicTermMiner.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      108 2019-01-30 06:48:40.000000 scattertext-0.1.9/scattertext/diachronic/DiachronicVisualizer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4911 2020-04-12 22:20:46.000000 scattertext-0.1.9/scattertext/diachronic/GanttChart.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1203 2021-06-06 00:24:52.000000 scattertext-0.1.9/scattertext/diachronic/TimeStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       58 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/diachronic/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.556744 scattertext-0.1.9/scattertext/dispersion/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     8896 2021-05-31 01:36:55.000000 scattertext-0.1.9/scattertext/dispersion/Dispersion.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-15 03:07:37.000000 scattertext-0.1.9/scattertext/dispersion/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.558581 scattertext-0.1.9/scattertext/distancemeasures/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      333 2019-04-18 22:11:50.000000 scattertext-0.1.9/scattertext/distancemeasures/DistanceMeasureBase.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      304 2019-04-18 22:12:12.000000 scattertext-0.1.9/scattertext/distancemeasures/EuclideanDistance.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      102 2019-04-18 22:16:17.000000 scattertext-0.1.9/scattertext/distancemeasures/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.559877 scattertext-0.1.9/scattertext/domain/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1050 2020-02-23 05:35:23.000000 scattertext-0.1.9/scattertext/domain/CombineDocsIntoDomains.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/domain/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.561877 scattertext-0.1.9/scattertext/emojis/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1977 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/emojis/EmojiExtractor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    68316 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/emojis/ProcessedEmojiStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/emojis/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.562111 scattertext-0.1.9/scattertext/external/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/external/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.562657 scattertext-0.1.9/scattertext/external/phrasemachine/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/external/phrasemachine/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    11067 2021-03-08 03:23:59.000000 scattertext-0.1.9/scattertext/external/phrasemachine/phrasemachine.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.577965 scattertext-0.1.9/scattertext/features/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    10371 2021-07-26 07:11:25.000000 scattertext-0.1.9/scattertext/features/CognitiveDistortionsOffsetGetter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    20724 2018-12-03 17:17:11.000000 scattertext-0.1.9/scattertext/features/FeatsFromGeneralInquirer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3167 2020-06-07 23:32:50.000000 scattertext-0.1.9/scattertext/features/FeatsFromMoralFoundationsDictionary.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      348 2021-02-03 08:22:17.000000 scattertext-0.1.9/scattertext/features/FeatsFromOnlyEmpath.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1860 2019-11-03 21:38:17.000000 scattertext-0.1.9/scattertext/features/FeatsFromScoredLexicon.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      548 2019-12-04 08:32:02.000000 scattertext-0.1.9/scattertext/features/FeatsFromSentencePiece.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3300 2022-06-17 02:54:35.000000 scattertext-0.1.9/scattertext/features/FeatsFromSpacyDoc.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2110 2021-02-03 08:23:49.000000 scattertext-0.1.9/scattertext/features/FeatsFromSpacyDocAndEmpath.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      451 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/features/FeatsFromSpacyDocOnlyEmoji.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      404 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/features/FeatsFromSpacyDocOnlyNounChunks.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4027 2021-03-06 03:35:02.000000 scattertext-0.1.9/scattertext/features/FeatsFromTopicModel.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1370 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/features/PhraseMachinePhrases.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2045 2021-03-08 05:39:42.000000 scattertext-0.1.9/scattertext/features/PyTextRankPhrases.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      432 2021-08-24 01:39:13.000000 scattertext-0.1.9/scattertext/features/PyatePhrases.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      936 2021-04-21 07:04:27.000000 scattertext-0.1.9/scattertext/features/RegexFeatAndOffsetGetter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      929 2020-07-17 03:42:17.000000 scattertext-0.1.9/scattertext/features/SpacyEntities.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      400 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/features/UnigramsFromSpacyDoc.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      365 2020-03-23 07:17:39.000000 scattertext-0.1.9/scattertext/features/UseFullDocAsFeature.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      430 2020-04-05 01:21:48.000000 scattertext-0.1.9/scattertext/features/UseFullDocAsMetadata.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/features/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.579350 scattertext-0.1.9/scattertext/features/featoffsets/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-24 20:37:18.000000 scattertext-0.1.9/scattertext/features/featoffsets/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      222 2022-03-20 23:29:02.000000 scattertext-0.1.9/scattertext/features/featoffsets/feat_and_offset_getter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2817 2022-11-11 01:04:57.000000 scattertext-0.1.9/scattertext/features/featoffsets/flexible_ngram_features.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      552 2021-12-28 08:50:38.000000 scattertext-0.1.9/scattertext/features/featoffsets/token_and_feat_offset_getter.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.580497 scattertext-0.1.9/scattertext/frequencyreaders/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2015 2022-03-24 19:19:45.000000 scattertext-0.1.9/scattertext/frequencyreaders/DefaultBackgroundFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/frequencyreaders/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.583808 scattertext-0.1.9/scattertext/graphs/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2891 2020-05-18 01:24:44.000000 scattertext-0.1.9/scattertext/graphs/ComponentDiGraph.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     5977 2020-05-18 02:25:17.000000 scattertext-0.1.9/scattertext/graphs/ComponentDiGraphHTMLRenderer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3682 2021-11-15 01:34:55.000000 scattertext-0.1.9/scattertext/graphs/GraphStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2554 2020-05-18 01:26:51.000000 scattertext-0.1.9/scattertext/graphs/SimpleDiGraph.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      202 2020-04-07 03:09:55.000000 scattertext-0.1.9/scattertext/graphs/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.585166 scattertext-0.1.9/scattertext/helpers/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      259 2021-01-01 08:59:53.000000 scattertext-0.1.9/scattertext/helpers/MakeUnique.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-01 08:40:25.000000 scattertext-0.1.9/scattertext/helpers/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.587433 scattertext-0.1.9/scattertext/indexstore/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2347 2022-07-07 00:21:34.000000 scattertext-0.1.9/scattertext/indexstore/IndexStore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      508 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/indexstore/IndexStoreFromDict.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      392 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/indexstore/IndexStoreFromList.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      137 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/indexstore/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.592864 scattertext-0.1.9/scattertext/representations/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     9122 2021-05-08 17:49:56.000000 scattertext-0.1.9/scattertext/representations/CategoryEmbeddings.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      567 2018-10-15 05:40:59.000000 scattertext-0.1.9/scattertext/representations/CorpusSentenceIterator.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1503 2019-03-25 00:47:57.000000 scattertext-0.1.9/scattertext/representations/Doc2VecBuilder.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4120 2021-11-15 03:14:28.000000 scattertext-0.1.9/scattertext/representations/EmbeddingsResolver.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       19 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/representations/GensimPhraseAugmenter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2420 2021-07-29 07:04:43.000000 scattertext-0.1.9/scattertext/representations/LatentSemanticScaling.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6207 2021-06-27 03:28:56.000000 scattertext-0.1.9/scattertext/representations/Word2VecFromParsedCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      196 2019-10-13 00:29:27.000000 scattertext-0.1.9/scattertext/representations/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.595971 scattertext-0.1.9/scattertext/semioticsquare/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2395 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/semioticsquare/FourSquare.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3797 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/semioticsquare/FourSquareAxis.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7662 2019-04-18 21:50:46.000000 scattertext-0.1.9/scattertext/semioticsquare/SemioticSquare.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3099 2020-09-30 02:03:08.000000 scattertext-0.1.9/scattertext/semioticsquare/SemioticSquareFromAxes.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       42 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/semioticsquare/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.624786 scattertext-0.1.9/scattertext/smoothing/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       57 2021-05-14 04:26:53.000000 scattertext-0.1.9/scattertext/smoothing/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      589 2022-11-04 20:27:25.000000 scattertext-0.1.9/scattertext/smoothing/lowess.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      684 2021-01-18 23:37:44.000000 scattertext-0.1.9/scattertext/smoothing/mean_isotonic.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      480 2021-04-28 04:38:57.000000 scattertext-0.1.9/scattertext/smoothing/power_law.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      725 2021-02-01 07:17:36.000000 scattertext-0.1.9/scattertext/smoothing/sigmoidal.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.629939 scattertext-0.1.9/scattertext/termcompaction/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7974 2022-10-21 06:18:58.000000 scattertext-0.1.9/scattertext/termcompaction/AssociationCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1106 2020-02-23 06:03:48.000000 scattertext-0.1.9/scattertext/termcompaction/ClassPercentageCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2839 2020-02-23 05:31:10.000000 scattertext-0.1.9/scattertext/termcompaction/CompactTerms.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1917 2020-02-23 05:37:20.000000 scattertext-0.1.9/scattertext/termcompaction/DomainCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1623 2020-02-23 05:42:15.000000 scattertext-0.1.9/scattertext/termcompaction/PhraseSelector.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      623 2022-08-17 01:27:55.000000 scattertext-0.1.9/scattertext/termcompaction/ScikitCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termcompaction/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.634858 scattertext-0.1.9/scattertext/termranking/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      468 2019-11-24 18:07:17.000000 scattertext-0.1.9/scattertext/termranking/AbsoluteFrequencyRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      340 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termranking/DocLengthDividedFrequencyRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1691 2019-11-24 18:08:36.000000 scattertext-0.1.9/scattertext/termranking/DocLengthNormalizedFrequencyRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      529 2020-03-19 04:27:10.000000 scattertext-0.1.9/scattertext/termranking/OncePerDocFrequencyRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1355 2020-02-23 00:28:44.000000 scattertext-0.1.9/scattertext/termranking/TermRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      286 2018-11-22 00:21:48.000000 scattertext-0.1.9/scattertext/termranking/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.649648 scattertext-0.1.9/scattertext/termscoring/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1810 2022-07-16 20:06:40.000000 scattertext-0.1.9/scattertext/termscoring/BM25Difference.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2923 2022-11-11 00:10:03.000000 scattertext-0.1.9/scattertext/termscoring/BNSScorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3888 2019-11-24 21:29:27.000000 scattertext-0.1.9/scattertext/termscoring/BetaPosterior.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2210 2022-03-26 09:20:41.000000 scattertext-0.1.9/scattertext/termscoring/CohensD.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3092 2021-06-22 06:15:15.000000 scattertext-0.1.9/scattertext/termscoring/CohensDCalculator.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1331 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termscoring/CornerScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     5351 2022-10-14 01:56:19.000000 scattertext-0.1.9/scattertext/termscoring/CorpusBasedTermScorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2360 2022-03-09 23:49:08.000000 scattertext-0.1.9/scattertext/termscoring/CraigsZeta.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     9983 2020-07-19 23:24:23.000000 scattertext-0.1.9/scattertext/termscoring/CredTFIDF.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      641 2021-06-22 01:17:05.000000 scattertext-0.1.9/scattertext/termscoring/DeltaJSDivergence.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1025 2022-01-02 00:02:26.000000 scattertext-0.1.9/scattertext/termscoring/LogOddsRatio.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2040 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termscoring/LogOddsUniformativePriorScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3706 2019-11-24 21:30:14.000000 scattertext-0.1.9/scattertext/termscoring/MannWhitneyU.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      946 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termscoring/OLSUngnarStyle.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4623 2022-07-07 01:11:22.000000 scattertext-0.1.9/scattertext/termscoring/Productivity.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      442 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termscoring/RankDifference.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1457 2022-01-02 00:08:08.000000 scattertext-0.1.9/scattertext/termscoring/RankDifferenceScorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1735 2018-10-15 06:13:55.000000 scattertext-0.1.9/scattertext/termscoring/RelativeEntropy.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    13605 2020-03-29 02:16:08.000000 scattertext-0.1.9/scattertext/termscoring/ScaledFScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4622 2022-08-17 01:34:11.000000 scattertext-0.1.9/scattertext/termscoring/ScikitTermScorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      854 2018-10-02 04:59:29.000000 scattertext-0.1.9/scattertext/termscoring/ZScores.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      230 2019-01-08 05:35:22.000000 scattertext-0.1.9/scattertext/termscoring/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      596 2019-04-30 04:58:21.000000 scattertext-0.1.9/scattertext/termscoring/test_credTFIDF.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.652739 scattertext-0.1.9/scattertext/termsignificance/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3145 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioInformativeDirichletPiror.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2601 2021-12-29 04:51:14.000000 scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioSmoothed.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3121 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioUninformativeDirichletPrior.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1348 2018-12-27 07:09:54.000000 scattertext-0.1.9/scattertext/termsignificance/ScaledFScoreSignificance.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      148 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termsignificance/TermSignificance.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       93 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/termsignificance/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.674731 scattertext-0.1.9/scattertext/test/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      692 2020-02-11 05:35:03.000000 scattertext-0.1.9/scattertext/test/test_BM25Difference.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1717 2019-11-03 21:03:34.000000 scattertext-0.1.9/scattertext/test/test_CSRMatrixTools.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1595 2018-12-11 10:17:21.000000 scattertext-0.1.9/scattertext/test/test_CategoryColorAssigner.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2178 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_CornerScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6127 2021-01-18 08:06:24.000000 scattertext-0.1.9/scattertext/test/test_CorpusFromParsedDocuments.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      655 2021-01-15 04:47:47.000000 scattertext-0.1.9/scattertext/test/test_CorpusWithoutCategoriesFromParsedDocuments.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1910 2021-01-16 07:51:31.000000 scattertext-0.1.9/scattertext/test/test_Dispersion.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4714 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_FeatsFromSpacyDoc.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      447 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_HTMLSemioticSquareViz.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    29944 2022-09-25 17:49:20.000000 scattertext-0.1.9/scattertext/test/test_HTMLVisualizationAssembly.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2367 2021-01-04 01:02:32.000000 scattertext-0.1.9/scattertext/test/test_PMIFiltering.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2528 2020-02-11 05:30:21.000000 scattertext-0.1.9/scattertext/test/test_ParsedCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4207 2021-01-04 01:10:05.000000 scattertext-0.1.9/scattertext/test/test_PriorFactory.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      756 2019-01-26 11:09:36.000000 scattertext-0.1.9/scattertext/test/test_Scalers.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    26533 2022-10-06 06:08:24.000000 scattertext-0.1.9/scattertext/test/test_TermDocMat.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1981 2019-10-08 19:45:28.000000 scattertext-0.1.9/scattertext/test/test_WhitespaceNLP.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      997 2020-02-11 05:34:02.000000 scattertext-0.1.9/scattertext/test/test_ZScores.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3648 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_asiannlp.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1409 2019-03-06 18:28:07.000000 scattertext-0.1.9/scattertext/test/test_associationCompator.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      847 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_autoTermSelector.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      845 2019-11-24 21:45:03.000000 scattertext-0.1.9/scattertext/test/test_betaPosterior.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      766 2018-12-27 08:24:21.000000 scattertext-0.1.9/scattertext/test/test_classPercentageCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2804 2020-06-08 01:19:45.000000 scattertext-0.1.9/scattertext/test/test_cohensD.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      565 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_combineDocsIntoDomains.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1723 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_compactTerms.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     9316 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_corpusFromFeatureDict.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3176 2020-02-11 05:30:21.000000 scattertext-0.1.9/scattertext/test/test_corpusFromPandas.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1515 2018-12-21 04:59:51.000000 scattertext-0.1.9/scattertext/test/test_corpusFromPandasWithoutCategories.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1180 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_corpusFromScikit.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1006 2020-02-14 16:58:51.000000 scattertext-0.1.9/scattertext/test/test_credTFIDF.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      492 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_denseRankCharacteristicness.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    32298 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_diachronicTermMiner.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6997 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_docsAndLabelsFromCorpus.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1231 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_domainCompactor.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2636 2021-11-15 03:16:25.000000 scattertext-0.1.9/scattertext/test/test_embeddingsResolver.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1025 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_extract_emoji.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1884 2020-02-11 05:33:21.000000 scattertext-0.1.9/scattertext/test/test_featsFromScoredLexicon.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6011 2018-10-15 06:26:19.000000 scattertext-0.1.9/scattertext/test/test_featsFromSpacyDocAndEmpath.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      907 2020-10-11 22:48:42.000000 scattertext-0.1.9/scattertext/test/test_featsFromTopicModel.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      867 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_featureLister.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3819 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_fourSquareAxes.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1077 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_gensimPhraseAdder.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3142 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_indexStore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      587 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_indexStoreFromDict.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      394 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_indexStoreFromList.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      703 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_large_int_format.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1064 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_logOddsRatioUninformativeDirichletPrior.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2121 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_logOddsUninformativePriorScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      366 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_oneClassScatterChart.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      420 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_percentile_lexicographic.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      553 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_phraseSelector.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      713 2020-02-11 05:35:03.000000 scattertext-0.1.9/scattertext/test/test_relativeEntropy.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2270 2019-02-21 08:21:33.000000 scattertext-0.1.9/scattertext/test/test_scaledFScore.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    14504 2020-02-11 05:04:46.000000 scattertext-0.1.9/scattertext/test/test_scatterChart.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     8772 2019-04-18 00:14:00.000000 scattertext-0.1.9/scattertext/test/test_scatterChartExplorer.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4311 2020-02-11 05:33:44.000000 scattertext-0.1.9/scattertext/test/test_semioticSquare.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3328 2019-04-19 00:53:26.000000 scattertext-0.1.9/scattertext/test/test_semioticSquareFromAxes.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     4401 2020-02-11 05:34:52.000000 scattertext-0.1.9/scattertext/test/test_termCategoryFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     5535 2019-08-13 02:04:11.000000 scattertext-0.1.9/scattertext/test/test_termDocMatrixFactory.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      784 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_termDocMatrixFromFrequencies.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    49161 2020-02-11 05:30:21.000000 scattertext-0.1.9/scattertext/test/test_termDocMatrixFromPandas.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1126 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_termDocMatrixFromScikit.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2640 2020-02-11 05:30:21.000000 scattertext-0.1.9/scattertext/test/test_termRanker.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      438 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_unigramsFromSpacyDoc.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      443 2020-03-23 04:41:28.000000 scattertext-0.1.9/scattertext/test/test_useFullDocAsFeature.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      454 2020-03-23 07:17:55.000000 scattertext-0.1.9/scattertext/test/test_useFullDocAsMetadata.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      982 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/test/test_vizDataAdapter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1892 2021-11-15 03:39:09.000000 scattertext-0.1.9/scattertext/test/test_word2VecFromParsedCorpus.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.675156 scattertext-0.1.9/scattertext/tokenizers/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2021-01-25 02:40:00.000000 scattertext-0.1.9/scattertext/tokenizers/__init__.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     2450 2021-03-14 01:28:31.000000 scattertext-0.1.9/scattertext/tokenizers/roberta.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.676372 scattertext-0.1.9/scattertext/topicmodel/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3519 2020-06-21 23:38:55.000000 scattertext-0.1.9/scattertext/topicmodel/SentencesForTopicModeling.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       64 2018-09-21 06:21:05.000000 scattertext-0.1.9/scattertext/topicmodel/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.676908 scattertext-0.1.9/scattertext/topicmodel/interface/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        0 2020-04-06 00:38:07.000000 scattertext-0.1.9/scattertext/topicmodel/interface/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.681259 scattertext-0.1.9/scattertext/viz/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6690 2022-01-01 23:28:02.000000 scattertext-0.1.9/scattertext/viz/BasicHTMLFromScatterplotStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     3255 2021-11-15 01:25:21.000000 scattertext-0.1.9/scattertext/viz/HTMLSemioticSquareViz.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     6050 2022-01-01 23:29:08.000000 scattertext-0.1.9/scattertext/viz/PairPlotFromScattertextStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     7405 2022-11-04 19:27:13.000000 scattertext-0.1.9/scattertext/viz/PyPlotFromScattertextStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    21947 2022-09-25 17:50:31.000000 scattertext-0.1.9/scattertext/viz/ScatterplotStructure.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1853 2021-02-15 02:32:51.000000 scattertext-0.1.9/scattertext/viz/TermInfo.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1159 2019-01-06 09:31:16.000000 scattertext-0.1.9/scattertext/viz/VizDataAdapter.py
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      329 2019-01-28 03:29:06.000000 scattertext-0.1.9/scattertext/viz/__init__.py
+drwxr-xr-x   0 jasonkessler   (501) staff       (20)        0 2022-11-11 01:06:39.462448 scattertext-0.1.9/scattertext.egg-info/
+-rw-r--r--   0 jasonkessler   (501) staff       (20)      276 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/PKG-INFO
+-rw-r--r--   0 jasonkessler   (501) staff       (20)    12519 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        1 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       53 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/entry_points.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)        1 2018-09-21 06:28:35.000000 scattertext-0.1.9/scattertext.egg-info/not-zip-safe
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       77 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/requires.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       12 2022-11-11 01:06:39.000000 scattertext-0.1.9/scattertext.egg-info/top_level.txt
+-rw-r--r--   0 jasonkessler   (501) staff       (20)       38 2022-11-11 01:06:39.682371 scattertext-0.1.9/setup.cfg
+-rw-r--r--   0 jasonkessler   (501) staff       (20)     1128 2022-11-10 23:49:58.000000 scattertext-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scattertext-0.1.8/LICENSE` & `scattertext-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext.egg-info/SOURCES.txt` & `scattertext-0.1.9/scattertext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixWithoutCategories.py` & `scattertext-0.1.9/scattertext/TermDocMatrixWithoutCategories.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/Word2VecFromParsedCorpus.py` & `scattertext-0.1.9/scattertext/representations/Word2VecFromParsedCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/EmbeddingsResolver.py` & `scattertext-0.1.9/scattertext/representations/EmbeddingsResolver.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/CategoryEmbeddings.py` & `scattertext-0.1.9/scattertext/representations/CategoryEmbeddings.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/CorpusSentenceIterator.py` & `scattertext-0.1.9/scattertext/representations/CorpusSentenceIterator.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/Doc2VecBuilder.py` & `scattertext-0.1.9/scattertext/representations/Doc2VecBuilder.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/representations/LatentSemanticScaling.py` & `scattertext-0.1.9/scattertext/representations/LatentSemanticScaling.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categorygrouping/CharacteristicGrouper.py` & `scattertext-0.1.9/scattertext/categorygrouping/CharacteristicGrouper.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/tokenizers/roberta.py` & `scattertext-0.1.9/scattertext/tokenizers/roberta.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/SampleCorpora.py` & `scattertext-0.1.9/scattertext/SampleCorpora.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/PriorFactory.py` & `scattertext-0.1.9/scattertext/PriorFactory.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/SampleLexicons.py` & `scattertext-0.1.9/scattertext/SampleLexicons.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/topicmodel/SentencesForTopicModeling.py` & `scattertext-0.1.9/scattertext/topicmodel/SentencesForTopicModeling.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusFromTermFrequencies.py` & `scattertext-0.1.9/scattertext/CorpusFromTermFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/OffsetCorpusFactory.py` & `scattertext-0.1.9/scattertext/OffsetCorpusFactory.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusFromScikit.py` & `scattertext-0.1.9/scattertext/CorpusFromScikit.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/characteristic/DenseRankCharacteristicness.py` & `scattertext-0.1.9/scattertext/characteristic/DenseRankCharacteristicness.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_cohensD.py` & `scattertext-0.1.9/scattertext/test/test_cohensD.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_associationCompator.py` & `scattertext-0.1.9/scattertext/test/test_associationCompator.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_CornerScore.py` & `scattertext-0.1.9/scattertext/test/test_CornerScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_combineDocsIntoDomains.py` & `scattertext-0.1.9/scattertext/test/test_combineDocsIntoDomains.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_ParsedCorpus.py` & `scattertext-0.1.9/scattertext/test/test_ParsedCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_scatterChartExplorer.py` & `scattertext-0.1.9/scattertext/test/test_scatterChartExplorer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termCategoryFrequencies.py` & `scattertext-0.1.9/scattertext/test/test_termCategoryFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_corpusFromPandas.py` & `scattertext-0.1.9/scattertext/test/test_corpusFromPandas.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_scaledFScore.py` & `scattertext-0.1.9/scattertext/test/test_scaledFScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_vizDataAdapter.py` & `scattertext-0.1.9/scattertext/test/test_vizDataAdapter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termDocMatrixFromPandas.py` & `scattertext-0.1.9/scattertext/test/test_termDocMatrixFromPandas.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_Dispersion.py` & `scattertext-0.1.9/scattertext/test/test_Dispersion.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_relativeEntropy.py` & `scattertext-0.1.9/scattertext/test/test_relativeEntropy.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_domainCompactor.py` & `scattertext-0.1.9/scattertext/test/test_domainCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_diachronicTermMiner.py` & `scattertext-0.1.9/scattertext/test/test_diachronicTermMiner.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_indexStoreFromDict.py` & `scattertext-0.1.9/scattertext/test/test_indexStoreFromDict.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_phraseSelector.py` & `scattertext-0.1.9/scattertext/test/test_phraseSelector.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_docsAndLabelsFromCorpus.py` & `scattertext-0.1.9/scattertext/test/test_docsAndLabelsFromCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_indexStore.py` & `scattertext-0.1.9/scattertext/test/test_indexStore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_featsFromSpacyDocAndEmpath.py` & `scattertext-0.1.9/scattertext/test/test_featsFromSpacyDocAndEmpath.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_logOddsUninformativePriorScore.py` & `scattertext-0.1.9/scattertext/test/test_logOddsUninformativePriorScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_semioticSquareFromAxes.py` & `scattertext-0.1.9/scattertext/test/test_semioticSquareFromAxes.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_compactTerms.py` & `scattertext-0.1.9/scattertext/test/test_compactTerms.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_CategoryColorAssigner.py` & `scattertext-0.1.9/scattertext/test/test_CategoryColorAssigner.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_betaPosterior.py` & `scattertext-0.1.9/scattertext/test/test_betaPosterior.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_CorpusFromParsedDocuments.py` & `scattertext-0.1.9/scattertext/test/test_CorpusFromParsedDocuments.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_autoTermSelector.py` & `scattertext-0.1.9/scattertext/test/test_autoTermSelector.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_Scalers.py` & `scattertext-0.1.9/scattertext/test/test_Scalers.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_corpusFromFeatureDict.py` & `scattertext-0.1.9/scattertext/test/test_corpusFromFeatureDict.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_CorpusWithoutCategoriesFromParsedDocuments.py` & `scattertext-0.1.9/scattertext/test/test_CorpusWithoutCategoriesFromParsedDocuments.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_semioticSquare.py` & `scattertext-0.1.9/scattertext/test/test_semioticSquare.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_logOddsRatioUninformativeDirichletPrior.py` & `scattertext-0.1.9/scattertext/test/test_logOddsRatioUninformativeDirichletPrior.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termDocMatrixFromFrequencies.py` & `scattertext-0.1.9/scattertext/test/test_termDocMatrixFromFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_ZScores.py` & `scattertext-0.1.9/scattertext/test/test_ZScores.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_FeatsFromSpacyDoc.py` & `scattertext-0.1.9/scattertext/test/test_FeatsFromSpacyDoc.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termRanker.py` & `scattertext-0.1.9/scattertext/test/test_termRanker.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_word2VecFromParsedCorpus.py` & `scattertext-0.1.9/scattertext/test/test_word2VecFromParsedCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_classPercentageCompactor.py` & `scattertext-0.1.9/scattertext/test/test_classPercentageCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_PMIFiltering.py` & `scattertext-0.1.9/scattertext/test/test_PMIFiltering.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_embeddingsResolver.py` & `scattertext-0.1.9/scattertext/test/test_embeddingsResolver.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_extract_emoji.py` & `scattertext-0.1.9/scattertext/test/test_extract_emoji.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_WhitespaceNLP.py` & `scattertext-0.1.9/scattertext/test/test_WhitespaceNLP.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_featureLister.py` & `scattertext-0.1.9/scattertext/test/test_featureLister.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_HTMLVisualizationAssembly.py` & `scattertext-0.1.9/scattertext/test/test_HTMLVisualizationAssembly.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_featsFromScoredLexicon.py` & `scattertext-0.1.9/scattertext/test/test_featsFromScoredLexicon.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_PriorFactory.py` & `scattertext-0.1.9/scattertext/test/test_PriorFactory.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_BM25Difference.py` & `scattertext-0.1.9/scattertext/test/test_BM25Difference.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_scatterChart.py` & `scattertext-0.1.9/scattertext/test/test_scatterChart.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_CSRMatrixTools.py` & `scattertext-0.1.9/scattertext/test/test_CSRMatrixTools.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_featsFromTopicModel.py` & `scattertext-0.1.9/scattertext/test/test_featsFromTopicModel.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_large_int_format.py` & `scattertext-0.1.9/scattertext/test/test_large_int_format.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_corpusFromPandasWithoutCategories.py` & `scattertext-0.1.9/scattertext/test/test_corpusFromPandasWithoutCategories.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_credTFIDF.py` & `scattertext-0.1.9/scattertext/test/test_credTFIDF.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_corpusFromScikit.py` & `scattertext-0.1.9/scattertext/test/test_corpusFromScikit.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_TermDocMat.py` & `scattertext-0.1.9/scattertext/test/test_TermDocMat.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_fourSquareAxes.py` & `scattertext-0.1.9/scattertext/test/test_fourSquareAxes.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termDocMatrixFactory.py` & `scattertext-0.1.9/scattertext/test/test_termDocMatrixFactory.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_termDocMatrixFromScikit.py` & `scattertext-0.1.9/scattertext/test/test_termDocMatrixFromScikit.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_asiannlp.py` & `scattertext-0.1.9/scattertext/test/test_asiannlp.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/test/test_gensimPhraseAdder.py` & `scattertext-0.1.9/scattertext/test/test_gensimPhraseAdder.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termranking/TermRanker.py` & `scattertext-0.1.9/scattertext/termranking/TermRanker.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termranking/DocLengthNormalizedFrequencyRanker.py` & `scattertext-0.1.9/scattertext/termranking/DocLengthNormalizedFrequencyRanker.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termranking/OncePerDocFrequencyRanker.py` & `scattertext-0.1.9/scattertext/termranking/OncePerDocFrequencyRanker.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CSRMatrixTools.py` & `scattertext-0.1.9/scattertext/CSRMatrixTools.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/DocsAndLabelsFromCorpus.py` & `scattertext-0.1.9/scattertext/DocsAndLabelsFromCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/ScatterChart.py` & `scattertext-0.1.9/scattertext/ScatterChart.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixFromPandas.py` & `scattertext-0.1.9/scattertext/TermDocMatrixFromPandas.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixFromFrequencies.py` & `scattertext-0.1.9/scattertext/TermDocMatrixFromFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/Scalers.py` & `scattertext-0.1.9/scattertext/Scalers.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 def scale_center_zero_abs(vec, other_vec=None):
     if other_vec is None:
         other_vec = vec
     max_abs = max(vec.max(), -vec.min())
     return ((((other_vec > 0).astype(float) * (other_vec / max_abs)) * 0.5 + 0.5)
             + ((other_vec < 0).astype(float) * (other_vec / max_abs) * 0.5))
 
+def scale_center_zero_separate_ranks(scores: np.array) -> np.array:
+    scaled = np.zeros(len(scores), dtype=np.float)
+    scaled[scores > 0] = rankdata(scores[scores > 0]) / len(scores[scores > 0]) / 2 + 0.5
+    scaled[scores < 0] = rankdata(scores[scores < 0]) / len(scores[scores < 0]) / 2
+    return scaled
 
 def scale_neg_1_to_1_with_zero_mean_abs_max(vec):
     max_abs = max(vec.max(), -vec.min())
     return ((((vec > 0).astype(float) * (vec / max_abs)) * 0.5 + 0.5)
             + ((vec < 0).astype(float) * (vec / max_abs) * 0.5))
 
 
@@ -207,7 +212,8 @@
         a[a > 0] = a[a > 0] * 1. / a[a > 0].max()
     return a
 
 
 def scale_0_to_1(vec_ss):
     vec_ss = (vec_ss - vec_ss.min()) * 1. / (vec_ss.max() - vec_ss.min())
     return vec_ss
+
```

### Comparing `scattertext-0.1.8/scattertext/smoothing/lowess.py` & `scattertext-0.1.9/scattertext/smoothing/lowess.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import numpy as np
 import pandas as pd
+
+
 class Lowess(object):
     def __init__(self):
         self.points = None
 
     def fit(self, xdata, ydata):
         import statsmodels.api as sm
-        self.model = sm.nonparametric.lowess(ydata, xdata)#, frac=1./3)
+        self.model = sm.nonparametric.lowess(ydata, xdata)  # , frac=1./3)
         return self
 
     def predict(self, x):
         return np.interp(x, self.model.T[0], self.model.T[1])
 
     def fit_predict(self, xdata, ydata):
         df = pd.DataFrame({
```

### Comparing `scattertext-0.1.8/scattertext/smoothing/sigmoidal.py` & `scattertext-0.1.9/scattertext/smoothing/sigmoidal.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/smoothing/mean_isotonic.py` & `scattertext-0.1.9/scattertext/smoothing/mean_isotonic.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/diachronic/GanttChart.py` & `scattertext-0.1.9/scattertext/diachronic/GanttChart.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/diachronic/DiachronicTermMiner.py` & `scattertext-0.1.9/scattertext/diachronic/DiachronicTermMiner.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/diachronic/BubbleDiachronicVisualization.py` & `scattertext-0.1.9/scattertext/diachronic/BubbleDiachronicVisualization.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/diachronic/TimeStructure.py` & `scattertext-0.1.9/scattertext/diachronic/TimeStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrix.py` & `scattertext-0.1.9/scattertext/TermDocMatrix.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categoryprojector/CategoryProjectorEvaluator.py` & `scattertext-0.1.9/scattertext/categoryprojector/CategoryProjectorEvaluator.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categoryprojector/pairplot.py` & `scattertext-0.1.9/scattertext/categoryprojector/pairplot.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categoryprojector/CategoryProjection.py` & `scattertext-0.1.9/scattertext/categoryprojector/CategoryProjection.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categoryprojector/CategoryProjector.py` & `scattertext-0.1.9/scattertext/categoryprojector/CategoryProjector.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categoryprojector/OptimalProjection.py` & `scattertext-0.1.9/scattertext/categoryprojector/OptimalProjection.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromSpacyDoc.py` & `scattertext-0.1.9/scattertext/features/FeatsFromSpacyDoc.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/PyTextRankPhrases.py` & `scattertext-0.1.9/scattertext/features/PyTextRankPhrases.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromGeneralInquirer.py` & `scattertext-0.1.9/scattertext/features/FeatsFromGeneralInquirer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/RegexFeatAndOffsetGetter.py` & `scattertext-0.1.9/scattertext/features/RegexFeatAndOffsetGetter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromScoredLexicon.py` & `scattertext-0.1.9/scattertext/features/FeatsFromScoredLexicon.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromMoralFoundationsDictionary.py` & `scattertext-0.1.9/scattertext/features/FeatsFromMoralFoundationsDictionary.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromSpacyDocAndEmpath.py` & `scattertext-0.1.9/scattertext/features/FeatsFromSpacyDocAndEmpath.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/PhraseMachinePhrases.py` & `scattertext-0.1.9/scattertext/features/PhraseMachinePhrases.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/featoffsets/flexible_ngram_features.py` & `scattertext-0.1.9/scattertext/features/featoffsets/flexible_ngram_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import List, Tuple, Union, Optional, Callable
 from collections import deque
 
-import spacy.tokens
-
 from scattertext.features.featoffsets.feat_and_offset_getter import FeatAndOffsetGetter
-from scattertext.Common import ENGLISH_STOP_WORDS, MY_ENGLISH_STOP_WORDS
+from scattertext.Common import MY_ENGLISH_STOP_WORDS
 
 
 def window(seq, n=2):
     # adapted from https://stackoverflow.com/questions/46516730/how-to-work-with-zip-on-2-generators-s-t-each-returns-the-same-item-that-changes
     it = iter(seq)
     win = deque((next(it, None) for _ in range(n)), maxlen=n)
     yield list(win)
```

### Comparing `scattertext-0.1.8/scattertext/features/featoffsets/token_and_feat_offset_getter.py` & `scattertext-0.1.9/scattertext/features/featoffsets/token_and_feat_offset_getter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromTopicModel.py` & `scattertext-0.1.9/scattertext/features/FeatsFromTopicModel.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/SpacyEntities.py` & `scattertext-0.1.9/scattertext/features/SpacyEntities.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/FeatsFromSentencePiece.py` & `scattertext-0.1.9/scattertext/features/FeatsFromSentencePiece.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/features/CognitiveDistortionsOffsetGetter.py` & `scattertext-0.1.9/scattertext/features/CognitiveDistortionsOffsetGetter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixFactory.py` & `scattertext-0.1.9/scattertext/TermDocMatrixFactory.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/__init__.py` & `scattertext-0.1.9/scattertext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import print_function
 
-
-version = [0, 1, 8]
+version = [0, 1, 9]
 __version__ = '.'.join([str(e) for e in version])
 
 import re
 import numpy as np
 import pandas as pd
 import warnings
 from scattertext.features.UseFullDocAsFeature import UseFullDocAsFeature
@@ -142,14 +141,16 @@
 from scattertext.termscoring.LogOddsRatio import LogOddsRatio
 from scattertext.termscoring.RankDifferenceScorer import RankDifferenceScorer
 from scattertext.categorygrouping.CharacteristicGrouper import CharacteristicGrouper
 from scattertext.termscoring.Productivity import ProductivityScorer, whole_corpus_productivity_scores
 from scattertext.viz.PyPlotFromScattertextStructure import pyplot_from_scattertext_structure
 from scattertext.termscoring.BNSScorer import BNSScorer
 from scattertext.features.featoffsets.flexible_ngram_features import PosStopgramFeatures, FlexibleNGramFeatures
+from scattertext.continuous.correlations import Correlations
+
 
 PhraseFeatsFromTopicModel = FeatsFromTopicModel  # Ensure backwards compatibility
 
 def cognitive_distortions_offset_getter_factory():
     return LexiconFeatAndOffsetGetter(COGNITIVE_DISTORTIONS_LEXICON, COGNITIVE_DISTORTIONS_DEFINITIONS)
 
 
@@ -788,15 +789,16 @@
     else:
         not_cat_freqs = tdf.sum(axis=1) - tdf[category + ' freq']
     if isinstance(term_scorer, CorpusBasedTermScorer) and not term_scorer.is_category_name_set():
         if show_neutral:
             term_scorer = term_scorer.set_categories(category, not_categories, neutral_categories)
         else:
             term_scorer = term_scorer.set_categories(category, not_categories)
-    return term_scorer.get_scores(cat_freqs, not_cat_freqs)
+    scores = term_scorer.get_scores(cat_freqs, not_cat_freqs)
+    return scores
 
 
 def produce_scattertext_html(term_doc_matrix,
                              category,
                              category_name,
                              not_category_name,
                              protocol='https',
@@ -1076,22 +1078,24 @@
     x_axis_values = [round_downer(10 ** x) for x
                      in np.linspace(0, np.log(freqs.max()) / np.log(10), 5)]
     x_axis_values = [x for x in x_axis_values if x > 1 and x <= freqs.max()]
     # y_axis_values = [-2.58, -1.96, 0, 1.96, 2.58]
     frequencies_log_scaled = frequency_transform(freqs)  # scale(np.log(freqs) - np.log(1))
 
     if 'scores' not in kwargs:
-        kwargs['scores'] = get_term_scorer_scores(category,
-                                                  corpus,
-                                                  kwargs.get('neutral_categories', False),
-                                                  not_categories,
-                                                  kwargs.get('show_neutral', False),
-                                                  term_ranker,
-                                                  term_scorer,
-                                                  kwargs.get('use_non_text_features', False))
+        kwargs['scores'] = get_term_scorer_scores(
+            category,
+            corpus,
+            kwargs.get('neutral_categories', False),
+            not_categories,
+            kwargs.get('show_neutral', False),
+            term_ranker,
+            term_scorer,
+            kwargs.get('use_non_text_features', False)
+        )
 
     def y_axis_rescale(coords):
         return ((coords - 0.5) / (np.abs(coords - 0.5).max()) + 1) / 2
 
     # from https://stackoverflow.com/questions/3410976/how-to-round-a-number-to-significant-figures-in-python
     def round_to_1(x):
         if x == 0:
```

### Comparing `scattertext-0.1.8/scattertext/TermCategoryFrequencies.py` & `scattertext-0.1.9/scattertext/TermCategoryFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/frequencyreaders/DefaultBackgroundFrequencies.py` & `scattertext-0.1.9/scattertext/frequencyreaders/DefaultBackgroundFrequencies.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/semioticsquare/SemioticSquare.py` & `scattertext-0.1.9/scattertext/semioticsquare/SemioticSquare.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/semioticsquare/FourSquare.py` & `scattertext-0.1.9/scattertext/semioticsquare/FourSquare.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/semioticsquare/FourSquareAxis.py` & `scattertext-0.1.9/scattertext/semioticsquare/FourSquareAxis.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/semioticsquare/SemioticSquareFromAxes.py` & `scattertext-0.1.9/scattertext/semioticsquare/SemioticSquareFromAxes.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/DeployedClassifier.py` & `scattertext-0.1.9/scattertext/DeployedClassifier.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/OffsetCorpus.py` & `scattertext-0.1.9/scattertext/OffsetCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CategoryColorAssigner.py` & `scattertext-0.1.9/scattertext/CategoryColorAssigner.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/WhitespaceNLP.py` & `scattertext-0.1.9/scattertext/WhitespaceNLP.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/PValGetter.py` & `scattertext-0.1.9/scattertext/PValGetter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixFromScikit.py` & `scattertext-0.1.9/scattertext/TermDocMatrixFromScikit.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/ScatterplotStructure.py` & `scattertext-0.1.9/scattertext/viz/ScatterplotStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/PyPlotFromScattertextStructure.py` & `scattertext-0.1.9/scattertext/viz/PyPlotFromScattertextStructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     matplotlib figure that can be used with plt.show() or plt.savefig()
 
     """
     try:
         import matplotlib.pyplot as plt
         import textalloc as ta
     except:
-        raise Exception("Ensure that the packages textalloc==0.0.2 and matplotlib>=3.6.0 have been installed.")
+        raise Exception("Ensure that the packages textalloc==0.0.3 and matplotlib>=3.6.0 have been installed.")
 
     # Extract the data
     if sample > 0:
         subset = random.sample(
             scatterplot_structure._visualization_data.word_dict["data"], sample
         )
     else:
```

### Comparing `scattertext-0.1.8/scattertext/viz/BasicHTMLFromScatterplotStructure.py` & `scattertext-0.1.9/scattertext/viz/BasicHTMLFromScatterplotStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/HTMLSemioticSquareViz.py` & `scattertext-0.1.9/scattertext/viz/HTMLSemioticSquareViz.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/PairPlotFromScattertextStructure.py` & `scattertext-0.1.9/scattertext/viz/PairPlotFromScattertextStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/VizDataAdapter.py` & `scattertext-0.1.9/scattertext/viz/VizDataAdapter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/viz/TermInfo.py` & `scattertext-0.1.9/scattertext/viz/TermInfo.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/BM25Difference.py` & `scattertext-0.1.9/scattertext/termscoring/BM25Difference.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/Productivity.py` & `scattertext-0.1.9/scattertext/termscoring/Productivity.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CohensD.py` & `scattertext-0.1.9/scattertext/termscoring/CohensD.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CornerScore.py` & `scattertext-0.1.9/scattertext/termscoring/CornerScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/BetaPosterior.py` & `scattertext-0.1.9/scattertext/termscoring/BetaPosterior.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/MannWhitneyU.py` & `scattertext-0.1.9/scattertext/termscoring/MannWhitneyU.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/ScikitTermScorer.py` & `scattertext-0.1.9/scattertext/termscoring/ScikitTermScorer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CredTFIDF.py` & `scattertext-0.1.9/scattertext/termscoring/CredTFIDF.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/DeltaJSDivergence.py` & `scattertext-0.1.9/scattertext/termscoring/DeltaJSDivergence.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/RankDifferenceScorer.py` & `scattertext-0.1.9/scattertext/termscoring/RankDifferenceScorer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/RelativeEntropy.py` & `scattertext-0.1.9/scattertext/termscoring/RelativeEntropy.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/LogOddsUniformativePriorScore.py` & `scattertext-0.1.9/scattertext/termscoring/LogOddsUniformativePriorScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CorpusBasedTermScorer.py` & `scattertext-0.1.9/scattertext/termscoring/CorpusBasedTermScorer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/ZScores.py` & `scattertext-0.1.9/scattertext/termscoring/ZScores.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/OLSUngnarStyle.py` & `scattertext-0.1.9/scattertext/termscoring/OLSUngnarStyle.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CohensDCalculator.py` & `scattertext-0.1.9/scattertext/termscoring/CohensDCalculator.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/BNSScorer.py` & `scattertext-0.1.9/scattertext/termscoring/BNSScorer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 import pandas as pd
 import numpy as np
 from scipy.stats import norm
 
 from scattertext.termscoring.CorpusBasedTermScorer import CorpusBasedTermScorer
 
-BNS_ALPHA_DEFAULT = 0.005 # Note: I've found this works better for content analysis than 0.0005 as suggested by Forman
+BNS_ALPHA_DEFAULT = None # 0.0005
 
 # Reference: George Forman. 2008. BNS feature scaling: an improved representation over tf-idf for
 # svm text classification. In Proceedings of the 17th ACM conference on Information and
 # knowledge management (CIKM '08). Association for Computing Machinery, New York, NY, USA,
 # 263–270. https://doi.org/10.1145/1458082.1458119
 
 class BNSScorer(CorpusBasedTermScorer):
     def _set_scorer_args(self, **kwargs):
         self.alpha = kwargs.get('alpha', BNS_ALPHA_DEFAULT)
+        if self.alpha is None:
+            self.alpha = 1. / pd.Series(self.corpus_.get_category_ids()).value_counts().min()
         assert 0 <= self.alpha <= 1
 
     def get_score_df(self):
         data = {}
         X = self._get_X() > 0
-        y = self.corpus_._y
+        y = self.corpus_.get_category_ids()
         for cat_i, cat in enumerate(self.corpus_.get_categories()):
             n_cat_is = [x for x in range(len(self.corpus_.get_categories())) if x != cat_i]
-            bns_scores = self._get_bns_score_for_category_index(cat_i, n_cat_is, X, y)
-            data[cat] = bns_scores
+            tp, fp, pos, neg, tpr, fpr, invn_tpr, invn_fpr = self._get_bns_score_for_category_index(cat_i, n_cat_is, X, y)
+            data[cat + ' BNS'] = invn_tpr - invn_fpr
+            data[cat + ' TP'] = tp
+            data[cat + ' FP'] = fp
+            data[cat + ' POS'] = pos
+            data[cat + ' NEG'] = neg
+            data[cat + ' TPR'] = tpr
+            data[cat + ' FPR'] = fpr
+            data[cat + ' INTPR'] = invn_tpr
+            data[cat + ' INFPR'] = invn_fpr
         return pd.DataFrame(data, index=self._get_index())
 
     def _get_bns_score_for_category_index(self, cat_i, not_cat_is, X, y):
         cat_mask = y == cat_i
         not_cat_mask = np.logical_or.reduce([y == i for i in not_cat_is])
-        invn_tpr = self._invnorm(X[cat_mask].sum(axis=0).A1/np.sum(cat_mask))
-        invn_fpr = self._invnorm(X[not_cat_mask].sum(axis=0).A1/np.sum(not_cat_mask))
-        return invn_tpr - invn_fpr
+        tp = X[cat_mask].sum(axis=0).A1
+        fp = X[not_cat_mask].sum(axis=0).A1
+        pos = np.sum(cat_mask)
+        neg = np.sum(not_cat_mask)
+        tpr = tp/pos
+        fpr = fp/neg
+        invn_tpr = self._invnorm(tpr)
+        invn_fpr = self._invnorm(fpr)
+        return tp, fp, pos, neg, tpr, fpr, invn_tpr, invn_fpr
 
     def _invnorm(self, scores: np.array) -> np.array:
         scores[scores < self.alpha] = self.alpha
         scores[scores > 1 - self.alpha] = 1 - self.alpha
         return norm.ppf(scores)
 
     def get_scores(self, *args) -> pd.Series:
+        tp, fp, pos, neg, tpr, fpr, invn_tpr, invn_fpr = self._get_bns_score_for_category_index(
+            cat_i=self.corpus_.get_categories().index(self.category_name),
+            not_cat_is=[self.corpus_.get_categories().index(c) for c in self.not_category_names],
+            X=self._get_X() > 0,
+            y=self.corpus_._y
+        )
         return pd.Series(
-            self._get_bns_score_for_category_index(
-                cat_i=self.corpus_.get_categories().index(self.category_name),
-                not_cat_is=[self.corpus_.get_categories().index(c) for c in self.not_category_names],
-                X=self._get_X() > 0,
-                y=self.corpus_._y
-            ),
+            invn_tpr - invn_fpr,
             index=self._get_index()
         )
 
     def get_name(self):
         return f"Bi-normal separation (alpha={self.alpha})"
```

### Comparing `scattertext-0.1.8/scattertext/termscoring/LogOddsRatio.py` & `scattertext-0.1.9/scattertext/termscoring/LogOddsRatio.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/test_credTFIDF.py` & `scattertext-0.1.9/scattertext/termscoring/test_credTFIDF.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/ScaledFScore.py` & `scattertext-0.1.9/scattertext/termscoring/ScaledFScore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termscoring/CraigsZeta.py` & `scattertext-0.1.9/scattertext/termscoring/CraigsZeta.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CLI.py` & `scattertext-0.1.9/scattertext/CLI.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/Common.py` & `scattertext-0.1.9/scattertext/Common.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/AutoTermSelector.py` & `scattertext-0.1.9/scattertext/AutoTermSelector.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusFromFeatureDict.py` & `scattertext-0.1.9/scattertext/CorpusFromFeatureDict.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/AsianNLP.py` & `scattertext-0.1.9/scattertext/AsianNLP.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/ScatterChartData.py` & `scattertext-0.1.9/scattertext/ScatterChartData.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/dispersion/Dispersion.py` & `scattertext-0.1.9/scattertext/dispersion/Dispersion.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/ScatterChartExplorer.py` & `scattertext-0.1.9/scattertext/ScatterChartExplorer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/ParsedCorpus.py` & `scattertext-0.1.9/scattertext/ParsedCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/graphs/GraphStructure.py` & `scattertext-0.1.9/scattertext/graphs/GraphStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/graphs/SimpleDiGraph.py` & `scattertext-0.1.9/scattertext/graphs/SimpleDiGraph.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/graphs/ComponentDiGraph.py` & `scattertext-0.1.9/scattertext/graphs/ComponentDiGraph.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/graphs/ComponentDiGraphHTMLRenderer.py` & `scattertext-0.1.9/scattertext/graphs/ComponentDiGraphHTMLRenderer.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/external/phrasemachine/phrasemachine.py` & `scattertext-0.1.9/scattertext/external/phrasemachine/phrasemachine.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/emojis/EmojiExtractor.py` & `scattertext-0.1.9/scattertext/emojis/EmojiExtractor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/emojis/ProcessedEmojiStructure.py` & `scattertext-0.1.9/scattertext/emojis/ProcessedEmojiStructure.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/categorytable/__init__.py` & `scattertext-0.1.9/scattertext/categorytable/__init__.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/indexstore/IndexStore.py` & `scattertext-0.1.9/scattertext/indexstore/IndexStore.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusDF.py` & `scattertext-0.1.9/scattertext/CorpusDF.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusFromParsedDocuments.py` & `scattertext-0.1.9/scattertext/CorpusFromParsedDocuments.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/mfd2.0.csv` & `scattertext-0.1.9/scattertext/data/mfd2.0.csv`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/whissells_df.csv` & `scattertext-0.1.9/scattertext/data/whissells_df.csv`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/inqtabs.txt` & `scattertext-0.1.9/scattertext/data/inqtabs.txt`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/political_data.csv` & `scattertext-0.1.9/scattertext/data/political_data.csv`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/rotten_tomatoes_corpus.csv.bz2` & `scattertext-0.1.9/scattertext/data/rotten_tomatoes_corpus.csv.bz2`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/arglex_Somasundaran07.json` & `scattertext-0.1.9/scattertext/data/arglex_Somasundaran07.json`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/count_1w.txt` & `scattertext-0.1.9/scattertext/data/count_1w.txt`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/political_data.json` & `scattertext-0.1.9/scattertext/data/political_data.json`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/punkt.english.pickle` & `scattertext-0.1.9/scattertext/data/punkt.english.pickle`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/count_2w.txt` & `scattertext-0.1.9/scattertext/data/count_2w.txt`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/rotten_tomatoes_corpus_full.csv.bz2` & `scattertext-0.1.9/scattertext/data/rotten_tomatoes_corpus_full.csv.bz2`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/pairplot_without_halo.html` & `scattertext-0.1.9/scattertext/data/viz/pairplot_without_halo.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/graph_plot.html` & `scattertext-0.1.9/scattertext/data/viz/graph_plot.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/semiotic_new.html` & `scattertext-0.1.9/scattertext/data/viz/semiotic_new.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/timeline.html` & `scattertext-0.1.9/scattertext/data/viz/timeline.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/autocomplete.css` & `scattertext-0.1.9/scattertext/data/viz/autocomplete.css`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/main_bk.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/main_bk.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/d3.min.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/d3.min.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/range-tree.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/range-tree.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/main.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/main.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/timelines-chart.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/timelines-chart.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/rectangle-holder.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/rectangle-holder.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/autocomplete_definition.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/autocomplete_definition.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scripts/d3-scale-chromatic.v1.min.js` & `scattertext-0.1.9/scattertext/data/viz/scripts/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/table_plot.html` & `scattertext-0.1.9/scattertext/data/viz/table_plot.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/pairplot.html` & `scattertext-0.1.9/scattertext/data/viz/pairplot.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/semiotic.html` & `scattertext-0.1.9/scattertext/data/viz/semiotic.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/time_plot.html` & `scattertext-0.1.9/scattertext/data/viz/time_plot.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/viz/scattertext.html` & `scattertext-0.1.9/scattertext/data/viz/scattertext.html`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/republican_convention_2016.csv` & `scattertext-0.1.9/scattertext/data/republican_convention_2016.csv`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/chinese.csv` & `scattertext-0.1.9/scattertext/data/chinese.csv`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/hamlet.txt` & `scattertext-0.1.9/scattertext/data/hamlet.txt`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/data/presidential_debates_2016.csv.gz` & `scattertext-0.1.9/scattertext/data/presidential_debates_2016.csv.gz`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/domain/CombineDocsIntoDomains.py` & `scattertext-0.1.9/scattertext/domain/CombineDocsIntoDomains.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/continuous/sklearnpipeline.py` & `scattertext-0.1.9/scattertext/continuous/sklearnpipeline.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/continuous/ungar.py` & `scattertext-0.1.9/scattertext/continuous/ungar.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/DataFrameCorpus.py` & `scattertext-0.1.9/scattertext/DataFrameCorpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioInformativeDirichletPiror.py` & `scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioInformativeDirichletPiror.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioUninformativeDirichletPrior.py` & `scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioUninformativeDirichletPrior.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termsignificance/LogOddsRatioSmoothed.py` & `scattertext-0.1.9/scattertext/termsignificance/LogOddsRatioSmoothed.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termsignificance/ScaledFScoreSignificance.py` & `scattertext-0.1.9/scattertext/termsignificance/ScaledFScoreSignificance.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusFromPandas.py` & `scattertext-0.1.9/scattertext/CorpusFromPandas.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/TermDocMatrixFilter.py` & `scattertext-0.1.9/scattertext/TermDocMatrixFilter.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/ClassPercentageCompactor.py` & `scattertext-0.1.9/scattertext/termcompaction/ClassPercentageCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/AssociationCompactor.py` & `scattertext-0.1.9/scattertext/termcompaction/AssociationCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/CompactTerms.py` & `scattertext-0.1.9/scattertext/termcompaction/CompactTerms.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/DomainCompactor.py` & `scattertext-0.1.9/scattertext/termcompaction/DomainCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/ScikitCompactor.py` & `scattertext-0.1.9/scattertext/termcompaction/ScikitCompactor.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/termcompaction/PhraseSelector.py` & `scattertext-0.1.9/scattertext/termcompaction/PhraseSelector.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/CorpusWithoutCategoriesFromParsedDocuments.py` & `scattertext-0.1.9/scattertext/CorpusWithoutCategoriesFromParsedDocuments.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/scattertext/Corpus.py` & `scattertext-0.1.9/scattertext/Corpus.py`

 * *Files identical despite different names*

### Comparing `scattertext-0.1.8/README.md` & `scattertext-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Build Status](https://travis-ci.org/JasonKessler/scattertext.svg?branch=master)](https://travis-ci.org/JasonKessler/scattertext)
 [![PyPI](https://img.shields.io/pypi/v/scattertext.svg)]()
 [![Gitter Chat](https://img.shields.io/badge/GITTER-join%20chat-green.svg)](https://gitter.im/scattertext/Lobby)
 [![Twitter Follow](https://img.shields.io/twitter/follow/espadrine.svg?style=social&label=Follow)](https://twitter.com/jasonkessler)
 
-# Scattertext 0.1.8
+# Scattertext 0.1.9
 
 A tool for finding distinguishing terms in corpora and displaying them in an 
 interactive HTML scatter plot. Points corresponding to terms are selectively labeled
 so that they don't overlap with other labels or points. 
 
 Below is an example of using Scattertext to create visualize terms used in 2012 American
 political conventions.  The 2,000 most party-associated unigrams are displayed as 
@@ -957,46 +957,121 @@
 ```  
 Click for an interactive version. 
 [![demo_cohens_d.html](https://jasonkessler.github.io/cohen_d.png)](https://jasonkessler.github.io/demo_cohens_d.html)
  
 
 ### Using Bi-Normal Separation (BNS) to score terms
 
-New in 0.1.8 is Bi-Normal Separation (BNS) (Forman, 2008). A variation of (BNS) is used 
-where $F^{-1}(tpr) - F^{-1}(fpr)$ is not used as an absolute value, but kept as a difference. 
+Bi-Normal Separation (BNS) (Forman, 2008) was added in version 0.1.8. A variation of (BNS) is used 
+where $F^{-1}(tpr) - F^{-1}(fpr)$ is not used as an absolute value, but kept as a difference. This allows for 
+terms strongly indicative of true positives and false positives to have a high or low score.
 Note that tpr and fpr are scaled to between $[\alpha, 1-\alpha]$ where 
-alpha is $\in [0, 1]$ and defaults to 0.005. While Forman (2008) suggests using $\alpha=0.0005$,
-I've found that value tends to over-emphasize very low and very high frequency terms.  Using the 
-Convention corpus, the `BNSScorer` can be just like any other term scorer.
+alpha is $\in [0, 1]$. In Forman (2008) and earlier literature $\alpha=0.0005$. In personal correspondence with Forman, 
+he kindly suggested using $\frac{1.}{\mbox{minimum(# positives, # negatives)}$. I have implemented this as
+$\alpha=\frac{1.}{\mbox{minimum(# documents in least frequent category)}$
 
 ```python
-term_scorer = (st.BNSScorer(corpus, alpha=0.005).set_categories('democrat'))
+corpus = (st.CorpusFromPandas(convention_df,
+                              category_col='party',
+                              text_col='text',
+                              nlp=st.whitespace_nlp_with_sentences)
+          .build()
+          .get_unigram_corpus()
+          .remove_infrequent_words(3, term_ranker=st.OncePerDocFrequencyRanker))
+
+term_scorer = (st.BNSScorer(corpus).set_categories('democrat'))
+print(term_scorer.get_score_df().sort_values(by='democrat BNS'))
 
 html = st.produce_frequency_explorer(
     corpus,
     category='democrat',
     category_name='Democratic',
     not_category_name='Republican',
-    term_scorer=term_scorer,
+    scores=term_scorer.get_score_df()['democrat BNS'].reindex(corpus.get_terms()).values,
     metadata=lambda c: c.get_df()['speaker'],
-    grey_threshold=0
+    minimum_term_frequency=0,
+    grey_threshold=0,
+    y_label=f'Bi-normal Separation (alpha={term_scorer.alpha})'
 )
 ```
 
-BNS Scored terms at $\alpha=0.005$:
+BNS Scored terms using an algorithmically found alpha.
 [![BNS](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/demo_bi_normal_separation.png)](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/demo_bi_normal_separation.html)
 
-Note that when using $\alpha=0.0005$, as recommended by Forman, low frequency terms such 
-as "achievement" and as well as the high frequency stopwords such as "is", "that" and "a" 
-top the Republican list.
-[![BNS](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/demo_bi_normal_separation_0.0005.png)](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/demo_bi_normal_separation_0.0005.html)
+### Using correlations to explain classifiers
+
+We can train a classifier to produce a prediction score for each document. Often classifiers or regressors
+use features which take into account features beyond the ones represented by Scatterext, be they n-gram, topic, 
+extra-linguistic, neural, etc.  
 
+We can use Scattertext to visualize the correlations between unigrams (or really any feature representation) and
+the document scores produced by a model.
+
+In the following example, we train a linear SVM using unigram and bi-gram features on the entire convention data set,
+and use the model to make a prediction on each document, and finally using Pearson's $r$ to correlate unigram features
+to the distance from the SVM decision boundary.
+
+```python
+from sklearn.svm import LinearSVC
+
+import scattertext as st
+
+df = st.SampleCorpora.ConventionData2012.get_data().assign(
+    parse=lambda df: df.text.apply(st.whitespace_nlp_with_sentences)
+)
+
+corpus = st.CorpusFromParsedDocuments(
+    df, category_col='party', parsed_col='parse'
+).build()
+
+X = corpus.get_term_doc_mat()
+y = corpus.get_category_ids()
+
+clf = LinearSVC()
+clf.fit(X=X, y=y==corpus.get_categories().index('democrat'))
+doc_scores = clf.decision_function(X=X)
+
+compactcorpus = corpus.get_unigram_corpus().compact(st.AssociationCompactor(2000))
+
+plot_df = st.Correlations().set_correlation_type(
+    'pearsonr'
+).get_correlation_df(
+    corpus=compactcorpus,
+    document_scores=doc_scores
+).reindex(compactcorpus.get_terms()).assign(
+    X=lambda df: df.Frequency,
+    Y=lambda df: df['r'],
+    Xpos=lambda df: st.Scalers.dense_rank(df.X),
+    Ypos=lambda df: st.Scalers.scale_center_zero_abs(df.Y),
+    SuppressDisplay=False,
+    ColorScore=lambda df: df.Ypos,
+)
+
+html = st.dataframe_scattertext(
+    compactcorpus,
+    plot_df=plot_df,
+    category='democrat',
+    category_name='Democratic',
+    not_category_name='Republican',
+    width_in_pixels=1000,
+    metadata=lambda c: c.get_df()['speaker'],
+    unified_context=False,
+    ignore_categories=False,
+    color_score_column='ColorScore',
+    left_list_column='ColorScore',
+    y_label="Pearson r (correlation to SVM document score)",
+    x_label='Frequency Ranks',
+    header_names={'upper': 'Top Democratic',
+                  'lower': 'Top Republican'},
+)
+```
+[![BNS](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/pearsons.png)](https://raw.githubusercontent.com/JasonKessler/jasonkessler.github.io/master/pearsons.html)
 
 
-### Using Custom Background Word Frequences
+### Using Custom Background Word Frequencies
 
 Scattertext relies on a set of general-domain English word frequencies when computing unigram characteristic  
 scores. When using running Scattertext on non-English data or in a specific domain, the quality of the scores
 will degrade.
 
 Ensure that you are on Scattertext 0.1.6 or higher.
 
@@ -2450,15 +2525,15 @@
 Click for an interactive visualization.  
 [![pca](https://jasonkessler.github.io/svd2.png)](https://jasonkessler.github.io/demo_embeddings_svd_0_1_scale_neg_1_to_1_with_zero_mean.html)
 
 ### Exporting plot to matplotlib
 
 To export the content of a scattertext explorer object (ScattertextStructure) to matplotlib you can use `produce_scattertext_pyplot`. The function returns a `matplotlib.figure.Figure` object which can be visualized using `plt.show` or `plt.savefig` as in the example below.
 
-Note that installation of textalloc==0.0.2 and matplotlib>=3.6.0 is required before running this.   
+Note that installation of textalloc==0.0.3 and matplotlib>=3.6.0 is required before running this.   
 
 ```pydocstring
 convention_df = st.SampleCorpora.ConventionData2012.get_data().assign(
 	parse = lambda df: df.text.apply(st.whitespace_nlp_with_sentences)
 )
 corpus = st.CorpusFromParsedDocuments(convention_df, category_col='party', parsed_col='parse').build()
 scattertext_structure = st.produce_scattertext_explorer(
```

### Comparing `scattertext-0.1.8/setup.py` & `scattertext-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='scattertext',
-      version='0.1.8',
+      version='0.1.9',
       description='An NLP package to visualize interesting terms in text.',
       url='https://github.com/JasonKessler/scattertext',
       author='Jason Kessler',
       author_email='jason.kessler@gmail.com',
       license='Apache 2.0',
       packages=find_packages(),
       install_requires=[
```

