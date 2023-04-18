# Comparing `tmp/typegraph-0.1.4.tar.gz` & `tmp/typegraph-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.4.tar", max compression
+gzip compressed data, was "typegraph-0.1.5.tar", max compression
```

## Comparing `typegraph-0.1.4.tar` & `typegraph-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5252 2023-04-11 08:10:14.940361 typegraph-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     1427 2023-04-11 08:10:14.940361 typegraph-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      225 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/models.py
--rw-r--r--   0        0        0     1947 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     7955 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7499 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     4078 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/policies.py
--rw-r--r--   0        0        0     1675 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    21779 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    13927 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2209 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     5234 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1403 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2789 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1352 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/python_wasi.py
--rw-r--r--   0        0        0     2880 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1169 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    20231 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2159 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-04-11 08:10:14.944361 typegraph-0.1.4/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 typegraph-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5252 2023-04-18 10:58:06.594397 typegraph-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     1427 2023-04-18 10:58:06.594397 typegraph-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/__init__.py
+-rw-r--r--   0        0        0      904 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/effects.py
+-rw-r--r--   0        0        0     3323 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      377 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1868 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3066 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1947 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     5774 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0     7955 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3667 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7499 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4236 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0     8909 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     4078 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/policies.py
+-rw-r--r--   0        0        0     1675 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28490 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    21712 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6601 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    13927 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2373 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2209 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1351 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5234 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1403 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2789 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1352 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/python_wasi.py
+-rw-r--r--   0        0        0     2880 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2053 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1169 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    20231 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/types.py
+-rw-r--r--   0        0        0      487 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     1977 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2198 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      185 2023-04-18 10:58:06.598397 typegraph-0.1.5/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.5/PKG-INFO
```

### Comparing `typegraph-0.1.4/LICENSE.md` & `typegraph-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/pyproject.toml` & `typegraph-0.1.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.4"
+version = "0.1.5"
 description = "Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
 license = "ELv2"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
@@ -14,35 +14,36 @@
 ]
 
 [tool.poetry.scripts]
 py-tg = "typegraph.utils.loaders:cmd"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-httpx = { extras = ["http2"], version = ">=0.22,<0.24" }
+httpx = { extras = ["http2"], version = "^0.24.0" }
 redbaron = "^0.9.2"
-frozendict = "2.3.6"
-semver = "^2.13.0"
+frozendict = "^2.3.7"
+semver = "^3.0.0"
 PyYAML = "^6.0"
 deepmerge = "^1.1.0"
 graphql-core = "^3.2.3"
 ordered-set = "^4.1.0"
 typing-extensions = "^4.5.0"
 attrs = "^22.2.0"
 astunparse = "^1.6.3"
-black = ">=22.12,<24.0"
-strenum = "^0.4.9"
-python-box = "^7.0.0"
+black = "^23.3.0"
+strenum = "^0.4.10"
+python-box = "^7.0.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 pytest-snapshot = "^0.9.0"
 pydoc-markdown = { git = "https://github.com/metatypedev/pydoc-markdown", branch = "develop" }
-ruff = ">=0.0.245,<0.0.261"
+ruff = "^0.0.261"
 respx = "^0.20.1"
+coverage = "^7.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 venvPath = ".."
```

### Comparing `typegraph-0.1.4/typegraph/effects.py` & `typegraph-0.1.5/typegraph/effects.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/graph/auth/__init__.py` & `typegraph-0.1.5/typegraph/graph/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/graph/builder.py` & `typegraph-0.1.5/typegraph/graph/builder.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/graph/models.py` & `typegraph-0.1.5/typegraph/graph/models.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/graph/nodes.py` & `typegraph-0.1.5/typegraph/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/graph/typegraph.py` & `typegraph-0.1.5/typegraph/graph/typegraph.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/importers/base/importer.py` & `typegraph-0.1.5/typegraph/importers/base/importer.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/importers/base/typify.py` & `typegraph-0.1.5/typegraph/importers/base/typify.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/importers/google_discovery.py` & `typegraph-0.1.5/typegraph/importers/google_discovery.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/importers/graphql.py` & `typegraph-0.1.5/typegraph/importers/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/importers/openapi.py` & `typegraph-0.1.5/typegraph/importers/openapi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/policies.py` & `typegraph-0.1.5/typegraph/policies.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.5/typegraph/providers/aws/runtimes/s3.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/prisma/relations.py` & `typegraph-0.1.5/typegraph/providers/prisma/relations.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/prisma/runtimes/prisma.py` & `typegraph-0.1.5/typegraph/providers/prisma/runtimes/prisma.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,57 +301,57 @@
             if isinstance(typ, t.typedef):
                 typ.register_name()
             typ = typ.name
         else:
             g = TypegraphContext.get_active()
         return LinkProxy(g, typ, rel_name=name, field=field, fkey=fkey)
 
-    def queryRaw(self, query: str, out: t.TypeNode, *, effect: Effect) -> t.func:
+    def raw_query(self, query: str, out: t.TypeNode, *, effect: Effect) -> t.func:
         """Generate a raw SQL query operation on the runtime
 
         Example:
         ```python
         db = PrismaRuntime("my-app", "POSTGRES")
         g.expose(
-            countUsers=db.queryRaw("SELECT COUNT(*) FROM User", t.integer())
+            countUsers=db.raw_query("SELECT COUNT(*) FROM User", t.integer())
         )
         ```
         """
         return t.func(
             t.struct(
                 {
                     "parameters": t.json(),
                 }
             ).named("QueryRawInp"),
             out,
             PrismaOperationMat(self, query, "queryRaw", effect=effect),
         )
 
-    def executeRaw(self, query: str, *, effect: Effect) -> t.func:
+    def raw_execute(self, query: str, *, effect: Effect) -> t.func:
         """Generate a raw SQL query operation without return
 
         Example:
         ```python
         db = PrismaRuntime("my-app", "POSTGRES")
         g.expose(
-            setActive=db.executeRaw("UPDATE User SET active = TRUE WHERE id=$1", effect=effects.update()),
+            setActive=db.raw_execute("UPDATE User SET active = TRUE WHERE id=$1", effect=effects.update()),
         )
         ```
         """
         return t.func(
             t.struct(
                 {
                     "parameters": t.json().optional().default("[]"),
                 }
             ).named(f"ExecuteRawInp_{TypegraphContext.get_active().next_type_id()}"),
             t.integer(),
             PrismaOperationMat(self, query, "executeRaw", effect=effect),
         )
 
-    def find_unique(self, tpe: Union[t.struct, t.NodeProxy], where=None) -> t.func:
+    def find(self, tpe: Union[t.struct, t.NodeProxy], where=None) -> t.func:
         self.__manage(tpe)
         typegen = self.__typegen
         _pref = get_name_generator("Unique", tpe)
         # output = typegen.get_out_type(base_output)
         output = typegen.add_nested_count(tpe)
         if where is None:
             # findUnique's where expression
@@ -597,17 +597,14 @@
         )
         return data
 
     @property
     def edges(self) -> List[Node]:
         return super().edges + list(self.reg.managed.values())
 
-    def insert_one(self, tpe):
-        return self.create(tpe)
-
 
 @frozen
 class PrismaMigrationRuntime(Runtime):
     runtime_name: str = always("prisma_migration")
 
 
 @frozen
```

### Comparing `typegraph-0.1.4/typegraph/providers/prisma/schema.py` & `typegraph-0.1.5/typegraph/providers/prisma/schema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.5/typegraph/providers/prisma/type_generator.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/prisma/utils.py` & `typegraph-0.1.5/typegraph/providers/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.5/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/base.py` & `typegraph-0.1.5/typegraph/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/deno.py` & `typegraph-0.1.5/typegraph/runtimes/deno.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/graphql.py` & `typegraph-0.1.5/typegraph/runtimes/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/http.py` & `typegraph-0.1.5/typegraph/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/python_wasi.py` & `typegraph-0.1.5/typegraph/runtimes/python_wasi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/random.py` & `typegraph-0.1.5/typegraph/runtimes/random.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/typegate.py` & `typegraph-0.1.5/typegraph/runtimes/typegate.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/runtimes/wasmedge.py` & `typegraph-0.1.5/typegraph/runtimes/wasmedge.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/types.py` & `typegraph-0.1.5/typegraph/types.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/utils/attrs.py` & `typegraph-0.1.5/typegraph/utils/attrs.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/utils/jsonschema.py` & `typegraph-0.1.5/typegraph/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.4/typegraph/utils/loaders.py` & `typegraph-0.1.5/typegraph/utils/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,7 +82,11 @@
             if isinstance(o, frozendict):
                 return dict(o)
             return super().default(o)
 
     opt = dict(indent=2) if args.pretty else {}
     output = json.dumps([tg.build() for tg in tgs], cls=JSONEncoder, **opt)
     print(output)
+
+
+if __name__ == "__main__":
+    cmd()
```

### Comparing `typegraph-0.1.4/PKG-INFO` & `typegraph-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.4
+Version: 0.1.5
 Summary: Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
 Home-page: https://metatype.dev
 License: ELv2
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: astunparse (>=1.6.3,<2.0.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
-Requires-Dist: black (>=22.12,<24.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
-Requires-Dist: frozendict (==2.3.6)
+Requires-Dist: frozendict (>=2.3.7,<3.0.0)
 Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
-Requires-Dist: httpx[http2] (>=0.22,<0.24)
+Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
-Requires-Dist: python-box (>=7.0.0,<8.0.0)
+Requires-Dist: python-box (>=7.0.1,<8.0.0)
 Requires-Dist: redbaron (>=0.9.2,<0.10.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0)
-Requires-Dist: strenum (>=0.4.9,<0.5.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
+Requires-Dist: strenum (>=0.4.10,<0.5.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/metatypedev/metatype
```

