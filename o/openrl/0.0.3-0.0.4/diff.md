# Comparing `tmp/openrl-0.0.3.tar.gz` & `tmp/openrl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrl-0.0.3.tar", last modified: Thu Apr 13 03:01:23 2023, max compression
+gzip compressed data, was "openrl-0.0.4.tar", last modified: Tue Apr 18 10:09:36 2023, max compression
```

## Comparing `openrl-0.0.3.tar` & `openrl-0.0.4.tar`

### file list

```diff
@@ -1,139 +1,132 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.125212 openrl-0.0.3/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-12 14:31:37.000000 openrl-0.0.3/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.3/LICENSE.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)     4757 2023-04-13 03:01:23.125050 openrl-0.0.3/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     3712 2023-04-13 02:44:18.000000 openrl-0.0.3/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.096970 openrl-0.0.3/openrl/
--rw-r--r--   0 4paradigm   (501) staff       (20)      186 2023-04-12 14:36:21.000000 openrl-0.0.3/openrl/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.098489 openrl-0.0.3/openrl/algorithms/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/algorithms/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2302 2023-04-11 10:43:47.000000 openrl-0.0.3/openrl/algorithms/base_algorithm.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    15587 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/algorithms/ppo.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.099445 openrl-0.0.3/openrl/buffers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/buffers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2503 2023-04-10 09:08:53.000000 openrl-0.0.3/openrl/buffers/normal_buffer.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    54966 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/buffers/replay_data.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.100566 openrl-0.0.3/openrl/buffers/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/buffers/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2418 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/buffers/utils/obs_data.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3221 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/buffers/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.101217 openrl-0.0.3/openrl/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1882 2023-04-12 14:36:21.000000 openrl-0.0.3/openrl/cli/cli.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1527 2023-04-13 02:37:01.000000 openrl-0.0.3/openrl/cli/train.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.101635 openrl-0.0.3/openrl/configs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/configs/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    37720 2023-04-12 14:36:21.000000 openrl-0.0.3/openrl/configs/config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.102160 openrl-0.0.3/openrl/datasets/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/datasets/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.103424 openrl-0.0.3/openrl/drivers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/drivers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      236 2023-03-28 06:23:04.000000 openrl-0.0.3/openrl/drivers/base_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9979 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/drivers/onpolicy_driver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      840 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/drivers/rl_driver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.103653 openrl-0.0.3/openrl/envs/
--rw-r--r--   0 4paradigm   (501) staff       (20)      125 2023-04-07 13:42:53.000000 openrl-0.0.3/openrl/envs/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.104294 openrl-0.0.3/openrl/envs/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)      716 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4182 2023-04-12 14:36:21.000000 openrl-0.0.3/openrl/envs/common/registration.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.104547 openrl-0.0.3/openrl/envs/gymnasium/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1435 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/gymnasium/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.107020 openrl-0.0.3/openrl/envs/mpe/
--rw-r--r--   0 4paradigm   (501) staff       (20)      672 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/mpe/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    14307 2023-04-07 13:52:40.000000 openrl-0.0.3/openrl/envs/mpe/core.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      614 2023-04-07 13:47:06.000000 openrl-0.0.3/openrl/envs/mpe/mpe_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2489 2023-04-10 07:48:10.000000 openrl-0.0.3/openrl/envs/mpe/multi_discrete.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19316 2023-04-11 11:55:11.000000 openrl-0.0.3/openrl/envs/mpe/multiagent_env.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11584 2023-04-10 13:20:30.000000 openrl-0.0.3/openrl/envs/mpe/rendering.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      361 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/envs/mpe/scenario.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.107489 openrl-0.0.3/openrl/envs/mpe/scenarios/
--rw-r--r--   0 4paradigm   (501) staff       (20)      147 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/envs/mpe/scenarios/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4404 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/mpe/scenarios/simple_spread.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.108831 openrl-0.0.3/openrl/envs/vec_env/
--rw-r--r--   0 4paradigm   (501) staff       (20)      254 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/vec_env/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    30679 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/vec_env/async_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7764 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/vec_env/base_venv.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    11099 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/vec_env/sync_venv.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.110069 openrl-0.0.3/openrl/envs/vec_env/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/vec_env/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6519 2023-04-11 08:43:14.000000 openrl-0.0.3/openrl/envs/vec_env/utils/numpy_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7903 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/vec_env/utils/share_memory.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/vec_env/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.110833 openrl-0.0.3/openrl/envs/vec_env/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/vec_env/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9933 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/envs/vec_env/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2653 2023-04-12 14:35:56.000000 openrl-0.0.3/openrl/envs/vec_env/wrappers/vec_monitor.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.111999 openrl-0.0.3/openrl/envs/wrappers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      342 2023-04-13 02:35:45.000000 openrl-0.0.3/openrl/envs/wrappers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1419 2023-04-13 02:36:05.000000 openrl-0.0.3/openrl/envs/wrappers/base_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1843 2023-04-13 02:35:45.000000 openrl-0.0.3/openrl/envs/wrappers/extra_wrappers.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-13 02:35:11.000000 openrl-0.0.3/openrl/envs/wrappers/multiagent_wrapper.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/envs/wrappers/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.113337 openrl-0.0.3/openrl/modules/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1542 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/base_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.114265 openrl-0.0.3/openrl/modules/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-03-27 09:25:06.000000 openrl-0.0.3/openrl/modules/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/common/base_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3212 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/common/ppo_net.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/model_config.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.115707 openrl-0.0.3/openrl/modules/networks/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/networks/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1230 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/networks/base_policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/networks/base_value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8094 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/networks/policy_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6483 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/networks/policy_value_network.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.119854 openrl-0.0.3/openrl/modules/networks/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      604 2022-09-01 14:01:33.000000 openrl-0.0.3/openrl/modules/networks/utils/FcEncoder.py
--rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.3/openrl/modules/networks/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     7493 2023-04-06 11:59:56.000000 openrl-0.0.3/openrl/modules/networks/utils/act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     8494 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/modules/networks/utils/attention.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2210 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/modules/networks/utils/cnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      803 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/networks/utils/distributed_utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3601 2022-09-16 11:16:47.000000 openrl-0.0.3/openrl/modules/networks/utils/distributions.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     9416 2023-03-30 08:33:37.000000 openrl-0.0.3/openrl/modules/networks/utils/mix.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5969 2023-04-11 10:43:47.000000 openrl-0.0.3/openrl/modules/networks/utils/mlp.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3796 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/modules/networks/utils/popart.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    13324 2022-09-21 05:38:47.000000 openrl-0.0.3/openrl/modules/networks/utils/pre_model_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3533 2022-07-24 12:50:33.000000 openrl-0.0.3/openrl/modules/networks/utils/rnn.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3332 2023-03-28 07:32:22.000000 openrl-0.0.3/openrl/modules/networks/utils/transformer_act.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      319 2023-03-28 07:32:36.000000 openrl-0.0.3/openrl/modules/networks/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    19229 2022-08-04 09:35:49.000000 openrl-0.0.3/openrl/modules/networks/utils/utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4619 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/networks/value_network.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5682 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/ppo_module.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     4699 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/modules/rl_module.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.121132 openrl-0.0.3/openrl/modules/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/modules/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      616 2023-03-28 07:42:17.000000 openrl-0.0.3/openrl/modules/utils/util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3381 2022-09-27 11:21:49.000000 openrl-0.0.3/openrl/modules/utils/valuenorm.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.121951 openrl-0.0.3/openrl/runners/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/runners/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      882 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/runners/base_runner.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      758 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/runners/base_trainer.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.122688 openrl-0.0.3/openrl/runners/common/
--rw-r--r--   0 4paradigm   (501) staff       (20)       83 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/runners/common/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1298 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/runners/common/base_agent.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     5055 2023-04-12 14:35:57.000000 openrl-0.0.3/openrl/runners/common/ppo_agent.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.122838 openrl-0.0.3/openrl/supports/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/supports/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.123463 openrl-0.0.3/openrl/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     6620 2023-04-12 14:34:56.000000 openrl-0.0.3/openrl/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      588 2023-04-11 10:43:47.000000 openrl-0.0.3/openrl/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.097739 openrl-0.0.3/openrl.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     4757 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     3435 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      143 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-13 03:01:23.000000 openrl-0.0.3/openrl.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-13 03:01:23.125260 openrl-0.0.3/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2721 2023-04-13 02:49:54.000000 openrl-0.0.3/setup.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.123788 openrl-0.0.3/tests/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/tests/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.124276 openrl-0.0.3/tests/project/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/tests/project/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      971 2023-04-12 14:36:21.000000 openrl-0.0.3/tests/project/test_version.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-13 03:01:23.124759 openrl-0.0.3/tests/test_buffer/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.3/tests/test_buffer/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-12 14:35:57.000000 openrl-0.0.3/tests/test_buffer/test_buffer.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.219174 openrl-0.0.4/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-04-12 14:31:37.000000 openrl-0.0.4/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11342 2023-03-23 09:43:52.000000 openrl-0.0.4/LICENSE.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4729 2023-04-18 10:09:36.219020 openrl-0.0.4/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3684 2023-04-13 06:07:12.000000 openrl-0.0.4/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.194804 openrl-0.0.4/openrl/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      194 2023-04-18 10:09:23.000000 openrl-0.0.4/openrl/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.196428 openrl-0.0.4/openrl/algorithms/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/algorithms/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2915 2023-04-18 09:39:06.000000 openrl-0.0.4/openrl/algorithms/base_algorithm.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    15908 2023-04-18 09:39:19.000000 openrl-0.0.4/openrl/algorithms/ppo.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.197187 openrl-0.0.4/openrl/buffers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      726 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/buffers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3100 2023-04-18 09:40:26.000000 openrl-0.0.4/openrl/buffers/normal_buffer.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    54666 2023-04-18 09:41:36.000000 openrl-0.0.4/openrl/buffers/replay_data.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.198095 openrl-0.0.4/openrl/buffers/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/buffers/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1686 2023-04-18 09:39:57.000000 openrl-0.0.4/openrl/buffers/utils/obs_data.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3153 2023-04-18 09:39:57.000000 openrl-0.0.4/openrl/buffers/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.198787 openrl-0.0.4/openrl/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2053 2023-04-18 08:43:57.000000 openrl-0.0.4/openrl/cli/cli.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1709 2023-04-18 08:57:15.000000 openrl-0.0.4/openrl/cli/train.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.199236 openrl-0.0.4/openrl/configs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/configs/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    29480 2023-04-18 09:55:21.000000 openrl-0.0.4/openrl/configs/config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.200300 openrl-0.0.4/openrl/drivers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/drivers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      236 2023-03-28 06:23:04.000000 openrl-0.0.4/openrl/drivers/base_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9767 2023-04-18 09:55:53.000000 openrl-0.0.4/openrl/drivers/onpolicy_driver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      840 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/drivers/rl_driver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.200537 openrl-0.0.4/openrl/envs/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      125 2023-04-07 13:42:53.000000 openrl-0.0.4/openrl/envs/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.201028 openrl-0.0.4/openrl/envs/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      716 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4196 2023-04-14 07:57:12.000000 openrl-0.0.4/openrl/envs/common/registration.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.201280 openrl-0.0.4/openrl/envs/gymnasium/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1435 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/gymnasium/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.203057 openrl-0.0.4/openrl/envs/mpe/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      673 2023-04-14 08:15:22.000000 openrl-0.0.4/openrl/envs/mpe/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    14285 2023-04-18 09:57:30.000000 openrl-0.0.4/openrl/envs/mpe/core.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      614 2023-04-07 13:47:06.000000 openrl-0.0.4/openrl/envs/mpe/mpe_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2489 2023-04-10 07:48:10.000000 openrl-0.0.4/openrl/envs/mpe/multi_discrete.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    19199 2023-04-18 09:57:30.000000 openrl-0.0.4/openrl/envs/mpe/multiagent_env.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11584 2023-04-10 13:20:30.000000 openrl-0.0.4/openrl/envs/mpe/rendering.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      361 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/envs/mpe/scenario.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.203501 openrl-0.0.4/openrl/envs/mpe/scenarios/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      147 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/envs/mpe/scenarios/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4404 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/mpe/scenarios/simple_spread.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.204702 openrl-0.0.4/openrl/envs/vec_env/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      254 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/envs/vec_env/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    30677 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/envs/vec_env/async_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8063 2023-04-14 07:26:31.000000 openrl-0.0.4/openrl/envs/vec_env/base_venv.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11100 2023-04-14 07:27:02.000000 openrl-0.0.4/openrl/envs/vec_env/sync_venv.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.205772 openrl-0.0.4/openrl/envs/vec_env/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6519 2023-04-11 08:43:14.000000 openrl-0.0.4/openrl/envs/vec_env/utils/numpy_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7903 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/share_memory.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1909 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.206548 openrl-0.0.4/openrl/envs/vec_env/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9291 2023-04-14 07:16:41.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2653 2023-04-14 08:16:46.000000 openrl-0.0.4/openrl/envs/vec_env/wrappers/vec_monitor.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.207870 openrl-0.0.4/openrl/envs/wrappers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      372 2023-04-14 07:11:32.000000 openrl-0.0.4/openrl/envs/wrappers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1419 2023-04-13 02:36:05.000000 openrl-0.0.4/openrl/envs/wrappers/base_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2480 2023-04-17 07:08:30.000000 openrl-0.0.4/openrl/envs/wrappers/extra_wrappers.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2533 2023-04-13 02:35:11.000000 openrl-0.0.4/openrl/envs/wrappers/multiagent_wrapper.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1188 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/envs/wrappers/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.208940 openrl-0.0.4/openrl/modules/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1540 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/base_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.209734 openrl-0.0.4/openrl/modules/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-03-27 09:25:06.000000 openrl-0.0.4/openrl/modules/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      738 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/common/base_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3300 2023-04-14 07:46:31.000000 openrl-0.0.4/openrl/modules/common/ppo_net.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1233 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/model_config.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.211431 openrl-0.0.4/openrl/modules/networks/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/networks/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1227 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/modules/networks/base_policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1190 2023-04-14 07:55:00.000000 openrl-0.0.4/openrl/modules/networks/base_value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     8075 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/policy_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6467 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/policy_value_network.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.214342 openrl-0.0.4/openrl/modules/networks/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)        0 2022-09-12 08:05:59.000000 openrl-0.0.4/openrl/modules/networks/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     7493 2023-04-06 11:59:56.000000 openrl-0.0.4/openrl/modules/networks/utils/act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     9383 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/attention.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2378 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/cnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      803 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/networks/utils/distributed_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3601 2022-09-16 11:16:47.000000 openrl-0.0.4/openrl/modules/networks/utils/distributions.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    10433 2023-04-14 07:55:18.000000 openrl-0.0.4/openrl/modules/networks/utils/mix.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5956 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/utils/mlp.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3796 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/modules/networks/utils/popart.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3533 2022-07-24 12:50:33.000000 openrl-0.0.4/openrl/modules/networks/utils/rnn.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3332 2023-03-28 07:32:22.000000 openrl-0.0.4/openrl/modules/networks/utils/transformer_act.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      319 2023-03-28 07:32:36.000000 openrl-0.0.4/openrl/modules/networks/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4602 2023-04-14 07:55:55.000000 openrl-0.0.4/openrl/modules/networks/value_network.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5674 2023-04-14 07:51:42.000000 openrl-0.0.4/openrl/modules/ppo_module.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     5172 2023-04-14 07:55:34.000000 openrl-0.0.4/openrl/modules/rl_module.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.215258 openrl-0.0.4/openrl/modules/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/modules/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      616 2023-03-28 07:42:17.000000 openrl-0.0.4/openrl/modules/utils/util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3381 2022-09-27 11:21:49.000000 openrl-0.0.4/openrl/modules/utils/valuenorm.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.215479 openrl-0.0.4/openrl/runners/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/runners/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.216196 openrl-0.0.4/openrl/runners/common/
+-rw-r--r--   0 4paradigm   (501) staff       (20)       83 2023-04-12 14:35:57.000000 openrl-0.0.4/openrl/runners/common/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1269 2023-04-14 08:27:24.000000 openrl-0.0.4/openrl/runners/common/base_agent.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6139 2023-04-14 09:38:42.000000 openrl-0.0.4/openrl/runners/common/ppo_agent.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.216432 openrl-0.0.4/openrl/supports/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/supports/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217122 openrl-0.0.4/openrl/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/openrl/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     6608 2023-04-14 10:20:15.000000 openrl-0.0.4/openrl/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      588 2023-04-14 09:35:30.000000 openrl-0.0.4/openrl/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.195626 openrl-0.0.4/openrl.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     4729 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3216 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      151 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       13 2023-04-18 10:09:36.000000 openrl-0.0.4/openrl.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-04-18 10:09:36.219223 openrl-0.0.4/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2740 2023-04-14 07:27:41.000000 openrl-0.0.4/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217347 openrl-0.0.4/tests/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.217866 openrl-0.0.4/tests/project/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/project/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      971 2023-04-12 14:36:21.000000 openrl-0.0.4/tests/project/test_version.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-04-18 10:09:36.218330 openrl-0.0.4/tests/test_buffer/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-04-12 14:34:56.000000 openrl-0.0.4/tests/test_buffer/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1803 2023-04-12 14:35:57.000000 openrl-0.0.4/tests/test_buffer/test_buffer.py
```

### Comparing `openrl-0.0.3/LICENSE` & `openrl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/LICENSE.txt` & `openrl-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/PKG-INFO` & `openrl-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.3
+Version: 0.0.4
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -30,15 +30,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/github/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=CS4Y70UWDS)](https://codecov.io/github/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
@@ -73,30 +73,30 @@
 pip install openrl
 ```
 
 ## 快速上手
 
 可以通过命令行快速训练`CartPole`环境:
 ```bash
-openrl --mode train --env CartPole-v0
+openrl --mode train --env CartPole-v1
 ```
 
 ## 支持者
 
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们的论文:
+如果我们的工作对你有帮助，欢迎引用我们:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
@@ -105,9 +105,7 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
-
-## 致谢
```

### Comparing `openrl-0.0.3/README.md` & `openrl-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/github/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=CS4Y70UWDS)](https://codecov.io/github/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
@@ -49,30 +49,30 @@
 pip install openrl
 ```
 
 ## 快速上手
 
 可以通过命令行快速训练`CartPole`环境:
 ```bash
-openrl --mode train --env CartPole-v0
+openrl --mode train --env CartPole-v1
 ```
 
 ## 支持者
 
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们的论文:
+如果我们的工作对你有帮助，欢迎引用我们:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
@@ -81,9 +81,7 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
-
-## 致谢
```

### Comparing `openrl-0.0.3/openrl/algorithms/__init__.py` & `openrl-0.0.4/openrl/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/algorithms/ppo.py` & `openrl-0.0.4/openrl/algorithms/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright 2023 The OpenRL Authors.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+""""""
+
 from typing import Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.nn.parallel import DistributedDataParallel
 
@@ -11,21 +29,21 @@
 
 from openrl.modules.networks.utils.distributed_utils import reduce_tensor
 
 
 class PPOAlgorithm(BaseAlgorithm):
     def __init__(
         self,
-        args,
+        cfg,
         init_module,
-        agent_num: int,
+        agent_num: int = 1,
         device: Union[str, torch.device] = "cpu",
     ) -> None:
-        self.use_joint_action_loss = args.use_joint_action_loss
-        super(PPOAlgorithm, self).__init__(args, init_module, agent_num, device)
+        self.use_joint_action_loss = cfg.use_joint_action_loss
+        super(PPOAlgorithm, self).__init__(cfg, init_module, agent_num, device)
 
     def ppo_update(self, sample, turn_on=True):
         for optimizer in self.algo_module.optimizers.values():
             optimizer.zero_grad()
 
         (
             critic_obs_batch,
@@ -37,16 +55,14 @@
             return_batch,
             masks_batch,
             active_masks_batch,
             old_action_log_probs_batch,
             adv_targ,
             available_actions_batch,
         ) = sample
-        # print(critic_obs_batch)
-        # exit()
 
         old_action_log_probs_batch = check(old_action_log_probs_batch).to(**self.tpdv)
         adv_targ = check(adv_targ).to(**self.tpdv)
         value_preds_batch = check(value_preds_batch).to(**self.tpdv)
         return_batch = check(return_batch).to(**self.tpdv)
         active_masks_batch = check(active_masks_batch).to(**self.tpdv)
 
@@ -137,23 +153,14 @@
         else:
             for optimizer in self.algo_module.optimizers.values():
                 optimizer.step()
 
         if self.world_size > 1:
             torch.cuda.synchronize()
 
-        # if not hasattr(self, "step_num"):
-        #     self.step_num = 0
-        # else:
-        #     self.step_num += 1
-        # if self.step_num % 10 == 0:
-        #     print(self.step_num, policy_loss)
-        # if self.step_num == 100:
-        #     exit()
-
         return (
             value_loss,
             critic_grad_norm,
             policy_loss,
             dist_entropy,
             actor_grad_norm,
             ratio,
```

### Comparing `openrl-0.0.3/openrl/buffers/__init__.py` & `openrl-0.0.4/openrl/buffers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/buffers/replay_data.py` & `openrl-0.0.4/openrl/buffers/replay_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,35 +37,38 @@
     _shuffle_agent_grid,
 )
 
 
 class ReplayData(object):
     def __init__(
         self,
-        args,
+        cfg,
         num_agents,
         obs_space,
         act_space,
-        data_client,
+        data_client=None,
         episode_length=None,
     ):
         if episode_length is None:
-            episode_length = args.episode_length
+            episode_length = cfg.episode_length
         self.episode_length = episode_length
 
-        self.n_rollout_threads = args.n_rollout_threads
+        self.n_rollout_threads = cfg.n_rollout_threads
 
-        self.hidden_size = args.rnn_hidden_size
-        self.recurrent_N = args.recurrent_N
-        self.gamma = args.gamma
-        self.gae_lambda = args.gae_lambda
-        self._use_gae = args.use_gae
-        self._use_popart = args.use_popart
-        self._use_valuenorm = args.use_valuenorm
-        self._use_proper_time_limits = args.use_proper_time_limits
+        if hasattr(cfg, "rnn_hidden_size"):
+            self.hidden_size = cfg.rnn_hidden_size
+        else:
+            self.hidden_size = cfg.hidden_size
+        self.recurrent_N = cfg.recurrent_N
+        self.gamma = cfg.gamma
+        self.gae_lambda = cfg.gae_lambda
+        self._use_gae = cfg.use_gae
+        self._use_popart = cfg.use_popart
+        self._use_valuenorm = cfg.use_valuenorm
+        self._use_proper_time_limits = cfg.use_proper_time_limits
 
         self._mixed_obs = False  # for mixed observation
 
         policy_obs_shape = get_policy_obs_space(obs_space)
         critic_obs_shape = get_critic_obs_space(obs_space)
 
         # for mixed observation
@@ -425,16 +428,14 @@
                     num_agents,
                     n_rollout_threads * episode_length * num_agents,
                     num_mini_batch,
                 )
             )
             mini_batch_size = batch_size // num_mini_batch
 
-        # rand = torch.randperm(batch_size).numpy()
-        # sampler = [rand[i*mini_batch_size:(i+1)*mini_batch_size] for i in range(num_mini_batch)]
         sampler = BatchSampler(
             SubsetRandomSampler(range(batch_size)), mini_batch_size, drop_last=True
         )
 
         if self._mixed_obs:
             critic_obs = {}
             policy_obs = {}
@@ -522,16 +523,14 @@
                     num_agents,
                     n_rollout_threads * episode_length,
                     num_mini_batch,
                 )
             )
             mini_batch_size = batch_size // num_mini_batch
 
-        # rand = torch.randperm(batch_size).numpy()
-        # sampler = [rand[i*mini_batch_size:(i+1)*mini_batch_size] for i in range(num_mini_batch)]
         sampler = BatchSampler(
             SubsetRandomSampler(range(batch_size)), mini_batch_size, drop_last=True
         )
 
         if self._mixed_obs:
             critic_obs = {}
             for key in self.critic_obs.keys():
@@ -753,15 +752,15 @@
 
             # [N[T, dim]]
             T, N = self.episode_length, num_envs_per_batch
             # These are all from_numpys of size (T, N, -1)
             if self._mixed_obs:
                 for key in critic_obs_batch.keys():
                     critic_obs_batch[key] = np.stack(critic_obs_batch[key], 1)
-                for key in obs_batch.keys():
+                for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = np.stack(policy_obs_batch[key], 1)
             else:
                 critic_obs_batch = np.stack(critic_obs_batch, 1)
                 policy_obs_batch = np.stack(policy_obs_batch, 1)
             actions_batch = np.stack(actions_batch, 1)
             if self.available_actions is not None:
                 available_actions_batch = np.stack(available_actions_batch, 1)
@@ -780,15 +779,15 @@
                 N, *self.rnn_states_critic.shape[3:]
             )
 
             # Flatten the (T, N, ...) from_numpys to (T * N, ...)
             if self._mixed_obs:
                 for key in critic_obs_batch.keys():
                     critic_obs_batch[key] = _flatten(T, N, critic_obs_batch[key])
-                for key in obs_batch.keys():
+                for key in policy_obs_batch.keys():
                     policy_obs_batch[key] = _flatten(T, N, policy_obs_batch[key])
             else:
                 critic_obs_batch = _flatten(T, N, critic_obs_batch)
                 policy_obs_batch = _flatten(T, N, policy_obs_batch)
             actions_batch = _flatten(T, N, actions_batch)
             if self.available_actions is not None:
                 available_actions_batch = _flatten(T, N, available_actions_batch)
@@ -1121,16 +1120,15 @@
         actions = _cast(self.actions)
         action_log_probs = _cast(self.action_log_probs)
         advantages = _cast(advantages)
         value_preds = _cast(self.value_preds[:-1])
         returns = _cast(self.returns[:-1])
         masks = _cast(self.masks[:-1])
         active_masks = _cast(self.active_masks[:-1])
-        # rnn_states = _cast(self.rnn_states[:-1])
-        # rnn_states_critic = _cast(self.rnn_states_critic[:-1])
+
         rnn_states = (
             self.rnn_states[:-1]
             .transpose(1, 2, 0, 3, 4)
             .reshape(-1, *self.rnn_states.shape[3:])
         )
         rnn_states_critic = (
             self.rnn_states_critic[:-1]
```

### Comparing `openrl-0.0.3/openrl/buffers/utils/__init__.py` & `openrl-0.0.4/openrl/buffers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/buffers/utils/util.py` & `openrl-0.0.4/openrl/buffers/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,10 +98,9 @@
 
 def _cast_v3(x):
     return x.transpose(1, 0, 2, 3).reshape(-1, *x.shape[2:])
 
 
 def _shuffle_agent_grid(x, y):
     rows = np.indices((x, y))[0]
-    # cols = np.stack([np.random.permutation(y) for _ in range(x)])
     cols = np.stack([np.arange(y) for _ in range(x)])
     return rows, cols
```

### Comparing `openrl-0.0.3/openrl/cli/__init__.py` & `openrl-0.0.4/openrl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/cli/cli.py` & `openrl-0.0.4/openrl/cli/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 )
 @click.option(
     "--env",
     prompt="Please enter environment name",
     type=str,
     help="RL environment name",
 )
-def run(mode: str, env: str):
+@click.option(
+    "--env_step",
+    type=int,
+    default=20000,
+    help="Maximum collected environment steps for training",
+)
+def run(mode: str, env: str, env_step: int):
     if mode == "train":
         from openrl.cli.train import train_agent
 
-        train_agent(env)
+        train_agent(env, total_time_steps=env_step)
     else:
         raise NotImplementedError
```

### Comparing `openrl-0.0.3/openrl/cli/train.py` & `openrl-0.0.4/openrl/cli/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,30 @@
 
 """"""
 import numpy as np
 
 from openrl.envs.common import make
 from openrl.modules.common import PPONet as Net
 from openrl.runners.common import PPOAgent as Agent
+from openrl.configs.config import create_config_parser
 
 
-def train_agent(env: str):
+def train_agent(env: str, total_time_steps: int = 20000):
     render_model = "rgb_array"
     env_num = 9
     env = make(env, render_mode=render_model, env_num=env_num, asynchronous=True)
+    cfg_parser = create_config_parser()
+    cfg = cfg_parser.parse_args([])
     # 创建 神经网络
-    net = Net(env)
+    net = Net(env, cfg=cfg)
 
     # 初始化训练器
     agent = Agent(net, use_wandb=False)
     # 开始训练
-    agent.train(total_time_steps=20000)
+    agent.train(total_time_steps=total_time_steps)
 
     agent.set_env(env)
     obs, info = env.reset()
     done = False
     step = 0
     total_reward = 0
     while not np.any(done):
```

### Comparing `openrl-0.0.3/openrl/configs/__init__.py` & `openrl-0.0.4/openrl/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/datasets/__init__.py` & `openrl-0.0.4/openrl/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/drivers/__init__.py` & `openrl-0.0.4/openrl/envs/vec_env/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/drivers/onpolicy_driver.py` & `openrl-0.0.4/openrl/drivers/onpolicy_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,79 +40,78 @@
         self.trainer = trainer
         self.buffer = buffer
         self.learner_episode = -1
         self.actor_id = 0
         self.weight_ids = [0]
         self.world_size = world_size
         self.logger = logger
-        args = config["args"]
-        self.program_type = args.program_type
+        cfg = config["cfg"]
+        self.program_type = cfg.program_type
         self.envs = config["envs"]
         self.device = config["device"]
 
         assert not (
             self.program_type != "actor" and self.world_size is None
         ), "world size can not be none, get {}".format(world_size)
 
         self.num_agents = config["num_agents"]
 
-        # print(args)
+        # print(cfg)
         assert isinstance(rank, int), "rank must be int, but get {}".format(rank)
         self.rank = rank
 
         # for distributed learning
         assert not (
             world_size is None and self.program_type == "learner"
         ), "world_size must be int, but get {}".format(world_size)
 
         # parameters
-        self.env_name = args.env_name
-        self.algorithm_name = args.algorithm_name
-        self.experiment_name = args.experiment_name
-
-        self.num_env_steps = args.num_env_steps
-        self.episode_length = args.episode_length
-        self.n_rollout_threads = args.n_rollout_threads
-        self.learner_n_rollout_threads = args.learner_n_rollout_threads
-        self.n_eval_rollout_threads = args.n_eval_rollout_threads
-        self.n_render_rollout_threads = args.n_render_rollout_threads
-        self.use_linear_lr_decay = args.use_linear_lr_decay
-        self.hidden_size = args.hidden_size
-        self.use_wandb = not args.disable_wandb
-        self.use_single_network = args.use_single_network
-        self.use_render = args.use_render
-        self.use_transmit = args.use_transmit
-        self.recurrent_N = args.recurrent_N
-        self.only_eval = args.only_eval
-        # interval
-        self.save_interval = args.save_interval
-        self.use_eval = args.use_eval
-        self.eval_interval = args.eval_interval
-        self.log_interval = args.log_interval
+        self.env_name = cfg.env_name
+        self.algorithm_name = cfg.algorithm_name
+        self.experiment_name = cfg.experiment_name
+
+        self.num_env_steps = cfg.num_env_steps
+        self.episode_length = cfg.episode_length
+        self.n_rollout_threads = cfg.n_rollout_threads
+        self.learner_n_rollout_threads = cfg.learner_n_rollout_threads
+        self.n_eval_rollout_threads = cfg.n_eval_rollout_threads
+        self.n_render_rollout_threads = cfg.n_render_rollout_threads
+        self.use_linear_lr_decay = cfg.use_linear_lr_decay
+        self.hidden_size = cfg.hidden_size
+        self.use_wandb = not cfg.disable_wandb
+        self.use_single_network = cfg.use_single_network
+        self.use_render = cfg.use_render
+        self.use_transmit = cfg.use_transmit
+        self.recurrent_N = cfg.recurrent_N
+        self.only_eval = cfg.only_eval
+        self.save_interval = cfg.save_interval
+        self.use_eval = cfg.use_eval
+        self.eval_interval = cfg.eval_interval
+        self.log_interval = cfg.log_interval
 
-        self.distributed_type = args.distributed_type
+        self.distributed_type = cfg.distributed_type
 
-        self.actor_num = args.actor_num
+        self.actor_num = cfg.actor_num
 
         if self.distributed_type == "async" and self.program_type == "whole":
             print("can't use async mode when program_type is whole!")
             exit()
 
         if self.program_type in ["whole", "local"]:
             assert (
                 self.actor_num == 1
             ), "when running actor and learner the same time, the actor number should be 1, but received {}".format(
                 self.actor_num
             )
         # dir
-        self.model_dir = args.model_dir
-        if hasattr(args, "save_dir"):
-            self.save_dir = args.save_dir
+        self.model_dir = cfg.model_dir
+        if hasattr(cfg, "save_dir"):
+            self.save_dir = cfg.save_dir
 
-        self.args = args
+        self.cfg = cfg
 
     def _inner_loop(
         self,
     ) -> None:
         rollout_infos = self.actor_rollout()
         train_infos = self.learner_update()
         self.buffer.after_update()
@@ -185,16 +184,14 @@
                 action_log_probs,
                 rnn_states,
                 rnn_states_critic,
             ) = self.act(step)
 
             obs, rewards, dones, infos = self.envs.step(actions)
 
-            # print(obs["policy"][0][0])
-            # exit()
             data = (
                 obs,
                 rewards,
                 dones,
                 infos,
                 values,
                 actions,
@@ -267,16 +264,14 @@
         self.buffer.compute_returns(next_values, value_normalizer)
 
     @torch.no_grad()
     def act(
         self,
         step: int,
     ):
-        # print("get_bach:", self.buffer.data.get_batch_data("critic_obs", step))
-        # exit()
         self.trainer.prep_rollout()
 
         (
             value,
             action,
             action_log_prob,
             rnn_states,
```

### Comparing `openrl-0.0.3/openrl/drivers/rl_driver.py` & `openrl-0.0.4/openrl/drivers/rl_driver.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/common/__init__.py` & `openrl-0.0.4/openrl/envs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/common/registration.py` & `openrl-0.0.4/openrl/envs/common/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     AsyncVectorEnv,
     VecMonitor,
 )
 
 
 def make(
     id: str,
+    cfg=None,
     env_num: int = 1,
     asynchronous: bool = False,
     add_monitor: bool = True,
     render_mode: Optional[str] = None,
     **kwargs,
 ) -> Env:
     if render_mode in [None, "human", "rgb_array"]:
```

### Comparing `openrl-0.0.3/openrl/envs/gymnasium/__init__.py` & `openrl-0.0.4/openrl/envs/gymnasium/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/mpe/__init__.py` & `openrl-0.0.4/openrl/envs/mpe/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,9 @@
         make=make,
         id=id,
         env_num=env_num,
         render_mode=render_mode,
         wrappers=env_wrappers,
         **kwargs,
     )
+
     return env_fns
```

### Comparing `openrl-0.0.3/openrl/envs/mpe/core.py` & `openrl-0.0.4/openrl/envs/mpe/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import seaborn as sns
 
 
 # physical/external base state of all entites
 class EntityState(object):
     def __init__(self):
         # physical position
         self.p_pos = None
```

### Comparing `openrl-0.0.3/openrl/envs/mpe/mpe_env.py` & `openrl-0.0.4/openrl/envs/mpe/mpe_env.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/mpe/multi_discrete.py` & `openrl-0.0.4/openrl/envs/mpe/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/mpe/multiagent_env.py` & `openrl-0.0.4/openrl/envs/mpe/multiagent_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,14 @@
         else:
             self.viewers = [None] * self.n
         self._reset_render()
 
     def seed(self, seed=None):
         if seed is not None:
             self._np_random, seed = seeding.np_random(seed)
-        # if seed is not None:
-        #     np.random.seed(seed)
 
     # step  this is  env.step()
     def step(self, action_n):
         self.current_step += 1
         obs_n = []
         reward_n = []
         done_n = []
@@ -193,16 +191,15 @@
         reward = np.sum(reward_n)
         if self.shared_reward:
             reward_n = [[reward]] * self.n
 
         if self.post_step_callback is not None:
             self.post_step_callback(self.world)
         self.deal_render()
-        # print("obs0:", obs_n[0])
-        # exit()
+
         return self.construct_obs(obs_n), reward_n, done_n, info_n
 
     def deal_render(self):
         if self.render_mode in [None, "rgb_array"]:
             return
         elif self.render_mode == "human":
             self.render("human")
```

### Comparing `openrl-0.0.3/openrl/envs/mpe/rendering.py` & `openrl-0.0.4/openrl/envs/mpe/rendering.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/mpe/scenarios/simple_spread.py` & `openrl-0.0.4/openrl/envs/mpe/scenarios/simple_spread.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/async_venv.py` & `openrl-0.0.4/openrl/envs/vec_env/async_venv.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,15 @@
             raise AlreadyPendingCallError(
                 "Calling `call_send` while waiting "
                 f"for a pending call to `{self._state.value}` to complete.",
                 str(self._state.value),
             )
 
         for pipe in self.parent_pipes:
-            pipe.send(("_call", (name, args, kwargs)))
+            pipe.send(("_call", (name, cfg, kwargs)))
         self._state = AsyncState.WAITING_CALL
 
     def call_fetch(self, timeout: Union[int, float, None] = None) -> list:
         """Calls all parent pipes and waits for the results.
 
         Args:
             timeout: Number of seconds before the call to `step_fetch` times out.
@@ -757,15 +757,15 @@
                 pipe.send(
                     (
                         (data[0] == observation_space, data[1] == action_space),
                         True,
                     )
                 )
             elif command == "_call":
-                name, args, kwargs = data
+                name, cfg, kwargs = data
                 if name in ["reset", "step", "seed", "close"]:
                     raise ValueError(
                         f"Trying to call function `{name}` with "
                         f"`_call`. Use `{name}` directly instead."
                     )
                 function = getattr(env, name)
                 if callable(function):
```

### Comparing `openrl-0.0.3/openrl/envs/vec_env/base_venv.py` & `openrl-0.0.4/openrl/envs/vec_env/base_venv.py`

 * *Files 5% similar despite different names*

```diff
@@ -253,7 +253,18 @@
 
         Args:
             name (str): Name of the property to be set in each individual environment.
             values (list, tuple, or object): Values of the property to be set to. If `values` is a list or
                 tuple, then it corresponds to the values for each individual environment, otherwise a single value
                 is set for all environments.
         """
+
+    def random_action(self):
+        """
+        Get a random action from the action space
+        """
+        return np.array(
+            [
+                [[self.action_space.sample()] for _ in range(self.agent_num)]
+                for _ in range(self.parallel_env_num)
+            ]
+        )
```

### Comparing `openrl-0.0.3/openrl/envs/vec_env/sync_venv.py` & `openrl-0.0.4/openrl/envs/vec_env/sync_venv.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,14 +174,15 @@
 
         Returns:
             The batched environment step results
         """
         _actions = iterate_action(self.action_space, actions)
 
         observations, infos = [], []
+
         for i, (env, action) in enumerate(zip(self.envs, _actions)):
             returns = env.step(action)
             assert isinstance(
                 returns, tuple
             ), "step return must be tuple, but got: {}".format(type(returns))
 
             _need_reset = not self._subenv_auto_reset
```

### Comparing `openrl-0.0.3/openrl/envs/vec_env/utils/__init__.py` & `openrl-0.0.4/openrl/envs/vec_env/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/utils/numpy_utils.py` & `openrl-0.0.4/openrl/envs/vec_env/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/utils/share_memory.py` & `openrl-0.0.4/openrl/envs/vec_env/utils/share_memory.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/utils/util.py` & `openrl-0.0.4/openrl/envs/vec_env/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/wrappers/__init__.py` & `openrl-0.0.4/openrl/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/vec_env/wrappers/base_wrapper.py` & `openrl-0.0.4/openrl/envs/vec_env/wrappers/base_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,31 +106,16 @@
         self._metadata = value
 
     @property
     def render_mode(self) -> Optional[str]:
         """Returns the :attr:`Env` :attr:`render_mode`."""
         return self.env.render_mode
 
-    # def step(
-    #     self, actions: ActType
-    # ) -> Tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
-    #     """Take an action for each parallel environment.
-    #
-    #     Args:
-    #         actions: element of :attr:`action_space` Batch of actions.
-    #
-    #     Returns:
-    #         Batch of (observations, rewards, terminations, truncations, infos)
-    #
-    #     Note:
-    #         As the vector environments autoreset for a terminating and truncating sub-environments,
-    #         the returned observation and info is not the final step's observation or info which is instead stored in
-    #         info as `"final_observation"` and `"final_info"`.
-    #     """
-    #     pass
+    def random_action(self):
+        return self.env.random_action()
 
     def reset(self, **kwargs):
         """Reset all environments."""
         return self.env.reset(**kwargs)
 
     def step(self, actions):
         """Step all environments."""
```

### Comparing `openrl-0.0.3/openrl/envs/vec_env/wrappers/vec_monitor.py` & `openrl-0.0.4/openrl/envs/vec_env/wrappers/vec_monitor.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/wrappers/base_wrapper.py` & `openrl-0.0.4/openrl/envs/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/wrappers/multiagent_wrapper.py` & `openrl-0.0.4/openrl/envs/wrappers/multiagent_wrapper.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/envs/wrappers/util.py` & `openrl-0.0.4/openrl/envs/wrappers/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/__init__.py` & `openrl-0.0.4/openrl/modules/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/base_module.py` & `openrl-0.0.4/openrl/modules/base_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 """"""
 from abc import ABC, abstractmethod
 
 import torch
 from torch.nn.parallel import DistributedDataParallel as DDP
 
+
 class BaseModule(ABC):
-    def __init__(self, args) -> None:
-        self.args = args
+    def __init__(self, cfg) -> None:
+        self.cfg = cfg
         self.models = {}
         self.optimizers = {}
 
     @abstractmethod
     def lr_decay(self, episode: int, episodes: int) -> None:
         raise NotImplementedError
```

### Comparing `openrl-0.0.3/openrl/modules/common/base_net.py` & `openrl-0.0.4/openrl/modules/common/base_net.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/common/ppo_net.py` & `openrl-0.0.4/openrl/modules/common/ppo_net.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,64 +19,64 @@
 from typing import Union, Tuple, Dict, Optional
 
 import numpy as np
 import gym
 import torch
 
 from openrl.modules.ppo_module import PPOModule
-from openrl.configs.config import build_parser
+from openrl.configs.config import create_config_parser
 from openrl.modules.common.base_net import BaseNet
 from openrl.utils.util import set_seed
 
 
 class PPONet(BaseNet):
     def __init__(
         self,
         env: Union[gym.Env, str],
+        cfg=None,
         device: Union[torch.device, str] = "cpu",
         n_rollout_threads: int = 1,
-        args=None,
     ) -> None:
         super().__init__()
 
-        if args is None:
-            parser = build_parser()
-            args = parser.parse_args()
-
-        set_seed(args.seed)
-        env.reset(seed=args.seed)
-
-        args.n_rollout_threads = n_rollout_threads
-        args.learner_n_rollout_threads = args.n_rollout_threads
-
-        if args.rnn_type == "gru":
-            rnn_hidden_size = args.hidden_size
-        elif args.rnn_type == "lstm":
-            rnn_hidden_size = args.hidden_size * 2
+        if cfg is None:
+            cfg_parser = create_config_parser()
+            cfg = cfg_parser.parse_args()
+
+        set_seed(cfg.seed)
+        env.reset(seed=cfg.seed)
+
+        cfg.n_rollout_threads = n_rollout_threads
+        cfg.learner_n_rollout_threads = cfg.n_rollout_threads
+
+        if cfg.rnn_type == "gru":
+            rnn_hidden_size = cfg.hidden_size
+        elif cfg.rnn_type == "lstm":
+            rnn_hidden_size = cfg.hidden_size * 2
         else:
             raise NotImplementedError(
-                f"RNN type {args.rnn_type} has not been implemented."
+                f"RNN type {cfg.rnn_type} has not been implemented."
             )
-        args.rnn_hidden_size = rnn_hidden_size
+        cfg.rnn_hidden_size = rnn_hidden_size
 
         if isinstance(device, str):
             device = torch.device(device)
 
         self.module = PPOModule(
-            args=args,
+            cfg=cfg,
             policy_input_space=env.observation_space,
             critic_input_space=env.observation_space,
             act_space=env.action_space,
             share_model=False,
             device=device,
             rank=0,
             world_size=1,
         )
 
-        self.args = args
+        self.cfg = cfg
         self.env = env
         self.device = device
         self.rnn_states_actor = None
         self.masks = None
 
     def act(
         self,
@@ -95,12 +95,15 @@
         )
 
         return actions, self.rnn_states_actor
 
     def reset(self):
         self.first_reset = False
         self.rnn_states_actor, self.masks = self.module.init_rnn_states(
-            rollout_num=self.args.n_rollout_threads,
+            rollout_num=self.cfg.n_rollout_threads,
             agent_num=self.env.agent_num,
-            rnn_layers=self.args.recurrent_N,
-            hidden_size=self.args.rnn_hidden_size,
+            rnn_layers=self.cfg.recurrent_N,
+            hidden_size=self.cfg.rnn_hidden_size,
         )
+
+    def load_policy(self, path: str) -> None:
+        self.module.load_policy(path)
```

### Comparing `openrl-0.0.3/openrl/modules/model_config.py` & `openrl-0.0.4/openrl/modules/model_config.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/__init__.py` & `openrl-0.0.4/openrl/modules/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/base_policy_network.py` & `openrl-0.0.4/openrl/modules/networks/base_policy_network.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 """"""
 import torch.nn as nn
 
 from openrl.modules.utils.valuenorm import ValueNorm
 
 
 class BasePolicyNetwork(nn.Module):
-    def __init__(self, args, device):
+    def __init__(self, cfg, device):
         super(BasePolicyNetwork, self).__init__()
         self.device = device
-        self._use_valuenorm = args.use_valuenorm
-        self._use_policy_vhead = args.use_policy_vhead
+        self._use_valuenorm = cfg.use_valuenorm
+        self._use_policy_vhead = cfg.use_policy_vhead
 
         if self._use_valuenorm:
             if self._use_policy_vhead:
                 self.policy_value_normalizer = ValueNorm(1, device=self.device)
         else:
             if self._use_policy_vhead:
                 self.policy_value_normalizer = None
```

### Comparing `openrl-0.0.3/openrl/modules/networks/base_value_network.py` & `openrl-0.0.4/openrl/modules/networks/base_value_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from abc import ABC, abstractmethod
 import torch.nn as nn
 
 from openrl.modules.utils.valuenorm import ValueNorm
 
 
 class BaseValueNetwork(ABC, nn.Module):
-    def __init__(self, args, device):
+    def __init__(self, cfg, device):
         super(BaseValueNetwork, self).__init__()
         self.device = device
-        self._use_valuenorm = args.use_valuenorm
+        self._use_valuenorm = cfg.use_valuenorm
 
         if self._use_valuenorm:
             self.value_normalizer = ValueNorm(1, device=self.device)
         else:
             self.value_normalizer = None
 
     @abstractmethod
```

### Comparing `openrl-0.0.3/openrl/modules/networks/policy_network.py` & `openrl-0.0.4/openrl/modules/networks/policy_network.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,65 +29,65 @@
 from openrl.modules.networks.base_policy_network import BasePolicyNetwork
 from openrl.utils.util import check_v2 as check
 
 
 class PolicyNetwork(BasePolicyNetwork):
     def __init__(
         self,
-        args,
+        cfg,
         input_space,
         action_space,
         device=torch.device("cpu"),
         use_half=False,
     ) -> None:
-        super(PolicyNetwork, self).__init__(args, device)
-        self.hidden_size = args.hidden_size
+        super(PolicyNetwork, self).__init__(cfg, device)
+        self.hidden_size = cfg.hidden_size
 
-        self._gain = args.gain
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._use_policy_active_masks = args.use_policy_active_masks
-        self._use_naive_recurrent_policy = args.use_naive_recurrent_policy
-        self._use_recurrent_policy = args.use_recurrent_policy
-        self._use_influence_policy = args.use_influence_policy
-        self._influence_layer_N = args.influence_layer_N
-        self._use_policy_vhead = args.use_policy_vhead
-        self._recurrent_N = args.recurrent_N
+        self._gain = cfg.gain
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._use_policy_active_masks = cfg.use_policy_active_masks
+        self._use_naive_recurrent_policy = cfg.use_naive_recurrent_policy
+        self._use_recurrent_policy = cfg.use_recurrent_policy
+        self._use_influence_policy = cfg.use_influence_policy
+        self._influence_layer_N = cfg.influence_layer_N
+        self._use_policy_vhead = cfg.use_policy_vhead
+        self._recurrent_N = cfg.recurrent_N
         self.use_half = use_half
         self.tpdv = dict(dtype=torch.float32, device=device)
 
         policy_obs_shape = get_policy_obs_space(input_space)
 
         if "Dict" in policy_obs_shape.__class__.__name__:
             self._mixed_obs = True
             self.base = MIXBase(
-                args, policy_obs_shape, cnn_layers_params=args.cnn_layers_params
+                cfg, policy_obs_shape, cnn_layers_params=cfg.cnn_layers_params
             )
         else:
             self._mixed_obs = False
             self.base = (
-                CNNBase(args, policy_obs_shape)
+                CNNBase(cfg, policy_obs_shape)
                 if len(policy_obs_shape) == 3
                 else MLPBase(
-                    args,
+                    cfg,
                     policy_obs_shape,
-                    use_attn_internal=args.use_attn_internal,
+                    use_attn_internal=cfg.use_attn_internal,
                     use_cat_self=True,
                 )
             )
 
         input_size = self.base.output_size
 
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
             self.rnn = RNNLayer(
                 input_size,
                 self.hidden_size,
                 self._recurrent_N,
                 self._use_orthogonal,
-                rnn_type=args.rnn_type,
+                rnn_type=cfg.rnn_type,
             )
             input_size = self.hidden_size
 
         if self._use_influence_policy:
             self.mlp = MLPLayer(
                 policy_obs_shape[0],
                 self.hidden_size,
```

### Comparing `openrl-0.0.3/openrl/modules/networks/policy_value_network.py` & `openrl-0.0.4/openrl/modules/networks/policy_value_network.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,61 +28,61 @@
 from openrl.utils.util import check_v2 as check
 from openrl.buffers.utils.util import get_policy_obs_space, get_critic_obs_space
 
 
 class PolicyValueNetwork(nn.Module):
     def __init__(
         self,
-        args,
+        cfg,
         obs_space,
         critic_obs_space,
         action_space,
         device=torch.device("cpu"),
         use_half=False,
     ):
         super(PolicyValueNetwork, self).__init__()
-        self._gain = args.gain
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._recurrent_N = args.recurrent_N
-        self._use_naive_recurrent_policy = args.use_naive_recurrent_policy
-        self._use_recurrent_policy = args.use_recurrent_policy
-        self._concat_obs_as_critic_obs = args.concat_obs_as_critic_obs
-        self._use_popart = args.use_popart
-        self.hidden_size = args.hidden_size
+        self._gain = cfg.gain
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._recurrent_N = cfg.recurrent_N
+        self._use_naive_recurrent_policy = cfg.use_naive_recurrent_policy
+        self._use_recurrent_policy = cfg.use_recurrent_policy
+        self._concat_obs_as_critic_obs = cfg.concat_obs_as_critic_obs
+        self._use_popart = cfg.use_popart
+        self.hidden_size = cfg.hidden_size
         self.device = device
         self.use_half = use_half
         self.tpdv = dict(dtype=torch.float32, device=device)
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][
             self._use_orthogonal
         ]
 
         # obs space
         policy_obs_shape = get_policy_obs_space(obs_space)
 
         self.obs_prep = (
-            CNNBase(args, policy_obs_shape)
+            CNNBase(cfg, policy_obs_shape)
             if len(policy_obs_shape) == 3
             else MLPBase(
-                args,
+                cfg,
                 policy_obs_shape,
-                use_attn_internal=args.use_attn_internal,
+                use_attn_internal=cfg.use_attn_internal,
                 use_cat_self=True,
             )
         )
 
         # critic_obs_shape = get_critic_obs_space(critic_obs_space)
         # self.critic_obs_prep = (
-        #     CNNBase(args, critic_obs_shape)
+        #     CNNBase(cfg, critic_obs_shape)
         #     if len(critic_obs_shape) == 3
         #     else MLPBase(
-        #         args,
+        #         cfg,
         #         critic_obs_shape,
         #         use_attn_internal=True,
-        #         use_cat_self=args.use_cat_self,
+        #         use_cat_self=cfg.use_cat_self,
         #     )
         # )
         #
         self.critic_obs_prep = self.obs_prep
 
         # common layer
         self.common = MLPLayer(
```

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/act.py` & `openrl-0.0.4/openrl/modules/networks/utils/act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/attention.py` & `openrl-0.0.4/openrl/modules/networks/utils/attention.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,34 +3,51 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .util import init, get_clones
 
+
 class Encoder(nn.Module):
-    def __init__(self, args, split_shape, cat_self=True):
+    def __init__(self, cfg, split_shape, cat_self=True):
         super(Encoder, self).__init__()
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._attn_N = args.attn_N
-        self._attn_size = args.attn_size
-        self._attn_heads = args.attn_heads
-        self._dropout = args.dropout
-        self._use_average_pool = args.use_average_pool
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._attn_N = cfg.attn_N
+        self._attn_size = cfg.attn_size
+        self._attn_heads = cfg.attn_heads
+        self._dropout = cfg.dropout
+        self._use_average_pool = cfg.use_average_pool
         self._cat_self = cat_self
         if self._cat_self:
             self.embedding = CatSelfEmbedding(
-                split_shape[1:], self._attn_size, self._use_orthogonal, self._activation_id)
+                split_shape[1:],
+                self._attn_size,
+                self._use_orthogonal,
+                self._activation_id,
+            )
         else:
             self.embedding = Embedding(
-                split_shape[1:], self._attn_size, self._use_orthogonal, self._activation_id)
-
-        self.layers = get_clones(EncoderLayer(
-            self._attn_size, self._attn_heads, self._dropout, self._use_orthogonal, self._activation_id), self._attn_N)
+                split_shape[1:],
+                self._attn_size,
+                self._use_orthogonal,
+                self._activation_id,
+            )
+
+        self.layers = get_clones(
+            EncoderLayer(
+                self._attn_size,
+                self._attn_heads,
+                self._dropout,
+                self._use_orthogonal,
+                self._activation_id,
+            ),
+            self._attn_N,
+        )
         self.norm = nn.LayerNorm(self._attn_size)
 
     def forward(self, x, self_idx=-1, mask=None):
         x, self_x = self.embedding(x, self_idx)
         for i in range(self._attn_N):
             x = self.layers[i](x, mask)
         x = self.norm(x)
@@ -45,32 +62,38 @@
 
 # [L,[1,2],[1,2],[1,2]]
 def split_obs(obs, split_shape):
     start_idx = 0
     split_obs = []
     for i in range(len(split_shape)):
         split_obs.append(
-            obs[:, start_idx:(start_idx+split_shape[i][0]*split_shape[i][1])])
-        start_idx += split_shape[i][0]*split_shape[i][1]
+            obs[:, start_idx : (start_idx + split_shape[i][0] * split_shape[i][1])]
+        )
+        start_idx += split_shape[i][0] * split_shape[i][1]
     return split_obs
 
 
 class FeedForward(nn.Module):
-    def __init__(self, d_model, d_ff=512, dropout=0.0, use_orthogonal=True, activation_id=1):
+    def __init__(
+        self, d_model, d_ff=512, dropout=0.0, use_orthogonal=True, activation_id=1
+    ):
         super(FeedForward, self).__init__()
         # We set d_ff as a default to 2048
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        gain = nn.init.calculate_gain(['tanh', 'relu', 'leaky_relu', 'leaky_relu'][activation_id])
+        gain = nn.init.calculate_gain(
+            ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
+        )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         self.linear_1 = nn.Sequential(
-            init_(nn.Linear(d_model, d_ff)), active_func, nn.LayerNorm(d_ff))
+            init_(nn.Linear(d_model, d_ff)), active_func, nn.LayerNorm(d_ff)
+        )
 
         self.dropout = nn.Dropout(dropout)
         self.linear_2 = init_(nn.Linear(d_ff, d_model))
 
     def forward(self, x):
         x = self.dropout(self.linear_1(x))
         x = self.linear_2(x)
@@ -90,15 +113,15 @@
     output = torch.matmul(scores, v)
     return output
 
 
 class MultiHeadAttention(nn.Module):
     def __init__(self, heads, d_model, dropout=0.0, use_orthogonal=True):
         super(MultiHeadAttention, self).__init__()
-        
+
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0))
 
         self.d_model = d_model
         self.d_k = d_model // heads
@@ -107,43 +130,49 @@
         self.q_linear = init_(nn.Linear(d_model, d_model))
         self.v_linear = init_(nn.Linear(d_model, d_model))
         self.k_linear = init_(nn.Linear(d_model, d_model))
         self.dropout = nn.Dropout(dropout)
         self.out = init_(nn.Linear(d_model, d_model))
 
     def forward(self, q, k, v, mask=None):
-
         bs = q.size(0)
 
         # perform linear operation and split into h heads
 
         k = self.k_linear(k).view(bs, -1, self.h, self.d_k)
         q = self.q_linear(q).view(bs, -1, self.h, self.d_k)
         v = self.v_linear(v).view(bs, -1, self.h, self.d_k)
 
         # transpose to get dimensions bs * h * sl * d_model
 
         k = k.transpose(1, 2)
         q = q.transpose(1, 2)
         v = v.transpose(1, 2)
         # calculate attention
-        scores = ScaledDotProductAttention(
-            q, k, v, self.d_k, mask, self.dropout)
+        scores = ScaledDotProductAttention(q, k, v, self.d_k, mask, self.dropout)
 
         # concatenate heads and put through final linear layer
-        concat = scores.transpose(1, 2).contiguous()\
-            .view(bs, -1, self.d_model)
+        concat = scores.transpose(1, 2).contiguous().view(bs, -1, self.d_model)
 
         output = self.out(concat)
 
         return output
 
 
 class EncoderLayer(nn.Module):
-    def __init__(self, d_model, heads, dropout=0.0, use_orthogonal=True, activation_id=False, d_ff=512, use_FF=False):
+    def __init__(
+        self,
+        d_model,
+        heads,
+        dropout=0.0,
+        use_orthogonal=True,
+        activation_id=False,
+        d_ff=512,
+        use_FF=False,
+    ):
         super(EncoderLayer, self).__init__()
         self._use_FF = use_FF
         self.norm_1 = nn.LayerNorm(d_model)
         self.norm_2 = nn.LayerNorm(d_model)
         self.attn = MultiHeadAttention(heads, d_model, dropout, use_orthogonal)
         self.ff = FeedForward(d_model, d_ff, dropout, use_orthogonal, activation_id)
         self.dropout_1 = nn.Dropout(dropout)
@@ -161,75 +190,101 @@
 class CatSelfEmbedding(nn.Module):
     def __init__(self, split_shape, d_model, use_orthogonal=True, activation_id=1):
         super(CatSelfEmbedding, self).__init__()
         self.split_shape = split_shape
 
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        gain = nn.init.calculate_gain(['tanh', 'relu', 'leaky_relu', 'leaky_relu'][activation_id])
+        gain = nn.init.calculate_gain(
+            ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
+        )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         for i in range(len(split_shape)):
-            if i == (len(split_shape)-1):
-                setattr(self, 'fc_'+str(i), nn.Sequential(init_(
-                    nn.Linear(split_shape[i][1], d_model)), active_func, nn.LayerNorm(d_model)))
+            if i == (len(split_shape) - 1):
+                setattr(
+                    self,
+                    "fc_" + str(i),
+                    nn.Sequential(
+                        init_(nn.Linear(split_shape[i][1], d_model)),
+                        active_func,
+                        nn.LayerNorm(d_model),
+                    ),
+                )
             else:
-                setattr(self, 'fc_'+str(i), nn.Sequential(init_(nn.Linear(
-                    split_shape[i][1]+split_shape[-1][1], d_model)), active_func, nn.LayerNorm(d_model)))
+                setattr(
+                    self,
+                    "fc_" + str(i),
+                    nn.Sequential(
+                        init_(
+                            nn.Linear(split_shape[i][1] + split_shape[-1][1], d_model)
+                        ),
+                        active_func,
+                        nn.LayerNorm(d_model),
+                    ),
+                )
 
     def forward(self, x, self_idx=-1):
         x = split_obs(x, self.split_shape)
         N = len(x)
 
         x1 = []
         self_x = x[self_idx]
-        for i in range(N-1):
+        for i in range(N - 1):
             K = self.split_shape[i][0]
             L = self.split_shape[i][1]
             for j in range(K):
-                temp = torch.cat((x[i][:, (L*j):(L*j+L)], self_x), dim=-1)
-                exec('x1.append(self.fc_{}(temp))'.format(i))
+                temp = torch.cat((x[i][:, (L * j) : (L * j + L)], self_x), dim=-1)
+                exec("x1.append(self.fc_{}(temp))".format(i))
         temp = x[self_idx]
-        exec('x1.append(self.fc_{}(temp))'.format(N-1))
+        exec("x1.append(self.fc_{}(temp))".format(N - 1))
 
         out = torch.stack(x1, 1)
 
         return out, self_x
 
 
 class Embedding(nn.Module):
     def __init__(self, split_shape, d_model, use_orthogonal=True, activation_id=1):
         super(Embedding, self).__init__()
         self.split_shape = split_shape
 
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        gain = nn.init.calculate_gain(['tanh', 'relu', 'leaky_relu', 'leaky_relu'][activation_id])
+        gain = nn.init.calculate_gain(
+            ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
+        )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         for i in range(len(split_shape)):
-            setattr(self, 'fc_'+str(i), nn.Sequential(init_(
-                nn.Linear(split_shape[i][1], d_model)), active_func, nn.LayerNorm(d_model)))
+            setattr(
+                self,
+                "fc_" + str(i),
+                nn.Sequential(
+                    init_(nn.Linear(split_shape[i][1], d_model)),
+                    active_func,
+                    nn.LayerNorm(d_model),
+                ),
+            )
 
     def forward(self, x, self_idx=None):
         x = split_obs(x, self.split_shape)
         N = len(x)
 
         x1 = []
         for i in range(N):
             K = self.split_shape[i][0]
             L = self.split_shape[i][1]
             for j in range(K):
-                temp = x[i][:, (L*j):(L*j+L)]
-                exec('x1.append(self.fc_{}(temp))'.format(i))
+                temp = x[i][:, (L * j) : (L * j + L)]
+                exec("x1.append(self.fc_{}(temp))".format(i))
 
         out = torch.stack(x1, 1)
 
         if self_idx is None:
             return out, None
         else:
             return out, x[self_idx]
-
```

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/distributed_utils.py` & `openrl-0.0.4/openrl/modules/networks/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/distributions.py` & `openrl-0.0.4/openrl/modules/networks/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/mix.py` & `openrl-0.0.4/openrl/modules/networks/utils/mix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 import numpy as np
 
 import torch
 import torch.nn as nn
 
 from .util import init
 
+
 class Flatten(nn.Module):
     def forward(self, x):
         return x.reshape(x.size(0), -1)
 
+
 class MIXBase(nn.Module):
-    def __init__(self, args, obs_shape, cnn_layers_params=None):
+    def __init__(self, cfg, obs_shape, cnn_layers_params=None):
         super(MIXBase, self).__init__()
 
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._use_maxpool2d = args.use_maxpool2d
-        self.hidden_size = args.hidden_size
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._use_maxpool2d = cfg.use_maxpool2d
+        self.hidden_size = cfg.hidden_size
         self.cnn_keys = []
         self.embed_keys = []
         self.mlp_keys = []
         self.n_cnn_input = 0
         self.n_embed_input = 0
         self.n_mlp_input = 0
 
         for key in obs_shape:
-            if obs_shape[key].__class__.__name__ == 'Box':
+            if obs_shape[key].__class__.__name__ == "Box":
                 key_obs_shape = obs_shape[key].shape
                 if len(key_obs_shape) == 3:
                     self.cnn_keys.append(key)
                 else:
                     if "orientation" in key:
                         self.embed_keys.append(key)
                     else:
                         self.mlp_keys.append(key)
             else:
                 raise NotImplementedError
 
         if len(self.cnn_keys) > 0:
-            self.cnn = self._build_cnn_model(obs_shape, cnn_layers_params, self.hidden_size, self._use_orthogonal, self._activation_id)
+            self.cnn = self._build_cnn_model(
+                obs_shape,
+                cnn_layers_params,
+                self.hidden_size,
+                self._use_orthogonal,
+                self._activation_id,
+            )
         if len(self.embed_keys) > 0:
             self.embed = self._build_embed_model(obs_shape)
         if len(self.mlp_keys) > 0:
-            self.mlp = self._build_mlp_model(obs_shape, self.hidden_size, self._use_orthogonal, self._activation_id)
+            self.mlp = self._build_mlp_model(
+                obs_shape, self.hidden_size, self._use_orthogonal, self._activation_id
+            )
 
     def forward(self, x):
         out_x = None
         if len(self.cnn_keys) > 0:
             cnn_input = self._build_cnn_input(x)
             out_x = self.cnn(cnn_input)
 
@@ -58,86 +68,111 @@
             else:
                 out_x = embed_x
         if len(self.mlp_keys) > 0:
             mlp_input = self._build_mlp_input(x)
             mlp_x = self.mlp(mlp_input).view(mlp_input.size(0), -1)
 
             if out_x is not None:
-                out_x = torch.cat([out_x, mlp_x], dim=1) # ! wrong
+                out_x = torch.cat([out_x, mlp_x], dim=1)  # ! wrong
             else:
                 out_x = mlp_x
         return out_x
 
-    def _build_cnn_model(self, obs_shape, cnn_layers_params, hidden_size, use_orthogonal, activation_id):
-        
+    def _build_cnn_model(
+        self, obs_shape, cnn_layers_params, hidden_size, use_orthogonal, activation_id
+    ):
         if cnn_layers_params is None:
             cnn_layers_params = [(32, 8, 4, 0), (64, 4, 2, 0), (64, 3, 1, 0)]
         else:
+
             def _convert(params):
                 output = []
-                for l in params.split(' '):
-                    output.append(tuple(map(int, l.split(','))))
+                for l in params.split(" "):
+                    output.append(tuple(map(int, l.split(","))))
                 return output
+
             cnn_layers_params = _convert(cnn_layers_params)
-        
+
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        gain = nn.init.calculate_gain(['tanh', 'relu', 'leaky_relu', 'leaky_relu'][activation_id])
+        gain = nn.init.calculate_gain(
+            ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
+        )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         for key in self.cnn_keys:
-            if key in ['rgb','depth','image','occupy_image']:
-                self.n_cnn_input += obs_shape[key].shape[2] 
+            if key in ["rgb", "depth", "image", "occupy_image"]:
+                self.n_cnn_input += obs_shape[key].shape[2]
                 cnn_dims = np.array(obs_shape[key].shape[:2], dtype=np.float32)
-            elif key in ['global_map','local_map','global_obs','global_merge_obs','global_merge_goal','gt_map']:
-                self.n_cnn_input += obs_shape[key].shape[0] 
+            elif key in [
+                "global_map",
+                "local_map",
+                "global_obs",
+                "global_merge_obs",
+                "global_merge_goal",
+                "gt_map",
+            ]:
+                self.n_cnn_input += obs_shape[key].shape[0]
                 cnn_dims = np.array(obs_shape[key].shape[1:3], dtype=np.float32)
             else:
                 raise NotImplementedError
 
         cnn_layers = []
         prev_out_channels = None
-        for i, (out_channels, kernel_size, stride, padding) in enumerate(cnn_layers_params):
+        for i, (out_channels, kernel_size, stride, padding) in enumerate(
+            cnn_layers_params
+        ):
             if self._use_maxpool2d and i != len(cnn_layers_params) - 1:
                 cnn_layers.append(nn.MaxPool2d(2))
 
             if i == 0:
                 in_channels = self.n_cnn_input
             else:
                 in_channels = prev_out_channels
 
-            cnn_layers.append(init_(nn.Conv2d(in_channels=in_channels,
-                                            out_channels=out_channels,
-                                            kernel_size=kernel_size,
-                                            stride=stride,
-                                            padding=padding,)))
-            #if i != len(cnn_layers_params) - 1:
+            cnn_layers.append(
+                init_(
+                    nn.Conv2d(
+                        in_channels=in_channels,
+                        out_channels=out_channels,
+                        kernel_size=kernel_size,
+                        stride=stride,
+                        padding=padding,
+                    )
+                )
+            )
+            # if i != len(cnn_layers_params) - 1:
             cnn_layers.append(active_func)
             prev_out_channels = out_channels
 
         for i, (_, kernel_size, stride, padding) in enumerate(cnn_layers_params):
             if self._use_maxpool2d and i != len(cnn_layers_params) - 1:
-                cnn_dims = self._maxpool_output_dim(dimension=cnn_dims,
-                dilation=np.array([1, 1], dtype=np.float32),
-                kernel_size=np.array([2, 2], dtype=np.float32),
-                stride=np.array([2, 2], dtype=np.float32))
+                cnn_dims = self._maxpool_output_dim(
+                    dimension=cnn_dims,
+                    dilation=np.array([1, 1], dtype=np.float32),
+                    kernel_size=np.array([2, 2], dtype=np.float32),
+                    stride=np.array([2, 2], dtype=np.float32),
+                )
             cnn_dims = self._cnn_output_dim(
                 dimension=cnn_dims,
                 padding=np.array([padding, padding], dtype=np.float32),
                 dilation=np.array([1, 1], dtype=np.float32),
                 kernel_size=np.array([kernel_size, kernel_size], dtype=np.float32),
                 stride=np.array([stride, stride], dtype=np.float32),
             )
-            
+
         cnn_layers += [
             Flatten(),
-            init_(nn.Linear(cnn_layers_params[-1][0] * cnn_dims[0] * cnn_dims[1],
-                        hidden_size)),
+            init_(
+                nn.Linear(
+                    cnn_layers_params[-1][0] * cnn_dims[0] * cnn_dims[1], hidden_size
+                )
+            ),
             active_func,
             nn.LayerNorm(hidden_size),
         ]
         return nn.Sequential(*cnn_layers)
 
     def _build_embed_model(self, obs_shape):
         self.embed_dim = 0
@@ -145,65 +180,93 @@
             self.n_embed_input = 72
             self.n_embed_output = 8
             self.embed_dim += np.prod(obs_shape[key].shape)
 
         return nn.Embedding(self.n_embed_input, self.n_embed_output)
 
     def _build_mlp_model(self, obs_shape, hidden_size, use_orthogonal, activation_id):
-
         active_func = [nn.Tanh(), nn.ReLU(), nn.LeakyReLU(), nn.ELU()][activation_id]
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][use_orthogonal]
-        gain = nn.init.calculate_gain(['tanh', 'relu', 'leaky_relu', 'leaky_relu'][activation_id])
+        gain = nn.init.calculate_gain(
+            ["tanh", "relu", "leaky_relu", "leaky_relu"][activation_id]
+        )
 
         def init_(m):
             return init(m, init_method, lambda x: nn.init.constant_(x, 0), gain=gain)
 
         for key in self.mlp_keys:
             self.n_mlp_input += np.prod(obs_shape[key].shape)
 
         return nn.Sequential(
-                    init_(nn.Linear(self.n_mlp_input, hidden_size)), active_func, nn.LayerNorm(hidden_size))
-         
+            init_(nn.Linear(self.n_mlp_input, hidden_size)),
+            active_func,
+            nn.LayerNorm(hidden_size),
+        )
+
     def _maxpool_output_dim(self, dimension, dilation, kernel_size, stride):
         """Calculates the output height and width based on the input
         height and width to the convolution layer.
         ref: https://pytorch.org/docs/master/nn.html#torch.nn.Conv2d
         """
         assert len(dimension) == 2
         out_dimension = []
         for i in range(len(dimension)):
             out_dimension.append(
-                int(np.floor(
-                    ((dimension[i] - dilation[i] * (kernel_size[i] - 1) - 1) / stride[i]) + 1
-                ))
+                int(
+                    np.floor(
+                        (
+                            (dimension[i] - dilation[i] * (kernel_size[i] - 1) - 1)
+                            / stride[i]
+                        )
+                        + 1
+                    )
+                )
             )
         return tuple(out_dimension)
 
     def _cnn_output_dim(self, dimension, padding, dilation, kernel_size, stride):
         """Calculates the output height and width based on the input
         height and width to the convolution layer.
         ref: https://pytorch.org/docs/master/nn.html#torch.nn.Conv2d
         """
         assert len(dimension) == 2
         out_dimension = []
         for i in range(len(dimension)):
             out_dimension.append(
-                int(np.floor(
-                    ((dimension[i] + 2 * padding[i] - dilation[i] * (kernel_size[i] - 1) - 1) / stride[i]) + 1
-                ))
+                int(
+                    np.floor(
+                        (
+                            (
+                                dimension[i]
+                                + 2 * padding[i]
+                                - dilation[i] * (kernel_size[i] - 1)
+                                - 1
+                            )
+                            / stride[i]
+                        )
+                        + 1
+                    )
+                )
             )
         return tuple(out_dimension)
 
     def _build_cnn_input(self, obs):
         cnn_input = []
 
         for key in self.cnn_keys:
-            if key in ['rgb','depth','image','occupy_image']:
+            if key in ["rgb", "depth", "image", "occupy_image"]:
                 cnn_input.append(obs[key].permute(0, 3, 1, 2) / 255.0)
-            elif key in ['global_map', 'local_map', 'global_obs', 'global_merge_obs', 'global_merge_goal','gt_map']:
+            elif key in [
+                "global_map",
+                "local_map",
+                "global_obs",
+                "global_merge_obs",
+                "global_merge_goal",
+                "gt_map",
+            ]:
                 cnn_input.append(obs[key])
             else:
                 raise NotImplementedError
 
         cnn_input = torch.cat(cnn_input, dim=1)
         return cnn_input
 
@@ -230,8 +293,8 @@
             output_size += self.hidden_size
 
         if len(self.embed_keys) > 0:
             output_size += 8 * self.embed_dim
 
         if len(self.mlp_keys) > 0:
             output_size += self.hidden_size
-        return output_size
+        return output_size
```

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/mlp.py` & `openrl-0.0.4/openrl/modules/networks/utils/mlp.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,28 +97,28 @@
 
     def forward(self, x):
         x = self.conv(x)
         return x
 
 
 class MLPBase(nn.Module):
-    def __init__(self, args, obs_shape, use_attn_internal=False, use_cat_self=True):
+    def __init__(self, cfg, obs_shape, use_attn_internal=False, use_cat_self=True):
         super(MLPBase, self).__init__()
 
-        self._use_feature_normalization = args.use_feature_normalization
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._use_attn = args.use_attn
+        self._use_feature_normalization = cfg.use_feature_normalization
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._use_attn = cfg.use_attn
         self._use_attn_internal = use_attn_internal
-        self._use_average_pool = args.use_average_pool
-        self._use_conv1d = args.use_conv1d
-        self._stacked_frames = args.stacked_frames
-        self._layer_N = 0 if args.use_single_network else args.layer_N
-        self._attn_size = args.attn_size
-        self.hidden_size = args.hidden_size
+        self._use_average_pool = cfg.use_average_pool
+        self._use_conv1d = cfg.use_conv1d
+        self._stacked_frames = cfg.stacked_frames
+        self._layer_N = 0 if cfg.use_single_network else cfg.layer_N
+        self._attn_size = cfg.attn_size
+        self.hidden_size = cfg.hidden_size
 
         obs_dim = obs_shape[0]
 
         if self._use_feature_normalization:
             self.feature_norm = nn.LayerNorm(obs_dim)
 
         if self._use_attn and self._use_attn_internal:
@@ -129,15 +129,15 @@
                     inputs_dim = self._attn_size
             else:
                 split_inputs_dim = 0
                 split_shape = obs_shape[1:]
                 for i in range(len(split_shape)):
                     split_inputs_dim += split_shape[i][0]
                 inputs_dim = split_inputs_dim * self._attn_size
-            self.attn = Encoder(args, obs_shape, use_cat_self)
+            self.attn = Encoder(cfg, obs_shape, use_cat_self)
             self.attn_norm = nn.LayerNorm(inputs_dim)
         else:
             inputs_dim = obs_dim
 
         if self._use_conv1d:
             self.conv = CONVLayer(
                 self._stacked_frames,
```

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/popart.py` & `openrl-0.0.4/openrl/modules/networks/utils/popart.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/rnn.py` & `openrl-0.0.4/openrl/modules/networks/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/utils/transformer_act.py` & `openrl-0.0.4/openrl/modules/networks/utils/transformer_act.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/networks/value_network.py` & `openrl-0.0.4/openrl/modules/networks/value_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,66 +29,66 @@
 from openrl.buffers.utils.util import get_critic_obs_space
 from openrl.utils.util import check_v2 as check
 
 
 class ValueNetwork(BaseValueNetwork):
     def __init__(
         self,
-        args,
+        cfg,
         input_space,
         action_space=None,
         use_half=False,
         device=torch.device("cpu"),
     ):
-        super(ValueNetwork, self).__init__(args, device)
+        super(ValueNetwork, self).__init__(cfg, device)
 
-        self.hidden_size = args.hidden_size
-        self._use_orthogonal = args.use_orthogonal
-        self._activation_id = args.activation_id
-        self._use_naive_recurrent_policy = args.use_naive_recurrent_policy
-        self._use_recurrent_policy = args.use_recurrent_policy
-        self._use_influence_policy = args.use_influence_policy
-        self._use_popart = args.use_popart
-        self._influence_layer_N = args.influence_layer_N
-        self._recurrent_N = args.recurrent_N
+        self.hidden_size = cfg.hidden_size
+        self._use_orthogonal = cfg.use_orthogonal
+        self._activation_id = cfg.activation_id
+        self._use_naive_recurrent_policy = cfg.use_naive_recurrent_policy
+        self._use_recurrent_policy = cfg.use_recurrent_policy
+        self._use_influence_policy = cfg.use_influence_policy
+        self._use_popart = cfg.use_popart
+        self._influence_layer_N = cfg.influence_layer_N
+        self._recurrent_N = cfg.recurrent_N
         self.tpdv = dict(dtype=torch.float32, device=device)
 
         init_method = [nn.init.xavier_uniform_, nn.init.orthogonal_][
             self._use_orthogonal
         ]
 
         critic_obs_shape = get_critic_obs_space(input_space)
 
         if "Dict" in critic_obs_shape.__class__.__name__:
             self._mixed_obs = True
             self.base = MIXBase(
-                args, critic_obs_shape, cnn_layers_params=args.cnn_layers_params
+                cfg, critic_obs_shape, cnn_layers_params=cfg.cnn_layers_params
             )
         else:
             self._mixed_obs = False
             self.base = (
-                CNNBase(args, critic_obs_shape)
+                CNNBase(cfg, critic_obs_shape)
                 if len(critic_obs_shape) == 3
                 else MLPBase(
-                    args,
+                    cfg,
                     critic_obs_shape,
                     use_attn_internal=True,
-                    use_cat_self=args.use_cat_self,
+                    use_cat_self=cfg.use_cat_self,
                 )
             )
 
         input_size = self.base.output_size
 
         if self._use_naive_recurrent_policy or self._use_recurrent_policy:
             self.rnn = RNNLayer(
                 input_size,
                 self.hidden_size,
                 self._recurrent_N,
                 self._use_orthogonal,
-                rnn_type=args.rnn_type,
+                rnn_type=cfg.rnn_type,
             )
             input_size = self.hidden_size
 
         if self._use_influence_policy:
             self.mlp = MLPLayer(
                 critic_obs_shape[0],
                 self.hidden_size,
```

### Comparing `openrl-0.0.3/openrl/modules/ppo_module.py` & `openrl-0.0.4/openrl/modules/ppo_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,52 +30,52 @@
 from openrl.modules.networks.value_network import ValueNetwork
 from openrl.modules.utils.util import update_linear_schedule
 
 
 class PPOModule(RLModule):
     def __init__(
         self,
-        args,
+        cfg,
         policy_input_space: gym.spaces.Box,
         critic_input_space: gym.spaces.Box,
         act_space: gym.spaces.Box,
         share_model: bool = False,
         device: Union[str, torch.device] = "cpu",
         rank: Optional[int] = None,
         world_size: Optional[int] = None,
     ):
         model_configs = {}
         if share_model:
             model_configs["model"] = ModelTrainConfig(
-                lr=args.lr,
+                lr=cfg.lr,
                 model=PolicyValueNetwork,
                 input_space=policy_input_space,
             )
         else:
             model_configs["policy"] = ModelTrainConfig(
-                lr=args.lr,
+                lr=cfg.lr,
                 model=PolicyNetwork,
                 input_space=policy_input_space,
             )
             model_configs["critic"] = ModelTrainConfig(
-                lr=args.critic_lr,
+                lr=cfg.critic_lr,
                 model=ValueNetwork,
                 input_space=critic_input_space,
             )
 
         super(PPOModule, self).__init__(
-            args=args,
+            cfg=cfg,
             model_configs=model_configs,
             act_space=act_space,
             rank=rank,
             world_size=world_size,
             device=device,
         )
         self.share_model = share_model
-        self.args = args
+        self.cfg = cfg
 
     def lr_decay(self, episode, episodes):
         if self.share_model:
             update_linear_schedule(self.optimizers["model"], episode, episodes, self.lr)
         else:
             update_linear_schedule(self.optimizers["actor"], episode, episodes, self.lr)
             update_linear_schedule(
```

### Comparing `openrl-0.0.3/openrl/modules/rl_module.py` & `openrl-0.0.4/openrl/modules/rl_module.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,64 +25,64 @@
 from openrl.modules.base_module import BaseModule
 from openrl.modules.model_config import ModelTrainConfig
 
 
 class RLModule(BaseModule):
     def __init__(
         self,
-        args,
+        cfg,
         model_configs: Dict[str, ModelTrainConfig],
         act_space: spaces.Box,
         rank: int = 0,
         world_size: int = 1,
         device: Union[str, torch.device] = "cpu",
     ) -> None:
-        super(RLModule, self).__init__(args)
+        super(RLModule, self).__init__(cfg)
 
         if isinstance(device, str):
             device = torch.device(device)
 
         self.device = device
-        self.lr = args.lr
-        self.critic_lr = args.critic_lr
-        self.opti_eps = args.opti_eps
-        self.weight_decay = args.weight_decay
-        self.load_optimizer = args.load_optimizer
+        self.lr = cfg.lr
+        self.critic_lr = cfg.critic_lr
+        self.opti_eps = cfg.opti_eps
+        self.weight_decay = cfg.weight_decay
+        self.load_optimizer = cfg.load_optimizer
 
         self.act_space = act_space
 
-        self.program_type = args.program_type
+        self.program_type = cfg.program_type
         self.rank = rank
         self.world_size = world_size
 
-        use_half_actor = self.program_type == "actor" and args.use_half_actor
+        use_half_actor = self.program_type == "actor" and cfg.use_half_actor
 
         for model_key in model_configs:
             model_cg = model_configs[model_key]
             model = model_cg["model"](
-                args=args,
+                cfg=cfg,
                 input_space=model_cg["input_space"],
                 action_space=act_space,
                 device=device,
                 use_half=use_half_actor,
             )
             self.models.update({model_key: model})
 
             if self.program_type == "actor":
                 continue
 
             optimizer = torch.optim.Adam(
                 model.parameters(),
                 lr=model_cg["lr"],
-                eps=args.opti_eps,
-                weight_decay=args.weight_decay,
+                eps=cfg.opti_eps,
+                weight_decay=cfg.weight_decay,
             )
             self.optimizers.update({model_key: optimizer})
 
-            if args.use_amp:
+            if cfg.use_amp:
                 self.scaler = torch.cuda.amp.GradScaler()
             else:
                 self.scaler = None
 
     @abstractmethod
     def get_actions(
         self,
@@ -121,14 +121,26 @@
     ):
         raise NotImplementedError
 
     @abstractmethod
     def get_critic_value_normalizer(self):
         raise NotImplementedError
 
+    def load_policy(self, model_path: str) -> None:
+        model_path = Path(model_path)
+        assert (
+            model_path.exists()
+        ), "can not find policy weight file to load: {}".format(model_path)
+        state_dict = torch.load(str(model_path), map_location=self.device)
+        if "policy" in self.models:
+            self.models["policy"].load_state_dict(state_dict)
+        else:
+            self.models["model"].load_state_dict(state_dict)
+        del state_dict
+
     def restore(self, model_dir: str) -> None:
         model_dir = Path(model_dir)
         assert model_dir.exists(), "can not find model directory to restore: {}".format(
             model_dir
         )
 
         for model_name in self.models:
```

### Comparing `openrl-0.0.3/openrl/modules/utils/__init__.py` & `openrl-0.0.4/openrl/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/utils/util.py` & `openrl-0.0.4/openrl/modules/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/modules/utils/valuenorm.py` & `openrl-0.0.4/openrl/modules/utils/valuenorm.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/runners/__init__.py` & `openrl-0.0.4/openrl/supports/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/runners/base_runner.py` & `openrl-0.0.4/tests/project/test_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# Copyright 2021 The OpenRL Authors.
+# Copyright 2023 The OpenRL Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from typing import TypeVar
-from abc import ABC, abstractmethod
+import os
+import sys
+import pytest
 
 
+@pytest.mark.unittest
+def test_version():
+    import openrl
 
-class BaseRunner(ABC):
-    def __init__(self, argv) -> None:
-        self.argv = argv
+    assert hasattr(openrl, "__version__"), "openrl has no __version__ attribute"
+    print(hasattr(openrl, "__version__"), openrl.__version__)
 
-    @abstractmethod
-    def run(self):
-        # main run
-        raise NotImplementedError
+
+if __name__ == "__main__":
+    sys.exit(pytest.main(["-sv", os.path.basename(__file__)]))
```

### Comparing `openrl-0.0.3/openrl/runners/common/base_agent.py` & `openrl-0.0.4/openrl/runners/common/base_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 from abc import ABC, abstractmethod
 import pathlib
 
 SelfAgent = TypeVar("SelfAgent", bound="BaseAgent")
 
 SelfBaseAgent = TypeVar("SelfBaseAgent", bound="BaseAgent")
 
+
 class BaseAgent(ABC):
     @abstractmethod
     def __init__(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def save(self, path: Union[str, pathlib.Path, io.BufferedIOBase], ) -> None:
+    def save(
+        self,
+        path: Union[str, pathlib.Path, io.BufferedIOBase],
+    ) -> None:
         raise NotImplementedError
 
-    @classmethod
+    @abstractmethod
     def load(
-            cls: Type[SelfBaseAgent],
-            path: Union[str, pathlib.Path, io.BufferedIOBase],
-    ) -> SelfBaseAgent:
-        agent = cls()
-        return agent
+        self,
+        path: Union[str, pathlib.Path, io.BufferedIOBase],
+    ):
+        raise NotImplementedError
```

### Comparing `openrl-0.0.3/openrl/runners/common/ppo_agent.py` & `openrl-0.0.4/openrl/runners/common/ppo_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         env_num: Optional[int] = None,
         rank: int = 0,
         world_size: int = 1,
         use_wandb: bool = False,
         use_tensorboard: bool = False,
     ) -> None:
         self.net = net
-        self._args = net.args
+        self._cfg = net.cfg
         self._use_wandb = use_wandb
         self._use_tensorboard = not use_wandb and use_tensorboard
 
         if env is not None:
             self._env = env
         elif hasattr(net, "env") and net.env is not None:
             self._env = net.env
@@ -60,69 +60,69 @@
             raise ValueError("env is None")
 
         if env_num is not None:
             self.env_num = env_num
         else:
             self.env_num = self._env.parallel_env_num
 
-        self._args.n_rollout_threads = self.env_num
-        self._args.learner_n_rollout_threads = self._args.n_rollout_threads
+        self._cfg.n_rollout_threads = self.env_num
+        self._cfg.learner_n_rollout_threads = self._cfg.n_rollout_threads
 
         self.rank = rank
         self.world_size = world_size
 
         self.client = None
         self.agent_num = self._env.agent_num
         if run_dir is None:
-            self.run_dir = self._args.run_dir
+            self.run_dir = self._cfg.run_dir
         else:
             self.run_dir = run_dir
 
         if self.run_dir is None:
             assert (not self._use_wandb) and (not self._use_tensorboard), (
                 "log_path must be set when using wandb or tensorboard."
                 "Please set log_path in PPOAgent or in the config file or pass run_dir in the command line."
             )
 
-        if self._args.experiment_name == "":
+        if self._cfg.experiment_name == "":
             self.exp_name = "ppo"
         else:
-            self.exp_name = self._args.experiment_name
+            self.exp_name = self._cfg.experiment_name
 
     def train(self: SelfAgent, total_time_steps: int) -> None:
-        self._args.num_env_steps = total_time_steps
+        self._cfg.num_env_steps = total_time_steps
 
         self.config = {
-            "args": self._args,
+            "cfg": self._cfg,
             "num_agents": self.agent_num,
             "run_dir": self.run_dir,
             "envs": self._env,
             "device": self.net.device,
         }
 
         trainer = TrainAlgo(
-            args=self._args,
+            cfg=self._cfg,
             init_module=self.net.module,
             device=self.net.device,
             agent_num=self.agent_num,
         )
 
         buffer = ReplayBuffer(
-            self._args,
+            self._cfg,
             self.agent_num,
             self._env.observation_space,
             self._env.action_space,
             data_client=None,
         )
 
         logger = Logger(
-            args=self._args,
+            cfg=self._cfg,
             project_name="PPOAgent",
             scenario_name=self._env.env_name,
-            wandb_entity=self._args.wandb_entity,
+            wandb_entity=self._cfg.wandb_entity,
             exp_name=self.exp_name,
             log_path=self.run_dir,
             use_wandb=self._use_wandb,
             use_tensorboard=self._use_tensorboard,
         )
         driver = Driver(
             config=self.config,
@@ -134,15 +134,15 @@
             logger=logger,
         )
         driver.run()
 
     def act(
         self,
         observation: Union[np.ndarray, Dict[str, np.ndarray]],
-        deterministic: bool = False,
+        deterministic: bool = True,
     ) -> Tuple[np.ndarray, Optional[Tuple[np.ndarray, ...]]]:
         assert self.net is not None, "net is None"
         observation = ObsData.prepare_input(observation)
         action, rnn_state = self.net.act(observation, deterministic=deterministic)
 
         action = np.array(np.split(_t2n(action), self.env_num))
 
@@ -152,11 +152,39 @@
         self,
         env: Union[gym.Env, str] = None,
     ):
         self.net.reset()
         if env is not None:
             self._env = env
             self.env_num = env.parallel_env_num
-        env.reset(seed=self._args.seed)
+        env.reset(seed=self._cfg.seed)
 
     def save(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
-        pass
+        if isinstance(path, str):
+            path = pathlib.Path(path)
+        path.mkdir(parents=True, exist_ok=True)
+        torch.save(self.net.module, path / "module.pt")
+
+    def load(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
+        if isinstance(path, str):
+            path = pathlib.Path(path)
+
+        assert path.exists(), f"{path} does not exist"
+
+        if path.is_dir():
+            path = path / "module.pt"
+
+        assert path.exists(), f"{path} does not exist"
+
+        if not torch.cuda.is_available():
+            self.net.module = torch.load(path, map_location=torch.device("cpu"))
+            self.net.module.device = torch.device("cpu")
+            self.net.module.device = torch.device("cpu")
+            for key in self.net.module.models:
+                self.net.module.models[key].tpdv = dict(
+                    dtype=torch.float32, device=torch.device("cpu")
+                )
+        else:
+            self.net.module = torch.load(path)
+
+    def load_policy(self, path: Union[str, pathlib.Path, io.BufferedIOBase]) -> None:
+        self.net.load_policy(path)
```

### Comparing `openrl-0.0.3/openrl/supports/__init__.py` & `openrl-0.0.4/openrl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/utils/__init__.py` & `openrl-0.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl/utils/logger.py` & `openrl-0.0.4/openrl/utils/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import numpy as np
 import torch
 
 
 class Logger:
     def __init__(
         self,
-        args,
+        cfg,
         project_name: str,
         scenario_name: str,
         wandb_entity: str,
         exp_name: Optional[str] = None,
         log_path: Optional[str] = None,
         use_wandb: bool = False,
         use_tensorboard: bool = False,
@@ -48,27 +48,27 @@
         self.log_path = log_path
         self.project_name = project_name
         self.scenario_name = scenario_name
         self.wandb_entity = wandb_entity
         if exp_name is not None:
             self.exp_name = exp_name
         else:
-            self.exp_name = args.experiment_name
-        self.args = args
+            self.exp_name = cfg.experiment_name
+        self.cfg = cfg
         self._init()
 
     def _init(self) -> None:
         running_programs = [
             "learner",
             "server_learner",
             "local",
             "whole",
             "local_evaluator",
         ]
-        if not self.args.program_type in running_programs:
+        if not self.cfg.program_type in running_programs:
             return None
 
         if self.log_path is None:
             assert (not self.use_wandb) and (
                 not self.use_tensorboard
             ), "log_path must be set when using wandb or tensorboard"
             self.use_wandb = False
@@ -98,39 +98,39 @@
                         curr_run = "run1"
                     else:
                         curr_run = "run%i" % (max(exst_run_nums) + 1)
                 run_dir = run_dir / curr_run
                 if not run_dir.exists():
                     os.makedirs(str(run_dir))
 
-        if hasattr(self.args, "render"):
-            self.args.render_save_path = run_dir / "render.png"
+        if hasattr(self.cfg, "render"):
+            self.cfg.render_save_path = run_dir / "render.png"
 
         handlers = [RichHandler()]
         if run_dir is not None:
             log_file = os.path.join(run_dir, "log.txt")
             handlers.append(logging.FileHandler(log_file))
 
         logging.basicConfig(
             level=self.log_level,
             format="%(asctime)s [%(levelname)s] %(message)s",
             handlers=handlers,
         )
 
         if self.use_wandb:
             wandb.init(
-                config=self.args,
+                config=self.cfg,
                 project=self.project_name,
                 entity=self.wandb_entity,
                 notes=socket.gethostname(),
                 name=self.scenario_name
                 + "_"
                 + str(self.exp_name)
                 + "_seed"
-                + str(self.args.seed),
+                + str(self.cfg.seed),
                 dir=str(run_dir),
                 job_type="training",
                 reinit=True,
             )
         elif self.use_tensorboard:
             from tensorboardX import SummaryWriter
 
@@ -188,28 +188,28 @@
             elif self.use_tensorboard:
                 self.writter.add_scalars(k, {k: v}, step)
 
 
 if __name__ == "__main__":
     from collections import namedtuple
 
-    ARG = namedtuple("args", ["seed", "algorithm_name", "program_type"])
+    ARG = namedtuple("cfg", ["seed", "algorithm_name", "program_type"])
 
     class Namespace(ARG):
         @property
         def __dict__(self):
             return self._asdict()
 
-    args = Namespace(seed=1, algorithm_name="algorithm", program_type="local")
+    cfg = Namespace(seed=1, algorithm_name="algorithm", program_type="local")
 
     logger = Logger(
-        args=args,
+        cfg=cfg,
         project_name="test_logger",
         scenario_name="logger",
-        wandb_entity="tmarl",
+        wandb_entity="openrl",
         exp_name="test",
         log_path="../../../test_logger/",
         use_wandb=False,
         use_tensorboard=True,
     )
     for step in range(100):
         logger.log_info({"test": step}, step)
```

### Comparing `openrl-0.0.3/openrl/utils/util.py` & `openrl-0.0.4/openrl/utils/util.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/openrl.egg-info/PKG-INFO` & `openrl-0.0.4/openrl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrl
-Version: 0.0.3
+Version: 0.0.4
 Summary: unified reinforcement learning framework
 Home-page: https://github.com/OpenRL-Lab/openrl
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openrl
 Project-URL: Documentation, https://openrl-docs.readthedocs.io/zh/latest/
 Keywords: reinforcement-learning multi-agent reinforcement-learning-algorithms pytorch machine-learning baselines toolbox python data-science gym gymnasium
@@ -30,15 +30,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/version.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/latest_release_date.svg)](https://anaconda.org/openrl/openrl)
 [![Anaconda-Server Badge](https://anaconda.org/openrl/openrl/badges/downloads.svg)](https://anaconda.org/openrl/openrl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/openrl?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/openrl/view?branch=main)
-[![codecov](https://codecov.io/github/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=CS4Y70UWDS)](https://codecov.io/github/OpenRL-Lab/openrl_release)
+[![codecov](https://codecov.io/gh/OpenRL-Lab/openrl_release/branch/main/graph/badge.svg?token=4FMEYMR83U)](https://codecov.io/gh/OpenRL-Lab/openrl_release)
 
 [![Documentation Status](https://readthedocs.org/projects/openrl-docs/badge/?version=latest)](https://openrl-docs.readthedocs.io/zh/latest/?badge=latest)
 [![Read the Docs](https://img.shields.io/readthedocs/openrl-docs-zh?label=%E4%B8%AD%E6%96%87%E6%96%87%E6%A1%A3)](https://openrl-docs.readthedocs.io/zh/latest/)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/OpenRL)
 [![GitHub stars](https://img.shields.io/github/stars/OpenRL-Lab/openrl)](https://github.com/opendilab/OpenRL/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network)
@@ -73,30 +73,30 @@
 pip install openrl
 ```
 
 ## 快速上手
 
 可以通过命令行快速训练`CartPole`环境:
 ```bash
-openrl --mode train --env CartPole-v0
+openrl --mode train --env CartPole-v1
 ```
 
 ## 支持者
 
 ### &#8627; Stargazers
 
 [![Stargazers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/stars/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/stargazers)
 
 ### &#8627; Forkers
 
 [![Forkers repo roster for @OpenRL-Lab/openrl](https://reporoster.com/forks/OpenRL-Lab/openrl)](https://github.com/OpenRL-Lab/openrl/network/members)
 
 ## Citing OpenRL
 
-如果我们的工作对你有帮助，欢迎引用我们的论文:
+如果我们的工作对你有帮助，欢迎引用我们:
 ```latex
 @misc{openrl2023,
     title={OpenRL},
     author={OpenRL Contributors},
     publisher = {GitHub},
     howpublished = {\url{https://github.com/OpenRL-Lab/openrl}},
     year={2023},
@@ -105,9 +105,7 @@
 
 ## Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=OpenRL-Lab/openrl&type=Date)](https://star-history.com/#OpenRL-Lab/openrl&Date)
 
 ## License
 OpenRL under the Apache 2.0 license.
-
-## 致谢
```

### Comparing `openrl-0.0.3/openrl.egg-info/SOURCES.txt` & `openrl-0.0.4/openrl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 openrl/buffers/utils/obs_data.py
 openrl/buffers/utils/util.py
 openrl/cli/__init__.py
 openrl/cli/cli.py
 openrl/cli/train.py
 openrl/configs/__init__.py
 openrl/configs/config.py
-openrl/datasets/__init__.py
 openrl/drivers/__init__.py
 openrl/drivers/base_driver.py
 openrl/drivers/onpolicy_driver.py
 openrl/drivers/rl_driver.py
 openrl/envs/__init__.py
 openrl/envs/common/__init__.py
 openrl/envs/common/registration.py
@@ -67,35 +66,30 @@
 openrl/modules/common/ppo_net.py
 openrl/modules/networks/__init__.py
 openrl/modules/networks/base_policy_network.py
 openrl/modules/networks/base_value_network.py
 openrl/modules/networks/policy_network.py
 openrl/modules/networks/policy_value_network.py
 openrl/modules/networks/value_network.py
-openrl/modules/networks/utils/FcEncoder.py
 openrl/modules/networks/utils/__init__.py
 openrl/modules/networks/utils/act.py
 openrl/modules/networks/utils/attention.py
 openrl/modules/networks/utils/cnn.py
 openrl/modules/networks/utils/distributed_utils.py
 openrl/modules/networks/utils/distributions.py
 openrl/modules/networks/utils/mix.py
 openrl/modules/networks/utils/mlp.py
 openrl/modules/networks/utils/popart.py
-openrl/modules/networks/utils/pre_model_util.py
 openrl/modules/networks/utils/rnn.py
 openrl/modules/networks/utils/transformer_act.py
 openrl/modules/networks/utils/util.py
-openrl/modules/networks/utils/utils.py
 openrl/modules/utils/__init__.py
 openrl/modules/utils/util.py
 openrl/modules/utils/valuenorm.py
 openrl/runners/__init__.py
-openrl/runners/base_runner.py
-openrl/runners/base_trainer.py
 openrl/runners/common/__init__.py
 openrl/runners/common/base_agent.py
 openrl/runners/common/ppo_agent.py
 openrl/supports/__init__.py
 openrl/utils/__init__.py
 openrl/utils/logger.py
 openrl/utils/util.py
```

### Comparing `openrl-0.0.3/setup.py` & `openrl-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "gym",
         "torch",
         "treevalue",
         "rich",
         "wandb",
         "seaborn",
         "jsonargparse",
+        "imageio",
     ]
 
 
 def get_extra_requires() -> dict:
     req = {
         "test": [
             "pytest",
```

### Comparing `openrl-0.0.3/tests/__init__.py` & `openrl-0.0.4/tests/project/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/tests/project/__init__.py` & `openrl-0.0.4/tests/test_buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `openrl-0.0.3/tests/test_buffer/test_buffer.py` & `openrl-0.0.4/tests/test_buffer/test_buffer.py`

 * *Files identical despite different names*

