# Comparing `tmp/csle_common-0.1.8.tar.gz` & `tmp/csle_common-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_common-0.1.8.tar", last modified: Mon Mar 20 15:26:54 2023, max compression
+gzip compressed data, was "csle_common-0.1.9.tar", last modified: Tue Mar 21 08:09:18 2023, max compression
```

## Comparing `csle_common-0.1.8.tar` & `csle_common-0.1.9.tar`

### file list

```diff
@@ -1,288 +1,288 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.147126 csle_common-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      685 2023-03-20 15:26:54.147281 csle_common-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      671 2023-02-12 08:59:32.000000 csle_common-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1476 2023-03-20 15:26:54.148306 csle_common-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_common-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.954828 csle_common-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.964308 csle_common-0.1.8/src/csle_common/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_common-0.1.8/src/csle_common/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.968607 csle_common-0.1.8/src/csle_common/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    66631 2023-03-20 14:34:43.000000 csle_common-0.1.8/src/csle_common/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.975850 csle_common-0.1.8/src/csle_common/consumer_threads/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4795 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2417 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2807 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/avg_host_metrics_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     3905 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/client_population_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2494 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2444 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     4779 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2390 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     3144 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     3197 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.992493 csle_common-0.1.8/src/csle_common/controllers/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/controllers/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    36830 2023-03-20 13:55:38.000000 csle_common-0.1.8/src/csle_common/controllers/container_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    17616 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/controllers/elk_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    47786 2023-03-20 15:01:14.000000 csle_common-0.1.8/src/csle_common/controllers/emulation_env_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)     2255 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/controllers/flags_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    67002 2023-03-16 12:53:21.000000 csle_common-0.1.8/src/csle_common/controllers/host_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    11832 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/controllers/installation_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    14738 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/controllers/kafka_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    19115 2023-02-17 08:02:19.000000 csle_common-0.1.8/src/csle_common/controllers/management_system_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    20424 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/controllers/ossec_ids_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)     5111 2023-03-20 14:23:31.000000 csle_common-0.1.8/src/csle_common/controllers/ovs_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)     3974 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/controllers/resource_constraints_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    14803 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/controllers/sdn_controller_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     1214 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/controllers/simulation_env_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    20361 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/controllers/snort_ids_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    11073 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/controllers/topology_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)    34689 2023-03-20 15:19:09.000000 csle_common-0.1.8/src/csle_common/controllers/traffic_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)     3839 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/controllers/users_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)     2884 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/controllers/vulnerabilities_controller.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.993213 csle_common-0.1.8/src/csle_common/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.994179 csle_common-0.1.8/src/csle_common/dao/datasets/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/datasets/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5914 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/datasets/statistics_dataset.py
--rw-r--r--   0 kimham     (501) staff       (20)     5674 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/datasets/traces_dataset.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.995610 csle_common-0.1.8/src/csle_common/dao/docker/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/docker/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6387 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/docker/docker_container_metadata.py
--rw-r--r--   0 kimham     (501) staff       (20)     3595 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/docker/docker_env_metadata.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.997952 csle_common-0.1.8/src/csle_common/dao/domain_randomization/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/domain_randomization/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2141 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/domain_randomization/node_randomizer_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      556 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/domain_randomization/randomization_space.py
--rw-r--r--   0 kimham     (501) staff       (20)     2900 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/domain_randomization/randomization_space_config.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.998714 csle_common-0.1.8/src/csle_common/dao/emulation_action/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.008632 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    11189 2023-03-16 08:30:07.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
--rw-r--r--   0 kimham     (501) staff       (20)    19979 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2172 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
--rw-r--r--   0 kimham     (501) staff       (20)      362 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
--rw-r--r--   0 kimham     (501) staff       (20)      295 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     1728 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
--rw-r--r--   0 kimham     (501) staff       (20)     1517 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
--rw-r--r--   0 kimham     (501) staff       (20)     1551 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
--rw-r--r--   0 kimham     (501) staff       (20)    29225 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
--rw-r--r--   0 kimham     (501) staff       (20)    12817 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
--rw-r--r--   0 kimham     (501) staff       (20)     2091 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.014542 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6875 2023-03-16 08:29:37.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
--rw-r--r--   0 kimham     (501) staff       (20)     4050 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      221 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
--rw-r--r--   0 kimham     (501) staff       (20)      286 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
--rw-r--r--   0 kimham     (501) staff       (20)      247 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     4705 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.026039 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      953 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
--rw-r--r--   0 kimham     (501) staff       (20)     1997 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nikto_vuln.py
--rw-r--r--   0 kimham     (501) staff       (20)      192 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     1938 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
--rw-r--r--   0 kimham     (501) staff       (20)     2523 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_hop.py
--rw-r--r--   0 kimham     (501) staff       (20)     3104 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_host_result.py
--rw-r--r--   0 kimham     (501) staff       (20)      199 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_host_status.py
--rw-r--r--   0 kimham     (501) staff       (20)      395 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
--rw-r--r--   0 kimham     (501) staff       (20)      411 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
--rw-r--r--   0 kimham     (501) staff       (20)     1174 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_os.py
--rw-r--r--   0 kimham     (501) staff       (20)     3715 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_port.py
--rw-r--r--   0 kimham     (501) staff       (20)      199 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_port_status.py
--rw-r--r--   0 kimham     (501) staff       (20)     1007 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
--rw-r--r--   0 kimham     (501) staff       (20)     2326 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_trace.py
--rw-r--r--   0 kimham     (501) staff       (20)     2546 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_vuln.py
--rw-r--r--   0 kimham     (501) staff       (20)      400 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.080838 csle_common-0.1.8/src/csle_common/dao/emulation_config/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4068 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/beats_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3182 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/client_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     8530 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/client_population_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      299 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/client_population_process_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     2576 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/cluster_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2926 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/cluster_node.py
--rw-r--r--   0 kimham     (501) staff       (20)    37157 2023-03-05 07:34:13.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4143 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/connection_setup_dto.py
--rw-r--r--   0 kimham     (501) staff       (20)     4084 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/container_network.py
--rw-r--r--   0 kimham     (501) staff       (20)     7691 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/containers_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4325 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/credential.py
--rw-r--r--   0 kimham     (501) staff       (20)     4829 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/default_network_firewall_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5296 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3418 2023-02-12 12:41:34.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     7236 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/elk_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3370 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/elk_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)    21787 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     7640 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     7410 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_state.py
--rw-r--r--   0 kimham     (501) staff       (20)     2392 2023-02-17 16:35:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_execution.py
--rw-r--r--   0 kimham     (501) staff       (20)     7851 2022-12-07 09:01:16.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_execution_info.py
--rw-r--r--   0 kimham     (501) staff       (20)    15758 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
--rw-r--r--   0 kimham     (501) staff       (20)     2768 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
--rw-r--r--   0 kimham     (501) staff       (20)     3406 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
--rw-r--r--   0 kimham     (501) staff       (20)    42526 2022-11-29 07:04:09.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_trace.py
--rw-r--r--   0 kimham     (501) staff       (20)     3693 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/flag.py
--rw-r--r--   0 kimham     (501) staff       (20)     3446 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/flags_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4658 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/host_manager_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3103 2022-11-29 17:55:52.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/host_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     7618 2023-03-16 10:11:01.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3108 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     3550 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_topic.py
--rw-r--r--   0 kimham     (501) staff       (20)     5079 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/network_service.py
--rw-r--r--   0 kimham     (501) staff       (20)     6950 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_beats_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     7334 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_container_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     8429 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_firewall_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3630 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_flags_config.py
--rw-r--r--   0 kimham     (501) staff       (20)    15661 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_network_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5446 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_resources_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3052 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_services_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5232 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_traffic_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3633 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_users_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5560 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/node_vulnerability_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5008 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3328 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/ossec_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     2901 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/ovs_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5217 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/ovs_switch_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      316 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
--rw-r--r--   0 kimham     (501) staff       (20)      269 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/packet_loss_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     3214 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/resources_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3502 2022-12-07 08:57:28.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/ryu_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)     7312 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/sdn_controller_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      205 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/sdn_controller_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     3562 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/services_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4910 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3618 2023-03-16 16:23:09.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/snort_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)      254 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     3503 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/topology_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4287 2023-03-02 15:35:33.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/traffic_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3216 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/traffic_managers_info.py
--rw-r--r--   0 kimham     (501) staff       (20)      782 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/transport_protocol.py
--rw-r--r--   0 kimham     (501) staff       (20)     2435 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/user.py
--rw-r--r--   0 kimham     (501) staff       (20)     3431 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/users_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3787 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/vulnerabilities_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      302 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_config/vulnerability_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.081414 csle_common-0.1.8/src/csle_common/dao/emulation_observation/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/__init__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.085227 csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    20554 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
--rw-r--r--   0 kimham     (501) staff       (20)    10470 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.087566 csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6143 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
--rw-r--r--   0 kimham     (501) staff       (20)     6055 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
--rw-r--r--   0 kimham     (501) staff       (20)     6278 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.089371 csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     8885 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
--rw-r--r--   0 kimham     (501) staff       (20)    19601 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.090488 csle_common-0.1.8/src/csle_common/dao/encoding/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/encoding/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      411 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/encoding/np_encoder.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.092745 csle_common-0.1.8/src/csle_common/dao/jobs/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/jobs/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     7084 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/jobs/data_collection_job_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4534 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/jobs/system_identification_job_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5495 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/jobs/training_job_config.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.094353 csle_common-0.1.8/src/csle_common/dao/management/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/management/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3542 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/management/management_user.py
--rw-r--r--   0 kimham     (501) staff       (20)     2775 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/management/session_token.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.110715 csle_common-0.1.8/src/csle_common/dao/simulation_config/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     1073 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/action.py
--rw-r--r--   0 kimham     (501) staff       (20)     2022 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/action_space_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      483 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/agent_log.py
--rw-r--r--   0 kimham     (501) staff       (20)      734 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/base_env.py
--rw-r--r--   0 kimham     (501) staff       (20)     1228 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/env_parameter.py
--rw-r--r--   0 kimham     (501) staff       (20)     1216 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/env_parameters_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1312 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1302 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/joint_action_space_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1163 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/joint_observation_space_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1242 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/observation.py
--rw-r--r--   0 kimham     (501) staff       (20)     1505 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/observation_function_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5039 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/observation_space_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1226 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/player_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1271 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/players_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1047 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/reward_function_config.py
--rw-r--r--   0 kimham     (501) staff       (20)    11210 2023-03-08 07:57:44.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/simulation_env_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      337 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/simulation_env_input_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5489 2023-03-01 10:57:15.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/simulation_trace.py
--rw-r--r--   0 kimham     (501) staff       (20)     1451 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/state.py
--rw-r--r--   0 kimham     (501) staff       (20)     1274 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/state_space_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      157 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/state_type.py
--rw-r--r--   0 kimham     (501) staff       (20)      166 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/time_step_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     1121 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/transition_operator_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      159 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/simulation_config/value_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.116879 csle_common-0.1.8/src/csle_common/dao/system_identification/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2998 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/empirical_conditional.py
--rw-r--r--   0 kimham     (501) staff       (20)     6116 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/empirical_system_model.py
--rw-r--r--   0 kimham     (501) staff       (20)    23200 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/emulation_statistics.py
--rw-r--r--   0 kimham     (501) staff       (20)     7292 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
--rw-r--r--   0 kimham     (501) staff       (20)     6623 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
--rw-r--r--   0 kimham     (501) staff       (20)     5215 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/gp_conditional.py
--rw-r--r--   0 kimham     (501) staff       (20)     6461 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/gp_system_model.py
--rw-r--r--   0 kimham     (501) staff       (20)     3260 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/system_identification_config.py
--rw-r--r--   0 kimham     (501) staff       (20)      768 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/system_model.py
--rw-r--r--   0 kimham     (501) staff       (20)      219 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/system_identification/system_model_type.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.126967 csle_common-0.1.8/src/csle_common/dao/training/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/training/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      633 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/training/agent_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     6605 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/alpha_vectors_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     7357 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/dqn_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     4362 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/experiment_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3648 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/experiment_execution.py
--rw-r--r--   0 kimham     (501) staff       (20)     3222 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/experiment_result.py
--rw-r--r--   0 kimham     (501) staff       (20)    11482 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/fnn_with_softmax_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     1959 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/hparam.py
--rw-r--r--   0 kimham     (501) staff       (20)    14043 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)    13851 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/multi_threshold_stopping_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)      179 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/training/player_type.py
--rw-r--r--   0 kimham     (501) staff       (20)      963 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/dao/training/policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     7424 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/ppo_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     4560 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/random_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     5276 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/tabular_policy.py
--rw-r--r--   0 kimham     (501) staff       (20)     4634 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/dao/training/vector_policy.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.128822 csle_common-0.1.8/src/csle_common/logging/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/logging/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      624 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/logging/custom_formatter.py
--rw-r--r--   0 kimham     (501) staff       (20)     2646 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/logging/log.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.129858 csle_common-0.1.8/src/csle_common/metastore/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/metastore/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)   219637 2023-03-01 07:00:43.000000 csle_common-0.1.8/src/csle_common/metastore/metastore_facade.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.132633 csle_common-0.1.8/src/csle_common/models/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-12-13 08:21:49.000000 csle_common-0.1.8/src/csle_common/models/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     4091 2022-12-13 08:21:49.000000 csle_common-0.1.8/src/csle_common/models/fnn_w_softmax.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.135419 csle_common-0.1.8/src/csle_common/tunneling/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/tunneling/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2325 2022-12-07 07:23:42.000000 csle_common-0.1.8/src/csle_common/tunneling/forward_ssh_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)      280 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/tunneling/forward_ssh_server.py
--rw-r--r--   0 kimham     (501) staff       (20)     1620 2022-12-07 07:23:42.000000 csle_common-0.1.8/src/csle_common/tunneling/forward_tunnel_thread.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:54.146594 csle_common-0.1.8/src/csle_common/util/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6225 2023-02-17 08:04:16.000000 csle_common-0.1.8/src/csle_common/util/cluster_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    35781 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/connection_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     8718 2023-03-20 10:38:35.000000 csle_common-0.1.8/src/csle_common/util/docker_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    21262 2023-03-05 07:26:30.000000 csle_common-0.1.8/src/csle_common/util/emulation_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    37527 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/env_dynamics_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    16211 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/experiment_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    19037 2022-11-29 07:04:09.000000 csle_common-0.1.8/src/csle_common/util/export_util.py
--rw-r--r--   0 kimham     (501) staff       (20)      809 2023-02-12 08:59:32.000000 csle_common-0.1.8/src/csle_common/util/general_util.py
--rw-r--r--   0 kimham     (501) staff       (20)      533 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/grpc_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     2514 2022-12-28 18:49:38.000000 csle_common-0.1.8/src/csle_common/util/import_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3542 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/management_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     2165 2023-03-16 16:22:51.000000 csle_common-0.1.8/src/csle_common/util/plotting_util.py
--rw-r--r--   0 kimham     (501) staff       (20)    17318 2023-03-16 16:22:45.000000 csle_common-0.1.8/src/csle_common/util/read_emulation_statistics_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     2512 2022-11-28 13:00:49.000000 csle_common-0.1.8/src/csle_common/util/ssh_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:53.967430 csle_common-0.1.8/src/csle_common.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      685 2023-03-20 15:26:53.000000 csle_common-0.1.8/src/csle_common.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)    14558 2023-03-20 15:26:53.000000 csle_common-0.1.8/src/csle_common.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:26:53.000000 csle_common-0.1.8/src/csle_common.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:23.000000 csle_common-0.1.8/src/csle_common.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      399 2023-03-20 15:26:53.000000 csle_common-0.1.8/src/csle_common.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       12 2023-03-20 15:26:53.000000 csle_common-0.1.8/src/csle_common.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.013213 csle_common-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-03-21 08:09:18.013213 csle_common-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      671 2023-02-11 20:28:41.000000 csle_common-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1476 2023-03-21 08:09:18.013213 csle_common-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_common-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.965213 csle_common-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_common-0.1.9/src/csle_common/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    66639 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common/consumer_threads/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4795 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2417 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2807 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/avg_host_metrics_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3905 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/client_population_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2494 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/defender_actions_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2444 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4779 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/docker_stats_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2390 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/host_metrics_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3144 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3197 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/controllers/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37233 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/container_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17707 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/elk_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    47786 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/emulation_env_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2255 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/controllers/flags_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    68167 2023-03-21 08:07:44.000000 csle_common-0.1.9/src/csle_common/controllers/host_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11832 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/installation_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14738 2023-03-04 20:08:15.000000 csle_common-0.1.9/src/csle_common/controllers/kafka_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19115 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/controllers/management_system_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20424 2023-03-04 15:16:49.000000 csle_common-0.1.9/src/csle_common/controllers/ossec_ids_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5548 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/ovs_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3974 2023-02-28 07:45:45.000000 csle_common-0.1.9/src/csle_common/controllers/resource_constraints_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14905 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/sdn_controller_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1214 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/controllers/simulation_env_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20361 2023-03-04 09:58:52.000000 csle_common-0.1.9/src/csle_common/controllers/snort_ids_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11073 2023-02-28 07:45:56.000000 csle_common-0.1.9/src/csle_common/controllers/topology_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34689 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/controllers/traffic_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3839 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/controllers/users_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2884 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/controllers/vulnerabilities_controller.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/datasets/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/datasets/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5914 2023-02-28 07:13:58.000000 csle_common-0.1.9/src/csle_common/dao/datasets/statistics_dataset.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5674 2023-02-28 07:14:17.000000 csle_common-0.1.9/src/csle_common/dao/datasets/traces_dataset.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/docker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/docker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6387 2023-02-28 07:15:04.000000 csle_common-0.1.9/src/csle_common/dao/docker/docker_container_metadata.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3595 2023-02-28 07:15:20.000000 csle_common-0.1.9/src/csle_common/dao/docker/docker_env_metadata.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/domain_randomization/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2141 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/node_randomizer_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      556 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2900 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.973213 csle_common-0.1.9/src/csle_common/dao/emulation_action/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.977213 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11189 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19979 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2172 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      362 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_outcome.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      295 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1728 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1517 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1551 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29225 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12817 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2091 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.977213 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6875 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4050 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      221 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_id.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      286 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_outcome.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      247 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4705 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.981213 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      953 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_scan_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1997 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_vuln.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      192 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_addr_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1938 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2523 2023-02-28 07:16:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_hop.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3104 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      199 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_status.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      395 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_http_enum.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      411 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_http_grep.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1174 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_os.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3715 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      199 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port_status.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_scan_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2326 2023-02-28 07:16:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2546 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vuln.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      400 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vulscan.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_config/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4068 2023-02-28 07:16:52.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/beats_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3182 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8530 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      299 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_process_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2576 2023-02-28 07:17:28.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2926 2023-02-28 07:17:43.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_node.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37157 2023-03-06 06:25:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4143 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/connection_setup_dto.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4084 2023-02-28 07:18:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/container_network.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7691 2023-03-04 17:24:13.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/containers_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4325 2023-02-28 07:19:02.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/credential.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4829 2023-02-28 07:19:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/default_network_firewall_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5296 2023-02-28 07:19:34.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3418 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7236 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3730 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21892 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7640 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_generation_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7410 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2392 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7851 2023-03-04 09:29:52.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15758 2023-02-28 07:20:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2768 2023-02-28 07:20:35.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_simulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3406 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    42526 2022-11-28 17:19:23.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3693 2023-02-28 07:21:01.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/flag.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3446 2023-02-28 07:21:17.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/flags_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4658 2023-02-28 07:21:32.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/host_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3103 2022-12-01 06:44:23.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/host_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7618 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3108 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3550 2023-02-28 07:21:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_topic.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5079 2023-02-28 07:22:17.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/network_service.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6950 2023-02-28 07:22:32.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_beats_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7334 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_container_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8429 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_firewall_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3630 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_flags_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15661 2023-02-28 07:24:01.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_network_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5446 2023-02-28 07:41:48.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_resources_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3052 2023-02-28 07:24:34.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_services_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5232 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_traffic_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_users_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5560 2023-02-28 07:45:02.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/node_vulnerability_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5008 2023-02-28 07:25:33.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3328 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3057 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5399 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_switch_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      316 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/packet_delay_distribution_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      269 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/packet_loss_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3214 2023-02-28 07:26:29.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/resources_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3888 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/ryu_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7312 2023-02-28 07:44:20.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      205 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3562 2023-02-28 07:27:00.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/services_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4910 2023-02-28 07:27:15.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_ids_manager_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3618 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      254 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/static_emulation_attacker_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3503 2023-02-28 07:27:24.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/topology_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4287 2023-03-03 06:17:37.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3216 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_managers_info.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      782 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/transport_protocol.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2435 2023-02-28 07:27:57.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/user.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3431 2023-02-28 07:28:10.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/users_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3787 2023-02-28 07:28:25.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerabilities_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      302 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerability_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/__init__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20554 2023-02-28 07:28:42.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10470 2023-02-28 07:12:35.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6143 2023-02-28 07:09:18.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6055 2023-02-28 07:10:13.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6278 2023-02-28 07:09:55.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.993213 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8885 2023-02-28 07:14:44.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19601 2023-02-28 07:29:48.000000 csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/encoding/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/encoding/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      411 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/encoding/np_encoder.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/jobs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/jobs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7084 2023-02-28 07:30:15.000000 csle_common-0.1.9/src/csle_common/dao/jobs/data_collection_job_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4534 2023-02-28 07:30:39.000000 csle_common-0.1.9/src/csle_common/dao/jobs/system_identification_job_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5495 2023-02-28 07:30:52.000000 csle_common-0.1.9/src/csle_common/dao/jobs/training_job_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.997213 csle_common-0.1.9/src/csle_common/dao/management/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/management/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2023-02-28 07:31:05.000000 csle_common-0.1.9/src/csle_common/dao/management/management_user.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2775 2023-02-28 07:31:19.000000 csle_common-0.1.9/src/csle_common/dao/management/session_token.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.001213 csle_common-0.1.9/src/csle_common/dao/simulation_config/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1073 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/action.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2022 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/action_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      483 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/agent_log.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      734 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/base_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1228 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameter.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1216 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameters_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1312 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/initial_state_distribution_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1302 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_action_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1163 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_observation_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1242 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1505 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_function_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5039 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1226 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/player_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1271 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/players_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1047 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/reward_function_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11210 2023-03-07 11:00:13.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      337 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_input_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5489 2023-03-03 06:17:37.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_trace.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1451 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1274 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state_space_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      157 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/state_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      166 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/time_step_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1121 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/transition_operator_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      159 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/simulation_config/value_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.001213 csle_common-0.1.9/src/csle_common/dao/system_identification/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2998 2023-02-28 07:31:32.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6116 2023-02-28 07:31:49.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    23200 2023-02-28 07:08:10.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/emulation_statistics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7292 2023-02-28 07:32:31.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6623 2023-02-28 07:32:47.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5215 2023-02-28 07:34:58.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gp_conditional.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6461 2023-02-28 07:35:13.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/gp_system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3260 2023-02-28 07:35:27.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_identification_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      768 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_model.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      219 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/system_identification/system_model_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/dao/training/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      633 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/agent_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6605 2023-02-28 07:35:45.000000 csle_common-0.1.9/src/csle_common/dao/training/alpha_vectors_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7357 2023-02-28 07:35:58.000000 csle_common-0.1.9/src/csle_common/dao/training/dqn_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4362 2023-02-28 07:36:11.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3648 2023-02-28 07:36:25.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_execution.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3222 2023-02-28 07:36:36.000000 csle_common-0.1.9/src/csle_common/dao/training/experiment_result.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11482 2023-02-28 07:36:57.000000 csle_common-0.1.9/src/csle_common/dao/training/fnn_with_softmax_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1959 2023-02-28 07:37:16.000000 csle_common-0.1.9/src/csle_common/dao/training/hparam.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14043 2023-02-28 07:37:33.000000 csle_common-0.1.9/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13851 2023-02-28 07:37:45.000000 csle_common-0.1.9/src/csle_common/dao/training/multi_threshold_stopping_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      179 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/player_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      963 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/dao/training/policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7424 2023-02-28 07:38:05.000000 csle_common-0.1.9/src/csle_common/dao/training/ppo_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4560 2023-02-28 07:38:20.000000 csle_common-0.1.9/src/csle_common/dao/training/random_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5276 2023-02-28 07:38:35.000000 csle_common-0.1.9/src/csle_common/dao/training/tabular_policy.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4634 2023-02-28 07:38:49.000000 csle_common-0.1.9/src/csle_common/dao/training/vector_policy.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/logging/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      624 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/custom_formatter.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2646 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/logging/log.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.005213 csle_common-0.1.9/src/csle_common/metastore/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/metastore/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   219637 2023-02-28 07:42:55.000000 csle_common-0.1.9/src/csle_common/metastore/metastore_facade.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.009213 csle_common-0.1.9/src/csle_common/models/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-12-11 08:33:52.000000 csle_common-0.1.9/src/csle_common/models/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4091 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/models/fnn_w_softmax.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.009213 csle_common-0.1.9/src/csle_common/tunneling/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/tunneling/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2325 2022-12-03 10:35:18.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      280 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1620 2022-12-03 09:27:05.000000 csle_common-0.1.9/src/csle_common/tunneling/forward_tunnel_thread.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:18.013213 csle_common-0.1.9/src/csle_common/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6225 2023-02-28 07:08:18.000000 csle_common-0.1.9/src/csle_common/util/cluster_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    35781 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/connection_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8718 2023-03-21 06:33:58.000000 csle_common-0.1.9/src/csle_common/util/docker_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    21262 2023-03-03 12:17:05.000000 csle_common-0.1.9/src/csle_common/util/emulation_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    37527 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/env_dynamics_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16211 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/experiment_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    19037 2022-11-28 17:13:00.000000 csle_common-0.1.9/src/csle_common/util/export_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      809 2023-02-11 17:47:01.000000 csle_common-0.1.9/src/csle_common/util/general_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      533 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/grpc_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2514 2022-12-24 11:45:22.000000 csle_common-0.1.9/src/csle_common/util/import_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3542 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/management_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2165 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/util/plotting_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17318 2023-03-17 07:49:22.000000 csle_common-0.1.9/src/csle_common/util/read_emulation_statistics_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2512 2022-11-28 13:03:16.000000 csle_common-0.1.9/src/csle_common/util/ssh_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:17.969213 csle_common-0.1.9/src/csle_common.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      685 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14558 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:28:51.000000 csle_common-0.1.9/src/csle_common.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      399 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       12 2023-03-21 08:09:17.000000 csle_common-0.1.9/src/csle_common.egg-info/top_level.txt
```

### Comparing `csle_common-0.1.8/PKG-INFO` & `csle_common-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_common
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.1.8/pyproject.toml` & `csle_common-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/setup.cfg` & `csle_common-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	random_username>=1.0.2
 	psycopg>=3.1.4
 	click>=8.1.3
 	flask>=2.2.2
 	waitress>=2.1.2
 	psutil>=5.9.4
 	csle_collector>=0.1.5
-	csle-ryu>=0.1.8
+	csle-ryu>=0.1.9
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_common-0.1.8/src/csle_common/constants/constants.py` & `csle_common-0.1.9/src/csle_common/constants/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
 class SSH:
     """
     Constants related to the SSH service
     """
     SERVICE_NAME = "ssh"
     DEFAULT_PORT = 22
     DIRECT_CHANNEL = "direct-tcpip"
-    MAX_FILE_READ_BYTES = 5
+    MAX_FILE_READ_BYTES = 500000000
 
 
 class TELNET:
     """
     Constants related to the Telnet service
     """
     PROMPT = b':~$'
```

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/aggregated_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/attacker_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/avg_host_metrics_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/avg_host_metrics_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/client_population_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/client_population_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/defender_actions_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/defender_actions_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/docker_host_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/docker_stats_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/docker_stats_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/host_metrics_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/host_metrics_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/ossec_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py` & `csle_common-0.1.9/src/csle_common/consumer_threads/snort_ids_log_consumer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/container_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/container_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,15 @@
             cmd = f"docker network disconnect none {container_name}"
             subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
 
             # Wait a few seconds before connecting
             time.sleep(2)
 
             for ip_net in c.ips_and_networks:
+                time.sleep(2)
                 ip, net = ip_net
                 cmd = f"{constants.DOCKER.NETWORK_CONNECT} --ip {ip} {net.name} " \
                       f"{container_name}"
                 logger.info(f"Connecting container:{container_name} to network:{net.name} with ip: {ip}, cmd: {cmd}")
                 subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
 
                 if c.docker_gw_bridge_ip == "" or c.docker_gw_bridge_ip is None:
@@ -409,16 +410,21 @@
             ContainerController.connect_container_to_network(container=emulation_env_config.kafka_config.container,
                                                              logger=logger)
         if emulation_env_config.elk_config.container.physical_host_ip == physical_server_ip:
             ContainerController.connect_container_to_network(container=emulation_env_config.elk_config.container,
                                                              logger=logger)
         if emulation_env_config.sdn_controller_config is not None and \
                 emulation_env_config.sdn_controller_config.container.physical_host_ip == physical_server_ip:
+            # Connect controller
             ContainerController.connect_container_to_network(
                 container=emulation_env_config.sdn_controller_config.container, logger=logger)
+            # Update IPs of OVS switches
+            for ovs_sw in emulation_env_config.ovs_config.switch_configs:
+                node_container_config = emulation_env_config.containers_config.get_container_from_ip(ovs_sw.ip)
+                ovs_sw.docker_gw_bridge_ip = node_container_config.docker_gw_bridge_ip
 
     @staticmethod
     def connect_container_to_network(container: NodeContainerConfig, logger: logging.Logger) -> None:
         """
         Connect a running container to networks
 
         :param container: the container to connect
@@ -430,14 +436,15 @@
         cmd = f"docker network disconnect none {container_name}"
         subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
 
         # Wait a few seconds before connecting
         time.sleep(2)
 
         for ip_net in container.ips_and_networks:
+            time.sleep(2)
             ip, net = ip_net
             cmd = f"{constants.DOCKER.NETWORK_CONNECT} --ip {ip} {net.name} " \
                   f"{container_name}"
             logger.info(f"Connecting container:{container_name} to network:{net.name} with ip: {ip}, cmd: {cmd}")
             subprocess.Popen(cmd, stdout=subprocess.DEVNULL, shell=True)
             if container.docker_gw_bridge_ip == "" or container.docker_gw_bridge_ip is None:
                 # Wait to make sure docker networks are updated
```

### Comparing `csle_common-0.1.8/src/csle_common/controllers/elk_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/elk_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,9 +354,10 @@
                     elk_managers_statuses.append(
                         csle_collector.elk_manager.elk_manager_util.ElkManagerUtil.elk_dto_empty())
                 elk_managers_running.append(running)
         execution_id = emulation_env_config.execution_id
         emulation_name = emulation_env_config.name
         elk_manager_info_dto = ELKManagersInfo(
             elk_managers_running=elk_managers_running, ips=elk_managers_ips, execution_id=execution_id,
-            emulation_name=emulation_name, elk_managers_statuses=elk_managers_statuses, ports=elk_managers_ports)
+            emulation_name=emulation_name, elk_managers_statuses=elk_managers_statuses, ports=elk_managers_ports,
+            physical_server_ip=emulation_env_config.elk_config.container.physical_host_ip)
         return elk_manager_info_dto
```

### Comparing `csle_common-0.1.8/src/csle_common/controllers/emulation_env_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/emulation_env_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/flags_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/flags_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/host_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/host_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,61 +16,66 @@
 
 class HostController:
     """
     Class controlling host managers and host specific configurations
     """
 
     @staticmethod
-    def start_host_managers(emulation_env_config: EmulationEnvConfig) -> None:
+    def start_host_managers(emulation_env_config: EmulationEnvConfig, logger: logging.Logger) -> None:
         """
         Utility method for checking if the host manager is running and starting it if it is not running
 
         :param emulation_env_config: the emulation env config
+        :param logger: the logger to use for logging
         :return: None
         """
 
         # Start host managers on emulation containers
         for c in emulation_env_config.containers_config.containers:
             # Connect
-            HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=c.docker_gw_bridge_ip)
+            HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=c.docker_gw_bridge_ip,
+                                              logger=logger)
 
         # Start host manager on kafka container
         HostController.start_host_manager(emulation_env_config=emulation_env_config,
-                                          ip=emulation_env_config.kafka_config.container.docker_gw_bridge_ip)
+                                          ip=emulation_env_config.kafka_config.container.docker_gw_bridge_ip,
+                                          logger=logger)
 
         # Start host manager on ELK container
         HostController.start_host_manager(emulation_env_config=emulation_env_config,
-                                          ip=emulation_env_config.elk_config.container.docker_gw_bridge_ip)
+                                          ip=emulation_env_config.elk_config.container.docker_gw_bridge_ip,
+                                          logger=logger)
 
         if emulation_env_config.sdn_controller_config is not None:
             # Start host manager on SDN controller container
             HostController.start_host_manager(
                 emulation_env_config=emulation_env_config,
-                ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip)
+                ip=emulation_env_config.sdn_controller_config.container.docker_gw_bridge_ip, logger=logger)
 
     @staticmethod
-    def start_host_manager(emulation_env_config: EmulationEnvConfig, ip: str) -> None:
+    def start_host_manager(emulation_env_config: EmulationEnvConfig, ip: str, logger: logging.Logger) -> None:
         """
         Utility method for starting the host manager on a specific container
 
         :param emulation_env_config: the emulation env config
         :param ip: the ip of the container
+        :param logger: the logger to use for logging
         :return: None
         """
         # Connect
         EmulationUtil.connect_admin(emulation_env_config=emulation_env_config, ip=ip)
 
         # Check if host_manager is already running
         cmd = (constants.COMMANDS.PS_AUX + " | " + constants.COMMANDS.GREP +
                constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.HOST_MANAGER_FILE_NAME)
         o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd,
                                                 conn=emulation_env_config.get_connection(ip=ip))
 
         if constants.COMMANDS.SEARCH_HOST_MANAGER not in str(o):
-            Logger.__call__().get_logger().info(f"Starting host manager on node {ip}")
+            logger.info(f"Host manager is not running on: {ip}, starting it. Output of {cmd} was: {str(o)}")
 
             # Stop old background job if running
             cmd = (constants.COMMANDS.SUDO + constants.COMMANDS.SPACE_DELIM + constants.COMMANDS.PKILL +
                    constants.COMMANDS.SPACE_DELIM + constants.TRAFFIC_COMMANDS.HOST_MANAGER_FILE_NAME)
             o, e, _ = EmulationUtil.execute_ssh_cmd(cmd=cmd,
                                                     conn=emulation_env_config.get_connection(ip=ip))
 
@@ -658,15 +663,15 @@
         to start the Host manager and the monitor thread
 
         :param emulation_env_config: the emulation env config
         :param ip: IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ip, port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.monitor_running:
             logger.info(f"Host monitor thread is not running on {ip}, starting it.")
             # Open a gRPC session
             with grpc.insecure_channel(
@@ -686,18 +691,18 @@
 
         :param emulation_env_config: the emulation env config
         :param ips: IP of the container
         :param initial_start: boolean indicating whether this method is called on emulation initialization or not
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0])
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
         if initial_start:
             node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=ips)
-            if not node_beats_config.start_filebeat_automatically:
+            if node_beats_config is None or not node_beats_config.start_filebeat_automatically:
                 return
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ips[0], port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.filebeat_running:
             logger.info(
                 f"Filebeat is not running on {ips[0]}, starting it.")
             # Open a gRPC session
@@ -715,18 +720,18 @@
 
         :param emulation_env_config: the emulation env config
         :param ips: IP of the container
         :param initial_start: boolean indicating whether this method is called on emulation initialization or not
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0])
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
         if initial_start:
             node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=ips)
-            if not node_beats_config.start_packetbeat_automatically:
+            if node_beats_config is None or not node_beats_config.start_packetbeat_automatically:
                 return
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ips[0], port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.packetbeat_running:
             logger.info(
                 f"Packetbeat is not running on {ips[0]}, starting it.")
             # Open a gRPC session
@@ -744,18 +749,18 @@
 
         :param emulation_env_config: the emulation env config
         :param ips: IP of the container
         :param initial_start: boolean indicating whether this method is called on emulation initialization or not
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0])
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
         if initial_start:
             node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=ips)
-            if not node_beats_config.start_metricbeat_automatically:
+            if node_beats_config is None or not node_beats_config.start_metricbeat_automatically:
                 return
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ips[0], port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.metricbeat_running:
             logger.info(
                 f"Metricbeat is not running on {ips[0]}, starting it.")
             # Open a gRPC session
@@ -774,18 +779,18 @@
 
         :param emulation_env_config: the emulation env config
         :param ips: IPs of the container
         :param initial_start: boolean indicating whether this method is called on emulation initialization or not
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0])
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ips[0], logger=logger)
         if initial_start:
             node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=ips)
-            if not node_beats_config.start_heartbeat_automatically:
+            if node_beats_config is None or not node_beats_config.start_heartbeat_automatically:
                 return
         host_monitor_dto = HostController.get_host_monitor_thread_status_by_port_and_ip(
             ip=ips[0], port=emulation_env_config.host_manager_config.host_manager_port)
         if not host_monitor_dto.heartbeat_running:
             logger.info(
                 f"Heartbeat is not running on {ips[0]}, starting it.")
             # Open a gRPC session
@@ -802,16 +807,19 @@
         to setup the filebeat configuration
 
         :param emulation_env_config: the emulation env config
         :param container: the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip,
+                                          logger=logger)
         node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=container.get_ips())
+        if node_beats_config is None:
+            return
         kafka_topics = list(map(lambda topic: topic.name, emulation_env_config.kafka_config.topics))
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{container.docker_gw_bridge_ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
@@ -838,15 +846,16 @@
         to setup the packetbeat configuration
 
         :param emulation_env_config: the emulation env config
         :param container: the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip,
+                                          logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{container.docker_gw_bridge_ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Configuring packetbeat on {container.docker_gw_bridge_ip}, {container.get_full_name()}, "
@@ -866,16 +875,19 @@
         to setup the metricbeat configuration
 
         :param emulation_env_config: the emulation env config
         :param container: the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip,
+                                          logger=logger)
         node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=container.get_ips())
+        if node_beats_config is None:
+            return
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{container.docker_gw_bridge_ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Configuring metricbeat on {container.docker_gw_bridge_ip}, {container.get_full_name()}, "
@@ -899,16 +911,19 @@
         to setup the heartbeat configuration
 
         :param emulation_env_config: the emulation env config
         :param container: the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=container.docker_gw_bridge_ip,
+                                          logger=logger)
         node_beats_config = emulation_env_config.beats_config.get_node_beats_config_by_ips(ips=container.get_ips())
+        if node_beats_config is None:
+            return
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{container.docker_gw_bridge_ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Configuring heartbeat on {container.docker_gw_bridge_ip}, {container.get_full_name()}, "
@@ -962,15 +977,15 @@
         A method that sends a request to the HostManager on a specific container to stop the monitor threads
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Stopping the Host monitor thread on {ip}.")
@@ -982,15 +997,15 @@
         A method that sends a request to the HostManager on a specific container to stop filebeat
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Stopping filebeat on {ip}.")
@@ -1002,15 +1017,15 @@
         A method that sends a request to the HostManager on a specific container to stop packetbeat
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Stopping packetbeat on {ip}.")
@@ -1022,15 +1037,15 @@
         A method that sends a request to the HostManager on a specific container to stop metricbeat
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Stopping metricbeat on {ip}.")
@@ -1042,36 +1057,38 @@
         A method that sends a request to the HostManager on a specific container to stop heartbeat
 
         :param emulation_env_config: the emulation env config
         :param ip: the IP of the container
         :param logger: the logger to use for logging
         :return: None
         """
-        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip)
+        HostController.start_host_manager(emulation_env_config=emulation_env_config, ip=ip, logger=logger)
 
         # Open a gRPC session
         with grpc.insecure_channel(
                 f'{ip}:'
                 f'{emulation_env_config.host_manager_config.host_manager_port}') as channel:
             stub = csle_collector.host_manager.host_manager_pb2_grpc.HostManagerStub(channel)
             logger.info(f"Stopping heartbeat on {ip}.")
             csle_collector.host_manager.query_host_manager.stop_heartbeat(stub=stub)
 
     @staticmethod
-    def get_host_monitor_threads_statuses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str) -> \
+    def get_host_monitor_threads_statuses(emulation_env_config: EmulationEnvConfig, physical_server_ip: str,
+                                          logger: logging.Logger) -> \
             List[Tuple[csle_collector.host_manager.host_manager_pb2.HostStatusDTO, str]]:
         """
         A method that sends a request to the HostManager on every container to get the status of the Host monitor thread
 
         :param emulation_env_config: the emulation config
         :param physical_server_ip: the ip of the physical server
+        :param logger: the logger to use for logging
         :return: List of monitor thread statuses
         """
         statuses = []
-        HostController.start_host_managers(emulation_env_config=emulation_env_config)
+        HostController.start_host_managers(emulation_env_config=emulation_env_config, logger=logger)
 
         # Get statuses of emulation containers
         for c in emulation_env_config.containers_config.containers:
             if c.physical_host_ip == physical_server_ip:
                 status = HostController.get_host_monitor_thread_status_by_port_and_ip(
                     ip=c.docker_gw_bridge_ip, port=emulation_env_config.host_manager_config.host_manager_port)
                 statuses.append((status, c.docker_gw_bridge_ip))
```

### Comparing `csle_common-0.1.8/src/csle_common/controllers/installation_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/installation_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/kafka_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/management_system_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/management_system_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/ossec_ids_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/ossec_ids_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/ovs_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/ovs_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,17 +73,22 @@
         :param emulation_env_config: the emulation env config
         :param physical_server_ip: ip of the physical server
         :param logger: the logger to use for logging
         :return: None
         """
         for ovs_sw in emulation_env_config.ovs_config.switch_configs:
             if ovs_sw.physical_host_ip != physical_server_ip:
+                logger.info(f"Wrong host IP of switch: {ovs_sw.container_name}, {ovs_sw.physical_host_ip}, "
+                            f"{physical_server_ip}")
                 continue
-            logger.info(f"Configuring OVS bridge on container: {ovs_sw.container_name}")
+            logger.info(f"Configuring OVS bridge on container: {ovs_sw.container_name}, "
+                        f"physical host: {ovs_sw.physical_host_ip}, gw ip: {ovs_sw.docker_gw_bridge_ip}")
             EmulationUtil.connect_admin(emulation_env_config=emulation_env_config, ip=ovs_sw.docker_gw_bridge_ip)
             bridge_name = constants.OVS.DEFAULT_BRIDGE_NAME
             cmd = f"{constants.COMMANDS.SUDO} {constants.OVS.OVS_VSCTL} set bridge {bridge_name} " \
                   f"protocols={','.join(ovs_sw.openflow_protocols)}"
+            logger.info(f"Running cmd:{cmd} on container: {ovs_sw.container_name}")
             EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.connections[ovs_sw.docker_gw_bridge_ip])
             cmd = f"{constants.COMMANDS.SUDO} {constants.OVS.OVS_VSCTL} set-controller {bridge_name} " \
                   f"{ovs_sw.controller_transport_protocol}:{ovs_sw.controller_ip}:{ovs_sw.controller_port}"
+            logger.info(f"Running cmd:{cmd} on container: {ovs_sw.container_name}")
             EmulationUtil.execute_ssh_cmd(cmd=cmd, conn=emulation_env_config.connections[ovs_sw.docker_gw_bridge_ip])
```

### Comparing `csle_common-0.1.8/src/csle_common/controllers/resource_constraints_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/resource_constraints_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/sdn_controller_manager.py` & `csle_common-0.1.9/src/csle_common/controllers/sdn_controller_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,9 +286,10 @@
             else:
                 ryu_managers_statuses.append(csle_collector.ryu_manager.ryu_manager_util.RyuManagerUtil.ryu_dto_empty())
             ryu_managers_running.append(running)
         execution_id = emulation_env_config.execution_id
         emulation_name = emulation_env_config.name
         ryu_manager_info_dto = RyuManagersInfo(
             ryu_managers_running=ryu_managers_running, ips=ryu_managers_ips, execution_id=execution_id,
-            emulation_name=emulation_name, ryu_managers_statuses=ryu_managers_statuses, ports=ryu_managers_ports)
+            emulation_name=emulation_name, ryu_managers_statuses=ryu_managers_statuses, ports=ryu_managers_ports,
+            physical_server_ip=emulation_env_config.sdn_controller_config.container.physical_host_ip)
         return ryu_manager_info_dto
```

### Comparing `csle_common-0.1.8/src/csle_common/controllers/simulation_env_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/simulation_env_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/snort_ids_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/snort_ids_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/topology_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/topology_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/traffic_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/traffic_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/users_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/users_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/controllers/vulnerabilities_controller.py` & `csle_common-0.1.9/src/csle_common/controllers/vulnerabilities_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/datasets/statistics_dataset.py` & `csle_common-0.1.9/src/csle_common/dao/datasets/statistics_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/datasets/traces_dataset.py` & `csle_common-0.1.9/src/csle_common/dao/datasets/traces_dataset.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/docker/docker_container_metadata.py` & `csle_common-0.1.9/src/csle_common/dao/docker/docker_container_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/docker/docker_env_metadata.py` & `csle_common-0.1.9/src/csle_common/dao/docker/docker_env_metadata.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/domain_randomization/node_randomizer_config.py` & `csle_common-0.1.9/src/csle_common/dao/domain_randomization/node_randomizer_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/domain_randomization/randomization_space.py` & `csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/domain_randomization/randomization_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/domain_randomization/randomization_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_action_id.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_masscan_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_network_service_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nikto_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_nmap_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_shell_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/attacker/emulation_attacker_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_action_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action/defender/emulation_defender_stopping_actions.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nikto_scan_result.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nikto_vuln.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nikto_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_brute_credentials.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_hop.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_hop.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_host_result.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_host_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_os.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_os.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_port.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_port.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_scan_result.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_scan_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_trace.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_action_result/nmap_vuln.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_action_result/nmap_vuln.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/beats_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/client_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/client_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/client_population_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/client_population_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/cluster_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/cluster_node.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/cluster_node.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/connection_setup_dto.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/connection_setup_dto.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/container_network.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/container_network.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/containers_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/containers_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/credential.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/credential.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/default_network_firewall_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/default_network_firewall_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/docker_stats_manager_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/docker_stats_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/docker_stats_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/elk_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/elk_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/elk_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_managers_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 from typing import List, Dict, Any
-import csle_collector.elk_manager.elk_manager_pb2_grpc
-import csle_collector.elk_manager.elk_manager_pb2
-import csle_collector.elk_manager.elk_manager_util as elk_manager_util
+import csle_collector.kafka_manager.kafka_manager_pb2_grpc
+import csle_collector.kafka_manager.kafka_manager_pb2
+import csle_collector.kafka_manager.kafka_manager_util as kafka_manager_util
 
 
-class ELKManagersInfo:
+class KafkaManagersInfo:
     """
-    DTO containing the status of the ELK managers for a given emulation execution
+    DTO containing the status of the Kafka managers for a given emulation execution
     """
 
     def __init__(self, ips: List[str], ports: List[int],
                  emulation_name: str, execution_id: int,
-                 elk_managers_statuses: List[csle_collector.elk_manager.elk_manager_pb2.ElkDTO],
-                 elk_managers_running: List[bool], local_kibana_port: int = -1):
+                 kafka_managers_statuses: List[csle_collector.kafka_manager.kafka_manager_pb2.KafkaDTO],
+                 kafka_managers_running: List[bool]):
         """
         Initializes the DTO
 
-        :param elk_managers_running: boolean list that indicate whether the elk managers are running
-        :param ips: the list of IPs of the running ELK managers
-        :param ports: the list of ports of the running ELK managers
+        :param ips: the list of IPs of the running Kafka managers
+        :param ports: the list of ports of the running Kafka managers
         :param emulation_name: the name of the corresponding emulation
         :param execution_id: the ID of the corresponding emulation execution
-        :param elk_managers_statuses: a list of statuses of the ELK managers
-        :param local_kibana_port: the local port that is forwarded to Kibana
+        :param kafka_managers_statuses: a list of statuses of the Kafka managers
+        :param kafka_managers_running: a list of booleans indicating whether the Kafka managers are running or not
         """
-        self.elk_managers_running = elk_managers_running
+        self.kafka_managers_running = kafka_managers_running
         self.ips = ips
         self.ports = ports
         self.emulation_name = emulation_name
         self.execution_id = execution_id
-        self.elk_managers_statuses = elk_managers_statuses
-        self.local_kibana_port = local_kibana_port
+        self.kafka_managers_statuses = kafka_managers_statuses
 
     def __str__(self):
         """
         :return: a string representation of the DTO
         """
-        return f"elk_managers_running: {self.elk_managers_running}, ips: {list(map(lambda x: str(x), self.ips))}, " \
+        return f"kafka_managers_running: {self.kafka_managers_running}, " \
+               f"ips: {list(map(lambda x: str(x), self.ips))}, " \
                f"emulation_name: {self.emulation_name}, " \
                f"execution_id: {self.execution_id}, " \
-               f"elk_managers_statuses: {list(map(lambda x: str(x), self.elk_managers_statuses))}, " \
-               f"ports: {list(map(lambda x: str(x), self.ports))}," \
-               f"local_kibana_port: {self.local_kibana_port}"
+               f"kafka_managers_statuses: {list(map(lambda x: str(x), self.kafka_managers_statuses))}, " \
+               f"ports: {list(map(lambda x: str(x), self.ports))}"
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
-        d["elk_managers_running"] = self.elk_managers_running
+        d["kafka_managers_running"] = self.kafka_managers_running
         d["ips"] = self.ips
         d["ports"] = self.ports
         d["emulation_name"] = self.emulation_name
         d["execution_id"] = self.execution_id
-        d["local_kibana_port"] = self.local_kibana_port
-        d["elk_managers_statuses"] = list(map(
-            lambda x: elk_manager_util.ElkManagerUtil.elk_dto_to_dict(x), self.elk_managers_statuses))
+        d["kafka_managers_statuses"] = list(map(
+            lambda x: kafka_manager_util.KafkaManagerUtil.kafka_dto_to_dict(x),
+            self.kafka_managers_statuses))
         return d
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "ELKManagersInfo":
+    def from_dict(d: Dict[str, Any]) -> "KafkaManagersInfo":
         """
         Convert a dict representation to a DTO representation
 
         :return: a dto representation of the object
         """
-        dto = ELKManagersInfo(elk_managers_running=d["elk_managers_running"], ips=d["ips"], ports=d["ports"],
-                              emulation_name=d["emulation_name"], execution_id=d["execution_id"],
-                              elk_managers_statuses=list(map(
-                                  lambda x: elk_manager_util.ElkManagerUtil.elk_dto_to_dict(x),
-                                  d["elk_managers_statuses"])), local_kibana_port=d["local_kibana_port"])
+        dto = KafkaManagersInfo(
+            kafka_managers_running=d["kafka_managers_running"], ips=d["ips"], ports=d["ports"],
+            emulation_name=d["emulation_name"], execution_id=d["execution_id"],
+            kafka_managers_statuses=list(map(
+                lambda x: kafka_manager_util.KafkaManagerUtil.kafka_dto_from_dict(x), d["kafka_managers_statuses"])))
         return dto
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,16 @@
         config.vuln_config = config.vuln_config.create_execution_config(ip_first_octet=ip_first_octet)
         config.topology_config = config.topology_config.create_execution_config(ip_first_octet=ip_first_octet)
         config.traffic_config = config.traffic_config.create_execution_config(ip_first_octet=ip_first_octet)
         config.resources_config = config.resources_config.create_execution_config(ip_first_octet=ip_first_octet)
         config.kafka_config = config.kafka_config.create_execution_config(ip_first_octet=ip_first_octet,
                                                                           physical_servers=physical_servers)
         config.services_config = config.services_config.create_execution_config(ip_first_octet=ip_first_octet)
-        config.ovs_config = config.ovs_config.create_execution_config(ip_first_octet=ip_first_octet)
+        config.ovs_config = config.ovs_config.create_execution_config(ip_first_octet=ip_first_octet,
+                                                                      physical_servers=physical_servers)
         config.host_manager_config = config.host_manager_config.create_execution_config(ip_first_octet=ip_first_octet)
         config.snort_ids_manager_config = config.snort_ids_manager_config.create_execution_config(
             ip_first_octet=ip_first_octet)
         config.ossec_ids_manager_config = config.ossec_ids_manager_config.create_execution_config(
             ip_first_octet=ip_first_octet)
         config.docker_stats_manager_config = config.docker_stats_manager_config.create_execution_config(
             ip_first_octet=ip_first_octet)
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_generation_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_generation_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_env_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_env_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_execution.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_execution_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_execution_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_metrics_time_series.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_simulation_trace.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_statistics_windowed.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/emulation_trace.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/emulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/flag.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/flag.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/flags_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/host_manager_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/host_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/host_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/host_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_managers_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from typing import List, Dict, Any
-import csle_collector.kafka_manager.kafka_manager_pb2_grpc
-import csle_collector.kafka_manager.kafka_manager_pb2
-import csle_collector.kafka_manager.kafka_manager_util as kafka_manager_util
+import csle_collector.traffic_manager.traffic_manager_pb2_grpc
+import csle_collector.traffic_manager.traffic_manager_pb2
+import csle_collector.traffic_manager.traffic_manager_util as traffic_manager_util
 
 
-class KafkaManagersInfo:
+class TrafficManagersInfo:
     """
-    DTO containing the status of the Kafka managers for a given emulation execution
+    DTO containing the status of the Traffic managers for a given emulation execution
     """
 
     def __init__(self, ips: List[str], ports: List[int],
                  emulation_name: str, execution_id: int,
-                 kafka_managers_statuses: List[csle_collector.kafka_manager.kafka_manager_pb2.KafkaDTO],
-                 kafka_managers_running: List[bool]):
+                 traffic_managers_statuses: List[csle_collector.traffic_manager.traffic_manager_pb2.TrafficDTO],
+                 traffic_managers_running: List[bool]):
         """
         Initializes the DTO
 
-        :param ips: the list of IPs of the running Kafka managers
-        :param ports: the list of ports of the running Kafka managers
+        :param ips: the list of IPs of the running traffic managers
+        :param ports: the list of ports of the running traffic managers
         :param emulation_name: the name of the corresponding emulation
         :param execution_id: the ID of the corresponding emulation execution
-        :param kafka_managers_statuses: a list of statuses of the Kafka managers
-        :param kafka_managers_running: a list of booleans indicating whether the Kafka managers are running or not
+        :param traffic_managers_statuses: a list of statuses of the traffic managers
+        :param traffic_managers_running: a list of booleans indicating whether the traffic managers are running
         """
-        self.kafka_managers_running = kafka_managers_running
+        self.traffic_managers_running = traffic_managers_running
         self.ips = ips
         self.ports = ports
         self.emulation_name = emulation_name
         self.execution_id = execution_id
-        self.kafka_managers_statuses = kafka_managers_statuses
+        self.traffic_managers_statuses = traffic_managers_statuses
 
     def __str__(self):
         """
         :return: a string representation of the DTO
         """
-        return f"kafka_managers_running: {self.kafka_managers_running}, " \
+        return f"traffic_managers_running: {self.traffic_managers_running}, " \
                f"ips: {list(map(lambda x: str(x), self.ips))}, " \
+               f"ports: {list(map(lambda x: str(x), self.ports))}," \
                f"emulation_name: {self.emulation_name}, " \
                f"execution_id: {self.execution_id}, " \
-               f"kafka_managers_statuses: {list(map(lambda x: str(x), self.kafka_managers_statuses))}, " \
-               f"ports: {list(map(lambda x: str(x), self.ports))}"
+               f"traffic_managers_statuses: {list(map(lambda x: str(x), self.traffic_managers_statuses))}"
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
-        d["kafka_managers_running"] = self.kafka_managers_running
+        d["traffic_managers_running"] = self.traffic_managers_running
         d["ips"] = self.ips
-        d["ports"] = self.ports
         d["emulation_name"] = self.emulation_name
         d["execution_id"] = self.execution_id
-        d["kafka_managers_statuses"] = list(map(
-            lambda x: kafka_manager_util.KafkaManagerUtil.kafka_dto_to_dict(x),
-            self.kafka_managers_statuses))
+        d["ports"] = self.ports
+        d["traffic_managers_statuses"] = list(map(
+            lambda x: traffic_manager_util.TrafficManagerUtil.traffic_dto_to_dict(x),
+            self.traffic_managers_statuses))
         return d
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "KafkaManagersInfo":
+    def from_dict(d: Dict[str, Any]) -> "TrafficManagersInfo":
         """
         Convert a dict representation to a DTO representation
 
         :return: a dto representation of the object
         """
-        dto = KafkaManagersInfo(
-            kafka_managers_running=d["kafka_managers_running"], ips=d["ips"], ports=d["ports"],
+        dto = TrafficManagersInfo(
+            traffic_managers_running=d["traffic_managers_running"], ips=d["ips"], ports=d["ports"],
             emulation_name=d["emulation_name"], execution_id=d["execution_id"],
-            kafka_managers_statuses=list(map(
-                lambda x: kafka_manager_util.KafkaManagerUtil.kafka_dto_from_dict(x), d["kafka_managers_statuses"])))
+            traffic_managers_statuses=list(map(lambda x: traffic_manager_util.TrafficManagerUtil.traffic_dto_to_dict(x),
+                                               d["traffic_managers_statuses"])))
         return dto
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/kafka_topic.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/network_service.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/network_service.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_beats_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_beats_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_container_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_container_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_firewall_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_firewall_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_flags_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_flags_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_network_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_network_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_resources_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_services_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_traffic_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_traffic_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_users_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/node_vulnerability_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/node_vulnerability_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/ossec_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/ossec_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/ovs_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,18 +78,20 @@
 
     def copy(self) -> "OVSConfig":
         """
         :return: a copy of the DTO
         """
         return OVSConfig.from_dict(self.to_dict())
 
-    def create_execution_config(self, ip_first_octet: int) -> "OVSConfig":
+    def create_execution_config(self, ip_first_octet: int, physical_servers: List[str]) -> "OVSConfig":
         """
         Creates a new config for an execution
 
         :param ip_first_octet: the first octet of the IP of the new execution
+        :param physical_servers: the list of physical servers of the execution
         :return: the new config
         """
         config = self.copy()
-        config.switch_configs = list(map(lambda x: x.create_execution_config(ip_first_octet=ip_first_octet),
+        config.switch_configs = list(map(lambda x: x.create_execution_config(
+            ip_first_octet=ip_first_octet, physical_servers=physical_servers),
                                          config.switch_configs))
         return config
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/ovs_switch_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/ovs_switch_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,20 +109,22 @@
 
     def copy(self) -> "OvsSwitchConfig":
         """
         :return: a copy of the DTO
         """
         return OvsSwitchConfig.from_dict(self.to_dict())
 
-    def create_execution_config(self, ip_first_octet: int) -> "OvsSwitchConfig":
+    def create_execution_config(self, ip_first_octet: int, physical_servers: List[str]) -> "OvsSwitchConfig":
         """
         Creates a new config for an execution
 
         :param ip_first_octet: the first octet of the IP of the new execution
+        :param physical_servers: the list of physical servers of the execution
         :return: the new config
         """
         config = self.copy()
         config.ip = GeneralUtil.replace_first_octet_of_ip(ip=config.ip, ip_first_octet=ip_first_octet)
         config.controller_ip = GeneralUtil.replace_first_octet_of_ip(ip=config.controller_ip,
                                                                      ip_first_octet=ip_first_octet)
         config.container_name = f"{config.container_name}-{ip_first_octet}"
+        config.physical_host_ip = physical_servers[0]  # TODO Update this
         return config
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/resources_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/resources_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/ryu_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/ryu_managers_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,56 +8,61 @@
     """
     DTO containing the status of the Ryu managers for a given emulation execution
     """
 
     def __init__(self, ips: List[str], ports: List[int],
                  emulation_name: str, execution_id: int,
                  ryu_managers_statuses: List[csle_collector.ryu_manager.ryu_manager_pb2.RyuDTO],
-                 ryu_managers_running: List[bool], local_controller_web_port: int = -1):
+                 ryu_managers_running: List[bool], local_controller_web_port: int = -1,
+                 physical_server_ip: str = ""):
         """
         Initializes the DTO
 
         :param ryu_managers_running: boolean list that indicate whether the Ryu managers are running
         :param ips: the list of IPs of the running Ryu managers
         :param ports: the list of ports of the running Ryu managers
         :param emulation_name: the name of the corresponding emulation
         :param execution_id: the ID of the corresponding emulation execution
         :param ryu_managers_statuses: a list of statuses of the Ryu managers
         :param local_controller_web_port: the local port that is forwarded to the SDN controller's web api
+        :param physical_server_ip: the ip of the physical server where Ryu is running
         """
         self.ryu_managers_running = ryu_managers_running
         self.ips = ips
         self.ports = ports
         self.emulation_name = emulation_name
         self.execution_id = execution_id
         self.ryu_managers_statuses = ryu_managers_statuses
         self.local_controller_web_port = local_controller_web_port
+        self.physical_server_ip = physical_server_ip
 
     def __str__(self):
         """
         :return: a string representation of the DTO
         """
         return f"ryu_managers_running: {self.ryu_managers_running}, ips: {list(map(lambda x: str(x), self.ips))}, " \
                f"emulation_name: {self.emulation_name}, " \
                f"execution_id: {self.execution_id}, " \
                f"ryu_managers_statuses: {list(map(lambda x: str(x), self.ryu_managers_statuses))}, " \
                f"ports: {list(map(lambda x: str(x), self.ports))}," \
-               f"local_controller_web_port: {self.local_controller_web_port}"
+               f"local_controller_web_port: {self.local_controller_web_port}, " \
+               f"physical_server_ip: {self.physical_server_ip}"
 
     def to_dict(self) -> Dict[str, Any]:
         """
         :return: a dict representation of the object
         """
         d = {}
         d["ryu_managers_running"] = self.ryu_managers_running
         d["ips"] = self.ips
         d["ports"] = self.ports
         d["emulation_name"] = self.emulation_name
         d["execution_id"] = self.execution_id
         d["local_controller_web_port"] = self.local_controller_web_port
+        d["physical_server_ip"] = self.physical_server_ip
         d["ryu_managers_statuses"] = list(map(
             lambda x: ryu_manager_util.RyuManagerUtil.ryu_dto_to_dict(x), self.ryu_managers_statuses))
         return d
 
     @staticmethod
     def from_dict(d: Dict[str, Any]) -> "RyuManagersInfo":
         """
@@ -66,9 +71,10 @@
         :return: a dto representation of the object
         """
         dto = RyuManagersInfo(ryu_managers_running=d["ryu_managers_running"], ips=d["ips"], ports=d["ports"],
                               emulation_name=d["emulation_name"], execution_id=d["execution_id"],
                               ryu_managers_statuses=list(map(
                                   lambda x: ryu_manager_util.RyuManagerUtil.ryu_dto_to_dict(x),
                                   d["ryu_managers_statuses"])),
-                              local_controller_web_port=d["local_controller_web_port"])
+                              local_controller_web_port=d["local_controller_web_port"],
+                              physical_server_ip=d["physical_server_ip"])
         return dto
```

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/sdn_controller_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/sdn_controller_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/services_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/services_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/snort_ids_manager_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_ids_manager_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/snort_managers_info.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/snort_managers_info.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/topology_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/topology_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/traffic_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/traffic_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/transport_protocol.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/transport_protocol.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/user.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/users_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/users_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_config/vulnerabilities_config.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_config/vulnerabilities_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_machine_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/attacker/emulation_attacker_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_connection_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_port_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/common/emulation_vulnerability_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_machine_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py` & `csle_common-0.1.9/src/csle_common/dao/emulation_observation/defender/emulation_defender_observation_state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/jobs/data_collection_job_config.py` & `csle_common-0.1.9/src/csle_common/dao/jobs/data_collection_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/jobs/system_identification_job_config.py` & `csle_common-0.1.9/src/csle_common/dao/jobs/system_identification_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/jobs/training_job_config.py` & `csle_common-0.1.9/src/csle_common/dao/jobs/training_job_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/management/management_user.py` & `csle_common-0.1.9/src/csle_common/dao/management/management_user.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/management/session_token.py` & `csle_common-0.1.9/src/csle_common/dao/management/session_token.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/action.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/action.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/action_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/base_env.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/base_env.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/env_parameter.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/env_parameters_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/env_parameters_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/initial_state_distribution_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/initial_state_distribution_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/joint_action_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_action_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/joint_observation_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/joint_observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/observation.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/observation_function_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/observation_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/observation_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/player_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/player_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/players_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/players_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/reward_function_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/reward_function_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/simulation_env_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_env_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/simulation_trace.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/simulation_trace.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/state.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/state.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/state_space_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/state_space_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/simulation_config/transition_operator_config.py` & `csle_common-0.1.9/src/csle_common/dao/simulation_config/transition_operator_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/empirical_conditional.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/empirical_system_model.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/empirical_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/emulation_statistics.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/emulation_statistics.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/gaussian_mixture_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/gp_conditional.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/gp_conditional.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/gp_system_model.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/gp_system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/system_identification_config.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/system_identification_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/system_identification/system_model.py` & `csle_common-0.1.9/src/csle_common/dao/system_identification/system_model.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/agent_type.py` & `csle_common-0.1.9/src/csle_common/dao/training/agent_type.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/alpha_vectors_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/alpha_vectors_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/dqn_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/dqn_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/experiment_config.py` & `csle_common-0.1.9/src/csle_common/dao/training/experiment_config.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/experiment_execution.py` & `csle_common-0.1.9/src/csle_common/dao/training/experiment_execution.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/experiment_result.py` & `csle_common-0.1.9/src/csle_common/dao/training/experiment_result.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/fnn_with_softmax_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/fnn_with_softmax_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/hparam.py` & `csle_common-0.1.9/src/csle_common/dao/training/hparam.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/mixed_multi_threshold_stopping_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/multi_threshold_stopping_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/multi_threshold_stopping_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/ppo_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/ppo_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/random_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/random_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/tabular_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/tabular_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/dao/training/vector_policy.py` & `csle_common-0.1.9/src/csle_common/dao/training/vector_policy.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/logging/custom_formatter.py` & `csle_common-0.1.9/src/csle_common/logging/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/logging/log.py` & `csle_common-0.1.9/src/csle_common/logging/log.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/metastore/metastore_facade.py` & `csle_common-0.1.9/src/csle_common/metastore/metastore_facade.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/models/fnn_w_softmax.py` & `csle_common-0.1.9/src/csle_common/models/fnn_w_softmax.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/tunneling/forward_ssh_controller.py` & `csle_common-0.1.9/src/csle_common/tunneling/forward_ssh_controller.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/tunneling/forward_tunnel_thread.py` & `csle_common-0.1.9/src/csle_common/tunneling/forward_tunnel_thread.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/cluster_util.py` & `csle_common-0.1.9/src/csle_common/util/cluster_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/connection_util.py` & `csle_common-0.1.9/src/csle_common/util/connection_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/docker_util.py` & `csle_common-0.1.9/src/csle_common/util/docker_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/emulation_util.py` & `csle_common-0.1.9/src/csle_common/util/emulation_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/env_dynamics_util.py` & `csle_common-0.1.9/src/csle_common/util/env_dynamics_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/experiment_util.py` & `csle_common-0.1.9/src/csle_common/util/experiment_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/export_util.py` & `csle_common-0.1.9/src/csle_common/util/export_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/general_util.py` & `csle_common-0.1.9/src/csle_common/util/general_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/grpc_util.py` & `csle_common-0.1.9/src/csle_common/util/grpc_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/import_util.py` & `csle_common-0.1.9/src/csle_common/util/import_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/management_util.py` & `csle_common-0.1.9/src/csle_common/util/management_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/plotting_util.py` & `csle_common-0.1.9/src/csle_common/util/plotting_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/read_emulation_statistics_util.py` & `csle_common-0.1.9/src/csle_common/util/read_emulation_statistics_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common/util/ssh_util.py` & `csle_common-0.1.9/src/csle_common/util/ssh_util.py`

 * *Files identical despite different names*

### Comparing `csle_common-0.1.8/src/csle_common.egg-info/PKG-INFO` & `csle_common-0.1.9/src/csle_common.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-common
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common functionality of the Cyber Security Learning Environment (CSLE)
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_common-0.1.8/src/csle_common.egg-info/SOURCES.txt` & `csle_common-0.1.9/src/csle_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

