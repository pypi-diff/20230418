# Comparing `tmp/dbt_feature_flags-0.4.1.tar.gz` & `tmp/dbt_feature_flags-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_feature_flags-0.4.1.tar", max compression
+gzip compressed data, was "dbt_feature_flags-0.5.0.tar", max compression
```

## Comparing `dbt_feature_flags-0.4.1.tar` & `dbt_feature_flags-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0    10142 2022-11-06 16:29:25.073909 dbt_feature_flags-0.4.1/LICENSE
--rw-r--r--   0        0        0     9611 2022-11-06 16:27:14.455036 dbt_feature_flags-0.4.1/README.md
--rw-r--r--   0        0        0      598 2022-11-06 16:30:32.539379 dbt_feature_flags-0.4.1/dbt_feature_flags/__init__.py
--rw-r--r--   0        0        0     3292 2022-11-06 16:29:55.680821 dbt_feature_flags-0.4.1/dbt_feature_flags/base.py
--rw-r--r--   0        0        0     3894 2022-11-06 16:29:59.959324 dbt_feature_flags-0.4.1/dbt_feature_flags/harness.py
--rw-r--r--   0        0        0     2524 2022-11-06 16:30:04.858005 dbt_feature_flags-0.4.1/dbt_feature_flags/launchdarkly.py
--rw-r--r--   0        0        0     1550 2022-11-06 16:30:08.337438 dbt_feature_flags-0.4.1/dbt_feature_flags/mock.py
--rw-r--r--   0        0        0     2591 2022-11-06 16:30:19.501417 dbt_feature_flags-0.4.1/dbt_feature_flags/patch.py
--rw-r--r--   0        0        0      609 2022-11-06 16:11:36.682608 dbt_feature_flags-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       70 2022-07-30 05:05:11.823869 dbt_feature_flags-0.4.1/zzz_dbt_feature_flags.pth
--rw-r--r--   0        0        0    10543 1970-01-01 00:00:00.000000 dbt_feature_flags-0.4.1/setup.py
--rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 dbt_feature_flags-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-11-06 16:29:25.073909 dbt_feature_flags-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9611 2022-11-06 16:27:14.455036 dbt_feature_flags-0.5.0/README.md
+-rw-r--r--   0        0        0      598 2022-11-06 16:30:32.539379 dbt_feature_flags-0.5.0/dbt_feature_flags/__init__.py
+-rw-r--r--   0        0        0     3292 2022-11-06 16:29:55.680821 dbt_feature_flags-0.5.0/dbt_feature_flags/base.py
+-rw-r--r--   0        0        0     3922 2023-04-18 06:39:35.939005 dbt_feature_flags-0.5.0/dbt_feature_flags/harness.py
+-rw-r--r--   0        0        0     2524 2022-11-06 16:30:04.858005 dbt_feature_flags-0.5.0/dbt_feature_flags/launchdarkly.py
+-rw-r--r--   0        0        0     3241 2023-04-18 06:46:15.524831 dbt_feature_flags-0.5.0/dbt_feature_flags/patch.py
+-rw-r--r--   0        0        0      609 2023-04-18 06:39:10.390159 dbt_feature_flags-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-07-30 05:05:11.823869 dbt_feature_flags-0.5.0/zzz_dbt_feature_flags.pth
+-rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 dbt_feature_flags-0.5.0/PKG-INFO
```

### Comparing `dbt_feature_flags-0.4.1/LICENSE` & `dbt_feature_flags-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.4.1/README.md` & `dbt_feature_flags-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.4.1/dbt_feature_flags/__init__.py` & `dbt_feature_flags-0.5.0/dbt_feature_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.4.1/dbt_feature_flags/base.py` & `dbt_feature_flags-0.5.0/dbt_feature_flags/base.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.4.1/dbt_feature_flags/harness.py` & `dbt_feature_flags-0.5.0/dbt_feature_flags/harness.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 class HarnessFeatureFlagsClient(BaseFeatureFlagsClient):
     def __init__(self):
         # Lazy imports
         import logging
         import os
 
         from featureflags.api.client import Client
-        from featureflags.api.default.get_all_segments import sync as retrieve_segments
-        from featureflags.api.default.get_feature_config import sync as retrieve_flags
+        from featureflags.api.default.get_all_segments import \
+            sync as retrieve_segments
+        from featureflags.api.default.get_feature_config import \
+            sync as retrieve_flags
         from featureflags.client import CfClient, Target
         from featureflags.client import log as logger
         from featureflags.config import Config
         from featureflags.evaluations.evaluator import Evaluator
         from featureflags.repository import Repository
 
         # Override default logging to preserve stderr (needed for dbt-bigquery)
```

### Comparing `dbt_feature_flags-0.4.1/dbt_feature_flags/launchdarkly.py` & `dbt_feature_flags-0.5.0/dbt_feature_flags/launchdarkly.py`

 * *Files identical despite different names*

### Comparing `dbt_feature_flags-0.4.1/dbt_feature_flags/patch.py` & `dbt_feature_flags-0.5.0/dbt_feature_flags/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,74 +7,100 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import os
+import typing as t
 from enum import Enum
+from functools import wraps
 
-from dbt_feature_flags import base, harness, launchdarkly, mock
+from dbt_feature_flags import base, harness, launchdarkly
+
+_MOCK_CLIENT = object()
 
 
 class SupportedProviders(str, Enum):
     Harness = "harness"
     LaunchDarkly = "launchdarkly"
     NoopClient = "mock"
 
 
-def _get_client() -> base.BaseFeatureFlagsClient:
-    """Return the user specified client, valid impementations MUST
-    inherit from BaseFeatureFlagsClient"""
-    ff_provider = os.getenv("FF_PROVIDER")
-    ff_client = None
-    if os.getenv("DBT_FF_DISABLE") or not ff_provider:
-        ff_client = mock.MockFeatureFlagClient()
-    elif ff_provider == SupportedProviders.Harness:
-        ff_client = harness.HarnessFeatureFlagsClient()
-    elif ff_provider == SupportedProviders.LaunchDarkly:
-        ff_client = launchdarkly.LaunchDarklyFeatureFlagsClient()
-    if not isinstance(ff_client, base.BaseFeatureFlagsClient):
+def _is_truthy(value: str) -> bool:
+    """Return True if the value is truthy, False otherwise."""
+    return value.lower() in ("1", "true", "yes")
+
+
+def _get_client() -> base.BaseFeatureFlagsClient | _MOCK_CLIENT:
+    """Return the user specified client.
+
+    Valid implementations MUST inherit from BaseFeatureFlagsClient.
+    """
+    provider, client = os.getenv("DBT_FF_PROVIDER"), None
+
+    if _is_truthy(os.getenv("DBT_FF_DISABLE", "0")):
+        client = _MOCK_CLIENT
+    elif not provider:
+        client = _MOCK_CLIENT
+    elif provider == SupportedProviders.Harness:
+        client = harness.HarnessFeatureFlagsClient()
+    elif provider == SupportedProviders.LaunchDarkly:
+        client = launchdarkly.LaunchDarklyFeatureFlagsClient()
+
+    if client is not _MOCK_CLIENT and not isinstance(
+        client, base.BaseFeatureFlagsClient
+    ):
         raise RuntimeError(
-            "Invalid feature flag client specified by (FF_PROVIDER=%s)",
-            ff_provider,
+            "Invalid dbt feature flag client specified by (DBT_FF_PROVIDER=%s)",
+            provider,
         )
-    return ff_client
-
 
-def patch_dbt_environment() -> None:
-    import functools
-
-    from dbt.clients import jinja
+    return client
 
-    # Getting environment function from dbt
-    jinja._get_environment = jinja.get_environment
 
-    # FF client
-    ff_client = _get_client()
+def get_rendered(
+    fn: t.Callable,
+    client: base.BaseFeatureFlagsClient,
+):
+    """Patch dbt's jinja environment to include feature flag functions."""
+
+    if getattr(fn, "status", None) == "patched":
+        return fn
+
+    @wraps(fn)
+    def _wrapped(
+        string: str,
+        ctx: t.Dict[str, t.Any],
+        node=None,
+        capture_macros: bool = False,
+        native: bool = False,
+    ):
+        if client is _MOCK_CLIENT:
+            ctx["feature_flag"] = ctx["var"]
+            ctx["feature_flag_str"] = ctx["var"]
+            ctx["feature_flag_num"] = ctx["var"]
+            ctx["feature_flag_json"] = ctx["var"]
+        else:
+            ctx["feature_flag"] = client.bool_variation
+            ctx["feature_flag_str"] = client.string_variation
+            ctx["feature_flag_num"] = client.number_variation
+            ctx["feature_flag_json"] = client.json_variation
+        return fn(string, ctx, node, capture_macros, native)
 
-    def add_ff_extension(func):
-        if getattr(func, "status", None) == "patched":
-            return func
+    _wrapped.status = "patched"
+    return _wrapped
 
-        @functools.wraps(func)
-        def with_ff_extension(*args, **kwargs):
-            env = func(*args, **kwargs)
-            env.globals["feature_flag"] = ff_client.bool_variation
-            env.globals["feature_flag_str"] = ff_client.string_variation
-            env.globals["feature_flag_num"] = ff_client.number_variation
-            env.globals["feature_flag_json"] = ff_client.json_variation
-            return env
 
-        with_ff_extension.status = "patched"
-
-        return with_ff_extension
-
-    env_with_ff = add_ff_extension(jinja._get_environment)
+def patch_dbt_environment() -> None:
+    """Patch dbt's jinja environment to include feature flag functions."""
+    from dbt.clients import jinja
 
-    jinja.get_environment = env_with_ff
+    jinja._get_rendered = jinja.get_rendered
+    jinja.get_rendered = get_rendered(jinja._get_rendered, _get_client())
 
 
 if __name__ == "__main__":
     patch_dbt_environment()
```

### Comparing `dbt_feature_flags-0.4.1/pyproject.toml` & `dbt_feature_flags-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-feature-flags"
-version = "0.4.1"
+version = "0.5.0"
 description = "Use feature flags in dbt models"
 authors = ["z3z1ma <butler.alex2010@gmail.com>"]
 include = ["zzz_dbt_feature_flags.pth"]
 readme = "README.md"
 repository = "https://github.com/z3z1ma/dbt-feature-flags"
 homepage = "https://github.com/z3z1ma/dbt-feature-flags"
```

### Comparing `dbt_feature_flags-0.4.1/setup.py` & `dbt_feature_flags-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dbt-feature-flags
+Version: 0.5.0
+Summary: Use feature flags in dbt models
+Home-page: https://github.com/z3z1ma/dbt-feature-flags
+Author: z3z1ma
+Author-email: butler.alex2010@gmail.com
+Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dbt-core (>=1.0.0)
+Requires-Dist: harness-featureflags (>=1.1.3,<2.0.0)
+Requires-Dist: launchdarkly-server-sdk (>=7.5.1,<8.0.0)
+Project-URL: Repository, https://github.com/z3z1ma/dbt-feature-flags
+Description-Content-Type: text/markdown
+
+# dbt-feature-flags
+
+![PyPI](https://img.shields.io/pypi/v/dbt-feature-flags)
+![Downloads](https://pepy.tech/badge/dbt-feature-flags)
+![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)
+![black](https://img.shields.io/badge/code%20style-black-000000.svg)
+![example workflow](https://github.com/z3z1ma/dbt-feature-flags/actions/workflows/run-tests.yml/badge.svg)
+
+## Why Feature Flags?
+
+> At a foundational level, feature flags enable code to be committed and deployed to production in a dormant state and then activated later. This gives teams more control over the user experience of the end product. Development teams can choose when and to which users new code is delivered. - Atlassian (Ian Buchannan)
+
+
+More often data is being called a product. Furthermore software engineering best practices have continued to show their effectiveness in the lifecycle of data model / product development. Commits, pull requests, code reviews, merges, versioning, CI/CD, feature branches, agile sprints, etc. Today, when much of data warehousing encourages an extract, load, transform pattern, we fundamentally have more paths we can take to reach our end goal of data marts. Deferred transformation means we have almost all of the possibilities that are available to slice, dice, aggregate, and join as there can be as opposed to ETL where predefined and much less agile transformations mutate the data away from its original representation. 
+
+This ELT pattern heavily encourages experimentation. dbt-feature-flags allow dbt developers to control SQL deployed at runtime. This allows faster iterations, faster & safer merges, and much safer experimentation. For example putting out a new v2 KPI column in a data mart behind a feature flag allows you to toggle between v1 and v2 in production without fear of regression. The same is applicable with rolling out a new `ref` to replace an old one. You could even toggle an entire experimental data mart on or off. You could put BigQuery ML models behind these flags, etc. If you "need" a data model in production but aren't confident in it, you can roll it out with the safety net of you or even a non-engineer being able to toggle it off. 
+
+## Usage
+
+This integration uses a mock client by default. The mock client serves up (optionally user-specified) defaults. These defaults can be defined centrally via `vars` which provides a 2-layer approach for more advanced uses, or alternatively they can be specified inline, statically. Execution with the mock client is only enabled so projects using dbt-feature-flags are _always_ executable regardless of being connected to a provider. Harness Feature Flags is the recommended provider. Sign up [here](https://harness.io/products/feature-flags). It's free to use and provides the interface for controlling your feature flags. 
+
+Interface
+![flow](https://files.helpdocs.io/kw8ldg1itf/articles/1j7pdkqh7j/1657792368788/screenshot-2022-07-14-at-10-52-03.png)
+
+Alternatively we also support [LaunchDarkly](https://launchdarkly.com/) and the package is architected in such a way that adding a new client is fairly straightforward.
+
+### Set Up
+
+Supported clients
+
+| clients      | supported |
+|--------------|-----------|
+| harness      | ✅         |
+| launchdarkly | ✅         |
+| unleashed    | ⛔️         |
+
+**Required env vars:**
+
+`FF_PROVIDER` - Must be one of above supported providers exactly as shown. Defaults to a mock client if unset. The mock client serves up defaults so that your project can run without any dependence on the FF provider. To override the default mock client and use a provider: FF_PROVIDER=harness
+
+`DBT_FF_API_KEY` - your feature flags SDK key. Instructions [here](https://docs.harness.io/article/1j7pdkqh7j-create-a-feature-flag#step_3_create_an_sdk_key) to set up a harness key. Because of the server-side use case with no client SDKs in play, the Harness free tier can sustain **any size** dbt deployment. Alternatively sign up for LaunchDarkly [here](https://launchdarkly.com/start-trial/).
+
+**Optional:**
+
+`DBT_TARGET` - this lets you serve different flag evaluations to different targets. This variable should be set by the user/server where dbt is running and mostly intuitively correlates to dbt targets but could technically be anything you want to differentiate and serve differently. When unset, `default` is the default target value and is also reasonable if differentiating is unimportant
+
+`DBT_FF_DISABLE` - disable the patch, note that feature_flag expressions will cause your dbt models not to compile until removed or replaced. If you have the package as a dependency and aren't using it, you can save a second of initialization
+
+### Jinja Functions
+
+These are available *anywhere* dbt jinja is evaluated. That includes profiles.yml, dbt_project.yml, models, macros, etc.
+
+`feature_flag(flag: str) -> bool`: Looks for boolean variation flag. By default returns False. Most flags are boolean. Will throw ValueError if different return type is detected.
+
+`feature_flag_str(flag: str) -> str`: Looks for string variation flag. By default returns "". Will throw ValueError if different return type is detected.
+
+`feature_flag_num(flag: str) -> float | int`: Looks for number variation flag. By default returns 0. Will throw ValueError if different return type is detected.
+
+`feature_flag_json(flag: str) -> dict | list`: Looks for json variation flag. By default returns an empty dict {}. Will throw ValueError if different return type is detected.
+
+## Examples
+
+A contrived example:
+
+```sql
+-- Use a feature_flag call as a bool value
+{{ config(enabled=feature_flag("custom_date_model", default=false)) }}
+
+select
+    * -- Example below uses FF + var macro for the default so you can toggle it while offline
+    {%- if feature_flag("new_relative_date_columns", default=var("new_relative_date_columns", false)) %},
+    case
+        when current_date between fiscal_quarter_start_date and fiscal_quarter_end_date
+            then 'Current'
+        when current_date < fiscal_quarter_start_date then 'Future'
+        when current_date > fiscal_quarter_end_date then 'Past'
+    end as relative_fiscal_quarter,
+    case
+        when current_date between fiscal_year_start_date and fiscal_year_end_date
+            then 'Current'
+        when current_date < fiscal_year_start_date then 'Future'
+        when current_date > fiscal_year_end_date then 'Past'
+    end as relative_fiscal_year
+    {% endif %}
+from
+    {{ ref('dim_dates__base') }}
+```
+
+BQ ML model example (this could be ran in a `run-operation`, feature flags are valid anywhere dbt evaluates jinja)
+
+```sql
+create or replace model `bqml_tutorial.penguins_model`
+options (
+  model_type='linear_reg',
+  input_label_cols=['body_mass_g'] ) as
+select
+  *
+from
+  {{ source('ml_datasets', 'penguins') }}
+where
+  {% if feature_flag("penguins_model_min_weight_filter") %}
+  body_mass_g > 100
+  {% else %}
+  body_mass_g is not null
+  {% endif %}
+```
+
+Another BQ ML example
+
+```sql
+select
+  *
+from
+  ml.evaluate(
+  {% if feature_flag("use_v2_ml_model") %}
+  model `bqml_tutorial.penguins_model_v2`,
+  {% else %}
+  model `bqml_tutorial.penguins_model`,
+  {% endif %} (
+    select
+      *
+    from
+      {{ source('ml_datasets', 'penguins') }}
+    where
+      body_mass_g is not null
+))
+```
+
+A dbt yaml example
+
+```yaml
+models:
+  project:
+    new_expermental_marts:
+      +schema: experimental
+      +enabled: "{{ feature_flag('use_new_marts') }}"
+
+```
+
+## Closing Remarks
+
+Given that most of what is relevant to software is either directly or periphally relevant to data product development, we will continue to pull the description from Atlassian:
+
+> ## Validate feature functionality
+> Developers can leverage feature flags to perform “soft rollouts” of new product features. New features can be built with immediate integration of feature toggles as part of the expected release. The feature flag can be set to "off" by default so that once the code is deployed, it remains dormant during production and the new feature will be disabled until the feature toggle is explicitly activated. Teams then choose when to turn on the feature flag, which activates the code, allowing teams to perform QA and verify that it behaves as expected. If the team discovers an issue during this process, they can immediately turn off the feature flag to disable the new code and minimize user exposure to the issue.
+> ## Minimize risk
+> Building on the idea of soft rollouts discussed above, industrious teams can leverage feature flags in conjunction with system monitoring and metrics as a response to any observable intermittent issues. For example, if an application experiences a spike in traffic and the monitoring system reports an uptick in issues, the team may use feature flags to disable poorly performing features.
+> ## Modify system behavior without disruptive changes
+> Feature flags can be used to help minimize complicated code integration and deployment scenarios. Complicated new features or sensitive refactor work can be challenging to integrate into the main production branch of a repository. This is further complicated if multiple developers work on overlapping parts of the codebase. 
+> Feature flags can be used to isolate new changes while known, stable code remains in place. This helps developers avoid long-running feature branches by committing frequently to the main branch of a repository behind the feature toggle. When the new code is ready there is no need for a disruptive collaborative merge and deploy scenario; the team can toggle the feature flag to enable the new system.
 
-packages = \
-['dbt_feature_flags']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dbt-core>=1.0.0',
- 'harness-featureflags>=1.1.3,<2.0.0',
- 'launchdarkly-server-sdk>=7.5.1,<8.0.0']
-
-setup_kwargs = {
-    'name': 'dbt-feature-flags',
-    'version': '0.4.1',
-    'description': 'Use feature flags in dbt models',
-    'long_description': '# dbt-feature-flags\n\n![PyPI](https://img.shields.io/pypi/v/dbt-feature-flags)\n![Downloads](https://pepy.tech/badge/dbt-feature-flags)\n![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)\n![black](https://img.shields.io/badge/code%20style-black-000000.svg)\n![example workflow](https://github.com/z3z1ma/dbt-feature-flags/actions/workflows/run-tests.yml/badge.svg)\n\n## Why Feature Flags?\n\n> At a foundational level, feature flags enable code to be committed and deployed to production in a dormant state and then activated later. This gives teams more control over the user experience of the end product. Development teams can choose when and to which users new code is delivered. - Atlassian (Ian Buchannan)\n\n\nMore often data is being called a product. Furthermore software engineering best practices have continued to show their effectiveness in the lifecycle of data model / product development. Commits, pull requests, code reviews, merges, versioning, CI/CD, feature branches, agile sprints, etc. Today, when much of data warehousing encourages an extract, load, transform pattern, we fundamentally have more paths we can take to reach our end goal of data marts. Deferred transformation means we have almost all of the possibilities that are available to slice, dice, aggregate, and join as there can be as opposed to ETL where predefined and much less agile transformations mutate the data away from its original representation. \n\nThis ELT pattern heavily encourages experimentation. dbt-feature-flags allow dbt developers to control SQL deployed at runtime. This allows faster iterations, faster & safer merges, and much safer experimentation. For example putting out a new v2 KPI column in a data mart behind a feature flag allows you to toggle between v1 and v2 in production without fear of regression. The same is applicable with rolling out a new `ref` to replace an old one. You could even toggle an entire experimental data mart on or off. You could put BigQuery ML models behind these flags, etc. If you "need" a data model in production but aren\'t confident in it, you can roll it out with the safety net of you or even a non-engineer being able to toggle it off. \n\n## Usage\n\nThis integration uses a mock client by default. The mock client serves up (optionally user-specified) defaults. These defaults can be defined centrally via `vars` which provides a 2-layer approach for more advanced uses, or alternatively they can be specified inline, statically. Execution with the mock client is only enabled so projects using dbt-feature-flags are _always_ executable regardless of being connected to a provider. Harness Feature Flags is the recommended provider. Sign up [here](https://harness.io/products/feature-flags). It\'s free to use and provides the interface for controlling your feature flags. \n\nInterface\n![flow](https://files.helpdocs.io/kw8ldg1itf/articles/1j7pdkqh7j/1657792368788/screenshot-2022-07-14-at-10-52-03.png)\n\nAlternatively we also support [LaunchDarkly](https://launchdarkly.com/) and the package is architected in such a way that adding a new client is fairly straightforward.\n\n### Set Up\n\nSupported clients\n\n| clients      | supported |\n|--------------|-----------|\n| harness      | ✅         |\n| launchdarkly | ✅         |\n| unleashed    | ⛔️         |\n\n**Required env vars:**\n\n`FF_PROVIDER` - Must be one of above supported providers exactly as shown. Defaults to a mock client if unset. The mock client serves up defaults so that your project can run without any dependence on the FF provider. To override the default mock client and use a provider: FF_PROVIDER=harness\n\n`DBT_FF_API_KEY` - your feature flags SDK key. Instructions [here](https://docs.harness.io/article/1j7pdkqh7j-create-a-feature-flag#step_3_create_an_sdk_key) to set up a harness key. Because of the server-side use case with no client SDKs in play, the Harness free tier can sustain **any size** dbt deployment. Alternatively sign up for LaunchDarkly [here](https://launchdarkly.com/start-trial/).\n\n**Optional:**\n\n`DBT_TARGET` - this lets you serve different flag evaluations to different targets. This variable should be set by the user/server where dbt is running and mostly intuitively correlates to dbt targets but could technically be anything you want to differentiate and serve differently. When unset, `default` is the default target value and is also reasonable if differentiating is unimportant\n\n`DBT_FF_DISABLE` - disable the patch, note that feature_flag expressions will cause your dbt models not to compile until removed or replaced. If you have the package as a dependency and aren\'t using it, you can save a second of initialization\n\n### Jinja Functions\n\nThese are available *anywhere* dbt jinja is evaluated. That includes profiles.yml, dbt_project.yml, models, macros, etc.\n\n`feature_flag(flag: str) -> bool`: Looks for boolean variation flag. By default returns False. Most flags are boolean. Will throw ValueError if different return type is detected.\n\n`feature_flag_str(flag: str) -> str`: Looks for string variation flag. By default returns "". Will throw ValueError if different return type is detected.\n\n`feature_flag_num(flag: str) -> float | int`: Looks for number variation flag. By default returns 0. Will throw ValueError if different return type is detected.\n\n`feature_flag_json(flag: str) -> dict | list`: Looks for json variation flag. By default returns an empty dict {}. Will throw ValueError if different return type is detected.\n\n## Examples\n\nA contrived example:\n\n```sql\n-- Use a feature_flag call as a bool value\n{{ config(enabled=feature_flag("custom_date_model", default=false)) }}\n\nselect\n    * -- Example below uses FF + var macro for the default so you can toggle it while offline\n    {%- if feature_flag("new_relative_date_columns", default=var("new_relative_date_columns", false)) %},\n    case\n        when current_date between fiscal_quarter_start_date and fiscal_quarter_end_date\n            then \'Current\'\n        when current_date < fiscal_quarter_start_date then \'Future\'\n        when current_date > fiscal_quarter_end_date then \'Past\'\n    end as relative_fiscal_quarter,\n    case\n        when current_date between fiscal_year_start_date and fiscal_year_end_date\n            then \'Current\'\n        when current_date < fiscal_year_start_date then \'Future\'\n        when current_date > fiscal_year_end_date then \'Past\'\n    end as relative_fiscal_year\n    {% endif %}\nfrom\n    {{ ref(\'dim_dates__base\') }}\n```\n\nBQ ML model example (this could be ran in a `run-operation`, feature flags are valid anywhere dbt evaluates jinja)\n\n```sql\ncreate or replace model `bqml_tutorial.penguins_model`\noptions (\n  model_type=\'linear_reg\',\n  input_label_cols=[\'body_mass_g\'] ) as\nselect\n  *\nfrom\n  {{ source(\'ml_datasets\', \'penguins\') }}\nwhere\n  {% if feature_flag("penguins_model_min_weight_filter") %}\n  body_mass_g > 100\n  {% else %}\n  body_mass_g is not null\n  {% endif %}\n```\n\nAnother BQ ML example\n\n```sql\nselect\n  *\nfrom\n  ml.evaluate(\n  {% if feature_flag("use_v2_ml_model") %}\n  model `bqml_tutorial.penguins_model_v2`,\n  {% else %}\n  model `bqml_tutorial.penguins_model`,\n  {% endif %} (\n    select\n      *\n    from\n      {{ source(\'ml_datasets\', \'penguins\') }}\n    where\n      body_mass_g is not null\n))\n```\n\nA dbt yaml example\n\n```yaml\nmodels:\n  project:\n    new_expermental_marts:\n      +schema: experimental\n      +enabled: "{{ feature_flag(\'use_new_marts\') }}"\n\n```\n\n## Closing Remarks\n\nGiven that most of what is relevant to software is either directly or periphally relevant to data product development, we will continue to pull the description from Atlassian:\n\n> ## Validate feature functionality\n> Developers can leverage feature flags to perform “soft rollouts” of new product features. New features can be built with immediate integration of feature toggles as part of the expected release. The feature flag can be set to "off" by default so that once the code is deployed, it remains dormant during production and the new feature will be disabled until the feature toggle is explicitly activated. Teams then choose when to turn on the feature flag, which activates the code, allowing teams to perform QA and verify that it behaves as expected. If the team discovers an issue during this process, they can immediately turn off the feature flag to disable the new code and minimize user exposure to the issue.\n> ## Minimize risk\n> Building on the idea of soft rollouts discussed above, industrious teams can leverage feature flags in conjunction with system monitoring and metrics as a response to any observable intermittent issues. For example, if an application experiences a spike in traffic and the monitoring system reports an uptick in issues, the team may use feature flags to disable poorly performing features.\n> ## Modify system behavior without disruptive changes\n> Feature flags can be used to help minimize complicated code integration and deployment scenarios. Complicated new features or sensitive refactor work can be challenging to integrate into the main production branch of a repository. This is further complicated if multiple developers work on overlapping parts of the codebase. \n> Feature flags can be used to isolate new changes while known, stable code remains in place. This helps developers avoid long-running feature branches by committing frequently to the main branch of a repository behind the feature toggle. When the new code is ready there is no need for a disruptive collaborative merge and deploy scenario; the team can toggle the feature flag to enable the new system.\n',
-    'author': 'z3z1ma',
-    'author_email': 'butler.alex2010@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/z3z1ma/dbt-feature-flags',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4',
-}
-
-
-setup(**setup_kwargs)
```

