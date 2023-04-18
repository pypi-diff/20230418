# Comparing `tmp/repository_service_tuf-0.1.1a2.tar.gz` & `tmp/repository_service_tuf-0.1.1a3.tar.gz`

## Comparing `repository_service_tuf-0.1.1a2.tar` & `repository_service_tuf-0.1.1a3.tar`

### file list

```diff
@@ -1,93 +1,86 @@
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.gitignore
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Makefile
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Pipfile
--rw-r--r--   0        0        0    80773 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Pipfile.lock
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/README.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/id_ed25519
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/id_ed25519.pub
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/requirements-dev.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/requirements.txt
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/rstuf.ini
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/cd.yml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    45409 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/tuf.py
--rwxr-xr-x   0        0        0      861 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/2.targets.json
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.pub
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JimiHendrix.pub
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online.pub
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/test__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    30060 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.gitignore
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Makefile
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Pipfile
+-rw-r--r--   0        0        0    80773 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Pipfile.lock
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/README.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/id_ed25519
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/id_ed25519.pub
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/requirements-dev.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/requirements.txt
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/rstuf.ini
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    45409 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/tuf.py
+-rwxr-xr-x   0        0        0      861 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/2.targets.json
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/README.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JoeCocker.key
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JoeCocker.key.pub
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online.pub
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    30164 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/key/test_generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/PKG-INFO
```

### Comparing `repository_service_tuf-0.1.1a2/.gitignore` & `repository_service_tuf-0.1.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.pre-commit-config.yaml` & `repository_service_tuf-0.1.1a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.readthedocs.yaml` & `repository_service_tuf-0.1.1a3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.1.1a3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/CONTRIBUTING.rst` & `repository_service_tuf-0.1.1a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/LICENSE` & `repository_service_tuf-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/Pipfile` & `repository_service_tuf-0.1.1a3/Pipfile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/Pipfile.lock` & `repository_service_tuf-0.1.1a3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/README.rst` & `repository_service_tuf-0.1.1a3/README.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/id_ed25519` & `repository_service_tuf-0.1.1a3/id_ed25519`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/pyproject.toml` & `repository_service_tuf-0.1.1a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/requirements-dev.txt` & `repository_service_tuf-0.1.1a3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/requirements.txt` & `repository_service_tuf-0.1.1a3/requirements.txt`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tox.ini` & `repository_service_tuf-0.1.1a3/tox.ini`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.1.1a3/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/workflows/cd.yml` & `repository_service_tuf-0.1.1a3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/workflows/ci.yml` & `repository_service_tuf-0.1.1a3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/.github/workflows/update-python-deps.yml` & `repository_service_tuf-0.1.1a3/.github/workflows/update-python-deps.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/Makefile` & `repository_service_tuf-0.1.1a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/make.bat` & `repository_service_tuf-0.1.1a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/conf.py` & `repository_service_tuf-0.1.1a3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C3.png` & `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C3.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/devel/design.rst` & `repository_service_tuf-0.1.1a3/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/docs/source/guide/index.rst` & `repository_service_tuf-0.1.1a3/docs/source/guide/index.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/constants.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/__init__.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/ceremony.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 def generate(context, scope, expires):
     """
     Generate new token.
     """
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
-    login = is_logged(server, logged_token)
+    login = is_logged(settings)
     if login.state is False:
         raise click.ClickException("Not logged. Use 'rstuf-cli admin login'")
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     payload = {"scopes": list(scope), "expires": expires}
     response = request_server(
         server,
@@ -82,15 +82,15 @@
 @click.pass_context
 def inspect(context, token):
     "Show token information details."
 
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
-    login = is_logged(server, logged_token)
+    login = is_logged(settings)
     if login.state is False:
         raise click.ClickException("Not logged. Use 'rstuf-cli admin login'")
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     response = request_server(
         server,
         f"{URL.token.value}?token={token}",
```

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/tuf.py` & `repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/2.targets.json` & `repository_service_tuf-0.1.1a3/tests/2.targets.json`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/conftest.py` & `repository_service_tuf-0.1.1a3/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,23 +76,23 @@
         "",  # What is the metadata expiration for the snapshot role?(Days) (365)?  # noqa
         "",  # What is the metadata expiration for the timestamp role?(Days) (365)?  # noqa
         "",  # What is the metadata expiration for the bins role?(Days) (365)?
         "Y",  # Ready to start loading the keys? Passwords will be required for keys [y/n]  # noqa
     ]
     input_step2 = [
         "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
-        "tests/files/online.key",  # Enter 1/1 the ONLINE`s private key path
+        "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
         "strongPass",  # Enter 1/1 the ONLINE`s private key password
     ]
     input_step3 = [
         "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
-        "tests/files/JanisJoplin.key",  # Enter 1/2 the root`s private key path
+        "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key pathh  # noqa
         "strongPass",  # Enter 1/2 the root`s private key password
         "",  # Choose 2/2 root key type [ed25519/ecdsa/rsa]
-        "tests/files/JimiHendrix.key",  # Enter 2/2 the root`s private key path
+        "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key pathh  # noqa
         "strongPass",  # Enter 2/2 the root`s private key password:
     ]
     input_step4 = [
         "y",  # Is the online key configuration correct? [y/n]
         "y",  # Is the root configuration correct? [y/n]
         "y",  # Is the targets configuration correct? [y/n]
         "y",  # Is the snapshot configuration correct? [y/n]
```

### Comparing `repository_service_tuf-0.1.1a2/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.1.1a3/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.key` & `repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.key` & `repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/files/online-rsa.key` & `repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/files/online-rsa.pub` & `repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/files/online.key` & `repository_service_tuf-0.1.1a3/tests/files/key_storage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/cli/test__init__.py` & `repository_service_tuf-0.1.1a3/tests/unit/cli/test__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_ceremony.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,19 +390,19 @@
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step2
         input_step2 = [
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
-            "tests/files/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
+            "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "wrong password",  # Enter 1/1 the ONLINE`s private key password
             "y",  # Try again?
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
-            "tests/files/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
+            "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "strongPass",  # Enter 1/1 the ONLINE`s private key password
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
@@ -420,15 +420,15 @@
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step2
         input_step2 = [
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
-            "tests/files/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
+            "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "wrong password",  # Enter 1/1 the ONLINE`s private key password
             "n",  # Try again?
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
@@ -447,21 +447,21 @@
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step3 with same key in input_step2 (online key)
         input_step3 = [
             "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
-            "tests/files/online.key",  # Enter 1/2 the root`s private key path
+            "tests/files/key_storage/online.key",  # Enter 1/2 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
             "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
-            "tests/files/JanisJoplin.key",  # Enter 1/2 the root`s private key path  # noqa
+            "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
             "",  # Choose 2/2 root key type [ed25519/ecdsa/rsa]
-            "tests/files/JimiHendrix.key",  # Enter 2/2 the root`s private key path  # noqa
+            "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key path  # noqa
             "strongPass",  # Enter 2/2 the root`s private key password:
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
@@ -482,15 +482,15 @@
 
         # overwrite the step 4
         # Say online key configuration is not correct, update with online-ecdsa
         # key and confirm the configuration
         input_step4 = [
             "n",  # Is the online key configuration correct? [y/n]
             "rsa",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
-            "tests/files/online-rsa.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
+            "tests/files/key_storage/online-rsa.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "strongPass",  # Enter 1/1 the ONLINE`s private key password
             "y",  # Is the online key configuration correct? [y/n]
             "y",  # Is the root configuration correct? [y/n]
             "y",  # Is the targets configuration correct? [y/n]
             "y",  # Is the snapshot configuration correct? [y/n]
             "y",  # Is the timestamp configuration correct? [y/n]
             "y",  # Is the bins configuration correct? [y/n]
@@ -521,15 +521,15 @@
         # and confirm the configuration
         input_step4 = [
             "y",  # Is the online key configuration correct? [y/n]
             "n",  # Is the root configuration correct? [y/n]
             "",  # What is the metadata expiration for the root role?(Days)
             "1",  # What is the number of keys for the root role? (2)
             "",  # Choose 1/1 root key type [ed25519/ecdsa/rsa]
-            "tests/files/JanisJoplin.key",  # Enter 1/1 the root`s private key path  # noqa
+            "tests/files/key_storage/JanisJoplin.key",  # Enter 1/1 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
             "y",  # Is the root configuration correct? [y/n]
             "y",  # Is the targets configuration correct? [y/n]
             "y",  # Is the snapshot configuration correct? [y/n]
             "y",  # Is the timestamp configuration correct? [y/n]
             "y",  # Is the bins configuration correct? [y/n]
         ]
```

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.1.1a3/tests/unit/cli/key/test_generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.1.1a3/tests/unit/helpers/test_api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/tests/unit/helpers/test_tuf.py` & `repository_service_tuf-0.1.1a3/tests/unit/helpers/test_tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a2/PKG-INFO` & `repository_service_tuf-0.1.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

