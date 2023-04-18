# Comparing `tmp/ariadne_codegen-0.5.0.tar.gz` & `tmp/ariadne_codegen-0.6.0.tar.gz`

## Comparing `ariadne_codegen-0.5.0.tar` & `ariadne_codegen-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/EXAMPLE.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/__init__.py
--rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/codegen.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/config.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/exceptions.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/py.typed
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/schema.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/settings.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/arguments.py
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/client.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/constants.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/enums.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/init_file.py
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/input_fields.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/input_types.py
--rw-r--r--   0        0        0    14554 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/package.py
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/result_fields.py
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/result_types.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/scalars.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/async_base_client.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/base_client.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/base_model.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/exceptions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/scalars.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/constants.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/directives.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/fields.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/named_types.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/schema.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/plugins/__init__.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/plugins/base.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/plugins/explorer.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/ariadne_codegen/plugins/manager.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/LICENSE
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/README.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 ariadne_codegen-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/EXAMPLE.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/__init__.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/codegen.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/config.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/exceptions.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/py.typed
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/schema.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/settings.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/__init__.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/arguments.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/client.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/constants.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/enums.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/init_file.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_fields.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_types.py
+-rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/package.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_fields.py
+-rw-r--r--   0        0        0    13819 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_types.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/scalars.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/__init__.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/async_base_client.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_client.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_model.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/exceptions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/scalars.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/constants.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/directives.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/fields.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/named_types.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/schema.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/__init__.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/base.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/explorer.py
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/ariadne_codegen/plugins/manager.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/LICENSE
+-rw-r--r--   0        0        0     9322 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/README.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 ariadne_codegen-0.6.0/PKG-INFO
```

### Comparing `ariadne_codegen-0.5.0/EXAMPLE.md` & `ariadne_codegen-0.6.0/EXAMPLE.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,17 +152,18 @@
 ### Client class
 
 Generated client class inherits from `AsyncBaseClient` and has async method for every provided query/mutation.
 
 ```py
 # graphql_client/client.py
 
-from typing import Optional
+from typing import Optional, Union
 
 from .async_base_client import AsyncBaseClient
+from .base_model import UNSET, UnsetType
 from .create_user import CreateUser
 from .input_types import UserCreateInput
 from .list_all_users import ListAllUsers
 from .list_users_by_country import ListUsersByCountry
 
 
 def gql(q: str) -> str:
@@ -203,15 +204,15 @@
         )
         variables: dict[str, object] = {}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return ListAllUsers.parse_obj(data)
 
     async def list_users_by_country(
-        self, country: Optional[str] = None
+        self, country: Union[Optional[str], UnsetType] = UNSET
     ) -> ListUsersByCountry:
         query = gql(
             """
             query ListUsersByCountry($country: String) {
               users(country: $country) {
                 ...BasicUser
                 ...UserPersonalData
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/codegen.py` & `ariadne_codegen-0.6.0/ariadne_codegen/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name: str, annotation: Optional[Union[ast.Name, ast.Subscript]] = None
 ) -> ast.arg:
     """Generate arg."""
     return ast.arg(arg=name, annotation=annotation)
 
 
 def generate_arguments(
-    args: Optional[List[ast.arg]] = None, defaults: Optional[List[ast.Constant]] = None
+    args: Optional[List[ast.arg]] = None, defaults: Optional[List[ast.expr]] = None
 ) -> ast.arguments:
     """Generate arguments."""
     return ast.arguments(
         posonlyargs=[],
         args=args if args else [],
         kwonlyargs=[],
         kw_defaults=[],
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/config.py` & `ariadne_codegen-0.6.0/ariadne_codegen/config.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/exceptions.py` & `ariadne_codegen-0.6.0/ariadne_codegen/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/main.py` & `ariadne_codegen-0.6.0/ariadne_codegen/main.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/schema.py` & `ariadne_codegen-0.6.0/ariadne_codegen/schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/settings.py` & `ariadne_codegen-0.6.0/ariadne_codegen/settings.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/utils.py` & `ariadne_codegen-0.6.0/ariadne_codegen/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import ast
 import re
+from keyword import iskeyword
 from textwrap import indent
+from typing import Optional
 
 import isort
 from autoflake import fix_code  # type: ignore
 from black import Mode, format_str
+from graphql import Node
+
+from .plugins.manager import PluginManager
 
 
 def ast_to_str(
     ast_obj: ast.AST,
     remove_unused_imports: bool = True,
     multiline_strings: bool = False,
 ) -> str:
@@ -66,7 +71,25 @@
         variable_indent_size = get_variable_indent_size(line)
         orginal_str_match = re.search("'.*'", line)
         if orginal_str_match:
             orginal_str = orginal_str_match.group()
             formatted = convert_to_multiline_string(orginal_str, variable_indent_size)
             formatted_source = formatted_source.replace(orginal_str, formatted)
     return formatted_source
+
+
+def process_name(
+    name: str,
+    convert_to_snake_case: bool,
+    plugin_manager: Optional[PluginManager] = None,
+    node: Optional[Node] = None,
+) -> str:
+    """Processes the GraphQL name to remove keywords
+    and optionally convert to snake_case."""
+    processed_name = name
+    if convert_to_snake_case:
+        processed_name = str_to_snake_case(processed_name)
+    if iskeyword(processed_name):
+        processed_name += "_"
+    if plugin_manager:
+        processed_name = plugin_manager.process_name(processed_name, node=node)
+    return processed_name
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/arguments.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/arguments.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ast
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union, cast
 
 from graphql import (
     GraphQLEnumType,
     GraphQLInputObjectType,
     GraphQLScalarType,
     GraphQLSchema,
     ListTypeNode,
@@ -18,19 +18,20 @@
     generate_arg,
     generate_arguments,
     generate_call,
     generate_constant,
     generate_dict,
     generate_list_annotation,
     generate_name,
+    generate_union_annotation,
 )
 from ..exceptions import ParsingError
 from ..plugins.manager import PluginManager
-from ..utils import str_to_snake_case
-from .constants import ANY, OPTIONAL, SIMPLE_TYPE_MAP
+from ..utils import process_name
+from .constants import ANY, OPTIONAL, SIMPLE_TYPE_MAP, UNSET_NAME, UNSET_TYPE_NAME
 from .scalars import ScalarData
 
 
 class ArgumentsGenerator:
     def __init__(
         self,
         schema: GraphQLSchema,
@@ -53,31 +54,39 @@
     ) -> Tuple[ast.arguments, ast.Dict]:
         """Generate arguments from given variable definitions."""
         required_args: List[ast.arg] = [generate_arg("self")]
         optional_args: List[ast.arg] = []
         dict_ = generate_dict()
         for variable_definition in variable_definitions:
             org_name = variable_definition.variable.name.value
-            name = self._process_name(org_name)
+            name = process_name(
+                org_name,
+                convert_to_snake_case=self.convert_to_snake_case,
+                plugin_manager=self.plugin_manager,
+                node=variable_definition,
+            )
             annotation, used_custom_scalar = self._parse_type_node(
                 variable_definition.type
             )
 
             arg = generate_arg(name, annotation)
-            if self.is_nullable(annotation):
+            if self._is_nullable(annotation):
+                arg.annotation = self._process_optional_arg_annotation(
+                    cast(ast.Subscript, annotation)
+                )
                 optional_args.append(arg)
             else:
                 required_args.append(arg)
 
             dict_.keys.append(generate_constant(org_name))
             dict_.values.append(self._get_dict_value(name, used_custom_scalar))
 
         arguments = generate_arguments(
             args=required_args + optional_args,
-            defaults=[generate_constant(None) for _ in optional_args],
+            defaults=[generate_name(UNSET_NAME) for _ in optional_args],
         )
 
         if self.plugin_manager:
             arguments = self.plugin_manager.generate_arguments(
                 arguments, variable_definitions=variable_definitions
             )
             dict_ = self.plugin_manager.generate_arguments_dict(
@@ -90,19 +99,14 @@
 
     def get_used_inputs(self) -> List[str]:
         return self._used_inputs
 
     def get_used_custom_scalars(self) -> List[str]:
         return self._used_custom_scalars
 
-    def _process_name(self, name: str) -> str:
-        if self.convert_to_snake_case:
-            return str_to_snake_case(name)
-        return name
-
     def _parse_type_node(
         self,
         node: Union[NamedTypeNode, ListTypeNode, NonNullTypeNode, TypeNode],
         nullable: bool = True,
     ) -> Tuple[Union[ast.Name, ast.Subscript], Optional[str]]:
         if isinstance(node, NamedTypeNode):
             return self._parse_named_type_node(node, nullable)
@@ -135,33 +139,40 @@
         elif isinstance(type_, GraphQLEnumType):
             self._used_enums.append(name)
         elif isinstance(type_, GraphQLScalarType):
             if name not in self.custom_scalars:
                 name = SIMPLE_TYPE_MAP.get(name, ANY)
             else:
                 used_custom_scalar = name
-                name = self.custom_scalars[name].type_
+                name = self.custom_scalars[name].type_name
         else:
             raise ParsingError(f"Incorrect argument type {name}")
 
         return generate_annotation_name(name, nullable), used_custom_scalar
 
-    def is_nullable(self, annotation: Union[ast.Name, ast.Subscript]) -> bool:
+    def _is_nullable(self, annotation: Union[ast.Name, ast.Subscript]) -> bool:
         return (
             isinstance(annotation, ast.Subscript)
             and isinstance(annotation.value, ast.Name)
             and annotation.value.id == OPTIONAL
         )
 
+    def _process_optional_arg_annotation(
+        self, annotation: ast.Subscript
+    ) -> ast.Subscript:
+        return generate_union_annotation(
+            types=[annotation, generate_name(UNSET_TYPE_NAME)], nullable=False
+        )
+
     def _get_dict_value(
         self, name: str, used_custom_scalar: Optional[str]
     ) -> Union[ast.Name, ast.Call]:
         if used_custom_scalar:
             self._used_custom_scalars.append(used_custom_scalar)
             scalar_data = self.custom_scalars[used_custom_scalar]
-            if scalar_data.serialize:
+            if scalar_data.serialize_name:
                 return generate_call(
-                    func=generate_name(scalar_data.serialize),
+                    func=generate_name(scalar_data.serialize_name),
                     args=[generate_name(name)],
                 )
 
         return generate_name(name)
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/client.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import ast
-from typing import List, Optional, Union, cast
+from typing import Dict, List, Optional, Union, cast
+
+from graphql import OperationDefinitionNode
 
 from ..codegen import (
     generate_ann_assign,
     generate_arg,
     generate_arguments,
     generate_assign,
     generate_async_method_definition,
@@ -18,76 +20,105 @@
     generate_module,
     generate_name,
     generate_return,
     generate_subscript,
     generate_tuple,
 )
 from ..plugins.manager import PluginManager
-from .constants import ANY, LIST, OPTIONAL, TYPING_MODULE
+from .arguments import ArgumentsGenerator
+from .constants import ANY, LIST, OPTIONAL, TYPING_MODULE, UNION
+from .scalars import ScalarData, generate_scalar_imports
 
 
 class ClientGenerator:
     def __init__(
         self,
         name: str,
         base_client: str,
+        enums_module_name: str,
+        input_types_module_name: str,
+        arguments_generator: ArgumentsGenerator,
+        base_client_import: Optional[ast.ImportFrom] = None,
+        unset_import: Optional[ast.ImportFrom] = None,
+        custom_scalars: Optional[Dict[str, ScalarData]] = None,
         plugin_manager: Optional[PluginManager] = None,
     ) -> None:
         self.name = name
+        self.enums_module_name = enums_module_name
+        self.input_types_module_name = input_types_module_name
         self.plugin_manager = plugin_manager
-        self.class_def = generate_class_def(name=name, base_names=[base_client])
-        self.imports: list = [
-            generate_import_from([OPTIONAL, LIST, ANY], TYPING_MODULE)
-        ]
+        self.custom_scalars = custom_scalars if custom_scalars else {}
+        self.arguments_generator = arguments_generator
+
+        self._imports: List[ast.ImportFrom] = []
+        self._add_import(
+            generate_import_from([OPTIONAL, LIST, ANY, UNION], TYPING_MODULE)
+        )
+        self._add_import(base_client_import)
+        self._add_import(unset_import)
 
+        self._class_def = generate_class_def(name=name, base_names=[base_client])
         self._gql_func_name = "gql"
         self._operation_str_variable = "query"
         self._variables_dict_variable = "variables"
         self._response_variable = "response"
         self._data_variable = "data"
 
     def generate(self) -> ast.Module:
         """Generate module with class definition of graphql client."""
+        self._add_import(
+            generate_import_from(
+                names=self.arguments_generator.get_used_inputs(),
+                from_=self.input_types_module_name,
+                level=1,
+            )
+        )
+        self._add_import(
+            generate_import_from(
+                names=self.arguments_generator.get_used_enums(),
+                from_=self.enums_module_name,
+                level=1,
+            )
+        )
+        for custom_scalar_name in self.arguments_generator.get_used_custom_scalars():
+            scalar_data = self.custom_scalars[custom_scalar_name]
+            for import_ in generate_scalar_imports(scalar_data):
+                self._add_import(import_)
+
         gql_func = self._generate_gql_func()
-        gql_func.lineno = len(self.imports) + 1
+        gql_func.lineno = len(self._imports) + 1
         if self.plugin_manager:
             gql_func = self.plugin_manager.generate_gql_function(gql_func)
 
-        self.class_def.lineno = len(self.imports) + 3
-        if not self.class_def.body:
-            self.class_def.body.append(ast.Pass())
+        self._class_def.lineno = len(self._imports) + 3
+        if not self._class_def.body:
+            self._class_def.body.append(ast.Pass())
         if self.plugin_manager:
-            self.class_def = self.plugin_manager.generate_client_class(self.class_def)
+            self._class_def = self.plugin_manager.generate_client_class(self._class_def)
 
         module = generate_module(
-            body=self.imports + [gql_func, self.class_def],
+            body=self._imports + [gql_func, self._class_def],
         )
         if self.plugin_manager:
             module = self.plugin_manager.generate_client_module(module)
         return module
 
-    def add_import(self, names: List[str], from_: str, level: int = 0) -> None:
-        """Add import to be included in module file."""
-        if not names:
-            return
-        import_ = generate_import_from(names=names, from_=from_, level=level)
-        if self.plugin_manager:
-            import_ = self.plugin_manager.generate_client_import(import_)
-        self.imports.append(import_)
-
     def add_method(
         self,
+        definition: OperationDefinitionNode,
         name: str,
         return_type: str,
-        arguments: ast.arguments,
-        arguments_dict: ast.Dict,
+        return_type_module: str,
         operation_str: str,
         async_: bool = True,
     ):
         """Add method to client."""
+        arguments, arguments_dict = self.arguments_generator.generate(
+            definition.variable_definitions
+        )
         method_def = (
             self._generate_async_method(
                 name=name,
                 return_type=return_type,
                 arguments=arguments,
                 arguments_dict=arguments_dict,
                 operation_str=operation_str,
@@ -97,20 +128,31 @@
                 name=name,
                 return_type=return_type,
                 arguments=arguments,
                 arguments_dict=arguments_dict,
                 operation_str=operation_str,
             )
         )
-        method_def.lineno = len(self.class_def.body) + 1
+        method_def.lineno = len(self._class_def.body) + 1
         if self.plugin_manager:
             method_def = self.plugin_manager.generate_client_method(
                 cast(Union[ast.FunctionDef, ast.AsyncFunctionDef], method_def)
             )
-        self.class_def.body.append(method_def)
+        self._class_def.body.append(method_def)
+        self._add_import(
+            generate_import_from(names=[return_type], from_=return_type_module, level=1)
+        )
+
+    def _add_import(self, import_: Optional[ast.ImportFrom] = None):
+        if not import_:
+            return
+        if self.plugin_manager:
+            import_ = self.plugin_manager.generate_client_import(import_)
+        if import_.names and import_.module:
+            self._imports.append(import_)
 
     def _generate_async_method(
         self,
         name: str,
         return_type: str,
         arguments: ast.arguments,
         arguments_dict: ast.Dict,
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/constants.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,7 +48,10 @@
     "GraphQlClientInvalidResponseError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
 ]
 
 SCALARS_PARSE_DICT_NAME = "SCALARS_PARSE_FUNCTIONS"
 SCALARS_SERIALIZE_DICT_NAME = "SCALARS_SERIALIZE_FUNCTIONS"
+
+UNSET_NAME = "UNSET"
+UNSET_TYPE_NAME = "UnsetType"
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/enums.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/enums.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/init_file.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/init_file.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/input_fields.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 ),
                 "",
             )
 
         if custom_scalars and type_.name in custom_scalars:
             return (
                 generate_annotation_name(
-                    name=custom_scalars[type_.name].type_, nullable=nullable
+                    name=custom_scalars[type_.name].type_name, nullable=nullable
                 ),
                 type_.name,
             )
 
         return generate_annotation_name(name=ANY, nullable=nullable), ""
 
     if isinstance(type_, GraphQLInputObjectType):
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/input_types.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/input_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     generate_field_with_alias,
     generate_import_from,
     generate_keyword,
     generate_method_call,
     generate_module,
 )
 from ..plugins.manager import PluginManager
-from ..utils import str_to_snake_case
+from ..utils import process_name
 from .constants import (
     ANY,
     BASE_MODEL_CLASS_NAME,
     FIELD_CLASS,
     LIST,
     OPTIONAL,
     PYDANTIC_MODULE,
     TYPING_MODULE,
     UNION,
     UPDATE_FORWARD_REFS_METHOD,
 )
 from .input_fields import parse_input_field_default_value, parse_input_field_type
-from .scalars import ScalarData
+from .scalars import ScalarData, generate_scalar_imports
 
 
 class InputTypesGenerator:
     def __init__(
         self,
         schema: GraphQLSchema,
         enums_module: str,
@@ -70,20 +70,16 @@
             self._imports.append(
                 generate_import_from(self._used_enums, self.enums_module, 1)
             )
 
         if self._used_scalars:
             for scalar_name in self._used_scalars:
                 scalar_data = self.custom_scalars[scalar_name]
-                if scalar_data.import_ and scalar_data.names_to_import:
-                    self._imports.append(
-                        generate_import_from(
-                            names=scalar_data.names_to_import, from_=scalar_data.import_
-                        )
-                    )
+                self._imports.extend(generate_scalar_imports(scalar_data))
+
         update_forward_refs_calls = [
             generate_expr(generate_method_call(c.name, UPDATE_FORWARD_REFS_METHOD))
             for c in self._class_defs
         ]
         module_body = (
             cast(List[ast.stmt], self._imports)
             + cast(List[ast.stmt], self._class_defs)
@@ -109,15 +105,20 @@
         self, definition: GraphQLInputObjectType
     ) -> ast.ClassDef:
         class_def = generate_class_def(
             name=definition.name, base_names=[BASE_MODEL_CLASS_NAME]
         )
 
         for lineno, (org_name, field) in enumerate(definition.fields.items(), start=1):
-            name = self._process_field_name(org_name)
+            name = process_name(
+                org_name,
+                convert_to_snake_case=self.convert_to_snake_case,
+                plugin_manager=self.plugin_manager,
+                node=field,
+            )
             annotation, field_type = parse_input_field_type(
                 field.type, custom_scalars=self.custom_scalars
             )
             field_implementation = generate_ann_assign(
                 target=name,
                 annotation=annotation,
                 value=parse_input_field_default_value(
@@ -140,19 +141,14 @@
         if self.plugin_manager:
             class_def = self.plugin_manager.generate_input_class(
                 class_def, input_type=definition
             )
 
         return class_def
 
-    def _process_field_name(self, name: str) -> str:
-        if self.convert_to_snake_case:
-            return str_to_snake_case(name)
-        return name
-
     def _process_field_value(
         self,
         field_implementation: ast.AnnAssign,
         alias: str,
     ) -> ast.Call:
         field_with_alias = generate_field_with_alias(alias)
         if field_implementation.value:
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/package.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/package.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from typing import Dict, List, Optional
 
 from graphql import FragmentDefinitionNode, GraphQLSchema, OperationDefinitionNode
 
 from ..codegen import generate_import_from
 from ..exceptions import ParsingError
 from ..plugins.manager import PluginManager
-from ..utils import ast_to_str, str_to_pascal_case, str_to_snake_case
+from ..utils import ast_to_str, process_name, str_to_pascal_case
 from .arguments import ArgumentsGenerator
 from .client import ClientGenerator
 from .constants import (
     BASE_MODEL_CLASS_NAME,
     COMMENT_DATETIME_FORMAT,
     DEFAULT_ASYNC_BASE_CLIENT_PATH,
     DEFAULT_BASE_CLIENT_PATH,
     GRAPHQL_CLIENT_EXCEPTIONS_NAMES,
     SOURCE_COMMENT,
     TIMESTAMP_COMMENT,
+    UNSET_NAME,
+    UNSET_TYPE_NAME,
 )
 from .enums import EnumsGenerator
 from .init_file import InitFileGenerator
 from .input_types import InputTypesGenerator
 from .result_types import ResultTypesGenerator
 from .scalars import ScalarData, ScalarsDefinitionsGenerator
 
@@ -43,15 +45,14 @@
         queries_source: str = "",
         schema_source: str = "",
         convert_to_snake_case: bool = True,
         async_client: bool = True,
         fragments: Optional[List[FragmentDefinitionNode]] = None,
         init_generator: Optional[InitFileGenerator] = None,
         client_generator: Optional[ClientGenerator] = None,
-        arguments_generator: Optional[ArgumentsGenerator] = None,
         enums_generator: Optional[EnumsGenerator] = None,
         input_types_generator: Optional[InputTypesGenerator] = None,
         files_to_include: Optional[List[str]] = None,
         custom_scalars: Optional[Dict[str, ScalarData]] = None,
         plugin_manager: Optional[PluginManager] = None,
     ) -> None:
         self.package_name = package_name
@@ -66,14 +67,17 @@
 
         self.base_model_file_path = (
             Path(__file__).parent / "dependencies" / "base_model.py"
         )
         self.base_model_import = generate_import_from(
             [BASE_MODEL_CLASS_NAME], self.base_model_file_path.stem, 1
         )
+        self.unset_import = generate_import_from(
+            [UNSET_NAME, UNSET_TYPE_NAME], self.base_model_file_path.stem, 1
+        )
         self.exceptions_file_path = (
             Path(__file__).parent / "dependencies" / "exceptions.py"
         )
 
         self.files_to_include = (
             [Path(f) for f in files_to_include] if files_to_include else []
         )
@@ -84,34 +88,47 @@
 
         self.include_comments = include_comments
         self.queries_source = queries_source
         self.schema_source = schema_source
         self.convert_to_snake_case = convert_to_snake_case
         self.async_client = async_client
 
+        if base_client_file_path:
+            self.base_client_file_path = Path(base_client_file_path)
+        else:
+            if self.async_client:
+                self.base_client_file_path = DEFAULT_ASYNC_BASE_CLIENT_PATH
+            else:
+                self.base_client_file_path = DEFAULT_BASE_CLIENT_PATH
+
         self.init_generator = (
             init_generator
             if init_generator
             else InitFileGenerator(plugin_manager=self.plugin_manager)
         )
         self.client_generator = (
             client_generator
             if client_generator
             else ClientGenerator(
                 name=self.client_name,
                 base_client=self.base_client_name,
-                plugin_manager=self.plugin_manager,
-            )
-        )
-        self.arguments_generator = (
-            arguments_generator
-            if arguments_generator
-            else ArgumentsGenerator(
-                schema=self.schema,
-                convert_to_snake_case=self.convert_to_snake_case,
+                enums_module_name=self.enums_module_name,
+                input_types_module_name=self.input_types_module_name,
+                arguments_generator=ArgumentsGenerator(
+                    schema=self.schema,
+                    convert_to_snake_case=self.convert_to_snake_case,
+                    custom_scalars=self.custom_scalars,
+                    plugin_manager=self.plugin_manager,
+                ),
+                base_client_import=generate_import_from(
+                    names=[self.base_client_name],
+                    from_=self.base_client_file_path.stem,
+                    level=1,
+                ),
+                unset_import=self.unset_import,
                 custom_scalars=self.custom_scalars,
                 plugin_manager=self.plugin_manager,
             )
         )
         self.input_types_generator = (
             input_types_generator
             if input_types_generator
@@ -126,22 +143,14 @@
         )
         self.enums_generator = (
             enums_generator
             if enums_generator
             else EnumsGenerator(schema=self.schema, plugin_manager=self.plugin_manager)
         )
 
-        if base_client_file_path:
-            self.base_client_file_path = Path(base_client_file_path)
-        else:
-            if self.async_client:
-                self.base_client_file_path = DEFAULT_ASYNC_BASE_CLIENT_PATH
-            else:
-                self.base_client_file_path = DEFAULT_BASE_CLIENT_PATH
-
         self.fragments_definitions = {f.name.value: f for f in fragments or []}
 
         self.result_types_files: Dict[str, ast.Module] = {}
         self.generated_files: List[str] = []
         self.include_exceptions_file = self._include_exceptions()
 
         self.scalars_definitions_generator = ScalarsDefinitionsGenerator(
@@ -167,15 +176,20 @@
 
     def add_operation(self, definition: OperationDefinitionNode):
         name = definition.name
         if not name:
             raise ParsingError("Query without name.")
 
         return_type_name = str_to_pascal_case(name.value)
-        method_name = str_to_snake_case(name.value)
+        method_name = process_name(
+            name.value,
+            convert_to_snake_case=True,
+            plugin_manager=self.plugin_manager,
+            node=definition,
+        )
         module_name = method_name
         file_name = f"{module_name}.py"
 
         query_types_generator = ResultTypesGenerator(
             schema=self.schema,
             operation_definition=definition,
             enums_module_name=self.enums_module_name,
@@ -187,26 +201,22 @@
         )
         self.result_types_files[file_name] = query_types_generator.generate()
         operation_str = query_types_generator.get_operation_as_str()
         self.init_generator.add_import(
             query_types_generator.get_generated_public_names(), module_name, 1
         )
 
-        arguments, arguments_dict = self.arguments_generator.generate(
-            definition.variable_definitions
-        )
         self.client_generator.add_method(
+            definition=definition,
             name=method_name,
             return_type=return_type_name,
-            arguments=arguments,
-            arguments_dict=arguments_dict,
+            return_type_module=module_name,
             operation_str=operation_str,
             async_=self.async_client,
         )
-        self.client_generator.add_import([return_type_name], module_name, 1)
 
     def _include_exceptions(self):
         return self.base_client_file_path in (
             DEFAULT_ASYNC_BASE_CLIENT_PATH,
             DEFAULT_BASE_CLIENT_PATH,
         )
 
@@ -229,39 +239,14 @@
         if len(file_names) != len(set(file_names)):
             seen = set()
             duplicated_files = {n for n in file_names if n in seen or seen.add(n)}
             raise ParsingError(f"Duplicated file names: {',' .join(duplicated_files)}")
 
     def _generate_client(self):
         client_file_path = self.package_path / f"{self.client_file_name}.py"
-
-        self.client_generator.add_import(
-            names=self.arguments_generator.get_used_inputs(),
-            from_=self.input_types_module_name,
-            level=1,
-        )
-        self.client_generator.add_import(
-            names=self.arguments_generator.get_used_enums(),
-            from_=self.enums_module_name,
-            level=1,
-        )
-
-        for custom_scalar_name in self.arguments_generator.get_used_custom_scalars():
-            scalar_data = self.custom_scalars[custom_scalar_name]
-            if scalar_data.import_:
-                self.client_generator.add_import(
-                    names=scalar_data.names_to_import, from_=scalar_data.import_
-                )
-
-        self.client_generator.add_import(
-            names=[self.base_client_name],
-            from_=self.base_client_file_path.stem,
-            level=1,
-        )
-
         client_module = self.client_generator.generate()
         code = self._proccess_generated_code(
             ast_to_str(client_module, multiline_strings=True), self.queries_source
         )
         if self.plugin_manager:
             code = self.plugin_manager.generate_client_code(code)
         client_file_path.write_text(code)
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/result_fields.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,18 @@
 ) -> Tuple[Annotation, List[FieldNames]]:
     """Parse graphql type and return generated annotation."""
     if isinstance(type_, GraphQLScalarType):
         if type_.name in SIMPLE_TYPE_MAP:
             return (generate_annotation_name(SIMPLE_TYPE_MAP[type_.name], nullable), [])
         if custom_scalars and type_.name in custom_scalars:
             return (
-                generate_annotation_name(custom_scalars[type_.name].type_, nullable),
-                [FieldNames(custom_scalars[type_.name].type_, type_.name)],
+                generate_annotation_name(
+                    custom_scalars[type_.name].type_name, nullable
+                ),
+                [FieldNames(custom_scalars[type_.name].type_name, type_.name)],
             )
         return (generate_annotation_name(ANY, nullable), [])
 
     if isinstance(type_, GraphQLInterfaceType):
         inline_fragments = []
         if field.selection_set:
             inline_fragments = [
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/result_types.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/result_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     generate_field_with_alias,
     generate_import_from,
     generate_method_call,
     generate_module,
 )
 from ..exceptions import NotSupported, ParsingError
 from ..plugins.manager import PluginManager
-from ..utils import str_to_pascal_case, str_to_snake_case
+from ..utils import process_name, str_to_pascal_case
 from .constants import (
     ANY,
     BASE_MODEL_CLASS_NAME,
     FIELD_CLASS,
     LIST,
     MIXIN_FROM_NAME,
     MIXIN_IMPORT_NAME,
@@ -46,15 +46,15 @@
     PYDANTIC_MODULE,
     TYPENAME_FIELD_NAME,
     TYPING_MODULE,
     UNION,
     UPDATE_FORWARD_REFS_METHOD,
 )
 from .result_fields import FieldNames, parse_operation_field
-from .scalars import ScalarData
+from .scalars import ScalarData, generate_scalar_imports
 from .types import CodegenResultFieldType
 
 
 class ResultTypesGenerator:
     def __init__(
         self,
         schema: GraphQLSchema,
@@ -112,20 +112,16 @@
         if self._used_enums:
             self._imports.append(
                 generate_import_from(self._used_enums, self.enums_module_name, 1)
             )
         if self._used_scalars:
             for scalar_name in self._used_scalars:
                 scalar_data = self.custom_scalars[scalar_name]
-                if scalar_data.import_ and scalar_data.names_to_import:
-                    self._imports.append(
-                        generate_import_from(
-                            names=scalar_data.names_to_import, from_=scalar_data.import_
-                        )
-                    )
+                self._imports.extend(generate_scalar_imports(scalar_data))
+
         update_forward_refs_calls = [
             generate_expr(
                 generate_method_call(class_def.name, UPDATE_FORWARD_REFS_METHOD)
             )
             for class_def in self._class_defs
         ]
         module_body = (
@@ -185,15 +181,15 @@
                 resolved_selection_set, selection_set
             )
         for lineno, field in enumerate(
             resolved_selection_set,
             start=1,
         ):
             field_name = self._get_field_name(field)
-            name = self._process_field_name(field_name)
+            name = self._process_field_name(field_name, field=field)
             field_definition = self._get_field_from_schema(type_name, field.name.value)
             annotation, field_types_names = parse_operation_field(
                 field=field,
                 type_=cast(CodegenResultFieldType, field_definition.type),
                 directives=field.directives,
                 class_name=class_name + str_to_pascal_case(name),
                 custom_scalars=self.custom_scalars,
@@ -269,20 +265,23 @@
         return resolved_fields, selection_set.selections
 
     def _get_field_name(self, field: FieldNode) -> str:
         if field.alias:
             return field.alias.value
         return field.name.value
 
-    def _process_field_name(self, name: str) -> str:
-        if self.convert_to_snake_case:
-            if name == TYPENAME_FIELD_NAME:
-                return "__typename__"
-            return str_to_snake_case(name)
-        return name
+    def _process_field_name(self, name: str, field: FieldNode) -> str:
+        if self.convert_to_snake_case and name == TYPENAME_FIELD_NAME:
+            return "__typename__"
+        return process_name(
+            name,
+            convert_to_snake_case=self.convert_to_snake_case,
+            plugin_manager=self.plugin_manager,
+            node=field,
+        )
 
     def _get_field_from_schema(self, type_name: str, field_name: str) -> GraphQLField:
         try:
             return cast(GraphQLObjectType, self.schema.type_map[type_name]).fields[
                 field_name
             ]
         except KeyError as exc:
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/types.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/async_base_client.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/async_base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 
+from .base_model import UNSET
 from .exceptions import (
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
     GraphQlClientInvalidResponseError,
 )
 
 Self = TypeVar("Self", bound="AsyncBaseClient")
@@ -65,16 +66,22 @@
         if errors:
             raise GraphQLClientGraphQLMultiError.from_errors_dicts(
                 errors_dicts=errors, data=data
             )
 
         return cast(dict[str, Any], data)
 
+    def _convert_value(self, value: Any) -> Any:
+        if isinstance(value, BaseModel):
+            return value.dict(by_alias=True, exclude_unset=True)
+        if isinstance(value, list):
+            return [self._convert_value(item) for item in value]
+        return value
+
     def _convert_dict_to_json_serializable(
         self, dict_: Dict[str, Any]
     ) -> Dict[str, Any]:
         return {
-            key: value
-            if not isinstance(value, BaseModel)
-            else value.dict(by_alias=True)
+            key: self._convert_value(value)
             for key, value in dict_.items()
+            if value is not UNSET
         }
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/base_client.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 
+from .base_model import UNSET
 from .exceptions import (
     GraphQLClientGraphQLMultiError,
     GraphQLClientHttpError,
     GraphQlClientInvalidResponseError,
 )
 
 Self = TypeVar("Self", bound="BaseClient")
@@ -63,16 +64,22 @@
         if errors:
             raise GraphQLClientGraphQLMultiError.from_errors_dicts(
                 errors_dicts=errors, data=data
             )
 
         return cast(dict[str, Any], data)
 
+    def _convert_value(self, value: Any) -> Any:
+        if isinstance(value, BaseModel):
+            return value.dict(by_alias=True, exclude_unset=True)
+        if isinstance(value, list):
+            return [self._convert_value(item) for item in value]
+        return value
+
     def _convert_dict_to_json_serializable(
         self, dict_: Dict[str, Any]
     ) -> Dict[str, Any]:
         return {
-            key: value
-            if not isinstance(value, BaseModel)
-            else value.dict(by_alias=True)
+            key: self._convert_value(value)
             for key, value in dict_.items()
+            if value is not UNSET
         }
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/base_model.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/base_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
 
 from .scalars import SCALARS_PARSE_FUNCTIONS, SCALARS_SERIALIZE_FUNCTIONS
 
 
+class UnsetType:
+    def __bool__(self) -> bool:
+        return False
+
+
+UNSET = UnsetType()
+
+
 class BaseModel(PydanticBaseModel):
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         arbitrary_types_allowed = True
 
     # pylint: disable=no-self-argument
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/client_generators/dependencies/exceptions.py` & `ariadne_codegen-0.6.0/ariadne_codegen/client_generators/dependencies/exceptions.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/directives.py` & `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/directives.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/fields.py` & `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/fields.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/named_types.py` & `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/named_types.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/schema.py` & `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/schema.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/graphql_schema_generators/utils.py` & `ariadne_codegen-0.6.0/ariadne_codegen/graphql_schema_generators/utils.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/plugins/base.py` & `ariadne_codegen-0.6.0/ariadne_codegen/plugins/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import ast
-from typing import Dict, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
 from graphql import (
     FieldNode,
     GraphQLEnumType,
     GraphQLInputField,
     GraphQLInputObjectType,
     GraphQLSchema,
+    Node,
     OperationDefinitionNode,
     SelectionSetNode,
     VariableDefinitionNode,
 )
 
 
 # pylint: disable=too-many-public-methods
@@ -140,7 +141,11 @@
         return copied_code
 
     def generate_scalars_code(self, generated_code: str) -> str:
         return generated_code
 
     def generate_init_code(self, generated_code: str) -> str:
         return generated_code
+
+    # pylint: disable=unused-argument
+    def process_name(self, name: str, node: Optional[Node] = None) -> str:
+        return name
```

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/plugins/explorer.py` & `ariadne_codegen-0.6.0/ariadne_codegen/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/ariadne_codegen/plugins/manager.py` & `ariadne_codegen-0.6.0/ariadne_codegen/plugins/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from graphql import (
     FieldNode,
     GraphQLEnumType,
     GraphQLInputField,
     GraphQLInputObjectType,
     GraphQLSchema,
+    Node,
     OperationDefinitionNode,
     SelectionSetNode,
     VariableDefinitionNode,
 )
 
 from .base import Plugin
 
@@ -182,7 +183,10 @@
         return self._apply_plugins_on_object("copy_code", copied_code)
 
     def generate_scalars_code(self, generated_code: str) -> str:
         return self._apply_plugins_on_object("generate_scalars_code", generated_code)
 
     def generate_init_code(self, generated_code: str) -> str:
         return self._apply_plugins_on_object("generate_init_code", generated_code)
+
+    def process_name(self, name: str, node: Optional[Node] = None) -> str:
+        return self._apply_plugins_on_object("process_name", name, node=node)
```

### Comparing `ariadne_codegen-0.5.0/.gitignore` & `ariadne_codegen-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/LICENSE` & `ariadne_codegen-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ariadne_codegen-0.5.0/README.md` & `ariadne_codegen-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ```
 $ pip install ariadne-codegen
 ```
 
 
 ## Configuration
 
-`ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`'. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
+`ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
 
 Required settings:
 
 - `queries_path` - path to file/directory with queries
 
 One of the following 2 parameters is required, in case of providing both of them `schema_path` is prioritized:
 
@@ -98,18 +98,18 @@
 You can provide information about specific scalar by adding section to `pyproject.toml`:
 
 ```toml
 [tool.ariadne-codegen.scalars.{graphql scalar name}]
 type = "(required) python type name"
 serialize = "function used to serialize scalar"
 parse = "function used to create scalar instance from serialized form"
-import = "module to import from"
 ```
 
-All occurences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization. In all files which use `type`/`serialize`/`parse` there will be added extra import `from {import} import {type}, {serialize}, {parse}`
+All occurrences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization.
+If `type`/`serialize`/`parse` contains at least one `.` then string will be split by it's last occurrence. First part will be used as module to import from, and second part as type/method name. For example, `type = "custom_scalars.a.ScalarA"` will produce `from custom_scalars.a import ScalarA`.
 
 
 ### Example with scalar mapped to built-in type
 
 In this case scalar is mapped to built-in `str` which doesn\`t require custom `serialize ` and `parse` methods. 
 
 ```toml
@@ -120,33 +120,31 @@
 
 ### Example with type supported by pydantic
 
 In this scenario scalar is represented as `datetime`, so it needs to be imported. Pydantic handles serialization and deserialization so custom `parse` and `serialize` is not necessary.
 
 ```toml
 [tool.ariadne-codegen.scalars.DATETIME]
-type = "datetime"
-import = "datetime"
+type = "datetime.datetime"
 ```
 
 
 ### Example with fully custom type
 
 In this example scalar is represented as class `TypeB`. Pydantic can\`t handle  serialization and deserialization so custom `parse` and `serialize` is necessary. To provide `type`, `parse` and `serialize` implementation we can use `files_to_include` to copy `type_b.py` file.
 
 ```toml
 [tool.ariadne-codegen]
 ...
 files_to_include = [".../type_b.py"]
 
 [tool.ariadne-codegen.scalars.SCALARB]
-type = "TypeB"
-parse = "parse_b"
-serialize = "serialize_b"
-import = ".type_b"
+type = ".type_b.TypeB"
+parse = ".type_b.parse_b"
+serialize = ".type_b.serialize_b"
 ```
 
 
 ## Extending generated types
 
 ### Extending models with custom mixins
 
@@ -159,15 +157,15 @@
 ```py
 from {from} import {import}
 ...
 class OperationNameField(BaseModel, {import}):
     ...
 ```
 
-This directive can be used along with `files_to_include` option to extend funcionallity of generated classes.
+This directive can be used along with `files_to_include` option to extend functionality of generated classes.
 
 
 #### Example of usage of `mixin` and `files_to_include`:
 
 Query with `mixin` directive: 
 ```gql
 query listUsers {
@@ -234,11 +232,13 @@
 - Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)` 
 
 
 ## Contributing
 
 We welcome all contributions to Ariadne! If you've found a bug or issue, feel free to use [GitHub issues](https://github.com/mirumee/ariadne-codegen/issues). If you have any questions or feedback, don't hesitate to catch us on [GitHub discussions](https://github.com/mirumee/ariadne/discussions/).
 
+For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md).
+
 Also make sure you follow [@AriadneGraphQL](https://twitter.com/AriadneGraphQL) on Twitter for latest updates, news and random musings!
 
 
 ## **Crafted with ❤️ by [Mirumee Software](http://mirumee.com)** hello@mirumee.com
```

### Comparing `ariadne_codegen-0.5.0/pyproject.toml` & `ariadne_codegen-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ariadne-codegen"
 description = "Generate fully typed GraphQL client from schema, queries and mutations!"
 authors = [{ name = "Mirumee Software", email = "hello@mirumee.com" }]
-version = "0.5.0"
+version = "0.6.0"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
```

### Comparing `ariadne_codegen-0.5.0/PKG-INFO` & `ariadne_codegen-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariadne-codegen
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate fully typed GraphQL client from schema, queries and mutations!
 Project-URL: Homepage, https://ariadnegraphql.org/
 Project-URL: Repository, https://github.com/mirumee/ariadne-codegen
 Project-URL: Bug Tracker, https://github.com/mirumee/ariadne-codegen/issues
 Project-URL: Community, https://github.com/mirumee/ariadne/discussions
 Project-URL: Twitter, https://twitter.com/AriadneGraphQL
 Author-email: Mirumee Software <hello@mirumee.com>
@@ -67,15 +67,15 @@
 ```
 $ pip install ariadne-codegen
 ```
 
 
 ## Configuration
 
-`ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`'. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
+`ariadne-codegen` reads configuration from `[tool.ariadne-codegen]` section in your `pyproject.toml`. You can use other configuration file with `--config` option, eg. `ariadne-codegen --config custom_file.toml`
 
 Required settings:
 
 - `queries_path` - path to file/directory with queries
 
 One of the following 2 parameters is required, in case of providing both of them `schema_path` is prioritized:
 
@@ -136,18 +136,18 @@
 You can provide information about specific scalar by adding section to `pyproject.toml`:
 
 ```toml
 [tool.ariadne-codegen.scalars.{graphql scalar name}]
 type = "(required) python type name"
 serialize = "function used to serialize scalar"
 parse = "function used to create scalar instance from serialized form"
-import = "module to import from"
 ```
 
-All occurences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization. In all files which use `type`/`serialize`/`parse` there will be added extra import `from {import} import {type}, {serialize}, {parse}`
+All occurrences of `{graphql scalar name}` will be represented as `type`. If provided, `serialize` and `parse` will be used for serialization and deserialization.
+If `type`/`serialize`/`parse` contains at least one `.` then string will be split by it's last occurrence. First part will be used as module to import from, and second part as type/method name. For example, `type = "custom_scalars.a.ScalarA"` will produce `from custom_scalars.a import ScalarA`.
 
 
 ### Example with scalar mapped to built-in type
 
 In this case scalar is mapped to built-in `str` which doesn\`t require custom `serialize ` and `parse` methods. 
 
 ```toml
@@ -158,33 +158,31 @@
 
 ### Example with type supported by pydantic
 
 In this scenario scalar is represented as `datetime`, so it needs to be imported. Pydantic handles serialization and deserialization so custom `parse` and `serialize` is not necessary.
 
 ```toml
 [tool.ariadne-codegen.scalars.DATETIME]
-type = "datetime"
-import = "datetime"
+type = "datetime.datetime"
 ```
 
 
 ### Example with fully custom type
 
 In this example scalar is represented as class `TypeB`. Pydantic can\`t handle  serialization and deserialization so custom `parse` and `serialize` is necessary. To provide `type`, `parse` and `serialize` implementation we can use `files_to_include` to copy `type_b.py` file.
 
 ```toml
 [tool.ariadne-codegen]
 ...
 files_to_include = [".../type_b.py"]
 
 [tool.ariadne-codegen.scalars.SCALARB]
-type = "TypeB"
-parse = "parse_b"
-serialize = "serialize_b"
-import = ".type_b"
+type = ".type_b.TypeB"
+parse = ".type_b.parse_b"
+serialize = ".type_b.serialize_b"
 ```
 
 
 ## Extending generated types
 
 ### Extending models with custom mixins
 
@@ -197,15 +195,15 @@
 ```py
 from {from} import {import}
 ...
 class OperationNameField(BaseModel, {import}):
     ...
 ```
 
-This directive can be used along with `files_to_include` option to extend funcionallity of generated classes.
+This directive can be used along with `files_to_include` option to extend functionality of generated classes.
 
 
 #### Example of usage of `mixin` and `files_to_include`:
 
 Query with `mixin` directive: 
 ```gql
 query listUsers {
@@ -272,11 +270,13 @@
 - Schema declaration `{schema_variable_name}: GraphQLSchema = GraphQLSchema(...)` 
 
 
 ## Contributing
 
 We welcome all contributions to Ariadne! If you've found a bug or issue, feel free to use [GitHub issues](https://github.com/mirumee/ariadne-codegen/issues). If you have any questions or feedback, don't hesitate to catch us on [GitHub discussions](https://github.com/mirumee/ariadne/discussions/).
 
+For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md).
+
 Also make sure you follow [@AriadneGraphQL](https://twitter.com/AriadneGraphQL) on Twitter for latest updates, news and random musings!
 
 
 ## **Crafted with ❤️ by [Mirumee Software](http://mirumee.com)** hello@mirumee.com
```

