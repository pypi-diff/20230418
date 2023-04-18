# Comparing `tmp/azure-mgmt-rdbms-9.1.0.zip` & `tmp/azure-mgmt-rdbms-9.1.0b1.zip`

## zipinfo {}

```diff
@@ -1,294 +1,294 @@
-Zip file size: 676009 bytes, number of entries: 292
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/
--rw-rw-r--  2.0 unx      126 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/MANIFEST.in
--rw-rw-r--  2.0 unx     1288 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/README.md
--rw-rw-r--  2.0 unx    23440 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/PKG-INFO
--rw-rw-r--  2.0 unx       67 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/setup.cfg
--rw-rw-r--  2.0 unx     2898 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/setup.py
--rw-rw-r--  2.0 unx    17554 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/CHANGELOG.md
--rw-rw-r--  2.0 unx      570 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/_meta.json
--rw-rw-r--  2.0 unx    17479 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mariadb.py
--rw-rw-r--  2.0 unx    12802 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mysql.py
--rw-rw-r--  2.0 unx    12099 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_postgresql.py
--rw-rw-r--  2.0 unx        1 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx      105 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/requires.txt
--rw-rw-r--  2.0 unx    23440 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    17487 b- defN 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/SOURCES.txt
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/
--rw-rw-r--  2.0 unx       64 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/
--rw-rw-r--  2.0 unx       64 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/
--rw-rw-r--  2.0 unx      345 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/_version.py
--rw-rw-r--  2.0 unx       22 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/
--rw-rw-r--  2.0 unx     3237 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_configuration.py
--rw-rw-r--  2.0 unx    10179 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_version.py
--rw-rw-r--  2.0 unx      734 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/
--rw-rw-r--  2.0 unx     3181 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_configuration.py
--rw-rw-r--  2.0 unx    10202 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py
--rw-rw-r--  2.0 unx      580 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/__init__.py
--rw-rw-r--  2.0 unx     4807 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3789 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     5321 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     4679 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21547 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    21414 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py
--rw-rw-r--  2.0 unx    15901 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     8720 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    21174 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py
--rw-rw-r--  2.0 unx    16624 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8842 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    21916 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5552 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5625 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    29894 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     2365 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5557 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx    22220 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    35246 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py
--rw-rw-r--  2.0 unx    87286 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models.py
--rw-rw-r--  2.0 unx    94652 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models_py3.py
--rw-rw-r--  2.0 unx     9295 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/__init__.py
--rw-rw-r--  2.0 unx     5674 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py
--rw-rw-r--  2.0 unx     4934 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3908 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_operations.py
--rw-rw-r--  2.0 unx     5389 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     4814 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21723 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    21590 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py
--rw-rw-r--  2.0 unx    16043 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     8838 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    21310 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py
--rw-rw-r--  2.0 unx    16766 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8951 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    22092 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5628 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5701 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    30120 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     2365 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/__init__.py
--rw-rw-r--  2.0 unx     5633 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx    22396 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    35412 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/
--rw-rw-r--  2.0 unx     3277 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py
--rw-rw-r--  2.0 unx     7077 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py
--rw-rw-r--  2.0 unx      486 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_version.py
--rw-rw-r--  2.0 unx      734 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/
--rw-rw-r--  2.0 unx     3221 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py
--rw-rw-r--  2.0 unx     7064 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py
--rw-rw-r--  2.0 unx      580 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py
--rw-rw-r--  2.0 unx     4855 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3821 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     3732 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
--rw-rw-r--  2.0 unx    21641 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    23038 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx    22092 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     1400 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5349 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
--rw-rw-r--  2.0 unx     5150 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py
--rw-rw-r--  2.0 unx    46983 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py
--rw-rw-r--  2.0 unx    57299 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py
--rw-rw-r--  2.0 unx    59917 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py
--rw-rw-r--  2.0 unx     6320 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py
--rw-rw-r--  2.0 unx     3946 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py
--rw-rw-r--  2.0 unx     4982 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3940 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py
--rw-rw-r--  2.0 unx     3851 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
--rw-rw-r--  2.0 unx    21817 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    23230 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx    22268 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     1400 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py
--rw-rw-r--  2.0 unx     5417 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py
--rw-rw-r--  2.0 unx     5285 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py
--rw-rw-r--  2.0 unx    47197 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/
--rw-rw-r--  2.0 unx     3222 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_configuration.py
--rw-rw-r--  2.0 unx      486 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_version.py
--rw-rw-r--  2.0 unx    12964 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_my_sql_management_client.py
--rw-rw-r--  2.0 unx      719 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/
--rw-rw-r--  2.0 unx     3166 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_configuration.py
--rw-rw-r--  2.0 unx    13015 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py
--rw-rw-r--  2.0 unx      565 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/__init__.py
--rw-rw-r--  2.0 unx     4787 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3774 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     5306 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     5687 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py
--rw-rw-r--  2.0 unx    10435 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py
--rw-rw-r--  2.0 unx     9551 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py
--rw-rw-r--  2.0 unx     4659 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21492 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py
--rw-rw-r--  2.0 unx     9583 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py
--rw-rw-r--  2.0 unx    21324 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py
--rw-rw-r--  2.0 unx    15856 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     9500 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py
--rw-rw-r--  2.0 unx     8807 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py
--rw-rw-r--  2.0 unx     4736 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
--rw-rw-r--  2.0 unx     8685 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    21119 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py
--rw-rw-r--  2.0 unx    16569 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8817 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    21861 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5537 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5605 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    29819 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     3392 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5542 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx     8518 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py
--rw-rw-r--  2.0 unx    22165 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    52367 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py
--rw-rw-r--  2.0 unx     5830 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py
--rw-rw-r--  2.0 unx   108922 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models.py
--rw-rw-r--  2.0 unx   117724 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models_py3.py
--rw-rw-r--  2.0 unx    11720 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/__init__.py
--rw-rw-r--  2.0 unx     4914 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3893 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_operations.py
--rw-rw-r--  2.0 unx     5374 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     5763 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py
--rw-rw-r--  2.0 unx    10608 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py
--rw-rw-r--  2.0 unx     9691 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py
--rw-rw-r--  2.0 unx     4794 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21668 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_databases_operations.py
--rw-rw-r--  2.0 unx     9709 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py
--rw-rw-r--  2.0 unx    21500 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py
--rw-rw-r--  2.0 unx    15998 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     9626 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py
--rw-rw-r--  2.0 unx     8933 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py
--rw-rw-r--  2.0 unx     4871 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py
--rw-rw-r--  2.0 unx     8803 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    21255 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py
--rw-rw-r--  2.0 unx    16711 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8926 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    22037 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5613 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5681 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    30045 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     3392 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/__init__.py
--rw-rw-r--  2.0 unx     5618 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx     8636 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py
--rw-rw-r--  2.0 unx    22341 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    52603 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_servers_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/
--rw-rw-r--  2.0 unx     3228 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_configuration.py
--rw-rw-r--  2.0 unx      486 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_version.py
--rw-rw-r--  2.0 unx    12342 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py
--rw-rw-r--  2.0 unx      725 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/
--rw-rw-r--  2.0 unx     3172 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_configuration.py
--rw-rw-r--  2.0 unx    12385 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py
--rw-rw-r--  2.0 unx      571 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/__init__.py
--rw-rw-r--  2.0 unx     4795 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3780 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     5312 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     5695 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py
--rw-rw-r--  2.0 unx     9617 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py
--rw-rw-r--  2.0 unx     4695 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21682 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py
--rw-rw-r--  2.0 unx     9651 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py
--rw-rw-r--  2.0 unx    15986 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     9568 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py
--rw-rw-r--  2.0 unx    10529 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py
--rw-rw-r--  2.0 unx     8873 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py
--rw-rw-r--  2.0 unx     4742 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
--rw-rw-r--  2.0 unx     8755 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    16703 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8883 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    22051 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5571 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5641 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    30073 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     3196 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5576 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx     8584 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py
--rw-rw-r--  2.0 unx    22355 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    46608 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py
--rw-rw-r--  2.0 unx    98438 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models.py
--rw-rw-r--  2.0 unx     4855 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py
--rw-rw-r--  2.0 unx   106073 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models_py3.py
--rw-rw-r--  2.0 unx    10709 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/__init__.py
--rw-rw-r--  2.0 unx     4922 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     3899 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_operations.py
--rw-rw-r--  2.0 unx     5380 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx     5771 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py
--rw-rw-r--  2.0 unx     9757 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py
--rw-rw-r--  2.0 unx     4830 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py
--rw-rw-r--  2.0 unx    21858 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py
--rw-rw-r--  2.0 unx     9777 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py
--rw-rw-r--  2.0 unx    16128 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     9694 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py
--rw-rw-r--  2.0 unx    10702 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py
--rw-rw-r--  2.0 unx     8999 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py
--rw-rw-r--  2.0 unx     4877 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py
--rw-rw-r--  2.0 unx     8873 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx    16845 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py
--rw-rw-r--  2.0 unx     8992 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py
--rw-rw-r--  2.0 unx    22227 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5647 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     5717 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py
--rw-rw-r--  2.0 unx    30299 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     3196 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/__init__.py
--rw-rw-r--  2.0 unx     5652 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py
--rw-rw-r--  2.0 unx     8702 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py
--rw-rw-r--  2.0 unx    22531 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py
--rw-rw-r--  2.0 unx    46810 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/
--rw-rw-r--  2.0 unx     3262 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py
--rw-rw-r--  2.0 unx      486 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_version.py
--rw-rw-r--  2.0 unx     7623 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py
--rw-rw-r--  2.0 unx      719 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-03 01:43 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/
--rw-rw-r--  2.0 unx     3206 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py
--rw-rw-r--  2.0 unx     7618 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py
--rw-rw-r--  2.0 unx      565 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py
--rw-rw-r--  2.0 unx     5061 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     4695 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py
--rw-rw-r--  2.0 unx     3929 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
--rw-rw-r--  2.0 unx    21646 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    22785 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     8604 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py
--rw-rw-r--  2.0 unx     5140 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py
--rw-rw-r--  2.0 unx    22008 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5603 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     1571 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     5325 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
--rw-rw-r--  2.0 unx    52282 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py
--rw-rw-r--  2.0 unx     3956 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py
--rw-rw-r--  2.0 unx    56298 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py
--rw-rw-r--  2.0 unx    59452 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py
--rw-rw-r--  2.0 unx     6534 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py
--rw-rw-r--  2.0 unx     5196 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py
--rw-rw-r--  2.0 unx     4755 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py
--rw-rw-r--  2.0 unx     4048 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
--rw-rw-r--  2.0 unx    21822 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py
--rw-rw-r--  2.0 unx    22961 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py
--rw-rw-r--  2.0 unx     8722 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py
--rw-rw-r--  2.0 unx     5275 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py
--rw-rw-r--  2.0 unx    22184 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py
--rw-rw-r--  2.0 unx     5679 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py
--rw-rw-r--  2.0 unx     1571 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py
--rw-rw-r--  2.0 unx     5393 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py
--rw-rw-r--  2.0 unx    52518 b- defN 21-Sep-03 01:41 azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py
-292 files, 3602850 bytes uncompressed, 603799 bytes compressed:  83.3%
+Zip file size: 677708 bytes, number of entries: 292
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/
+-rw-rw-r--  2.0 unx      580 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/_meta.json
+-rw-rw-r--  2.0 unx     1288 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/README.md
+-rw-rw-r--  2.0 unx    23316 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx    17476 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx      126 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     2898 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/setup.py
+-rw-rw-r--  2.0 unx       67 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/setup.cfg
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/
+-rw-rw-r--  2.0 unx       64 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/
+-rw-rw-r--  2.0 unx       64 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/
+-rw-rw-r--  2.0 unx       22 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/__init__.py
+-rw-rw-r--  2.0 unx      347 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/
+-rw-rw-r--  2.0 unx      719 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py
+-rw-rw-r--  2.0 unx     7623 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py
+-rw-rw-r--  2.0 unx     3270 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/
+-rw-rw-r--  2.0 unx      565 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py
+-rw-rw-r--  2.0 unx     7618 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py
+-rw-rw-r--  2.0 unx     3214 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3937 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
+-rw-rw-r--  2.0 unx     5333 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
+-rw-rw-r--  2.0 unx     1571 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     5611 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    52362 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5069 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     5148 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py
+-rw-rw-r--  2.0 unx    22040 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8620 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py
+-rw-rw-r--  2.0 unx     4703 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    21678 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx    22817 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     4056 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
+-rw-rw-r--  2.0 unx     5401 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py
+-rw-rw-r--  2.0 unx     1571 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py
+-rw-rw-r--  2.0 unx     5687 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    52598 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5204 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     5283 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py
+-rw-rw-r--  2.0 unx    22216 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8738 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py
+-rw-rw-r--  2.0 unx     4763 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py
+-rw-rw-r--  2.0 unx    21854 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx    22993 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     3980 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py
+-rw-rw-r--  2.0 unx     6638 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py
+-rw-rw-r--  2.0 unx    57604 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py
+-rw-rw-r--  2.0 unx    60812 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/
+-rw-rw-r--  2.0 unx      734 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/__init__.py
+-rw-rw-r--  2.0 unx    10179 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py
+-rw-rw-r--  2.0 unx     3237 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/
+-rw-rw-r--  2.0 unx      580 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/__init__.py
+-rw-rw-r--  2.0 unx    10202 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py
+-rw-rw-r--  2.0 unx     3181 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_configuration.py
+-rw-rw-r--  2.0 unx     8842 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     2365 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     8720 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    29894 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5552 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    21414 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py
+-rw-rw-r--  2.0 unx    35246 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5557 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4807 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4679 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22220 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx    21174 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py
+-rw-rw-r--  2.0 unx    21916 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     5625 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3789 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    21547 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5321 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16624 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    15901 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     8951 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     2365 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/__init__.py
+-rw-rw-r--  2.0 unx     8838 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    30120 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5628 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    21590 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py
+-rw-rw-r--  2.0 unx    35412 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5633 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4934 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4814 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22396 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx    21310 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py
+-rw-rw-r--  2.0 unx    22092 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     5701 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3908 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_operations.py
+-rw-rw-r--  2.0 unx    21723 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5389 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16766 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    16043 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     9295 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/__init__.py
+-rw-rw-r--  2.0 unx     5674 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py
+-rw-rw-r--  2.0 unx    87286 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models.py
+-rw-rw-r--  2.0 unx    94652 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/
+-rw-rw-r--  2.0 unx      725 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/__init__.py
+-rw-rw-r--  2.0 unx     3228 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_version.py
+-rw-rw-r--  2.0 unx    12342 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/
+-rw-rw-r--  2.0 unx      571 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/__init__.py
+-rw-rw-r--  2.0 unx     3172 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_configuration.py
+-rw-rw-r--  2.0 unx    12385 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py
+-rw-rw-r--  2.0 unx     9568 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py
+-rw-rw-r--  2.0 unx     5695 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py
+-rw-rw-r--  2.0 unx     8883 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     3196 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     4742 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+-rw-rw-r--  2.0 unx     8755 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    30073 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5571 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    10529 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py
+-rw-rw-r--  2.0 unx    46608 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5576 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4795 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4695 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22355 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx     8584 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py
+-rw-rw-r--  2.0 unx    22051 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8873 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py
+-rw-rw-r--  2.0 unx     9651 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py
+-rw-rw-r--  2.0 unx     9617 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py
+-rw-rw-r--  2.0 unx     5641 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3780 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    21682 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5312 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16703 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    15986 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     9694 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py
+-rw-rw-r--  2.0 unx     5771 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py
+-rw-rw-r--  2.0 unx     8992 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     3196 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/__init__.py
+-rw-rw-r--  2.0 unx     4877 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+-rw-rw-r--  2.0 unx     8873 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    30299 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5647 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    10702 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py
+-rw-rw-r--  2.0 unx    46810 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5652 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4922 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4830 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22531 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx     8702 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py
+-rw-rw-r--  2.0 unx    22227 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8999 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py
+-rw-rw-r--  2.0 unx     9777 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py
+-rw-rw-r--  2.0 unx     9757 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py
+-rw-rw-r--  2.0 unx     5717 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3899 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_operations.py
+-rw-rw-r--  2.0 unx    21858 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5380 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16845 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    16128 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx    10709 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/__init__.py
+-rw-rw-r--  2.0 unx    98438 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models.py
+-rw-rw-r--  2.0 unx     4855 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py
+-rw-rw-r--  2.0 unx   106073 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/
+-rw-rw-r--  2.0 unx      719 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/__init__.py
+-rw-rw-r--  2.0 unx    12964 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_my_sql_management_client.py
+-rw-rw-r--  2.0 unx     3222 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/
+-rw-rw-r--  2.0 unx      565 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/__init__.py
+-rw-rw-r--  2.0 unx    13015 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py
+-rw-rw-r--  2.0 unx     3166 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_configuration.py
+-rw-rw-r--  2.0 unx     9500 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py
+-rw-rw-r--  2.0 unx     5687 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py
+-rw-rw-r--  2.0 unx     8817 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     3392 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     4736 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+-rw-rw-r--  2.0 unx     8685 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    29819 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5537 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    21324 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py
+-rw-rw-r--  2.0 unx    52367 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5542 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4787 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4659 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22165 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx     8518 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py
+-rw-rw-r--  2.0 unx    21119 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py
+-rw-rw-r--  2.0 unx    21861 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8807 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py
+-rw-rw-r--  2.0 unx     9583 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py
+-rw-rw-r--  2.0 unx     9551 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py
+-rw-rw-r--  2.0 unx     5605 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3774 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    21492 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5306 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16569 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    10435 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py
+-rw-rw-r--  2.0 unx    15856 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     9626 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py
+-rw-rw-r--  2.0 unx     5763 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py
+-rw-rw-r--  2.0 unx     8926 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py
+-rw-rw-r--  2.0 unx     3392 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/__init__.py
+-rw-rw-r--  2.0 unx     4871 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+-rw-rw-r--  2.0 unx     8803 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    30045 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5613 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py
+-rw-rw-r--  2.0 unx    21500 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py
+-rw-rw-r--  2.0 unx    52603 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     5618 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py
+-rw-rw-r--  2.0 unx     4914 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx     4794 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py
+-rw-rw-r--  2.0 unx    22341 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py
+-rw-rw-r--  2.0 unx     8636 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py
+-rw-rw-r--  2.0 unx    21255 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py
+-rw-rw-r--  2.0 unx    22037 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     8933 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py
+-rw-rw-r--  2.0 unx     9709 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py
+-rw-rw-r--  2.0 unx     9691 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py
+-rw-rw-r--  2.0 unx     5681 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx     3893 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_operations.py
+-rw-rw-r--  2.0 unx    21668 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx     5374 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py
+-rw-rw-r--  2.0 unx    16711 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py
+-rw-rw-r--  2.0 unx    10608 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py
+-rw-rw-r--  2.0 unx    15998 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     5830 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py
+-rw-rw-r--  2.0 unx    11720 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/__init__.py
+-rw-rw-r--  2.0 unx   108866 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models.py
+-rw-rw-r--  2.0 unx   117668 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models_py3.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/
+-rw-rw-r--  2.0 unx      734 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py
+-rw-rw-r--  2.0 unx     7077 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py
+-rw-rw-r--  2.0 unx     3277 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py
+-rw-rw-r--  2.0 unx      488 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/
+-rw-rw-r--  2.0 unx      580 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py
+-rw-rw-r--  2.0 unx     7064 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py
+-rw-rw-r--  2.0 unx     3221 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3732 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
+-rw-rw-r--  2.0 unx     5349 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
+-rw-rw-r--  2.0 unx     1400 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     5150 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py
+-rw-rw-r--  2.0 unx    46983 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     4855 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx    22092 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     3821 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    21641 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx    23038 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     3851 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
+-rw-rw-r--  2.0 unx     5417 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py
+-rw-rw-r--  2.0 unx     1400 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py
+-rw-rw-r--  2.0 unx     5285 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py
+-rw-rw-r--  2.0 unx    47197 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py
+-rw-rw-r--  2.0 unx     4982 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py
+-rw-rw-r--  2.0 unx    22268 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py
+-rw-rw-r--  2.0 unx     3940 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py
+-rw-rw-r--  2.0 unx    21817 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py
+-rw-rw-r--  2.0 unx    23230 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py
+-rw-rw-r--  2.0 unx     6320 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py
+-rw-rw-r--  2.0 unx     3946 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py
+-rw-rw-r--  2.0 unx    57299 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py
+-rw-rw-r--  2.0 unx    59917 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py
+-rw-rw-r--  2.0 unx    12802 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mysql.py
+-rw-rw-r--  2.0 unx    17479 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mariadb.py
+-rw-rw-r--  2.0 unx    12099 b- defN 21-Jul-20 02:47 azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_postgresql.py
+-rw-rw-r--  2.0 unx        6 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    23316 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx    17487 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      105 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 21-Jul-20 02:50 azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/dependency_links.txt
+292 files, 3605724 bytes uncompressed, 604330 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -1,877 +1,877 @@
-Filename: azure-mgmt-rdbms-9.1.0/
+Filename: azure-mgmt-rdbms-9.1.0b1/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/tests/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/
+Filename: azure-mgmt-rdbms-9.1.0b1/tests/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/MANIFEST.in
+Filename: azure-mgmt-rdbms-9.1.0b1/_meta.json
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/README.md
+Filename: azure-mgmt-rdbms-9.1.0b1/README.md
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/PKG-INFO
+Filename: azure-mgmt-rdbms-9.1.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/setup.cfg
+Filename: azure-mgmt-rdbms-9.1.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/setup.py
+Filename: azure-mgmt-rdbms-9.1.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/CHANGELOG.md
+Filename: azure-mgmt-rdbms-9.1.0b1/setup.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/_meta.json
+Filename: azure-mgmt-rdbms-9.1.0b1/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mariadb.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mysql.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_postgresql.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/not-zip-safe
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/dependency_links.txt
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/requires.txt
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/PKG-INFO
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/top_level.txt
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/SOURCES.txt
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models_py3.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_my_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models_py3.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_my_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models_py3.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_version.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_version.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mysql.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mariadb.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_postgresql.py
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py
+Filename: azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-rdbms-9.1.0/README.md` & `azure-mgmt-rdbms-9.1.0b1/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/PKG-INFO` & `azure-mgmt-rdbms-9.1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-rdbms
-Version: 9.1.0
+Version: 9.1.0b1
 Summary: Microsoft Azure RDBMS Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -35,20 +35,14 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-rdbms%2FREADME.png)
         
         
         # Release History
         
-        ## 9.1.0 (2021-09-02)
-        
-        **Features**
-        
-          - Upgrade api-version to `2021-05-01`
-        
         ## 9.1.0b1 (2021-07-19)
         
         **Features**
         
           - Added operation group BackupsOperations
         
         ## 9.0.0 (2021-07-01)
```

## Comparing `azure-mgmt-rdbms-9.1.0/setup.py` & `azure-mgmt-rdbms-9.1.0b1/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/CHANGELOG.md` & `azure-mgmt-rdbms-9.1.0b1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # Release History
 
-## 9.1.0 (2021-09-02)
-
-**Features**
-
-  - Upgrade api-version to `2021-05-01`
-
 ## 9.1.0b1 (2021-07-19)
 
 **Features**
 
   - Added operation group BackupsOperations
 
 ## 9.0.0 (2021-07-01)
```

## Comparing `azure-mgmt-rdbms-9.1.0/_meta.json` & `azure-mgmt-rdbms-9.1.0b1/_meta.json`

 * *Files 26% similar despite different names*

### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/postgresql/resource-manager/readme.md --multiapi "*

 * *                       '--python --python-mode=update '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 '*

 * *                       '--use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 '*

 * *                       "--version=3.4.5'",*

 * * "'commit'": "'1a22ee0be121e33f98b6290cc737f613f2e1a2d8'",*

 * * "'readme'": "'specification/postgresql/resource-manager/readme. […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.4.5",
-    "autorest_command": "autorest specification/mysql/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 --use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 --version=3.4.5",
-    "commit": "5d442a18cbb7ede47abfd7ae8b7acc20cc1d7946",
-    "readme": "specification/mysql/resource-manager/readme.md",
+    "autorest_command": "autorest specification/postgresql/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 --use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 --version=3.4.5",
+    "commit": "1a22ee0be121e33f98b6290cc737f613f2e1a2d8",
+    "readme": "specification/postgresql/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
         "@autorest/python@5.8.4",
         "@autorest/modelerfour@4.19.2"
     ]
 }
```

## Comparing `azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mariadb.py` & `azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mariadb.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_mysql.py` & `azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_mysql.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/tests/test_cli_mgmt_postgresql.py` & `azure-mgmt-rdbms-9.1.0b1/tests/test_cli_mgmt_postgresql.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/PKG-INFO` & `azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-rdbms
-Version: 9.1.0
+Version: 9.1.0b1
 Summary: Microsoft Azure RDBMS Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -35,20 +35,14 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-rdbms%2FREADME.png)
         
         
         # Release History
         
-        ## 9.1.0 (2021-09-02)
-        
-        **Features**
-        
-          - Upgrade api-version to `2021-05-01`
-        
         ## 9.1.0b1 (2021-07-19)
         
         **Features**
         
           - Added operation group BackupsOperations
         
         ## 9.0.0 (2021-07-01)
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure_mgmt_rdbms.egg-info/SOURCES.txt` & `azure-mgmt-rdbms-9.1.0b1/azure_mgmt_rdbms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/_postgre_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/_postgre_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_keys_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_administrators_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/aio/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_models_py3.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/models/_postgre_sql_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_keys_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_administrators_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/_postgre_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/_postgre_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_location_based_capabilities_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_virtual_network_subnet_usage_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/aio/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/models/_postgre_sql_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_location_based_capabilities_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_virtual_network_subnet_usage_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/postgresql_flexibleservers/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/_my_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/_my_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/_my_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_result_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_my_sql_management_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recommended_actions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_top_query_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_keys_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_wait_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_query_texts_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_administrators_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_advisors_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_my_sql_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2001,16 +2001,15 @@
     :type public_network_access: str or ~azure.mgmt.rdbms.mysql.models.PublicNetworkAccessEnum
     :param storage_profile: Storage profile of a server.
     :type storage_profile: ~azure.mgmt.rdbms.mysql.models.StorageProfile
     :param create_mode: Required. The mode to create a new server.Constant filled by server.
      Possible values include: "Default", "PointInTimeRestore", "GeoRestore", "Replica".
     :type create_mode: str or ~azure.mgmt.rdbms.mysql.models.CreateMode
     :param administrator_login: Required. The administrator's login name of a server. Can only be
-     specified when the server is being created (and is required for creation). The login name is
-     required when updating password.
+     specified when the server is being created (and is required for creation).
     :type administrator_login: str
     :param administrator_login_password: Required. The password of the administrator login.
     :type administrator_login_password: str
     """
 
     _validation = {
         'create_mode': {'required': True},
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/_models_py3.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/_models_py3.py`

 * *Files 0% similar despite different names*

```diff
@@ -2152,16 +2152,15 @@
     :type public_network_access: str or ~azure.mgmt.rdbms.mysql.models.PublicNetworkAccessEnum
     :param storage_profile: Storage profile of a server.
     :type storage_profile: ~azure.mgmt.rdbms.mysql.models.StorageProfile
     :param create_mode: Required. The mode to create a new server.Constant filled by server.
      Possible values include: "Default", "PointInTimeRestore", "GeoRestore", "Replica".
     :type create_mode: str or ~azure.mgmt.rdbms.mysql.models.CreateMode
     :param administrator_login: Required. The administrator's login name of a server. Can only be
-     specified when the server is being created (and is required for creation). The login name is
-     required when updating password.
+     specified when the server is being created (and is required for creation).
     :type administrator_login: str
     :param administrator_login_password: Required. The password of the administrator login.
     :type administrator_login_password: str
     """
 
     _validation = {
         'create_mode': {'required': True},
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/models/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_result_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_my_sql_management_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recommended_actions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_top_query_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_keys_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_wait_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_query_texts_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_location_based_recommended_action_sessions_operation_status_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_administrators_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_advisors_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/_maria_db_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/_maria_db_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_result_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recommended_actions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_top_query_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_wait_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_maria_db_management_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_query_texts_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_location_based_recommended_action_sessions_operation_status_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_advisors_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/aio/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_maria_db_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/_models_py3.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/models/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_check_name_availability_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_result_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recommended_actions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_recoverable_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_databases_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_top_query_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_configurations_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_wait_statistics_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_maria_db_management_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_query_texts_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_location_based_recommended_action_sessions_operation_status_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_security_alert_policies_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_parameters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_firewall_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_replicas_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_server_based_performance_tier_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_log_files_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_advisors_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_virtual_network_rules_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mariadb/operations/_servers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(MySQLManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-05-01"
+        self.api_version = "2021-05-01-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-rdbms/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs  # type: Any
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/_my_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(MySQLManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-05-01"
+        self.api_version = "2021-05-01-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-rdbms/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs: Any
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/_my_sql_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_name_availability_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.NameAvailability"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_get_private_dns_zone_suffix_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.GetPrivateDnsZoneSuffixResponse"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
 
         # Construct parameters
         query_parameters = {}  # type: Dict[str, Any]
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_databases_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         **kwargs: Any
     ) -> Optional["_models.Database"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Database"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -187,15 +187,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -315,15 +315,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Database"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -374,15 +374,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.DatabaseListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_configurations_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         **kwargs: Any
     ) -> Optional["_models.Configuration"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Configuration"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -197,15 +197,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Configuration"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -246,15 +246,15 @@
         **kwargs: Any
     ) -> Optional["_models.ConfigurationListResult"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.ConfigurationListResult"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._batch_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -382,15 +382,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ConfigurationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_backups_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerBackup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -121,15 +121,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerBackupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_check_virtual_network_subnet_usage_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.VirtualNetworkSubnetUsageResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_firewall_rules_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         **kwargs: Any
     ) -> Optional["_models.FirewallRule"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.FirewallRule"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -187,15 +187,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -315,15 +315,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.FirewallRule"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -374,15 +374,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.FirewallRuleListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_replicas_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_location_based_capabilities_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CapabilitiesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/aio/operations/_servers_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         **kwargs: Any
     ) -> Optional["_models.Server"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Server"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -181,15 +181,15 @@
         **kwargs: Any
     ) -> Optional["_models.Server"]:
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Server"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -307,15 +307,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -426,15 +426,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Server"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -481,15 +481,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -548,15 +548,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -609,15 +609,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._failover_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -718,15 +718,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._restart_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -835,15 +835,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._start_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -943,15 +943,15 @@
         **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._stop_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_my_sql_management_client_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     ENABLED = "Enabled"
     DISABLED = "Disabled"
 
 class HighAvailabilityMode(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """High availability mode for a server.
     """
 
+    ENABLED = "Enabled"
     DISABLED = "Disabled"
     ZONE_REDUNDANT = "ZoneRedundant"
     SAME_ZONE = "SameZone"
 
 class HighAvailabilityState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """The state of server high availability.
     """
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,16 +615,16 @@
 
 
 class HighAvailability(msrest.serialization.Model):
     """Network related properties of a server.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param mode: High availability mode for a server. Possible values include: "Disabled",
-     "ZoneRedundant", "SameZone".
+    :param mode: High availability mode for a server. Possible values include: "Enabled",
+     "Disabled", "ZoneRedundant", "SameZone".
     :type mode: str or ~azure.mgmt.rdbms.mysql_flexibleservers.models.HighAvailabilityMode
     :ivar state: The state of server high availability. Possible values include: "NotEnabled",
      "CreatingStandby", "Healthy", "FailingOver", "RemovingStandby".
     :vartype state: str or ~azure.mgmt.rdbms.mysql_flexibleservers.models.HighAvailabilityState
     :param standby_availability_zone: Availability zone of the standby server.
     :type standby_availability_zone: str
     """
@@ -645,14 +645,49 @@
     ):
         super(HighAvailability, self).__init__(**kwargs)
         self.mode = kwargs.get('mode', None)
         self.state = None
         self.standby_availability_zone = kwargs.get('standby_availability_zone', None)
 
 
+class Identity(msrest.serialization.Model):
+    """Identity for the resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar principal_id: The principal ID of resource identity.
+    :vartype principal_id: str
+    :ivar tenant_id: The tenant ID of resource.
+    :vartype tenant_id: str
+    :param type: The identity type. The only acceptable values to pass in are None and
+     "SystemAssigned". The default value is None.
+    :type type: str
+    """
+
+    _validation = {
+        'principal_id': {'readonly': True},
+        'tenant_id': {'readonly': True},
+    }
+
+    _attribute_map = {
+        'principal_id': {'key': 'principalId', 'type': 'str'},
+        'tenant_id': {'key': 'tenantId', 'type': 'str'},
+        'type': {'key': 'type', 'type': 'str'},
+    }
+
+    def __init__(
+        self,
+        **kwargs
+    ):
+        super(Identity, self).__init__(**kwargs)
+        self.principal_id = None
+        self.tenant_id = None
+        self.type = kwargs.get('type', None)
+
+
 class MaintenanceWindow(msrest.serialization.Model):
     """Maintenance window of a server.
 
     :param custom_window: indicates whether custom window is enabled or disabled.
     :type custom_window: str
     :param start_hour: start hour for maintenance window.
     :type start_hour: int
@@ -918,14 +953,16 @@
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :param tags: A set of tags. Resource tags.
     :type tags: dict[str, str]
     :param location: Required. The geo-location where the resource lives.
     :type location: str
+    :param identity: The Azure Active Directory identity of the server.
+    :type identity: ~azure.mgmt.rdbms.mysql_flexibleservers.models.Identity
     :param sku: The SKU (pricing tier) of the server.
     :type sku: ~azure.mgmt.rdbms.mysql_flexibleservers.models.Sku
     :ivar system_data: The system metadata relating to this resource.
     :vartype system_data: ~azure.mgmt.rdbms.mysql_flexibleservers.models.SystemData
     :param administrator_login: The administrator's login name of a server. Can only be specified
      when the server is being created (and is required for creation).
     :type administrator_login: str
@@ -979,14 +1016,15 @@
 
     _attribute_map = {
         'id': {'key': 'id', 'type': 'str'},
         'name': {'key': 'name', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'location': {'key': 'location', 'type': 'str'},
+        'identity': {'key': 'identity', 'type': 'Identity'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'system_data': {'key': 'systemData', 'type': 'SystemData'},
         'administrator_login': {'key': 'properties.administratorLogin', 'type': 'str'},
         'administrator_login_password': {'key': 'properties.administratorLoginPassword', 'type': 'str'},
         'version': {'key': 'properties.version', 'type': 'str'},
         'availability_zone': {'key': 'properties.availabilityZone', 'type': 'str'},
         'create_mode': {'key': 'properties.createMode', 'type': 'str'},
@@ -1004,14 +1042,15 @@
     }
 
     def __init__(
         self,
         **kwargs
     ):
         super(Server, self).__init__(**kwargs)
+        self.identity = kwargs.get('identity', None)
         self.sku = kwargs.get('sku', None)
         self.system_data = None
         self.administrator_login = kwargs.get('administrator_login', None)
         self.administrator_login_password = kwargs.get('administrator_login_password', None)
         self.version = kwargs.get('version', None)
         self.availability_zone = kwargs.get('availability_zone', None)
         self.create_mode = kwargs.get('create_mode', None)
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,16 +649,16 @@
 
 
 class HighAvailability(msrest.serialization.Model):
     """Network related properties of a server.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :param mode: High availability mode for a server. Possible values include: "Disabled",
-     "ZoneRedundant", "SameZone".
+    :param mode: High availability mode for a server. Possible values include: "Enabled",
+     "Disabled", "ZoneRedundant", "SameZone".
     :type mode: str or ~azure.mgmt.rdbms.mysql_flexibleservers.models.HighAvailabilityMode
     :ivar state: The state of server high availability. Possible values include: "NotEnabled",
      "CreatingStandby", "Healthy", "FailingOver", "RemovingStandby".
     :vartype state: str or ~azure.mgmt.rdbms.mysql_flexibleservers.models.HighAvailabilityState
     :param standby_availability_zone: Availability zone of the standby server.
     :type standby_availability_zone: str
     """
@@ -682,14 +682,51 @@
     ):
         super(HighAvailability, self).__init__(**kwargs)
         self.mode = mode
         self.state = None
         self.standby_availability_zone = standby_availability_zone
 
 
+class Identity(msrest.serialization.Model):
+    """Identity for the resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar principal_id: The principal ID of resource identity.
+    :vartype principal_id: str
+    :ivar tenant_id: The tenant ID of resource.
+    :vartype tenant_id: str
+    :param type: The identity type. The only acceptable values to pass in are None and
+     "SystemAssigned". The default value is None.
+    :type type: str
+    """
+
+    _validation = {
+        'principal_id': {'readonly': True},
+        'tenant_id': {'readonly': True},
+    }
+
+    _attribute_map = {
+        'principal_id': {'key': 'principalId', 'type': 'str'},
+        'tenant_id': {'key': 'tenantId', 'type': 'str'},
+        'type': {'key': 'type', 'type': 'str'},
+    }
+
+    def __init__(
+        self,
+        *,
+        type: Optional[str] = None,
+        **kwargs
+    ):
+        super(Identity, self).__init__(**kwargs)
+        self.principal_id = None
+        self.tenant_id = None
+        self.type = type
+
+
 class MaintenanceWindow(msrest.serialization.Model):
     """Maintenance window of a server.
 
     :param custom_window: indicates whether custom window is enabled or disabled.
     :type custom_window: str
     :param start_hour: start hour for maintenance window.
     :type start_hour: int
@@ -986,14 +1023,16 @@
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :param tags: A set of tags. Resource tags.
     :type tags: dict[str, str]
     :param location: Required. The geo-location where the resource lives.
     :type location: str
+    :param identity: The Azure Active Directory identity of the server.
+    :type identity: ~azure.mgmt.rdbms.mysql_flexibleservers.models.Identity
     :param sku: The SKU (pricing tier) of the server.
     :type sku: ~azure.mgmt.rdbms.mysql_flexibleservers.models.Sku
     :ivar system_data: The system metadata relating to this resource.
     :vartype system_data: ~azure.mgmt.rdbms.mysql_flexibleservers.models.SystemData
     :param administrator_login: The administrator's login name of a server. Can only be specified
      when the server is being created (and is required for creation).
     :type administrator_login: str
@@ -1047,14 +1086,15 @@
 
     _attribute_map = {
         'id': {'key': 'id', 'type': 'str'},
         'name': {'key': 'name', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'location': {'key': 'location', 'type': 'str'},
+        'identity': {'key': 'identity', 'type': 'Identity'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'system_data': {'key': 'systemData', 'type': 'SystemData'},
         'administrator_login': {'key': 'properties.administratorLogin', 'type': 'str'},
         'administrator_login_password': {'key': 'properties.administratorLoginPassword', 'type': 'str'},
         'version': {'key': 'properties.version', 'type': 'str'},
         'availability_zone': {'key': 'properties.availabilityZone', 'type': 'str'},
         'create_mode': {'key': 'properties.createMode', 'type': 'str'},
@@ -1072,14 +1112,15 @@
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
+        identity: Optional["Identity"] = None,
         sku: Optional["Sku"] = None,
         administrator_login: Optional[str] = None,
         administrator_login_password: Optional[str] = None,
         version: Optional[Union[str, "ServerVersion"]] = None,
         availability_zone: Optional[str] = None,
         create_mode: Optional[Union[str, "CreateMode"]] = None,
         source_server_resource_id: Optional[str] = None,
@@ -1089,14 +1130,15 @@
         backup: Optional["Backup"] = None,
         high_availability: Optional["HighAvailability"] = None,
         network: Optional["Network"] = None,
         maintenance_window: Optional["MaintenanceWindow"] = None,
         **kwargs
     ):
         super(Server, self).__init__(tags=tags, location=location, **kwargs)
+        self.identity = identity
         self.sku = sku
         self.system_data = None
         self.administrator_login = administrator_login
         self.administrator_login_password = administrator_login_password
         self.version = version
         self.availability_zone = availability_zone
         self.create_mode = create_mode
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     from ._models_py3 import DelegatedSubnetUsage
     from ._models_py3 import ErrorAdditionalInfo
     from ._models_py3 import ErrorResponse
     from ._models_py3 import FirewallRule
     from ._models_py3 import FirewallRuleListResult
     from ._models_py3 import GetPrivateDnsZoneSuffixResponse
     from ._models_py3 import HighAvailability
+    from ._models_py3 import Identity
     from ._models_py3 import MaintenanceWindow
     from ._models_py3 import NameAvailability
     from ._models_py3 import NameAvailabilityRequest
     from ._models_py3 import Network
     from ._models_py3 import Operation
     from ._models_py3 import OperationDisplay
     from ._models_py3 import OperationListResult
@@ -61,14 +62,15 @@
     from ._models import DelegatedSubnetUsage  # type: ignore
     from ._models import ErrorAdditionalInfo  # type: ignore
     from ._models import ErrorResponse  # type: ignore
     from ._models import FirewallRule  # type: ignore
     from ._models import FirewallRuleListResult  # type: ignore
     from ._models import GetPrivateDnsZoneSuffixResponse  # type: ignore
     from ._models import HighAvailability  # type: ignore
+    from ._models import Identity  # type: ignore
     from ._models import MaintenanceWindow  # type: ignore
     from ._models import NameAvailability  # type: ignore
     from ._models import NameAvailabilityRequest  # type: ignore
     from ._models import Network  # type: ignore
     from ._models import Operation  # type: ignore
     from ._models import OperationDisplay  # type: ignore
     from ._models import OperationListResult  # type: ignore
@@ -120,14 +122,15 @@
     'DelegatedSubnetUsage',
     'ErrorAdditionalInfo',
     'ErrorResponse',
     'FirewallRule',
     'FirewallRuleListResult',
     'GetPrivateDnsZoneSuffixResponse',
     'HighAvailability',
+    'Identity',
     'MaintenanceWindow',
     'NameAvailability',
     'NameAvailabilityRequest',
     'Network',
     'Operation',
     'OperationDisplay',
     'OperationListResult',
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_name_availability_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.NameAvailability"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_get_private_dns_zone_suffix_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.GetPrivateDnsZoneSuffixResponse"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
 
         # Construct parameters
         query_parameters = {}  # type: Dict[str, Any]
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_databases_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     ):
         # type: (...) -> Optional["_models.Database"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Database"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -194,15 +194,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -324,15 +324,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Database"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -384,15 +384,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.DatabaseListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_configurations_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     ):
         # type: (...) -> Optional["_models.Configuration"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Configuration"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -204,15 +204,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Configuration"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -254,15 +254,15 @@
     ):
         # type: (...) -> Optional["_models.ConfigurationListResult"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.ConfigurationListResult"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._batch_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -392,15 +392,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ConfigurationListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_backups_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerBackup"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -127,15 +127,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerBackupListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_check_virtual_network_subnet_usage_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.VirtualNetworkSubnetUsageResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.execute.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_firewall_rules_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     ):
         # type: (...) -> Optional["_models.FirewallRule"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.FirewallRule"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -194,15 +194,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -324,15 +324,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.FirewallRule"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -384,15 +384,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.FirewallRuleListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_replicas_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_location_based_capabilities_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.CapabilitiesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-rdbms-9.1.0/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py` & `azure-mgmt-rdbms-9.1.0b1/azure/mgmt/rdbms/mysql_flexibleservers/operations/_servers_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ):
         # type: (...) -> Optional["_models.Server"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Server"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -188,15 +188,15 @@
     ):
         # type: (...) -> Optional["_models.Server"]
         cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Server"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -316,15 +316,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -437,15 +437,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.Server"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -493,15 +493,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -561,15 +561,15 @@
         :raises: ~azure.core.exceptions.HttpResponseError
         """
         cls = kwargs.pop('cls', None)  # type: ClsType["_models.ServerListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -623,15 +623,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._failover_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -734,15 +734,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._restart_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
@@ -853,15 +853,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._start_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
@@ -963,15 +963,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2021-05-01"
+        api_version = "2021-05-01-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._stop_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str', min_length=1),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str', max_length=90, min_length=1),
```

