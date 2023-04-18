# Comparing `tmp/kolo-2.6.0.tar.gz` & `tmp/kolo-2.6.1.tar.gz`

## Comparing `kolo-2.6.0.tar` & `kolo-2.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.6.0/rust/Cargo.toml
--rw-r--r--   0     1001      123       54 2023-03-17 10:25:16.000000 kolo-2.6.0/rust/build.rs
--rw-r--r--   0     1001      123    35236 2023-03-17 10:25:16.000000 kolo-2.6.0/rust/src/lib.rs
--rw-r--r--   0     1001      123     2106 2023-03-17 10:25:16.000000 kolo-2.6.0/pyproject.toml
--rw-r--r--   0     1001      123    11199 2023-03-17 10:26:46.000000 kolo-2.6.0/rust/Cargo.lock
--rw-r--r--   0     1001      123     3556 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/db.py
--rw-r--r--   0     1001      123     6765 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/__main__.py
--rw-r--r--   0     1001      123     3681 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/serialize.py
--rw-r--r--   0     1001      123     2481 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/config.py
--rw-r--r--   0     1001      123      108 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/__init__.py
--rw-r--r--   0     1001      123     3210 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/generate_tests.py
--rw-r--r--   0     1001      123      228 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/pytest_plugin.py
--rw-r--r--   0     1001      123      141 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/pypy.py
--rw-r--r--   0     1001      123     1322 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/unittest.py
--rw-r--r--   0     1001      123     3161 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/requests.py
--rw-r--r--   0     1001      123     1778 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/logging.py
--rw-r--r--   0     1001      123     3157 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/urllib.py
--rw-r--r--   0     1001      123     4345 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/sql.py
--rw-r--r--   0     1001      123     4355 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/exception.py
--rw-r--r--   0     1001      123      348 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/kolo.py
--rw-r--r--   0     1001      123        0 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/__init__.py
--rw-r--r--   0     1001      123     1457 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/pytest.py
--rw-r--r--   0     1001      123     4055 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/django.py
--rw-r--r--   0     1001      123     5180 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/core.py
--rw-r--r--   0     1001      123     2921 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/huey.py
--rw-r--r--   0     1001      123     2262 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/celery.py
--rw-r--r--   0     1001      123     3707 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/urllib3.py
--rw-r--r--   0     1001      123      809 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/filters/attrs.py
--rw-r--r--   0     1001      123    13710 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/profiler.py
--rw-r--r--   0     1001      123      951 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/templates/django_request_test.py.j2
--rw-r--r--   0     1001      123      473 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/git.py
--rw-r--r--   0     1001      123      169 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/version.py
--rw-r--r--   0     1001      123     2640 2023-03-17 10:25:16.000000 kolo-2.6.0/src/kolo/middleware.py
--rw-r--r--   0     1001      123      228 2023-03-17 10:25:16.000000 kolo-2.6.0/README.md
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.6.1/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-04-18 10:49:25.000000 kolo-2.6.1/rust/build.rs
+-rw-rw-r--   0     1000     1001    35236 2023-04-18 10:49:25.000000 kolo-2.6.1/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2106 2023-04-18 10:49:25.000000 kolo-2.6.1/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-04-18 10:50:04.000000 kolo-2.6.1/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     3681 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3161 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4355 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4055 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001      951 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/version.py
+-rw-rw-r--   0     1000     1001     3210 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001     6765 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     3556 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-04-18 10:49:25.000000 kolo-2.6.1/README.md
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.6.1/PKG-INFO
```

### Comparing `kolo-2.6.0/rust/Cargo.toml` & `kolo-2.6.1/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/rust/src/lib.rs` & `kolo-2.6.1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/pyproject.toml` & `kolo-2.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.6.0"
+version = "2.6.1"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
```

### Comparing `kolo-2.6.0/rust/Cargo.lock` & `kolo-2.6.1/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bstr"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ffdb39cb703212f3c11973452c2861b972f757b021158f3516ba10f2fa8b2c1"
+checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
 dependencies = [
  "memchr",
  "once_cell",
  "regex-automata",
  "serde",
 ]
 
@@ -42,34 +42,34 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -81,17 +81,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -147,75 +147,75 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
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
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -282,23 +282,23 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.156"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "314b5b092c0ade17c00142951e50ced110ec27cea304b1037c6969246c2469a4"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
```

### Comparing `kolo-2.6.0/src/kolo/db.py` & `kolo-2.6.1/src/kolo/db.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/__main__.py` & `kolo-2.6.1/src/kolo/__main__.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/serialize.py` & `kolo-2.6.1/src/kolo/serialize.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/config.py` & `kolo-2.6.1/src/kolo/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 import toolz
 from cerberus import Validator
 
 
 logger = logging.getLogger("kolo")
 
 
+class KoloWriteError(Exception):
+    pass
+
+
 schema = {
     "filters": {
         "type": "dict",
         "schema": {
             "include_frames": {"type": "list"},
             "ignore_frames": {"type": "list"},
             "ignore_request_paths": {"type": "list"},
@@ -60,20 +64,30 @@
 def create_kolo_directory() -> Path:
     """
     Create the kolo directory and contents if they do not exist
 
     Returns the path to the .kolo directory for convenience.
     """
     kolo_directory = (Path(os.environ.get("KOLO_PATH", ".")) / ".kolo").resolve()
-    kolo_directory.mkdir(parents=True, exist_ok=True)
-    with open(kolo_directory / ".gitignore", "w") as gitignore:
-        gitignore.write("db.sqlite3\n")
-        gitignore.write("db.sqlite3-shm\n")
-        gitignore.write("db.sqlite3-wal\n")
-        gitignore.write(".gitignore\n")
+    try:
+        kolo_directory.mkdir(parents=True, exist_ok=True)
+    except Exception as e:
+        message = f"Could not create .kolo directory at {kolo_directory}."
+        raise KoloWriteError(message) from e
+
+    gitignore_path = kolo_directory / ".gitignore"
+    try:
+        with open(gitignore_path, "w") as gitignore:
+            gitignore.write("db.sqlite3\n")
+            gitignore.write("db.sqlite3-shm\n")
+            gitignore.write("db.sqlite3-wal\n")
+            gitignore.write(".gitignore\n")
+    except Exception as e:
+        message = f"Could not write to {gitignore_path}."
+        raise KoloWriteError(message) from e
     return kolo_directory
 
 
 def merge_or_last(args):
     if all(isinstance(arg, dict) for arg in args):
         return toolz.merge(*args)
     return args[-1]
```

### Comparing `kolo-2.6.0/src/kolo/generate_tests.py` & `kolo-2.6.1/src/kolo/generate_tests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/unittest.py` & `kolo-2.6.1/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/requests.py` & `kolo-2.6.1/src/kolo/filters/requests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/logging.py` & `kolo-2.6.1/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/urllib.py` & `kolo-2.6.1/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/sql.py` & `kolo-2.6.1/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/exception.py` & `kolo-2.6.1/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/pytest.py` & `kolo-2.6.1/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/django.py` & `kolo-2.6.1/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/core.py` & `kolo-2.6.1/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/huey.py` & `kolo-2.6.1/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/celery.py` & `kolo-2.6.1/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/urllib3.py` & `kolo-2.6.1/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/filters/attrs.py` & `kolo-2.6.1/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/profiler.py` & `kolo-2.6.1/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/templates/django_request_test.py.j2` & `kolo-2.6.1/src/kolo/templates/django_request_test.py.j2`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/src/kolo/middleware.py` & `kolo-2.6.1/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.0/PKG-INFO` & `kolo-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.6.0
+Version: 2.6.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -35,17 +35,17 @@
 Requires-Dist: jinja2>=3.0.0; extra == 'test_generation'
 Provides-Extra: test_generation
 Summary: See everything happening in your running Django app
 Author-email: Wilhelm Klopp <team@kolo.app>, Lily Foote <lily@kolo.app>
 License: © Kolo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
 Project-URL: Repository, https://github.com/kolofordjango/kolo
 Project-URL: Homepage, https://kolo.app
-Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
 
 # Kolo
 
 See everything happening in your running Django app
 
 More information: https://kolo.app
```

