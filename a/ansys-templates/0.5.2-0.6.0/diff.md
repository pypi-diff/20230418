# Comparing `tmp/ansys-templates-0.5.2.tar.gz` & `tmp/ansys-templates-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-templates-0.5.2.tar", last modified: Mon Mar 20 12:18:15 2023, max compression
+gzip compressed data, was "ansys-templates-0.6.0.tar", last modified: Tue Apr 18 16:04:14 2023, max compression
```

## Comparing `ansys-templates-0.5.2.tar` & `ansys-templates-0.6.0.tar`

### file list

```diff
@@ -1,195 +1,194 @@
--rw-r--r--   0        0        0     1091 2023-03-20 12:17:57.019903 ansys-templates-0.5.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9473 2023-03-20 12:17:57.019903 ansys-templates-0.5.2/README.rst
--rw-r--r--   0        0        0     3046 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2271 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3563 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3558 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      472 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3701 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2780 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      478 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       17 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      282 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0      753 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      970 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       64 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      459 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rwxr-xr-x   0        0        0     3506 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3203 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       26 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       79 2023-03-20 12:17:57.023903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2468 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1076 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2104 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3240 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1184 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      826 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2952 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      802 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      110 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3119 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      765 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       57 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      103 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3104 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      954 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       43 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      115 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2880 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      862 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-03-20 12:17:57.027903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1159 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3411 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2795 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6579 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1010 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1883 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1084 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3182 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0      994 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     2889 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      283 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     4776 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3052 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      214 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       17 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     7477 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      929 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      443 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3351 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3636 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    30006 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-03-20 12:17:57.031903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       52 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      916 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0     9913 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0   749872 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
--rw-r--r--   0        0        0      121 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
--rw-r--r--   0        0        0     2030 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
--rw-r--r--   0        0        0     4695 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
--rw-r--r--   0        0        0     5241 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
--rw-r--r--   0        0        0      593 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
--rw-r--r--   0        0        0       20 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1430 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-03-20 12:17:57.035903 ansys-templates-0.5.2/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 ansys-templates-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:04:01.152234 ansys-templates-0.6.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9732 2023-04-18 16:04:01.152234 ansys-templates-0.6.0/README.rst
+-rw-r--r--   0        0        0     3132 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2271 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3563 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3558 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3729 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      282 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4078 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2903 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3070 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3055 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2831 2023-04-18 16:04:01.156232 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1110 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2619 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1010 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1035 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      994 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     2840 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      283 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     4828 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3060 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     8371 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3351 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3825 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    34868 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       52 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      916 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0     9913 2023-04-18 16:04:01.160230 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0   749872 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
+-rw-r--r--   0        0        0      121 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
+-rw-r--r--   0        0        0     2030 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
+-rw-r--r--   0        0        0     4695 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
+-rw-r--r--   0        0        0     5241 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
+-rw-r--r--   0        0        0       20 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-04-18 16:04:01.164228 ansys-templates-0.6.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11220 1970-01-01 00:00:00.000000 ansys-templates-0.6.0/PKG-INFO
```

### Comparing `ansys-templates-0.5.2/LICENSES/MIT.txt` & `ansys-templates-0.6.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/README.rst` & `ansys-templates-0.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 .. IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 .. FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 .. AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 .. LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 .. OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 .. SOFTWARE.
 
-Welcome to Ansys templates
-==========================
-|pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
+Ansys templates
+===============
+|ansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
+.. |ansys| image:: https://img.shields.io/badge/Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://github.com/ansys
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/ansys-templates?logo=pypi
    :target: https://pypi.org/project/ansys-templates/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-templates.svg?logo=python&logoColor=white
@@ -48,14 +48,16 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
+.. |implemented| image:: <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path d="M21.03 5.72a.75.75 0 0 1 0 1.06l-11.5 11.5a.747.747 0 0 1-1.072-.012l-5.5-5.75a.75.75 0 1 1 1.084-1.036l4.97 5.195L19.97 5.72a.75.75 0 0 1 1.06 0Z"></path></svg>
+
 
 The ``ansys-templates`` repository holds a collection of useful templates compliant
 with PyAnsys guidelines. It also provides the ``ansys-templates`` command line tool
 for interactively generating new projects based on previous templates.
 
 The main advantages of using this tool are:
 
@@ -73,15 +75,15 @@
 
 
 How to install
 --------------
 Users can install ``ansys-templates`` by running:
 
 .. code-block:: text
-        
+
     python -m pip install ansys-templates
 
 The usage of `pipx`_ is encouraged too. See `installing ansys-templates using
 pipx`_.
 
 .. _pipx: https://pypa.github.io/pipx/
 .. _installing ansys-templates using pipx: https://templates.pyansys.com/getting_started/index.html#installing-pipx
```

### Comparing `ansys-templates-0.5.2/pyproject.toml` & `ansys-templates-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -22,52 +22,54 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "0.5.2"
+version = "0.6.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
-    {name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"},
+    {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata >=4.0",
     "click>=7.0,<8.0.0",
     "cookiecutter>=2.1.0",
     "isort>=5.10.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.2.1",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.8.2",
+    "ansys-sphinx-theme==0.9.7",
     "numpydoc==1.5.0",
     "sphinx==5.3.0",
-    "sphinx-copybutton==0.5.1",
+    "sphinx-copybutton==0.5.2",
 ]
 
 [tool.flit.module]
 name = "ansys.templates"
 
 [project.scripts]
 ansys-templates = "ansys.templates.cli:main"
@@ -75,23 +77,23 @@
 [project.urls]
 Source = "https://github.com/ansys-templates/ansys-templates"
 Homepage = "https://templates.ansys.com/"
 Documentation = "https://templates.ansys.com/"
 Tracker = "https://github.com/ansys/ansys-templates/issues"
 
 [tool.black]
-force-exclude = ["src/ansys/templates/python"]
+force-exclude = ["src/ansys/templates/python/"]
 line-length = "100"
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = "100"
 default_section = "THIRDPARTY"
-skip_glob = ["src/ansys/templates/python/*"] 
+skip_glob = ["src/ansys/templates/python/*"]
 filter_files = "true"
 src_paths = ["doc", "src", "tests"]
 
 [tool.coverage.run]
 source = ["ansys/templates"]
 omit = ["ansys/templates/python/*"]
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/__init__.py` & `ansys-templates-0.6.0/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/__main__.py` & `ansys-templates-0.6.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/cli.py` & `ansys-templates-0.6.0/src/ansys/templates/cli.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/licenses/LICENSE_MIT` & `ansys-templates-0.6.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/paths.py` & `ansys-templates-0.6.0/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: GitHub CI
+name: CI
 on:
   pull_request:
   push:
     tags:
       - "*"
     branches:
       - main
@@ -19,23 +19,23 @@
 
 jobs:
 
   code-style:
     name: "Code style"
     runs-on: ubuntu-latest
     steps:
-      - uses: pyansys/actions/code-style@v2
+      - uses: pyansys/actions/code-style@v4
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
 
   doc-style:
     name: "Documentation style"
     runs-on: ubuntu-latest
     steps:
-      - uses: pyansys/actions/doc-style@v2
+      - uses: pyansys/actions/doc-style@v4
         with:
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
   smoke-tests:
     name: "Build and Smoke tests"
     runs-on: {{ '${{ matrix.os }}' }}
     needs: [code-style]
@@ -48,15 +48,15 @@
         {%- for minor in range(7, 11) -%}
         {%- if minor >= required_minor -%}
         {{ python_versions.append("3." + minor | string ) or ''}}
         {%- endif -%}
         {%- endfor -%}
         python-version: {{ python_versions }}
     steps:
-      - uses: pyansys/actions/build-wheelhouse@v2
+      - uses: pyansys/actions/build-wheelhouse@v4
         with:
           library-name: {{ '${{ env.LIBRARY_NAME }}' }}
           library-namespace: {{ '${{ env.LIBRARY_NAMESPACE }}' }}
           operating-system: {{ '${{ matrix.os }}' }}
           python-version: {{ '${{ matrix.python-version }}' }}
 
   tests:
@@ -72,51 +72,53 @@
        {%- if minor >= required_minor -%}
        {{ python_versions.append("3." + minor | string ) or ''}}
        {%- endif -%}
        {%- endfor -%}
        python-version: {{ python_versions }}
       fail-fast: false
     steps:
-      - uses: pyansys/actions/tests-pytest@v2
+      - uses: pyansys/actions/tests-pytest@v4
         with:
           pytest-extra-args: "--cov=ansys --cov-report=term --cov-report=html:.cov/html"
 
   doc-build:
     name: "Build documentation"
     runs-on: ubuntu-latest
     needs: [doc-style]
     steps:
-      - uses: pyansys/actions/doc-build@v2
+      - uses: pyansys/actions/doc-build@v4
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
 
+  build-library:
+    name: "Build library basic example"
+    runs-on: ubuntu-latest
+    needs: [doc-build, tests]
+    steps:
+      - uses: pyansys/actions/build-library@v4
+        with:
+          library-name: {{ '${{ env.LIBRARY_NAME }}' }}
+          python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
+
   doc-deploy-dev:
     name: "Deploy development documentation"
     runs-on: ubuntu-latest
-    needs: [doc-build]
-    if: github.event_name == 'push'
+    needs: [build-library]
+    if: github.event_name == 'push' && !contains(github.ref, 'refs/tags')
     steps:
-      - uses: pyansys/actions/doc-deploy-dev@v2
+      - uses: pyansys/actions/doc-deploy-dev@v4
         with:
           cname: {{ '${{ env.DOCUMENTATION_CNAME }}' }}
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
   doc-deploy-stable:
     name: "Deploy stable documentation"
     runs-on: ubuntu-latest
-    needs: [doc-deploy-dev]
+    needs: [build-library]
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags')
     steps:
-      - uses: pyansys/actions/doc-deploy-stable@v2
+      - uses: pyansys/actions/doc-deploy-stable@v4
         with:
           cname: {{ '${{ env.DOCUMENTATION_CNAME }}' }}
           token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
-  build-library:
-    name: "Build library basic example"
-    runs-on: ubuntu-latest
-    needs: [tests, doc-deploy-stable]
-    steps:
-      - uses: pyansys/actions/build-library@v2
-        with:
-          library-name: {{ '${{ env.LIBRARY_NAME }}' }}
-          python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
+
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       with:
         repo-token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
         sync-labels: ''
 
     # Label based on branch name
     - uses: actions-ecosystem/action-add-labels@v1
       if: |
-        startsWith(github.event.pull_request.head.ref, 'doc') || 
+        startsWith(github.event.pull_request.head.ref, 'doc') ||
         startsWith(github.event.pull_request.head.ref, 'docs')
       with:
         labels: documentation
 
     - uses: actions-ecosystem/action-add-labels@v1
       if: |
         startsWith(github.event.pull_request.head.ref, 'maint') ||
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :clean
-rmdir /s /q %BUILDDIR% > /NUL 2>&1 
+rmdir /s /q %BUILDDIR% > /NUL 2>&1
 for /d /r %SOURCEDIR% %%d in (_autosummary) do @if exist "%%d" rmdir /s /q "%%d"
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """Sphinx documentation configuration file."""
 from datetime import datetime
+import os
 
+from ansys_sphinx_theme import get_version_match
 {%- if cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "white" %}
 from ansys_sphinx_theme import ansys_logo_white as logo
 {%- elif cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "black" %}
 from ansys_sphinx_theme import ansys_logo_black as logo
 {%- elif cookiecutter.__logo == "pyansys" and cookiecutter.__logo_color == "white" %}
 from ansys_sphinx_theme import pyansys_logo_white as logo
 {%- elif cookiecutter.__logo == "pyansys" and cookiecutter.__logo_color == "black" %}
 from ansys_sphinx_theme import pyansys_logo_black as logo
 {%- endif %}
 
+{%- if cookiecutter.__template_name != "doc-project" %}
+from {{cookiecutter.__pkg_namespace}} import __version__
+{%- endif %}
+
+
 # Project information
 {%- if cookiecutter.__template_name in ["doc-project"] %}
 project = "{{ cookiecutter.__project_name_slug }}"
 {%- else %}
 project = "{{ cookiecutter.__pkg_name }}"
 {%- endif %}
 copyright = f"(c) {datetime.now().year} ANSYS, Inc. All rights reserved"
 author = "ANSYS, Inc."
+{%- if cookiecutter.__template_name != "doc-project" %}
+release = version = __version__
+{%- elif cookiecutter.__template_name == "doc-project" %}
 release = version = "{{ cookiecutter.__version }}"
+{%- endif %}
+cname = os.getenv("DOCUMENTATION_CNAME", "docs.pyansys.com")
 
 # Select desired logo, theme, and declare the html title
 html_logo = logo
 html_theme = "ansys_sphinx_theme"
 html_short_title = html_title = "{{ cookiecutter.__project_name_slug }}"
 
 # specify the location of your github repo
@@ -34,14 +46,19 @@
     "additional_breadcrumbs": [
         {%- if cookiecutter.__logo == "ansys" %}
         ("Ansys", "https://dev.docs.ansys.com/"),
         {%- elif cookiecutter.__logo == "pyansys" %}
         ("PyAnsys", "https://docs.pyansys.com/"),
         {%- endif %}
     ],
+    "switcher": {
+        "json_url": f"https://{cname}/versions.json",
+        "version_match": get_version_match(__version__),
+    },
+    "check_switcher": False,
 }
 
 # Sphinx extensions
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "numpydoc",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,27 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata >=4.0",
 ]
 
+[project.optional-dependencies]
+tests = [
+    "pytest==7.3.0",
+    "pytest-cov==4.0.0",
+]
+doc = [
+    "ansys-sphinx-theme==0.9.7",
+    "numpydoc==1.5.0",
+    "sphinx==5.3.0",
+    "sphinx-copybutton==0.5.1",
+]
+
+
 [tool.flit.module]
 name = "{{ cookiecutter.__pkg_namespace }}"
 
 [project.urls]
 Source = "{{ cookiecutter.__repository_url }}"
 Tracker = "{{ cookiecutter.__repository_url }}/issues"
 Homepage = "{{ cookiecutter.__repository_url }}"
@@ -47,15 +60,15 @@
 {% elif cookiecutter.__build_system == "poetry"  %}
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "{{ cookiecutter.__pkg_name }}"
 version = "{{ cookiecutter.__version }}"
 description = "{{ cookiecutter.__short_description }}"
 license = "MIT"
-authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
+authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "{{ cookiecutter.__repository_url }}"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -70,32 +83,32 @@
 importlib-metadata = {version = "^4.0", python = "<3.8"}
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
-Sphinx = "^5.1.1"
-numpydoc = "^1.4.0"
-ansys-sphinx-theme = "^0.4.2"
-sphinx-copybutton = "^0.5.0"
+Sphinx = "^5.3.0"
+numpydoc = "^1.5.0"
+ansys-sphinx-theme = "^0.9.7"
+sphinx-copybutton = "^0.5.1"
 
 # Optional testing dependencies
 [tool.poetry.group.tests]
 optional = true
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pytest = "^7.3.0"
+pytest-cov = "^4.0.0"
 
 # Optional build requirements
 [tool.poetry.group.build]
 optional = true
 [tool.poetry.group.build.dependencies]
-build = "^0.8.0"
-twine = "^4.0.1"
+build = "^0.10.0"
+twine = "^4.0.2"
 {% endif %}
 [tool.black]
 line-length = {{ cookiecutter.__max_linelength }}
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 [tox]
 description = Default tox environments list
 envlist =
-    style,{py37,py38,py39,py310}{,-coverage},doc
+    style,{py37,py38,py39,py310,py311}{,-coverage},doc
 skip_missing_interpreters = true
 {%- if cookiecutter.__build_system != "setuptools" %}
 isolated_build = true
 {%- if cookiecutter.__build_system == "flit" %}
 isolated_build_env = build
 {%- endif %}
 {%- endif %}
 
-[gh-actions]
-description = The tox environment to be executed in gh-actions for a given python version
-python =
-    3.7: style,py37-coverage,doc
-    3.8: style,py38-coverage,doc
-    3.9: style,py39-coverage,doc
-    3.10: style,py310-coverage,doc
-
 [testenv]
 description = Checks for project unit tests and coverage (if desired)
 basepython =
     py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
@@ -31,17 +23,20 @@
     {%- else %}
     {style,reformat,doc}: python3
     {%- endif -%}
 {%- if cookiecutter.__build_system == "poetry" %}
 skip_install = true
 whitelist_externals =
     poetry
-{%- elif cookiecutter.__build_system != "poetry" %}
+{%- elif cookiecutter.__build_system == "setuptools" %}
 deps =
     -r{toxinidir}/requirements/requirements_tests.txt
+{%- elif cookiecutter.__build_system == "flit" %}
+extras =
+    tests
 {%- endif %}
 setenv =
     PYTHONUNBUFFERED = yes
     coverage: PYTEST_EXTRA_ARGS = --cov=ansys.{{ cookiecutter.__product_name_slug }} --cov-report=term --cov-report=xml:.cov/xml --cov-report=html:.cov/html
 commands =
     {%- if cookiecutter.__build_system != "poetry" %}
     pytest {env:PYTEST_MARKERS:} {env:PYTEST_EXTRA_ARGS:} {posargs:-vv}
@@ -57,22 +52,25 @@
     pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:doc]
 description = Check if documentation generates properly
-{%- if cookiecutter.__build_system != "poetry" %}
+{%- if cookiecutter.__build_system == "setuptools" %}
 deps =
     -r{toxinidir}/requirements/requirements_doc.txt
 {%- elif cookiecutter.__build_system == "poetry" %}
 skip_install = true
 whitelist_externals =
     poetry
+{%- elif cookiecutter.__build_system == "flit" %}
+extras =
+    doc
 {%- endif %}
 commands =
     {%- if cookiecutter.__build_system != "poetry" %}
-    sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxworkdir}/doc_out" --color -vW -bhtml
+    sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxinidir}/_build/html" --color -vW -bhtml
     {%- elif cookiecutter.__build_system == "poetry" %}
     poetry install
-    poetry run sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxworkdir}/doc_out" --color -vW -bhtml
+    poetry run sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxinidir}/_build/html" --color -vW -bhtml
     {%- endif %}
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'project_name'": "'doc-project'"}*

```diff
@@ -22,15 +22,15 @@
         "setuptools"
     ],
     "logo": [
         "Ansys",
         "PyAnsys"
     ],
     "max_linelength": "100",
-    "project_name": "",
+    "project_name": "doc-project",
     "repository_url": "https://github.com/pyansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
         "3.7",
         "3.8",
         "3.9",
         "3.10"
     ],
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,25 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".github/dependabot.yml",
     ".github/labeler.yml",
     ".github/labels.yml",
     ".github/workflows/ci_cd.yml",
     ".github/workflows/label.yml",
     ".gitignore",
     "LICENSE",
     "README.rst",
     ".pre-commit-config.yaml",
-    "ignore_words.txt",
     "requirements/requirements_build.txt",
     "requirements/requirements_doc.txt",
     "tox.ini",
 ]
 """A list holding all desired files to be included in the project."""
 
 
@@ -59,17 +57,17 @@
 
     # Apply isort with desired config
     isort_config = isort.settings.Config(
         line_length="{{ cookiecutter.__max_linelength }}",
         profile="black",
     )
     filepaths_list = [
-        project_path / "doc/source/conf.py",
+        project_path / "doc" / "source" / "conf.py",
     ]
     for filepath in filepaths_list:
-        isort.api.sort_file(filepath, isort_config)
+        isort.api.sort_file(filepath, config=isort_config)
 
     # Apply the desired structure to the project
     keep_files(DESIRED_STRUCTURE)
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         run: tox -e style
 
   docs-style:
     name: Documentation Style Check
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-  
+
       - name: Running Vale
         uses: errata-ai/vale-action@reviewdog
         env:
           GITHUB_TOKEN: {{ '${{secrets.GITHUB_TOKEN}}' }}
         with:
           files: doc
           reporter: github-pr-check
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 repos:
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.1.0
   hooks:
   - id: black
-    args: ["doc/source/conf.py"]
+    args: ["doc/"]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
     args: [
       "--profile", "black",
       "--force-sort-within-sections",
       "--line-length", "100",
     ]
 
 - repo: https://gitlab.com/PyCQA/flake8
-  rev: 3.9.2
+  rev: 6.0.0
   hooks:
   - id: flake8
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.1.0
+  rev: v2.2.2
   hooks:
   - id: codespell
-    args: [--ignore-words=ignore_words.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
+    args: [--ignore-words=doc/styles/Vocab/ANSYS/accept.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.1.0
+  rev: v4.4.0
   hooks:
   - id: check-merge-conflict
   - id: debug-statements
 
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.16.0
+  rev: 0.21.0
   hooks:
     - id: check-github-workflows
       name: "Check GitHub workflows"
       files: ^\.github/workflows/
       types: [yaml]
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.6.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 [testenv:doc]
 description = Checks if project documentation properly builds
 skip_install = false
 deps =
     -r{toxinidir}/requirements/requirements_doc.txt
 allowlist_externals=*
-commands = 
+commands =
     sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxworkdir}/doc_out_html" --color -vW -b html
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ---------------------------
 FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update \ 
-    && apt-get install -y \ 
+RUN apt-get update \
+    && apt-get install -y \
     && rm -rf /var/lib/apt/lists/*
 
 WORKDIR /app
 
 COPY requirements/requirements_build.txt .
 
 RUN pip install --no-cache-dir --upgrade pip && \
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ---------------------------
 FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update \ 
-    && apt-get install -y \ 
+RUN apt-get update \
+    && apt-get install -y \
     && rm -rf /var/lib/apt/lists/*
 
 WORKDIR /app
 
 COPY requirements/requirements_build.txt .
 
 RUN pip install --no-cache-dir --upgrade pip && \
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # ---------------------------
 FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update \ 
-    && apt-get install -y \ 
+RUN apt-get update \
+    && apt-get install -y \
     && rm -rf /var/lib/apt/lists/*
 
 WORKDIR /app
 
 COPY requirements/requirements_build.txt .
 
 RUN pip install --no-cache-dir --upgrade pip && \
     pip install --no-cache-dir -r requirements_build.txt
 
 RUN mkdir stubs
 
 ADD protobufs/ ./protobufs/
 RUN python -m grpc_tools.protoc  \
-    -I ./protobufs  \ 
+    -I ./protobufs  \
     --python_out=./stubs \
     --grpc_python_out=./stubs  \
     ./protobufs/*.proto
 
 # ---------------------------
 FROM base AS test
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # Keeps Python from generating .pyc files in the container
 ENV PYTHONDONTWRITEBYTECODE=1
 
 # Turns off buffering for easier container logging
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update \ 
-    && apt-get install -y \ 
+RUN apt-get update \
+    && apt-get install -y \
     && rm -rf /var/lib/apt/lists/*
 
 COPY requirements/requirements_build.txt ./
 
 RUN pip install --no-cache-dir --upgrade pip && \
     pip install --no-cache-dir -r requirements_build.txt
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     "LICENSE",
     "pyproject.toml",
     "README.rst",
     "requirements_build.txt",
     "requirements_doc.txt",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 For developers
 ^^^^^^^^^^^^^^
 
 Installing Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }} in developer mode allows
 you to modify the source and enhance it.
 
-Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will 
+Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will
 need to follow these steps:
 
 #. Start by cloning this repository:
 
    .. code:: bash
 
       git clone {{ cookiecutter.repository_url }}
@@ -55,29 +55,29 @@
    .. code:: bash
 
       python -m pip install -U pip
 
 #. Install the project in editable mode:
 
    .. code:: bash
-    
+
       python -m pip install --editable {{ cookiecutter.__pkg_name }}
 
 #. Install additional requirements (if needed):
 
    .. code:: bash
 
       python -m pip install -r requirements/requirements_build.txt
       python -m pip install -r requirements/requirements_doc.txt
       python -m pip install -r requirements/requirements_tests.txt
 
 #. Finally, verify your development installation by running:
 
    .. code:: bash
-        
+
       python -m pip install -r requirements/requirements_tests.txt
       pytest tests -v
 
 
 Style and Testing
 -----------------
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,32 +19,28 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".github/dependabot.yml",
     ".github/labeler.yml",
     ".github/labels.yml",
     ".github/workflows/ci_cd.yml",
     ".github/workflows/label.yml",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
     "pyproject.toml",
     "README.rst",
-    "requirements/requirements_build.txt",
-    "requirements/requirements_doc.txt",
-    "requirements/requirements_tests.txt",
     "src/ansys/{{ cookiecutter.__product_name_slug }}/{{ cookiecutter.__library_name_slug }}/__init__.py",
     "tests/test_metadata.py",
     "tox.ini",
 ]
 """A list holding all desired files to be included in the project."""
 
 def main():
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -58,25 +58,25 @@
     python -m pip install {{ cookiecutter.__pkg_name }}
 
 {% elif cookiecutter.build_system == "poetry" -%}
 
 .. code:: bash
 
     poetry run python -m pip install {{ cookiecutter.__pkg_name }}
-    
+
 {% endif -%}
 
 
 For developers
 ^^^^^^^^^^^^^^
 
 Installing Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }} in developer mode allows
 you to modify the source and enhance it.
 
-Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will 
+Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will
 need to follow these steps:
 
 #. Start by cloning this repository:
 
    .. code:: bash
 
       git clone {{ cookiecutter.repository_url }}
@@ -106,40 +106,40 @@
       python -m pip install -r requirements/requirements_doc.txt
       python -m pip install -r requirements/requirements_tests.txt
 
 
 #. Install the project in editable mode:
 
     {% if cookiecutter.build_system in ["flit", "setuptools"] -%}
-    
+
    .. code:: bash
-    
+
       python -m pip install --editable {{ cookiecutter.__pkg_name }}
-    
+
     {% elif cookiecutter.build_system == "poetry" -%}
-    
+
    .. code:: bash
-    
+
       poetry run python -m pip install {{ cookiecutter.__pkg_name }}
-        
+
     {% endif -%}
 
 #. Finally, verify your development installation by running:
 
    .. code:: bash
-        
+
       tox
 
 
 How to testing
 --------------
 
 This project takes advantage of `tox`_. This tool allows to automate common
 development tasks (similar to Makefile) but it is oriented towards Python
-development. 
+development.
 
 Using tox
 ^^^^^^^^^
 
 As Makefile has rules, `tox`_ has environments. In fact, the tool creates its
 own virtual environment so anything being tested is isolated from the project in
 order to guarantee project's integrity. The following environments commands are provided:
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files 9% similar despite different names*

```diff
@@ -18,36 +18,36 @@
     steps:
     - name: Get Bot Application Token
       id: get_workflow_token
       uses: peter-murray/workflow-application-token-action@v1
       with:
         application_id: {{ '${{ secrets.BOT_APPLICATION_ID }}' }}
         application_private_key: {{ '${{ secrets.BOT_APPLICATION_PRIVATE_KEY }}' }}
-    
+
     - uses: actions/checkout@v2
       with:
         token: {{ '${{ steps.get_workflow_token.outputs.token }}' }}
-    
+
     - name: Set up JDK 11
       uses: actions/setup-java@v2
       with:
         java-version: '11'
         distribution: 'adopt'
         cache: maven
-    
+
     - name: Clean library folder
       run: rm -rf {{ cookiecutter.__pkg_name }}
-      
+
     - name: Build client library
       run: mvn -Dbuild-id={{ '${{ github.run_number }}' }} -s .m2/settings.xml compile
       env:
         MAVEN_OPTS: "-Dlog4j2.formatMsgNoLookups=true"
         SERVER_USERNAME: {{ '${{ secrets.REPO_USER }}' }}
         SERVER_PASSWORD: {{ '${{ secrets.REPO_TOKEN }}' }}
-        
+
     - name: Create Pull Request
       uses: peter-evans/create-pull-request@v3
       with:
         commit-message: Update client library
         committer: GitHub <noreply@github.com>
         author: {{ '${{ github.actor }}' }} <{{ '${{ github.actor }}' }}@users.noreply.github.com>
         signoff: false
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys-templates-0.6.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     "pyproject.toml",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -52,30 +52,30 @@
    .. code:: bash
 
       python -m pip install -U pip
 
 #. Install the project in editable mode:
 
    .. code:: bash
-    
+
       python -m pip install --editable {{ cookiecutter.__pkg_name }}
 
 #. Install additional requirements (if needed):
 
    .. code:: bash
 
       python -m pip install -r requirements_build.txt
       python -m pip install -r requirements_doc.txt
       python -m pip install -r requirements_tests.txt
 
 
 #. Finally, verify your development installation by running:
 
    .. code:: bash
-        
+
       python -m pip install -r requirements_tests.txt
       pytest tests -vv
 
 
 Style and Testing
 -----------------
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys-templates-0.6.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/cookiecutter.json` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 DESIRED_STRUCTURE = [
     ".github/workflows/ci.yml",
     ".vscode/launch.json",
     "doc/source/_static/ansys-solutions-logo-black-background.png",
     "doc/source/_static/README.md",
     "doc/source/_templates/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/styles/.gitignore",
     "doc/.vale.ini",
     "doc/make.bat",
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     types: [opened, reopened, synchronize, ready_for_review]
   release:
     types: [published]
   workflow_dispatch:
 
 env:
   MAIN_PYTHON_VERSION: "3.8"
+  # To be updated with GitHub pages url.
   DOCUMENTATION_CNAME: '{{ cookiecutter.__solution_name_slug }}.docs.solutions.ansys.com'
-  POETRY_VERSION: "1.4"
-  TOX_VERSION: "3.27.1"
+  # When changing this value, update setup_environment.py --build-system-version default value to match
+  POETRY_VERSION: "1.4.2"
   POETRY_HTTP_BASIC_SOLUTIONS_PRIVATE_PYPI_USERNAME: "PAT"
   POETRY_HTTP_BASIC_SOLUTIONS_PRIVATE_PYPI_PASSWORD: {{ '${{ secrets.SOLUTIONS_PRIVATE_PYPI_PAT }}' }}
 
 concurrency:
   group: {{ '${{ github.workflow }}-${{ github.ref }}' }}
   cancel-in-progress: true
 
@@ -31,123 +32,122 @@
       github.event_name == 'pull_request' &&
       github.event.pull_request.draft == false ||
       github.event_name == 'push'
     name: Check documentation style
     runs-on: [ubuntu-latest]
     steps:
       - name: Check documentation style
-        uses: Solution-Applications/actions/check-doc-style@v0.2.1
+        uses: Solution-Applications/actions/check-doc-style@v2.1.0
         with:
           gh-token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
 
   build-doc:
     if: |
       github.event_name == 'pull_request' &&
       github.event.pull_request.draft == false ||
       github.event_name == 'push'
     name: Build documentation
     runs-on: [ubuntu-latest]
     needs: [check-doc-style]
     steps:
       - name: Build documentation
-        uses: Solution-Applications/actions/build-doc@v0.2.1
+        uses: Solution-Applications/actions/build-doc@v2.1.0
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
           poetry-version: {{ '${{ env.POETRY_VERSION }}' }}
           documentation-artifact: html-documentation
           dependencies-source: build-system
 
   deploy-doc:
     if: |
       github.event_name == 'push'
     name: Deploy documentation
     runs-on: [ubuntu-latest]
     needs: [build-doc]
     steps:
       - name: Deploy documentation
-        uses: Solution-Applications/actions/deploy-doc@v0.2.1
+        uses: Solution-Applications/actions/deploy-doc@v2.1.0
         with:
           gh-token: {{ '${{ secrets.WORKFLOW_TOKEN }}' }}
           documentation-artifact: html-documentation
-          cname: {{ '${{ env.DOCUMENTATION_CNAME }}' }}
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
           render-last: 10
           short-version: false
 
   check-copyright:
     if: |
       github.event_name == 'pull_request' &&
-      github.event.pull_request.draft == false 
+      github.event.pull_request.draft == false
     name: Check copyright
     runs-on: [ubuntu-latest]
     steps:
       - name: Check copyright
-        uses: Solution-Applications/actions/check-copyright@v0.2.1
+        uses: Solution-Applications/actions/check-copyright@v2.1.0
         with:
           gh-token: {{ '${{ secrets.WORKFLOW_TOKEN }}' }}
 
   check-code-style:
     if: |
       github.event_name == 'pull_request' &&
-      github.event.pull_request.draft == false 
+      github.event.pull_request.draft == false
     name: Check code style
     runs-on: [ubuntu-latest]
     steps:
       - name: Check code style
-        uses: Solution-Applications/actions/check-code-style@v0.2.1
+        uses: Solution-Applications/actions/check-code-style@v2.1.0
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
           tox-version: {{ '${{ env.TOX_VERSION }}' }}
-          
+
   build:
     if: |
       github.event.pull_request.draft == false
-    name: Build 
+    name: Build
     runs-on: [windows-latest]
     steps:
       - name: Build
-        uses: Solution-Applications/actions/build@v0.2.1
+        uses: Solution-Applications/actions/build@v2.1.0
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
           poetry-version: {{ '${{ env.POETRY_VERSION }}' }}
           solutions-pypi-token: {{ '${{ secrets.SOLUTIONS_PRIVATE_PYPI_PAT }}' }}
           artifact-name: wheel
           run-in-venv: false
           dependencies-source: build-system
           retention-days: 7
-          
+
   run-tests:
     if: |
       github.event_name == 'pull_request' &&
-      github.event.pull_request.draft == false 
+      github.event.pull_request.draft == false
     name: Run tests
     runs-on: [windows-latest]
     strategy:
       matrix:
-        python-version: ['3.7', '3.8']
+        python-version: ['3.8', '3.9', '3.10']
       fail-fast: false
     steps:
       - name: Run tests
-        uses: Solution-Applications/actions/run-tests@v0.2.1
+        uses: Solution-Applications/actions/run-tests@v2.1.0
         with:
           python-version: {{ '${{ matrix.python-version }}' }}
           poetry-version: {{ '${{ env.POETRY_VERSION }}' }}
           tox-version: {{ '${{ env.TOX_VERSION }}' }}
           check-coverage-ratio: false
           min-coverage-ratio: 80
-          run-in-venv: true
+          run-in-venv: false
           retention-days: 7
 
   release:
     if: |
       github.event_name == 'release'
     name: Release
     needs: [build]
     runs-on: [ubuntu-latest]
     steps:
       - name: Release
-        uses: Solution-Applications/actions/release@v0.2.1
+        uses: Solution-Applications/actions/release@v2.1.0
         with:
           python-version: {{ '${{ env.MAIN_PYTHON_VERSION }}' }}
           gh-token: {{ '${{ secrets.WORKFLOW_TOKEN }}' }}
           solutions-pypi-token: {{ '${{ secrets.SOLUTIONS_PRIVATE_PYPI_PAT }}' }}
           solutions-pypi-repository-url: https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/upload/
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
+.poetry
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ANSYS, Inc. Legal Notices
 ==========================
 
 Copyright and Trademark Information
 ------------------------------------
 
-© 2022 ANSYS, Inc. All rights reserved. Unauthorized use, distribution, or duplication is prohibited. This solution is subject to U.S. laws governing export and re-export.
+© 2023 ANSYS, Inc. All rights reserved. Unauthorized use, distribution, or duplication is prohibited. This solution is subject to U.S. laws governing export and re-export.
 
 ANSYS, Ansys Workbench, AUTODYN, CFX, FLUENT and any and all ANSYS, Inc. brand, product, service and feature names, logos and slogans are registered trademarks or trademarks of ANSYS, Inc. or its subsidiaries located in the United States or other countries. ICEM CFD is a trademark used by ANSYS, Inc. under license. CFX is a trademark of Sony Corporation in Japan. All other brand, product, service, and feature names or trademarks are the property of their respective owners. FLEXlm and FLEXnet are trademarks of Flexera Software LLC.
 
 Disclaimer Notice
 -----------------
 
 THIS ANSYS SOFTWARE PRODUCT AND PROGRAM DOCUMENTATION INCLUDE TRADE SECRETS AND ARE CONFIDENTIAL AND PROPRIETARY PRODUCTS OF ANSYS, INC., ITS SUBSIDIARIES, OR LICENSORS. The software products and documentation are furnished by ANSYS, Inc., its subsidiaries, or affiliates under a software license agreement that contains provisions concerning non-disclosure, copying, length and nature of use, compliance with exporting laws, warranties, disclaimers, limitations of liability, and remedies, and other provisions. The software products and documentation may be used, disclosed, transferred, or copied only in accordance with the terms and conditions of that software license agreement.
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ##############################################
 Ansys Solutions {{cookiecutter.solution_name}}
 ##############################################
 
 .. note::
-  This content needs to be configured according to the project specifics. 
+  This content needs to be configured according to the project specifics.
 
 
 Introduction
 ============
 
 .. note::
   Add here a description of the project.
@@ -29,36 +29,36 @@
 ~~~~~~~~~~~~~~~~~~~~~~
 
 .. note::
   Add here the supported Python versions.
 
 For example:
 
-  Officially Python 3.7 to 3.8.
+  Officially Python 3.8 to 3.10
 
 Private PyPI servers
 ~~~~~~~~~~~~~~~~~~~~
 
 Connection to Ansys-Solutions private PyPI server is required. Access is controlled via a ``Personal Access Token (PAT)`` which is available
 in the `Solutions Developer's Guide <https://dev-docs.solutions.ansys.com/index.html>`_. To declare the PAT on your system:
 
-  1. Visit the `Connecting to the private PyPI <https://dev-docs.solutions.ansys.com/how_to/get_started_org.html#connecting-to-the-private-pypi>`_ section of the `Solutions Developer's Guide <https://dev-docs.solutions.ansys.com/index.html>`_,
+  1. Visit the `Connecting to the private PyPI <https://dev-docs.solutions.ansys.com/getting_started/canonical_development_environment.html#connecting-to-the-private-pypi-servers>`_ section of the `Solutions Developer's Guide <https://dev-docs.solutions.ansys.com/index.html>`_,
      navigate to the Private PyPI servers section and copy the token related to Ansys-Solutions PyPI.
 
   2. Create a system environment variable named SOLUTIONS_PRIVATE_PYPI_PAT and assign the token.
-  
+
 .. note::
-  In addition to the Ansys-Solutions private PyPI server, you can add several private sources such as PyAnsys private PyPI server. 
+  In addition to the Ansys-Solutions private PyPI server, you can add several private sources such as PyAnsys private PyPI server.
 
 Flagship products
 ~~~~~~~~~~~~~~~~~
 
 .. note::
-  Add here the name and the versions of Ansys flagship products needed to run the solution. 
-  Remove this section if useless. 
+  Add here the name and the versions of Ansys flagship products needed to run the solution.
+  Remove this section if useless.
 
 For example:
 
   .. list-table:: Required flagship products
     :widths: 200 100
     :header-rows: 1
 
@@ -77,14 +77,30 @@
 Setup the development environment
 ---------------------------------
 
 In order to start using the solution or to develop inside the solution you need to install the Python ecosystem required.
 
 ``poetry`` is the dependency manager tool used in this project. The dependencies are declared in ``pyproject.toml`` at project root.
 
+From now on, the version of the dependency manager tool must be defined in the pyproject.toml file.
+
+For example, if you are using Poetry version 1.4.2 (the latest poetry version), the following lines must be part of your pyproject.toml file, after the ``build-system`` section:
+
+  .. code:: bash
+
+    [build-system-requirements]
+    build-system-version = "1.4.2"
+
+For this project, the poetry version used is 1.4.2.
+
+Otherwise if you want to use the version of poetry of your choice, you can use the -s option to run the setup_environment.py script.
+For example, ``python setup_environment.py -d all -s 1.3``
+
+Last but not least, please make sure that the version of poetry in your pyproject.toml file is the same as in the ci.yml file (located in the .github\workflows folder) for consistency.
+
 Automatic installation
 ~~~~~~~~~~~~~~~~~~~~~~
 
 The automatic installation consists in running the setup_environment.py script at project root. Basically, this script creates a virtual environment,
 and installs the dependency management tool ``poetry``. The ``-d`` option is used to specify the group of dependencies to install. For production
 dependencies use ``-d run``, for doc dependencies use ``-d doc``, for tests dependencies ``-d tests``, and for build dependencies use ``-d build``.
 
@@ -92,21 +108,27 @@
 
 1. Navigate to project root:
 
   .. code:: bash
 
     cd {{ cookiecutter.__project_name_slug }}
 
-2. Setup the Python environment (the ``-d all`` option means that ``run``, ``doc``, ``tests``, and ``build`` dependencies will be installed):
+2. Install ``toml`` and ``packaging``:
+
+  .. code:: bash
+
+    pip install toml packaging
+
+3. Setup the Python environment (the ``-d all`` option means that ``run``, ``doc``, ``tests``, and ``build`` dependencies will be installed):
 
   .. code:: bash
 
     python setup_environment.py -d all
 
-3. Activate the virtual environment:
+4. Activate the virtual environment:
 
   * For Linux system:
 
     .. code:: bash
 
       source .venv/bin/activate
 
@@ -123,15 +145,15 @@
       .venv\Scripts\Activate.ps1
 
 From now on, all the commands listed in the documentation must be executed within the virtual environment.
 
 Update dependencies
 ~~~~~~~~~~~~~~~~~~~
 
-To add a new dependency or to update the version of an existing dependency use the ``poetry add`` command. 
+To add a new dependency or to update the version of an existing dependency use the ``poetry add`` command.
 
 For packages collected from public PyPI run:
 
   .. code:: bash
 
     poetry add <name-of-package>
 
@@ -164,48 +186,48 @@
 
 
 Code style check
 ================
 
 In this project, the following code style checks are required:
 
-  * black 
+  * black
 
   * isort
 
   * flake8
 
   * codespell
 
   * pydocstyle
 
 All-in-one checks using pre-commit
 ----------------------------------
 
 All those checks can be triggered with one single tool: ``pre-commit``. ``pre-commit`` is a GIT hook allowing to trigger all the code style commands at once at the point when you perform a git commit.
-``pre-commit`` prevents you from forgetting to run the required actions against your code and it ensures the exact same style policies are applied. The code style policy is defined in the 
-``.pre-commit-config.yaml`` at project root. 
+``pre-commit`` prevents you from forgetting to run the required actions against your code and it ensures the exact same style policies are applied. The code style policy is defined in the
+``.pre-commit-config.yaml`` at project root.
 
 Developers are not forced but encouraged to install ``pre-commit`` via:
 
   .. code:: bash
 
     python -m pip install pre-commit
-        
+
   .. code:: bash
-        
+
     pre-commit install
 
 To run pre-commit:
 
   .. code:: bash
 
     pre-commit run --all-files --show-diff-on-failure
 
-How to remove ``pre-commit``? 
+How to remove ``pre-commit``?
 
   * Navigate to the git directory at the root of the repository
 
   * Select the hooks directory
 
   * Remove pre-commit file
 
@@ -242,15 +264,15 @@
 
     python -m codespell .
 
 
 Testing
 =======
 
-**Unit tests** and **Integration tests** are executed via the ``pytest`` framework. 
+**Unit tests** and **Integration tests** are executed via the ``pytest`` framework.
 
 To run the unit tests:
 
   .. code:: bash
 
     pytest tests/unit
 
@@ -296,15 +318,15 @@
 
 Build the package:
 
   .. code:: bash
 
     python -m build
 
-Using poetry 
+Using poetry
 ------------
 
 Build the package:
 
   .. code:: bash
 
     poetry build
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys-templates-0.6.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -20,7 +20,13 @@
 
 
 # Customized clean due to examples gallery
 clean:
 	rm -rf $(BUILDDIR)/*
 	rm -rf $(SOURCEDIR)/examples
 	find . -type d -name "_autosummary" -exec rm -rf {} +
+
+# Customized pdf for svg format images
+pdf:
+	@$(SPHINXBUILD) -M latex "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	cd $(BUILDDIR)/latex && latexmk -r latexmkrc -pdf *.tex -interaction=nonstopmode || true
+	(test -f $(BUILDDIR)/latex/*.pdf && echo pdf exists) || exit 1
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :clean
-rmdir /s /q %BUILDDIR% > /NUL 2>&1 
+rmdir /s /q %BUILDDIR% > /NUL 2>&1
 for /d /r %SOURCEDIR% %%d in (_autosummary) do @if exist "%%d" rmdir /s /q "%%d"
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Sphinx documentation configuration file."""
 
 # ==================================================== [Imports] ==================================================== #
 
 from datetime import datetime
 import os
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0,<1.3.0", "setuptools>=65.0"]
 build-backend = "poetry.core.masonry.api"
 
+[build-system-requirements]
+build-system-version = "1.4.2"
+
 [tool.poetry]
 name = "{{cookiecutter.__pkg_name}}"
 version = "{{cookiecutter.__version}}"
 description = "{{cookiecutter.__short_description}}"
 license = "Proprietary"
 authors = ["ANSYS, Inc. <solution-applications.maintainers@ansys.com>"]
 maintainers = ["ANSYS, Inc. <solution-applications.maintainers@ansys.com>"]
@@ -15,42 +18,43 @@
 keywords = ["Ansys Solutions"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Other Audience",
     "License :: Other/Proprietary License",
     "Natural Language :: English",
     "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering"
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [[tool.poetry.source]]
 name = "solutions-private-pypi"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/"
 default = false
 secondary = true
 
 # Main dependencies
 [tool.poetry.dependencies]
-python = ">=3.7, <3.9"
+python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
-ansys-saf-glow = {version = "0.1.9", source = "solutions-private-pypi" }
-ansys-saf-portal = {version = "0.1.4", source = "solutions-private-pypi"}
-toml = {version = "*"}
-tox = {version = "*"} 
-{% if cookiecutter.with_dash_ui == "yes" %} 
-dash = {version = "^2.6"}  
+ansys-saf-glow = {version = "^0.2.0", source = "solutions-private-pypi" }
+ansys-saf-portal = {version = "^0.1.6", source = "solutions-private-pypi"}
+toml = {version = "^0.10.0"} # supports python versions until 3.9
+{% if cookiecutter.with_dash_ui == "yes" %}
+dash = {version = "^2.6"}
 dash_bootstrap_components = {version = "^1.2"}
 dash-extensions = {version = "^0.1"}
 dash-iconify = {version = "^0.1"}
 dash-uploader = {version = "^0.6"}
+packaging = {version = "^23"}
 {% endif %}
 
 # Optional documentation dependencies
 [tool.poetry.group.doc]
 optional = true
 [tool.poetry.group.doc.dependencies]
 ansys-sphinx-theme = {version = "^0.8.0"}
@@ -58,15 +62,15 @@
 sphinx = {version = "5.1.0"}
 sphinx-copybutton = {version = "^0.5.1"}
 sphinx_design = {version = "^0.3.0"}
 sphinx_code_tabs = {version = "^0.5.3"}
 sphinx-gallery = {version = "^0.11.1"}
 sphinx_mdinclude= {version = "^0.5.3"}
 sphinx-tabs = {version = ">=1.2.1,<3.5.0"}
-toml = {version = "*"} # Needed by conf.py
+toml = {version = "^0.10.0"} # Needed by conf.py
 
 # Optional testing dependencies
 [tool.poetry.group.tests]
 optional = true
 [tool.poetry.group.tests.dependencies]
 coverage = {version = "^6.4.1"}
 filelock = {version = "^3.8.0"}
@@ -75,14 +79,15 @@
 pytest-cov = {version = "^3.0.0"}
 pytest-dependency = {version = "^0.5.1"}
 pytest-flakes = {version = "^4.0.5"}
 pytest-pep8 = {version = "*"}
 pytest-pythonpath = {version = "*"}
 pytest-xdist = {version = "^3.0.2"}
 pytest-mock = {version = "*"}
+tox = {version = "^4.4.0"}
 
 # Optional build requirements
 [tool.poetry.group.build]
 optional = true
 [tool.poetry.group.build.dependencies]
 build = {version = "^0.8.0"}
 twine = {version = "^4.0.1"}
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """
 A Python script to automate the setup of the ecosystem of a Python project.
 
 Usage
 -----
 
@@ -25,15 +25,15 @@
 testing, ``style`` for code linting, and ``build`` for build. For example:
     ``python setup_environment.py -d run`` installs production dependencies
     ``python setup_environment.py -d doc`` installs doc dependencies
     ``python setup_environment.py -d tests`` installs tests dependencies
     ``python setup_environment.py -d style`` installs style dependencies
     ``python setup_environment.py -d build`` installs build dependencies
 
-It is also possible to cummulate several groups:
+It is also possible to combine several groups:
     ``python setup_environment.py -d run doc tests``
 
 Extra dependency groups refer to any group declared in the configuration file of the dependency management system which
 are not part of doc, tests, style and build. To install these groups use the ``x`` option:
     ``python setup_environment.py -x <name-of-the-group>``
 
 Currently, this code only supports:
@@ -53,14 +53,19 @@
 │  ├── requirements_tests.txt       # Requirements file associated to the tests group.
 │  ├── requirements_style.txt       # Requirements file associated to the style group.
 │  └── requirements_build.txt       # Requirements file associated to the build group.
 
 The following project structure is expected for projects with a dependency management system:
 project-name
 └── pyproject.toml                  # Configuration of the build system.
+
+The following lines should be present in the ``pyproject.toml`` file for managing the version of the dependency management system:
+Example for using poetry 1.4.0:
+[build-system-requirements]
+build-system-version = "1.4.0"
 """
 
 # ==================================================== [Imports] ==================================================== #
 
 import argparse
 import os
 from pathlib import Path
@@ -79,49 +84,53 @@
 
 supported_dependency_management_systems = {
     "poetry": {
         "configuration_file": "pyproject.toml",
         "build_backend": "poetry.core.masonry.api",
         "required_venv_name": ".venv",
         "lock_file": "poetry.lock",
+        "cache_folder": ".poetry\.cache",
+        "build_system_venv": ".poetry\.venv",
     },
     "flit": {
         "configuration_file": "pyproject.toml",
         "build_backend": "flit_core.buildapi",
         "required_venv_name": None,
         "lock_file": None,
+        "cache_folder": ".flit/.cache",
+        "build_system_venv": ".flit/.venv",
     },
 }
 
-standard_optional_dependency_groups = ["doc", "tests", "build", "style"]
+standard_optional_dependency_groups = ["doc", "tests", "build", "style", "external"]
 
 # =================================================== [Functions] =================================================== #
 
 # Console prints ----------------------------------------------------------------------------------------------------
 
 
-def print_main_header(text, max_lenght=100):
+def print_main_header(text, max_length=100):
     """Display main header."""
 
-    for i in range(max_lenght):
+    for i in range(max_length):
         print("=", end="")
     print()
     print(text)
-    for i in range(max_lenght):
+    for i in range(max_length):
         print("=", end="")
     print()
     print()
 
 
-def print_section_header(text, max_lenght=100):
+def print_section_header(text, max_length=100):
     """Display a section header in the console."""
     section_header = ""
-    if len(text) < max_lenght:
+    if len(text) < max_length:
         section_header = text + " "
-        for i in range(len(text), max_lenght):
+        for i in range(len(text), max_length):
             section_header += "-"
     else:
         section_header = text
     print(section_header)
     print()
 
 
@@ -136,18 +145,18 @@
         text = input + " " + separator + " " + value
     print(text)
 
 
 def print_inputs_summary(args):
     """Display a summary of the inputs."""
 
-    print("OS                                   : %s" % (platform.system()))
-    print("Python version                       : %s" % (get_python_version()))
-    print("Virtual environment name             : %s" % (args.venv_name))
-    print("run dependencies                     : %s" % ("yes" if "run" in args.dependencies else "no"))
+    print(f"OS                                   : {platform.system()}")
+    print(f"Python version                       : {get_python_version()}")
+    print(f"Virtual environment name             : {args.venv_name}")
+    print(f"run dependencies                     : {'yes' if 'run' in args.dependencies else 'no'}")
     for dependency_group in standard_optional_dependency_groups:
         print_input_value(
             f"{dependency_group} dependencies",
             "yes" if dependency_group in args.dependencies else "no",
             separator=":",
             separator_position=37,
         )
@@ -155,18 +164,18 @@
         for dependency_group in args.extra_dependencies:
             print_input_value(
                 f"{dependency_group} dependencies",
                 "yes",
                 separator=":",
                 separator_position=37,
             )
-    print("Dependency management system         : %s" % (args.build_system))
-    print("Dependency management system version : %s" % (args.build_system_version))
-    print("Credentials management               : %s" % (args.credentials_management_method))
-    print("")
+    print(f"Dependency management system         : {args.build_system}")
+    print(f"Dependency management system version : {args.build_system_version}")
+    print(f"Credentials management               : {args.credentials_management_method}")
+    print()
 
 
 # Checks ------------------------------------------------------------------------------------------------------------
 
 
 def check_dependency_management_system():
     """Check if a dependency management system is available at project root."""
@@ -184,31 +193,32 @@
     """Check if the virtual environment name is consistent with the build system expectations."""
     if args.build_system:
         if supported_dependency_management_systems[args.build_system]["required_venv_name"]:
             if supported_dependency_management_systems[args.build_system]["required_venv_name"] != args.venv_name:
                 old_name = args.venv_name
                 args.venv_name = supported_dependency_management_systems[args.build_system]["required_venv_name"]
                 print(
-                    f"Warning: {args.build_system} expects the name of the virtual environment name to be "
-                    f"{args.venv_name}. {old_name} is replaced by {args.venv_name}."
+                    f"Warning: {args.build_system} expects the name of the virtual environment name to be {args.venv_name}."
+                    f"{old_name} is replaced by {args.venv_name}."
                 )
 
 
 def check_python_version(args):
     """
     Check if the version of the current Python interpreter is consistent with the python version specifications
     from the build system.
     """
     if args.build_system:
         # Initialize lower/upper versions
-        lower_version, upper_version, lower_sign, upper_sign = None, None, None, None
+        lower_version, upper_version, lower_bound_symbol, upper_bound_symbol = None, None, None, None
         lower_specification, upper_specification, single_specification = None, None, None
         # Read TOML
         configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
         # Read Python version constraint
+        python_compatibility = ""
         if args.build_system == "poetry":
             python_compatibility = configuration["tool"][args.build_system]["dependencies"]["python"].replace(" ", "")
         elif args.build_system == "flit":
             python_compatibility = configuration["project"]["requires-python"].replace(" ", "")
         # Split lower/upper version constraint
         if "," in python_compatibility:
             lower_specification, upper_specification = (
@@ -221,40 +231,39 @@
             elif python_compatibility.startswith("<"):
                 lower_specification, upper_specification = None, python_compatibility
             else:
                 single_specification = python_compatibility
         # Process lower constraint
         if lower_specification:
             lower_version = get_version_from_python_specification(lower_specification)
-            lower_sign = get_sign_from_python_specification(lower_specification)
-            marker = Marker(f"python_full_version {lower_sign} '{lower_version}'")
+            lower_bound_symbol = get_sign_from_python_specification(lower_specification)
+            marker = Marker(f"python_full_version {lower_bound_symbol} '{lower_version}'")
             if not marker.evaluate():
-                raise Exception(f"Python version must be greater than or equal to {lower_version}.")
+                raise Exception(f"Python version must be {lower_bound_symbol} {lower_version}.")
         # Process upper constraint
         if upper_specification:
             upper_version = get_version_from_python_specification(upper_specification)
-            upper_sign = get_sign_from_python_specification(upper_specification)
-            marker = Marker(f"python_full_version {upper_sign} '{upper_version}'")
+            upper_bound_symbol = get_sign_from_python_specification(upper_specification)
+            marker = Marker(f"python_full_version {upper_bound_symbol} '{upper_version}'")
             if not marker.evaluate():
-                raise Exception(f"Python version must be lower than or equal to {upper_version}.")
+                raise Exception(f"Python version must be {upper_bound_symbol} {upper_version}.")
         # Process single
         if single_specification:
             version = get_version_from_python_specification(single_specification)
             sign = get_sign_from_python_specification(single_specification)
             if sign != "==":
                 raise Exception("Unable to interpret python version specification.")
             marker = Marker(f"python_full_version {sign} '{version}'")
             if not marker.evaluate():
                 raise Exception(f"Python version must be equal to {version}.")
 
 
 def check_existing_install(args):
     """Check if an install exists already."""
-    if os.path.isdir(args.venv_name):
-        return True
+    return os.path.isdir(args.venv_name)
 
 
 def check_inputs(args):
     """Check inputs consistency."""
     # Check platform
     if sys.platform != "win32":
         raise Exception("Only Windows operating systems are supported.")
@@ -279,15 +288,15 @@
 
 def read_integers_from_string(string):
     """
     Scan a string and extract integers.
 
     The regex matches any digit character (0-9).
     """
-    return re.findall("\d+", string)
+    return re.findall(r"\d+", string)
 
 
 def remove_scheme_from_url(url):
     """Remove the scheme part of a URL."""
     items = url.split("://")
     if len(items) == 2:
         return items[0], items[1]
@@ -301,15 +310,15 @@
 
 
 def get_python_package(
     package_name: str,
     package_version: str = "*",
     method: str = "install",
     pypi_url: str = "https://pypi.org/simple",
-    private_pypi_token_name: str = None,
+    private_pypi_token_name: str = "",
     no_deps: bool = False,
     python_executable: str = sys.executable,
     verbose: bool = True,
 ) -> None:
     """
     Install or download a python package using PIP.
 
@@ -340,18 +349,17 @@
         command += f"=={package_version}"
     # Add part related to private PyPI source
     if pypi_url != "https://pypi.org/simple":
         # Check if token is available
         if private_pypi_token_name is None:
             raise Exception(f"No token specified for private PyPI server {pypi_url}.")
         # Check if the environment variable associated to the private PyPI token exists
-        if os.environ.get(private_pypi_token_name) is None:
-            raise Exception("Environment variable {private_pypi_token_name} does not exist.")
-        # Get private PyPI token
-        private_pypi_token = os.environ[private_pypi_token_name]
+        private_pypi_token = os.getenv(private_pypi_token_name)
+        if private_pypi_token is None:
+            raise Exception(f"Environment variable {private_pypi_token_name} does not exist.")
         # Split absolute URL
         url_scheme, relative_url = remove_scheme_from_url(pypi_url)
         # Update command line
         command += f" -i {url_scheme}://PAT:{private_pypi_token}@{relative_url}"
     # Add no-deps option
     if no_deps:
         command += " --no-deps"
@@ -365,18 +373,19 @@
 def run_command(cmd, display_output=True):
     """
     Run command.
     """
     process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     if display_output:
         stdout, stderr = b"", b""
-        for line in process.stdout:
-            sys.stdout.buffer.write(line)
-            sys.stdout.buffer.flush()
-            stdout += line
+        if process.stdout is not None:
+            for line in process.stdout:
+                sys.stdout.buffer.write(line)
+                sys.stdout.buffer.flush()
+                stdout += line
         process.wait()
     else:
         stdout, stderr = process.communicate()
 
     if isinstance(stdout, bytes):
         try:
             stdout = stdout.decode().splitlines()
@@ -389,30 +398,30 @@
         except:
             raise Exception("Unable to decode stderr.")
 
     return process.returncode, stdout, stderr
 
 
 def upgrade_pip(python_executable: str = sys.executable) -> None:
-    """Upgrade to latest PIP version"""
+    """Upgrade to latest PIP version in the virtual environment"""
     print("Upgrade to latest pip version")
     subprocess.run(
         [python_executable, "-m", "pip", "install", "--upgrade", "pip"],
         check=True,
         shell=True,
     )
     print()
 
 
-def create_virtual_environment(args):
+def create_virtual_environment(args, venv: str = ".venv"):
     """Create a virtual environment."""
 
     print("Create virtual environment")
-    if not args.has_install or args.force_clear:
-        subprocess.run([sys.executable, "-m", "venv", ".venv"])
+    if not args.has_install or args.force_clear or args.force_clear_all:
+        subprocess.run([sys.executable, "-m", "venv", venv], check=True, shell=True)
     else:
         print("Skipped")
     print()
 
 
 # Dependency Management System (Build System) -----------------------------------------------------------------------
 
@@ -439,75 +448,127 @@
     if sign == "":
         sign = "=="
     return sign
 
 
 def install_build_system(args):
     """Install build system."""
-    print(f"Install dependency management system.")
+    print("Install dependency management system.")
     if args.build_system:
-        if not args.has_install or args.force_clear:
-            get_python_package(
-                args.build_system,
-                args.build_system_version,
-                method="install",
-                python_executable=rf".\{args.venv_name}\Scripts\python",
-                verbose=args.verbose,
-            )
+        if not args.has_install or args.force_clear or args.force_clear_all:
+            configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
+            if (
+                args.build_system_version == "*"
+                and "build-system-version" in configuration["build-system-requirements"]
+            ):
+                args.build_system_version = configuration["build-system-requirements"]["build-system-version"]
+            if args.build_system == "poetry":
+                create_virtual_environment(
+                    args, venv=supported_dependency_management_systems[args.build_system]["build_system_venv"]
+                )
+                upgrade_pip(
+                    python_executable=rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python"
+                )
+                get_python_package(
+                    args.build_system,
+                    args.build_system_version,
+                    method="install",
+                    python_executable=rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python",
+                    verbose=args.verbose,
+                )
+            else:
+                get_python_package(
+                    args.build_system,
+                    args.build_system_version,
+                    method="install",
+                    python_executable=rf".\{args.venv_name}\Scripts\python",
+                    verbose=args.verbose,
+                )
             print()
+            # Create a file symbolic link from the virtual environment (.venv) that the build system (poetry) manages
+            # to the build system executable (poetry.exe) in the poetry virtual environment (.poetry/.venv).  This
+            # ensures that the correct poetry is accessible when the managed virtual environment is activated
+            build_system_executable = rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\{args.build_system}.exe"
+            if os.path.exists(build_system_executable):
+                subprocess.run(
+                    [
+                        "powershell",
+                        "-Command",
+                        "New-Item",
+                        "-ItemType",
+                        "SymbolicLink",
+                        "-Path",
+                        rf".\{args.venv_name}\Scripts\{args.build_system}.exe",
+                        "-Target",
+                        build_system_executable,
+                    ]
+                )
             return
     print("Skipped")
     print()
 
 
 def configure_build_system(args):
     """Configure the build system to enable connection to private sources."""
-    print(f"Configure dependency management system.")
+    print("Configure dependency management system.")
     if args.build_system:
-        if not args.has_install or args.force_clear:
+        if not args.has_install or args.force_clear or args.force_clear_all:
             if args.build_system == "poetry":
-                configure_poetry(args.venv_name, args.credentials_management_method)
+                configure_poetry(
+                    supported_dependency_management_systems[args.build_system]["build_system_venv"],
+                    args.credentials_management_method,
+                )
                 print()
             return
     print("Skipped")
     print()
 
 
 def configure_poetry(venv_name, credentials_management_method):
     """Configure Poetry."""
-    # Turn-on in-project
-    subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.in-project", "true"])
     # Get list of private sources
     private_sources = get_private_sources("pyproject.toml")
     # Delete existing configuration
     print("Clean-up existing poetry configurations")
     if sys.platform == "win32":
         username = os.getlogin()
-        path_poetry_config = r"C:\Users\%s\AppData\Roaming\pypoetry" % (username)
+        path_poetry_config = rf"C:\Users\{username}\AppData\Roaming\pypoetry"
         if os.path.isfile(os.path.join(path_poetry_config, "config.toml")):
             os.remove(os.path.join(path_poetry_config, "config.toml"))
         if os.path.isfile(os.path.join(path_poetry_config, "auth.toml")):
             os.remove(os.path.join(path_poetry_config, "auth.toml"))
+    # Turn-on in-project
+    subprocess.run([rf".\{venv_name}\Scripts\poetry", "config", "virtualenvs.in-project", "true"], check=True)
+    # Turn-on poetry cache
+    subprocess.run(
+        [
+            rf".\{venv_name}\Scripts\poetry",
+            "config",
+            "cache-dir",
+            supported_dependency_management_systems["poetry"]["cache_folder"],
+        ],
+        check=True,
+    )
     # Declare credentials for private sources
     for source in private_sources:
-        print("Declare credentials for %s" % (source["name"]))
+        print(f"Declare credentials for {source['name']}")
         # Get source PAT
         if source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/pyansys/pypi/simple/":
             token = os.environ["PYANSYS_PRIVATE_PYPI_PAT"]
         elif source["url"] == "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple/":
             token = os.environ["SOLUTIONS_PRIVATE_PYPI_PAT"]
         else:
-            raise Exception("Unknown private source %s with url %s." % (source["name"], source["url"]))
+            raise Exception(f"Unknown private source {source['name']} with url {source['url']}.")
         # Store credentials
         if credentials_management_method == "keyring":
             # Declare source URL
-            command_line = "%s/Scripts/poetry config repositories.%s %s" % (venv_name, source["name"], source["url"])
+            command_line = f"{venv_name}/Scripts/poetry config repositories.{source['name']} {source['url']}"
             subprocess.run(command_line, check=True)
             # Declare source credentials
-            command_line = "%s/Scripts/poetry config http-basic.%s PAT %s" % (venv_name, source["name"], token)
+            command_line = f"{venv_name}/Scripts/poetry config http-basic.{source['name']} PAT {token}"
             subprocess.run(command_line, check=True)
         elif credentials_management_method == "environment-variables":
             # Format source name to comply with Poetry environment variable syntax
             source_name = source["name"].upper().replace("-", "_")
             # Create Poetry environment variable
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_USERNAME"] = "PAT"
             os.environ[f"POETRY_HTTP_BASIC_{source_name}_PASSWORD"] = token
@@ -537,15 +598,14 @@
         usage=None,
         prefix_chars="-",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=textwrap.dedent(program_description),
     )
     parser._action_groups.pop()
     # Definition of the group of arguments
-    required_inputs = parser.add_argument_group("Required arguments")
     optional_inputs = parser.add_argument_group("Optional arguments")
     # Optional parameters
     optional_inputs.add_argument(
         "-d",
         "--dependencies",
         type=str,
         nargs="+",
@@ -580,22 +640,29 @@
         choices=["keyring", "environment-variables"],
         required=False,
     )
     optional_inputs.add_argument(
         "-e",
         "--venv-name",
         type=str,
-        help="Name of the virtual environment.",
+        help="Name of the virtual environment. Must be '.venv' when using poetry",
         default=".venv",
         required=False,
     )
     optional_inputs.add_argument(
+        "-F",
+        "--force-clear-all",
+        help="Clean-up the workspace. Delete existing .venv, .poetry\.venv, .poetry\.cache and poetry.lock.",
+        action="store_true",
+        required=False,
+    )
+    optional_inputs.add_argument(
         "-f",
         "--force-clear",
-        help="Clean-up the workspace. Delete existing .venv and poetry.lock.",
+        help="Clean-up the workspace. Delete existing .venv., .poetry\.venv and .poetry\.cache.",
         action="store_true",
         required=False,
     )
     optional_inputs.add_argument(
         "-v",
         "--verbose",
         help="Activate verbose mode.",
@@ -605,75 +672,100 @@
 
     return parser.parse_args()
 
 
 def clear_workspace(args):
     """Remove residual items form previous installation (like venv directory, lock file ...)."""
     print("Clear workspace")
-    if args.force_clear:
+    if args.force_clear or args.force_clear_all:
         # Remove virtual environment
         if os.path.isdir(args.venv_name):
             print(f"Delete existing virtual environment {args.venv_name}.")
             shutil.rmtree(args.venv_name)
-        # Remove lock file
-        if args.build_system:
-            if supported_dependency_management_systems[args.build_system]["lock_file"]:
-                if os.path.isfile(supported_dependency_management_systems[args.build_system]["lock_file"]):
-                    print("Delete existing poetry lock file")
-                    os.remove(supported_dependency_management_systems[args.build_system]["lock_file"])
+        # Remove poetry virtual environment
+        if os.path.isdir(supported_dependency_management_systems[args.build_system]["build_system_venv"]):
+            print("Delete existing poetry virtual environment")
+            shutil.rmtree(supported_dependency_management_systems[args.build_system]["build_system_venv"])
+        # Remove poetry cache
+        if os.path.isdir(supported_dependency_management_systems[args.build_system]["cache_folder"]):
+            print("Delete existing poetry cache")
+            shutil.rmtree(supported_dependency_management_systems[args.build_system]["cache_folder"])
+        if args.force_clear_all:
+            # Remove lock file
+            if args.build_system:
+                if supported_dependency_management_systems[args.build_system]["lock_file"]:
+                    if os.path.isfile(supported_dependency_management_systems[args.build_system]["lock_file"]):
+                        print("Delete existing poetry lock file")
+                        os.remove(supported_dependency_management_systems[args.build_system]["lock_file"])
     else:
         print("Skipped")
-    print("")
+    print()
 
 
 def install_production_dependencies(args):
     """Install the package (mandatory requirements only)."""
-    print(f"Install production dependencies")
+    print("Install production dependencies")
     if args.build_system and "run" in args.dependencies:
         if args.build_system == "poetry":
             subprocess.run(
-                [rf".\{args.venv_name}\Scripts\poetry", "install", "--only", "main", "-vv"], check=True, shell=True
+                [
+                    rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
+                    "install",
+                    "-vv",
+                ],
+                check=True,
+                shell=True,
             )
         elif args.build_system == "flit":
             subprocess.run([rf".\{args.venv_name}\Scripts\flit", "install"], check=True, shell=True)
         print()
         return
     print("Skipped")
     print()
 
 
 def install_optional_dependencies(args):
     """Install optional requirements (doc, tests, build or style)."""
     # Load configuration file if a dependency management system is available
     if args.build_system:
         configuration = toml.load(supported_dependency_management_systems[args.build_system]["configuration_file"])
+    else:
+        configuration = {}
     # Install standard optional dependency groups
     for dependency_group in standard_optional_dependency_groups:
-        print("Install %s dependencies" % (dependency_group))
+        print(f"Install {dependency_group} dependencies")
         if dependency_group in args.dependencies:
             # Install dependency group in the configuration file of the build system
             if args.build_system:
                 has_dependency_group = check_dependency_group(dependency_group, configuration)
                 if has_dependency_group:
                     print("Installing from build system configuration file.")
                     subprocess.run(
-                        [rf".\{args.venv_name}\Scripts\poetry", "install", "--only", dependency_group, "-vv"],
+                        [
+                            rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
+                            "install",
+                            "--only",
+                            dependency_group,
+                            "-vv",
+                        ],
                         check=True,
                         shell=True,
                     )
                     print()
                     continue
             # Alternatively search dependency group in the requirements folder
             requirements_file = os.path.join("requirements", f"requirements_{dependency_group}.txt")
             if os.path.exists(requirements_file):
                 print("Installing from requirements file.")
                 subprocess.run(
                     [
-                        rf".\{args.venv_name}\Scripts\python",
+                        rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\python",
                         "-m",
+                        "poetry",
+                        "run",
                         "pip",
                         "install",
                         "-r",
                         requirements_file,
                         "--no-warn-conflicts",
                     ],
                     check=True,
@@ -682,19 +774,25 @@
                 print()
                 continue
         print("Skipped")
         print()
     # Install extra optional dependency groups
     if args.build_system and args.extra_dependencies:
         for dependency_group in args.extra_dependencies:
-            print("Install %s dependencies" % (dependency_group))
+            print(f"Install {dependency_group} dependencies")
             has_dependency_group = check_dependency_group(dependency_group, configuration)
             if has_dependency_group:
                 subprocess.run(
-                    [rf".\{args.venv_name}\Scripts\poetry", "install", "--only", dependency_group, "-vv"],
+                    [
+                        rf".\{supported_dependency_management_systems[args.build_system]['build_system_venv']}\Scripts\poetry",
+                        "install",
+                        "--only",
+                        dependency_group,
+                        "-vv",
+                    ],
                     check=True,
                     shell=True,
                 )
             else:
                 print(f"No dependency group named {dependency_group}.")
                 print("Skipped")
             print()
@@ -724,37 +822,37 @@
     print_main_header("Setup Environment")
 
     # Display inputs summary
     print_inputs_summary(args)
 
     # Clear workspace -------------------------------------------------------------------------------------------------
 
-    print_section_header("Clear workspace", max_lenght=100)
+    print_section_header("Clear workspace", max_length=100)
 
     clear_workspace(args)
 
     # Setup virtual environment ---------------------------------------------------------------------------------------
 
-    print_section_header("Setup virtual environment", max_lenght=100)
+    print_section_header("Setup virtual environment", max_length=100)
 
     create_virtual_environment(args)
 
     upgrade_pip(python_executable=rf".\{args.venv_name}\Scripts\python")
 
     # Setup dependency management system ------------------------------------------------------------------------------
 
-    print_section_header("Setup dependency management system", max_lenght=100)
+    print_section_header("Setup dependency management system", max_length=100)
 
     install_build_system(args)
 
     configure_build_system(args)
 
     # Install dependencies --------------------------------------------------------------------------------------------
 
-    print_section_header("Install dependencies", max_lenght=100)
+    print_section_header("Install dependencies", max_length=100)
 
     install_production_dependencies(args)
 
     install_optional_dependencies(args)
 
     # Back to current working directory
     os.chdir(working_directory)
@@ -763,16 +861,16 @@
     elapsed_time = (time.time() - time_on) / 60  # in minutes
 
     print("You are all set!")
     print("Navigate to project root and activate your environment with one these commands:")
     print(rf"   - For Windows CMD       : {args.venv_name}\Scripts\activate.bat")
     print(rf"   - For Windows Powershell: {args.venv_name}\Scripts\Activate.ps1")
     print("Enjoy!")
-    print("")
+    print()
     print("Execution time: %.1f minutes." % (elapsed_time))
-    print("")
+    print()
 
 
 # =================================================== [Execution] =================================================== #
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Entry point."""
 
 from ansys.saf.glow.runtime import glow_main
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution import definition
 {% if cookiecutter.with_dash_ui == "yes" %}
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Solution definition module."""
 
 
 from ansys.saf.glow.solution import Solution, StepsModel
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.first_step import FirstStep
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Backend of the first step."""
 
 
 from ansys.saf.glow.solution import StepModel, StepSpec, transaction
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Application."""
 
 import os
 import tempfile
 
 import dash_bootstrap_components as dbc
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the first step."""
 
 
 from ansys.saf.glow.client.dashclient import DashClient
 from dash_extensions.enrich import Input, Output, State, callback, dcc, html
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the first step."""
 
 import base64
 import os
 from pathlib import Path
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Initialization of the frontend layout across all the steps."""
 
 
 from ansys.saf.glow.client.dashclient import DashClient
 from ansys_dash_treeview import AnsysDashTreeview
 import dash_bootstrap_components as dbc
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Frontend of the second step."""
 
 
 from dash_extensions.enrich import dcc, html
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.solution.second_step import SecondStep
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ©2022, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
+# ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 # ==================================================== [Imports] ==================================================== #
 
 from pathlib import Path
 
 # =================================================== [Variables] =================================================== #
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys-templates-0.6.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tox]
 description = Default tox environments list
 envlist =
-    style,{py37,py38}{,-coverage},doc,build
+    style,{py38,py39,py310}{,-coverage},doc,build
 skip_missing_interpreters = true
 isolated_build = true
 
 [gh-actions]
 description = The tox environment to be executed in gh-actions for a given python version
 python =
-    3.7: style,py37-coverage,doc,build
     3.8: style,py38-coverage,doc,build
+    3.9: style,py39-coverage,doc,build
+    3.10: style,py310-coverage,doc,build
 
 [testenv]
 description = Perform functional testing
 basepython =
-    py37: python3.7
     py38: python3.8
+    py39: python3.9
+    py310: python3.10
     py: python3
     {style,reformat,doc,build}: python3
 skip_install = true
 passenv = *
 allowlist_externals = poetry
 commands =
     poetry config virtualenvs.create false
@@ -44,11 +46,11 @@
     poetry install --only doc -vv
     poetry run sphinx-build doc/source doc/build/html --color -vW -bhtml
 
 [testenv:build]
 description = Check source code build
 skip_install = true
 commands =
-    poetry config virtualenvs.create false 
+    poetry config virtualenvs.create false
     poetry install --only build -vv
     poetry run python -m build
```

### Comparing `ansys-templates-0.5.2/src/ansys/templates/testing.py` & `ansys-templates-0.6.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/src/ansys/templates/utils.py` & `ansys-templates-0.6.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.5.2/PKG-INFO` & `ansys-templates-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 0.5.2
+Version: 0.6.0
 Summary: Creates Python projects according to PyAnsys guidelines
-Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
+Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: click>=7.0,<8.0.0
 Requires-Dist: cookiecutter>=2.1.0
 Requires-Dist: isort>=5.10.1
-Requires-Dist: ansys-sphinx-theme==0.8.2 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: pytest==7.2.1 ; extra == "tests"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Project-URL: Documentation, https://templates.ansys.com/
 Project-URL: Homepage, https://templates.ansys.com/
 Project-URL: Source, https://github.com/ansys-templates/ansys-templates
 Project-URL: Tracker, https://github.com/ansys/ansys-templates/issues
 Provides-Extra: doc
 Provides-Extra: tests
@@ -48,20 +50,20 @@
 .. IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 .. FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 .. AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 .. LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 .. OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 .. SOFTWARE.
 
-Welcome to Ansys templates
-==========================
-|pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
+Ansys templates
+===============
+|ansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
+.. |ansys| image:: https://img.shields.io/badge/Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://github.com/ansys
    :alt: PyAnsys
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/ansys-templates?logo=pypi
    :target: https://pypi.org/project/ansys-templates/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-templates.svg?logo=python&logoColor=white
@@ -80,14 +82,16 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
+.. |implemented| image:: <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path d="M21.03 5.72a.75.75 0 0 1 0 1.06l-11.5 11.5a.747.747 0 0 1-1.072-.012l-5.5-5.75a.75.75 0 1 1 1.084-1.036l4.97 5.195L19.97 5.72a.75.75 0 0 1 1.06 0Z"></path></svg>
+
 
 The ``ansys-templates`` repository holds a collection of useful templates compliant
 with PyAnsys guidelines. It also provides the ``ansys-templates`` command line tool
 for interactively generating new projects based on previous templates.
 
 The main advantages of using this tool are:
 
@@ -105,15 +109,15 @@
 
 
 How to install
 --------------
 Users can install ``ansys-templates`` by running:
 
 .. code-block:: text
-        
+
     python -m pip install ansys-templates
 
 The usage of `pipx`_ is encouraged too. See `installing ansys-templates using
 pipx`_.
 
 .. _pipx: https://pypa.github.io/pipx/
 .. _installing ansys-templates using pipx: https://templates.pyansys.com/getting_started/index.html#installing-pipx
```

