# Comparing `tmp/tuxtrigger-0.6.4.tar.gz` & `tmp/tuxtrigger-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxtrigger-0.6.4.tar", last modified: Wed Feb 22 06:32:38 2023, max compression
+gzip compressed data, was "tuxtrigger-0.6.5.tar", last modified: Tue Apr 18 09:42:51 2023, max compression
```

## Comparing `tuxtrigger-0.6.4.tar` & `tuxtrigger-0.6.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0       81 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/.flake8
--rw-r--r--   0        0        0       95 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/.gitignore
--rw-r--r--   0        0        0     1082 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      427 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/Dockerfile
--rw-r--r--   0        0        0      135 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/Dockerfile.ci
--rw-r--r--   0        0        0      752 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/Dockerfile.ci-debian
--rw-r--r--   0        0        0      469 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/LICENSE
--rw-r--r--   0        0        0      458 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/Makefile
--rw-r--r--   0        0        0     2168 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/README.md
--rw-r--r--   0        0        0      151 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/debian/changelog
--rw-r--r--   0        0        0      961 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/debian/control
--rw-r--r--   0        0        0      100 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/debian/gbp.conf
--rwxr-xr-x   0        0        0      105 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/debian/rules
--rw-r--r--   0        0        0       12 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/debian/source/format
--rw-r--r--   0        0        0      635 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/docs/install-deb.md
--rw-r--r--   0        0        0      377 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/docs/install-pypi.md
--rw-r--r--   0        0        0      663 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/docs/install-rpm.md
--rw-r--r--   0        0        0      519 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/docs/run-uninstalled.md
--rw-r--r--   0        0        0     2099 2023-02-22 06:32:36.680173 tuxtrigger-0.6.4/docs/run.md
--rw-r--r--   0        0        0     3394 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/docs/subcommands.md
--rw-r--r--   0        0        0      774 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/mkdocs.yml
--rw-r--r--   0        0        0       36 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/mypy.ini
--rw-r--r--   0        0        0      510 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/pyproject.toml
--rw-r--r--   0        0        0       50 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/requirements-dev.txt
--rw-r--r--   0        0        0       28 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/requirements.txt
--rwxr-xr-x   0        0        0      125 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/run
--rwxr-xr-x   0        0        0      166 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/scripts/readme2index.sh
--rw-r--r--   0        0        0       75 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/__init__.py
--rw-r--r--   0        0        0     1362 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/conftest.py
--rw-r--r--   0        0        0      650 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_argparser.py
--rw-r--r--   0        0        0     8265 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_builder.py
--rw-r--r--   0        0        0      678 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_exceptions.py
--rw-r--r--   0        0        0      292 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/error_path.yaml
--rw-r--r--   0        0        0      491 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/gitsha.yaml
--rw-r--r--   0        0        0      379 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/gitsha2.yaml
--rw-r--r--   0        0        0      656 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/happy_path.yaml
--rw-r--r--   0        0        0    82080 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/manifest.js.gz
--rw-r--r--   0        0        0      125 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/planTest.yaml
--rw-r--r--   0        0        0      163 2023-02-22 06:32:36.681173 tuxtrigger-0.6.4/test/test_files/test.json
--rw-r--r--   0        0        0    11837 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/test/test_main.py
--rw-r--r--   0        0        0     2724 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/test/test_manifest.py
--rw-r--r--   0        0        0     1983 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/test/test_request.py
--rw-r--r--   0        0        0     7121 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/test/test_yamlload.py
--rw-r--r--   0        0        0     1579 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger.spec
--rw-r--r--   0        0        0      134 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/__init__.py
--rw-r--r--   0        0        0     7746 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/__main__.py
--rw-r--r--   0        0        0     2401 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/argparser.py
--rw-r--r--   0        0        0    11178 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/builder.py
--rw-r--r--   0        0        0      454 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/exceptions.py
--rw-r--r--   0        0        0      729 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/inputvalidation.py
--rw-r--r--   0        0        0     2275 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/manifest.py
--rw-r--r--   0        0        0      890 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/request.py
--rw-r--r--   0        0        0     5699 2023-02-22 06:32:36.682173 tuxtrigger-0.6.4/tuxtrigger/yamlload.py
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 tuxtrigger-0.6.4/setup.py
--rw-r--r--   0        0        0      190 1970-01-01 00:00:00.000000 tuxtrigger-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/.flake8
+-rw-r--r--   0        0        0       95 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1082 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      427 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/Dockerfile
+-rw-r--r--   0        0        0      135 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/Dockerfile.ci
+-rw-r--r--   0        0        0      752 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      469 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/LICENSE
+-rw-r--r--   0        0        0      458 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/Makefile
+-rw-r--r--   0        0        0     2168 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/README.md
+-rw-r--r--   0        0        0      151 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/debian/changelog
+-rw-r--r--   0        0        0      961 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/debian/control
+-rw-r--r--   0        0        0      100 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/debian/gbp.conf
+-rwxr-xr-x   0        0        0      105 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/debian/rules
+-rw-r--r--   0        0        0       12 2023-04-18 09:42:49.148705 tuxtrigger-0.6.5/debian/source/format
+-rw-r--r--   0        0        0      635 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/install-deb.md
+-rw-r--r--   0        0        0      377 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/install-pypi.md
+-rw-r--r--   0        0        0      663 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/install-rpm.md
+-rw-r--r--   0        0        0      519 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/run-uninstalled.md
+-rw-r--r--   0        0        0     2099 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/run.md
+-rw-r--r--   0        0        0     3394 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/docs/subcommands.md
+-rw-r--r--   0        0        0      774 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/mkdocs.yml
+-rw-r--r--   0        0        0       36 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/mypy.ini
+-rw-r--r--   0        0        0      510 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/requirements-dev.txt
+-rw-r--r--   0        0        0       28 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/requirements.txt
+-rwxr-xr-x   0        0        0      125 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/run
+-rwxr-xr-x   0        0        0      166 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/scripts/readme2index.sh
+-rw-r--r--   0        0        0       75 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/conftest.py
+-rw-r--r--   0        0        0      650 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_argparser.py
+-rw-r--r--   0        0        0     8265 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_builder.py
+-rw-r--r--   0        0        0      678 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_exceptions.py
+-rw-r--r--   0        0        0      292 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_files/error_path.yaml
+-rw-r--r--   0        0        0      491 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_files/gitsha.yaml
+-rw-r--r--   0        0        0      379 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_files/gitsha2.yaml
+-rw-r--r--   0        0        0      656 2023-04-18 09:42:49.149705 tuxtrigger-0.6.5/test/test_files/happy_path.yaml
+-rw-r--r--   0        0        0    82080 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_files/manifest.js.gz
+-rw-r--r--   0        0        0      125 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_files/planTest.yaml
+-rw-r--r--   0        0        0      163 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_files/test.json
+-rw-r--r--   0        0        0    12215 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_main.py
+-rw-r--r--   0        0        0     2724 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_manifest.py
+-rw-r--r--   0        0        0     1983 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_request.py
+-rw-r--r--   0        0        0     7121 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/test/test_yamlload.py
+-rw-r--r--   0        0        0     1579 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger.spec
+-rw-r--r--   0        0        0      134 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/__init__.py
+-rw-r--r--   0        0        0     7772 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/__main__.py
+-rw-r--r--   0        0        0     2401 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/argparser.py
+-rw-r--r--   0        0        0    11178 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/builder.py
+-rw-r--r--   0        0        0      454 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/exceptions.py
+-rw-r--r--   0        0        0      728 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/inputvalidation.py
+-rw-r--r--   0        0        0     2275 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/manifest.py
+-rw-r--r--   0        0        0      890 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/request.py
+-rw-r--r--   0        0        0     5699 2023-04-18 09:42:49.150705 tuxtrigger-0.6.5/tuxtrigger/yamlload.py
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 tuxtrigger-0.6.5/setup.py
+-rw-r--r--   0        0        0      190 1970-01-01 00:00:00.000000 tuxtrigger-0.6.5/PKG-INFO
```

### Comparing `tuxtrigger-0.6.4/.gitlab-ci.yml` & `tuxtrigger-0.6.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/Dockerfile.ci-debian` & `tuxtrigger-0.6.5/Dockerfile.ci-debian`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/LICENSE` & `tuxtrigger-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/README.md` & `tuxtrigger-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/debian/control` & `tuxtrigger-0.6.5/debian/control`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/docs/install-deb.md` & `tuxtrigger-0.6.5/docs/install-deb.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/docs/install-rpm.md` & `tuxtrigger-0.6.5/docs/install-rpm.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/docs/run-uninstalled.md` & `tuxtrigger-0.6.5/docs/run-uninstalled.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/docs/run.md` & `tuxtrigger-0.6.5/docs/run.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/docs/subcommands.md` & `tuxtrigger-0.6.5/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/mkdocs.yml` & `tuxtrigger-0.6.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/conftest.py` & `tuxtrigger-0.6.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_argparser.py` & `tuxtrigger-0.6.5/test/test_argparser.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_builder.py` & `tuxtrigger-0.6.5/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_exceptions.py` & `tuxtrigger-0.6.5/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_files/happy_path.yaml` & `tuxtrigger-0.6.5/test/test_files/happy_path.yaml`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_files/manifest.js.gz` & `tuxtrigger-0.6.5/test/test_files/manifest.js.gz`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_main.py` & `tuxtrigger-0.6.5/test/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,15 +164,26 @@
         main_check_squad_project.assert_called()
         main_lsremote.assert_called()
         main_build_uid.assert_called()
         main_compare_squad_sha.assert_called()
         main_build_output.assert_called()
         main_squad_metadata_request.assert_called()
         main_tux_console_plan.assert_called()
-        main_update_squad_metadata.assert_called()
+        main_update_squad_metadata.assert_called_with(
+            {
+                "empty": "no_real_values",
+                "uid": "1234",
+                "git_repo": "https://gitlab.com/no_real_repo",
+                "git_ref": "master",
+                "git_describe": "v5.19-rc7",
+            },
+            "~non.existing",
+            "example_project",
+            "2c8d80ee6d795dc6951bbdef466ef19c64ff717d",
+        )
         exit.assert_called_with(0)
 
     def test_main_correct_data_yaml(self, argv, monkeypatch, mocker):
         argv.extend([f"{BASE}/test/test_files/happy_path.yaml"])
         argv.append("--sha-compare=yaml")
         monkeypatch.setattr(main_module, "__name__", "__main__")
         main_create_dynamic_configuration = mocker.patch(
```

### Comparing `tuxtrigger-0.6.4/test/test_manifest.py` & `tuxtrigger-0.6.5/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_request.py` & `tuxtrigger-0.6.5/test/test_request.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/test/test_yamlload.py` & `tuxtrigger-0.6.5/test/test_yamlload.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/tuxtrigger.spec` & `tuxtrigger-0.6.5/tuxtrigger.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxtrigger
-Version:   0.6.4
+Version:   0.6.5
 Release:   0%{?dist}
 Summary:   FIXME
 License:   MIT
 URL:       https://tuxsuite.org/
 Source0:   %{pypi_source}
```

### Comparing `tuxtrigger-0.6.4/tuxtrigger/__main__.py` & `tuxtrigger-0.6.5/tuxtrigger/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,17 +196,17 @@
                             squad_config[uid][2],
                             json_save,
                             squad_config[uid][3],
                         )
                     if options.sha_compare == "squad":
                         update_squad_metadata(
                             json_build_output,
-                            group_name,
-                            squad_project,
-                            fingerprint,
+                            squad_config[uid][1],
+                            squad_config[uid][2],
+                            squad_config[uid][3],
                         )
                     uid_queue.remove(uid)
         LOG.info("** Submiting Plans Phase Completed **")
         if options.sha_compare == "yaml":
             yaml_file_write(output_data, output_file)
             LOG.info("** SHA List Updated **")
     else:
```

### Comparing `tuxtrigger-0.6.4/tuxtrigger/argparser.py` & `tuxtrigger-0.6.5/tuxtrigger/argparser.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/tuxtrigger/builder.py` & `tuxtrigger-0.6.5/tuxtrigger/builder.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/tuxtrigger/inputvalidation.py` & `tuxtrigger-0.6.5/tuxtrigger/inputvalidation.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     def url_path(self):
         return urlparse(self.url.rstrip("/"))
 
 
 @dataclass
 class YamlValidator(Base):
-
     url: str
     squad_group: str
     branches: List[Dict]
     regex: Optional[str] = None
     default_plan: Optional[str] = None
     squad_project_prefix: Optional[str] = None
```

### Comparing `tuxtrigger-0.6.4/tuxtrigger/manifest.py` & `tuxtrigger-0.6.5/tuxtrigger/manifest.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/tuxtrigger/request.py` & `tuxtrigger-0.6.5/tuxtrigger/request.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/tuxtrigger/yamlload.py` & `tuxtrigger-0.6.5/tuxtrigger/yamlload.py`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.6.4/setup.py` & `tuxtrigger-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['tuxsuite', 'squad-client', 'jinja2', 'requests', 'PyYAML']
 
 entry_points = \
 {'console_scripts': ['tuxtrigger = tuxtrigger.__main__:main']}
 
 setup(name='tuxtrigger',
-      version='0.6.4',
+      version='0.6.5',
       description='TuxTrigger Project by Linaro',
       author='Pawel Szymaszek',
       author_email='pawel.szymaszek@linaro.org',
       url='https://tuxsuite.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

