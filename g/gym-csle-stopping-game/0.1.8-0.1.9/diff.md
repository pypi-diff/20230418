# Comparing `tmp/gym_csle_stopping_game-0.1.8.tar.gz` & `tmp/gym_csle_stopping_game-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.1.8.tar", last modified: Mon Mar 20 15:28:12 2023, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.1.9.tar", last modified: Tue Mar 21 08:09:55 2023, max compression
```

## Comparing `gym_csle_stopping_game-0.1.8.tar` & `gym_csle_stopping_game-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.814321 gym_csle_stopping_game-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      715 2023-03-20 15:28:12.814443 gym_csle_stopping_game-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      695 2023-02-12 08:59:32.000000 gym_csle_stopping_game-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1370 2023-03-20 15:28:12.815075 gym_csle_stopping_game-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.804996 gym_csle_stopping_game-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.806882 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/
--rw-r--r--   0 kimham     (501) staff       (20)      651 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.809143 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1030 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.811276 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3002 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4948 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3249 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1375 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.813221 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/
--rw-r--r--   0 kimham     (501) staff       (20)       74 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    24342 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-r--r--   0 kimham     (501) staff       (20)     8926 2023-03-01 09:02:43.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-r--r--   0 kimham     (501) staff       (20)     7639 2023-03-01 09:02:43.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.813878 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18598 2022-11-28 13:00:49.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:12.808703 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      715 2023-03-20 15:28:12.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     1130 2023-03-20 15:28:12.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:28:12.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:06.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-03-20 15:28:12.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       23 2023-03-20 15:28:12.000000 gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      695 2023-02-11 20:28:41.000000 gym_csle_stopping_game-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1370 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      651 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3002 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4948 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3249 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1375 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24342 2022-12-02 09:20:45.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8926 2023-03-03 06:17:38.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7639 2023-03-03 06:17:38.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.177246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18598 2022-11-28 13:03:16.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:55.173246 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      715 2023-03-21 08:09:54.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1130 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:54.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-03-21 08:09:55.000000 gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/top_level.txt
```

### Comparing `gym_csle_stopping_game-0.1.8/PKG-INFO` & `gym_csle_stopping_game-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_stopping_game
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.1.8/pyproject.toml` & `gym_csle_stopping_game-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/setup.cfg` & `gym_csle_stopping_game-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gym>=0.21
-	csle-common>=0.1.8
-	csle-attacker>=0.1.8
-	csle-defender>=0.1.8
-	csle-collector>=0.1.8
+	csle-common>=0.1.9
+	csle-attacker>=0.1.9
+	csle-defender>=0.1.9
+	csle-collector>=0.1.9
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-stopping-game
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.1.8/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.1.9/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

