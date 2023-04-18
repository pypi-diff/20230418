# Comparing `tmp/astronomer_cosmos-0.6.0.dev0.tar.gz` & `tmp/astronomer_cosmos-0.6.1.tar.gz`

## Comparing `astronomer_cosmos-0.6.0.dev0.tar` & `astronomer_cosmos-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/LICENSE
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/README.rst
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0     7255 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11586 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/README.rst
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.1/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/docker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from __future__ import annotations
 
 import logging
 from typing import Sequence
 
 import yaml
-from airflow.providers.docker.operators.docker import DockerOperator
 from airflow.utils.context import Context
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
 
+# docker is an optional dependency, so we need to check if it's installed
+try:
+    from airflow.providers.docker.operators.docker import DockerOperator
+except ImportError:
+    raise ImportError(
+        "Could not import DockerOperator. Ensure you've installed the docker provider separately or "
+        "with with `pip install astronomer-cosmos[...,docker]`."
+    )
+
 
 class DbtDockerBaseOperator(DockerOperator, DbtBaseOperator):
     """
     Executes a dbt core cli command in a Docker container.
 
     """
```

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from __future__ import annotations
 
 import logging
 from typing import Sequence
 
 import yaml
-from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
-    convert_env_vars,
-)
-from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import (
-    KubernetesPodOperator,
-)
 from airflow.utils.context import Context
-from kubernetes.client import models as k8s
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
 
+# kubernetes is an optional dependency, so we need to check if it's installed
+try:
+    from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
+        convert_env_vars,
+    )
+    from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import (
+        KubernetesPodOperator,
+    )
+    from kubernetes.client import models as k8s
+except ImportError:
+    raise ImportError(
+        "Could not import KubernetesPodOperator. Ensure you've installed the Kubernetes provider "
+        "separately or with with `pip install astronomer-cosmos[...,kubernetes]`."
+    )
+
 
 class DbtKubernetesBaseOperator(KubernetesPodOperator, DbtBaseOperator):
     """
     Executes a dbt core cli command in a Kubernetes Pod.
 
     """
```

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.1/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/.gitignore` & `astronomer_cosmos-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/LICENSE` & `astronomer_cosmos-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/README.rst` & `astronomer_cosmos-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.0.dev0/pyproject.toml` & `astronomer_cosmos-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,14 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "apache-airflow>=2.4",
-    "apache-airflow-providers-docker>=3.5.0",
-    "apache-airflow-providers-cncf-kubernetes>=5.1.1",
-    "filelock",
     "Jinja2>=3.0.0",
     "typing-extensions; python_version < '3.8'",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
     "dbt-bigquery",
@@ -92,14 +89,21 @@
     "requests-mock",
     "pytest-cov",
     "pytest-describe",
     "types-requests",
     "mypy",
     "sqlalchemy-stubs", # Change when sqlalchemy is upgraded https://docs.sqlalchemy.org/en/14/orm/extensions/mypy.html
 ]
+docker = [
+    "apache-airflow-providers-docker>=3.5.0",
+]
+kubernetes = [
+    "apache-airflow-providers-cncf-kubernetes>=5.1.1",
+]
+
 
 [project.urls]
 Homepage = "https://github.com/astronomer/astronomer-cosmos"
 Documentation = "https://github.com/astronomer/astronomer-cosmos"
 
 [tool.hatch.version]
 path = "cosmos/__init__.py"
```

### Comparing `astronomer_cosmos-0.6.0.dev0/PKG-INFO` & `astronomer_cosmos-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.0.dev0
+Version: 0.6.1
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -18,18 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
-Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1
-Requires-Dist: apache-airflow-providers-docker>=3.5.0
 Requires-Dist: apache-airflow>=2.4
-Requires-Dist: filelock
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
@@ -49,20 +46,24 @@
 Requires-Dist: openlineage-dbt>=0.21.1; extra == 'dbt-openlineage'
 Provides-Extra: dbt-postgres
 Requires-Dist: dbt-postgres; extra == 'dbt-postgres'
 Provides-Extra: dbt-redshift
 Requires-Dist: dbt-redshift; extra == 'dbt-redshift'
 Provides-Extra: dbt-snowflake
 Requires-Dist: dbt-snowflake; extra == 'dbt-snowflake'
+Provides-Extra: docker
+Requires-Dist: apache-airflow-providers-docker>=3.5.0; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-tabs; extra == 'docs'
+Provides-Extra: kubernetes
+Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
 Requires-Dist: pytest>=6.0; extra == 'tests'
```

