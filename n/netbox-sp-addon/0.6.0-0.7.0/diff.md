# Comparing `tmp/netbox-sp-addon-0.6.0.tar.gz` & `tmp/netbox_sp_addon-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-sp-addon-0.6.0.tar", last modified: Fri Jul 15 06:22:08 2022, max compression
+gzip compressed data, was "netbox_sp_addon-0.7.0.tar", max compression
```

## Comparing `netbox-sp-addon-0.6.0.tar` & `netbox_sp_addon-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxr-xr-x   0 tgenannt  (1000) tgenannt  (1000)        0 2022-07-15 06:22:08.038916 netbox-sp-addon-0.6.0/
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)    10174 2020-08-19 12:46:44.000000 netbox-sp-addon-0.6.0/LICENSE.txt
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      294 2022-07-15 06:22:08.038916 netbox-sp-addon-0.6.0/PKG-INFO
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)       19 2021-07-23 09:00:24.000000 netbox-sp-addon-0.6.0/README.md
-drwxr-xr-x   0 tgenannt  (1000) tgenannt  (1000)        0 2022-07-15 06:22:08.034916 netbox-sp-addon-0.6.0/netbox_sp_addon/
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      805 2022-07-15 06:06:20.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/__init__.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)       33 2020-08-19 06:52:21.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/admin.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      314 2021-05-10 11:22:56.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/filters.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)     1030 2022-07-15 06:05:58.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/forms.py
-drwxr-xr-x   0 tgenannt  (1000) tgenannt  (1000)        0 2022-07-15 06:22:08.038916 netbox-sp-addon-0.6.0/netbox_sp_addon/migrations/
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)        0 2020-08-19 06:45:45.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/migrations/__init__.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)       29 2020-08-19 06:52:25.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/models.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      340 2020-08-19 11:55:42.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/navigation.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      203 2020-08-19 11:56:02.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/template_content.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      292 2020-08-19 11:56:02.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/urls.py
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      326 2020-08-19 11:56:02.000000 netbox-sp-addon-0.6.0/netbox_sp_addon/views.py
-drwxr-xr-x   0 tgenannt  (1000) tgenannt  (1000)        0 2022-07-15 06:22:08.038916 netbox-sp-addon-0.6.0/netbox_sp_addon.egg-info/
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      294 2022-07-15 06:22:08.000000 netbox-sp-addon-0.6.0/netbox_sp_addon.egg-info/PKG-INFO
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      471 2022-07-15 06:22:08.000000 netbox-sp-addon-0.6.0/netbox_sp_addon.egg-info/SOURCES.txt
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)        1 2022-07-15 06:22:08.000000 netbox-sp-addon-0.6.0/netbox_sp_addon.egg-info/dependency_links.txt
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)       16 2022-07-15 06:22:08.000000 netbox-sp-addon-0.6.0/netbox_sp_addon.egg-info/top_level.txt
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)       38 2022-07-15 06:22:08.038916 netbox-sp-addon-0.6.0/setup.cfg
--rw-r--r--   0 tgenannt  (1000) tgenannt  (1000)      520 2022-07-15 06:06:28.000000 netbox-sp-addon-0.6.0/setup.py
+-rw-r--r--   0        0        0    10174 2020-08-19 12:46:44.245428 netbox_sp_addon-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0       18 2023-04-18 06:36:09.409522 netbox_sp_addon-0.7.0/README.md
+-rw-r--r--   0        0        0      855 2023-04-18 06:42:58.141525 netbox_sp_addon-0.7.0/netbox_sp_addon/__init__.py
+-rw-r--r--   0        0        0       33 2020-08-19 06:52:21.758355 netbox_sp_addon-0.7.0/netbox_sp_addon/admin.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:50:54.486440 netbox_sp_addon-0.7.0/netbox_sp_addon/api/serializers.py
+-rw-r--r--   0        0        0       96 2020-08-19 06:50:48.874445 netbox_sp_addon-0.7.0/netbox_sp_addon/api/urls.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:50:37.790456 netbox_sp_addon-0.7.0/netbox_sp_addon/api/views.py
+-rw-r--r--   0        0        0      314 2022-07-15 06:25:44.678883 netbox_sp_addon-0.7.0/netbox_sp_addon/filters.py
+-rw-r--r--   0        0        0     1072 2023-04-18 06:41:16.389118 netbox_sp_addon-0.7.0/netbox_sp_addon/forms.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:45:45.614774 netbox_sp_addon-0.7.0/netbox_sp_addon/migrations/__init__.py
+-rw-r--r--   0        0        0       29 2020-08-19 06:52:25.914351 netbox_sp_addon-0.7.0/netbox_sp_addon/models.py
+-rw-r--r--   0        0        0      340 2020-08-19 11:55:42.757704 netbox_sp_addon-0.7.0/netbox_sp_addon/navigation.py
+-rw-r--r--   0        0        0      203 2020-08-19 11:56:02.973697 netbox_sp_addon-0.7.0/netbox_sp_addon/template_content.py
+-rw-r--r--   0        0        0      292 2020-08-19 11:56:02.981697 netbox_sp_addon-0.7.0/netbox_sp_addon/urls.py
+-rw-r--r--   0        0        0      326 2020-08-19 11:56:02.977697 netbox_sp_addon-0.7.0/netbox_sp_addon/views.py
+-rw-r--r--   0        0        0      732 2023-04-18 06:35:01.440290 netbox_sp_addon-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 netbox_sp_addon-0.7.0/PKG-INFO
```

### Comparing `netbox-sp-addon-0.6.0/LICENSE.txt` & `netbox_sp_addon-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox-sp-addon-0.6.0/netbox_sp_addon/forms.py` & `netbox_sp_addon-0.7.0/netbox_sp_addon/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from dcim.forms import DeviceFilterForm
 from dcim.models import RackRole
-from utilities.forms import DynamicModelMultipleChoiceField
+from utilities.forms.fields import DynamicModelMultipleChoiceField
 
 
 class SPDeviceFilterForm(DeviceFilterForm):
     fieldsets = (
-        (None, ('q', 'tag')),
+        (None, ('q', 'filter_id', 'tag')),
         ('Location', ('region_id', 'site_group_id', 'site_id', 'location_id', 'rack_role', 'rack_id')),
         ('Operation', ('status', 'role_id', 'airflow', 'serial', 'asset_tag', 'mac_address')),
         ('Hardware', ('manufacturer_id', 'device_type_id', 'platform_id')),
         ('Tenant', ('tenant_group_id', 'tenant_id')),
         ('Contacts', ('contact', 'contact_role', 'contact_group')),
         ('Components', (
             'console_ports', 'console_server_ports', 'power_ports', 'power_outlets', 'interfaces', 'pass_through_ports',
         )),
-        ('Miscellaneous', ('has_primary_ip', 'virtual_chassis_member', 'local_context_data'))
+        ('Miscellaneous', ('has_primary_ip', 'virtual_chassis_member', 'config_template_id', 'local_context_data'))
     )
 
     rack_role = DynamicModelMultipleChoiceField(
         queryset=RackRole.objects.all(),
         required=False,
         label="Rack role",
     )
```

