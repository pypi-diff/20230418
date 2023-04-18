# Comparing `tmp/symlib-1.2.8.tar.gz` & `tmp/symlib-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.2.8.tar", last modified: Mon Mar  6 21:06:12 2023, max compression
+gzip compressed data, was "symlib-1.2.9.tar", last modified: Tue Apr 18 17:25:41 2023, max compression
```

## Comparing `symlib-1.2.8.tar` & `symlib-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-03-06 21:06:12.245968 symlib-1.2.8/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.2.8/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-03-06 21:06:12.245845 symlib-1.2.8/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.2.8/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.2.8/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-03-06 21:06:12.246008 symlib-1.2.8/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-03-06 21:06:09.000000 symlib-1.2.8/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-03-06 21:06:12.244934 symlib-1.2.8/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1586 2023-02-07 17:29:32.000000 symlib-1.2.8/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.2.8/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    40269 2023-03-06 21:06:09.000000 symlib-1.2.8/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    35326 2023-01-27 23:41:55.000000 symlib-1.2.8/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8469 2022-09-02 12:56:37.000000 symlib-1.2.8/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-03-06 21:06:12.245694 symlib-1.2.8/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-03-06 21:06:12.000000 symlib-1.2.8/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-03-06 21:06:12.000000 symlib-1.2.8/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-03-06 21:06:12.000000 symlib-1.2.8/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-03-06 21:06:12.000000 symlib-1.2.8/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-03-06 21:06:12.000000 symlib-1.2.8/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.753183 symlib-1.2.9/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.2.9/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-04-18 17:25:41.753067 symlib-1.2.9/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.2.9/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.2.9/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-18 17:25:41.753219 symlib-1.2.9/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-04-18 17:25:39.000000 symlib-1.2.9/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.752300 symlib-1.2.9/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.2.9/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.2.9/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    44206 2023-04-18 17:25:19.000000 symlib-1.2.9/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.2.9/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     8469 2022-09-02 12:56:37.000000 symlib-1.2.9/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.752878 symlib-1.2.9/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.2.8/LICENSE` & `symlib-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.2.8/PKG-INFO` & `symlib-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.2.8
+Version: 1.2.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.2.8/setup.py` & `symlib-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.2.8"
+version = "1.2.9"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.2.8/symlib/__init__.py` & `symlib-1.2.9/symlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Data types
-from .lib import SUBHALO_DTYPE, HISTORY_DTYPE, BRANCH_DTYPE, CORE_DTYPE, UM_DTYPE
+from .lib import SUBHALO_DTYPE, HISTORY_DTYPE, BRANCH_DTYPE, CORE_DTYPE, UM_DTYPE, PARTICLE_DTYPE
 # I/O function
 from .lib import read_subhalos, read_cores, read_branches, read_tree, read_particles, ParticleInfo
+from .lib import Particles
 # Utilities
 from .lib import simulation_parameters, parameter_table, scale_factors, pristine_merger_indices, merger_stats, propagate_parent_indices, colossus_parameters, suite_names, merger_lookup_table, find_merger_branch, find_all_merger_branches, is_real_confirmed, read_um
 # TODO: better names for pristine_merger_indices and propagate_parent_indices
 
 # Abstract models
 from .star_tagging import ProfileModel, RHalfModel, MStarModel, AbstractRanking
 # Profile models
```

### Comparing `symlib-1.2.8/symlib/file_management.py` & `symlib-1.2.9/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.2.8/symlib/lib.py` & `symlib-1.2.9/symlib/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,22 @@
       false otherwise
 """
 UM_DTYPE = [("m_star", "f4"), ("m_in_situ", "f4"), ("m_icl", "f4"),
             ("sfr", "f4"), ("x", "f4", (3,)), ("v", "f4", (3,)),
             ("rank", "f4"), ("mvir", "f4"), ("vmax", "f4"),
             ("is_orphan", "?"), ("ok", "?")]
 
+""" TODO
+"""
+PARTICLE_DTYPE = [
+    ("x", "f4", (3,)), ("v", "f4", (3,)),
+    ("snap", "i4"), ("id", "i4"),
+    ("ok", "?"), ("smooth", "?")
+]
+
 """ TREE_COL_NAMES is the mapping of variable names to columns in the
 consistent-trees file. These are the variable names you need to pass to
 read_tree().
 """
 TREE_COL_NAMES = {
     "dfid": 28,
     "id": 1,
@@ -707,15 +715,15 @@
 def tree_var_offset(hd, var_name):
     i = tree_var_col(hd, var_name)
     hd_size = 4*4 + 4*(hd.n_int + hd.n_float + hd.n_vec)
     return hd.n*4*(i + 2*max(0, i - hd.n_int - hd.n_float)) + hd_size    
 
 def merger_lookup_table(b, dfid):
     """ merger_lookup_table creates a look-up table for finding the branches of
-    mergers. It's used alongsize find_merger_branch and
+    mergers. It's used along side find_merger_branch and
     find_all_merger_branches.
 
     b is an array of branches (BRANCH_DTYPE) and dfid is an array of
     depth-first IDs with merger tree ordering (can be read by calling 
     read_tree on "dfid")
     """
     return dfid[b["start"]]
@@ -748,16 +756,24 @@
     n_merger = struct.unpack("i", f.read(4))[0]
 
     idx = np.fromfile(f, np.int32, n_merger)    
     
 class ParticleHeader(object):
     def __init__(self, base_dir):
         file_name = path.join(base_dir, "particles", "particle_header.dat")
-        f = open(file_name, "rb")
-        
+        ## BH: first attempt
+        #        if not file_name.is_file():
+        #           raise FileNotFoundError("The particle data for {} has not been generated.".format(file_name))
+        try:
+            f = open(file_name, "rb")
+        except FileNotFoundError as e:
+            # TODO: raise error here
+            print("The particle data for this halo does not exist.", e.args)
+        # TODO: if not working, try os.path.exists() and os.path.isfile() after that
+
         self.n_file = struct.unpack("i", f.read(4))[0]
         self.n_halo = struct.unpack("i", f.read(4))[0]
         self.n_particle = struct.unpack("i", f.read(4))[0]
         
         self.file_lengths = np.fromfile(f, np.int32, self.n_file)
         self.offsets = np.fromfile(f, np.int32, self.n_halo)
         self.sizes = np.fromfile(f, np.int32, self.n_halo)
@@ -839,14 +855,96 @@
             base_dir, include_false_selections=True)
 
 def is_real_confirmed(part_info, h, i_sub):
     first_snap = np.where(h[i_sub]["ok"])[0][0]
     ok = read_particles(part_info, None, first_snap, "valid", owner=i_sub)
     return np.sum(ok) > 0
 
+class Particles(object):
+    def __init__(self, sim_dir):
+        # TODO: write docstring
+        self.sim_dir = sim_dir
+        self.part_info = ParticleInfo(sim_dir)
+        self.params = simulation_parameters(sim_dir)
+        self.scale = scale_factors(sim_dir)
+        self.h_cmov, _ = read_subhalos(sim_dir, comoving=True)
+
+    def read(self, snap, halo=-1, mode="current", comoving=False):
+        # TODO: write docstring
+        """ mode_args: ["all", "current", "smooth"]
+        """
+
+        sim_dir = self.sim_dir
+        part_info = self.part_info
+        h0 = self.h_cmov[0,snap]
+        a = self.scale[snap]
+
+        # These modes need to read in all particles simultaneously: cannot
+        # just read one halo.
+        if mode == "all" or mode == "current":
+            idp = read_particles(part_info, sim_dir, snap, "id")
+            x = read_particles(part_info, sim_dir, snap, "x")
+            v = read_particles(part_info, sim_dir, snap, "v")
+            if not comoving:
+                for s in range(len(x)):
+                    x[s] = util.set_units_x(x[s], h0, a, self.params)
+                    v[s] = util.set_units_v(v[s], h0, a, self.params)
+            
+            snaps = read_particles(part_info, sim_dir, snap, "snap")
+            valid = read_particles(part_info, sim_dir, snap, "valid")
+            smooth = read_particles(part_info, sim_dir, snap, "ownership")
+            
+            # Remove invalid particles.
+            if mode == "current":
+                for i in range(len(x)):
+                    ok = valid[i]
+                    x[i], v[i], idp[i] = x[i][ok], v[i][ok], idp[i][ok]
+                    snaps[i], smooth[i] = snaps[i][ok], smooth[i][ok]
+                    valid[i] = valid[i][ok]
+
+        if mode == "smooth":
+            for sh in range(len(h)):
+                # A single halo read is fast for smooth particles, so we only
+                # have to read the specified halo in this mode
+                if halo != -1 and sh != halo: continue
+                idp = read_particles(part_info, sim_dir, snap, "id", owner=sh)
+                x = read_particles(part_info, sim_dir, snap, "x", owner=sh)
+                v = read_particles(part_info, sim_dir, snap, "v", owner=sh)
+                if not comoving:
+                    x[s] = util.set_units_x(x[s], h0, a, self.params)
+                    v[s] = util.set_units_v(v[s], h0, a, self.params)
+            
+                snaps = read_particles(part_info, sim_dir, snap,
+                                       "snap", owner=sh)
+                valid = read_particles(part_info, sim_dir, snap,
+                                       "valid", owner=sh)
+                smooth = read_particles(part_info, sim_dir, snap,
+                                        "ownership", owner=sh)
+
+
+        p = [None]*len(x)
+        for i in range(len(x)):
+            if halo == -1 or i == halo:
+                p[i] = np.zeros(len(x[i]), dtype=PARTICLE_DTYPE)
+                p[i]["id"] = idp[i]
+                p[i]["x"] = x[i]
+                p[i]["v"] = v[i]
+                p[i]["snap"] = snaps[i]
+                p[i]["ok"] = valid[i]
+                p[i]["smooth"] = smooth[i] == 0
+
+        if halo == -1:
+            return p 
+        else:
+            return p[halo]
+
+
+    def core_particles(self, snap, halo=-1, comoving=False):
+        pass
+
 def read_particles(part_info, base_dir, snap, var_name,
                    owner=None, include_false_selections=False):
     hd, tags = part_info.part_hd, part_info.tags
     
     h_idx = np.arange(len(part_info.hist_false), dtype=int)
     if include_false_selections:
         false_remapping = h_idx
```

### Comparing `symlib-1.2.8/symlib/star_tagging.py` & `symlib-1.2.9/symlib/star_tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
         return Ms
     
     def var_names(self):
         """ var_names returns the names of the variables this model requires.
         """
         return ["mpeak", "z"]
     
-
+    
 class RadialEnergyRanking(AbstractRanking):
     def __init__(self, params, x, v, idx, n_max,
                  core_particles=DEFAULT_CORE_PARTICLES,
                  quantile_edges=DEFAULT_QUANTILE_EDGES):
         """ Takes mp (Msun; may be a scalar), x (pkpc), v (pkm/s), idx (the
         index into the full particle array), and n_max (the number of particles
         in the full particle arrays).
```

### Comparing `symlib-1.2.8/symlib/util.py` & `symlib-1.2.9/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.2.8/symlib.egg-info/PKG-INFO` & `symlib-1.2.9/symlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.2.8
+Version: 1.2.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

