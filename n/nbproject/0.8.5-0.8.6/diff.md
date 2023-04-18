# Comparing `tmp/nbproject-0.8.5.tar.gz` & `tmp/nbproject-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbproject-0.8.5.tar", last modified: Mon Apr 17 13:01:13 2023, max compression
+gzip compressed data, was "nbproject-0.8.6.tar", last modified: Tue Apr 18 16:40:16 2023, max compression
```

## Comparing `nbproject-0.8.5.tar` & `nbproject-0.8.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     2574 2023-04-17 07:11:01.411035 nbproject-0.8.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.8.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.8.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.8.5/.gitignore
--rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.8.5/CITATION.cff
--rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.8.5/LICENSE
--rw-r--r--   0        0        0     1404 2023-04-17 07:11:01.411511 nbproject-0.8.5/README.md
--rw-r--r--   0        0        0    19810 2023-04-17 13:00:39.473943 nbproject-0.8.5/docs/changelog.md
--rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.213819 nbproject-0.8.5/docs/faq/example-after-init-set-filename.ipynb
--rw-r--r--   0        0        0     1481 2022-10-07 21:00:12.845099 nbproject-0.8.5/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
--rw-r--r--   0        0        0      123 2022-09-06 11:40:41.171382 nbproject-0.8.5/docs/faq/example-project-uninitialized/index.md
--rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.214012 nbproject-0.8.5/docs/faq/example-project/2022-05-13-my-task-x.ipynb
--rw-r--r--   0        0        0     1661 2022-11-12 18:33:53.214173 nbproject-0.8.5/docs/faq/example-project/2022-07-18-my-task-y.ipynb
--rw-r--r--   0        0        0      101 2022-09-06 11:40:41.171829 nbproject-0.8.5/docs/faq/example-project/index.md
--rw-r--r--   0        0        0      364 2022-11-12 18:33:53.214429 nbproject-0.8.5/docs/faq/example-project/nbproject_metadata.yml
--rw-r--r--   0        0        0     1873 2022-11-12 18:33:53.214599 nbproject-0.8.5/docs/faq/header-author-field.ipynb
--rw-r--r--   0        0        0     1520 2022-11-12 18:33:53.214757 nbproject-0.8.5/docs/faq/inconsistent-packages-parents-no-store.ipynb
--rw-r--r--   0        0        0     2330 2022-11-12 18:33:53.214908 nbproject-0.8.5/docs/faq/inconsistent-packages-parents-store.ipynb
--rw-r--r--   0        0        0     1096 2022-10-10 12:03:49.454347 nbproject-0.8.5/docs/faq/index.md
--rw-r--r--   0        0        0     1311 2022-09-06 11:40:41.172354 nbproject-0.8.5/docs/faq/initialize-set-env.ipynb
--rw-r--r--   0        0        0     2049 2022-09-06 11:40:41.172505 nbproject-0.8.5/docs/faq/initialize.ipynb
--rw-r--r--   0        0        0     4086 2022-11-12 18:33:53.215053 nbproject-0.8.5/docs/faq/internal-functions.ipynb
--rw-r--r--   0        0        0     2708 2022-09-06 11:40:41.172679 nbproject-0.8.5/docs/faq/not-initialized.ipynb
--rw-r--r--   0        0        0     1803 2022-11-12 18:33:53.215192 nbproject-0.8.5/docs/faq/publish-not-last-cell.ipynb
--rw-r--r--   0        0        0     1399 2022-11-12 18:33:53.215339 nbproject-0.8.5/docs/faq/publish-set-version.ipynb
--rw-r--r--   0        0        0     1818 2022-11-12 18:33:53.215489 nbproject-0.8.5/docs/faq/publish-without-saving.ipynb
--rw-r--r--   0        0        0     1787 2022-11-12 18:33:53.215632 nbproject-0.8.5/docs/faq/publish-without-title.ipynb
--rw-r--r--   0        0        0     1653 2022-11-12 18:33:53.215765 nbproject-0.8.5/docs/faq/publish-wrapper.ipynb
--rw-r--r--   0        0        0     1577 2022-10-07 21:00:16.804143 nbproject-0.8.5/docs/faq/set-env-via-environment-var.ipynb
--rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.8.5/docs/faq/setup.md
--rw-r--r--   0        0        0     1357 2022-09-06 11:40:41.173529 nbproject-0.8.5/docs/faq/trigger-exit-upon-init.ipynb
--rw-r--r--   0        0        0     2694 2022-11-12 18:33:53.215926 nbproject-0.8.5/docs/guide/basic-metadata.ipynb
--rw-r--r--   0        0        0     2675 2022-09-06 11:40:41.173736 nbproject-0.8.5/docs/guide/cli.md
--rw-r--r--   0        0        0      328 2022-09-06 11:40:41.173880 nbproject-0.8.5/docs/guide/index.md
--rw-r--r--   0        0        0     4639 2023-04-17 07:11:01.412769 nbproject-0.8.5/docs/guide/meta.ipynb
--rw-r--r--   0        0        0     1637 2022-11-12 18:33:53.216221 nbproject-0.8.5/docs/guide/received.ipynb
--rw-r--r--   0        0        0     2964 2022-11-12 18:33:53.216369 nbproject-0.8.5/docs/guide/update-metadata.ipynb
--rw-r--r--   0        0        0      142 2023-04-17 07:11:01.413339 nbproject-0.8.5/docs/index.md
--rw-r--r--   0        0        0     2755 2022-11-12 18:33:53.216521 nbproject-0.8.5/docs/quickstart.ipynb
--rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.8.5/docs/reference.md
--rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.8.5/lamin-project.yaml
--rw-r--r--   0        0        0      658 2023-04-17 12:59:28.739410 nbproject-0.8.5/nbproject/__init__.py
--rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.8.5/nbproject/__main__.py
--rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.8.5/nbproject/_cli.py
--rw-r--r--   0        0        0     5720 2023-04-17 07:11:01.414277 nbproject-0.8.5/nbproject/_header.py
--rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.8.5/nbproject/_is_run_from_ipython.py
--rw-r--r--   0        0        0       48 2022-07-23 18:45:14.093130 nbproject-0.8.5/nbproject/_logger.py
--rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.8.5/nbproject/_meta.py
--rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.8.5/nbproject/_publish.py
--rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.8.5/nbproject/_schemas.py
--rw-r--r--   0        0        0      924 2022-09-26 22:11:29.434198 nbproject-0.8.5/nbproject/dev/__init__.py
--rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.8.5/nbproject/dev/_check_last_cell.py
--rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.8.5/nbproject/dev/_classic_nb_commands.py
--rw-r--r--   0        0        0     1471 2022-08-27 06:14:49.459673 nbproject-0.8.5/nbproject/dev/_consecutiveness.py
--rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.8.5/nbproject/dev/_frontend_commands.py
--rw-r--r--   0        0        0     1693 2022-10-10 18:44:26.046062 nbproject-0.8.5/nbproject/dev/_initialize.py
--rw-r--r--   0        0        0     5136 2023-04-17 12:58:56.403151 nbproject-0.8.5/nbproject/dev/_jupyter_communicate.py
--rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.8.5/nbproject/dev/_jupyter_lab_commands.py
--rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.8.5/nbproject/dev/_lamin_communicate.py
--rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.8.5/nbproject/dev/_meta_live.py
--rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.8.5/nbproject/dev/_meta_store.py
--rw-r--r--   0        0        0     5385 2022-11-12 18:33:53.217735 nbproject-0.8.5/nbproject/dev/_metadata_display.py
--rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.8.5/nbproject/dev/_notebook.py
--rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.8.5/nbproject/dev/_pypackage.py
--rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.8.5/nbproject/dev/_set_version.py
--rw-r--r--   0        0        0      575 2023-04-17 07:11:01.416205 nbproject-0.8.5/noxfile.py
--rw-r--r--   0        0        0     1091 2023-04-17 07:11:01.416607 nbproject-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.8.5/tests/conftest.py
--rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.8.5/tests/test_cli.py
--rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.8.5/tests/test_jupyter.py
--rw-r--r--   0        0        0      322 2022-08-29 09:33:05.137063 nbproject-0.8.5/tests/test_notebooks.py
--rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.8.5/tests/test_set_version.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 nbproject-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     2574 2023-04-17 07:11:01.411035 nbproject-0.8.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-06-10 19:50:58.313927 nbproject-0.8.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-06-10 19:50:58.314964 nbproject-0.8.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1880 2022-07-10 12:10:29.382368 nbproject-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1645 2022-08-29 09:33:05.135542 nbproject-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      740 2022-10-24 12:29:45.346974 nbproject-0.8.6/CITATION.cff
+-rw-r--r--   0        0        0    11357 2022-04-18 20:46:44.681265 nbproject-0.8.6/LICENSE
+-rw-r--r--   0        0        0     1404 2023-04-17 07:11:01.411511 nbproject-0.8.6/README.md
+-rw-r--r--   0        0        0    19961 2023-04-18 16:39:58.542962 nbproject-0.8.6/docs/changelog.md
+-rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.213819 nbproject-0.8.6/docs/faq/example-after-init-set-filename.ipynb
+-rw-r--r--   0        0        0     1481 2022-10-07 21:00:12.845099 nbproject-0.8.6/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb
+-rw-r--r--   0        0        0      123 2022-09-06 11:40:41.171382 nbproject-0.8.6/docs/faq/example-project-uninitialized/index.md
+-rw-r--r--   0        0        0     1874 2022-11-12 18:33:53.214012 nbproject-0.8.6/docs/faq/example-project/2022-05-13-my-task-x.ipynb
+-rw-r--r--   0        0        0     1661 2022-11-12 18:33:53.214173 nbproject-0.8.6/docs/faq/example-project/2022-07-18-my-task-y.ipynb
+-rw-r--r--   0        0        0      101 2022-09-06 11:40:41.171829 nbproject-0.8.6/docs/faq/example-project/index.md
+-rw-r--r--   0        0        0      364 2022-11-12 18:33:53.214429 nbproject-0.8.6/docs/faq/example-project/nbproject_metadata.yml
+-rw-r--r--   0        0        0     1873 2022-11-12 18:33:53.214599 nbproject-0.8.6/docs/faq/header-author-field.ipynb
+-rw-r--r--   0        0        0     1520 2022-11-12 18:33:53.214757 nbproject-0.8.6/docs/faq/inconsistent-packages-parents-no-store.ipynb
+-rw-r--r--   0        0        0     2330 2022-11-12 18:33:53.214908 nbproject-0.8.6/docs/faq/inconsistent-packages-parents-store.ipynb
+-rw-r--r--   0        0        0     1096 2022-10-10 12:03:49.454347 nbproject-0.8.6/docs/faq/index.md
+-rw-r--r--   0        0        0     1311 2022-09-06 11:40:41.172354 nbproject-0.8.6/docs/faq/initialize-set-env.ipynb
+-rw-r--r--   0        0        0     2049 2022-09-06 11:40:41.172505 nbproject-0.8.6/docs/faq/initialize.ipynb
+-rw-r--r--   0        0        0     4086 2022-11-12 18:33:53.215053 nbproject-0.8.6/docs/faq/internal-functions.ipynb
+-rw-r--r--   0        0        0     2708 2022-09-06 11:40:41.172679 nbproject-0.8.6/docs/faq/not-initialized.ipynb
+-rw-r--r--   0        0        0     1803 2022-11-12 18:33:53.215192 nbproject-0.8.6/docs/faq/publish-not-last-cell.ipynb
+-rw-r--r--   0        0        0     1399 2022-11-12 18:33:53.215339 nbproject-0.8.6/docs/faq/publish-set-version.ipynb
+-rw-r--r--   0        0        0     1818 2022-11-12 18:33:53.215489 nbproject-0.8.6/docs/faq/publish-without-saving.ipynb
+-rw-r--r--   0        0        0     1787 2022-11-12 18:33:53.215632 nbproject-0.8.6/docs/faq/publish-without-title.ipynb
+-rw-r--r--   0        0        0     1653 2022-11-12 18:33:53.215765 nbproject-0.8.6/docs/faq/publish-wrapper.ipynb
+-rw-r--r--   0        0        0     1577 2022-10-07 21:00:16.804143 nbproject-0.8.6/docs/faq/set-env-via-environment-var.ipynb
+-rw-r--r--   0        0        0      679 2022-10-10 14:54:28.366976 nbproject-0.8.6/docs/faq/setup.md
+-rw-r--r--   0        0        0     1357 2022-09-06 11:40:41.173529 nbproject-0.8.6/docs/faq/trigger-exit-upon-init.ipynb
+-rw-r--r--   0        0        0     2694 2022-11-12 18:33:53.215926 nbproject-0.8.6/docs/guide/basic-metadata.ipynb
+-rw-r--r--   0        0        0     2675 2022-09-06 11:40:41.173736 nbproject-0.8.6/docs/guide/cli.md
+-rw-r--r--   0        0        0      328 2022-09-06 11:40:41.173880 nbproject-0.8.6/docs/guide/index.md
+-rw-r--r--   0        0        0     4639 2023-04-17 07:11:01.412769 nbproject-0.8.6/docs/guide/meta.ipynb
+-rw-r--r--   0        0        0     1637 2022-11-12 18:33:53.216221 nbproject-0.8.6/docs/guide/received.ipynb
+-rw-r--r--   0        0        0     2964 2022-11-12 18:33:53.216369 nbproject-0.8.6/docs/guide/update-metadata.ipynb
+-rw-r--r--   0        0        0      142 2023-04-17 07:11:01.413339 nbproject-0.8.6/docs/index.md
+-rw-r--r--   0        0        0     2755 2022-11-12 18:33:53.216521 nbproject-0.8.6/docs/quickstart.ipynb
+-rw-r--r--   0        0        0       57 2023-04-17 07:11:01.413670 nbproject-0.8.6/docs/reference.md
+-rw-r--r--   0        0        0      137 2022-06-01 14:27:38.468097 nbproject-0.8.6/lamin-project.yaml
+-rw-r--r--   0        0        0      763 2023-04-18 16:39:50.848566 nbproject-0.8.6/nbproject/__init__.py
+-rw-r--r--   0        0        0     1631 2022-08-17 11:48:35.494040 nbproject-0.8.6/nbproject/__main__.py
+-rw-r--r--   0        0        0     5121 2022-11-12 18:33:53.216715 nbproject-0.8.6/nbproject/_cli.py
+-rw-r--r--   0        0        0     5720 2023-04-17 07:11:01.414277 nbproject-0.8.6/nbproject/_header.py
+-rw-r--r--   0        0        0      285 2022-11-13 23:00:04.437788 nbproject-0.8.6/nbproject/_is_run_from_ipython.py
+-rw-r--r--   0        0        0       48 2022-07-23 18:45:14.093130 nbproject-0.8.6/nbproject/_logger.py
+-rw-r--r--   0        0        0     3080 2022-10-10 12:03:49.455892 nbproject-0.8.6/nbproject/_meta.py
+-rw-r--r--   0        0        0     3943 2022-11-12 18:52:44.680900 nbproject-0.8.6/nbproject/_publish.py
+-rw-r--r--   0        0        0     4007 2022-11-12 18:33:53.217134 nbproject-0.8.6/nbproject/_schemas.py
+-rw-r--r--   0        0        0      924 2022-09-26 22:11:29.434198 nbproject-0.8.6/nbproject/dev/__init__.py
+-rw-r--r--   0        0        0      590 2022-10-07 21:00:16.805272 nbproject-0.8.6/nbproject/dev/_check_last_cell.py
+-rw-r--r--   0        0        0      681 2022-08-17 11:48:35.496655 nbproject-0.8.6/nbproject/dev/_classic_nb_commands.py
+-rw-r--r--   0        0        0     1471 2022-08-27 06:14:49.459673 nbproject-0.8.6/nbproject/dev/_consecutiveness.py
+-rw-r--r--   0        0        0      525 2022-08-17 11:48:35.496751 nbproject-0.8.6/nbproject/dev/_frontend_commands.py
+-rw-r--r--   0        0        0     1693 2022-10-10 18:44:26.046062 nbproject-0.8.6/nbproject/dev/_initialize.py
+-rw-r--r--   0        0        0     5136 2023-04-17 12:58:56.403151 nbproject-0.8.6/nbproject/dev/_jupyter_communicate.py
+-rw-r--r--   0        0        0      822 2023-04-17 07:11:01.415333 nbproject-0.8.6/nbproject/dev/_jupyter_lab_commands.py
+-rw-r--r--   0        0        0      343 2023-04-17 07:11:01.415771 nbproject-0.8.6/nbproject/dev/_lamin_communicate.py
+-rw-r--r--   0        0        0     3642 2022-10-10 18:44:26.046429 nbproject-0.8.6/nbproject/dev/_meta_live.py
+-rw-r--r--   0        0        0     4541 2022-11-12 18:33:53.217570 nbproject-0.8.6/nbproject/dev/_meta_store.py
+-rw-r--r--   0        0        0     5385 2022-11-12 18:33:53.217735 nbproject-0.8.6/nbproject/dev/_metadata_display.py
+-rw-r--r--   0        0        0      922 2022-07-15 19:53:53.061564 nbproject-0.8.6/nbproject/dev/_notebook.py
+-rw-r--r--   0        0        0     3900 2022-07-23 14:31:43.204220 nbproject-0.8.6/nbproject/dev/_pypackage.py
+-rw-r--r--   0        0        0      575 2022-11-12 18:52:44.681103 nbproject-0.8.6/nbproject/dev/_set_version.py
+-rw-r--r--   0        0        0      575 2023-04-17 07:11:01.416205 nbproject-0.8.6/noxfile.py
+-rw-r--r--   0        0        0     1091 2023-04-17 07:11:01.416607 nbproject-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      920 2022-09-06 11:40:41.175303 nbproject-0.8.6/tests/conftest.py
+-rw-r--r--   0        0        0     2428 2022-09-06 11:40:41.175526 nbproject-0.8.6/tests/test_cli.py
+-rw-r--r--   0        0        0     1472 2023-04-17 07:11:01.416978 nbproject-0.8.6/tests/test_jupyter.py
+-rw-r--r--   0        0        0      322 2022-08-29 09:33:05.137063 nbproject-0.8.6/tests/test_notebooks.py
+-rw-r--r--   0        0        0      303 2022-11-12 18:52:44.681259 nbproject-0.8.6/tests/test_set_version.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 nbproject-0.8.6/PKG-INFO
```

### Comparing `nbproject-0.8.5/.github/workflows/build.yml` & `nbproject-0.8.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/.github/workflows/latest-changes.yml` & `nbproject-0.8.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/.gitignore` & `nbproject-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/.pre-commit-config.yaml` & `nbproject-0.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/CITATION.cff` & `nbproject-0.8.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/LICENSE` & `nbproject-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/README.md` & `nbproject-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/changelog.md` & `nbproject-0.8.6/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Safer ipylab initialization | [263](https://github.com/laminlabs/nbproject/pull/263) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 | 0.8.6
 🐛 Fix VS Code integration for recent VS Code versions | [260](https://github.com/laminlabs/nbproject/pull/260) | [Koncopd](https://github.com/Koncopd) | 2023-04-17 | 0.8.5
 ♻️ Replace `display` with `metadata_only` arg in `header` | [257](https://github.com/laminlabs/nbproject/pull/257) | [Koncopd](https://github.com/Koncopd) | 2023-04-10 | 0.8.4
 🚸 Allow to not display metadata | [255](https://github.com/laminlabs/nbproject/pull/255) | [falexwolf](https://github.com/falexwolf) | 2023-03-12 | 0.8.3
 ⬆️ Observe `lndb-setup` rename to `lndb` | [253](https://github.com/laminlabs/nbproject/pull/253) | [bpenteado](https://github.com/bpenteado) | 2023-02-16 | 0.8.2
 ✨ Safer notebook path inference and more ways to do it | [251](https://github.com/laminlabs/nbproject/pull/251) | [Koncopd](https://github.com/Koncopd) | 2023-02-10 |
 🐛 Check keys before accessing in `notebook_path` | [250](https://github.com/laminlabs/nbproject/pull/250) | [Koncopd](https://github.com/Koncopd) | 2023-02-08 |
 :zap: Do nothing with ipylab when not in ipython | [247](https://github.com/laminlabs/nbproject/pull/247) | [Koncopd](https://github.com/Koncopd) | 2022-11-14 |
```

### Comparing `nbproject-0.8.5/docs/faq/example-after-init-set-filename.ipynb` & `nbproject-0.8.6/docs/faq/example-after-init-set-filename.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb` & `nbproject-0.8.6/docs/faq/example-project-uninitialized/2022-07-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/example-project/2022-05-13-my-task-x.ipynb` & `nbproject-0.8.6/docs/faq/example-project/2022-05-13-my-task-x.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/example-project/2022-07-18-my-task-y.ipynb` & `nbproject-0.8.6/docs/faq/example-project/2022-07-18-my-task-y.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/header-author-field.ipynb` & `nbproject-0.8.6/docs/faq/header-author-field.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/inconsistent-packages-parents-no-store.ipynb` & `nbproject-0.8.6/docs/faq/inconsistent-packages-parents-no-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/inconsistent-packages-parents-store.ipynb` & `nbproject-0.8.6/docs/faq/inconsistent-packages-parents-store.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/index.md` & `nbproject-0.8.6/docs/faq/index.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/initialize-set-env.ipynb` & `nbproject-0.8.6/docs/faq/initialize-set-env.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/initialize.ipynb` & `nbproject-0.8.6/docs/faq/initialize.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/internal-functions.ipynb` & `nbproject-0.8.6/docs/faq/internal-functions.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/not-initialized.ipynb` & `nbproject-0.8.6/docs/faq/not-initialized.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/publish-not-last-cell.ipynb` & `nbproject-0.8.6/docs/faq/publish-not-last-cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/publish-set-version.ipynb` & `nbproject-0.8.6/docs/faq/publish-set-version.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/publish-without-saving.ipynb` & `nbproject-0.8.6/docs/faq/publish-without-saving.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/publish-without-title.ipynb` & `nbproject-0.8.6/docs/faq/publish-without-title.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/publish-wrapper.ipynb` & `nbproject-0.8.6/docs/faq/publish-wrapper.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/set-env-via-environment-var.ipynb` & `nbproject-0.8.6/docs/faq/set-env-via-environment-var.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/setup.md` & `nbproject-0.8.6/docs/faq/setup.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/faq/trigger-exit-upon-init.ipynb` & `nbproject-0.8.6/docs/faq/trigger-exit-upon-init.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/guide/basic-metadata.ipynb` & `nbproject-0.8.6/docs/guide/basic-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/guide/cli.md` & `nbproject-0.8.6/docs/guide/cli.md`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/guide/meta.ipynb` & `nbproject-0.8.6/docs/guide/meta.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/guide/received.ipynb` & `nbproject-0.8.6/docs/guide/received.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/guide/update-metadata.ipynb` & `nbproject-0.8.6/docs/guide/update-metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/docs/quickstart.ipynb` & `nbproject-0.8.6/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/__main__.py` & `nbproject-0.8.6/nbproject/__main__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/_cli.py` & `nbproject-0.8.6/nbproject/_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/_header.py` & `nbproject-0.8.6/nbproject/_header.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/_meta.py` & `nbproject-0.8.6/nbproject/_meta.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/_publish.py` & `nbproject-0.8.6/nbproject/_publish.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/_schemas.py` & `nbproject-0.8.6/nbproject/_schemas.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/__init__.py` & `nbproject-0.8.6/nbproject/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_check_last_cell.py` & `nbproject-0.8.6/nbproject/dev/_check_last_cell.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_classic_nb_commands.py` & `nbproject-0.8.6/nbproject/dev/_classic_nb_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_consecutiveness.py` & `nbproject-0.8.6/nbproject/dev/_consecutiveness.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_frontend_commands.py` & `nbproject-0.8.6/nbproject/dev/_frontend_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_initialize.py` & `nbproject-0.8.6/nbproject/dev/_initialize.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_jupyter_communicate.py` & `nbproject-0.8.6/nbproject/dev/_jupyter_communicate.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_jupyter_lab_commands.py` & `nbproject-0.8.6/nbproject/dev/_jupyter_lab_commands.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_meta_live.py` & `nbproject-0.8.6/nbproject/dev/_meta_live.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_meta_store.py` & `nbproject-0.8.6/nbproject/dev/_meta_store.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_metadata_display.py` & `nbproject-0.8.6/nbproject/dev/_metadata_display.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_notebook.py` & `nbproject-0.8.6/nbproject/dev/_notebook.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_pypackage.py` & `nbproject-0.8.6/nbproject/dev/_pypackage.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/nbproject/dev/_set_version.py` & `nbproject-0.8.6/nbproject/dev/_set_version.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/noxfile.py` & `nbproject-0.8.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/pyproject.toml` & `nbproject-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/tests/conftest.py` & `nbproject-0.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/tests/test_cli.py` & `nbproject-0.8.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/tests/test_jupyter.py` & `nbproject-0.8.6/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `nbproject-0.8.5/PKG-INFO` & `nbproject-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbproject
-Version: 0.8.5
+Version: 0.8.6
 Summary: nbproject: Manage Jupyter notebooks.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

