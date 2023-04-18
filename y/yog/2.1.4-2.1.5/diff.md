# Comparing `tmp/yog-2.1.4.tar.gz` & `tmp/yog-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.1.4.tar", max compression
+gzip compressed data, was "yog-2.1.5.tar", max compression
```

## Comparing `yog-2.1.4.tar` & `yog-2.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     6801 2023-02-01 20:50:54.524689 yog-2.1.4/README.md
--rw-r--r--   0        0        0      541 2023-02-22 22:13:34.371954 yog-2.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.1.4/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.1.4/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.1.4/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.1.4/yog/host/__init__.py
--rw-r--r--   0        0        0    11082 2023-02-01 20:50:54.524689 yog-2.1.4/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.1.4/yog/host/main.py
--rw-r--r--   0        0        0     7454 2023-02-22 20:47:28.668366 yog-2.1.4/yog/host/manage.py
--rw-r--r--   0        0        0     8418 2023-02-22 04:11:12.414451 yog-2.1.4/yog/host/necronomicon.py
--rw-r--r--   0        0        0    11317 2023-02-22 22:13:28.278626 yog-2.1.4/yog/host/pki.py
--rw-r--r--   0        0        0      492 2023-02-22 04:11:12.414451 yog-2.1.4/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.1.4/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.1.4/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.1.4/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.1.4/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.1.4/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.1.4/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.1.4/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.1.4/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.1.4/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.1.4/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.1.4/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.1.4/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    10283 2023-02-22 04:11:12.414451 yog-2.1.4/yog/ssh_utils.py
--rw-r--r--   0        0        0     7903 2023-02-22 22:13:58.005527 yog-2.1.4/setup.py
--rw-r--r--   0        0        0     7380 2023-02-22 22:13:58.006146 yog-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.1.5/README.md
+-rw-r--r--   0        0        0      541 2023-04-18 02:34:04.537034 yog-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.1.5/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.1.5/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.1.5/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.1.5/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.1.5/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.1.5/yog/host/main.py
+-rw-r--r--   0        0        0     7468 2023-04-17 17:46:06.818706 yog-2.1.5/yog/host/manage.py
+-rw-r--r--   0        0        0     8557 2023-04-17 17:47:42.812155 yog-2.1.5/yog/host/necronomicon.py
+-rw-r--r--   0        0        0    11317 2023-02-22 22:13:28.278626 yog-2.1.5/yog/host/pki.py
+-rw-r--r--   0        0        0      492 2023-02-22 04:11:12.414451 yog-2.1.5/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.1.5/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.1.5/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.1.5/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.1.5/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.1.5/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.1.5/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.1.5/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.1.5/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.1.5/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.1.5/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.1.5/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.1.5/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    10283 2023-02-22 04:11:12.414451 yog-2.1.5/yog/ssh_utils.py
+-rw-r--r--   0        0        0    11384 2023-04-18 02:34:17.535767 yog-2.1.5/setup.py
+-rw-r--r--   0        0        0    10753 2023-04-18 02:34:17.536693 yog-2.1.5/PKG-INFO
```

### Comparing `yog-2.1.4/pyproject.toml` & `yog-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.1.4"
+version = "2.1.5"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.1.4/yog/git_utils.py` & `yog-2.1.5/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/host/docker_attrs.py` & `yog-2.1.5/yog/host/docker_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,45 @@
     def from_necronomicon(self, dc: DockerContainer) -> 'DockerAttributeInstance':
         return SimpleDockerAttributeInstance(dc.name)
 
     def from_container(self, c: Container) -> 'DockerAttributeInstance':
         return SimpleDockerAttributeInstance(c.name)
 
 
+class DockerNetworkingModeDef(DockerAttribute):
+    def run_arg_name(self) -> str:
+        return "network_mode"
+
+    def from_necronomicon(self, dc: DockerContainer) -> 'DockerAttributeInstance':
+        return SimpleDockerAttributeInstance(dc.network_mode)
+
+    def from_container(self, c: Container) -> 'DockerAttributeInstance':
+        found = c.attrs['HostConfig']['NetworkMode']
+        # if found == "default":
+        #     found = "bridge"
+        return SimpleDockerAttributeInstance(found)
+
+
+class DockerNetworkingModeDefInstance(DockerAttributeInstance):
+    def __init__(self, network_mode_name):
+        self.network_mode_name = network_mode_name
+
+    def to_run_arg(self) -> t.Any:
+        if self.network_mode_name == "default":
+            return None
+        else:
+            return self.network_mode_name
+
+    def is_satisfied_by(self, other: 'DockerNetworkingModeDefInstance'):
+        return self.network_mode_name == other.network_mode_name
+
+    def __repr__(self) -> str:
+        return repr(self.network_mode_name)
+
+
 def diff_container(c: Container, dc: DockerContainer) -> t.List[t.Tuple[str, t.Any, t.Any]]:
     diffs = []
     for da in SUPPORTED_DOCKER_ATTRS:
         desired = da.from_necronomicon(dc)
         found = da.from_container(c)
 
         if not desired.is_satisfied_by(found):
@@ -328,8 +359,9 @@
     DockerCommandDef(),
     DockerSysctlDef(),
     DockerCapabilitiesDef(),
     DockerDetachDef(),
     DockerLoggingDef(),
     DockerRestartPolicyDef(),
     DockerNameDef(),
+    DockerNetworkingModeDef(),
 ]
```

### Comparing `yog-2.1.4/yog/host/manage.py` & `yog-2.1.5/yog/host/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
                         log.info(f"[{host}][docker]: OK {desired_container.name}@{desired_container.fingerprint[7:13]}")
                         log.debug("Existing container matches our desired state. No need to kill it.")
                         continue
 
                     log.debug(f"[{host}][docker][{c.name}]: diffs:")
                     for diff in diffs:
                         log.debug(f"[{host}][docker][{c.name}]: {diff[0]}")
-                        log.debug(f"[{host}][docker][{c.name}]: {diff[1]}")
-                        log.debug(f"[{host}][docker][{c.name}]: {diff[2]}")
+                        log.debug(f"[{host}][docker][{c.name}]: desired {diff[1]}")
+                        log.debug(f"[{host}][docker][{c.name}]: found {diff[2]}")
 
                     if c.status in ["running", "restarting"]:
                         log.debug(f"STOP {c.name}:{c.id}")
                         c.stop()
                     log.debug(f"RM: {c.name}:{c.id}")
                     c.remove()
```

### Comparing `yog-2.1.4/yog/host/necronomicon.py` & `yog-2.1.5/yog/host/necronomicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             e['fingerprint'],
             e['volumes'] if 'volumes' in e else {},
             [PortEntry.from_yaml(pe) for pe in (e['ports'] if 'ports' in e else [])],
             e['env'] if 'env' in e else {},
             e['command'] if 'command' in e else None,
             e['capabilities'] if 'capabilities' in e else [],
             {str(k): str(v) for k, v in e['sysctls'].items()} if 'sysctls' in e else {},
+            e['network_mode'] if 'network_mode' in e else "default",
         ) for e in parsed_necronomicon['docker']])
     else:
         ds = DockerSection([])
 
     if 'cron' in parsed_necronomicon:
         cs = CronSection([CronJob(e['expr'], e['command'], e['user'] if 'user' in e else 'root') for e in parsed_necronomicon['cron']])
     else:
@@ -103,14 +104,15 @@
                 desired_container.fingerprint,
                 desired_container.volumes,
                 desired_container.ports,
                 inflated_desired_container_env,
                 desired_container.command,
                 desired_container.capabilities,
                 desired_container.sysctls,
+                desired_container.network_mode,
             ))
 
         return Necronomicon(
             self.ident,
             self.tunnels,
             DockerSection(inflated_containers),
             self.cron,
@@ -129,14 +131,15 @@
     fingerprint: str
     volumes: t.Mapping[str, str]
     ports: t.List['PortEntry']
     env: t.Mapping[str, str]
     command: t.Optional[str]
     capabilities: t.List[str]
     sysctls: t.Mapping[str, str]
+    network_mode: str
 
 
 class PortEntry(t.NamedTuple):
     container: 'PortString'
     host: t.List['PortString']
 
     @staticmethod
```

### Comparing `yog-2.1.4/yog/host/pki.py` & `yog-2.1.5/yog/host/pki.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/host/test_docker_attrs.py` & `yog-2.1.5/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/logging_utils.py` & `yog-2.1.5/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/repo/main.py` & `yog-2.1.5/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/res/docker_test.yml` & `yog-2.1.5/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.1.4/yog/ssh_utils.py` & `yog-2.1.5/yog/ssh_utils.py`

 * *Files identical despite different names*

