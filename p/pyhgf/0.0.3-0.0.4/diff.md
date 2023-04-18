# Comparing `tmp/pyhgf-0.0.3.tar.gz` & `tmp/pyhgf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgf-0.0.3.tar", last modified: Sun Mar 19 20:14:39 2023, max compression
+gzip compressed data, was "pyhgf-0.0.4.tar", last modified: Tue Apr 18 16:32:25 2023, max compression
```

## Comparing `pyhgf-0.0.3.tar` & `pyhgf-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:14:39.440641 pyhgf-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-03-19 20:14:28.000000 pyhgf-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-19 20:14:28.000000 pyhgf-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-19 20:14:39.436641 pyhgf-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-03-19 20:14:28.000000 pyhgf-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:14:39.436641 pyhgf-0.0.3/pyhgf/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/continuous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:14:39.436641 pyhgf-0.0.3/pyhgf/data/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/data/binary_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/data/usdchf.dat
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-19 20:14:28.000000 pyhgf-0.0.3/pyhgf/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:14:39.436641 pyhgf-0.0.3/pyhgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-19 20:14:39.000000 pyhgf-0.0.3/pyhgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-19 20:14:39.000000 pyhgf-0.0.3/pyhgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 20:14:39.000000 pyhgf-0.0.3/pyhgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-19 20:14:39.000000 pyhgf-0.0.3/pyhgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 20:14:39.000000 pyhgf-0.0.3/pyhgf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 20:14:39.440641 pyhgf-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-19 20:14:28.000000 pyhgf-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 20:14:39.436641 pyhgf-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-19 20:14:28.000000 pyhgf-0.0.3/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.313437 pyhgf-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-04-18 16:32:14.000000 pyhgf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 16:32:14.000000 pyhgf-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-18 16:32:25.313437 pyhgf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-18 16:32:14.000000 pyhgf-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/continuous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/data/binary_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/data/usdchf.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-18 16:32:14.000000 pyhgf-0.0.4/pyhgf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/pyhgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 16:32:25.000000 pyhgf-0.0.4/pyhgf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:32:25.313437 pyhgf-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-18 16:32:14.000000 pyhgf-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:32:25.309437 pyhgf-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-18 16:32:14.000000 pyhgf-0.0.4/tests/test_structure.py
```

### Comparing `pyhgf-0.0.3/LICENSE` & `pyhgf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/PKG-INFO` & `pyhgf-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.3
+Version: 0.0.4
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
```

### Comparing `pyhgf-0.0.3/README.md` & `pyhgf-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf/__init__.py` & `pyhgf-0.0.4/pyhgf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Author: Nicolas Legrand <nicolas.legrand@cas.au.dk>
 
 import pkg_resources  # type: ignore
 from numpy import loadtxt
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def load_data(dataset: str):
     """Load dataset for continuous or binary HGF.
 
     Parameters
     ----------
```

### Comparing `pyhgf-0.0.3/pyhgf/binary.py` & `pyhgf-0.0.4/pyhgf/binary.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf/continuous.py` & `pyhgf-0.0.4/pyhgf/continuous.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,77 +293,14 @@
         # update input node's parameters
         parameters_structure[value_parents_idx[0]]["pihat"] = pihat_va_pa
         parameters_structure[value_parents_idx[0]]["pi"] = pi_va_pa
         parameters_structure[value_parents_idx[0]]["muhat"] = muhat_va_pa
         parameters_structure[value_parents_idx[0]]["mu"] = mu_va_pa
         parameters_structure[value_parents_idx[0]]["nu"] = nu_va_pa
 
-    #############################
-    # Update volatility parents #
-    #############################
-    if volatility_parents_idx is not None:
-        # unpack the current parent's parameters with value and volatility parents
-        vo_pa_node_parameters = parameters_structure[volatility_parents_idx[0]]
-        vo_pa_value_parents_idx = node_structure[
-            volatility_parents_idx[0]
-        ].value_parents
-        vo_pa_volatility_parents_idx = node_structure[
-            volatility_parents_idx[0]
-        ].volatility_parents
-
-        vope = (1 / pi_va_pa + (value - mu_va_pa) ** 2) * pihat - 1
-
-        # Compute new value for nu and pihat
-        logvol = vo_pa_node_parameters["omega"]
-
-        # Look at the (optional) vo_pa's volatility parents
-        # and update logvol accordingly
-        if vo_pa_volatility_parents_idx is not None:
-            for vo_pa_vo_pa in vo_pa_volatility_parents_idx:
-                kappa = vo_pa_vo_pa[0]["kappas"]
-                logvol += kappa * parameters_structure[vo_pa_vo_pa]["mu"]
-
-        # Estimate new_nu
-        nu = time_step * jnp.exp(logvol)
-        new_nu = jnp.where(nu > 1e-128, nu, jnp.nan)
-
-        pihat_vo_pa, nu_vo_pa = [
-            1 / (1 / vo_pa_node_parameters["pi"] + new_nu),
-            new_nu,
-        ]
-
-        pi_vo_pa = pihat_vo_pa + 0.5 * jnp.square(input_node_parameters["kappas"]) * (
-            1 + vope
-        )
-        pi_vo_pa = jnp.where(pi_vo_pa <= 0, jnp.nan, pi_vo_pa)
-
-        # Compute new muhat
-        driftrate = vo_pa_node_parameters["rho"]
-
-        # Look at the (optional) va_pa's value parents
-        # and update driftrate accordingly
-        if vo_pa_value_parents_idx is not None:
-            for vo_pa_va_pa, p in zip(
-                vo_pa_value_parents_idx, vo_pa_node_parameters["psis"]
-            ):
-                driftrate += p * parameters_structure[vo_pa_va_pa]["mu"]
-
-        muhat_vo_pa = vo_pa_node_parameters["mu"] + time_step * driftrate
-        mu_vo_pa = (
-            muhat_vo_pa
-            + jnp.multiply(0.5, input_node_parameters["kappas"]) / pi_vo_pa * vope
-        )
-
-        # Update this parent's parameters
-        parameters_structure[volatility_parents_idx[0]]["pihat"] = pihat_vo_pa
-        parameters_structure[volatility_parents_idx[0]]["pi"] = pi_vo_pa
-        parameters_structure[volatility_parents_idx[0]]["muhat"] = muhat_vo_pa
-        parameters_structure[volatility_parents_idx[0]]["mu"] = mu_vo_pa
-        parameters_structure[volatility_parents_idx[0]]["nu"] = nu_vo_pa
-
     # store value and timestep in the node's parameters
     parameters_structure[node_idx]["time_step"] = time_step
     parameters_structure[node_idx]["value"] = value
 
     return parameters_structure
```

### Comparing `pyhgf-0.0.3/pyhgf/data/usdchf.dat` & `pyhgf-0.0.4/pyhgf/data/usdchf.dat`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf/distribution.py` & `pyhgf-0.0.4/pyhgf/distribution.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf/model.py` & `pyhgf-0.0.4/pyhgf/model.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf/plots.py` & `pyhgf-0.0.4/pyhgf/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,19 +189,20 @@
                 label="Surprise",
             )
             surprise_ax.fill_between(
                 x=trajectories_df.time,
                 y1=trajectories_df[f"x_{i}_surprise"],
                 y2=trajectories_df[f"x_{i}_surprise"].min(),
                 color="#7f7f7f",
-                alpha=0.2,
+                alpha=0.1,
                 zorder=-1,
             )
+            sp = trajectories_df[f"x_{i}_surprise"].sum()
             surprise_ax.set_title(
-                f"Node {i} surprise: {trajectories_df[f'x_{i}_surprise'].sum()}",
+                f"Node {i} - Surprise: {sp:.2f}",
                 loc="left",
             )
             surprise_ax.set_ylabel("Surprise")
         axs[ax_i].legend()
         axs[ax_i].set_ylabel(rf"$\mu_{i}$")
 
     # global surprise
@@ -220,17 +221,16 @@
         trajectories_df.surprise,
         color="#2a2a2a",
         linewidth=0.5,
         linestyle="--",
         zorder=-1,
         label="Surprise",
     )
-    surprise_ax.set_title(
-        f"Total surprise: {trajectories_df.surprise.sum()}", loc="left"
-    )
+    sp = trajectories_df.surprise.sum()
+    surprise_ax.set_title(f"Total surprise: {sp:.2f}", loc="left")
     surprise_ax.set_ylabel("Surprise")
     surprise_ax.set_xlabel("Time")
 
     return axs
 
 
 def plot_correlations(hgf: "HGF") -> Axes:
@@ -325,26 +325,26 @@
     for i in range(len(hgf.node_structure)):
         # only if node is not an input node
         if i not in list_of_input_idx:
             graphviz_structure.node(f"x_{i}", label=str(i), shape="circle")
 
     # connect value parents
     for i, idx in enumerate(hgf.node_structure):
-        value_parents, _ = idx
+        value_parents = idx.value_parents
 
         if value_parents is not None:
             for value_parents_idx in value_parents:
                 graphviz_structure.edge(
                     f"x_{value_parents_idx}",
                     f"x_{i}",
                 )
 
     # connect volatility parents
     for i, idx in enumerate(hgf.node_structure):
-        _, volatility_parents = idx
+        volatility_parents = idx.volatility_parents
 
         if volatility_parents is not None:
             for volatility_parents_idx in volatility_parents:
                 graphviz_structure.edge(
                     f"x_{volatility_parents_idx}",
                     f"x_{i}",
                     color="gray",
```

### Comparing `pyhgf-0.0.3/pyhgf/structure.py` & `pyhgf-0.0.4/pyhgf/structure.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/pyhgf.egg-info/PKG-INFO` & `pyhgf-0.0.4/pyhgf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgf
-Version: 0.0.3
+Version: 0.0.4
 Summary: The generalized, nodalized HGF for predictive coding.
 Author: ILAB
 Author-email: nicolas.legrand@cas.au.dk
 Maintainer: Nicolas Legrand
 Maintainer-email: nicolas.legrand@cas.au.dk
 License: GPL-3.0
 Description-Content-Type: text/markdown
```

### Comparing `pyhgf-0.0.3/pyhgf.egg-info/SOURCES.txt` & `pyhgf-0.0.4/pyhgf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/setup.py` & `pyhgf-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/tests/test_binary.py` & `pyhgf-0.0.4/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/tests/test_continuous.py` & `pyhgf-0.0.4/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/tests/test_distribution.py` & `pyhgf-0.0.4/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/tests/test_model.py` & `pyhgf-0.0.4/tests/test_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import unittest
 from unittest import TestCase
 
 import jax.numpy as jnp
 
 from pyhgf import load_data
 from pyhgf.model import HGF
-
+from pyhgf.response import total_gaussian_surprise
 
 class Testmodel(TestCase):
     def test_HGF(self):
         """Test the model class"""
 
         ##############
         # Continuous #
@@ -47,14 +47,17 @@
             rho={"1": 0.0, "2": 0.0, "3": 0.0},
             kappas={"1": 1.0, "2": 1.0},
         )
         three_level_continuous_hgf.input_data(input_data=timeserie)
         surprise = three_level_continuous_hgf.surprise()
         assert jnp.isclose(surprise, -394.20514)
 
+        # test an alternative response function
+        sp = total_gaussian_surprise(three_level_continuous_hgf)
+        assert jnp.isclose(sp, 1646.3826)
 
         ##########
         # Binary #
         ##########
         timeseries = load_data("binary")
 
         # two-level
```

### Comparing `pyhgf-0.0.3/tests/test_plots.py` & `pyhgf-0.0.4/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `pyhgf-0.0.3/tests/test_structure.py` & `pyhgf-0.0.4/tests/test_structure.py`

 * *Files identical despite different names*

