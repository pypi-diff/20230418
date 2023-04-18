# Comparing `tmp/dsp_tools-2.2.0.tar.gz` & `tmp/dsp_tools-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.2.0.tar", max compression
+gzip compressed data, was "dsp_tools-2.2.1.tar", max compression
```

## Comparing `dsp_tools-2.2.0.tar` & `dsp_tools-2.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    35149 2023-03-22 08:39:57.748322 dsp_tools-2.2.0/LICENSE
--rw-r--r--   0        0        0     4358 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/docs/index.md
--rw-r--r--   0        0        0     2798 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    15536 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    81051 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      963 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     9310 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0      734 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     9455 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16931 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     9709 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    23033 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      506 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    19734 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2973 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    19103 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1930 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    20992 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1896 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    21923 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    34104 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      419 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0     1293 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    27204 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    34694 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     2153 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      747 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0      254 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlerror.py
--rw-r--r--   0        0        0     1841 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2371 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8874 2023-03-22 08:39:57.768322 dsp_tools-2.2.0/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2614 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0     1488 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23019 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2664 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15031 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4865 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     6830 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0     9106 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3184 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0    40633 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     7686 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4513 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    16570 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4164 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    12067 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6611 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    49312 2023-03-22 08:39:57.772322 dsp_tools-2.2.0/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5697 1970-01-01 00:00:00.000000 dsp_tools-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 13:44:56.402144 dsp_tools-2.2.1/LICENSE
+-rw-r--r--   0        0        0     4349 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/docs/index.md
+-rw-r--r--   0        0        0     2894 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    15548 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    81068 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      962 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     9310 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0      734 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     9454 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16923 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     9702 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    23026 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      506 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    19726 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2972 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    19102 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1930 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    20984 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1896 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    22008 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    34116 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      419 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0     1295 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    27204 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    34694 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     2153 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      747 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0      254 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlerror.py
+-rw-r--r--   0        0        0     1841 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2371 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8874 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2614 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0     1488 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23019 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-04-18 13:44:56.418144 dsp_tools-2.2.1/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0     2664 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0        0 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15024 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4865 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     7607 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0     9873 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3185 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0    41414 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8068 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4521 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18755 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4164 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    12087 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0     6633 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    49615 2023-04-18 13:44:56.422144 dsp_tools-2.2.1/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5688 1970-01-01 00:00:00.000000 dsp_tools-2.2.1/PKG-INFO
```

### Comparing `dsp_tools-2.2.0/LICENSE` & `dsp_tools-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/docs/index.md` & `dsp_tools-2.2.1/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
 
 # DSP-TOOLS documentation
 
-DSP-TOOLS is a Python package with a command line interface that helps you interact with a DSP server. A DSP server 
-is a remote server or a local machine where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on. 
+DSP-TOOLS is a Python package with a command line interface 
+that helps you interact with a DSP server. 
+A DSP server is a remote server or a local machine 
+where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on. 
 
 To install the latest version, run:
 
 ```bash
 pip3 install dsp-tools
 ```
 
@@ -16,22 +18,26 @@
 ```bash
 pip3 install --upgrade dsp-tools
 ```
 
 The two main tasks that DSP-TOOLS serves for are:
 
 - **Create a project with its data model(s), described in a JSON file, on a DSP server**  
-  In order to archive your data on the DaSCH Service Platform, you need a data model that describes your data.
-  The data model is defined in a JSON project definition file which has to be transmitted to the DSP server. If the DSP 
-  server is aware of the data model for your project, conforming data can be uploaded into the DSP repository.
+  In order to archive your data on the DaSCH Service Platform, 
+  you need a data model that describes your data.
+  The data model is defined in a JSON project definition file 
+  which has to be transmitted to the DSP server. 
+  If the DSP server is aware of the data model for your project, 
+  conforming data can be uploaded into the DSP repository.
 - **Upload data, described in an XML file, to a DSP server that has a project with a matching data model**  
-  Sometimes, data is added in large quantities. Therefore, DSP-TOOLS allows you to perform bulk imports of your
-  data. In order to do so, the data has to be described in an XML file. DSP-TOOLS is able to read the XML file and 
-  upload
-  all data to the DSP server.
+  Sometimes, data is added in large quantities. 
+  Therefore, DSP-TOOLS allows you to perform bulk imports of your data.
+  In order to do so, the data has to be described in an XML file. 
+  DSP-TOOLS is able to read the XML file 
+  and upload all data to the DSP server.
 
 All functionalities of DSP-TOOLS revolve around these two basic tasks. 
 
 DSP-TOOLS provides the following functionalities:
 
 - [`dsp-tools create`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#create) 
   creates the project with its data model(s) on a DSP server from a JSON file.
@@ -39,26 +45,26 @@
   reads a project with its data model(s) from 
   a DSP server and writes it into a JSON file.
 - [`dsp-tools xmlupload`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#xmlupload) 
   uploads data from an XML file (bulk data import)
   and writes the mapping from internal IDs to IRIs into a local file.
 - [`dsp-tools excel2json`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2json) 
   creates an entire JSON project file from a folder with Excel files in it.
-    - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
-      creates the "lists" section of a JSON project file from one or several Excel files. 
-      The resulting section can be integrated into a JSON project file
-      and then be uploaded to a DSP server with `dsp-tools create`.
-    - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
-      creates the "resources" section of a JSON project file from an Excel file. 
-      The resulting section can be integrated into a JSON project file 
-      and then be uploaded to a DSP server with `dsp-tools create`.
-    - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
-      creates the "properties" section of a JSON project file from an Excel file. 
-      The resulting section can be integrated into a JSON project file 
-      and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
+    creates the "lists" section of a JSON project file from one or several Excel files. 
+    The resulting section can be integrated into a JSON project file
+    and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
+    creates the "resources" section of a JSON project file from an Excel file. 
+    The resulting section can be integrated into a JSON project file 
+    and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
+    creates the "properties" section of a JSON project file from an Excel file. 
+    The resulting section can be integrated into a JSON project file 
+    and then be uploaded to a DSP server with `dsp-tools create`.
 - [`dsp-tools excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2xml) 
   transforms a data source to XML 
   if it is already structured according to the DSP specifications.
 - [The module `excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/excel2xml-module) 
   provides helper methods that can be used in a Python script 
   to convert data from a tabular format into XML.
 - [`dsp-tools id2iri`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#id2iri)
```

### Comparing `dsp_tools-2.2.0/pyproject.toml` & `dsp_tools-2.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.2.0"
+version = "2.2.1"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -41,14 +41,15 @@
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.11"
 mkdocs-include-markdown-plugin = "^4.0.3"
 mypy = "^0.991"
 autopep8 = "^2.0.1"
 pytest = "^7.2.0"
 types-requests = "^2.28.11.7"
+types-lxml = "^2023.3.28"
 
 
 [tool.poetry.scripts]
 # definition of the entry point
 dsp-tools = "dsp_tools.dsp_tools:main"
 
 
@@ -83,7 +84,11 @@
 
 
 [tool.mypy]
 ignore_missing_imports = true
 follow_imports = "silent"
 show_column_numbers = true
 strict = true
+
+[tool.isort]
+multi_line_output = 3
+known_first_party = ["dsp_tools"]
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.2.1/src/dsp_tools/dsp_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """
 The code in this file handles the arguments passed by the user from the command line and calls the requested actions.
 """
 import argparse
 import datetime
 import logging
 import logging.handlers
-from pathlib import Path
 import sys
 from importlib.metadata import version
+from pathlib import Path
 
 from dsp_tools.excel2xml import excel2xml
 from dsp_tools.models.exceptions import UserError
-from dsp_tools.utils.excel_to_json_lists import excel2lists, validate_lists_section_with_schema
+from dsp_tools.utils.excel_to_json_lists import (
+    excel2lists,
+    validate_lists_section_with_schema
+)
 from dsp_tools.utils.excel_to_json_project import excel2json
 from dsp_tools.utils.excel_to_json_properties import excel2properties
 from dsp_tools.utils.excel_to_json_resources import excel2resources
+from dsp_tools.utils.generate_templates import generate_template_repo
 from dsp_tools.utils.id_to_iri import id_to_iri
-from dsp_tools.utils.project_create_lists import create_lists
 from dsp_tools.utils.project_create import create_project
+from dsp_tools.utils.project_create_lists import create_lists
 from dsp_tools.utils.project_get import get_project
 from dsp_tools.utils.project_validate import validate_project
+from dsp_tools.utils.rosetta import upload_rosetta
 from dsp_tools.utils.shared import validate_xml_against_schema
 from dsp_tools.utils.stack_handling import start_stack, stop_stack
 from dsp_tools.utils.xml_upload import xml_upload
-from dsp_tools.utils.generate_templates import generate_template_repo
-from dsp_tools.utils.rosetta import upload_rosetta
 
 
 def make_parser() -> argparse.ArgumentParser:
     """
     Create a parser for the command line arguments
 
     Returns:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/excel2xml.py` & `dsp_tools-2.2.1/src/dsp_tools/excel2xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 import dataclasses
 import datetime
 import difflib
 import json
 import os
 import re
 import uuid
@@ -15,15 +16,19 @@
 from lxml import etree
 from lxml.builder import E
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import DateTimeStamp
 from dsp_tools.models.propertyelement import PropertyElement
 from dsp_tools.models.value import UriValue
-from dsp_tools.utils.shared import simplify_name, check_notna, validate_xml_against_schema
+from dsp_tools.utils.shared import (
+    check_notna,
+    simplify_name,
+    validate_xml_against_schema
+)
 
 xml_namespace_map = {
     None: "https://dasch.swiss/schema",
     "xsi": "http://www.w3.org/2001/XMLSchema-instance"
 }
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.2.1/src/dsp_tools/models/bitstream.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import Optional, Any
-
+from typing import Any, Optional
 
 from dsp_tools.models.helpers import Actions
 from dsp_tools.models.permission import Permissions
 
 
 class Bitstream:
     """
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/connection.py` & `dsp_tools-2.2.1/src/dsp_tools/models/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import re
-from typing import Optional, Union, Any
+from typing import Any, Optional, Union
 
 import requests
 
 from dsp_tools.models.exceptions import BaseError
 
 
 class Connection:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.2.1/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/group.py` & `dsp_tools-2.2.1/src/dsp_tools/models/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import json
-from typing import Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
-from dsp_tools.models.langstring import LangString
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions
+from dsp_tools.models.langstring import LangString
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 
 """
 This module implements the handling (CRUD) of Knora groups.
 
 CREATE:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/helpers.py` & `dsp_tools-2.2.1/src/dsp_tools/models/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import sys
 from dataclasses import dataclass
 from enum import Enum, unique
-from typing import NewType, Optional, Any, Tuple, Union, Pattern
-
+from typing import Any, NewType, Optional, Pattern, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 #
 # here we do some data typing that should help
 #
 
@@ -63,15 +62,15 @@
     _index: int
 
     def __init__(self, context: 'Context'):
         self._context = context
         self._prefixes = [x for x in self._context.context]
         self._index = 0
 
-    def __next__(self) -> Tuple[Optional[str], Optional[OntoIri]]:
+    def __next__(self) -> tuple[Optional[str], Optional[OntoIri]]:
         if len(self._context.context) == 0 and self._index == 0:
             return None, None
         elif self._index < len(self._context.context):
             tmp = self._prefixes[self._index]
             self._index += 1
             return tmp, self._context.context[tmp]
         else:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/langstring.py` & `dsp_tools-2.2.1/src/dsp_tools/models/langstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum, unique
-from typing import Tuple, Optional, Any, Union
+from typing import Any, Optional, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 
 @unique
 class Languages(Enum):
     EN = 'en'
@@ -55,15 +55,15 @@
     ```
     """
     _langstrs: dict[Languages, str]
     _simplestring: str
 
     def __init__(self, initvalue: LangStringParam = None):
 
-        def mymapper(p: Tuple[Union[Languages, str], str]) -> Tuple[Languages, str]:
+        def mymapper(p: tuple[Union[Languages, str], str]) -> tuple[Languages, str]:
             lmap = dict(map(lambda a: (a.value, a), Languages))
             if isinstance(p[0], str) and p[0] in lmap:
                 lang = lmap[p[0].lower()]
             elif isinstance(p[0], Languages):
                 lang = p[0]
             else:
                 raise BaseError("Not a valid language definition!")
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/listnode.py` & `dsp_tools-2.2.1/src/dsp_tools/models/listnode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 from pprint import pprint
-from typing import List, Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
-from dsp_tools.models.set_encoder import SetEncoder
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.langstring import Languages, LangString
+from dsp_tools.models.helpers import Actions
+from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
+from dsp_tools.models.set_encoder import SetEncoder
 
 """
 This module implements the handling (CRUD) of list nodes and adds some function to read whole lists.
 
 CREATE:
     * Instantiate a new object of the class ListNode
     * Call the ``create`` method on the instance
@@ -186,15 +185,15 @@
         self._name = str(name) if name else None
         if parent and isinstance(parent, ListNode):
             self._parent = parent.id
         else:
             self._parent = str(parent) if parent else None
         self._isRootNode = isRootNode
         if children:
-            if isinstance(children, List) and len(children) > 0 and isinstance(children[0], ListNode):
+            if isinstance(children, list) and len(children) > 0 and isinstance(children[0], ListNode):
                 self._children = children
             else:
                 raise BaseError('ERROR Children must be list of ListNodes!')
         else:
             self._children = None
         if not isinstance(rootNodeIri, str) and rootNodeIri:
             raise BaseError('ERROR rootNodeIri must be of type string')
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/ontology.py` & `dsp_tools-2.2.1/src/dsp_tools/models/ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import copy
 import json
 import re
-from typing import Tuple, Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 from dsp_tools.models.propertyclass import PropertyClass
 from dsp_tools.models.resourceclass import ResourceClass
 from dsp_tools.models.set_encoder import SetEncoder
 
 """
@@ -143,15 +142,15 @@
     def resource_classes(self) -> list[ResourceClass]:
         return self._resource_classes
 
     @resource_classes.setter
     def resource_classes(self, value: list[ResourceClass]) -> None:
         self._resource_classes = value
 
-    def addResourceClass(self, resourceclass: ResourceClass, create: bool = False) -> Tuple[int, ResourceClass]:
+    def addResourceClass(self, resourceclass: ResourceClass, create: bool = False) -> tuple[int, ResourceClass]:
         if create:
             print('Calling resourceclass.create in Ontology.addResourceClass')
             lmd, resourceclass = resourceclass.create(self._lastModificationDate)
             self._lastModificationDate = lmd
         self._resource_classes.append(resourceclass)
         index = len(self._resource_classes) - 1
         return index, resourceclass
@@ -172,15 +171,15 @@
     def property_classes(self) -> list[PropertyClass]:
         return self._property_classes
 
     @property_classes.setter
     def property_classes(self, value: list[PropertyClass]):
         self._property_classes = value
 
-    def addPropertyClass(self, propclass: PropertyClass, create: bool = False) -> Tuple[int, ResourceClass]:
+    def addPropertyClass(self, propclass: PropertyClass, create: bool = False) -> tuple[int, ResourceClass]:
         if create:
             lmd, resourceclass = propclass.create(self._lastModificationDate)
             self._lastModificationDate = lmd
         self._property_classes.append(resourceclass)
         index = len(self._property_classes) - 1
         return index, propclass
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/permission.py` & `dsp_tools-2.2.1/src/dsp_tools/models/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from enum import Enum, unique
 from typing import Optional, Union
 
 
-
 @unique
 class PermissionValue(Enum):
     RV = 1
     V = 2
     M = 4
     D = 8
     CR = 16
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/project.py` & `dsp_tools-2.2.1/src/dsp_tools/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import json
 from pprint import pprint
-from typing import Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
-from dsp_tools.models.set_encoder import SetEncoder
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.langstring import Languages, LangString
+from dsp_tools.models.helpers import Actions
+from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
+from dsp_tools.models.set_encoder import SetEncoder
 
 """
 This module implements the handling (CRUD) of Knora projects.
 
 CREATE:
     * Instantiate a new object of the class Project with all required parameters
     * Call the ``create``-method on the instance
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.2.1/src/dsp_tools/models/projectContext.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.group import Group
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.group import Group
 from dsp_tools.models.project import Project
 
 
 class ProjectContext:
     """Represents the project context"""
 
     _projects: list[Project]
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.2.1/src/dsp_tools/models/propertyclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 import re
-from typing import Tuple, Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
-from dsp_tools.models.set_encoder import SetEncoder
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.langstring import Languages, LangString
+from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
+from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.model import Model
+from dsp_tools.models.set_encoder import SetEncoder
 
 
 class PropertyClass(Model):
     ROUTE: str = "/v2/ontologies/properties"
 
     _context: Context
     _id: str
@@ -376,22 +375,22 @@
                     tmp['@graph'][0]['rdfs:label'] = self._label.toJsonLdObj()
             if what == 'comment':
                 if not self._comment.isEmpty() and 'comment' in self._changed:
                     tmp['@graph'][0]['rdfs:comment'] = self._comment.toJsonLdObj()
 
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'PropertyClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'PropertyClass']:
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=2)
         result = self._con.post(PropertyClass.ROUTE, jsondata)
         last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
         return last_modification_date, PropertyClass.fromJsonObj(self._con, self._context, result['@graph'])
 
-    def update(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
         #
         # Note: Knora is able to change only one thing per call, either label or comment!
         #
         result = None
         something_changed = False
         if 'label' in self._changed:
             jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'label')
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.2.1/src/dsp_tools/models/propertyelement.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Union, Optional
+from typing import Optional, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 
 @dataclass(frozen=True)
 class PropertyElement:
     """
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/resource.py` & `dsp_tools-2.2.1/src/dsp_tools/models/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 import json
 import re
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Optional, Any, Union, Type
+from typing import Any, Optional, Type, Union
 from urllib.parse import quote_plus
 
-
 from dsp_tools.models.bitstream import Bitstream
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import OntoIri, Actions, Cardinality, Context, DateTimeStamp
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import (
+    Actions,
+    Cardinality,
+    Context,
+    DateTimeStamp,
+    OntoIri
+)
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.model import Model
 from dsp_tools.models.ontology import Ontology
-from dsp_tools.models.permission import PermissionValue, Permissions
+from dsp_tools.models.permission import Permissions, PermissionValue
 from dsp_tools.models.project import Project
 from dsp_tools.models.resourceclass import HasProperty
-from dsp_tools.models.value import KnoraStandoffXml, Value, TextValue, ColorValue, DateValue, DecimalValue, GeomValue, GeonameValue, \
-    IntValue, BooleanValue, UriValue, TimeValue, IntervalValue, ListValue, LinkValue, fromJsonLdObj
+from dsp_tools.models.value import (
+    BooleanValue,
+    ColorValue,
+    DateValue,
+    DecimalValue,
+    GeomValue,
+    GeonameValue,
+    IntervalValue,
+    IntValue,
+    KnoraStandoffXml,
+    LinkValue,
+    ListValue,
+    TextValue,
+    TimeValue,
+    UriValue,
+    Value,
+    fromJsonLdObj
+)
 
 
 class KnoraStandoffXmlEncoder(json.JSONEncoder):
     """Classes used as wrapper for knora standoff-XML"""
 
     def default(self, obj) -> str:
         if isinstance(obj, KnoraStandoffXml):
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.2.1/src/dsp_tools/models/resourceclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
 import re
 from enum import Enum
-from typing import Tuple, Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
-from dsp_tools.models.set_encoder import SetEncoder
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.helpers import Actions, Context, Cardinality, DateTimeStamp
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.langstring import Languages, LangString
+from dsp_tools.models.helpers import (
+    Actions,
+    Cardinality,
+    Context,
+    DateTimeStamp
+)
+from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
+from dsp_tools.models.set_encoder import SetEncoder
 
 """
 This model implements the handling of resource classes. It contains two classes that work closely together:
     * "HasProperty" deals with the association of Property-instances with the Resource-instances. This association
       is done using the "cardinality"-clause
     * "ResourceClass" is the main class representing a knora resource class.
 """
@@ -109,15 +113,15 @@
         self._changed.add('gui_order')
 
     @property
     def ptype(self) -> Ptype:
         return self._ptype
 
     @classmethod
-    def fromJsonObj(cls, con: Connection, context: Context, jsonld_obj: Any) -> Tuple[str, 'HasProperty']:
+    def fromJsonObj(cls, con: Connection, context: Context, jsonld_obj: Any) -> tuple[str, 'HasProperty']:
         if not isinstance(con, Connection):
             raise BaseError('"con"-parameter must be an instance of Connection')
         if not isinstance(context, Context):
             raise BaseError('"context"-parameter must be an instance of Context')
 
         rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
@@ -235,29 +239,29 @@
                 }],
                 "@context": self._context.toJsonObj()
             }
             if self._gui_order is not None and 'gui_order' in self._changed:
                 tmp["@graph"][0]["rdfs:subClassOf"]["salsah-gui:guiOrder"] = self._gui_order
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'ResourceClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
         if self._ontology_id is None:
             raise BaseError("Ontology id required")
         if self._property_id is None:
             raise BaseError("Property id required")
         if self._cardinality is None:
             raise BaseError("Cardinality id required")
 
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=2)
         result = self._con.post(HasProperty.ROUTE, jsondata)
         last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
         return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
 
-    def update(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
         if self._ontology_id is None:
             raise BaseError("Ontology id required")
         if self._property_id is None:
             raise BaseError("Property id required")
         if self._cardinality is None:
             raise BaseError("Cardinality id required")
         jsonobj = self.toJsonObj(last_modification_date, Actions.Update)
@@ -730,22 +734,22 @@
                 if not self._label.isEmpty() and 'label' in self._changed:
                     tmp['@graph'][0]['rdfs:label'] = self._label.toJsonLdObj()
             if what == 'comment':
                 if not self._comment.isEmpty() and 'comment' in self._changed:
                     tmp['@graph'][0]['rdfs:comment'] = self._comment.toJsonLdObj()
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'ResourceClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
         result = self._con.post(ResourceClass.ROUTE, jsondata)
         last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
         return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
 
-    def update(self, last_modification_date: DateTimeStamp) -> Tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
         #
         # Note: Knora is able to change only one thing per call, either label or comment!
         #
         result = None
         something_changed = False
         if 'label' in self._changed:
             jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'label')
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/sipi.py` & `dsp_tools-2.2.1/src/dsp_tools/models/sipi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
-import requests
 from typing import Any
+
+import requests
+
 from dsp_tools.models.exceptions import BaseError
 
 
 def on_api_error(res):
     """
     Checks for any API errors
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/user.py` & `dsp_tools-2.2.1/src/dsp_tools/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
+
 import json
 import os
 import sys
 import urllib.parse
-from typing import Optional, Any, Union
+from typing import Any, Optional, Union
 from urllib.parse import quote_plus
 
-
 from dsp_tools.models.connection import Connection
+from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.group import Group
 from dsp_tools.models.helpers import Actions
-from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.langstring import Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.project import Project
 
 path = os.path.abspath(os.path.dirname(__file__))
 (head, tail) = os.path.split(path)
 if not head in sys.path:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/value.py` & `dsp_tools-2.2.1/src/dsp_tools/models/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
-from typing import Optional, Any, Union
+from typing import Any, Optional, Union
 
 import regex
 
-from dsp_tools.models.helpers import IriTest, Actions
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions, IriTest
 from dsp_tools.models.langstring import LangString
 from dsp_tools.models.listnode import ListNode
-from dsp_tools.models.permission import PermissionValue, Permissions
+from dsp_tools.models.permission import Permissions, PermissionValue
 
 
 class KnoraStandoffXml:
     """Used to handle XML strings for standoff markup"""
 
     __iriregexp = re.compile(r'IRI:[^:]*:IRI')
     __xmlstr: str
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlproperty.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from lxml import etree
 
-from dsp_tools.models.xmlvalue import XMLValue
 from dsp_tools.models.xmlerror import XmlError
+from dsp_tools.models.xmlvalue import XMLValue
 
 
 class XMLProperty:
     """Represents a property of a resource in the XML used for data import"""
 
     _name: str
     _valtype: str
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.2.1/src/dsp_tools/models/xmlvalue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Optional
+from typing import Optional, Union
 
 from lxml import etree
 
 from dsp_tools.models.value import KnoraStandoffXml
 
 
 class XMLValue:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.2.1/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.2.1/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.2.1/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.2.1/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.2.1/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.2.1/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.2.1/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.2.1/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 version: '3.7'
 
 services:
 
   app:
-    image: daschswiss/dsp-app:v10.16.0  # on the verge of every deployment (fortnightly),
+    image: daschswiss/dsp-app:v10.18.0  # on the verge of every deployment (fortnightly),
                                         # take the tag of https://hub.docker.com/r/daschswiss/dsp-app/tags
                                         # that corresponds to the version
                                         # on https://admin.staging.dasch.swiss/help
     ports:
       - "4200:4200"
     networks:
       - knora-net
@@ -21,15 +21,15 @@
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
-    image: daschswiss/knora-sipi:28.0.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    image: daschswiss/knora-sipi:28.1.1  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -40,15 +40,15 @@
       - SIPI_WEBAPI_HOSTNAME=api
       - SIPI_WEBAPI_PORT=3333
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
-    image: daschswiss/knora-api:28.0.0  # on the verge of every deployment (fortnightly),
+    image: daschswiss/knora-api:28.1.1  # on the verge of every deployment (fortnightly),
                                         # take the tag of https://hub.docker.com/r/daschswiss/knora-api/tags
                                         # that corresponds to the version
                                         # on https://admin.staging.dasch.swiss/help
     depends_on:
       - sipi
       - db
     ports:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module handles all the operations which are used for the creation of JSON lists from Excel files."""
-import importlib.resources
 import glob
+import importlib.resources
 import json
 import os
 import re
-from typing import Any, Union, Optional, Tuple
+from typing import Any, Optional, Union
 
 import jsonschema
 import regex
 from openpyxl import load_workbook
 from openpyxl.cell import Cell
 from openpyxl.worksheet.worksheet import Worksheet
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 import importlib.resources
 import json
 import re
 import warnings
 from typing import Any, Optional
 
-import jsonschema
 import jsonpath_ng.ext
+import jsonschema
 import pandas as pd
 
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.utils.shared import prepare_dataframe, check_notna
+from dsp_tools.utils.shared import check_notna, prepare_dataframe
 
 languages = ["en", "de", "fr", "it", "rm"]
 
 
-def _validate_properties_with_schema(properties_list: list[dict[str, Any]]) -> bool:
+def _validate_properties(properties_list: list[dict[str, Any]], excelfile: str) -> bool:
     """
-    This function checks if the "properties" section of a JSON project file is valid according to the schema.
+    This function checks if the "properties" section of a JSON project file is valid according to the JSON schema,
+    and if the property names are unique.
 
     Args:
         properties_list: the "properties" section of a JSON project as a list of dicts
+        excelfile: path to the Excel file containing the properties
     
     Raises:
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "properties" section passed validation
     """
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/properties-only.json").open() as schema_file:
         properties_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=properties_list, schema=properties_schema)
     except jsonschema.ValidationError as err:
-        err_msg = f"'properties' section did not pass validation. "
+        err_msg = f"The 'properties' section defined in the Excel file '{excelfile}' did not pass validation. "
         json_path_to_property = re.search(r"^\$\[(\d+)\]", err.json_path)
         if json_path_to_property:
             wrong_property_name = jsonpath_ng.ext.parse(json_path_to_property.group(0)).find(properties_list)[0].value["name"]
             excel_row = int(json_path_to_property.group(1)) + 2
             err_msg += f"The problematic property is '{wrong_property_name}' in Excel row {excel_row}. "
             affected_field = re.search(r"name|labels|comments|super|subject|object|gui_element|gui_attributes", err.json_path)
             if affected_field:
                 err_msg += f"The problem is that the column '{affected_field.group(0)}' has an invalid value: {err.message}"
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
+    
+    # check if property names are unique
+    all_names = [p["name"] for p in properties_list]
+    duplicates: dict[int, str] = dict()
+    for index, propdef in enumerate(properties_list):
+        if all_names.count(propdef["name"]) > 1:
+            duplicates[index+2] = propdef["name"]
+    if duplicates:
+        err_msg = f"Property names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
+        for row_no, propname in duplicates.items():
+            err_msg += f" - Row {row_no}: {propname}\n"
+        raise BaseError(err_msg)
+    
     return True
 
 
 def _row2prop(row: pd.Series, row_count: int, excelfile: str) -> dict[str, Any]:
     """
     Takes a row from a pandas DataFrame, reads its content, and returns a dict object of the property
 
@@ -154,14 +169,15 @@
         warnings.warn(f"The file '{excelfile}' has a column 'hlist', which is deprecated. "
                       f"Please use the column 'gui_attributes' for the attribute 'hlist'.")
 
     # transform every row into a property
     props = [_row2prop(row, i, excelfile) for i, row in df.iterrows()]
 
     # write final JSON file
-    _validate_properties_with_schema(props)
+    _validate_properties(properties_list=props, excelfile=excelfile)
     if path_to_output_file:
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(props, file, indent=4, ensure_ascii=False)
             print('"properties" section was created successfully and written to file:', path_to_output_file)
 
+
     return props, True
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import importlib.resources
 import json
 import warnings
 from typing import Any, Optional
 
-import jsonschema
 import jsonpath_ng.ext
+import jsonschema
 import pandas as pd
 import regex
 
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.utils.shared import prepare_dataframe, check_notna
+from dsp_tools.utils.shared import check_notna, prepare_dataframe
 
 languages = ["en", "de", "fr", "it", "rm"]
 
 
-def _validate_resources_with_schema(resources_list: list[dict[str, Any]]) -> bool:
+def _validate_resources(resources_list: list[dict[str, Any]], excelfile: str) -> bool:
     """
-    This function checks if the "resources" section of a JSON project file is valid according to the schema.
+    This function checks if the "resources" section of a JSON project file is valid according to the JSON schema,
+    and if the resource names are unique.
 
     Args:
         resources_list: the "resources" section of a JSON project as a list of dicts
+        excelfile: path to the Excel file containing the resources
 
     Raises:
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "resources" section passed validation
     """
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/resources-only.json").open() as schema_file:
         resources_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=resources_list, schema=resources_schema)
     except jsonschema.ValidationError as err:
-        err_msg = f"'resources' section did not pass validation. "
+        err_msg = f"The 'resources' section defined in the Excel file '{excelfile}' did not pass validation. "
         json_path_to_resource = regex.search(r"^\$\[(\d+)\]", err.json_path)
         if json_path_to_resource:
             wrong_resource_name = jsonpath_ng.ext.parse(json_path_to_resource.group(0)).find(resources_list)[0].value["name"]
             affected_field = regex.search(r"name|labels|comments|super|cardinalities\[(\d+)\]", err.json_path)
             if affected_field and affected_field.group(0) in ["name", "labels", "comments", "super"]:
                 excel_row = int(json_path_to_resource.group(1)) + 2
                 err_msg += f"The problem is that the Excel sheet 'classes' contains an invalid value for resource '{wrong_resource_name}', " \
@@ -48,14 +50,27 @@
                                f"in row {excel_row}, column 'Cardinality': {err.message}"
                 elif err.json_path.endswith("propname"):
                     err_msg += f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value " \
                                f"in row {excel_row}, column 'Property': {err.message}"
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
+    
+    # check if resource names are unique
+    all_names = [r["name"] for r in resources_list]
+    duplicates: dict[int, str] = dict()
+    for index, resdef in enumerate(resources_list):
+        if all_names.count(resdef["name"]) > 1:
+            duplicates[index+2] = resdef["name"]
+    if duplicates:
+        err_msg = f"Resource names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
+        for row_no, resname in duplicates.items():
+            err_msg += f" - Row {row_no}: {resname}\n"
+        raise BaseError(err_msg)
+    
     return True
 
 
 def _row2resource(row: pd.Series, excelfile: str) -> dict[str, Any]:
     """
     Method that reads one row from the "classes" DataFrame, 
     opens the corresponding details DataFrame, 
@@ -193,14 +208,14 @@
         warnings.warn(f"The file {excelfile} uses {languages} as column titles, which is deprecated. "
                       f"Please use {[f'label_{lang}' for lang in languages]}")
 
     # transform every row into a resource
     resources = [_row2resource(row, excelfile) for i, row in all_classes_df.iterrows()]
 
     # write final "resources" section into a JSON file
-    _validate_resources_with_schema(resources)
+    _validate_resources(resources_list=resources, excelfile=excelfile)
     if path_to_output_file:
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(resources, file, indent=4, ensure_ascii=False)
             print('"resources" section was created successfully and written to file:', path_to_output_file)
 
     return resources, True
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/id_to_iri.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import Optional
 
 from lxml import etree
 
 from dsp_tools.models.exceptions import BaseError
 
+
 def id_to_iri(xml_file: str, json_file: str, out_file: Optional[str], verbose: bool) -> bool:
 
     """
     This function replaces all occurrences of internal IDs with their respective IRIs inside an XML file. It gets the
     mapping from the JSON file provided as parameter for this function.
 
     Args:
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/project_create.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """This module handles the ontology creation, update and upload to a DSP server. This includes the creation and update
 of the project, the creation of groups, users, lists, resource classes, properties and cardinalities."""
-from pathlib import Path
+import logging
 import re
+from pathlib import Path
 from typing import Any, Union, cast
 
 from dsp_tools.models.connection import Connection
+from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.group import Group
-from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Cardinality, Context, DateTimeStamp
 from dsp_tools.models.langstring import LangString
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.project import Project
 from dsp_tools.models.propertyclass import PropertyClass
 from dsp_tools.models.resourceclass import ResourceClass
 from dsp_tools.models.user import User
 from dsp_tools.utils.excel_to_json_lists import expand_lists_from_excel
 from dsp_tools.utils.project_create_lists import create_lists_on_server
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.shared import login, parse_json_input, try_network_action
 
+logger = logging.getLogger(__name__)
+
 
 def _create_project_on_server(
     project_definition: dict[str, Any],
     con: Connection,
     verbose: bool
 ) -> tuple[Project, bool]:
     """
@@ -31,59 +34,59 @@
 
     Args:
         project_definition: parsed JSON project definition
         con: connection to the DSP server
         verbose: verbose switch
 
     Raises:
-        BaseError: if the project cannot be created on the DSP server
+        UserError: if the project cannot be created on the DSP server
 
     Returns:
         a tuple of the remote project and the success status (True if everything went smoothly, False otherwise)
     """
     try:
         # the normal, expected case is that this try block fails
         project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
-        project_remote: Project = try_network_action(
-            action=lambda: project_local.read(),
-            failure_msg=""
-        )
-        print(f"\tWARNING: Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP "
-              f"server. Updating it...")
-        success = False
+        project_remote: Project = try_network_action(lambda: project_local.read())
+        print(f"\tWARNING: Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
+        logger.warning(f"Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
         # try to update the basic info
         project_remote, _ = _update_basic_info_of_project(project=project_remote, project_definition=project_definition, verbose=verbose)
-        # It doesn't matter if the update is successful or not: continue anyway, because success is already false. 
+        # It doesn't matter if the update is successful or not: continue anyway, because success is anyways false. 
         # There are other things from this file that can be created on the server, e.g. the groups and users, so the process must continue.
+        return project_remote, False
     except BaseError:
-        success = True
-        project_local = Project(
-            con=con,
-            shortcode=project_definition["project"]["shortcode"],
-            shortname=project_definition["project"]["shortname"],
-            longname=project_definition["project"]["longname"],
-            description=LangString(project_definition["project"].get("descriptions")),
-            keywords=set(project_definition["project"].get("keywords")),
-            selfjoin=False,
-            status=True
-        )
-        project_remote = try_network_action(
-            action=lambda: project_local.create(),
-            failure_msg=f"ERROR: Cannot create project '{project_definition['project']['shortname']}' "
-                        f"({project_definition['project']['shortcode']}) on DSP server."
-        )
-        print(f"\tCreated project '{project_remote.shortname}' ({project_remote.shortcode}).")
-
+        pass
+    
+    success = True
+    project_local = Project(
+        con=con,
+        shortcode=project_definition["project"]["shortcode"],
+        shortname=project_definition["project"]["shortname"],
+        longname=project_definition["project"]["longname"],
+        description=LangString(project_definition["project"].get("descriptions")),
+        keywords=set(project_definition["project"].get("keywords")),
+        selfjoin=False,
+        status=True
+    )
+    try:
+        project_remote = try_network_action(lambda: project_local.create())
+    except BaseError:
+        err_msg = f"Cannot create project '{project_definition['project']['shortname']}' " \
+                  f"({project_definition['project']['shortcode']}) on DSP server."
+        logger.error(err_msg, exc_info=True)
+        raise UserError(err_msg) from None
+    print(f"\tCreated project '{project_remote.shortname}' ({project_remote.shortcode}).")
     return project_remote, success
 
 
 def _update_basic_info_of_project(
-        project: Project,
-        project_definition: dict[str, Any],
-        verbose: bool
+    project: Project,
+    project_definition: dict[str, Any],
+    verbose: bool
 ) -> tuple[Project, bool]:
     """
     Updates the longname, description and keywords of a project on a DSP server. 
     Returns the updated project (or the unchanged project if not successful) and a boolean saying if the update was successful or not. 
     If the update was not successful, an error message is printed to stdout.
 
     Args:
@@ -93,24 +96,22 @@
     Returns:
         tuple of (updated project, success status)
     """
     project.longname = project_definition["project"]["longname"]
     project.description = project_definition["project"].get("descriptions")
     project.keywords = project_definition["project"].get("keywords")
     try:
-        project_remote: Project = try_network_action(
-            action=lambda: project.update(),
-            failure_msg=f"WARNING: Could not update project '{project_definition['project']['shortname']}' "
-                        f"({project_definition['project']['shortcode']})."
-        )
+        project_remote: Project = try_network_action(lambda: project.update())
         if verbose:
             print(f"\tUpdated project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']}).")
+        logger.info(f"Updated project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']}).")
         return project_remote, True
-    except BaseError as err:
-        print(err.message)
+    except BaseError:
+        print(f"WARNING: Could not update project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']}).")
+        logger.warning(f"Could not update project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']}).", exc_info=True)
         return project, False
 
 
 def _create_groups(con: Connection, groups: list[dict[str, str]], project: Project) -> tuple[dict[str, Group], bool]:
     """
     Creates groups on a DSP server from the "groups" section of a JSON project file. If a group cannot be created, it is
     skipped and a warning is printed, but such a group will still be part of the returned dict.
@@ -127,20 +128,21 @@
         dict of the form ``{group name: group object}`` with the groups that have successfully been created (or already exist). Empty dict if no group was created.
         True if everything went smoothly, False if a warning or error occurred
     """
     overall_success = True
     current_project_groups: dict[str, Group] = {}
     try:
         remote_groups: list[Group] = try_network_action(
-            action=lambda: Group.getAllGroupsForProject(con=con, proj_iri=project.id),  # type: ignore
-            failure_msg="WARNING: Unable to check if group names are already existing on DSP server, because it is "
-                        "not possible to retrieve the remote groups from DSP server."
+            lambda: Group.getAllGroupsForProject(con=con, proj_iri=project.id)  # type: ignore
         )
-    except BaseError as err:
-        print(err.message)
+    except BaseError:
+        err_msg = "Unable to check if group names are already existing on DSP server, because it is " \
+                  "not possible to retrieve the remote groups from the DSP server."
+        print(f"WARNING: {err_msg}")
+        logger.warning(err_msg, exc_info=True)
         remote_groups = []
         overall_success = False
         
     for group in groups:
         group_name = group["name"]
 
         # if the group already exists, add it to "current_project_groups" (for later usage), then skip it
@@ -157,20 +159,18 @@
             name=group_name,
             descriptions=LangString(group["descriptions"]),
             project=project,
             status=bool(group.get("status", True)),  
             selfjoin=bool(group.get("selfjoin", False))
         )
         try:
-            group_remote: Group = try_network_action(
-                action=lambda: group_local.create(),
-                failure_msg=f"\tWARNING: Unable to create group '{group_name}'."
-            )
-        except BaseError as err:
-            print(err.message)
+            group_remote: Group = try_network_action(lambda: group_local.create())
+        except BaseError:
+            print(f"\tWARNING: Unable to create group '{group_name}'.")
+            logger.warning(f"Unable to create group '{group_name}'.", exc_info=True)
             overall_success = False
             continue
 
         current_project_groups[group_remote.name] = group_remote  # type: ignore
         print(f"\tCreated group '{group_name}'.")
 
     return current_project_groups, overall_success
@@ -227,21 +227,20 @@
                 success = False
                 continue
             group = current_project_groups[group_name]
         else:
             # full_group_name refers to an already existing group on DSP
             try:
                 # "remote_groups" might be available from a previous loop cycle
-                remote_groups = remote_groups or try_network_action(
-                    action=lambda: Group.getAllGroups(con=con),
-                    failure_msg=f"\tWARNING: User '{username}' is referring to the group {full_group_name} that "
-                                f"exists on the DSP server, but no groups could be retrieved from the DSP server."
-                )
-            except BaseError as err:
-                print(err.message)
+                remote_groups = remote_groups or try_network_action(lambda: Group.getAllGroups(con=con))
+            except BaseError:
+                err_msg = f"User '{username}' is referring to the group {full_group_name} that " \
+                          f"exists on the DSP server, but no groups could be retrieved from the DSP server."
+                print(f"\tWARNING: {err_msg}")
+                logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             existing_group = [g for g in remote_groups if g.project == current_project.id and g.name == group_name]
             if not existing_group:
                 print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because "
                         f"such a group doesn't exist.")
                 success = False
@@ -289,21 +288,20 @@
         if not project_name:
             # full_project_name refers to the current project
             in_project = current_project
         else:
             # full_project_name refers to an already existing project on DSP
             try:
                 # "remote_projects" might be available from a previous loop cycle
-                remote_projects = remote_projects or try_network_action(
-                    action=lambda: current_project.getAllProjects(con=con),
-                    failure_msg=f"\tWARNING: User '{username}' cannot be added to the projects {json_user_definition['projects']} "
-                                f"because the projects cannot be retrieved from the DSP server."
-                )
-            except BaseError as err:
-                print(err.message)
+                remote_projects = remote_projects or try_network_action(lambda: current_project.getAllProjects(con=con))
+            except BaseError:
+                err_msg = f"User '{username}' cannot be added to the projects {json_user_definition['projects']} " \
+                          f"because the projects cannot be retrieved from the DSP server."
+                print(f"\tWARNING: {err_msg}")
+                logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             in_project_list = [p for p in remote_projects if p.shortname == project_name]
             if not in_project_list:
                 print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. "
                         f"Skipping...")
                 success = False
@@ -341,19 +339,17 @@
     overall_success = True
     for json_user_definition in users_section:
         username = json_user_definition["username"]
 
         # skip the user if he already exists
         try:
             # the normal case is that this try block fails
-            try_network_action(
-                action=lambda: User(con, email=json_user_definition["email"]).read(),
-                failure_msg=""
-            )
+            try_network_action(lambda: User(con, email=json_user_definition["email"]).read())
             print(f"\tWARNING: User '{username}' already exists on the DSP server. Skipping...")
+            logger.warning(f"User '{username}' already exists on the DSP server. Skipping...")
             overall_success = False
             continue
         except BaseError:
             pass
 
         # add user to the group(s)
         group_iris, sysadmin, success = _get_group_iris_for_user(
@@ -387,20 +383,18 @@
             status=bool(json_user_definition.get("status", True)),
             lang=json_user_definition.get("lang", "en"),
             sysadmin=sysadmin,
             in_projects=project_info,
             in_groups=group_iris
         )
         try:
-            try_network_action(
-                action=lambda: user_local.create(),
-                failure_msg=f"\tWARNING: Unable to create user '{username}'."
-            )
-        except BaseError as err:
-            print(err.message)
+            try_network_action(lambda: user_local.create())
+        except BaseError:
+            print(f"\tWARNING: Unable to create user '{username}'.")
+            logger.warning(f"Unable to create user '{username}'.", exc_info=True)
             overall_success = False
             continue
         print(f"\tCreated user '{username}'.")
 
     return overall_success
 
 
@@ -466,21 +460,21 @@
                 sorted_prop_classes.append(prop)
                 ok_propclass_names.append(prop_name)
                 prop_classes_to_sort.remove(prop)
     return sorted_prop_classes
 
 
 def _create_ontologies(
-        con: Connection,
-        context: Context,
-        knora_api_prefix: str,
-        list_root_nodes: dict[str, Any],
-        project_definition: dict[str, Any],
-        project_remote: Project,
-        verbose: bool
+    con: Connection,
+    context: Context,
+    knora_api_prefix: str,
+    list_root_nodes: dict[str, Any],
+    project_definition: dict[str, Any],
+    project_remote: Project,
+    verbose: bool
 ) -> bool:
     """
     Iterates over the ontologies in a JSON project file and creates the ontologies that don't exist on the DSP server
     yet. For every ontology, it first creates the resource classes, then the properties, and then adds the cardinalities
     to the resource classes.
 
     Args:
@@ -489,28 +483,32 @@
         knora_api_prefix: the prefix that stands for the knora-api ontology
         list_root_nodes: the IRIs of the list nodes that were already created and are now available on the DSP server
         project_definition: the parsed JSON project file
         project_remote: representation of the project on the DSP server
         verbose: verbose switch
 
     Raises:
-        BaseError if an error occurs during the creation of an ontology. 
+        UserError if an error occurs during the creation of an ontology. 
         All other errors are printed, the process continues, but the success status will be false.
 
     Returns:
         True if everything went smoothly, False otherwise
     """
 
     overall_success = True
 
     print("Create ontologies...")
-    project_ontologies: list[Ontology] = try_network_action(
-        action=lambda: Ontology.getProjectOntologies(con=con, project_id=project_remote.id),  # type: ignore
-        failure_msg="WARNING: Unable to retrieve remote ontologies. Cannot check if your ontology already exists."
-    )
+    try:
+        project_ontologies: list[Ontology] = try_network_action(
+            lambda: Ontology.getProjectOntologies(con=con, project_id=project_remote.id)  # type: ignore
+        )
+    except BaseError:
+        print("WARNING: Unable to retrieve remote ontologies. Cannot check if your ontology already exists.")
+        logger.warning("Unable to retrieve remote ontologies. Cannot check if your ontology already exists.", exc_info=True)
+        project_ontologies = []
     for ontology_definition in project_definition.get("project", {}).get("ontologies", {}):
         ontology_definition = cast(dict[str, Any], ontology_definition)
         if ontology_definition["name"] in [onto.name for onto in project_ontologies]:
             print(f"\tWARNING: Ontology '{ontology_definition['name']}' already exists on the DSP server. Skipping...")
             overall_success = False
             continue
 
@@ -520,20 +518,23 @@
             con=con,
             project=project_remote,
             label=ontology_definition["label"],
             name=ontology_definition["name"],
             comment=ontology_definition.get("comment")
         )
         # if ontology cannot be created, let the error escalate
-        ontology_remote: Ontology = try_network_action(
-            action=lambda: ontology_local.create(),
-            failure_msg=f"ERROR while trying to create ontology '{ontology_definition['name']}'."
+        try:
+            ontology_remote: Ontology = try_network_action(lambda: ontology_local.create())
+        except BaseError:
+            logger.error(f"ERROR while trying to create ontology '{ontology_definition['name']}'.", exc_info=True)
+            raise UserError(f"ERROR while trying to create ontology '{ontology_definition['name']}'.") from None
+        context.add_context(
+            ontology_remote.name,
+            ontology_remote.id + ('#' if not ontology_remote.id.endswith('#') else '')
         )
-        context.add_context(ontology_remote.name,
-                            ontology_remote.id + ('#' if not ontology_remote.id.endswith('#') else ''))
         last_modification_date = ontology_remote.lastModificationDate
         if verbose:
             print(f"\tCreated ontology '{ontology_definition['name']}'.")
 
         # add the prefixes defined in the JSON file
         for onto_prefix, onto_info in context:
             if onto_info and onto_prefix not in ontology_remote.context:
@@ -576,19 +577,19 @@
         if not success:
             overall_success = False
 
     return overall_success
 
 
 def _add_resource_classes_to_remote_ontology(
-        ontology_definition: dict[str, Any],
-        ontology_remote: Ontology,
-        con: Connection,
-        last_modification_date: DateTimeStamp,
-        verbose: bool
+    ontology_definition: dict[str, Any],
+    ontology_remote: Ontology,
+    con: Connection,
+    last_modification_date: DateTimeStamp,
+    verbose: bool
 ) -> tuple[DateTimeStamp, dict[str, ResourceClass], bool]:
     """
     Creates the resource classes (without cardinalities) defined in the "resources" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a resource class, it is printed out, the process continues, but the success
     status will be false.
 
@@ -620,37 +621,37 @@
             name=res_class["name"],
             superclasses=super_classes,
             label=LangString(res_class.get("labels")),
             comment=LangString(res_class.get("comments")) if res_class.get("comments") else None
         )
         try:
             last_modification_date, res_class_remote = try_network_action(
-                action=lambda: res_class_local.create(last_modification_date=last_modification_date),
-                failure_msg=f"WARNING: Unable to create resource class '{res_class['name']}'."
+                lambda: res_class_local.create(last_modification_date=last_modification_date)
             )
             res_class_remote = cast(ResourceClass, res_class_remote)
             new_res_classes[str(res_class_remote.id)] = res_class_remote
             ontology_remote.lastModificationDate = last_modification_date
             if verbose:
                 print(f"\tCreated resource class '{res_class['name']}'")
-        except BaseError as err:
-            print(err.message)
+        except BaseError:
+            print(f"WARNING: Unable to create resource class '{res_class['name']}'.")
+            logger.warning(f"Unable to create resource class '{res_class['name']}'.", exc_info=True)
             overall_success = False
 
     return last_modification_date, new_res_classes, overall_success
 
 
 def _add_property_classes_to_remote_ontology(
-        ontology_definition: dict[str, Any],
-        ontology_remote: Ontology,
-        list_root_nodes: dict[str, Any],
-        con: Connection,
-        last_modification_date: DateTimeStamp,
-        knora_api_prefix: str,
-        verbose: bool
+    ontology_definition: dict[str, Any],
+    ontology_remote: Ontology,
+    list_root_nodes: dict[str, Any],
+    con: Connection,
+    last_modification_date: DateTimeStamp,
+    knora_api_prefix: str,
+    verbose: bool
 ) -> tuple[DateTimeStamp, bool]:
     """
     Creates the property classes defined in the "properties" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a property class, it is printed out, the process continues, but the success
     status will be false.
 
@@ -713,35 +714,35 @@
             object=prop_object,
             subject=prop_class.get("subject"),
             gui_element="salsah-gui:" + prop_class["gui_element"],
             gui_attributes=gui_attributes,
             comment=LangString(prop_class["comments"]) if prop_class.get("comments") else None
         )
         try:
-            last_modification_date, prop_class_remote = try_network_action(
-                action=lambda: prop_class_local.create(last_modification_date=last_modification_date),
-                failure_msg=f"WARNING: Unable to create property class '{prop_class['name']}'."
+            last_modification_date, _ = try_network_action(
+                lambda: prop_class_local.create(last_modification_date=last_modification_date)
             )
             ontology_remote.lastModificationDate = last_modification_date
             if verbose:
                 print(f"\tCreated property class '{prop_class['name']}'")
-        except BaseError as err:
-            print(err.message)
+        except BaseError:
+            print(f"WARNING: Unable to create property class '{prop_class['name']}'.")
+            logger.warning(f"Unable to create property class '{prop_class['name']}'.", exc_info=True)
             overall_success = False
 
     return last_modification_date, overall_success
 
 
 def _add_cardinalities_to_resource_classes(
-        ontology_definition: dict[str, Any],
-        ontology_remote: Ontology,
-        remote_res_classes: dict[str, ResourceClass],
-        last_modification_date: DateTimeStamp,
-        knora_api_prefix: str,
-        verbose: bool
+    ontology_definition: dict[str, Any],
+    ontology_remote: Ontology,
+    remote_res_classes: dict[str, ResourceClass],
+    last_modification_date: DateTimeStamp,
+    knora_api_prefix: str,
+    verbose: bool
 ) -> bool:
     """
     Iterates over the resource classes of an ontology of a JSON project definition, and adds the cardinalities to each 
     resource class. The resource classes and the properties must already be existing on the DSP server.
     If an error occurs during creation of a cardinality, it is printed out, the process continues, but the success
     status will be false.
 
@@ -776,27 +777,26 @@
                 prefix, prop = card_info["propname"].split(":")
                 qualified_propname = card_info["propname"] if prefix else f"{ontology_remote.name}:{prop}"
             else:
                 qualified_propname = knora_api_prefix + card_info["propname"]
 
             try:
                 last_modification_date = try_network_action(
-                    action=lambda: res_class_remote.addProperty(  # type: ignore
+                    lambda: res_class_remote.addProperty(  # type: ignore
                         property_id=qualified_propname,
                         cardinality=switcher[card_info["cardinality"]],
                         gui_order=card_info.get("gui_order"),
                         last_modification_date=last_modification_date
-                    ),
-                    failure_msg=f"WARNING: Unable to add cardinality '{qualified_propname}' to resource class "
-                                f"{res_class['name']}."
+                    )
                 )
                 if verbose:
                     print(f"\tAdded cardinality '{card_info['propname']}' to resource class '{res_class['name']}'")
-            except BaseError as err:
-                print(err.message)
+            except BaseError:
+                print(f"WARNING: Unable to add cardinality '{qualified_propname}' to resource class {res_class['name']}.")
+                logger.warning(f"Unable to add cardinality '{qualified_propname}' to resource class {res_class['name']}.", exc_info=True)
                 overall_success = False
 
             ontology_remote.lastModificationDate = last_modification_date
 
     return overall_success
 
 
@@ -820,21 +820,22 @@
         server: the URL of the DSP server on which the project should be created
         user_mail: a username (e-mail) who has the permission to create a project
         password: the user's password
         verbose: prints more information if set to True
         dump: dumps test files (JSON) for DSP API requests if set to True
 
     Raises:
+        UserError: 
+           - if the project cannot be created
+           - if the login fails
+           - if an ontology cannot be created
         BaseError: 
            - if the input is invalid
            - if an Excel file referenced in the "lists" section cannot be expanded
            - if the validation doesn't pass
-           - if the login fails
-           - if the project cannot be created
-           - if an ontology cannot be created
 
     Returns:
         True if everything went smoothly, False if a warning or error occurred
     """
 
     knora_api_prefix = "knora-api:"
     overall_success = True
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/project_create_lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import logging
 from typing import Any, Optional, Union
 
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.project import Project
 from dsp_tools.utils.excel_to_json_lists import expand_lists_from_excel
-from dsp_tools.utils.shared import parse_json_input
 from dsp_tools.utils.project_validate import validate_project
-from dsp_tools.utils.shared import login, try_network_action
+from dsp_tools.utils.shared import login, parse_json_input, try_network_action
+
+logger = logging.getLogger(__name__)
 
 
 def _create_list_node(
     con: Connection,
     project: Project,
     node: dict[str, Any],
     parent_node: Optional[ListNode] = None
@@ -39,20 +41,18 @@
         project=project,
         label=node["labels"],
         comments=node.get("comments"),
         name=node["name"],
         parent=parent_node
     )
     try:
-        new_node = try_network_action(
-            action=lambda: new_node.create(),
-            failure_msg=f"ERROR while trying to create list node '{node['name']}'."
-        )
-    except BaseError as err:
-        print(err.message)
+        new_node = try_network_action(lambda: new_node.create())
+    except BaseError:
+        print(f"WARNING: Cannot create list node '{node['name']}'.")
+        logger.warning("Cannot create list node '{node['name']}'.", exc_info=True)
         return {}, False
 
     # if node has child nodes, call the method recursively
     if node.get("nodes"):
         overall_success = True
         subnode_list = []
         for subnode in node["nodes"]:
@@ -69,14 +69,15 @@
     lists_to_create: list[dict[str, Any]],
     con: Connection,
     project_remote: Project
 ) -> tuple[dict[str, Any], bool]:
     """
     Creates the "lists" section of a JSON project definition on a DSP server.
     If a list with the same name is already existing in this project on the DSP server, this list is skipped.
+    If a node or an entire list cannot be created, an error message is printed, but the process continues.
 
     Args:
         lists_to_create: "lists" section of a JSON project definition
         con: connection to the DSP server
         project_remote: representation of the project on the DSP server
 
     Returns:
@@ -84,19 +85,19 @@
     """
     
     overall_success = True
     
     # retrieve existing lists
     try:
         existing_lists: list[ListNode] = try_network_action(
-            action=lambda: ListNode.getAllLists(con=con, project_iri=project_remote.id),
-            failure_msg="WARNING: Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing."
+            lambda: ListNode.getAllLists(con=con, project_iri=project_remote.id)
         )
-    except BaseError as err:
-        print(err.message)
+    except BaseError:
+        print("WARNING: Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.")
+        logger.warning("Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.", exc_info=True)
         existing_lists = []
         overall_success = False
     
     current_project_lists: dict[str, Any] = {}
     for new_list in lists_to_create:
         # if list exists already, add it to "current_project_lists" (for later usage), then skip it
         existing_list = [x for x in existing_lists if x.project == project_remote.id and x.name == new_list["name"]]
@@ -135,20 +136,21 @@
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
         server: URL of the DSP server
         user: Username (e-mail) for the DSP server, must have the permissions to create a project
         password: Password of the user
         dump: if True, the request is dumped as JSON (used for testing)
 
     Raises:
+        UserError:
+           - if the project cannot be read from the server
+           - if the connection to the DSP server cannot be established
         BaseError: 
            - if the input is invalid
            - if a problem occurred while trying to expand the Excel files
            - if the JSON file is invalid according to the schema
-           - if the connection to the DSP server cannot be established
-           - if the project cannot be read from the server
 
     Returns:
         Returns a tuple consisting of a dict and a bool. 
         The dict contains the IRIs of the created list nodes,
         nested according to their hierarchy structure,
         i.e. ``{nodename: {"id": IRI, "nodes": {...}}}``.
         If there are no lists in the project definition, 
@@ -171,18 +173,20 @@
     # connect to the DSP server
     con = login(server, user, password)
     if dump:
         con.start_logging()
 
     # retrieve the project
     project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
-    project_remote = try_network_action(
-        action=lambda: project_local.read(),
-        failure_msg="ERROR while trying to create the lists: Project couldn't be read from the DSP server."
-    )
+    try:
+        project_remote = try_network_action(lambda: project_local.read())
+    except BaseError:
+        err_msg = f"Unable to create the lists: The project {project_definition['project']['shortcode']} cannot be found on the DSP server."
+        logger.error(err_msg, exc_info=True)
+        raise UserError(err_msg) from None
 
     # create new lists
     current_project_lists, success = create_lists_on_server(lists_to_create=lists_to_create, con=con, project_remote=project_remote)
     if not success:
         overall_success = False
 
     return current_project_lists, overall_success
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/project_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
 from typing import Optional
 
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.group import Group
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.group import Group
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.project import Project
 from dsp_tools.models.user import User
 
 
 def get_project(project_identifier: str, outfile_path: str, server: str, user: str, password: str, verbose: bool) -> bool:
@@ -33,15 +33,15 @@
     if user and password:
         con.login(user, password)
 
     project = None
     if re.match("[0-9A-F]{4}", project_identifier):  # shortcode
         project = Project(con=con, shortcode=project_identifier)
     elif re.match("^[\\w-]+$", project_identifier):  # shortname
-        project = Project(con=con, shortname=project_identifier)
+        project = Project(con=con, shortname=project_identifier.lower())
     elif re.match("^(http)s?://([\\w\\.\\-~]+:?\\d{,4})(/[\\w\\-~]+)+$", project_identifier):  # iri
         project = Project(con=con, shortname=project_identifier)
     else:
         raise BaseError(f"ERROR Invalid project identifier '{project_identifier}'. Use the project's shortcode, shortname or IRI.")
 
     project = project.read()
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/project_validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,64 @@
 import networkx as nx
 import regex
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.excel_to_json_lists import expand_lists_from_excel
 
 
-def check_for_undefined_super_resource(project_definition: dict[str, Any]) -> bool:
+def _check_for_duplicate_names(project_definition: dict[str, Any]) -> bool:
+    """
+    Check that the resource names and property names are unique.
+
+    Args:
+        project_definition: parsed JSON project definition
+
+    Raises:
+        BaseError: detailed error message if there is a duplicate resource name / property name
+
+    Returns:
+        True if the resource/property names are unique
+    """
+    resnames_duplicates: dict[str, set[str]] = dict()
+    propnames_duplicates: dict[str, set[str]] = dict()
+    for onto in project_definition["project"]["ontologies"]:
+        resnames = [r["name"] for r in onto["resources"]]
+        if len(set(resnames)) != len(resnames):
+            for elem in resnames:
+                if resnames.count(elem) > 1:
+                    if not resnames_duplicates.get(onto["name"]):
+                        resnames_duplicates[onto["name"]] = {elem,}
+                    else:
+                        resnames_duplicates[onto["name"]].add(elem)
+        
+        propnames = [p["name"] for p in onto["properties"]]
+        if len(set(propnames)) != len(propnames):
+            for elem in propnames:
+                if propnames.count(elem) > 1:
+                    if not propnames_duplicates.get(onto["name"]):
+                        propnames_duplicates[onto["name"]] = {elem,}
+                    else:
+                        propnames_duplicates[onto["name"]].add(elem)
+        
+    if not resnames_duplicates and not propnames_duplicates:
+        return True
+    
+    err_msg = "Resource names and property names must be unique inside every ontology.\n"
+    for ontoname, res_duplicates in resnames_duplicates.items():
+        for res_duplicate in sorted(res_duplicates):
+            err_msg += f"Resource '{res_duplicate}' appears multiple times in the ontology '{ontoname}'.\n" 
+    for ontoname, prop_duplicates in propnames_duplicates.items():
+        for prop_duplicate in sorted(prop_duplicates):
+            err_msg += f"Property '{prop_duplicate}' appears multiple times in the ontology '{ontoname}'.\n" 
+        
+    raise BaseError(err_msg)
+    
+
+
+def _check_for_undefined_super_resource(project_definition: dict[str, Any]) -> bool:
     """
     Check the superresources that claim to point to a resource defined in the same JSON project.
     Check if the resource they point to actually exists.
     (DSP base resources and resources from other ontologies are not considered.)
 
     Args:
         project_definition: parsed JSON project definition
@@ -56,15 +105,15 @@
     if errors:
         err_msg = "Your data model contains resources that are derived from an invalid super-resource:\n"
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
-def check_for_undefined_super_property(project_definition: dict[str, Any]) -> bool:
+def _check_for_undefined_super_property(project_definition: dict[str, Any]) -> bool:
     """
     Check the superproperties that claim to point to a property defined in the same JSON project.
     Check if the property they point to actually exists.
     (DSP base properties and properties from other ontologies are not considered.)
 
     Args:
         project_definition: parsed JSON project definition
@@ -103,15 +152,15 @@
     if errors:
         err_msg = "Your data model contains properties that are derived from an invalid super-property:\n"
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
-def check_for_undefined_cardinalities(project_definition: dict[str, Any]) -> bool:
+def _check_for_undefined_cardinalities(project_definition: dict[str, Any]) -> bool:
     """
     Check if the propnames that are used in the cardinalities of each resource are defined in the "properties" 
     section. (DSP base properties and properties from other ontologies are not considered.)
 
     Args:
         project_definition: parsed JSON project definition
 
@@ -154,62 +203,71 @@
 
 
 def validate_project(
     input_file_or_json: Union[dict[str, Any], str],
     expand_lists: bool = True
 ) -> bool:
     """
-    Validates a JSON project definition file. First, the Excel file references in the "lists" section are expanded
-    (unless this behaviour is disabled). Then, the project is validated against the JSON schema. At last, a check is
-    performed if this project's ontologies contain properties derived from hasLinkTo that form a circular reference. If
-    so, these properties must have the cardinality 0-1 or 0-n, because during the xmlupload process, these values
-    are temporarily removed.
+    Validates a JSON project definition file. 
+
+    First, the Excel file references in the "lists" section are expanded
+    (unless this behaviour is disabled). 
+
+    Then, the project is validated against the JSON schema. 
+
+    Next, some checks are performed that are too complex for JSON schema.
+    
+    At last, a check is performed
+    if this project's ontologies contain properties derived from hasLinkTo 
+    that form a circular reference.
+    If so, these properties must have the cardinality 0-1 or 0-n, 
+    because during the xmlupload process, 
+    these values are temporarily removed.
 
     Args:
         input_file_or_json: the project to be validated, can either be a file path or a parsed JSON file
         expand_lists: if True, the Excel file references in the "lists" section will be expanded
 
     Raises:
         BaseError: detailed error report if the validation doesn't pass
 
     Returns:
         True if the project passed validation. 
     """
 
+    # parse input
     if isinstance(input_file_or_json, dict) and "project" in input_file_or_json:
         project_definition = input_file_or_json
     elif isinstance(input_file_or_json, str) and os.path.isfile(input_file_or_json) and regex.search(r"\.json$", input_file_or_json):
         with open(input_file_or_json) as f:
             project_definition = json.load(f)
     else:
         raise BaseError(f"Input '{input_file_or_json}' is neither a file path nor a JSON object.")
 
+    # expand all lists referenced in the "lists" section of the project definition, and add them to the project definition
     if expand_lists:
-        # expand all lists referenced in the "lists" section of the project definition, and add them to the project
-        # definition
         new_lists = expand_lists_from_excel(project_definition["project"].get("lists", []))
         if new_lists:
             project_definition["project"]["lists"] = new_lists
 
     # validate the project definition against the schema
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/project.json").open() as schema_file:
         project_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=project_definition, schema=project_schema)
     except jsonschema.ValidationError as err:
         raise BaseError(f"The JSON project file cannot be created due to the following validation error: {err.message}.\n"
                         f"The error occurred at {err.json_path}:\n"
                         f"{err.instance}") from None
 
-    # make sure that there is no undefined superproperty or superresource
-    check_for_undefined_super_property(project_definition)
-    check_for_undefined_super_resource(project_definition)
-
-    # make sure that every cardinality was defined in the properties section
-    check_for_undefined_cardinalities(project_definition)
+    # make some checks that are too complex for JSON schema
+    _check_for_undefined_super_property(project_definition)
+    _check_for_undefined_super_resource(project_definition)
+    _check_for_undefined_cardinalities(project_definition)
+    _check_for_duplicate_names(project_definition)
 
     # cardinalities check for circular references
     return _check_cardinalities_of_circular_references(project_definition)
 
 
 def _check_cardinalities_of_circular_references(project_definition: dict[Any, Any]) -> bool:
     """
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/shared.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/shared.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,94 @@
 from __future__ import annotations
+
 import copy
 import importlib.resources
 import json
 import logging
-from pathlib import Path
 import time
 import unicodedata
 from datetime import datetime
-from typing import Callable, Any, Optional, Union
+from pathlib import Path
+from typing import Any, Callable, Optional, Union
 
 import pandas as pd
 import regex
 from lxml import etree
 from requests import RequestException
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.propertyelement import PropertyElement
 
-
 logger = logging.getLogger(__name__)
 
 
 def login(server: str, user: str, password: str) -> Connection:
     """
-    Logs in and returns the active connection.
+    Creates a connection, 
+    makes a login (handling temporary network interruptions),
+    and returns the active connection.
 
     Args:
         server: URL of the DSP server to connect to
         user: Username (e-mail)
         password: Password of the user
 
     Raises:
-        BaseError if the login fails
+        UserError if the login fails permanently
 
     Return:
         Connection instance
     """
     con = Connection(server)
-    try_network_action(
-        action=lambda: con.login(email=user, password=password),
-        failure_msg="ERROR: Cannot login to DSP server"
-    )
+    try:
+        try_network_action(lambda: con.login(email=user, password=password))
+    except BaseError:
+        logger.error("Cannot login to DSP server", exc_info=True)
+        raise UserError("Cannot login to DSP server") from None
     return con
 
 
-def try_network_action(
-    failure_msg: str,
-    action: Callable[..., Any]
-) -> Any:
-    """
-    Helper method that tries 7 times to execute an action. Each time, it catches ConnectionError and
-    requests.exceptions.RequestException, which lead to a waiting time and a retry. The waiting times are 1,
-    2, 4, 8, 16, 32, 64 seconds.
-
-    In case of a BaseError or Exception, a BaseError is raised with failure_msg.
-
-    If there is no success at the end, a BaseError with failure_msg is raised.
+def try_network_action(action: Callable[..., Any]) -> Any:
+    """
+    Helper method that tries 7 times to execute an action. 
+    If a ConnectionError, a requests.exceptions.RequestException, or a non-permanent BaseError occors, 
+    it waits and retries. 
+    The waiting times are 1, 2, 4, 8, 16, 32, 64 seconds.
+    If another exception occurs, it escalates.
 
     Args:
-        failure_msg: message of the raised BaseError if action cannot be executed
         action: a lambda with the code to be executed
 
     Raises:
-        BaseError if action fails permanently
+        BaseError or unexpected exception if the action fails permanently
 
     Returns:
         the return value of action
     """
 
     for i in range(7):
         try:
             return action()
-        except ConnectionError:
-            print(f'{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...')
-            time.sleep(2 ** i)
-            continue
-        except RequestException:
-            print(f'{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...')
+        except (ConnectionError, RequestException):
+            print(f"{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...")
+            logger.error(f"Try reconnecting to DSP server, next attempt in {2 ** i} seconds...", exc_info=True)
             time.sleep(2 ** i)
             continue
         except BaseError as err:
-            if regex.search(r'try again later', err.message) or regex.search(r'status code=5\d\d', err.message):
-                print(f'{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...')
+            if regex.search(r"try again later", err.message) or regex.search(r"status code=5\d\d", err.message):
+                print(f"{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...")
+                logger.error(f"Try reconnecting to DSP server, next attempt in {2 ** i} seconds...", exc_info=True)
                 time.sleep(2 ** i)
                 continue
-            logger.exception(failure_msg)
-            raise BaseError(failure_msg) from None
-        except Exception:
-            logger.exception(failure_msg)
-            raise BaseError(failure_msg) from None
+            else:
+                raise err
 
-    logger.error(failure_msg)
-    raise BaseError(failure_msg)
+    logger.error("Permanently unable to execute the network action. See logs for more details.")
+    raise BaseError("Permanently unable to execute the network action. See logs for more details.")
 
 
 def validate_xml_against_schema(input_file: Union[str, Path, etree._ElementTree[Any]]) -> bool:
     """
     Validates an XML file against the DSP XSD schema.
 
     Args:
@@ -110,15 +102,15 @@
     """
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/data.xsd").open() as schema_file:
         xmlschema = etree.XMLSchema(etree.parse(schema_file))
     if isinstance(input_file, str) or isinstance(input_file, Path):
         try:
             doc = etree.parse(source=input_file)
         except etree.XMLSyntaxError as err:
-            logger.exception(f"The XML file contains the following syntax error: {err.msg}")
+            logger.error(f"The XML file contains the following syntax error: {err.msg}", exc_info=True)
             raise UserError(f"The XML file contains the following syntax error: {err.msg}") from None
     else:
         doc = input_file
 
     if not xmlschema.validate(doc):
         error_msg = "The XML file cannot be uploaded due to the following validation error(s):"
         for error in xmlschema.error_log:
@@ -166,15 +158,15 @@
                 sourceline = f" line {text.sourceline}: " if text.sourceline else " "
                 propname = text.getparent().attrib["name"]
                 resname = text.getparent().getparent().attrib["id"]
                 resources_with_illegal_xml_tags.append(f" -{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
         err_msg = f"XML-tags are not allowed in text properties with encoding=utf8. The following resources of your XML file violate this rule:\n" 
         err_msg += "\n".join(resources_with_illegal_xml_tags)
-        logger.exception(err_msg)
+        logger.error(err_msg, exc_info=True)
         raise UserError(err_msg)
     
     return True
 
 
 def prepare_dataframe(df: pd.DataFrame, required_columns: list[str], location_of_sheet: str) -> pd.DataFrame:
     """
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/stack_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     docker_path_of_distribution = importlib.resources.files("dsp_tools").joinpath("resources/start-stack")
     for file in docker_path_of_distribution.iterdir():
         with importlib.resources.as_file(file) as f:
             file_path = Path(f)
         shutil.copy(file_path, docker_path_of_user / file.name)
 
     # get sipi.docker-config.lua
-    commit_of_used_api_version = "55a91852b8583d907a0be9b954c3208837b3684c"
+    commit_of_used_api_version = "571246eec32ad44e6b7c87bbb8eab5cad50596bb"      # gitleaks:allow
     url_prefix = f"https://github.com/dasch-swiss/dsp-api/raw/{commit_of_used_api_version}/"
     docker_config_lua_text = requests.get(f"{url_prefix}sipi/config/sipi.docker-config.lua").text
     if max_file_size:
         max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
         if not re.search(max_post_size_regex, docker_config_lua_text):
             raise BaseError("Unable to set max_file_size. Please try again without this flag.")
         docker_config_lua_text = re.sub(max_post_size_regex, f"max_post_size = '{max_file_size}M'", docker_config_lua_text)
```

### Comparing `dsp_tools-2.2.0/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.2.1/src/dsp_tools/utils/xml_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """
 This module handles the import of XML data into the DSP platform.
 """
 from __future__ import annotations
+
 import base64
 import copy
 import json
 import logging
 import os
 import re
 import uuid
 from collections import namedtuple
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, Union, cast, Tuple, Any
+from typing import Any, Optional, Union, cast
 from urllib.parse import quote_plus
 
 import pandas as pd
 from lxml import etree
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.permission import Permissions
 from dsp_tools.models.projectContext import ProjectContext
-from dsp_tools.models.resource import ResourceInstanceFactory, ResourceInstance, KnoraStandoffXmlEncoder
+from dsp_tools.models.resource import (
+    KnoraStandoffXmlEncoder,
+    ResourceInstance,
+    ResourceInstanceFactory
+)
 from dsp_tools.models.sipi import Sipi
 from dsp_tools.models.value import KnoraStandoffXml
 from dsp_tools.models.xmlpermission import XmlPermission
 from dsp_tools.models.xmlproperty import XMLProperty
 from dsp_tools.models.xmlresource import XMLResource
-from dsp_tools.utils.shared import try_network_action, validate_xml_against_schema
+from dsp_tools.utils.shared import (
+    login,
+    try_network_action,
+    validate_xml_against_schema
+)
 
 MetricRecord = namedtuple("MetricRecord", ["res_id", "filetype", "filesize_mb", "event", "duration_ms", "mb_per_sec"])
 
 logger = logging.getLogger(__name__)
 
 
 def _transform_server_url_to_foldername(server: str) -> str:
@@ -206,15 +215,15 @@
 
 def _stash_circular_references(
     nok_resources: list[XMLResource],
     ok_res_ids: list[str],
     ok_resources: list[XMLResource],
     stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
     stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]]
-) -> Tuple[
+) -> tuple[
     list[XMLResource],
     list[str],
     list[XMLResource],
     dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
     dict[XMLResource, dict[XMLProperty, list[str]]]
 ]:
     """
@@ -247,15 +256,15 @@
                         else:
                             if link_prop not in stashed_resptr_props[res]:
                                 stashed_resptr_props[res][link_prop] = [str(value.value)]
                             else:
                                 stashed_resptr_props[res][link_prop].append(str(value.value))
                         link_prop.values.remove(value)
             else:
-                logger.exception("ERROR in remove_circular_references(): link_prop.valtype is neither text nor resptr.")
+                logger.error("ERROR in remove_circular_references(): link_prop.valtype is neither text nor resptr.")
                 raise BaseError("ERROR in remove_circular_references(): link_prop.valtype is neither text nor resptr.")
 
             if len(link_prop.values) == 0:
                 # if all values of a link property have been stashed, the property needs to be removed
                 res.properties.remove(link_prop)
 
         ok_resources.append(res)
@@ -287,24 +296,24 @@
     """
     # create the DaSCH namespace to create version 5 UUIDs
     generic_namespace_url = uuid.NAMESPACE_URL
     dasch_uuid_ns = uuid.uuid5(generic_namespace_url, "https://dasch.swiss")  # cace8b00-717e-50d5-bcb9-486f39d733a2
 
     # get the salsah resource ID from the ARK and convert it to a UUID version 5 (base64 encoded)
     if ark.count("-") != 2:
-        logger.exception(f"while converting ARK '{ark}'. The ARK seems to be invalid")
+        logger.error(f"while converting ARK '{ark}'. The ARK seems to be invalid")
         raise BaseError(f"while converting ARK '{ark}'. The ARK seems to be invalid")
     project_id, resource_id, _ = ark.split("-")
     _, project_id = project_id.rsplit("/", 1)
     project_id = project_id.upper()
     if not re.match("^[0-9a-fA-F]{4}$", project_id):
-        logger.exception(f"while converting ARK '{ark}'. Invalid project shortcode '{project_id}'")
+        logger.error(f"while converting ARK '{ark}'. Invalid project shortcode '{project_id}'")
         raise BaseError(f"while converting ARK '{ark}'. Invalid project shortcode '{project_id}'")
     if not re.match("^[0-9A-Za-z]+$", resource_id):
-        logger.exception(f"while converting ARK '{ark}'. Invalid Salsah ID '{resource_id}'")
+        logger.error(f"while converting ARK '{ark}'. Invalid Salsah ID '{resource_id}'")
         raise BaseError(f"while converting ARK '{ark}'. Invalid Salsah ID '{resource_id}'")
 
     # make a UUID v5 from the namespace created above (which is a UUID itself) and the resource ID and encode it to base64
     dsp_uuid = base64.urlsafe_b64encode(uuid.uuid5(dasch_uuid_ns, resource_id).bytes).decode("utf-8")
     dsp_uuid = dsp_uuid[:-2]
 
     # use the new UUID to create the resource IRI
@@ -374,15 +383,15 @@
     """
     if verbose:
         print("Check if the resource types and properties are consistent with the ontology...")
         logger.info("Check if the resource types and properties are consistent with the ontology...")
     if not any([x.startswith(ontoname) for x in resclass_name_2_type.keys()]):
         err_msg = f"The <knora> tag of your XML file references the ontology '{ontoname}', " \
                   f"but the project {shortcode} on the DSP server doesn't contain an ontology with this name."
-        logger.exception(err_msg)
+        logger.error(err_msg)
         raise UserError(err_msg)
     knora_properties = resclass_name_2_type[resources[0].restype].knora_properties  # type: ignore
 
     for resource in resources:
 
         # check that the resource type is consistent with the ontology
         if resource.restype not in resclass_name_2_type:
@@ -391,15 +400,15 @@
                       f"'{resource.restype}'. Is your syntax correct? Remember the rules:\n" \
                       f" - DSP-API internals: <resource restype=\"restype\">         " \
                               f"(will be interpreted as 'knora-api:restype')\n" \
                       f" - current ontology:  <resource restype=\":restype\">        " \
                               f"('restype' must be defined in the 'resources' section of your ontology)\n" \
                       f" - other ontology:    <resource restype=\"other:restype\">   " \
                               f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)" 
-            logger.exception(err_msg)
+            logger.error(err_msg)
             raise UserError(err_msg)
 
         # check that the property types are consistent with the ontology
         resource_properties = resclass_name_2_type[resource.restype].properties.keys()  # type: ignore
         for propname in [prop.name for prop in resource.properties]:
             if propname not in knora_properties and propname not in resource_properties:
                 err_msg = f"=========================\n" \
@@ -407,15 +416,15 @@
                           f"Is your syntax correct? Remember the rules:\n" \
                           f" - DSP-API internals: <text-prop name=\"propname\">         " \
                                   f"(will be interpreted as 'knora-api:propname')\n" \
                           f" - current ontology:  <text-prop name=\":propname\">        " \
                                   f"('propname' must be defined in the 'properties' section of your ontology)\n" \
                           f" - other ontology:    <text-prop name=\"other:propname\">   " \
                                   f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)" 
-                logger.exception(err_msg)
+                logger.error(err_msg)
                 raise UserError(err_msg)
 
     print("Resource types and properties are consistent with the ontology.")
     logger.info("Resource types and properties are consistent with the ontology.")
 
 
 def xml_upload(
@@ -440,15 +449,15 @@
         imgdir: the image directory
         sipi: the sipi instance to be used
         verbose: verbose option for the command, if used more output is given to the user
         incremental: if set, IRIs instead of internal IDs are expected as resource pointers
         save_metrics: if true, saves time measurements into a "metrics" folder in the current working directory
 
     Raises:
-        BaseError in case of permanent network or software failure
+        BaseError or UserError in case of permanent network or software failure
         UserError if the XML file is invalid
     
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
 
@@ -471,35 +480,38 @@
     logger.info(f"save_location='{save_location}'")
     
     # start metrics
     metrics: list[MetricRecord] = []
     preparation_start = datetime.now()
 
     # Connect to the DaSCH Service Platform API and get the project context
-    con = Connection(server)
-    try_network_action(failure_msg="Unable to login to DSP server", action=lambda: con.login(user, password))
-    proj_context = try_network_action(failure_msg="Unable to retrieve project context from DSP server",
-                                      action=lambda: ProjectContext(con=con))
+    con = login(server=server, user=user, password=password)
+    try:
+        proj_context = try_network_action(lambda: ProjectContext(con=con))
+    except BaseError:
+        logger.error("Unable to retrieve project context from DSP server", exc_info=True)
+        raise UserError("Unable to retrieve project context from DSP server") from None
     sipi_server = Sipi(sipi, con.get_token())
 
     # make Python object representations of the XML file
     resources: list[XMLResource] = []
     permissions: dict[str, XmlPermission] = {}
     for child in root:
         if child.tag == "permissions":
             permission = XmlPermission(child, proj_context)
             permissions[permission.id] = permission
         elif child.tag == "resource":
             resources.append(XMLResource(child, default_ontology))
 
     # get the project information and project ontology from the server
-    res_inst_factory = try_network_action(
-        failure_msg=f"A project with shortcode {shortcode} could not be found on the DSP server", 
-        action=lambda: ResourceInstanceFactory(con, shortcode)
-    )
+    try:
+        res_inst_factory = try_network_action(lambda: ResourceInstanceFactory(con, shortcode))
+    except BaseError:
+        logger.error(f"A project with shortcode {shortcode} could not be found on the DSP server", exc_info=True)
+        raise UserError(f"A project with shortcode {shortcode} could not be found on the DSP server") from None
     permissions_lookup: dict[str, Permissions] = {s: perm.get_permission_instance() for s, perm in permissions.items()}
     resclass_name_2_type: dict[str, type] = {s: res_inst_factory.get_resclass_type(s) for s in res_inst_factory.get_resclass_names()}
 
     # check if the data in the XML is consistent with the ontology
     _check_consistency_with_ontology(
         resources=resources,
         resclass_name_2_type=resclass_name_2_type,
@@ -530,15 +542,15 @@
             failed_uploads, metrics
         )
         if stashed_xml_texts:
             nonapplied_xml_texts = _upload_stashed_xml_texts(verbose, id2iri_mapping, con, stashed_xml_texts) 
         if stashed_resptr_props:
             nonapplied_resptr_props = _upload_stashed_resptr_props(verbose, id2iri_mapping, con, stashed_resptr_props)
         if nonapplied_resptr_props or nonapplied_xml_texts:
-            logger.exception("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
+            logger.error("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
             raise BaseError("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
     except BaseException as err:
         # The forseeable errors are already handled by the variables failed_uploads, nonapplied_xml_texts, and nonapplied_resptr_props.
         # Here we catch the unforseeable exceptions, hence BaseException (=the base class of all exceptions)
         _handle_upload_error(
             err=err,
             id2iri_mapping=id2iri_mapping,
@@ -615,25 +627,23 @@
         # in case of a multimedia resource: upload the multimedia file
         resource_bitstream = None
         if resource.bitstream:
             try:
                 bitstream_start = datetime.now()
                 filetype = Path(resource.bitstream.value).suffix[1:]
                 img: Optional[dict[Any, Any]] = try_network_action(
-                    action=lambda: sipi_server.upload_bitstream(filepath=str(Path(imgdir) / Path(resource.bitstream.value))),  # type: ignore
-                    failure_msg=f'ERROR while trying to upload file "{resource.bitstream.value}" of resource '
-                                f'"{resource.label}" ({resource.id}).'
+                    lambda: sipi_server.upload_bitstream(filepath=str(Path(imgdir) / Path(resource.bitstream.value))),  # type: ignore
                 )
                 bitstream_duration = datetime.now() - bitstream_start
                 bitstream_duration_ms = bitstream_duration.seconds * 1000 + int(bitstream_duration.microseconds / 1000)
                 mb_per_sec = round((filesize / bitstream_duration_ms) * 1000, 1)
                 metrics.append(MetricRecord(resource.id, filetype, filesize, "bitstream upload", bitstream_duration_ms, mb_per_sec))
-            except BaseError as err:
-                print(err.message)
-                logger.exception(err.message)
+            except BaseError:
+                print(f'WARNING: Unable to upload file "{resource.bitstream.value}" of resource "{resource.label}" ({resource.id}).')
+                logger.warning(f'Unable to upload file "{resource.bitstream.value}" of resource "{resource.label}" ({resource.id}).', exc_info=True)
                 failed_uploads.append(resource.id)
                 continue
             bitstream_size_uploaded_mb += bitstream_all_sizes_mb[i]  # type: ignore
             print(f"Uploaded file '{resource.bitstream.value}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)")  # type: ignore
             logger.info(f"Uploaded file '{resource.bitstream.value}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)")  # type: ignore
             internal_file_name_bitstream = img['uploadedFiles'][0]['internalFilename']  # type: ignore
             resource_bitstream = resource.get_bitstream(internal_file_name_bitstream, permissions_lookup)
@@ -648,24 +658,21 @@
                 iri=resource_iri,
                 permissions=permissions_lookup.get(resource.permissions),  # type: ignore
                 creation_date=resource.creation_date,
                 bitstream=resource_bitstream,
                 values=properties
             )
             resource_creation_start = datetime.now()
-            created_resource: ResourceInstance = try_network_action(
-                action=lambda: resource_instance.create(),
-                failure_msg=f"ERROR while trying to create resource '{resource.label}' ({resource.id})."
-            )
+            created_resource: ResourceInstance = try_network_action(lambda: resource_instance.create())
             resource_creation_duration = datetime.now() - resource_creation_start
             resource_creation_duration_ms = resource_creation_duration.seconds * 1000 + int(resource_creation_duration.microseconds / 1000)
             metrics.append(MetricRecord(resource.id, filetype, filesize, "resource creation", resource_creation_duration_ms, ""))
-        except BaseError as err:
-            print(err.message)
-            logger.exception(err.message)
+        except BaseError:
+            print(f"WARNING: Unable to create resource '{resource.label}' ({resource.id}).")
+            logger.warning(f"Unable to create resource '{resource.label}' ({resource.id}).", exc_info=True)
             failed_uploads.append(resource.id)
             continue
         id2iri_mapping[resource.id] = created_resource.iri
         print(f"Created resource {i+1}/{len(resources)}: '{created_resource.label}' (ID: '{resource.id}', IRI: '{created_resource.iri}')")
         logger.info(f"Created resource {i+1}/{len(resources)}: '{created_resource.label}' (ID: '{resource.id}', IRI: '{created_resource.iri}')")
         resource_duration = datetime.now() - resource_start
         resource_duration_ms = resource_duration.seconds * 1000 + int(resource_duration.microseconds / 1000)
@@ -700,22 +707,20 @@
     for resource, link_props in stashed_xml_texts.items():
         if resource.id not in id2iri_mapping:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in nonapplied_xml_texts, which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
-            existing_resource = try_network_action(
-                action=lambda: con.get(path=f'/v2/resources/{quote_plus(res_iri)}'),
-                failure_msg=f'  Unable to upload XML texts of resource "{resource.id}", because the resource cannot be retrieved from the DSP server.'
-            )
-        except BaseError as err:
+            existing_resource = try_network_action(lambda: con.get(path=f'/v2/resources/{quote_plus(res_iri)}'))
+        except BaseError:
             # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
             # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
-            print(err.message)
+            print(f'  WARNING: Unable to upload XML texts of resource "{resource.id}", because the resource cannot be retrieved from the DSP server.')
+            logger.warning(f'Unable to upload XML texts of resource "{resource.id}", because the resource cannot be retrieved from the DSP server.', exc_info=True)
             continue
         print(f'  Upload XML text(s) of resource "{resource.id}"...')
         logger.info(f'  Upload XML text(s) of resource "{resource.id}"...')
         for link_prop, hash_to_value in link_props.items():
             existing_values = existing_resource[link_prop.name]
             if not isinstance(existing_values, list):
                 existing_values = [existing_values, ]
@@ -753,23 +758,20 @@
                     },
                     "@context": existing_resource['@context']
                 }
                 jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '), cls=KnoraStandoffXmlEncoder)
 
                 # execute API call
                 try:
-                    try_network_action(
-                        action=lambda: con.put(path='/v2/values', jsondata=jsondata),
-                        failure_msg=f'    ERROR while uploading the xml text of "{link_prop.name}" of resource "{resource.id}"'
-                    )
-                except BaseError as err:
+                    try_network_action(lambda: con.put(path='/v2/values', jsondata=jsondata))
+                except BaseError:
                     # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
                     # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
-                    print(err.message)
-                    logger.exception(err.message)
+                    print(f'    WARNING: Unable to upload the xml text of "{link_prop.name}" of resource "{resource.id}"')
+                    logger.warning(f'Unable to upload the xml text of "{link_prop.name}" of resource "{resource.id}"', exc_info=True)
                     continue
                 nonapplied_xml_texts[resource][link_prop].pop(pure_text)
                 if verbose:
                     print(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
                     logger.info(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
 
     # make a purged version of nonapplied_xml_texts, without empty entries
@@ -832,23 +834,20 @@
     for resource, prop_2_resptrs in stashed_resptr_props.items():
         if resource.id not in id2iri_mapping:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in nonapplied_resptr_props, which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
-            existing_resource = try_network_action(
-                action=lambda: con.get(path=f'/v2/resources/{quote_plus(res_iri)}'),
-                failure_msg=f'  Unable to upload resptrs of resource "{resource.id}", because the resource cannot be retrieved from the DSP server'
-            )
-        except BaseError as err:
+            existing_resource = try_network_action(lambda: con.get(path=f'/v2/resources/{quote_plus(res_iri)}'))
+        except BaseError:
             # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
             # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
-            print(err.message)
-            logger.exception(err.message)
+            print(f'  WARNING: Unable to upload resptrs of resource "{resource.id}", because the resource cannot be retrieved from the DSP server')
+            logger.warning(f'Unable to upload resptrs of resource "{resource.id}", because the resource cannot be retrieved from the DSP server', exc_info=True)
             continue
         print(f'  Upload resptrs of resource "{resource.id}"...')
         logger.info(f'  Upload resptrs of resource "{resource.id}"...')
         for link_prop, resptrs in prop_2_resptrs.items():
             for resptr in resptrs.copy():
                 jsonobj = {
                     '@id': res_iri,
@@ -861,27 +860,25 @@
                             '@id': id2iri_mapping.get(resptr, resptr)
                         }
                     },
                     '@context': existing_resource['@context']
                 }
                 jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '))
                 try:
-                    try_network_action(
-                        action=lambda: con.post(path='/v2/values', jsondata=jsondata),
-                        failure_msg=f'    ERROR while uploading the resptr prop of "{link_prop.name}" of resource "{resource.id}"'
-                    )
-                except BaseError as err:
+                    try_network_action(lambda: con.post(path='/v2/values', jsondata=jsondata))
+                except BaseError:
                     # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
                     # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
-                    print(err.message)
+                    print(f'    WARNING: Unable to upload the resptr prop of "{link_prop.name}" of resource "{resource.id}"')
+                    logger.warning(f'Unable to upload the resptr prop of "{link_prop.name}" of resource "{resource.id}"', exc_info=True)
                     continue
                 nonapplied_resptr_props[resource][link_prop].remove(resptr)
                 if verbose:
                     print(f'  Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
-                    logger.info(f'  Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
+                    logger.info(f'Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
 
     # make a purged version of nonapplied_resptr_props, without empty entries
     nonapplied_resptr_props = _purge_stashed_resptr_props(stashed_resptr_props=nonapplied_resptr_props, id2iri_mapping=id2iri_mapping)
     return nonapplied_resptr_props
 
 
 def _purge_stashed_resptr_props(
```

### Comparing `dsp_tools-2.2.0/PKG-INFO` & `dsp_tools-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.2.0
+Version: 2.2.1
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -28,16 +28,18 @@
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
 
 # DSP-TOOLS documentation
 
-DSP-TOOLS is a Python package with a command line interface that helps you interact with a DSP server. A DSP server 
-is a remote server or a local machine where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on. 
+DSP-TOOLS is a Python package with a command line interface 
+that helps you interact with a DSP server. 
+A DSP server is a remote server or a local machine 
+where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on. 
 
 To install the latest version, run:
 
 ```bash
 pip3 install dsp-tools
 ```
 
@@ -46,22 +48,26 @@
 ```bash
 pip3 install --upgrade dsp-tools
 ```
 
 The two main tasks that DSP-TOOLS serves for are:
 
 - **Create a project with its data model(s), described in a JSON file, on a DSP server**  
-  In order to archive your data on the DaSCH Service Platform, you need a data model that describes your data.
-  The data model is defined in a JSON project definition file which has to be transmitted to the DSP server. If the DSP 
-  server is aware of the data model for your project, conforming data can be uploaded into the DSP repository.
+  In order to archive your data on the DaSCH Service Platform, 
+  you need a data model that describes your data.
+  The data model is defined in a JSON project definition file 
+  which has to be transmitted to the DSP server. 
+  If the DSP server is aware of the data model for your project, 
+  conforming data can be uploaded into the DSP repository.
 - **Upload data, described in an XML file, to a DSP server that has a project with a matching data model**  
-  Sometimes, data is added in large quantities. Therefore, DSP-TOOLS allows you to perform bulk imports of your
-  data. In order to do so, the data has to be described in an XML file. DSP-TOOLS is able to read the XML file and 
-  upload
-  all data to the DSP server.
+  Sometimes, data is added in large quantities. 
+  Therefore, DSP-TOOLS allows you to perform bulk imports of your data.
+  In order to do so, the data has to be described in an XML file. 
+  DSP-TOOLS is able to read the XML file 
+  and upload all data to the DSP server.
 
 All functionalities of DSP-TOOLS revolve around these two basic tasks. 
 
 DSP-TOOLS provides the following functionalities:
 
 - [`dsp-tools create`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#create) 
   creates the project with its data model(s) on a DSP server from a JSON file.
@@ -69,26 +75,26 @@
   reads a project with its data model(s) from 
   a DSP server and writes it into a JSON file.
 - [`dsp-tools xmlupload`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#xmlupload) 
   uploads data from an XML file (bulk data import)
   and writes the mapping from internal IDs to IRIs into a local file.
 - [`dsp-tools excel2json`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2json) 
   creates an entire JSON project file from a folder with Excel files in it.
-    - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
-      creates the "lists" section of a JSON project file from one or several Excel files. 
-      The resulting section can be integrated into a JSON project file
-      and then be uploaded to a DSP server with `dsp-tools create`.
-    - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
-      creates the "resources" section of a JSON project file from an Excel file. 
-      The resulting section can be integrated into a JSON project file 
-      and then be uploaded to a DSP server with `dsp-tools create`.
-    - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
-      creates the "properties" section of a JSON project file from an Excel file. 
-      The resulting section can be integrated into a JSON project file 
-      and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2lists`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2lists)
+    creates the "lists" section of a JSON project file from one or several Excel files. 
+    The resulting section can be integrated into a JSON project file
+    and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2resources`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2resources)
+    creates the "resources" section of a JSON project file from an Excel file. 
+    The resulting section can be integrated into a JSON project file 
+    and then be uploaded to a DSP server with `dsp-tools create`.
+  - [`dsp-tools excel2properties`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2properties)
+    creates the "properties" section of a JSON project file from an Excel file. 
+    The resulting section can be integrated into a JSON project file 
+    and then be uploaded to a DSP server with `dsp-tools create`.
 - [`dsp-tools excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#excel2xml) 
   transforms a data source to XML 
   if it is already structured according to the DSP specifications.
 - [The module `excel2xml`](https://docs.dasch.swiss/latest/DSP-TOOLS/excel2xml-module) 
   provides helper methods that can be used in a Python script 
   to convert data from a tabular format into XML.
 - [`dsp-tools id2iri`](https://docs.dasch.swiss/latest/DSP-TOOLS/cli-commands/#id2iri)
```

