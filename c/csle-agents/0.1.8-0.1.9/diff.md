# Comparing `tmp/csle_agents-0.1.8.tar.gz` & `tmp/csle_agents-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_agents-0.1.8.tar", last modified: Mon Mar 20 15:29:11 2023, max compression
+gzip compressed data, was "csle_agents-0.1.9.tar", last modified: Tue Mar 21 08:10:20 2023, max compression
```

## Comparing `csle_agents-0.1.8.tar` & `csle_agents-0.1.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.930801 csle_agents-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-03-20 15:29:11.930914 csle_agents-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4154 2023-01-11 18:45:47.000000 csle_agents-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_agents-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1410 2023-03-20 15:29:11.931530 csle_agents-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_agents-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.897459 csle_agents-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.904899 csle_agents-0.1.8/src/csle_agents/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_agents-0.1.8/src/csle_agents/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.907465 csle_agents-0.1.8/src/csle_agents/agents/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.907999 csle_agents-0.1.8/src/csle_agents/agents/base/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1854 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/base/base_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.908806 csle_agents-0.1.8/src/csle_agents/agents/bayes_opt/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/bayes_opt/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    27850 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.909752 csle_agents-0.1.8/src/csle_agents/agents/cross_entropy/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/cross_entropy/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26825 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.910853 csle_agents-0.1.8/src/csle_agents/agents/differential_evolution/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/differential_evolution/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    31102 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.911801 csle_agents-0.1.8/src/csle_agents/agents/dqn/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/dqn/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    19026 2022-12-13 08:21:49.000000 csle_agents-0.1.8/src/csle_agents/agents/dqn/dqn_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.913446 csle_agents-0.1.8/src/csle_agents/agents/dynasec/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/dynasec/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75221 2022-12-10 18:50:08.000000 csle_agents-0.1.8/src/csle_agents/agents/dynasec/dynasec_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.915150 csle_agents-0.1.8/src/csle_agents/agents/fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18132 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/fp/fictitious_play_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.916218 csle_agents-0.1.8/src/csle_agents/agents/hsvi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/hsvi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    49186 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/hsvi/hsvi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.917053 csle_agents-0.1.8/src/csle_agents/agents/hsvi_os_posg/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/hsvi_os_posg/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    75141 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.917920 csle_agents-0.1.8/src/csle_agents/agents/kiefer_wolfowitz/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    29138 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.918849 csle_agents-0.1.8/src/csle_agents/agents/lp_nf/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/lp_nf/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    18233 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.919477 csle_agents-0.1.8/src/csle_agents/agents/pi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/pi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17515 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/pi/pi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.920119 csle_agents-0.1.8/src/csle_agents/agents/ppo/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/ppo/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    23280 2023-03-16 16:33:06.000000 csle_agents-0.1.8/src/csle_agents/agents/ppo/ppo_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.921112 csle_agents-0.1.8/src/csle_agents/agents/q_learning/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/q_learning/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17233 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/q_learning/q_learning_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.922041 csle_agents-0.1.8/src/csle_agents/agents/random_search/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/random_search/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    26063 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/random_search/random_search_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.922676 csle_agents-0.1.8/src/csle_agents/agents/reinforce/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/reinforce/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    24982 2022-12-13 08:21:49.000000 csle_agents-0.1.8/src/csle_agents/agents/reinforce/reinforce_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.923256 csle_agents-0.1.8/src/csle_agents/agents/sarsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/sarsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    17329 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/sarsa/sarsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.923865 csle_agents-0.1.8/src/csle_agents/agents/shapley_iteration/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/shapley_iteration/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    15674 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.924478 csle_agents-0.1.8/src/csle_agents/agents/sondik_vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/sondik_vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    22055 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.925124 csle_agents-0.1.8/src/csle_agents/agents/t_fp/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/t_fp/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    41769 2022-12-10 18:50:08.000000 csle_agents-0.1.8/src/csle_agents/agents/t_fp/t_fp_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.926181 csle_agents-0.1.8/src/csle_agents/agents/t_spsa/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/t_spsa/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    32591 2022-12-10 18:50:08.000000 csle_agents-0.1.8/src/csle_agents/agents/t_spsa/t_spsa_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.927245 csle_agents-0.1.8/src/csle_agents/agents/vi/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/vi/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    15759 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/agents/vi/vi_agent.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.929168 csle_agents-0.1.8/src/csle_agents/common/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/common/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5759 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/common/actor_critic_net.py
--rw-r--r--   0 kimham     (501) staff       (20)     4595 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/common/fnn_w_gaussian.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/common/fnn_w_linear.py
--rw-r--r--   0 kimham     (501) staff       (20)     3460 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/common/pruning.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.929669 csle_agents-0.1.8/src/csle_agents/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    10945 2023-03-08 07:57:44.000000 csle_agents-0.1.8/src/csle_agents/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.930390 csle_agents-0.1.8/src/csle_agents/job_controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/job_controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2459 2022-11-28 13:00:49.000000 csle_agents-0.1.8/src/csle_agents/job_controllers/training_job_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:29:11.907221 csle_agents-0.1.8/src/csle_agents.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      653 2023-03-20 15:29:11.000000 csle_agents-0.1.8/src/csle_agents.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     2852 2023-03-20 15:29:11.000000 csle_agents-0.1.8/src/csle_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:29:11.000000 csle_agents-0.1.8/src/csle_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:04:28.000000 csle_agents-0.1.8/src/csle_agents.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      371 2023-03-20 15:29:11.000000 csle_agents-0.1.8/src/csle_agents.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       12 2023-03-20 15:29:11.000000 csle_agents-0.1.8/src/csle_agents.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-03-21 08:10:20.905268 csle_agents-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4154 2023-01-03 16:53:40.000000 csle_agents-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-02-11 20:28:41.000000 csle_agents-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1410 2023-03-21 08:10:20.905268 csle_agents-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_agents-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_agents-0.1.9/src/csle_agents/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents/agents/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/base/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/base/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1854 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/base/base_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    27850 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26825 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    31102 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/dqn/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/dqn/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19026 2022-12-11 08:50:43.000000 csle_agents-0.1.9/src/csle_agents/agents/dqn/dqn_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/dynasec/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/dynasec/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75221 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/dynasec/dynasec_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18132 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/fp/fictitious_play_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/hsvi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    49186 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi/hsvi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.897268 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    75141 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29138 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18233 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/pi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/pi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17515 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/pi/pi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/ppo/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/ppo/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    23280 2023-03-17 07:49:22.000000 csle_agents-0.1.9/src/csle_agents/agents/ppo/ppo_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/q_learning/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/q_learning/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17233 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/q_learning/q_learning_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/random_search/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/random_search/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    26063 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/random_search/random_search_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/reinforce/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/reinforce/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24982 2022-12-11 08:51:55.000000 csle_agents-0.1.9/src/csle_agents/agents/reinforce/reinforce_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/sarsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sarsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17329 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sarsa/sarsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.901268 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15674 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22055 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/t_fp/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/t_fp/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    41769 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/t_fp/t_fp_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    32591 2022-12-11 08:32:31.000000 csle_agents-0.1.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/agents/vi/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/vi/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15759 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/agents/vi/vi_agent.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5759 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/actor_critic_net.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4595 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/fnn_w_gaussian.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/fnn_w_linear.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3460 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/common/pruning.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10945 2023-03-06 21:38:13.000000 csle_agents-0.1.9/src/csle_agents/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.905268 csle_agents-0.1.9/src/csle_agents/job_controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/job_controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2459 2022-11-28 13:03:16.000000 csle_agents-0.1.9/src/csle_agents/job_controllers/training_job_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:20.893268 csle_agents-0.1.9/src/csle_agents.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      653 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2852 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:05.000000 csle_agents-0.1.9/src/csle_agents.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      371 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-03-21 08:10:20.000000 csle_agents-0.1.9/src/csle_agents.egg-info/top_level.txt
```

### Comparing `csle_agents-0.1.8/PKG-INFO` & `csle_agents-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_agents
-Version: 0.1.8
+Version: 0.1.9
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.1.8/README.md` & `csle_agents-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/pyproject.toml` & `csle_agents-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/setup.cfg` & `csle_agents-0.1.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.8
-	csle-collector>=0.1.8
-	csle-attacker>=0.1.8
-	csle-defender>=0.1.8
-	csle-system-identification>=0.1.8
-	gym-csle-stopping-game>=0.1.8
+	csle-common>=0.1.9
+	csle-collector>=0.1.9
+	csle-attacker>=0.1.9
+	csle-defender>=0.1.9
+	csle-system-identification>=0.1.9
+	gym-csle-stopping-game>=0.1.9
 	stable-baselines3>=1.6.2
 	pulp>=2.7.0
 	bayesian-optimization>=1.3.1
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
```

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/base/base_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/base/base_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/bayes_opt/bayes_opt_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/cross_entropy/cross_entropy_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/differential_evolution/differential_evolution_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/dqn/dqn_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/dqn/dqn_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/dynasec/dynasec_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/dynasec/dynasec_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/fp/fictitious_play_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/fp/fictitious_play_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/hsvi/hsvi_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/hsvi/hsvi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/hsvi_os_posg/hsvi_os_posg_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/kiefer_wolfowitz/kiefer_wolfowitz_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/lp_nf/linear_programming_normal_form_game_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/pi/pi_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/pi/pi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/ppo/ppo_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/ppo/ppo_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/q_learning/q_learning_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/q_learning/q_learning_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/random_search/random_search_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/random_search/random_search_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/reinforce/reinforce_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/reinforce/reinforce_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/sarsa/sarsa_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/sarsa/sarsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/shapley_iteration/shapley_iteration_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/sondik_vi/sondik_vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/t_fp/t_fp_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/t_fp/t_fp_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/t_spsa/t_spsa_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/t_spsa/t_spsa_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/agents/vi/vi_agent.py` & `csle_agents-0.1.9/src/csle_agents/agents/vi/vi_agent.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/common/actor_critic_net.py` & `csle_agents-0.1.9/src/csle_agents/common/actor_critic_net.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/common/fnn_w_gaussian.py` & `csle_agents-0.1.9/src/csle_agents/common/fnn_w_gaussian.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/common/fnn_w_linear.py` & `csle_agents-0.1.9/src/csle_agents/common/fnn_w_linear.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/common/pruning.py` & `csle_agents-0.1.9/src/csle_agents/common/pruning.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/constants/constants.py` & `csle_agents-0.1.9/src/csle_agents/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents/job_controllers/training_job_manager.py` & `csle_agents-0.1.9/src/csle_agents/job_controllers/training_job_manager.py`

 * *Files identical despite different names*

### Comparing `csle_agents-0.1.8/src/csle_agents.egg-info/PKG-INFO` & `csle_agents-0.1.9/src/csle_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-agents
-Version: 0.1.8
+Version: 0.1.9
 Summary: Reinforcement learning agents for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_agents-0.1.8/src/csle_agents.egg-info/SOURCES.txt` & `csle_agents-0.1.9/src/csle_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

