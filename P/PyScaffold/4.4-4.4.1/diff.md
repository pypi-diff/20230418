# Comparing `tmp/PyScaffold-4.4.tar.gz` & `tmp/PyScaffold-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyscaffold/pyscaffold/dist/.tmp-zx5wiua5/PyScaffold-4.4.tar", last modified: Mon Jan 23 12:13:26 2023, max compression
+gzip compressed data, was "/home/runner/work/pyscaffold/pyscaffold/dist/.tmp-9k67q_dv/PyScaffold-4.4.1.tar", last modified: Tue Apr 18 16:08:44 2023, max compression
```

## Comparing `PyScaffold-4.4.tar` & `PyScaffold-4.4.1.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-01-23 12:13:10.000000 PyScaffold-4.4/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-23 12:13:10.000000 PyScaffold-4.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/workflows/make-demo-repo.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-23 12:13:10.000000 PyScaffold-4.4/.github/workflows/publish-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-23 12:13:10.000000 PyScaffold-4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-23 12:13:10.000000 PyScaffold-4.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-01-23 12:13:10.000000 PyScaffold-4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-23 12:13:10.000000 PyScaffold-4.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-23 12:13:10.000000 PyScaffold-4.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23121 2023-01-23 12:13:10.000000 PyScaffold-4.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-01-23 12:13:10.000000 PyScaffold-4.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-01-23 12:13:10.000000 PyScaffold-4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-01-23 12:13:26.000000 PyScaffold-4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-01-23 12:13:10.000000 PyScaffold-4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/source/options
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-23 12:13:10.000000 PyScaffold-4.4/debian/watch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/_static/pyscaffold-custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/action-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/dev-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/example_setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/cirrus-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/gitlab-ci-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/namespace-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/no-skeleton-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/no-tox-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/examples/pre-commit-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26731 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21513 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/docs/gfx/
--rwxr-xr-x   0 runner    (1001) docker     (123)   159443 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/action-pipeline-paths.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    36777 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/action-pipeline.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)   165295 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/api-paths.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    34942 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/api.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)   134198 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/demo.cast
--rwxr-xr-x   0 runner    (1001) docker     (123)  4772106 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   115081 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71500 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/github_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/sidebar.png
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/gfx/simple-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/reasons.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/updating.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-01-23 12:13:10.000000 PyScaffold-4.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-23 12:13:10.000000 PyScaffold-4.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-23 12:13:10.000000 PyScaffold-4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-01-23 12:13:26.000000 PyScaffold-4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-23 12:13:10.000000 PyScaffold-4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 12:13:25.000000 PyScaffold-4.4/src/PyScaffold.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/PyScaffold.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/pyscaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/pyscaffold/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/cirrus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/no_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/no_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/no_tox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/extensions/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/src/pyscaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/__init__.template
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/authors.template
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/changelog.template
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/cirrus.template
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/conftest_py.template
--rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/contributing.template
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/coveragerc.template
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/github_ci_workflow.template
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/gitignore_empty.template
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/gitlab_ci.template
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/header_interactive.template
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/isort_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_affero_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_apache.template
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_artistic_2.0.template
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_bsd0.template
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_cc0_1.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_eclipse_1.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_gpl_2.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_gpl_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_isc.template
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_lgpl_2.1.template
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_lgpl_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_mit.template
--rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_mozilla.template
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_new_bsd.template
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_none.template
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_public_domain.template
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/license_simplified_bsd.template
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/pre-commit-config.template
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/pyproject_toml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/readme.template
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/rtd_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/rtd_requirements.template
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/setup_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/setup_py.template
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/skeleton.template
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_authors.template
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_changelog.template
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_conf.template
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_contributing.template
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_index.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_license.template
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_makefile.template
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/sphinx_readme.template
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/test_skeleton.template
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/templates/tox_ini.template
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-01-23 12:13:10.000000 PyScaffold-4.4/src/pyscaffold/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/demoapp/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/demoapp_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/demoapp_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp_data/data/hello_world.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp_data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp_data/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp_data/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/demoapp_data/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/examples/issue-506/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/examples/issue-506/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/incompatible_v3_api_fake_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_cirrus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_interactive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8481 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_no_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_no_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_no_tox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/extensions/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/log_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:26.000000 PyScaffold-4.4/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/system/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/system/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/system/test_dependency_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_termui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-01-23 12:13:10.000000 PyScaffold-4.4/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-01-23 12:13:10.000000 PyScaffold-4.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/make-demo-repo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/publish-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/source/options
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/watch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/_static/pyscaffold-custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/action-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/example_setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/cirrus-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/gitlab-ci-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/namespace-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/no-skeleton-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/no-tox-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/pre-commit-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/gfx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159443 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/action-pipeline-paths.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36777 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/action-pipeline.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165295 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/api-paths.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34942 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/api.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   134198 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/demo.cast
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4772106 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   115081 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71500 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/github_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/simple-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/reasons.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/updating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:43.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/cirrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_tox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/__init__.template
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/authors.template
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/changelog.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/cirrus.template
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/conftest_py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/contributing.template
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/coveragerc.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/github_ci_workflow.template
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitignore_empty.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitlab_ci.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/header_interactive.template
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/isort_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_affero_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_apache.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_artistic_2.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_bsd0.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_cc0_1.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_eclipse_1.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_2.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_isc.template
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_2.1.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_mit.template
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_mozilla.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_new_bsd.template
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_none.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_public_domain.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_simplified_bsd.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/pre-commit-config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/pyproject_toml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/rtd_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/rtd_requirements.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/setup_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/setup_py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/skeleton.template
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_authors.template
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_changelog.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_contributing.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_index.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_license.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_makefile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/test_skeleton.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/tox_ini.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/data/hello_world.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/examples/issue-506/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/examples/issue-506/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/incompatible_v3_api_fake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_cirrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_interactive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8481 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_tox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/log_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/test_dependency_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tox.ini
```

### Comparing `PyScaffold-4.4/.cirrus.yml` & `PyScaffold-4.4.1/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.coveragerc` & `PyScaffold-4.4.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.github/FUNDING.yml` & `PyScaffold-4.4.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.github/workflows/codeql-analysis.yml` & `PyScaffold-4.4.1/.github/workflows/codeql-analysis.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     branches: [ master ]
   pull_request:
     # The branches below must be a subset of the branches above
     branches: [ master ]
   schedule:
     - cron: '40 1 * * 2'
 
+permissions:
+  security-events: write
+  contents: read
+
 jobs:
   analyze:
     name: Analyze
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
```

### Comparing `PyScaffold-4.4/.github/workflows/make-demo-repo.yml` & `PyScaffold-4.4.1/.github/workflows/make-demo-repo.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.github/workflows/publish-package.yml` & `PyScaffold-4.4.1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.gitignore` & `PyScaffold-4.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/.pre-commit-config.yaml` & `PyScaffold-4.4.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -20,43 +20,43 @@
 - repo: https://github.com/asottile/pyupgrade
   rev: v3.3.1
   hooks:
   - id: pyupgrade
     args: ['--py36-plus']
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.0
+  rev: v2.1.0
   hooks:
   - id: autoflake
     args: [
       --in-place,
       --remove-all-unused-imports,
       --remove-unused-variables,
     ]
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.11.4
+  rev: 5.11.5
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.13.0
   hooks:
   - id: blacken-docs
     additional_dependencies: [black]
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
+  rev: 5.0.4
   hooks:
   - id: flake8
     additional_dependencies: [flake8-bugbear!=23.1.14]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.2
+  rev: v2.2.4
   hooks:
   - id: codespell
```

### Comparing `PyScaffold-4.4/.readthedocs.yml` & `PyScaffold-4.4.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/CHANGELOG.rst` & `PyScaffold-4.4.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,37 @@
     Version 4.X.X, 2023-XX-XX
     -------------------------
 
 
 Current versions
 ================
 
-Version 4.4, 2023-01-23
------------------------
+Version 4.4.1, 2023-04-18
+-------------------------
 
-- Add ``codespell`` to ``pre-commit`` config, #674
-- Allow ``venv_install`` in config file, #680
-- Avoid problematic ``tox`` 4.0 and 4.1, #689
-- Update ``macos`` instances on Cirrus CI, #690
-- Replace deprecated ``set-output``, #688
-- Update CI templates, #693
-- Add comments about  building ``sdist`` in ``tox.ini`` and FAQ, #694
-- Update Python version in Read The Docs configuration, #695
+- Re-use pre-built wheels in CI for upgrade tests in :pr:`702`
+- Make security permissions explicit in GHA template :pr:`704`
+- Fix ``GITHUB_TOKEN`` variable in GHA template :pr:`715`
 
 
 Older versions
 ==============
 
+Version 4.4, 2023-01-23
+-----------------------
+
+- Add ``codespell`` to ``pre-commit`` config, :pr:`674`
+- Allow ``venv_install`` in config file, :pr:`680`
+- Avoid problematic ``tox`` 4.0 and 4.1, :pr:`689`
+- Update ``macos`` instances on Cirrus CI, :pr:`690`
+- Replace deprecated ``set-output``, :pr:`688`
+- Update CI templates, :pr:`693`
+- Add comments about  building ``sdist`` in ``tox.ini`` and FAQ, :pr:`694`
+- Update Python version in Read The Docs configuration, :pr:`695`
+
 Version 4.3.1, 2022-09-20
 -------------------------
 
 - Modify ``tox.ini`` template to allow passing the ``TWINE_REPOSITORY_URL``
   environment variable, :pr:`666`.
 
 Version 4.3, 2022-07-20
```

### Comparing `PyScaffold-4.4/CONTRIBUTING.rst` & `PyScaffold-4.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/LICENSE.txt` & `PyScaffold-4.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/PKG-INFO` & `PyScaffold-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScaffold
-Version: 4.4
+Version: 4.4.1
 Summary: Template tool for putting up the scaffold of a Python project
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Florian Wilhelm
 Author-email: Florian.Wilhelm@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/pyscaffold/pyscaffold/
```

### Comparing `PyScaffold-4.4/README.rst` & `PyScaffold-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/Makefile` & `PyScaffold-4.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/_static/pyscaffold-custom.css` & `PyScaffold-4.4.1/docs/_static/pyscaffold-custom.css`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/action-pipeline.rst` & `PyScaffold-4.4.1/docs/action-pipeline.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/conf.py` & `PyScaffold-4.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/dependencies.rst` & `PyScaffold-4.4.1/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/dev-guide.rst` & `PyScaffold-4.4.1/docs/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/example_setup.cfg` & `PyScaffold-4.4.1/docs/example_setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/extensions.rst` & `PyScaffold-4.4.1/docs/extensions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -434,15 +434,16 @@
 
 Conventions for Community Extensions
 ====================================
 
 In order to make it easy to find PyScaffold extensions, community packages
 should be namespaced as in ``pyscaffoldext.${EXT_NAME}`` (where ``${EXT_NAME}``
 is the name of the extension being developed). Although this naming convention
-slightly differs from `PEP423`_, it is close enough and shorter.
+slightly differs from :pep:`423 <423#use-standard-pattern-for-community-contributions>`,
+it is close enough and shorter.
 
 Similarly to ``sphinxcontrib-*`` packages, names registered in PyPI should
 contain a dash ``-``, instead of a dot ``.``. This way, third-party extension
 development can be easily bootstrapped with the command::
 
     putup pyscaffoldext-${EXT_NAME} -p ${EXT_NAME} --namespace pyscaffoldext --no-skeleton
 
@@ -502,15 +503,14 @@
 
        # No:
        import ${package}
        from ${package} import module
        from ${package}.module import function
 
 
-.. _PEP423: https://www.python.org/dev/peps/pep-0423/#use-standard-pattern-for-community-contributions
 .. _setuptools entry point: https://setuptools.pypa.io/en/stable/userguide/entry_point.html
 .. _custom_extension: https://github.com/pyscaffold/pyscaffoldext-custom-extension
 .. _Cookiecutter templates: https://github.com/pyscaffold/pyscaffoldext-cookiecutter
 .. _pyscaffoldext-cookiecutter: https://github.com/pyscaffold/pyscaffoldext-cookiecutter
 .. _Python decorators: https://en.wikipedia.org/wiki/Python_syntax_and_semantics#Decorators
 .. _semantic versioning: https://semver.org
 .. _pull request: https://github.com/pyscaffold/pyscaffold/pulls
```

### Comparing `PyScaffold-4.4/docs/faq.rst` & `PyScaffold-4.4.1/docs/faq.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    Starting from version 4, your package is completely independent from PyScaffold, we just kick-start your project and
    take care of the boilerplate.
    However, we do include some build-time dependencies that make your life easier, such as :pypi:`setuptools-scm`.
    But don't worry, if you distribute your project in the recommended `wheel format`_ those dependencies will not affect
    the final users, they are just required during development to assembling the package file.
 
    That means if someone clones your repository and tries to build it, the dependencies in ``pyproject.toml``
-   will be automatically pulled. This mechanism is described by `PEP 517`_/`PEP 518`_ and definitely beyond the scope of this answer.
+   will be automatically pulled. This mechanism is described by :pep:`517`/:pep:`518` and definitely beyond the scope of this answer.
 
 Can I use PyScaffold ≥ 3 to develop a Python package that is Python 2 & 3 compatible?
    Python 2 reached *end-of-life* in 2020, which means that no security updates will be available, and therefore any
    software running on Python 2 is potentially vulnerable. PyScaffold strongly recommends all packages to be ported to
    the latest supported version of Python.
 
    That being said, Python 3 is actually only needed for the ``putup`` command and whenever you use ``setup.py``. This means that with
@@ -62,15 +62,15 @@
 
 Why would I use PyScaffold instead of Cookiecutter?
    PyScaffold is focused on a good out-of-the-box experience for developing distributable Python packages (exclusively).
    The idea is to standardize the structure of Python packages. Thus, PyScaffold sticks to
 
        "There should be one-- and preferably only one --obvious way to do it."
 
-   from the `Zen of Python`_. The long-term goal is that PyScaffold becomes for Python what `Cargo`_ is for `Rust`_.
+   from the :pep:`Zen of Python <20>`. The long-term goal is that PyScaffold becomes for Python what `Cargo`_ is for `Rust`_.
    Still, with the help of PyScaffold's :ref:`extension system <extensions>` customizing a project scaffold is possible.
 
    Cookiecutter on the other hand is a really flexible templating tool that allows you to define own templates according
    to your needs. Although some standard templates are provided that will give you quite similar results as PyScaffold,
    the overall goal of the project is quite different.
 
    Still, if you so desire, PyScaffold allows users to augment PyScaffold projects with certain types of cookiecutter
@@ -200,15 +200,15 @@
    A nice `blog post by Ionel`_ gives a thorough explanation why this is so. In a nutshell, the most severe
    problem comes from the fact that Python imports a package by first looking at the current working directory and then
    into the ``PYTHONPATH`` environment variable. If your current working directory is the root of your project directory
    you are thus not testing the installation of your package but the local package directly. Eventually, this always
    leads to huge confusion (*"But the unit tests ran perfectly on my machine!"*).
 
    Moreover, having a dedicated ``src`` directory to store the package files, makes it easy to comply with recent standards
-   in the Python community (for example `PEP 420`_).
+   in the Python community (for example :pep:`420`).
 
    Please notice that PyScaffold assumes all the files inside ``src`` are meant to be part of the package.
 
 Can I have other files inside the ``src`` folder that are not meant for distribution?
    PyScaffold considers the ``src`` directory to be exclusively dedicated to
    store files meant to be distributed, and relies on this assumption to
    generate configuration for the several aspects of your project. Therefore
@@ -224,16 +224,16 @@
 
 
 Namespaces
 ----------
 
 .. _remove_implicit_namespaces:
 
-How can I get rid of the implicit namespaces (`PEP 420`_)?
-    PyScaffold uses ``setup.cfg`` to ensure `setuptools`_ will follow `PEP 420`_.
+How can I get rid of the implicit namespaces (:pep:`420`)?
+    PyScaffold uses ``setup.cfg`` to ensure `setuptools`_ will follow :pep:`420`.
     If this configuration particularly messes up with your package, or
     you simply want to follow the old behavior, please replace
     ``packages = find_namespace:`` with ``packages = find:`` in the ``[options]``
     section of that file.
 
     You should also remove the ``--implicit-namespaces`` option in the
     ``cmd_line_template`` variable in the ``docs/conf.py`` file.
@@ -243,28 +243,28 @@
     official guide`_.  If there are already other projects with packages
     registered in the same namespace, chances are you just need to copy from
     them a sample of the ``__init__.py`` file for the umbrella folder working as
     namespace.
 
 How can I fix problems with my namespace package after an upgrade to PyScaffold 4?
     That is likely to be happening because PyScaffold 4 removed support for
-    `pkg_resources`_ namespaces in favour of `PEP 420`_. Unfortunately these two
+    `pkg_resources`_ namespaces in favour of :pep:`420`. Unfortunately these two
     methodologies for creating namespaces are not compatible, as documented in
     the `packaging namespace packages official guide`_. To fix this problem you
     (or other maintainers) will need to either **(a)** update all the existing
-    "subpackages" in the same namespace to be implicit (`PEP 420`_-style), or
+    "subpackages" in the same namespace to be implicit (:pep:`420`-style), or
     **(b)** get rid of the implicit namespace configuration PyScaffold
     automatically sets up during project creation/update. Please check the
     answers for these other questions about :ref:`removing <remove_implicit_namespaces>`
     or :ref:`adding <add_implicit_namespaces>` implicit namespaces and the
     :ref:`updating <updating>` guides for some tips on how to achieve that.
 
 .. _add_implicit_namespaces:
 
-How can I convert an existing package to use implicit namespaces (`PEP 420`_)?
+How can I convert an existing package to use implicit namespaces (:pep:`420`])?
     The easiest answer for that question is to **(a)** convert the existing
     package to a PyScaffold-enabled project (*if it isn't yet*; please check
     :ref:`our guides <migration>` for instructions) and **(b)** :ref:`update
     <updating>` your existing project to the latest version of PyScaffold
     passing the correct ``--namespace`` option.
 
     The slightly more difficult answer for that question is to **(a)** make sure
@@ -289,15 +289,15 @@
     mean that you want to run ``sphinx-apidoc`` with the
     ``--implicit-namespaces`` flag after extending the ``PYTHONPATH`` with the
     ``src`` folder).
 
     The previous steps assume your existing package uses `setuptools`_ and you
     are willing to have a `src layout`_, if that is not the case refer to the
     documentation of your package creator (or the software you use to package
-    up your Python projects) and the `PEP 420`_ for more information.
+    up your Python projects) and the :pep:`420` for more information.
 
 
 pyproject.toml
 --------------
 
 Can I modify ``requires`` despite the warning in ``pyproject.toml`` to avoid doing that?
     You can definitely modify ``pyproject.toml``, but it is good to understand how PyScaffold uses it.
@@ -446,23 +446,19 @@
 .. _blog post by Ionel: https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure
 .. _src layout: https://blog.ionelmc.ro/2014/05/25/python-packaging/#the-structure
 .. _discussions: https://github.com/pyscaffold/pyscaffold/discussions
 .. _Q&A: https://github.com/pyscaffold/pyscaffold/discussions/categories/q-a
 .. _wheel format: https://pythonwheels.com
 .. _Cargo: https://doc.rust-lang.org/stable/cargo/
 .. _Rust: https://www.rust-lang.org
-.. _Zen of Python: https://www.python.org/dev/peps/pep-0020
 .. _six: https://six.readthedocs.io
 .. _Twitter: https://twitter.com/FlorianWilhelm
 .. _setuptools: https://setuptools.pypa.io/en/stable/userguide/declarative_config.html
 .. _setuptools docs on data files: https://setuptools.pypa.io/en/latest/userguide/datafiles.html
 .. _Cython: https://cython.org
-.. _PEP 517: https://www.python.org/dev/peps/pep-0517/
-.. _PEP 518: https://www.python.org/dev/peps/pep-0518/
-.. _PEP 420: https://www.python.org/dev/peps/pep-0420/
 .. _isolated environment: https://realpython.com/python-virtual-environments-a-primer/
 .. _setup.cfg: https://setuptools.pypa.io/en/stable/userguide/declarative_config.html
 .. _tox: https://tox.wiki/en/stable/
 .. _packaging namespace packages official guide: https://packaging.python.org/guides/packaging-namespace-packages
 .. _pkg_resources: https://setuptools.pypa.io/en/stable/pkg_resources.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _pyscaffoldext-cookiecutter: https://github.com/pyscaffold/pyscaffoldext-cookiecutter
```

### Comparing `PyScaffold-4.4/docs/features.rst` & `PyScaffold-4.4.1/docs/features.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 All configuration can be done in ``setup.cfg`` like changing the description,
 URL, classifiers, installation requirements and so on as defined by setuptools_.
 That means in most cases it is not necessary to tamper with ``setup.py``.
 The syntax of ``setup.cfg`` is pretty much self-explanatory and well commented,
 check out this :ref:`example <configuration>` or `setuptools' documentation`_.
 
 If you use tox_, PyScaffold will already configure everything out of the box
-[#feat1]_ so you can easily build your distribution, in a `PEP 517`_/`PEP 518`_
+[#feat1]_ so you can easily build your distribution, in a :pep:`517`/:pep:`518`
 compliant way, by just running::
 
     tox -e build
 
 Alternatively, if you are not a huge fan of isolated builds, or prefer running
 the commands yourself, you can execute ``python -m build --no-isolation``.
 
@@ -58,30 +58,30 @@
    Old guides might mention ``python setup.py upload``, but its use is strongly discouraged
    nowadays and even some of the new PyPI_ features won't work correctly if you don't use twine_.
 
 Namespace Packages
 ------------------
 
 If you want to work with `namespace packages`_, you will be glad to hear that
-PyScaffold supports the `PEP 420`_ specification for implicit namespaces,
+PyScaffold supports the :pep:`420` specification for implicit namespaces,
 which is very useful to distribute a larger package as a collection of smaller ones.
 ``putup`` can automatically setup everything you need with the ``--namespace``
 option. For example, use::
 
     putup my_project --package my_package --namespace com.my_domain
 
 to define ``my_package`` inside the namespace ``com.my_domain``, Java-style.
 
 .. note::
    Prior to PyScaffold 4.0, namespaces were generated
-   explicitly with `pkg_resources`_, instead of  `PEP 420`_. Moreover, if you
+   explicitly with `pkg_resources`_, instead of :pep:`420`. Moreover, if you
    are developing "subpackages" for already existing namespaces, please check
    which convention the namespaces are currently following. Different styles of
    `namespace packages`_ might be incompatible. If you don't want to update
-   existing namespace packages to `PEP 420`_, you will probably need to
+   existing namespace packages to :pep:`420`, you will probably need to
    manually copy the ``__init__.py`` file for the umbrella namespace folder
    from an existing project. Additionally have a look in our :ref:`FAQ <faq>`
    about how to disable implicit namespaces.
 
 Package and Files Data
 ----------------------
 
@@ -92,15 +92,15 @@
 It is not necessary to have a ``MANIFEST.in`` file for this to work. Just make
 sure that all files are added to your repository.
 To read this data in your code, use::
 
     from pkgutil import get_data
     data = get_data('my_package', 'path/to/my/data.txt')
 
-Starting from Python 3.7 an even better approach is using :ref:`importlib.resources`::
+Starting from Python 3.7 an even better approach is using :obj:`importlib.resources`::
 
     from importlib.resources import read_text, read_binary
     data = read_text('my_package.sub_package', 'data.txt')
 
 Note that we need a proper package structure in this case, i.e. directories need
 to contain ``__init__.py`` and be named as a valid Python package (which follow
 the same rules as variable names).
@@ -135,15 +135,15 @@
 ==============================
 
 Your project is already an initialised Git repository and setuptools_ uses the
 information of tags to infer the version of your project with the help of
 `setuptools_scm`_.  To use this feature you need to tag with the format
 ``MAJOR.MINOR[.PATCH]`` , e.g. ``0.0.1`` or ``0.1``.
 
-You can run ``python -m setuptools_scm`` to retrieve the current `PEP 440`_-compliant version [#feat4]_.
+You can run ``python -m setuptools_scm`` to retrieve the current :pep:`440`-compliant version [#feat4]_.
 This version will be used when building a package and is also accessible through
 ``my_project.__version__``. If you want to upload to PyPI_ you have to tag the current commit
 before uploading since PyPI_ does not allow local versions, e.g. ``0.0.dev5+gc5da6ad``,
 for practical reasons.
 
 Please check our docs for the :ref:`best practices and common errors with version
 numbers <version-faq>`.
@@ -411,18 +411,14 @@
 .. _TestPyPI: https://test.pypi.org/
 .. _twine: https://twine.readthedocs.io/en/stable/
 .. _using TestPyPI: https://packaging.python.org/guides/using-testpypi/
 .. _importlib_resources: https://importlib-resources.readthedocs.io/en/stable/
 .. _flake8: https://flake8.pycqa.org/en/stable/
 .. _GitLab CI: https://docs.gitlab.com/ee/ci/
 .. _GitHub Actions: https://github.com/features/actions
-.. _PEP 420: https://www.python.org/dev/peps/pep-0420/
-.. _PEP 440: https://www.python.org/dev/peps/pep-0440/
-.. _PEP 517: https://www.python.org/dev/peps/pep-0517/
-.. _PEP 518: https://www.python.org/dev/peps/pep-0518/
 .. _pre-commit hooks: https://pre-commit.com/
 .. _setuptools_scm: https://pypi.org/project/setuptools-scm/
 .. _pytest: https://docs.pytest.org/en/stable/
 .. _Cirrus CI: https://cirrus-ci.org/
 .. _pytest-cov: https://github.com/pytest-dev/pytest-cov
 .. _Coveralls: https://coveralls.io/
 .. _pyscaffoldext-dsproject: https://github.com/pyscaffold/pyscaffoldext-dsproject
```

### Comparing `PyScaffold-4.4/docs/gfx/action-pipeline-paths.svg` & `PyScaffold-4.4.1/docs/gfx/action-pipeline-paths.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/action-pipeline.svg` & `PyScaffold-4.4.1/docs/gfx/action-pipeline.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/api-paths.svg` & `PyScaffold-4.4.1/docs/gfx/api-paths.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/api.svg` & `PyScaffold-4.4.1/docs/gfx/api.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/demo.cast` & `PyScaffold-4.4.1/docs/gfx/demo.cast`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/demo.gif` & `PyScaffold-4.4.1/docs/gfx/demo.gif`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/github_logo.png` & `PyScaffold-4.4.1/docs/gfx/github_logo.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/github_logo.svg` & `PyScaffold-4.4.1/docs/gfx/github_logo.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/logo.ico` & `PyScaffold-4.4.1/docs/gfx/logo.ico`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/logo.png` & `PyScaffold-4.4.1/docs/gfx/logo.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/logo.svg` & `PyScaffold-4.4.1/docs/gfx/logo.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/sidebar.png` & `PyScaffold-4.4.1/docs/gfx/sidebar.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/gfx/simple-icon.svg` & `PyScaffold-4.4.1/docs/gfx/simple-icon.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/index.rst` & `PyScaffold-4.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/install.rst` & `PyScaffold-4.4.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/migration.rst` & `PyScaffold-4.4.1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/project-structure.rst` & `PyScaffold-4.4.1/docs/project-structure.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/docs/reasons.rst` & `PyScaffold-4.4.1/docs/reasons.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     setuptools_ (the de facto standard for building Python packages), Sphinx_ (the one & only
     Python documentation tool), pytest_ and tox_ (most commonly used Python testing framework & task runner),
     so the users can run these common tasks using e.g. ``tox -e build``, ``tox -e docs``,
     or ``tox -e publish``.
 
     For those who want to go the extra mile, PyScaffold can also bring `pre-commit`_
     into the mix to run a set of prolific linters and automatic
-    formatters in each commit in order to adhere to common coding standards like `pep8`_
+    formatters in each commit in order to adhere to common coding standards like :pep:`8`
     and `black`_.
 
 Composable
     PyScaffold shows its strengths when combined with other tools, and indeed
     we bring configurations for lots of them by default.
     In the end of the day, a project generated by PyScaffold is just a plain,
     standard Python package, and will interoperate well with the majority of
@@ -113,9 +113,8 @@
 
 .. _setuptools: https://setuptools.pypa.io/en/stable/
 .. _tox: https://tox.wiki/en/stable/
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _pytest: https://docs.pytest.org/en/stable/
 .. _pre-commit: https://pre-commit.com/
 .. _demo project: https://github.com/pyscaffold/pyscaffold-demo
-.. _pep8: https://www.python.org/dev/peps/pep-0008/
 .. _black: https://black.readthedocs.io/en/stable/
```

### Comparing `PyScaffold-4.4/docs/updating.rst` & `PyScaffold-4.4.1/docs/updating.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 
 
 Updates from PyScaffold 3 to PyScaffold 4
 -----------------------------------------
 
 **Most of the time, updating from PyScaffold 3 should be completely automatic**.
 However, since in version 4 we have adopted Python's new standards for
-packaging (`PEP 517`_/`PEP 518`_), you might find the new build process incompatible.
+packaging (:pep:`517`/:pep:`518`), you might find the new build process incompatible.
 
 .. _no-pyproject-steps:
 
 If that is the case, you might want to try reverting to the legacy behaviour
-and preventing the build tools from using isolated builds (`PEP 517`_).
+and preventing the build tools from using isolated builds (:pep:`517`).
 That can be easily done by deleting the `pyproject.toml` file from your package
 root.
 
 You will need, though, to manually follow a few extra steps to make sure
 everything works:
 
 1) Remove PyScaffold from your build dependencies (``setup_requires`` in ``setup.cfg``)
@@ -73,33 +73,33 @@
 
 2) Migrate any configuration options for tools that might be
    using ``pyproject.toml`` to alternative files. For example if you have
    ``isort`` and ``coverage`` configurations in your ``pyproject.toml``, you
    might want to rewrite them in the |isortcfg|_ and |coveragerc|_ files respectively.
 
 3) Please open an issue_ with PyScaffold so we understand with kind of backward
-   incompatibilities `PEP 517`_ and `PEP 518`_ might be causing and try to help.
+   incompatibilities :pep:`517` and :pep:`518` might be causing and try to help.
    Similarly you might also consider opening an issue with setuptools_.
 
 .. warning::
    For the time being you can use the **transitional** ``--no-pyproject``
    option, when running ``putup``, but have in mind that this option will
    be removed in future versions of PyScaffold.
 
-PyScaffold 4 also adopts the `PEP 420`_ scheme for implicit namespaces and will
+PyScaffold 4 also adopts the :pep:`420` scheme for implicit namespaces and will
 automatically migrate existing packages. This is incompatible with the
 previously adopted `pkg_resources`_ methodology. **Fortunately, this will not
 affect you if you are not using namespaces**, but in the case you are,
-installing a new `PEP 420`_-compliant package in an environment that already
+installing a new :pep:`420`-compliant package in an environment that already
 contains other packages with the same namespace but that use the
 `pkg_resources`_ methodology, will likely result in errors (please check the
 `official packaging namespace packages guides`_ for more information).
 
 To solve this problem you will need to either migrate the existing
-packages to `PEP 420`_ or revert some specific configurations in ``setup.cfg``
+packages to :pep:`420` or revert some specific configurations in ``setup.cfg``
 after the update. In particular ``packages = find_namespace:`` should
 be converted back to ``packages = find:`` in the ``[options]`` section (use
 a ``git difftool`` to help you with that).
 If using `Sphinx`_ for the documentation, you can also remove the
 ``--implicit-namespaces`` option in the ``cmd_line_template`` variable in the
 ``docs/conf.py`` file.
 
@@ -121,17 +121,14 @@
    (when the numbers on the right are missing, just assume them as being 0),
    so PyScaffold 3.1.2 has the same major version as PyScaffold 3.3.1, but not
    PyScaffold 4.
 
 .. |isortcfg| replace:: *.isort.cfg*
 .. |coveragerc| replace:: *.coveragerc*
 
-.. _PEP 420: https://www.python.org/dev/peps/pep-0420/
-.. _PEP 517: https://www.python.org/dev/peps/pep-0517/
-.. _PEP 518: https://www.python.org/dev/peps/pep-0518/
 .. _setuptools-scm: https://pypi.org/project/setuptools-scm/
 .. _tox: https://tox.wiki/en/stable/
 .. _make: https://www.gnu.org/software/make/manual/html_node/index.html
 .. _skip_install: https://tox.wiki/en/stable/config.html#skip_install
 .. _official packaging namespace packages guides: https://packaging.python.org/guides/packaging-namespace-packages/
 .. _pkg_resources: https://setuptools.pypa.io/en/stable/pkg_resources.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
```

### Comparing `PyScaffold-4.4/docs/usage.rst` & `PyScaffold-4.4.1/docs/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     from zope import subpackage
     # zope is the namespace and subpackage is the package name
 
   To be honest, there is really only the `Zope project <https://www.zope.org/>`_
   that comes to my mind which is using this exotic feature of Python's packaging system.
   Chances are high, that you will never ever need a namespace package in your life.
-  To learn more about namespaces in the Python ecosystem, check `PEP 420`_.
+  To learn more about namespaces in the Python ecosystem, check :pep:`420`.
 
 
 .. [#ex1] Notice the usage of `SPDX identifiers`_ for specifying the license
    in the CLI
 
 .. [#ex2] Requires the installation of pyscaffoldext-django_.
 
@@ -174,15 +174,15 @@
 we do that to make updates a little smarter.
 
 .. note::
    To avoid splitting the configuration and build parameters among several
    files, PyScaffold uses the same file as `setuptools`_ (``setup.cfg``).
    Storing configuration in `pyproject.toml`_ is not supported.
    In the future, if the default build metadata location changes (as proposed
-   by `PEP 621`_), PyScaffold will follow the same pattern.
+   by :pep:`621`), PyScaffold will follow the same pattern.
 
 
 .. _default-cfg:
 
 PyScaffold's Own Configuration
 ==============================
 
@@ -238,30 +238,28 @@
 option. See ``putup --help`` for more details.
 
 .. warning::
 
     *Experimental Feature* - We are still evaluating how this new and exciting
     feature will work, so its API (including file format and name) is not considered
     stable and might change between minor versions. As previously stated, if
-    the configuration file for `setuptools`_ changes (e.g. with `PEP 621`_),
+    the configuration file for `setuptools`_ changes (e.g. with :pep:`621`),
     PyScaffold will follow that and change its own configuration.
 
     This means that in future versions, PyScaffold will likely adopt a more
     `pyproject.toml`-style configuration (and as a consequence the file name
     and extension might change).
 
 
 .. _setuptools: https://setuptools.pypa.io/en/stable/userguide/declarative_config.html
 .. _pyproject.toml: https://setuptools.pypa.io/en/stable/build_meta.html
-.. _PEP 621: https://www.python.org/dev/peps/pep-0621/
 .. _SPDX identifiers: https://spdx.org/licenses/
 .. _pyscaffoldext-django: https://pyscaffold.org/projects/django/en/stable/
 .. _pip: https://pip.pypa.io/en/stable/
 .. _PyPI: https://pypi.org
-.. _PEP 420: https://www.python.org/dev/peps/pep-0420/
 .. _video tutorial: https://www.youtube.com/watch?v=JwwlRkLKj7o
 .. _this demo project: https://github.com/pyscaffold/pyscaffold-demo
 .. _editable: https://pip.pypa.io/en/stable/cli/pip_install/#editable-installs
 .. _isolated development environment: https://realpython.com/python-virtual-environments-a-primer/
 .. also good, but sometimes medium can get on the way: https://towardsdatascience.com/virtual-environments-104c62d48c54
 .. _virtualenv: https://virtualenv.pypa.io/en/stable/
 .. _conda: https://docs.conda.io/en/latest/
```

### Comparing `PyScaffold-4.4/setup.cfg` & `PyScaffold-4.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/PyScaffold.egg-info/PKG-INFO` & `PyScaffold-4.4.1/src/PyScaffold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScaffold
-Version: 4.4
+Version: 4.4.1
 Summary: Template tool for putting up the scaffold of a Python project
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Florian Wilhelm
 Author-email: Florian.Wilhelm@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/pyscaffold/pyscaffold/
```

### Comparing `PyScaffold-4.4/src/PyScaffold.egg-info/SOURCES.txt` & `PyScaffold-4.4.1/src/PyScaffold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/PyScaffold.egg-info/entry_points.txt` & `PyScaffold-4.4.1/src/PyScaffold.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/PyScaffold.egg-info/requires.txt` & `PyScaffold-4.4.1/src/PyScaffold.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/actions.py` & `PyScaffold-4.4.1/src/pyscaffold/actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/api.py` & `PyScaffold-4.4.1/src/pyscaffold/api.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/cli.py` & `PyScaffold-4.4.1/src/pyscaffold/cli.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/dependencies.py` & `PyScaffold-4.4.1/src/pyscaffold/dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 
 BUILD = ("setuptools_scm>=5",)
 """Dependencies that will be required to build the created project"""
 RUNTIME = ('importlib-metadata; python_version<"3.8"',)
 # TODO: Remove `importlib-metadata` when `python_requires = >= 3.8`
 """Dependencies that will be required at runtime by the created project"""
 ISOLATED = ("setuptools>=46.1.0", "setuptools_scm[toml]>=5", *BUILD[1:])
-"""Dependencies for isolated builds (PEP517/518).
+"""Dependencies for isolated builds (:pep:`517`/:pep:`518`).
 - setuptools min version might be slightly higher then the version required at runtime.
 - setuptools_scm requires an optional dependency to work with pyproject.toml
 """
 # Although version 36.6.0 introduces PEP517 implementation,
 # version 46.1.0 fix a bug with setuptools.finalize_distribution_options,
 # which is a hook used by setuptools_scm (better safe then sorry).
 
 REQ_SPLITTER = re.compile(r";(?!\s*(python|platform|implementation|os|sys)_)", re.M)
-"""Regex to split requirements that considers both `setup.cfg specs`_ and `PEP 508`_
+"""Regex to split requirements that considers both `setup.cfg specs`_ and :pep:`508`
 (in a *good enough* simplified fashion).
 
 .. _setup.cfg specs: https://setuptools.pypa.io/en/latest/userguide/declarative_config.html
-.. _PEP 508: https://www.python.org/dev/peps/pep-0508/
 """  # noqa
 
 
 def split(requirements: str) -> List[str]:
     """Split a combined requirement string (such as the values for ``setup_requires``
     and ``install_requires`` in ``setup.cfg``) into a list of individual requirement
     strings, that can be used in :obj:`is_included`, :obj:`get_requirements_str`,
@@ -61,16 +60,16 @@
 def add(requirements: Iterable[str], to_add: Iterable[str] = BUILD) -> List[str]:
     """Given a sequence of individual requirement strings, add ``to_add`` to it.
     By default adds :obj:`BUILD` if ``to_add`` is not given."""
     return deduplicate(chain(requirements, to_add))
 
 
 def attempt_pkg_name(requirement: str) -> str:
-    """In the case the given string is a dependency specification (PEP 508/440),
-    it returns the "package name" part of dependency (without versions).
+    """In the case the given string is a dependency specification (:pep:`508`/
+    :pep`440`), it returns the "package name" part of dependency (without versions).
     Otherwise, it returns the same string (removed the comment marks).
     """
     req = requirement.strip("#").strip()
     try:
         return Requirement(req).name
     except InvalidRequirement:
         return req
```

### Comparing `PyScaffold-4.4/src/pyscaffold/exceptions.py` & `PyScaffold-4.4.1/src/pyscaffold/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
 
     def exceptions2exit_decorator(func):
         @functools.wraps(func)
         def func_wrapper(*args, **kwargs):
             try:
                 func(*args, **kwargs)
-            except tuple(exception_list) as ex:
+            except tuple(exception_list) as ex:  # noqa: B030
                 from .cli import get_log_level  # defer circular imports to avoid errors
 
                 if get_log_level() <= logging.DEBUG:
                     # user surely wants to see the stacktrace
                     traceback.print_exc()
                 print(f"ERROR: {ex}")
                 sys.exit(1)
```

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/__init__.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/cirrus.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/cirrus.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/config.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/config.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/github_actions.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/gitlab_ci.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/interactive.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/interactive.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/namespace.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/namespace.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/no_pyproject.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/no_pyproject.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/no_skeleton.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/no_skeleton.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/no_tox.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/no_tox.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/pre_commit.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/extensions/venv.py` & `PyScaffold-4.4.1/src/pyscaffold/extensions/venv.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/file_system.py` & `PyScaffold-4.4.1/src/pyscaffold/file_system.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/identification.py` & `PyScaffold-4.4.1/src/pyscaffold/identification.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/info.py` & `PyScaffold-4.4.1/src/pyscaffold/info.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/log.py` & `PyScaffold-4.4.1/src/pyscaffold/log.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/operations.py` & `PyScaffold-4.4.1/src/pyscaffold/operations.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/repo.py` & `PyScaffold-4.4.1/src/pyscaffold/repo.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/shell.py` & `PyScaffold-4.4.1/src/pyscaffold/shell.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/structure.py` & `PyScaffold-4.4.1/src/pyscaffold/structure.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/__init__.py` & `PyScaffold-4.4.1/src/pyscaffold/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/__init__.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/__init__.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/cirrus.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/cirrus.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/contributing.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/contributing.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/coveragerc.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/coveragerc.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/github_ci_workflow.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/github_ci_workflow.template`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
   pull_request:  # Run in every PR
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
 
+permissions:
+  contents: read
+
 concurrency:
   group: >-
     ${{ github.workflow }}-${{ github.ref_type }}-
     ${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 jobs:
@@ -80,15 +83,15 @@
           -- -rFEx --durations 10 --color yes  # pytest args
       - name: Generate coverage report
         run: pipx run coverage lcov -o coverage.lcov
       - name: Upload partial coverage report
         uses: coverallsapp/github-action@master
         with:
           path-to-lcov: coverage.lcov
-          github-token: ${{ secrets.github_token }}
+          github-token: ${{ secrets.GITHUB_TOKEN }}
           flag-name: ${{ matrix.platform }} - py${{ matrix.python }}
           parallel: true
 
   finalize:
     needs: test
     runs-on: ubuntu-latest
     steps:
@@ -98,14 +101,16 @@
           github-token: ${{ secrets.GITHUB_TOKEN }}
           parallel-finished: true
 
   publish:
     needs: finalize
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with: {python-version: "3.11"}
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
```

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/gitignore.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/gitlab_ci.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/gitlab_ci.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/header_interactive.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/header_interactive.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_affero_3.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_affero_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_apache.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_artistic_2.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_artistic_2.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_bsd0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_bsd0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_cc0_1.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_cc0_1.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_eclipse_1.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_eclipse_1.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_gpl_2.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_2.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_gpl_3.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_isc.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_isc.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_lgpl_2.1.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_2.1.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_lgpl_3.0.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_mit.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_mozilla.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_mozilla.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_new_bsd.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_new_bsd.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_public_domain.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_public_domain.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/license_simplified_bsd.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/license_simplified_bsd.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/pre-commit-config.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/pre-commit-config.template`

 * *Files 5% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 #   rev: v3.3.1
 #   hooks:
 #   - id: pyupgrade
 #     args: ['--py37-plus']
 
 ## If you want to avoid flake8 errors due to unused vars or imports:
 # - repo: https://github.com/PyCQA/autoflake
-#   rev: v2.0.0
+#   rev: v2.0.2
 #   hooks:
 #   - id: autoflake
 #     args: [
 #       --in-place,
 #       --remove-all-unused-imports,
 #       --remove-unused-variables,
 #     ]
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.11.4
+  rev: 5.11.5
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
   rev: stable
   hooks:
   - id: black
@@ -58,10 +58,10 @@
   hooks:
   - id: flake8
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
 
 ## Check for misspells in documentation files:
 # - repo: https://github.com/codespell-project/codespell
-#   rev: v2.2.2
+#   rev: v2.2.4
 #   hooks:
 #   - id: codespell
```

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/readme.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/readme.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/rtd_cfg.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/rtd_cfg.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/setup_cfg.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/setup_cfg.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/setup_py.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/setup_py.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/skeleton.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/skeleton.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/sphinx_conf.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_conf.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/sphinx_index.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_index.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/sphinx_makefile.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_makefile.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/test_skeleton.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/test_skeleton.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/templates/tox_ini.template` & `PyScaffold-4.4.1/src/pyscaffold/templates/tox_ini.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/termui.py` & `PyScaffold-4.4.1/src/pyscaffold/termui.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/src/pyscaffold/toml.py` & `PyScaffold-4.4.1/src/pyscaffold/toml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Thin wrapper around the dependency so we can maintain some stability while being able
 to swap implementations (e.g. replace `tomlkit`_ with `toml`_).
 
-Despite being used in `pep517`_, `toml`_ offers limited support for comments, so we
-prefer `tomlkit`_.
-
+`tomlkit`_ is preferred because it supports comments.
 
 .. _tomlkit: https://github.com/sdispater/tomlkit
 .. _toml: https://github.com/uiri/toml
-.. _pep517: https://github.com/pypa/pep517
 """
 from typing import Any, List, MutableMapping, NewType, Tuple, TypeVar, Union, cast
 
 import tomlkit
 
 TOMLMapping = NewType("TOMLMapping", MutableMapping)
 """Abstraction on the value returned by :obj:`loads`.
```

### Comparing `PyScaffold-4.4/src/pyscaffold/update.py` & `PyScaffold-4.4.1/src/pyscaffold/update.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/conftest.py` & `PyScaffold-4.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/demoapp/runner.py` & `PyScaffold-4.4.1/tests/demoapp/runner.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/demoapp/setup.cfg` & `PyScaffold-4.4.1/tests/demoapp/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/demoapp_data/runner.py` & `PyScaffold-4.4.1/tests/demoapp_data/runner.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/demoapp_data/setup.cfg` & `PyScaffold-4.4.1/tests/demoapp_data/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/examples/issue-506/setup.cfg` & `PyScaffold-4.4.1/tests/examples/issue-506/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/incompatible_v3_api_fake_extension.py` & `PyScaffold-4.4.1/tests/extensions/incompatible_v3_api_fake_extension.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_cirrus.py` & `PyScaffold-4.4.1/tests/extensions/test_cirrus.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_config.py` & `PyScaffold-4.4.1/tests/extensions/test_config.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_github_actions.py` & `PyScaffold-4.4.1/tests/extensions/test_github_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_gitlab_ci.py` & `PyScaffold-4.4.1/tests/extensions/test_gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_interactive.py` & `PyScaffold-4.4.1/tests/extensions/test_interactive.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_namespace.py` & `PyScaffold-4.4.1/tests/extensions/test_namespace.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_no_pyproject.py` & `PyScaffold-4.4.1/tests/extensions/test_no_pyproject.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_no_skeleton.py` & `PyScaffold-4.4.1/tests/extensions/test_no_skeleton.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_no_tox.py` & `PyScaffold-4.4.1/tests/extensions/test_no_tox.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_pre_commit.py` & `PyScaffold-4.4.1/tests/extensions/test_pre_commit.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/extensions/test_venv.py` & `PyScaffold-4.4.1/tests/extensions/test_venv.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/helpers.py` & `PyScaffold-4.4.1/tests/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import builtins
 import logging
 import os
+import os.path
 import stat
 import traceback
 from contextlib import contextmanager
 from glob import glob
 from pathlib import Path
 from pprint import pformat
 from shutil import rmtree
@@ -18,14 +19,19 @@
 skip_on_conda_build = pytest.mark.skipif(
     os.getenv("CONDA_BUILD"),
     reason="conda build does not run inside virtualenv/tox and "
     "it does not have PyScaffold's source code available when running tests",
 )
 
 
+def in_ci() -> bool:
+    ci = os.getenv("CI", None) or ""
+    return bool(ci.lower() in ("1", "true") or os.getenv("CI_NAME", None))
+
+
 def uniqstr():
     """Generates a unique random long string every time it is called"""
     return str(uuid4())
 
 
 def uniqpath(nested=False):
     path = uniqstr()
@@ -50,14 +56,18 @@
     except FileNotFoundError:
         return
     except Exception:
         msg = f"rmpath: Impossible to remove {path}, probably an OS issue...\n\n"
         warn(msg + traceback.format_exc())
 
 
+def path_as_uri(path):
+    return Path(os.path.abspath(path)).as_uri()
+
+
 def set_writable(func, path, exc_info):
     max_attempts = 15
     retry_interval = 0.1
     effective_ids = os.access in os.supports_effective_ids
     existing_files = glob(f"{path}/*")
 
     if not os.access(path, os.W_OK, effective_ids=effective_ids):
```

### Comparing `PyScaffold-4.4/tests/log_helpers.py` & `PyScaffold-4.4.1/tests/log_helpers.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/system/helpers.py` & `PyScaffold-4.4.1/tests/system/helpers.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/system/test_common.py` & `PyScaffold-4.4.1/tests/system/test_common.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/system/test_dependency_managers.py` & `PyScaffold-4.4.1/tests/system/test_dependency_managers.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_actions.py` & `PyScaffold-4.4.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_api.py` & `PyScaffold-4.4.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_cli.py` & `PyScaffold-4.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_dependencies.py` & `PyScaffold-4.4.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_examples.py` & `PyScaffold-4.4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_exceptions.py` & `PyScaffold-4.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_extensions.py` & `PyScaffold-4.4.1/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_file_system.py` & `PyScaffold-4.4.1/tests/test_file_system.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_identification.py` & `PyScaffold-4.4.1/tests/test_identification.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_info.py` & `PyScaffold-4.4.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_install.py` & `PyScaffold-4.4.1/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_log.py` & `PyScaffold-4.4.1/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_operations.py` & `PyScaffold-4.4.1/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_repo.py` & `PyScaffold-4.4.1/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_shell.py` & `PyScaffold-4.4.1/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_structure.py` & `PyScaffold-4.4.1/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_templates.py` & `PyScaffold-4.4.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_termui.py` & `PyScaffold-4.4.1/tests/test_termui.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_toml.py` & `PyScaffold-4.4.1/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4/tests/test_update.py` & `PyScaffold-4.4.1/tests/test_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pytest
 from packaging.version import Version
 
 from pyscaffold import __path__ as pyscaffold_paths
 from pyscaffold import __version__, actions, info, update
 from pyscaffold.file_system import chdir
 
-from .helpers import skip_on_conda_build
+from .helpers import in_ci, path_as_uri, skip_on_conda_build
 
 EDITABLE_PYSCAFFOLD = re.compile(r"^-e.+pyscaffold.*$", re.M | re.I)
 
 
 class VenvManager:
     def __init__(self, tmpdir, venv, pytestconfig):
         self.tmpdir = str(tmpdir)  # convert Path to str
@@ -40,18 +40,15 @@
         # var for trusted hosts
         return self.run(
             f"{python} -m pip install {pkg} --trusted-host pypi.python.org "
             "--trusted-host files.pythonhosted.org --trusted-host pypi.org",
             **kwargs,
         )
 
-    def install_this_pyscaffold(self):
-        # Normally the following command should do the trick
-        # self.venv.install_package('PyScaffold')
-        # but sadly pytest-virtualenv chokes on the src-layout of PyScaffold
+    def _get_proj_dir(self) -> Path:
         if "TOXINIDIR" in os.environ:
             # so pytest runs within tox
             proj_dir = Path(os.environ["TOXINIDIR"])
             logging.debug("SRC via TOXINIDIR: %s", proj_dir)
         else:
             try:
                 location = Path(pyscaffold_paths[0])
@@ -59,21 +56,43 @@
                 proj_dir = location.parent.parent
             except:  # noqa
                 print("\n\nInstall PyScaffold with python setup.py develop!\n\n")
                 raise
 
             logging.debug("SRC via working_set: %s, location: %s", proj_dir, location)
 
+        return proj_dir
+
+    def _install_pre_built_wheel(self, proj_dir: Path):
+        # CI should pre-build wheels that can be used.
+        candidates = (proj_dir / "dist").glob("PyScaffold*.whl")
+        wheel = next(iter(sorted(candidates, reverse=True, key=str)), None)
+        assert wheel, "PyScaffold should be pre-built by CI, but it is not..."
+        return self.install(path_as_uri(wheel))
+
+    def _install_from_src(self, proj_dir: Path):
         env = {**os.environ, "SETUPTOOLS_SCM_PRETEND_VERSION": __version__}
         assert proj_dir.exists(), f"{proj_dir} is supposed to exist"
-        self.install(proj_dir, editable=True, env=env)
-        # Make sure pyscaffold was not installed using PyPI
-        assert self.running_version.public <= self.pyscaffold_version().public
+        out = self.install(proj_dir, editable=True, env=env)
         pkg_list = self.run(f"{self.venv.python} -m pip freeze")
         assert EDITABLE_PYSCAFFOLD.findall(pkg_list)
+        return out
+
+    def install_this_pyscaffold(self):
+        # Normally the following command should do the trick
+        # self.venv.install_package('PyScaffold')
+        # but sadly pytest-virtualenv chokes on the src-layout of PyScaffold
+        proj_dir = self._get_proj_dir()
+        if in_ci():
+            self._install_pre_built_wheel(proj_dir)
+        else:
+            self._install_from_src(proj_dir)
+
+        # Make sure pyscaffold was not installed using PyPI
+        assert self.running_version.public <= self.pyscaffold_version().public
         self.installed = True
         return self
 
     def install_pyscaffold(self, major, minor):
         ver = f"pyscaffold>={major}.{minor},<{major}.{minor + 1}a0"
         self.install(ver)
         installed_version = self.pyscaffold_version()._version.release[:2]
```

### Comparing `PyScaffold-4.4/tox.ini` & `PyScaffold-4.4.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     PIP_CACHE
     PIP_TRUSTED_HOST
     PRE_COMMIT_HOME
     REQUESTS_CA_BUNDLE
     CURL_CA_BUNDLE
     USING_CONDA
     SETUPTOOLS_*
+    CI
+    CI_*
 extras =
     # TODO: Uncomment `all` once all the extensions are updated
     #       to the new version of pyscaffold
     all
     testing
 commands =
     default: pytest -k "not system" {posargs}
```

