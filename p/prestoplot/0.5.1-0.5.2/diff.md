# Comparing `tmp/prestoplot-0.5.1.tar.gz` & `tmp/prestoplot-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prestoplot-0.5.1.tar", last modified: Tue May 10 18:58:31 2022, max compression
+gzip compressed data, was "prestoplot-0.5.2.tar", last modified: Tue Apr 18 19:23:12 2023, max compression
```

## Comparing `prestoplot-0.5.1.tar` & `prestoplot-0.5.2.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.221386 prestoplot-0.5.1/
--rw-r--r--   0 eykd       (502) staff       (20)       46 2019-12-07 18:58:42.000000 prestoplot-0.5.1/.coverall.yml
--rw-r--r--   0 eykd       (502) staff       (20)      190 2019-11-21 14:43:16.000000 prestoplot-0.5.1/.isort.cfg
--rw-r--r--   0 eykd       (502) staff       (20)      290 2022-05-06 23:24:31.000000 prestoplot-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 eykd       (502) staff       (20)       27 2019-12-07 16:08:07.000000 prestoplot-0.5.1/AUTHORS
--rw-r--r--   0 eykd       (502) staff       (20)     1454 2019-02-07 15:20:17.000000 prestoplot-0.5.1/LICENSE
--rw-r--r--   0 eykd       (502) staff       (20)       57 2022-05-09 04:03:36.000000 prestoplot-0.5.1/MANIFEST.in
--rw-r--r--   0 eykd       (502) staff       (20)    11283 2022-05-10 18:58:31.221534 prestoplot-0.5.1/PKG-INFO
--rw-r--r--   0 eykd       (502) staff       (20)     6406 2022-05-10 18:58:13.000000 prestoplot-0.5.1/README.rst
--rw-r--r--   0 eykd       (502) staff       (20)       85 2022-05-09 05:16:37.000000 prestoplot-0.5.1/pyproject.toml
--rw-r--r--   0 eykd       (502) staff       (20)      113 2022-05-10 18:13:41.000000 prestoplot-0.5.1/requirements-dev.txt
--rw-r--r--   0 eykd       (502) staff       (20)      203 2022-05-10 18:50:51.000000 prestoplot-0.5.1/requirements-test.txt
--rw-r--r--   0 eykd       (502) staff       (20)        5 2022-05-10 18:13:33.000000 prestoplot-0.5.1/requirements.txt
--rwxr--r--   0 eykd       (502) staff       (20)      131 2019-11-21 02:46:25.000000 prestoplot-0.5.1/runtests.sh
--rw-r--r--   0 eykd       (502) staff       (20)     1593 2022-05-10 18:58:31.222069 prestoplot-0.5.1/setup.cfg
--rw-r--r--   0 eykd       (502) staff       (20)      208 2022-05-09 05:18:36.000000 prestoplot-0.5.1/setup.py
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.206696 prestoplot-0.5.1/src/
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.222215 prestoplot-0.5.1/src/prestoplot/
--rw-r--r--   0 eykd       (502) staff       (20)       73 2022-05-09 04:03:57.000000 prestoplot-0.5.1/src/prestoplot/__init__.py
--rw-r--r--   0 eykd       (502) staff       (20)      497 2022-05-10 18:58:31.222244 prestoplot-0.5.1/src/prestoplot/_version.py
--rw-r--r--   0 eykd       (502) staff       (20)     2441 2022-05-06 23:23:36.000000 prestoplot-0.5.1/src/prestoplot/cli.py
--rw-r--r--   0 eykd       (502) staff       (20)      329 2022-05-10 17:52:00.000000 prestoplot-0.5.1/src/prestoplot/contexts.py
--rw-r--r--   0 eykd       (502) staff       (20)     3117 2022-05-09 06:09:08.000000 prestoplot-0.5.1/src/prestoplot/db.py
--rw-r--r--   0 eykd       (502) staff       (20)     3815 2019-11-24 06:59:47.000000 prestoplot-0.5.1/src/prestoplot/grammars.py
--rw-r--r--   0 eykd       (502) staff       (20)     2532 2022-05-09 06:08:40.000000 prestoplot-0.5.1/src/prestoplot/markov.py
--rw-r--r--   0 eykd       (502) staff       (20)      843 2022-05-10 17:52:00.000000 prestoplot-0.5.1/src/prestoplot/seeds.py
--rw-r--r--   0 eykd       (502) staff       (20)     1903 2019-11-21 02:47:23.000000 prestoplot-0.5.1/src/prestoplot/storages.py
--rw-r--r--   0 eykd       (502) staff       (20)      305 2022-05-10 17:52:17.000000 prestoplot-0.5.1/src/prestoplot/story.py
--rw-r--r--   0 eykd       (502) staff       (20)     3216 2019-10-23 13:46:18.000000 prestoplot-0.5.1/src/prestoplot/texts.py
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.219581 prestoplot-0.5.1/src/prestoplot.egg-info/
--rw-r--r--   0 eykd       (502) staff       (20)    11283 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/PKG-INFO
--rw-r--r--   0 eykd       (502) staff       (20)      955 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/SOURCES.txt
--rw-r--r--   0 eykd       (502) staff       (20)        1 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/dependency_links.txt
--rw-r--r--   0 eykd       (502) staff       (20)       48 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/entry_points.txt
--rw-r--r--   0 eykd       (502) staff       (20)       47 2022-05-06 23:13:17.000000 prestoplot-0.5.1/src/prestoplot.egg-info/pbr.json
--rw-r--r--   0 eykd       (502) staff       (20)       66 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/requires.txt
--rw-r--r--   0 eykd       (502) staff       (20)       11 2022-05-10 18:58:31.000000 prestoplot-0.5.1/src/prestoplot.egg-info/top_level.txt
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.220283 prestoplot-0.5.1/tests/
-drwxr-xr-x   0 eykd       (502) staff       (20)        0 2022-05-10 18:58:31.221151 prestoplot-0.5.1/tests/data/
--rw-r--r--   0 eykd       (502) staff       (20)     1221 2022-05-09 05:50:00.000000 prestoplot-0.5.1/tests/data/characters.yaml
--rw-r--r--   0 eykd       (502) staff       (20)     1303 2019-07-03 16:46:47.000000 prestoplot-0.5.1/tests/data/characters_jinja.yaml
--rw-r--r--   0 eykd       (502) staff       (20)      605 2022-05-10 17:51:30.000000 prestoplot-0.5.1/tests/data/names.mp
--rw-r--r--   0 eykd       (502) staff       (20)     1096 2022-05-10 17:51:30.000000 prestoplot-0.5.1/tests/data/names.yaml
--rw-r--r--   0 eykd       (502) staff       (20)        0 2019-02-08 03:52:11.000000 prestoplot-0.5.1/tests/test_grammars.py
--rw-r--r--   0 eykd       (502) staff       (20)      982 2019-11-21 14:44:09.000000 prestoplot-0.5.1/tests/test_storages.py
--rw-r--r--   0 eykd       (502) staff       (20)     1681 2022-05-10 17:52:00.000000 prestoplot-0.5.1/tests/test_story.py
--rw-r--r--   0 eykd       (502) staff       (20)      697 2019-10-14 18:36:54.000000 prestoplot-0.5.1/tests/test_texts.py
--rw-r--r--   0 eykd       (502) staff       (20)      373 2022-05-09 05:23:03.000000 prestoplot-0.5.1/tox.ini
--rw-r--r--   0 eykd       (502) staff       (20)    81180 2022-05-09 05:16:52.000000 prestoplot-0.5.1/versioneer.py
--rwxr--r--   0 eykd       (502) staff       (20)      143 2019-02-08 20:12:48.000000 prestoplot-0.5.1/watchtests.sh
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.022648 prestoplot-0.5.2/
+-rw-r--r--   0 eykd       (502) staff       (20)       46 2019-12-07 18:58:42.000000 prestoplot-0.5.2/.coverall.yml
+-rw-r--r--   0 eykd       (502) staff       (20)      190 2019-11-21 14:43:16.000000 prestoplot-0.5.2/.isort.cfg
+-rw-r--r--   0 eykd       (502) staff       (20)      290 2022-05-06 23:24:31.000000 prestoplot-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 eykd       (502) staff       (20)       27 2019-12-07 16:08:07.000000 prestoplot-0.5.2/AUTHORS
+-rw-r--r--   0 eykd       (502) staff       (20)     1821 2022-05-10 17:58:35.000000 prestoplot-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 eykd       (502) staff       (20)     1454 2019-02-07 15:20:17.000000 prestoplot-0.5.2/LICENSE
+-rw-r--r--   0 eykd       (502) staff       (20)       57 2022-05-09 04:03:36.000000 prestoplot-0.5.2/MANIFEST.in
+-rw-r--r--   0 eykd       (502) staff       (20)     8968 2023-04-18 19:23:12.022727 prestoplot-0.5.2/PKG-INFO
+-rw-r--r--   0 eykd       (502) staff       (20)     6406 2022-05-10 18:58:13.000000 prestoplot-0.5.2/README.rst
+-rw-r--r--   0 eykd       (502) staff       (20)       85 2022-05-09 05:16:37.000000 prestoplot-0.5.2/pyproject.toml
+-rw-r--r--   0 eykd       (502) staff       (20)       76 2023-04-18 19:15:54.000000 prestoplot-0.5.2/requirements-dev.txt
+-rw-r--r--   0 eykd       (502) staff       (20)      203 2022-05-10 18:50:51.000000 prestoplot-0.5.2/requirements-test.txt
+-rw-r--r--   0 eykd       (502) staff       (20)        5 2022-05-10 18:13:33.000000 prestoplot-0.5.2/requirements.txt
+-rwxr--r--   0 eykd       (502) staff       (20)      131 2019-11-21 02:46:25.000000 prestoplot-0.5.2/runtests.sh
+-rw-r--r--   0 eykd       (502) staff       (20)     1571 2023-04-18 19:23:12.023240 prestoplot-0.5.2/setup.cfg
+-rw-r--r--   0 eykd       (502) staff       (20)      208 2022-05-09 05:18:36.000000 prestoplot-0.5.2/setup.py
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.014770 prestoplot-0.5.2/src/
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.023376 prestoplot-0.5.2/src/prestoplot/
+-rw-r--r--   0 eykd       (502) staff       (20)       73 2022-05-09 04:03:57.000000 prestoplot-0.5.2/src/prestoplot/__init__.py
+-rw-r--r--   0 eykd       (502) staff       (20)      497 2023-04-18 19:23:12.023408 prestoplot-0.5.2/src/prestoplot/_version.py
+-rw-r--r--   0 eykd       (502) staff       (20)     4074 2023-04-18 19:15:54.000000 prestoplot-0.5.2/src/prestoplot/cli.py
+-rw-r--r--   0 eykd       (502) staff       (20)      329 2022-05-10 17:52:00.000000 prestoplot-0.5.2/src/prestoplot/contexts.py
+-rw-r--r--   0 eykd       (502) staff       (20)     3117 2022-05-09 06:09:08.000000 prestoplot-0.5.2/src/prestoplot/db.py
+-rw-r--r--   0 eykd       (502) staff       (20)     3815 2019-11-24 06:59:47.000000 prestoplot-0.5.2/src/prestoplot/grammars.py
+-rw-r--r--   0 eykd       (502) staff       (20)     1587 2023-04-18 19:15:54.000000 prestoplot-0.5.2/src/prestoplot/http.py
+-rw-r--r--   0 eykd       (502) staff       (20)     2532 2022-05-09 06:08:40.000000 prestoplot-0.5.2/src/prestoplot/markov.py
+-rw-r--r--   0 eykd       (502) staff       (20)      843 2022-05-10 17:52:00.000000 prestoplot-0.5.2/src/prestoplot/seeds.py
+-rw-r--r--   0 eykd       (502) staff       (20)     1903 2019-11-21 02:47:23.000000 prestoplot-0.5.2/src/prestoplot/storages.py
+-rw-r--r--   0 eykd       (502) staff       (20)      305 2022-05-10 17:52:17.000000 prestoplot-0.5.2/src/prestoplot/story.py
+-rw-r--r--   0 eykd       (502) staff       (20)     3216 2019-10-23 13:46:18.000000 prestoplot-0.5.2/src/prestoplot/texts.py
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.020872 prestoplot-0.5.2/src/prestoplot.egg-info/
+-rw-r--r--   0 eykd       (502) staff       (20)     8968 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/PKG-INFO
+-rw-r--r--   0 eykd       (502) staff       (20)     1013 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/SOURCES.txt
+-rw-r--r--   0 eykd       (502) staff       (20)        1 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/dependency_links.txt
+-rw-r--r--   0 eykd       (502) staff       (20)       47 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/entry_points.txt
+-rw-r--r--   0 eykd       (502) staff       (20)       47 2022-05-06 23:13:17.000000 prestoplot-0.5.2/src/prestoplot.egg-info/pbr.json
+-rw-r--r--   0 eykd       (502) staff       (20)       43 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/requires.txt
+-rw-r--r--   0 eykd       (502) staff       (20)       11 2023-04-18 19:23:11.000000 prestoplot-0.5.2/src/prestoplot.egg-info/top_level.txt
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.021821 prestoplot-0.5.2/tests/
+drwxr-xr-x   0 eykd       (502) staff       (20)        0 2023-04-18 19:23:12.022419 prestoplot-0.5.2/tests/data/
+-rw-r--r--   0 eykd       (502) staff       (20)     1221 2022-05-09 05:50:00.000000 prestoplot-0.5.2/tests/data/characters.yaml
+-rw-r--r--   0 eykd       (502) staff       (20)     1303 2019-07-03 16:46:47.000000 prestoplot-0.5.2/tests/data/characters_jinja.yaml
+-rw-r--r--   0 eykd       (502) staff       (20)      605 2022-05-10 17:51:30.000000 prestoplot-0.5.2/tests/data/names.mp
+-rw-r--r--   0 eykd       (502) staff       (20)     1096 2022-05-10 17:51:30.000000 prestoplot-0.5.2/tests/data/names.yaml
+-rw-r--r--   0 eykd       (502) staff       (20)        0 2019-02-08 03:52:11.000000 prestoplot-0.5.2/tests/test_grammars.py
+-rw-r--r--   0 eykd       (502) staff       (20)     1165 2022-05-10 17:51:26.000000 prestoplot-0.5.2/tests/test_markov.py
+-rw-r--r--   0 eykd       (502) staff       (20)      982 2019-11-21 14:44:09.000000 prestoplot-0.5.2/tests/test_storages.py
+-rw-r--r--   0 eykd       (502) staff       (20)     1681 2022-05-10 17:52:00.000000 prestoplot-0.5.2/tests/test_story.py
+-rw-r--r--   0 eykd       (502) staff       (20)      697 2019-10-14 18:36:54.000000 prestoplot-0.5.2/tests/test_texts.py
+-rw-r--r--   0 eykd       (502) staff       (20)      373 2022-05-09 05:23:03.000000 prestoplot-0.5.2/tox.ini
+-rw-r--r--   0 eykd       (502) staff       (20)    81180 2022-05-09 05:16:52.000000 prestoplot-0.5.2/versioneer.py
+-rwxr--r--   0 eykd       (502) staff       (20)      143 2019-02-08 20:12:48.000000 prestoplot-0.5.2/watchtests.sh
```

### Comparing `prestoplot-0.5.1/LICENSE` & `prestoplot-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/PKG-INFO` & `prestoplot-0.5.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,311 +1,312 @@
 Metadata-Version: 2.1
 Name: prestoplot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generative grammars for idea generation.
 Home-page: https://github.com/eykd/prestoplot
 Author: David Eyk
 Author-email: david@eykd.net
 License: MIT
 Project-URL: Bug Tracker, https://github.com/eykd/prestoplot/issues
 Project-URL: Source Code, https://github.com/eykd/prestoplot
-Description: PrestoPlot
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/prestoplot
-            :target: https://pypi.org/project/prestoplot/
-            :alt: PyPI version
-        
-        .. image:: https://github.com/eykd/prestoplot/workflows/Tests/badge.svg
-           :target: https://github.com/eykd/prestoplot/actions?query=workflow%3ATests
-           :alt: GitHub Actions - CI
-        
-        .. image:: https://coveralls.io/repos/github/eykd/prestoplot/badge.svg?branch=master
-            :target: https://coveralls.io/github/eykd/prestoplot?branch=master
-            :alt: Test coverage
-        
-        A library and tool for text generation, inspired by Tracery.
-        
-        PrestoPlot is a tool for idea generation, name generation, and other tomfoolery
-        when you should otherwise be writing.
-        
-        Goes best with the oracles from the `PrestoPlot Oracles repository`_.
-        
-        .. _PrestoPlot Oracles repository: https://github.com/eykd/prestoplot-oracles/
-        
-        Install
-        -------
-        
-        PrestoPlot is available from PyPI::
-        
-            pip install prestoplot
-        
-        Usage
-        -----
-        
-        PrestoPlot may be invoked with the ``presto`` CLI script::
-        
-            presto --help
-        
-        The "oracle" consulted directly must include a ``Begin:`` stanza::
-        
-            $ cat names.yaml
-            Begin:
-              - "{Name}"
-        
-            Name:
-              - George
-              - Martha
-        
-            $ presto run names.yaml
-            George
-        
-        
-        Generative Grammars
-        -------------------
-        
-        The main feature right now is a generative grammar that uses a simple YAML-based
-        language and `Python f-string syntax`_ to create `"oracles"`_ for idea generation.
-        
-        .. _"oracles": https://github.com/eykd/prestoplot-oracles/
-        .. _Python f-string syntax: https://realpython.com/python-f-strings/
-        
-        The best way to learn the grammar is to look at examples. We'll consider the
-        `YAML for generating a Pirate story`_, which begins like this::
-        
-          include:
-            - setup
-        
-          Begin:
-            - "{PiratesOracle}"
-        
-        .. _YAML for generating a Pirate story: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/pirates.yaml
-        
-        There is the ``Begin:`` stanza that we require to directly consult an oracle.
-        This contains a list of strings that may be chosen from by the random generator.
-        In this case, we have an f-string template that invokes ``PiratesOracle``. We
-        find that below::
-        
-          PiratesOracle:
-            - |
-              {Setup}
-              - {Letters.One}
-              - {Letters.Two}
-              - {Letters.Three}
-              - {Letters.Four}
-            - |
-              {Setup}
-              - {CutlassDagger.One}
-              - {CutlassDagger.Two}
-              - {CutlassDagger.Three}
-              - {CutlassDagger.Four}
-        
-        We see another list of strings. ``|`` followed by an indented new line means to
-        treat what follows at that indentation level as a literal string, instead of
-        YAML::
-        
-          {Setup}
-            - {Letters.One}
-            - {Letters.Two}
-            - {Letters.Three}
-            - {Letters.Four}
-        
-        So this is a string with a Markdown-style list, instead of a YAML list, all
-        because of the ``|``.
-        
-        So here we see ``Setup`` invoked, and then ``Letters`` invoked four times.
-        ``Letters`` is defined below::
-        
-          Letters:
-            - mode: pick
-            - "Betrayal and treachery!"
-            - "Captured {Nationality} charts, carefully copied, and used by the Royal Navy."
-            - "Dolphins, seen frolicking in the bow-wake of a ship, perhaps leading it toward its goal."
-            - "Flotsam and jetsam, washed ashore after a sea-battle."
-            - "Fo’c’sle gossip blaming the ship’s misfortunes on a crewman who killed an albatross."
-            - "Forged documents, implying that their bearer speaks for the Crown."
-            - "Hidden reefs, which at low tide endanger any ship that passes over them."
-        
-        We have another list, containing piratical thematic elements. ``mode: pick``
-        tells the generator to randomly pick from among them, then remove that option
-        from consideration for future picks. The normal mode is ``reuse`` which allows
-        list items to be re-used by the generator. Another mode, ``markov``, tells the
-        generator to build a Markov chain from the list, as with `these name lists`_.
-        
-        .. _these name lists: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/names-markov.yaml
-        
-        Going back to ``PiratesOracle``, we see that ``Letters`` is invoked four times,
-        each time with a new *key*. The values of the keys are important only to the
-        reader. Each new key acts as a fresh seed for the random generator when working
-        inside that stanza. For instance, if ``{Letters.One}`` picked the element
-        ``"Captured {Nationality} charts, carefully copied, and used by the Royal
-        Navy."``, the value ``One`` provides the seed for picking a ``Nationality``,
-        say, ``English``. Later, if ``{Letters.Two}`` encounters another element
-        containing ``{Nationality}``, the key ``Two`` will provide a different seed for
-        picking a nationality the second time.
-        
-        The plot thickens when we examine the ``include`` stanza, which includes the
-        ``setup.yaml`` file `next door`_. This file includes more files. We will next examine `characters.yaml`_.
-        
-        .. _next door: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/setup.yaml
-        .. _characters.yaml: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/characters.yaml
-        
-        Inside of ``characters.yaml`` we find this fascinating set of stanzas::
-        
-          Sex:
-            - male
-            - female
-        
-          He:
-            - >
-              {'She' if Sex[key] == 'female' else 'He'}
-          his:
-            - >
-              {'her' if Sex[key] == 'female' else 'his'}
-          His:
-            - >
-              {'Her' if Sex[key] == 'female' else 'His'}
-          hero:
-            - "{'heroine' if Sex[key] == 'female' else 'hero'}"
-        
-        
-        With this set of tools, we could write the following string::
-        
-          That {hero.protag}! {He.protag} sure loves {his.protag} mom.
-        
-        The long and short of it is that, depending on the sex of the protagonist, this
-        will render either::
-        
-          That heroine! She sure loves her mom.
-        
-        or::
-        
-          That hero! He sure loves his mom.
-        
-        So here we see that inside of f-string syntax, we can use pythonic expressions,
-        and the variable ``key`` contains the key from the outer scope: ``{He.protag}``
-        assigns the value ``"protag"`` to ``key``. ``{Sex[key]}`` will reliably produce
-        the same result for the same key (assuming the same initial seed).
-        
-        Everything else is just YAML syntax and Python f-string expressions.
-        
-        
-        About
-        -----
-        
-        I wrote PrestoPlot to support idea generation and name generation for my
-        pulp-inspired science fiction space opera series, `Salvage of Empire`_:
-        
-          When his brother-in-law threatens to reveal his terrible secret, Director Kolteo
-          Ais must sacrifice everything he has worked for to save the Galactic Empire—and
-          his marriage—from utter ruin.
-        
-        .. _Salvage of Empire: https://eykd.net/salvage/
-        
-        
-        CHANGES
-        =======
-        
-        0.5
-        ---
-        
-        * Allow instances of ``random.Random()`` as seeds.
-        * Rename ``ChangeLog`` to ``CHANGELOG.rst``, include in ``long_description``.
-        * Changelog is now manually written, instead of derived from git logs.
-        
-        0.4
-        ---
-        
-        * Fixed major instability of markov generator in the presence of a seed.
-        
-        
-        0.3.4
-        -----
-        
-        * Update packaging and requirements
-        
-        0.3.3
-        -----
-        
-        * Improved badge
-        * Update README w/ build status and better lede
-        * Update dev and test requirements
-        * Allow customization of start key when rendering story
-        * Add python 3.8 to tests
-        
-        0.3.2
-        -----
-        
-        * Remove more debug logging
-        
-        0.3.1
-        -----
-        
-        * Remove debug logging
-        * Add extra whitespace
-        * Add known third parties to isort cfg
-        * Add twine dev dependency
-        
-        0.3
-        ---
-        
-        * Add msgpack-compiled test data
-        * Add new more efficient storages
-        * Improve runtests invocation
-        * Tailor flake8 exclusions
-        * Pin versions; add msgpack
-        * Add some debug logging
-        * Add pyyaml requirement
-        * Revert "Use strictyaml instead of yaml"
-        * Add dev and test requirements
-        * Move prestplot package into src/
-        * Add Travis CI integration
-        * Add .isort.cfg
-        * Use collections.abc in prep for python 3.8
-        * Use strictyaml instead of yaml
-        * Add requirements.txt
-        * Use longer python environ specifiers for tox.ini
-        * Add project URLs
-        
-        0.2
-        ---
-        
-        * A whole bunch of refactoring
-        * Improve dev and test harness w/ dev requirements and test scripts
-        
-        0.1.3
-        -----
-        
-        * Add extended documentation on generative grammar syntax
-        * Further README improvements
-        
-        0.1.2
-        -----
-        
-        * Improve README
-        
-        0.1.1
-        -----
-        
-        * Add ``--seed`` option to CLI for pre-seeding oracles
-        * Add install/usage documentation to README
-        * Add documentation to CLI
-        
-        0.1
-        ---
-        
-        * Add basic test to exercise render\_story()
-        * Fix email, summary
-        * Remove future features from setup.cfg
-        * Finish writing README
-        * Fix link in README
-        * Initial commit
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+PrestoPlot
+==========
+
+.. image:: https://img.shields.io/pypi/v/prestoplot
+    :target: https://pypi.org/project/prestoplot/
+    :alt: PyPI version
+
+.. image:: https://github.com/eykd/prestoplot/workflows/Tests/badge.svg
+   :target: https://github.com/eykd/prestoplot/actions?query=workflow%3ATests
+   :alt: GitHub Actions - CI
+
+.. image:: https://coveralls.io/repos/github/eykd/prestoplot/badge.svg?branch=master
+    :target: https://coveralls.io/github/eykd/prestoplot?branch=master
+    :alt: Test coverage
+
+A library and tool for text generation, inspired by Tracery.
+
+PrestoPlot is a tool for idea generation, name generation, and other tomfoolery
+when you should otherwise be writing.
+
+Goes best with the oracles from the `PrestoPlot Oracles repository`_.
+
+.. _PrestoPlot Oracles repository: https://github.com/eykd/prestoplot-oracles/
+
+Install
+-------
+
+PrestoPlot is available from PyPI::
+
+    pip install prestoplot
+
+Usage
+-----
+
+PrestoPlot may be invoked with the ``presto`` CLI script::
+
+    presto --help
+
+The "oracle" consulted directly must include a ``Begin:`` stanza::
+
+    $ cat names.yaml
+    Begin:
+      - "{Name}"
+
+    Name:
+      - George
+      - Martha
+
+    $ presto run names.yaml
+    George
+
+
+Generative Grammars
+-------------------
+
+The main feature right now is a generative grammar that uses a simple YAML-based
+language and `Python f-string syntax`_ to create `"oracles"`_ for idea generation.
+
+.. _"oracles": https://github.com/eykd/prestoplot-oracles/
+.. _Python f-string syntax: https://realpython.com/python-f-strings/
+
+The best way to learn the grammar is to look at examples. We'll consider the
+`YAML for generating a Pirate story`_, which begins like this::
+
+  include:
+    - setup
+
+  Begin:
+    - "{PiratesOracle}"
+
+.. _YAML for generating a Pirate story: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/pirates.yaml
+
+There is the ``Begin:`` stanza that we require to directly consult an oracle.
+This contains a list of strings that may be chosen from by the random generator.
+In this case, we have an f-string template that invokes ``PiratesOracle``. We
+find that below::
+
+  PiratesOracle:
+    - |
+      {Setup}
+      - {Letters.One}
+      - {Letters.Two}
+      - {Letters.Three}
+      - {Letters.Four}
+    - |
+      {Setup}
+      - {CutlassDagger.One}
+      - {CutlassDagger.Two}
+      - {CutlassDagger.Three}
+      - {CutlassDagger.Four}
+
+We see another list of strings. ``|`` followed by an indented new line means to
+treat what follows at that indentation level as a literal string, instead of
+YAML::
+
+  {Setup}
+    - {Letters.One}
+    - {Letters.Two}
+    - {Letters.Three}
+    - {Letters.Four}
+
+So this is a string with a Markdown-style list, instead of a YAML list, all
+because of the ``|``.
+
+So here we see ``Setup`` invoked, and then ``Letters`` invoked four times.
+``Letters`` is defined below::
+
+  Letters:
+    - mode: pick
+    - "Betrayal and treachery!"
+    - "Captured {Nationality} charts, carefully copied, and used by the Royal Navy."
+    - "Dolphins, seen frolicking in the bow-wake of a ship, perhaps leading it toward its goal."
+    - "Flotsam and jetsam, washed ashore after a sea-battle."
+    - "Fo’c’sle gossip blaming the ship’s misfortunes on a crewman who killed an albatross."
+    - "Forged documents, implying that their bearer speaks for the Crown."
+    - "Hidden reefs, which at low tide endanger any ship that passes over them."
+
+We have another list, containing piratical thematic elements. ``mode: pick``
+tells the generator to randomly pick from among them, then remove that option
+from consideration for future picks. The normal mode is ``reuse`` which allows
+list items to be re-used by the generator. Another mode, ``markov``, tells the
+generator to build a Markov chain from the list, as with `these name lists`_.
+
+.. _these name lists: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/names-markov.yaml
+
+Going back to ``PiratesOracle``, we see that ``Letters`` is invoked four times,
+each time with a new *key*. The values of the keys are important only to the
+reader. Each new key acts as a fresh seed for the random generator when working
+inside that stanza. For instance, if ``{Letters.One}`` picked the element
+``"Captured {Nationality} charts, carefully copied, and used by the Royal
+Navy."``, the value ``One`` provides the seed for picking a ``Nationality``,
+say, ``English``. Later, if ``{Letters.Two}`` encounters another element
+containing ``{Nationality}``, the key ``Two`` will provide a different seed for
+picking a nationality the second time.
+
+The plot thickens when we examine the ``include`` stanza, which includes the
+``setup.yaml`` file `next door`_. This file includes more files. We will next examine `characters.yaml`_.
+
+.. _next door: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/setup.yaml
+.. _characters.yaml: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/characters.yaml
+
+Inside of ``characters.yaml`` we find this fascinating set of stanzas::
+
+  Sex:
+    - male
+    - female
+
+  He:
+    - >
+      {'She' if Sex[key] == 'female' else 'He'}
+  his:
+    - >
+      {'her' if Sex[key] == 'female' else 'his'}
+  His:
+    - >
+      {'Her' if Sex[key] == 'female' else 'His'}
+  hero:
+    - "{'heroine' if Sex[key] == 'female' else 'hero'}"
+
+
+With this set of tools, we could write the following string::
+
+  That {hero.protag}! {He.protag} sure loves {his.protag} mom.
+
+The long and short of it is that, depending on the sex of the protagonist, this
+will render either::
+
+  That heroine! She sure loves her mom.
+
+or::
+
+  That hero! He sure loves his mom.
+
+So here we see that inside of f-string syntax, we can use pythonic expressions,
+and the variable ``key`` contains the key from the outer scope: ``{He.protag}``
+assigns the value ``"protag"`` to ``key``. ``{Sex[key]}`` will reliably produce
+the same result for the same key (assuming the same initial seed).
+
+Everything else is just YAML syntax and Python f-string expressions.
+
+
+About
+-----
+
+I wrote PrestoPlot to support idea generation and name generation for my
+pulp-inspired science fiction space opera series, `Salvage of Empire`_:
+
+  When his brother-in-law threatens to reveal his terrible secret, Director Kolteo
+  Ais must sacrifice everything he has worked for to save the Galactic Empire—and
+  his marriage—from utter ruin.
+
+.. _Salvage of Empire: https://eykd.net/salvage/
+
+
+CHANGES
+=======
+
+0.5
+---
+
+* Allow instances of ``random.Random()`` as seeds.
+* Rename ``ChangeLog`` to ``CHANGELOG.rst``, include in ``long_description``.
+* Changelog is now manually written, instead of derived from git logs.
+
+0.4
+---
+
+* Fixed major instability of markov generator in the presence of a seed.
+
+
+0.3.4
+-----
+
+* Update packaging and requirements
+
+0.3.3
+-----
+
+* Improved badge
+* Update README w/ build status and better lede
+* Update dev and test requirements
+* Allow customization of start key when rendering story
+* Add python 3.8 to tests
+
+0.3.2
+-----
+
+* Remove more debug logging
+
+0.3.1
+-----
+
+* Remove debug logging
+* Add extra whitespace
+* Add known third parties to isort cfg
+* Add twine dev dependency
+
+0.3
+---
+
+* Add msgpack-compiled test data
+* Add new more efficient storages
+* Improve runtests invocation
+* Tailor flake8 exclusions
+* Pin versions; add msgpack
+* Add some debug logging
+* Add pyyaml requirement
+* Revert "Use strictyaml instead of yaml"
+* Add dev and test requirements
+* Move prestplot package into src/
+* Add Travis CI integration
+* Add .isort.cfg
+* Use collections.abc in prep for python 3.8
+* Use strictyaml instead of yaml
+* Add requirements.txt
+* Use longer python environ specifiers for tox.ini
+* Add project URLs
+
+0.2
+---
+
+* A whole bunch of refactoring
+* Improve dev and test harness w/ dev requirements and test scripts
+
+0.1.3
+-----
+
+* Add extended documentation on generative grammar syntax
+* Further README improvements
+
+0.1.2
+-----
+
+* Improve README
+
+0.1.1
+-----
+
+* Add ``--seed`` option to CLI for pre-seeding oracles
+* Add install/usage documentation to README
+* Add documentation to CLI
+
+0.1
+---
+
+* Add basic test to exercise render\_story()
+* Fix email, summary
+* Remove future features from setup.cfg
+* Finish writing README
+* Fix link in README
+* Initial commit
```

### Comparing `prestoplot-0.5.1/README.rst` & `prestoplot-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/setup.cfg` & `prestoplot-0.5.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -21,33 +21,34 @@
 	Source Code = https://github.com/eykd/prestoplot
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	msgpack==1.0.3
-	pyyaml==6.0
-	jinja2==3.1.2
-	funcy==1.17
-	click==8.1.3
+	msgpack
+	pyyaml
+	jinja2
+	funcy
+	click
+	Markdown
 
 [options.packages.find]
 where = src
 
 [files]
 packages = 
 	prestoplot
 
 [options.entry_points]
 console_scripts = 
 	presto = prestoplot.cli:main
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = src/prestoplot/_version.py
 versionfile_build = prestoplot/_version.py
 tag_prefix = 
 
 [flake8]
 exclude =
```

### Comparing `prestoplot-0.5.1/src/prestoplot/db.py` & `prestoplot-0.5.2/src/prestoplot/db.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot/grammars.py` & `prestoplot-0.5.2/src/prestoplot/grammars.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot/markov.py` & `prestoplot-0.5.2/src/prestoplot/markov.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot/seeds.py` & `prestoplot-0.5.2/src/prestoplot/seeds.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot/storages.py` & `prestoplot-0.5.2/src/prestoplot/storages.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot/texts.py` & `prestoplot-0.5.2/src/prestoplot/texts.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/src/prestoplot.egg-info/PKG-INFO` & `prestoplot-0.5.2/src/prestoplot.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,311 +1,312 @@
 Metadata-Version: 2.1
 Name: prestoplot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generative grammars for idea generation.
 Home-page: https://github.com/eykd/prestoplot
 Author: David Eyk
 Author-email: david@eykd.net
 License: MIT
 Project-URL: Bug Tracker, https://github.com/eykd/prestoplot/issues
 Project-URL: Source Code, https://github.com/eykd/prestoplot
-Description: PrestoPlot
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/prestoplot
-            :target: https://pypi.org/project/prestoplot/
-            :alt: PyPI version
-        
-        .. image:: https://github.com/eykd/prestoplot/workflows/Tests/badge.svg
-           :target: https://github.com/eykd/prestoplot/actions?query=workflow%3ATests
-           :alt: GitHub Actions - CI
-        
-        .. image:: https://coveralls.io/repos/github/eykd/prestoplot/badge.svg?branch=master
-            :target: https://coveralls.io/github/eykd/prestoplot?branch=master
-            :alt: Test coverage
-        
-        A library and tool for text generation, inspired by Tracery.
-        
-        PrestoPlot is a tool for idea generation, name generation, and other tomfoolery
-        when you should otherwise be writing.
-        
-        Goes best with the oracles from the `PrestoPlot Oracles repository`_.
-        
-        .. _PrestoPlot Oracles repository: https://github.com/eykd/prestoplot-oracles/
-        
-        Install
-        -------
-        
-        PrestoPlot is available from PyPI::
-        
-            pip install prestoplot
-        
-        Usage
-        -----
-        
-        PrestoPlot may be invoked with the ``presto`` CLI script::
-        
-            presto --help
-        
-        The "oracle" consulted directly must include a ``Begin:`` stanza::
-        
-            $ cat names.yaml
-            Begin:
-              - "{Name}"
-        
-            Name:
-              - George
-              - Martha
-        
-            $ presto run names.yaml
-            George
-        
-        
-        Generative Grammars
-        -------------------
-        
-        The main feature right now is a generative grammar that uses a simple YAML-based
-        language and `Python f-string syntax`_ to create `"oracles"`_ for idea generation.
-        
-        .. _"oracles": https://github.com/eykd/prestoplot-oracles/
-        .. _Python f-string syntax: https://realpython.com/python-f-strings/
-        
-        The best way to learn the grammar is to look at examples. We'll consider the
-        `YAML for generating a Pirate story`_, which begins like this::
-        
-          include:
-            - setup
-        
-          Begin:
-            - "{PiratesOracle}"
-        
-        .. _YAML for generating a Pirate story: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/pirates.yaml
-        
-        There is the ``Begin:`` stanza that we require to directly consult an oracle.
-        This contains a list of strings that may be chosen from by the random generator.
-        In this case, we have an f-string template that invokes ``PiratesOracle``. We
-        find that below::
-        
-          PiratesOracle:
-            - |
-              {Setup}
-              - {Letters.One}
-              - {Letters.Two}
-              - {Letters.Three}
-              - {Letters.Four}
-            - |
-              {Setup}
-              - {CutlassDagger.One}
-              - {CutlassDagger.Two}
-              - {CutlassDagger.Three}
-              - {CutlassDagger.Four}
-        
-        We see another list of strings. ``|`` followed by an indented new line means to
-        treat what follows at that indentation level as a literal string, instead of
-        YAML::
-        
-          {Setup}
-            - {Letters.One}
-            - {Letters.Two}
-            - {Letters.Three}
-            - {Letters.Four}
-        
-        So this is a string with a Markdown-style list, instead of a YAML list, all
-        because of the ``|``.
-        
-        So here we see ``Setup`` invoked, and then ``Letters`` invoked four times.
-        ``Letters`` is defined below::
-        
-          Letters:
-            - mode: pick
-            - "Betrayal and treachery!"
-            - "Captured {Nationality} charts, carefully copied, and used by the Royal Navy."
-            - "Dolphins, seen frolicking in the bow-wake of a ship, perhaps leading it toward its goal."
-            - "Flotsam and jetsam, washed ashore after a sea-battle."
-            - "Fo’c’sle gossip blaming the ship’s misfortunes on a crewman who killed an albatross."
-            - "Forged documents, implying that their bearer speaks for the Crown."
-            - "Hidden reefs, which at low tide endanger any ship that passes over them."
-        
-        We have another list, containing piratical thematic elements. ``mode: pick``
-        tells the generator to randomly pick from among them, then remove that option
-        from consideration for future picks. The normal mode is ``reuse`` which allows
-        list items to be re-used by the generator. Another mode, ``markov``, tells the
-        generator to build a Markov chain from the list, as with `these name lists`_.
-        
-        .. _these name lists: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/names-markov.yaml
-        
-        Going back to ``PiratesOracle``, we see that ``Letters`` is invoked four times,
-        each time with a new *key*. The values of the keys are important only to the
-        reader. Each new key acts as a fresh seed for the random generator when working
-        inside that stanza. For instance, if ``{Letters.One}`` picked the element
-        ``"Captured {Nationality} charts, carefully copied, and used by the Royal
-        Navy."``, the value ``One`` provides the seed for picking a ``Nationality``,
-        say, ``English``. Later, if ``{Letters.Two}`` encounters another element
-        containing ``{Nationality}``, the key ``Two`` will provide a different seed for
-        picking a nationality the second time.
-        
-        The plot thickens when we examine the ``include`` stanza, which includes the
-        ``setup.yaml`` file `next door`_. This file includes more files. We will next examine `characters.yaml`_.
-        
-        .. _next door: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/setup.yaml
-        .. _characters.yaml: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/characters.yaml
-        
-        Inside of ``characters.yaml`` we find this fascinating set of stanzas::
-        
-          Sex:
-            - male
-            - female
-        
-          He:
-            - >
-              {'She' if Sex[key] == 'female' else 'He'}
-          his:
-            - >
-              {'her' if Sex[key] == 'female' else 'his'}
-          His:
-            - >
-              {'Her' if Sex[key] == 'female' else 'His'}
-          hero:
-            - "{'heroine' if Sex[key] == 'female' else 'hero'}"
-        
-        
-        With this set of tools, we could write the following string::
-        
-          That {hero.protag}! {He.protag} sure loves {his.protag} mom.
-        
-        The long and short of it is that, depending on the sex of the protagonist, this
-        will render either::
-        
-          That heroine! She sure loves her mom.
-        
-        or::
-        
-          That hero! He sure loves his mom.
-        
-        So here we see that inside of f-string syntax, we can use pythonic expressions,
-        and the variable ``key`` contains the key from the outer scope: ``{He.protag}``
-        assigns the value ``"protag"`` to ``key``. ``{Sex[key]}`` will reliably produce
-        the same result for the same key (assuming the same initial seed).
-        
-        Everything else is just YAML syntax and Python f-string expressions.
-        
-        
-        About
-        -----
-        
-        I wrote PrestoPlot to support idea generation and name generation for my
-        pulp-inspired science fiction space opera series, `Salvage of Empire`_:
-        
-          When his brother-in-law threatens to reveal his terrible secret, Director Kolteo
-          Ais must sacrifice everything he has worked for to save the Galactic Empire—and
-          his marriage—from utter ruin.
-        
-        .. _Salvage of Empire: https://eykd.net/salvage/
-        
-        
-        CHANGES
-        =======
-        
-        0.5
-        ---
-        
-        * Allow instances of ``random.Random()`` as seeds.
-        * Rename ``ChangeLog`` to ``CHANGELOG.rst``, include in ``long_description``.
-        * Changelog is now manually written, instead of derived from git logs.
-        
-        0.4
-        ---
-        
-        * Fixed major instability of markov generator in the presence of a seed.
-        
-        
-        0.3.4
-        -----
-        
-        * Update packaging and requirements
-        
-        0.3.3
-        -----
-        
-        * Improved badge
-        * Update README w/ build status and better lede
-        * Update dev and test requirements
-        * Allow customization of start key when rendering story
-        * Add python 3.8 to tests
-        
-        0.3.2
-        -----
-        
-        * Remove more debug logging
-        
-        0.3.1
-        -----
-        
-        * Remove debug logging
-        * Add extra whitespace
-        * Add known third parties to isort cfg
-        * Add twine dev dependency
-        
-        0.3
-        ---
-        
-        * Add msgpack-compiled test data
-        * Add new more efficient storages
-        * Improve runtests invocation
-        * Tailor flake8 exclusions
-        * Pin versions; add msgpack
-        * Add some debug logging
-        * Add pyyaml requirement
-        * Revert "Use strictyaml instead of yaml"
-        * Add dev and test requirements
-        * Move prestplot package into src/
-        * Add Travis CI integration
-        * Add .isort.cfg
-        * Use collections.abc in prep for python 3.8
-        * Use strictyaml instead of yaml
-        * Add requirements.txt
-        * Use longer python environ specifiers for tox.ini
-        * Add project URLs
-        
-        0.2
-        ---
-        
-        * A whole bunch of refactoring
-        * Improve dev and test harness w/ dev requirements and test scripts
-        
-        0.1.3
-        -----
-        
-        * Add extended documentation on generative grammar syntax
-        * Further README improvements
-        
-        0.1.2
-        -----
-        
-        * Improve README
-        
-        0.1.1
-        -----
-        
-        * Add ``--seed`` option to CLI for pre-seeding oracles
-        * Add install/usage documentation to README
-        * Add documentation to CLI
-        
-        0.1
-        ---
-        
-        * Add basic test to exercise render\_story()
-        * Fix email, summary
-        * Remove future features from setup.cfg
-        * Finish writing README
-        * Fix link in README
-        * Initial commit
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+PrestoPlot
+==========
+
+.. image:: https://img.shields.io/pypi/v/prestoplot
+    :target: https://pypi.org/project/prestoplot/
+    :alt: PyPI version
+
+.. image:: https://github.com/eykd/prestoplot/workflows/Tests/badge.svg
+   :target: https://github.com/eykd/prestoplot/actions?query=workflow%3ATests
+   :alt: GitHub Actions - CI
+
+.. image:: https://coveralls.io/repos/github/eykd/prestoplot/badge.svg?branch=master
+    :target: https://coveralls.io/github/eykd/prestoplot?branch=master
+    :alt: Test coverage
+
+A library and tool for text generation, inspired by Tracery.
+
+PrestoPlot is a tool for idea generation, name generation, and other tomfoolery
+when you should otherwise be writing.
+
+Goes best with the oracles from the `PrestoPlot Oracles repository`_.
+
+.. _PrestoPlot Oracles repository: https://github.com/eykd/prestoplot-oracles/
+
+Install
+-------
+
+PrestoPlot is available from PyPI::
+
+    pip install prestoplot
+
+Usage
+-----
+
+PrestoPlot may be invoked with the ``presto`` CLI script::
+
+    presto --help
+
+The "oracle" consulted directly must include a ``Begin:`` stanza::
+
+    $ cat names.yaml
+    Begin:
+      - "{Name}"
+
+    Name:
+      - George
+      - Martha
+
+    $ presto run names.yaml
+    George
+
+
+Generative Grammars
+-------------------
+
+The main feature right now is a generative grammar that uses a simple YAML-based
+language and `Python f-string syntax`_ to create `"oracles"`_ for idea generation.
+
+.. _"oracles": https://github.com/eykd/prestoplot-oracles/
+.. _Python f-string syntax: https://realpython.com/python-f-strings/
+
+The best way to learn the grammar is to look at examples. We'll consider the
+`YAML for generating a Pirate story`_, which begins like this::
+
+  include:
+    - setup
+
+  Begin:
+    - "{PiratesOracle}"
+
+.. _YAML for generating a Pirate story: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/pirates.yaml
+
+There is the ``Begin:`` stanza that we require to directly consult an oracle.
+This contains a list of strings that may be chosen from by the random generator.
+In this case, we have an f-string template that invokes ``PiratesOracle``. We
+find that below::
+
+  PiratesOracle:
+    - |
+      {Setup}
+      - {Letters.One}
+      - {Letters.Two}
+      - {Letters.Three}
+      - {Letters.Four}
+    - |
+      {Setup}
+      - {CutlassDagger.One}
+      - {CutlassDagger.Two}
+      - {CutlassDagger.Three}
+      - {CutlassDagger.Four}
+
+We see another list of strings. ``|`` followed by an indented new line means to
+treat what follows at that indentation level as a literal string, instead of
+YAML::
+
+  {Setup}
+    - {Letters.One}
+    - {Letters.Two}
+    - {Letters.Three}
+    - {Letters.Four}
+
+So this is a string with a Markdown-style list, instead of a YAML list, all
+because of the ``|``.
+
+So here we see ``Setup`` invoked, and then ``Letters`` invoked four times.
+``Letters`` is defined below::
+
+  Letters:
+    - mode: pick
+    - "Betrayal and treachery!"
+    - "Captured {Nationality} charts, carefully copied, and used by the Royal Navy."
+    - "Dolphins, seen frolicking in the bow-wake of a ship, perhaps leading it toward its goal."
+    - "Flotsam and jetsam, washed ashore after a sea-battle."
+    - "Fo’c’sle gossip blaming the ship’s misfortunes on a crewman who killed an albatross."
+    - "Forged documents, implying that their bearer speaks for the Crown."
+    - "Hidden reefs, which at low tide endanger any ship that passes over them."
+
+We have another list, containing piratical thematic elements. ``mode: pick``
+tells the generator to randomly pick from among them, then remove that option
+from consideration for future picks. The normal mode is ``reuse`` which allows
+list items to be re-used by the generator. Another mode, ``markov``, tells the
+generator to build a Markov chain from the list, as with `these name lists`_.
+
+.. _these name lists: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/names-markov.yaml
+
+Going back to ``PiratesOracle``, we see that ``Letters`` is invoked four times,
+each time with a new *key*. The values of the keys are important only to the
+reader. Each new key acts as a fresh seed for the random generator when working
+inside that stanza. For instance, if ``{Letters.One}`` picked the element
+``"Captured {Nationality} charts, carefully copied, and used by the Royal
+Navy."``, the value ``One`` provides the seed for picking a ``Nationality``,
+say, ``English``. Later, if ``{Letters.Two}`` encounters another element
+containing ``{Nationality}``, the key ``Two`` will provide a different seed for
+picking a nationality the second time.
+
+The plot thickens when we examine the ``include`` stanza, which includes the
+``setup.yaml`` file `next door`_. This file includes more files. We will next examine `characters.yaml`_.
+
+.. _next door: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/setup.yaml
+.. _characters.yaml: https://github.com/eykd/prestoplot-oracles/blob/master/oracles/characters.yaml
+
+Inside of ``characters.yaml`` we find this fascinating set of stanzas::
+
+  Sex:
+    - male
+    - female
+
+  He:
+    - >
+      {'She' if Sex[key] == 'female' else 'He'}
+  his:
+    - >
+      {'her' if Sex[key] == 'female' else 'his'}
+  His:
+    - >
+      {'Her' if Sex[key] == 'female' else 'His'}
+  hero:
+    - "{'heroine' if Sex[key] == 'female' else 'hero'}"
+
+
+With this set of tools, we could write the following string::
+
+  That {hero.protag}! {He.protag} sure loves {his.protag} mom.
+
+The long and short of it is that, depending on the sex of the protagonist, this
+will render either::
+
+  That heroine! She sure loves her mom.
+
+or::
+
+  That hero! He sure loves his mom.
+
+So here we see that inside of f-string syntax, we can use pythonic expressions,
+and the variable ``key`` contains the key from the outer scope: ``{He.protag}``
+assigns the value ``"protag"`` to ``key``. ``{Sex[key]}`` will reliably produce
+the same result for the same key (assuming the same initial seed).
+
+Everything else is just YAML syntax and Python f-string expressions.
+
+
+About
+-----
+
+I wrote PrestoPlot to support idea generation and name generation for my
+pulp-inspired science fiction space opera series, `Salvage of Empire`_:
+
+  When his brother-in-law threatens to reveal his terrible secret, Director Kolteo
+  Ais must sacrifice everything he has worked for to save the Galactic Empire—and
+  his marriage—from utter ruin.
+
+.. _Salvage of Empire: https://eykd.net/salvage/
+
+
+CHANGES
+=======
+
+0.5
+---
+
+* Allow instances of ``random.Random()`` as seeds.
+* Rename ``ChangeLog`` to ``CHANGELOG.rst``, include in ``long_description``.
+* Changelog is now manually written, instead of derived from git logs.
+
+0.4
+---
+
+* Fixed major instability of markov generator in the presence of a seed.
+
+
+0.3.4
+-----
+
+* Update packaging and requirements
+
+0.3.3
+-----
+
+* Improved badge
+* Update README w/ build status and better lede
+* Update dev and test requirements
+* Allow customization of start key when rendering story
+* Add python 3.8 to tests
+
+0.3.2
+-----
+
+* Remove more debug logging
+
+0.3.1
+-----
+
+* Remove debug logging
+* Add extra whitespace
+* Add known third parties to isort cfg
+* Add twine dev dependency
+
+0.3
+---
+
+* Add msgpack-compiled test data
+* Add new more efficient storages
+* Improve runtests invocation
+* Tailor flake8 exclusions
+* Pin versions; add msgpack
+* Add some debug logging
+* Add pyyaml requirement
+* Revert "Use strictyaml instead of yaml"
+* Add dev and test requirements
+* Move prestplot package into src/
+* Add Travis CI integration
+* Add .isort.cfg
+* Use collections.abc in prep for python 3.8
+* Use strictyaml instead of yaml
+* Add requirements.txt
+* Use longer python environ specifiers for tox.ini
+* Add project URLs
+
+0.2
+---
+
+* A whole bunch of refactoring
+* Improve dev and test harness w/ dev requirements and test scripts
+
+0.1.3
+-----
+
+* Add extended documentation on generative grammar syntax
+* Further README improvements
+
+0.1.2
+-----
+
+* Improve README
+
+0.1.1
+-----
+
+* Add ``--seed`` option to CLI for pre-seeding oracles
+* Add install/usage documentation to README
+* Add documentation to CLI
+
+0.1
+---
+
+* Add basic test to exercise render\_story()
+* Fix email, summary
+* Remove future features from setup.cfg
+* Finish writing README
+* Fix link in README
+* Initial commit
```

### Comparing `prestoplot-0.5.1/src/prestoplot.egg-info/SOURCES.txt` & `prestoplot-0.5.2/src/prestoplot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .coverall.yml
 .isort.cfg
 .pre-commit-config.yaml
 AUTHORS
+CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements-dev.txt
 requirements-test.txt
 requirements.txt
@@ -17,27 +18,29 @@
 watchtests.sh
 src/prestoplot/__init__.py
 src/prestoplot/_version.py
 src/prestoplot/cli.py
 src/prestoplot/contexts.py
 src/prestoplot/db.py
 src/prestoplot/grammars.py
+src/prestoplot/http.py
 src/prestoplot/markov.py
 src/prestoplot/seeds.py
 src/prestoplot/storages.py
 src/prestoplot/story.py
 src/prestoplot/texts.py
 src/prestoplot.egg-info/PKG-INFO
 src/prestoplot.egg-info/SOURCES.txt
 src/prestoplot.egg-info/dependency_links.txt
 src/prestoplot.egg-info/entry_points.txt
 src/prestoplot.egg-info/pbr.json
 src/prestoplot.egg-info/requires.txt
 src/prestoplot.egg-info/top_level.txt
 tests/test_grammars.py
+tests/test_markov.py
 tests/test_storages.py
 tests/test_story.py
 tests/test_texts.py
 tests/data/characters.yaml
 tests/data/characters_jinja.yaml
 tests/data/names.mp
 tests/data/names.yaml
```

### Comparing `prestoplot-0.5.1/tests/data/characters.yaml` & `prestoplot-0.5.2/tests/data/characters.yaml`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/data/characters_jinja.yaml` & `prestoplot-0.5.2/tests/data/characters_jinja.yaml`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/data/names.mp` & `prestoplot-0.5.2/tests/data/names.mp`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/data/names.yaml` & `prestoplot-0.5.2/tests/data/names.yaml`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/test_storages.py` & `prestoplot-0.5.2/tests/test_storages.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/test_story.py` & `prestoplot-0.5.2/tests/test_story.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/tests/test_texts.py` & `prestoplot-0.5.2/tests/test_texts.py`

 * *Files identical despite different names*

### Comparing `prestoplot-0.5.1/versioneer.py` & `prestoplot-0.5.2/versioneer.py`

 * *Files identical despite different names*

