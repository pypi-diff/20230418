# Comparing `tmp/gym_csle_intrusion_response_game-0.1.8.tar.gz` & `tmp/gym_csle_intrusion_response_game-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_intrusion_response_game-0.1.8.tar", last modified: Mon Mar 20 15:28:46 2023, max compression
+gzip compressed data, was "gym_csle_intrusion_response_game-0.1.9.tar", last modified: Tue Mar 21 08:10:08 2023, max compression
```

## Comparing `gym_csle_intrusion_response_game-0.1.8.tar` & `gym_csle_intrusion_response_game-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.982843 gym_csle_intrusion_response_game-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      719 2023-03-20 15:28:46.982957 gym_csle_intrusion_response_game-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      705 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1394 2023-03-20 15:28:46.983540 gym_csle_intrusion_response_game-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.968665 gym_csle_intrusion_response_game-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.970644 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/
--rw-r--r--   0 kimham     (501) staff       (20)     1183 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.973200 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1403 2023-03-16 16:15:11.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.978811 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3189 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3194 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2468 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
--rw-r--r--   0 kimham     (501) staff       (20)     5513 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5154 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2890 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2890 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.981207 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/
--rw-r--r--   0 kimham     (501) staff       (20)      588 2023-03-08 07:57:44.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    12607 2023-03-16 16:21:28.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
--rw-r--r--   0 kimham     (501) staff       (20)    12670 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
--rw-r--r--   0 kimham     (501) staff       (20)    12682 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
--rw-r--r--   0 kimham     (501) staff       (20)    12691 2023-03-16 16:16:16.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.982059 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-01 07:00:43.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    36796 2023-03-16 16:20:11.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:28:46.972665 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      719 2023-03-20 15:28:46.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     1837 2023-03-20 15:28:46.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:28:46.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-05 11:23:52.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-03-20 15:28:46.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       33 2023-03-20 15:28:46.000000 gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      705 2023-02-28 13:20:12.000000 gym_csle_intrusion_response_game-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1394 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1183 2023-03-07 08:02:15.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1403 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3189 2023-03-06 16:53:37.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3194 2023-03-06 16:51:52.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2468 2023-03-06 13:37:53.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5513 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5154 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2890 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      588 2023-03-07 08:02:15.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12607 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12670 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12682 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12691 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.785258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    36796 2023-03-17 07:49:22.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:08.781258 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      719 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1837 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-02-28 13:33:21.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       33 2023-03-21 08:10:08.000000 gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
```

### Comparing `gym_csle_intrusion_response_game-0.1.8/PKG-INFO` & `gym_csle_intrusion_response_game-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_intrusion_response_game
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.1.8/pyproject.toml` & `gym_csle_intrusion_response_game-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/setup.cfg` & `gym_csle_intrusion_response_game-0.1.9/setup.cfg`

 * *Files 26% similar despite different names*

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

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/__init__.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/constants/constants.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/__init__.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-intrusion-response-game
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.1.8/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt` & `gym_csle_intrusion_response_game-0.1.9/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

