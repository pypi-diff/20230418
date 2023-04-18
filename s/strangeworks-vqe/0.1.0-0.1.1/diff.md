# Comparing `tmp/strangeworks_vqe-0.1.0.tar.gz` & `tmp/strangeworks_vqe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_vqe-0.1.0.tar", max compression
+gzip compressed data, was "strangeworks_vqe-0.1.1.tar", max compression
```

## Comparing `strangeworks_vqe-0.1.0.tar` & `strangeworks_vqe-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       19 2023-02-13 17:03:39.236689 strangeworks_vqe-0.1.0/README.md
--rw-r--r--   0        0        0      636 2023-02-13 17:03:51.732178 strangeworks_vqe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10213 2023-02-13 17:03:39.240683 strangeworks_vqe-0.1.0/strangeworks_vqe/sdk.py
--rw-r--r--   0        0        0      691 2023-02-13 17:03:39.240683 strangeworks_vqe-0.1.0/strangeworks_vqe/serializer.py
--rw-r--r--   0        0        0     5626 2023-02-13 17:03:39.240683 strangeworks_vqe-0.1.0/strangeworks_vqe/utils.py
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.0/setup.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/README.md
+-rw-r--r--   0        0        0      659 2023-04-18 10:47:24.411928 strangeworks_vqe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11197 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/sdk.py
+-rw-r--r--   0        0        0      691 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/serializer.py
+-rw-r--r--   0        0        0     5677 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/utils.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.1/PKG-INFO
```

### Comparing `strangeworks_vqe-0.1.0/pyproject.toml` & `strangeworks_vqe-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "strangeworks-vqe"
-version = "0.1.0"
+version = "0.1.1"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_vqe"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "0.4.0rc1" 
+strangeworks = "^0.4.0"
 tweedledum = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
 pre-commit = "^3.0.4"
 ipykernel = "^6.21.1"
+python-dotenv = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `strangeworks_vqe-0.1.0/strangeworks_vqe/sdk.py` & `strangeworks_vqe-0.1.1/strangeworks_vqe/sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
 from typing import Optional
 
 import strangeworks
+from strangeworks.core.errors.error import StrangeworksError
 
 import strangeworks_vqe.serializer as serializer
 import strangeworks_vqe.utils as utils
 
 
 class StrangeworksVQE:
     """Strangeworks client object."""
@@ -23,15 +24,15 @@
 
     def backends(self):
         """
         To-Do: Add cross check as to which backends the current user actually has access to.
                 Currently, this just lists all backends that could work with the qaoa service.
         """
 
-        all_backends = strangeworks.backends()
+        all_backends = strangeworks.backends(backend_type_slugs=["sw-vqe"])
 
         aws_backends = []
         aws_sim_backends = []
         ibmq_backends = []
         ibm_cloud_backends = []
         ibm_sim_backends = []
         for bb in range(len(all_backends)):
@@ -159,15 +160,15 @@
         try:
             optimizer = problem_params["optimizer"]
         except:
             x = None
         try:
             ansatz = problem_params["ansatz"]
         except:
-            x = None
+            None
 
         hyperparams = {
             "H": serializer.pickle_serializer(H, "json"),
             "Ham": serializer.pickle_serializer(Ham, "json"),
             "nqubits": str(nqubits),
             "maxiter": str(maxiter),
             "optimizer": optimizer,
@@ -204,49 +205,71 @@
 
         status = strangeworks.execute(
             self.rsc, {"payload": {"job_slug": job_slug}}, "status"
         )
 
         return status
 
-    def get_results(self, sw_job, calculate_exact_sol=False):
+    def get_results(self, sw_job, calculate_exact_sol=False, display_results=False):
         if type(sw_job) is dict:
             job_slug = sw_job.get("slug")
         else:
             job_slug = sw_job.slug
-        result = strangeworks.execute(
-            self.rsc, {"payload": {"job_slug": job_slug}}, "result"
-        )
 
-        status = strangeworks.execute(
-            self.rsc, {"payload": {"job_slug": job_slug}}, "status"
+        result_url = strangeworks.execute(
+            self.rsc, {"payload": {"job_slug": job_slug}}, "get_results_url"
         )
 
-        result = serializer.pickle_deserializer(result, "json")
+        if result_url:
+            result_file = strangeworks.download_job_files([result_url])[0]
+        else:
+            result = strangeworks.execute(
+                self.rsc, {"payload": {"job_slug": job_slug}}, "result"
+            )
+
+            result = serializer.pickle_deserializer(result, "json")
 
-        if calculate_exact_sol is True and status == "COMPLETED":
-            inputs = strangeworks.execute(
-                self.rsc, {"payload": {"job_slug": job_slug}}, "get_inputs"
+            if result.strip().upper() == "COMPLETED":
+                result_url = strangeworks.execute(
+                    self.rsc, {"payload": {"job_slug": job_slug}}, "get_results_url"
+                )
+                if result_url:
+                    result_file = strangeworks.download_job_files([result_url])[0]
+                else:
+                    raise StrangeworksError(f"unable to open {result_url}")
+            else:
+                return result
+
+        if calculate_exact_sol:
+            inputs_url = strangeworks.execute(
+                self.rsc, {"payload": {"job_slug": job_slug}}, "get_inputs_url"
             )
-            inputs = serializer.pickle_deserializer(inputs, "json")
+            inputs = strangeworks.download_job_files([inputs_url])[0]
 
             try:
                 H = serializer.pickle_deserializer(inputs["H"], "json")
-            except:
+            except Exception:
                 H = serializer.pickle_deserializer(inputs["hyperparams"]["H"], "json")
 
             try:
                 En_exact = utils.get_exact_en(H, H.num_qubits)
-            except:
+            except Exception:
                 En_exact = "!!problem too big for exact solution!!"
-            result["En_exact"] = En_exact
-        elif status == "COMPLETED":
-            result["En_exact"] = None
+            result_file["En_exact"] = En_exact
+        else:
+            result_file["En_exact"] = None
+
+        if display_results:
+            En_exact = result_file["En_exact"]
+            En_sol = result_file["en_sol"]
+
+            print(f"The energy of the solution found by the algorithm is {En_sol}")
+            print(f"The exact optimal energy is {En_exact}")
 
-        return result
+        return result_file
 
     def job_list(self, update_status=True):
         job_list = strangeworks.jobs()
 
         qaoa_job_list = []
         for jj in range(len(job_list)):
             if job_list[jj].resource.product.slug == "vqe":
@@ -258,15 +281,15 @@
                 if job_list[jj].status != "COMPLETED" and update_status is True:
                     try:
                         status = strangeworks.execute(
                             self.rsc,
                             {"payload": {"job_slug": job_list[jj].slug}},
                             "status",
                         )
-                    except:
+                    except Exception:
                         status = job_list[jj].status
                 else:
                     status = job_list[jj].status
 
                 temp = {
                     "slug": job_list[jj].slug,
                     "Status": status,
```

### Comparing `strangeworks_vqe-0.1.0/strangeworks_vqe/serializer.py` & `strangeworks_vqe-0.1.1/strangeworks_vqe/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_vqe-0.1.0/strangeworks_vqe/utils.py` & `strangeworks_vqe-0.1.1/strangeworks_vqe/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def get_Ham_from_graph(G):
     Ham = []
     for nn in list(G.nodes()):
         try:
             G.nodes[nn]["weight"]
-        except:
+        except NameError:
             # if not specified, node weights will be considered zero
             G.nodes[nn]["weight"] = 0
 
         if G.nodes[nn]["weight"] != 0:
             if nn == 0:
                 temp = "Z"
             else:
@@ -67,15 +67,15 @@
                 temp = temp + "I"
 
             Ham.append((G.nodes[nn]["weight"], temp, nn))
 
     for pair in list(G.edges()):
         try:
             G.edges[pair]["weight"]
-        except:
+        except NameError:
             # if not specified, edge weight will be set equal to 1.0
             G.edges[pair]["weight"] = 1.0
 
         if pair[0] == 0:
             temp = "Z"
         else:
             temp = "I"
@@ -101,17 +101,17 @@
 
 def get_Ham_from_PauliSumOp(H_pauliSum):
     Ham = []
     for nn in range(len(H_pauliSum._primitive)):
         op_str = str(H_pauliSum._primitive[nn]._pauli_list[0])
 
         pair = []
-        for l in range(len(op_str)):
-            if op_str[l] == "Z":
-                pair.append(l)
+        for ll in range(len(op_str)):
+            if op_str[ll] == "Z":
+                pair.append(ll)
 
         if len(pair) > 1:
             pair = tuple(pair)
         else:
             pair = pair[0]
 
         Ham.append((np.real(H_pauliSum._primitive[nn]._coeffs[0]), op_str, pair))
@@ -170,29 +170,30 @@
 
 
 def convert_QUBO_to_Ising(QUBO_mat):
     nodes = np.size(QUBO_mat[0])
     Ising_mat = QUBO_mat / 4
 
     for nn in range(nodes):
-        Ising_mat[nn][nn] = QUBO_mat[nn][nn] / 2 + sum(QUBO_mat[nn][nn + 1 :] / 4)
+        Ising_mat[nn][nn] = QUBO_mat[nn][nn] / 2 + sum(QUBO_mat[nn][nn + 1:] / 4)
 
     for nn in range(nodes):
         Ising_mat[nn][nn] += sum(QUBO_mat[:nn, nn] / 4)
 
     return Ising_mat
 
 
 def get_graph_from_Ham(H):
     G = nx.Graph()
     for nn in range(len(H)):
         Num_z = H[nn][1].count("Z")
         if Num_z > 2:
             print(
-                "Error: cannot create networkX graph. Hamiltonian has more than pairwise connections"
+                """Error: cannot create networkX graph.
+                Hamiltonian has more than pairwise connections"""
             )
         elif Num_z == 1:
             ind = H[nn][1].find("Z")
             G.add_nodes_from([(ind, {"weight": H[nn][0]})])
         else:
             G.add_edges_from([(H[nn][2][0], H[nn][2][1], {"weight": H[nn][0]})])
 
@@ -223,8 +224,8 @@
 
 def get_exact_en(H, nodes):
     if nodes > 24:
         Egs_exact = "!!problem too big for exact solution!!"
     else:
         Egs_exact = NumPyMinimumEigensolver().compute_minimum_eigenvalue(H).eigenvalue
 
-    return Egs_exact
+    return np.real(Egs_exact)
```

### Comparing `strangeworks_vqe-0.1.0/PKG-INFO` & `strangeworks_vqe-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: strangeworks-vqe
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: qiskit (>=0.41.0,<0.42.0)
-Requires-Dist: strangeworks (==0.4.0rc1)
+Requires-Dist: strangeworks (>=0.4.0,<0.5.0)
 Requires-Dist: tweedledum (>=1.1.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # strangeworks-vqe
```

