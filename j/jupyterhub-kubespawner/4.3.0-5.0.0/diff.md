# Comparing `tmp/jupyterhub-kubespawner-4.3.0.tar.gz` & `tmp/jupyterhub_kubespawner-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-kubespawner-4.3.0.tar", last modified: Thu Nov  3 14:06:43 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterhub-kubespawner-4.3.0.tar` & `jupyterhub_kubespawner-5.0.0.tar`

### file list

```diff
@@ -1,22 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-03 14:06:43.649145 jupyterhub-kubespawner-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2022-11-03 14:06:43.649145 jupyterhub-kubespawner-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5073 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-03 14:06:43.649145 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2022-11-03 14:06:43.000000 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      442 2022-11-03 14:06:43.000000 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-03 14:06:43.000000 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      172 2022-11-03 14:06:43.000000 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-03 14:06:43.000000 jupyterhub-kubespawner-4.3.0/jupyterhub_kubespawner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-03 14:06:43.649145 jupyterhub-kubespawner-4.3.0/kubespawner/
--rw-r--r--   0 runner    (1001) docker     (122)      526 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/clients.py
--rw-r--r--   0 runner    (1001) docker     (122)    33570 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    17623 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)    16100 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/reflector.py
--rw-r--r--   0 runner    (1001) docker     (122)   122146 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/spawner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7360 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/kubespawner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      769 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-03 14:06:43.649145 jupyterhub-kubespawner-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1408 2022-11-03 14:06:26.000000 jupyterhub-kubespawner-4.3.0/setup.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.flake8
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/RELEASE.md
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/jupyterhub_config.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/Makefile
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/make.bat
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0    66490 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/changelog.md
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/index.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/objects.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/reflector.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/spawner.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/ssl.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/utils.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/_version.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/clients.py
+-rw-r--r--   0        0        0    37969 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/objects.py
+-rw-r--r--   0        0        0    22353 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/proxy.py
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/reflector.py
+-rw-r--r--   0        0        0   125371 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/spawner.py
+-rw-r--r--   0        0        0     8415 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/utils.py
+-rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/jupyterhub_config.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_clients.py
+-rw-r--r--   0        0        0   102281 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_objects.py
+-rw-r--r--   0        0        0    46364 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_spawner.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.gitignore
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/LICENSE
+-rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/README.md
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/PKG-INFO
```

### Comparing `jupyterhub-kubespawner-4.3.0/LICENSE` & `jupyterhub_kubespawner-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-kubespawner-4.3.0/PKG-INFO` & `jupyterhub_kubespawner-5.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: jupyterhub-kubespawner
-Version: 4.3.0
-Summary: JupyterHub Spawner for Kubernetes
-Home-page: http://github.com/jupyterhub/kubespawner
-Author: Jupyter Contributors
-Author-email: jupyter@googlegroups.com
-License: BSD
-Project-URL: Documentation, https://jupyterhub-kubespawner.readthedocs.io
-Project-URL: Source, https://github.com/jupyterhub/kubespawner
-Project-URL: Tracker, https://github.com/jupyterhub/kubespawner/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # [kubespawner](https://github.com/jupyterhub/kubespawner) (jupyterhub-kubespawner @ PyPI)
 
+[![Latest PyPI version](https://img.shields.io/pypi/v/jupyterhub-kubespawner?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
+[![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/jupyterhub-kubespawner?logo=conda-forge)](https://anaconda.org/conda-forge/jupyterhub-kubespawner)
 [![Documentation status](https://img.shields.io/readthedocs/jupyterhub-kubespawner?logo=read-the-docs)](https://jupyterhub-kubespawner.readthedocs.io/en/latest/?badge=latest)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jupyterhub/kubespawner/Test?logo=github)](https://github.com/jupyterhub/kubespawner/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jupyterhub/kubespawner/test.yaml?logo=github&label=tests)](https://github.com/jupyterhub/kubespawner/actions)
 [![Code coverage](https://codecov.io/gh/jupyterhub/kubespawner/branch/main/graph/badge.svg)](https://codecov.io/gh/jupyterhub/kubespawner)
 [![](https://img.shields.io/pypi/v/jupyterhub-kubespawner.svg?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
 
 The _kubespawner_ (also known as JupyterHub Kubernetes Spawner) enables JupyterHub to spawn
 single-user notebook servers on a [Kubernetes](https://kubernetes.io/)
 cluster.
```

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/clients.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/clients.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/objects.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/objects.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Helper methods for generating k8s API objects.
 """
 import base64
 import ipaddress
 import json
 import operator
 import re
-from typing import Optional
+from typing import Dict, List, Optional, Tuple
 from urllib.parse import urlparse
 
 from kubernetes_asyncio.client.models import (
     V1Affinity,
     V1Container,
     V1ContainerPort,
     V1EndpointAddress,
@@ -20,14 +20,15 @@
     V1HTTPIngressPath,
     V1HTTPIngressRuleValue,
     V1Ingress,
     V1IngressBackend,
     V1IngressRule,
     V1IngressServiceBackend,
     V1IngressSpec,
+    V1IngressTLS,
     V1Lifecycle,
     V1LocalObjectReference,
     V1Namespace,
     V1NodeAffinity,
     V1NodeSelector,
     V1NodeSelectorTerm,
     V1ObjectMeta,
@@ -55,15 +56,27 @@
 # libraries generated from an OpenAPI schema for k8s 1.21+ will name
 # V1EndpointPort as CoreV1EndpointPort.
 try:
     from kubernetes_asyncio.client.models import CoreV1EndpointPort
 except ImportError:
     from kubernetes_asyncio.client.models import V1EndpointPort as CoreV1EndpointPort
 
-from .utils import get_k8s_model, update_k8s_model
+from .utils import get_k8s_model, host_matching, update_k8s_model
+
+# Matches Kubernetes DNS names template for services
+# https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#namespaces-of-services:
+# * service.namespace.svc.cluster.local
+# * service.namespace.svc.cluster
+# * service.namespace.svc
+# * service.namespace
+# * service
+# User by `KubeIngressProxy.reuse_existing_services=True`
+SERVICE_DNS_PATTERN = re.compile(
+    r"(?P<service>[^.]+)\.?(?P<namespace>[^.]+)?(?P<rest>\.svc(\.cluster(\.local)?)?)?"
+)
 
 
 def make_pod(
     name,
     cmd,
     port,
     image,
@@ -730,56 +743,71 @@
 
 
 def make_ingress(
     name: str,
     routespec: str,
     target: str,
     data: dict,
+    namespace: str,
     common_labels: Optional[dict] = None,
-):
+    ingress_extra_labels: Optional[dict] = None,
+    ingress_extra_annotations: Optional[dict] = None,
+    ingress_class_name: Optional[str] = None,
+    ingress_specifications: Optional[List[Dict]] = None,
+    reuse_existing_services: bool = False,
+) -> Tuple[Optional[V1Endpoints], Optional[V1Service], V1Ingress]:
     """
     Returns an ingress, service, endpoint object that'll work for this service
     """
 
     default_labels = {
         'hub.jupyter.org/proxy-route': 'true',
     }
 
     common_labels = (common_labels or {}).copy()
     common_labels.update(default_labels)
 
+    common_annotations = {
+        'hub.jupyter.org/proxy-data': json.dumps(data),
+        'hub.jupyter.org/proxy-routespec': routespec,
+        'hub.jupyter.org/proxy-target': target,
+    }
+
     meta = V1ObjectMeta(
         name=name,
-        annotations={
-            'hub.jupyter.org/proxy-data': json.dumps(data),
-            'hub.jupyter.org/proxy-routespec': routespec,
-            'hub.jupyter.org/proxy-target': target,
-        },
+        annotations=common_annotations,
         labels=common_labels,
     )
 
-    if routespec.startswith('/'):
-        host = None
-        path = routespec
-    else:
-        host, path = routespec.split('/', 1)
+    # /myuser/myserver or https://myuser.example.com/myserver for spawned server
+    # /services/myservice or https://services.example.com/myservice for service
+    # / or https://example.com/ for hub
+    route_parts = urlparse(routespec)
+    routespec_host = route_parts.netloc or None
+    routespec_path = route_parts.path
 
     target_parts = urlparse(target)
     target_port = target_parts.port
 
     try:
         # Try to parse as an IP address
         target_ip = ipaddress.ip_address(target_parts.hostname)
     except ValueError:
         target_is_ip = False
     else:
         target_is_ip = True
 
+    service_name = name
+
     if target_is_ip:
-        # Make endpoint object
+        # c.KubeSpawner.services_enabled = False
+        # routespec='http://192.168.1.1:8888/'
+
+        # ingress -> service -> endpoint -> pod
+        # endpoint is used just to allow access from ingress to Pod IP (if PodNetworkPolicy is used)
         endpoint = V1Endpoints(
             kind='Endpoints',
             metadata=meta,
             subsets=[
                 V1EndpointSubset(
                     addresses=[V1EndpointAddress(ip=target_ip.compressed)],
                     ports=[CoreV1EndpointPort(port=target_port)],
@@ -795,52 +823,130 @@
                 external_name='',
                 ports=[V1ServicePort(port=target_port, target_port=target_port)],
             ),
         )
     else:
         endpoint = None
 
-        # Make service object
-        service = V1Service(
-            kind='Service',
-            metadata=meta,
-            spec=V1ServiceSpec(
-                type='ExternalName',
-                external_name=target_parts.hostname,
-                cluster_ip='',
-                ports=[V1ServicePort(port=target_port, target_port=target_port)],
+        service_match = SERVICE_DNS_PATTERN.match(target_parts.hostname)
+        if (
+            reuse_existing_services
+            and service_match
+            and (
+                not service_match.group("namespace")
+                or service_match.group("namespace") == namespace
+            )
+        ):
+            # c.KubeSpawner.services_enabled = True
+            # routespec='http://myservice.mynamespace.svc.cluster.local:8888/'
+            # routespec='http://myservice.mynamespace.svc.cluster:8888/'
+            # routespec='http://myservice.mynamespace.svc:8888/'
+            # routespec='http://myservice.mynamespace:8888/'
+            # routespec='http://hub:8888/'
+
+            # Ingress -> Service (same namespace, created by KubeSpawner)
+            service = None  # just use this service in ingress, do not create it
+            service_name = service_match.group("service")
+        else:
+            # config: c.KubeSpawner.namespace='another-namespace'
+            # routespec: 'http://myservice.another-namespace...:8888/'
+            # or
+            # config: c.KubeSpawner.enable_user_namespaces=True
+            # routespec: 'http://myservice.user-namespace...:8888/'
+            # or
+            # c.JupyterHub.services = [{"name": "my-service", "url": "http://some.domain:9000"}]
+            # routespec: 'http://some.domain:9000/'
+
+            # Ingress -> ExternalName -> Service (different namespace or some external domain)
+            service = V1Service(
+                kind='Service',
+                metadata=meta,
+                spec=V1ServiceSpec(
+                    type='ExternalName',
+                    external_name=target_parts.hostname,
+                    cluster_ip='',
+                    ports=[V1ServicePort(port=target_port, target_port=target_port)],
+                ),
+            )
+
+    # Make Ingress object
+
+    ingress_labels = common_labels.copy()
+    ingress_labels.update(ingress_extra_labels or {})
+
+    ingress_annotations = common_annotations.copy()
+    ingress_annotations.update(ingress_extra_annotations or {})
+
+    ingress_meta = V1ObjectMeta(
+        name=name,
+        annotations=ingress_annotations,
+        labels=ingress_labels,
+    )
+
+    ingress_specifications = ingress_specifications or []
+
+    hosts = []
+    add_routespec_host = True
+    for ingress_spec in ingress_specifications:
+        if routespec_host and host_matching(routespec_host, ingress_spec["host"]):
+            # if routespec is URL like "http[s]://user.example.com"
+            # and ingress_specifications contains item like
+            # {"host": "user.example.com"} or {"host": "*.example.com"},
+            # prefer routespec_host over than wildcard
+            if add_routespec_host:
+                hosts.append(routespec_host)
+
+            add_routespec_host = False
+        elif ingress_spec["host"] not in hosts:
+            hosts.append(ingress_spec["host"])
+
+    if add_routespec_host and (routespec_host or not hosts):
+        # if routespec is URL like "http[s]://user.example.com"
+        # and does not match any host from ingress_specifications, create rule with routespec_host.
+
+        # if routespec is path like /base/url, and ingress_specifications is empty,
+        # create one ingress rule without host name.
+        hosts.insert(0, routespec_host)
+
+    rules = [
+        V1IngressRule(
+            host=host,
+            http=V1HTTPIngressRuleValue(
+                paths=[
+                    V1HTTPIngressPath(
+                        path=routespec_path,
+                        path_type="Prefix",
+                        backend=V1IngressBackend(
+                            service=V1IngressServiceBackend(
+                                name=service_name,
+                                port=V1ServiceBackendPort(
+                                    number=target_port,
+                                ),
+                            ),
+                        ),
+                    ),
+                ],
             ),
         )
+        for host in hosts
+    ]
+
+    tls = [
+        V1IngressTLS(hosts=[spec["host"]], secret_name=spec["tlsSecret"])
+        for spec in ingress_specifications
+        if "tlsSecret" in spec
+    ]
 
-    # Make Ingress object
     ingress = V1Ingress(
         kind='Ingress',
-        metadata=meta,
+        metadata=ingress_meta,
         spec=V1IngressSpec(
-            rules=[
-                V1IngressRule(
-                    host=host,
-                    http=V1HTTPIngressRuleValue(
-                        paths=[
-                            V1HTTPIngressPath(
-                                path=path,
-                                path_type="Prefix",
-                                backend=V1IngressBackend(
-                                    service=V1IngressServiceBackend(
-                                        name=name,
-                                        port=V1ServiceBackendPort(
-                                            number=target_port,
-                                        ),
-                                    ),
-                                ),
-                            )
-                        ]
-                    ),
-                )
-            ]
+            rules=rules,
+            tls=tls or None,
+            ingress_class_name=ingress_class_name,
         ),
     )
 
     return endpoint, service, ingress
 
 
 def make_owner_reference(name, uid):
@@ -915,31 +1021,33 @@
             "notebooks-ca_trust.crt"
         ] + encoded.decode("utf-8")
 
     return secret
 
 
 def make_service(
-    name,
-    port,
-    servername,
-    owner_references,
-    labels=None,
-    annotations=None,
+    name: str,
+    port: int,
+    selector: dict,
+    owner_references: List[V1OwnerReference],
+    labels: Optional[dict] = None,
+    annotations: Optional[dict] = None,
 ):
     """
     Make a k8s service specification for using dns to communicate with the notebook.
 
     Parameters
     ----------
     name:
         Name of the service. Must be unique within the namespace the object is
         going to be created in.
-    env:
-        Dictionary of environment variables.
+    selector:
+        Labels of server pod to be used in spec.selector
+    owner_references:
+        Pod's owner references used to automatically remote service after pod removal
     labels:
         Labels to add to the service.
     annotations:
         Annotations to add to the service.
 
     """
 
@@ -952,19 +1060,15 @@
 
     service = V1Service(
         kind='Service',
         metadata=metadata,
         spec=V1ServiceSpec(
             type='ClusterIP',
             ports=[V1ServicePort(name='http', port=port, target_port=port)],
-            selector={
-                'component': 'singleuser-server',
-                'hub.jupyter.org/servername': servername,
-                'hub.jupyter.org/username': metadata.labels['hub.jupyter.org/username'],
-            },
+            selector=selector,
         ),
     )
 
     return service
 
 
 def make_namespace(name, labels=None, annotations=None):
```

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/proxy.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/proxy.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import string
 
 import escapism
 from jupyterhub.proxy import Proxy
 from jupyterhub.utils import exponential_backoff
 from kubernetes_asyncio import client
-from traitlets import Dict, Unicode
+from traitlets import Bool, Dict, List, Unicode
 
 from .clients import load_config, shared_client
 from .objects import make_ingress
 from .reflector import ResourceReflector
 from .utils import generate_hashed_slug
 
 
@@ -177,16 +177,101 @@
         See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__
         for more info on what labels are and why you might want to use them!
 
         `{username}`, `{servername}`, `{servicename}`, `{routespec}`, `{hubnamespace}`,
         `{unescaped_username}`, `{unescaped_servername}`, `{unescaped_servicename}` and `{unescaped_routespec}` will be expanded if
         found within strings of this configuration.
 
-        Names have to be are escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        Names have to be are escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
+        """,
+    )
+
+    ingress_extra_labels = Dict(
+        config=True,
+        help="""
+        Extra kubernetes labels to set to Ingress objects.
+
+        The keys and values must both be strings that match the kubernetes
+        label key / value constraints.
+
+        See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__
+        for more info on what labels are and why you might want to use them!
+
+        `{username}`, `{servername}`, `{servicename}`, `{routespec}`, `{hubnamespace}`,
+        `{unescaped_username}`, `{unescaped_servername}`, `{unescaped_servicename}` and `{unescaped_routespec}` will be expanded if
+        found within strings of this configuration.
+
+        Names have to be are escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
+        """,
+    )
+
+    ingress_extra_annotations = Dict(
+        config=True,
+        help="""
+        Extra kubernetes annotations to set on the Ingress object.
+
+        The keys and values must both be strings.
+
+        See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__
+        for more info on what labels are and why you might want to use them!
+
+        `{username}`, `{servername}`, `{servicename}`, `{routespec}`, `{hubnamespace}`,
+        `{unescaped_username}`, `{unescaped_servername}`, `{unescaped_servicename}` and `{unescaped_routespec}` will be expanded if
+        found within strings of this configuration.
+
+        Names have to be are escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
+        """,
+    )
+
+    ingress_class_name = Unicode(
+        config=True,
+        help="""
+        Default value for 'ingressClassName' field in Ingress specification
+        """,
+    )
+
+    ingress_specifications = List(
+        trait=Dict,
+        config=True,
+        help="""
+        Specifications for ingress routes. List of dicts of the following format:
+
+        [{'host': 'host.example.domain'}]
+        [{'host': 'host.example.domain', 'tlsSecret': 'tlsSecretName'}]
+        [{'host': 'jh.{hubnamespace}.domain', 'tlsSecret': 'tlsSecretName'}]
+
+        Wildcard might not work, refer to your ingress controller documentation.
+
+        `{routespec}`, `{hubnamespace}`, and `{unescaped_routespec}` will be expanded if
+        found within strings of this configuration.
+
+        Names have to be are escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
+        """,
+    )
+
+    reuse_existing_services = Bool(
+        False,
+        config=True,
+        help="""
+        If `True`, proxy will try to reuse existing services created by `KubeSpawner.services_enabled=True`
+        or `KubeSpawner.internal_ssl=True`.
+        If `False` (default), KubeSpawner creates service with type `ExternalName`, pointing to the pod's service.
+
+        Sometimes `ExternalName` could lead to issues with accessing pod, like `500 Redirect loop detected`,
+        so setting this option to `True` could solve this issue.
+
+        By default, KubeSpawner does not create service for a pod at all (`service_enabled=False`, `internal_ssl=False`).
+        In such a case KubeSpawner creates service with type `ClusterIP`, pointing to the pod IP and port.
+
+        If KubeSpawner creates pod in a different namespace, this option is ignored,
+        because Ingress(namespace=hub) cannot point to Service(namespace=user).
         """,
     )
 
     k8s_api_ssl_ca_cert = Unicode(
         "",
         config=True,
         help="""
@@ -313,22 +398,44 @@
 
     async def add_route(self, routespec, target, data):
         # Create a route with the name being escaped routespec
         # Use full routespec in label
         # 'data' is JSON encoded and put in an annotation - we don't need to query for it
 
         safe_name = self._safe_name_for_routespec(routespec).lower()
+        full_name = f'{self.namespace}/{safe_name}'
+
         common_labels = self._expand_all(self.common_labels, routespec, data)
         common_labels.update({'component': self.component_label})
+
+        ingress_extra_labels = self._expand_all(
+            self.ingress_extra_labels, routespec, data
+        )
+        ingress_extra_annotations = self._expand_all(
+            self.ingress_extra_annotations, routespec, data
+        )
+
+        ingress_specifications = self._expand_all(
+            self.ingress_specifications,
+            routespec,
+            data,
+        )
+
         endpoint, service, ingress = make_ingress(
             name=safe_name,
             routespec=routespec,
             target=target,
-            common_labels=common_labels,
             data=data,
+            namespace=self.namespace,
+            common_labels=common_labels,
+            ingress_extra_labels=ingress_extra_labels,
+            ingress_extra_annotations=ingress_extra_annotations,
+            ingress_class_name=self.ingress_class_name,
+            ingress_specifications=ingress_specifications,
+            reuse_existing_services=self.reuse_existing_services,
         )
 
         async def ensure_object(create_func, patch_func, body, kind):
             try:
                 await create_func(namespace=self.namespace, body=body)
                 self.log.info('Created %s/%s', kind, safe_name)
             except client.rest.ApiException as e:
@@ -350,49 +457,53 @@
                 self.core_api.create_namespaced_endpoints,
                 self.core_api.patch_namespaced_endpoints,
                 body=endpoint,
                 kind='endpoints',
             )
 
             await exponential_backoff(
-                lambda: f'{self.namespace}/{safe_name}'
-                in self.endpoint_reflector.endpoints.keys(),
+                lambda: full_name in self.endpoint_reflector.endpoints,
                 'Could not find endpoints/%s after creating it' % safe_name,
             )
         else:
             delete_endpoint = self.core_api.delete_namespaced_endpoints(
                 name=safe_name,
                 namespace=self.namespace,
                 body=client.V1DeleteOptions(grace_period_seconds=0),
             )
             await self._delete_if_exists('endpoint', safe_name, delete_endpoint)
 
-        await ensure_object(
-            self.core_api.create_namespaced_service,
-            self.core_api.patch_namespaced_service,
-            body=service,
-            kind='service',
-        )
-
-        await exponential_backoff(
-            lambda: f'{self.namespace}/{safe_name}'
-            in self.service_reflector.services.keys(),
-            'Could not find service/%s after creating it' % safe_name,
-        )
+        if service is not None:
+            await ensure_object(
+                self.core_api.create_namespaced_service,
+                self.core_api.patch_namespaced_service,
+                body=service,
+                kind='service',
+            )
+            await exponential_backoff(
+                lambda: full_name in self.service_reflector.services,
+                'Could not find services/%s after creating it' % safe_name,
+            )
+        else:
+            delete_service = self.core_api.delete_namespaced_service(
+                name=safe_name,
+                namespace=self.namespace,
+                body=client.V1DeleteOptions(grace_period_seconds=0),
+            )
+            await self._delete_if_exists('service', safe_name, delete_service)
 
         await ensure_object(
             self.networking_api.create_namespaced_ingress,
             self.networking_api.patch_namespaced_ingress,
             body=ingress,
             kind='ingress',
         )
 
         await exponential_backoff(
-            lambda: f'{self.namespace}/{safe_name}'
-            in self.ingress_reflector.ingresses.keys(),
+            lambda: full_name in self.ingress_reflector.ingresses,
             'Could not find ingress/%s after creating it' % safe_name,
         )
 
     async def delete_route(self, routespec):
         # We just ensure that these objects are deleted.
         # This means if some of them are already deleted, we just let it
         # be.
```

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/reflector.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/reflector.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/spawner.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/spawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 """
 import asyncio
 import ipaddress
 import os
 import string
 import sys
 import warnings
-from functools import partial, wraps
+from functools import partial
+from typing import Optional, Tuple, Type
 from urllib.parse import urlparse
 
 import escapism
 from jinja2 import BaseLoader, Environment
 from jupyterhub.spawner import Spawner
 from jupyterhub.traitlets import Callable, Command
 from jupyterhub.utils import exponential_backoff, maybe_future
@@ -39,31 +40,27 @@
     make_owner_reference,
     make_pod,
     make_pvc,
     make_secret,
     make_service,
 )
 from .reflector import ResourceReflector
+from .utils import recursive_update
 
 
 class PodReflector(ResourceReflector):
     """
     PodReflector is merely a configured ResourceReflector. It exposes
     the pods property, which is simply mapping to self.resources where the
     ResourceReflector keeps an updated list of the resource defined by
     the `kind` field and the `list_method_name` field.
     """
 
     kind = "pods"
 
-    # The default component label can be over-ridden by specifying the component_label property
-    labels = {
-        'component': 'singleuser-server',
-    }
-
     @property
     def pods(self):
         """
         A dictionary of pods for the namespace as returned by the Kubernetes
         API. The dictionary keys are the pod ids and the values are
         dictionaries of the actual pod resource values.
 
@@ -114,38 +111,48 @@
 
 class KubeSpawner(Spawner):
     """
     A JupyterHub spawner that spawn pods in a Kubernetes Cluster. Each server
     spawned by a user will have its own KubeSpawner instance.
     """
 
-    reflectors = {
-        "pods": None,
-        "events": None,
-    }
+    # Reflectors keeping track of the k8s api-server's state for various k8s
+    # resources are singletons as that state can be tracked and shared by all
+    # KubeSpawner objects.
+    reflectors = {}
 
     # Characters as defined by safe for DNS
     # Note: '-' is not in safe_chars, as it is being used as escape character
     safe_chars = set(string.ascii_lowercase + string.digits)
 
+    def _get_reflector_key(self, kind: str) -> Tuple[str, str, Optional[str]]:
+        if self.enable_user_namespaces:
+            # one reflector fo all namespaces
+            return (kind, None)
+
+        return (kind, self.namespace)
+
     @property
     def pod_reflector(self):
         """
-        A convenience alias to the class variable reflectors['pods'].
+        Returns instance of ResourceReflector for pods.
         """
-        return self.__class__.reflectors['pods']
+        key = self._get_reflector_key('pods')
+        return self.__class__.reflectors.get(key, None)
 
     @property
     def event_reflector(self):
         """
-        A convenience alias to the class variable reflectors['events'] if the
+        Returns instance of ResourceReflector for events, if the
         spawner instance has events_enabled.
         """
         if self.events_enabled:
-            return self.__class__.reflectors['events']
+            key = self._get_reflector_key('events')
+            return self.__class__.reflectors.get(key, None)
+        return None
 
     def __init__(self, *args, **kwargs):
         _mock = kwargs.pop('_mock', False)
         super().__init__(*args, **kwargs)
 
         if _mock:
             # runs during test execution only
@@ -191,51 +198,14 @@
             self.port = 8888
         # The attribute needs to exist, even though it is unset to start with
         self._start_future = None
 
         load_config(host=self.k8s_api_host, ssl_ca_cert=self.k8s_api_ssl_ca_cert)
         self.api = shared_client("CoreV1Api")
 
-        self._start_watching_pods()
-        if self.events_enabled:
-            self._start_watching_events()
-
-    def _await_pod_reflector(method):
-        """Decorator to wait for pod reflector to load
-
-        Apply to methods which require the pod reflector
-        to have completed its first load of pods.
-        """
-
-        @wraps(method)
-        async def async_method(self, *args, **kwargs):
-            if not self.pod_reflector.first_load_future.done():
-                await self.pod_reflector.first_load_future
-            return await method(self, *args, **kwargs)
-
-        return async_method
-
-    def _await_event_reflector(method):
-        """Decorator to wait for event reflector to load
-
-        Apply to methods which require the event reflector
-        to have completed its first load of events.
-        """
-
-        @wraps(method)
-        async def async_method(self, *args, **kwargs):
-            if (
-                self.events_enabled
-                and not self.event_reflector.first_load_future.done()
-            ):
-                await self.event_reflector.first_load_future
-            return await method(self, *args, **kwargs)
-
-        return async_method
-
     k8s_api_ssl_ca_cert = Unicode(
         "",
         config=True,
         help="""
         Location (absolute filepath) for CA certs of the k8s API server.
 
         Typically this is unnecessary, CA certs are picked up by
@@ -332,16 +302,16 @@
 
         Note that these are only set when the namespaces are created, not
         later when this setting is updated.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     user_namespace_annotations = Dict(
         config=True,
         help="""
         Kubernetes annotations that user namespaces will get (only if
@@ -349,31 +319,31 @@
 
         Note that these are only set when the namespaces are created, not
         later when this setting is updated.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     user_namespace_template = Unicode(
         "{hubnamespace}-{username}",
         config=True,
         help="""
         Template to use to form the namespace of user's pods (only if
         enable_user_namespaces is True).
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     namespace = Unicode(
         config=True,
         help="""
         Kubernetes namespace to spawn user pods in.
@@ -452,16 +422,16 @@
         help="""
         The working directory where the Notebook server will be started inside the container.
         Defaults to `None` so the working directory will be the one defined in the Dockerfile.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     # FIXME: Don't override 'default_value' ("") or 'allow_none' (False) (Breaking change)
     service_account = Unicode(
         None,
         allow_none=True,
@@ -507,16 +477,16 @@
         config=True,
         help="""
         Template to use to form the name of user's pods.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
 
         Trailing `-` characters are stripped for safe handling of empty server names (user default servers).
 
         This must be unique within the namespace the pods are being spawned
         in, so if you are running multiple jupyterhubs spawning in the
         same namespace, consider setting this to be something more unique.
 
@@ -530,21 +500,21 @@
 
     pod_connect_ip = Unicode(
         config=True,
         help="""
         The IP address (or hostname) of user's pods which KubeSpawner connects to.
         If you do not specify the value, KubeSpawner will use the pod IP.
 
-        e.g. 'jupyter-{username}--{servername}.notebooks.jupyterhub.svc.cluster.local',
+        e.g. `jupyter-{username}--{servername}.notebooks.jupyterhub.svc.cluster.local`,
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
 
         Trailing `-` characters in each domain level are stripped for safe handling of empty server names (user default servers).
 
         This must be unique within the namespace the pods are being spawned
         in, so if you are running multiple jupyterhubs spawning in the
         same namespace, consider setting this to be something more unique.
         """,
@@ -582,16 +552,16 @@
         config=True,
         help="""
         Template to use to form the name of user's pvc.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
 
         Trailing `-` characters are stripped for safe handling of empty server names (user default servers).
 
         This must be unique within the namespace the pvc are being spawned
         in, so if you are running multiple jupyterhubs spawning in the
         same namespace, consider setting this to be something more unique.
 
@@ -618,16 +588,16 @@
         config=True,
         help="""
         Template to use to form the name of user's secret.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
 
         This must be unique within the namespace the pvc are being spawned
         in, so if you are running multiple jupyterhubs spawning in the
         same namespace, consider setting this to be something more unique.
         """,
     )
 
@@ -692,16 +662,16 @@
 
         See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__
         for more info on what labels are and why you might want to use them!
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     extra_annotations = Dict(
         config=True,
         help="""
         Extra Kubernetes annotations to set on the spawned single-user pods, as
@@ -1063,16 +1033,16 @@
         See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/storage/volumes>`__
         for more information on the various kinds of volumes available and their options.
         Your kubernetes cluster must already be configured to support the volume types you want to use.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     volume_mounts = List(
         config=True,
         help="""
         List of paths on which to mount volumes in the user notebook's pod.
@@ -1086,16 +1056,16 @@
 
         See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/storage/volumes>`__
         for more information on how the `volumeMount` item works.
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     # FIXME: Don't override 'default_value' ("") or 'allow_none' (False) (Breaking change)
     storage_capacity = Unicode(
         None,
         config=True,
@@ -1148,16 +1118,16 @@
 
         See `the Kubernetes documentation <https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/>`__
         for more info on what labels are and why you might want to use them!
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     # FIXME: Don't override 'default_value' ("") or 'allow_none' (False) (Breaking change)
     storage_class = Unicode(
         None,
         config=True,
@@ -1210,16 +1180,16 @@
         For example to match the Nodes that have a label of `content: jupyter` use::
 
            c.KubeSpawner.storage_selector = {'matchLabels':{'content': 'jupyter'}}
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     lifecycle_hooks = Dict(
         config=True,
         help="""
         Kubernetes lifecycle hooks to set on the spawned single-user pods.
@@ -1346,16 +1316,16 @@
                 "image": "supercronic",
                 "command": ["/usr/local/bin/supercronic", "/etc/crontab"]
             }]
 
         `{username}`, `{userid}`, `{servername}`, `{hubnamespace}`,
         `{unescaped_username}`, and `{unescaped_servername}` will be expanded if
         found within strings of this configuration. The username and servername
-        come escaped to follow the [DNS label
-        standard](https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names).
+        come escaped to follow the `DNS label standard
+        <https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#dns-label-names>`__.
         """,
     )
 
     # FIXME: Don't override 'default_value' ("") or 'allow_none' (False) (Breaking change)
     scheduler_name = Unicode(
         None,
         allow_none=True,
@@ -1596,30 +1566,38 @@
         - `slug`: the machine readable slug to identify the profile
           (missing slugs are generated from display_name)
         - `description`: Optional description of this profile displayed to the user.
         - `kubespawner_override`: a dictionary with overrides to apply to the KubeSpawner
           settings. Each value can be either the final value to change or a callable that
           take the `KubeSpawner` instance as parameter and return the final value. This can
           be further overridden by 'profile_options'
-        - 'profile_options': A dictionary of sub-options that allow users to further customize the
+          If the traitlet being overriden is a *dictionary*, the dictionary
+          will be *recursively updated*, rather than overriden. If you want to
+          remove a key, set its value to `None`
+        - `profile_options`: A dictionary of sub-options that allow users to further customize the
           selected profile. By default, these are rendered as a dropdown with the label
           provided by `display_name`. Items should have a unique key representing the customization,
           and the value is a dictionary with the following keys:
-          - 'display_name': Name used to identify this particular option
-          - 'choices': A dictionary containing list of choices for the user to choose from
+
+          - `display_name`: Name used to identify this particular option
+          - `choices`: A dictionary containing list of choices for the user to choose from
             to set the value for this particular option. The key is an identifier for this
             choice, and the value is a dictionary with the following possible keys:
-            - 'display_name': Human readable display name for this choice.
-            - 'default': (optional Bool) True if this is the default selected choice
-            - 'kubespawner_override': A dictionary with overrides to apply to the KubeSpawner
-              settings, on top of whatever was applied with the 'kubespawner_override' key
+
+            - `display_name`: Human readable display name for this choice.
+            - `default`: (optional Bool) True if this is the default selected choice
+            - `kubespawner_override`: A dictionary with overrides to apply to the KubeSpawner
+              settings, on top of whatever was applied with the `kubespawner_override` key
               for the profile itself. The key should be the name of the kubespawner setting,
               and value can be either the final value or a callable that returns the final
               value when called with the spawner instance as the only parameter. The callable
               may be async.
+              If the traitlet being overriden is a *dictionary*, the dictionary
+              will be *recursively updated*, rather than overriden. If you want to
+              remove a key, set its value to `None`
         - `default`: (optional Bool) True if this is the default selected option
 
         kubespawner setting overrides work in the following manner, with items further in the
         list *replacing* (not merging with) items earlier in the list:
 
         1. Settings directly set on KubeSpawner, via c.KubeSpawner.<traitlet_name>
         2. `kubespawner_override` in the profile the user has chosen
@@ -1909,15 +1887,17 @@
         return labels
 
     def _build_pod_labels(self, extra_labels):
         labels = self._build_common_labels(extra_labels)
         labels.update(
             {
                 'component': self.component_label,
-                'hub.jupyter.org/servername': self.name,
+                'hub.jupyter.org/servername': escapism.escape(
+                    self.name, safe=self.safe_chars, escape_char='-'
+                ).lower(),
             }
         )
         return labels
 
     def _build_common_annotations(self, extra_annotations):
         # Annotations don't need to be escaped
         annotations = {'hub.jupyter.org/username': self.user.name}
@@ -2051,15 +2031,15 @@
             gid=gid,
             fs_gid=fs_gid,
             supplemental_gids=supplemental_gids,
             privileged=self.privileged,
             allow_privilege_escalation=self.allow_privilege_escalation,
             container_security_context=csc,
             pod_security_context=psc,
-            env=self.get_env(),
+            env=self._expand_all(self.get_env()),
             volumes=self._expand_all(self.volumes),
             volume_mounts=self._expand_all(self.volume_mounts),
             working_dir=self.working_dir,
             labels=labels,
             annotations=annotations,
             cpu_limit=self.cpu_limit,
             cpu_guarantee=self.cpu_guarantee,
@@ -2113,20 +2093,21 @@
         Make a service manifest for dns.
         """
 
         labels = self._build_common_labels(self._expand_all(self.extra_labels))
         annotations = self._build_common_annotations(
             self._expand_all(self.extra_annotations)
         )
+        selector = self._build_pod_labels(self._expand_all(self.extra_labels))
 
         # TODO: validate that the service name
         return make_service(
             name=self.pod_name,
             port=self.port,
-            servername=self.name,
+            selector=selector,
             owner_references=[owner_reference],
             labels=labels,
             annotations=annotations,
         )
 
     def get_pvc_manifest(self):
         """
@@ -2184,17 +2165,22 @@
 
         We save the `pod_name`, even though we could easily compute it,
         because JupyterHub requires you save *some* state! Otherwise
         it assumes your server is dead. This works around that.
 
         It's also useful for cases when the `pod_template` changes between
         restarts - this keeps the old pods around.
+
+        We also save the namespace and DNS name for use cases where the namespace is
+        calculated dynamically, or it changes between restarts.
         """
         state = super().get_state()
         state['pod_name'] = self.pod_name
+        state['namespace'] = self.namespace
+        state['dns_name'] = self.dns_name
         return state
 
     def get_env(self):
         """Return the environment dict to use for the Spawner.
 
         See also: jupyterhub.Spawner.get_env
         """
@@ -2211,32 +2197,42 @@
         Load state from storage required to reinstate this user's pod
 
         Since this runs after `__init__`, this will override the generated `pod_name`
         if there's one we have saved in state. These are the same in most cases,
         but if the `pod_template` has changed in between restarts, it will no longer
         be the case. This allows us to continue serving from the old pods with
         the old names.
+
+        For a similar reason, we also save the namespace.
         """
         if 'pod_name' in state:
             self.pod_name = state['pod_name']
 
-    @_await_pod_reflector
+        if 'namespace' in state:
+            self.namespace = state['namespace']
+
+        if 'dns_name' in state:
+            self.dns_name = state['dns_name']
+
     async def poll(self):
         """
         Check if the pod is still running.
 
         Uses the same interface as subprocess.Popen.poll(): if the pod is
         still running, returns None.  If the pod has exited, return the
         exit code if we can determine it, or 1 if it has exited but we
         don't know how.  These are the return values JupyterHub expects.
 
         Note that a clean exit will have an exit code of zero, so it is
         necessary to check that the returned value is None, rather than
         just Falsy, to determine that the pod is still running.
         """
+
+        await self._start_watching_pods()
+
         ref_key = f"{self.namespace}/{self.pod_name}"
         pod = self.pod_reflector.pods.get(ref_key, None)
         if pod is not None:
             if pod["status"]["phase"] == 'Pending':
                 return None
             ctr_stat = pod["status"].get("containerStatuses")
             if ctr_stat is None:  # No status, no container (we hope)
@@ -2318,17 +2314,20 @@
         This function is reporting back the progress of spawning a pod until
         self._start_future has fired.
 
         This is working with events parsed by the python kubernetes client,
         and here is the specification of events that is relevant to understand:
         ref: https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#event-v1-core
         """
+
         if not self.events_enabled:
             return
 
+        await self._start_watching_events()
+
         self.log.debug('progress generator: %s', self.pod_name)
         start_future = self._start_future
         progress = 0
         next_event = 0
 
         break_while_loop = False
         while True:
@@ -2370,106 +2369,139 @@
                     }
                 next_event = len_events
 
             if break_while_loop:
                 break
             await asyncio.sleep(1)
 
-    def _start_reflector(
+    async def _start_reflector(
         self,
-        kind=None,
-        reflector_class=ResourceReflector,
-        replace=False,
+        kind: str,
+        reflector_class: Type[ResourceReflector],
+        replace: bool = False,
         **kwargs,
     ):
         """Start a shared reflector on the KubeSpawner class
 
-
-        kind: key for the reflector (e.g. 'pod' or 'events')
+        kind: used to generate key to store reflector shared instance (e.g. 'pod' or 'events')
         reflector_class: Reflector class to be instantiated
         kwargs: extra keyword-args to be relayed to ReflectorClass
 
         If replace=False and the pod reflector is already running,
         do nothing.
 
         If replace=True, a running pod reflector will be stopped
         and a new one started (for recovering from possible errors).
         """
-        key = kind
-        ReflectorClass = reflector_class
 
-        def on_reflector_failure():
-            self.log.critical(
-                "%s reflector failed, halting Hub.",
-                key.title(),
-            )
-            sys.exit(1)
+        key = self._get_reflector_key(kind)
+        previous_reflector = self.__class__.reflectors.get(key, None)
 
-        previous_reflector = self.__class__.reflectors.get(key)
+        if previous_reflector and not replace:
+            # fast path
+            return previous_reflector
 
-        if replace or not previous_reflector:
-            self.__class__.reflectors[key] = ReflectorClass(
-                parent=self,
-                namespace=self.namespace,
-                on_failure=on_reflector_failure,
-                **kwargs,
-            )
-            f = asyncio.ensure_future(self.__class__.reflectors[key].start())
+        if self.enable_user_namespaces:
+            # Create one reflector for all namespaces.
+            # This requires binding ServiceAccount to ClusterRole.
 
-            async def catch_reflector_start():
+            def on_reflector_failure():
+                # If reflector cannot be started, halt the JH application.
+                self.log.critical(
+                    "Reflector with key %r reflector, halting Hub.",
+                    key,
+                )
+                sys.exit(1)
+
+            async def catch_reflector_start(func):
                 try:
-                    await f
-                except Exception as e:
-                    self.log.exception(f"Reflector for {kind} failed to start.")
+                    await func
+                except Exception:
+                    self.log.exception(f"Reflector with key {key} failed to start.")
                     sys.exit(1)
 
-            asyncio.create_task(catch_reflector_start())
+        else:
+            # Create a dedicated reflector for each namespace.
+            # This allows JH to run pods in multiple namespaces without binding ServiceAccount to ClusterRole.
+
+            on_reflector_failure = None
+
+            async def catch_reflector_start(func):
+                # If reflector cannot be started (e.g. insufficient access rights, namespace cannot be found),
+                # just raise an exception instead halting the entire JH application.
+                try:
+                    await func
+                except Exception:
+                    self.log.exception(f"Reflector with key {key} failed to start.")
+                    raise
+
+        self.__class__.reflectors[key] = current_reflector = reflector_class(
+            parent=self,
+            namespace=self.namespace,
+            on_failure=on_reflector_failure,
+            **kwargs,
+        )
+        await catch_reflector_start(current_reflector.start())
 
-        if replace and previous_reflector:
+        if previous_reflector:
             # we replaced the reflector, stop the old one
             asyncio.ensure_future(previous_reflector.stop())
 
         # return the current reflector
-        return self.__class__.reflectors[key]
+        return current_reflector
 
-    def _start_watching_events(self, replace=False):
+    async def _start_watching_events(self, replace=False):
         """Start the events reflector
 
         If replace=False and the event reflector is already running,
         do nothing.
 
         If replace=True, a running pod reflector will be stopped
         and a new one started (for recovering from possible errors).
         """
-        return self._start_reflector(
+        return await self._start_reflector(
             kind="events",
             reflector_class=EventReflector,
             fields={"involvedObject.kind": "Pod"},
             omit_namespace=self.enable_user_namespaces,
             replace=replace,
         )
 
-    def _start_watching_pods(self, replace=False):
-        """Start the pod reflector
+    async def _start_watching_pods(self, replace=False):
+        """Start the pods reflector
 
         If replace=False and the pod reflector is already running,
         do nothing.
 
         If replace=True, a running pod reflector will be stopped
         and a new one started (for recovering from possible errors).
         """
-        pod_reflector_class = PodReflector
-        pod_reflector_class.labels.update({"component": self.component_label})
-        return self._start_reflector(
-            "pods",
-            PodReflector,
+        return await self._start_reflector(
+            kind="pods",
+            reflector_class=PodReflector,
+            labels={"component": self.component_label},
             omit_namespace=self.enable_user_namespaces,
             replace=replace,
         )
 
+    @classmethod
+    async def _stop_all_reflectors(cls):
+        """Stop reflectors for all instances, a function used when running tests."""
+        tasks = []
+        for key in list(cls.reflectors.keys()):
+            reflector = cls.reflectors.pop(key)
+            tasks.append(reflector.stop())
+
+        try:
+            await asyncio.gather(*tasks)
+        except Exception:
+            for task in tasks:
+                task.cancel()
+            raise
+
     def start(self):
         """Thin wrapper around self._start
 
         so we can hold onto a reference for the Future
         start returns, which we can use to terminate
         .progress()
         """
@@ -2645,14 +2677,26 @@
         await self.load_user_options()
 
         # If we have user_namespaces enabled, create the namespace.
         #  It's fine if it already exists.
         if self.enable_user_namespaces:
             await self._ensure_namespace()
 
+        # namespace can be changed via kubespawner_override, start watching pods only after
+        # load_user_options() is called
+        start_futures = [self._start_watching_pods()]
+        if self.events_enabled:
+            start_futures.append(self._start_watching_events())
+        try:
+            await asyncio.gather(*start_futures)
+        except Exception:
+            for future in start_futures:
+                future.cancel()
+            raise
+
         # record latest event so we don't include old
         # events from previous pods in self.events
         # track by order and name instead of uid
         # so we get events like deletion of a previously stale
         # pod if it's part of this spawn process
         events = self.events
         if events:
@@ -2767,15 +2811,15 @@
                 # if pod never showed up at all,
                 # restart the pod reflector which may have become disconnected.
                 self.log.error(
                     "Pod %s never showed up in reflector, restarting pod reflector",
                     ref_key,
                 )
                 self.log.error(f"Pods: {self.pod_reflector.pods}")
-                self._start_watching_pods(replace=True)
+                asyncio.ensure_future(self._start_watching_pods(replace=True))
             raise
 
         pod = self.pod_reflector.pods[ref_key]
         self.pod_id = pod["metadata"]["uid"]
         if self.event_reflector:
             self.log.debug(
                 'pod %s events before launch: %s',
@@ -2856,16 +2900,16 @@
                     pvc_name,
                 )
                 # If there isn't a PVC to delete, that's ok too!
                 return True
             else:
                 raise
 
-    @_await_pod_reflector
     async def stop(self, now=False):
+        await self._start_watching_pods()
 
         delete_options = client.V1DeleteOptions()
 
         if now:
             grace_seconds = 0
         else:
             grace_seconds = self.delete_grace_period
@@ -2892,15 +2936,15 @@
                 % (ref_key, self.start_timeout),
                 timeout=self.start_timeout,
             )
         except TimeoutError:
             self.log.error(
                 "Pod %s did not disappear, restarting pod reflector", ref_key
             )
-            self._start_watching_pods(replace=True)
+            asyncio.ensure_future(self._start_watching_pods(replace=True))
             raise
 
     @default('env_keep')
     def _env_keep_default(self):
         return []
 
     _profile_list = None
@@ -3012,15 +3056,23 @@
             if callable(v):
                 v = v(self)
                 self.log.debug(
                     ".. overriding KubeSpawner value %s=%s (callable result)", k, v
                 )
             else:
                 self.log.debug(".. overriding KubeSpawner value %s=%s", k, v)
-            setattr(self, k, v)
+
+            # If v is a dict, *merge* it with existing values, rather than completely
+            # resetting it. This allows *adding* things like environment variables rather
+            # than completely replacing them. If value is set to None, the key
+            # will be removed
+            if isinstance(v, dict) and isinstance(getattr(self, k), dict):
+                recursive_update(getattr(self, k), v)
+            else:
+                setattr(self, k, v)
 
         if profile.get('profile_options'):
             # each option specified here *must* have a value in our POST, as we
             # render our HTML such that there's always something selected.
 
             # We only honor options that are defined in the selected profile *and*
             # are in the form data posted. This prevents users who may be authorized
@@ -3028,15 +3080,15 @@
             # profiles
             for user_selected_option_name in selected_profile_user_options.keys():
                 if (
                     user_selected_option_name
                     not in profile.get('profile_options').keys()
                 ):
                     raise ValueError(
-                        f'Expected option {user_selected_option_name} for profile {slug}, not found in posted form'
+                        f'Expected option {user_selected_option_name} for profile {profile["slug"]}, not found in posted form'
                     )
 
             # Get selected options or default to the first option if none is passed
             for option_name, option in profile.get('profile_options').items():
                 chosen_option = selected_profile_user_options.get(option_name, None)
                 # If none was selected get the default
                 if not chosen_option:
@@ -3056,15 +3108,23 @@
                         self.log.debug(
                             f'.. overriding traitlet {k}={v} for option {option_name}={chosen_option} from callabale'
                         )
                     else:
                         self.log.debug(
                             f'.. overriding traitlet {k}={v} for option {option_name}={chosen_option}'
                         )
-                    setattr(self, k, v)
+
+                    # If v is a dict, *merge* it with existing values, rather than completely
+                    # resetting it. This allows *adding* things like environment variables rather
+                    # than completely replacing them. If value is set to None, the key
+                    # will be removed
+                    if isinstance(v, dict) and isinstance(getattr(self, k), dict):
+                        recursive_update(getattr(self, k), v)
+                    else:
+                        setattr(self, k, v)
 
     # set of recognised user option keys
     # used for warning about ignoring unrecognised options
     _user_option_keys = {'profile'}
 
     def _init_profile_list(self, profile_list):
         # generate missing slug fields from display_name
```

### Comparing `jupyterhub-kubespawner-4.3.0/kubespawner/utils.py` & `jupyterhub_kubespawner-5.0.0/kubespawner/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -182,7 +182,43 @@
             return key
     else:
         raise ValueError(
             "'{}' did not have an attribute matching '{}'".format(
                 model_type.__name__, field_name
             )
         )
+
+
+def host_matching(host: str, wildcard: str) -> bool:
+    # user.example.com == user.example.com
+    # user.example.com != wrong.example.com
+    # user.example.com != example.com
+    if not wildcard.startswith("*."):
+        return host == wildcard
+
+    host_parts = host.split(".")
+    wildcard_parts = wildcard.split(".")
+
+    # user.example.com =~ *.example.com
+    # user.example.com !~ *.user.example.com
+    # user.example.com !~ *.example
+    return host_parts[1:] == wildcard_parts[1:]
+
+
+# From https://github.com/jupyter-server/jupyter_server/blob/fc0ac3236fdd92778ea765db6e8982212c8389ee/jupyter_server/config_manager.py#L14
+def recursive_update(target, new):
+    """
+    Recursively update one dictionary in-place using another.
+
+    None values will delete their keys.
+    """
+    for k, v in new.items():
+        if isinstance(v, dict):
+            if k not in target:
+                target[k] = {}
+            recursive_update(target[k], v)
+
+        elif v is None:
+            target.pop(k, None)
+
+        else:
+            target[k] = v
```

