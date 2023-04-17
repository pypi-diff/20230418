# Comparing `tmp/dipdup-6.5.4.tar.gz` & `tmp/dipdup-6.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-6.5.4.tar", max compression
+gzip compressed data, was "dipdup-6.5.5.tar", max compression
```

## Comparing `dipdup-6.5.4.tar` & `dipdup-6.5.5.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0     1067 2023-03-31 18:14:08.338169 dipdup-6.5.4/LICENSE
--rw-r--r--   0        0        0     2787 2023-03-31 18:14:08.338169 dipdup-6.5.4/README.md
--rw-r--r--   0        0        0     2778 2023-03-31 18:14:08.374170 dipdup-6.5.4/pyproject.toml
--rw-r--r--   0        0        0      557 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/__init__.py
--rw-r--r--   0        0        0      106 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/__main__.py
--rw-r--r--   0        0        0      585 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/baking_bad.py
--rw-r--r--   0        0        0    19101 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/cli.py
--rw-r--r--   0        0        0    22171 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/codegen.py
--rw-r--r--   0        0        0    69504 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/config.py
--rw-r--r--   0        0        0    25902 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/context.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/coinbase/__init__.py
--rw-r--r--   0        0        0     2387 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/coinbase/datasource.py
--rw-r--r--   0        0        0     1309 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/coinbase/models.py
--rw-r--r--   0        0        0     6250 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/datasource.py
--rw-r--r--   0        0        0     2420 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/factory.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/ipfs/__init__.py
--rw-r--r--   0        0        0      688 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/ipfs/datasource.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/metadata/__init__.py
--rw-r--r--   0        0        0     1773 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/metadata/datasource.py
--rw-r--r--   0        0        0      155 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/metadata/enums.py
--rw-r--r--   0        0        0     2172 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/subscription.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/tzkt/__init__.py
--rw-r--r--   0        0        0    46860 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/tzkt/datasource.py
--rw-r--r--   0        0        0     9895 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/datasources/tzkt/models.py
--rw-r--r--   0        0        0    24980 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     2013 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/enums.py
--rw-r--r--   0        0        0     2192 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/env.py
--rw-r--r--   0        0        0    10487 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     2734 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/fetcher.py
--rw-r--r--   0        0        0    25590 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/hasura.py
--rw-r--r--   0        0        0     9870 2023-03-31 18:14:08.374170 dipdup-6.5.4/src/dipdup/http.py
--rw-r--r--   0        0        0     7414 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/big_map/__init__.py
--rw-r--r--   0        0        0     3033 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/big_map/fetcher.py
--rw-r--r--   0        0        0     7103 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/big_map/index.py
--rw-r--r--   0        0        0     2131 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/big_map/matcher.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/event/__init__.py
--rw-r--r--   0        0        0     1402 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/event/fetcher.py
--rw-r--r--   0        0        0     5324 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/event/index.py
--rw-r--r--   0        0        0     3297 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/event/matcher.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/head/__init__.py
--rw-r--r--   0        0        0     2320 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/head/index.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/operation/__init__.py
--rw-r--r--   0        0        0    19397 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/operation/fetcher.py
--rw-r--r--   0        0        0    13344 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/operation/index.py
--rw-r--r--   0        0        0     7386 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/operation/matcher.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/token_transfer/__init__.py
--rw-r--r--   0        0        0     1357 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/token_transfer/fetcher.py
--rw-r--r--   0        0        0     5377 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/token_transfer/index.py
--rw-r--r--   0        0        0     1791 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/indexes/token_transfer/matcher.py
--rwxr-xr-x   0        0        0     8269 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/install.py
--rw-r--r--   0        0        0    22523 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/models.py
--rw-r--r--   0        0        0    10968 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/project.py
--rw-r--r--   0        0        0      203 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0     2097 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      431 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/Dockerfile.j2
--rw-r--r--   0        0        0      474 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      489 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/dipdup.dev.yml.j2
--rw-r--r--   0        0        0      481 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/dipdup.prod.yml.j2
--rw-r--r--   0        0        0     2907 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/docker-compose.swarm.yml.j2
--rw-r--r--   0        0        0     1341 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/docker-compose.yml.j2
--rw-r--r--   0        0        0       37 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/replay.json.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0      197 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
--rw-r--r--   0        0        0      128 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/blank/dipdup.yml.j2
--rw-r--r--   0        0        0       95 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-auction.json
--rw-r--r--   0        0        0       98 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-big-maps.json
--rw-r--r--   0        0        0       83 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-dao.json
--rw-r--r--   0        0        0       83 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-dex.json
--rw-r--r--   0        0        0       95 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-domains.json
--rw-r--r--   0        0        0       92 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-events.json
--rw-r--r--   0        0        0      101 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-factories.json
--rw-r--r--   0        0        0       86 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-head.json
--rw-r--r--   0        0        0      119 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-nft-marketplace.json
--rw-r--r--   0        0        0       83 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-raw.json
--rw-r--r--   0        0        0      119 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-token-transfers.json
--rw-r--r--   0        0        0       89 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo-token.json
--rw-r--r--   0        0        0     1116 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      918 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1624 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      853 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1524 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      779 2023-03-31 18:14:08.378170 dipdup-6.5.4/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      847 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1713 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      840 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      702 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dao/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      416 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     4878 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0     1842 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1769 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      587 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1642 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1689 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1039 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      960 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1868 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1795 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      581 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1636 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1655 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1160 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      956 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      948 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      900 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      564 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      536 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1475 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      819 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      592 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_events/dipdup.yml.j2
--rw-r--r--   0        0        0      976 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      716 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      416 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      333 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_head/dipdup.yml.j2
--rw-r--r--   0        0        0     1230 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      586 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1018 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      949 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      866 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1382 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      486 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_raw/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      350 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      235 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      787 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      453 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      647 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      945 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      456 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      550 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      822 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     1226 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/linters_default/Makefile.j2
--rw-r--r--   0        0        0     1032 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/linters_default/pyproject.toml.j2
--rw-r--r--   0        0        0      923 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/linters_none/Makefile.j2
--rw-r--r--   0        0        0      552 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/projects/linters_none/pyproject.toml.j2
--rw-r--r--   0        0        0     4008 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/py.typed
--rw-r--r--   0        0        0     4845 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     6041 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0      227 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0      157 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/templates/models.py.j2
--rw-r--r--   0        0        0     3029 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/transactions.py
--rw-r--r--   0        0        0     4631 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/utils/__init__.py
--rw-r--r--   0        0        0     1824 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/utils/codegen.py
--rw-r--r--   0        0        0    11813 2023-03-31 18:14:08.382170 dipdup-6.5.4/src/dipdup/utils/database.py
--rw-r--r--   0        0        0     2044 2023-03-31 18:14:08.386170 dipdup-6.5.4/src/dipdup/utils/sys.py
--rw-r--r--   0        0        0     4097 2023-03-31 18:14:08.386170 dipdup-6.5.4/src/dipdup/yaml.py
--rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 dipdup-6.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-17 23:05:28.327453 dipdup-6.5.5/LICENSE
+-rw-r--r--   0        0        0     2787 2023-04-17 23:05:28.327453 dipdup-6.5.5/README.md
+-rw-r--r--   0        0        0     2778 2023-04-17 23:05:28.355454 dipdup-6.5.5/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      585 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/baking_bad.py
+-rw-r--r--   0        0        0    18507 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/cli.py
+-rw-r--r--   0        0        0    22289 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/codegen.py
+-rw-r--r--   0        0        0    69778 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/config.py
+-rw-r--r--   0        0        0    25902 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/context.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/__init__.py
+-rw-r--r--   0        0        0     2387 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/datasource.py
+-rw-r--r--   0        0        0     1309 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/coinbase/models.py
+-rw-r--r--   0        0        0     6291 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/datasource.py
+-rw-r--r--   0        0        0     2420 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/factory.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/ipfs/__init__.py
+-rw-r--r--   0        0        0      688 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/ipfs/datasource.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/__init__.py
+-rw-r--r--   0        0        0     1773 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/datasource.py
+-rw-r--r--   0        0        0      155 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/metadata/enums.py
+-rw-r--r--   0        0        0     2172 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/subscription.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/tzkt/__init__.py
+-rw-r--r--   0        0        0    46886 2023-04-17 23:05:28.355454 dipdup-6.5.5/src/dipdup/datasources/tzkt/datasource.py
+-rw-r--r--   0        0        0     9895 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/datasources/tzkt/models.py
+-rw-r--r--   0        0        0    24980 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     2013 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/enums.py
+-rw-r--r--   0        0        0     2192 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/env.py
+-rw-r--r--   0        0        0     9500 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     2734 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0    25590 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/hasura.py
+-rw-r--r--   0        0        0     9795 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/http.py
+-rw-r--r--   0        0        0     7414 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/__init__.py
+-rw-r--r--   0        0        0     3033 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/fetcher.py
+-rw-r--r--   0        0        0     7103 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/index.py
+-rw-r--r--   0        0        0     2131 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/big_map/matcher.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/__init__.py
+-rw-r--r--   0        0        0     1402 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/fetcher.py
+-rw-r--r--   0        0        0     5324 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/index.py
+-rw-r--r--   0        0        0     3297 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/event/matcher.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/head/__init__.py
+-rw-r--r--   0        0        0     2320 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/head/index.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/__init__.py
+-rw-r--r--   0        0        0    19397 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/fetcher.py
+-rw-r--r--   0        0        0    13344 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/index.py
+-rw-r--r--   0        0        0     7386 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/operation/matcher.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/__init__.py
+-rw-r--r--   0        0        0     1357 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/fetcher.py
+-rw-r--r--   0        0        0     5377 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/index.py
+-rw-r--r--   0        0        0     1791 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/indexes/token_transfer/matcher.py
+-rwxr-xr-x   0        0        0     8269 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/install.py
+-rw-r--r--   0        0        0    22523 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/models.py
+-rw-r--r--   0        0        0    10978 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/project.py
+-rw-r--r--   0        0        0      203 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0     2097 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0      431 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/Dockerfile.j2
+-rw-r--r--   0        0        0      474 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      489 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/dipdup.dev.yml.j2
+-rw-r--r--   0        0        0      481 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/dipdup.prod.yml.j2
+-rw-r--r--   0        0        0     2907 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/docker-compose.swarm.yml.j2
+-rw-r--r--   0        0        0     1341 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/docker-compose.yml.j2
+-rw-r--r--   0        0        0       37 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/replay.json.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
+-rw-r--r--   0        0        0      197 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
+-rw-r--r--   0        0        0      128 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/blank/dipdup.yml.j2
+-rw-r--r--   0        0        0       95 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-auction.json
+-rw-r--r--   0        0        0       98 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-big-maps.json
+-rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-dao.json
+-rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-dex.json
+-rw-r--r--   0        0        0       95 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-domains.json
+-rw-r--r--   0        0        0       92 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-events.json
+-rw-r--r--   0        0        0      101 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-factories.json
+-rw-r--r--   0        0        0       86 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-head.json
+-rw-r--r--   0        0        0      119 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-nft-marketplace.json
+-rw-r--r--   0        0        0       83 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-raw.json
+-rw-r--r--   0        0        0      119 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-token-transfers.json
+-rw-r--r--   0        0        0       89 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo-token.json
+-rw-r--r--   0        0        0     1116 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      918 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1624 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      853 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1524 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      779 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      847 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1713 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      840 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      702 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_dao/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.359454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      416 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     4878 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0     1842 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1769 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      587 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1642 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1689 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1039 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      960 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1868 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1795 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      581 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1636 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1655 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1160 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      956 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      948 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      900 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      564 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      536 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1475 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      819 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      592 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_events/dipdup.yml.j2
+-rw-r--r--   0        0        0      976 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      716 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
+-rw-r--r--   0        0        0      416 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      523 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      858 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      333 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_head/dipdup.yml.j2
+-rw-r--r--   0        0        0     1230 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      586 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1018 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      949 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      866 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1382 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      486 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      350 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      235 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      787 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      453 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      647 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      945 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0      456 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
+-rw-r--r--   0        0        0      550 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      822 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      389 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
+-rw-r--r--   0        0        0     1226 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_default/Makefile.j2
+-rw-r--r--   0        0        0     1032 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_default/pyproject.toml.j2
+-rw-r--r--   0        0        0      923 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_none/Makefile.j2
+-rw-r--r--   0        0        0      552 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/projects/linters_none/pyproject.toml.j2
+-rw-r--r--   0        0        0     4008 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/py.typed
+-rw-r--r--   0        0        0     4845 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     6041 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0      227 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0      157 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/templates/models.py.j2
+-rw-r--r--   0        0        0     3029 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     4631 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/codegen.py
+-rw-r--r--   0        0        0    11813 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/database.py
+-rw-r--r--   0        0        0     2044 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/utils/sys.py
+-rw-r--r--   0        0        0     4513 2023-04-17 23:05:28.363454 dipdup-6.5.5/src/dipdup/yaml.py
+-rw-r--r--   0        0        0     4690 1970-01-01 00:00:00.000000 dipdup-6.5.5/PKG-INFO
```

### Comparing `dipdup-6.5.4/LICENSE` & `dipdup-6.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/README.md` & `dipdup-6.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/pyproject.toml` & `dipdup-6.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dipdup"
 description = "Modular framework for creating selective indexers and featureful backends for dapps"
-version = "6.5.4"
+version = "6.5.5"
 license = "MIT"
 authors = [
     "Lev Gorodetskiy <dipdup@drsr.io>",
     "Michael Zaikin <mz@baking-bad.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/dipdup-io/dipdup"
@@ -27,27 +27,27 @@
     { include = "dipdup", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 
 asyncpg = "0.27.0"
-datamodel-code-generator = "0.17.2"
+datamodel-code-generator = "0.18.0"
 pydantic = "1.10.7"
-pysignalr = "0.1.2"
 tortoise-orm = "0.19.3"
 
 aiohttp = "^3.8.1"
 aiolimiter = "^1.0.0"
 anyio = "^3.3.2"
 APScheduler = "^3.8.0"
 asyncclick = "^8.0.1"
 orjson = "^3.6.6"
 prometheus-client = "^0.14.1"
 pyhumps = "^3.0.2"
+pysignalr = "0.2.0"
 python-dotenv = "^0.19.0"
 "ruamel.yaml" = "^0.17.2"
 sentry-sdk = "^1.4.3"
 sqlparse = "^0.4.2"
 tabulate = "^0.9.0"
 
 pytezos = {version = "3.9.0", optional = true}
```

### Comparing `dipdup-6.5.4/src/dipdup/baking_bad.py` & `dipdup-6.5.5/src/dipdup/baking_bad.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/cli.py` & `dipdup-6.5.5/src/dipdup/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,16 @@
 from typing import Awaitable
 from typing import Callable
 from typing import TypeVar
 from typing import cast
 
 import asyncclick as click
 
-from dipdup import __spec_version__
 from dipdup import __version__
 from dipdup import env
-from dipdup import spec_reindex_mapping
-from dipdup import spec_version_mapping
 from dipdup.utils.sys import IGNORE_CONFIG_CMDS
 from dipdup.utils.sys import set_up_logging
 from dipdup.utils.sys import set_up_process
 
 DEFAULT_CONFIG_NAME = 'dipdup.yml'
 
 
@@ -155,15 +152,14 @@
 
     from dataclasses import dataclass
 
     from dipdup.codegen import CodeGenerator
     from dipdup.config import DipDupConfig
     from dipdup.exceptions import ConfigurationError
     from dipdup.exceptions import InitializationRequiredError
-    from dipdup.exceptions import MigrationRequiredError
     from dipdup.sentry import init_sentry
 
     _config = DipDupConfig.load(config_paths)
     _config.set_up_logging()
 
     init_sentry(_config)
 
@@ -176,21 +172,14 @@
 
     # NOTE: Avoid import errors if project package is incomplete
     try:
         CodeGenerator(_config, {}).create_package()
     except Exception as e:
         raise InitializationRequiredError(f'Failed to create a project package: {e}') from e
 
-    # NOTE: Ensure that `spec_version` is valid and supported
-    if _config.spec_version not in spec_version_mapping:
-        raise ConfigurationError(f'Unknown `spec_version`, correct ones: {", ".join(spec_version_mapping)}')
-    if _config.spec_version != __spec_version__:
-        reindex = spec_reindex_mapping[__spec_version__]
-        raise MigrationRequiredError(_config.spec_version, __spec_version__, reindex)
-
     @dataclass
     class CLIContext:
         config_paths: list[str]
         config: DipDupConfig
 
     ctx.obj = CLIContext(
         config_paths=config,
```

### Comparing `dipdup-6.5.4/src/dipdup/codegen.py` & `dipdup-6.5.5/src/dipdup/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,14 +383,18 @@
             '--input',
             str(schema_path),
             '--output',
             str(output_path),
             '--class-name',
             class_name,
             '--disable-timestamp',
+            '--input-file-type',
+            'jsonschema',
+            '--target-python-version',
+            '3.10',
         ]
         self._logger.debug(' '.join(args))
         subprocess.run(args, check=True)
 
     async def generate_types(self, overwrite_types: bool = False) -> None:
         """Generate typeclasses from fetched JSONSchemas: contract's storage, parameters, big maps and events."""
```

### Comparing `dipdup-6.5.4/src/dipdup/config.py` & `dipdup-6.5.5/src/dipdup/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -624,16 +624,14 @@
     optional: bool = False
     alias: str | None = None
 
     def __post_init_post_parse__(self) -> None:
         StorageTypeMixin.__post_init_post_parse__(self)
         ParameterTypeMixin.__post_init_post_parse__(self)
         SubgroupIndexMixin.__post_init_post_parse__(self)
-        if self.entrypoint and not self.destination:
-            raise ConfigurationError('Transactions with entrypoint must also have destination')
 
     def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
         if self.typed_contract:
             module_name = self.typed_contract.module_name
             yield 'dipdup.models', 'Transaction'
             yield self.format_parameter_import(
                 package,
@@ -1688,14 +1686,21 @@
             if not isinstance(datasource_config, TzktDatasourceConfig):
                 continue
             if datasource_config.buffer_size and self.advanced.rollback_depth:
                 raise ConfigurationError(
                     f'`{name}`: `buffer_size` option is incompatible with `advanced.rollback_depth`'
                 )
 
+        # NOTE: Bigmap indexes with `skip_history` require early realtime
+        for name, index_config in self.indexes.items():
+            if isinstance(index_config, BigMapIndexConfig) and index_config.skip_history != SkipHistory.never:
+                _logger.warning('`%s` index is configured to skip history; enabling early realtime', name)
+                self.advanced.early_realtime = True
+                break
+
     def _resolve_template(self, template_config: IndexTemplateConfig) -> None:
         _logger.debug('Resolving index config `%s` from template `%s`', template_config.name, template_config.template)
 
         template = self.get_template(template_config.template)
         raw_template = json.dumps(template, default=pydantic_encoder)
         for key, value in template_config.values.items():
             value_regex = r'<[ ]*' + key + r'[ ]*>'
```

### Comparing `dipdup-6.5.4/src/dipdup/context.py` & `dipdup-6.5.5/src/dipdup/context.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/coinbase/datasource.py` & `dipdup-6.5.5/src/dipdup/datasources/coinbase/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/coinbase/models.py` & `dipdup-6.5.5/src/dipdup/datasources/coinbase/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/datasource.py` & `dipdup-6.5.5/src/dipdup/datasources/datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 TokenTransfersCallbackT = Callable[['IndexDatasource', Tuple[TokenTransferData, ...]], Awaitable[None]]
 BigMapsCallbackT = Callable[['IndexDatasource', Tuple[BigMapData, ...]], Awaitable[None]]
 EventsCallbackT = Callable[['IndexDatasource', Tuple[EventData, ...]], Awaitable[None]]
 RollbackCallbackT = Callable[['IndexDatasource', MessageType, int, int], Awaitable[None]]
 
 
 class Datasource(HTTPGateway):
+    _default_http_config = HTTPConfig()
+
     def __init__(self, url: str, http_config: HTTPConfig | None = None) -> None:
         config = ResolvedHTTPConfig.create(self._default_http_config, http_config)
         super().__init__(url, config)
         self._logger = _logger
 
     @abstractmethod
     async def run(self) -> None:
```

### Comparing `dipdup-6.5.4/src/dipdup/datasources/factory.py` & `dipdup-6.5.5/src/dipdup/datasources/factory.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/ipfs/datasource.py` & `dipdup-6.5.5/src/dipdup/datasources/ipfs/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/metadata/datasource.py` & `dipdup-6.5.5/src/dipdup/datasources/metadata/datasource.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/subscription.py` & `dipdup-6.5.5/src/dipdup/datasources/subscription.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/datasources/tzkt/datasource.py` & `dipdup-6.5.5/src/dipdup/datasources/tzkt/datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -906,15 +906,15 @@
     async def _send(
         self,
         method: str,
         arguments: list[dict[str, Any]],
         on_invocation: Callable[[CompletionMessage], Awaitable[None]] | None = None,
     ) -> None:
         client = self._get_signalr_client()
-        await client.send(method, arguments, on_invocation)
+        await client.send(method, arguments, on_invocation)  # type: ignore[arg-type]
 
     async def _on_connected(self) -> None:
         self._logger.info('Realtime connection established')
         # NOTE: Subscribing here will block WebSocket loop, don't do it.
         await self.emit_connected()
 
     async def _on_disconnected(self) -> None:
```

### Comparing `dipdup-6.5.4/src/dipdup/datasources/tzkt/models.py` & `dipdup-6.5.5/src/dipdup/datasources/tzkt/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/dipdup.py` & `dipdup-6.5.5/src/dipdup/dipdup.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/enums.py` & `dipdup-6.5.5/src/dipdup/enums.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/env.py` & `dipdup-6.5.5/src/dipdup/env.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/exceptions.py` & `dipdup-6.5.5/src/dipdup/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Type
 
-from tabulate import tabulate
 from tortoise.models import Model
 
-from dipdup import spec_version_mapping
 from dipdup.enums import ReindexingReason
 
 tab = ('_' * 80) + '\n\n'
 
 
 def unindent(text: str) -> str:
     """Remove indentation from text"""
@@ -158,45 +156,14 @@
             See https://docs.dipdup.io/deployment/database-engines
             See https://docs.dipdup.io/advanced/sql
             See https://docs.dipdup.io/config/database
         """
 
 
 @dataclass(repr=False)
-class MigrationRequiredError(Error):
-    """Project and DipDup spec versions don't match"""
-
-    from_: str
-    to: str
-    reindex: bool = False
-
-    def _help(self) -> str:
-        version_table = tabulate(
-            [
-                ['current', self.from_, spec_version_mapping[self.from_]],
-                ['required', self.to, spec_version_mapping[self.to]],
-            ],
-            headers=['', 'spec_version', 'DipDup version'],
-        )
-        reindex = '\n\n' + tab + ReindexingRequiredError(ReindexingReason.migration).help() if self.reindex else ''
-        return f"""
-            Project migration required!
-
-            {version_table.strip()}
-
-            Perform the following actions:
-
-              1. Run `dipdup migrate`.
-              2. Review and commit changes.
-
-            See https://docs.dipdup.io/release-notes for more information. {reindex}
-        """
-
-
-@dataclass(repr=False)
 class ReindexingRequiredError(Error):
     """Unable to continue indexing with existing database"""
 
     reason: ReindexingReason
     context: Dict[str, Any] = field(default_factory=dict)
 
     def _help(self) -> str:
```

### Comparing `dipdup-6.5.4/src/dipdup/fetcher.py` & `dipdup-6.5.5/src/dipdup/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/hasura.py` & `dipdup-6.5.5/src/dipdup/hasura.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/http.py` & `dipdup-6.5.5/src/dipdup/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 import aiohttp
 import aiohttp.test_utils
 import orjson
 from aiolimiter import AsyncLimiter
 
 from dipdup import __version__
-from dipdup.config import HTTPConfig
 from dipdup.config import ResolvedHTTPConfig
 from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import InvalidRequestError
 from dipdup.prometheus import Metrics
 
 safe_exceptions = (
     aiohttp.ClientConnectionError,
@@ -34,16 +33,14 @@
     aiohttp.ClientPayloadError,
 )
 
 
 class HTTPGateway(AbstractAsyncContextManager[None]):
     """Base class for datasources which connect to remote HTTP endpoints"""
 
-    _default_http_config: HTTPConfig
-
     def __init__(self, url: str, http_config: ResolvedHTTPConfig) -> None:
         self._http_config = http_config
         self._http = _HTTPGateway(url, self._http_config)
 
     async def __aenter__(self) -> None:
         """Create underlying aiohttp session"""
         await self._http.__aenter__()
```

### Comparing `dipdup-6.5.4/src/dipdup/index.py` & `dipdup-6.5.5/src/dipdup/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/big_map/fetcher.py` & `dipdup-6.5.5/src/dipdup/indexes/big_map/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/big_map/index.py` & `dipdup-6.5.5/src/dipdup/indexes/big_map/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/big_map/matcher.py` & `dipdup-6.5.5/src/dipdup/indexes/big_map/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/event/fetcher.py` & `dipdup-6.5.5/src/dipdup/indexes/event/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/event/index.py` & `dipdup-6.5.5/src/dipdup/indexes/event/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/event/matcher.py` & `dipdup-6.5.5/src/dipdup/indexes/event/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/head/index.py` & `dipdup-6.5.5/src/dipdup/indexes/head/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/operation/fetcher.py` & `dipdup-6.5.5/src/dipdup/indexes/operation/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/operation/index.py` & `dipdup-6.5.5/src/dipdup/indexes/operation/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/operation/matcher.py` & `dipdup-6.5.5/src/dipdup/indexes/operation/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/token_transfer/fetcher.py` & `dipdup-6.5.5/src/dipdup/indexes/token_transfer/fetcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/token_transfer/index.py` & `dipdup-6.5.5/src/dipdup/indexes/token_transfer/index.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/indexes/token_transfer/matcher.py` & `dipdup-6.5.5/src/dipdup/indexes/token_transfer/matcher.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/install.py` & `dipdup-6.5.5/src/dipdup/install.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/models.py` & `dipdup-6.5.5/src/dipdup/models.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/project.py` & `dipdup-6.5.5/src/dipdup/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import asyncclick as cl
 import orjson as json
 from pydantic import BaseModel
 from pydantic import Field
 from tabulate import tabulate
 
-from dipdup import major_version
+from dipdup import __version__
 from dipdup.exceptions import ConfigurationError
 from dipdup.utils.codegen import load_template
 from dipdup.utils.codegen import write
 
 _logger = logging.getLogger('dipdup.project')
 
 
@@ -119,15 +119,15 @@
         cl.echo(table)
         return str(self.choices[super().prompt()])
 
 
 class JinjaAnswers(dict[str, Any]):
     def __init__(self, *args: str, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
-        self['dipdup_version'] = major_version
+        self['dipdup_version'] = __version__.split('.')[0]
 
     def __getattr__(self, item: str) -> Any:
         return self[item]
 
 
 class Project(BaseModel):
     path: Path
@@ -282,16 +282,16 @@
             name='hasura_image',
             description=(
                 'Choose Hasura version\n'
                 'Test new releases before using in production; new versions may break compatibility.'
             ),
             default=0,
             choices=(
-                'hasura/graphql-engine:v2.21.0',
-                'hasura/graphql-engine:v2.21.0',
+                'hasura/graphql-engine:v2.23.0',
+                'hasura/graphql-engine:v2.23.0',
             ),
             comments=(
                 'stable',
                 'beta',
             ),
         ),
         NotifyQuestion(
```

### Comparing `dipdup-6.5.4/src/dipdup/projects/base/.gitignore.j2` & `dipdup-6.5.5/src/dipdup/projects/base/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/base/docker-compose.swarm.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/base/docker-compose.swarm.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/base/docker-compose.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/base/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_auction/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_auction/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_big_maps/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dao/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dao/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_domains/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_domains/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_events/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_events/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_factories/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_factories/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_token/dipdup.yml.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_token/dipdup.yml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2` & `dipdup-6.5.5/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/linters_default/Makefile.j2` & `dipdup-6.5.5/src/dipdup/projects/linters_default/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/linters_default/pyproject.toml.j2` & `dipdup-6.5.5/src/dipdup/projects/linters_default/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/linters_none/Makefile.j2` & `dipdup-6.5.5/src/dipdup/projects/linters_none/Makefile.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/projects/linters_none/pyproject.toml.j2` & `dipdup-6.5.5/src/dipdup/projects/linters_none/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/prometheus.py` & `dipdup-6.5.5/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/scheduler.py` & `dipdup-6.5.5/src/dipdup/scheduler.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/sentry.py` & `dipdup-6.5.5/src/dipdup/sentry.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/sql/truncate_schema.sql` & `dipdup-6.5.5/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/transactions.py` & `dipdup-6.5.5/src/dipdup/transactions.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/utils/__init__.py` & `dipdup-6.5.5/src/dipdup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/utils/codegen.py` & `dipdup-6.5.5/src/dipdup/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/utils/database.py` & `dipdup-6.5.5/src/dipdup/utils/database.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/utils/sys.py` & `dipdup-6.5.5/src/dipdup/utils/sys.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.4/src/dipdup/yaml.py` & `dipdup-6.5.5/src/dipdup/yaml.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from os import environ as env
 from pathlib import Path
 from typing import Any
 
 from pydantic.json import pydantic_encoder
 from ruamel.yaml import YAML
 
+from dipdup import __spec_version__
 from dipdup.exceptions import ConfigurationError
 
 # NOTE: ${VARIABLE:-default} | ${VARIABLE}
 ENV_VARIABLE_REGEX = r'\$\{(?P<var_name>[\w]+)(?:\:\-(?P<default_value>.*?))?\}'
 
 
 _logger = logging.getLogger('dipdup.yaml')
@@ -101,14 +102,16 @@
 
             if environment:
                 path_yaml, path_environment = substitute_env_variables(path_yaml)
                 config_environment.update(path_environment)
 
             config.update(yaml.load(path_yaml))
 
+        config.validate_version()
+
         # FIXME: Can't use `from_` field alias in dataclass; fixed in dipdup.yaml instead
         # FIXME: See https://github.com/pydantic/pydantic/issues/4286
         fix_dataclass_field_aliases(config)
 
         return config, config_environment
 
     def dump(self) -> str:
@@ -117,7 +120,14 @@
         yaml.indent = 2
 
         config_json = json.dumps(self, default=pydantic_encoder)
         config_yaml = exclude_none(yaml.load(config_json))
         buffer = StringIO()
         yaml.dump(config_yaml, buffer)
         return buffer.getvalue()
+
+    def validate_version(self) -> None:
+        config_spec_version = self['spec_version']
+        if config_spec_version != __spec_version__:
+            raise ConfigurationError(
+                f'Incompatible spec version: expected {__spec_version__}, got {config_spec_version}. See https://docs.dipdup.io/config/spec_version'
+            )
```

### Comparing `dipdup-6.5.4/PKG-INFO` & `dipdup-6.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipdup
-Version: 6.5.4
+Version: 6.5.5
 Summary: Modular framework for creating selective indexers and featureful backends for dapps
 Home-page: https://dipdup.io/
 License: MIT
 Keywords: tezos,blockchain,sdk,michelson,indexers,tzkt,cryptocurrencies,smart-contracts
 Author: Lev Gorodetskiy
 Author-email: dipdup@drsr.io
 Requires-Python: >=3.10,<3.11
@@ -23,20 +23,20 @@
 Provides-Extra: pytezos
 Requires-Dist: APScheduler (>=3.8.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
 Requires-Dist: anyio (>=3.3.2,<4.0.0)
 Requires-Dist: asyncclick (>=8.0.1,<9.0.0)
 Requires-Dist: asyncpg (==0.27.0)
-Requires-Dist: datamodel-code-generator (==0.17.2)
+Requires-Dist: datamodel-code-generator (==0.18.0)
 Requires-Dist: orjson (>=3.6.6,<4.0.0)
 Requires-Dist: prometheus-client (>=0.14.1,<0.15.0)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: pyhumps (>=3.0.2,<4.0.0)
-Requires-Dist: pysignalr (==0.1.2)
+Requires-Dist: pysignalr (==0.2.0)
 Requires-Dist: pytezos (==3.9.0) ; extra == "pytezos"
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: ruamel.yaml (>=0.17.2,<0.18.0)
 Requires-Dist: sentry-sdk (>=1.4.3,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tortoise-orm (==0.19.3)
```

