# Comparing `tmp/psi-score-0.2.0.tar.gz` & `tmp/psi_score-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psi-score-0.2.0.tar", max compression
+gzip compressed data, was "psi_score-1.0.0.tar", max compression
```

## Comparing `psi-score-0.2.0.tar` & `psi_score-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      302 2022-07-19 12:37:09.230622 psi-score-0.2.0/AUTHORS.md
--rw-r--r--   0        0        0      336 2022-07-25 16:31:27.248843 psi-score-0.2.0/CHANGELOG.md
--rwxr-xr-x   0        0        0     2246 2022-07-13 14:20:43.125467 psi-score-0.2.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     1077 2022-07-13 11:45:59.813074 psi-score-0.2.0/LICENSE
--rw-r--r--   0        0        0     1721 2022-07-25 16:40:45.292583 psi-score-0.2.0/README.md
--rw-r--r--   0        0        0      138 2022-07-25 16:43:19.156055 psi-score-0.2.0/psi_score/__init__.py
--rw-r--r--   0        0        0        0 2022-07-25 13:17:23.551303 psi-score-0.2.0/psi_score/linalg/__init__.py
--rw-r--r--   0        0        0     7397 2022-07-25 16:30:23.232642 psi-score-0.2.0/psi_score/linalg/psi_solvers.py
--rw-r--r--   0        0        0      806 2022-07-25 15:49:37.377222 psi-score-0.2.0/psi_score/linalg/push.py
--rw-r--r--   0        0        0     4712 2022-07-25 16:25:29.670749 psi-score-0.2.0/psi_score/psi_score.py
--rw-r--r--   0        0        0      567 2022-07-12 14:23:17.105377 psi-score-0.2.0/psi_score/utils.py
--rw-r--r--   0        0        0      774 2022-07-25 16:45:45.210502 psi-score-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       32 2022-07-13 11:45:59.875074 psi-score-0.2.0/tests/test_psi_score.py
--rw-r--r--   0        0        0     2534 2022-07-25 16:48:36.165015 psi-score-0.2.0/setup.py
--rw-r--r--   0        0        0     2503 2022-07-25 16:48:36.165659 psi-score-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      302 2023-03-09 11:00:12.047019 psi_score-1.0.0/AUTHORS.md
+-rw-r--r--   0        0        0      499 2023-04-18 14:53:46.907492 psi_score-1.0.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2246 2023-03-09 11:00:12.047019 psi_score-1.0.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     1077 2023-03-09 11:00:12.047019 psi_score-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1823 2023-04-04 15:21:12.782459 psi_score-1.0.0/README.md
+-rw-r--r--   0        0        0      139 2023-04-18 14:46:24.567558 psi_score-1.0.0/psi_score/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 11:00:12.051019 psi_score-1.0.0/psi_score/linalg/__init__.py
+-rw-r--r--   0        0        0     8624 2023-04-18 14:29:14.302099 psi_score-1.0.0/psi_score/linalg/psi_solvers.py
+-rw-r--r--   0        0        0     1617 2023-03-16 10:35:51.527743 psi_score-1.0.0/psi_score/linalg/push.py
+-rw-r--r--   0        0        0     5595 2023-04-04 15:19:27.301992 psi_score-1.0.0/psi_score/psi_score.py
+-rw-r--r--   0        0        0      567 2023-03-09 11:00:12.051019 psi_score-1.0.0/psi_score/utils.py
+-rw-r--r--   0        0        0      774 2023-04-18 14:46:04.226962 psi_score-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-03-09 11:00:12.051019 psi_score-1.0.0/tests/test_psi_score.py
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 psi_score-1.0.0/PKG-INFO
```

### Comparing `psi-score-0.2.0/CONTRIBUTING.md` & `psi_score-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `psi-score-0.2.0/LICENSE` & `psi_score-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psi-score-0.2.0/README.md` & `psi_score-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -43,12 +43,13 @@
 
 `psi-score` was created by Nouamane Arhachoui. It is licensed under the terms of the MIT license.
 
 ## References
 
 * Giovanidis, A., Baynat, B., Magnien, C., & Vendeville, A. (2021).
   Ranking Online Social Users by Their Influence. 
-  IEEE/ACM Transactions on Networking, 29(5), 2198–2214. https://doi.org/10.1109/tnet.2021.3085201
+  IEEE/ACM Transactions on Networking, 29(5), 2198-2214. https://doi.org/10.1109/tnet.2021.3085201
 
 * Arhachoui, N., Bautista, E., Danisch, M., & Giovanidis, A. (2022). 
   A Fast Algorithm for Ranking Users by their Influence in Online Social Platforms. 
-  arXiv Preprint. https://doi.org/10.48550/ARXIV.2206.09960
+  2022 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM), 526-533. 
+  https://doi.org/10.1109/ASONAM55673.2022.10068673
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `psi-score-0.2.0/psi_score/linalg/psi_solvers.py` & `psi_score-1.0.0/psi_score/linalg/psi_solvers.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,71 +2,77 @@
 from scipy import sparse
 import numpy as np
 from scipy.sparse.linalg import norm
 from time import time
 from progressbar import progressbar
 from psi_score.utils import l_plus_m, dict_to_sparse_matrix, X
 
-from psi_score.linalg.push import push_nf_fifo
+from psi_score.linalg.push import push_nf_fifo, push_fifo
 
 def propagation_matrix(adjacency, ls, ms, lpms, solver):
     N = len(adjacency)
     A = dict()
-    if solver == 'push':
+    if solver == 'push_nf':
         A_t = {i: {} for i in adjacency}
         B_t = {i: {} for i in adjacency}
     else:
         B = {i: {} for i in range(N)}
         Deg = N*[0]
     c = []
     d = []
     for j in adjacency:
         A[j] = dict()
         for k in adjacency[j]:
             A[j][k] = ms[k] / lpms[j]
-            if solver == 'push':
+            if solver == 'push_nf':
                 if ms[k] != 0:
                     A_t[k][j] = ms[k] / lpms[j]
                 if ls[k] != 0:
                     B_t[k][j] = ls[k] / lpms[j]
             else:
                 B[j][k] = ls[k] / lpms[j]
                 Deg[j] += 1
         if ls[j]+ms[j] == 0:
             c.append(0)
             d.append(0)
         else:
             c.append(ms[j]/(ls[j]+ms[j]))
             d.append(ls[j]/(ls[j]+ms[j]))
 
+    if solver == 'push_psi':
+        # A_t = dict_to_sparse_matrix(A_t, shape=(N, N))
+        return A, B, c, d
+
     A = dict_to_sparse_matrix(A, shape=(N, N))
-    if solver == 'push':
+    if solver == 'push_nf':
         return A_t, B_t, c, d, A
     else:
         B = dict_to_sparse_matrix(B, shape=(N, N))
         c = np.array(c)
         d = np.array(d)
         Deg = np.array(Deg)
         return A, B, c, d, Deg
 
-def power_newsfeed(A, b_i, Deg, n_iter=500, tol=1e-4):
+def power_newsfeed(A, b_i, Deg, max_iter=500, tol=1e-4):
     p_i = b_i.copy()
     n_mult = 0
     n_msg = 0
-    for _ in range(n_iter):
+    n_iter = 0
+    for _ in range(max_iter):
         p_i_old = p_i.copy()
         nnz_idx = np.where(p_i != 0)[0]
         n_msg += Deg[nnz_idx].sum()     
         p_i = A.dot(p_i) + b_i
         n_mult += 1
         gap = np.sum(abs(p_i - p_i_old))
         # gap = norm(p_i - p_i_old, ord=1)
+        n_iter += 1
         if gap < tol:
-            return p_i, n_msg, n_mult
-    raise RuntimeError(f'Power-NF error: failed to converge in {n_iter} iterations.')
+            return p_i, n_msg, n_mult, n_iter
+    raise RuntimeError(f'Power-NF error: failed to converge in {max_iter} iterations.')
 
 def wall_steady_state(i, c, p_i, d):
     if isinstance(p_i, dict):
         q_i = dict()
         for j in p_i:
             q_i[j] = c[j] * p_i[j]
             if j == i:
@@ -77,15 +83,15 @@
         N = len(d)
         d_i = d[i]*X(i, N)
         q_i = c * p_i + d_i
     return q_i
 
 def get_psi_score(
         adjacency: dict[list], ls: Union[list, np.ndarray], 
-        ms: Union[list, np.ndarray], n_iter: int =500, 
+        ms: Union[list, np.ndarray], max_iter: int =500, 
         tol: float =1e-4, solver: str ='power_psi',
         ps: list[int] =[], qs: list[int] =[] 
     ) -> tuple:
     """ Solves the Psi-score problem with a chosen algorithm.
 
     Parameters
     ----------
@@ -95,17 +101,18 @@
         Posting activity of each node.
     ms: Union[list, np.ndarray]
         Re-posting activity of each node.
     solver: str
         * ``'power_psi'``, power iterations for the Psi_score vector.
         * ``'power_nf'``, for each ``i`` it uses power iterations for the vector ``p_i``, the expected probabilities to find a post of origin ``i`` on other users' NewsFeeds.
         * ``'scipy'``, use the linear system solver from the scipy.sparse library.
-        * ``'push'``, use push-based method for each vector ``p_i``.
+        * ``'push_nf'``, use push-based method for each vector ``p_i``.
+        * ``'push_psi'`` use push-based method for the Psi_score vector.
 
-    n_iter: int, optional
+    max_iter: int, optional
         Maximum number of iterations for Power-Psi and Power-NF, default=500
         
     tol: float, optional
         Tolerance for the convergence of the algorithms (except for scipy's solver), default=1e-4
     ps: list
         List of nodes ``i`` for which we want to have the ``p_i`` with the push and power_nf methods
     qs: list
@@ -117,101 +124,125 @@
         Psi-score vector
     t: float
         Computation time in seconds.
     n_msg: int or None
         Number of messages (or update in the Psi-score vector), ``None`` for the scipy solver.
     n_mult: int or None
         Number of matrix-vector multiplications to reach convergence, ``None`` for the scipy solver.
-    P: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push'``)
-        The ``p_i`` vectors of some chosen ``i`` obtained with the push or the power_nf method
-    Q: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push'``)
-        The ``q_i`` vectors of some chosen ``i`` obtained with the push or the power_nf method
+    n_iter: int or None
+        Number of iterations to reach convergence.
+    P: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push_nf'``)
+        The ``p_i`` vectors of some chosen ``i`` obtained with the push_nf or the power_nf method
+    Q: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push_nf'``)
+        The ``q_i`` vectors of some chosen ``i`` obtained with the push_nf or the power_nf method
     
     References
     ----------
     * Giovanidis, A., Baynat, B., Magnien, C., & Vendeville, A. (2021). 
-      Ranking Online Social Users by Their Influence. IEEE/ACM Transactions on Networking, 29(5), 2198–2214. 
+      Ranking Online Social Users by Their Influence. IEEE/ACM Transactions on Networking, 29(5), 2198-2214. 
       https://doi.org/10.1109/tnet.2021.3085201
     * Arhachoui, N., Bautista, E., Danisch, M., & Giovanidis, A. (2022). 
       A Fast Algorithm for Ranking Users by their Influence in Online Social Platforms. 
-      arXiv preprint. https://doi.org/10.48550/ARXIV.2206.09960
+      2022 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM), 526-533. 
+      https://doi.org/10.1109/ASONAM55673.2022.10068673
     """
 
     N = len(adjacency)
     lpms = l_plus_m(adjacency, ls, ms)
-    if solver == 'push':
-        A_t, B_t, c, d, A = propagation_matrix(adjacency, ls, ms, lpms, solver='push')
+    if solver == 'push_nf':
+        A_t, B_t, c, d, A = propagation_matrix(adjacency, ls, ms, lpms, solver='push_nf')
+    elif solver == 'push_psi':
+        A, B, c, d = propagation_matrix(adjacency, ls, ms, lpms, solver='push_psi')
     else:
         A, B, c, d, Deg = propagation_matrix(adjacency, ls, ms, lpms, solver)
     t = time()
     n_mult = 0
     n_msg = 0
+    n_iter = 0
 
     if solver == 'scipy':
-        P = sparse.linalg.spsolve((sparse.identity(N)-A).tocsc(), B.tocsc())
-        Psi = 1/N * (P.T.dot(c) + d)
+        s = sparse.linalg.spsolve((sparse.identity(N)-A.T).tocsc(), c)
+        Psi = 1/N * (B.T.dot(s) + d)
         t = time() - t
         return Psi, t
 
     elif solver == 'power_nf':
         t = time()
         Psi = []
         P = {}
         Q = {}
         for i in progressbar(range(N)):
             b_i = B.dot(X(i, N))
-            p_i, n_msg_i, n_mult_i = power_newsfeed(A, b_i, Deg, n_iter=n_iter, tol=tol)
+            p_i, n_msg_i, n_mult_i, n_iter_i = power_newsfeed(A, b_i, Deg, max_iter=max_iter, tol=tol)
             n_mult += n_mult_i
             n_msg += n_msg_i
+            n_iter += n_iter_i
             q_i = wall_steady_state(i, c, p_i, d)
             Psi.append(1/N * np.sum(q_i))
             if i in ps:
                 P[i] = p_i
             if i in qs:
                 Q[i] = q_i
         t = time() - t
-        return Psi, t, n_msg, n_mult, P, Q
+        return Psi, t, n_msg, n_mult, n_iter, P, Q
 
     elif solver == 'power_psi':
         At = A.T 
         s = c
         B_norm = norm(B, ord=1)
-        for i in progressbar(range(n_iter)):
+        for i in progressbar(range(max_iter)):
             s_old = s.copy()
             nnz_idx = np.where(s != 0)[0]
             n_msg += Deg[nnz_idx].sum()
             s = At.dot(s) + c
             n_mult += 1
             gap = sum(abs(s - s_old))
             gap = gap * B_norm
+            n_iter += 1
             if gap < tol:
                 Psi = 1/N * (B.T.dot(s) + d)
                 n_mult += 1
+                t = time() - t
+                return Psi, t, n_msg, n_mult, n_iter
         if gap >= tol:
-            raise RuntimeError(f'Power-Psi error: failed to converge in {n_iter} iterations.')
+            raise RuntimeError(f'Power-Psi error: failed to converge in {max_iter} iterations.')
 
-    elif solver == 'push':
+    elif solver == 'push_nf':
         Psi = []
         P = {}
         Q = {}
         tol = tol * (1 - np.max(A.sum(axis=1)))
         for i in progressbar(range(N)):
             if i in B_t:
-                p_i, n_msg_i = push_nf_fifo(i, A_t, B_t[i], eps=tol)
+                p_i, n_msg_i, n_iter_i = push_nf_fifo(i, A_t, B_t[i], eps=tol)
                 n_msg += n_msg_i
+                n_iter += n_iter_i
             else:
                 p_i = dict()
             q_i = wall_steady_state(i, c, p_i, d)
             Psi.append(1/N * sum(q_i.values()))
             if i in ps:
                 P[i] = p_i
             if i in qs:
                 Q[i] = q_i
         t = time() - t
         Psi = np.array(Psi)
-        return Psi, t, n_msg, P, Q
+        return Psi, t, n_msg, n_iter, P, Q
+    
+    elif solver == 'push_psi':
+        c = {i: c[i] for i in range(N) if c[i] != 0}
+        d = np.array(d)
+        B = dict_to_sparse_matrix(B, shape=(N, N))
+        A_t = dict_to_sparse_matrix(A, shape=(N, N))
+        tol = tol * (1 - np.max(A_t.sum(axis=1)))
+        s, n_msg, n_iter = push_fifo(A, c, eps=tol)
+        s = [s[i] if i in s else 0 for i in range(N)]
+        Psi = 1/N * (B.T.dot(s) + d)
+
+        t = time() - t
+
+        return Psi, t, n_msg, n_iter
+
     
     else:
         raise ValueError('Unknown solver.')
 
-    t = time() - t
-    return Psi, t, n_msg, n_mult
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `psi-score-0.2.0/psi_score/psi_score.py` & `psi_score-1.0.0/psi_score/psi_score.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
     Parameters
     ----------
     solver: str
         * ``'power_psi'``, power iterations for the Psi_score vector.
         * ``'power_nf'``, for each ``i`` it uses power iterations for the vector ``p_i``, the expected probabilities to find a post of origin ``i`` on other users' NewsFeeds.
         * ``'scipy'``, use the linear system solver from the scipy.sparse library.
-        * ``'push'``, use push-based method for each vector ``p_i``.
+        * ``'push_nf'``, use push-based method for each vector ``p_i``.
+        * ``'push_psi'`` use push-based method for the Psi_score vector.
 
-    n_iter: int, optional
+    max_iter: int, optional
         Maximum number of iterations for Power-Psi and Power-NF, default=500
 
     tol: float, optional
         Tolerance for the convergence of the algorithms (except for scipy's solver), default=1e-4
 
     Attributes
     ----------
@@ -27,18 +28,20 @@
         Psi-score of each node.
     t: float
         Computation time in seconds.
     n_msg: int or None
         Number of messages (or update in the Psi-score vector), ``None`` for the scipy solver.
     n_mult: int or None
         Number of matrix-vector multiplications to reach convergence, ``None`` for the scipy solver.
-    P: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push'``)
-        The ``p_i`` vectors of some chosen ``i`` obtained with the push or the power_nf method
-    Q: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push'``)
-        The ``q_i`` vectors of some chosen ``i`` obtained with the push or the power_nf method
+    n_iter: int or None
+        Number of iterations to reach convergence.
+    P: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push_nf'``)
+        The ``p_i`` vectors of some chosen ``i`` obtained with the push_nf or the power_nf method
+    Q: dict[np.ndarray] (with ``solver='power_nf'``) or dict[dict] (with ``solver='push_nf'``)
+        The ``q_i`` vectors of some chosen ``i`` obtained with the push_nf or the power_nf method
 
     Example
     -------
     >>> from psi_score import PsiScore
     >>> adjacency = {0: [1, 3], 1: [0, 2], 2: [0, 1, 3], 3: [0]}
     >>> lambdas = [0.23, 0.50, 0.86, 0.19]
     >>> mus = [0.42, 0.17, 0.10, 0.37]
@@ -48,27 +51,32 @@
     array([0.21158803, 0.35253745, 0.28798439, 0.14789014])
     >>> np.round(scores, 2)
     array([0.21, 0.35, 0.29, 0.15])
 
     References
     ----------
     * Giovanidis, A., Baynat, B., Magnien, C., & Vendeville, A. (2021). 
-      Ranking Online Social Users by Their Influence. IEEE/ACM Transactions on Networking, 29(5), 2198–2214. 
+      Ranking Online Social Users by Their Influence. IEEE/ACM Transactions on Networking, 29(5), 2198-2214. 
       https://doi.org/10.1109/tnet.2021.3085201
+    * Arhachoui, N., Bautista, E., Danisch, M., & Giovanidis, A. (2022). 
+      A Fast Algorithm for Ranking Users by their Influence in Online Social Platforms. 
+      2022 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM), 526-533. 
+      https://doi.org/10.1109/ASONAM55673.2022.10068673
     """
 
-    def __init__(self, solver: str = 'power_psi', n_iter: int = 500, tol: float = 1e-4):
+    def __init__(self, solver: str = 'power_psi', max_iter: int = 500, tol: float = 1e-4):
         super(PsiScore, self).__init__()
         self.solver = solver
-        self.n_iter = n_iter
+        self.max_iter = max_iter
         self.tol = tol
         self.scores = None
         self.time = None
         self.n_msg = None
         self.n_mult = None
+        self.n_iter = None
         self.P = None
         self.Q = None
 
     def fit(self, adjacency: dict[list], lambdas: Union[list, np.ndarray], mus: Union[list, np.ndarray],
             ps: list[int] =[], qs: list[int] =[]) -> 'PsiScore':
         """Fit algorithm.
         
@@ -77,26 +85,30 @@
         adjacency:
             Adjacency list of the graph where edges go from followers to leaders.
         lambdas:
             Posting activity of each node.
         mus:
             Re-posting activity of each node.
         ps: list
-            List of nodes ``i`` for which we want to have the ``p_i`` with the push and power_nf methods
+            List of nodes ``i`` for which we want to have the ``p_i`` with the push_nf and power_nf methods
         qs: list
-            List of nodes ``i`` for which we want to have the ``q_i`` with the push and power_nf methods
+            List of nodes ``i`` for which we want to have the ``q_i`` with the push_nf and power_nf methods
         """
         if self.solver == 'scipy':
-            self.scores, self.time = get_psi_score(adjacency, lambdas, mus, n_iter=self.n_iter, solver=self.solver, tol=self.tol)
-        elif self.solver == 'push':
-            self.scores, self.time, self.n_msg, self.P, self.Q = get_psi_score(adjacency, lambdas, mus, n_iter=self.n_iter, solver=self.solver, tol=self.tol, ps=ps, qs=qs)
+            self.scores, self.time = get_psi_score(adjacency, lambdas, mus, max_iter=self.max_iter, solver=self.solver, tol=self.tol)
+        elif self.solver == 'push_nf':
+            self.scores, self.time, self.n_msg, self.n_iter, self.P, self.Q = get_psi_score(adjacency, lambdas, mus, max_iter=self.max_iter, solver=self.solver, tol=self.tol, ps=ps, qs=qs)
         elif self.solver == 'power_nf':
-            self.scores, self.time, self.n_msg, self.n_mult, self.P, self.Q = get_psi_score(adjacency, lambdas, mus, n_iter=self.n_iter, solver=self.solver, tol=self.tol, ps=ps, qs=qs)
+            self.scores, self.time, self.n_msg, self.n_mult, self.n_iter, self.P, self.Q = get_psi_score(adjacency, lambdas, mus, max_iter=self.max_iter, solver=self.solver, tol=self.tol, ps=ps, qs=qs)
+        elif self.solver == 'power_psi':
+            self.scores, self.time, self.n_msg, self.n_mult, self.n_iter = get_psi_score(adjacency, lambdas, mus, max_iter=self.max_iter, solver=self.solver, tol=self.tol)
+        elif self.solver == 'push_psi':
+            self.scores, self.time, self.n_msg, self.n_iter = get_psi_score(adjacency, lambdas, mus, max_iter=self.max_iter, solver=self.solver, tol=self.tol)
         else:
-            self.scores, self.time, self.n_msg, self.n_mult = get_psi_score(adjacency, lambdas, mus, n_iter=self.n_iter, solver=self.solver, tol=self.tol)
+            raise ValueError('Unknown solver.')
         return self
 
     def fit_transform(self, *args, **kwargs) -> np.ndarray:
         """Fit algorithm and return the Psi-score vector.
 
         Parameters
         ----------
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `psi-score-0.2.0/psi_score/utils.py` & `psi_score-1.0.0/psi_score/utils.py`

 * *Files identical despite different names*

### Comparing `psi-score-0.2.0/pyproject.toml` & `psi_score-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psi-score"
-version = "0.2.0"
+version = "1.0.0"
 description = "Metric of user influence in Online Social Networks"
 authors = ["Nouamane Arhachoui <nouamane.arhachoui@lip6.fr>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/NouamaneA/psi-score"
 repository = "https://github.com/NouamaneA/psi-score"
 keywords = ["graph algorithms", "network science", "markov chain", "social networks", "pagerank"]
```

### Comparing `psi-score-0.2.0/PKG-INFO` & `psi_score-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: psi-score
-Version: 0.2.0
+Version: 1.0.0
 Summary: Metric of user influence in Online Social Networks
 Home-page: https://github.com/NouamaneA/psi-score
 License: MIT
 Keywords: graph algorithms,network science,markov chain,social networks,pagerank
 Author: Nouamane Arhachoui
 Author-email: nouamane.arhachoui@lip6.fr
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: progressbar2 (>=4.0.0,<5.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Project-URL: Repository, https://github.com/NouamaneA/psi-score
 Description-Content-Type: text/markdown
 
 # Psi-score
@@ -63,13 +63,14 @@
 
 `psi-score` was created by Nouamane Arhachoui. It is licensed under the terms of the MIT license.
 
 ## References
 
 * Giovanidis, A., Baynat, B., Magnien, C., & Vendeville, A. (2021).
   Ranking Online Social Users by Their Influence. 
-  IEEE/ACM Transactions on Networking, 29(5), 2198–2214. https://doi.org/10.1109/tnet.2021.3085201
+  IEEE/ACM Transactions on Networking, 29(5), 2198-2214. https://doi.org/10.1109/tnet.2021.3085201
 
 * Arhachoui, N., Bautista, E., Danisch, M., & Giovanidis, A. (2022). 
   A Fast Algorithm for Ranking Users by their Influence in Online Social Platforms. 
-  arXiv Preprint. https://doi.org/10.48550/ARXIV.2206.09960
+  2022 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM), 526-533. 
+  https://doi.org/10.1109/ASONAM55673.2022.10068673
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

