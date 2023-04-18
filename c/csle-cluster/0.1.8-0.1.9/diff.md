# Comparing `tmp/csle_cluster-0.1.8.tar.gz` & `tmp/csle_cluster-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.1.8.tar", last modified: Mon Mar 20 15:30:02 2023, max compression
+gzip compressed data, was "csle_cluster-0.1.9.tar", last modified: Tue Mar 21 08:10:49 2023, max compression
```

## Comparing `csle_cluster-0.1.8.tar` & `csle_cluster-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.763039 csle_cluster-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-03-20 15:30:02.763163 csle_cluster-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-03-20 15:30:02.763757 csle_cluster-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.743600 csle_cluster-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.746344 csle_cluster-0.1.8/src/csle_cluster/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.1.8/src/csle_cluster/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_cluster-0.1.8/src/csle_cluster/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.760643 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)   222811 2023-03-20 12:28:23.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)   260471 2023-03-20 13:23:39.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)   189385 2023-03-16 07:13:37.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)   339988 2023-03-16 07:14:54.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)   184506 2023-03-16 16:29:03.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)   182935 2023-03-16 16:24:28.000000 csle_cluster-0.1.8/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.762505 csle_cluster-0.1.8/src/csle_cluster/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.1.8/src/csle_cluster/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.1.8/src/csle_cluster/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:30:02.748880 csle_cluster-0.1.8/src/csle_cluster.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-03-20 15:30:02.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      805 2023-03-20 15:30:02.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:30:02.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-03-20 15:30:02.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       13 2023-03-20 15:30:02.000000 csle_cluster-0.1.8/src/csle_cluster.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4256 2023-03-04 16:33:53.000000 csle_cluster-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1406 2023-03-21 08:10:49.085291 csle_cluster-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.077291 csle_cluster-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/src/csle_cluster/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_cluster-0.1.9/src/csle_cluster/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-02-13 15:55:11.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   222811 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   260635 2023-03-21 08:07:44.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   189531 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   339988 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   185021 2023-03-21 06:33:58.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   182935 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-03 14:11:41.000000 csle_cluster-0.1.9/src/csle_cluster/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      375 2023-03-17 07:49:22.000000 csle_cluster-0.1.9/src/csle_cluster/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:10:49.081291 csle_cluster-0.1.9/src/csle_cluster.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      804 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      805 2023-03-21 08:10:49.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      251 2023-03-21 08:10:48.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       13 2023-03-21 08:10:49.000000 csle_cluster-0.1.9/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.1.8/PKG-INFO` & `csle_cluster-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.1.8/README.md` & `csle_cluster-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.8/pyproject.toml` & `csle_cluster-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.8/setup.cfg` & `csle_cluster-0.1.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.1.8
-	csle-common>=0.1.8
-	csle-ryu>=0.1.8
+	csle-collector>=0.1.9
+	csle-common>=0.1.9
+	csle-ryu>=0.1.9
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -808,15 +808,15 @@
         """
         Configures OVS switches in an execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: an OperationOutcomeDTO
         """
-        logging.info(f"Configures OVS switches in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Configuring OVS switches in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         OVSController.apply_ovs_config(emulation_env_config=execution.emulation_env_config,
                                        physical_server_ip=GeneralUtil.get_host_ip(), logger=logging.getLogger())
@@ -1618,15 +1618,15 @@
         """
         Gets the number of active clients of a given execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a GetNumActiveClientsMsg
         """
-        logging.info(f"Gets the number of active clients in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the number of active clients in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None \
                 and execution.emulation_env_config.traffic_config.client_population_config.physical_host_ip == \
                 GeneralUtil.get_host_ip():
             clients_dto = TrafficController.get_num_active_clients(emulation_env_config=execution.emulation_env_config,
@@ -1717,15 +1717,15 @@
         """
         Gets the info of client managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a ClientManagersInfoDTO
         """
-        logging.info(f"Gets the info of client managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of client managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None and \
                 execution.emulation_env_config.traffic_config.client_population_config.physical_host_ip \
                 == GeneralUtil.get_host_ip():
             client_managers_dto = TrafficController.get_client_managers_info(
@@ -1741,15 +1741,15 @@
         """
         Gets the info of traffic managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a TrafficManagersInfoDTO
         """
-        logging.info(f"Gets the info of traffic managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of traffic managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             traffic_managers_dto = TrafficController.get_traffic_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -2059,15 +2059,15 @@
         """
         Gets the info of docker stats maangers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a DockerStatsManagersInfoDTO
         """
-        logging.info(f"Gets the info of docker stats managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of docker stats managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             docker_stats_managers_dto = ContainerController.get_docker_stats_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -2305,15 +2305,15 @@
         """
         Gets the info of elk managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a ElkManagersInfoDTO
         """
-        logging.info(f"Gets the info of elk managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of elk managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             elk_managers_dto = ELKController.get_elk_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -2395,15 +2395,15 @@
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is None:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
         container_config = ClusterManagerUtil.get_container_config(execution=execution, ip=request.containerIp)
         if container_config is not None:
             HostController.start_host_manager(emulation_env_config=execution.emulation_env_config,
-                                              ip=container_config.docker_gw_bridge_ip)
+                                              ip=container_config.docker_gw_bridge_ip, logger=logging.getLogger())
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=True)
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO(outcome=False)
 
     def stopHostManagers(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.StopHostManagersMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
@@ -2881,22 +2881,23 @@
         """
         Gets the host monitor thread statuses of a given execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a HostManagerStatusesDTO
         """
-        logging.info(f"Gets the host monitor thread statuses "
+        logging.info(f"Getting the host monitor thread statuses "
                      f"in execution with id: {request.ipFirstOctet} and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             host_statuses_and_ips = \
                 HostController.get_host_monitor_threads_statuses(emulation_env_config=execution.emulation_env_config,
-                                                                 physical_server_ip=GeneralUtil.get_host_ip())
+                                                                 physical_server_ip=GeneralUtil.get_host_ip(),
+                                                                 logger=logging.getLogger())
             host_statuses = list(map(lambda x: ClusterManagerUtil.convert_host_status_to_host_manager_status_dto(x),
                                      host_statuses_and_ips))
             return csle_cluster.cluster_manager.cluster_manager_pb2.HostManagerStatusesDTO(
                 hostManagerStatuses=host_statuses
             )
         else:
             return csle_cluster.cluster_manager.cluster_manager_pb2.HostManagerStatusesDTO(
@@ -2909,15 +2910,15 @@
         """
         Gets the info of host managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a HostManagersInfoDTO
         """
-        logging.info(f"Gets the info of host managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of host managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             host_managers_dto = HostController.get_host_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -3062,15 +3063,15 @@
         """
         Gets the info of kafka managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a KafkaManagersInfoDTO
         """
-        logging.info(f"Gets the info of kafka managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of kafka managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             kafka_managers_info_dto = KafkaController.get_kafka_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -3360,15 +3361,15 @@
         """
         Gets the info of OSSEC IDS managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a OSSECIdsManagersInfoDTO
         """
-        logging.info(f"Gets the info of OSSEC IDS managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of OSSEC IDS managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             ossec_ids_managers_info_dto = OSSECIDSController.get_ossec_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -3499,15 +3500,15 @@
         """
         Gets the info of Ryu managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a RyuManagersInfoDTO
         """
-        logging.info(f"Gets the info of Ryu managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of Ryu managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             ryu_managers_info_dto = SDNControllerManager.get_ryu_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -3816,15 +3817,15 @@
         """
         Gets the info of Snort IDS managers
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a SnortIdsManagersInfoDTO
         """
-        logging.info(f"Gets the info of Snort IDS managers in execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of Snort IDS managers in execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             snort_ids_managers_info_dto = SnortIDSController.get_snort_managers_info(
                 emulation_env_config=execution.emulation_env_config, logger=logging.getLogger(),
                 active_ips=ClusterManagerUtil.get_active_ips(emulation_env_config=execution.emulation_env_config),
@@ -3839,15 +3840,15 @@
         """
         Gets the info of a given execution
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: an ExecutionInfoDTO
         """
-        logging.info(f"Gets the info of the execution with id: {request.ipFirstOctet} "
+        logging.info(f"Getting the info of the execution with id: {request.ipFirstOctet} "
                      f"and emulation: {request.emulation}")
         execution = MetastoreFacade.get_emulation_execution(ip_first_octet=request.ipFirstOctet,
                                                             emulation_name=request.emulation)
         if execution is not None:
             execution_info_dto = EmulationEnvController.get_execution_info(
                 execution=execution, logger=logging.getLogger(), physical_server_ip=GeneralUtil.get_host_ip())
             return ClusterManagerUtil.convert_execution_info_dto(execution_info_dto=execution_info_dto)
@@ -3860,29 +3861,29 @@
         """
         Lists the Kibana tunnels
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: an KibanaTunnelsDTO
         """
-        logging.info("Gets the Kibana tunnels")
+        logging.info("Getting the Kibana tunnels")
         return ClusterManagerUtil.create_kibana_tunnels_dto_from_dict(
             dict=cluster_constants.KIBANA_TUNNELS.KIBANA_TUNNELS_DICT)
 
     def listRyuTunnels(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.ListRyuTunnelsMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.RyuTunnelsDTO:
         """
         Lists the Ryu tunnels
 
         :param request: the gRPC request
         :param context: the gRPC context
         :return: a RyuTunnelsDTO
         """
-        logging.info("Gets the Ryu tunnels")
+        logging.info("Getting the Ryu tunnels")
         return ClusterManagerUtil.create_ryu_tunnels_dto_from_dict(
             dict=cluster_constants.RYU_TUNNELS.RYU_TUNNELS_DICT)
 
     def createKibanaTunnel(
             self, request: csle_cluster.cluster_manager.cluster_manager_pb2.CreateKibanaTunnelMsg,
             context: grpc.ServicerContext) -> csle_cluster.cluster_manager.cluster_manager_pb2.OperationOutcomeDTO:
         """
```

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x63luster_manager.proto\"Y\n\x1dGetExecutionTimeSeriesDataMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x0f\n\x07minutes\x18\x03 \x01(\x05\"\xa3\t\n\x1d\x45mulationMetricsTimeSeriesDTO\x12\x33\n\x0e\x63lient_metrics\x18\x01 \x03(\x0b\x32\x1b.ClientPopulationMetricsDTO\x12\x30\n\x17\x61ggregated_docker_stats\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\x12+\n\x11\x64ocker_host_stats\x18\x03 \x03(\x0b\x32\x10.DockerStatsDict\x12&\n\x0chost_metrics\x18\x04 \x03(\x0b\x32\x10.HostMetricsDict\x12\x34\n\x17\x61ggregated_host_metrics\x18\x05 \x03(\x0b\x32\x13.HostMetricsDataDTO\x12\x35\n\x10\x64\x65\x66\x65nder_actions\x18\x06 \x03(\x0b\x32\x1b.EmulationDefenderActionDTO\x12\x35\n\x10\x61ttacker_actions\x18\x07 \x03(\x0b\x32\x1b.EmulationAttackerActionDTO\x12\x34\n\x11snort_ids_metrics\x18\x08 \x03(\x0b\x32\x19.SnortIdsAlertCountersDTO\x12\x14\n\x0c\x65mulation_id\x18\t \x01(\x05\x12=\n\x19ossec_host_alert_counters\x18\n \x03(\x0b\x32\x1a.OSSECIdsAlertCountersDict\x12G\n$aggregated_ossec_host_alert_counters\x18\x0b \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\x12.\n\x13openflow_flow_stats\x18\x0c \x03(\x0b\x32\x11.FlowStatisticDTO\x12.\n\x13openflow_port_stats\x18\r \x03(\x0b\x32\x11.PortStatisticDTO\x12\x35\n\x17\x61vg_openflow_flow_stats\x18\x0e \x03(\x0b\x32\x14.AvgFlowStatisticDTO\x12\x35\n\x17\x61vg_openflow_port_stats\x18\x0f \x03(\x0b\x32\x14.AvgPortStatisticDTO\x12<\n openflow_flow_metrics_per_switch\x18\x10 \x03(\x0b\x32\x12.FlowStatisticDict\x12<\n openflow_port_metrics_per_switch\x18\x11 \x03(\x0b\x32\x12.PortStatisticDict\x12\x43\n$openflow_flow_avg_metrics_per_switch\x18\x12 \x03(\x0b\x32\x15.AvgFlowStatisticDict\x12\x43\n$openflow_port_avg_metrics_per_switch\x18\x13 \x03(\x0b\x32\x15.AvgPortStatisticDict\x12\x43\n$agg_openflow_flow_metrics_per_switch\x18\x14 \x03(\x0b\x32\x15.AggFlowStatisticDict\x12\x35\n\x17\x61gg_openflow_flow_stats\x18\x15 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgPortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgPortStatisticDTO\"G\n\x14\x41ggFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgFlowStatisticDTO\"A\n\x11PortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.PortStatisticDTO\"A\n\x11\x46lowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.FlowStatisticDTO\"Q\n\x19OSSECIdsAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\"A\n\x0fHostMetricsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x13.HostMetricsDataDTO\"=\n\x0f\x44ockerStatsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\"\xbc\x04\n\x13\x41vgPortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\"\n\x1atotal_num_received_packets\x18\x03 \x01(\x05\x12 \n\x18total_num_received_bytes\x18\x04 \x01(\x05\x12!\n\x19total_num_received_errors\x18\x05 \x01(\x05\x12%\n\x1dtotal_num_transmitted_packets\x18\x06 \x01(\x05\x12#\n\x1btotal_num_transmitted_bytes\x18\x07 \x01(\x05\x12$\n\x1ctotal_num_transmitted_errors\x18\x08 \x01(\x05\x12\"\n\x1atotal_num_received_dropped\x18\t \x01(\x05\x12%\n\x1dtotal_num_transmitted_dropped\x18\n \x01(\x05\x12\'\n\x1ftotal_num_received_frame_errors\x18\x0b \x01(\x05\x12)\n!total_num_received_overrun_errors\x18\x0c \x01(\x05\x12%\n\x1dtotal_num_received_crc_errors\x18\r \x01(\x05\x12\x1c\n\x14total_num_collisions\x18\x0e \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x0f \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x10 \x01(\x05\"\x8f\x02\n\x13\x41vgFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x05 \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x06 \x01(\x05\x12\x18\n\x10\x61vg_hard_timeout\x18\x07 \x01(\x05\x12\x18\n\x10\x61vg_idle_timeout\x18\x08 \x01(\x05\x12\x14\n\x0c\x61vg_priority\x18\t \x01(\x05\x12\x12\n\navg_cookie\x18\n \x01(\x05\"\x8a\x01\n\x13\x41ggFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12\x17\n\x0ftotal_num_flows\x18\x05 \x01(\x05\"\xf7\x03\n\x10PortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x1c\n\x14num_received_packets\x18\x04 \x01(\x05\x12\x1a\n\x12num_received_bytes\x18\x05 \x01(\x05\x12\x1b\n\x13num_received_errors\x18\x06 \x01(\x05\x12\x1f\n\x17num_transmitted_packets\x18\x07 \x01(\x05\x12\x1d\n\x15num_transmitted_bytes\x18\x08 \x01(\x05\x12\x1e\n\x16num_transmitted_errors\x18\t \x01(\x05\x12\x1c\n\x14num_received_dropped\x18\n \x01(\x05\x12\x1f\n\x17num_transmitted_dropped\x18\x0b \x01(\x05\x12!\n\x19num_received_frame_errors\x18\x0c \x01(\x05\x12#\n\x1bnum_received_overrun_errors\x18\r \x01(\x05\x12\x1f\n\x17num_received_crc_errors\x18\x0e \x01(\x05\x12\x16\n\x0enum_collisions\x18\x0f \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x10 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x11 \x01(\x05\"\xa4\x02\n\x10\x46lowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0f\n\x07in_port\x18\x03 \x01(\x05\x12\x10\n\x08out_port\x18\x04 \x01(\x05\x12\x17\n\x0f\x64st_mac_address\x18\x05 \x01(\t\x12\x13\n\x0bnum_packets\x18\x06 \x01(\x05\x12\x11\n\tnum_bytes\x18\x07 \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x08 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\t \x01(\x05\x12\x14\n\x0chard_timeout\x18\n \x01(\x05\x12\x14\n\x0cidle_timeout\x18\x0b \x01(\x05\x12\x10\n\x08priority\x18\x0c \x01(\x05\x12\x0e\n\x06\x63ookie\x18\r \x01(\x05\"\xc5\x01\n\x18OSSECIdsAlertCountersDTO\x12\x14\n\x0clevel_alerts\x18\x01 \x03(\x05\x12\x14\n\x0cgroup_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12\x14\n\x0ctotal_alerts\x18\x05 \x01(\x05\x12 \n\x18\x61lerts_weighted_by_level\x18\x06 \x01(\x02\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xb5\x01\n\x18SnortIdsAlertCountersDTO\x12\x17\n\x0fpriority_alerts\x18\x01 \x03(\x05\x12\x14\n\x0c\x63lass_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18\x05 \x01(\x02\x12\n\n\x02ip\x18\x06 \x01(\t\x12\n\n\x02ts\x18\x07 \x01(\x02\"\xf4\x01\n\x1a\x45mulationAttackerActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\x12\x15\n\rvulnerability\x18\x0c \x01(\t\x12\x10\n\x08\x62\x61\x63kdoor\x18\r \x01(\x08\"\xcb\x01\n\x1a\x45mulationDefenderActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\"\xce\x01\n\x12HostMetricsDataDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xf8\x01\n\x0e\x44ockerStatsDTO\x12\x0c\n\x04pids\x18\x01 \x01(\x02\x12\x11\n\ttimestamp\x18\x02 \x01(\t\x12\x13\n\x0b\x63pu_percent\x18\x03 \x01(\x02\x12\x13\n\x0bmem_current\x18\x04 \x01(\x02\x12\x11\n\tmem_total\x18\x05 \x01(\x02\x12\x13\n\x0bmem_percent\x18\x06 \x01(\x02\x12\x10\n\x08\x62lk_read\x18\x07 \x01(\x02\x12\x11\n\tblk_write\x18\x08 \x01(\x02\x12\x0e\n\x06net_rx\x18\t \x01(\x02\x12\x0e\n\x06net_tx\x18\n \x01(\x02\x12\x16\n\x0e\x63ontainer_name\x18\x0b \x01(\t\x12\n\n\x02ip\x18\x0c \x01(\t\x12\n\n\x02ts\x18\r \x01(\x02\"W\n\x1a\x43lientPopulationMetricsDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\n\n\x02ts\x18\x02 \x01(\x02\x12\x13\n\x0bnum_clients\x18\x03 \x01(\x05\x12\x0c\n\x04rate\x18\x04 \x01(\x02\"\x1a\n\x18GetClusterManagerLogsMsg\"S\n\x13GetContainerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17GetClientManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetKafkaManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fGetKafkaLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12GetSnortIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetSnortIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetOSSECIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"R\n\x12GetOSSECIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"U\n\x15GetHostManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18GetTrafficManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14GetElkManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"8\n\rGetElkLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14GetRyuManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetRyuControllerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StopHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StopHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"@\n\x15RemoveKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15\x43reateKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14ListKibanaTunnelsMsg\"5\n\x10KibanaTunnelsDTO\x12!\n\x07tunnels\x18\x01 \x03(\x0b\x32\x10.KibanaTunnelDTO\"T\n\x0fKibanaTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"=\n\x12RemoveRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12\x43reateRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x13\n\x11ListRyuTunnelsMsg\"/\n\rRyuTunnelsDTO\x12\x1e\n\x07tunnels\x18\x01 \x03(\x0b\x32\r.RyuTunnelDTO\"Q\n\x0cRyuTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"P\n SnortIdsMonitorThreadStatusesDTO\x12,\n\x10snortIDSStatuses\x18\x01 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"E\n\x1aGetSnortIdsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"N\n#GetSnortIdsMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16StopSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StartSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17StopSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"M\n\rStartSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"I\n\x1eStartSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"L\n\x0cStopSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\\\n\x1cStopSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"J\n\x1fStopSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetRyuManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StopRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetRyuServiceStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aGetOSSECIDSManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n OSSECIdsMonitorThreadStatusesDTO\x12,\n\x10ossecIDSStatuses\x18\x01 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"N\n#GetOSSECIDSMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopOSSECIDSMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\\\n\x1cStopOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StopOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"T\n\x14StartOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14StopOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n\x10StartOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"=\n\x12StartOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetKafkaManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StartKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18GetKafkaManagerStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateKafkaTopicsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StopKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetHostManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n GetHostMonitorThreadsStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16\x41pplyFileBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyPacketBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyMetricBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17\x41pplyHeartBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"P\n\x10StopHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"f\n\x10StartFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"g\n\x11StartHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"Y\n\x19StartHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopHeartbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopPacketbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StopFilebeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopMetricbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStartHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12StopHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StartHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\">\n\x13StopHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xad\x05\n\x10\x45xecutionInfoDTO\x12\x15\n\remulationName\x18\x01 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x02 \x01(\x05\x12\x36\n\x14snortIdsManagersInfo\x18\x03 \x01(\x0b\x32\x18.SnortIdsManagersInfoDTO\x12\x36\n\x14ossecIdsManagersInfo\x18\x04 \x01(\x0b\x32\x18.OSSECIdsManagersInfoDTO\x12\x30\n\x11kafkaManagersInfo\x18\x05 \x01(\x0b\x32\x15.KafkaManagersInfoDTO\x12.\n\x10hostManagersInfo\x18\x06 \x01(\x0b\x32\x14.HostManagersInfoDTO\x12\x32\n\x12\x63lientManagersInfo\x18\x07 \x01(\x0b\x32\x16.ClientManagersInfoDTO\x12<\n\x17\x64ockerStatsManagersInfo\x18\x08 \x01(\x0b\x32\x1b.DockerStatsManagersInfoDTO\x12\x30\n\x11runningContainers\x18\t \x01(\x0b\x32\x15.RunningContainersDTO\x12\x30\n\x11stoppedContainers\x18\n \x01(\x0b\x32\x15.StoppedContainersDTO\x12\x37\n\x16trafficManagersInfoDTO\x18\x0b \x01(\x0b\x32\x17.TrafficManagersInfoDTO\x12*\n\x0e\x61\x63tiveNetworks\x18\x0c \x01(\x0b\x32\x12.DockerNetworksDTO\x12/\n\x12\x65lkManagersInfoDTO\x18\r \x01(\x0b\x32\x13.ElkManagersInfoDTO\x12/\n\x12ryuManagersInfoDTO\x18\x0e \x01(\x0b\x32\x13.RyuManagersInfoDTO\"\xab\x01\n\x12RyuManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12ryuManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x13ryuManagersStatuses\x18\x06 \x03(\x0b\x32\x14.RyuManagerStatusDTO\"\xb4\x01\n\x13RyuManagerStatusDTO\x12\x13\n\x0bryu_running\x18\x01 \x01(\x08\x12\x17\n\x0fmonitor_running\x18\x02 \x01(\x08\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x10\n\x08web_port\x18\x04 \x01(\x05\x12\x12\n\ncontroller\x18\x05 \x01(\t\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x15\n\rtime_step_len\x18\x08 \x01(\x05\"\xaf\x01\n\x13HostManagersInfoDTO\x12\x0b\n\x03ips\x18\x15 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1b\n\x13hostManagersRunning\x18\x05 \x03(\x08\x12\x33\n\x14hostManagersStatuses\x18\x06 \x03(\x0b\x32\x15.HostManagerStatusDTO\"L\n\x16HostManagerStatusesDTO\x12\x32\n\x13hostManagerStatuses\x18\x01 \x03(\x0b\x32\x15.HostManagerStatusDTO\"\xa8\x01\n\x14HostManagerStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\x12\n\n\x02ip\x18\x06 \x01(\t\"\xac\x01\n\x14KafkaManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1c\n\x14kafkaManagersRunning\x18\x05 \x03(\x08\x12.\n\x15kafkaManagersStatuses\x18\x06 \x03(\x0b\x32\x0f.KafkaStatusDTO\"1\n\x0eKafkaStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06topics\x18\x02 \x03(\t\"\xb8\x01\n\x17OSSECIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17ossecIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18ossecIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"G\n\x11OSSECIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11ossec_ids_running\x18\x02 \x01(\x08\"\xb8\x01\n\x17SnortIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17snortIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18snortIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"G\n\x11SnortIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\">\n\x13GetExecutionInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStopContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"y\n\x0fRunContainerMsg\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x10\n\x08num_cpus\x18\x04 \x01(\x05\x12\x16\n\x0e\x63reate_network\x18\x05 \x01(\x08\x12\x0f\n\x07version\x18\x06 \x01(\t\"H\n\x1dStartContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetElkManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xbd\x01\n\x12\x45lkManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12\x65lkManagersRunning\x18\x05 \x03(\x08\x12*\n\x13\x65lkManagersStatuses\x18\x06 \x03(\x0b\x32\r.ElkStatusDTO\x12\x17\n\x0flocalKibanaPort\x18\x07 \x01(\x05\"A\n\x16StopLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StopElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StartElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fStopElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x0c\x45lkStatusDTO\x12\x16\n\x0e\x65lasticRunning\x18\x01 \x01(\x08\x12\x15\n\rkibanaRunning\x18\x02 \x01(\x08\x12\x17\n\x0flogstashRunning\x18\x03 \x01(\x08\"?\n\x14GetElkStackStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dGetDockerStatsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xcb\x01\n\x1a\x44ockerStatsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\"\n\x1a\x64ockerStatsManagersRunning\x18\x05 \x03(\x08\x12\x41\n\x1b\x64ockerStatsManagersStatuses\x18\x06 \x03(\x0b\x32\x1c.DockerStatsMonitorStatusDTO\"\x1c\n\x1aRemoveAllDockerNetworksMsg\"+\n\x17RemoveDockerNetworksMsg\x12\x10\n\x08networks\x18\x01 \x03(\t\"e\n\x1b\x44ockerStatsMonitorStatusDTO\x12\x14\n\x0cnum_monitors\x18\x01 \x01(\x05\x12\x12\n\nemulations\x18\x02 \x03(\t\x12\x1c\n\x14\x65mulation_executions\x18\x03 \x03(\x05\".\n\x1eGetDockerStatsManagerStatusMsg\x12\x0c\n\x04port\x18\x01 \x01(\x05\"J\n\x1fStopDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x43reateEmulationNetworksMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x1d\n\x1bListAllStoppedContainersMsg\"F\n\x14StoppedContainersDTO\x12.\n\x11stoppedContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"\x1d\n\x1bListAllRunningEmulationsMsg\"1\n\x14RunningEmulationsDTO\x12\x19\n\x11runningEmulations\x18\x01 \x03(\t\"\x1d\n\x1bListAllRunningContainersMsg\"F\n\x14RunningContainersDTO\x12.\n\x11runningContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"=\n\x12\x44ockerContainerDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05image\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"!\n\x11StartContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1e\n\x1cStartAllStoppedContainersMsg\"\x1a\n\x18ListAllDockerNetworksMsg\":\n\x11\x44ockerNetworksDTO\x12\x10\n\x08networks\x18\x01 \x03(\t\x12\x13\n\x0bnetwork_ids\x18\x02 \x03(\x05\"8\n\x12\x43ontainerImagesDTO\x12\"\n\x06images\x18\x01 \x03(\x0b\x32\x12.ContainerImageDTO\"f\n\x11\x43ontainerImageDTO\x12\x10\n\x08repoTags\x18\x01 \x01(\t\x12\x0f\n\x07\x63reated\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x03\"\x1b\n\x19ListAllContainerImagesMsg\"\'\n\x17RemoveContainerImageMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bRemoveAllContainerImagesMsg\"\x1f\n\x1dRemoveAllStoppedContainersMsg\"\"\n\x12RemoveContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x10StopContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bStopAllRunningContainersMsg\"D\n\x19GetTrafficManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xb9\x01\n\x16TrafficManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1e\n\x16trafficManagersRunning\x18\x05 \x03(\x08\x12\x37\n\x17trafficManagersStatuses\x18\x06 \x03(\x0b\x32\x16.TrafficManagerInfoDTO\"8\n\x15TrafficManagerInfoDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06script\x18\x02 \x01(\t\"\xb1\x01\n\x15\x43lientManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1d\n\x15\x63lientManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x16\x63lientManagersStatuses\x18\x06 \x03(\x0b\x32\x11.GetNumClientsDTO\"C\n\x18GetClientManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StartTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StopTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"C\n\x18StopTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xae\x01\n\x10GetNumClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\"A\n\x16GetNumActiveClientsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StopTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"U\n\x15StopTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"V\n\x16StartTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\x17\n\x15\x43leanAllExecutionsMsg\"\x16\n\x14StopAllExecutionsMsg\";\n\x10StopExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43leanExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"4\n\x1fStopAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"5\n CleanAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"\x14\n\x12GetCsleLogFilesMsg\"\x1d\n\rGetLogFileMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"H\n\x1dStartContainersInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"S\n(AttachContainersToNetworksInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13InstallLibrariesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13\x41pplyKafkaConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartSdnControllerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x41pplyResouceConstraintsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateOvsSwitchesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10PingExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0f\x43onfigureOvsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStartSdnControllerMonitorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateUsersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateVulnsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateFlagsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43reateTopologyMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"F\n\x1bStartKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStopKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartOSSECIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartOSSECIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StartElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17\x41pplyFileBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyPacketBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyMetricBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18\x41pplyHeartBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x11StartFileBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartPacketBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartMetricBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"S\n\x12StartHeartBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"\x1e\n\x1cGetDockerStatsManagerLogsMsg\"\x16\n\x14GetPrometheusLogsMsg\"\x18\n\x16GetNodeExporterLogsMsg\"\x14\n\x12GetCAdvisorLogsMsg\"\x13\n\x11GetPgAdminLogsMsg\"\x13\n\x11GetGrafanaLogsMsg\"\x11\n\x0fGetNginxLogsMsg\"\x12\n\x10GetDockerLogsMsg\"\x16\n\x14GetPostgreSQLLogsMsg\"\x11\n\x0fGetFlaskLogsMsg\"\x17\n\x07LogsDTO\x12\x0c\n\x04logs\x18\x01 \x03(\t\"&\n\x13OperationOutcomeDTO\x12\x0f\n\x07outcome\x18\x01 \x01(\x08\"\x12\n\x10GetNodeStatusMsg\"\xb3\x02\n\rNodeStatusDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0e\n\x06leader\x18\x02 \x01(\x08\x12\x17\n\x0f\x63\x41\x64visorRunning\x18\x03 \x01(\x08\x12\x19\n\x11prometheusRunning\x18\x04 \x01(\x08\x12\x16\n\x0egrafanaRunning\x18\x05 \x01(\x08\x12\x16\n\x0epgAdminRunning\x18\x06 \x01(\x08\x12\x14\n\x0cnginxRunning\x18\x07 \x01(\x08\x12\x14\n\x0c\x66laskRunning\x18\x08 \x01(\x08\x12!\n\x19\x64ockerStatsManagerRunning\x18\t \x01(\x08\x12\x1b\n\x13nodeExporterRunning\x18\n \x01(\x08\x12\x19\n\x11postgreSQLRunning\x18\x0b \x01(\x08\x12\x1b\n\x13\x64ockerEngineRunning\x18\x0c \x01(\x08\"#\n\x10ServiceStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\"\x14\n\x12StartPostgreSQLMsg\"\x12\n\x10StartCAdvisorMsg\"\x16\n\x14StartNodeExporterMsg\"\x11\n\x0fStartGrafanaMsg\"\x14\n\x12StartPrometheusMsg\"\x11\n\x0fStartPgAdminMsg\"\x0f\n\rStartNginxMsg\"\x0f\n\rStartFlaskMsg\"\x1c\n\x1aStartDockerStatsManagerMsg\"K\n StartDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14StartDockerEngineMsg\"\x13\n\x11StopPostgreSQLMsg\"\x11\n\x0fStopCAdvisorMsg\"\x15\n\x13StopNodeExporterMsg\"\x10\n\x0eStopGrafanaMsg\"\x13\n\x11StopPrometheusMsg\"\x10\n\x0eStopPgAdminMsg\"\x0e\n\x0cStopNginxMsg\"\x0e\n\x0cStopFlaskMsg\"\x1b\n\x19StopDockerStatsManagerMsg\"\x15\n\x13StopDockerEngineMsg2\xd7o\n\x0e\x43lusterManager\x12\x34\n\rgetNodeStatus\x12\x11.GetNodeStatusMsg\x1a\x0e.NodeStatusDTO\"\x00\x12;\n\x0fstartPostgreSQL\x12\x13.StartPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x37\n\rstartCAdvisor\x12\x11.StartCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startNodeExporter\x12\x15.StartNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartGrafana\x12\x10.StartGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12;\n\x0fstartPrometheus\x12\x13.StartPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartPgAdmin\x12\x10.StartPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartNginx\x12\x0e.StartNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartFlask\x12\x0e.StartFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12K\n\x17startDockerStatsManager\x12\x1b.StartDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12W\n\x1dstartDockerStatsManagerThread\x12!.StartDockerStatsManagerThreadMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startDockerEngine\x12\x15.StartDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPostgreSQL\x12\x12.StopPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstopCAdvisor\x12\x10.StopCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopNodeExporter\x12\x14.StopNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopGrafana\x12\x0f.StopGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPrometheus\x12\x12.StopPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopPgAdmin\x12\x0f.StopPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopNginx\x12\r.StopNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopFlask\x12\r.StopFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12I\n\x16stopDockerStatsManager\x12\x1a.StopDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopDockerEngine\x12\x14.StopDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x32\n\x0fgetCsleLogFiles\x12\x13.GetCsleLogFilesMsg\x1a\x08.LogsDTO\"\x00\x12\x46\n\x19getDockerStatsManagerLogs\x12\x1d.GetDockerStatsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getPrometheusLogs\x12\x15.GetPrometheusLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getNodeExporterLogs\x12\x17.GetNodeExporterLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetCadvisorLogs\x12\x13.GetCAdvisorLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetPgAdminLogs\x12\x12.GetPgAdminLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetGrafanaLogs\x12\x12.GetGrafanaLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetNginxLogs\x12\x10.GetNginxLogsMsg\x1a\x08.LogsDTO\"\x00\x12.\n\rgetDockerLogs\x12\x11.GetDockerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x37\n\x12getPostrgreSQLLogs\x12\x15.GetPostgreSQLLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetFlaskLogs\x12\x10.GetFlaskLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetLogFile\x12\x0e.GetLogFileMsg\x1a\x08.LogsDTO\"\x00\x12T\n\x1astartContainersInExecution\x12\x1e.StartContainersInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12j\n%attachContainersInExecutionToNetworks\x12).AttachContainersToNetworksInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10installLibraries\x12\x14.InstallLibrariesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10\x61pplyKafkaConfig\x12\x14.ApplyKafkaConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startSdnController\x12\x16.StartSdnControllerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12O\n\x18\x61pplyResourceConstraints\x12\x1b.ApplyResouceConstraintsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateOvsSwitches\x12\x15.CreateOvsSwitchesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rpingExecution\x12\x11.PingExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0c\x63onfigureOvs\x12\x10.ConfigureOvsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19startSdnControllerMonitor\x12\x1d.StartSdnControllerMonitorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateUsers\x12\x0f.CreateUsersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x15\x63reateVulnerabilities\x12\x0f.CreateVulnsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateFlags\x12\x0f.CreateFlagsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63reateTopology\x12\x12.CreateTopologyMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startTrafficGenerators\x12\x1a.StartTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startClientPopulation\x12\x19.StartClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18startKafkaClientProducer\x12\x1c.StartKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17stopKafkaClientProducer\x12\x1b.StopKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartSnortIdses\x12\x13.StartSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartSnortIdsesMonitorThreads\x12!.StartSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOssecIdses\x12\x13.StartOSSECIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartOssecIdsesMonitorThreads\x12!.StartOSSECIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartElkStack\x12\x11.StartElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startHostManagers\x12\x15.StartHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyFileBeatsConfig\x12\x18.ApplyFileBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyPacketBeatsConfig\x12\x1a.ApplyPacketBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyMetricBeatsConfig\x12\x1a.ApplyMetricBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyHeartBeatsConfig\x12\x19.ApplyHeartBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartFilebeats\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startPacketbeats\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startMetricbeats\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartHeartbeats\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopAllExecutionsOfEmulation\x12 .StopAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopExecution\x12\x11.StopExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopAllExecutions\x12\x15.StopAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12\x63leanAllExecutions\x12\x16.CleanAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1d\x63leanAllExecutionsOfEmulation\x12!.CleanAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63leanExecution\x12\x12.CleanExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13startTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x12stopTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x13stopTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startClientManager\x12\x16.StartClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopClientPopulation\x12\x18.StopClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopClientManager\x12\x15.StopClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13getNumActiveClients\x12\x17.GetNumActiveClientsMsg\x1a\x11.GetNumClientsDTO\"\x00\x12J\n\x15startTrafficGenerator\x12\x19.StartTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopTrafficGenerators\x12\x19.StopTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopTrafficGenerator\x12\x18.StopTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x15getClientManagersInfo\x12\x19.GetClientManagersInfoMsg\x1a\x16.ClientManagersInfoDTO\"\x00\x12N\n\x16getTrafficManagersInfo\x12\x1a.GetTrafficManagersInfoMsg\x1a\x16.TrafficManagerInfoDTO\"\x00\x12P\n\x18stopAllRunningContainers\x12\x1c.StopAllRunningContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopContainer\x12\x11.StopContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1aremoveAllStoppedContainers\x12\x1e.RemoveAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveContainer\x12\x13.RemoveContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18removeAllContainerImages\x12\x1c.RemoveAllContainerImagesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14removeContainerImage\x12\x18.RemoveContainerImageMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12K\n\x16listAllContainerImages\x12\x1a.ListAllContainerImagesMsg\x1a\x13.ContainerImagesDTO\"\x00\x12H\n\x15listAllDockerNetworks\x12\x19.ListAllDockerNetworksMsg\x1a\x12.DockerNetworksDTO\"\x00\x12R\n\x19startAllStoppedContainers\x12\x1d.StartAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartContainer\x12\x12.StartContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Q\n\x18listAllRunningContainers\x12\x1c.ListAllRunningContainersMsg\x1a\x15.RunningContainersDTO\"\x00\x12Q\n\x18listAllRunningEmulations\x12\x1c.ListAllRunningEmulationsMsg\x1a\x15.RunningEmulationsDTO\"\x00\x12Q\n\x18listAllStoppedContainers\x12\x1c.ListAllStoppedContainersMsg\x1a\x15.StoppedContainersDTO\"\x00\x12N\n\x17\x63reateEmulationNetworks\x12\x1b.CreateEmulationNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopDockerStatsManagerThread\x12 .StopDockerStatsManagerThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12^\n\x1bgetDockerStatsManagerStatus\x12\x1f.GetDockerStatsManagerStatusMsg\x1a\x1c.DockerStatsMonitorStatusDTO\"\x00\x12H\n\x14removeDockerNetworks\x12\x18.RemoveDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17removeAllDockerNetworks\x12\x1b.RemoveAllDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12[\n\x1agetDockerStatsManagersInfo\x12\x1e.GetDockerStatsManagersInfoMsg\x1a\x1b.DockerStatsManagersInfoDTO\"\x00\x12>\n\x0fstartElkManager\x12\x13.StartElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopElkManager\x12\x12.StopElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0cgetElkStatus\x12\x15.GetElkStackStatusMsg\x1a\r.ElkStatusDTO\"\x00\x12\x38\n\x0cstopElkStack\x12\x10.StopElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstartElastic\x12\x17.StartElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstopElastic\x12\x16.StopElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstartKibana\x12\x16.StartKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\nstopKibana\x12\x15.StopKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x41\n\rstartLogstash\x12\x18.StartLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstopLogstash\x12\x17.StopLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getElkManagersInfo\x12\x16.GetElkManagersInfoMsg\x1a\x13.ElkManagersInfoDTO\"\x00\x12T\n\x1astartContainersOfExecution\x12\x1e.StartContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0crunContainer\x12\x10.RunContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopContainersOfExecution\x12\x1d.StopContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startHostManager\x12\x14.StartHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10stopHostManagers\x12\x14.StopHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopHostManager\x12\x13.StopHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopFilebeats\x12\x11.StopFilebeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopPacketbeats\x12\x13.StopPacketbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopMetricbeats\x12\x13.StopMetricbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopHeartbeats\x12\x12.StopHeartbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17startHostMonitorThreads\x12\x1b.StartHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startHostMonitorThread\x12\x1a.StartHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\rstartFilebeat\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartPacketbeat\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartMetricbeat\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0estartHeartbeat\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopFilebeat\x12\x10.StopFileBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopPacketbeat\x12\x12.StopPacketBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopMetricbeat\x12\x12.StopMetricBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopHeartbeat\x12\x11.StopHeartBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13\x61pplyFileBeatConfig\x12\x17.ApplyFileBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyPacketBeatConfig\x12\x19.ApplyPacketBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyMetricBeatConfig\x12\x19.ApplyMetricBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyHeartBeatConfig\x12\x18.ApplyHeartBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12]\n\x1dgetHostMonitorThreadsStatuses\x12!.GetHostMonitorThreadsStatusesMsg\x1a\x17.HostManagerStatusesDTO\"\x00\x12\x46\n\x13getHostManagersInfo\x12\x17.GetHostManagersInfoMsg\x1a\x14.HostManagersInfoDTO\"\x00\x12@\n\x10stopKafkaManager\x12\x14.StopKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startKafkaManager\x12\x15.StartKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateKafkaTopics\x12\x15.CreateKafkaTopicsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0egetKafkaStatus\x12\x19.GetKafkaManagerStatusMsg\x1a\x0f.KafkaStatusDTO\"\x00\x12>\n\x0fstopKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x10startKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12I\n\x14getKafkaManagersInfo\x12\x18.GetKafkaManagersInfoMsg\x1a\x15.KafkaManagersInfoDTO\"\x00\x12<\n\x0estopOSSECIDSes\x12\x12.StopOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOSSECIDSes\x12\x13.StartOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopOSSECIDS\x12\x10.StopOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartOSSECIDS\x12\x11.StartOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x15startOSSECIDSManagers\x12\x16.StartOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14stopOSSECIDSManagers\x12\x15.StopOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14startOSSECIDSManager\x12\x15.StartOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13stopOSSECIDSManager\x12\x14.StopOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartOSSECIDSMonitorThread\x12\x1e.StartOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopOSSECIDSMonitorThread\x12\x1d.StopOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopOSSECIDSMonitorThreads\x12\x1e.StopOSSECIDSMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getOSSECIDSMonitorThreadStatuses\x12$.GetOSSECIDSMonitorThreadStatusesMsg\x1a!.OSSECIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getOSSECIdsManagersInfo\x12\x1b.GetOSSECIDSManagersInfoMsg\x1a\x18.OSSECIdsManagersInfoDTO\"\x00\x12>\n\x0fstartRyuManager\x12\x13.StartRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopRyuManager\x12\x12.StopRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cgetRyuStatus\x12\x17.GetRyuServiceStatusMsg\x1a\x14.RyuManagerStatusDTO\"\x00\x12\x37\n\x08startRyu\x12\x13.StartRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x07stopRyu\x12\x12.StopRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getRyuManagersInfo\x12\x16.GetRyuManagersInfoMsg\x1a\x13.RyuManagersInfoDTO\"\x00\x12<\n\x0estopSnortIdses\x12\x12.StopSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopSnortIdsesMonitorThreads\x12 .StopSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x0cstopSnortIds\x12\r.StopSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopSnortIdsMonitorThread\x12\x1d.StopSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x37\n\rstartSnortIds\x12\x0e.StartSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12V\n\x1bstartSnortIdsMonitorThreads\x12\x1f.StartSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartSnortIdsMonitorThread\x12\x1e.StartSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startSnortIdsManagers\x12\x19.StartSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopSnortIdsManagers\x12\x18.StopSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startSnortIdsManager\x12\x18.StartSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13stopSnortIdsManager\x12\x17.StopSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopSnortIdsMonitorThreads\x12\x1e.StopSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getSnortIdsMonitorThreadStatuses\x12$.GetSnortIdsMonitorThreadStatusesMsg\x1a!.SnortIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getSnortIdsManagersInfo\x12\x1b.GetSnortIdsManagersInfoMsg\x1a\x18.SnortIdsManagersInfoDTO\"\x00\x12=\n\x10getExecutionInfo\x12\x14.GetExecutionInfoMsg\x1a\x11.ExecutionInfoDTO\"\x00\x12?\n\x11listKibanaTunnels\x12\x15.ListKibanaTunnelsMsg\x1a\x11.KibanaTunnelsDTO\"\x00\x12\x44\n\x12\x63reateKibanaTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0elistRyuTunnels\x12\x12.ListRyuTunnelsMsg\x1a\x0e.RyuTunnelsDTO\"\x00\x12\x41\n\x0f\x63reateRyuTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12removeKibanaTunnel\x12\x16.RemoveKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveRyuTunnel\x12\x13.RemoveRyuTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16stopHostMonitorThreads\x12\x1a.StopHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopHostMonitorThread\x12\x19.StopHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x0fstartRyuMonitor\x12\x19.StartRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x0estopRyuMonitor\x12\x18.StopRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x14getRyuControllerLogs\x12\x18.GetRyuControllerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getRyuManagerLogs\x12\x15.GetRyuManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetElkLogs\x12\x0e.GetElkLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getElkManagerLogs\x12\x15.GetElkManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getTrafficManagerLogs\x12\x19.GetTrafficManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x38\n\x12getHostManagerLogs\x12\x16.GetHostManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetOSSECIdsLogs\x12\x13.GetOSSECIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getOSSECIdsManagerLogsMsg\x12\x1a.GetOSSECIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetSnortIdsLogs\x12\x13.GetSnortIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getSnortIdsManagerLogsMsg\x12\x1a.GetSnortIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetKafkaLogs\x12\x10.GetKafkaLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getKafkaManagerLogs\x12\x17.GetKafkaManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12?\n\x17getClientManagerLogsMsg\x12\x18.GetClientManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x34\n\x10getContainerLogs\x12\x14.GetContainerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getClusterManagerLogs\x12\x19.GetClusterManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12^\n\x1agetExecutionTimeSeriesData\x12\x1e.GetExecutionTimeSeriesDataMsg\x1a\x1e.EmulationMetricsTimeSeriesDTO\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x63luster_manager.proto\"Y\n\x1dGetExecutionTimeSeriesDataMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x0f\n\x07minutes\x18\x03 \x01(\x05\"\xa3\t\n\x1d\x45mulationMetricsTimeSeriesDTO\x12\x33\n\x0e\x63lient_metrics\x18\x01 \x03(\x0b\x32\x1b.ClientPopulationMetricsDTO\x12\x30\n\x17\x61ggregated_docker_stats\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\x12+\n\x11\x64ocker_host_stats\x18\x03 \x03(\x0b\x32\x10.DockerStatsDict\x12&\n\x0chost_metrics\x18\x04 \x03(\x0b\x32\x10.HostMetricsDict\x12\x34\n\x17\x61ggregated_host_metrics\x18\x05 \x03(\x0b\x32\x13.HostMetricsDataDTO\x12\x35\n\x10\x64\x65\x66\x65nder_actions\x18\x06 \x03(\x0b\x32\x1b.EmulationDefenderActionDTO\x12\x35\n\x10\x61ttacker_actions\x18\x07 \x03(\x0b\x32\x1b.EmulationAttackerActionDTO\x12\x34\n\x11snort_ids_metrics\x18\x08 \x03(\x0b\x32\x19.SnortIdsAlertCountersDTO\x12\x14\n\x0c\x65mulation_id\x18\t \x01(\x05\x12=\n\x19ossec_host_alert_counters\x18\n \x03(\x0b\x32\x1a.OSSECIdsAlertCountersDict\x12G\n$aggregated_ossec_host_alert_counters\x18\x0b \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\x12.\n\x13openflow_flow_stats\x18\x0c \x03(\x0b\x32\x11.FlowStatisticDTO\x12.\n\x13openflow_port_stats\x18\r \x03(\x0b\x32\x11.PortStatisticDTO\x12\x35\n\x17\x61vg_openflow_flow_stats\x18\x0e \x03(\x0b\x32\x14.AvgFlowStatisticDTO\x12\x35\n\x17\x61vg_openflow_port_stats\x18\x0f \x03(\x0b\x32\x14.AvgPortStatisticDTO\x12<\n openflow_flow_metrics_per_switch\x18\x10 \x03(\x0b\x32\x12.FlowStatisticDict\x12<\n openflow_port_metrics_per_switch\x18\x11 \x03(\x0b\x32\x12.PortStatisticDict\x12\x43\n$openflow_flow_avg_metrics_per_switch\x18\x12 \x03(\x0b\x32\x15.AvgFlowStatisticDict\x12\x43\n$openflow_port_avg_metrics_per_switch\x18\x13 \x03(\x0b\x32\x15.AvgPortStatisticDict\x12\x43\n$agg_openflow_flow_metrics_per_switch\x18\x14 \x03(\x0b\x32\x15.AggFlowStatisticDict\x12\x35\n\x17\x61gg_openflow_flow_stats\x18\x15 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgPortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgPortStatisticDTO\"G\n\x14\x41ggFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AggFlowStatisticDTO\"G\n\x14\x41vgFlowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x14.AvgFlowStatisticDTO\"A\n\x11PortStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.PortStatisticDTO\"A\n\x11\x46lowStatisticDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x11.FlowStatisticDTO\"Q\n\x19OSSECIdsAlertCountersDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x19.OSSECIdsAlertCountersDTO\"A\n\x0fHostMetricsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x13.HostMetricsDataDTO\"=\n\x0f\x44ockerStatsDict\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x04\x64tos\x18\x02 \x03(\x0b\x32\x0f.DockerStatsDTO\"\xbc\x04\n\x13\x41vgPortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\"\n\x1atotal_num_received_packets\x18\x03 \x01(\x05\x12 \n\x18total_num_received_bytes\x18\x04 \x01(\x05\x12!\n\x19total_num_received_errors\x18\x05 \x01(\x05\x12%\n\x1dtotal_num_transmitted_packets\x18\x06 \x01(\x05\x12#\n\x1btotal_num_transmitted_bytes\x18\x07 \x01(\x05\x12$\n\x1ctotal_num_transmitted_errors\x18\x08 \x01(\x05\x12\"\n\x1atotal_num_received_dropped\x18\t \x01(\x05\x12%\n\x1dtotal_num_transmitted_dropped\x18\n \x01(\x05\x12\'\n\x1ftotal_num_received_frame_errors\x18\x0b \x01(\x05\x12)\n!total_num_received_overrun_errors\x18\x0c \x01(\x05\x12%\n\x1dtotal_num_received_crc_errors\x18\r \x01(\x05\x12\x1c\n\x14total_num_collisions\x18\x0e \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x0f \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x10 \x01(\x05\"\x8f\x02\n\x13\x41vgFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12 \n\x18\x61vg_duration_nanoseconds\x18\x05 \x01(\x05\x12\x1c\n\x14\x61vg_duration_seconds\x18\x06 \x01(\x05\x12\x18\n\x10\x61vg_hard_timeout\x18\x07 \x01(\x05\x12\x18\n\x10\x61vg_idle_timeout\x18\x08 \x01(\x05\x12\x14\n\x0c\x61vg_priority\x18\t \x01(\x05\x12\x12\n\navg_cookie\x18\n \x01(\x05\"\x8a\x01\n\x13\x41ggFlowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x19\n\x11total_num_packets\x18\x03 \x01(\x05\x12\x17\n\x0ftotal_num_bytes\x18\x04 \x01(\x05\x12\x17\n\x0ftotal_num_flows\x18\x05 \x01(\x05\"\xf7\x03\n\x10PortStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x1c\n\x14num_received_packets\x18\x04 \x01(\x05\x12\x1a\n\x12num_received_bytes\x18\x05 \x01(\x05\x12\x1b\n\x13num_received_errors\x18\x06 \x01(\x05\x12\x1f\n\x17num_transmitted_packets\x18\x07 \x01(\x05\x12\x1d\n\x15num_transmitted_bytes\x18\x08 \x01(\x05\x12\x1e\n\x16num_transmitted_errors\x18\t \x01(\x05\x12\x1c\n\x14num_received_dropped\x18\n \x01(\x05\x12\x1f\n\x17num_transmitted_dropped\x18\x0b \x01(\x05\x12!\n\x19num_received_frame_errors\x18\x0c \x01(\x05\x12#\n\x1bnum_received_overrun_errors\x18\r \x01(\x05\x12\x1f\n\x17num_received_crc_errors\x18\x0e \x01(\x05\x12\x16\n\x0enum_collisions\x18\x0f \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x10 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\x11 \x01(\x05\"\xa4\x02\n\x10\x46lowStatisticDTO\x12\x11\n\ttimestamp\x18\x01 \x01(\x02\x12\x13\n\x0b\x64\x61tapath_id\x18\x02 \x01(\x05\x12\x0f\n\x07in_port\x18\x03 \x01(\x05\x12\x10\n\x08out_port\x18\x04 \x01(\x05\x12\x17\n\x0f\x64st_mac_address\x18\x05 \x01(\t\x12\x13\n\x0bnum_packets\x18\x06 \x01(\x05\x12\x11\n\tnum_bytes\x18\x07 \x01(\x05\x12\x1c\n\x14\x64uration_nanoseconds\x18\x08 \x01(\x05\x12\x18\n\x10\x64uration_seconds\x18\t \x01(\x05\x12\x14\n\x0chard_timeout\x18\n \x01(\x05\x12\x14\n\x0cidle_timeout\x18\x0b \x01(\x05\x12\x10\n\x08priority\x18\x0c \x01(\x05\x12\x0e\n\x06\x63ookie\x18\r \x01(\x05\"\xc5\x01\n\x18OSSECIdsAlertCountersDTO\x12\x14\n\x0clevel_alerts\x18\x01 \x03(\x05\x12\x14\n\x0cgroup_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12\x14\n\x0ctotal_alerts\x18\x05 \x01(\x05\x12 \n\x18\x61lerts_weighted_by_level\x18\x06 \x01(\x02\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xb5\x01\n\x18SnortIdsAlertCountersDTO\x12\x17\n\x0fpriority_alerts\x18\x01 \x03(\x05\x12\x14\n\x0c\x63lass_alerts\x18\x02 \x03(\x05\x12\x15\n\rsevere_alerts\x18\x03 \x01(\x05\x12\x16\n\x0ewarning_alerts\x18\x04 \x01(\x05\x12#\n\x1b\x61lerts_weighted_by_priority\x18\x05 \x01(\x02\x12\n\n\x02ip\x18\x06 \x01(\t\x12\n\n\x02ts\x18\x07 \x01(\x02\"\xf4\x01\n\x1a\x45mulationAttackerActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\x12\x15\n\rvulnerability\x18\x0c \x01(\t\x12\x10\n\x08\x62\x61\x63kdoor\x18\r \x01(\x08\"\xcb\x01\n\x1a\x45mulationDefenderActionDTO\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63mds\x18\x03 \x03(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\r\n\x05\x64\x65scr\x18\x05 \x01(\t\x12\x0b\n\x03ips\x18\x06 \x03(\t\x12\r\n\x05index\x18\x07 \x01(\x05\x12\x16\n\x0e\x61\x63tion_outcome\x18\x08 \x01(\x05\x12\x10\n\x08\x61lt_cmds\x18\t \x03(\t\x12\x16\n\x0e\x65xecution_time\x18\n \x01(\x02\x12\n\n\x02ts\x18\x0b \x01(\x02\"\xce\x01\n\x12HostMetricsDataDTO\x12\x1b\n\x13num_logged_in_users\x18\x01 \x01(\x05\x12!\n\x19num_failed_login_attempts\x18\x02 \x01(\x05\x12\x1c\n\x14num_open_connections\x18\x03 \x01(\x05\x12\x18\n\x10num_login_events\x18\x04 \x01(\x05\x12\x15\n\rnum_processes\x18\x05 \x01(\x05\x12\x11\n\tnum_users\x18\x06 \x01(\x05\x12\n\n\x02ip\x18\x07 \x01(\t\x12\n\n\x02ts\x18\x08 \x01(\x02\"\xf8\x01\n\x0e\x44ockerStatsDTO\x12\x0c\n\x04pids\x18\x01 \x01(\x02\x12\x11\n\ttimestamp\x18\x02 \x01(\t\x12\x13\n\x0b\x63pu_percent\x18\x03 \x01(\x02\x12\x13\n\x0bmem_current\x18\x04 \x01(\x02\x12\x11\n\tmem_total\x18\x05 \x01(\x02\x12\x13\n\x0bmem_percent\x18\x06 \x01(\x02\x12\x10\n\x08\x62lk_read\x18\x07 \x01(\x02\x12\x11\n\tblk_write\x18\x08 \x01(\x02\x12\x0e\n\x06net_rx\x18\t \x01(\x02\x12\x0e\n\x06net_tx\x18\n \x01(\x02\x12\x16\n\x0e\x63ontainer_name\x18\x0b \x01(\t\x12\n\n\x02ip\x18\x0c \x01(\t\x12\n\n\x02ts\x18\r \x01(\x02\"W\n\x1a\x43lientPopulationMetricsDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\n\n\x02ts\x18\x02 \x01(\x02\x12\x13\n\x0bnum_clients\x18\x03 \x01(\x05\x12\x0c\n\x04rate\x18\x04 \x01(\x02\"\x1a\n\x18GetClusterManagerLogsMsg\"S\n\x13GetContainerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17GetClientManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetKafkaManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fGetKafkaLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12GetSnortIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetSnortIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Y\n\x19GetOSSECIdsManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"R\n\x12GetOSSECIdsLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"U\n\x15GetHostManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18GetTrafficManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14GetElkManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"8\n\rGetElkLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14GetRyuManagerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetRyuControllerLogsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartRyuMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StopHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StopHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"@\n\x15RemoveKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15\x43reateKibanaTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14ListKibanaTunnelsMsg\"5\n\x10KibanaTunnelsDTO\x12!\n\x07tunnels\x18\x01 \x03(\x0b\x32\x10.KibanaTunnelDTO\"T\n\x0fKibanaTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"=\n\x12RemoveRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12\x43reateRyuTunnelMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x13\n\x11ListRyuTunnelsMsg\"/\n\rRyuTunnelsDTO\x12\x1e\n\x07tunnels\x18\x01 \x03(\x0b\x32\r.RyuTunnelDTO\"Q\n\x0cRyuTunnelDTO\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x11\n\temulation\x18\x03 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x04 \x01(\x05\"P\n SnortIdsMonitorThreadStatusesDTO\x12,\n\x10snortIDSStatuses\x18\x01 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"E\n\x1aGetSnortIdsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"N\n#GetSnortIdsMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16StopSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StartSnortIdsManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"B\n\x17StopSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartSnortIdsManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"M\n\rStartSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"I\n\x1eStartSnortIdsMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"L\n\x0cStopSnortMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\\\n\x1cStopSnortIdsMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"J\n\x1fStopSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetRyuManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StopRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartRyuMonitorServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetRyuServiceStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartRyuManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aGetOSSECIDSManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n OSSECIdsMonitorThreadStatusesDTO\x12,\n\x10ossecIDSStatuses\x18\x01 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"N\n#GetOSSECIDSMonitorThreadStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dStopOSSECIDSMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\\\n\x1cStopOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"]\n\x1dStartOSSECIDSMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StopOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"T\n\x14StartOSSECIDSManager\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"?\n\x14StopOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartOSSECIDSManagers\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"P\n\x10StartOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopOSSECIDSMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"=\n\x12StartOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopOSSECIDSesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17GetKafkaManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StartKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopKafkaServerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18GetKafkaManagerStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateKafkaTopicsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13StopKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartKafkaManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16GetHostManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n GetHostMonitorThreadsStatusesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x16\x41pplyFileBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyPacketBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"X\n\x18\x41pplyMetricBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17\x41pplyHeartBeatConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"O\n\x0fStopFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"Q\n\x11StopMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"P\n\x10StopHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"f\n\x10StartFileBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartPacketBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"h\n\x12StartMetricBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"g\n\x11StartHeartBeatMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\x12\x13\n\x0b\x63ontainerIp\x18\x04 \x01(\t\"Y\n\x19StartHostMonitorThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"<\n\x11StopHeartbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopPacketbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StopFilebeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StopMetricbeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStartHostMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x12StopHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"S\n\x13StartHostManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\">\n\x13StopHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xad\x05\n\x10\x45xecutionInfoDTO\x12\x15\n\remulationName\x18\x01 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x02 \x01(\x05\x12\x36\n\x14snortIdsManagersInfo\x18\x03 \x01(\x0b\x32\x18.SnortIdsManagersInfoDTO\x12\x36\n\x14ossecIdsManagersInfo\x18\x04 \x01(\x0b\x32\x18.OSSECIdsManagersInfoDTO\x12\x30\n\x11kafkaManagersInfo\x18\x05 \x01(\x0b\x32\x15.KafkaManagersInfoDTO\x12.\n\x10hostManagersInfo\x18\x06 \x01(\x0b\x32\x14.HostManagersInfoDTO\x12\x32\n\x12\x63lientManagersInfo\x18\x07 \x01(\x0b\x32\x16.ClientManagersInfoDTO\x12<\n\x17\x64ockerStatsManagersInfo\x18\x08 \x01(\x0b\x32\x1b.DockerStatsManagersInfoDTO\x12\x30\n\x11runningContainers\x18\t \x01(\x0b\x32\x15.RunningContainersDTO\x12\x30\n\x11stoppedContainers\x18\n \x01(\x0b\x32\x15.StoppedContainersDTO\x12\x37\n\x16trafficManagersInfoDTO\x18\x0b \x01(\x0b\x32\x17.TrafficManagersInfoDTO\x12*\n\x0e\x61\x63tiveNetworks\x18\x0c \x01(\x0b\x32\x12.DockerNetworksDTO\x12/\n\x12\x65lkManagersInfoDTO\x18\r \x01(\x0b\x32\x13.ElkManagersInfoDTO\x12/\n\x12ryuManagersInfoDTO\x18\x0e \x01(\x0b\x32\x13.RyuManagersInfoDTO\"\xe5\x01\n\x12RyuManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12ryuManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x13ryuManagersStatuses\x18\x06 \x03(\x0b\x32\x14.RyuManagerStatusDTO\x12\x1e\n\x16localControllerWebPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"\xb4\x01\n\x13RyuManagerStatusDTO\x12\x13\n\x0bryu_running\x18\x01 \x01(\x08\x12\x17\n\x0fmonitor_running\x18\x02 \x01(\x08\x12\x0c\n\x04port\x18\x03 \x01(\x05\x12\x10\n\x08web_port\x18\x04 \x01(\x05\x12\x12\n\ncontroller\x18\x05 \x01(\t\x12\x10\n\x08kafka_ip\x18\x06 \x01(\t\x12\x12\n\nkafka_port\x18\x07 \x01(\x05\x12\x15\n\rtime_step_len\x18\x08 \x01(\x05\"\xaf\x01\n\x13HostManagersInfoDTO\x12\x0b\n\x03ips\x18\x15 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1b\n\x13hostManagersRunning\x18\x05 \x03(\x08\x12\x33\n\x14hostManagersStatuses\x18\x06 \x03(\x0b\x32\x15.HostManagerStatusDTO\"L\n\x16HostManagerStatusesDTO\x12\x32\n\x13hostManagerStatuses\x18\x01 \x03(\x0b\x32\x15.HostManagerStatusDTO\"\xa8\x01\n\x14HostManagerStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x18\n\x10\x66ilebeat_running\x18\x02 \x01(\x08\x12\x1a\n\x12packetbeat_running\x18\x03 \x01(\x08\x12\x1a\n\x12metricbeat_running\x18\x04 \x01(\x08\x12\x19\n\x11heartbeat_running\x18\x05 \x01(\x08\x12\n\n\x02ip\x18\x06 \x01(\t\"\xac\x01\n\x14KafkaManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1c\n\x14kafkaManagersRunning\x18\x05 \x03(\x08\x12.\n\x15kafkaManagersStatuses\x18\x06 \x03(\x0b\x32\x0f.KafkaStatusDTO\"1\n\x0eKafkaStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06topics\x18\x02 \x03(\t\"\xb8\x01\n\x17OSSECIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17ossecIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18ossecIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.OSSECIdsStatusDTO\"G\n\x11OSSECIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11ossec_ids_running\x18\x02 \x01(\x08\"\xb8\x01\n\x17SnortIdsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1f\n\x17snortIdsManagersRunning\x18\x05 \x03(\x08\x12\x34\n\x18snortIdsManagersStatuses\x18\x06 \x03(\x0b\x32\x12.SnortIdsStatusDTO\"G\n\x11SnortIdsStatusDTO\x12\x17\n\x0fmonitor_running\x18\x01 \x01(\x08\x12\x19\n\x11snort_ids_running\x18\x02 \x01(\x08\">\n\x13GetExecutionInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStopContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"y\n\x0fRunContainerMsg\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x10\n\x08num_cpus\x18\x04 \x01(\x05\x12\x16\n\x0e\x63reate_network\x18\x05 \x01(\x08\x12\x0f\n\x07version\x18\x06 \x01(\t\"H\n\x1dStartContainersOfExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15GetElkManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xd7\x01\n\x12\x45lkManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1a\n\x12\x65lkManagersRunning\x18\x05 \x03(\x08\x12*\n\x13\x65lkManagersStatuses\x18\x06 \x03(\x0b\x32\r.ElkStatusDTO\x12\x17\n\x0flocalKibanaPort\x18\x07 \x01(\x05\x12\x18\n\x10physicalServerIp\x18\x08 \x01(\t\"A\n\x16StopLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartLogstashServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartKibanaServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StopElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StartElasticServiceMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0fStopElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"V\n\x0c\x45lkStatusDTO\x12\x16\n\x0e\x65lasticRunning\x18\x01 \x01(\x08\x12\x15\n\rkibanaRunning\x18\x02 \x01(\x08\x12\x17\n\x0flogstashRunning\x18\x03 \x01(\x08\"?\n\x14GetElkStackStatusMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11StopElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartElkManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"H\n\x1dGetDockerStatsManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xcb\x01\n\x1a\x44ockerStatsManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\"\n\x1a\x64ockerStatsManagersRunning\x18\x05 \x03(\x08\x12\x41\n\x1b\x64ockerStatsManagersStatuses\x18\x06 \x03(\x0b\x32\x1c.DockerStatsMonitorStatusDTO\"\x1c\n\x1aRemoveAllDockerNetworksMsg\"+\n\x17RemoveDockerNetworksMsg\x12\x10\n\x08networks\x18\x01 \x03(\t\"e\n\x1b\x44ockerStatsMonitorStatusDTO\x12\x14\n\x0cnum_monitors\x18\x01 \x01(\x05\x12\x12\n\nemulations\x18\x02 \x03(\t\x12\x1c\n\x14\x65mulation_executions\x18\x03 \x03(\x05\".\n\x1eGetDockerStatsManagerStatusMsg\x12\x0c\n\x04port\x18\x01 \x01(\x05\"J\n\x1fStopDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x43reateEmulationNetworksMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x1d\n\x1bListAllStoppedContainersMsg\"F\n\x14StoppedContainersDTO\x12.\n\x11stoppedContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"\x1d\n\x1bListAllRunningEmulationsMsg\"1\n\x14RunningEmulationsDTO\x12\x19\n\x11runningEmulations\x18\x01 \x03(\t\"\x1d\n\x1bListAllRunningContainersMsg\"F\n\x14RunningContainersDTO\x12.\n\x11runningContainers\x18\x01 \x03(\x0b\x32\x13.DockerContainerDTO\"=\n\x12\x44ockerContainerDTO\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05image\x18\x02 \x01(\t\x12\n\n\x02ip\x18\x03 \x01(\t\"!\n\x11StartContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1e\n\x1cStartAllStoppedContainersMsg\"\x1a\n\x18ListAllDockerNetworksMsg\":\n\x11\x44ockerNetworksDTO\x12\x10\n\x08networks\x18\x01 \x03(\t\x12\x13\n\x0bnetwork_ids\x18\x02 \x03(\x05\"8\n\x12\x43ontainerImagesDTO\x12\"\n\x06images\x18\x01 \x03(\x0b\x32\x12.ContainerImageDTO\"f\n\x11\x43ontainerImageDTO\x12\x10\n\x08repoTags\x18\x01 \x01(\t\x12\x0f\n\x07\x63reated\x18\x02 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x04 \x01(\t\x12\x0c\n\x04size\x18\x05 \x01(\x03\"\x1b\n\x19ListAllContainerImagesMsg\"\'\n\x17RemoveContainerImageMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bRemoveAllContainerImagesMsg\"\x1f\n\x1dRemoveAllStoppedContainersMsg\"\"\n\x12RemoveContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\" \n\x10StopContainerMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1d\n\x1bStopAllRunningContainersMsg\"D\n\x19GetTrafficManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xb9\x01\n\x16TrafficManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1e\n\x16trafficManagersRunning\x18\x05 \x03(\x08\x12\x37\n\x17trafficManagersStatuses\x18\x06 \x03(\x0b\x32\x16.TrafficManagerInfoDTO\"8\n\x15TrafficManagerInfoDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\x12\x0e\n\x06script\x18\x02 \x01(\t\"\xb1\x01\n\x15\x43lientManagersInfoDTO\x12\x0b\n\x03ips\x18\x01 \x03(\t\x12\r\n\x05ports\x18\x02 \x03(\x05\x12\x15\n\remulationName\x18\x03 \x01(\t\x12\x13\n\x0b\x65xecutionId\x18\x04 \x01(\x05\x12\x1d\n\x15\x63lientManagersRunning\x18\x05 \x03(\x08\x12\x31\n\x16\x63lientManagersStatuses\x18\x06 \x03(\x0b\x32\x11.GetNumClientsDTO\"C\n\x18GetClientManagersInfoMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"X\n\x18StartTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"W\n\x17StopTrafficGeneratorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"C\n\x18StopTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\xae\x01\n\x10GetNumClientsDTO\x12\x13\n\x0bnum_clients\x18\x01 \x01(\x05\x12\x1d\n\x15\x63lient_process_active\x18\x02 \x01(\x08\x12\x17\n\x0fproducer_active\x18\x03 \x01(\x08\x12%\n\x1d\x63lients_time_step_len_seconds\x18\x04 \x01(\x05\x12&\n\x1eproducer_time_step_len_seconds\x18\x05 \x01(\x05\"A\n\x16GetNumActiveClientsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StopClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StopClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartClientManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"A\n\x16StopTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"U\n\x15StopTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"V\n\x16StartTrafficManagerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x13\n\x0b\x63ontainerIp\x18\x03 \x01(\t\"\x17\n\x15\x43leanAllExecutionsMsg\"\x16\n\x14StopAllExecutionsMsg\";\n\x10StopExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43leanExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"4\n\x1fStopAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"5\n CleanAllExecutionsOfEmulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\"\x14\n\x12GetCsleLogFilesMsg\"\x1d\n\rGetLogFileMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\"H\n\x1dStartContainersInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"S\n(AttachContainersToNetworksInExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13InstallLibrariesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\">\n\x13\x41pplyKafkaConfigMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"@\n\x15StartSdnControllerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1a\x41pplyResouceConstraintsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14\x43reateOvsSwitchesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10PingExecutionMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\":\n\x0f\x43onfigureOvsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"G\n\x1cStartSdnControllerMonitorMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateUsersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateVulnsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"9\n\x0e\x43reateFlagsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"<\n\x11\x43reateTopologyMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17StartTrafficManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19StartTrafficGeneratorsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18StartClientPopulationMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"F\n\x1bStartKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"E\n\x1aStopKafkaClientProducerMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartSnortIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartSnortIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"=\n\x12StartOSSECIdsesMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"K\n StartOSSECIdsesMonitorThreadsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\";\n\x10StartElkStackMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"?\n\x14StartHostManagersMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"B\n\x17\x41pplyFileBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyPacketBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"D\n\x19\x41pplyMetricBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"C\n\x18\x41pplyHeartBeatConfigsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"R\n\x11StartFileBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartPacketBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"T\n\x13StartMetricBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"S\n\x12StartHeartBeatsMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\x12\x14\n\x0cinitialStart\x18\x03 \x01(\x08\"\x1e\n\x1cGetDockerStatsManagerLogsMsg\"\x16\n\x14GetPrometheusLogsMsg\"\x18\n\x16GetNodeExporterLogsMsg\"\x14\n\x12GetCAdvisorLogsMsg\"\x13\n\x11GetPgAdminLogsMsg\"\x13\n\x11GetGrafanaLogsMsg\"\x11\n\x0fGetNginxLogsMsg\"\x12\n\x10GetDockerLogsMsg\"\x16\n\x14GetPostgreSQLLogsMsg\"\x11\n\x0fGetFlaskLogsMsg\"\x17\n\x07LogsDTO\x12\x0c\n\x04logs\x18\x01 \x03(\t\"&\n\x13OperationOutcomeDTO\x12\x0f\n\x07outcome\x18\x01 \x01(\x08\"\x12\n\x10GetNodeStatusMsg\"\xb3\x02\n\rNodeStatusDTO\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0e\n\x06leader\x18\x02 \x01(\x08\x12\x17\n\x0f\x63\x41\x64visorRunning\x18\x03 \x01(\x08\x12\x19\n\x11prometheusRunning\x18\x04 \x01(\x08\x12\x16\n\x0egrafanaRunning\x18\x05 \x01(\x08\x12\x16\n\x0epgAdminRunning\x18\x06 \x01(\x08\x12\x14\n\x0cnginxRunning\x18\x07 \x01(\x08\x12\x14\n\x0c\x66laskRunning\x18\x08 \x01(\x08\x12!\n\x19\x64ockerStatsManagerRunning\x18\t \x01(\x08\x12\x1b\n\x13nodeExporterRunning\x18\n \x01(\x08\x12\x19\n\x11postgreSQLRunning\x18\x0b \x01(\x08\x12\x1b\n\x13\x64ockerEngineRunning\x18\x0c \x01(\x08\"#\n\x10ServiceStatusDTO\x12\x0f\n\x07running\x18\x01 \x01(\x08\"\x14\n\x12StartPostgreSQLMsg\"\x12\n\x10StartCAdvisorMsg\"\x16\n\x14StartNodeExporterMsg\"\x11\n\x0fStartGrafanaMsg\"\x14\n\x12StartPrometheusMsg\"\x11\n\x0fStartPgAdminMsg\"\x0f\n\rStartNginxMsg\"\x0f\n\rStartFlaskMsg\"\x1c\n\x1aStartDockerStatsManagerMsg\"K\n StartDockerStatsManagerThreadMsg\x12\x11\n\temulation\x18\x01 \x01(\t\x12\x14\n\x0cipFirstOctet\x18\x02 \x01(\x05\"\x16\n\x14StartDockerEngineMsg\"\x13\n\x11StopPostgreSQLMsg\"\x11\n\x0fStopCAdvisorMsg\"\x15\n\x13StopNodeExporterMsg\"\x10\n\x0eStopGrafanaMsg\"\x13\n\x11StopPrometheusMsg\"\x10\n\x0eStopPgAdminMsg\"\x0e\n\x0cStopNginxMsg\"\x0e\n\x0cStopFlaskMsg\"\x1b\n\x19StopDockerStatsManagerMsg\"\x15\n\x13StopDockerEngineMsg2\xd7o\n\x0e\x43lusterManager\x12\x34\n\rgetNodeStatus\x12\x11.GetNodeStatusMsg\x1a\x0e.NodeStatusDTO\"\x00\x12;\n\x0fstartPostgreSQL\x12\x13.StartPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x37\n\rstartCAdvisor\x12\x11.StartCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startNodeExporter\x12\x15.StartNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartGrafana\x12\x10.StartGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12;\n\x0fstartPrometheus\x12\x13.StartPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstartPgAdmin\x12\x10.StartPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartNginx\x12\x0e.StartNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x31\n\nstartFlask\x12\x0e.StartFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12K\n\x17startDockerStatsManager\x12\x1b.StartDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12W\n\x1dstartDockerStatsManagerThread\x12!.StartDockerStatsManagerThreadMsg\x1a\x11.ServiceStatusDTO\"\x00\x12?\n\x11startDockerEngine\x12\x15.StartDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPostgreSQL\x12\x12.StopPostgreSQLMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x35\n\x0cstopCAdvisor\x12\x10.StopCAdvisorMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopNodeExporter\x12\x14.StopNodeExporterMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopGrafana\x12\x0f.StopGrafanaMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x39\n\x0estopPrometheus\x12\x12.StopPrometheusMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x33\n\x0bstopPgAdmin\x12\x0f.StopPgAdminMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopNginx\x12\r.StopNginxMsg\x1a\x11.ServiceStatusDTO\"\x00\x12/\n\tstopFlask\x12\r.StopFlaskMsg\x1a\x11.ServiceStatusDTO\"\x00\x12I\n\x16stopDockerStatsManager\x12\x1a.StopDockerStatsManagerMsg\x1a\x11.ServiceStatusDTO\"\x00\x12=\n\x10stopDockerEngine\x12\x14.StopDockerEngineMsg\x1a\x11.ServiceStatusDTO\"\x00\x12\x32\n\x0fgetCsleLogFiles\x12\x13.GetCsleLogFilesMsg\x1a\x08.LogsDTO\"\x00\x12\x46\n\x19getDockerStatsManagerLogs\x12\x1d.GetDockerStatsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getPrometheusLogs\x12\x15.GetPrometheusLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getNodeExporterLogs\x12\x17.GetNodeExporterLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetCadvisorLogs\x12\x13.GetCAdvisorLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetPgAdminLogs\x12\x12.GetPgAdminLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x30\n\x0egetGrafanaLogs\x12\x12.GetGrafanaLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetNginxLogs\x12\x10.GetNginxLogsMsg\x1a\x08.LogsDTO\"\x00\x12.\n\rgetDockerLogs\x12\x11.GetDockerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x37\n\x12getPostrgreSQLLogs\x12\x15.GetPostgreSQLLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetFlaskLogs\x12\x10.GetFlaskLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetLogFile\x12\x0e.GetLogFileMsg\x1a\x08.LogsDTO\"\x00\x12T\n\x1astartContainersInExecution\x12\x1e.StartContainersInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12j\n%attachContainersInExecutionToNetworks\x12).AttachContainersToNetworksInExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10installLibraries\x12\x14.InstallLibrariesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10\x61pplyKafkaConfig\x12\x14.ApplyKafkaConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startSdnController\x12\x16.StartSdnControllerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12O\n\x18\x61pplyResourceConstraints\x12\x1b.ApplyResouceConstraintsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateOvsSwitches\x12\x15.CreateOvsSwitchesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rpingExecution\x12\x11.PingExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0c\x63onfigureOvs\x12\x10.ConfigureOvsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19startSdnControllerMonitor\x12\x1d.StartSdnControllerMonitorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateUsers\x12\x0f.CreateUsersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x15\x63reateVulnerabilities\x12\x0f.CreateVulnsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0b\x63reateFlags\x12\x0f.CreateFlagsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63reateTopology\x12\x12.CreateTopologyMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startTrafficGenerators\x12\x1a.StartTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startClientPopulation\x12\x19.StartClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18startKafkaClientProducer\x12\x1c.StartKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17stopKafkaClientProducer\x12\x1b.StopKafkaClientProducerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartSnortIdses\x12\x13.StartSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartSnortIdsesMonitorThreads\x12!.StartSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOssecIdses\x12\x13.StartOSSECIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1dstartOssecIdsesMonitorThreads\x12!.StartOSSECIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartElkStack\x12\x11.StartElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startHostManagers\x12\x15.StartHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyFileBeatsConfig\x12\x18.ApplyFileBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyPacketBeatsConfig\x12\x1a.ApplyPacketBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16\x61pplyMetricBeatsConfig\x12\x1a.ApplyMetricBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyHeartBeatsConfig\x12\x19.ApplyHeartBeatConfigsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartFilebeats\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startPacketbeats\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startMetricbeats\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartHeartbeats\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopAllExecutionsOfEmulation\x12 .StopAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopExecution\x12\x11.StopExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopAllExecutions\x12\x15.StopAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12\x63leanAllExecutions\x12\x16.CleanAllExecutionsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Z\n\x1d\x63leanAllExecutionsOfEmulation\x12!.CleanAllExecutionsOfEmulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0e\x63leanExecution\x12\x12.CleanExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13startTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x12stopTrafficManager\x12\x17.StartTrafficManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x13stopTrafficManagers\x12\x18.StartTrafficManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12startClientManager\x12\x16.StartClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopClientPopulation\x12\x18.StopClientPopulationMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11stopClientManager\x12\x15.StopClientManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13getNumActiveClients\x12\x17.GetNumActiveClientsMsg\x1a\x11.GetNumClientsDTO\"\x00\x12J\n\x15startTrafficGenerator\x12\x19.StartTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopTrafficGenerators\x12\x19.StopTrafficGeneratorsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopTrafficGenerator\x12\x18.StopTrafficGeneratorMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x15getClientManagersInfo\x12\x19.GetClientManagersInfoMsg\x1a\x16.ClientManagersInfoDTO\"\x00\x12N\n\x16getTrafficManagersInfo\x12\x1a.GetTrafficManagersInfoMsg\x1a\x16.TrafficManagerInfoDTO\"\x00\x12P\n\x18stopAllRunningContainers\x12\x1c.StopAllRunningContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopContainer\x12\x11.StopContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1aremoveAllStoppedContainers\x12\x1e.RemoveAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveContainer\x12\x13.RemoveContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12P\n\x18removeAllContainerImages\x12\x1c.RemoveAllContainerImagesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14removeContainerImage\x12\x18.RemoveContainerImageMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12K\n\x16listAllContainerImages\x12\x1a.ListAllContainerImagesMsg\x1a\x13.ContainerImagesDTO\"\x00\x12H\n\x15listAllDockerNetworks\x12\x19.ListAllDockerNetworksMsg\x1a\x12.DockerNetworksDTO\"\x00\x12R\n\x19startAllStoppedContainers\x12\x1d.StartAllStoppedContainersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estartContainer\x12\x12.StartContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12Q\n\x18listAllRunningContainers\x12\x1c.ListAllRunningContainersMsg\x1a\x15.RunningContainersDTO\"\x00\x12Q\n\x18listAllRunningEmulations\x12\x1c.ListAllRunningEmulationsMsg\x1a\x15.RunningEmulationsDTO\"\x00\x12Q\n\x18listAllStoppedContainers\x12\x1c.ListAllStoppedContainersMsg\x1a\x15.StoppedContainersDTO\"\x00\x12N\n\x17\x63reateEmulationNetworks\x12\x1b.CreateEmulationNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopDockerStatsManagerThread\x12 .StopDockerStatsManagerThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12^\n\x1bgetDockerStatsManagerStatus\x12\x1f.GetDockerStatsManagerStatusMsg\x1a\x1c.DockerStatsMonitorStatusDTO\"\x00\x12H\n\x14removeDockerNetworks\x12\x18.RemoveDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17removeAllDockerNetworks\x12\x1b.RemoveAllDockerNetworksMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12[\n\x1agetDockerStatsManagersInfo\x12\x1e.GetDockerStatsManagersInfoMsg\x1a\x1b.DockerStatsManagersInfoDTO\"\x00\x12>\n\x0fstartElkManager\x12\x13.StartElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopElkManager\x12\x12.StopElkManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0cgetElkStatus\x12\x15.GetElkStackStatusMsg\x1a\r.ElkStatusDTO\"\x00\x12\x38\n\x0cstopElkStack\x12\x10.StopElkStackMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstartElastic\x12\x17.StartElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstopElastic\x12\x16.StopElasticServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0bstartKibana\x12\x16.StartKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\nstopKibana\x12\x15.StopKibanaServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x41\n\rstartLogstash\x12\x18.StartLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cstopLogstash\x12\x17.StopLogstashServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getElkManagersInfo\x12\x16.GetElkManagersInfoMsg\x1a\x13.ElkManagersInfoDTO\"\x00\x12T\n\x1astartContainersOfExecution\x12\x1e.StartContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0crunContainer\x12\x10.RunContainerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopContainersOfExecution\x12\x1d.StopContainersOfExecutionMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10startHostManager\x12\x14.StartHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12@\n\x10stopHostManagers\x12\x14.StopHostManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopHostManager\x12\x13.StopHostManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopFilebeats\x12\x11.StopFilebeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopPacketbeats\x12\x13.StopPacketbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstopMetricbeats\x12\x13.StopMetricbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopHeartbeats\x12\x12.StopHeartbeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12N\n\x17startHostMonitorThreads\x12\x1b.StartHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16startHostMonitorThread\x12\x1a.StartHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12;\n\rstartFilebeat\x12\x12.StartFileBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartPacketbeat\x12\x14.StartPacketBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0fstartMetricbeat\x12\x14.StartMetricBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12=\n\x0estartHeartbeat\x12\x13.StartHeartBeatsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopFilebeat\x12\x10.StopFileBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopPacketbeat\x12\x12.StopPacketBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopMetricbeat\x12\x12.StopMetricBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstopHeartbeat\x12\x11.StopHeartBeatMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13\x61pplyFileBeatConfig\x12\x17.ApplyFileBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyPacketBeatConfig\x12\x19.ApplyPacketBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15\x61pplyMetricBeatConfig\x12\x19.ApplyMetricBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14\x61pplyHeartBeatConfig\x12\x18.ApplyHeartBeatConfigMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12]\n\x1dgetHostMonitorThreadsStatuses\x12!.GetHostMonitorThreadsStatusesMsg\x1a\x17.HostManagerStatusesDTO\"\x00\x12\x46\n\x13getHostManagersInfo\x12\x17.GetHostManagersInfoMsg\x1a\x14.HostManagersInfoDTO\"\x00\x12@\n\x10stopKafkaManager\x12\x14.StopKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11startKafkaManager\x12\x15.StartKafkaManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x11\x63reateKafkaTopics\x12\x15.CreateKafkaTopicsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0egetKafkaStatus\x12\x19.GetKafkaManagerStatusMsg\x1a\x0f.KafkaStatusDTO\"\x00\x12>\n\x0fstopKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x10startKafkaServer\x12\x13.StopKafkaServerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12I\n\x14getKafkaManagersInfo\x12\x18.GetKafkaManagersInfoMsg\x1a\x15.KafkaManagersInfoDTO\"\x00\x12<\n\x0estopOSSECIDSes\x12\x12.StopOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fstartOSSECIDSes\x12\x13.StartOSSECIDSesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x38\n\x0cstopOSSECIDS\x12\x10.StopOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12:\n\rstartOSSECIDS\x12\x11.StartOSSECIDSMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12G\n\x15startOSSECIDSManagers\x12\x16.StartOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14stopOSSECIDSManagers\x12\x15.StopOSSECIDSManagers\x1a\x14.OperationOutcomeDTO\"\x00\x12\x45\n\x14startOSSECIDSManager\x12\x15.StartOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x13stopOSSECIDSManager\x12\x14.StopOSSECIDSManager\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartOSSECIDSMonitorThread\x12\x1e.StartOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopOSSECIDSMonitorThread\x12\x1d.StopOSSECIDSMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopOSSECIDSMonitorThreads\x12\x1e.StopOSSECIDSMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getOSSECIDSMonitorThreadStatuses\x12$.GetOSSECIDSMonitorThreadStatusesMsg\x1a!.OSSECIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getOSSECIdsManagersInfo\x12\x1b.GetOSSECIDSManagersInfoMsg\x1a\x18.OSSECIdsManagersInfoDTO\"\x00\x12>\n\x0fstartRyuManager\x12\x13.StartRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x0estopRyuManager\x12\x12.StopRyuManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12?\n\x0cgetRyuStatus\x12\x17.GetRyuServiceStatusMsg\x1a\x14.RyuManagerStatusDTO\"\x00\x12\x37\n\x08startRyu\x12\x13.StartRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x07stopRyu\x12\x12.StopRyuServiceMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x43\n\x12getRyuManagersInfo\x12\x16.GetRyuManagersInfoMsg\x1a\x13.RyuManagersInfoDTO\"\x00\x12<\n\x0estopSnortIdses\x12\x12.StopSnortIdsesMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12X\n\x1cstopSnortIdsesMonitorThreads\x12 .StopSnortIdsesMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x35\n\x0cstopSnortIds\x12\r.StopSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12R\n\x19stopSnortIdsMonitorThread\x12\x1d.StopSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x37\n\rstartSnortIds\x12\x0e.StartSnortMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12V\n\x1bstartSnortIdsMonitorThreads\x12\x1f.StartSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astartSnortIdsMonitorThread\x12\x1e.StartSnortIdsMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15startSnortIdsManagers\x12\x19.StartSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14stopSnortIdsManagers\x12\x18.StopSnortIdsManagersMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12H\n\x14startSnortIdsManager\x12\x18.StartSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x46\n\x13stopSnortIdsManager\x12\x17.StopSnortIdsManagerMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12T\n\x1astopSnortIdsMonitorThreads\x12\x1e.StopSnortIdsMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12m\n getSnortIdsMonitorThreadStatuses\x12$.GetSnortIdsMonitorThreadStatusesMsg\x1a!.SnortIdsMonitorThreadStatusesDTO\"\x00\x12R\n\x17getSnortIdsManagersInfo\x12\x1b.GetSnortIdsManagersInfoMsg\x1a\x18.SnortIdsManagersInfoDTO\"\x00\x12=\n\x10getExecutionInfo\x12\x14.GetExecutionInfoMsg\x1a\x11.ExecutionInfoDTO\"\x00\x12?\n\x11listKibanaTunnels\x12\x15.ListKibanaTunnelsMsg\x1a\x11.KibanaTunnelsDTO\"\x00\x12\x44\n\x12\x63reateKibanaTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x36\n\x0elistRyuTunnels\x12\x12.ListRyuTunnelsMsg\x1a\x0e.RyuTunnelsDTO\"\x00\x12\x41\n\x0f\x63reateRyuTunnel\x12\x16.CreateKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x12removeKibanaTunnel\x12\x16.RemoveKibanaTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12>\n\x0fremoveRyuTunnel\x12\x13.RemoveRyuTunnelMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12L\n\x16stopHostMonitorThreads\x12\x1a.StopHostMonitorThreadsMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12J\n\x15stopHostMonitorThread\x12\x19.StopHostMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x44\n\x0fstartRyuMonitor\x12\x19.StartRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12\x42\n\x0estopRyuMonitor\x12\x18.StopRyuMonitorThreadMsg\x1a\x14.OperationOutcomeDTO\"\x00\x12<\n\x14getRyuControllerLogs\x12\x18.GetRyuControllerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getRyuManagerLogs\x12\x15.GetRyuManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12(\n\ngetElkLogs\x12\x0e.GetElkLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x36\n\x11getElkManagerLogs\x12\x15.GetElkManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getTrafficManagerLogs\x12\x19.GetTrafficManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x38\n\x12getHostManagerLogs\x12\x16.GetHostManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetOSSECIdsLogs\x12\x13.GetOSSECIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getOSSECIdsManagerLogsMsg\x12\x1a.GetOSSECIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x32\n\x0fgetSnortIdsLogs\x12\x13.GetSnortIdsLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x43\n\x19getSnortIdsManagerLogsMsg\x12\x1a.GetSnortIdsManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12,\n\x0cgetKafkaLogs\x12\x10.GetKafkaLogsMsg\x1a\x08.LogsDTO\"\x00\x12:\n\x13getKafkaManagerLogs\x12\x17.GetKafkaManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12?\n\x17getClientManagerLogsMsg\x12\x18.GetClientManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12\x34\n\x10getContainerLogs\x12\x14.GetContainerLogsMsg\x1a\x08.LogsDTO\"\x00\x12>\n\x15getClusterManagerLogs\x12\x19.GetClusterManagerLogsMsg\x1a\x08.LogsDTO\"\x00\x12^\n\x1agetExecutionTimeSeriesData\x12\x1e.GetExecutionTimeSeriesDataMsg\x1a\x1e.EmulationMetricsTimeSeriesDTO\"\x00\x62\x06proto3')
 
 
 
 _GETEXECUTIONTIMESERIESDATAMSG = DESCRIPTOR.message_types_by_name['GetExecutionTimeSeriesDataMsg']
 _EMULATIONMETRICSTIMESERIESDTO = DESCRIPTOR.message_types_by_name['EmulationMetricsTimeSeriesDTO']
 _AVGPORTSTATISTICDICT = DESCRIPTOR.message_types_by_name['AvgPortStatisticDict']
 _AGGFLOWSTATISTICDICT = DESCRIPTOR.message_types_by_name['AggFlowStatisticDict']
@@ -2401,307 +2401,307 @@
   _STARTHOSTMANAGERMSG._serialized_start=12005
   _STARTHOSTMANAGERMSG._serialized_end=12088
   _STOPHOSTMANAGERSMSG._serialized_start=12090
   _STOPHOSTMANAGERSMSG._serialized_end=12152
   _EXECUTIONINFODTO._serialized_start=12155
   _EXECUTIONINFODTO._serialized_end=12840
   _RYUMANAGERSINFODTO._serialized_start=12843
-  _RYUMANAGERSINFODTO._serialized_end=13014
-  _RYUMANAGERSTATUSDTO._serialized_start=13017
-  _RYUMANAGERSTATUSDTO._serialized_end=13197
-  _HOSTMANAGERSINFODTO._serialized_start=13200
-  _HOSTMANAGERSINFODTO._serialized_end=13375
-  _HOSTMANAGERSTATUSESDTO._serialized_start=13377
-  _HOSTMANAGERSTATUSESDTO._serialized_end=13453
-  _HOSTMANAGERSTATUSDTO._serialized_start=13456
-  _HOSTMANAGERSTATUSDTO._serialized_end=13624
-  _KAFKAMANAGERSINFODTO._serialized_start=13627
-  _KAFKAMANAGERSINFODTO._serialized_end=13799
-  _KAFKASTATUSDTO._serialized_start=13801
-  _KAFKASTATUSDTO._serialized_end=13850
-  _OSSECIDSMANAGERSINFODTO._serialized_start=13853
-  _OSSECIDSMANAGERSINFODTO._serialized_end=14037
-  _OSSECIDSSTATUSDTO._serialized_start=14039
-  _OSSECIDSSTATUSDTO._serialized_end=14110
-  _SNORTIDSMANAGERSINFODTO._serialized_start=14113
-  _SNORTIDSMANAGERSINFODTO._serialized_end=14297
-  _SNORTIDSSTATUSDTO._serialized_start=14299
-  _SNORTIDSSTATUSDTO._serialized_end=14370
-  _GETEXECUTIONINFOMSG._serialized_start=14372
-  _GETEXECUTIONINFOMSG._serialized_end=14434
-  _STOPCONTAINERSOFEXECUTIONMSG._serialized_start=14436
-  _STOPCONTAINERSOFEXECUTIONMSG._serialized_end=14507
-  _RUNCONTAINERMSG._serialized_start=14509
-  _RUNCONTAINERMSG._serialized_end=14630
-  _STARTCONTAINERSOFEXECUTIONMSG._serialized_start=14632
-  _STARTCONTAINERSOFEXECUTIONMSG._serialized_end=14704
-  _GETELKMANAGERSINFOMSG._serialized_start=14706
-  _GETELKMANAGERSINFOMSG._serialized_end=14770
-  _ELKMANAGERSINFODTO._serialized_start=14773
-  _ELKMANAGERSINFODTO._serialized_end=14962
-  _STOPLOGSTASHSERVICEMSG._serialized_start=14964
-  _STOPLOGSTASHSERVICEMSG._serialized_end=15029
-  _STARTLOGSTASHSERVICEMSG._serialized_start=15031
-  _STARTLOGSTASHSERVICEMSG._serialized_end=15097
-  _STOPKIBANASERVICEMSG._serialized_start=15099
-  _STOPKIBANASERVICEMSG._serialized_end=15162
-  _STARTKIBANASERVICEMSG._serialized_start=15164
-  _STARTKIBANASERVICEMSG._serialized_end=15228
-  _STOPELASTICSERVICEMSG._serialized_start=15230
-  _STOPELASTICSERVICEMSG._serialized_end=15294
-  _STARTELASTICSERVICEMSG._serialized_start=15296
-  _STARTELASTICSERVICEMSG._serialized_end=15361
-  _STOPELKSTACKMSG._serialized_start=15363
-  _STOPELKSTACKMSG._serialized_end=15421
-  _ELKSTATUSDTO._serialized_start=15423
-  _ELKSTATUSDTO._serialized_end=15509
-  _GETELKSTACKSTATUSMSG._serialized_start=15511
-  _GETELKSTACKSTATUSMSG._serialized_end=15574
-  _STOPELKMANAGERMSG._serialized_start=15576
-  _STOPELKMANAGERMSG._serialized_end=15636
-  _STARTELKMANAGERMSG._serialized_start=15638
-  _STARTELKMANAGERMSG._serialized_end=15699
-  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_start=15701
-  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_end=15773
-  _DOCKERSTATSMANAGERSINFODTO._serialized_start=15776
-  _DOCKERSTATSMANAGERSINFODTO._serialized_end=15979
-  _REMOVEALLDOCKERNETWORKSMSG._serialized_start=15981
-  _REMOVEALLDOCKERNETWORKSMSG._serialized_end=16009
-  _REMOVEDOCKERNETWORKSMSG._serialized_start=16011
-  _REMOVEDOCKERNETWORKSMSG._serialized_end=16054
-  _DOCKERSTATSMONITORSTATUSDTO._serialized_start=16056
-  _DOCKERSTATSMONITORSTATUSDTO._serialized_end=16157
-  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_start=16159
-  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_end=16205
-  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_start=16207
-  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_end=16281
-  _CREATEEMULATIONNETWORKSMSG._serialized_start=16283
-  _CREATEEMULATIONNETWORKSMSG._serialized_end=16352
-  _LISTALLSTOPPEDCONTAINERSMSG._serialized_start=16354
-  _LISTALLSTOPPEDCONTAINERSMSG._serialized_end=16383
-  _STOPPEDCONTAINERSDTO._serialized_start=16385
-  _STOPPEDCONTAINERSDTO._serialized_end=16455
-  _LISTALLRUNNINGEMULATIONSMSG._serialized_start=16457
-  _LISTALLRUNNINGEMULATIONSMSG._serialized_end=16486
-  _RUNNINGEMULATIONSDTO._serialized_start=16488
-  _RUNNINGEMULATIONSDTO._serialized_end=16537
-  _LISTALLRUNNINGCONTAINERSMSG._serialized_start=16539
-  _LISTALLRUNNINGCONTAINERSMSG._serialized_end=16568
-  _RUNNINGCONTAINERSDTO._serialized_start=16570
-  _RUNNINGCONTAINERSDTO._serialized_end=16640
-  _DOCKERCONTAINERDTO._serialized_start=16642
-  _DOCKERCONTAINERDTO._serialized_end=16703
-  _STARTCONTAINERMSG._serialized_start=16705
-  _STARTCONTAINERMSG._serialized_end=16738
-  _STARTALLSTOPPEDCONTAINERSMSG._serialized_start=16740
-  _STARTALLSTOPPEDCONTAINERSMSG._serialized_end=16770
-  _LISTALLDOCKERNETWORKSMSG._serialized_start=16772
-  _LISTALLDOCKERNETWORKSMSG._serialized_end=16798
-  _DOCKERNETWORKSDTO._serialized_start=16800
-  _DOCKERNETWORKSDTO._serialized_end=16858
-  _CONTAINERIMAGESDTO._serialized_start=16860
-  _CONTAINERIMAGESDTO._serialized_end=16916
-  _CONTAINERIMAGEDTO._serialized_start=16918
-  _CONTAINERIMAGEDTO._serialized_end=17020
-  _LISTALLCONTAINERIMAGESMSG._serialized_start=17022
-  _LISTALLCONTAINERIMAGESMSG._serialized_end=17049
-  _REMOVECONTAINERIMAGEMSG._serialized_start=17051
-  _REMOVECONTAINERIMAGEMSG._serialized_end=17090
-  _REMOVEALLCONTAINERIMAGESMSG._serialized_start=17092
-  _REMOVEALLCONTAINERIMAGESMSG._serialized_end=17121
-  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_start=17123
-  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_end=17154
-  _REMOVECONTAINERMSG._serialized_start=17156
-  _REMOVECONTAINERMSG._serialized_end=17190
-  _STOPCONTAINERMSG._serialized_start=17192
-  _STOPCONTAINERMSG._serialized_end=17224
-  _STOPALLRUNNINGCONTAINERSMSG._serialized_start=17226
-  _STOPALLRUNNINGCONTAINERSMSG._serialized_end=17255
-  _GETTRAFFICMANAGERSINFOMSG._serialized_start=17257
-  _GETTRAFFICMANAGERSINFOMSG._serialized_end=17325
-  _TRAFFICMANAGERSINFODTO._serialized_start=17328
-  _TRAFFICMANAGERSINFODTO._serialized_end=17513
-  _TRAFFICMANAGERINFODTO._serialized_start=17515
-  _TRAFFICMANAGERINFODTO._serialized_end=17571
-  _CLIENTMANAGERSINFODTO._serialized_start=17574
-  _CLIENTMANAGERSINFODTO._serialized_end=17751
-  _GETCLIENTMANAGERSINFOMSG._serialized_start=17753
-  _GETCLIENTMANAGERSINFOMSG._serialized_end=17820
-  _STARTTRAFFICGENERATORMSG._serialized_start=17822
-  _STARTTRAFFICGENERATORMSG._serialized_end=17910
-  _STOPTRAFFICGENERATORMSG._serialized_start=17912
-  _STOPTRAFFICGENERATORMSG._serialized_end=17999
-  _STOPTRAFFICGENERATORSMSG._serialized_start=18001
-  _STOPTRAFFICGENERATORSMSG._serialized_end=18068
-  _GETNUMCLIENTSDTO._serialized_start=18071
-  _GETNUMCLIENTSDTO._serialized_end=18245
-  _GETNUMACTIVECLIENTSMSG._serialized_start=18247
-  _GETNUMACTIVECLIENTSMSG._serialized_end=18312
-  _STOPCLIENTPOPULATIONMSG._serialized_start=18314
-  _STOPCLIENTPOPULATIONMSG._serialized_end=18380
-  _STOPCLIENTMANAGERMSG._serialized_start=18382
-  _STOPCLIENTMANAGERMSG._serialized_end=18445
-  _STARTCLIENTMANAGERMSG._serialized_start=18447
-  _STARTCLIENTMANAGERMSG._serialized_end=18511
-  _STOPTRAFFICMANAGERSMSG._serialized_start=18513
-  _STOPTRAFFICMANAGERSMSG._serialized_end=18578
-  _STOPTRAFFICMANAGERMSG._serialized_start=18580
-  _STOPTRAFFICMANAGERMSG._serialized_end=18665
-  _STARTTRAFFICMANAGERMSG._serialized_start=18667
-  _STARTTRAFFICMANAGERMSG._serialized_end=18753
-  _CLEANALLEXECUTIONSMSG._serialized_start=18755
-  _CLEANALLEXECUTIONSMSG._serialized_end=18778
-  _STOPALLEXECUTIONSMSG._serialized_start=18780
-  _STOPALLEXECUTIONSMSG._serialized_end=18802
-  _STOPEXECUTIONMSG._serialized_start=18804
-  _STOPEXECUTIONMSG._serialized_end=18863
-  _CLEANEXECUTIONMSG._serialized_start=18865
-  _CLEANEXECUTIONMSG._serialized_end=18925
-  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_start=18927
-  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_end=18979
-  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_start=18981
-  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_end=19034
-  _GETCSLELOGFILESMSG._serialized_start=19036
-  _GETCSLELOGFILESMSG._serialized_end=19056
-  _GETLOGFILEMSG._serialized_start=19058
-  _GETLOGFILEMSG._serialized_end=19087
-  _STARTCONTAINERSINEXECUTIONMSG._serialized_start=19089
-  _STARTCONTAINERSINEXECUTIONMSG._serialized_end=19161
-  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_start=19163
-  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_end=19246
-  _INSTALLLIBRARIESMSG._serialized_start=19248
-  _INSTALLLIBRARIESMSG._serialized_end=19310
-  _APPLYKAFKACONFIGMSG._serialized_start=19312
-  _APPLYKAFKACONFIGMSG._serialized_end=19374
-  _STARTSDNCONTROLLERMSG._serialized_start=19376
-  _STARTSDNCONTROLLERMSG._serialized_end=19440
-  _APPLYRESOUCECONSTRAINTSMSG._serialized_start=19442
-  _APPLYRESOUCECONSTRAINTSMSG._serialized_end=19511
-  _CREATEOVSSWITCHESMSG._serialized_start=19513
-  _CREATEOVSSWITCHESMSG._serialized_end=19576
-  _PINGEXECUTIONMSG._serialized_start=19578
-  _PINGEXECUTIONMSG._serialized_end=19637
-  _CONFIGUREOVSMSG._serialized_start=19639
-  _CONFIGUREOVSMSG._serialized_end=19697
-  _STARTSDNCONTROLLERMONITORMSG._serialized_start=19699
-  _STARTSDNCONTROLLERMONITORMSG._serialized_end=19770
-  _CREATEUSERSMSG._serialized_start=19772
-  _CREATEUSERSMSG._serialized_end=19829
-  _CREATEVULNSMSG._serialized_start=19831
-  _CREATEVULNSMSG._serialized_end=19888
-  _CREATEFLAGSMSG._serialized_start=19890
-  _CREATEFLAGSMSG._serialized_end=19947
-  _CREATETOPOLOGYMSG._serialized_start=19949
-  _CREATETOPOLOGYMSG._serialized_end=20009
-  _STARTTRAFFICMANAGERSMSG._serialized_start=20011
-  _STARTTRAFFICMANAGERSMSG._serialized_end=20077
-  _STARTTRAFFICGENERATORSMSG._serialized_start=20079
-  _STARTTRAFFICGENERATORSMSG._serialized_end=20147
-  _STARTCLIENTPOPULATIONMSG._serialized_start=20149
-  _STARTCLIENTPOPULATIONMSG._serialized_end=20216
-  _STARTKAFKACLIENTPRODUCERMSG._serialized_start=20218
-  _STARTKAFKACLIENTPRODUCERMSG._serialized_end=20288
-  _STOPKAFKACLIENTPRODUCERMSG._serialized_start=20290
-  _STOPKAFKACLIENTPRODUCERMSG._serialized_end=20359
-  _STARTSNORTIDSESMSG._serialized_start=20361
-  _STARTSNORTIDSESMSG._serialized_end=20422
-  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_start=20424
-  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_end=20499
-  _STARTOSSECIDSESMSG._serialized_start=20501
-  _STARTOSSECIDSESMSG._serialized_end=20562
-  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_start=20564
-  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_end=20639
-  _STARTELKSTACKMSG._serialized_start=20641
-  _STARTELKSTACKMSG._serialized_end=20700
-  _STARTHOSTMANAGERSMSG._serialized_start=20702
-  _STARTHOSTMANAGERSMSG._serialized_end=20765
-  _APPLYFILEBEATCONFIGSMSG._serialized_start=20767
-  _APPLYFILEBEATCONFIGSMSG._serialized_end=20833
-  _APPLYPACKETBEATCONFIGSMSG._serialized_start=20835
-  _APPLYPACKETBEATCONFIGSMSG._serialized_end=20903
-  _APPLYMETRICBEATCONFIGSMSG._serialized_start=20905
-  _APPLYMETRICBEATCONFIGSMSG._serialized_end=20973
-  _APPLYHEARTBEATCONFIGSMSG._serialized_start=20975
-  _APPLYHEARTBEATCONFIGSMSG._serialized_end=21042
-  _STARTFILEBEATSMSG._serialized_start=21044
-  _STARTFILEBEATSMSG._serialized_end=21126
-  _STARTPACKETBEATSMSG._serialized_start=21128
-  _STARTPACKETBEATSMSG._serialized_end=21212
-  _STARTMETRICBEATSMSG._serialized_start=21214
-  _STARTMETRICBEATSMSG._serialized_end=21298
-  _STARTHEARTBEATSMSG._serialized_start=21300
-  _STARTHEARTBEATSMSG._serialized_end=21383
-  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_start=21385
-  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_end=21415
-  _GETPROMETHEUSLOGSMSG._serialized_start=21417
-  _GETPROMETHEUSLOGSMSG._serialized_end=21439
-  _GETNODEEXPORTERLOGSMSG._serialized_start=21441
-  _GETNODEEXPORTERLOGSMSG._serialized_end=21465
-  _GETCADVISORLOGSMSG._serialized_start=21467
-  _GETCADVISORLOGSMSG._serialized_end=21487
-  _GETPGADMINLOGSMSG._serialized_start=21489
-  _GETPGADMINLOGSMSG._serialized_end=21508
-  _GETGRAFANALOGSMSG._serialized_start=21510
-  _GETGRAFANALOGSMSG._serialized_end=21529
-  _GETNGINXLOGSMSG._serialized_start=21531
-  _GETNGINXLOGSMSG._serialized_end=21548
-  _GETDOCKERLOGSMSG._serialized_start=21550
-  _GETDOCKERLOGSMSG._serialized_end=21568
-  _GETPOSTGRESQLLOGSMSG._serialized_start=21570
-  _GETPOSTGRESQLLOGSMSG._serialized_end=21592
-  _GETFLASKLOGSMSG._serialized_start=21594
-  _GETFLASKLOGSMSG._serialized_end=21611
-  _LOGSDTO._serialized_start=21613
-  _LOGSDTO._serialized_end=21636
-  _OPERATIONOUTCOMEDTO._serialized_start=21638
-  _OPERATIONOUTCOMEDTO._serialized_end=21676
-  _GETNODESTATUSMSG._serialized_start=21678
-  _GETNODESTATUSMSG._serialized_end=21696
-  _NODESTATUSDTO._serialized_start=21699
-  _NODESTATUSDTO._serialized_end=22006
-  _SERVICESTATUSDTO._serialized_start=22008
-  _SERVICESTATUSDTO._serialized_end=22043
-  _STARTPOSTGRESQLMSG._serialized_start=22045
-  _STARTPOSTGRESQLMSG._serialized_end=22065
-  _STARTCADVISORMSG._serialized_start=22067
-  _STARTCADVISORMSG._serialized_end=22085
-  _STARTNODEEXPORTERMSG._serialized_start=22087
-  _STARTNODEEXPORTERMSG._serialized_end=22109
-  _STARTGRAFANAMSG._serialized_start=22111
-  _STARTGRAFANAMSG._serialized_end=22128
-  _STARTPROMETHEUSMSG._serialized_start=22130
-  _STARTPROMETHEUSMSG._serialized_end=22150
-  _STARTPGADMINMSG._serialized_start=22152
-  _STARTPGADMINMSG._serialized_end=22169
-  _STARTNGINXMSG._serialized_start=22171
-  _STARTNGINXMSG._serialized_end=22186
-  _STARTFLASKMSG._serialized_start=22188
-  _STARTFLASKMSG._serialized_end=22203
-  _STARTDOCKERSTATSMANAGERMSG._serialized_start=22205
-  _STARTDOCKERSTATSMANAGERMSG._serialized_end=22233
-  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_start=22235
-  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_end=22310
-  _STARTDOCKERENGINEMSG._serialized_start=22312
-  _STARTDOCKERENGINEMSG._serialized_end=22334
-  _STOPPOSTGRESQLMSG._serialized_start=22336
-  _STOPPOSTGRESQLMSG._serialized_end=22355
-  _STOPCADVISORMSG._serialized_start=22357
-  _STOPCADVISORMSG._serialized_end=22374
-  _STOPNODEEXPORTERMSG._serialized_start=22376
-  _STOPNODEEXPORTERMSG._serialized_end=22397
-  _STOPGRAFANAMSG._serialized_start=22399
-  _STOPGRAFANAMSG._serialized_end=22415
-  _STOPPROMETHEUSMSG._serialized_start=22417
-  _STOPPROMETHEUSMSG._serialized_end=22436
-  _STOPPGADMINMSG._serialized_start=22438
-  _STOPPGADMINMSG._serialized_end=22454
-  _STOPNGINXMSG._serialized_start=22456
-  _STOPNGINXMSG._serialized_end=22470
-  _STOPFLASKMSG._serialized_start=22472
-  _STOPFLASKMSG._serialized_end=22486
-  _STOPDOCKERSTATSMANAGERMSG._serialized_start=22488
-  _STOPDOCKERSTATSMANAGERMSG._serialized_end=22515
-  _STOPDOCKERENGINEMSG._serialized_start=22517
-  _STOPDOCKERENGINEMSG._serialized_end=22538
-  _CLUSTERMANAGER._serialized_start=22541
-  _CLUSTERMANAGER._serialized_end=36836
+  _RYUMANAGERSINFODTO._serialized_end=13072
+  _RYUMANAGERSTATUSDTO._serialized_start=13075
+  _RYUMANAGERSTATUSDTO._serialized_end=13255
+  _HOSTMANAGERSINFODTO._serialized_start=13258
+  _HOSTMANAGERSINFODTO._serialized_end=13433
+  _HOSTMANAGERSTATUSESDTO._serialized_start=13435
+  _HOSTMANAGERSTATUSESDTO._serialized_end=13511
+  _HOSTMANAGERSTATUSDTO._serialized_start=13514
+  _HOSTMANAGERSTATUSDTO._serialized_end=13682
+  _KAFKAMANAGERSINFODTO._serialized_start=13685
+  _KAFKAMANAGERSINFODTO._serialized_end=13857
+  _KAFKASTATUSDTO._serialized_start=13859
+  _KAFKASTATUSDTO._serialized_end=13908
+  _OSSECIDSMANAGERSINFODTO._serialized_start=13911
+  _OSSECIDSMANAGERSINFODTO._serialized_end=14095
+  _OSSECIDSSTATUSDTO._serialized_start=14097
+  _OSSECIDSSTATUSDTO._serialized_end=14168
+  _SNORTIDSMANAGERSINFODTO._serialized_start=14171
+  _SNORTIDSMANAGERSINFODTO._serialized_end=14355
+  _SNORTIDSSTATUSDTO._serialized_start=14357
+  _SNORTIDSSTATUSDTO._serialized_end=14428
+  _GETEXECUTIONINFOMSG._serialized_start=14430
+  _GETEXECUTIONINFOMSG._serialized_end=14492
+  _STOPCONTAINERSOFEXECUTIONMSG._serialized_start=14494
+  _STOPCONTAINERSOFEXECUTIONMSG._serialized_end=14565
+  _RUNCONTAINERMSG._serialized_start=14567
+  _RUNCONTAINERMSG._serialized_end=14688
+  _STARTCONTAINERSOFEXECUTIONMSG._serialized_start=14690
+  _STARTCONTAINERSOFEXECUTIONMSG._serialized_end=14762
+  _GETELKMANAGERSINFOMSG._serialized_start=14764
+  _GETELKMANAGERSINFOMSG._serialized_end=14828
+  _ELKMANAGERSINFODTO._serialized_start=14831
+  _ELKMANAGERSINFODTO._serialized_end=15046
+  _STOPLOGSTASHSERVICEMSG._serialized_start=15048
+  _STOPLOGSTASHSERVICEMSG._serialized_end=15113
+  _STARTLOGSTASHSERVICEMSG._serialized_start=15115
+  _STARTLOGSTASHSERVICEMSG._serialized_end=15181
+  _STOPKIBANASERVICEMSG._serialized_start=15183
+  _STOPKIBANASERVICEMSG._serialized_end=15246
+  _STARTKIBANASERVICEMSG._serialized_start=15248
+  _STARTKIBANASERVICEMSG._serialized_end=15312
+  _STOPELASTICSERVICEMSG._serialized_start=15314
+  _STOPELASTICSERVICEMSG._serialized_end=15378
+  _STARTELASTICSERVICEMSG._serialized_start=15380
+  _STARTELASTICSERVICEMSG._serialized_end=15445
+  _STOPELKSTACKMSG._serialized_start=15447
+  _STOPELKSTACKMSG._serialized_end=15505
+  _ELKSTATUSDTO._serialized_start=15507
+  _ELKSTATUSDTO._serialized_end=15593
+  _GETELKSTACKSTATUSMSG._serialized_start=15595
+  _GETELKSTACKSTATUSMSG._serialized_end=15658
+  _STOPELKMANAGERMSG._serialized_start=15660
+  _STOPELKMANAGERMSG._serialized_end=15720
+  _STARTELKMANAGERMSG._serialized_start=15722
+  _STARTELKMANAGERMSG._serialized_end=15783
+  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_start=15785
+  _GETDOCKERSTATSMANAGERSINFOMSG._serialized_end=15857
+  _DOCKERSTATSMANAGERSINFODTO._serialized_start=15860
+  _DOCKERSTATSMANAGERSINFODTO._serialized_end=16063
+  _REMOVEALLDOCKERNETWORKSMSG._serialized_start=16065
+  _REMOVEALLDOCKERNETWORKSMSG._serialized_end=16093
+  _REMOVEDOCKERNETWORKSMSG._serialized_start=16095
+  _REMOVEDOCKERNETWORKSMSG._serialized_end=16138
+  _DOCKERSTATSMONITORSTATUSDTO._serialized_start=16140
+  _DOCKERSTATSMONITORSTATUSDTO._serialized_end=16241
+  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_start=16243
+  _GETDOCKERSTATSMANAGERSTATUSMSG._serialized_end=16289
+  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_start=16291
+  _STOPDOCKERSTATSMANAGERTHREADMSG._serialized_end=16365
+  _CREATEEMULATIONNETWORKSMSG._serialized_start=16367
+  _CREATEEMULATIONNETWORKSMSG._serialized_end=16436
+  _LISTALLSTOPPEDCONTAINERSMSG._serialized_start=16438
+  _LISTALLSTOPPEDCONTAINERSMSG._serialized_end=16467
+  _STOPPEDCONTAINERSDTO._serialized_start=16469
+  _STOPPEDCONTAINERSDTO._serialized_end=16539
+  _LISTALLRUNNINGEMULATIONSMSG._serialized_start=16541
+  _LISTALLRUNNINGEMULATIONSMSG._serialized_end=16570
+  _RUNNINGEMULATIONSDTO._serialized_start=16572
+  _RUNNINGEMULATIONSDTO._serialized_end=16621
+  _LISTALLRUNNINGCONTAINERSMSG._serialized_start=16623
+  _LISTALLRUNNINGCONTAINERSMSG._serialized_end=16652
+  _RUNNINGCONTAINERSDTO._serialized_start=16654
+  _RUNNINGCONTAINERSDTO._serialized_end=16724
+  _DOCKERCONTAINERDTO._serialized_start=16726
+  _DOCKERCONTAINERDTO._serialized_end=16787
+  _STARTCONTAINERMSG._serialized_start=16789
+  _STARTCONTAINERMSG._serialized_end=16822
+  _STARTALLSTOPPEDCONTAINERSMSG._serialized_start=16824
+  _STARTALLSTOPPEDCONTAINERSMSG._serialized_end=16854
+  _LISTALLDOCKERNETWORKSMSG._serialized_start=16856
+  _LISTALLDOCKERNETWORKSMSG._serialized_end=16882
+  _DOCKERNETWORKSDTO._serialized_start=16884
+  _DOCKERNETWORKSDTO._serialized_end=16942
+  _CONTAINERIMAGESDTO._serialized_start=16944
+  _CONTAINERIMAGESDTO._serialized_end=17000
+  _CONTAINERIMAGEDTO._serialized_start=17002
+  _CONTAINERIMAGEDTO._serialized_end=17104
+  _LISTALLCONTAINERIMAGESMSG._serialized_start=17106
+  _LISTALLCONTAINERIMAGESMSG._serialized_end=17133
+  _REMOVECONTAINERIMAGEMSG._serialized_start=17135
+  _REMOVECONTAINERIMAGEMSG._serialized_end=17174
+  _REMOVEALLCONTAINERIMAGESMSG._serialized_start=17176
+  _REMOVEALLCONTAINERIMAGESMSG._serialized_end=17205
+  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_start=17207
+  _REMOVEALLSTOPPEDCONTAINERSMSG._serialized_end=17238
+  _REMOVECONTAINERMSG._serialized_start=17240
+  _REMOVECONTAINERMSG._serialized_end=17274
+  _STOPCONTAINERMSG._serialized_start=17276
+  _STOPCONTAINERMSG._serialized_end=17308
+  _STOPALLRUNNINGCONTAINERSMSG._serialized_start=17310
+  _STOPALLRUNNINGCONTAINERSMSG._serialized_end=17339
+  _GETTRAFFICMANAGERSINFOMSG._serialized_start=17341
+  _GETTRAFFICMANAGERSINFOMSG._serialized_end=17409
+  _TRAFFICMANAGERSINFODTO._serialized_start=17412
+  _TRAFFICMANAGERSINFODTO._serialized_end=17597
+  _TRAFFICMANAGERINFODTO._serialized_start=17599
+  _TRAFFICMANAGERINFODTO._serialized_end=17655
+  _CLIENTMANAGERSINFODTO._serialized_start=17658
+  _CLIENTMANAGERSINFODTO._serialized_end=17835
+  _GETCLIENTMANAGERSINFOMSG._serialized_start=17837
+  _GETCLIENTMANAGERSINFOMSG._serialized_end=17904
+  _STARTTRAFFICGENERATORMSG._serialized_start=17906
+  _STARTTRAFFICGENERATORMSG._serialized_end=17994
+  _STOPTRAFFICGENERATORMSG._serialized_start=17996
+  _STOPTRAFFICGENERATORMSG._serialized_end=18083
+  _STOPTRAFFICGENERATORSMSG._serialized_start=18085
+  _STOPTRAFFICGENERATORSMSG._serialized_end=18152
+  _GETNUMCLIENTSDTO._serialized_start=18155
+  _GETNUMCLIENTSDTO._serialized_end=18329
+  _GETNUMACTIVECLIENTSMSG._serialized_start=18331
+  _GETNUMACTIVECLIENTSMSG._serialized_end=18396
+  _STOPCLIENTPOPULATIONMSG._serialized_start=18398
+  _STOPCLIENTPOPULATIONMSG._serialized_end=18464
+  _STOPCLIENTMANAGERMSG._serialized_start=18466
+  _STOPCLIENTMANAGERMSG._serialized_end=18529
+  _STARTCLIENTMANAGERMSG._serialized_start=18531
+  _STARTCLIENTMANAGERMSG._serialized_end=18595
+  _STOPTRAFFICMANAGERSMSG._serialized_start=18597
+  _STOPTRAFFICMANAGERSMSG._serialized_end=18662
+  _STOPTRAFFICMANAGERMSG._serialized_start=18664
+  _STOPTRAFFICMANAGERMSG._serialized_end=18749
+  _STARTTRAFFICMANAGERMSG._serialized_start=18751
+  _STARTTRAFFICMANAGERMSG._serialized_end=18837
+  _CLEANALLEXECUTIONSMSG._serialized_start=18839
+  _CLEANALLEXECUTIONSMSG._serialized_end=18862
+  _STOPALLEXECUTIONSMSG._serialized_start=18864
+  _STOPALLEXECUTIONSMSG._serialized_end=18886
+  _STOPEXECUTIONMSG._serialized_start=18888
+  _STOPEXECUTIONMSG._serialized_end=18947
+  _CLEANEXECUTIONMSG._serialized_start=18949
+  _CLEANEXECUTIONMSG._serialized_end=19009
+  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_start=19011
+  _STOPALLEXECUTIONSOFEMULATIONMSG._serialized_end=19063
+  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_start=19065
+  _CLEANALLEXECUTIONSOFEMULATIONMSG._serialized_end=19118
+  _GETCSLELOGFILESMSG._serialized_start=19120
+  _GETCSLELOGFILESMSG._serialized_end=19140
+  _GETLOGFILEMSG._serialized_start=19142
+  _GETLOGFILEMSG._serialized_end=19171
+  _STARTCONTAINERSINEXECUTIONMSG._serialized_start=19173
+  _STARTCONTAINERSINEXECUTIONMSG._serialized_end=19245
+  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_start=19247
+  _ATTACHCONTAINERSTONETWORKSINEXECUTIONMSG._serialized_end=19330
+  _INSTALLLIBRARIESMSG._serialized_start=19332
+  _INSTALLLIBRARIESMSG._serialized_end=19394
+  _APPLYKAFKACONFIGMSG._serialized_start=19396
+  _APPLYKAFKACONFIGMSG._serialized_end=19458
+  _STARTSDNCONTROLLERMSG._serialized_start=19460
+  _STARTSDNCONTROLLERMSG._serialized_end=19524
+  _APPLYRESOUCECONSTRAINTSMSG._serialized_start=19526
+  _APPLYRESOUCECONSTRAINTSMSG._serialized_end=19595
+  _CREATEOVSSWITCHESMSG._serialized_start=19597
+  _CREATEOVSSWITCHESMSG._serialized_end=19660
+  _PINGEXECUTIONMSG._serialized_start=19662
+  _PINGEXECUTIONMSG._serialized_end=19721
+  _CONFIGUREOVSMSG._serialized_start=19723
+  _CONFIGUREOVSMSG._serialized_end=19781
+  _STARTSDNCONTROLLERMONITORMSG._serialized_start=19783
+  _STARTSDNCONTROLLERMONITORMSG._serialized_end=19854
+  _CREATEUSERSMSG._serialized_start=19856
+  _CREATEUSERSMSG._serialized_end=19913
+  _CREATEVULNSMSG._serialized_start=19915
+  _CREATEVULNSMSG._serialized_end=19972
+  _CREATEFLAGSMSG._serialized_start=19974
+  _CREATEFLAGSMSG._serialized_end=20031
+  _CREATETOPOLOGYMSG._serialized_start=20033
+  _CREATETOPOLOGYMSG._serialized_end=20093
+  _STARTTRAFFICMANAGERSMSG._serialized_start=20095
+  _STARTTRAFFICMANAGERSMSG._serialized_end=20161
+  _STARTTRAFFICGENERATORSMSG._serialized_start=20163
+  _STARTTRAFFICGENERATORSMSG._serialized_end=20231
+  _STARTCLIENTPOPULATIONMSG._serialized_start=20233
+  _STARTCLIENTPOPULATIONMSG._serialized_end=20300
+  _STARTKAFKACLIENTPRODUCERMSG._serialized_start=20302
+  _STARTKAFKACLIENTPRODUCERMSG._serialized_end=20372
+  _STOPKAFKACLIENTPRODUCERMSG._serialized_start=20374
+  _STOPKAFKACLIENTPRODUCERMSG._serialized_end=20443
+  _STARTSNORTIDSESMSG._serialized_start=20445
+  _STARTSNORTIDSESMSG._serialized_end=20506
+  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_start=20508
+  _STARTSNORTIDSESMONITORTHREADSMSG._serialized_end=20583
+  _STARTOSSECIDSESMSG._serialized_start=20585
+  _STARTOSSECIDSESMSG._serialized_end=20646
+  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_start=20648
+  _STARTOSSECIDSESMONITORTHREADSMSG._serialized_end=20723
+  _STARTELKSTACKMSG._serialized_start=20725
+  _STARTELKSTACKMSG._serialized_end=20784
+  _STARTHOSTMANAGERSMSG._serialized_start=20786
+  _STARTHOSTMANAGERSMSG._serialized_end=20849
+  _APPLYFILEBEATCONFIGSMSG._serialized_start=20851
+  _APPLYFILEBEATCONFIGSMSG._serialized_end=20917
+  _APPLYPACKETBEATCONFIGSMSG._serialized_start=20919
+  _APPLYPACKETBEATCONFIGSMSG._serialized_end=20987
+  _APPLYMETRICBEATCONFIGSMSG._serialized_start=20989
+  _APPLYMETRICBEATCONFIGSMSG._serialized_end=21057
+  _APPLYHEARTBEATCONFIGSMSG._serialized_start=21059
+  _APPLYHEARTBEATCONFIGSMSG._serialized_end=21126
+  _STARTFILEBEATSMSG._serialized_start=21128
+  _STARTFILEBEATSMSG._serialized_end=21210
+  _STARTPACKETBEATSMSG._serialized_start=21212
+  _STARTPACKETBEATSMSG._serialized_end=21296
+  _STARTMETRICBEATSMSG._serialized_start=21298
+  _STARTMETRICBEATSMSG._serialized_end=21382
+  _STARTHEARTBEATSMSG._serialized_start=21384
+  _STARTHEARTBEATSMSG._serialized_end=21467
+  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_start=21469
+  _GETDOCKERSTATSMANAGERLOGSMSG._serialized_end=21499
+  _GETPROMETHEUSLOGSMSG._serialized_start=21501
+  _GETPROMETHEUSLOGSMSG._serialized_end=21523
+  _GETNODEEXPORTERLOGSMSG._serialized_start=21525
+  _GETNODEEXPORTERLOGSMSG._serialized_end=21549
+  _GETCADVISORLOGSMSG._serialized_start=21551
+  _GETCADVISORLOGSMSG._serialized_end=21571
+  _GETPGADMINLOGSMSG._serialized_start=21573
+  _GETPGADMINLOGSMSG._serialized_end=21592
+  _GETGRAFANALOGSMSG._serialized_start=21594
+  _GETGRAFANALOGSMSG._serialized_end=21613
+  _GETNGINXLOGSMSG._serialized_start=21615
+  _GETNGINXLOGSMSG._serialized_end=21632
+  _GETDOCKERLOGSMSG._serialized_start=21634
+  _GETDOCKERLOGSMSG._serialized_end=21652
+  _GETPOSTGRESQLLOGSMSG._serialized_start=21654
+  _GETPOSTGRESQLLOGSMSG._serialized_end=21676
+  _GETFLASKLOGSMSG._serialized_start=21678
+  _GETFLASKLOGSMSG._serialized_end=21695
+  _LOGSDTO._serialized_start=21697
+  _LOGSDTO._serialized_end=21720
+  _OPERATIONOUTCOMEDTO._serialized_start=21722
+  _OPERATIONOUTCOMEDTO._serialized_end=21760
+  _GETNODESTATUSMSG._serialized_start=21762
+  _GETNODESTATUSMSG._serialized_end=21780
+  _NODESTATUSDTO._serialized_start=21783
+  _NODESTATUSDTO._serialized_end=22090
+  _SERVICESTATUSDTO._serialized_start=22092
+  _SERVICESTATUSDTO._serialized_end=22127
+  _STARTPOSTGRESQLMSG._serialized_start=22129
+  _STARTPOSTGRESQLMSG._serialized_end=22149
+  _STARTCADVISORMSG._serialized_start=22151
+  _STARTCADVISORMSG._serialized_end=22169
+  _STARTNODEEXPORTERMSG._serialized_start=22171
+  _STARTNODEEXPORTERMSG._serialized_end=22193
+  _STARTGRAFANAMSG._serialized_start=22195
+  _STARTGRAFANAMSG._serialized_end=22212
+  _STARTPROMETHEUSMSG._serialized_start=22214
+  _STARTPROMETHEUSMSG._serialized_end=22234
+  _STARTPGADMINMSG._serialized_start=22236
+  _STARTPGADMINMSG._serialized_end=22253
+  _STARTNGINXMSG._serialized_start=22255
+  _STARTNGINXMSG._serialized_end=22270
+  _STARTFLASKMSG._serialized_start=22272
+  _STARTFLASKMSG._serialized_end=22287
+  _STARTDOCKERSTATSMANAGERMSG._serialized_start=22289
+  _STARTDOCKERSTATSMANAGERMSG._serialized_end=22317
+  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_start=22319
+  _STARTDOCKERSTATSMANAGERTHREADMSG._serialized_end=22394
+  _STARTDOCKERENGINEMSG._serialized_start=22396
+  _STARTDOCKERENGINEMSG._serialized_end=22418
+  _STOPPOSTGRESQLMSG._serialized_start=22420
+  _STOPPOSTGRESQLMSG._serialized_end=22439
+  _STOPCADVISORMSG._serialized_start=22441
+  _STOPCADVISORMSG._serialized_end=22458
+  _STOPNODEEXPORTERMSG._serialized_start=22460
+  _STOPNODEEXPORTERMSG._serialized_end=22481
+  _STOPGRAFANAMSG._serialized_start=22483
+  _STOPGRAFANAMSG._serialized_end=22499
+  _STOPPROMETHEUSMSG._serialized_start=22501
+  _STOPPROMETHEUSMSG._serialized_end=22520
+  _STOPPGADMINMSG._serialized_start=22522
+  _STOPPGADMINMSG._serialized_end=22538
+  _STOPNGINXMSG._serialized_start=22540
+  _STOPNGINXMSG._serialized_end=22554
+  _STOPFLASKMSG._serialized_start=22556
+  _STOPFLASKMSG._serialized_end=22570
+  _STOPDOCKERSTATSMANAGERMSG._serialized_start=22572
+  _STOPDOCKERSTATSMANAGERMSG._serialized_end=22599
+  _STOPDOCKERENGINEMSG._serialized_start=22601
+  _STOPDOCKERENGINEMSG._serialized_end=22622
+  _CLUSTERMANAGER._serialized_start=22625
+  _CLUSTERMANAGER._serialized_end=36920
 # @@protoc_insertion_point(module_scope)
```

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -993,15 +993,15 @@
             ips=elk_managers_dto.ips,
             ports=elk_managers_dto.ports,
             emulationName=elk_managers_dto.emulation_name,
             executionId=elk_managers_dto.execution_id,
             elkManagersRunning=elk_managers_dto.elk_managers_running,
             elkManagersStatuses=list(map(
                 lambda x: ClusterManagerUtil.convert_elk_dto(x), elk_managers_dto.elk_managers_statuses)),
-            localKibanaPort=elk_managers_dto.local_kibana_port
+            localKibanaPort=elk_managers_dto.local_kibana_port, physicalServerIp=elk_managers_dto.physical_server_ip
         )
 
     @staticmethod
     def convert_elk_info_dto_reverse(elk_managers_dto: cluster_manager_pb2.ElkManagersInfoDTO) -> ELKManagersInfo:
         """
         Converts a ELKManagersInfo into a ElkManagersInfoDTO
 
@@ -1014,15 +1014,16 @@
             ips=elk_managers_dto.ips,
             ports=elk_managers_dto.ports,
             emulation_name=elk_managers_dto.emulationName,
             execution_id=elk_managers_dto.executionId,
             elk_managers_running=elk_managers_dto.elkManagersRunning,
             elk_managers_statuses=list(map(
                 lambda x: ClusterManagerUtil.convert_elk_dto_reverse(x), elk_managers_dto.elkManagersStatuses)),
-            local_kibana_port=elk_managers_dto.localKibanaPort
+            local_kibana_port=elk_managers_dto.localKibanaPort,
+            physical_server_ip=elk_managers_dto.physicalServerIp
         )
 
     @staticmethod
     def convert_ryu_info_dto(ryu_managers_info_dto: RyuManagersInfo) -> cluster_manager_pb2.RyuManagersInfoDTO:
         """
         Converts a RyuManagersInfo into a RyuManagersInfoDTO
 
@@ -1035,15 +1036,17 @@
             ips=ryu_managers_info_dto.ips,
             ports=ryu_managers_info_dto.ports,
             emulationName=ryu_managers_info_dto.emulation_name,
             executionId=ryu_managers_info_dto.execution_id,
             ryuManagersRunning=ryu_managers_info_dto.ryu_managers_running,
             ryuManagersStatuses=list(
                 map(lambda x: ClusterManagerUtil.convert_ryu_dto_to_ryu_status_dto(x),
-                    ryu_managers_info_dto.ryu_managers_statuses))
+                    ryu_managers_info_dto.ryu_managers_statuses)),
+            physicalServerIp=ryu_managers_info_dto.physical_server_ip,
+            localControllerWebPort=ryu_managers_info_dto.local_controller_web_port
         )
 
     @staticmethod
     def convert_ryu_info_dto_reverse(ryu_managers_info_dto: cluster_manager_pb2.RyuManagersInfoDTO) -> RyuManagersInfo:
         """
         Converts a RyuManagersInfoDTO into a RyuManagersInfo
 
@@ -1056,15 +1059,17 @@
             ips=ryu_managers_info_dto.ips,
             ports=ryu_managers_info_dto.ports,
             emulation_name=ryu_managers_info_dto.emulationName,
             execution_id=ryu_managers_info_dto.executionId,
             ryu_managers_running=ryu_managers_info_dto.ryuManagersRunning,
             ryu_managers_statuses=list(
                 map(lambda x: ClusterManagerUtil.convert_ryu_dto_to_ryu_status_dto_reverse(x),
-                    ryu_managers_info_dto.ryuManagersStatuses))
+                    ryu_managers_info_dto.ryuManagersStatuses)),
+            physical_server_ip=ryu_managers_info_dto.physicalServerIp,
+            local_controller_web_port=ryu_managers_info_dto.localControllerWebPort
         )
 
     @staticmethod
     def convert_host_info_dto(host_managers_dto: HostManagersInfo) -> cluster_manager_pb2.HostManagersInfoDTO:
         """
         Converts a HostManagersInfo into a HostManagersInfoDTO
 
@@ -1432,24 +1437,25 @@
     @staticmethod
     def get_empty_elk_managers_info_dto() -> cluster_manager_pb2.ElkManagersInfoDTO:
         """
         :return: an empty ElkManagersInfoDTO
         """
         return cluster_manager_pb2.ElkManagersInfoDTO(
             ips=[], ports=[], emulationName="", executionId="", elkManagersRunning=[], elkManagersStatuses=[],
-            localKibanaPort=-1
+            localKibanaPort=-1, physicalServerIp = ""
         )
 
     @staticmethod
     def get_empty_ryu_managers_info_dto() -> cluster_manager_pb2.RyuManagersInfoDTO:
         """
         :return: an empty RyuManagersInfoDTO
         """
         return cluster_manager_pb2.RyuManagersInfoDTO(
-            ips=[], ports=[], emulationName="", executionId=-1, ryuManagersRunning=[], ryuManagersStatuses=[]
+            ips=[], ports=[], emulationName="", executionId=-1, ryuManagersRunning=[], ryuManagersStatuses=[],
+            physicalServerIp = "", localControllerWebPort=-1
         )
 
     @staticmethod
     def get_empty_host_managers_info_dto() -> cluster_manager_pb2.HostManagersInfoDTO:
         """
         :return: an empty HostManagersInfoDTO
         """
```

### Comparing `csle_cluster-0.1.8/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.1.9/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.1.8/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.1.9/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.1.8/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.1.9/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

