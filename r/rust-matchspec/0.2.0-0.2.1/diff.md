# Comparing `tmp/rust_matchspec-0.2.0.tar.gz` & `tmp/rust_matchspec-0.2.1.tar.gz`

## Comparing `rust_matchspec-0.2.0.tar` & `rust_matchspec-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 rust_matchspec-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2770 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/.github/workflows/maturin-build.yml
--rw-r--r--   0     1001      123      580 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/.github/workflows/rust.yml
--rw-r--r--   0     1001      123       60 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1522 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/LICENSE
--rw-r--r--   0     1001      123     4100 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/README.md
--rw-r--r--   0     1001      123     1592 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/benches/parsing.rs
--rw-r--r--   0     1001      123     2587 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/benches/test_python.py
--rw-r--r--   0     1001      123      104 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/environment.yml
--rw-r--r--   0     1001      123      453 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123       81 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/python/rust_matchspec/__init__.py
--rw-r--r--   0     1001      123      345 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/recipe/bld.bat
--rw-r--r--   0     1001      123      369 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/recipe/build.sh
--rw-r--r--   0     1001      123      508 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/recipe/meta.yaml
--rw-r--r--   0     1001      123      317 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/error.rs
--rw-r--r--   0     1001      123     3406 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/input_table.rs
--rw-r--r--   0     1001      123      179 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123    18548 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/matchspec.rs
--rw-r--r--   0     1001      123     4307 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/package_candidate.rs
--rw-r--r--   0     1001      123    19616 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/parsers.rs
--rw-r--r--   0     1001      123     2066 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/src/python.rs
--rw-r--r--   0     1001      123  3033732 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/test_data/linux_64-depends.txt
--rw-r--r--   0     1001      123 39921865 2023-04-07 03:55:09.000000 rust_matchspec-0.2.0/test_data/repodata-linux-64.json
--rw-r--r--   0     1001      123    20901 2023-04-07 03:56:21.000000 rust_matchspec-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 rust_matchspec-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 rust_matchspec-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     2770 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/.github/workflows/maturin-build.yml
+-rw-r--r--   0     1001      123      580 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123       60 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     1522 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     5727 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/README.md
+-rw-r--r--   0     1001      123     1592 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/benches/parsing.rs
+-rw-r--r--   0     1001      123     3226 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/benches/test_python.py
+-rw-r--r--   0     1001      123      104 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/environment.yml
+-rw-r--r--   0     1001      123      453 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123       81 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/python/rust_matchspec/__init__.py
+-rw-r--r--   0     1001      123      345 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/recipe/bld.bat
+-rw-r--r--   0     1001      123      369 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/recipe/build.sh
+-rw-r--r--   0     1001      123      508 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/recipe/meta.yaml
+-rw-r--r--   0     1001      123      489 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/error.rs
+-rw-r--r--   0     1001      123     3406 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/input_table.rs
+-rw-r--r--   0     1001      123      179 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123    18548 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/matchspec.rs
+-rw-r--r--   0     1001      123     4652 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/package_candidate.rs
+-rw-r--r--   0     1001      123    19616 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/parsers.rs
+-rw-r--r--   0     1001      123     4408 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/src/python.rs
+-rw-r--r--   0     1001      123  3033732 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/test_data/linux_64-depends.txt
+-rw-r--r--   0     1001      123 39921865 2023-04-18 18:26:21.000000 rust_matchspec-0.2.1/test_data/repodata-linux-64.json
+-rw-r--r--   0     1001      123    20911 2023-04-18 18:26:58.000000 rust_matchspec-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     6125 1970-01-01 00:00:00.000000 rust_matchspec-0.2.1/PKG-INFO
```

### Comparing `rust_matchspec-0.2.0/Cargo.toml` & `rust_matchspec-0.2.1/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [package]
 name = "matchspec"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 
 [lib]
 # This is the python target
 name = "rust_matchspec"
 crate-type = ["lib", "cdylib"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [dependencies]
 nom = "7"
 pyo3 = { version = "0.18", optional = true }
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 version-compare = "0.1"
+rayon = "1.7"
 
 [dev-dependencies]
 criterion = "0.3"
 
 [features]
 default = ["python"]
 python = ["pyo3/extension-module"]
```

### Comparing `rust_matchspec-0.2.0/.github/workflows/maturin-build.yml` & `rust_matchspec-0.2.1/.github/workflows/maturin-build.yml`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/.github/workflows/rust.yml` & `rust_matchspec-0.2.1/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/LICENSE` & `rust_matchspec-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/README.md` & `rust_matchspec-0.2.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -40,14 +40,46 @@
 | license      | str           |           |
 | md5          | str           |           |
 | sha256       | str           |           |
 | size         | u64           |           |
 | subdir       | str           |           |
 | timestamp    | u64           |           |
 
+## `parallel_filter_package_list()`
+
+Using all available cores will take a `list` of `dicts` and returns all the dicts inside that match a given matchspec. The `dicts` must have a `name` key with a `str` value, but all other fields are optional.
+
+**Note** Probably won't show any noticable speed improvements until your list of packages is in the millions.
+
+```python
+import rust_matchspec
+list = [{'name': 'tensorflow', 'version': '2.10.0'},
+	{'name': 'pytorch', 'version': '2.0.0'},
+	{'name': 'pytorch', 'version': '1.11.1'}]
+
+rust_matchspec.parallel_filter_package_list('pytorch>1.12', list) # returns [PackageCandidate(name=pytorch)]
+```
+
+## `parallel_filter_package_list_with_matchspec_list()`
+
+Using all available cores will take a `list` of `dicts` and a `list` of Matchspecs (as `str`) and returns all the dicts inside that match any given matchspec. The `dicts` must have a `name` key with a `str` value, but all other fields are optional. **May contain duplicates** since it runs all of the matchspecs against the package list in parallel and does not dedup the resulting matches.
+
+In my testing this has a very small overhead, but matching 4 matchspecs is approximately the same speed as matching a single matchspec with the other functions.
+
+```python
+import rust_matchspec
+package_list = [{'name': 'tensorflow', 'version': '2.10.0'},
+	{'name': 'pytorch', 'version': '2.0.0'},
+	{'name': 'pytorch', 'version': '1.11.1'}]
+
+matchspec_list = ['python>=3.9.1', 'pytorch>1.12']
+
+rust_matchspec.parallel_filter_package_list_with_matchspec_list(matchspec_list, package_list) # returns [PackageCandidate(name=pytorch)]
+```
+
 # Rust Library
 
 ## Example
 
 The way you instantiate a MatchSpec is by parsing a string into the type:
 
 ```rust
```

### Comparing `rust_matchspec-0.2.0/benches/parsing.rs` & `rust_matchspec-0.2.1/benches/parsing.rs`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/benches/test_python.py` & `rust_matchspec-0.2.1/benches/test_python.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,81 +4,97 @@
 import json
 
 test_data = Path('./test_data')
 depends_file = test_data / 'linux_64-depends.txt'
 repodata_file = test_data / 'repodata-linux-64.json'
 
 
-def bench_match_against_matchspec(list: [str]):
-    """ Takes the list of matchspecs and matches against python 3.9.1 """
-    for item in list:
-        rust_matchspec.match_against_matchspec(item, 'python', '3.9.1')
-
-
 def test_rust_matchspec_on_repodata_depends(benchmark):
     """
     Test the rust_matchspec.match_against_matchspec using the
     linux_64-depends.txt file.
     """
+    def bench_match_against_matchspec(list: [str]):
+        for item in list:
+            rust_matchspec.match_against_matchspec(item, 'python', '3.9.1')
+
     with open(depends_file) as f:
         depends = f.readlines()
 
     benchmark(bench_match_against_matchspec, list=depends)
 
 
-def bench_conda_against_repodata_depends(list: [str]):
-    """
-    Runs a list of matchspecs against a static package, this is a little
-    contrived, but it is meant to compare the instantiation and filtering speed
-    of MatchSpec
-    """
-    for item in list:
-        ms = MatchSpec(item)
-        ms.match({'name': 'python', 'version': '3.9.1',
-                 'build': 'hbdb9e5c_0', 'build_number': 0})
-
-
 def test_conda_matchspec_on_repodata_depends(benchmark):
     """
     Test Conda's MatchSpec against the linux_64-depends.txt file
     """
+    def bench_conda_against_repodata_depends(list: [str]):
+        for item in list:
+            ms = MatchSpec(item)
+            ms.match({'name': 'python', 'version': '3.9.1',
+                     'build': 'hbdb9e5c_0', 'build_number': 0})
+
     with open(depends_file) as f:
         depends = f.readlines()
 
     benchmark(bench_conda_against_repodata_depends, list=depends)
 
 
-def bench_rust_matchspec_filter_package_list(list: [dict[str, str]]):
+def test_rust_matchspec_filter_package_list(benchmark):
     """
-    Runs rust_matchspec.filter_package_list() against a list of packages
+    Test rust_matchspec's filter_package_list() against the full linux-64
+    repodata.json from Anaconda's defaults.
     """
-    _matches = rust_matchspec.filter_package_list('python>=3.9.1', list)
+    def bench_rust_matchspec_filter_package_list(list: [dict[str, str]]):
+        _matches = rust_matchspec.filter_package_list('python>=3.9.1', list)
 
+    with open(repodata_file) as f:
+        repodata = list(json.load(f)['packages'].values())
 
-def test_rust_matchspec_filter_package_list(benchmark):
+    benchmark(bench_rust_matchspec_filter_package_list, list=repodata)
+
+
+def test_rust_matchspec_parallel_filter_package_list(benchmark):
     """
     Test rust_matchspec's filter_package_list() against the full linux-64
     repodata.json from Anaconda's defaults.
     """
+    def bench(list: [dict[str, str]]):
+        _matches = rust_matchspec.parallel_filter_package_list(
+            'python>=3.9.1', list)
+
     with open(repodata_file) as f:
         repodata = list(json.load(f)['packages'].values())
 
-    benchmark(bench_rust_matchspec_filter_package_list, list=repodata)
+    benchmark(bench, list=repodata)
 
 
-def bench_conda_filter_package_list(list: [dict[str, str]]):
+def test_rust_matchspec_parallel_filter_package_list_with_matchspec_list(benchmark):
     """
-    Runs uses MatchSpec against a list of packages to filter out non-matches
+    Test rust_matchspec's filter_package_list() against the full linux-64
+    repodata.json from Anaconda's defaults.
     """
-    ms = MatchSpec('python>=3.9.1')
-    _matches = [p for p in list if ms.match(p)]
+    def bench(list: [dict[str, str]]):
+        ms = ['python>=3.9.1', 'openssl>1', 'tensorflow<2.0', 'pip']
+        _m = rust_matchspec.parallel_filter_package_list_with_matchspec_list(
+            ms, list)
+
+    with open(repodata_file) as f:
+        repodata = list(json.load(f)['packages'].values())
+
+    benchmark(bench, list=repodata)
 
 
 def test_conda_filter_package_list(benchmark):
     """
     Benchmark conda MatchSpec filtering all of the linux-64 repodata from
     Anaconda's defaults
     """
+
+    def bench_conda_filter_package_list(list: [dict[str, str]]):
+        ms = MatchSpec('python>=3.9.1')
+        _matches = [p for p in list if ms.match(p)]
+
     with open(repodata_file) as f:
         repodata = list(json.load(f)['packages'].values())
 
     benchmark(bench_conda_filter_package_list, list=repodata)
```

### Comparing `rust_matchspec-0.2.0/src/input_table.rs` & `rust_matchspec-0.2.1/src/input_table.rs`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/src/matchspec.rs` & `rust_matchspec-0.2.1/src/matchspec.rs`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/src/package_candidate.rs` & `rust_matchspec-0.2.1/src/package_candidate.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     pub md5: Option<String>,
     pub sha256: Option<String>,
     pub size: Option<u64>,
     pub subdir: Option<String>,
     pub timestamp: Option<u64>,
 }
 
+// These are safe to assume because Option, String, and u64 are all Send/Sync
+unsafe impl Send for PackageCandidate {}
+unsafe impl Sync for PackageCandidate {}
+
 impl From<&str> for PackageCandidate {
     fn from(s: &str) -> Self {
         let package_candidate: PackageCandidate = serde_json::from_str(s).unwrap();
         package_candidate
     }
 }
 
@@ -108,14 +112,21 @@
             timestamp: dict
                 .get_item("build_number")
                 .and_then(|i| PyAny::extract(i).ok()),
         })
     }
 }
 
+impl TryFrom<&PyDict> for PackageCandidate {
+    type Error = PyErr;
+    fn try_from(value: &PyDict) -> Result<Self, Self::Error> {
+        PackageCandidate::from_dict(value)
+    }
+}
+
 #[cfg(test)]
 mod test {
     #[cfg(test)]
     mod package_candidate {
         use crate::package_candidate::*;
 
         #[test]
```

### Comparing `rust_matchspec-0.2.0/src/parsers.rs` & `rust_matchspec-0.2.1/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/test_data/linux_64-depends.txt` & `rust_matchspec-0.2.1/test_data/linux_64-depends.txt`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/test_data/repodata-linux-64.json` & `rust_matchspec-0.2.1/test_data/repodata-linux-64.json`

 * *Files identical despite different names*

### Comparing `rust_matchspec-0.2.0/Cargo.lock` & `rust_matchspec-0.2.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -243,19 +243,20 @@
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "matchspec"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "criterion",
  "nom",
  "pyo3",
+ "rayon",
  "serde",
  "serde_json",
  "version-compare",
 ]
 
 [[package]]
 name = "memchr"
@@ -377,66 +378,66 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -513,17 +514,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -532,28 +533,28 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -571,17 +572,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

