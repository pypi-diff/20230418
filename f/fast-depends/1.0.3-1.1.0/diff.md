# Comparing `tmp/fast_depends-1.0.3.tar.gz` & `tmp/fast_depends-1.1.0.tar.gz`

## Comparing `fast_depends-1.0.3.tar` & `fast_depends-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/__init__.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/construct.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/injector.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/model.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/provider.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/types.py
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/usage.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.0.3/fast_depends/utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.0.3/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 fast_depends-1.0.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.0.3/LICENSE
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 fast_depends-1.0.3/README.md
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 fast_depends-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 fast_depends-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/__init__.py
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/construct.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/injector.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/model.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/provider.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/types.py
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/usage.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 fast_depends-1.1.0/fast_depends/library/model.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.0/README.md
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 fast_depends-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 fast_depends-1.1.0/PKG-INFO
```

### Comparing `fast_depends-1.0.3/CONTRIBUTING.md` & `fast_depends-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/.github/workflows/documentation.yml` & `fast_depends-1.1.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/.github/workflows/tests.yml` & `fast_depends-1.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/fast_depends/construct.py` & `fast_depends-1.1.0/fast_depends/construct.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 )
 from pydantic.schema import get_annotation_from_field_info
 from pydantic.typing import ForwardRef, evaluate_forwardref, get_args, get_origin
 from typing_extensions import Annotated
 
 from fast_depends import model
 from fast_depends.types import AnyCallable, AnyDict
+from fast_depends.library import CustomField
+
 
 sequence_shapes = {
     SHAPE_LIST,
     SHAPE_SET,
     SHAPE_FROZENSET,
     SHAPE_TUPLE,
     SHAPE_SEQUENCE,
@@ -49,25 +51,28 @@
         return_field=None,
     )
 
     endpoint_signature = get_typed_signature(call)
     signature_params = endpoint_signature.parameters
 
     for param in signature_params.values():
-        depends, param_field = analyze_param(
+        custom, depends, param_field = analyze_param(
             param_name=param.name,
             annotation=param.annotation,
             default=param.default,
         )
 
         if param.name == model.RETURN_FIELD:
             dependant.return_field = param_field
             continue
 
-        if depends is not None:
+        elif custom is not None:
+            dependant.custom.append(custom)
+
+        elif depends is not None:
             sub_dependant = get_param_sub_dependant(
                 param_name=param.name,
                 depends=depends,
                 path=path,
             )
             dependant.dependencies.append(sub_dependant)
 
@@ -77,60 +82,73 @@
 
 
 def analyze_param(
     *,
     param_name: str,
     annotation: Any,
     default: Any,
-) -> Tuple[Any, Optional[model.Depends], Optional[ModelField]]:
+) -> Tuple[Optional[CustomField], Optional[model.Depends], Optional[ModelField]]:
     depends = None
+    custom = None
     field_info = None
 
     if (
         annotation is not inspect.Signature.empty
         and get_origin(annotation) is Annotated  # type: ignore[comparison-overlap]
     ):
         annotated_args = get_args(annotation)
         custom_annotations = [
             arg
             for arg in annotated_args[1:]
-            if isinstance(arg, (FieldInfo, model.Depends))
+            if isinstance(arg, (FieldInfo, model.Depends, CustomField))
         ]
 
         custom_annotations = next(iter(custom_annotations), None)
         if isinstance(custom_annotations, FieldInfo):
             field_info = custom_annotations
             assert field_info.default is Undefined or field_info.default is Required, (
                 f"`{field_info.__class__.__name__}` default value cannot be set in"
                 f" `Annotated` for {param_name!r}. Set the default value with `=` instead."
             )
             field_info.default = Required
 
-        elif isinstance(custom_annotations, model.Depends):  # pragma: no branch
+        elif isinstance(custom_annotations, model.Depends):
             depends = custom_annotations
 
+        elif isinstance(custom_annotations, CustomField):  # pragma: no branch
+            custom_annotations.set_param_name(param_name)
+            custom = custom_annotations
+            if custom.cast is False:
+                annotation = Any
+
     if isinstance(default, model.Depends):
         assert depends is None, (
             "Cannot specify `Depends` in `Annotated` and default value"
             f" together for {param_name!r}"
         )
         assert field_info is None, (
             "Cannot specify a annotation in `Annotated` and `Depends` as a"
             f" default value together for {param_name!r}"
         )
         depends = default
 
+    elif isinstance(default, CustomField):
+        default.set_param_name(param_name)
+        custom = default
+        if custom.cast is False:
+            annotation = Any
+
     elif isinstance(default, FieldInfo):
         assert field_info is None, (
             "Cannot specify annotations in `Annotated` and default value"
             f" together for {param_name!r}"
         )
         field_info = default
 
-    if depends is not None:
+    if (depends or custom) is not None:
         field = None
 
     if field_info is not None:
         annotation = get_annotation_from_field_info(
             annotation if annotation is not inspect.Signature.empty else Any,
             field_info,
             param_name,
@@ -145,15 +163,15 @@
         type_=annotation,
         default=field_info.default if depends is None else None,
         alias=alias,
         required=field_info.default in (Required, Undefined, inspect._empty),
         field_info=field_info,
     )
 
-    return depends, field
+    return custom, depends, field
 
 
 def get_typed_signature(call: AnyCallable) -> inspect.Signature:
     signature = inspect.signature(call)
     globalns = getattr(call, "__globals__", {})
     typed_params = [
         inspect.Parameter(
```

### Comparing `fast_depends-1.0.3/fast_depends/injector.py` & `fast_depends-1.1.0/fast_depends/injector.py`

 * *Files 16% similar despite different names*

```diff
@@ -111,14 +111,17 @@
 
         if use_sub_dependant.name is not None:  # pragma: no branch
             body[use_sub_dependant.name] = solved
 
         if use_sub_dependant.cache_key not in dependency_cache:
             dependency_cache[use_sub_dependant.cache_key] = solved
 
+    for custom in dependant.custom:
+        body = await run_async(custom.use, **(body or {}))
+
     params, main_errors = params_to_args(dependant.params, body or {})
     errors.extend(main_errors)
     return params, errors, dependency_cache
 
 
 def solve_dependencies_sync(
     *,
@@ -199,14 +202,19 @@
 
         if use_sub_dependant.name is not None:  # pragma: no branch
             body[sub_dependant.name] = solved
 
         if use_sub_dependant.cache_key not in dependency_cache:
             dependency_cache[use_sub_dependant.cache_key] = solved
 
+    for custom in dependant.custom:
+        assert not is_coroutine_callable(custom.use) and not is_async_gen_callable(custom.use), \
+                f"You can't use async `{type(custom).__name__}` at sync code"
+        body = custom.use(**(body or {}))
+
     params, main_errors = params_to_args(dependant.params, body or {})
     errors.extend(main_errors)
     return params, errors, dependency_cache
 
 
 def params_to_args(
     required_params: Sequence[ModelField],
```

### Comparing `fast_depends-1.0.3/fast_depends/model.py` & `fast_depends-1.1.0/fast_depends/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from typing import Any, List, Optional, Tuple
 
 from pydantic import create_model
 from pydantic.error_wrappers import ErrorList
 from pydantic.fields import ModelField
 
 from fast_depends.types import AnyCallable
+from fast_depends.library import CustomField
+
 
 RETURN_FIELD = "custom_return"
 
 
 class Dependant:
     def __init__(
         self,
         *,
         call: Optional[AnyCallable] = None,
         params: Optional[List[ModelField]] = None,
         return_field: Optional[ModelField] = None,
         dependencies: Optional[List["Dependant"]] = None,
+        custom: Optional[List[CustomField]] = None,
         use_cache: bool = True,
         path: Optional[str] = None,
         name: Optional[str] = None,
     ) -> None:
         self.params = params or []
         self.return_field = return_field
         self.dependencies = dependencies or []
+        self.custom = custom or []
         self.call = call
         self.use_cache = use_cache
         # Parent argument name at subdependency
         self.name = name
         # Store the path to be able to re-generate a dependable from it in overrides
         self.path = path
         # Save the cache key at creation to optimize performance
```

### Comparing `fast_depends-1.0.3/fast_depends/usage.py` & `fast_depends-1.1.0/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/fast_depends/utils.py` & `fast_depends-1.1.0/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/LICENSE` & `fast_depends-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.0.3/README.md` & `fast_depends-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -174,40 +174,96 @@
 00000ad0: 6570 656e 6473 2a20 636c 6173 7365 730a  epends* classes.
 00000ae0: 2a20 6361 7374 2074 7970 6573 2061 6363  * cast types acc
 00000af0: 6f72 6469 6e67 2074 6f20 5079 7468 6f6e  ording to Python
 00000b00: 2061 6e6e 6f74 6174 696f 6e0a 2a20 7661   annotation.* va
 00000b10: 6c69 6461 7465 2069 6e63 6f6d 696e 6720  lidate incoming 
 00000b20: 7061 7261 6d65 7465 7273 2075 7369 6e67  parameters using
 00000b30: 202a 7079 6461 6e74 6963 2a0a 0a2d 2d2d   *pydantic*..---
-00000b40: 0a0a 2323 2320 4665 6174 7572 6573 0a53  ..### Features.S
-00000b50: 796e 6368 726f 6e6f 7573 2063 6f64 6520  ynchronous code 
-00000b60: 6973 2066 756c 6c79 2073 7570 706f 7274  is fully support
-00000b70: 6564 2069 6e20 7468 6973 2070 6163 6b61  ed in this packa
-00000b80: 6765 3a20 7769 7468 6f75 7420 616e 7920  ge: without any 
-00000b90: 6061 7379 6e63 5f74 6f5f 7379 6e63 602c  `async_to_sync`,
-00000ba0: 2060 7275 6e5f 7379 6e63 602c 2060 7379   `run_sync`, `sy
-00000bb0: 6e63 6966 7960 206f 7220 616e 7920 6f74  ncify` or any ot
-00000bc0: 6865 7220 7472 6963 6b73 2e0a 0a41 6c73  her tricks...Als
-00000bd0: 6f2c 202a 4661 7374 4465 7065 6e64 732a  o, *FastDepends*
-00000be0: 2063 6173 7473 2066 756e 6374 696f 6e73   casts functions
-00000bf0: 2720 7265 7475 726e 2076 616c 7565 7320  ' return values 
-00000c00: 7468 6520 7361 6d65 2077 6179 2c20 6974  the same way, it
-00000c10: 2063 616e 2062 6520 7665 7279 2068 656c   can be very hel
-00000c20: 7066 756c 2069 6e20 6275 696c 6469 6e67  pful in building
-00000c30: 2079 6f75 7220 6f77 6e20 746f 6f6c 732e   your own tools.
-00000c40: 0a0a 5468 6573 6520 6172 6520 7477 6f20  ..These are two 
-00000c50: 6d61 696e 2064 6566 6665 7265 6e63 6573  main defferences
-00000c60: 2066 726f 6d20 6e61 7469 7665 2046 6173   from native Fas
-00000c70: 7461 7069 2044 4920 5379 7374 656d 2e0a  tapi DI System..
-00000c80: 0a2d 2d2d 0a0a 2323 2320 4e6f 7465 0a4c  .---..### Note.L
-00000c90: 6962 7261 7279 2077 6173 2062 6173 6564  ibrary was based
-00000ca0: 206f 6e20 2a2a 302e 3935 2e30 2046 6173   on **0.95.0 Fas
-00000cb0: 7441 5049 2a2a 2076 6572 7369 6f6e 2e0a  tAPI** version..
-00000cc0: 0a49 6620 7765 2061 7265 2074 6f6f 2066  .If we are too f
-00000cd0: 6172 2062 6568 696e 642c 2070 6c65 6173  ar behind, pleas
-00000ce0: 652c 2063 6f6e 7461 6374 205b 6d65 5d28  e, contact [me](
-00000cf0: 6d61 696c 746f 3a64 6965 6d65 6e74 726f  mailto:diementro
-00000d00: 7340 7961 6e64 6578 2e72 7529 0a6f 7220  s@yandex.ru).or 
-00000d10: 636f 6e74 7562 7574 6520 796f 7572 7365  contubute yourse
-00000d20: 6c66 2e20 5265 616c 6c79 2061 7070 7265  lf. Really appre
-00000d30: 6369 6174 6520 796f 7572 2068 656c 702e  ciate your help.
-00000d40: 0a                                       .
+00000b40: 0a0a 2323 2320 4665 6174 7572 6573 0a0a  ..### Features..
+00000b50: 5379 6e63 6872 6f6e 6f75 7320 636f 6465  Synchronous code
+00000b60: 2069 7320 6675 6c6c 7920 7375 7070 6f72   is fully suppor
+00000b70: 7465 6420 696e 2074 6869 7320 7061 636b  ted in this pack
+00000b80: 6167 653a 2077 6974 686f 7574 2061 6e79  age: without any
+00000b90: 2060 6173 796e 635f 746f 5f73 796e 6360   `async_to_sync`
+00000ba0: 2c20 6072 756e 5f73 796e 6360 2c20 6073  , `run_sync`, `s
+00000bb0: 796e 6369 6679 6020 6f72 2061 6e79 206f  yncify` or any o
+00000bc0: 7468 6572 2074 7269 636b 732e 0a0a 416c  ther tricks...Al
+00000bd0: 736f 2c20 2a46 6173 7444 6570 656e 6473  so, *FastDepends
+00000be0: 2a20 6361 7374 7320 6675 6e63 7469 6f6e  * casts function
+00000bf0: 7327 2072 6574 7572 6e20 7661 6c75 6573  s' return values
+00000c00: 2074 6865 2073 616d 6520 7761 792c 2069   the same way, i
+00000c10: 7420 6361 6e20 6265 2076 6572 7920 6865  t can be very he
+00000c20: 6c70 6675 6c20 696e 2062 7569 6c64 696e  lpful in buildin
+00000c30: 6720 796f 7572 206f 776e 2074 6f6f 6c73  g your own tools
+00000c40: 2e0a 0a54 6865 7365 2061 7265 2074 776f  ...These are two
+00000c50: 206d 6169 6e20 6465 6666 6572 656e 6365   main defference
+00000c60: 7320 6672 6f6d 206e 6174 6976 6520 4661  s from native Fa
+00000c70: 7374 6170 6920 4449 2053 7973 7465 6d2e  stapi DI System.
+00000c80: 0a0a 2d2d 2d0a 0a23 2323 2043 7573 746f  ..---..### Custo
+00000c90: 6d20 4669 656c 6473 0a0a 4966 2079 6f75  m Fields..If you
+00000ca0: 2077 6973 6820 746f 2077 7269 7465 2079   wish to write y
+00000cb0: 6f75 7220 6f77 6e20 4661 7374 4150 4920  our own FastAPI 
+00000cc0: 6f72 2061 6e6f 7468 6572 2063 6c6f 7365  or another close
+00000cd0: 6c79 2062 7920 6172 6368 6974 6563 7475  ly by architectu
+00000ce0: 7265 2074 6f6f 6c2c 2079 6f75 2073 686f  re tool, you sho
+00000cf0: 756c 6420 6465 6669 6e65 2079 6f75 7220  uld define your 
+00000d00: 6f77 6e20 6375 7374 6f6d 2066 6965 6c64  own custom field
+00000d10: 7320 746f 2073 7065 6369 6679 2061 7070  s to specify app
+00000d20: 6c69 6361 7469 6f6e 2062 6568 6176 696f  lication behavio
+00000d30: 722e 0a0a 4375 7374 6f6d 2066 6965 6c64  r...Custom field
+00000d40: 7320 6361 6e20 6265 2075 7365 6420 746f  s can be used to
+00000d50: 2061 6464 696e 6720 736f 6d65 7468 696e   adding somethin
+00000d60: 6720 7370 6563 6966 6963 2074 6f20 6120  g specific to a 
+00000d70: 6675 6e63 7469 6f6e 2061 7267 756d 656e  function argumen
+00000d80: 7473 2028 6c69 6b65 2061 2042 6163 6b67  ts (like a Backg
+00000d90: 726f 756e 6454 6173 6b29 206f 7220 7061  roundTask) or pa
+00000da0: 7273 696e 6720 696e 636f 6d69 6e67 206f  rsing incoming o
+00000db0: 626a 6563 7473 2073 7065 6369 616c 2077  bjects special w
+00000dc0: 6179 2e20 596f 7520 6162 6c65 2064 6563  ay. You able dec
+00000dd0: 6964 6520 6279 206f 776e 2c20 7768 7920  ide by own, why 
+00000de0: 616e 6420 686f 7720 796f 7520 7769 6c6c  and how you will
+00000df0: 2075 7365 2074 6865 7365 2074 6f6f 6c73   use these tools
+00000e00: 2e0a 0a46 6173 7444 6570 656e 6473 2067  ...FastDepends g
+00000e10: 7261 6e74 7320 796f 7520 7468 6973 206f  rants you this o
+00000e20: 7070 6f72 7475 6e69 7479 2061 2076 6572  pportunity a ver
+00000e30: 7920 696e 7475 6974 6976 6520 616e 6420  y intuitive and 
+00000e40: 636f 6d66 6f72 7461 626c 6520 7761 792e  comfortable way.
+00000e50: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000e60: 2066 6173 745f 6465 7065 6e64 7320 696d   fast_depends im
+00000e70: 706f 7274 2069 6e6a 6563 740a 6672 6f6d  port inject.from
+00000e80: 2066 6173 745f 6465 7065 6e64 732e 6c69   fast_depends.li
+00000e90: 6272 6172 7920 696d 706f 7274 2043 7573  brary import Cus
+00000ea0: 746f 6d46 6965 6c64 0a0a 636c 6173 7320  tomField..class 
+00000eb0: 4865 6164 6572 2843 7573 746f 6d46 6965  Header(CustomFie
+00000ec0: 6c64 293a 0a20 2020 2064 6566 2075 7365  ld):.    def use
+00000ed0: 2873 656c 662c 202a 2a6b 7761 7267 733a  (self, **kwargs:
+00000ee0: 2041 6e79 4469 6374 2920 2d3e 2041 6e79   AnyDict) -> Any
+00000ef0: 4469 6374 3a0a 2020 2020 2020 2020 6b77  Dict:.        kw
+00000f00: 6172 6773 203d 2073 7570 6572 2829 2e75  args = super().u
+00000f10: 7365 282a 2a6b 7761 7267 7329 0a20 2020  se(**kwargs).   
+00000f20: 2020 2020 206b 7761 7267 735b 7365 6c66       kwargs[self
+00000f30: 2e70 6172 616d 5f6e 616d 655d 203d 206b  .param_name] = k
+00000f40: 7761 7267 735b 2268 6561 6465 7273 225d  wargs["headers"]
+00000f50: 5b73 656c 662e 7061 7261 6d5f 6e61 6d65  [self.param_name
+00000f60: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+00000f70: 206b 7761 7267 730a 0a40 696e 6a65 6374   kwargs..@inject
+00000f80: 0a64 6566 206d 795f 6675 6e63 2868 6561  .def my_func(hea
+00000f90: 6465 725f 6669 656c 643a 2069 6e74 203d  der_field: int =
+00000fa0: 2048 6561 6465 7228 2929 3a0a 2020 2020   Header()):.    
+00000fb0: 7265 7475 726e 2068 6561 6465 725f 6669  return header_fi
+00000fc0: 656c 640a 0a61 7373 6572 7420 6d79 5f66  eld..assert my_f
+00000fd0: 756e 6328 0a20 2020 2068 6561 6465 7273  unc(.    headers
+00000fe0: 3d7b 2022 6865 6164 6572 5f66 6965 6c64  ={ "header_field
+00000ff0: 223a 2022 3122 207d 0a29 203d 3d20 310a  ": "1" }.) == 1.
+00001000: 6060 600a 0a2d 2d2d 0a0a 2323 2320 4e6f  ```..---..### No
+00001010: 7465 0a4c 6962 7261 7279 2077 6173 2062  te.Library was b
+00001020: 6173 6564 206f 6e20 2a2a 302e 3935 2e30  ased on **0.95.0
+00001030: 2046 6173 7441 5049 2a2a 2076 6572 7369   FastAPI** versi
+00001040: 6f6e 2e0a 0a49 6620 7765 2061 7265 2074  on...If we are t
+00001050: 6f6f 2066 6172 2062 6568 696e 642c 2070  oo far behind, p
+00001060: 6c65 6173 652c 2063 6f6e 7461 6374 205b  lease, contact [
+00001070: 6d65 5d28 6d61 696c 746f 3a64 6965 6d65  me](mailto:dieme
+00001080: 6e74 726f 7340 7961 6e64 6578 2e72 7529  ntros@yandex.ru)
+00001090: 0a6f 7220 636f 6e74 7562 7574 6520 796f  .or contubute yo
+000010a0: 7572 7365 6c66 2e20 5265 616c 6c79 2061  urself. Really a
+000010b0: 7070 7265 6369 6174 6520 796f 7572 2068  ppreciate your h
+000010c0: 656c 702e 0a                             elp..
```

### Comparing `fast_depends-1.0.3/pyproject.toml` & `fast_depends-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 Homepage = "https://lancetnik.github.io/FastDepends/"
 Documentation = "https://lancetnik.github.io/FastDepends/"
 Tracker = "https://github.com/Lancetnik/FastDepends/issues"
 Source = "https://github.com/Lancetnik/FastDepends"
 
 [project.optional-dependencies]
 test = [
+    "toml",
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
     "pytest-xdist[psutil]",
 
     "asyncmock; python_version < '3.8'",
 ]
@@ -63,16 +64,16 @@
 doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
 ]
 
 dev = [
-    "FastDepends[test]",
-    "FastDepends[doc]",
+    "fast-depends[test]",
+    "fast-depends[doc]",
 
     "mypy>=1.1",
     "black>=23.3.0",
     "isort>=5",
     "ruff>=0.0.260",
 ]
```

### Comparing `fast_depends-1.0.3/PKG-INFO` & `fast_depends-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 2d64 6570 656e 6473 0a56 6572 7369 6f6e  -depends.Version
-00000030: 3a20 312e 302e 330a 5375 6d6d 6172 793a  : 1.0.3.Summary:
+00000030: 3a20 312e 312e 300a 5375 6d6d 6172 793a  : 1.1.0.Summary:
 00000040: 2046 6173 7444 6570 656e 6473 202d 2065   FastDepends - e
 00000050: 7874 7261 6374 6564 2061 6e64 2063 6c65  xtracted and cle
 00000060: 6172 6564 2066 726f 6d20 4854 5450 2064  ared from HTTP d
 00000070: 6f6d 6169 6e20 6c6f 6769 6320 4661 7374  omain logic Fast
 00000080: 4150 4920 4465 7065 6e64 656e 6379 2049  API Dependency I
 00000090: 6e6a 6563 7469 6f6e 2053 7973 7465 6d2e  njection System.
 000000a0: 2041 7379 6e63 2061 6e64 2073 796e 6320   Async and sync 
@@ -101,267 +101,325 @@
 00000640: 696f 0a52 6571 7569 7265 732d 4469 7374  io.Requires-Dist
 00000650: 3a20 7079 6461 6e74 6963 3e3d 312e 380a  : pydantic>=1.8.
 00000660: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 00000670: 6465 760a 5265 7175 6972 6573 2d44 6973  dev.Requires-Dis
 00000680: 743a 2062 6c61 636b 3e3d 3233 2e33 2e30  t: black>=23.3.0
 00000690: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
 000006a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006b0: 6661 7374 6465 7065 6e64 735b 646f 635d  fastdepends[doc]
-000006c0: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
-000006d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000006e0: 6661 7374 6465 7065 6e64 735b 7465 7374  fastdepends[test
-000006f0: 5d3b 2065 7874 7261 203d 3d20 2764 6576  ]; extra == 'dev
-00000700: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00000710: 2069 736f 7274 3e3d 353b 2065 7874 7261   isort>=5; extra
-00000720: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
-00000730: 6573 2d44 6973 743a 206d 7970 793e 3d31  es-Dist: mypy>=1
-00000740: 2e31 3b20 6578 7472 6120 3d3d 2027 6465  .1; extra == 'de
-00000750: 7627 0a52 6571 7569 7265 732d 4469 7374  v'.Requires-Dist
-00000760: 3a20 7275 6666 3e3d 302e 302e 3236 303b  : ruff>=0.0.260;
-00000770: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000780: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000790: 646f 630a 5265 7175 6972 6573 2d44 6973  doc.Requires-Dis
-000007a0: 743a 206d 6478 2d69 6e63 6c75 6465 3c32  t: mdx-include<2
-000007b0: 2e30 2e30 2c3e 3d31 2e34 2e31 3b20 6578  .0.0,>=1.4.1; ex
-000007c0: 7472 6120 3d3d 2027 646f 6327 0a52 6571  tra == 'doc'.Req
-000007d0: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
-000007e0: 6373 2d6d 6172 6b64 6f77 6e65 7874 7261  cs-markdownextra
-000007f0: 6461 7461 2d70 6c75 6769 6e3c 302e 332e  data-plugin<0.3.
-00000800: 302c 3e3d 302e 312e 373b 2065 7874 7261  0,>=0.1.7; extra
-00000810: 203d 3d20 2764 6f63 270a 5265 7175 6972   == 'doc'.Requir
-00000820: 6573 2d44 6973 743a 206d 6b64 6f63 732d  es-Dist: mkdocs-
-00000830: 6d61 7465 7269 616c 3c39 2e30 2e30 2c3e  material<9.0.0,>
-00000840: 3d38 2e31 2e34 3b20 6578 7472 6120 3d3d  =8.1.4; extra ==
-00000850: 2027 646f 6327 0a50 726f 7669 6465 732d   'doc'.Provides-
-00000860: 4578 7472 613a 2074 6573 740a 5265 7175  Extra: test.Requ
-00000870: 6972 6573 2d44 6973 743a 2061 7379 6e63  ires-Dist: async
-00000880: 6d6f 636b 3b20 7079 7468 6f6e 5f76 6572  mock; python_ver
-00000890: 7369 6f6e 203c 2027 332e 3827 2061 6e64  sion < '3.8' and
-000008a0: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-000008b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000008c0: 636f 7665 7261 6765 5b74 6f6d 6c5d 3e3d  coverage[toml]>=
-000008d0: 372e 323b 2065 7874 7261 203d 3d20 2774  7.2; extra == 't
-000008e0: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-000008f0: 7374 3a20 7079 7465 7374 2d61 7379 6e63  st: pytest-async
-00000900: 696f 3e3d 302e 3231 3b20 6578 7472 6120  io>=0.21; extra 
-00000910: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-00000920: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
-00000930: 7864 6973 745b 7073 7574 696c 5d3b 2065  xdist[psutil]; e
-00000940: 7874 7261 203d 3d20 2774 6573 7427 0a52  xtra == 'test'.R
-00000950: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000960: 7465 7374 3e3d 373b 2065 7874 7261 203d  test>=7; extra =
-00000970: 3d20 2774 6573 7427 0a44 6573 6372 6970  = 'test'.Descrip
-00000980: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00000990: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000009a0: 0a0a 2320 4661 7374 4465 7065 6e64 730a  ..# FastDepends.
-000009b0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000009c0: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
-000009d0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000009e0: 636f 6d2f 4c61 6e63 6574 6e69 6b2f 4661  com/Lancetnik/Fa
-000009f0: 7374 4465 7065 6e64 732f 6163 7469 6f6e  stDepends/action
-00000a00: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000a10: 732e 796d 6c22 2074 6172 6765 743d 225f  s.yml" target="_
-00000a20: 626c 616e 6b22 3e0a 2020 2020 2020 2020  blank">.        
-00000a30: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000a40: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 616e  //github.com/Lan
-00000a50: 6365 746e 696b 2f46 6173 7444 6570 656e  cetnik/FastDepen
-00000a60: 6473 2f61 6374 696f 6e73 2f77 6f72 6b66  ds/actions/workf
-00000a70: 6c6f 7773 2f74 6573 7473 2e79 6d6c 2f62  lows/tests.yml/b
-00000a80: 6164 6765 2e73 7667 2220 616c 743d 2254  adge.svg" alt="T
-00000a90: 6573 7473 2063 6f76 6572 6167 6522 2f3e  ests coverage"/>
-00000aa0: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
-00000ab0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
-00000ac0: 6f76 6572 6167 652d 6261 6467 652e 7361  overage-badge.sa
-00000ad0: 6d75 656c 636f 6c76 696e 2e77 6f72 6b65  muelcolvin.worke
-00000ae0: 7273 2e64 6576 2f72 6564 6972 6563 742f  rs.dev/redirect/
-00000af0: 6c61 6e63 6574 6e69 6b2f 6661 7374 6465  lancetnik/fastde
-00000b00: 7065 6e64 7322 2074 6172 6765 743d 225f  pends" target="_
-00000b10: 626c 616e 6b22 3e0a 2020 2020 2020 2020  blank">.        
-00000b20: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000b30: 2f2f 636f 7665 7261 6765 2d62 6164 6765  //coverage-badge
-00000b40: 2e73 616d 7565 6c63 6f6c 7669 6e2e 776f  .samuelcolvin.wo
-00000b50: 726b 6572 732e 6465 762f 6c61 6e63 6574  rkers.dev/lancet
-00000b60: 6e69 6b2f 6661 7374 6465 7065 6e64 732e  nik/fastdepends.
-00000b70: 7376 6722 2061 6c74 3d22 436f 7665 7261  svg" alt="Covera
-00000b80: 6765 223e 0a20 2020 203c 2f61 3e0a 2020  ge">.    </a>.  
-00000b90: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000ba0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000bb0: 6563 742f 6661 7374 2d64 6570 656e 6473  ect/fast-depends
-00000bc0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000bd0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-00000be0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000bf0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000c00: 2f76 2f66 6173 742d 6465 7065 6e64 733f  /v/fast-depends?
-00000c10: 6c61 6265 6c3d 7079 7069 2532 3070 6163  label=pypi%20pac
-00000c20: 6b61 6765 2220 616c 743d 2250 6163 6b61  kage" alt="Packa
-00000c30: 6765 2076 6572 7369 6f6e 223e 0a20 2020  ge version">.   
-00000c40: 203c 2f61 3e0a 2020 2020 3c61 2068 7265   </a>.    <a hre
-00000c50: 663d 2268 7474 7073 3a2f 2f70 6570 792e  f="https://pepy.
-00000c60: 7465 6368 2f70 726f 6a65 6374 2f66 6173  tech/project/fas
-00000c70: 742d 6465 7065 6e64 7322 2074 6172 6765  t-depends" targe
-00000c80: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00000c90: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000ca0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-00000cb0: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
-00000cc0: 7a65 642d 6261 6467 652f 6661 7374 2d64  zed-badge/fast-d
-00000cd0: 6570 656e 6473 3f70 6572 696f 643d 746f  epends?period=to
-00000ce0: 7461 6c26 756e 6974 733d 696e 7465 726e  tal&units=intern
-00000cf0: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
-00000d00: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
-00000d10: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-00000d20: 6c65 6674 5f74 6578 743d 446f 776e 6c6f  left_text=Downlo
-00000d30: 6164 7322 2061 6c74 3d22 646f 776e 6c6f  ads" alt="downlo
-00000d40: 6164 7322 2f3e 0a20 2020 203c 2f61 3e0a  ads"/>.    </a>.
-00000d50: 2020 2020 3c62 722f 3e0a 2020 2020 3c61      <br/>.    <a
-00000d60: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000d70: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000d80: 6661 7374 2d64 6570 656e 6422 2074 6172  fast-depend" tar
-00000d90: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
-00000da0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
-00000db0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000dc0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
-00000dd0: 7273 696f 6e73 2f66 6173 742d 6465 7065  rsions/fast-depe
-00000de0: 6e64 732e 7376 6722 2061 6c74 3d22 5375  nds.svg" alt="Su
-00000df0: 7070 6f72 7465 6420 5079 7468 6f6e 2076  pported Python v
-00000e00: 6572 7369 6f6e 7322 3e0a 2020 2020 3c2f  ersions">.    </
-00000e10: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
-00000e20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000e30: 6f6d 2f4c 616e 6365 746e 696b 2f46 6173  om/Lancetnik/Fas
-00000e40: 7444 6570 656e 6473 2f62 6c6f 622f 6d61  tDepends/blob/ma
-00000e50: 696e 2f4c 4943 454e 5345 2220 7461 7267  in/LICENSE" targ
-00000e60: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-00000e70: 2020 2020 203c 696d 6720 616c 743d 2247       <img alt="G
-00000e80: 6974 4875 6222 2073 7263 3d22 6874 7470  itHub" src="http
-00000e90: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000ea0: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
-00000eb0: 652f 4c61 6e63 6574 6e69 6b2f 4661 7374  e/Lancetnik/Fast
-00000ec0: 4465 7065 6e64 733f 636f 6c6f 723d 2532  Depends?color=%2
-00000ed0: 3330 3037 6563 3622 3e0a 2020 2020 3c2f  3007ec6">.    </
-00000ee0: 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a 446f  a>.</p>..---..Do
-00000ef0: 6375 6d65 6e74 6174 696f 6e3a 2068 7474  cumentation: htt
-00000f00: 7073 3a2f 2f6c 616e 6365 746e 696b 2e67  ps://lancetnik.g
-00000f10: 6974 6875 622e 696f 2f46 6173 7444 6570  ithub.io/FastDep
-00000f20: 656e 6473 2f0a 0a2d 2d2d 0a0a 4661 7374  ends/..---..Fast
-00000f30: 4465 7065 6e64 7320 2d20 4661 7374 4150  Depends - FastAP
-00000f40: 4920 4465 7065 6e64 656e 6379 2049 6e6a  I Dependency Inj
-00000f50: 6563 7469 6f6e 2073 7973 7465 6d20 6578  ection system ex
-00000f60: 7472 6163 7465 6420 6672 6f6d 2046 6173  tracted from Fas
-00000f70: 7441 5049 2061 6e64 2063 6c65 6172 6564  tAPI and cleared
-00000f80: 206f 6620 616c 6c20 4854 5450 206c 6f67   of all HTTP log
-00000f90: 6963 2e0a 5468 6973 2069 7320 6120 736d  ic..This is a sm
-00000fa0: 616c 6c20 6c69 6272 6172 7920 7768 6963  all library whic
-00000fb0: 6820 7072 6f76 6964 6573 2079 6f75 2077  h provides you w
-00000fc0: 6974 6820 7468 6520 6162 696c 6974 7920  ith the ability 
-00000fd0: 746f 2075 7365 206c 6f76 656c 7920 4661  to use lovely Fa
-00000fe0: 7374 6170 6920 696e 7465 7266 6163 6573  stapi interfaces
-00000ff0: 2069 6e20 796f 7572 206f 776e 0a70 726f   in your own.pro
-00001000: 6a65 6374 7320 6f72 2074 6f6f 6c73 2e0a  jects or tools..
-00001010: 0a54 6861 6e6b 7320 746f 205b 2a66 6173  .Thanks to [*fas
-00001020: 7461 7069 2a5d 2868 7474 7073 3a2f 2f66  tapi*](https://f
-00001030: 6173 7461 7069 2e74 6961 6e67 6f6c 6f2e  astapi.tiangolo.
-00001040: 636f 6d2f 2920 616e 6420 5b2a 7079 6461  com/) and [*pyda
-00001050: 6e74 6963 2a5d 2868 7474 7073 3a2f 2f64  ntic*](https://d
-00001060: 6f63 732e 7079 6461 6e74 6963 2e64 6576  ocs.pydantic.dev
-00001070: 2f29 2070 726f 6a65 6374 7320 666f 7220  /) projects for 
-00001080: 7468 6973 0a67 7265 6174 6520 6675 6e63  this.greate func
-00001090: 7469 6f6e 616c 6974 792e 2054 6869 7320  tionality. This 
-000010a0: 7061 636b 6167 6520 6973 206a 7573 7420  package is just 
-000010b0: 6120 736d 616c 6c20 6368 616e 6765 206f  a small change o
-000010c0: 6620 7468 6520 6f72 6967 696e 616c 2046  f the original F
-000010d0: 6173 7461 7069 2073 6f75 7263 6573 2074  astapi sources t
-000010e0: 6f20 7072 6f76 6964 6520 4449 2066 756e  o provide DI fun
-000010f0: 6374 696f 6e61 6c69 7479 2069 6e20 6120  ctionality in a 
-00001100: 7079 7265 2d50 7974 686f 6e20 7761 792e  pyre-Python way.
-00001110: 0a0a 4173 796e 6320 616e 6420 7379 6e63  ..Async and sync
-00001120: 206d 6f64 6573 2061 7265 2062 6f74 6820   modes are both 
-00001130: 7375 7070 6f72 7465 642e 0a0a 2323 2049  supported...## I
-00001140: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-00001150: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
-00001160: 2066 6173 742d 6465 7065 6e64 730a 6060   fast-depends.``
-00001170: 600a 0a23 2320 5573 6167 650a 0a54 6865  `..## Usage..The
-00001180: 7265 2069 7320 6e6f 2077 6179 2074 6f20  re is no way to 
-00001190: 6d61 6b65 2044 6570 656e 6465 6e63 7920  make Dependency 
-000011a0: 496e 6a65 6374 696f 6e20 6561 7369 6572  Injection easier
-000011b0: 0a0a 596f 7520 6361 6e20 7573 6520 7468  ..You can use th
-000011c0: 6973 206c 6962 7261 7279 2077 6974 686f  is library witho
-000011d0: 7574 2061 6e79 2066 7261 6d65 776f 726b  ut any framework
-000011e0: 7320 696e 2062 6f74 6820 2a2a 7379 6e63  s in both **sync
-000011f0: 2a2a 2061 6e64 202a 2a61 7379 6e63 2a2a  ** and **async**
-00001200: 2063 6f64 652e 0a0a 2323 2320 4173 796e   code...### Asyn
-00001210: 6320 636f 6465 0a60 6060 7079 7468 6f6e  c code.```python
-00001220: 0a69 6d70 6f72 7420 6173 796e 6369 6f0a  .import asyncio.
-00001230: 0a66 726f 6d20 6661 7374 5f64 6570 656e  .from fast_depen
-00001240: 6473 2069 6d70 6f72 7420 696e 6a65 6374  ds import inject
-00001250: 2c20 4465 7065 6e64 730a 0a61 7379 6e63  , Depends..async
-00001260: 2064 6566 2064 6570 656e 6465 6e63 7928   def dependency(
-00001270: 613a 2069 6e74 2920 2d3e 2069 6e74 3a0a  a: int) -> int:.
-00001280: 2020 2020 7265 7475 726e 2061 0a0a 4069      return a..@i
-00001290: 6e6a 6563 740a 6173 796e 6320 6465 6620  nject.async def 
-000012a0: 6d61 696e 280a 2020 2020 613a 2069 6e74  main(.    a: int
-000012b0: 2c0a 2020 2020 623a 2069 6e74 2c0a 2020  ,.    b: int,.  
-000012c0: 2020 633a 2069 6e74 203d 2044 6570 656e    c: int = Depen
-000012d0: 6473 2864 6570 656e 6465 6e63 7929 0a29  ds(dependency).)
-000012e0: 202d 3e20 666c 6f61 743a 0a20 2020 2072   -> float:.    r
-000012f0: 6574 7572 6e20 6120 2b20 6220 2b20 630a  eturn a + b + c.
-00001300: 0a61 7373 6572 7420 6173 796e 6369 6f2e  .assert asyncio.
-00001310: 7275 6e28 6d61 696e 2822 3122 2c20 3229  run(main("1", 2)
-00001320: 2920 3d3d 2034 2e30 0a60 6060 0a0a 2323  ) == 4.0.```..##
-00001330: 2320 5379 6e63 2063 6f64 650a 6060 6070  # Sync code.```p
-00001340: 7974 686f 6e0a 6672 6f6d 2066 6173 745f  ython.from fast_
-00001350: 6465 7065 6e64 7320 696d 706f 7274 2069  depends import i
-00001360: 6e6a 6563 742c 2044 6570 656e 6473 0a0a  nject, Depends..
-00001370: 6465 6620 6465 7065 6e64 656e 6379 2861  def dependency(a
-00001380: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
-00001390: 2020 2072 6574 7572 6e20 610a 0a40 696e     return a..@in
-000013a0: 6a65 6374 0a64 6566 206d 6169 6e28 0a20  ject.def main(. 
-000013b0: 2020 2061 3a20 696e 742c 0a20 2020 2062     a: int,.    b
-000013c0: 3a20 696e 742c 0a20 2020 2063 3a20 696e  : int,.    c: in
-000013d0: 7420 3d20 4465 7065 6e64 7328 6465 7065  t = Depends(depe
-000013e0: 6e64 656e 6379 290a 2920 2d3e 2066 6c6f  ndency).) -> flo
-000013f0: 6174 3a0a 2020 2020 7265 7475 726e 2061  at:.    return a
-00001400: 202b 2062 202b 2063 0a0a 6173 7365 7274   + b + c..assert
-00001410: 206d 6169 6e28 2231 222c 2032 2920 3d3d   main("1", 2) ==
-00001420: 2034 2e30 0a60 6060 0a0a 6040 696e 6a65   4.0.```..`@inje
-00001430: 6374 6020 6465 636f 7261 746f 7220 706c  ct` decorator pl
-00001440: 6179 7320 6d75 6c74 6970 6c65 2072 6f6c  ays multiple rol
-00001450: 6573 2061 7420 7468 6520 7361 6d65 2074  es at the same t
-00001460: 696d 653a 0a0a 2a20 7265 736f 6c76 6520  ime:..* resolve 
-00001470: 2a44 6570 656e 6473 2a20 636c 6173 7365  *Depends* classe
-00001480: 730a 2a20 6361 7374 2074 7970 6573 2061  s.* cast types a
-00001490: 6363 6f72 6469 6e67 2074 6f20 5079 7468  ccording to Pyth
-000014a0: 6f6e 2061 6e6e 6f74 6174 696f 6e0a 2a20  on annotation.* 
-000014b0: 7661 6c69 6461 7465 2069 6e63 6f6d 696e  validate incomin
-000014c0: 6720 7061 7261 6d65 7465 7273 2075 7369  g parameters usi
-000014d0: 6e67 202a 7079 6461 6e74 6963 2a0a 0a2d  ng *pydantic*..-
-000014e0: 2d2d 0a0a 2323 2320 4665 6174 7572 6573  --..### Features
-000014f0: 0a53 796e 6368 726f 6e6f 7573 2063 6f64  .Synchronous cod
-00001500: 6520 6973 2066 756c 6c79 2073 7570 706f  e is fully suppo
-00001510: 7274 6564 2069 6e20 7468 6973 2070 6163  rted in this pac
-00001520: 6b61 6765 3a20 7769 7468 6f75 7420 616e  kage: without an
-00001530: 7920 6061 7379 6e63 5f74 6f5f 7379 6e63  y `async_to_sync
-00001540: 602c 2060 7275 6e5f 7379 6e63 602c 2060  `, `run_sync`, `
-00001550: 7379 6e63 6966 7960 206f 7220 616e 7920  syncify` or any 
-00001560: 6f74 6865 7220 7472 6963 6b73 2e0a 0a41  other tricks...A
-00001570: 6c73 6f2c 202a 4661 7374 4465 7065 6e64  lso, *FastDepend
-00001580: 732a 2063 6173 7473 2066 756e 6374 696f  s* casts functio
-00001590: 6e73 2720 7265 7475 726e 2076 616c 7565  ns' return value
-000015a0: 7320 7468 6520 7361 6d65 2077 6179 2c20  s the same way, 
-000015b0: 6974 2063 616e 2062 6520 7665 7279 2068  it can be very h
-000015c0: 656c 7066 756c 2069 6e20 6275 696c 6469  elpful in buildi
-000015d0: 6e67 2079 6f75 7220 6f77 6e20 746f 6f6c  ng your own tool
-000015e0: 732e 0a0a 5468 6573 6520 6172 6520 7477  s...These are tw
-000015f0: 6f20 6d61 696e 2064 6566 6665 7265 6e63  o main defferenc
-00001600: 6573 2066 726f 6d20 6e61 7469 7665 2046  es from native F
-00001610: 6173 7461 7069 2044 4920 5379 7374 656d  astapi DI System
-00001620: 2e0a 0a2d 2d2d 0a0a 2323 2320 4e6f 7465  ...---..### Note
-00001630: 0a4c 6962 7261 7279 2077 6173 2062 6173  .Library was bas
-00001640: 6564 206f 6e20 2a2a 302e 3935 2e30 2046  ed on **0.95.0 F
-00001650: 6173 7441 5049 2a2a 2076 6572 7369 6f6e  astAPI** version
-00001660: 2e0a 0a49 6620 7765 2061 7265 2074 6f6f  ...If we are too
-00001670: 2066 6172 2062 6568 696e 642c 2070 6c65   far behind, ple
-00001680: 6173 652c 2063 6f6e 7461 6374 205b 6d65  ase, contact [me
-00001690: 5d28 6d61 696c 746f 3a64 6965 6d65 6e74  ](mailto:diement
-000016a0: 726f 7340 7961 6e64 6578 2e72 7529 0a6f  ros@yandex.ru).o
-000016b0: 7220 636f 6e74 7562 7574 6520 796f 7572  r contubute your
-000016c0: 7365 6c66 2e20 5265 616c 6c79 2061 7070  self. Really app
-000016d0: 7265 6369 6174 6520 796f 7572 2068 656c  reciate your hel
-000016e0: 702e 0a                                  p..
+000006b0: 6661 7374 2d64 6570 656e 6473 5b64 6f63  fast-depends[doc
+000006c0: 5d3b 2065 7874 7261 203d 3d20 2764 6576  ]; extra == 'dev
+000006d0: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
+000006e0: 2066 6173 742d 6465 7065 6e64 735b 7465   fast-depends[te
+000006f0: 7374 5d3b 2065 7874 7261 203d 3d20 2764  st]; extra == 'd
+00000700: 6576 270a 5265 7175 6972 6573 2d44 6973  ev'.Requires-Dis
+00000710: 743a 2069 736f 7274 3e3d 353b 2065 7874  t: isort>=5; ext
+00000720: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
+00000730: 6972 6573 2d44 6973 743a 206d 7970 793e  ires-Dist: mypy>
+00000740: 3d31 2e31 3b20 6578 7472 6120 3d3d 2027  =1.1; extra == '
+00000750: 6465 7627 0a52 6571 7569 7265 732d 4469  dev'.Requires-Di
+00000760: 7374 3a20 7275 6666 3e3d 302e 302e 3236  st: ruff>=0.0.26
+00000770: 303b 2065 7874 7261 203d 3d20 2764 6576  0; extra == 'dev
+00000780: 270a 5072 6f76 6964 6573 2d45 7874 7261  '.Provides-Extra
+00000790: 3a20 646f 630a 5265 7175 6972 6573 2d44  : doc.Requires-D
+000007a0: 6973 743a 206d 6478 2d69 6e63 6c75 6465  ist: mdx-include
+000007b0: 3c32 2e30 2e30 2c3e 3d31 2e34 2e31 3b20  <2.0.0,>=1.4.1; 
+000007c0: 6578 7472 6120 3d3d 2027 646f 6327 0a52  extra == 'doc'.R
+000007d0: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
+000007e0: 646f 6373 2d6d 6172 6b64 6f77 6e65 7874  docs-markdownext
+000007f0: 7261 6461 7461 2d70 6c75 6769 6e3c 302e  radata-plugin<0.
+00000800: 332e 302c 3e3d 302e 312e 373b 2065 7874  3.0,>=0.1.7; ext
+00000810: 7261 203d 3d20 2764 6f63 270a 5265 7175  ra == 'doc'.Requ
+00000820: 6972 6573 2d44 6973 743a 206d 6b64 6f63  ires-Dist: mkdoc
+00000830: 732d 6d61 7465 7269 616c 3c39 2e30 2e30  s-material<9.0.0
+00000840: 2c3e 3d38 2e31 2e34 3b20 6578 7472 6120  ,>=8.1.4; extra 
+00000850: 3d3d 2027 646f 6327 0a50 726f 7669 6465  == 'doc'.Provide
+00000860: 732d 4578 7472 613a 2074 6573 740a 5265  s-Extra: test.Re
+00000870: 7175 6972 6573 2d44 6973 743a 2061 7379  quires-Dist: asy
+00000880: 6e63 6d6f 636b 3b20 7079 7468 6f6e 5f76  ncmock; python_v
+00000890: 6572 7369 6f6e 203c 2027 332e 3827 2061  ersion < '3.8' a
+000008a0: 6e64 2065 7874 7261 203d 3d20 2774 6573  nd extra == 'tes
+000008b0: 7427 0a52 6571 7569 7265 732d 4469 7374  t'.Requires-Dist
+000008c0: 3a20 636f 7665 7261 6765 5b74 6f6d 6c5d  : coverage[toml]
+000008d0: 3e3d 372e 323b 2065 7874 7261 203d 3d20  >=7.2; extra == 
+000008e0: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
+000008f0: 4469 7374 3a20 7079 7465 7374 2d61 7379  Dist: pytest-asy
+00000900: 6e63 696f 3e3d 302e 3231 3b20 6578 7472  ncio>=0.21; extr
+00000910: 6120 3d3d 2027 7465 7374 270a 5265 7175  a == 'test'.Requ
+00000920: 6972 6573 2d44 6973 743a 2070 7974 6573  ires-Dist: pytes
+00000930: 742d 7864 6973 745b 7073 7574 696c 5d3b  t-xdist[psutil];
+00000940: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
+00000950: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000960: 7079 7465 7374 3e3d 373b 2065 7874 7261  pytest>=7; extra
+00000970: 203d 3d20 2774 6573 7427 0a52 6571 7569   == 'test'.Requi
+00000980: 7265 732d 4469 7374 3a20 746f 6d6c 3b20  res-Dist: toml; 
+00000990: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
+000009a0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000009b0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000009c0: 6172 6b64 6f77 6e0a 0a23 2046 6173 7444  arkdown..# FastD
+000009d0: 6570 656e 6473 0a0a 3c70 2061 6c69 676e  epends..<p align
+000009e0: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+000009f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000a00: 6769 7468 7562 2e63 6f6d 2f4c 616e 6365  github.com/Lance
+00000a10: 746e 696b 2f46 6173 7444 6570 656e 6473  tnik/FastDepends
+00000a20: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000a30: 7773 2f74 6573 7473 2e79 6d6c 2220 7461  ws/tests.yml" ta
+00000a40: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00000a50: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+00000a60: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000a70: 636f 6d2f 4c61 6e63 6574 6e69 6b2f 4661  com/Lancetnik/Fa
+00000a80: 7374 4465 7065 6e64 732f 6163 7469 6f6e  stDepends/action
+00000a90: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+00000aa0: 732e 796d 6c2f 6261 6467 652e 7376 6722  s.yml/badge.svg"
+00000ab0: 2061 6c74 3d22 5465 7374 7320 636f 7665   alt="Tests cove
+00000ac0: 7261 6765 222f 3e0a 2020 2020 3c2f 613e  rage"/>.    </a>
+00000ad0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000ae0: 7470 733a 2f2f 636f 7665 7261 6765 2d62  tps://coverage-b
+00000af0: 6164 6765 2e73 616d 7565 6c63 6f6c 7669  adge.samuelcolvi
+00000b00: 6e2e 776f 726b 6572 732e 6465 762f 7265  n.workers.dev/re
+00000b10: 6469 7265 6374 2f6c 616e 6365 746e 696b  direct/lancetnik
+00000b20: 2f66 6173 7464 6570 656e 6473 2220 7461  /fastdepends" ta
+00000b30: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00000b40: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+00000b50: 2268 7474 7073 3a2f 2f63 6f76 6572 6167  "https://coverag
+00000b60: 652d 6261 6467 652e 7361 6d75 656c 636f  e-badge.samuelco
+00000b70: 6c76 696e 2e77 6f72 6b65 7273 2e64 6576  lvin.workers.dev
+00000b80: 2f6c 616e 6365 746e 696b 2f66 6173 7464  /lancetnik/fastd
+00000b90: 6570 656e 6473 2e73 7667 2220 616c 743d  epends.svg" alt=
+00000ba0: 2243 6f76 6572 6167 6522 3e0a 2020 2020  "Coverage">.    
+00000bb0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000bc0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000bd0: 7267 2f70 726f 6a65 6374 2f66 6173 742d  rg/project/fast-
+00000be0: 6465 7065 6e64 7322 2074 6172 6765 743d  depends" target=
+00000bf0: 225f 626c 616e 6b22 3e0a 2020 2020 2020  "_blank">.      
+00000c00: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000c10: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000c20: 696f 2f70 7970 692f 762f 6661 7374 2d64  io/pypi/v/fast-d
+00000c30: 6570 656e 6473 3f6c 6162 656c 3d70 7970  epends?label=pyp
+00000c40: 6925 3230 7061 636b 6167 6522 2061 6c74  i%20package" alt
+00000c50: 3d22 5061 636b 6167 6520 7665 7273 696f  ="Package versio
+00000c60: 6e22 3e0a 2020 2020 3c2f 613e 0a20 2020  n">.    </a>.   
+00000c70: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000c80: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
+00000c90: 6563 742f 6661 7374 2d64 6570 656e 6473  ect/fast-depends
+00000ca0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000cb0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+00000cc0: 7372 633d 2268 7474 7073 3a2f 2f73 7461  src="https://sta
+00000cd0: 7469 632e 7065 7079 2e74 6563 682f 7065  tic.pepy.tech/pe
+00000ce0: 7273 6f6e 616c 697a 6564 2d62 6164 6765  rsonalized-badge
+00000cf0: 2f66 6173 742d 6465 7065 6e64 733f 7065  /fast-depends?pe
+00000d00: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
+00000d10: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
+00000d20: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
+00000d30: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+00000d40: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+00000d50: 3d44 6f77 6e6c 6f61 6473 2220 616c 743d  =Downloads" alt=
+00000d60: 2264 6f77 6e6c 6f61 6473 222f 3e0a 2020  "downloads"/>.  
+00000d70: 2020 3c2f 613e 0a20 2020 203c 6272 2f3e    </a>.    <br/>
+00000d80: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000d90: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000da0: 726f 6a65 6374 2f66 6173 742d 6465 7065  roject/fast-depe
+00000db0: 6e64 2220 7461 7267 6574 3d22 5f62 6c61  nd" target="_bla
+00000dc0: 6e6b 223e 0a20 2020 2020 2020 203c 696d  nk">.        <im
+00000dd0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000de0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000df0: 7069 2f70 7976 6572 7369 6f6e 732f 6661  pi/pyversions/fa
+00000e00: 7374 2d64 6570 656e 6473 2e73 7667 2220  st-depends.svg" 
+00000e10: 616c 743d 2253 7570 706f 7274 6564 2050  alt="Supported P
+00000e20: 7974 686f 6e20 7665 7273 696f 6e73 223e  ython versions">
+00000e30: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+00000e40: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000e50: 6974 6875 622e 636f 6d2f 4c61 6e63 6574  ithub.com/Lancet
+00000e60: 6e69 6b2f 4661 7374 4465 7065 6e64 732f  nik/FastDepends/
+00000e70: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000e80: 4522 2074 6172 6765 743d 225f 626c 616e  E" target="_blan
+00000e90: 6b22 3e0a 2020 2020 2020 2020 3c69 6d67  k">.        <img
+00000ea0: 2061 6c74 3d22 4769 7448 7562 2220 7372   alt="GitHub" sr
+00000eb0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000ec0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000ed0: 2f6c 6963 656e 7365 2f4c 616e 6365 746e  /license/Lancetn
+00000ee0: 696b 2f46 6173 7444 6570 656e 6473 3f63  ik/FastDepends?c
+00000ef0: 6f6c 6f72 3d25 3233 3030 3765 6336 223e  olor=%23007ec6">
+00000f00: 0a20 2020 203c 2f61 3e0a 3c2f 703e 0a0a  .    </a>.</p>..
+00000f10: 2d2d 2d0a 0a44 6f63 756d 656e 7461 7469  ---..Documentati
+00000f20: 6f6e 3a20 6874 7470 733a 2f2f 6c61 6e63  on: https://lanc
+00000f30: 6574 6e69 6b2e 6769 7468 7562 2e69 6f2f  etnik.github.io/
+00000f40: 4661 7374 4465 7065 6e64 732f 0a0a 2d2d  FastDepends/..--
+00000f50: 2d0a 0a46 6173 7444 6570 656e 6473 202d  -..FastDepends -
+00000f60: 2046 6173 7441 5049 2044 6570 656e 6465   FastAPI Depende
+00000f70: 6e63 7920 496e 6a65 6374 696f 6e20 7379  ncy Injection sy
+00000f80: 7374 656d 2065 7874 7261 6374 6564 2066  stem extracted f
+00000f90: 726f 6d20 4661 7374 4150 4920 616e 6420  rom FastAPI and 
+00000fa0: 636c 6561 7265 6420 6f66 2061 6c6c 2048  cleared of all H
+00000fb0: 5454 5020 6c6f 6769 632e 0a54 6869 7320  TTP logic..This 
+00000fc0: 6973 2061 2073 6d61 6c6c 206c 6962 7261  is a small libra
+00000fd0: 7279 2077 6869 6368 2070 726f 7669 6465  ry which provide
+00000fe0: 7320 796f 7520 7769 7468 2074 6865 2061  s you with the a
+00000ff0: 6269 6c69 7479 2074 6f20 7573 6520 6c6f  bility to use lo
+00001000: 7665 6c79 2046 6173 7461 7069 2069 6e74  vely Fastapi int
+00001010: 6572 6661 6365 7320 696e 2079 6f75 7220  erfaces in your 
+00001020: 6f77 6e0a 7072 6f6a 6563 7473 206f 7220  own.projects or 
+00001030: 746f 6f6c 732e 0a0a 5468 616e 6b73 2074  tools...Thanks t
+00001040: 6f20 5b2a 6661 7374 6170 692a 5d28 6874  o [*fastapi*](ht
+00001050: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
+00001060: 616e 676f 6c6f 2e63 6f6d 2f29 2061 6e64  angolo.com/) and
+00001070: 205b 2a70 7964 616e 7469 632a 5d28 6874   [*pydantic*](ht
+00001080: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
+00001090: 7469 632e 6465 762f 2920 7072 6f6a 6563  tic.dev/) projec
+000010a0: 7473 2066 6f72 2074 6869 730a 6772 6561  ts for this.grea
+000010b0: 7465 2066 756e 6374 696f 6e61 6c69 7479  te functionality
+000010c0: 2e20 5468 6973 2070 6163 6b61 6765 2069  . This package i
+000010d0: 7320 6a75 7374 2061 2073 6d61 6c6c 2063  s just a small c
+000010e0: 6861 6e67 6520 6f66 2074 6865 206f 7269  hange of the ori
+000010f0: 6769 6e61 6c20 4661 7374 6170 6920 736f  ginal Fastapi so
+00001100: 7572 6365 7320 746f 2070 726f 7669 6465  urces to provide
+00001110: 2044 4920 6675 6e63 7469 6f6e 616c 6974   DI functionalit
+00001120: 7920 696e 2061 2070 7972 652d 5079 7468  y in a pyre-Pyth
+00001130: 6f6e 2077 6179 2e0a 0a41 7379 6e63 2061  on way...Async a
+00001140: 6e64 2073 796e 6320 6d6f 6465 7320 6172  nd sync modes ar
+00001150: 6520 626f 7468 2073 7570 706f 7274 6564  e both supported
+00001160: 2e0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00001170: 6f6e 0a0a 6060 6062 6173 680a 7069 7020  on..```bash.pip 
+00001180: 696e 7374 616c 6c20 6661 7374 2d64 6570  install fast-dep
+00001190: 656e 6473 0a60 6060 0a0a 2323 2055 7361  ends.```..## Usa
+000011a0: 6765 0a0a 5468 6572 6520 6973 206e 6f20  ge..There is no 
+000011b0: 7761 7920 746f 206d 616b 6520 4465 7065  way to make Depe
+000011c0: 6e64 656e 6379 2049 6e6a 6563 7469 6f6e  ndency Injection
+000011d0: 2065 6173 6965 720a 0a59 6f75 2063 616e   easier..You can
+000011e0: 2075 7365 2074 6869 7320 6c69 6272 6172   use this librar
+000011f0: 7920 7769 7468 6f75 7420 616e 7920 6672  y without any fr
+00001200: 616d 6577 6f72 6b73 2069 6e20 626f 7468  ameworks in both
+00001210: 202a 2a73 796e 632a 2a20 616e 6420 2a2a   **sync** and **
+00001220: 6173 796e 632a 2a20 636f 6465 2e0a 0a23  async** code...#
+00001230: 2323 2041 7379 6e63 2063 6f64 650a 6060  ## Async code.``
+00001240: 6070 7974 686f 6e0a 696d 706f 7274 2061  `python.import a
+00001250: 7379 6e63 696f 0a0a 6672 6f6d 2066 6173  syncio..from fas
+00001260: 745f 6465 7065 6e64 7320 696d 706f 7274  t_depends import
+00001270: 2069 6e6a 6563 742c 2044 6570 656e 6473   inject, Depends
+00001280: 0a0a 6173 796e 6320 6465 6620 6465 7065  ..async def depe
+00001290: 6e64 656e 6379 2861 3a20 696e 7429 202d  ndency(a: int) -
+000012a0: 3e20 696e 743a 0a20 2020 2072 6574 7572  > int:.    retur
+000012b0: 6e20 610a 0a40 696e 6a65 6374 0a61 7379  n a..@inject.asy
+000012c0: 6e63 2064 6566 206d 6169 6e28 0a20 2020  nc def main(.   
+000012d0: 2061 3a20 696e 742c 0a20 2020 2062 3a20   a: int,.    b: 
+000012e0: 696e 742c 0a20 2020 2063 3a20 696e 7420  int,.    c: int 
+000012f0: 3d20 4465 7065 6e64 7328 6465 7065 6e64  = Depends(depend
+00001300: 656e 6379 290a 2920 2d3e 2066 6c6f 6174  ency).) -> float
+00001310: 3a0a 2020 2020 7265 7475 726e 2061 202b  :.    return a +
+00001320: 2062 202b 2063 0a0a 6173 7365 7274 2061   b + c..assert a
+00001330: 7379 6e63 696f 2e72 756e 286d 6169 6e28  syncio.run(main(
+00001340: 2231 222c 2032 2929 203d 3d20 342e 300a  "1", 2)) == 4.0.
+00001350: 6060 600a 0a23 2323 2053 796e 6320 636f  ```..### Sync co
+00001360: 6465 0a60 6060 7079 7468 6f6e 0a66 726f  de.```python.fro
+00001370: 6d20 6661 7374 5f64 6570 656e 6473 2069  m fast_depends i
+00001380: 6d70 6f72 7420 696e 6a65 6374 2c20 4465  mport inject, De
+00001390: 7065 6e64 730a 0a64 6566 2064 6570 656e  pends..def depen
+000013a0: 6465 6e63 7928 613a 2069 6e74 2920 2d3e  dency(a: int) ->
+000013b0: 2069 6e74 3a0a 2020 2020 7265 7475 726e   int:.    return
+000013c0: 2061 0a0a 4069 6e6a 6563 740a 6465 6620   a..@inject.def 
+000013d0: 6d61 696e 280a 2020 2020 613a 2069 6e74  main(.    a: int
+000013e0: 2c0a 2020 2020 623a 2069 6e74 2c0a 2020  ,.    b: int,.  
+000013f0: 2020 633a 2069 6e74 203d 2044 6570 656e    c: int = Depen
+00001400: 6473 2864 6570 656e 6465 6e63 7929 0a29  ds(dependency).)
+00001410: 202d 3e20 666c 6f61 743a 0a20 2020 2072   -> float:.    r
+00001420: 6574 7572 6e20 6120 2b20 6220 2b20 630a  eturn a + b + c.
+00001430: 0a61 7373 6572 7420 6d61 696e 2822 3122  .assert main("1"
+00001440: 2c20 3229 203d 3d20 342e 300a 6060 600a  , 2) == 4.0.```.
+00001450: 0a60 4069 6e6a 6563 7460 2064 6563 6f72  .`@inject` decor
+00001460: 6174 6f72 2070 6c61 7973 206d 756c 7469  ator plays multi
+00001470: 706c 6520 726f 6c65 7320 6174 2074 6865  ple roles at the
+00001480: 2073 616d 6520 7469 6d65 3a0a 0a2a 2072   same time:..* r
+00001490: 6573 6f6c 7665 202a 4465 7065 6e64 732a  esolve *Depends*
+000014a0: 2063 6c61 7373 6573 0a2a 2063 6173 7420   classes.* cast 
+000014b0: 7479 7065 7320 6163 636f 7264 696e 6720  types according 
+000014c0: 746f 2050 7974 686f 6e20 616e 6e6f 7461  to Python annota
+000014d0: 7469 6f6e 0a2a 2076 616c 6964 6174 6520  tion.* validate 
+000014e0: 696e 636f 6d69 6e67 2070 6172 616d 6574  incoming paramet
+000014f0: 6572 7320 7573 696e 6720 2a70 7964 616e  ers using *pydan
+00001500: 7469 632a 0a0a 2d2d 2d0a 0a23 2323 2046  tic*..---..### F
+00001510: 6561 7475 7265 730a 0a53 796e 6368 726f  eatures..Synchro
+00001520: 6e6f 7573 2063 6f64 6520 6973 2066 756c  nous code is ful
+00001530: 6c79 2073 7570 706f 7274 6564 2069 6e20  ly supported in 
+00001540: 7468 6973 2070 6163 6b61 6765 3a20 7769  this package: wi
+00001550: 7468 6f75 7420 616e 7920 6061 7379 6e63  thout any `async
+00001560: 5f74 6f5f 7379 6e63 602c 2060 7275 6e5f  _to_sync`, `run_
+00001570: 7379 6e63 602c 2060 7379 6e63 6966 7960  sync`, `syncify`
+00001580: 206f 7220 616e 7920 6f74 6865 7220 7472   or any other tr
+00001590: 6963 6b73 2e0a 0a41 6c73 6f2c 202a 4661  icks...Also, *Fa
+000015a0: 7374 4465 7065 6e64 732a 2063 6173 7473  stDepends* casts
+000015b0: 2066 756e 6374 696f 6e73 2720 7265 7475   functions' retu
+000015c0: 726e 2076 616c 7565 7320 7468 6520 7361  rn values the sa
+000015d0: 6d65 2077 6179 2c20 6974 2063 616e 2062  me way, it can b
+000015e0: 6520 7665 7279 2068 656c 7066 756c 2069  e very helpful i
+000015f0: 6e20 6275 696c 6469 6e67 2079 6f75 7220  n building your 
+00001600: 6f77 6e20 746f 6f6c 732e 0a0a 5468 6573  own tools...Thes
+00001610: 6520 6172 6520 7477 6f20 6d61 696e 2064  e are two main d
+00001620: 6566 6665 7265 6e63 6573 2066 726f 6d20  efferences from 
+00001630: 6e61 7469 7665 2046 6173 7461 7069 2044  native Fastapi D
+00001640: 4920 5379 7374 656d 2e0a 0a2d 2d2d 0a0a  I System...---..
+00001650: 2323 2320 4375 7374 6f6d 2046 6965 6c64  ### Custom Field
+00001660: 730a 0a49 6620 796f 7520 7769 7368 2074  s..If you wish t
+00001670: 6f20 7772 6974 6520 796f 7572 206f 776e  o write your own
+00001680: 2046 6173 7441 5049 206f 7220 616e 6f74   FastAPI or anot
+00001690: 6865 7220 636c 6f73 656c 7920 6279 2061  her closely by a
+000016a0: 7263 6869 7465 6374 7572 6520 746f 6f6c  rchitecture tool
+000016b0: 2c20 796f 7520 7368 6f75 6c64 2064 6566  , you should def
+000016c0: 696e 6520 796f 7572 206f 776e 2063 7573  ine your own cus
+000016d0: 746f 6d20 6669 656c 6473 2074 6f20 7370  tom fields to sp
+000016e0: 6563 6966 7920 6170 706c 6963 6174 696f  ecify applicatio
+000016f0: 6e20 6265 6861 7669 6f72 2e0a 0a43 7573  n behavior...Cus
+00001700: 746f 6d20 6669 656c 6473 2063 616e 2062  tom fields can b
+00001710: 6520 7573 6564 2074 6f20 6164 6469 6e67  e used to adding
+00001720: 2073 6f6d 6574 6869 6e67 2073 7065 6369   something speci
+00001730: 6669 6320 746f 2061 2066 756e 6374 696f  fic to a functio
+00001740: 6e20 6172 6775 6d65 6e74 7320 286c 696b  n arguments (lik
+00001750: 6520 6120 4261 636b 6772 6f75 6e64 5461  e a BackgroundTa
+00001760: 736b 2920 6f72 2070 6172 7369 6e67 2069  sk) or parsing i
+00001770: 6e63 6f6d 696e 6720 6f62 6a65 6374 7320  ncoming objects 
+00001780: 7370 6563 6961 6c20 7761 792e 2059 6f75  special way. You
+00001790: 2061 626c 6520 6465 6369 6465 2062 7920   able decide by 
+000017a0: 6f77 6e2c 2077 6879 2061 6e64 2068 6f77  own, why and how
+000017b0: 2079 6f75 2077 696c 6c20 7573 6520 7468   you will use th
+000017c0: 6573 6520 746f 6f6c 732e 0a0a 4661 7374  ese tools...Fast
+000017d0: 4465 7065 6e64 7320 6772 616e 7473 2079  Depends grants y
+000017e0: 6f75 2074 6869 7320 6f70 706f 7274 756e  ou this opportun
+000017f0: 6974 7920 6120 7665 7279 2069 6e74 7569  ity a very intui
+00001800: 7469 7665 2061 6e64 2063 6f6d 666f 7274  tive and comfort
+00001810: 6162 6c65 2077 6179 2e0a 0a60 6060 7079  able way...```py
+00001820: 7468 6f6e 0a66 726f 6d20 6661 7374 5f64  thon.from fast_d
+00001830: 6570 656e 6473 2069 6d70 6f72 7420 696e  epends import in
+00001840: 6a65 6374 0a66 726f 6d20 6661 7374 5f64  ject.from fast_d
+00001850: 6570 656e 6473 2e6c 6962 7261 7279 2069  epends.library i
+00001860: 6d70 6f72 7420 4375 7374 6f6d 4669 656c  mport CustomFiel
+00001870: 640a 0a63 6c61 7373 2048 6561 6465 7228  d..class Header(
+00001880: 4375 7374 6f6d 4669 656c 6429 3a0a 2020  CustomField):.  
+00001890: 2020 6465 6620 7573 6528 7365 6c66 2c20    def use(self, 
+000018a0: 2a2a 6b77 6172 6773 3a20 416e 7944 6963  **kwargs: AnyDic
+000018b0: 7429 202d 3e20 416e 7944 6963 743a 0a20  t) -> AnyDict:. 
+000018c0: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+000018d0: 7375 7065 7228 292e 7573 6528 2a2a 6b77  super().use(**kw
+000018e0: 6172 6773 290a 2020 2020 2020 2020 6b77  args).        kw
+000018f0: 6172 6773 5b73 656c 662e 7061 7261 6d5f  args[self.param_
+00001900: 6e61 6d65 5d20 3d20 6b77 6172 6773 5b22  name] = kwargs["
+00001910: 6865 6164 6572 7322 5d5b 7365 6c66 2e70  headers"][self.p
+00001920: 6172 616d 5f6e 616d 655d 0a20 2020 2020  aram_name].     
+00001930: 2020 2072 6574 7572 6e20 6b77 6172 6773     return kwargs
+00001940: 0a0a 4069 6e6a 6563 740a 6465 6620 6d79  ..@inject.def my
+00001950: 5f66 756e 6328 6865 6164 6572 5f66 6965  _func(header_fie
+00001960: 6c64 3a20 696e 7420 3d20 4865 6164 6572  ld: int = Header
+00001970: 2829 293a 0a20 2020 2072 6574 7572 6e20  ()):.    return 
+00001980: 6865 6164 6572 5f66 6965 6c64 0a0a 6173  header_field..as
+00001990: 7365 7274 206d 795f 6675 6e63 280a 2020  sert my_func(.  
+000019a0: 2020 6865 6164 6572 733d 7b20 2268 6561    headers={ "hea
+000019b0: 6465 725f 6669 656c 6422 3a20 2231 2220  der_field": "1" 
+000019c0: 7d0a 2920 3d3d 2031 0a60 6060 0a0a 2d2d  }.) == 1.```..--
+000019d0: 2d0a 0a23 2323 204e 6f74 650a 4c69 6272  -..### Note.Libr
+000019e0: 6172 7920 7761 7320 6261 7365 6420 6f6e  ary was based on
+000019f0: 202a 2a30 2e39 352e 3020 4661 7374 4150   **0.95.0 FastAP
+00001a00: 492a 2a20 7665 7273 696f 6e2e 0a0a 4966  I** version...If
+00001a10: 2077 6520 6172 6520 746f 6f20 6661 7220   we are too far 
+00001a20: 6265 6869 6e64 2c20 706c 6561 7365 2c20  behind, please, 
+00001a30: 636f 6e74 6163 7420 5b6d 655d 286d 6169  contact [me](mai
+00001a40: 6c74 6f3a 6469 656d 656e 7472 6f73 4079  lto:diementros@y
+00001a50: 616e 6465 782e 7275 290a 6f72 2063 6f6e  andex.ru).or con
+00001a60: 7475 6275 7465 2079 6f75 7273 656c 662e  tubute yourself.
+00001a70: 2052 6561 6c6c 7920 6170 7072 6563 6961   Really apprecia
+00001a80: 7465 2079 6f75 7220 6865 6c70 2e0a       te your help..
```

