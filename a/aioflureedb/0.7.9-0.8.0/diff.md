# Comparing `tmp/aioflureedb-0.7.9.tar.gz` & `tmp/aioflureedb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioflureedb-0.7.9.tar", last modified: Wed Apr  5 11:59:03 2023, max compression
+gzip compressed data, was "aioflureedb-0.8.0.tar", last modified: Tue Apr 18 10:23:15 2023, max compression
```

## Comparing `aioflureedb-0.7.9.tar` & `aioflureedb-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/
--rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.7.9/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/aioflureedb/
--rw-r--r--   0 rob       (1000) rob       (1000)    74028 2023-04-05 11:57:42.000000 aioflureedb-0.7.9/aioflureedb/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6858 2023-03-29 11:47:10.000000 aioflureedb-0.7.9/aioflureedb/__main__.py
--rw-r--r--   0 rob       (1000) rob       (1000)    25924 2022-09-14 15:46:46.000000 aioflureedb-0.7.9/aioflureedb/domain_api.py
--rw-r--r--   0 rob       (1000) rob       (1000)     7010 2022-06-30 09:29:56.000000 aioflureedb-0.7.9/aioflureedb/signing.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/aioflureedb.egg-info/
--rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-04-05 11:59:02.000000 aioflureedb-0.7.9/aioflureedb.egg-info/PKG-INFO
--rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/SOURCES.txt
--rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-04-05 11:59:02.000000 aioflureedb-0.7.9/aioflureedb.egg-info/dependency_links.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/requires.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-04-05 11:59:03.000000 aioflureedb-0.7.9/aioflureedb.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-05 11:59:03.453185 aioflureedb-0.7.9/setup.cfg
--rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-04-05 11:57:53.000000 aioflureedb-0.7.9/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.8.0/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/aioflureedb/
+-rw-r--r--   0 rob       (1000) rob       (1000)    74739 2023-04-18 07:49:10.000000 aioflureedb-0.8.0/aioflureedb/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6874 2023-04-14 14:10:59.000000 aioflureedb-0.8.0/aioflureedb/__main__.py
+-rw-r--r--   0 rob       (1000) rob       (1000)    25925 2023-04-14 14:07:21.000000 aioflureedb-0.8.0/aioflureedb/domain_api.py
+-rw-r--r--   0 rob       (1000) rob       (1000)     7030 2023-04-14 14:06:52.000000 aioflureedb-0.8.0/aioflureedb/signing.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/aioflureedb.egg-info/
+-rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/PKG-INFO
+-rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/SOURCES.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/dependency_links.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/requires.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/setup.cfg
+-rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-04-18 10:21:47.000000 aioflureedb-0.8.0/setup.py
```

### Comparing `aioflureedb-0.7.9/PKG-INFO` & `aioflureedb-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.7.9
+Version: 0.8.0
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.7.9/README.md` & `aioflureedb-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.7.9/aioflureedb/__init__.py` & `aioflureedb-0.8.0/aioflureedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
         Raises
         ------
         FlureeHttpError
             If the server returns something different than a 200 OK status
         """
         if self.debug:
-            print("Unsigned GET: url =", self.url,", ssl_verify_disabled =", self.ssl_verify_disabled)
+            print("Unsigned GET: url =", self.url, ", ssl_verify_disabled =", self.ssl_verify_disabled)
         if self.ssl_verify_disabled:
             async with self.session.get(self.url, ssl=False) as resp:
                 if resp.status != 200:
                     raise FlureeHttpError(await resp.text(), resp.status)
                 response = await resp.text()
                 if self.debug:
                     print("Result:")
@@ -369,15 +369,15 @@
 
         Raises
         ------
         FlureeHttpError
             When Fluree server returns a status code other than 200
         """
         if self.debug:
-            print("Signed POST: url =", self.url,", headers =", headers, ",ssl_verify_disabled =", self.ssl_verify_disabled)
+            print("Signed POST: url =", self.url, ", headers =", headers, ",ssl_verify_disabled =", self.ssl_verify_disabled)
             print("  body = ", body)
         if self.ssl_verify_disabled:
             async with self.session.post(self.url, data=body, headers=headers, ssl=False) as resp:
                 if resp.status != 200:
                     raise FlureeHttpError(await resp.text(), resp.status)
                 data = await resp.text()
                 if self.debug:
@@ -414,46 +414,49 @@
             JSON decoded response from FlureeDB server
 
         Raises
         ------
         TypeError
             If an unknown kwarg is used on invocation OR a required kwarg is not supplied
         """
-        # pylint: disable=too-many-locals
+        # pylint: disable=too-many-locals, too-many-branches
         kwset = set()
         kwdict = {}
         for key, value in kwargs.items():
             if not (key in self.required or key in self.optional):
                 raise TypeError("SignedPoster got unexpected keyword argument '" + key + "'")
             kwset.add(key)
-            if key == "db_id" or key == "ledger_id":
+            if key in {"db_id", "ledger_id"}:
                 kwdict["ledger/id"] = value
             else:
                 kwdict[key] = value
         for reqkey in self.required:
             if reqkey not in kwset:
                 raise TypeError("SignedPoster is missing one required named argument '", reqkey, "'")
+        if self.url.endswith("/new-ledger"):
+            if "owners" not in kwdict:
+                kwdict["owners"] = []
+            if self.signer.auth_id not in kwdict["owners"]:
+                kwdict["owners"].append(self.signer.auth_id)
         body = json.dumps(kwdict, indent=4, sort_keys=True)
         headers = {"Content-Type": "application/json"}
         if not self.unsigned:
             if self.debug:
                 print("Signing with:", self.signer.auth_id)
             body, headers, _ = self.signer.sign_query(kwdict)
         rval = await self._post_body_with_headers(body, headers)
         # If this is a new-db or new-legger, we need to await till it comes into existance.
+        # pylint: disable=too-many-boolean-expressions
         if (isinstance(rval, str) and len(rval) == 64 and
                 (
                     (self.url.split("/")[-1] == "new-db" and "db_id" in kwargs) or
                     (self.url.split("/")[-1] == "new-ledger" and "ledger_id" in kwargs)
                 )):
-            if "ledger_id" in kwargs:
-                dbid = kwargs["ledger_id"]
-            else:
-                dbid = kwargs["db_id"]
-            while True:
+            dbid = kwargs.get("ledger_id", kwargs.get("db_id", None))
+            while dbid:
                 databases = await self.client.ledgers()
                 for database in databases:
                     dbid2 = database[0] + "/" + database[1]
                     if dbid == dbid2:
                         return rval
                 await asyncio.sleep(0.1)
         return rval
@@ -609,15 +612,15 @@
         sig_fuel : int
                    Not sure what this is for, consult FlureeDB documentation for info.
 
         """
         assert isinstance(sig_validity, (float, int))
         self.debug = False
         if environ.get("AIOFLUREEDB_DEBUG") == "TRUE":
-            self.debug=True
+            self.debug = True
         self.host = host
         self.port = port
         self.https = https
         self.ssl_verify = ssl_verify
         self.ssl_verify_disabled = False
         if https and not ssl_verify:
             self.ssl_verify_disabled = True
@@ -642,25 +645,25 @@
         self.depricated = {
                     "dbs": "ledgers",
                     "new_db": "new_ledger",
                     "delete_db": "delete_ledger",
                     "add_server": None,
                     "remove_server": None
                 }
-        self.unsigned_endpoints = set(["dbs","ledgers","health", "new_keys", "nw_state", "version"])
+        self.unsigned_endpoints = set(["dbs", "ledgers", "health", "new_keys", "nw_state", "version"])
         self.use_get = set(["health", "new_keys", "nw_state", "version"])
         self.required = {}
         self.required["new_db"] = set(["db_id"])
         self.required["new_ledger"] = set(["ledger_id"])
         self.required["delete_db"] = set(["db_id"])
         self.required["delete_ledger"] = set(["ledger_id"])
         self.required["add_server"] = set(["server"])
         self.required["delete_server"] = set(["server"])
         self.optional = {"new_db": set(["snapshot"])}
-        self.optional = {"new_ledger": set(["snapshot"])}
+        self.optional = {"new_ledger": set(["snapshot","owners"])}
         self.implemented = set(["dbs",
                                 "ledgers",
                                 "new_keys",
                                 "health",
                                 "new_db",
                                 "new_ledger",
                                 "delete_db",
@@ -746,20 +749,35 @@
         required = set()
         if api_endpoint in self.required:
             required = self.required[api_endpoint]
         optional = set()
         if api_endpoint in self.optional:
             optional = self.optional[api_endpoint]
         if signed:
-            return _SignedPoster(self, self.session, self.signer, url, required, optional, self.ssl_verify_disabled, debug=self.debug)
+            return _SignedPoster(self,
+                                 self.session,
+                                 self.signer,
+                                 url,
+                                 required,
+                                 optional,
+                                 self.ssl_verify_disabled,
+                                 debug=self.debug)
         if use_get:
             if api_endpoint == "health":
                 return _UnsignedGetter(self.session, url, self.ssl_verify_disabled, ready="ready", debug=self.debug)
             return _UnsignedGetter(self.session, url, self.ssl_verify_disabled, debug=self.debug)
-        return _SignedPoster(self, self.session, self.signer, url, required, optional, self.ssl_verify_disabled, unsigned=True, debug=self.debug)
+        return _SignedPoster(self,
+                             self.session,
+                             self.signer,
+                             url,
+                             required,
+                             optional,
+                             self.ssl_verify_disabled,
+                             unsigned=True,
+                             debug=self.debug)
 
     async def __getitem__(self, key):
         """Square bracket operator
 
         Parameters
         ----------
         key : string
@@ -1629,14 +1647,15 @@
             Defined endpoint without library implementation (for now)
         AttributeError
             Undefined API endpoint invoked
         FlureeKeyRequired
             When 'command' endpoint is invoked in open-API mode.
         """
         debug = self.debug
+
         class _StringEndpoint:
             def __init__(self, api_endpoint, client, ssl_verify_disabled=False):
                 """Constructor
 
                 Parameters
                 ----------
                 api_endpoint : string
@@ -1718,15 +1737,15 @@
 
                 Returns
                 -------
                 string
                     Return body from server
                 """
                 if self.signer:
-                    if self.debug:
+                    if debug:
                         print("Signing with:", self.signer.auth_id)
                     body, headers, _ = self.signer.sign_query(query_body, querytype=self.api_endpoint)
                 else:
                     body = json.dumps(query_body, indent=4, sort_keys=True)
                     headers = {"Content-Type": contenttype}
                 return await self._post_body_with_headers(body, headers)
 
@@ -1741,15 +1760,15 @@
 
                 Returns
                 -------
                 string
                     Return body from server
 
                 """
-                if self.debug:
+                if debug:
                     print("Signing with:", self.signer.auth_id)
                 command = self.signer.sign_transaction(transact_obj, deps)
                 body = json.dumps(command, indent=4, sort_keys=True)
                 headers = {"content-type": "application/json"}
                 return await self._post_body_with_headers(body, headers)
 
             async def empty_post_unsigned(self):
```

### Comparing `aioflureedb-0.7.9/aioflureedb/__main__.py` & `aioflureedb-0.8.0/aioflureedb/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import asyncio
 import argparse
 import json
 from . import FlureeClient
 # from .domain_api import FlureeDomainAPI
 
+
 async def fluree_main(client, endpoint, data):
     """main for invoking single top level flureedb API endpoint
 
     Parameters
     ----------
     client: FlureeClient
         Flureedb API client object
@@ -22,34 +23,35 @@
     -------
     str
         response from API endpoint.
     """
     # pylint: disable=too-many-return-statements
     if endpoint is None:
         print("No endpoint specified, default to health")
-        endpoint="health"
+        endpoint = "health"
     if endpoint == "health":
         return await client.health()
     await client.health.ready()
     if endpoint == "dbs":
         return await client.dbs()
     if endpoint == "ledgers":
         return await client.ledgers()
     if endpoint == "new_keys":
         return await client.new_keys()
     if endpoint == "version":
         return await client.version()
     if endpoint == "new_db":
-        print("data: '", data , "'")
+        print("data: '", data ,"'")
         return await client.new_db(db_id=data)
     if endpoint == "new_ledger":
-        print("data: '", data , "'")
+        print("data: '", data, "'")
         return await client.new_ledger(db_id=data)
     return "Unknown endpoint:" + str(endpoint)
 
+
 async def database_main(client, dbase, endpoint, data, key):
     """Main for invoking DB specific FlureeDB database endpoints
 
 
     Parameters
     ----------
     client: FlureeClient
@@ -80,14 +82,15 @@
             return await database.history.actual_query(json.loads(data))
         if endpoint == "block":
             return await database.block.actual_query(json.loads(data))
         if endpoint == "command":
             return await database.command.transaction(json.loads(data))
     return "Unknown endpoint:" + str(endpoint)
 
+
 async def argparse_main():
     """Arguments parsting main"""
     # pylint: disable=too-many-locals,too-many-branches
     parsers = {}
     parsers["main"] = argparse.ArgumentParser()
     subparsers = parsers["main"].add_subparsers()
     subcommands = ["fluree", "database"]
@@ -177,24 +180,24 @@
         if args.datafile is not None:
             if args.datafile == "-":
                 inf = sys.stdin
             else:
                 inf = open(args.datafile, encoding="utf-8")
             data = inf.read()
     async with FlureeClient(args.masterkey,
-                          args.host,
-                          int(args.port),
-                          args.https != "false",
-                          args.sslverify != "false",
-                          float(args.sigvalidity),
-                          float(args.sigfuel)) as client:
+                            args.host,
+                            int(args.port),
+                            args.https != "false",
+                            args.sslverify != "false",
+                            float(args.sigvalidity),
+                            float(args.sigfuel)) as client:
         try:
             if args.subcommand == "fluree":
                 print(json.dumps(await fluree_main(client, args.endpoint, data), indent=2))
             elif args.subcommand == "database":
                 print(json.dumps(await database_main(client, args.db, args.endpoint, data, args.masterkey), indent=2))
-        except Exception as exp: # pylint: disable=broad-except
+        except Exception as exp:  # pylint: disable=broad-except
             print(exp)
 
 
 LOOP = asyncio.get_event_loop()
 LOOP.run_until_complete(argparse_main())
```

### Comparing `aioflureedb-0.7.9/aioflureedb/domain_api.py` & `aioflureedb-0.8.0/aioflureedb/domain_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 except ImportError:
     AIOFLUREEDB_HAS_JSONATA = False
 
     class JsonataContext:
         """Dummy Context for install witout jsonata"""
         def __init__(self, bigint_patch, debug_print):
             pass
+
         def __call__(self, xform, json_data):
             """We don't want to fail on import, we only want to fail on usage
 
             Parameters
             ----------
 
             xform : str
```

### Comparing `aioflureedb-0.7.9/aioflureedb/signing.py` & `aioflureedb-0.8.0/aioflureedb/signing.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         -------
         dict
             Python dict with command and signature fields.
         """
         obj = {}
         obj["type"] = "tx"
         obj["tx"] = transaction
-        obj["db"] = self.database
+        obj["ledger"] = self.database  # db -> ledger
         obj["auth"] = self.auth_id
         obj["fuel"] = self.fuel
         nonce = random.randint(0, 9007199254740991)
         obj["nonce"] = nonce
         obj["expire"] = int((time.time() + self.validity)*1000)
         if deps:
             obj["deps"] = deps
```

### Comparing `aioflureedb-0.7.9/aioflureedb.egg-info/PKG-INFO` & `aioflureedb-0.8.0/aioflureedb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.7.9
+Version: 0.8.0
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.7.9/setup.py` & `aioflureedb-0.8.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sys import platform
 here = path.abspath(path.dirname(__file__))
 
 requirements = ["starkbank-ecdsa>=2.0.3", "aiohttp", "base58"]
 
 setup(
     name='aioflureedb',
-    version='0.7.9',
+    version='0.8.0',
     description='Asynchonous library for usage of the FlureeDB API',
     long_description="""An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     """,
     url='https://github.com/pibara/aioflureedb',
     author='Rob J Meijer',
     author_email='pibara@gmail.com',
     license='BSD',
```

