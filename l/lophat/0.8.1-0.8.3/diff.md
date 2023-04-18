# Comparing `tmp/lophat-0.8.1.tar.gz` & `tmp/lophat-0.8.3.tar.gz`

## Comparing `lophat-0.8.1.tar` & `lophat-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 lophat-0.8.1/Cargo.toml
--rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.8.1/.gitignore
--rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.8.1/LICENSE
--rw-r--r--   0     1000     1001     4203 2023-03-27 15:27:02.000000 lophat-0.8.1/README.md
--rw-r--r--   0     1000     1001     1154 2023-03-27 07:14:32.000000 lophat-0.8.1/example.py
--rw-r--r--   0     1000     1001     2249 2023-03-24 12:16:44.000000 lophat-0.8.1/lophat.pyi
--rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.8.1/pyproject.toml
--rw-r--r--   0     1000     1001     4028 2023-03-27 14:48:35.000000 lophat-0.8.1/src/anti_transpose.rs
--rw-r--r--   0     1000     1001     3745 2023-03-27 14:52:52.000000 lophat-0.8.1/src/column.rs
--rw-r--r--   0     1000     1001     5905 2023-03-31 10:49:18.000000 lophat-0.8.1/src/decomposition.rs
--rw-r--r--   0     1000     1001     1658 2023-04-11 08:28:55.000000 lophat-0.8.1/src/diagram.rs
--rw-r--r--   0     1000     1001     1360 2023-03-24 12:16:44.000000 lophat-0.8.1/src/indexing.rs
--rw-r--r--   0     1000     1001     4925 2023-04-11 08:28:55.000000 lophat-0.8.1/src/lib.rs
--rw-r--r--   0     1000     1001    11702 2023-04-11 08:28:55.000000 lophat-0.8.1/src/lock_free.rs
--rw-r--r--   0     1000     1001     3438 2023-04-11 08:28:55.000000 lophat-0.8.1/src/options.rs
--rw-r--r--   0     1000     1001     2416 2023-03-27 07:19:20.000000 lophat-0.8.1/timing_test.py
--rw-r--r--   0     1000     1001    19340 2023-04-11 08:28:55.000000 lophat-0.8.1/Cargo.lock
--rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 lophat-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 lophat-0.8.3/Cargo.toml
+-rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.8.3/.gitignore
+-rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.8.3/LICENSE
+-rw-r--r--   0     1000     1001     4365 2023-04-12 13:01:54.000000 lophat-0.8.3/README.md
+-rw-r--r--   0     1000     1001     1154 2023-03-27 07:14:32.000000 lophat-0.8.3/example.py
+-rw-r--r--   0     1000     1001     2249 2023-03-24 12:16:44.000000 lophat-0.8.3/lophat.pyi
+-rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.8.3/pyproject.toml
+-rw-r--r--   0     1000     1001     4020 2023-04-14 09:38:24.000000 lophat-0.8.3/src/anti_transpose.rs
+-rw-r--r--   0     1000     1001     6683 2023-04-14 10:16:52.000000 lophat-0.8.3/src/column.rs
+-rw-r--r--   0     1000     1001     5905 2023-03-31 10:49:18.000000 lophat-0.8.3/src/decomposition.rs
+-rw-r--r--   0     1000     1001     1342 2023-04-12 13:01:54.000000 lophat-0.8.3/src/diagram.rs
+-rw-r--r--   0     1000     1001     1360 2023-03-24 12:16:44.000000 lophat-0.8.3/src/indexing.rs
+-rw-r--r--   0     1000     1001     5018 2023-04-18 07:35:51.000000 lophat-0.8.3/src/lib.rs
+-rw-r--r--   0     1000     1001    11898 2023-04-18 07:39:38.000000 lophat-0.8.3/src/lock_free.rs
+-rw-r--r--   0     1000     1001    12379 2023-04-17 07:42:42.000000 lophat-0.8.3/src/locking.rs
+-rw-r--r--   0     1000     1001     2097 2023-04-12 13:01:54.000000 lophat-0.8.3/src/options.rs
+-rw-r--r--   0     1000     1001     2416 2023-04-18 07:14:49.000000 lophat-0.8.3/timing_test.py
+-rw-r--r--   0     1000     1001    19352 2023-04-18 09:32:34.000000 lophat-0.8.3/Cargo.lock
+-rw-r--r--   0        0        0     4892 1970-01-01 00:00:00.000000 lophat-0.8.3/PKG-INFO
```

### Comparing `lophat-0.8.1/Cargo.toml` & `lophat-0.8.3/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [package]
 name = "lophat"
-version = "0.8.1"
+version = "0.8.3"
 edition = "2021"
 license = "MIT"
 description = "Lockfree Persistent Homology Algorithm Toolbox"
 homepage = "https://github.com/tomchaplin/lophat"
 repository = "https://github.com/tomchaplin/lophat"
 readme = "README.md"
 exclude = ["scripts/**/*", "docs/**/*"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lophat"
 crate-type = ["lib", "cdylib"]
 
 [dependencies]
+bit-set = "0.5.3"
 crossbeam = "0.8.2"
 hashbrown = { version = "0.13.2", features = ["rayon"] }
-pinboard = "2.1.0"
+pinboard = "2.2.0"
 pyo3 = { version = "0.18.1", features = ["hashbrown", "extension-module"], optional=true }
 rayon = "1.7.0"
 
 [features]
 default = ["python", "local_thread_pool"]
 python = ["dep:pyo3"]
 local_thread_pool = []
```

### Comparing `lophat-0.8.1/.gitignore` & `lophat-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/LICENSE` & `lophat-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/README.md` & `lophat-0.8.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 <b>Lo</b>ckfree <b>P</b>ersistent <b>H</b>omology <b>A</b>lgorithm <b>T</b>oolbox
 
 [![crates.io](https://img.shields.io/crates/v/lophat)](https://crates.io/crates/lophat)
 [![PyPi](https://img.shields.io/pypi/v/lophat)](https://pypi.org/project/lophat/)
 [![docs.rs](https://img.shields.io/docsrs/lophat?label=Docs.rs)](https://docs.rs/lophat/latest/lophat/)
 [![Read the Docs](https://img.shields.io/readthedocs/lophat?label=Read%20The%20Docs)](https://lophat.readthedocs.io/en/latest/)
 
+Try in: [Your Browser](https://lophat.tomchaplin.xyz/) • [Google Colab](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing)
+
 </div>
 
 ## Overview
 
 LoPHAT is a Rust library implementing the lockfree algorithm for computing persistent homology (PH), introduced in [[1]](#1).
 Python bindings are provided via PyO3, with an interface familiar to those who have used PHAT [[2]](#2).
```

### Comparing `lophat-0.8.1/example.py` & `lophat-0.8.3/example.py`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/lophat.pyi` & `lophat-0.8.3/lophat.pyi`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/src/anti_transpose.rs` & `lophat-0.8.3/src/anti_transpose.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     let max_dim = matrix.iter().map(|col| col.dimension()).max().unwrap();
     let mut return_matrix: Vec<_> = matrix
         .iter()
         .rev()
         .map(|col| C::new_with_dimension(max_dim - col.dimension()))
         .collect();
     for (j, col) in matrix.iter().enumerate() {
-        for i in col.boundary().iter() {
+        for i in col.entries() {
             return_matrix[matrix_width - 1 - i].add_entry(matrix_width - 1 - j);
         }
     }
     return_matrix
 }
 
 #[cfg(test)]
```

### Comparing `lophat-0.8.1/src/decomposition.rs` & `lophat-0.8.3/src/decomposition.rs`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/src/diagram.rs` & `lophat-0.8.3/src/diagram.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 use hashbrown::HashSet;
 
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 
-#[cfg(feature = "python")]
-/// Stores the pairings from a matrix decomposition,
-/// as well as those columns which did not appear in a pairing.
-#[pyclass]
-#[derive(Default, Debug, Clone, PartialEq)]
-pub struct PersistenceDiagram {
-    #[pyo3(get)]
-    pub unpaired: HashSet<usize>,
-    #[pyo3(get)]
-    pub paired: HashSet<(usize, usize)>,
-}
-
-#[cfg(not(feature = "python"))]
 /// Stores the pairings from a matrix decomposition,
 /// as well as those columns which did not appear in a pairing.
+#[cfg_attr(feature = "python", pyclass(get_all, set_all))]
 #[derive(Default, Debug, Clone, PartialEq)]
 pub struct PersistenceDiagram {
     pub unpaired: HashSet<usize>,
     pub paired: HashSet<(usize, usize)>,
 }
 
 impl std::fmt::Display for PersistenceDiagram {
```

### Comparing `lophat-0.8.1/src/indexing.rs` & `lophat-0.8.3/src/indexing.rs`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/src/lib.rs` & `lophat-0.8.3/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 
 mod anti_transpose;
 mod column;
 mod decomposition;
 mod diagram;
 mod indexing;
 mod lock_free;
+mod locking;
 mod options;
 
-pub use crate::column::{Column, VecColumn};
+pub use crate::column::{BitSetColumn, Column, VecColumn};
 pub use crate::decomposition::{rv_decompose_serial, RVDecomposition};
 pub use crate::diagram::{DiagramReadOff, PersistenceDiagram};
 //pub use crate::indexing::{IndexMap, VecIndexMap};
 pub use crate::anti_transpose::*;
 pub use crate::lock_free::{rv_decompose_lock_free, LockFreeAlgorithm};
+pub use crate::locking::{rv_decompose_locking, LockingAlgorithm};
 pub use crate::options::LoPhatOptions;
 
 /// Decomposes the input matrix, choosing between the serial and parallel
 /// algorithms depending on `options.num_threads`.
 ///
 /// * `matrix` - iterator over columns of the matrix you wish to decompose.
 /// * `options` - additional options to control decompositon, see [`LoPhatOptions`].
```

### Comparing `lophat-0.8.1/src/lock_free.rs` & `lophat-0.8.3/src/lock_free.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use crate::DiagramReadOff;
 use crate::LoPhatOptions;
 use crate::PersistenceDiagram;
 use crate::RVDecomposition;
 
 use crossbeam::atomic::AtomicCell;
 use hashbrown::HashSet;
+use pinboard::GuardedRef;
 use pinboard::NonEmptyPinboard;
 use rayon::prelude::*;
 #[cfg(feature = "local_thread_pool")]
 use rayon::ThreadPoolBuilder;
 
 enum LoPhatThreadPool {
     #[cfg(not(feature = "local_thread_pool"))]
@@ -88,19 +89,19 @@
             max_dim,
         }
     }
 
     /// Return a column with index `l`, if one exists.
     /// If found, returns `(col_idx, col)`, where col is a tuple consisting of the corresponding column in R and V.
     /// If not maintaining V, second entry of tuple is `None`.
-    pub fn get_col_with_pivot(&self, l: usize) -> Option<(usize, (C, Option<C>))> {
+    pub fn get_col_with_pivot(&self, l: usize) -> Option<(usize, GuardedRef<(C, Option<C>)>)> {
         loop {
             let piv = self.pivots[l].load();
             if let Some(piv) = piv {
-                let cols = self.matrix[piv].read();
+                let cols = self.matrix[piv].get_ref();
                 if cols.0.pivot() != Some(l) {
                     // Got a column but it now has the wrong pivot; loop again.
                     continue;
                 };
                 // Get column with correct pivot, return to caller.
                 return Some((piv, cols));
             } else {
@@ -113,26 +114,27 @@
     /// Reduces the `j`th column of the matrix as far as possible.
     /// If a pivot is found to the right of `j` (e.g. redued by another thread)
     /// then will switch to reducing that column.
     /// It is safe to reduce all columns in parallel.
     pub fn reduce_column(&self, j: usize) {
         let mut working_j = j;
         'outer: loop {
-            //println!("{:?}", working_j);
+            // We make a copy of the column because we want to mutate our local copy
+            // without locking other threads from reading
             let mut curr_column = self.matrix[working_j].read();
             while let Some(l) = (&curr_column).0.pivot() {
                 let piv_with_column_opt = self.get_col_with_pivot(l);
                 if let Some((piv, piv_column)) = piv_with_column_opt {
                     // Lines 17-24
                     if piv < working_j {
                         curr_column.0.add_col(&piv_column.0);
                         // Only add V columns if we need to
                         if self.options.maintain_v {
                             let curr_v_col = curr_column.1.as_mut().unwrap();
-                            curr_v_col.add_col(&piv_column.1.unwrap());
+                            curr_v_col.add_col(piv_column.1.as_ref().unwrap());
                         }
                     } else if piv > working_j {
                         self.matrix[working_j].set(curr_column);
                         if self.pivots[l]
                             .compare_exchange(Some(piv), Some(working_j))
                             .is_ok()
                         {
@@ -161,50 +163,51 @@
                 return;
             }
         }
     }
 
     /// Uses the boundary built up in column `boudary_idx` to clear the column corresponding to its pivot
     pub fn clear_with_column(&self, boudary_idx: usize) {
-        let (boundary_r, _boundary_v) = self.matrix[boudary_idx].read();
+        let boundary = self.matrix[boudary_idx].get_ref();
+        let boundary_r = &boundary.0;
         let clearing_idx = boundary_r
             .pivot()
             .expect("Attempted to clear using cycle column");
-        let clearing_dimension = self.matrix[clearing_idx].read().0.dimension();
+        let clearing_dimension = self.matrix[clearing_idx].get_ref().0.dimension();
         // The cleared R column is empty
         let r_col = C::new_with_dimension(clearing_dimension);
         // The corresponding R column should be the R column of the boundary
         let v_col = self
             .options
             .maintain_v
-            .then_some(boundary_r.with_dimension(clearing_dimension));
+            .then_some(boundary_r.clone().with_dimension(clearing_dimension));
         self.matrix[clearing_idx].set((r_col, v_col));
     }
 
     /// Reduce all columns of given dimension in parallel, according to `options`.
     pub fn reduce_dimension(&self, dimension: usize) {
         // Reduce matrix for columns of that dimension
         self.thread_pool.install(|| {
             (0..self.matrix.len())
                 .into_par_iter()
                 .with_min_len(self.options.min_chunk_len)
-                .filter(|&j| self.matrix[j].read().0.dimension() == dimension)
+                .filter(|&j| self.matrix[j].get_ref().0.dimension() == dimension)
                 .for_each(|j| self.reduce_column(j));
         });
     }
 
     /// Clear all columns of given dimension in parallel
     pub fn clear_dimension(&self, dimension: usize) {
         // Reduce matrix for columns of that dimension
         self.thread_pool.install(|| {
             (0..self.matrix.len())
                 .into_par_iter()
                 .with_min_len(self.options.min_chunk_len)
-                .filter(|&j| self.matrix[j].read().0.dimension() == dimension)
-                .filter(|&j| self.matrix[j].read().0.is_boundary())
+                .filter(|&j| self.matrix[j].get_ref().0.dimension() == dimension)
+                .filter(|&j| self.matrix[j].get_ref().0.is_boundary())
                 .for_each(|j| self.clear_with_column(j));
         });
     }
 
     /// Reduce all columns in parallel, according to `options`.
     pub fn reduce(&self) {
         for dimension in (0..=self.max_dim).rev() {
@@ -219,15 +222,15 @@
 impl<'a, C: Column + 'static> DiagramReadOff for LockFreeAlgorithm<'a, C> {
     fn diagram(&self) -> crate::PersistenceDiagram {
         let paired: HashSet<(usize, usize)> = self
             .matrix
             .par_iter()
             .enumerate()
             .filter_map(|(idx, col)| {
-                let lowest_idx = col.read().0.pivot()?;
+                let lowest_idx = col.get_ref().0.pivot()?;
                 Some((lowest_idx, idx))
             })
             .collect();
         let mut unpaired: HashSet<usize> = (0..self.matrix.len()).collect();
         for (birth, death) in paired.iter() {
             unpaired.remove(birth);
             unpaired.remove(death);
```

### Comparing `lophat-0.8.1/src/options.rs` & `lophat-0.8.3/src/options.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,10 @@
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 
-#[cfg(feature = "python")]
-/// A simple struct for specifying options for R=DV decompositions
-///
-/// * `maintain_v` - if true, returns full R=DV decomposition,
-///   otherwise returns [`RVDecomposition`](crate::RVDecomposition) with field `v` set to `None`.
-/// * `n_threads` - number of threads to use in thread pool; ignored by serial algorithms.
-///   see [`num_threads`](rayon::ThreadPoolBuilder::num_threads) for more details.
-///   Only relevant for lockfree algorithm.
-/// * `column_height` - an optional hint to the height of the columns.
-///   If `None`, assumed to be `matrix.collect().len()`.
-///   All indices must lie in the range `0..column_height`.
-///   Only relevant for lockfree algorithm.
-/// * `min_chunk_len` - When splitting work, don't reduce chunks to smaller than this size.
-///   Only relevant for lockfree algorithm.
-/// * `clearing` - Whether to employ the clearing optimisation.
-///   Note, if input matrix is not square then can't use this optimisation since it assumes D*D = 0.
-///   Only relevant for lockfree algorithm.
-#[pyclass]
-#[derive(Clone)]
-pub struct LoPhatOptions {
-    #[pyo3(get, set)]
-    pub maintain_v: bool,
-    #[pyo3(get, set)]
-    pub num_threads: usize,
-    #[pyo3(get, set)]
-    pub column_height: Option<usize>,
-    #[pyo3(get, set)]
-    pub min_chunk_len: usize,
-    #[pyo3(get, set)]
-    pub clearing: bool,
-}
-
-#[cfg(not(feature = "python"))]
 /// A simple struct for specifying options for R=DV decompositions
 ///
 /// * `maintain_v` - if true, returns full R=DV decomposition,
 ///   otherwise returns [`RVDecomposition`](crate::RVDecomposition) with field `v` set to `None`.
 /// * `n_threads` - number of threads to use in thread pool; ignored by serial algorithms.
 ///   see [`num_threads`](rayon::ThreadPoolBuilder::num_threads) for more details.
 ///   Only relevant for lockfree algorithm.
@@ -46,14 +13,15 @@
 ///   All indices must lie in the range `0..column_height`.
 ///   Only relevant for lockfree algorithm.
 /// * `min_chunk_len` - When splitting work, don't reduce chunks to smaller than this size.
 ///   Only relevant for lockfree algorithm.
 /// * `clearing` - Whether to employ the clearing optimisation.
 ///   Note, if input matrix is not square then can't use this optimisation since it assumes D*D = 0.
 ///   Only relevant for lockfree algorithm.
+#[cfg_attr(feature = "python", pyclass(get_all, set_all))]
 #[derive(Clone)]
 pub struct LoPhatOptions {
     pub maintain_v: bool,
     pub num_threads: usize,
     pub column_height: Option<usize>,
     pub min_chunk_len: usize,
     pub clearing: bool,
```

### Comparing `lophat-0.8.1/timing_test.py` & `lophat-0.8.3/timing_test.py`

 * *Files identical despite different names*

### Comparing `lophat-0.8.1/Cargo.lock` & `lophat-0.8.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "lophat"
-version = "0.8.1"
+version = "0.8.3"
 dependencies = [
+ "bit-set",
  "crossbeam",
  "hashbrown",
  "pinboard",
  "proptest",
  "pyo3",
  "rayon",
 ]
@@ -324,17 +325,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "pinboard"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6502324eee9cd4cd7dc8f22b0ed7683185a09e9ddcc0ac3028e010e2721662a3"
+checksum = "1fd5f86cbd9a742b934e6d0917ab0005988c480807913b05f4357ebf4e2a739e"
 dependencies = [
  "crossbeam-epoch",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
```

### Comparing `lophat-0.8.1/PKG-INFO` & `lophat-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lophat
-Version: 0.8.1
+Version: 0.8.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Lockfree Persistent Homology Algorithm Toolbox
 Home-Page: https://github.com/tomchaplin/lophat
 License: MIT
@@ -19,14 +19,16 @@
 <b>Lo</b>ckfree <b>P</b>ersistent <b>H</b>omology <b>A</b>lgorithm <b>T</b>oolbox
 
 [![crates.io](https://img.shields.io/crates/v/lophat)](https://crates.io/crates/lophat)
 [![PyPi](https://img.shields.io/pypi/v/lophat)](https://pypi.org/project/lophat/)
 [![docs.rs](https://img.shields.io/docsrs/lophat?label=Docs.rs)](https://docs.rs/lophat/latest/lophat/)
 [![Read the Docs](https://img.shields.io/readthedocs/lophat?label=Read%20The%20Docs)](https://lophat.readthedocs.io/en/latest/)
 
+Try in: [Your Browser](https://lophat.tomchaplin.xyz/) • [Google Colab](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing)
+
 </div>
 
 ## Overview
 
 LoPHAT is a Rust library implementing the lockfree algorithm for computing persistent homology (PH), introduced in [[1]](#1).
 Python bindings are provided via PyO3, with an interface familiar to those who have used PHAT [[2]](#2).
```

