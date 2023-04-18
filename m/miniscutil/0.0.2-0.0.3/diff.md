# Comparing `tmp/miniscutil-0.0.2.tar.gz` & `tmp/miniscutil-0.0.3.tar.gz`

## Comparing `miniscutil-0.0.2.tar` & `miniscutil-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/__about__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/misc.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/type_util.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_humansize.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.0.2/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 miniscutil-0.0.2/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 miniscutil-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/misc.py
+-rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/type_util.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_humansize.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 miniscutil-0.0.3/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 miniscutil-0.0.3/PKG-INFO
```

### Comparing `miniscutil-0.0.2/miniscutil/__init__.py` & `miniscutil-0.0.3/miniscutil/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     map_keys,
     map_values,
     partition,
     append_url_params,
 )
 from .adapt import adapt, restore, register_adapter
 from .current import Current
-from .type_util import as_optional, is_optional
+from .type_util import as_optional, is_optional, as_list, as_newtype
 from .sum import Sum
 from .dispatch import Dispatcher, classdispatch
 from .config import (
     get_app_config_dir,
     get_app_cache_dir,
     get_workspace_dir,
     get_git_root,
```

### Comparing `miniscutil-0.0.2/miniscutil/adapt.py` & `miniscutil-0.0.3/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/asyncio_helpers.py` & `miniscutil-0.0.3/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/config.py` & `miniscutil-0.0.3/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/current.py` & `miniscutil-0.0.3/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/deep.py` & `miniscutil-0.0.3/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/deepeq.py` & `miniscutil-0.0.3/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/dispatch.py` & `miniscutil-0.0.3/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/misc.py` & `miniscutil-0.0.3/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/ofdict.py` & `miniscutil-0.0.3/miniscutil/ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/sum.py` & `miniscutil-0.0.3/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/miniscutil/type_util.py` & `miniscutil-0.0.3/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_classdispatch.py` & `miniscutil-0.0.3/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_config.py` & `miniscutil-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_current.py` & `miniscutil-0.0.3/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_deepeq.py` & `miniscutil-0.0.3/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_ofdict.py` & `miniscutil-0.0.3/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/tests/test_typing.py` & `miniscutil-0.0.3/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/.gitignore` & `miniscutil-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/LICENSE.txt` & `miniscutil-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/README.md` & `miniscutil-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/pyproject.toml` & `miniscutil-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.2/PKG-INFO` & `miniscutil-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

