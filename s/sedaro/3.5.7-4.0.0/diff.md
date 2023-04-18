# Comparing `tmp/sedaro-3.5.7.tar.gz` & `tmp/sedaro-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedaro-3.5.7.tar", last modified: Fri Mar 17 22:04:59 2023, max compression
+gzip compressed data, was "sedaro-4.0.0.tar", last modified: Tue Apr 18 16:29:26 2023, max compression
```

## Comparing `sedaro-3.5.7.tar` & `sedaro-4.0.0.tar`

### file list

```diff
@@ -1,807 +1,273 @@
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.564791 sedaro-3.5.7/
--rw-r--r--   0 sedaro     (501) staff       (20)    34889 2023-02-08 20:29:31.000000 sedaro-3.5.7/LICENSE
--rw-r--r--   0 sedaro     (501) staff       (20)    10881 2023-03-17 22:04:59.564262 sedaro-3.5.7/PKG-INFO
--rw-r--r--   0 sedaro     (501) staff       (20)    10279 2023-03-17 19:57:59.000000 sedaro-3.5.7/README.md
--rw-r--r--   0 sedaro     (501) staff       (20)      841 2023-03-17 21:58:52.000000 sedaro-3.5.7/pyproject.toml
--rw-r--r--   0 sedaro     (501) staff       (20)       38 2023-03-17 22:04:59.564918 sedaro-3.5.7/setup.cfg
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.372411 sedaro-3.5.7/src/
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.503799 sedaro-3.5.7/src/sedaro/
--rw-r--r--   0 sedaro     (501) staff       (20)      103 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10776 2023-02-09 02:42:27.000000 sedaro-3.5.7/src/sedaro/block_class_client.py
--rw-r--r--   0 sedaro     (501) staff       (20)    11346 2023-02-09 02:42:27.000000 sedaro-3.5.7/src/sedaro/block_client.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4618 2023-02-27 22:11:09.000000 sedaro-3.5.7/src/sedaro/branch_client.py
--rw-r--r--   0 sedaro     (501) staff       (20)      986 2023-02-09 02:42:27.000000 sedaro-3.5.7/src/sedaro/exceptions.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.511782 sedaro-3.5.7/src/sedaro/results/
--rw-r--r--   0 sedaro     (501) staff       (20)      154 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4538 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/agent.py
--rw-r--r--   0 sedaro     (501) staff       (20)     3544 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/block.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4973 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/series.py
--rw-r--r--   0 sedaro     (501) staff       (20)     6853 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/simulation.py
--rw-r--r--   0 sedaro     (501) staff       (20)     3106 2023-03-17 19:57:59.000000 sedaro-3.5.7/src/sedaro/results/utils.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4167 2023-03-09 04:52:35.000000 sedaro-3.5.7/src/sedaro/sedaro_api_client.py
--rw-r--r--   0 sedaro     (501) staff       (20)      177 2023-02-09 02:42:27.000000 sedaro-3.5.7/src/sedaro/settings.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2481 2023-02-08 20:29:31.000000 sedaro-3.5.7/src/sedaro/sim_client.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5459 2023-02-09 02:42:27.000000 sedaro-3.5.7/src/sedaro/utils.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.506926 sedaro-3.5.7/src/sedaro.egg-info/
--rw-r--r--   0 sedaro     (501) staff       (20)    10881 2023-03-17 22:04:58.000000 sedaro-3.5.7/src/sedaro.egg-info/PKG-INFO
--rw-r--r--   0 sedaro     (501) staff       (20)    56874 2023-03-17 22:04:58.000000 sedaro-3.5.7/src/sedaro.egg-info/SOURCES.txt
--rw-r--r--   0 sedaro     (501) staff       (20)        1 2023-03-17 22:04:58.000000 sedaro-3.5.7/src/sedaro.egg-info/dependency_links.txt
--rw-r--r--   0 sedaro     (501) staff       (20)      132 2023-03-17 22:04:58.000000 sedaro-3.5.7/src/sedaro.egg-info/requires.txt
--rw-r--r--   0 sedaro     (501) staff       (20)       26 2023-03-17 22:04:58.000000 sedaro-3.5.7/src/sedaro.egg-info/top_level.txt
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.515345 sedaro-3.5.7/src/sedaro_base_client/
--rw-r--r--   0 sedaro     (501) staff       (20)     2691 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    60424 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/api_client.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.518533 sedaro-3.5.7/src/sedaro_base_client/apis/
--rw-r--r--   0 sedaro     (501) staff       (20)      214 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/apis/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    61126 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/path_to_api.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.754566 sedaro-3.5.7/src/sedaro_base_client/apis/paths/
--rw-r--r--   0 sedaro     (501) staff       (20)      245 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)       98 2023-03-17 21:30:00.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/data_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      430 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      153 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_agents_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      288 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_agents_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      194 2023-03-17 21:29:50.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_celestial_targets_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      351 2023-03-17 21:29:50.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      181 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_conditions_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      331 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_conditions_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      188 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_ground_targets_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      342 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      192 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_group_conditions_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      348 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_group_conditions_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      194 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_operational_modes_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      351 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_operational_modes_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      186 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_space_targets_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      339 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_space_targets_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      186 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_target_groups_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      339 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_conops_target_groups_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      171 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_antenna_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      316 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_antenna_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      217 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      386 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      178 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_busses_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      327 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_busses_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      176 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_modes_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      324 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_modes_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      180 2023-03-17 21:30:04.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_storage_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      330 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_storage_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      176 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_types_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      324 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_data_types_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      203 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      365 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      189 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_laser_comm_module_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      344 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_laser_comm_module_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      167 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_modem_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      310 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_modem_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      209 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      374 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      192 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_receive_interfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      348 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_cdh_data_receive_interfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      166 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_clock_configs_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      308 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_clock_configs_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      193 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_magnetorquers_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      349 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_magnetorquers_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      196 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      354 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      185 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_thrusters_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      337 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_actuators_thrusters_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      207 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      371 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      224 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      397 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      231 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      407 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      221 2023-03-17 21:30:23.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      392 2023-03-17 21:30:23.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      223 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      395 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      213 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      380 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      213 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      380 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      237 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      417 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      177 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      325 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      207 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      371 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      217 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      386 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      184 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_lock_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      336 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_lock_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      212 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      379 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      190 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_passive_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      345 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_pointing_modes_passive_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      215 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      383 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      207 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      371 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      220 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      391 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      209 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      374 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      209 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      374 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      196 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_direction_sensors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      354 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_direction_sensors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      225 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      212 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      379 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      225 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      209 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      374 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      194 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_position_sensors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      351 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_position_sensors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      190 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_vector_sensors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      345 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_gnc_sensors_vector_sensors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      153 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_orbits_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      288 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_orbits_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      188 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_batteries_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      181 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_batteries_cells_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      331 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_batteries_cells_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      181 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_batteries_packs_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      331 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_batteries_packs_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      186 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_eps_bus_regulators_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      339 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_eps_bus_regulators_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      206 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_eps_power_processor_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      175 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      322 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      186 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_cells_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      339 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_cells_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      188 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_panels_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      342 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_power_solar_arrays_panels_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      205 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_body_frame_vectors_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      368 2023-03-17 21:29:44.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_body_frame_vectors_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      187 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_surfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      340 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_surfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      206 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_surfaces_materials_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      369 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_geometry_surfaces_materials_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      164 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_loads_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      305 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_loads_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      177 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_loads_states_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      325 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_loads_states_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      190 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_satellite_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      174 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_subsystems_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      320 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_subsystems_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      195 2023-03-17 21:29:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_subsystems_components_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      352 2023-03-17 21:29:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_system_subsystems_components_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      202 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_coolers_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      363 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_coolers_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      202 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_heaters_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      363 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_heaters_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      200 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_states_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      360 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_temp_controllers_states_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      208 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_thermal_interface_materials_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      372 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_thermal_interface_materials_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      191 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_thermal_interfaces_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      346 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_id_thermal_thermal_interfaces_block_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      154 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_idcommits_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      155 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_idcommitted_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      147 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_idsaved_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      159 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_branch_idshare_auth_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      200 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/models_branches_current_branch_id_merge_incoming_branch_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)      271 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_.py
--rw-r--r--   0 sedaro     (501) staff       (20)      294 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_job_id.py
--rw-r--r--   0 sedaro     (501) staff       (20)    13676 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tag_to_api.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.868659 sedaro-3.5.7/src/sedaro_base_client/apis/tags/
--rw-r--r--   0 sedaro     (501) staff       (20)     3141 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2650 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/agent_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2852 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/angular_velocity_sensor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2694 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/antenna_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2864 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/averaging_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2445 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2737 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_cell_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2737 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_pack_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2804 2023-03-17 21:29:44.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/body_frame_vector_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     3326 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/branches_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2753 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/bus_regulator_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2786 2023-03-17 21:29:50.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/celestial_target_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2819 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/celestial_vector_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2868 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/circular_field_of_view_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2713 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/clock_config_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2744 2023-03-17 21:29:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/component_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2723 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/condition_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2717 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/constant_load_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2735 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/cooler_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2913 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/cooperative_transmit_interface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2383 2023-03-17 21:30:00.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2706 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_bus_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2710 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_mode_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2737 2023-03-17 21:30:04.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_storage_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2710 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_type_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2789 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/direction_sensor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2795 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/ekf_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2802 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/fov_constraint_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2745 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/fuel_reservoir_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2795 2023-03-17 21:30:11.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/gps_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2756 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/ground_target_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2776 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/group_condition_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2735 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/heater_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2843 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/internal_data_interface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2805 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/jobs_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2780 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/laser_comm_module_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2717 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/load_state_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2779 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/local_vector_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2778 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/lock_pointing_mode_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2762 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/magnetorquer_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2851 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/max_align_pointing_mode_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2814 2023-03-17 21:30:23.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/mekf_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2674 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/modem_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2786 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/operational_mode_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2852 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/optical_attitude_sensor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2650 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/orbit_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2808 2023-03-17 21:30:34.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/passive_pointing_mode_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2873 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/passive_transmit_interface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2786 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/pid_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2779 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/position_sensor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2476 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/power_processor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2775 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/reaction_wheel_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2790 2023-03-17 21:30:39.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/receive_interface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2889 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/rectangular_field_of_view_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2452 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/satellite_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2869 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/sliding_mode_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2721 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/solar_array_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2732 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/solar_cell_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2742 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/solar_panel_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2746 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/space_target_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2821 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/spherical_fuel_tank_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2871 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/spherocylinder_fuel_tank_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2946 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/static_thrust_control_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2711 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/subsystem_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2718 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/surface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2804 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/surface_material_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2746 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/target_group_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2842 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/target_group_vector_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2789 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/target_vector_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2823 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/temp_controller_state_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2787 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/thermal_interface_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2870 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/thermal_interface_material_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2722 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/thruster_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2824 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/triad_algorithm_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)     2759 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/apis/tags/vector_sensor_api.py
--rw-r--r--   0 sedaro     (501) staff       (20)    17085 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/configuration.py
--rw-r--r--   0 sedaro     (501) staff       (20)     6422 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/exceptions.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.905976 sedaro-3.5.7/src/sedaro_base_client/model/
--rw-r--r--   0 sedaro     (501) staff       (20)      352 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/model/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5208 2023-03-17 21:29:25.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_create.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5992 2023-03-17 21:29:26.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_delete_res.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5930 2023-03-17 21:29:27.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_merge.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5375 2023-03-17 21:29:27.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_merge_conflicts_res.py
--rw-r--r--   0 sedaro     (501) staff       (20)    22580 2023-03-17 21:29:28.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_scenario_res.py
--rw-r--r--   0 sedaro     (501) staff       (20)     6444 2023-03-17 21:29:30.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_update.py
--rw-r--r--   0 sedaro     (501) staff       (20)    22578 2023-03-17 21:29:31.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_vehicle_res.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4405 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/branch_verify_password.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5455 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/conflicts_obj.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4392 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/data_service_response.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4873 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/data_set.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4804 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/deleted_entity.py
--rw-r--r--   0 sedaro     (501) staff       (20)     5298 2023-03-17 21:29:32.000000 sedaro-3.5.7/src/sedaro_base_client/model/http_validation_error.py
--rw-r--r--   0 sedaro     (501) staff       (20)     4369 2023-03-17 21:29:33.000000 sedaro-3.5.7/src/sedaro_base_client/model/message_res.py
--rw-r--r--   0 sedaro     (501) staff       (20)    11802 2023-03-17 21:29:33.000000 sedaro-3.5.7/src/sedaro_base_client/model/simulation_job.py
--rw-r--r--   0 sedaro     (501) staff       (20)     3604 2023-03-17 21:29:33.000000 sedaro-3.5.7/src/sedaro_base_client/model/statuses.py
--rw-r--r--   0 sedaro     (501) staff       (20)     8485 2023-03-17 21:29:33.000000 sedaro-3.5.7/src/sedaro_base_client/model/validation_error.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.906957 sedaro-3.5.7/src/sedaro_base_client/models/
--rw-r--r--   0 sedaro     (501) staff       (20)     1563 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/models/__init__.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.907873 sedaro-3.5.7/src/sedaro_base_client/paths/
--rw-r--r--   0 sedaro     (501) staff       (20)    19206 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/__init__.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.910241 sedaro-3.5.7/src/sedaro_base_client/paths/data_/
--rw-r--r--   0 sedaro     (501) staff       (20)      305 2023-03-17 21:30:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/data_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    11278 2023-03-17 21:30:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/data_/get.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.913574 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      345 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10289 2023-03-17 21:29:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10170 2023-03-17 21:29:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/get.py
--rw-r--r--   0 sedaro     (501) staff       (20)    14227 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/patch.py
--rw-r--r--   0 sedaro     (501) staff       (20)    14231 2023-03-17 21:29:44.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.914973 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_/
--rw-r--r--   0 sedaro     (501) staff       (20)      361 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12369 2023-03-17 21:29:34.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.917381 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      377 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10522 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12677 2023-03-17 21:29:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.920202 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_/
--rw-r--r--   0 sedaro     (501) staff       (20)      404 2023-03-17 21:29:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12490 2023-03-17 21:29:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.923584 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      420 2023-03-17 21:29:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10643 2023-03-17 21:29:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12798 2023-03-17 21:29:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.925732 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_/
--rw-r--r--   0 sedaro     (501) staff       (20)      391 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12407 2023-03-17 21:29:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.928851 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      407 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10560 2023-03-17 21:29:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12715 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.947359 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_/
--rw-r--r--   0 sedaro     (501) staff       (20)      398 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:30:11.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.950745 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      414 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:30:11.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:30:11.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.953076 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_/
--rw-r--r--   0 sedaro     (501) staff       (20)      402 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12477 2023-03-17 21:30:12.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.956086 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      418 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10630 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12785 2023-03-17 21:30:13.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_group_conditions_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.957724 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_/
--rw-r--r--   0 sedaro     (501) staff       (20)      404 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12490 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.959842 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      420 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10643 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12798 2023-03-17 21:30:28.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_operational_modes_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.961440 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_/
--rw-r--r--   0 sedaro     (501) staff       (20)      396 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.963761 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_space_targets_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.965541 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_/
--rw-r--r--   0 sedaro     (501) staff       (20)      396 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.969048 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_target_groups_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.971768 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_/
--rw-r--r--   0 sedaro     (501) staff       (20)      381 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12383 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.976224 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      397 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10536 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12691 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_antenna_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.979051 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      427 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12662 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:58.998510 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      443 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10815 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12970 2023-03-17 21:29:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_cooperative_transmit_interfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.000214 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_/
--rw-r--r--   0 sedaro     (501) staff       (20)      388 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12394 2023-03-17 21:30:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.003423 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      404 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10547 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12702 2023-03-17 21:30:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_busses_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.005672 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_/
--rw-r--r--   0 sedaro     (501) staff       (20)      386 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12406 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.008918 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      402 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10559 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12714 2023-03-17 21:30:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_modes_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.011123 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_/
--rw-r--r--   0 sedaro     (501) staff       (20)      390 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.014592 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      406 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:30:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_storage_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.016741 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_/
--rw-r--r--   0 sedaro     (501) staff       (20)      386 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12406 2023-03-17 21:30:04.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.020895 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      402 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10559 2023-03-17 21:30:04.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12714 2023-03-17 21:30:04.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_data_types_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.023620 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      413 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12573 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.027314 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      429 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10726 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12881 2023-03-17 21:30:15.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_internal_data_interfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.047170 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_/
--rw-r--r--   0 sedaro     (501) staff       (20)      399 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12501 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.049699 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      415 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10654 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12809 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_laser_comm_module_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.051104 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_/
--rw-r--r--   0 sedaro     (501) staff       (20)      377 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12359 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.053317 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      393 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10512 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12667 2023-03-17 21:30:27.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_modem_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.055291 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      419 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12614 2023-03-17 21:30:34.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.057448 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      435 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10767 2023-03-17 21:30:34.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12922 2023-03-17 21:30:34.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_passive_transmit_interfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.059090 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      402 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12507 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.061112 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      418 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10660 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12815 2023-03-17 21:30:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_data_receive_interfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.062370 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_/
--rw-r--r--   0 sedaro     (501) staff       (20)      374 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12460 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.064408 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      390 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10613 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12768 2023-03-17 21:29:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_clock_configs_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.066061 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_/
--rw-r--r--   0 sedaro     (501) staff       (20)      403 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12443 2023-03-17 21:30:23.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.068549 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      419 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10596 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12751 2023-03-17 21:30:24.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_magnetorquers_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.070471 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_/
--rw-r--r--   0 sedaro     (501) staff       (20)      406 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12466 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.073245 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      422 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10619 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12774 2023-03-17 21:30:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_reaction_wheels_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.075752 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_/
--rw-r--r--   0 sedaro     (501) staff       (20)      395 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12395 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.079019 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      411 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10548 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12703 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_actuators_thrusters_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.097724 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_/
--rw-r--r--   0 sedaro     (501) staff       (20)      418 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12458 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.100760 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      434 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10611 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12766 2023-03-17 21:30:32.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_pid_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.102766 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_/
--rw-r--r--   0 sedaro     (501) staff       (20)      435 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12565 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.105302 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      451 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10718 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12873 2023-03-17 21:30:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_control_sliding_mode_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.106928 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_/
--rw-r--r--   0 sedaro     (501) staff       (20)      442 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12526 2023-03-17 21:29:38.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.109330 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      458 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10679 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12834 2023-03-17 21:29:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.111053 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_/
--rw-r--r--   0 sedaro     (501) staff       (20)      432 2023-03-17 21:30:22.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12466 2023-03-17 21:30:22.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.113184 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      448 2023-03-17 21:30:23.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10619 2023-03-17 21:30:22.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12774 2023-03-17 21:30:22.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_mekf_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.114685 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_/
--rw-r--r--   0 sedaro     (501) staff       (20)      434 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12478 2023-03-17 21:31:01.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.117325 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      450 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10631 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12786 2023-03-17 21:31:02.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_attitude_determination_triad_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.119737 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_/
--rw-r--r--   0 sedaro     (501) staff       (20)      424 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.122957 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      440 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:30:07.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_ekf_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.125205 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_/
--rw-r--r--   0 sedaro     (501) staff       (20)      424 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.127945 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      440 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:30:10.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_orbit_determination_gps_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.129949 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_/
--rw-r--r--   0 sedaro     (501) staff       (20)      448 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12668 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.150780 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      464 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10821 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12976 2023-03-17 21:30:49.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_algorithms_thrust_control_static_thrust_control_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.152878 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_/
--rw-r--r--   0 sedaro     (501) staff       (20)      386 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12466 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.155840 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      402 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10619 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12774 2023-03-17 21:30:09.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.159682 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_/
--rw-r--r--   0 sedaro     (501) staff       (20)      418 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12525 2023-03-17 21:30:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.162778 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      434 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10678 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12833 2023-03-17 21:30:47.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherical_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.164693 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_/
--rw-r--r--   0 sedaro     (501) staff       (20)      428 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12585 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.170306 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      444 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10738 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12893 2023-03-17 21:30:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_fuel_reservoirs_tanks_spherocylinder_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.173543 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_/
--rw-r--r--   0 sedaro     (501) staff       (20)      394 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12523 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.177562 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      410 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10676 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12831 2023-03-17 21:30:21.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_lock_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.196813 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_/
--rw-r--r--   0 sedaro     (501) staff       (20)      422 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12586 2023-03-17 21:30:25.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.200042 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      438 2023-03-17 21:30:26.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10739 2023-03-17 21:30:25.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12894 2023-03-17 21:30:25.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_max_secondary_align_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.202844 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_/
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12549 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.206013 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      416 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10702 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12857 2023-03-17 21:30:33.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_pointing_modes_passive_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.208196 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      425 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12490 2023-03-17 21:29:50.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.210896 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      441 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10643 2023-03-17 21:29:50.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12798 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.212667 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      417 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.215376 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      433 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:30:20.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_local_vectors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.217199 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      430 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12525 2023-03-17 21:30:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.221256 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      446 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10678 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12833 2023-03-17 21:30:55.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_group_vectors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.223437 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      419 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.226870 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      435 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:30:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_reference_vectors_target_vectors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.229246 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      419 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12573 2023-03-17 21:29:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.248267 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      435 2023-03-17 21:29:37.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10726 2023-03-17 21:29:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12881 2023-03-17 21:29:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.250319 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      406 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12490 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.253147 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      422 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10643 2023-03-17 21:30:05.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12798 2023-03-17 21:30:06.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_direction_sensors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.254986 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_/
--rw-r--r--   0 sedaro     (501) staff       (20)      436 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12560 2023-03-17 21:29:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.258142 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      452 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10713 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12868 2023-03-17 21:29:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_circ_fields_of_view_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.260146 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_/
--rw-r--r--   0 sedaro     (501) staff       (20)      423 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12476 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.263162 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      439 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10629 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12784 2023-03-17 21:30:08.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_constraints_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.265168 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_/
--rw-r--r--   0 sedaro     (501) staff       (20)      436 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12596 2023-03-17 21:30:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.269345 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      452 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10749 2023-03-17 21:30:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12904 2023-03-17 21:30:39.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_fields_of_view_rect_fields_of_view_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.271559 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      419 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12573 2023-03-17 21:30:29.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.275217 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      435 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10726 2023-03-17 21:30:29.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12881 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_optical_attitude_sensors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.277843 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      404 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12478 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.299325 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      420 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10631 2023-03-17 21:30:35.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12786 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_position_sensors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.301601 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.306056 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      416 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:31:03.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_gnc_sensors_vector_sensors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.309116 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_/
--rw-r--r--   0 sedaro     (501) staff       (20)      361 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12359 2023-03-17 21:30:30.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.312146 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      377 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10512 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12667 2023-03-17 21:30:31.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_orbits_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.314383 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      395 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12691 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.317493 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_/
--rw-r--r--   0 sedaro     (501) staff       (20)      391 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.320705 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      407 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:29:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_cells_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.322935 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_/
--rw-r--r--   0 sedaro     (501) staff       (20)      391 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12442 2023-03-17 21:29:41.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.326326 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      407 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10595 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12750 2023-03-17 21:29:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_batteries_packs_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.328569 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_/
--rw-r--r--   0 sedaro     (501) staff       (20)      396 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:29:47.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.348015 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:29:48.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_bus_regulators_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.349624 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_power_processor_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      414 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_power_processor_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12785 2023-03-17 21:30:36.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_eps_power_processor_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.351471 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_/
--rw-r--r--   0 sedaro     (501) staff       (20)      384 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12430 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.354374 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10583 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12738 2023-03-17 21:30:42.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.356298 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_/
--rw-r--r--   0 sedaro     (501) staff       (20)      396 2023-03-17 21:30:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12418 2023-03-17 21:30:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.359263 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:30:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10571 2023-03-17 21:30:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12726 2023-03-17 21:30:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_cells_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.361006 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_/
--rw-r--r--   0 sedaro     (501) staff       (20)      398 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12430 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.363734 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      414 2023-03-17 21:30:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10583 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12738 2023-03-17 21:30:44.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_power_solar_arrays_panels_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.365774 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_/
--rw-r--r--   0 sedaro     (501) staff       (20)      415 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12501 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.369293 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      431 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10654 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12809 2023-03-17 21:29:43.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_body_frame_vectors_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.371470 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      397 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12383 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.375226 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      413 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10536 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12691 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.379810 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_/
--rw-r--r--   0 sedaro     (501) staff       (20)      417 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12490 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.399450 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      433 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10643 2023-03-17 21:30:52.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12798 2023-03-17 21:30:53.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_geometry_surfaces_materials_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.401664 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_/
--rw-r--r--   0 sedaro     (501) staff       (20)      373 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.405851 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      389 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10607 2023-03-17 21:29:56.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12762 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.413140 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_/
--rw-r--r--   0 sedaro     (501) staff       (20)      387 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12418 2023-03-17 21:30:18.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.427327 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      403 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10571 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12726 2023-03-17 21:30:19.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_loads_states_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.448399 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_satellite_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      397 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_satellite_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12715 2023-03-17 21:30:40.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_satellite_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.451207 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_/
--rw-r--r--   0 sedaro     (501) staff       (20)      383 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12407 2023-03-17 21:30:50.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.455291 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      399 2023-03-17 21:30:51.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10560 2023-03-17 21:30:50.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12715 2023-03-17 21:30:50.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.457646 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_/
--rw-r--r--   0 sedaro     (501) staff       (20)      405 2023-03-17 21:29:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12407 2023-03-17 21:29:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.461633 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      421 2023-03-17 21:29:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10560 2023-03-17 21:29:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12715 2023-03-17 21:29:54.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_system_subsystems_components_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.464328 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12371 2023-03-17 21:29:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.468483 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      428 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10524 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12679 2023-03-17 21:29:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_coolers_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.473674 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_/
--rw-r--r--   0 sedaro     (501) staff       (20)      412 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12371 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.499013 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      428 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10524 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12679 2023-03-17 21:30:14.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_heaters_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.501812 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_/
--rw-r--r--   0 sedaro     (501) staff       (20)      410 2023-03-17 21:30:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12556 2023-03-17 21:30:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.505633 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      426 2023-03-17 21:30:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10709 2023-03-17 21:30:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12864 2023-03-17 21:30:57.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_temp_controllers_states_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.512331 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_/
--rw-r--r--   0 sedaro     (501) staff       (20)      417 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12609 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.516104 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      433 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10762 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12917 2023-03-17 21:31:00.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interface_materials_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.520053 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_/
--rw-r--r--   0 sedaro     (501) staff       (20)      400 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12502 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.524348 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_block_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      416 2023-03-17 21:30:59.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_block_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10655 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_block_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12810 2023-03-17 21:30:58.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_thermal_thermal_interfaces_block_id/patch.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.526927 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommits_/
--rw-r--r--   0 sedaro     (501) staff       (20)      361 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommits_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12528 2023-03-17 21:29:44.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommits_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.529782 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/
--rw-r--r--   0 sedaro     (501) staff       (20)      365 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10342 2023-03-17 21:29:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/get.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.551966 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idsaved_/
--rw-r--r--   0 sedaro     (501) staff       (20)      357 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idsaved_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10302 2023-03-17 21:29:45.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idsaved_/get.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.554170 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/
--rw-r--r--   0 sedaro     (501) staff       (20)      366 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    14435 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.556593 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      411 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    16283 2023-03-17 21:29:46.000000 sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.560088 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/
--rw-r--r--   0 sedaro     (501) staff       (20)      373 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    13257 2023-03-17 21:30:16.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10306 2023-03-17 21:30:16.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py
-drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-03-17 22:04:59.563249 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/
--rw-r--r--   0 sedaro     (501) staff       (20)      385 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/__init__.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10645 2023-03-17 21:30:17.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py
--rw-r--r--   0 sedaro     (501) staff       (20)    10564 2023-03-17 21:30:16.000000 sedaro-3.5.7/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py
--rw-r--r--   0 sedaro     (501) staff       (20)    12454 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/rest.py
--rw-r--r--   0 sedaro     (501) staff       (20)    99566 2023-03-17 21:31:04.000000 sedaro-3.5.7/src/sedaro_base_client/schemas.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.379835 sedaro-4.0.0/
+-rw-r--r--   0 sedaro     (501) staff       (20)    34889 2023-02-08 20:29:31.000000 sedaro-4.0.0/LICENSE
+-rw-r--r--   0 sedaro     (501) staff       (20)    10041 2023-04-18 16:29:26.376176 sedaro-4.0.0/PKG-INFO
+-rw-r--r--   0 sedaro     (501) staff       (20)     9439 2023-04-18 14:04:45.000000 sedaro-4.0.0/README.md
+-rw-r--r--   0 sedaro     (501) staff       (20)      841 2023-04-18 16:28:48.000000 sedaro-4.0.0/pyproject.toml
+-rw-r--r--   0 sedaro     (501) staff       (20)       38 2023-04-18 16:29:26.380062 sedaro-4.0.0/setup.cfg
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.778460 sedaro-4.0.0/src/
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.819119 sedaro-4.0.0/src/sedaro/
+-rw-r--r--   0 sedaro     (501) staff       (20)      103 2023-03-17 19:57:59.000000 sedaro-4.0.0/src/sedaro/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5943 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/block_class_client.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7588 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/block_client.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13757 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/branch_client.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      986 2023-02-09 02:42:27.000000 sedaro-4.0.0/src/sedaro/exceptions.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.829733 sedaro-4.0.0/src/sedaro/results/
+-rw-r--r--   0 sedaro     (501) staff       (20)      154 2023-03-17 19:57:59.000000 sedaro-4.0.0/src/sedaro/results/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4538 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/results/agent.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3544 2023-03-17 19:57:59.000000 sedaro-4.0.0/src/sedaro/results/block.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4973 2023-03-17 19:57:59.000000 sedaro-4.0.0/src/sedaro/results/series.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6685 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/results/simulation.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3100 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/results/utils.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4060 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/sedaro_api_client.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      535 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/settings.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     2753 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/sim_client.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3878 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro/utils.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.824121 sedaro-4.0.0/src/sedaro.egg-info/
+-rw-r--r--   0 sedaro     (501) staff       (20)    10041 2023-04-18 16:29:25.000000 sedaro-4.0.0/src/sedaro.egg-info/PKG-INFO
+-rw-r--r--   0 sedaro     (501) staff       (20)    12825 2023-04-18 16:29:25.000000 sedaro-4.0.0/src/sedaro.egg-info/SOURCES.txt
+-rw-r--r--   0 sedaro     (501) staff       (20)        1 2023-04-18 16:29:25.000000 sedaro-4.0.0/src/sedaro.egg-info/dependency_links.txt
+-rw-r--r--   0 sedaro     (501) staff       (20)      132 2023-04-18 16:29:25.000000 sedaro-4.0.0/src/sedaro.egg-info/requires.txt
+-rw-r--r--   0 sedaro     (501) staff       (20)       26 2023-04-18 16:29:25.000000 sedaro-4.0.0/src/sedaro.egg-info/top_level.txt
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.835208 sedaro-4.0.0/src/sedaro_base_client/
+-rw-r--r--   0 sedaro     (501) staff       (20)     2688 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    60421 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/api_client.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.838801 sedaro-4.0.0/src/sedaro_base_client/apis/
+-rw-r--r--   0 sedaro     (501) staff       (20)      214 2023-03-17 21:31:04.000000 sedaro-4.0.0/src/sedaro_base_client/apis/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3011 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/path_to_api.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.872164 sedaro-4.0.0/src/sedaro_base_client/apis/paths/
+-rw-r--r--   0 sedaro     (501) staff       (20)      245 2023-03-17 21:31:03.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      102 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/data_id.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      430 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_id.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      159 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_id_template.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      154 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_idcommits_.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      155 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_idcommitted_.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      147 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_idsaved_.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      159 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_branch_idshare_auth_.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      200 2023-03-17 21:29:47.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/models_branches_current_branch_id_merge_incoming_branch_id.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      271 2023-03-17 21:30:17.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      294 2023-03-17 21:30:17.000000 sedaro-4.0.0/src/sedaro_base_client/apis/paths/simulations_branches_branch_id_control_job_id.py
+-rw-r--r--   0 sedaro     (501) staff       (20)      730 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tag_to_api.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:25.875502 sedaro-4.0.0/src/sedaro_base_client/apis/tags/
+-rw-r--r--   0 sedaro     (501) staff       (20)      379 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tags/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3323 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tags/branches_api.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     2382 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tags/data_api.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     2802 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tags/jobs_api.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     2425 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/apis/tags/template_api.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    17082 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/configuration.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6419 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/exceptions.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.286567 sedaro-4.0.0/src/sedaro_base_client/model/
+-rw-r--r--   0 sedaro     (501) staff       (20)      352 2023-03-17 21:31:04.000000 sedaro-4.0.0/src/sedaro_base_client/model/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9330 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/agent.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8614 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/agent_group.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4467 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_base220.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4701 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_field_of_view31.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4702 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_field_of_view36.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4702 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_field_of_view37.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4635 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_sensors20.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4635 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_sensors51.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4635 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angle_sensors56.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4804 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angular_velocity_base220.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    38403 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/angular_velocity_sensor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4972 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/angular_velocity_sensors82.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    34259 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/antenna.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12946 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/averaging_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    23468 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/battery.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13190 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/battery_cell.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    39378 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/battery_pack.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13180 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/body_frame_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3051 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/body_frame_vector_types.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11699 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/body_in_fov_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5205 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_create.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5989 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_delete_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5927 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_merge.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5372 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_merge_conflicts_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18164 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    16273 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_scenario_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5172 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_update.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    16263 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_vehicle_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4402 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/branch_verify_password.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18686 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/bus_regulator.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3587 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/categories.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4016 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/celestial_pointing_directions.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15693 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/celestial_target.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10117 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/celestial_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10416 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/circular_field_of_view.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7904 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/classical_orbital_elements.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6550 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/clock_config.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    31809 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/component.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14700 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/compound_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3094 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/compound_operators.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3516 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/condition_relationship.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3017 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/configuration_types.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5452 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/conflicts_obj.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4543 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/constant_power_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4469 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/constant_resistance_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    41442 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/cooler.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15175 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/cooperative_transmit_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6462 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/crud_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7853 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_bus.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11396 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11182 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_mode.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4389 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_service_response.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4870 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_set.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12374 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_storage.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5386 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/data_type.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4801 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/deleted_entity.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    40403 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/direction_sensor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5670 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/distance_sensors70.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5716 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_load70.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5738 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode18.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5738 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode19.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5738 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode20.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5738 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode28.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5738 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode29.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18705 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/ekf_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3053 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/eps_output_types.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6304 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/equatorial_circular_reference_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    24274 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/fixed_surface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6281 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/frame_vector_base220.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9580 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/fuel_reservoir.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    42744 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/fully_reg_det_power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8064 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/fully_reg_det_topology_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5625 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/geostationary_reference_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7110 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/geostationary_transfer_reference_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18705 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/gps_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14184 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/ground_target.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3861 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/group_rollers.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    39924 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/heater.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5295 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/http_validation_error.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3390 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/initial_state_def_type.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3057 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/input_types.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11932 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/internal_data_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6289 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/iss_reference_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    34275 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/laser_comm_module.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13144 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/load_state.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4554 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/local_pointing_directions.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10882 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/local_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    16755 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/lock_pointing_mode.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    43968 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/magnetorquer.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15682 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/max_align_pointing_mode.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13698 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/mekf_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4366 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/message_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7852 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/metamodel.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    33631 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/modem.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    23219 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/operational_mode.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    41220 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/optical_attitude_sensor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18614 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7755 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/orbital_elements_data.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12274 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/passive_pointing_mode.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15167 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/passive_transmit_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15355 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/pid_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6990 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/polar_circular_reference_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4012 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/polynomial_ephemeris_body.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    38384 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/position_sensor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15491 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/power_load.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    42722 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    42744 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/quasi_reg_det_power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8144 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/quasi_reg_det_topology_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    44788 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/reaction_wheel.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15151 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/receive_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13902 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/rectangular_field_of_view.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15541 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/resistance_load.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11427 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/same_target_multi_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4665 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/satellite.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3860 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/satellite_parameters.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14145 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/satellite_to_satellite_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12430 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/satellite_to_scalar_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14896 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/satellite_to_target_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9040 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/scenario_template.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9759 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/scenario_template_crud.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4624 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/scenario_template_update.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3135 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/side_categories.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9997 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/simulation_job.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    44251 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/single_conv_hybrid_power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6264 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/single_conv_hybrid_topology_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    44247 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/single_conv_mppt_power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5235 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/single_conv_mppt_topology_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13234 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/sliding_mode_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7715 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/solar_array.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10142 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/solar_cell.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    47548 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/solar_panel.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13535 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/space_target.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5284 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/spherical_angles.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    39932 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/spherical_fuel_tank.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    41409 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/spherocylinder_fuel_tank.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5242 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/state_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6609 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/static_thrust_control_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3601 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/statuses.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9592 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/subsystem.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     6885 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/sun_synchronous_circular_orbit.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    30325 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/sun_tracking_surface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15425 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/surface_material.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12761 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13609 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group_in_fov_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    23058 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group_to_satellite_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    21251 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group_to_scalar_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    23603 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group_to_target_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7891 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_group_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8393 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_in_fov_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4427 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_parameters.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13089 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_to_scalar_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15475 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_to_target_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     7933 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/target_vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11141 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/temp_controller_state.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5229 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/temperature_base220.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4949 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/template_crud_res.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    22894 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/thermal_interface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    13435 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/thermal_interface_material.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    39123 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/thruster.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     9932 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/time_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     4288 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/tle.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12812 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/triad_algorithm.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    44241 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/two_conv_mppt_power_processor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8112 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/two_conv_mppt_topology_params.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     3196 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/types.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8482 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/validation_error.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     5198 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/vector.py
+-rw-r--r--   0 sedaro     (501) staff       (20)     8497 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/vector_in_fov_condition.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    37295 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/model/vector_sensor.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    30981 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/vector_tracking_surface.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    16668 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/vehicle_template.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    20802 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/vehicle_template_crud.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12251 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/model/vehicle_template_update.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.287481 sedaro-4.0.0/src/sedaro_base_client/models/
+-rw-r--r--   0 sedaro     (501) staff       (20)    13254 2023-04-18 15:27:58.000000 sedaro-4.0.0/src/sedaro_base_client/models/__init__.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.289315 sedaro-4.0.0/src/sedaro_base_client/paths/
+-rw-r--r--   0 sedaro     (501) staff       (20)     1100 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/__init__.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.291846 sedaro-4.0.0/src/sedaro_base_client/paths/data_id/
+-rw-r--r--   0 sedaro     (501) staff       (20)      309 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/data_id/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12944 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/data_id/get.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.326552 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/
+-rw-r--r--   0 sedaro     (501) staff       (20)      345 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10272 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/delete.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11644 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/get.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15701 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/patch.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    15705 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/post.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.328254 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id_template/
+-rw-r--r--   0 sedaro     (501) staff       (20)      363 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id_template/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    18004 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id_template/patch.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.330766 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommits_/
+-rw-r--r--   0 sedaro     (501) staff       (20)      361 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommits_/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12511 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommits_/post.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.332450 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/
+-rw-r--r--   0 sedaro     (501) staff       (20)      365 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11808 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/get.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.334452 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idsaved_/
+-rw-r--r--   0 sedaro     (501) staff       (20)      357 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idsaved_/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    11768 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idsaved_/get.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.336120 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/
+-rw-r--r--   0 sedaro     (501) staff       (20)      366 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14418 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/post.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.338473 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/
+-rw-r--r--   0 sedaro     (501) staff       (20)      411 2023-03-17 21:29:46.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    16249 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.342896 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/
+-rw-r--r--   0 sedaro     (501) staff       (20)      373 2023-03-17 21:30:17.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    14785 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10289 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py
+drwxr-xr-x   0 sedaro     (501) staff       (20)        0 2023-04-18 16:29:26.348512 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/
+-rw-r--r--   0 sedaro     (501) staff       (20)      385 2023-03-17 21:30:17.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/__init__.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10611 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    10530 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    12451 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/rest.py
+-rw-r--r--   0 sedaro     (501) staff       (20)    99563 2023-04-17 16:35:16.000000 sedaro-4.0.0/src/sedaro_base_client/schemas.py
```

### Comparing `sedaro-3.5.7/LICENSE` & `sedaro-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sedaro-3.5.7/PKG-INFO` & `sedaro-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sedaro
-Version: 3.5.7
+Version: 4.0.0
 Summary: A python client to interact with the Sedaro Satellite API.
 Author-email: Sedaro <support@sedarotech.com>
 Project-URL: Homepage, https://github.com/sedaro/sedaro-python
 Project-URL: Bug Tracker, https://github.com/sedaro/sedaro-python/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sedaro Python Client (Beta)
+# Sedaro Python Client
 
 A python client for interacting with the Sedaro Satellite API using intuitive classes and methods.
 
 This client is intended to be used alongside our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/). Please refer to this documentation for detailed information on the names, attributes, and relationships of each Sedaro Block.
 
 Package release versions correspond to the Sedaro Satellite application version at the time of package updates.
 
@@ -31,264 +31,200 @@
 
 1.  Instantiate the `SedaroApiClient` as a context manager. All code interacting with the API should be within the scope of that context manager. Generate an API key in the Sedaro Satellite Management Console.
 
     ```py
     from sedaro import SedaroApiClient
 
     API_KEY = 'my_api_key' # Generated in Sedaro Satellite Management Console
-    AGENT_TEMPLATE_BRANCH_ID = 1 # id of a Branch owned by my Sedaro account with the given api key
+    AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-' # id of a Branch owned by my Sedaro account with the given api key
 
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
         ...
     ```
 
     ```py
     # If using a dedicated enterprise Sedaro instance, overwrite the default `host` kwarg.
-    ...
-    HOST = 'url-to-my-sedaro-server-instance.com'
+    HOST = 'url-to-my-sedaro-instance.com'
 
-    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro:
         ...
     ```
 
 2.  Use the client to instantiate a `BranchClient`.
 
     ```py
-    ...
-
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
+        branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
     ```
 
 3.  Use the `BranchClient` to access and utilize `BlockClassClient`s. A `BlockClassClient` is used to create and access Sedaro Blocks of the respective class.
 
     ```py
-    ...
-
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+    branch.BatteryCell
+    branch.Component
+    branch.Subsystem
 
-        branch_client.BatteryCell
+    # ...etc.
+    ```
 
-        branch_client.Component
+    Valid `BlockClassClient`s for Agent Template Branches and Scenario Branches can be found in our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/), by viewing the valid classes in the `blocks` key for the `Template` `PATCH` route.
 
-        branch_client.Subsystem
-
-        # ...etc.
-
-    ```
-
-    - Valid `BlockClassClient`s for an Agent Template Branch are as follows:
-
-      - AngularVelocitySensor
-      - AveragingAlgorithm
-      - Battery
-      - BatteryCell
-      - BatteryPack
-      - BodyFrameVector
-      - BusRegulator
-      - CelestialTarget
-      - CelestialVector
-      - CircularFieldOfView
-      - Component
-      - Condition
-      - ConOps
-      - ConstantLoad
-      - Cooler
-      - DirectionSensor
-      - EKFAlgorithm
-      - FOVConstraint
-      - FuelReservoir
-      - GPSAlgorithm
-      - GroundTarget
-      - GroupCondition
-      - Heater
-      - LoadState
-      - LocalVector
-      - LockPointingMode
-      - Magnetorquer
-      - MaxAlignPointingMode
-      - MEKFAlgorithm
-      - OperationalMode
-      - OpticalAttitudeSensor
-      - PassivePointingMode
-      - PIDAlgorithm
-      - PositionSensor
-      - ReactionWheel
-      - RectangularFieldOfView
-      - Satellite
-      - SlidingModeAlgorithm
-      - SolarArray
-      - SolarCell
-      - SolarPanel
-      - SpaceTarget
-      - SphericalFuelTank
-      - SpherocylinderFuelTank
-      - StaticThrustControlAlgorithm
-      - Subsystem
-      - Surface
-      - SurfaceMaterial
-      - TargetGroup
-      - TargetGroupVector
-      - TargetVector
-      - TempControllerState
-      - ThermalInterface
-      - ThermalInterfaceMaterial
-      - Thruster
-      - PowerProcessor
-      - TriadAlgorithm
-      - VectorSensor
-
-    - Valid `BlockClassClient`s for an Scenario Branch are as follows:
-      - Agent
-      - ClockConfig
-      - Orbit
+    In code editors that support it, intellisense will suggest names for `BlockClassClients`. Pay attention to what is valid for an Agent Template vs a Scenario branch. If you key into an invalid value, an error will be raised.
 
 4.  A `BlockClassClient` has several methods:
 
     ```py
-    ...
-        branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'  # The ID of the related Satellite Block
-        )
-
-        branch_client.Subsystem.get(block_id) # ID of desired Subsystem
-        branch_client.Subsystem.get_all()
-        branch_client.Subsystem.get_first()
-        branch_client.Subsystem.get_last()
-        branch_client.Subsystem.get_all_ids()
+    branch.Subsystem.create(name='Structure')
+    branch.Subsystem.get(block_id) # ID of desired Subsystem
+    branch.Subsystem.get_all_ids()
+    branch.Subsystem.get_all()
+    branch.Subsystem.get_where()
+    branch.Subsystem.get_first()
+    branch.Subsystem.get_last()
     ```
 
-5.  Most `BlockClassClient` methods return a `BlockClient` which has several methods and properties.
+5.  These methods (except for `get_all_ids`) return a single or list of `BlockClient`(s). A `BlockClassClient` has several methods and properties.
 
     ```py
-    ...
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
+    subsystem = branch.Subsystem.create(name='Structure')
 
-        subsystem_client.update(name='Structure 2.0')
+    subsystem.update(name='Structure 2.0')
 
-        subsystem_client.delete()
+    subsystem.delete()
     ```
 
-    ```py
-    ...
-    # A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
-
-        subsystem_client_2 = subsystem_client.update(
-         name='Structure 2.0'
-        )
+    A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
 
-        subsystem_client_3 = branch_client.Subsystem.get(subsystem_client.id)
+    ```py
+    subsystem = branch.Subsystem.create(name='Structure')
+    subsystem_2 = subsystem.update(name='Structure 2.0')
+    subsystem_3 = branch.Subsystem.get(subsystem.id)
 
-        assert subsystem_client == subsystem_client_2 == subsystem_client_3
+    assert subsystem == subsystem_2 == subsystem_3
     ```
 
+    The `repr` of a `BlockClient` will show you the corresponding Sedaro Block's data:
+
     ```py
-    ...
-    # Printing a `BlockClient` will show you the corresponding Sedaro Block's data:
-        print(subsystem_client)
+    repr(subsystem)
 
     >>> Subsystem(
-    >>>   id=27
-    >>>   name=Structure 2.0
-    >>>   category=CUSTOM
-    >>>   satellite=3
-    >>>   components=()
+    >>>   category='CUSTOM'
+    >>>   components=[]
+    >>>   id='NShHxZwUh1JGRfZKDvqdA'
+    >>>   name='Structure 2.0'
+    >>>   type='Subsystem'
     >>> )
     ```
 
+    Keying into any field existing on the corresponding Sedaro Block will return the value.
+
     ```py
-    # Keying into any property existing on the corresponding Sedaro Block will return that properties value.
-        subsystem_client.name
+    subsystem.name
 
     >>> 'Structure 2.0'
-    # Keying into a property that is a relationship field, will return a `BlockClient` corresponding to the related `Block` (or `list` of `BlockClient`s if it's a many-side relationship field).
-        subsystem.satellite
-
-    >>> Satellite(
-    >>>   id=3
-    >>>   mass=1000
-    >>>   ...etc
-    >>> )
     ```
 
+    Keying into relationship fields returns `BlockClient`s corresponding to the related Sedaro `Block`s as follows:
+
+    - `OneSide`: a `BlockClient`
+    - `ManySide`: a `list` of `BlockClient`s
+    - `DataSide`: a dictionary with `BlockClient`s as keys and relationship data as values
+
     ```py
-    # This allows for traversing Blocks in the model via relationship fields:
-        solar_panel_client = branch_client.SolarPanel.get_first()
+    solar_panel = subsystem.components[0]
 
-        solar_panel_client.cell.panels[-1].subsystem.satellite.components[0].delete()
+    >>> SolarPanel(id='NShKPImRZHxGAXqkPsluk')
+    ```
+
+    Note that this allows for traversing via chained relationship fields.
+
+    ```py
+    solar_panel.cell.panels[-1].subsystem.components[0].delete()
     ```
 
 ### Full Example
 
 ```py
 from sedaro import SedaroApiClient
 from sedaro.exceptions import NonexistantBlockError
 
-API_KEY = 'my_api_key_generated_by_sedaro_satellite'
-AGENT_TEMPLATE_BRANCH_ID = 1
+API_KEY = 'api_key_generated_by_sedaro'
+AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-    branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
 
-    battery_cell_client = branch_client.BatteryCell.create(
-        partNumber='987654321',
-        manufacturer='Sedaro Corporation',
-        esr=0.01,
-        maxChargeCurrent=15,
-        maxDischargeCurrent=100,
-        minSoc=0.2,
-        capacity=500,
-        curve=[[0, 0.5, 1], [12.2, 14.1, 16.8]],
-        powerProcessor='5',
+    solar_cell = branch.SolarCell.create(
+      partNumber="987654321",
+      manufacturer='Sedaro Corporation',
+      openCircuitVoltage=3.95,
+      shortCircuitCurrent=0.36,
+      maxPowerVoltage=3.54,
+      maxPowerCurrent=0.345,
+      numJunctions=3,
     )
 
-    bc_id = battery_cell_client.id
+    bc_id = solar_cell.id
 
-    battery_cell_client.update(partNumber="123456789")
+    solar_cell.update(partNumber="123456789")
 
-    battery_cell_client.delete()
+    solar_cell.delete()
 
     try:
-        battery_cell_client.update(partNumber="987654321")
+        solar_cell.update(partNumber="987654321")
     except NonexistantBlockError as e:
         assert str(e) == f'The referenced "BatteryCell" (id: {bc_id}) no longer exists.'
 ```
 
+### Multi-Block CRUD
+
+The `crud` method is also available for performing CRUD operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
+- `root`: update fields on the root by passing a dictionary
+- `blocks`: create/update 1+ blocks by passing a list of dictionaries. If an `id` is present, the corresponding block will be updated. If an `id` isn't present, a new block will be created. The `type` is always required.
+- `delete`: delete 1+ blocks by passing a list of their block `id`s.
+
+```py
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+
+    branch.crud(
+        root={ "field": "value" }, # update fields on root
+        blocks=[
+            { "id": "NTF7...", "type": "Modem", "field": "value" }, # update block
+            { "type": "SolarCell",  "field": "value", ... }, # create block
+        ],
+        delete=["NTF8-90Sh93mPKxJkq6z-"] # delete block
+    )
+```
+
+
 ## Use: Simulation
 
 ```py
-SCENARIO_BRANCH_ID = 2
+SCENARIO_BRANCH_ID = 'NShL7J0Rni63llTcEUp4F'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
 
     # Instantiate sim client
-    sim_client = sedaro_client.get_sim_client(SCENARIO_BRANCH_ID)
+    sim = sedaro.get_sim_client(SCENARIO_BRANCH_ID)
 
     # Start simulation
-    sim_client.start()
+    sim.start()
 
     # Get simulation
-    response = sim_client.get_latest()
+    job_res = sim.get_latest()[0]
 
     # Check status & percentage complete
-    job = response.body[0]
-    assert job['status'] == 'RUNNING'
-    print(job['progress']['percentComplete'])
+    assert job_res['status'] == 'RUNNING'
+    print(job_res['progress']['percentComplete'])
 
     # Terminate simulation
-    response = sim_client.terminate(job['id'])
-    assert response.body['message'] == 'Successfully terminated simulation.'
+    response = sim.terminate(job_res['id'])
+    assert response['message'] == 'Successfully terminated simulation.'
 
 ```
 
 ## Use: View Results
 
 The primary entrypoint of the results API is the `SedaroSimulationResult` class. This class offers a few methods for pulling data from scenarios. The most commonly-used method is `.get_scenario_latest` that pulls the latest results into a new result object. If the simulation is not complete, the resulting object will indicate the status is "Running" and not contain any results.
 
@@ -305,30 +241,31 @@
 Any object in the results API will provide a descriptive summary of its contents when the `.summarize` method is called. See the `results_api_demo` notebook in the [modsim notebooks](https://github.com/sedaro/modsim-notebooks) repository for more examples.
 
 ## Use: Send Requests
 
 Use built-in method to send customized requests to the host. See [OpenAPI Specification](https://sedaro.github.io/openapi/) for documentation on resource paths and body params.
 
 ```py
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
     # get a branch
-    sedaro_client.send_request(
+    sedaro.send_request(
         f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}',
         'GET'
     )
 
     # create a celestial target in a branch
-    sedaro_client.send_request(
-        f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}/cdh/conops/celestial-targets/',
-        'POST',
-        body={
-            'name': 'Sun',
-            'polynomialEphemerisBody': 'SUN',
-            'conOps': 2
-        }
+    sun = {
+        'name': 'Sun',
+        'type': 'CelestialTarget'
+    }
+
+    sedaro.send_request(
+        f'/models/branches/{self.id}/template/',
+        'PATCH',
+        { 'blocks': [sun] }
     )
 ```
 
 Note that requests sent this way to CRUD Sedaro Blocks won't automatically update already instantiated `BranchClient`s or `BlockClient`s.
 
 ## Further information
```

### Comparing `sedaro-3.5.7/README.md` & `sedaro-4.0.0/src/sedaro.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,23 @@
-# Sedaro Python Client (Beta)
+Metadata-Version: 2.1
+Name: sedaro
+Version: 4.0.0
+Summary: A python client to interact with the Sedaro Satellite API.
+Author-email: Sedaro <support@sedarotech.com>
+Project-URL: Homepage, https://github.com/sedaro/sedaro-python
+Project-URL: Bug Tracker, https://github.com/sedaro/sedaro-python/issues
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Sedaro Python Client
 
 A python client for interacting with the Sedaro Satellite API using intuitive classes and methods.
 
 This client is intended to be used alongside our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/). Please refer to this documentation for detailed information on the names, attributes, and relationships of each Sedaro Block.
 
 Package release versions correspond to the Sedaro Satellite application version at the time of package updates.
 
@@ -16,264 +31,200 @@
 
 1.  Instantiate the `SedaroApiClient` as a context manager. All code interacting with the API should be within the scope of that context manager. Generate an API key in the Sedaro Satellite Management Console.
 
     ```py
     from sedaro import SedaroApiClient
 
     API_KEY = 'my_api_key' # Generated in Sedaro Satellite Management Console
-    AGENT_TEMPLATE_BRANCH_ID = 1 # id of a Branch owned by my Sedaro account with the given api key
+    AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-' # id of a Branch owned by my Sedaro account with the given api key
 
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
         ...
     ```
 
     ```py
     # If using a dedicated enterprise Sedaro instance, overwrite the default `host` kwarg.
-    ...
-    HOST = 'url-to-my-sedaro-server-instance.com'
+    HOST = 'url-to-my-sedaro-instance.com'
 
-    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro:
         ...
     ```
 
 2.  Use the client to instantiate a `BranchClient`.
 
     ```py
-    ...
-
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
+        branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
     ```
 
 3.  Use the `BranchClient` to access and utilize `BlockClassClient`s. A `BlockClassClient` is used to create and access Sedaro Blocks of the respective class.
 
     ```py
-    ...
+    branch.BatteryCell
+    branch.Component
+    branch.Subsystem
 
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
-
-        branch_client.BatteryCell
+    # ...etc.
+    ```
 
-        branch_client.Component
+    Valid `BlockClassClient`s for Agent Template Branches and Scenario Branches can be found in our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/), by viewing the valid classes in the `blocks` key for the `Template` `PATCH` route.
 
-        branch_client.Subsystem
-
-        # ...etc.
-
-    ```
-
-    - Valid `BlockClassClient`s for an Agent Template Branch are as follows:
-
-      - AngularVelocitySensor
-      - AveragingAlgorithm
-      - Battery
-      - BatteryCell
-      - BatteryPack
-      - BodyFrameVector
-      - BusRegulator
-      - CelestialTarget
-      - CelestialVector
-      - CircularFieldOfView
-      - Component
-      - Condition
-      - ConOps
-      - ConstantLoad
-      - Cooler
-      - DirectionSensor
-      - EKFAlgorithm
-      - FOVConstraint
-      - FuelReservoir
-      - GPSAlgorithm
-      - GroundTarget
-      - GroupCondition
-      - Heater
-      - LoadState
-      - LocalVector
-      - LockPointingMode
-      - Magnetorquer
-      - MaxAlignPointingMode
-      - MEKFAlgorithm
-      - OperationalMode
-      - OpticalAttitudeSensor
-      - PassivePointingMode
-      - PIDAlgorithm
-      - PositionSensor
-      - ReactionWheel
-      - RectangularFieldOfView
-      - Satellite
-      - SlidingModeAlgorithm
-      - SolarArray
-      - SolarCell
-      - SolarPanel
-      - SpaceTarget
-      - SphericalFuelTank
-      - SpherocylinderFuelTank
-      - StaticThrustControlAlgorithm
-      - Subsystem
-      - Surface
-      - SurfaceMaterial
-      - TargetGroup
-      - TargetGroupVector
-      - TargetVector
-      - TempControllerState
-      - ThermalInterface
-      - ThermalInterfaceMaterial
-      - Thruster
-      - PowerProcessor
-      - TriadAlgorithm
-      - VectorSensor
-
-    - Valid `BlockClassClient`s for an Scenario Branch are as follows:
-      - Agent
-      - ClockConfig
-      - Orbit
+    In code editors that support it, intellisense will suggest names for `BlockClassClients`. Pay attention to what is valid for an Agent Template vs a Scenario branch. If you key into an invalid value, an error will be raised.
 
 4.  A `BlockClassClient` has several methods:
 
     ```py
-    ...
-        branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'  # The ID of the related Satellite Block
-        )
-
-        branch_client.Subsystem.get(block_id) # ID of desired Subsystem
-        branch_client.Subsystem.get_all()
-        branch_client.Subsystem.get_first()
-        branch_client.Subsystem.get_last()
-        branch_client.Subsystem.get_all_ids()
+    branch.Subsystem.create(name='Structure')
+    branch.Subsystem.get(block_id) # ID of desired Subsystem
+    branch.Subsystem.get_all_ids()
+    branch.Subsystem.get_all()
+    branch.Subsystem.get_where()
+    branch.Subsystem.get_first()
+    branch.Subsystem.get_last()
     ```
 
-5.  Most `BlockClassClient` methods return a `BlockClient` which has several methods and properties.
+5.  These methods (except for `get_all_ids`) return a single or list of `BlockClient`(s). A `BlockClassClient` has several methods and properties.
 
     ```py
-    ...
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
+    subsystem = branch.Subsystem.create(name='Structure')
 
-        subsystem_client.update(name='Structure 2.0')
+    subsystem.update(name='Structure 2.0')
 
-        subsystem_client.delete()
+    subsystem.delete()
     ```
 
-    ```py
-    ...
-    # A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
-
-        subsystem_client_2 = subsystem_client.update(
-         name='Structure 2.0'
-        )
+    A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
 
-        subsystem_client_3 = branch_client.Subsystem.get(subsystem_client.id)
+    ```py
+    subsystem = branch.Subsystem.create(name='Structure')
+    subsystem_2 = subsystem.update(name='Structure 2.0')
+    subsystem_3 = branch.Subsystem.get(subsystem.id)
 
-        assert subsystem_client == subsystem_client_2 == subsystem_client_3
+    assert subsystem == subsystem_2 == subsystem_3
     ```
 
+    The `repr` of a `BlockClient` will show you the corresponding Sedaro Block's data:
+
     ```py
-    ...
-    # Printing a `BlockClient` will show you the corresponding Sedaro Block's data:
-        print(subsystem_client)
+    repr(subsystem)
 
     >>> Subsystem(
-    >>>   id=27
-    >>>   name=Structure 2.0
-    >>>   category=CUSTOM
-    >>>   satellite=3
-    >>>   components=()
+    >>>   category='CUSTOM'
+    >>>   components=[]
+    >>>   id='NShHxZwUh1JGRfZKDvqdA'
+    >>>   name='Structure 2.0'
+    >>>   type='Subsystem'
     >>> )
     ```
 
+    Keying into any field existing on the corresponding Sedaro Block will return the value.
+
     ```py
-    # Keying into any property existing on the corresponding Sedaro Block will return that properties value.
-        subsystem_client.name
+    subsystem.name
 
     >>> 'Structure 2.0'
-    # Keying into a property that is a relationship field, will return a `BlockClient` corresponding to the related `Block` (or `list` of `BlockClient`s if it's a many-side relationship field).
-        subsystem.satellite
-
-    >>> Satellite(
-    >>>   id=3
-    >>>   mass=1000
-    >>>   ...etc
-    >>> )
     ```
 
+    Keying into relationship fields returns `BlockClient`s corresponding to the related Sedaro `Block`s as follows:
+
+    - `OneSide`: a `BlockClient`
+    - `ManySide`: a `list` of `BlockClient`s
+    - `DataSide`: a dictionary with `BlockClient`s as keys and relationship data as values
+
     ```py
-    # This allows for traversing Blocks in the model via relationship fields:
-        solar_panel_client = branch_client.SolarPanel.get_first()
+    solar_panel = subsystem.components[0]
 
-        solar_panel_client.cell.panels[-1].subsystem.satellite.components[0].delete()
+    >>> SolarPanel(id='NShKPImRZHxGAXqkPsluk')
+    ```
+
+    Note that this allows for traversing via chained relationship fields.
+
+    ```py
+    solar_panel.cell.panels[-1].subsystem.components[0].delete()
     ```
 
 ### Full Example
 
 ```py
 from sedaro import SedaroApiClient
 from sedaro.exceptions import NonexistantBlockError
 
-API_KEY = 'my_api_key_generated_by_sedaro_satellite'
-AGENT_TEMPLATE_BRANCH_ID = 1
+API_KEY = 'api_key_generated_by_sedaro'
+AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-    branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
 
-    battery_cell_client = branch_client.BatteryCell.create(
-        partNumber='987654321',
-        manufacturer='Sedaro Corporation',
-        esr=0.01,
-        maxChargeCurrent=15,
-        maxDischargeCurrent=100,
-        minSoc=0.2,
-        capacity=500,
-        curve=[[0, 0.5, 1], [12.2, 14.1, 16.8]],
-        powerProcessor='5',
+    solar_cell = branch.SolarCell.create(
+      partNumber="987654321",
+      manufacturer='Sedaro Corporation',
+      openCircuitVoltage=3.95,
+      shortCircuitCurrent=0.36,
+      maxPowerVoltage=3.54,
+      maxPowerCurrent=0.345,
+      numJunctions=3,
     )
 
-    bc_id = battery_cell_client.id
+    bc_id = solar_cell.id
 
-    battery_cell_client.update(partNumber="123456789")
+    solar_cell.update(partNumber="123456789")
 
-    battery_cell_client.delete()
+    solar_cell.delete()
 
     try:
-        battery_cell_client.update(partNumber="987654321")
+        solar_cell.update(partNumber="987654321")
     except NonexistantBlockError as e:
         assert str(e) == f'The referenced "BatteryCell" (id: {bc_id}) no longer exists.'
 ```
 
+### Multi-Block CRUD
+
+The `crud` method is also available for performing CRUD operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
+- `root`: update fields on the root by passing a dictionary
+- `blocks`: create/update 1+ blocks by passing a list of dictionaries. If an `id` is present, the corresponding block will be updated. If an `id` isn't present, a new block will be created. The `type` is always required.
+- `delete`: delete 1+ blocks by passing a list of their block `id`s.
+
+```py
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+
+    branch.crud(
+        root={ "field": "value" }, # update fields on root
+        blocks=[
+            { "id": "NTF7...", "type": "Modem", "field": "value" }, # update block
+            { "type": "SolarCell",  "field": "value", ... }, # create block
+        ],
+        delete=["NTF8-90Sh93mPKxJkq6z-"] # delete block
+    )
+```
+
+
 ## Use: Simulation
 
 ```py
-SCENARIO_BRANCH_ID = 2
+SCENARIO_BRANCH_ID = 'NShL7J0Rni63llTcEUp4F'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
 
     # Instantiate sim client
-    sim_client = sedaro_client.get_sim_client(SCENARIO_BRANCH_ID)
+    sim = sedaro.get_sim_client(SCENARIO_BRANCH_ID)
 
     # Start simulation
-    sim_client.start()
+    sim.start()
 
     # Get simulation
-    response = sim_client.get_latest()
+    job_res = sim.get_latest()[0]
 
     # Check status & percentage complete
-    job = response.body[0]
-    assert job['status'] == 'RUNNING'
-    print(job['progress']['percentComplete'])
+    assert job_res['status'] == 'RUNNING'
+    print(job_res['progress']['percentComplete'])
 
     # Terminate simulation
-    response = sim_client.terminate(job['id'])
-    assert response.body['message'] == 'Successfully terminated simulation.'
+    response = sim.terminate(job_res['id'])
+    assert response['message'] == 'Successfully terminated simulation.'
 
 ```
 
 ## Use: View Results
 
 The primary entrypoint of the results API is the `SedaroSimulationResult` class. This class offers a few methods for pulling data from scenarios. The most commonly-used method is `.get_scenario_latest` that pulls the latest results into a new result object. If the simulation is not complete, the resulting object will indicate the status is "Running" and not contain any results.
 
@@ -290,30 +241,31 @@
 Any object in the results API will provide a descriptive summary of its contents when the `.summarize` method is called. See the `results_api_demo` notebook in the [modsim notebooks](https://github.com/sedaro/modsim-notebooks) repository for more examples.
 
 ## Use: Send Requests
 
 Use built-in method to send customized requests to the host. See [OpenAPI Specification](https://sedaro.github.io/openapi/) for documentation on resource paths and body params.
 
 ```py
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
     # get a branch
-    sedaro_client.send_request(
+    sedaro.send_request(
         f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}',
         'GET'
     )
 
     # create a celestial target in a branch
-    sedaro_client.send_request(
-        f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}/cdh/conops/celestial-targets/',
-        'POST',
-        body={
-            'name': 'Sun',
-            'polynomialEphemerisBody': 'SUN',
-            'conOps': 2
-        }
+    sun = {
+        'name': 'Sun',
+        'type': 'CelestialTarget'
+    }
+
+    sedaro.send_request(
+        f'/models/branches/{self.id}/template/',
+        'PATCH',
+        { 'blocks': [sun] }
     )
 ```
 
 Note that requests sent this way to CRUD Sedaro Blocks won't automatically update already instantiated `BranchClient`s or `BlockClient`s.
 
 ## Further information
```

### Comparing `sedaro-3.5.7/pyproject.toml` & `sedaro-4.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sedaro"
-version = "3.5.7"
+version = "4.0.0"
 description = "A python client to interact with the Sedaro Satellite API."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3.7", "License :: OSI Approved :: GNU General Public License v3 (GPLv3)", "Operating System :: OS Independent", "Topic :: Software Development",]
 dependencies = [ "certifi >= 14.5.14", "frozendict ~= 2.3.4", "python-dateutil ~= 2.7.0", "setuptools >= 21.0.0", "typing_extensions ~= 4.3.0", "urllib3 ~= 1.26.7", "pydash >= 5.1.1",]
 [[project.authors]]
 name = "Sedaro"
```

### Comparing `sedaro-3.5.7/src/sedaro/exceptions.py` & `sedaro-4.0.0/src/sedaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `sedaro-3.5.7/src/sedaro/results/agent.py` & `sedaro-4.0.0/src/sedaro/results/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,30 +91,30 @@
         hfill()
 
         print("🧩 Simulated Modules")
         for module in self.__series:
             print(f'    • {ENGINE_EXPANSION[module]}')
 
         print("\n📦 Available Blocks")
-        print('    ' + '-' * 68)
-        print('    |' + 'id'.center(38) + 'name'.center(40-12) + '|')
-        print('    ' + '-' * 68)
+        print('    ' + '-' * 58)
+        print('    |' + 'id'.center(38) + 'name'.center(30-12) + '|')
+        print('    ' + '-' * 58)
         for block_id in self.__block_ids:
             if block_id != 'root':
                 block_name = self.__block_structures[block_id].get('name', None)
-                block_id_col = f"{block_id[:36]}"
+                block_id_col = f"{block_id[:26]}"
                 if block_name is not None:
                     name_id_col = f'{block_name[:25]}'
                 else:
                     name_id_col = f'<Unnamed Block>'
             else:
                 block_id_col = f"root"
                 name_id_col = ''
-            print(f"    | {block_id_col:36s} | {name_id_col:25s} |")
-        print('    ' + '-' * 68)
+            print(f"    | {block_id_col:26s} | {name_id_col:25s} |")
+        print('    ' + '-' * 58)
 
         no_data_blocks = len(self.__block_structures) - len(self.__block_ids)
         if no_data_blocks > 0:
             print(f"\n    {no_data_blocks} block(s) with no associated data")
 
         hfill()
         print("❓ Query block results with .block(<ID>) or .block(<PARTIAL_ID>)")
```

### Comparing `sedaro-3.5.7/src/sedaro/results/block.py` & `sedaro-4.0.0/src/sedaro/results/block.py`

 * *Files identical despite different names*

### Comparing `sedaro-3.5.7/src/sedaro/results/series.py` & `sedaro-4.0.0/src/sedaro/results/series.py`

 * *Files identical despite different names*

### Comparing `sedaro-3.5.7/src/sedaro/results/simulation.py` & `sedaro-4.0.0/src/sedaro/results/simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,115 +1,109 @@
 
+import datetime as dt
 import gzip
 import json
 import time
-
-import datetime as dt
-
-from typing import List, Union
 from pathlib import Path
+from typing import List, Union
+
 from sedaro import SedaroApiClient
-from sedaro_base_client.apis.tags import jobs_api
-from sedaro.results.utils import (
-    _get_agent_id_name_map, _restructure_data, progress_bar, hfill, HFILL, STATUS_ICON_MAP
-)
 from sedaro.results.agent import SedaroAgentResult
+from sedaro.results.utils import (HFILL, STATUS_ICON_MAP,
+                                  _get_agent_id_name_map, _restructure_data,
+                                  hfill, progress_bar)
+from sedaro_base_client.apis.tags import jobs_api
 
 
 class SedaroSimulationResult:
 
     def __init__(self, simulation: dict, data: dict):
         '''Initialize a new Simulation Result.
 
         See the following class methods for simple initialization:
             - get_scenario_latest
             - poll_scenario_latest
             - from_file
         '''
         self.__simulation = {
-            'branch': int(simulation['branch']),
-            'simulatedAgents': dict(simulation['simulatedAgents']),
+            'branch': simulation['branch'],
             'dateCreated': simulation['dateCreated'],
             'dateModified': simulation['dateModified'],
             'status': str(simulation['status']),
         }
         self.__data = data
         self.__branch = simulation['branch']
         if self.success:
             self.__meta = data['Data']['meta']
             raw_series = data['Data']['series']
             agent_id_name_map = _get_agent_id_name_map(self.__meta)
-            agent_simbed_id_map = {value: key for key, value in self.__simulation['simulatedAgents'].items()}
-            self.__simpleseries, self._agent_blocks = _restructure_data(
-                raw_series, agent_id_name_map, self.__meta, agent_simbed_id_map
-            )
+            self.__simpleseries, self._agent_blocks = _restructure_data(raw_series, agent_id_name_map, self.__meta)
         else:
             self.__meta = None
             self.__simpleseries = None
             self._agent_blocks = None
 
     def __repr__(self) -> str:
         return f'SedaroSimulationResult(branch={self.__branch}, status={self.status})'
 
     @classmethod
     def get_scenario_latest(cls, api_key: str, scenario_id: int, host: str = 'https://api.sedaro.com'):
         '''Query latest scenario result.'''
         with SedaroApiClient(api_key=api_key, host=host) as sedaro_client:
-            api_instance = jobs_api.JobsApi(sedaro_client)
-            simulation = cls.__get_simulation(api_instance, scenario_id)
+            simulation = cls.__get_simulation(sedaro_client, scenario_id)
             if simulation['status'] == 'SUCCEEDED':
-                data = sedaro_client.get_data(simulation['dataId'])
+                data = sedaro_client.get_data(simulation['dataArray'])
             else:
                 data = None
             return cls(simulation, data)
 
     @classmethod
     def poll_scenario_latest(
         cls,
         api_key: str,
         scenario_id: int,
         host: str = 'https://api.sedaro.com',
         retry_interval: int = 2
     ):
         '''Query latest scenario result and wait for sim if it is running.'''
         with SedaroApiClient(api_key=api_key, host=host) as sedaro_client:
-            api_instance = jobs_api.JobsApi(sedaro_client)
-            simulation = cls.__get_simulation(api_instance, scenario_id)
+            simulation = cls.__get_simulation(sedaro_client, scenario_id)
 
             while simulation['status'] in ('PENDING', 'RUNNING'):
-                simulation = cls.__get_simulation(api_instance, scenario_id)
+                simulation = cls.__get_simulation(sedaro_client, scenario_id)
                 progress_bar(simulation['progress']['percentComplete'])
                 time.sleep(retry_interval)
 
             return cls.get_scenario_latest(api_key, scenario_id, host=host)
 
     @staticmethod
-    def __get_simulation(api_instance, scenario_id: int) -> dict:
+    def __get_simulation(client, scenario_id: int) -> dict:
         try:
-            return api_instance.get_simulations(
-                path_params={'branchId': scenario_id},
-                query_params={'latest': ''}
-            ).body[0]
+            sim = client.get_sim_client(scenario_id)
+            return sim.get_latest()[0]
         except IndexError:
-            raise IndexError(f'Could not find any simulation results for scenario: {scenario_id}')
+            raise IndexError(
+                f'Could not find any simulation results for scenario: {scenario_id}')
 
     @property
     def templated_agents(self) -> List[str]:
+        self.__assert_success()
         return tuple([
             entry['name'] for _, entry
-            in self.__meta['structure']['scenario']['Agent'].items()
-            if not entry['peripheral']
+            in self.__meta['structure']['scenario']['blocks'].items()
+            if entry['type'] == 'Agent' and not entry['peripheral']
         ])
 
     @property
     def peripheral_agents(self) -> List[str]:
+        self.__assert_success()
         return tuple([
             entry['name'] for _, entry
-            in self.__meta['structure']['scenario']['Agent'].items()
-            if entry['peripheral']
+            in self.__meta['structure']['scenario']['blocks'].items()
+            if entry['type'] == 'Agent' and entry['peripheral']
         ])
 
     @property
     def status(self) -> str:
         return str(self.__simulation['status'])
 
     @property
@@ -126,19 +120,20 @@
 
     @property
     def success(self) -> bool:
         return str(self.__simulation['status']) == 'SUCCEEDED'
 
     def __assert_success(self) -> None:
         if not self.success:
-            raise ValueError('This operation cannot be completed because the simulation failed.')
+            raise ValueError(
+                'This operation cannot be completed because the simulation failed.')
 
     def __agent_id_from_name(self, name: str) -> str:
-        for id_, entry in self.__meta['structure']['scenario']['Agent'].items():
-            if name == entry['name']:
+        for id_, entry in self.__meta['structure']['scenario']['blocks'].items():
+            if entry['type'] == 'Agent' and name == entry['name']:
                 return id_
         else:
             raise ValueError(f"Agent {name} not found in data set.")
 
     def agent(self, name: str) -> SedaroAgentResult:
         '''Query results for a particular agent by name.'''
         self.__assert_success()
@@ -160,15 +155,16 @@
             return cls(contents['simulation'], contents['data'])
 
     def summarize(self) -> None:
         '''Summarize these results in the console.'''
         hfill()
         print(f'Sedaro Simulation Result Summary'.center(HFILL))
         hfill()
-        print(f'{STATUS_ICON_MAP[self.status]} Simulation {self.status.lower()} after {self.run_time:.1f}s')
+        print(
+            f'{STATUS_ICON_MAP[self.status]} Simulation {self.status.lower()} after {self.run_time:.1f}s')
 
         agents = self.templated_agents
         if len(agents) > 0:
             print('\n🛰️ Templated Agents ')
             for entry in agents:
                 print(f'    • {entry}')
```

### Comparing `sedaro-3.5.7/src/sedaro/results/utils.py` & `sedaro-4.0.0/src/sedaro/results/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 STATUS_ICON_MAP = {
     "SUCCEEDED": "✅",
     "FAILED": "❌",
     "TERMINATED": "❌",
     "PAUSED": "⏸️",
     "PENDING": "⌛",
     "RUNNING": "⌛",
+    "ERROR": "❌"
 }
 HFILL = 75
 
 
 def hfill(char="-", len=HFILL):
     print(char * len)
 
@@ -47,15 +48,20 @@
                         out[id_] = value
 
     return out
 
 
 def _get_agent_id_name_map(meta):
     '''Get mapping from agent ID to name.'''
-    return {id_: entry['name'] for id_, entry in meta['structure']['scenario']['Agent'].items()}
+    return {
+        id_: entry['name']
+        for id_, entry in meta['structure']['scenario']['blocks'].items()
+        if entry['type'] == 'Agent'
+    }
+
 
 def _simplify_series(engine_data: dict, blocks: dict) -> dict:
     '''Build a simplified series data structure
 
     Creates a dictionary with the following hierarchy:
         Block ID (or root)
             Variable Name
@@ -70,15 +76,15 @@
             # Ignore engine variables
             continue
         else:
             data['root'][key] = value
     return data
 
 
-def _restructure_data(series, agents, meta, agent_map):
+def _restructure_data(series, agents, meta):
     '''Build a simplified internal data structure.
 
     Creates a dictionary with the following key hierarchy:
 
         Agent Name
             Engine Name (gnc, cdh, power, thermal)
                 Time
@@ -86,27 +92,26 @@
                     Block ID (or root)
                         Variable Name
     '''
     data = {}
     blocks = {}
     for series_key in series:
         agent_id, engine_id = series_key.split("/")
-        agent_simbed_id = agent_map[agent_id]
-        agent_name = agents[agent_simbed_id]
+        agent_name = agents[agent_id]
         engine_name = ENGINE_MAP[engine_id]
 
         if agent_name not in data:
             data[agent_name] = {}
 
         time, sub_series = series[series_key]
-        if agent_simbed_id not in blocks:
-            blocks[agent_simbed_id] = _element_id_dict(meta['structure']['agents'].get(agent_id, {}))
+        if agent_id not in blocks:
+            blocks[agent_id] = _element_id_dict(meta['structure']['agents'].get(agent_id, {}))
         data[agent_name][engine_name] = {
             'time': time,
-            'series': _simplify_series(sub_series[agent_id], blocks[agent_simbed_id])
+            'series': _simplify_series(sub_series[agent_id], blocks[agent_id])
         }
     return data, blocks
 
 
 def _get_series_type(series):
     for entry in series:
         if entry is not None:
```

### Comparing `sedaro-3.5.7/src/sedaro/sedaro_api_client.py` & `sedaro-4.0.0/src/sedaro/sedaro_api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sedaro_base_client.api_client import ApiClient
 from sedaro_base_client.apis.tags import branches_api
 
 from .branch_client import BranchClient
 from .exceptions import SedaroApiException
 from .settings import COMMON_API_KWARGS
 from .sim_client import SimClient
-from .utils import parse_urllib_response
+from .utils import body_from_res, parse_urllib_response
 
 
 class SedaroApiClient(ApiClient):
     """A client to interact with the Sedaro API"""
 
     def __init__(self, api_key, host='https://api.sedaro.com', *args, **kwargs):
         return super().__init__(
@@ -36,22 +36,19 @@
             Branch.
         """
         branches_api_instance = branches_api.BranchesApi(self)
         # res = branches_api_instance.get_branch(path_params={'branchId': id}) # TODO: temp_crud
         # return BranchClient(res.body, self)
         res = branches_api_instance.get_branch(
             path_params={'branchId': id}, **COMMON_API_KWARGS)
-        body = res.body
-        if COMMON_API_KWARGS['skip_deserialization']:
-            body = parse_urllib_response(res.response)
-        return BranchClient(body, self)
+        return BranchClient(body_from_res(res), self)
 
     def get_data(self, id, start: float = None, stop: float = None, binWidth: float = None, limit: float = None, axisOrder: str = None):
         """Simplified Data Service getter with significantly higher performance over the Swagger-generated client."""
-        url = f'/data/?id={id}'
+        url = f'/data/{id}?'
         if start is not None:
             url += f'&start={start}'
         if stop is not None:
             url += f'&stop={stop}'
         if binWidth is not None:
             url += f'&binWidth={binWidth}'
         elif limit is not None:
```

### Comparing `sedaro-3.5.7/src/sedaro.egg-info/PKG-INFO` & `sedaro-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-Metadata-Version: 2.1
-Name: sedaro
-Version: 3.5.7
-Summary: A python client to interact with the Sedaro Satellite API.
-Author-email: Sedaro <support@sedarotech.com>
-Project-URL: Homepage, https://github.com/sedaro/sedaro-python
-Project-URL: Bug Tracker, https://github.com/sedaro/sedaro-python/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Sedaro Python Client (Beta)
+# Sedaro Python Client
 
 A python client for interacting with the Sedaro Satellite API using intuitive classes and methods.
 
 This client is intended to be used alongside our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/). Please refer to this documentation for detailed information on the names, attributes, and relationships of each Sedaro Block.
 
 Package release versions correspond to the Sedaro Satellite application version at the time of package updates.
 
@@ -31,264 +16,200 @@
 
 1.  Instantiate the `SedaroApiClient` as a context manager. All code interacting with the API should be within the scope of that context manager. Generate an API key in the Sedaro Satellite Management Console.
 
     ```py
     from sedaro import SedaroApiClient
 
     API_KEY = 'my_api_key' # Generated in Sedaro Satellite Management Console
-    AGENT_TEMPLATE_BRANCH_ID = 1 # id of a Branch owned by my Sedaro account with the given api key
+    AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-' # id of a Branch owned by my Sedaro account with the given api key
 
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
         ...
     ```
 
     ```py
     # If using a dedicated enterprise Sedaro instance, overwrite the default `host` kwarg.
-    ...
-    HOST = 'url-to-my-sedaro-server-instance.com'
+    HOST = 'url-to-my-sedaro-instance.com'
 
-    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro_client:
+    with SedaroApiClient(api_key=API_KEY, host=HOST) as sedaro:
         ...
     ```
 
 2.  Use the client to instantiate a `BranchClient`.
 
     ```py
-    ...
-
-    with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+    with SedaroApiClient(api_key=API_KEY) as sedaro:
+        branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
     ```
 
 3.  Use the `BranchClient` to access and utilize `BlockClassClient`s. A `BlockClassClient` is used to create and access Sedaro Blocks of the respective class.
 
     ```py
-    ...
+    branch.BatteryCell
+    branch.Component
+    branch.Subsystem
 
-        branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
-
-        branch_client.BatteryCell
+    # ...etc.
+    ```
 
-        branch_client.Component
+    Valid `BlockClassClient`s for Agent Template Branches and Scenario Branches can be found in our redocs [OpenAPI Specification](https://sedaro.github.io/openapi/), by viewing the valid classes in the `blocks` key for the `Template` `PATCH` route.
 
-        branch_client.Subsystem
-
-        # ...etc.
-
-    ```
-
-    - Valid `BlockClassClient`s for an Agent Template Branch are as follows:
-
-      - AngularVelocitySensor
-      - AveragingAlgorithm
-      - Battery
-      - BatteryCell
-      - BatteryPack
-      - BodyFrameVector
-      - BusRegulator
-      - CelestialTarget
-      - CelestialVector
-      - CircularFieldOfView
-      - Component
-      - Condition
-      - ConOps
-      - ConstantLoad
-      - Cooler
-      - DirectionSensor
-      - EKFAlgorithm
-      - FOVConstraint
-      - FuelReservoir
-      - GPSAlgorithm
-      - GroundTarget
-      - GroupCondition
-      - Heater
-      - LoadState
-      - LocalVector
-      - LockPointingMode
-      - Magnetorquer
-      - MaxAlignPointingMode
-      - MEKFAlgorithm
-      - OperationalMode
-      - OpticalAttitudeSensor
-      - PassivePointingMode
-      - PIDAlgorithm
-      - PositionSensor
-      - ReactionWheel
-      - RectangularFieldOfView
-      - Satellite
-      - SlidingModeAlgorithm
-      - SolarArray
-      - SolarCell
-      - SolarPanel
-      - SpaceTarget
-      - SphericalFuelTank
-      - SpherocylinderFuelTank
-      - StaticThrustControlAlgorithm
-      - Subsystem
-      - Surface
-      - SurfaceMaterial
-      - TargetGroup
-      - TargetGroupVector
-      - TargetVector
-      - TempControllerState
-      - ThermalInterface
-      - ThermalInterfaceMaterial
-      - Thruster
-      - PowerProcessor
-      - TriadAlgorithm
-      - VectorSensor
-
-    - Valid `BlockClassClient`s for an Scenario Branch are as follows:
-      - Agent
-      - ClockConfig
-      - Orbit
+    In code editors that support it, intellisense will suggest names for `BlockClassClients`. Pay attention to what is valid for an Agent Template vs a Scenario branch. If you key into an invalid value, an error will be raised.
 
 4.  A `BlockClassClient` has several methods:
 
     ```py
-    ...
-        branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'  # The ID of the related Satellite Block
-        )
-
-        branch_client.Subsystem.get(block_id) # ID of desired Subsystem
-        branch_client.Subsystem.get_all()
-        branch_client.Subsystem.get_first()
-        branch_client.Subsystem.get_last()
-        branch_client.Subsystem.get_all_ids()
+    branch.Subsystem.create(name='Structure')
+    branch.Subsystem.get(block_id) # ID of desired Subsystem
+    branch.Subsystem.get_all_ids()
+    branch.Subsystem.get_all()
+    branch.Subsystem.get_where()
+    branch.Subsystem.get_first()
+    branch.Subsystem.get_last()
     ```
 
-5.  Most `BlockClassClient` methods return a `BlockClient` which has several methods and properties.
+5.  These methods (except for `get_all_ids`) return a single or list of `BlockClient`(s). A `BlockClassClient` has several methods and properties.
 
     ```py
-    ...
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
+    subsystem = branch.Subsystem.create(name='Structure')
 
-        subsystem_client.update(name='Structure 2.0')
+    subsystem.update(name='Structure 2.0')
 
-        subsystem_client.delete()
+    subsystem.delete()
     ```
 
-    ```py
-    ...
-    # A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
-        subsystem_client = branch_client.Subsystem.create(
-            name='Structure',
-            satellite='3'
-        )
-
-        subsystem_client_2 = subsystem_client.update(
-         name='Structure 2.0'
-        )
+    A `BlockClient` will always be equal to and in sync with all other `BlockClient`s referencing the same Sedaro Block:
 
-        subsystem_client_3 = branch_client.Subsystem.get(subsystem_client.id)
+    ```py
+    subsystem = branch.Subsystem.create(name='Structure')
+    subsystem_2 = subsystem.update(name='Structure 2.0')
+    subsystem_3 = branch.Subsystem.get(subsystem.id)
 
-        assert subsystem_client == subsystem_client_2 == subsystem_client_3
+    assert subsystem == subsystem_2 == subsystem_3
     ```
 
+    The `repr` of a `BlockClient` will show you the corresponding Sedaro Block's data:
+
     ```py
-    ...
-    # Printing a `BlockClient` will show you the corresponding Sedaro Block's data:
-        print(subsystem_client)
+    repr(subsystem)
 
     >>> Subsystem(
-    >>>   id=27
-    >>>   name=Structure 2.0
-    >>>   category=CUSTOM
-    >>>   satellite=3
-    >>>   components=()
+    >>>   category='CUSTOM'
+    >>>   components=[]
+    >>>   id='NShHxZwUh1JGRfZKDvqdA'
+    >>>   name='Structure 2.0'
+    >>>   type='Subsystem'
     >>> )
     ```
 
+    Keying into any field existing on the corresponding Sedaro Block will return the value.
+
     ```py
-    # Keying into any property existing on the corresponding Sedaro Block will return that properties value.
-        subsystem_client.name
+    subsystem.name
 
     >>> 'Structure 2.0'
-    # Keying into a property that is a relationship field, will return a `BlockClient` corresponding to the related `Block` (or `list` of `BlockClient`s if it's a many-side relationship field).
-        subsystem.satellite
-
-    >>> Satellite(
-    >>>   id=3
-    >>>   mass=1000
-    >>>   ...etc
-    >>> )
     ```
 
+    Keying into relationship fields returns `BlockClient`s corresponding to the related Sedaro `Block`s as follows:
+
+    - `OneSide`: a `BlockClient`
+    - `ManySide`: a `list` of `BlockClient`s
+    - `DataSide`: a dictionary with `BlockClient`s as keys and relationship data as values
+
     ```py
-    # This allows for traversing Blocks in the model via relationship fields:
-        solar_panel_client = branch_client.SolarPanel.get_first()
+    solar_panel = subsystem.components[0]
 
-        solar_panel_client.cell.panels[-1].subsystem.satellite.components[0].delete()
+    >>> SolarPanel(id='NShKPImRZHxGAXqkPsluk')
+    ```
+
+    Note that this allows for traversing via chained relationship fields.
+
+    ```py
+    solar_panel.cell.panels[-1].subsystem.components[0].delete()
     ```
 
 ### Full Example
 
 ```py
 from sedaro import SedaroApiClient
 from sedaro.exceptions import NonexistantBlockError
 
-API_KEY = 'my_api_key_generated_by_sedaro_satellite'
-AGENT_TEMPLATE_BRANCH_ID = 1
+API_KEY = 'api_key_generated_by_sedaro'
+AGENT_TEMPLATE_BRANCH_ID = 'NShL_CIU9iuufSII49xm-'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
-    branch_client = sedaro_client.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
 
-    battery_cell_client = branch_client.BatteryCell.create(
-        partNumber='987654321',
-        manufacturer='Sedaro Corporation',
-        esr=0.01,
-        maxChargeCurrent=15,
-        maxDischargeCurrent=100,
-        minSoc=0.2,
-        capacity=500,
-        curve=[[0, 0.5, 1], [12.2, 14.1, 16.8]],
-        powerProcessor='5',
+    solar_cell = branch.SolarCell.create(
+      partNumber="987654321",
+      manufacturer='Sedaro Corporation',
+      openCircuitVoltage=3.95,
+      shortCircuitCurrent=0.36,
+      maxPowerVoltage=3.54,
+      maxPowerCurrent=0.345,
+      numJunctions=3,
     )
 
-    bc_id = battery_cell_client.id
+    bc_id = solar_cell.id
 
-    battery_cell_client.update(partNumber="123456789")
+    solar_cell.update(partNumber="123456789")
 
-    battery_cell_client.delete()
+    solar_cell.delete()
 
     try:
-        battery_cell_client.update(partNumber="987654321")
+        solar_cell.update(partNumber="987654321")
     except NonexistantBlockError as e:
         assert str(e) == f'The referenced "BatteryCell" (id: {bc_id}) no longer exists.'
 ```
 
+### Multi-Block CRUD
+
+The `crud` method is also available for performing CRUD operations on multiple Sedaro blocks and/or root at the same time using kwargs as follows:
+- `root`: update fields on the root by passing a dictionary
+- `blocks`: create/update 1+ blocks by passing a list of dictionaries. If an `id` is present, the corresponding block will be updated. If an `id` isn't present, a new block will be created. The `type` is always required.
+- `delete`: delete 1+ blocks by passing a list of their block `id`s.
+
+```py
+with SedaroApiClient(api_key=API_KEY) as sedaro:
+    branch = sedaro.get_branch(AGENT_TEMPLATE_BRANCH_ID)
+
+    branch.crud(
+        root={ "field": "value" }, # update fields on root
+        blocks=[
+            { "id": "NTF7...", "type": "Modem", "field": "value" }, # update block
+            { "type": "SolarCell",  "field": "value", ... }, # create block
+        ],
+        delete=["NTF8-90Sh93mPKxJkq6z-"] # delete block
+    )
+```
+
+
 ## Use: Simulation
 
 ```py
-SCENARIO_BRANCH_ID = 2
+SCENARIO_BRANCH_ID = 'NShL7J0Rni63llTcEUp4F'
 
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
 
     # Instantiate sim client
-    sim_client = sedaro_client.get_sim_client(SCENARIO_BRANCH_ID)
+    sim = sedaro.get_sim_client(SCENARIO_BRANCH_ID)
 
     # Start simulation
-    sim_client.start()
+    sim.start()
 
     # Get simulation
-    response = sim_client.get_latest()
+    job_res = sim.get_latest()[0]
 
     # Check status & percentage complete
-    job = response.body[0]
-    assert job['status'] == 'RUNNING'
-    print(job['progress']['percentComplete'])
+    assert job_res['status'] == 'RUNNING'
+    print(job_res['progress']['percentComplete'])
 
     # Terminate simulation
-    response = sim_client.terminate(job['id'])
-    assert response.body['message'] == 'Successfully terminated simulation.'
+    response = sim.terminate(job_res['id'])
+    assert response['message'] == 'Successfully terminated simulation.'
 
 ```
 
 ## Use: View Results
 
 The primary entrypoint of the results API is the `SedaroSimulationResult` class. This class offers a few methods for pulling data from scenarios. The most commonly-used method is `.get_scenario_latest` that pulls the latest results into a new result object. If the simulation is not complete, the resulting object will indicate the status is "Running" and not contain any results.
 
@@ -305,30 +226,31 @@
 Any object in the results API will provide a descriptive summary of its contents when the `.summarize` method is called. See the `results_api_demo` notebook in the [modsim notebooks](https://github.com/sedaro/modsim-notebooks) repository for more examples.
 
 ## Use: Send Requests
 
 Use built-in method to send customized requests to the host. See [OpenAPI Specification](https://sedaro.github.io/openapi/) for documentation on resource paths and body params.
 
 ```py
-with SedaroApiClient(api_key=API_KEY) as sedaro_client:
+with SedaroApiClient(api_key=API_KEY) as sedaro:
     # get a branch
-    sedaro_client.send_request(
+    sedaro.send_request(
         f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}',
         'GET'
     )
 
     # create a celestial target in a branch
-    sedaro_client.send_request(
-        f'/models/branches/{AGENT_TEMPLATE_BRANCH_ID}/cdh/conops/celestial-targets/',
-        'POST',
-        body={
-            'name': 'Sun',
-            'polynomialEphemerisBody': 'SUN',
-            'conOps': 2
-        }
+    sun = {
+        'name': 'Sun',
+        'type': 'CelestialTarget'
+    }
+
+    sedaro.send_request(
+        f'/models/branches/{self.id}/template/',
+        'PATCH',
+        { 'blocks': [sun] }
     )
 ```
 
 Note that requests sent this way to CRUD Sedaro Blocks won't automatically update already instantiated `BranchClient`s or `BlockClient`s.
 
 ## Further information
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/__init__.py` & `sedaro-4.0.0/src/sedaro_base_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
 from sedaro_base_client.api_client import ApiClient
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/api_client.py` & `sedaro-4.0.0/src/sedaro_base_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
 from decimal import Decimal
 import enum
 import email
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/agent_api.py` & `sedaro-4.0.0/src/sedaro_base_client/apis/tags/data_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_agents_.post import CreateAgent
-from sedaro_base_client.paths.models_branches_branch_id_agents_block_id.delete import DeleteAgent
-from sedaro_base_client.paths.models_branches_branch_id_agents_block_id.patch import UpdateAgent
+from sedaro_base_client.paths.data_id.get import GetData
 
 
-class AgentApi(
-    CreateAgent,
-    DeleteAgent,
-    UpdateAgent,
+class DataApi(
+    GetData,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/angular_velocity_sensor_api.py` & `sedaro-4.0.0/src/sedaro_base_client/apis/tags/jobs_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_gnc_sensors_angular_velocity_sensors_.post import CreateAngularVelocitySensor
-from sedaro_base_client.paths.models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id.delete import DeleteAngularVelocitySensor
-from sedaro_base_client.paths.models_branches_branch_id_gnc_sensors_angular_velocity_sensors_block_id.patch import UpdateAngularVelocitySensor
+from sedaro_base_client.paths.simulations_branches_branch_id_control_job_id.get import GetSimulation
+from sedaro_base_client.paths.simulations_branches_branch_id_control_.get import GetSimulations
+from sedaro_base_client.paths.simulations_branches_branch_id_control_.post import StartSimulation
+from sedaro_base_client.paths.simulations_branches_branch_id_control_job_id.delete import TerminateSimulation
 
 
-class AngularVelocitySensorApi(
-    CreateAngularVelocitySensor,
-    DeleteAngularVelocitySensor,
-    UpdateAngularVelocitySensor,
+class JobsApi(
+    GetSimulation,
+    GetSimulations,
+    StartSimulation,
+    TerminateSimulation,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/antenna_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/eps_output_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_cdh_data_antenna_.post import CreateAntenna
-from sedaro_base_client.paths.models_branches_branch_id_cdh_data_antenna_block_id.delete import DeleteAntenna
-from sedaro_base_client.paths.models_branches_branch_id_cdh_data_antenna_block_id.patch import UpdateAntenna
-
-
-class AntennaApi(
-    CreateAntenna,
-    DeleteAntenna,
-    UpdateAntenna,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class EpsOutputTypes(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "CORE_OUTPUT": "CORE_OUTPUT",
+            "BUS_REGULATOR": "BUS_REGULATOR",
+        }
+    
+    @schemas.classproperty
+    def CORE_OUTPUT(cls):
+        return cls("CORE_OUTPUT")
+    
+    @schemas.classproperty
+    def BUS_REGULATOR(cls):
+        return cls("BUS_REGULATOR")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/averaging_algorithm_api.py` & `sedaro-4.0.0/src/sedaro_base_client/apis/tags/template_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_.post import CreateAveragingAlgorithm
-from sedaro_base_client.paths.models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id.delete import DeleteAveragingAlgorithm
-from sedaro_base_client.paths.models_branches_branch_id_gnc_algorithms_attitude_determination_averaging_block_id.patch import UpdateAveragingAlgorithm
+from sedaro_base_client.paths.models_branches_branch_id_template.patch import CrudTemplate
 
 
-class AveragingAlgorithmApi(
-    CreateAveragingAlgorithm,
-    DeleteAveragingAlgorithm,
-    UpdateAveragingAlgorithm,
+class TemplateApi(
+    CrudTemplate,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/body_frame_vector_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,51 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_block_id.patch import UpdateBattery
-
-
-class BatteryApi(
-    UpdateBattery,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class BodyFrameVectorTypes(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "SPHERICAL_ANGLES": "SPHERICAL_ANGLES",
+            "VECTOR": "VECTOR",
+        }
+    
+    @schemas.classproperty
+    def SPHERICAL_ANGLES(cls):
+        return cls("SPHERICAL_ANGLES")
+    
+    @schemas.classproperty
+    def VECTOR(cls):
+        return cls("VECTOR")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_cell_api.py` & `sedaro-4.0.0/src/sedaro_base_client/apis/tags/branches_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_cells_.post import CreateBatteryCell
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_cells_block_id.delete import DeleteBatteryCell
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_cells_block_id.patch import UpdateBatteryCell
-
-
-class BatteryCellApi(
-    CreateBatteryCell,
-    DeleteBatteryCell,
-    UpdateBatteryCell,
+from sedaro_base_client.paths.models_branches_branch_idcommits_.post import CommitToBranch
+from sedaro_base_client.paths.models_branches_branch_id.post import CreateBranch
+from sedaro_base_client.paths.models_branches_branch_id.delete import DeleteBranch
+from sedaro_base_client.paths.models_branches_branch_id.get import GetBranch
+from sedaro_base_client.paths.models_branches_branch_idcommitted_.get import GetCommittedBranchData
+from sedaro_base_client.paths.models_branches_branch_idsaved_.get import GetSavedBranchData
+from sedaro_base_client.paths.models_branches_current_branch_id_merge_incoming_branch_id.post import MergeBranches
+from sedaro_base_client.paths.models_branches_branch_id.patch import UpdateBranch
+from sedaro_base_client.paths.models_branches_branch_idshare_auth_.post import VerifyBranchPassword
+
+
+class BranchesApi(
+    CommitToBranch,
+    CreateBranch,
+    DeleteBranch,
+    GetBranch,
+    GetCommittedBranchData,
+    GetSavedBranchData,
+    MergeBranches,
+    UpdateBranch,
+    VerifyBranchPassword,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/battery_pack_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/configuration_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_packs_.post import CreateBatteryPack
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_packs_block_id.delete import DeleteBatteryPack
-from sedaro_base_client.paths.models_branches_branch_id_power_batteries_packs_block_id.patch import UpdateBatteryPack
-
-
-class BatteryPackApi(
-    CreateBatteryPack,
-    DeleteBatteryPack,
-    UpdateBatteryPack,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class ConfigurationTypes(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "SERIES": "SERIES",
+            "PARALLEL": "PARALLEL",
+        }
+    
+    @schemas.classproperty
+    def SERIES(cls):
+        return cls("SERIES")
+    
+    @schemas.classproperty
+    def PARALLEL(cls):
+        return cls("PARALLEL")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/body_frame_vector_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/compound_operators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_system_geometry_body_frame_vectors_.post import CreateBodyFrameVector
-from sedaro_base_client.paths.models_branches_branch_id_system_geometry_body_frame_vectors_block_id.delete import DeleteBodyFrameVector
-from sedaro_base_client.paths.models_branches_branch_id_system_geometry_body_frame_vectors_block_id.patch import UpdateBodyFrameVector
-
-
-class BodyFrameVectorApi(
-    CreateBodyFrameVector,
-    DeleteBodyFrameVector,
-    UpdateBodyFrameVector,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class CompoundOperators(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "ALL": "ALL",
+            "ANY": "ANY",
+            "COUNT": "COUNT",
+        }
+    
+    @schemas.classproperty
+    def ALL(cls):
+        return cls("ALL")
+    
+    @schemas.classproperty
+    def ANY(cls):
+        return cls("ANY")
+    
+    @schemas.classproperty
+    def COUNT(cls):
+        return cls("COUNT")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/bus_regulator_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/input_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,51 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_power_eps_bus_regulators_.post import CreateBusRegulator
-from sedaro_base_client.paths.models_branches_branch_id_power_eps_bus_regulators_block_id.delete import DeleteBusRegulator
-from sedaro_base_client.paths.models_branches_branch_id_power_eps_bus_regulators_block_id.patch import UpdateBusRegulator
-
-
-class BusRegulatorApi(
-    CreateBusRegulator,
-    DeleteBusRegulator,
-    UpdateBusRegulator,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class InputTypes(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "EPS_ROOT_NODE": "EPS_ROOT_NODE",
+            "BUS_REGULATOR": "BUS_REGULATOR",
+        }
+    
+    @schemas.classproperty
+    def EPS_ROOT_NODE(cls):
+        return cls("EPS_ROOT_NODE")
+    
+    @schemas.classproperty
+    def BUS_REGULATOR(cls):
+        return cls("BUS_REGULATOR")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/celestial_target_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_cdh_conops_celestial_targets_.post import CreateCelestialTarget
-from sedaro_base_client.paths.models_branches_branch_id_cdh_conops_celestial_targets_block_id.delete import DeleteCelestialTarget
-from sedaro_base_client.paths.models_branches_branch_id_cdh_conops_celestial_targets_block_id.patch import UpdateCelestialTarget
-
-
-class CelestialTargetApi(
-    CreateCelestialTarget,
-    DeleteCelestialTarget,
-    UpdateCelestialTarget,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class Types(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "SpaceTarget": "SPACE_TARGET",
+            "CelestialTarget": "CELESTIAL_TARGET",
+            "GroundTarget": "GROUND_TARGET",
+        }
+    
+    @schemas.classproperty
+    def SPACE_TARGET(cls):
+        return cls("SpaceTarget")
+    
+    @schemas.classproperty
+    def CELESTIAL_TARGET(cls):
+        return cls("CelestialTarget")
+    
+    @schemas.classproperty
+    def GROUND_TARGET(cls):
+        return cls("GroundTarget")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/celestial_vector_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/initial_state_def_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,66 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_gnc_reference_vectors_celestial_vectors_.post import CreateCelestialVector
-from sedaro_base_client.paths.models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id.delete import DeleteCelestialVector
-from sedaro_base_client.paths.models_branches_branch_id_gnc_reference_vectors_celestial_vectors_block_id.patch import UpdateCelestialVector
-
-
-class CelestialVectorApi(
-    CreateCelestialVector,
-    DeleteCelestialVector,
-    UpdateCelestialVector,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class InitialStateDefType(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "ORBITAL_ELEMENTS": "ORBITAL_ELEMENTS",
+            "REF_ORBIT": "REF_ORBIT",
+            "ECI_STATE": "ECI_STATE",
+            "TLE": "TLE",
+            "": "EMPTY",
+        }
+    
+    @schemas.classproperty
+    def ORBITAL_ELEMENTS(cls):
+        return cls("ORBITAL_ELEMENTS")
+    
+    @schemas.classproperty
+    def REF_ORBIT(cls):
+        return cls("REF_ORBIT")
+    
+    @schemas.classproperty
+    def ECI_STATE(cls):
+        return cls("ECI_STATE")
+    
+    @schemas.classproperty
+    def TLE(cls):
+        return cls("TLE")
+    
+    @schemas.classproperty
+    def EMPTY(cls):
+        return cls("")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/component_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/side_categories.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_system_subsystems_components_.post import CreateComponent
-from sedaro_base_client.paths.models_branches_branch_id_system_subsystems_components_block_id.delete import DeleteComponent
-from sedaro_base_client.paths.models_branches_branch_id_system_subsystems_components_block_id.patch import UpdateComponent
-
-
-class ComponentApi(
-    CreateComponent,
-    DeleteComponent,
-    UpdateComponent,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class SideCategories(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "COMPONENT": "COMPONENT",
+            "SURFACE": "SURFACE",
+            "COOLER": "COOLER",
+        }
+    
+    @schemas.classproperty
+    def COMPONENT(cls):
+        return cls("COMPONENT")
+    
+    @schemas.classproperty
+    def SURFACE(cls):
+        return cls("SURFACE")
+    
+    @schemas.classproperty
+    def COOLER(cls):
+        return cls("COOLER")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/data_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/statuses.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,76 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.data_.get import GetData
-
-
-class DataApi(
-    GetData,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class Statuses(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "PENDING": "PENDING",
+            "RUNNING": "RUNNING",
+            "PAUSED": "PAUSED",
+            "TERMINATED": "TERMINATED",
+            "FAILED": "FAILED",
+            "SUCCEEDED": "SUCCEEDED",
+            "ERROR": "ERROR",
+        }
+    
+    @schemas.classproperty
+    def PENDING(cls):
+        return cls("PENDING")
+    
+    @schemas.classproperty
+    def RUNNING(cls):
+        return cls("RUNNING")
+    
+    @schemas.classproperty
+    def PAUSED(cls):
+        return cls("PAUSED")
+    
+    @schemas.classproperty
+    def TERMINATED(cls):
+        return cls("TERMINATED")
+    
+    @schemas.classproperty
+    def FAILED(cls):
+        return cls("FAILED")
+    
+    @schemas.classproperty
+    def SUCCEEDED(cls):
+        return cls("SUCCEEDED")
+    
+    @schemas.classproperty
+    def ERROR(cls):
+        return cls("ERROR")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/apis/tags/lock_pointing_mode_api.py` & `sedaro-4.0.0/src/sedaro_base_client/model/categories.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,76 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
-from sedaro_base_client.paths.models_branches_branch_id_gnc_pointing_modes_lock_.post import CreateLockPointingMode
-from sedaro_base_client.paths.models_branches_branch_id_gnc_pointing_modes_lock_block_id.delete import DeleteLockPointingMode
-from sedaro_base_client.paths.models_branches_branch_id_gnc_pointing_modes_lock_block_id.patch import UpdateLockPointingMode
-
-
-class LockPointingModeApi(
-    CreateLockPointingMode,
-    DeleteLockPointingMode,
-    UpdateLockPointingMode,
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from sedaro_base_client import schemas  # noqa: F401
+
+
+class Categories(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE: This class is auto generated by OpenAPI Generator
+    """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    An enumeration.
     """
-    pass
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "POWER": "POWER",
+            "CDH": "CDH",
+            "DATA_HANDLING": "DATA_HANDLING",
+            "GNC": "GNC",
+            "THERMAL": "THERMAL",
+            "STRUCTURE": "STRUCTURE",
+            "CUSTOM": "CUSTOM",
+        }
+    
+    @schemas.classproperty
+    def POWER(cls):
+        return cls("POWER")
+    
+    @schemas.classproperty
+    def CDH(cls):
+        return cls("CDH")
+    
+    @schemas.classproperty
+    def DATA_HANDLING(cls):
+        return cls("DATA_HANDLING")
+    
+    @schemas.classproperty
+    def GNC(cls):
+        return cls("GNC")
+    
+    @schemas.classproperty
+    def THERMAL(cls):
+        return cls("THERMAL")
+    
+    @schemas.classproperty
+    def STRUCTURE(cls):
+        return cls("STRUCTURE")
+    
+    @schemas.classproperty
+    def CUSTOM(cls):
+        return cls("CUSTOM")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/configuration.py` & `sedaro-4.0.0/src/sedaro_base_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
 import sys
@@ -351,15 +351,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 3.5.7\n"\
+               "Version of the API: 3.3.7\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/exceptions.py` & `sedaro-4.0.0/src/sedaro_base_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 import dataclasses
 import typing
 
 from urllib3._collections import HTTPHeaderDict
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_create.py` & `sedaro-4.0.0/src/sedaro_base_client/model/branch_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_delete_res.py` & `sedaro-4.0.0/src/sedaro_base_client/model/branch_delete_res.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_merge.py` & `sedaro-4.0.0/src/sedaro_base_client/model/branch_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_merge_conflicts_res.py` & `sedaro-4.0.0/src/sedaro_base_client/model/branch_merge_conflicts_res.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_scenario_res.py` & `sedaro-4.0.0/src/sedaro_base_client/model/target_group_to_satellite_condition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -19,451 +19,412 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 
-class BranchScenarioRes(
+class TargetGroupToSatelliteCondition(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Class to be used internally and inherited by `Metamodel` and `Block`. Adds helper methods and properties.
     """
 
 
     class MetaOapg:
         required = {
-            "shareable",
-            "blockGroupNames",
-            "dataSchema",
-            "blockIdToTypeMap",
-            "sharePwRqd",
-            "dateModified",
-            "repository",
-            "uuid",
-            "mission",
-            "dateCreated",
+            "tgParam",
             "name",
-            "numSimulations",
-            "id",
-            "user",
-            "blockClassToBlockGroupMap",
+            "relationship",
         }
         
         class properties:
             
             
             class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 32
-            id = schemas.IntSchema
-            dateCreated = schemas.DateTimeSchema
-            dateModified = schemas.DateTimeSchema
+                    max_length = 100
             
             
-            class repository(
+            class relationship(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            ConditionRelationship,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'repository':
+                ) -> 'relationship':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class mission(
+            class tgParam(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            TargetParameters,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'mission':
+                ) -> 'tgParam':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            id = schemas.StrSchema
+        
+            @staticmethod
+            def metamodel() -> typing.Type['Metamodel']:
+                return Metamodel
+            terminator = schemas.BoolSchema
+            compliance = schemas.BoolSchema
+            targetGroup = schemas.StrSchema
+            isFilter = schemas.StrSchema
+            
+            
+            class targetCompliance(
+                schemas.DictSchema
+            ):
+            
+            
+                class MetaOapg:
+                    additional_properties = schemas.BoolSchema
+                
+                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    # dict_instance[name] accessor
+                    return super().__getitem__(name)
+                
+                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    return super().get_item_oapg(name)
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[MetaOapg.additional_properties, bool, ],
+                ) -> 'targetCompliance':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class user(
+            class countRelationship(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            ConditionRelationship,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'user':
+                ) -> 'countRelationship':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            uuid = schemas.UUIDSchema
-            shareable = schemas.BoolSchema
-            sharePwRqd = schemas.BoolSchema
-            numSimulations = schemas.IntSchema
-            dataSchema = schemas.DictSchema
+            countValue = schemas.IntSchema
             
             
-            class blockIdToTypeMap(
-                schemas.DictSchema
+            class groupRoller(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    additional_properties = schemas.StrSchema
-                
-                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    # dict_instance[name] accessor
-                    return super().__getitem__(name)
-                
-                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    return super().get_item_oapg(name)
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            GroupRollers,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'blockIdToTypeMap':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'groupRoller':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class blockClassToBlockGroupMap(
-                schemas.DictSchema
+            class satParam(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    additional_properties = schemas.StrSchema
-                
-                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    # dict_instance[name] accessor
-                    return super().__getitem__(name)
-                
-                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    return super().get_item_oapg(name)
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            SatelliteParameters,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'blockClassToBlockGroupMap':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'satParam':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            
-            
-            class blockGroupNames(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'blockGroupNames':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
-            
-            class description(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 300
             __annotations__ = {
                 "name": name,
+                "relationship": relationship,
+                "tgParam": tgParam,
                 "id": id,
-                "dateCreated": dateCreated,
-                "dateModified": dateModified,
-                "repository": repository,
-                "mission": mission,
-                "user": user,
-                "uuid": uuid,
-                "shareable": shareable,
-                "sharePwRqd": sharePwRqd,
-                "numSimulations": numSimulations,
-                "dataSchema": dataSchema,
-                "blockIdToTypeMap": blockIdToTypeMap,
-                "blockClassToBlockGroupMap": blockClassToBlockGroupMap,
-                "blockGroupNames": blockGroupNames,
-                "description": description,
+                "metamodel": metamodel,
+                "terminator": terminator,
+                "compliance": compliance,
+                "targetGroup": targetGroup,
+                "isFilter": isFilter,
+                "targetCompliance": targetCompliance,
+                "countRelationship": countRelationship,
+                "countValue": countValue,
+                "groupRoller": groupRoller,
+                "satParam": satParam,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
-    shareable: MetaOapg.properties.shareable
-    blockGroupNames: MetaOapg.properties.blockGroupNames
-    dataSchema: MetaOapg.properties.dataSchema
-    blockIdToTypeMap: MetaOapg.properties.blockIdToTypeMap
-    sharePwRqd: MetaOapg.properties.sharePwRqd
-    dateModified: MetaOapg.properties.dateModified
-    repository: MetaOapg.properties.repository
-    uuid: MetaOapg.properties.uuid
-    mission: MetaOapg.properties.mission
-    dateCreated: MetaOapg.properties.dateCreated
+    tgParam: MetaOapg.properties.tgParam
     name: MetaOapg.properties.name
-    numSimulations: MetaOapg.properties.numSimulations
-    id: MetaOapg.properties.id
-    user: MetaOapg.properties.user
-    blockClassToBlockGroupMap: MetaOapg.properties.blockClassToBlockGroupMap
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    relationship: MetaOapg.properties.relationship
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dateCreated"]) -> MetaOapg.properties.dateCreated: ...
+    def __getitem__(self, name: typing_extensions.Literal["tgParam"]) -> MetaOapg.properties.tgParam: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dateModified"]) -> MetaOapg.properties.dateModified: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["repository"]) -> MetaOapg.properties.repository: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["mission"]) -> MetaOapg.properties.mission: ...
+    def __getitem__(self, name: typing_extensions.Literal["relationship"]) -> MetaOapg.properties.relationship: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def __getitem__(self, name: typing_extensions.Literal["metamodel"]) -> 'Metamodel': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["shareable"]) -> MetaOapg.properties.shareable: ...
+    def __getitem__(self, name: typing_extensions.Literal["terminator"]) -> MetaOapg.properties.terminator: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sharePwRqd"]) -> MetaOapg.properties.sharePwRqd: ...
+    def __getitem__(self, name: typing_extensions.Literal["compliance"]) -> MetaOapg.properties.compliance: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numSimulations"]) -> MetaOapg.properties.numSimulations: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetGroup"]) -> MetaOapg.properties.targetGroup: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dataSchema"]) -> MetaOapg.properties.dataSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["isFilter"]) -> MetaOapg.properties.isFilter: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockIdToTypeMap"]) -> MetaOapg.properties.blockIdToTypeMap: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetCompliance"]) -> MetaOapg.properties.targetCompliance: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockClassToBlockGroupMap"]) -> MetaOapg.properties.blockClassToBlockGroupMap: ...
+    def __getitem__(self, name: typing_extensions.Literal["countRelationship"]) -> MetaOapg.properties.countRelationship: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockGroupNames"]) -> MetaOapg.properties.blockGroupNames: ...
+    def __getitem__(self, name: typing_extensions.Literal["countValue"]) -> MetaOapg.properties.countValue: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["groupRoller"]) -> MetaOapg.properties.groupRoller: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["satParam"]) -> MetaOapg.properties.satParam: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "dateCreated", "dateModified", "repository", "mission", "user", "uuid", "shareable", "sharePwRqd", "numSimulations", "dataSchema", "blockIdToTypeMap", "blockClassToBlockGroupMap", "blockGroupNames", "description", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["tgParam"], typing_extensions.Literal["name"], typing_extensions.Literal["relationship"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["terminator"], typing_extensions.Literal["compliance"], typing_extensions.Literal["targetGroup"], typing_extensions.Literal["isFilter"], typing_extensions.Literal["targetCompliance"], typing_extensions.Literal["countRelationship"], typing_extensions.Literal["countValue"], typing_extensions.Literal["groupRoller"], typing_extensions.Literal["satParam"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["tgParam"]) -> MetaOapg.properties.tgParam: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dateCreated"]) -> MetaOapg.properties.dateCreated: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dateModified"]) -> MetaOapg.properties.dateModified: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["repository"]) -> MetaOapg.properties.repository: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["mission"]) -> MetaOapg.properties.mission: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["relationship"]) -> MetaOapg.properties.relationship: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metamodel"]) -> typing.Union['Metamodel', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["shareable"]) -> MetaOapg.properties.shareable: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["terminator"]) -> typing.Union[MetaOapg.properties.terminator, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sharePwRqd"]) -> MetaOapg.properties.sharePwRqd: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["compliance"]) -> typing.Union[MetaOapg.properties.compliance, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numSimulations"]) -> MetaOapg.properties.numSimulations: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetGroup"]) -> typing.Union[MetaOapg.properties.targetGroup, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dataSchema"]) -> MetaOapg.properties.dataSchema: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["isFilter"]) -> typing.Union[MetaOapg.properties.isFilter, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockIdToTypeMap"]) -> MetaOapg.properties.blockIdToTypeMap: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetCompliance"]) -> typing.Union[MetaOapg.properties.targetCompliance, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockClassToBlockGroupMap"]) -> MetaOapg.properties.blockClassToBlockGroupMap: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["countRelationship"]) -> typing.Union[MetaOapg.properties.countRelationship, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockGroupNames"]) -> MetaOapg.properties.blockGroupNames: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["countValue"]) -> typing.Union[MetaOapg.properties.countValue, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["groupRoller"]) -> typing.Union[MetaOapg.properties.groupRoller, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["satParam"]) -> typing.Union[MetaOapg.properties.satParam, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "dateCreated", "dateModified", "repository", "mission", "user", "uuid", "shareable", "sharePwRqd", "numSimulations", "dataSchema", "blockIdToTypeMap", "blockClassToBlockGroupMap", "blockGroupNames", "description", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tgParam"], typing_extensions.Literal["name"], typing_extensions.Literal["relationship"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["terminator"], typing_extensions.Literal["compliance"], typing_extensions.Literal["targetGroup"], typing_extensions.Literal["isFilter"], typing_extensions.Literal["targetCompliance"], typing_extensions.Literal["countRelationship"], typing_extensions.Literal["countValue"], typing_extensions.Literal["groupRoller"], typing_extensions.Literal["satParam"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        shareable: typing.Union[MetaOapg.properties.shareable, bool, ],
-        blockGroupNames: typing.Union[MetaOapg.properties.blockGroupNames, list, tuple, ],
-        dataSchema: typing.Union[MetaOapg.properties.dataSchema, dict, frozendict.frozendict, ],
-        blockIdToTypeMap: typing.Union[MetaOapg.properties.blockIdToTypeMap, dict, frozendict.frozendict, ],
-        sharePwRqd: typing.Union[MetaOapg.properties.sharePwRqd, bool, ],
-        dateModified: typing.Union[MetaOapg.properties.dateModified, str, datetime, ],
-        repository: typing.Union[MetaOapg.properties.repository, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        uuid: typing.Union[MetaOapg.properties.uuid, str, uuid.UUID, ],
-        mission: typing.Union[MetaOapg.properties.mission, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        dateCreated: typing.Union[MetaOapg.properties.dateCreated, str, datetime, ],
+        tgParam: typing.Union[MetaOapg.properties.tgParam, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        numSimulations: typing.Union[MetaOapg.properties.numSimulations, decimal.Decimal, int, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        user: typing.Union[MetaOapg.properties.user, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        blockClassToBlockGroupMap: typing.Union[MetaOapg.properties.blockClassToBlockGroupMap, dict, frozendict.frozendict, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        relationship: typing.Union[MetaOapg.properties.relationship, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        metamodel: typing.Union['Metamodel', schemas.Unset] = schemas.unset,
+        terminator: typing.Union[MetaOapg.properties.terminator, bool, schemas.Unset] = schemas.unset,
+        compliance: typing.Union[MetaOapg.properties.compliance, bool, schemas.Unset] = schemas.unset,
+        targetGroup: typing.Union[MetaOapg.properties.targetGroup, str, schemas.Unset] = schemas.unset,
+        isFilter: typing.Union[MetaOapg.properties.isFilter, str, schemas.Unset] = schemas.unset,
+        targetCompliance: typing.Union[MetaOapg.properties.targetCompliance, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        countRelationship: typing.Union[MetaOapg.properties.countRelationship, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        countValue: typing.Union[MetaOapg.properties.countValue, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        groupRoller: typing.Union[MetaOapg.properties.groupRoller, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        satParam: typing.Union[MetaOapg.properties.satParam, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'BranchScenarioRes':
+    ) -> 'TargetGroupToSatelliteCondition':
         return super().__new__(
             cls,
             *_args,
-            shareable=shareable,
-            blockGroupNames=blockGroupNames,
-            dataSchema=dataSchema,
-            blockIdToTypeMap=blockIdToTypeMap,
-            sharePwRqd=sharePwRqd,
-            dateModified=dateModified,
-            repository=repository,
-            uuid=uuid,
-            mission=mission,
-            dateCreated=dateCreated,
+            tgParam=tgParam,
             name=name,
-            numSimulations=numSimulations,
+            relationship=relationship,
             id=id,
-            user=user,
-            blockClassToBlockGroupMap=blockClassToBlockGroupMap,
-            description=description,
+            metamodel=metamodel,
+            terminator=terminator,
+            compliance=compliance,
+            targetGroup=targetGroup,
+            isFilter=isFilter,
+            targetCompliance=targetCompliance,
+            countRelationship=countRelationship,
+            countValue=countValue,
+            groupRoller=groupRoller,
+            satParam=satParam,
             _configuration=_configuration,
-            **kwargs,
         )
+
+from sedaro_base_client.model.condition_relationship import ConditionRelationship
+from sedaro_base_client.model.group_rollers import GroupRollers
+from sedaro_base_client.model.metamodel import Metamodel
+from sedaro_base_client.model.satellite_parameters import SatelliteParameters
+from sedaro_base_client.model.target_parameters import TargetParameters
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_update.py` & `sedaro-4.0.0/src/sedaro_base_client/model/duration_operational_mode18.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -19,115 +19,89 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 
-class BranchUpdate(
+class DurationOperationalMode18(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         
         class properties:
+            s = schemas.NumberSchema
+            hour = schemas.NumberSchema
             
             
-            class name(
-                schemas.StrSchema
+            class day(
+                schemas.NumberSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 32
-            
-            
-            class description(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 300
-            shareable = schemas.BoolSchema
-            
-            
-            class password(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 128
-                    min_length = 8
+                    inclusive_minimum = 0.0
+            min = schemas.NumberSchema
             __annotations__ = {
-                "name": name,
-                "description": description,
-                "shareable": shareable,
-                "password": password,
+                "s": s,
+                "hour": hour,
+                "day": day,
+                "min": min,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["s"]) -> MetaOapg.properties.s: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["shareable"]) -> MetaOapg.properties.shareable: ...
+    def __getitem__(self, name: typing_extensions.Literal["hour"]) -> MetaOapg.properties.hour: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["password"]) -> MetaOapg.properties.password: ...
+    def __getitem__(self, name: typing_extensions.Literal["day"]) -> MetaOapg.properties.day: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["min"]) -> MetaOapg.properties.min: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "description", "shareable", "password", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["s"], typing_extensions.Literal["hour"], typing_extensions.Literal["day"], typing_extensions.Literal["min"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["s"]) -> typing.Union[MetaOapg.properties.s, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["shareable"]) -> typing.Union[MetaOapg.properties.shareable, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["hour"]) -> typing.Union[MetaOapg.properties.hour, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["password"]) -> typing.Union[MetaOapg.properties.password, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["day"]) -> typing.Union[MetaOapg.properties.day, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["min"]) -> typing.Union[MetaOapg.properties.min, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "description", "shareable", "password", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["s"], typing_extensions.Literal["hour"], typing_extensions.Literal["day"], typing_extensions.Literal["min"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        shareable: typing.Union[MetaOapg.properties.shareable, bool, schemas.Unset] = schemas.unset,
-        password: typing.Union[MetaOapg.properties.password, str, schemas.Unset] = schemas.unset,
+        s: typing.Union[MetaOapg.properties.s, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        hour: typing.Union[MetaOapg.properties.hour, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        day: typing.Union[MetaOapg.properties.day, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        min: typing.Union[MetaOapg.properties.min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'BranchUpdate':
+    ) -> 'DurationOperationalMode18':
         return super().__new__(
             cls,
             *_args,
-            name=name,
-            description=description,
-            shareable=shareable,
-            password=password,
+            s=s,
+            hour=hour,
+            day=day,
+            min=min,
             _configuration=_configuration,
-            **kwargs,
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_vehicle_res.py` & `sedaro-4.0.0/src/sedaro_base_client/model/target_group_to_target_condition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -19,451 +19,423 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 
-class BranchVehicleRes(
+class TargetGroupToTargetCondition(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Class to be used internally and inherited by `Metamodel` and `Block`. Adds helper methods and properties.
     """
 
 
     class MetaOapg:
         required = {
-            "shareable",
-            "blockGroupNames",
-            "dataSchema",
-            "blockIdToTypeMap",
-            "sharePwRqd",
-            "dateModified",
-            "repository",
-            "uuid",
-            "mission",
-            "dateCreated",
+            "tgParam",
             "name",
-            "numSimulations",
-            "id",
-            "user",
-            "blockClassToBlockGroupMap",
+            "targetParam",
+            "relationship",
         }
         
         class properties:
             
             
             class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 32
-            id = schemas.IntSchema
-            dateCreated = schemas.DateTimeSchema
-            dateModified = schemas.DateTimeSchema
+                    max_length = 100
             
             
-            class repository(
+            class relationship(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            ConditionRelationship,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'repository':
+                ) -> 'relationship':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class mission(
+            class tgParam(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            TargetParameters,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'mission':
+                ) -> 'tgParam':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class user(
+            class targetParam(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.DictSchema
-                    any_of_1 = schemas.IntSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            TargetParameters,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'user':
+                ) -> 'targetParam':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            uuid = schemas.UUIDSchema
-            shareable = schemas.BoolSchema
-            sharePwRqd = schemas.BoolSchema
-            numSimulations = schemas.IntSchema
-            dataSchema = schemas.DictSchema
+            id = schemas.StrSchema
+        
+            @staticmethod
+            def metamodel() -> typing.Type['Metamodel']:
+                return Metamodel
+            terminator = schemas.BoolSchema
+            compliance = schemas.BoolSchema
+            targetGroup = schemas.StrSchema
+            isFilter = schemas.StrSchema
             
             
-            class blockIdToTypeMap(
+            class targetCompliance(
                 schemas.DictSchema
             ):
             
             
                 class MetaOapg:
-                    additional_properties = schemas.StrSchema
+                    additional_properties = schemas.BoolSchema
                 
                 def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
                     # dict_instance[name] accessor
                     return super().__getitem__(name)
                 
                 def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
                     return super().get_item_oapg(name)
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'blockIdToTypeMap':
+                    **kwargs: typing.Union[MetaOapg.additional_properties, bool, ],
+                ) -> 'targetCompliance':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class blockClassToBlockGroupMap(
-                schemas.DictSchema
+            class countRelationship(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    additional_properties = schemas.StrSchema
-                
-                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    # dict_instance[name] accessor
-                    return super().__getitem__(name)
-                
-                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    return super().get_item_oapg(name)
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ConditionRelationship,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'blockClassToBlockGroupMap':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'countRelationship':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            countValue = schemas.IntSchema
             
             
-            class blockGroupNames(
-                schemas.ListSchema
+            class groupRoller(
+                schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            GroupRollers,
+                        ]
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'blockGroupNames':
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'groupRoller':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
+                        **kwargs,
                     )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
-            
-            class description(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 300
+            targetA = schemas.StrSchema
             __annotations__ = {
                 "name": name,
+                "relationship": relationship,
+                "tgParam": tgParam,
+                "targetParam": targetParam,
                 "id": id,
-                "dateCreated": dateCreated,
-                "dateModified": dateModified,
-                "repository": repository,
-                "mission": mission,
-                "user": user,
-                "uuid": uuid,
-                "shareable": shareable,
-                "sharePwRqd": sharePwRqd,
-                "numSimulations": numSimulations,
-                "dataSchema": dataSchema,
-                "blockIdToTypeMap": blockIdToTypeMap,
-                "blockClassToBlockGroupMap": blockClassToBlockGroupMap,
-                "blockGroupNames": blockGroupNames,
-                "description": description,
+                "metamodel": metamodel,
+                "terminator": terminator,
+                "compliance": compliance,
+                "targetGroup": targetGroup,
+                "isFilter": isFilter,
+                "targetCompliance": targetCompliance,
+                "countRelationship": countRelationship,
+                "countValue": countValue,
+                "groupRoller": groupRoller,
+                "targetA": targetA,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
-    shareable: MetaOapg.properties.shareable
-    blockGroupNames: MetaOapg.properties.blockGroupNames
-    dataSchema: MetaOapg.properties.dataSchema
-    blockIdToTypeMap: MetaOapg.properties.blockIdToTypeMap
-    sharePwRqd: MetaOapg.properties.sharePwRqd
-    dateModified: MetaOapg.properties.dateModified
-    repository: MetaOapg.properties.repository
-    uuid: MetaOapg.properties.uuid
-    mission: MetaOapg.properties.mission
-    dateCreated: MetaOapg.properties.dateCreated
+    tgParam: MetaOapg.properties.tgParam
     name: MetaOapg.properties.name
-    numSimulations: MetaOapg.properties.numSimulations
-    id: MetaOapg.properties.id
-    user: MetaOapg.properties.user
-    blockClassToBlockGroupMap: MetaOapg.properties.blockClassToBlockGroupMap
+    targetParam: MetaOapg.properties.targetParam
+    relationship: MetaOapg.properties.relationship
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["tgParam"]) -> MetaOapg.properties.tgParam: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dateCreated"]) -> MetaOapg.properties.dateCreated: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dateModified"]) -> MetaOapg.properties.dateModified: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["repository"]) -> MetaOapg.properties.repository: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetParam"]) -> MetaOapg.properties.targetParam: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["mission"]) -> MetaOapg.properties.mission: ...
+    def __getitem__(self, name: typing_extensions.Literal["relationship"]) -> MetaOapg.properties.relationship: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def __getitem__(self, name: typing_extensions.Literal["metamodel"]) -> 'Metamodel': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["shareable"]) -> MetaOapg.properties.shareable: ...
+    def __getitem__(self, name: typing_extensions.Literal["terminator"]) -> MetaOapg.properties.terminator: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sharePwRqd"]) -> MetaOapg.properties.sharePwRqd: ...
+    def __getitem__(self, name: typing_extensions.Literal["compliance"]) -> MetaOapg.properties.compliance: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numSimulations"]) -> MetaOapg.properties.numSimulations: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetGroup"]) -> MetaOapg.properties.targetGroup: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dataSchema"]) -> MetaOapg.properties.dataSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["isFilter"]) -> MetaOapg.properties.isFilter: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockIdToTypeMap"]) -> MetaOapg.properties.blockIdToTypeMap: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetCompliance"]) -> MetaOapg.properties.targetCompliance: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockClassToBlockGroupMap"]) -> MetaOapg.properties.blockClassToBlockGroupMap: ...
+    def __getitem__(self, name: typing_extensions.Literal["countRelationship"]) -> MetaOapg.properties.countRelationship: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["blockGroupNames"]) -> MetaOapg.properties.blockGroupNames: ...
+    def __getitem__(self, name: typing_extensions.Literal["countValue"]) -> MetaOapg.properties.countValue: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["groupRoller"]) -> MetaOapg.properties.groupRoller: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["targetA"]) -> MetaOapg.properties.targetA: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "dateCreated", "dateModified", "repository", "mission", "user", "uuid", "shareable", "sharePwRqd", "numSimulations", "dataSchema", "blockIdToTypeMap", "blockClassToBlockGroupMap", "blockGroupNames", "description", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["tgParam"], typing_extensions.Literal["name"], typing_extensions.Literal["targetParam"], typing_extensions.Literal["relationship"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["terminator"], typing_extensions.Literal["compliance"], typing_extensions.Literal["targetGroup"], typing_extensions.Literal["isFilter"], typing_extensions.Literal["targetCompliance"], typing_extensions.Literal["countRelationship"], typing_extensions.Literal["countValue"], typing_extensions.Literal["groupRoller"], typing_extensions.Literal["targetA"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dateCreated"]) -> MetaOapg.properties.dateCreated: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["tgParam"]) -> MetaOapg.properties.tgParam: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dateModified"]) -> MetaOapg.properties.dateModified: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["repository"]) -> MetaOapg.properties.repository: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetParam"]) -> MetaOapg.properties.targetParam: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["mission"]) -> MetaOapg.properties.mission: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["relationship"]) -> MetaOapg.properties.relationship: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metamodel"]) -> typing.Union['Metamodel', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["shareable"]) -> MetaOapg.properties.shareable: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["terminator"]) -> typing.Union[MetaOapg.properties.terminator, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sharePwRqd"]) -> MetaOapg.properties.sharePwRqd: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["compliance"]) -> typing.Union[MetaOapg.properties.compliance, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numSimulations"]) -> MetaOapg.properties.numSimulations: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetGroup"]) -> typing.Union[MetaOapg.properties.targetGroup, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dataSchema"]) -> MetaOapg.properties.dataSchema: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["isFilter"]) -> typing.Union[MetaOapg.properties.isFilter, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockIdToTypeMap"]) -> MetaOapg.properties.blockIdToTypeMap: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetCompliance"]) -> typing.Union[MetaOapg.properties.targetCompliance, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockClassToBlockGroupMap"]) -> MetaOapg.properties.blockClassToBlockGroupMap: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["countRelationship"]) -> typing.Union[MetaOapg.properties.countRelationship, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["blockGroupNames"]) -> MetaOapg.properties.blockGroupNames: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["countValue"]) -> typing.Union[MetaOapg.properties.countValue, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["groupRoller"]) -> typing.Union[MetaOapg.properties.groupRoller, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["targetA"]) -> typing.Union[MetaOapg.properties.targetA, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "dateCreated", "dateModified", "repository", "mission", "user", "uuid", "shareable", "sharePwRqd", "numSimulations", "dataSchema", "blockIdToTypeMap", "blockClassToBlockGroupMap", "blockGroupNames", "description", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tgParam"], typing_extensions.Literal["name"], typing_extensions.Literal["targetParam"], typing_extensions.Literal["relationship"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["terminator"], typing_extensions.Literal["compliance"], typing_extensions.Literal["targetGroup"], typing_extensions.Literal["isFilter"], typing_extensions.Literal["targetCompliance"], typing_extensions.Literal["countRelationship"], typing_extensions.Literal["countValue"], typing_extensions.Literal["groupRoller"], typing_extensions.Literal["targetA"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        shareable: typing.Union[MetaOapg.properties.shareable, bool, ],
-        blockGroupNames: typing.Union[MetaOapg.properties.blockGroupNames, list, tuple, ],
-        dataSchema: typing.Union[MetaOapg.properties.dataSchema, dict, frozendict.frozendict, ],
-        blockIdToTypeMap: typing.Union[MetaOapg.properties.blockIdToTypeMap, dict, frozendict.frozendict, ],
-        sharePwRqd: typing.Union[MetaOapg.properties.sharePwRqd, bool, ],
-        dateModified: typing.Union[MetaOapg.properties.dateModified, str, datetime, ],
-        repository: typing.Union[MetaOapg.properties.repository, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        uuid: typing.Union[MetaOapg.properties.uuid, str, uuid.UUID, ],
-        mission: typing.Union[MetaOapg.properties.mission, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        dateCreated: typing.Union[MetaOapg.properties.dateCreated, str, datetime, ],
+        tgParam: typing.Union[MetaOapg.properties.tgParam, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        numSimulations: typing.Union[MetaOapg.properties.numSimulations, decimal.Decimal, int, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        user: typing.Union[MetaOapg.properties.user, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        blockClassToBlockGroupMap: typing.Union[MetaOapg.properties.blockClassToBlockGroupMap, dict, frozendict.frozendict, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        targetParam: typing.Union[MetaOapg.properties.targetParam, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        relationship: typing.Union[MetaOapg.properties.relationship, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        metamodel: typing.Union['Metamodel', schemas.Unset] = schemas.unset,
+        terminator: typing.Union[MetaOapg.properties.terminator, bool, schemas.Unset] = schemas.unset,
+        compliance: typing.Union[MetaOapg.properties.compliance, bool, schemas.Unset] = schemas.unset,
+        targetGroup: typing.Union[MetaOapg.properties.targetGroup, str, schemas.Unset] = schemas.unset,
+        isFilter: typing.Union[MetaOapg.properties.isFilter, str, schemas.Unset] = schemas.unset,
+        targetCompliance: typing.Union[MetaOapg.properties.targetCompliance, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        countRelationship: typing.Union[MetaOapg.properties.countRelationship, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        countValue: typing.Union[MetaOapg.properties.countValue, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        groupRoller: typing.Union[MetaOapg.properties.groupRoller, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        targetA: typing.Union[MetaOapg.properties.targetA, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'BranchVehicleRes':
+    ) -> 'TargetGroupToTargetCondition':
         return super().__new__(
             cls,
             *_args,
-            shareable=shareable,
-            blockGroupNames=blockGroupNames,
-            dataSchema=dataSchema,
-            blockIdToTypeMap=blockIdToTypeMap,
-            sharePwRqd=sharePwRqd,
-            dateModified=dateModified,
-            repository=repository,
-            uuid=uuid,
-            mission=mission,
-            dateCreated=dateCreated,
+            tgParam=tgParam,
             name=name,
-            numSimulations=numSimulations,
+            targetParam=targetParam,
+            relationship=relationship,
             id=id,
-            user=user,
-            blockClassToBlockGroupMap=blockClassToBlockGroupMap,
-            description=description,
+            metamodel=metamodel,
+            terminator=terminator,
+            compliance=compliance,
+            targetGroup=targetGroup,
+            isFilter=isFilter,
+            targetCompliance=targetCompliance,
+            countRelationship=countRelationship,
+            countValue=countValue,
+            groupRoller=groupRoller,
+            targetA=targetA,
             _configuration=_configuration,
-            **kwargs,
         )
+
+from sedaro_base_client.model.condition_relationship import ConditionRelationship
+from sedaro_base_client.model.group_rollers import GroupRollers
+from sedaro_base_client.model.metamodel import Metamodel
+from sedaro_base_client.model.target_parameters import TargetParameters
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/branch_verify_password.py` & `sedaro-4.0.0/src/sedaro_base_client/model/branch_verify_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/conflicts_obj.py` & `sedaro-4.0.0/src/sedaro_base_client/model/conflicts_obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/data_service_response.py` & `sedaro-4.0.0/src/sedaro_base_client/model/data_service_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/data_set.py` & `sedaro-4.0.0/src/sedaro_base_client/model/data_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/deleted_entity.py` & `sedaro-4.0.0/src/sedaro_base_client/model/deleted_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/http_validation_error.py` & `sedaro-4.0.0/src/sedaro_base_client/model/http_validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/message_res.py` & `sedaro-4.0.0/src/sedaro_base_client/model/message_res.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/simulation_job.py` & `sedaro-4.0.0/src/sedaro_base_client/model/celestial_vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -19,40 +19,37 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 
-class SimulationJob(
+class CelestialVector(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Class to be used internally and inherited by `Metamodel` and `Block`. Adds helper methods and properties.
     """
 
 
     class MetaOapg:
         required = {
-            "dataId",
-            "bedRef",
-            "startTime",
-            "stopTime",
-            "id",
-            "simulatedAgents",
-            "status",
+            "name",
+            "celestialPointingDirection",
         }
         
         class properties:
-            id = schemas.IntSchema
+            name = schemas.StrSchema
             
             
-            class status(
+            class celestialPointingDirection(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -62,179 +59,121 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            Statuses,
+                            CelestialPointingDirections,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'status':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
-            bedRef = schemas.StrSchema
-            dataId = schemas.IntSchema
-            startTime = schemas.NumberSchema
-            stopTime = schemas.NumberSchema
-            
-            
-            class simulatedAgents(
-                schemas.DictSchema
-            ):
-            
-            
-                class MetaOapg:
-                    additional_properties = schemas.StrSchema
-                
-                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    # dict_instance[name] accessor
-                    return super().__getitem__(name)
-                
-                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-                    return super().get_item_oapg(name)
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[dict, frozendict.frozendict, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-                ) -> 'simulatedAgents':
+                ) -> 'celestialPointingDirection':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            realTime = schemas.BoolSchema
-            progress = schemas.DictSchema
+            id = schemas.StrSchema
+        
+            @staticmethod
+            def metamodel() -> typing.Type['Metamodel']:
+                return Metamodel
+            truth = schemas.AnyTypeSchema
+            estimate = schemas.AnyTypeSchema
+            eclipsed = schemas.BoolSchema
             __annotations__ = {
+                "name": name,
+                "celestialPointingDirection": celestialPointingDirection,
                 "id": id,
-                "status": status,
-                "bedRef": bedRef,
-                "dataId": dataId,
-                "startTime": startTime,
-                "stopTime": stopTime,
-                "simulatedAgents": simulatedAgents,
-                "realTime": realTime,
-                "progress": progress,
+                "metamodel": metamodel,
+                "truth": truth,
+                "estimate": estimate,
+                "eclipsed": eclipsed,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
-    dataId: MetaOapg.properties.dataId
-    bedRef: MetaOapg.properties.bedRef
-    startTime: MetaOapg.properties.startTime
-    stopTime: MetaOapg.properties.stopTime
-    id: MetaOapg.properties.id
-    simulatedAgents: MetaOapg.properties.simulatedAgents
-    status: MetaOapg.properties.status
+    name: MetaOapg.properties.name
+    celestialPointingDirection: MetaOapg.properties.celestialPointingDirection
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
+    def __getitem__(self, name: typing_extensions.Literal["celestialPointingDirection"]) -> MetaOapg.properties.celestialPointingDirection: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["bedRef"]) -> MetaOapg.properties.bedRef: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["dataId"]) -> MetaOapg.properties.dataId: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["startTime"]) -> MetaOapg.properties.startTime: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["stopTime"]) -> MetaOapg.properties.stopTime: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["simulatedAgents"]) -> MetaOapg.properties.simulatedAgents: ...
+    def __getitem__(self, name: typing_extensions.Literal["metamodel"]) -> 'Metamodel': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["realTime"]) -> MetaOapg.properties.realTime: ...
+    def __getitem__(self, name: typing_extensions.Literal["truth"]) -> MetaOapg.properties.truth: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["progress"]) -> MetaOapg.properties.progress: ...
+    def __getitem__(self, name: typing_extensions.Literal["estimate"]) -> MetaOapg.properties.estimate: ...
     
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    def __getitem__(self, name: typing_extensions.Literal["eclipsed"]) -> MetaOapg.properties.eclipsed: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "status", "bedRef", "dataId", "startTime", "stopTime", "simulatedAgents", "realTime", "progress", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name"], typing_extensions.Literal["celestialPointingDirection"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["truth"], typing_extensions.Literal["estimate"], typing_extensions.Literal["eclipsed"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["status"]) -> MetaOapg.properties.status: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["bedRef"]) -> MetaOapg.properties.bedRef: ...
-    
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["dataId"]) -> MetaOapg.properties.dataId: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["startTime"]) -> MetaOapg.properties.startTime: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["celestialPointingDirection"]) -> MetaOapg.properties.celestialPointingDirection: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["stopTime"]) -> MetaOapg.properties.stopTime: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["simulatedAgents"]) -> MetaOapg.properties.simulatedAgents: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["metamodel"]) -> typing.Union['Metamodel', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["realTime"]) -> typing.Union[MetaOapg.properties.realTime, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["truth"]) -> typing.Union[MetaOapg.properties.truth, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["progress"]) -> typing.Union[MetaOapg.properties.progress, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["estimate"]) -> typing.Union[MetaOapg.properties.estimate, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["eclipsed"]) -> typing.Union[MetaOapg.properties.eclipsed, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "status", "bedRef", "dataId", "startTime", "stopTime", "simulatedAgents", "realTime", "progress", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name"], typing_extensions.Literal["celestialPointingDirection"], typing_extensions.Literal["id"], typing_extensions.Literal["metamodel"], typing_extensions.Literal["truth"], typing_extensions.Literal["estimate"], typing_extensions.Literal["eclipsed"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        dataId: typing.Union[MetaOapg.properties.dataId, decimal.Decimal, int, ],
-        bedRef: typing.Union[MetaOapg.properties.bedRef, str, ],
-        startTime: typing.Union[MetaOapg.properties.startTime, decimal.Decimal, int, float, ],
-        stopTime: typing.Union[MetaOapg.properties.stopTime, decimal.Decimal, int, float, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        simulatedAgents: typing.Union[MetaOapg.properties.simulatedAgents, dict, frozendict.frozendict, ],
-        status: typing.Union[MetaOapg.properties.status, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        realTime: typing.Union[MetaOapg.properties.realTime, bool, schemas.Unset] = schemas.unset,
-        progress: typing.Union[MetaOapg.properties.progress, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        celestialPointingDirection: typing.Union[MetaOapg.properties.celestialPointingDirection, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        metamodel: typing.Union['Metamodel', schemas.Unset] = schemas.unset,
+        truth: typing.Union[MetaOapg.properties.truth, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        estimate: typing.Union[MetaOapg.properties.estimate, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        eclipsed: typing.Union[MetaOapg.properties.eclipsed, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SimulationJob':
+    ) -> 'CelestialVector':
         return super().__new__(
             cls,
             *_args,
-            dataId=dataId,
-            bedRef=bedRef,
-            startTime=startTime,
-            stopTime=stopTime,
+            name=name,
+            celestialPointingDirection=celestialPointingDirection,
             id=id,
-            simulatedAgents=simulatedAgents,
-            status=status,
-            realTime=realTime,
-            progress=progress,
+            metamodel=metamodel,
+            truth=truth,
+            estimate=estimate,
+            eclipsed=eclipsed,
             _configuration=_configuration,
-            **kwargs,
         )
 
-from sedaro_base_client.model.statuses import Statuses
+from sedaro_base_client.model.celestial_pointing_directions import CelestialPointingDirections
+from sedaro_base_client.model.metamodel import Metamodel
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/statuses.py` & `sedaro-4.0.0/src/sedaro_base_client/model/celestial_pointing_directions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
@@ -19,58 +19,78 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 
-class Statuses(
+class CelestialPointingDirections(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     An enumeration.
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
-            "PENDING": "PENDING",
-            "RUNNING": "RUNNING",
-            "PAUSED": "PAUSED",
-            "TERMINATED": "TERMINATED",
-            "FAILED": "FAILED",
-            "SUCCEEDED": "SUCCEEDED",
-            "ERROR": "ERROR",
+            "SUN": "SUN",
+            "MOON": "MOON",
+            "EARTH": "EARTH",
+            "MERCURY": "MERCURY",
+            "VENUS": "VENUS",
+            "MARS": "MARS",
+            "JUPITER": "JUPITER",
+            "SATURN": "SATURN",
+            "URANUS": "URANUS",
+            "NEPTUNE": "NEPTUNE",
+            "PLUTO": "PLUTO",
         }
     
     @schemas.classproperty
-    def PENDING(cls):
-        return cls("PENDING")
+    def SUN(cls):
+        return cls("SUN")
     
     @schemas.classproperty
-    def RUNNING(cls):
-        return cls("RUNNING")
+    def MOON(cls):
+        return cls("MOON")
     
     @schemas.classproperty
-    def PAUSED(cls):
-        return cls("PAUSED")
+    def EARTH(cls):
+        return cls("EARTH")
     
     @schemas.classproperty
-    def TERMINATED(cls):
-        return cls("TERMINATED")
+    def MERCURY(cls):
+        return cls("MERCURY")
     
     @schemas.classproperty
-    def FAILED(cls):
-        return cls("FAILED")
+    def VENUS(cls):
+        return cls("VENUS")
     
     @schemas.classproperty
-    def SUCCEEDED(cls):
-        return cls("SUCCEEDED")
+    def MARS(cls):
+        return cls("MARS")
     
     @schemas.classproperty
-    def ERROR(cls):
-        return cls("ERROR")
+    def JUPITER(cls):
+        return cls("JUPITER")
+    
+    @schemas.classproperty
+    def SATURN(cls):
+        return cls("SATURN")
+    
+    @schemas.classproperty
+    def URANUS(cls):
+        return cls("URANUS")
+    
+    @schemas.classproperty
+    def NEPTUNE(cls):
+        return cls("NEPTUNE")
+    
+    @schemas.classproperty
+    def PLUTO(cls):
+        return cls("PLUTO")
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/model/validation_error.py` & `sedaro-4.0.0/src/sedaro_base_client/model/validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/data_/get.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,71 +21,46 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
-from sedaro_base_client.model.data_service_response import DataServiceResponse
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
+from sedaro_base_client.model.branch_delete_res import BranchDeleteRes
 
 from . import path
 
-# Query params
-IdSchema = schemas.IntSchema
-StartSchema = schemas.NumberSchema
-StopSchema = schemas.NumberSchema
-BinWidthSchema = schemas.NumberSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
+# Path params
+BranchIdSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    'RequestRequiredPathParams',
     {
-        'id': typing.Union[IdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
+RequestOptionalPathParams = typing_extensions.TypedDict(
+    'RequestOptionalPathParams',
     {
-        'start': typing.Union[StartSchema, decimal.Decimal, int, float, ],
-        'stop': typing.Union[StopSchema, decimal.Decimal, int, float, ],
-        'binWidth': typing.Union[BinWidthSchema, decimal.Decimal, int, float, ],
     },
     total=False
 )
 
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_query_id = api_client.QueryParameter(
-    name="id",
-    style=api_client.ParameterStyle.FORM,
-    schema=IdSchema,
+request_path_branch_id = api_client.PathParameter(
+    name="branchId",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=BranchIdSchema,
     required=True,
-    explode=True,
 )
-request_query_start = api_client.QueryParameter(
-    name="start",
-    style=api_client.ParameterStyle.FORM,
-    schema=StartSchema,
-    explode=True,
-)
-request_query_stop = api_client.QueryParameter(
-    name="stop",
-    style=api_client.ParameterStyle.FORM,
-    schema=StopSchema,
-    explode=True,
-)
-request_query_bin_width = api_client.QueryParameter(
-    name="binWidth",
-    style=api_client.ParameterStyle.FORM,
-    schema=BinWidthSchema,
-    explode=True,
-)
-SchemaFor200ResponseBodyApplicationJson = DataServiceResponse
+SchemaFor200ResponseBodyApplicationJson = BranchDeleteRes
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -126,90 +101,87 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_data_oapg(
+    def _delete_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_data_oapg(
+    def _delete_branch_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_data_oapg(
+    def _delete_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_data_oapg(
+    def _delete_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Query Data
+        Delete a branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
-        prefix_separator_iterator = None
+        _path_params = {}
         for parameter in (
-            request_query_id,
-            request_query_start,
-            request_query_stop,
-            request_query_bin_width,
+            request_path_branch_id,
         ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
+            parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='delete'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -226,117 +198,117 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetData(BaseApi):
+class DeleteBranch(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_data(
+    def delete_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_data(
+    def delete_branch(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_data(
+    def delete_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_data(
+    def delete_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_data_oapg(
-            query_params=query_params,
+        return self._delete_branch_oapg(
+            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiFordelete(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def delete(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get(
+    def delete(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def delete(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def delete(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_data_oapg(
-            query_params=query_params,
+        return self._delete_branch_oapg(
+            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/delete.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,25 +21,27 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.simulation_job import SimulationJob
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
-from sedaro_base_client.model.branch_delete_res import BranchDeleteRes
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
+JobIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
+        'jobId': typing.Union[JobIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -52,15 +54,21 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = BranchDeleteRes
+request_path_job_id = api_client.PathParameter(
+    name="jobId",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=JobIdSchema,
+    required=True,
+)
+SchemaFor200ResponseBodyApplicationJson = SimulationJob
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -101,68 +109,69 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _delete_branch_oapg(
+    def _get_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _delete_branch_oapg(
+    def _get_simulation_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _delete_branch_oapg(
+    def _get_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _delete_branch_oapg(
+    def _get_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Delete a branch
+        Get a simulation
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
+            request_path_job_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -173,15 +182,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='delete'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -198,116 +207,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class DeleteBranch(BaseApi):
+class GetSimulation(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def delete_branch(
+    def get_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete_branch(
+    def get_simulation(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete_branch(
+    def get_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete_branch(
+    def get_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_branch_oapg(
+        return self._get_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiFordelete(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_branch_oapg(
+        return self._get_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/get.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/post.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,25 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.simulation_job import SimulationJob
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -51,15 +52,15 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = SimulationJob
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -100,58 +101,58 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_branch_oapg(
+    def _start_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_branch_oapg(
+    def _start_simulation_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_branch_oapg(
+    def _start_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_branch_oapg(
+    def _start_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get a branch
+        Start a simulation
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
@@ -172,15 +173,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -197,116 +198,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetBranch(BaseApi):
+class StartSimulation(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_branch(
+    def start_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_branch(
+    def start_simulation(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_branch(
+    def start_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_branch(
+    def start_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_branch_oapg(
+        return self._start_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def post(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_branch_oapg(
+        return self._start_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/patch.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,27 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
-from sedaro_base_client.model.branch_update import BranchUpdate
+from sedaro_base_client.model.branch_scenario_res import BranchScenarioRes
+from sedaro_base_client.model.branch_vehicle_res import BranchVehicleRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
+from sedaro_base_client.model.branch_create import BranchCreate
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -53,25 +55,61 @@
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
 # body param
-SchemaForRequestBodyApplicationJson = BranchUpdate
+SchemaForRequestBodyApplicationJson = BranchCreate
 
 
-request_body_branch_update = api_client.RequestBody(
+request_body_branch_create = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                BranchVehicleRes,
+                BranchScenarioRes,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -112,81 +150,81 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _update_branch_oapg(
+    def _create_branch_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _update_branch_oapg(
+    def _create_branch_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def _update_branch_oapg(
+    def _create_branch_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _update_branch_oapg(
+    def _create_branch_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _update_branch_oapg(
+    def _create_branch_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Update a branch
+        Branch off existing branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
@@ -210,23 +248,23 @@
                 _headers.add('Accept', accept_content_type)
 
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_branch_update.serialize(body, content_type)
+        serialized_data = request_body_branch_create.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='patch'.upper(),
+            method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             stream=stream,
             timeout=timeout,
         )
 
@@ -245,164 +283,164 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class UpdateBranch(BaseApi):
+class CreateBranch(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def update_branch(
+    def create_branch(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def update_branch(
+    def create_branch(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def update_branch(
+    def create_branch(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def update_branch(
+    def create_branch(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def update_branch(
+    def create_branch(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_branch_oapg(
+        return self._create_branch_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpatch(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def patch(
+    def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def patch(
+    def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def patch(
+    def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def patch(
+    def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def patch(
+    def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_branch_oapg(
+        return self._create_branch_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id/post.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idshare_auth_/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,26 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.message_res import MessageRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
-from sedaro_base_client.model.branch_create import BranchCreate
+from sedaro_base_client.model.branch_verify_password import BranchVerifyPassword
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -53,25 +54,25 @@
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
 # body param
-SchemaForRequestBodyApplicationJson = BranchCreate
+SchemaForRequestBodyApplicationJson = BranchVerifyPassword
 
 
-request_body_branch_create = api_client.RequestBody(
+request_body_branch_verify_password = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = MessageRes
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -112,81 +113,81 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_branch_oapg(
+    def _verify_branch_password_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _create_branch_oapg(
+    def _verify_branch_password_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def _create_branch_oapg(
+    def _verify_branch_password_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_branch_oapg(
+    def _verify_branch_password_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_branch_oapg(
+    def _verify_branch_password_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Branch off existing branch
+        Verify branch bassword
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
@@ -210,15 +211,15 @@
                 _headers.add('Accept', accept_content_type)
 
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_branch_create.serialize(body, content_type)
+        serialized_data = request_body_branch_verify_password.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -245,84 +246,84 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateBranch(BaseApi):
+class VerifyBranchPassword(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_branch(
+    def verify_branch_password(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def create_branch(
+    def verify_branch_password(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def create_branch(
+    def verify_branch_password(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_branch(
+    def verify_branch_password(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_branch(
+    def verify_branch_password(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_branch_oapg(
+        return self._verify_branch_password_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
@@ -394,15 +395,15 @@
         content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_branch_oapg(
+        return self._verify_branch_password_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_/post.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/data_id/get.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,72 +21,88 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.data_service_response import DataServiceResponse
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
-DataSchema = schemas.NoneSchema
+StartSchema = schemas.NumberSchema
+StopSchema = schemas.NumberSchema
+BinWidthSchema = schemas.NumberSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'data': typing.Union[DataSchema, None, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'start': typing.Union[StartSchema, decimal.Decimal, int, float, ],
+        'stop': typing.Union[StopSchema, decimal.Decimal, int, float, ],
+        'binWidth': typing.Union[BinWidthSchema, decimal.Decimal, int, float, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_data = api_client.QueryParameter(
-    name="data",
+request_query_start = api_client.QueryParameter(
+    name="start",
     style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
+    schema=StartSchema,
+    explode=True,
+)
+request_query_stop = api_client.QueryParameter(
+    name="stop",
+    style=api_client.ParameterStyle.FORM,
+    schema=StopSchema,
+    explode=True,
+)
+request_query_bin_width = api_client.QueryParameter(
+    name="binWidth",
+    style=api_client.ParameterStyle.FORM,
+    schema=BinWidthSchema,
     explode=True,
 )
 # Path params
-BranchIdSchema = schemas.IntSchema
+IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'id': typing.Union[IdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_branch_id = api_client.PathParameter(
-    name="branchId",
+request_path_id = api_client.PathParameter(
+    name="id",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=BranchIdSchema,
+    schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = DataServiceResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -127,86 +143,88 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_agent_oapg(
+    def _get_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _create_agent_oapg(
+    def _get_data_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_agent_oapg(
+    def _get_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_agent_oapg(
+    def _get_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create Simulated Agent
+        Query Data
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
-            request_path_branch_id,
+            request_path_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_data,
+            request_query_start,
+            request_query_stop,
+            request_query_bin_width,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -217,15 +235,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -242,125 +260,125 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateAgent(BaseApi):
+class GetData(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_agent(
+    def get_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def create_agent(
+    def get_data(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_agent(
+    def get_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_agent(
+    def get_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_agent_oapg(
+        return self._get_data_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpost(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def post(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_agent_oapg(
+        return self._get_data_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/delete.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_job_id/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.message_res import MessageRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
-BlockIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
+JobIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
-        'blockId': typing.Union[BlockIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
+        'jobId': typing.Union[JobIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -53,21 +54,21 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-request_path_block_id = api_client.PathParameter(
-    name="blockId",
+request_path_job_id = api_client.PathParameter(
+    name="jobId",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=BlockIdSchema,
+    schema=JobIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = MessageRes
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -108,69 +109,69 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _delete_agent_oapg(
+    def _terminate_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _delete_agent_oapg(
+    def _terminate_simulation_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _delete_agent_oapg(
+    def _terminate_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _delete_agent_oapg(
+    def _terminate_simulation_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Delete Simulated Agent
+        Terminate a simulation
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
-            request_path_block_id,
+            request_path_job_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -206,61 +207,61 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class DeleteAgent(BaseApi):
+class TerminateSimulation(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def delete_agent(
+    def terminate_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete_agent(
+    def terminate_simulation(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete_agent(
+    def terminate_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete_agent(
+    def terminate_simulation(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_agent_oapg(
+        return self._terminate_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
@@ -307,15 +308,15 @@
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_agent_oapg(
+        return self._terminate_simulation_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_agents_block_id/patch.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,53 +21,26 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.branch_scenario_res import BranchScenarioRes
+from sedaro_base_client.model.branch_vehicle_res import BranchVehicleRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
-# Query params
-DataSchema = schemas.NoneSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-        'data': typing.Union[DataSchema, None, ],
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_data = api_client.QueryParameter(
-    name="data",
-    style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
-    explode=True,
-)
 # Path params
-BranchIdSchema = schemas.IntSchema
-BlockIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
-        'blockId': typing.Union[BlockIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -80,21 +53,51 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-request_path_block_id = api_client.PathParameter(
-    name="blockId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=BlockIdSchema,
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                BranchVehicleRes,
+                BranchScenarioRes,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -135,106 +138,87 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _update_agent_oapg(
+    def _get_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _update_agent_oapg(
+    def _get_branch_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _update_agent_oapg(
+    def _get_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _update_agent_oapg(
+    def _get_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Update Simulated Agent
+        Get a branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
-            request_path_block_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_data,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='patch'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -251,126 +235,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class UpdateAgent(BaseApi):
+class GetBranch(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def update_agent(
+    def get_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def update_agent(
+    def get_branch(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def update_agent(
+    def get_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def update_agent(
+    def get_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_agent_oapg(
-            query_params=query_params,
+        return self._get_branch_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpatch(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def patch(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_agent_oapg(
-            query_params=query_params,
+        return self._get_branch_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_/post.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommits_/post.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,51 +21,52 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.message_res import MessageRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
-DataSchema = schemas.NoneSchema
+CommitMessageSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'data': typing.Union[DataSchema, None, ],
+        'commitMessage': typing.Union[CommitMessageSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_data = api_client.QueryParameter(
-    name="data",
+request_query_commit_message = api_client.QueryParameter(
+    name="commitMessage",
     style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
+    schema=CommitMessageSchema,
     required=True,
     explode=True,
 )
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -78,15 +79,15 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = MessageRes
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -127,62 +128,62 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_celestial_target_oapg(
+    def _commit_to_branch_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _create_celestial_target_oapg(
+    def _commit_to_branch_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_celestial_target_oapg(
+    def _commit_to_branch_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_celestial_target_oapg(
+    def _commit_to_branch_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create Celestial Target
+        Commit changes to a branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -198,15 +199,15 @@
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_data,
+            request_query_commit_message,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -242,65 +243,65 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateCelestialTarget(BaseApi):
+class CommitToBranch(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_celestial_target(
+    def commit_to_branch(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def create_celestial_target(
+    def commit_to_branch(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_celestial_target(
+    def commit_to_branch(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_celestial_target(
+    def commit_to_branch(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_celestial_target_oapg(
+        return self._commit_to_branch_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
@@ -352,15 +353,15 @@
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_celestial_target_oapg(
+        return self._commit_to_branch_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/delete.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idsaved_/get.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
+from sedaro_base_client.model.vehicle_template import VehicleTemplate
+from sedaro_base_client.model.scenario_template import ScenarioTemplate
 
 from . import path
 
 # Path params
-BranchIdSchema = schemas.IntSchema
-BlockIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
-        'blockId': typing.Union[BlockIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -53,21 +53,51 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-request_path_block_id = api_client.PathParameter(
-    name="blockId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=BlockIdSchema,
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                VehicleTemplate,
+                ScenarioTemplate,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -108,69 +138,68 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _delete_celestial_target_oapg(
+    def _get_saved_branch_data_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _delete_celestial_target_oapg(
+    def _get_saved_branch_data_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _delete_celestial_target_oapg(
+    def _get_saved_branch_data_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _delete_celestial_target_oapg(
+    def _get_saved_branch_data_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Delete Celestial Target
+        Get committed branch data
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
-            request_path_block_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -181,15 +210,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='delete'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -206,116 +235,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class DeleteCelestialTarget(BaseApi):
+class GetSavedBranchData(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def delete_celestial_target(
+    def get_saved_branch_data(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete_celestial_target(
+    def get_saved_branch_data(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete_celestial_target(
+    def get_saved_branch_data(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete_celestial_target(
+    def get_saved_branch_data(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_celestial_target_oapg(
+        return self._get_saved_branch_data_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiFordelete(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._delete_celestial_target_oapg(
+        return self._get_saved_branch_data_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_celestial_targets_block_id/patch.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_idcommitted_/get.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,52 +22,25 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
+from sedaro_base_client.model.vehicle_template import VehicleTemplate
+from sedaro_base_client.model.scenario_template import ScenarioTemplate
 
 from . import path
 
-# Query params
-DataSchema = schemas.NoneSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-        'data': typing.Union[DataSchema, None, ],
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_data = api_client.QueryParameter(
-    name="data",
-    style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
-    explode=True,
-)
 # Path params
-BranchIdSchema = schemas.IntSchema
-BlockIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
-        'blockId': typing.Union[BlockIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -80,21 +53,51 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-request_path_block_id = api_client.PathParameter(
-    name="blockId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=BlockIdSchema,
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                VehicleTemplate,
+                ScenarioTemplate,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -135,106 +138,87 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _update_celestial_target_oapg(
+    def _get_committed_branch_data_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _update_celestial_target_oapg(
+    def _get_committed_branch_data_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _update_celestial_target_oapg(
+    def _get_committed_branch_data_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _update_celestial_target_oapg(
+    def _get_committed_branch_data_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Update Celestial Target
+        Get saved branch data
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
-            request_path_block_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_data,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='patch'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -251,126 +235,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class UpdateCelestialTarget(BaseApi):
+class GetCommittedBranchData(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def update_celestial_target(
+    def get_committed_branch_data(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def update_celestial_target(
+    def get_committed_branch_data(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def update_celestial_target(
+    def get_committed_branch_data(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def update_celestial_target(
+    def get_committed_branch_data(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_celestial_target_oapg(
-            query_params=query_params,
+        return self._get_committed_branch_data_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpatch(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def patch(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def patch(
+    def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_celestial_target_oapg(
-            query_params=query_params,
+        return self._get_committed_branch_data_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_conditions_/post.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/simulations_branches_branch_id_control_/get.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,51 +21,66 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.simulation_job import SimulationJob
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
-DataSchema = schemas.NoneSchema
+
+
+class LatestSchema(
+    schemas.EnumBase,
+    schemas.StrSchema
+):
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "": "EMPTY",
+        }
+    
+    @schemas.classproperty
+    def EMPTY(cls):
+        return cls("")
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'data': typing.Union[DataSchema, None, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'latest': typing.Union[LatestSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_data = api_client.QueryParameter(
-    name="data",
+request_query_latest = api_client.QueryParameter(
+    name="latest",
     style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
+    schema=LatestSchema,
     explode=True,
 )
 # Path params
-BranchIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -78,15 +93,77 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        
+        class any_of_0(
+            schemas.ListSchema
+        ):
+        
+        
+            class MetaOapg:
+                
+                @staticmethod
+                def items() -> typing.Type['SimulationJob']:
+                    return SimulationJob
+        
+            def __new__(
+                cls,
+                _arg: typing.Union[typing.Tuple['SimulationJob'], typing.List['SimulationJob']],
+                _configuration: typing.Optional[schemas.Configuration] = None,
+            ) -> 'any_of_0':
+                return super().__new__(
+                    cls,
+                    _arg,
+                    _configuration=_configuration,
+                )
+        
+            def __getitem__(self, i: int) -> 'SimulationJob':
+                return super().__getitem__(i)
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                cls.any_of_0,
+                SimulationJob,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -127,62 +204,62 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_condition_oapg(
+    def _get_simulations_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _create_condition_oapg(
+    def _get_simulations_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_condition_oapg(
+    def _get_simulations_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_condition_oapg(
+    def _get_simulations_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create Condition
+        Get all simulations
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -198,15 +275,15 @@
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_data,
+            request_query_latest,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -217,15 +294,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='get'.upper(),
             headers=_headers,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -242,125 +319,125 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateCondition(BaseApi):
+class GetSimulations(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_condition(
+    def get_simulations(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def create_condition(
+    def get_simulations(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_condition(
+    def get_simulations(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_condition(
+    def get_simulations(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_condition_oapg(
+        return self._get_simulations_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpost(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def post(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def post(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_condition_oapg(
+        return self._get_simulations_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_/post.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_current_branch_id_merge_incoming_branch_id/post.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,72 +21,105 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.branch_scenario_res import BranchScenarioRes
+from sedaro_base_client.model.branch_merge import BranchMerge
+from sedaro_base_client.model.branch_vehicle_res import BranchVehicleRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
+from sedaro_base_client.model.branch_merge_conflicts_res import BranchMergeConflictsRes
 
 from . import path
 
-# Query params
-DataSchema = schemas.NoneSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-        'data': typing.Union[DataSchema, None, ],
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_data = api_client.QueryParameter(
-    name="data",
-    style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
-    explode=True,
-)
 # Path params
-BranchIdSchema = schemas.IntSchema
+CurrentBranchIdSchema = schemas.StrSchema
+IncomingBranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
+        'currentBranchId': typing.Union[CurrentBranchIdSchema, str, ],
+        'incomingBranchId': typing.Union[IncomingBranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_branch_id = api_client.PathParameter(
-    name="branchId",
+request_path_current_branch_id = api_client.PathParameter(
+    name="currentBranchId",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=BranchIdSchema,
+    schema=CurrentBranchIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+request_path_incoming_branch_id = api_client.PathParameter(
+    name="incomingBranchId",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=IncomingBranchIdSchema,
+    required=True,
+)
+# body param
+SchemaForRequestBodyApplicationJson = BranchMerge
+
+
+request_body_branch_merge = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
+)
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                BranchVehicleRes,
+                BranchScenarioRes,
+                BranchMergeConflictsRes,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -127,106 +160,125 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_ground_target_oapg(
+    def _merge_branches_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _create_ground_target_oapg(
+    def _merge_branches_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def _merge_branches_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_ground_target_oapg(
+    def _merge_branches_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_ground_target_oapg(
+    def _merge_branches_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create Ground Target
+        Merge branch into another branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
-            request_path_branch_id,
+            request_path_current_branch_id,
+            request_path_incoming_branch_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_data,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_branch_merge.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
+            fields=_fields,
+            body=_body,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
@@ -242,127 +294,167 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateGroundTarget(BaseApi):
+class MergeBranches(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_ground_target(
+    def merge_branches(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def merge_branches(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def create_ground_target(
+    def merge_branches(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_ground_target(
+    def merge_branches(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_ground_target(
+    def merge_branches(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_ground_target_oapg(
-            query_params=query_params,
+        return self._merge_branches_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
     def post(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
     def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_ground_target_oapg(
-            query_params=query_params,
+        return self._merge_branches_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/paths/models_branches_branch_id_cdh_conops_ground_targets_block_id/patch.py` & `sedaro-4.0.0/src/sedaro_base_client/paths/models_branches_branch_id/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,53 +21,27 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from sedaro_base_client import schemas  # noqa: F401
 
+from sedaro_base_client.model.branch_scenario_res import BranchScenarioRes
+from sedaro_base_client.model.branch_update import BranchUpdate
+from sedaro_base_client.model.branch_vehicle_res import BranchVehicleRes
 from sedaro_base_client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
-# Query params
-DataSchema = schemas.NoneSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-        'data': typing.Union[DataSchema, None, ],
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_data = api_client.QueryParameter(
-    name="data",
-    style=api_client.ParameterStyle.FORM,
-    schema=DataSchema,
-    required=True,
-    explode=True,
-)
 # Path params
-BranchIdSchema = schemas.IntSchema
-BlockIdSchema = schemas.IntSchema
+BranchIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'branchId': typing.Union[BranchIdSchema, decimal.Decimal, int, ],
-        'blockId': typing.Union[BlockIdSchema, decimal.Decimal, int, ],
+        'branchId': typing.Union[BranchIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -80,21 +54,62 @@
 
 request_path_branch_id = api_client.PathParameter(
     name="branchId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=BranchIdSchema,
     required=True,
 )
-request_path_block_id = api_client.PathParameter(
-    name="blockId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=BlockIdSchema,
+# body param
+SchemaForRequestBodyApplicationJson = BranchUpdate
+
+
+request_body_branch_update = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+
+
+    class MetaOapg:
+        
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                BranchVehicleRes,
+                BranchScenarioRes,
+            ]
+
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -135,107 +150,124 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _update_ground_target_oapg(
+    def _update_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _update_ground_target_oapg(
+    def _update_branch_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def _update_branch_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _update_ground_target_oapg(
+    def _update_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _update_ground_target_oapg(
+    def _update_branch_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Update Ground Target
+        Update a branch
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_branch_id,
-            request_path_block_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_data,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_branch_update.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
             method='patch'.upper(),
             headers=_headers,
+            fields=_fields,
+            body=_body,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
@@ -251,127 +283,167 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class UpdateGroundTarget(BaseApi):
+class UpdateBranch(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def update_ground_target(
+    def update_branch(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def update_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def update_ground_target(
+    def update_branch(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def update_ground_target(
+    def update_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def update_ground_target(
+    def update_branch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_ground_target_oapg(
-            query_params=query_params,
+        return self._update_branch_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
 class ApiForpatch(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def patch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def patch(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
     def patch(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def patch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
     def patch(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._update_ground_target_oapg(
-            query_params=query_params,
+        return self._update_branch_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/rest.py` & `sedaro-4.0.0/src/sedaro_base_client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 import logging
 import ssl
 from urllib.parse import urlencode
 import typing
```

### Comparing `sedaro-3.5.7/src/sedaro_base_client/schemas.py` & `sedaro-4.0.0/src/sedaro_base_client/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Sedaro Satellite API
 
-     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the  Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests  via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised,  you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
+     Allows for consumption of Sedaro Satellite services. Read more about Sedaro Satellite at [docs.sedaro.com](https://docs.sedaro.com).  ### Clients  **Python:** [sedaro](https://pypi.org/project/sedaro/) - This package provides additional functionality on top of the auto-generated OpenAPI client. See the package docs for more information.  ### API Key  To access the Sedaro service via this API, you will need an API key.  You can generate an API key for your account in the Sedaro [Management Console](https://satellite.sedaro.com/#/account). Once complete, pass the API key in all requests via the `X_API_KEY` HTTP header.  *API keys grant full access to your account and should never be shared. If you think your API key has been compromised, you can revoke it in the [Management Console](https://satellite.sedaro.com/#/account).*  ### Jupyter Notebooks  For additional examples of how to use this API for modeling and simulation, see our [Mod-Sim Notebooks](https://github.com/sedaro/modsim-notebooks).  ### Community, Support, Discussion  If you have any issues or suggestions, please reach out:  1. Join the Sedaro Community [Slack](https://join.slack.com/t/sedaro-community/shared_invite/zt-1jps4i711-mXy88AZQ9AV7YcEXr8x7Ow) 2. Email us at support@sedarotech.com  ### Known Issues  - Currently the documentation for 200 responses to Block create, read, update, and delete (CRUD) operations is incorrect. This is due to an issue with our documentation generator.  Under each Block Group, the documentation will show `name`, `collection`, and `data` keys.  In reality, this level does not exist and should be skipped.  See the schema under the `data` key of a Template's Block Group for the correct schema of such Block Group. - Error responses are more specific than what is shown throughout the documentation.  A 4xx or 5xx error will be returned in all error cases.  Only a `200` status indicates success.  See a given error response for additional details.   # noqa: E501
 
-    The version of the OpenAPI document: 3.5.7
+    The version of the OpenAPI document: 3.3.7
     Generated by: https://openapi-generator.tech
 """
 
 from collections import defaultdict
 from datetime import date, datetime, timedelta  # noqa: F401
 import functools
 import decimal
```

