# Comparing `tmp/dxd-0.0.3.tar.gz` & `tmp/dxd-0.0.4.tar.gz`

## Comparing `dxd-0.0.3.tar` & `dxd-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/__about__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/column.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/engine.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/expr.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/pattern.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/postgres_engine.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/sqlite_engine.py
--rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 dxd-0.0.3/dxd/table.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dxd-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dxd-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dxd-0.0.3/tests/test_tinyorm.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 dxd-0.0.3/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dxd-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dxd-0.0.3/README.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dxd-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dxd-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/__about__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/column.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/engine.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/expr.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/kvstore.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/pattern.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/postgres_engine.py
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/sqlite_engine.py
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 dxd-0.0.4/dxd/table.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dxd-0.0.4/tests/test_tinyorm.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 dxd-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dxd-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 dxd-0.0.4/README.md
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dxd-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dxd-0.0.4/PKG-INFO
```

### Comparing `dxd-0.0.3/dxd/column.py` & `dxd-0.0.4/dxd/column.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 
     def __repr__(self):
         return f"{self.schema.__name__}.{self.name}"
 
     def __hash__(self):
         return hash((self.schema.__name__, self.name))
 
+    def __eq__(self, other):
+        if isinstance(other, Column):
+            return hash(self) == hash(other)
+        return super().__eq__(other)
+
     @classmethod
     def of_field(cls, schema, f: Field) -> "Column":
         cls = f.metadata.get("cls", cls)
         return cls(schema, f)
 
 
 class JsonCol(Column):
@@ -122,15 +127,18 @@
             raise ValueError("Cannot set both default and default_factory.")
         default_factory = lambda: default
     # [todo] kwonly = true
     if encoding is not None:
         cls = JsonCol
     else:
         cls = Column
-    assert foreign_key is None or isinstance(foreign_key, Column)
+    if not any(
+        [foreign_key is None, foreign_key is True, isinstance(foreign_key, Column)]
+    ):
+        raise TypeError("foreign_key must be None, True, or a Column")
     return field(
         metadata={
             **metadata,
             "primary": primary,
             "cls": cls,
             "foreign_key": foreign_key,
         },
```

### Comparing `dxd-0.0.3/dxd/engine.py` & `dxd-0.0.4/dxd/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
     def adapt(self, value):
         return adapt(value, self.protocol)
 
     def restore(self, T, value):
         return restore(T, value)
 
+    def commit(self):
+        raise NotImplementedError()
+
     # [todo] transaction context manager
 
 
 engine_context: ContextVar[Engine] = ContextVar("engine")
 
 
 @contextmanager
```

### Comparing `dxd-0.0.3/dxd/expr.py` & `dxd-0.0.4/dxd/expr.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,23 +30,29 @@
 
     def __radd__(self, other):
         return Expr.binary("+", [other, self], 8)
 
     def __and__(self, other):
         return Expr.binary(" AND ", [self, other], precedence=2)
 
+    def __or__(self, other):
+        return Expr.binary(" OR ", [self, other], precedence=2)
+
     def __eq__(self, other):
         return Expr.binary(" = ", [self, other], 4)
 
     def __ne__(self, other):
         return Expr.binary(" != ", [self, other], 4)
 
     def __not__(self):
         return Expr("NOT ( ? )", [self], 3)
 
+    def __bool__(self):
+        raise ValueError(f"{self} is not a boolean expression")
+
 
 class Expr(AbstractExpr):
     """A sqlite expression. That is, it's a template string full of '?'s and a value for each '?'.
 
     Any user-provided data should be represented as a '?' with an item in `values` to prevent injection attacks.
     However we don't add any checks for this.
     """
```

### Comparing `dxd-0.0.3/dxd/pattern.py` & `dxd-0.0.4/dxd/pattern.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 class Pattern(Generic[S]):
     """A list of Exprs and a function sending these exprs to a python value."""
 
     items: list[Expr]
     outfn: Callable[[list[Any]], S]
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({repr(self.items), repr(self.outfn)})"
+
     def __len__(self):
         return len(self.items)
 
     @overload
     def __init__(self, obj: S):
         ...
 
@@ -101,7 +104,18 @@
         def comp(x):
             return fn(self.outfn(x))
 
         return Pattern(self.items, comp)
 
     def to_expr(self) -> "Expr":
         return Expr.binary(", ", self.items)
+
+
+def sum(inner) -> Any:
+    """Runs the SUM reduction on the given select pattern."""
+    inner = Pattern(inner)
+    if len(inner.items) != 1:
+        raise ValueError(
+            f"Pattern {inner} has {len(inner.items)} items but needs 1 for a SUM."
+        )
+    item = inner.items[0]
+    return Pattern([Expr("SUM(?)", [item])], lambda x: x[0] or 0)
```

### Comparing `dxd-0.0.3/dxd/postgres_engine.py` & `dxd-0.0.4/dxd/postgres_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 type_map = {
     bool: "boolean",
     int: "integer",
     float: "float8",
     Decimal: "numeric",
     str: "text",
-    bytes: "bytes",
+    bytes: "BYTEA",
     datetime.date: "date",
     datetime.datetime: "timestamp",
     datetime.time: "time",
     datetime.timedelta: "interval",
     UUID: "uuid",
 }
```

### Comparing `dxd-0.0.3/dxd/sqlite_engine.py` & `dxd-0.0.4/dxd/sqlite_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum
 import logging
 from sqlite3 import PrepareProtocol as P, Connection
 import datetime
 import textwrap
-from typing import Any, Type
+from typing import Any, NewType, Type
 import uuid
 from miniscutil import as_optional, register_adapter
+from miniscutil.type_util import as_newtype
 from .engine import Engine
 
 logger = logging.getLogger("dxd.sqlite3")
 
 
 def ident(x):
     return x
@@ -55,16 +56,24 @@
         logger.debug(f"SqliteEngine.executemany {len(values)}:\n{msg}")
         return self.connection.executemany(query, values)
 
     def transaction(self):
         with self.connection:
             yield self
 
+    def commit(self):
+        self.connection.commit()
+
     def get_storage_type(self, T: Type):
         def core(T: Type):
+            S = as_newtype(T)
+            if S is not None:
+                return core(S)
+            if not isinstance(T, type):
+                raise TypeError(f"{T} is not a type")
             if issubclass(T, str):
                 return "TEXT"
             elif issubclass(T, int):
                 return "INTEGER"
             elif issubclass(T, float):
                 return "REAL"
             elif issubclass(T, bool):
```

### Comparing `dxd-0.0.3/dxd/table.py` & `dxd-0.0.4/dxd/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from dataclasses import dataclass, fields
+from dataclasses import dataclass, fields, is_dataclass
 from enum import Enum
+from functools import cache, reduce
+import logging
+import operator
 from typing import (
     Any,
     Generic,
     Iterable,
     Iterator,
+    Literal,
     Optional,
     Type,
     TypeVar,
     Union,
     overload,
 )
 from .engine import Engine, engine_context
-from .column import Column
+from .column import Column, col
 from .expr import Expr
 from .pattern import Pattern
 
 T = TypeVar("T", bound="Schema")
 S = TypeVar("S")
 R = TypeVar("R")
 
+logger = logging.getLogger("dxd")
+
 
 class OrderKind(Enum):
     Ascending = "ASC"
     Descending = "DESC"
 
 
-WhereClause = Union[bool, dict]
-
-
-def where_to_expr(where: WhereClause):
-    if where is True:
-        return Expr.empty
+WhereClause = Union[bool, dict, tuple]
 
 
 class SchemaMeta(type):
     def __getattr__(self, key):
         """If we call `User.name`, it should return the `Column` object for that."""
         if key.startswith("__"):
             raise AttributeError()
@@ -44,82 +45,133 @@
             # [todo] pydantic support
             raise ValueError("Remember to make Schema a dataclass")
         field = fields.get(key, None)
         if field is None:
             raise AttributeError(f"No column named {key}")
         return Column.of_field(self, field)
 
-    def default_name(self):
-        return self.__name__ + "_table"
-
 
 class Schema(metaclass=SchemaMeta):
     @classmethod
+    def default_name(cls):
+        return cls.__name__ + "_table"
+
+    @classmethod
     def create_table(
         cls: Type[T],
         name: Optional[str] = None,
         engine: Optional[Engine] = None,
         references: dict[Any, "Table[Any]"] = {},
+        check_schema: Literal["ignore", "raise", "clobber"] = "clobber",
     ) -> "Table[T]":
         # if clobber is true then if the table exists but the schema has changed we
         # just brutally wipe everything.
         # [todo] validate column names and table name.
         # [todo] migrations?
+        if not is_dataclass(cls):
+            raise TypeError(
+                f"{cls.__name__} is not a dataclass. "
+                f"dxd requires all Schema subclasses to be dataclasses."
+            )
         engine = engine or engine_context.get()
-        name = name or cls.default_name()
+        name = name or cls.default_name()  # type: ignore
 
         fields = [c.sql_schema for c in columns(cls)]
         if not any(c.primary for c in columns(cls)):
             raise TypeError(
-                f"At least one of the fields in {cls.__name__} should be labelled as primary: `= col(primary = True)`"
+                f"at least one of the fields in {cls.__name__} should be labelled as primary: `= col(primary = True)`"
             )
         ks = ", ".join([c.name for c in columns(cls) if c.primary])
         fields.append(f"PRIMARY KEY ({ks})")
         for c in columns(cls):
             fk = c.foreign_key
             if fk is not None:
-                assert isinstance(fk, Column)
-                table: Table | None = references.get(c, references.get(c.name, None))
+                table: Optional[Table] = references.get(c, references.get(c.name, None))
                 if table is None:
                     raise ValueError(
-                        f"No reference table found for foreign key {repr(c)}."
+                        f"no reference table found for foreign key {repr(c)}"
                     )
-                if table.schema != fk.schema:
-                    raise ValueError(f"Incompatible foreign key {repr(fk)} in {table}")
-                if fk.type != c.type:
-                    raise TypeError(
-                        f"types {repr(fk)} : {fk.type} and {repr(c)} : {c.type} do not match."
+                if isinstance(fk, Column):
+                    if table.schema != fk.schema:
+                        raise ValueError(
+                            f"Incompatible foreign key {repr(fk)} in {table}"
+                        )
+                    if fk.type != c.type:
+                        raise TypeError(
+                            f"types {repr(fk)} : {fk.type} and {repr(c)} : {c.type} do not match"
+                        )
+                    fields.append(
+                        f"FOREIGN KEY ({c.name}) REFERENCES {table.name} ({fk.name}) ON DELETE CASCADE"
                     )
-                fields.append(
-                    f"FOREIGN KEY ({c.name}) REFERENCES {table.name} ({fk.name}) ON DELETE CASCADE"
-                )
+                elif fk is True:
+                    # get the primary key
+                    p = table.primary_key_pattern()
+                    e = p.to_expr()
+                    assert len(e.values) == 0, "pattern had values"
+                    t = e.template
+                    logger.debug(f"Guessing template {t} for table {table.name}")
+                    fields.append(
+                        f"FOREIGN KEY ({c.name}) REFERENCES {table.name} ({t}) ON DELETE CASCADE"
+                    )
+                else:
+                    raise TypeError(f"unknown foreign key {repr(fk)}")
         fields = ",\n  ".join(fields)
+
+        if check_schema != "ignore":
+            schema_table = get_schema_table(engine)
+            schemas = list(
+                schema_table.select(
+                    where=(SchemaRecord.table_name == name)
+                    & (SchemaRecord.fields != fields)
+                )
+            )
+            if len(schemas) > 0:
+                if check_schema == "raise":
+                    raise RuntimeError(
+                        f"Schema for {name} has changed, please migrate the table and try again."
+                    )
+                elif check_schema == "clobber":
+                    logger.warning(
+                        f"Schema for {name} already exists, clobbering. Data is lost."
+                    )
+                    # [todo] add a feature where table names are prefixed with a schema version
+                    # just keep multiple incompatible tables.
+                    # [todo] migration stuff will eventually go here.
+                    # [todo] cascading?
+                    engine.execute(f"DROP TABLE {name};")
+                    schema_table.delete(where=(SchemaRecord.table_name == name))
+            schema_table.insert_one(
+                SchemaRecord(table_name=name, fields=fields), or_ignore=True
+            )
+
         q = f"CREATE TABLE IF NOT EXISTS {name} (\n  {fields}\n);"
         engine.execute(q)
-        return Table(name=name, connection=engine, schema=cls)
+        engine.commit()
+        return Table(name=name, connection=engine, schema=cls)  # type: ignore
 
     @classmethod
     def as_column(cls, item: Union[Column, str]) -> Column:
         if isinstance(item, Column):
             return item
-        else:
-            assert isinstance(item, str)
+        elif isinstance(item, str):
             fields = getattr(cls, "__dataclass_fields__")
             # [todo] pydantic
             return Column.of_field(cls, fields.get(item))
+        else:
+            raise TypeError(f"can't convert {item} to a table column")
 
 
 @dataclass
 class Table(Generic[T]):
     name: str
     connection: Engine
     schema: "Type[T]"
 
     def __len__(self):
-        c = self.connection.execute(f"SELECT COUNT(*) FROM {self.name}")
+        c = self.connection.execute(f"SELECT COUNT(*) FROM {self.name} ; ")
         return c.fetchone()[0]
 
     def drop(self, not_exists_ok: bool = True):
         """Drops the table.
 
         Note that once this is called subsequent queries to the table will error."""
         ne = "IF EXISTS " if not_exists_ok else ""
@@ -141,22 +193,41 @@
             e = [self.schema.as_column(k) == v for k, v in where.items()]
             e = Expr.binary("AND", e, precedence=2)
         else:
             assert isinstance(where, Expr)
             e = where
         return Expr("WHERE ?", [e])
 
+    def primary_key_pattern(self) -> Pattern:
+        pcs = [c for c in columns(self) if c.primary]
+        if len(pcs) == 1:
+            return Pattern(pcs[0])
+        return Pattern(tuple(Pattern(c) for c in pcs))
+
     def pattern(self) -> Pattern[T]:
         cs = list(columns(self))
 
         def blam(d: dict) -> T:
             return self.schema(**d)
 
         return Pattern({c.name: Pattern(c) for c in cs}).map(blam)
 
+    def where_to_expr(self, where: WhereClause) -> Expr:
+        if where is True:
+            return Expr.empty()
+        elif isinstance(where, dict):
+            kvs = reduce(
+                operator.and_, [self.schema.as_column(k) == v for k, v in where.items()]
+            )
+            return kvs
+        elif isinstance(where, tuple):
+            return reduce(operator.and_, where)
+        else:
+            return Expr(where)
+
     @overload
     def select(
         self,
         *,
         where: WhereClause = True,
         order_by: Optional[Any] = None,
         descending=False,
@@ -188,14 +259,22 @@
             asc = "DESC" if descending else "ASC"
             query = Expr(f"?\nORDER BY ? {asc}", [query, order_by])
         if limit is not None:
             query = Expr(f"?\nLIMIT {limit}", [query])
         xs = self.connection.execute_expr(query)
         return map(p.outfn, xs)
 
+    def sum(self, col, where=True) -> float:
+        c = self.schema.as_column(col)
+        query = Expr(f"SELECT SUM({c.name}) \nFROM {self.name} ", [])
+        if where is not True:
+            query = Expr("?\n?", [query, self._mk_where_clause(where)])
+        xs = self.connection.execute_expr(query)
+        return next(iter(xs))[0] or 0
+
     @overload
     def insert_one(self, item: T, *, or_ignore=False) -> None:
         ...
 
     @overload
     def insert_one(self, item: T, *, returning: S, or_ignore=False) -> S:
         ...
@@ -300,16 +379,17 @@
 
     @overload
     def update(self, values, *, where: bool = True) -> int:
         """Run an UPDATE query on the object. Returns the number of records that were updated."""
         ...
 
     def update(self, values, where=True, returning=None):  # type: ignore
+        # [todo] if 'where : T', set where to be T's primary key.
         def mk_setter(key, value) -> "Expr":
-            assert isinstance(key, Column)  # [todo] strings for column names are ok too
+            key = self.schema.as_column(key)
             return Expr(f"{key.name} = ?", [value])
 
         setters = Expr.binary(", ", [mk_setter(k, v) for k, v in values.items()])
         t = "UPDATE"
         query = Expr(f"{t} {self.name} SET ? ", [setters])
         if where is not True:
             assert isinstance(where, Expr)
@@ -341,8 +421,23 @@
 
 
 def columns(x) -> Iterable[Column]:
     if isinstance(x, Table):
         x = x.schema
     assert x is not Schema
     assert issubclass(x, Schema)
+    assert is_dataclass(x), f"Expected dataclass, got {type(x)}"
     return [Column.of_field(x, f) for f in fields(x)]
+
+
+@dataclass
+class SchemaRecord(Schema):
+    table_name: str = col(primary=True)
+    fields: str = col(primary=True)
+
+
+@cache
+def get_schema_table(engine: Engine) -> Table[SchemaRecord]:
+    table = SchemaRecord.create_table(
+        "_dxd_schema_table", engine, check_schema="ignore"
+    )
+    return table
```

### Comparing `dxd-0.0.3/tests/conftest.py` & `dxd-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.3/tests/test_tinyorm.py` & `dxd-0.0.4/tests/test_tinyorm.py`

 * *Files identical despite different names*

### Comparing `dxd-0.0.3/.gitignore` & `dxd-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dxd-0.0.3/LICENSE.txt` & `dxd-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dxd-0.0.3/README.md` & `dxd-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dxd-0.0.3/pyproject.toml` & `dxd-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 [tool.hatch.version]
 path = "dxd/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
+  "miniscutil @ {root:uri}/../miniscutil",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=dxd --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["39", "310", "311"]
@@ -59,11 +60,10 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.hatch.envs.test]
 dependencies = [
   "pytest", "pytest-cov", "hypothesis", "pytest-snapshot",
-  "numpy", "pandas", "pillow",
-  "torch; python_version < '3.11'",
+  "numpy",
   "psycopg"
 ]
```

### Comparing `dxd-0.0.3/PKG-INFO` & `dxd-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxd
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/EdAyers/sss/dxd#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/dxd/issues
 Project-URL: Source, https://github.com/EdAyers/sss/dxd
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

