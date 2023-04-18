# Comparing `tmp/cloudformation-cli-java-plugin-2.0.8.tar.gz` & `tmp/cloudformation-cli-java-plugin-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudformation-cli-java-plugin-2.0.8.tar", last modified: Mon Dec 13 20:01:50 2021, max compression
+gzip compressed data, was "cloudformation-cli-java-plugin-2.0.9.tar", last modified: Wed Dec 15 18:16:02 2021, max compression
```

## Comparing `cloudformation-cli-java-plugin-2.0.8.tar` & `cloudformation-cli-java-plugin-2.0.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.774118 cloudformation-cli-java-plugin-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-12-13 20:01:50.774118 cloudformation-cli-java-plugin-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3634 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.766118 cloudformation-cli-java-plugin-2.0.8/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.766118 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 20:01:50.000000 cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.766118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.770118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22995 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.770118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.770118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/build-image-src/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/build-image-src/Dockerfile-java11
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/build-image-src/Dockerfile-java8
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/java.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/jsonSchemas.xml
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/log4j2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.766118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.770118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/
--rw-r--r--   0 runner    (1001) docker     (121)      782 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/BaseConfiguration.java
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/BaseHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     9127 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/HandlerWrapper.java
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/POJO.java
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/ResourceModel.java
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.766118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.770118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubHandlerTest.java
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubListHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubListHandlerTest.java
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.774118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/AbstractTestBase.java
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/BaseHandlerStd.java
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/ClientBuilder.java
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/ResourceModel.java
--rw-r--r--   0 runner    (1001) docker     (121)     6949 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubCreateHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubDeleteHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubHandlerTest.java
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubListHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubListHandlerTest.java
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubReadHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)     8291 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubUpdateHandler.java
--rw-r--r--   0 runner    (1001) docker     (121)    10115 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/TagHelper.java
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/Translator.java
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 20:01:50.774118 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/CallbackContext.java
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/StubConfiguration.java
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/lombok.config
--rw-r--r--   0 runner    (1001) docker     (121)     9170 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/pom.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2021-12-13 20:01:50.774118 cloudformation-cli-java-plugin-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-12-13 20:01:41.000000 cloudformation-cli-java-plugin-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.447286 cloudformation-cli-java-plugin-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-12-15 18:16:02.447286 cloudformation-cli-java-plugin-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3634 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.435286 cloudformation-cli-java-plugin-2.0.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5307 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 18:16:02.000000 cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.435286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22995 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/build-image-src/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/build-image-src/Dockerfile-java11
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/build-image-src/Dockerfile-java8
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/java.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/jsonSchemas.xml
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/log4j2.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.443286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/BaseConfiguration.java
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/BaseHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     9127 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/HandlerWrapper.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/POJO.java
+-rw-r--r--   0 runner    (1001) docker     (121)     4334 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/ResourceModel.java
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.439286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.443286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubHandlerTest.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubListHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubListHandlerTest.java
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.443286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/AbstractTestBase.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/BaseHandlerStd.java
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/ClientBuilder.java
+-rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/ResourceModel.java
+-rw-r--r--   0 runner    (1001) docker     (121)     6949 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubCreateHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubDeleteHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubHandlerTest.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubListHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubListHandlerTest.java
+-rw-r--r--   0 runner    (1001) docker     (121)     3714 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubReadHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)     8291 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubUpdateHandler.java
+-rw-r--r--   0 runner    (1001) docker     (121)    10115 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/TagHelper.java
+-rw-r--r--   0 runner    (1001) docker     (121)     6407 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/Translator.java
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 18:16:02.447286 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/CallbackContext.java
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/StubConfiguration.java
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/lombok.config
+-rw-r--r--   0 runner    (1001) docker     (121)     9170 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/pom.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2021-12-15 18:16:02.447286 cloudformation-cli-java-plugin-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-12-15 18:15:53.000000 cloudformation-cli-java-plugin-2.0.9/setup.py
```

### Comparing `cloudformation-cli-java-plugin-2.0.8/LICENSE` & `cloudformation-cli-java-plugin-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/PKG-INFO` & `cloudformation-cli-java-plugin-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-java-plugin
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-java-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Description: ## AWS CloudFormation Resource Provider Java Plugin
```

### Comparing `cloudformation-cli-java-plugin-2.0.8/README.md` & `cloudformation-cli-java-plugin-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/PKG-INFO` & `cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-java-plugin
-Version: 2.0.8
+Version: 2.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-java-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Description: ## AWS CloudFormation Resource Provider Java Plugin
```

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/cloudformation_cli_java_plugin.egg-info/SOURCES.txt` & `cloudformation-cli-java-plugin-2.0.9/python/cloudformation_cli_java_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/codegen.py` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/codegen.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/jsonSchemas.xml` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/jsonSchemas.xml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/data/log4j2.xml` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/data/log4j2.xml`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/resolver.py` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/resolver.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/BaseConfiguration.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/BaseConfiguration.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/BaseHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/BaseHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/HandlerWrapper.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/HandlerWrapper.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/POJO.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/POJO.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/generate/ResourceModel.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/generate/ResourceModel.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubHandlerTest.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubHandlerTest.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubListHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubListHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/default/StubListHandlerTest.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/default/StubListHandlerTest.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/AbstractTestBase.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/AbstractTestBase.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/BaseHandlerStd.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/BaseHandlerStd.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/ClientBuilder.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/ClientBuilder.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/ResourceModel.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/ResourceModel.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubCreateHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubCreateHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubDeleteHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubDeleteHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubHandlerTest.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubHandlerTest.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubListHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubListHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubListHandlerTest.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubListHandlerTest.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubReadHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubReadHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/StubUpdateHandler.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/StubUpdateHandler.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/TagHelper.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/TagHelper.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/guided_aws/Translator.java` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/guided_aws/Translator.java`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/README.md` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/README.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/pom.xml` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/pom.xml`

 * *Files 1% similar despite different names*

#### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/templates/init/shared/pom.xml` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/templates/init/shared/pom.xml`

```diff
@@ -26,21 +26,21 @@
       <version>1.18.4</version>
       <scope>provided</scope>
     </dependency>
     <!-- https://mvnrepository.com/artifact/org.apache.logging.log4j/log4j-api -->
     <dependency>
       <groupId>org.apache.logging.log4j</groupId>
       <artifactId>log4j-api</artifactId>
-      <version>2.15.0</version>
+      <version>2.16.0</version>
     </dependency>
     <!-- https://mvnrepository.com/artifact/org.apache.logging.log4j/log4j-core -->
     <dependency>
       <groupId>org.apache.logging.log4j</groupId>
       <artifactId>log4j-core</artifactId>
-      <version>2.15.0</version>
+      <version>2.16.0</version>
     </dependency>
     <!-- https://mvnrepository.com/artifact/org.apache.logging.log4j/log4j-slf4j-impl -->
     <dependency>
       <groupId>org.apache.logging.log4j</groupId>
       <artifactId>log4j-slf4j-impl</artifactId>
       <version>2.13.3</version>
     </dependency>
```

### Comparing `cloudformation-cli-java-plugin-2.0.8/python/rpdk/java/utils.py` & `cloudformation-cli-java-plugin-2.0.9/python/rpdk/java/utils.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/setup.cfg` & `cloudformation-cli-java-plugin-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-java-plugin-2.0.8/setup.py` & `cloudformation-cli-java-plugin-2.0.9/setup.py`

 * *Files identical despite different names*

