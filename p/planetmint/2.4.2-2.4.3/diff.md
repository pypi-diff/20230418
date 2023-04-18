# Comparing `tmp/planetmint-2.4.2.tar.gz` & `tmp/planetmint-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint-2.4.2.tar", max compression
+gzip compressed data, was "planetmint-2.4.3.tar", max compression
```

## Comparing `planetmint-2.4.2.tar` & `planetmint-2.4.3.tar`

### file list

```diff
@@ -1,82 +1,80 @@
--rw-r--r--   0        0        0    34523 2023-04-14 09:37:53.850957 planetmint-2.4.2/LICENSE
--rw-r--r--   0        0        0     1614 2023-04-14 09:37:53.850957 planetmint-2.4.2/LICENSES.md
--rw-r--r--   0        0        0     3126 2023-04-14 09:37:53.850957 planetmint-2.4.2/README.md
--rw-r--r--   0        0        0     1796 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/README.md
--rw-r--r--   0        0        0      205 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/__init__.py
--rw-r--r--   0        0        0    10928 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/application_logic.py
--rw-r--r--   0        0        0      104 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/block.py
--rw-r--r--   0        0        0     4896 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/parallel_validation.py
--rw-r--r--   0        0        0     2994 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/rpc.py
--rw-r--r--   0        0        0     5291 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/abci/utils.py
--rw-r--r--   0        0        0       86 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/application/__init__.py
--rw-r--r--   0        0        0      833 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/application/basevalidationrules.py
--rw-r--r--   0        0        0    23655 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/application/validator.py
--rw-r--r--   0        0        0     2319 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/README.md
--rw-r--r--   0        0        0      705 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/__init__.py
--rw-r--r--   0        0        0     4496 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/connection.py
--rw-r--r--   0        0        0      891 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/exceptions.py
--rw-r--r--   0        0        0     1192 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/localmongodb/__init__.py
--rw-r--r--   0        0        0     6303 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/localmongodb/connection.py
--rw-r--r--   0        0        0     9498 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/localmongodb/query.py
--rw-r--r--   0        0        0     2995 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/localmongodb/schema.py
--rw-r--r--   0        0        0      438 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/__init__.py
--rw-r--r--   0        0        0      938 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/asset.py
--rw-r--r--   0        0        0      727 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/block.py
--rw-r--r--   0        0        0     3050 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/dbtransaction.py
--rw-r--r--   0        0        0      446 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/fulfills.py
--rw-r--r--   0        0        0     1971 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/input.py
--rw-r--r--   0        0        0      603 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/metadata.py
--rw-r--r--   0        0        0     4387 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/output.py
--rw-r--r--   0        0        0      600 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/models/script.py
--rw-r--r--   0        0        0    10645 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/query.py
--rw-r--r--   0        0        0     4826 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/schema.py
--rw-r--r--   0        0        0      127 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/__init__.py
--rw-r--r--   0        0        0      917 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/const.py
--rw-r--r--   0        0        0      457 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/opt/functions.lua
--rw-r--r--   0        0        0    11752 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/opt/init.lua
--rw-r--r--   0        0        0     2861 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/opt/migrations.lua
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/sync_io/__init__.py
--rw-r--r--   0        0        0     2714 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/sync_io/connection.py
--rw-r--r--   0        0        0    19127 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/sync_io/query.py
--rw-r--r--   0        0        0     1278 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/sync_io/schema.py
--rw-r--r--   0        0        0      916 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/tarantool/tarantool.md
--rw-r--r--   0        0        0     1123 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/backend/utils.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/commands/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/commands/election_types.py
--rw-r--r--   0        0        0    14309 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/commands/planetmint.py
--rw-r--r--   0        0        0     4976 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/commands/utils.py
--rw-r--r--   0        0        0     6711 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/config.py
--rw-r--r--   0        0        0    12361 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/config_utils.py
--rw-r--r--   0        0        0      401 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/const.py
--rw-r--r--   0        0        0      390 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/ipc/__init__.py
--rw-r--r--   0        0        0      951 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/ipc/events.py
--rw-r--r--   0        0        0     2195 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/ipc/exchange.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/model/__init__.py
--rw-r--r--   0        0        0    14086 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/model/dataaccessor.py
--rw-r--r--   0        0        0     3442 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/start.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/utils/lazy.py
--rw-r--r--   0        0        0     2253 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/utils/processes.py
--rw-r--r--   0        0        0      261 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/utils/python.py
--rw-r--r--   0        0        0      239 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/utils/singleton.py
--rw-r--r--   0        0        0      327 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/version.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/routes.py
--rw-r--r--   0        0        0     3671 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/server.py
--rw-r--r--   0        0        0      947 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/strip_content_type_middleware.py
--rw-r--r--   0        0        0        0 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/views/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/views/assets.py
--rw-r--r--   0        0        0     1525 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/views/base.py
--rw-r--r--   0        0        0     2345 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/views/blocks.py
--rw-r--r--   0        0        0     1817 2023-04-14 09:37:53.866958 planetmint-2.4.2/planetmint/web/views/info.py
--rw-r--r--   0        0        0     1428 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/views/metadata.py
--rw-r--r--   0        0        0     1455 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/views/outputs.py
--rw-r--r--   0        0        0     1631 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/views/parameters.py
--rw-r--r--   0        0        0     4785 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/views/transactions.py
--rw-r--r--   0        0        0      677 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/views/validators.py
--rw-r--r--   0        0        0     3548 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/websocket_dispatcher.py
--rw-r--r--   0        0        0     4906 2023-04-14 09:37:53.870958 planetmint-2.4.2/planetmint/web/websocket_server.py
--rw-r--r--   0        0        0     2664 2023-04-14 09:37:53.870958 planetmint-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-18 07:58:18.168430 planetmint-2.4.3/LICENSE
+-rw-r--r--   0        0        0     1614 2023-04-18 07:58:18.168430 planetmint-2.4.3/LICENSES.md
+-rw-r--r--   0        0        0     3126 2023-04-18 07:58:18.168430 planetmint-2.4.3/README.md
+-rw-r--r--   0        0        0     1796 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/README.md
+-rw-r--r--   0        0        0      205 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/__init__.py
+-rw-r--r--   0        0        0    10928 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/application_logic.py
+-rw-r--r--   0        0        0      104 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/block.py
+-rw-r--r--   0        0        0     4896 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/parallel_validation.py
+-rw-r--r--   0        0        0     2994 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/rpc.py
+-rw-r--r--   0        0        0     5291 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/abci/utils.py
+-rw-r--r--   0        0        0       86 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/application/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/application/basevalidationrules.py
+-rw-r--r--   0        0        0    23655 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/application/validator.py
+-rw-r--r--   0        0        0     2319 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/README.md
+-rw-r--r--   0        0        0      705 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/__init__.py
+-rw-r--r--   0        0        0     4496 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/connection.py
+-rw-r--r--   0        0        0      891 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/localmongodb/__init__.py
+-rw-r--r--   0        0        0     6303 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/localmongodb/connection.py
+-rw-r--r--   0        0        0     9498 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/localmongodb/query.py
+-rw-r--r--   0        0        0     2995 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/localmongodb/schema.py
+-rw-r--r--   0        0        0      438 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/asset.py
+-rw-r--r--   0        0        0      727 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/block.py
+-rw-r--r--   0        0        0     3050 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/dbtransaction.py
+-rw-r--r--   0        0        0      446 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/fulfills.py
+-rw-r--r--   0        0        0     1971 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/input.py
+-rw-r--r--   0        0        0      603 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/metadata.py
+-rw-r--r--   0        0        0     4387 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/output.py
+-rw-r--r--   0        0        0      600 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/models/script.py
+-rw-r--r--   0        0        0    10645 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/query.py
+-rw-r--r--   0        0        0     4516 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/schema.py
+-rw-r--r--   0        0        0      127 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/__init__.py
+-rw-r--r--   0        0        0      917 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/const.py
+-rw-r--r--   0        0        0    13754 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/opt/init.lua
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/sync_io/__init__.py
+-rw-r--r--   0        0        0     2714 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/sync_io/connection.py
+-rw-r--r--   0        0        0    19127 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/sync_io/query.py
+-rw-r--r--   0        0        0     1154 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/sync_io/schema.py
+-rw-r--r--   0        0        0      916 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/tarantool/tarantool.md
+-rw-r--r--   0        0        0     1123 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/backend/utils.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/commands/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/commands/election_types.py
+-rw-r--r--   0        0        0    14108 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/commands/planetmint.py
+-rw-r--r--   0        0        0     4976 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/commands/utils.py
+-rw-r--r--   0        0        0     6711 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/config.py
+-rw-r--r--   0        0        0    12361 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/config_utils.py
+-rw-r--r--   0        0        0      401 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/const.py
+-rw-r--r--   0        0        0      390 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/ipc/__init__.py
+-rw-r--r--   0        0        0      951 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/ipc/events.py
+-rw-r--r--   0        0        0     2195 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/ipc/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/model/__init__.py
+-rw-r--r--   0        0        0    14086 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/model/dataaccessor.py
+-rw-r--r--   0        0        0     3442 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/start.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/utils/lazy.py
+-rw-r--r--   0        0        0     2253 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/utils/processes.py
+-rw-r--r--   0        0        0      261 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/utils/python.py
+-rw-r--r--   0        0        0      239 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/utils/singleton.py
+-rw-r--r--   0        0        0      327 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/version.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/__init__.py
+-rw-r--r--   0        0        0     1341 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/routes.py
+-rw-r--r--   0        0        0     3671 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/server.py
+-rw-r--r--   0        0        0      947 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/strip_content_type_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/assets.py
+-rw-r--r--   0        0        0     1525 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/base.py
+-rw-r--r--   0        0        0     2345 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/blocks.py
+-rw-r--r--   0        0        0     1817 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/info.py
+-rw-r--r--   0        0        0     1428 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/metadata.py
+-rw-r--r--   0        0        0     1464 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/outputs.py
+-rw-r--r--   0        0        0     1631 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/parameters.py
+-rw-r--r--   0        0        0     4785 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/transactions.py
+-rw-r--r--   0        0        0      677 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/views/validators.py
+-rw-r--r--   0        0        0     3548 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/websocket_dispatcher.py
+-rw-r--r--   0        0        0     4906 2023-04-18 07:58:18.184432 planetmint-2.4.3/planetmint/web/websocket_server.py
+-rw-r--r--   0        0        0     2664 2023-04-18 07:58:18.188433 planetmint-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 planetmint-2.4.3/PKG-INFO
```

### Comparing `planetmint-2.4.2/LICENSE` & `planetmint-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/LICENSES.md` & `planetmint-2.4.3/LICENSES.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/README.md` & `planetmint-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/README.md` & `planetmint-2.4.3/planetmint/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/abci/application_logic.py` & `planetmint-2.4.3/planetmint/abci/application_logic.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/abci/parallel_validation.py` & `planetmint-2.4.3/planetmint/abci/parallel_validation.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/abci/rpc.py` & `planetmint-2.4.3/planetmint/abci/rpc.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/abci/utils.py` & `planetmint-2.4.3/planetmint/abci/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/application/basevalidationrules.py` & `planetmint-2.4.3/planetmint/application/basevalidationrules.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/application/validator.py` & `planetmint-2.4.3/planetmint/application/validator.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/README.md` & `planetmint-2.4.3/planetmint/backend/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/__init__.py` & `planetmint-2.4.3/planetmint/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/connection.py` & `planetmint-2.4.3/planetmint/backend/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/exceptions.py` & `planetmint-2.4.3/planetmint/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/localmongodb/__init__.py` & `planetmint-2.4.3/planetmint/backend/localmongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/localmongodb/connection.py` & `planetmint-2.4.3/planetmint/backend/localmongodb/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/localmongodb/query.py` & `planetmint-2.4.3/planetmint/backend/localmongodb/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/localmongodb/schema.py` & `planetmint-2.4.3/planetmint/backend/localmongodb/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/asset.py` & `planetmint-2.4.3/planetmint/backend/models/asset.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/block.py` & `planetmint-2.4.3/planetmint/backend/models/block.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/dbtransaction.py` & `planetmint-2.4.3/planetmint/backend/models/dbtransaction.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/input.py` & `planetmint-2.4.3/planetmint/backend/models/input.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/metadata.py` & `planetmint-2.4.3/planetmint/backend/models/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/output.py` & `planetmint-2.4.3/planetmint/backend/models/output.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/models/script.py` & `planetmint-2.4.3/planetmint/backend/models/script.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/query.py` & `planetmint-2.4.3/planetmint/backend/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/schema.py` & `planetmint-2.4.3/planetmint/backend/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,28 +134,16 @@
             configuration.
     """
 
     raise NotImplementedError
 
 
 @singledispatch
-def migrate_up(connection):
-    """Migrate database up
-
-    Args:
-        connection (:class:`~planetmint.backend.connection.Connection`): an
-            existing connection to use to migrate the database.
-            Creates one if not given.
-    """
-    raise NotImplementedError
-
-
-@singledispatch
-def migrate_down(connection):
-    """Migrate database down
+def migrate(connection):
+    """Migrate database
 
     Args:
         connection (:class:`~planetmint.backend.connection.Connection`): an
             existing connection to use to migrate the database.
             Creates one if not given.
     """
     raise NotImplementedError
```

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/const.py` & `planetmint-2.4.3/planetmint/backend/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/opt/init.lua` & `planetmint-2.4.3/planetmint/backend/tarantool/opt/init.lua`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-local migrations = require('migrations')
+local fiber = require('fiber')
 
 box.cfg{listen = 3303}
 
 box.once("bootstrap", function()
     box.schema.user.grant('guest','read,write,execute,create,drop','universe')
 end)
 
@@ -330,16 +330,68 @@
     return result_set
 end
 
 function delete_output( id )
     box.space.outputs:delete(id)
 end
 
-function migrate_up()
-    migrations.update_utxo_13042023.up()
-    -- add newer migrations below
+function atomic(batch_size, iter, fn)
+    box.atomic(function()
+        local i = 0
+        for _, x in iter:unwrap() do
+            fn(x)
+            i = i + 1
+            if i % batch_size == 0 then
+                box.commit()
+                fiber.yield() -- for read-only operations when `commit` doesn't yield
+                box.begin()
+            end
+        end
+    end)
 end
 
-function migrate_down()
-    -- add newer migrations above
-    migrations.update_utxo_13042023.down()
-end
+function migrate()
+    -- migration code from 2.4.0 to 2.4.3
+    box.once("planetmint:v2.4.3", function()
+        box.space.utxos:drop()
+        utxos = box.schema.create_space('utxos', { if_not_exists = true })
+        utxos:format({
+            { name = 'id', type = 'string' },
+            { name = 'amount' , type = 'unsigned' },
+            { name = 'public_keys', type = 'array' },
+            { name = 'condition', type = 'map' },
+            { name = 'output_index', type = 'number' },
+            { name = 'transaction_id' , type = 'string' }
+        })
+        utxos:create_index('id', { 
+            if_not_exists = true,
+            parts = {{ field = 'id', type = 'string' }}
+        })
+        utxos:create_index('utxos_by_transaction_id', {
+            if_not_exists = true,
+            unique = false,
+            parts = {{ field = 'transaction_id', type = 'string' }}
+        })
+        utxos:create_index('utxo_by_transaction_id_and_output_index', { 
+            if_not_exists = true,
+            parts = {
+                { field = 'transaction_id', type = 'string' },
+                { field = 'output_index', type = 'unsigned' }
+            }
+        })
+        utxos:create_index('public_keys', { 
+            if_not_exists = true,
+            unique = false,
+            parts = {{field = 'public_keys[*]', type  = 'string' }}
+        })
+
+        atomic(1000, outputs:pairs(), function(output)
+            utxos:insert{output[0], output[1], output[2], output[3], output[4], output[5]}
+        end)
+        atomic(1000, utxos:pairs(), function(utxo) 
+            spending_transaction = transactions.index.spending_transaction_by_id_and_output_index:select{utxo[5], utxo[4]}
+            if table.getn(spending_transaction) > 0 then
+                utxos:delete(utxo[0])
+            end
+        end)
+    end)
+end
```

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/sync_io/connection.py` & `planetmint-2.4.3/planetmint/backend/tarantool/sync_io/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/sync_io/query.py` & `planetmint-2.4.3/planetmint/backend/tarantool/sync_io/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/sync_io/schema.py` & `planetmint-2.4.3/planetmint/backend/tarantool/sync_io/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,9 @@
 
 @register_schema(TarantoolDBConnection)
 def create_tables(connection, dbname):
     connection.connect().call("init")
 
 
 @register_schema(TarantoolDBConnection)
-def migrate_up(connection):
-    connection.connect().call("migrate_up")
-
-
-@register_schema(TarantoolDBConnection)
-def migrate_down(connection):
-    connection.connect().call("migrate_down")
+def migrate(connection):
+    connection.connect().call("migrate")
```

### Comparing `planetmint-2.4.2/planetmint/backend/tarantool/tarantool.md` & `planetmint-2.4.3/planetmint/backend/tarantool/tarantool.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/backend/utils.py` & `planetmint-2.4.3/planetmint/backend/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/commands/election_types.py` & `planetmint-2.4.3/planetmint/commands/election_types.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/commands/planetmint.py` & `planetmint-2.4.3/planetmint/commands/planetmint.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,23 +255,17 @@
 @configure_planetmint
 def run_init(args):
     """Initialize the database"""
     _run_init()
 
 
 @configure_planetmint
-def run_migrate_up(args):
+def run_migrate(args):
     validator = Validator()
-    schema.migrate_up(validator.models.connection)
-
-
-@configure_planetmint
-def run_migrate_down(args):
-    validator = Validator()
-    schema.migrate_up(validator.models.connection)
+    schema.migrate(validator.models.connection)
 
 
 @configure_planetmint
 def run_drop(args):
     """Drop the database"""
 
     if not args.yes:
@@ -373,16 +367,14 @@
     # parser for database-level commands
     subparsers.add_parser("init", help="Init the database")
 
     subparsers.add_parser("drop", help="Drop the database")
 
     subparsers.add_parser("migrate_up", help="Migrate up")
 
-    subparsers.add_parser("migrate_down", help="Migrate down")
-
     # parser for starting Planetmint
     start_parser = subparsers.add_parser("start", help="Start Planetmint")
 
     start_parser.add_argument(
         "--no-init",
         dest="skip_initialize_database",
         default=False,
```

### Comparing `planetmint-2.4.2/planetmint/commands/utils.py` & `planetmint-2.4.3/planetmint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/config.py` & `planetmint-2.4.3/planetmint/config.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/config_utils.py` & `planetmint-2.4.3/planetmint/config_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/ipc/events.py` & `planetmint-2.4.3/planetmint/ipc/events.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/ipc/exchange.py` & `planetmint-2.4.3/planetmint/ipc/exchange.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/model/dataaccessor.py` & `planetmint-2.4.3/planetmint/model/dataaccessor.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/start.py` & `planetmint-2.4.3/planetmint/start.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/utils/lazy.py` & `planetmint-2.4.3/planetmint/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/utils/processes.py` & `planetmint-2.4.3/planetmint/utils/processes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/routes.py` & `planetmint-2.4.3/planetmint/web/routes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/server.py` & `planetmint-2.4.3/planetmint/web/server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/strip_content_type_middleware.py` & `planetmint-2.4.3/planetmint/web/strip_content_type_middleware.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/assets.py` & `planetmint-2.4.3/planetmint/web/views/assets.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/base.py` & `planetmint-2.4.3/planetmint/web/views/base.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/blocks.py` & `planetmint-2.4.3/planetmint/web/views/blocks.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/info.py` & `planetmint-2.4.3/planetmint/web/views/info.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/metadata.py` & `planetmint-2.4.3/planetmint/web/views/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/outputs.py` & `planetmint-2.4.3/planetmint/web/views/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,8 +28,8 @@
                 outputs = validator.models.get_outputs_filtered(args["public_key"], args["spent"])
             except Exception as e:
                 return make_error(
                     500,
                     "Invalid output ({}): {} : {} - {}".format(type(e).__name__, e, args["public_key"], args["spent"]),
                     level="error",
                 )
-            return [{"transaction_id": output.txid, "output_index": output.output} for output in outputs]
+            return [{"transaction_id": output.transaction_id, "output_index": output.index} for output in outputs]
```

### Comparing `planetmint-2.4.2/planetmint/web/views/parameters.py` & `planetmint-2.4.3/planetmint/web/views/parameters.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/transactions.py` & `planetmint-2.4.3/planetmint/web/views/transactions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/views/validators.py` & `planetmint-2.4.3/planetmint/web/views/validators.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/websocket_dispatcher.py` & `planetmint-2.4.3/planetmint/web/websocket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/planetmint/web/websocket_server.py` & `planetmint-2.4.3/planetmint/web/websocket_server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.2/pyproject.toml` & `planetmint-2.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint"
-version = "2.4.2"
+version = "2.4.3"
 description = "Planetmint: The Blockchain Database"
 authors = ["Planetmint contributors"]
 license = "AGPLv3"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
```

### Comparing `planetmint-2.4.2/PKG-INFO` & `planetmint-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint
-Version: 2.4.2
+Version: 2.4.3
 Summary: Planetmint: The Blockchain Database
 License: AGPLv3
 Author: Planetmint contributors
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

