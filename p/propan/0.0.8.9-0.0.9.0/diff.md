# Comparing `tmp/propan-0.0.8.9.tar.gz` & `tmp/propan-0.0.9.0.tar.gz`

## Comparing `propan-0.0.8.9.tar` & `propan-0.0.9.0.tar`

### file list

```diff
@@ -1,73 +1,77 @@
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 propan-0.0.8.9/CONTRIBUTING.md
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/1_basic_usage.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/5_publishing.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.8.9/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__about__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/__init__.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/app.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/main.py
--rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/supervisors/watchgodreloader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/__init__.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/formatter.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/log/logging.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/classes.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/functions.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/decorate.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/context/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/types/__init__.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 propan-0.0.8.9/propan/utils/types/decorate.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/publish.sh
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 propan-0.0.8.9/scripts/test.sh
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 propan-0.0.8.9/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.8.9/LICENSE
--rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 propan-0.0.8.9/README.md
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.0.8.9/pyproject.toml
--rw-r--r--   0        0        0     8980 2020-02-02 00:00:00.000000 propan-0.0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.0/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/5_publishing.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__about__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__main__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/annotations.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/app.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/main.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/logging.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/test.sh
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 propan-0.0.9.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.0/LICENSE
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 propan-0.0.9.0/README.md
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 propan-0.0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13373 2020-02-02 00:00:00.000000 propan-0.0.9.0/PKG-INFO
```

### Comparing `propan-0.0.8.9/examples/3_lifespan_events.py` & `propan-0.0.9.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/4_cli_attributes_promotion.py` & `propan-0.0.9.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/6_arguments_casting.py` & `propan-0.0.9.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/7_handler_errors_processing.py` & `propan-0.0.9.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/dependencies/1_dependency_injection.py` & `propan-0.0.9.0/examples/dependencies/1_dependency_injection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
 Propan use dependencies management policy close to `pytest fixtures`.
 You can specify in functions argument parameters which dependencies
 you would to use. And framework passes them from the global Context object.
 
 Default context fields are: app, broker, context (itself), logger and message.
-If you call not existed field it returns None value.
+If you call not existed field, raises "pydantic.error_wrappers.ValidationError" value.
 """
-from logging import Logger
-
-import aio_pika
-from propan import PropanApp
+from propan import Context, PropanApp
+from propan.annotations import App, ContextRepo, Logger
+from propan.annotations import RabbitBroker as Rabbit
+from propan.annotations import RabbitMessage
 from propan.brokers.rabbit import RabbitBroker
-from propan.utils import Context
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
 
 @rabbit_broker.handle("test")
 async def base_handler(
     body: dict,
-    app: PropanApp,
-    broker: RabbitBroker,
-    context: Context,
+    app: App,
+    broker: Rabbit,
+    context: ContextRepo,
     logger: Logger,
-    message: aio_pika.Message,
-    not_existed_field,
+    message: RabbitMessage,
+    not_found_field=Context(required=False),
 ):
+    assert not_found_field is None
     assert broker is rabbit_broker
-    assert not_existed_field is None
```

### Comparing `propan-0.0.8.9/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.9.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Alias is able to provide access to specific attributes of dependency
 """
-from propan import Alias, Context, PropanApp
+from propan import Context, PropanApp
+from propan.annotations import ContextRepo
 from propan.brokers.rabbit import RabbitBroker
 from pydantic import BaseSettings, Field
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
@@ -13,15 +14,15 @@
 
 
 class Settings(BaseSettings):
     key: str = Field("")
 
 
 @app.on_startup
-async def setup_later(context: Context):
+async def setup(context: ContextRepo):
     settings = Settings(key=KEY)
     context.set_context("settings", settings)
 
 
 @app.on_startup
-def setup(key: str = Alias("settings.key")):
+def setup_later(key: str = Context("settings.key")):
     assert key is KEY
```

### Comparing `propan-0.0.8.9/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.9.0/examples/dependencies/7_annotated.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """
-Depends parameter allows to call function before
-natural handler with providing all arguments and context
-inside dependency function
+With Python 3.10+ you can use
+typing.Annotated class as a shortcut to Depends and Alias
 """
-from propan import PropanApp
+import logging
+
+from propan import Context, Depends, PropanApp, apply_types
 from propan.brokers.rabbit import RabbitBroker
-from propan.utils import Depends, use_context
+from typing_extensions import Annotated
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
+Logger = Annotated[logging.Logger, Context("broker.logger")]
+
 
-@use_context
-async def async_dependency(body, logger):
+@apply_types
+async def async_dependency(body, logger: Logger):
     logger.info(f"Async calls with: {body}")
     return True
 
 
-def sync_dependency():
-    print("Hello, i am here!")
-    return True
+Dependency = Annotated[bool, Depends(async_dependency)]
 
 
 @broker.handle("test")
-async def base_handler(
-    body: dict,
-    async_called: bool = Depends(async_dependency),
-    sync_called: bool = Depends(sync_dependency),
-):
-    assert async_called and sync_called
+async def base_handler(body: dict, async_called: Dependency):
+    assert async_called is True
```

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/quart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
-from fastapi import FastAPI
 from propan.brokers.rabbit import RabbitBroker
+from quart import Quart
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
-app = FastAPI()
+app = Quart(__name__)
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
 
 
-@app.on_event("startup")
+@app.before_serving
 async def start_broker():
     await broker.start()
 
 
-@app.on_event("shutdown")
+@app.after_serving
 async def stop_broker():
     await broker.close()
 
 
-@app.get("/")
-def read_root():
-    return {"Hello": "World"}
+@app.route("/")
+async def json():
+    return {"hello": "world"}
```

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/quart.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/tornado.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
+import asyncio
+
+import tornado.web
 from propan.brokers.rabbit import RabbitBroker
-from quart import Quart
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
-app = Quart(__name__)
-
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
 
 
-@app.before_serving
-async def start_broker():
-    await broker.start()
+class MainHandler(tornado.web.RequestHandler):
+    def get(self):
+        self.write("Hello, world")
+
+
+def make_app():
+    return tornado.web.Application(
+        [
+            (r"/", MainHandler),
+        ]
+    )
+
+
+async def main():
+    app = make_app()
+    app.listen(8888)
 
-
-@app.after_serving
-async def stop_broker():
-    await broker.close()
+    await broker.start()
+    try:
+        await asyncio.Event().wait()
+    finally:
+        await broker.close()
 
 
-@app.route("/")
-async def json():
-    return {"hello": "world"}
+if __name__ == "__main__":
+    asyncio.run(main())
```

### Comparing `propan-0.0.8.9/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.9.0/examples/http_frameworks_integrations/sanic.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
 
 
-@app.get("/")
-async def hello_world(request):
-    return text("Hello, world.")
-
-
 @app.after_server_start
 async def start_broker(app, loop):
     await broker.start()
 
 
 @app.after_server_stop
 async def stop_broker(app, loop):
     await broker.close()
+
+
+@app.get("/")
+async def hello_world(request):
+    return text("Hello, world.")
```

### Comparing `propan-0.0.8.9/propan/brokers/push_back_watcher.py` & `propan-0.0.9.0/propan/brokers/push_back_watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,19 @@
         return False
 
     def remove(self, message_id: str) -> None:
         pass
 
 
 class PushBackWatcher(BaseWatcher):
-    memory: Counter[str] = Counter()
+    memory: "Counter[str]"
 
     def __init__(self, max_tries: int = 3, logger: Optional[Logger] = None):
         super().__init__(logger=logger, max_tries=max_tries)
+        self.memory = Counter()
 
     def add(self, message_id: str) -> None:
         self.memory[message_id] += 1
 
     def is_max(self, message_id: str) -> bool:
         is_max = self.memory[message_id] > self.max_tries
         if self.logger is not None:
```

### Comparing `propan-0.0.8.9/propan/brokers/model/broker_usecase.py` & `propan-0.0.9.0/propan/brokers/model/broker_usecase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
 from time import perf_counter
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.log import access_logger
-from propan.utils import apply_types, use_context
+from propan.types import DecodedMessage, DecoratedCallable, Wrapper
+from propan.utils import apply_types
 from propan.utils.context import context
 from propan.utils.context import message as message_context
+from propan.utils.functions import call_or_await
 
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
-    _connection: Any = None
-    _fmt: str = "%(asctime)s %(levelname)s - %(message)s"
+    handlers: List[Any]
+    _connection: Any
+    _fmt: str
 
     def __init__(
         self,
         *args: Any,
         apply_types: bool = True,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
+        log_fmt: str = "%(asctime)s %(levelname)s - %(message)s",
         **kwargs: Any,
     ):
         self.logger = logger
         self.log_level = log_level
+        self._fmt = log_fmt
 
+        self._connection = None
         self._is_apply_types = apply_types
         self._connection_args = args
         self._connection_kwargs = kwargs
+        self.handlers = []
 
         context.set_context("logger", logger)
         context.set_context("broker", self)
 
     async def connect(self, *args: Any, **kwargs: Any) -> Any:
         if self._connection is None:
             _args = args or self._connection_args
@@ -55,122 +62,130 @@
         raise NotImplementedError()
 
     @abstractmethod
     async def close(self) -> None:
         raise NotImplementedError()
 
     @abstractmethod
-    async def _decode_message(self, message: Any) -> Union[str, Dict[str, Any]]:
+    async def _decode_message(self, message: Any) -> DecodedMessage:
         raise NotImplementedError()
 
     @abstractmethod
     def _process_message(
-        self, func: Callable[..., Any], watcher: Optional[BaseWatcher]
-    ) -> Callable[..., Any]:
+        self, func: DecoratedCallable, watcher: Optional[BaseWatcher]
+    ) -> Wrapper:
         raise NotImplementedError()
 
     async def start(self) -> None:
         if self.logger is not None:
             self._init_logger(self.logger)
-
         await self.connect()
 
     def _get_log_context(self, **kwargs: Any) -> Dict[str, Any]:
         return {}
 
     @abstractmethod
     def handle(
         self,
         *broker_args: Any,
         retry: Union[bool, int] = False,
         **broker_kwargs: Any,
-    ) -> Callable[[Callable[..., Any]], None]:
+    ) -> Callable[[DecoratedCallable], None]:
         raise NotImplementedError()
 
     @property
     def fmt(self) -> str:
         return self._fmt
 
     def _init_logger(self, logger: logging.Logger) -> None:
         for handler in logger.handlers:
-            if handler.formatter is not None:
-                handler.setFormatter(type(handler.formatter)(self.fmt))
+            formatter = handler.formatter
+            if formatter is not None:
+                if getattr(formatter, "use_colors", None) is not None:
+                    kwargs = {"use_colors": formatter.use_colors}
+                else:
+                    kwargs = {}
+                handler.setFormatter(type(formatter)(self.fmt, **kwargs))
 
     async def __aenter__(self) -> "BrokerUsecase":
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.close()
 
     def _wrap_handler(
-        self, func: Callable[..., Any], retry: Union[bool, int], **broker_args: Any
-    ) -> Callable[..., Any]:
-        func = use_context(func)
-
-        if self._is_apply_types:
+        self, func: DecoratedCallable, retry: Union[bool, int], **broker_args: Any
+    ) -> DecoratedCallable:
+        if self._is_apply_types is True:
             func = apply_types(func)
 
+        if self.logger is not None:
+            func = self._log_execution(self.logger, **broker_args)(func)
+
         func = self._wrap_decode_message(func)
 
         func = self._process_message(func, _get_watcher(self.logger, retry))
 
-        if self.logger is not None:
-            func = self._log_execution(self.logger, **broker_args)(func)
-
         func = _set_message_context(func)
 
         return func
 
-    def _wrap_decode_message(self, func: Callable[..., Any]) -> Callable[..., Any]:
+    def _wrap_decode_message(self, func: DecoratedCallable) -> Wrapper:
         @wraps(func)
         async def wrapper(message: Any) -> Any:
             return await func(await self._decode_message(message))
 
         return wrapper
 
     def _log_execution(
         self, logger: logging.Logger, **broker_args: Any
-    ) -> Callable[[Callable[..., Any]], Any]:
-        def decor(func: Callable[..., Any]) -> Callable[..., Any]:
+    ) -> Callable[[DecoratedCallable], Wrapper]:
+        def decor(func: DecoratedCallable) -> Wrapper:
             @wraps(func)
-            async def wrapper(message: Any) -> Any:
+            async def wrapper(*args: Any, **kwargs: Any) -> Any:
+                message = message_context.get()
+
                 start = perf_counter()
 
                 self._get_log_context(message=message, **broker_args)
                 logger.log(self.log_level, "Received")
 
                 try:
-                    r = await func(message)
+                    r = await call_or_await(func, *args, **kwargs)
                 except Exception as e:
                     logger.error(repr(e))
                 else:
                     logger.log(
                         self.log_level, f"Processed by {(perf_counter() - start):.4f}"
                     )
                     return r
 
             return wrapper
 
         return decor
 
+    def _log(self, message: str, log_level: Optional[int] = None) -> None:
+        if self.logger is not None:
+            self.logger.log(message, log_level or self.log_level)
+
 
 def _get_watcher(
     logger: Optional[logging.Logger], try_number: Union[bool, int] = True
 ) -> Optional[BaseWatcher]:
     watcher: Optional[BaseWatcher]
     if try_number is True:
         watcher = FakePushBackWatcher()
     elif try_number is False:
         watcher = None
     else:
         watcher = PushBackWatcher(logger=logger, max_tries=try_number)
     return watcher
 
 
-def _set_message_context(func: Callable[..., Any]) -> Callable[[Any], Any]:
+def _set_message_context(func: DecoratedCallable) -> Wrapper:
     @wraps(func)
     async def wrapper(message: Any) -> Any:
         message_context.set(message)
         return await func(message)
 
     return wrapper
```

### Comparing `propan-0.0.8.9/propan/brokers/model/schemas.py` & `propan-0.0.9.0/propan/brokers/model/schemas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+from enum import Enum
 from typing import Any, Optional
 
 from pydantic import BaseModel, Field
 
 
+class ContentTypes(str, Enum):
+    text = "text/plain"
+    json = "application/json"
+
+
 class NameRequired(BaseModel):
     name: Optional[str] = Field(...)
 
     def __init__(self, name: str, **kwargs: Any):
         super().__init__(name=name, **kwargs)
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `propan-0.0.8.9/propan/brokers/nats/nats_broker.py` & `propan-0.0.9.0/propan/brokers/nats/nats_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,46 +2,53 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Union
 from uuid import uuid4
 
 import nats
 from nats.aio.client import Client
 from nats.aio.msg import Msg
-from propan.brokers.model import BrokerUsecase
+from propan.brokers.model import BrokerUsecase, ContentTypes
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
+from propan.types import DecoratedCallable
 from propan.utils.context.main import log_context
 
 
 class NatsBroker(BrokerUsecase):
-    handlers: List[Handler] = []
-    _connection: Optional[Client] = None
+    handlers: List[Handler]
+    _connection: Optional[Client]
 
-    __max_queue_len = 0
-    __max_subject_len = 4
+    __max_queue_len: int
+    __max_subject_len: int
 
     def __init__(self, *args: Any, log_fmt: Optional[str] = None, **kwargs: Any):
-        super().__init__(*args, **kwargs)
-        self._fmt = log_fmt
+        super().__init__(*args, log_fmt=log_fmt, **kwargs)
+
+        self._connection = None
+
+        self.__max_queue_len = 0
+        self.__max_subject_len = 4
 
     async def _connect(self, *args: Any, **kwargs: Any) -> Client:
         return await nats.connect(*args, **kwargs)
 
     def handle(
         self, subject: str, queue: str = "", retry: Union[bool, int] = False
-    ) -> Callable[[Callable[..., Any]], None]:
-        if (i := len(subject)) > self.__max_subject_len:
+    ) -> Callable[[DecoratedCallable], None]:
+        i = len(subject)
+        if i > self.__max_subject_len:
             self.__max_subject_len = i
 
-        if (i := len(queue)) > self.__max_queue_len:
+        i = len(queue)
+        if i > self.__max_queue_len:
             self.__max_queue_len = i
 
         parent = super()
 
-        def wrapper(func: Callable[..., Any]) -> None:
+        def wrapper(func: DecoratedCallable) -> None:
             for handler in self.handlers:
                 if handler.subject == subject and handler.queue == queue:
                     raise ValueError(
                         f"`{func.__name__}` uses already "
                         f"using `{subject}` subject with "
                         f"`{queue}` queue"
                     )
@@ -71,20 +78,20 @@
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
         if isinstance(message, dict):
             message = json.dumps(message)
             headers = {
                 **publish_args.pop("headers", {}),
-                "content-type": "application/json",
+                "content-type": ContentTypes.json.value,
             }
         else:
             headers = {
                 **publish_args.pop("headers", {}),
-                "content-type": "text/plain",
+                "content-type": ContentTypes.text.value,
             }
 
         return await self._connection.publish(
             subject, message.encode(), headers=headers, **publish_args
         )
 
     async def close(self) -> None:
@@ -117,22 +124,26 @@
             f"%(subject)-{self.__max_subject_len}s | "
             + (f"%(queue)-{self.__max_queue_len}s | " if self.__max_queue_len else "")
             + "%(message_id)-10s "
             "- %(message)s"
         )
 
     @staticmethod
-    async def _decode_message(message: Msg) -> Union[str, dict]:
-        body = message.data.decode()
-        if message.header and message.header.get("content-type") == "application/json":
-            body = json.loads(body)
+    async def _decode_message(message: Msg) -> Union[str, dict, bytes]:
+        body = message.data
+        if message.header:
+            content_type = message.header.get("content-type", "")
+            if ContentTypes.json.value in content_type:
+                body = json.loads(body.decode())
+            elif ContentTypes.text.value in content_type:
+                body = body.decode()
         return body
 
     @staticmethod
     def _process_message(
-        func: Callable[..., Any], watcher: Optional[BaseWatcher] = None
+        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
     ) -> Callable[[Msg], Any]:
         @wraps(func)
         async def wrapper(message: Msg):
             return await func(message)
 
         return wrapper
```

### Comparing `propan-0.0.8.9/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.9.0/propan/brokers/nats/nats_broker.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     SignatureCallback,
 )
 from nats.aio.msg import Msg
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
+from propan.types import DecoratedCallable
 
 class NatsBroker(BrokerUsecase):
     logger: logging.Logger
     handlers: List[Handler] = []
     _connection: Optional[Client] = None
 
     def __init__(
@@ -109,20 +110,20 @@
         message: Union[str, Dict[str, Any]],
         subject: str,
         reply: str = "",
         headers: Optional[Dict[str, str]] = None,
     ) -> None: ...
     def handle(
         self, subject: str, queue: str = "", retry: Union[bool, int] = False
-    ) -> Callable[[Callable[..., Any]], None]: ...
+    ) -> Callable[[DecoratedCallable], None]: ...
     async def __aenter__(self) -> "NatsBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
     async def close(self) -> None: ...
     def _get_log_context(
         self, message: Optional[Msg], subject: str, queue: str = "", **kwargs
     ) -> Dict[str, Any]: ...
     @staticmethod
     async def _decode_message(message: Msg) -> Union[str, dict]: ...
     @staticmethod
     def _process_message(
-        func: Callable[..., Any], watcher: Optional[BaseWatcher] = None
+        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
     ) -> Callable[[Msg], Any]: ...
```

### Comparing `propan-0.0.8.9/propan/brokers/nats/nats_js_broker.py` & `propan-0.0.9.0/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 import asyncio
 import json
+import logging
 from functools import partial, wraps
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import aio_pika
 import aiormq
-from propan.brokers.model import BrokerUsecase
+from propan.brokers.model import BrokerUsecase, ContentTypes
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
+from propan.types import DecodedMessage, DecoratedCallable, Wrapper
 from propan.utils.context.main import log_context
 
 
 class RabbitBroker(BrokerUsecase):
-    handlers: List[Handler] = []
-    _connection: Optional[aio_pika.RobustConnection] = None
-    _channel: Optional[aio_pika.RobustChannel] = None
+    handlers: List[Handler]
+    _connection: Optional[aio_pika.RobustConnection]
+    _channel: Optional[aio_pika.RobustChannel]
 
-    __max_queue_len = 4
-    __max_exchange_len = 4
+    __max_queue_len: int
+    __max_exchange_len: int
 
     def __init__(
         self,
         *args: Any,
         consumers: Optional[int] = None,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ):
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, log_fmt=log_fmt, **kwargs)
         self._max_consumers = consumers
-        self._fmt = log_fmt
+
+        self._channel = None
+        self.handlers = []
+
+        self.__max_queue_len = 4
+        self.__max_exchange_len = 4
 
     async def __aenter__(self) -> "RabbitBroker":
         await self.connect()
-        await self.init_channel()
+        await self._init_channel()
         return self
 
     async def _connect(self, *args: Any, **kwargs: Any) -> aio_pika.Connection:
         return await aio_pika.connect_robust(
             *args, **kwargs, loop=asyncio.get_event_loop()
         )
 
-    async def init_channel(self, max_consumers: Optional[int] = None) -> None:
+    async def _init_channel(self, max_consumers: Optional[int] = None) -> None:
         if self._channel is None:
             if self._connection is None:
                 raise ValueError("RabbitBroker not connected yet")
 
             max_consumers = max_consumers or self._max_consumers
             self._channel = await self._connection.channel()
-            if max_consumers and self.logger:
-                self.logger.info(f"Set max consumers to {max_consumers}")
+
+            if max_consumers:
+                self._log(f"Set max consumers to {max_consumers}", logging.INFO)
                 await self._channel.set_qos(prefetch_count=int(max_consumers))
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
-    ) -> Callable[[Callable[..., Any]], None]:
+    ) -> Wrapper:
         queue, exchange = _validate_exchange_and_queue(queue, exchange)
 
-        if exchange and (i := len(exchange.name)) > self.__max_exchange_len:
-            self.__max_exchange_len = i
+        if exchange:
+            i = len(exchange.name)
+            if i > self.__max_exchange_len:  # pragma: no branch
+                self.__max_exchange_len = i
 
-        if (i := len(queue.name)) > self.__max_queue_len:
+        i = len(queue.name)
+        if i > self.__max_queue_len:  # pragma: no branch
             self.__max_queue_len = i
 
         parent = super()
 
-        def wrapper(func: Callable[..., Any]) -> None:
+        def wrapper(func: DecoratedCallable) -> Any:
             for handler in self.handlers:
                 if handler.exchange == exchange and handler.queue == queue:
                     raise ValueError(
                         f"`{func.__name__}` uses already "
                         f"using `{queue.name}` queue to listen "
                         f"`{exchange.name if exchange else 'default'}` exchange"
                     )
@@ -80,67 +91,71 @@
             handler = Handler(callback=func, queue=queue, exchange=exchange)
             self.handlers.append(handler)
 
         return wrapper
 
     async def start(self) -> None:
         await super().start()
-        await self.init_channel()
+        await self._init_channel()
 
         for handler in self.handlers:
             queue = await self._init_handler(handler)
 
             func = handler.callback
 
-            if self.logger:
+            if self.logger is not None:
                 self._get_log_context(None, handler.queue, handler.exchange)
                 self.logger.info(f"`{func.__name__}` waiting for messages")
 
             await queue.consume(func)
 
     async def publish_message(
         self,
         message: Union[aio_pika.Message, str, Dict[str, Any]],
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
+        *,
+        routing_key: str = "",
         **publish_args,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
         queue, exchange = _validate_exchange_and_queue(queue, exchange)
 
         if not isinstance(message, aio_pika.Message):
             if isinstance(message, dict):
                 message = aio_pika.Message(
-                    json.dumps(message).encode(), content_type="application/json"
+                    json.dumps(message).encode(), content_type=ContentTypes.json.value
                 )
             else:
-                message = aio_pika.Message(message.encode(), content_type="text/plain")
+                message = aio_pika.Message(
+                    message.encode(), content_type=ContentTypes.text.value
+                )
 
         if exchange is None:
             exchange_obj = self._channel.default_exchange
         else:
             exchange_obj = await self._init_exchange(exchange)
 
         return await exchange_obj.publish(
             message=message,
-            routing_key=queue.name,
+            routing_key=routing_key or queue.name,
             **publish_args,
         )
 
     async def close(self) -> None:
-        if self._connection:
+        if self._connection is not None:
             await self._connection.close()
 
     async def _init_handler(self, handler: Handler) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self._init_queue(handler.queue)
         if handler.exchange is not None:
             exchange = await self._init_exchange(handler.exchange)
-            await queue.bind(exchange)
+            await queue.bind(exchange, handler.queue.routing_key or handler.queue.name)
         return queue
 
     async def _init_queue(self, queue: RabbitQueue) -> aio_pika.abc.AbstractRobustQueue:
         if queue.declare is True:
             return await self._channel.declare_queue(**queue.dict())
         else:
             return await self._channel.get_queue(queue.name, ensure=False)
@@ -162,14 +177,15 @@
     ) -> Dict[str, Any]:
         exchange_name = exchange.name if exchange else "default"
         context = {
             "exchange": exchange_name,
             "queue": queue.name,
             "message_id": message.message_id[:10] if message else "",
         }
+
         log_context.set(context)
         return context
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
@@ -178,51 +194,59 @@
             f"%(message_id)-10s "
             "- %(message)s"
         )
 
     @staticmethod
     async def _decode_message(
         message: aio_pika.IncomingMessage,
-    ) -> Union[str, Dict[str, Any]]:
-        body = message.body.decode()
-        if message.content_type == "application/json":
-            body = json.loads(body)
+    ) -> DecodedMessage:
+        body = message.body
+        if message.content_type is not None:
+            if ContentTypes.text.value in message.content_type:
+                body = body.decode()
+            elif ContentTypes.json.value in message.content_type:  # pragma: no branch
+                body = json.loads(body.decode())
         return body
 
     @staticmethod
     def _process_message(
-        func: Callable[..., Any], watcher: Optional[BaseWatcher] = None
-    ) -> Callable[..., Any]:
+        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
+    ) -> DecoratedCallable:
         @wraps(func)
         async def wrapper(message: aio_pika.Message):
             if watcher is None:
                 context = message.process()
             else:
                 context = WatcherContext(
                     watcher,
                     message.message_id,
                     on_success=partial(message.ack),
                     on_error=partial(message.reject, True),
                     on_max=partial(message.reject, False),
                 )
             async with context:
-                return await func(message)
+                r = await func(message)
+                return r
 
         return wrapper
 
 
 def _validate_exchange_and_queue(
-    queue: Union[str, RabbitQueue], exchange: Union[str, RabbitExchange, None] = None
-) -> tuple[RabbitQueue, Optional[RabbitExchange]]:
-    if isinstance(queue, str):
-        queue = RabbitQueue(name=queue)
-    elif not isinstance(queue, RabbitQueue):
-        raise ValueError(f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance")
+    queue: Union[str, RabbitQueue, None],
+    exchange: Union[str, RabbitExchange, None] = None,
+) -> Tuple[RabbitQueue, Optional[RabbitExchange]]:
+    if queue is not None:  # pragma: no branch
+        if isinstance(queue, str):
+            queue = RabbitQueue(name=queue)
+        elif not isinstance(queue, RabbitQueue):
+            raise ValueError(
+                f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
+            )
 
-    if exchange is not None:
+    if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
             exchange = RabbitExchange(name=exchange)
         elif not isinstance(exchange, RabbitExchange):
             raise ValueError(
                 f"Exchange '{exchange}' should be 'str' | 'RabbitExchange' instance"
             )
```

### Comparing `propan-0.0.8.9/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import logging
 from ssl import SSLContext
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import aio_pika
 import aiormq
 from pamqp.common import FieldTable
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.brokers.rabbit.schemas import RabbitExchange, RabbitQueue
+from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
+from propan.types import DecodedMessage, DecoratedCallable, Wrapper
 from yarl import URL
 
 class RabbitBroker(BrokerUsecase):
+    handlers: List[Handler]
+    _connection: Optional[aio_pika.RobustConnection]
+    _channel: Optional[aio_pika.RobustChannel]
+
+    __max_queue_len: int
+    __max_exchange_len: int
+
     async def __init__(
         self,
         url: Union[str, URL, None] = None,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
@@ -91,39 +99,52 @@
         """
         ...
     async def publish_message(
         self,
         message: Union[aio_pika.Message, str, Dict[str, Any]],
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
+        *,
+        routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
         timeout: aio_pika.abc.TimeoutType = None,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]: ...
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
-    ) -> Callable[[Callable[..., Any]], None]:
+    ) -> Wrapper:
         """
         retry: Union[bool, int] - at exeption message will returns to queue `int` times or endless if `True`
         """
         ...
     async def __aenter__(self) -> "RabbitBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> aio_pika.Connection: ...
     async def close(self) -> None: ...
     @staticmethod
     async def _decode_message(
         message: aio_pika.IncomingMessage,
-    ) -> Union[str, Dict[str, Any]]: ...
+    ) -> DecodedMessage: ...
     @staticmethod
     def _process_message(
-        func: Callable[..., Any], watcher: Optional[BaseWatcher] = None
-    ) -> Callable[..., Any]: ...
+        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
+    ) -> DecoratedCallable: ...
     def _get_log_context(
         self,
         message: Optional[aio_pika.Message],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
         **kwrags,
     ) -> Dict[str, Any]: ...
+    async def _init_channel(self, max_consumers: Optional[int] = None) -> None: ...
+    async def _init_handler(
+        self, handler: Handler
+    ) -> aio_pika.abc.AbstractRobustQueue: ...
+    async def _init_queue(
+        self, queue: RabbitQueue
+    ) -> aio_pika.abc.AbstractRobustQueue: ...
+    async def _init_exchange(
+        self, exchange: RabbitExchange
+    ) -> aio_pika.abc.AbstractRobustExchange: ...
+    async def start(self) -> None: ...
```

### Comparing `propan-0.0.8.9/propan/brokers/rabbit/schemas.py` & `propan-0.0.9.0/propan/brokers/rabbit/schemas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from aio_pika.abc import ExchangeType, TimeoutType
 from propan.brokers.model.schemas import NameRequired, Queue
+from propan.types import DecoratedCallable
 from pydantic import BaseModel, Field
 
 __all__ = (
     "RabbitQueue",
     "RabbitExchange",
     "Handler",
     "ExchangeType",
@@ -16,26 +17,29 @@
     durable: bool = False
     exclusive: bool = False
     passive: bool = False
     auto_delete: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
+
     declare: bool = Field(default=True, exclude=True)
+    routing_key: str = Field(default="", exclude=True)
 
 
 class RabbitExchange(NameRequired):
     type: Union[ExchangeType, str] = ExchangeType.DIRECT
     durable: bool = False
     auto_delete: bool = False
     internal: bool = False
     passive: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
+
     declare: bool = Field(default=True, exclude=True)
 
 
 class Handler(BaseModel):
-    callback: Callable[..., Any]
+    callback: DecoratedCallable
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = None
```

### Comparing `propan-0.0.8.9/propan/cli/main.py` & `propan-0.0.9.0/propan/cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,56 @@
+import asyncio
 import logging
+import sys
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 import typer
 from propan.__about__ import __version__
 from propan.cli.app import PropanApp
-from propan.cli.utils.imports import get_app_object
+from propan.cli.utils.imports import get_app_path, import_object
 from propan.cli.utils.logs import LogLevels, set_log_level
 from propan.cli.utils.parser import parse_cli_args
 from propan.log import logger
 
 cli = typer.Typer()
 
 
 def version_callback(version: bool) -> None:
     if version is True:
         import platform
 
         typer.echo(
-            "Running propan %s with %s %s on %s"
+            "Running Propan %s with %s %s on %s"
             % (
                 __version__,
                 platform.python_implementation(),
                 platform.python_version(),
                 platform.system(),
             )
         )
 
         raise typer.Exit()
 
 
+@cli.callback()
+def main(
+    version: Optional[bool] = typer.Option(
+        False,
+        "--version",
+        callback=version_callback,
+        is_eager=True,
+        help="Show current platform, python and propan version",
+    )
+):
+    """
+    Generate, run and manage Propan apps to greater development experience
+    """
+
+
 @cli.command()
 def create(appname: str) -> None:
     """Create a new Propan project at [APPNAME] directory"""
     from propan.cli.startproject import create
 
     project = create(Path.cwd() / appname, __version__)
     typer.echo(f"Create Propan project template at: {project}")
@@ -47,71 +64,74 @@
     app: str = typer.Argument(
         ..., help="[python_module:PropanApp] - path to your application"
     ),
     workers: int = typer.Option(
         1, show_default=False, help="Run [workers] applications with process spawning"
     ),
     log_level: LogLevels = typer.Option(
-        LogLevels.info,
-        case_sensitive=False,
-        show_default=False,
-        help="[INFO] default",
-        autocompletion=lambda: list(LogLevels._member_map_.keys()),
+        LogLevels.info, case_sensitive=False, show_default=False, help="[INFO] default"
     ),
     reload: bool = typer.Option(
         False, "--reload", is_flag=True, help="Restart app at directory files changes"
     ),
 ) -> None:
     """Run [MODULE:APP] Propan application"""
     app, extra = parse_cli_args(app, *ctx.args)
 
-    args = (app, extra)
+    module, app = get_app_path(app)
+
+    app_dir = module.parent
+    sys.path.insert(0, str(app_dir))
+
+    args = (module, app, extra)
 
     if reload and workers > 1:
         raise ValueError("You can't use reload option with multiprocessing")
 
     set_log_level(log_level)
 
     if reload is True:
-        from propan.cli.supervisors.watchgodreloader import WatchGodReload
+        from propan.cli.supervisors.watchfiles import WatchReloader
 
-        WatchGodReload(target=_run, args=args).run()
+        WatchReloader(target=_run, args=args, reload_dirs=(app_dir,)).run()
 
     elif workers > 1:
         from propan.cli.supervisors.multiprocess import Multiprocess
 
         Multiprocess(target=_run, args=(*args, logging.DEBUG), workers=workers).run()
 
     else:
         _run(*args)
 
 
-@cli.callback()
-def main(
-    version: Optional[bool] = typer.Option(
-        False,
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-        help="Show current platform, python and propan version",
-    )
-):
-    """
-    Generate, run and manage Propan apps to greater development experience
-    """
-
-
 def _run(
-    app: PropanApp,
-    context_kwargs: Dict[str, Union[bool, str]],
+    module: Path,
+    app: str,
+    extra_options: Dict[str, Union[bool, str]],
     log_level: int = logging.INFO,
 ) -> None:
     try:
-        propan_app = get_app_object(app)
+        propan_app = import_object(module, app)
+
+        if not isinstance(propan_app, PropanApp):
+            raise ValueError(f"{propan_app} is not a PropanApp")
 
     except (ValueError, FileNotFoundError, AttributeError) as e:
         logger.error(e)
-        logger.error("Please, input module like python_file:propan_app_name")
+        logger.error("Please, input module like [python_file:propan_app_name]")
         exit()
 
     else:
-        propan_app.run(log_level, **context_kwargs)
+        propan_app._command_line_options = extra_options
+
+        if sys.platform not in ("win32", "cygwin", "cli"):
+            import uvloop
+
+            if sys.version_info >= (3, 11):
+                with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
+                    runner.run(propan_app.run(log_level))
+                    return
+
+            else:
+                uvloop.install()
+
+        asyncio.run(propan_app.run(log_level))
```

### Comparing `propan-0.0.8.9/propan/cli/startproject.py` & `propan-0.0.9.0/propan/cli/startproject.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from pathlib import Path
+from typing import Union
 
 
 def create(project_dir: Path, version: str) -> Path:
     project_dir = _create_project_dir(project_dir, version)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
     _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path, version: str) -> Path:
     project_dir = _touch_dir(dirname)
 
-    if project_dir.exists() is False:
-        project_dir.mkdir()
-
     _write_file(project_dir / "README.md")
 
     _write_file(
         project_dir / "Dockerfile",
         "FROM python:3.11.3-slim",
         "",
         "RUN useradd -ms /bin/bash user",
@@ -207,15 +205,18 @@
         "async def base_handler(body: dict, logger):",
         "    logger.info(body)",
     )
 
     return apps_dir
 
 
-def _touch_dir(dir: Path) -> Path:
+def _touch_dir(dir: Union[Path, str]) -> Path:
+    if isinstance(dir, str) is True:
+        dir = Path(dir).resolve()
+
     if dir.exists() is False:
         dir.mkdir()
     return dir
 
 
 def _write_file(path: Path, *content: str) -> None:
     path.touch()
```

### Comparing `propan-0.0.8.9/propan/cli/supervisors/basereload.py` & `propan-0.0.9.0/propan/cli/supervisors/basereload.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import threading
 from multiprocessing.context import SpawnProcess
-from typing import Any, Callable, Optional, Tuple
+from typing import Any, Optional, Tuple
 
 from propan.cli.supervisors.utils import get_subprocess, set_exit
 from propan.log import logger
+from propan.types import DecoratedCallable
 
 
 class BaseReload:
     _process: SpawnProcess
-    _target: Callable[..., Any]
+    _target: DecoratedCallable
     _args: Tuple[Any, ...]
 
     reload_delay: Optional[float]
     should_exit: threading.Event
     pid: int
     reloader_name: str = ""
 
     def __init__(
         self,
-        target: Callable[..., Any],
+        target: DecoratedCallable,
         args: Tuple[Any, ...],
         reload_delay: Optional[float] = 0.5,
     ) -> None:
         self._target = target
         self._args = args
 
         self.should_exit = threading.Event()
@@ -31,15 +32,15 @@
         self.reload_delay = reload_delay
 
         set_exit(lambda *_: self.should_exit.set())
 
     def run(self) -> None:
         self.startup()
         while not self.should_exit.wait(self.reload_delay):
-            if self.should_restart():
+            if self.should_restart():  # pragma: no branch
                 self.restart()
         self.shutdown()
 
     def startup(self) -> None:
         logger.info(f"Started reloader process [{self.pid}] using {self.reloader_name}")
         self._process = self._start_process()
```

### Comparing `propan-0.0.8.9/propan/cli/supervisors/multiprocess.py` & `propan-0.0.9.0/propan/cli/supervisors/multiprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import os
-import threading
 from multiprocessing.context import SpawnProcess
-from typing import Any, Callable, List, Tuple
+from typing import Any, List, Tuple
 
 from propan.cli.supervisors.basereload import BaseReload
-from propan.cli.supervisors.utils import get_subprocess, set_exit
 from propan.log import logger
+from propan.types import DecoratedCallable
 
 
 class Multiprocess(BaseReload):
     def __init__(
-        self,
-        target: Callable[..., Any],
-        args: Tuple[Any, ...],
-        workers: int
+        self, target: DecoratedCallable, args: Tuple[Any, ...], workers: int
     ) -> None:
         super().__init__(target, args, None)
 
         self.workers = workers
         self.processes: List[SpawnProcess] = []
 
     def startup(self) -> None:
```

### Comparing `propan-0.0.8.9/propan/cli/utils/logs.py` & `propan-0.0.9.0/propan/cli/utils/logs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import logging
+from collections import defaultdict
 from enum import Enum
-from typing import Dict
+from typing import Union
 
 from propan.log import access_logger, logger
 
 
 class LogLevels(str, Enum):
     critical = "critical"
     error = "error"
     warning = "warning"
     info = "info"
     debug = "debug"
 
 
-LOG_LEVELS: Dict[str, int] = {
-    "critical": logging.CRITICAL,
-    "error": logging.ERROR,
-    "warning": logging.WARNING,
-    "info": logging.INFO,
-    "debug": logging.DEBUG,
-}
-
-
-def set_log_level(level: LogLevels) -> None:
-    log_level = LOG_LEVELS[level.value]
+LOG_LEVELS: "defaultdict[str, int]" = defaultdict(
+    lambda: logging.INFO,
+    **{
+        "critical": logging.CRITICAL,
+        "error": logging.ERROR,
+        "warning": logging.WARNING,
+        "info": logging.INFO,
+        "debug": logging.DEBUG,
+    },
+)
+
+
+def set_log_level(level: Union[LogLevels, str]) -> None:
+    if isinstance(level, LogLevels):
+        level = level.value
+    log_level = LOG_LEVELS[level]
     logger.setLevel(log_level)
     access_logger.setLevel(log_level)
```

### Comparing `propan-0.0.8.9/propan/cli/utils/parser.py` & `propan-0.0.9.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/propan/log/logging.py` & `propan-0.0.9.0/propan/log/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 LOGGING_CONFIG: Dict[str, Any] = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "default": {
             "()": partial(configure_formatter, DefaultFormatter),
             "fmt": "%(asctime)s %(levelname)s - %(message)s",
-            "use_colors": None,
+            "use_colors": True,
         },
         "access": {
             "()": partial(configure_formatter, AccessFormatter),
             "fmt": "%(asctime)s %(levelname)s - %(message)s",
+            "use_colors": True,
         },
     },
     "handlers": {
         "default": {
             "formatter": "default",
             "class": "logging.StreamHandler",
             "stream": "ext://sys.stderr",
```

### Comparing `propan-0.0.8.9/propan/utils/context/main.py` & `propan-0.0.9.0/propan/utils/context/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from propan.utils.classes import Singlethon
 
 message: ContextVar[Optional[str]] = ContextVar("message", default=None)
 log_context: ContextVar[Dict[str, Any]] = ContextVar("message", default={})
 
 
-class Context(Singlethon):
+class ContextRepo(Singlethon):
     _context: Dict[str, Any] = {}
 
     def set_context(self, key: str, v: Any) -> None:
         self._context[key] = v
 
     def remove_context(self, key: str) -> None:
         self._context.pop(key, None)
@@ -23,8 +23,8 @@
         return self.context.get(__name)
 
     @property
     def context(self) -> Dict[str, Any]:
         return {**self._context, "context": self, "message": message.get()}
 
 
-context: Context = Context()
+context: ContextRepo = ContextRepo()
```

### Comparing `propan-0.0.8.9/LICENSE` & `propan-0.0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.8.9/pyproject.toml` & `propan-0.0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -41,56 +41,70 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "pydantic>=1.8",
-    "watchgod",
+    "fast-depends>=1.1.1",
+    "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/Lancetnik/Propan"
-Documentation = "https://github.com/Lancetnik/Propan"
+Homepage = "https://lancetnik.github.io/Propan/"
+Documentation = "https://lancetnik.github.io/Propan/"
 Tracker = "https://github.com/Lancetnik/Propan/issues"
 Source = "https://github.com/Lancetnik/Propan"
 
 [project.scripts]
-propan = "propan:cli"
+propan = "propan.__main__:cli"
 
 [project.optional-dependencies]
-async_rabbit = [
-    "pika-stubs",
+async-rabbit = [
     "aio-pika>=9",
 ]
 
-async_nats = [
+async-nats = [
     "nats-py>=2"
 ]
 
 test = [
-    "propan[async_rabbit]",
-    "propan[async_nats]",
+    "propan[async-rabbit]",
+    "propan[async-nats]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
+    "pytest-xdist[psutil]",
+
+    "asyncmock; python_version < '3.8'",
+]
+
+doc = [
+    "mkdocs >=1.1.2,<2.0.0",
+    "mkdocs-material >=8.1.4,<9.0.0",
+    "mkdocs-static-i18n",
+    "mdx-include >=1.4.1,<2.0.0",
+    "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
+    "pyyaml >=5.3.1,<7.0.0",
+
+    "typer[all]",
 ]
 
 dev = [
     "propan[test]",
+    "propan[doc]",
 
     "mypy==1.1.1",
     "black==23.3.0",
-    "isort==5.12.0",
+    "isort>=5",
     "ruff==0.0.261",
     "typer[all]",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
@@ -113,17 +127,32 @@
 ]
 
 [tool.hatch.envs.test]
 features = [
   "test",
 ]
 
+[tool.hatch.envs.test.scripts]
+run = "pytest -q -m 'not slow'"
+run-all = "pytest -m 'all'"
+
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
+[tool.hatch.envs.test-last]
+python = "3.11"
+features = [
+  "test",
+]
+
+[tool.hatch.envs.test-last.scripts]
+run = "pytest -q -m 'not slow'"
+run-all = "pytest -v -m 'all'"
+cov = "bash ./scripts/test-cov.sh -v -m 'all'"
+
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 known_third_party = ["propan", "pydantic", "aio-pika", "nats-py"]
@@ -149,33 +178,60 @@
 extend-immutable-calls = [
     "propan.Depends", "propan.Alias",
     "propan.utils.Depends", "propan.utils.Alias",
     "propan.utils.context.Depends", "propan.utils.context.Alias",
     "typer.Argument", "typer.Option",
 ]
 
+[tool.pytest.ini_options]
+minversion = "7.0"
+addopts = "-q -m 'not slow'"
+testpaths = [
+    "tests",
+]
+markers = [
+    "slow",
+    "rabbit",
+    "nats",
+    "all",
+]
+
 [tool.coverage.run]
 parallel = true
+branch = true
+concurrency = [
+    "multiprocessing",
+    "thread"
+]
 source = [
     "propan",
     "tests"
 ]
 context = '${CONTEXT}'
 omit = [
     "**/__init__.py",
 ]
 
 [tool.coverage.report]
 show_missing = true
 skip_empty = true
 exclude_lines = [
+    ".*# pragma: no cover",
     "if __name__ == .__main__.:",
+    "self.logger",
+    "def __repr__",
+    "lambda: None",
     "from .*",
     "import .*",
     '@(abc\.)?abstractmethod',
     "raise NotImplementedError",
     'raise AssertionError',
-    'if self.logger is not None:',
+    'raise ValueError',
     'logger\..*',
     "pass",
     '\.\.\.',
 ]
+omit = [
+    '*/__about__.py',
+    '*/__main__.py',
+    '*/__init__.py',
+]
```

