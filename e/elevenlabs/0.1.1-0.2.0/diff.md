# Comparing `tmp/elevenlabs-0.1.1.tar.gz` & `tmp/elevenlabs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.1.1.tar", last modified: Sat Mar 25 18:08:50 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.0.tar", last modified: Tue Apr 18 16:27:04 2023, max compression
```

## Comparing `elevenlabs-0.1.1.tar` & `elevenlabs-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     1058 2023-02-06 23:35:09.000000 elevenlabs-0.1.1/LICENSE
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2892 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/PKG-INFO
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     1799 2023-03-15 00:36:25.000000 elevenlabs-0.1.1/README.md
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     1847 2023-03-13 19:24:51.000000 elevenlabs-0.1.1/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/elevenlabs/
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     1198 2023-02-06 23:58:01.000000 elevenlabs-0.1.1/elevenlabs/__init__.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      172 2023-02-06 22:56:26.000000 elevenlabs-0.1.1/elevenlabs/endpoint.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)        2 2023-02-06 23:57:38.000000 elevenlabs-0.1.1/elevenlabs/exceptions.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      295 2023-02-06 23:29:12.000000 elevenlabs-0.1.1/elevenlabs/tts.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/elevenlabs/voices/
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     1703 2023-03-13 18:41:07.000000 elevenlabs-0.1.1/elevenlabs/voices/__init__.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      823 2023-03-24 20:51:33.000000 elevenlabs-0.1.1/elevenlabs/voices/audiofile.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     1725 2023-03-13 19:34:49.000000 elevenlabs-0.1.1/elevenlabs/voices/voice.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      333 2023-03-13 18:34:39.000000 elevenlabs-0.1.1/elevenlabs/voices/voices_iter.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/elevenlabs.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2892 2023-03-25 18:08:50.000000 elevenlabs-0.1.1/elevenlabs.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      426 2023-03-25 18:08:50.000000 elevenlabs-0.1.1/elevenlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-03-25 18:08:50.000000 elevenlabs-0.1.1/elevenlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-03-25 18:08:50.000000 elevenlabs-0.1.1/elevenlabs.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       11 2023-03-25 18:08:50.000000 elevenlabs-0.1.1/elevenlabs.egg-info/top_level.txt
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      103 2023-03-25 18:08:50.374123 elevenlabs-0.1.1/setup.cfg
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      827 2023-03-25 18:07:48.000000 elevenlabs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:27:04.562462 elevenlabs-0.2.0/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:27:04.000000 elevenlabs-0.2.0/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:27:04.566462 elevenlabs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-18 16:26:51.000000 elevenlabs-0.2.0/setup.py
```

