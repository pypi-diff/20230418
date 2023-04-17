# Comparing `tmp/pyutplugins-0.8.42.tar.gz` & `tmp/pyutplugins-0.8.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-0.8.42.tar", last modified: Sat Apr  1 02:45:06 2023, max compression
+gzip compressed data, was "pyutplugins-0.8.50.tar", last modified: Mon Apr 17 23:31:46 2023, max compression
```

## Comparing `pyutplugins-0.8.42.tar` & `pyutplugins-0.8.50.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.422311 pyutplugins-0.8.42/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2087 2023-04-01 02:45:06.422186 pyutplugins-0.8.42/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1732 2023-01-26 02:00:12.000000 pyutplugins-0.8.42/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.407219 pyutplugins-0.8.42/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.42/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.42/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.42/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.408507 pyutplugins-0.8.42/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.42/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.409162 pyutplugins-0.8.42/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.42/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2023-01-19 02:57:28.000000 pyutplugins-0.8.42/pyutplugins/common/ui/Dimensions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2505 2023-01-20 15:07:17.000000 pyutplugins-0.8.42/pyutplugins/common/ui/DimensionsControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-01 03:01:55.000000 pyutplugins-0.8.42/pyutplugins/common/ui/DualSpinnerControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.409368 pyutplugins-0.8.42/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2023-02-05 15:39:41.000000 pyutplugins-0.8.42/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.42/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.409984 pyutplugins-0.8.42/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.411321 pyutplugins-0.8.42/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7373 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.411895 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.412359 pyutplugins-0.8.42/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.412835 pyutplugins-0.8.42/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.413302 pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10897 2023-02-03 22:23:17.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.413878 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.415004 pyutplugins-0.8.42/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/Python3LexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/Python3ParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/PyutPythonVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17467 2023-01-20 18:33:44.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.415935 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/python/transformGrammar.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.416416 pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4854 2023-01-20 15:07:17.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.417140 pyutplugins-0.8.42/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11799 2023-01-30 01:49:48.000000 pyutplugins-0.8.42/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.42/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.42/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.418605 pyutplugins-0.8.42/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.418935 pyutplugins-0.8.42/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.42/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.42/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.42/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.419812 pyutplugins-0.8.42/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/ToolAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.420578 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1994 2023-01-20 15:07:17.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.422031 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-01 02:45:06.407873 pyutplugins-0.8.42/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2087 2023-04-01 02:45:06.000000 pyutplugins-0.8.42/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5226 2023-04-01 02:45:06.000000 pyutplugins-0.8.42/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-01 02:45:06.000000 pyutplugins-0.8.42/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-04-01 02:45:06.000000 pyutplugins-0.8.42/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-01 02:45:06.000000 pyutplugins-0.8.42/pyutplugins.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-01 02:45:06.422347 pyutplugins-0.8.42/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-04-01 02:37:36.000000 pyutplugins-0.8.42/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.690317 pyutplugins-0.8.50/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-04-17 23:31:46.690189 pyutplugins-0.8.50/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1956 2023-04-14 20:22:33.000000 pyutplugins-0.8.50/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.675513 pyutplugins-0.8.50/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6400 2023-01-04 04:59:38.000000 pyutplugins-0.8.50/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2023-01-20 18:33:44.000000 pyutplugins-0.8.50/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8054 2023-03-31 00:30:02.000000 pyutplugins-0.8.50/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.676799 pyutplugins-0.8.50/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1130 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2353 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-01-19 02:57:18.000000 pyutplugins-0.8.50/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.677497 pyutplugins-0.8.50/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-01-20 15:07:17.000000 pyutplugins-0.8.50/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      705 2023-01-19 02:57:28.000000 pyutplugins-0.8.50/pyutplugins/common/ui/Dimensions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2505 2023-01-20 15:07:17.000000 pyutplugins-0.8.50/pyutplugins/common/ui/DimensionsControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-01 03:01:55.000000 pyutplugins-0.8.50/pyutplugins/common/ui/DualSpinnerControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.677706 pyutplugins-0.8.50/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2023-02-05 15:39:41.000000 pyutplugins-0.8.50/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-01 02:55:47.000000 pyutplugins-0.8.50/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.678248 pyutplugins-0.8.50/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.679586 pyutplugins-0.8.50/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1924 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3245 2023-01-30 01:49:48.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3864 2023-02-03 02:52:30.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7373 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8266 2023-01-30 01:49:48.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.680445 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10397 2023-01-20 18:33:44.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.680942 pyutplugins-0.8.50/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8647 2023-02-01 01:59:25.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.681396 pyutplugins-0.8.50/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    27944 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11156 2023-02-01 01:52:43.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.681875 pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-02-01 20:38:32.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12464 2023-04-17 23:17:22.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-30 01:49:48.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.682492 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9553 2023-01-20 18:33:44.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.683674 pyutplugins-0.8.50/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3579 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/Python3LexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      192 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/Python3ParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12836 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/PyutPythonVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12487 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17467 2023-01-20 18:33:44.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/ReverseEngineerPython2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.684648 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    47673 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   399206 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    37475 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    22412 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      804 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/python/transformGrammar.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.685124 pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4854 2023-01-20 15:07:17.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.685698 pyutplugins-0.8.50/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11799 2023-01-30 01:49:48.000000 pyutplugins-0.8.50/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-01-20 21:59:06.000000 pyutplugins-0.8.50/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-01-20 15:37:30.000000 pyutplugins-0.8.50/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.686995 pyutplugins-0.8.50/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-02-03 02:56:53.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.687281 pyutplugins-0.8.50/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7651 2023-03-31 00:30:24.000000 pyutplugins-0.8.50/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-18 02:02:54.000000 pyutplugins-0.8.50/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 pyutplugins-0.8.50/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.688078 pyutplugins-0.8.50/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1730 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3592 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/ToolAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2023-01-20 18:45:21.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-01-20 18:45:20.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.688761 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1994 2023-01-20 15:07:17.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-01-19 03:33:52.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-01-20 18:33:44.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.690052 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3545 2023-02-22 02:39:48.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28462 2023-02-01 01:51:21.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-01-20 15:25:55.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-04 04:11:16.000000 pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-17 23:31:46.676163 pyutplugins-0.8.50/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2311 2023-04-17 23:31:46.000000 pyutplugins-0.8.50/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5226 2023-04-17 23:31:46.000000 pyutplugins-0.8.50/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-17 23:31:46.000000 pyutplugins-0.8.50/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      203 2023-04-17 23:31:46.000000 pyutplugins-0.8.50/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-17 23:31:46.000000 pyutplugins-0.8.50/pyutplugins.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-17 23:31:46.690353 pyutplugins-0.8.50/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3207 2023-04-17 23:17:22.000000 pyutplugins-0.8.50/setup.py
```

### Comparing `pyutplugins-0.8.42/LICENSE` & `pyutplugins-0.8.50/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/PKG-INFO` & `pyutplugins-0.8.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7574  : 2.1.Name: pyut
 00000020: 706c 7567 696e 730a 5665 7273 696f 6e3a  plugins.Version:
-00000030: 2030 2e38 2e34 320a 5375 6d6d 6172 793a   0.8.42.Summary:
+00000030: 2030 2e38 2e35 300a 5375 6d6d 6172 793a   0.8.50.Summary:
 00000040: 2050 7975 7420 506c 7567 696e 730a 486f   Pyut Plugins.Ho
 00000050: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000060: 2f67 6974 6875 622e 636f 6d2f 6861 7369  /github.com/hasi
 00000070: 6932 3031 312f 7079 7574 706c 7567 696e  i2011/pyutplugin
 00000080: 730a 4175 7468 6f72 3a20 4875 6d62 6572  s.Author: Humber
 00000090: 746f 2041 2e20 5361 6e63 6865 7a20 4949  to A. Sanchez II
 000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 2068  .Author-email: h
@@ -68,64 +68,78 @@
 00000430: 7254 6865 4261 6467 652e 636f 6d2f 696d  rTheBadge.com/im
 00000440: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
 00000450: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
 00000460: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
 00000470: 7974 686f 6e2e 6f72 672f 290a 0a0a 2320  ython.org/)...# 
 00000480: 496e 7472 6f64 7563 7469 6f6e 0a2a 2a54  Introduction.**T
 00000490: 4244 2a2a 0a0a 2320 4f76 6572 7669 6577  BD**..# Overview
-000004a0: 0a0a 2a2a 5442 442a 2a0a 0a2d 2d2d 2d2d  ..**TBD**..-----
-000004b0: 2d0a 0a55 7365 6420 746f 2062 6520 6361  -..Used to be ca
-000004c0: 6c6c 6564 2070 7975 7470 6c75 6769 6e63  lled pyutpluginc
-000004d0: 6f72 650a 0a21 5b48 756d 6265 7274 6f27  ore..![Humberto'
-000004e0: 7320 4d6f 6469 6669 6564 204c 6f67 6f5d  s Modified Logo]
-000004f0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000500: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000510: 6f6d 2f77 696b 692f 6861 7369 6932 3031  om/wiki/hasii201
-00000520: 312f 6769 7474 6f64 6f69 7374 636c 6f6e  1/gittodoistclon
-00000530: 652f 696d 6167 6573 2f53 696c 6c79 4769  e/images/SillyGi
-00000540: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
-00000550: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
-00000560: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
-00000570: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
-00000580: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
-00000590: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
-000005a0: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
-000005b0: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
-000005c0: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
-000005d0: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
-000005e0: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
-000005f0: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
-00000600: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
-00000610: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
-00000620: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
-00000630: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
-00000640: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
-00000650: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
-00000660: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
-00000670: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
-00000680: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
-00000690: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
-000006a0: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
-000006b0: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
-000006c0: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
-000006d0: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
-000006e0: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
-000006f0: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
-00000700: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
-00000710: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
-00000720: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
-00000730: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
-00000740: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
-00000750: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
-00000760: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
-00000770: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
-00000780: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
-00000790: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
-000007a0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-000007b0: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
-000007c0: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
-000007d0: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
-000007e0: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
-000007f0: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
-00000800: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
-00000810: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
-00000820: 6e65 2073 6f2e 0a                        ne so..
+000004a0: 0a0a 2a2a 5442 442a 2a0a 0a23 2320 4465  ..**TBD**..## De
+000004b0: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+000004c0: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+000004d0: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+000004e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004f0: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+00000500: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+00000510: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+00000520: 6e74 2062 7569 6c64 730a 0a5f 5f5f 0a0a  nt builds..___..
+00000530: 5772 6974 7465 6e20 6279 203c 6120 6872  Written by <a hr
+00000540: 6566 3d22 6d61 696c 746f 3a65 6d61 696c  ef="mailto:email
+00000550: 4068 756d 6265 7274 6f2e 612e 7361 6e63  @humberto.a.sanc
+00000560: 6865 7a2e 6969 4067 6d61 696c 2e63 6f6d  hez.ii@gmail.com
+00000570: 3f73 7562 6a65 6374 3d48 656c 6c6f 2048  ?subject=Hello H
+00000580: 756d 6265 7274 6f22 3e48 756d 6265 7274  umberto">Humbert
+00000590: 6f20 412e 2053 616e 6368 657a 2049 493c  o A. Sanchez II<
+000005a0: 2f61 3e20 2028 4329 2032 3032 330a 0a5f  /a>  (C) 2023.._
+000005b0: 5f5f 0a0a 0a21 5b48 756d 6265 7274 6f27  __...![Humberto'
+000005c0: 7320 4d6f 6469 6669 6564 204c 6f67 6f5d  s Modified Logo]
+000005d0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+000005e0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000005f0: 6f6d 2f77 696b 692f 6861 7369 6932 3031  om/wiki/hasii201
+00000600: 312f 6769 7474 6f64 6f69 7374 636c 6f6e  1/gittodoistclon
+00000610: 652f 696d 6167 6573 2f53 696c 6c79 4769  e/images/SillyGi
+00000620: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
+00000630: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
+00000640: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
+00000650: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
+00000660: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
+00000670: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
+00000680: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
+00000690: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
+000006a0: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
+000006b0: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
+000006c0: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
+000006d0: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
+000006e0: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
+000006f0: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
+00000700: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
+00000710: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
+00000720: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
+00000730: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
+00000740: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
+00000750: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
+00000760: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
+00000770: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
+00000780: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
+00000790: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
+000007a0: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
+000007b0: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
+000007c0: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
+000007d0: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
+000007e0: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
+000007f0: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
+00000800: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
+00000810: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
+00000820: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
+00000830: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
+00000840: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
+00000850: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
+00000860: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
+00000870: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
+00000880: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
+00000890: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
+000008a0: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
+000008b0: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
+000008c0: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
+000008d0: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
+000008e0: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
+000008f0: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
+00000900: 6e65 2073 6f2e 0a                        ne so..
```

### Comparing `pyutplugins-0.8.42/README.md` & `pyutplugins-0.8.50/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -46,64 +46,78 @@
 000002d0: 6542 6164 6765 2e63 6f6d 2f69 6d61 6765  eBadge.com/image
 000002e0: 732f 6261 6467 6573 2f6d 6164 652d 7769  s/badges/made-wi
 000002f0: 7468 2d70 7974 686f 6e2e 7376 6729 5d28  th-python.svg)](
 00000300: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
 00000310: 6f6e 2e6f 7267 2f29 0a0a 0a23 2049 6e74  on.org/)...# Int
 00000320: 726f 6475 6374 696f 6e0a 2a2a 5442 442a  roduction.**TBD*
 00000330: 2a0a 0a23 204f 7665 7276 6965 770a 0a2a  *..# Overview..*
-00000340: 2a54 4244 2a2a 0a0a 2d2d 2d2d 2d2d 0a0a  *TBD**..------..
-00000350: 5573 6564 2074 6f20 6265 2063 616c 6c65  Used to be calle
-00000360: 6420 7079 7574 706c 7567 696e 636f 7265  d pyutplugincore
-00000370: 0a0a 215b 4875 6d62 6572 746f 2773 204d  ..![Humberto's M
-00000380: 6f64 6966 6965 6420 4c6f 676f 5d28 6874  odified Logo](ht
-00000390: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000003a0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000003b0: 7769 6b69 2f68 6173 6969 3230 3131 2f67  wiki/hasii2011/g
-000003c0: 6974 746f 646f 6973 7463 6c6f 6e65 2f69  ittodoistclone/i
-000003d0: 6d61 6765 732f 5369 6c6c 7947 6974 4875  mages/SillyGitHu
-000003e0: 622e 706e 6729 0a0a 4920 616d 2063 6f6e  b.png)..I am con
-000003f0: 6365 726e 6564 2061 626f 7574 2047 6974  cerned about Git
-00000400: 4875 6227 7320 436f 7069 6c6f 7420 7072  Hub's Copilot pr
-00000410: 6f6a 6563 740a 0a0a 0a49 2075 7267 6520  oject....I urge 
-00000420: 796f 7520 746f 2072 6561 6420 6162 6f75  you to read abou
-00000430: 7420 7468 650a 5b47 6976 6520 7570 2047  t the.[Give up G
-00000440: 6974 4875 625d 2868 7474 7073 3a2f 2f47  itHub](https://G
-00000450: 6976 6555 7047 6974 4875 622e 6f72 6729  iveUpGitHub.org)
-00000460: 2063 616d 7061 6967 6e20 6672 6f6d 0a5b   campaign from.[
-00000470: 7468 6520 536f 6674 7761 7265 2046 7265  the Software Fre
-00000480: 6564 6f6d 2043 6f6e 7365 7276 616e 6379  edom Conservancy
-00000490: 5d28 6874 7470 733a 2f2f 7366 636f 6e73  ](https://sfcons
-000004a0: 6572 7661 6e63 792e 6f72 6729 2e0a 0a57  ervancy.org)...W
-000004b0: 6869 6c65 2049 2064 6f20 6e6f 7420 6164  hile I do not ad
-000004c0: 766f 6361 7465 2066 6f72 2061 6c6c 2074  vocate for all t
-000004d0: 6865 2069 7373 7565 7320 6c69 7374 6564  he issues listed
-000004e0: 2074 6865 7265 2049 2064 6f20 6e6f 7420   there I do not 
-000004f0: 6c69 6b65 2074 6861 740a 6120 636f 6d70  like that.a comp
-00000500: 616e 7920 6c69 6b65 204d 6963 726f 736f  any like Microso
-00000510: 6674 206d 6179 2070 726f 6669 7420 6672  ft may profit fr
-00000520: 6f6d 206f 7065 6e20 736f 7572 6365 2070  om open source p
-00000530: 726f 6a65 6374 732e 0a0a 4920 636f 6e74  rojects...I cont
-00000540: 696e 7565 2074 6f20 7573 6520 4769 7448  inue to use GitH
-00000550: 7562 2062 6563 6175 7365 2069 7420 6f66  ub because it of
-00000560: 6665 7273 2074 6865 2073 6572 7669 6365  fers the service
-00000570: 7320 4920 6e65 6564 2066 6f72 2066 7265  s I need for fre
-00000580: 652e 2020 4275 742c 2049 2063 6f6e 7469  e.  But, I conti
-00000590: 6e75 650a 746f 206d 6f6e 6974 6f72 2074  nue.to monitor t
-000005a0: 6865 6972 2074 6572 6d73 206f 6620 7365  heir terms of se
-000005b0: 7276 6963 652e 0a0a 416e 7920 7573 6520  rvice...Any use 
-000005c0: 6f66 2074 6869 7320 7072 6f6a 6563 7427  of this project'
-000005d0: 7320 636f 6465 2062 7920 4769 7448 7562  s code by GitHub
-000005e0: 2043 6f70 696c 6f74 2c20 7061 7374 206f   Copilot, past o
-000005f0: 7220 7072 6573 656e 742c 2069 7320 646f  r present, is do
-00000600: 6e65 0a77 6974 686f 7574 206d 7920 7065  ne.without my pe
-00000610: 726d 6973 7369 6f6e 2e20 2049 2064 6f20  rmission.  I do 
-00000620: 6e6f 7420 636f 6e73 656e 7420 746f 2047  not consent to G
-00000630: 6974 4875 6227 7320 7573 6520 6f66 2074  itHub's use of t
-00000640: 6869 7320 7072 6f6a 6563 7427 730a 636f  his project's.co
-00000650: 6465 2069 6e20 436f 7069 6c6f 742e 0a0a  de in Copilot...
-00000660: 4120 7265 706f 7369 746f 7279 206f 776e  A repository own
-00000670: 6572 206d 6179 206f 7074 206f 7574 206f  er may opt out o
-00000680: 6620 436f 7069 6c6f 7420 6279 2063 6861  f Copilot by cha
-00000690: 6e67 696e 6720 5365 7474 696e 6773 202d  nging Settings -
-000006a0: 2d3e 2047 6974 4875 6220 436f 7069 6c6f  -> GitHub Copilo
-000006b0: 742e 0a0a 4920 6861 7665 2064 6f6e 6520  t...I have done 
-000006c0: 736f 2e0a                                so..
+00000340: 2a54 4244 2a2a 0a0a 2323 2044 6576 656c  *TBD**..## Devel
+00000350: 6f70 6572 204e 6f74 6573 0a54 6869 7320  oper Notes.This 
+00000360: 7072 6f6a 6563 7420 7573 6573 205b 6275  project uses [bu
+00000370: 696c 646c 6163 6b65 795d 2868 7474 7073  ildlackey](https
+00000380: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
+00000390: 7369 6932 3031 312f 6275 696c 646c 6163  sii2011/buildlac
+000003a0: 6b65 7929 2066 6f72 2064 6179 2074 6f20  key) for day to 
+000003b0: 6461 7920 6465 7665 6c6f 706d 656e 7420  day development 
+000003c0: 6275 696c 6473 0a0a 5f5f 5f0a 0a57 7269  builds..___..Wri
+000003d0: 7474 656e 2062 7920 3c61 2068 7265 663d  tten by <a href=
+000003e0: 226d 6169 6c74 6f3a 656d 6169 6c40 6875  "mailto:email@hu
+000003f0: 6d62 6572 746f 2e61 2e73 616e 6368 657a  mberto.a.sanchez
+00000400: 2e69 6940 676d 6169 6c2e 636f 6d3f 7375  .ii@gmail.com?su
+00000410: 626a 6563 743d 4865 6c6c 6f20 4875 6d62  bject=Hello Humb
+00000420: 6572 746f 223e 4875 6d62 6572 746f 2041  erto">Humberto A
+00000430: 2e20 5361 6e63 6865 7a20 4949 3c2f 613e  . Sanchez II</a>
+00000440: 2020 2843 2920 3230 3233 0a0a 5f5f 5f0a    (C) 2023..___.
+00000450: 0a0a 215b 4875 6d62 6572 746f 2773 204d  ..![Humberto's M
+00000460: 6f64 6966 6965 6420 4c6f 676f 5d28 6874  odified Logo](ht
+00000470: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000480: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000490: 7769 6b69 2f68 6173 6969 3230 3131 2f67  wiki/hasii2011/g
+000004a0: 6974 746f 646f 6973 7463 6c6f 6e65 2f69  ittodoistclone/i
+000004b0: 6d61 6765 732f 5369 6c6c 7947 6974 4875  mages/SillyGitHu
+000004c0: 622e 706e 6729 0a0a 4920 616d 2063 6f6e  b.png)..I am con
+000004d0: 6365 726e 6564 2061 626f 7574 2047 6974  cerned about Git
+000004e0: 4875 6227 7320 436f 7069 6c6f 7420 7072  Hub's Copilot pr
+000004f0: 6f6a 6563 740a 0a0a 0a49 2075 7267 6520  oject....I urge 
+00000500: 796f 7520 746f 2072 6561 6420 6162 6f75  you to read abou
+00000510: 7420 7468 650a 5b47 6976 6520 7570 2047  t the.[Give up G
+00000520: 6974 4875 625d 2868 7474 7073 3a2f 2f47  itHub](https://G
+00000530: 6976 6555 7047 6974 4875 622e 6f72 6729  iveUpGitHub.org)
+00000540: 2063 616d 7061 6967 6e20 6672 6f6d 0a5b   campaign from.[
+00000550: 7468 6520 536f 6674 7761 7265 2046 7265  the Software Fre
+00000560: 6564 6f6d 2043 6f6e 7365 7276 616e 6379  edom Conservancy
+00000570: 5d28 6874 7470 733a 2f2f 7366 636f 6e73  ](https://sfcons
+00000580: 6572 7661 6e63 792e 6f72 6729 2e0a 0a57  ervancy.org)...W
+00000590: 6869 6c65 2049 2064 6f20 6e6f 7420 6164  hile I do not ad
+000005a0: 766f 6361 7465 2066 6f72 2061 6c6c 2074  vocate for all t
+000005b0: 6865 2069 7373 7565 7320 6c69 7374 6564  he issues listed
+000005c0: 2074 6865 7265 2049 2064 6f20 6e6f 7420   there I do not 
+000005d0: 6c69 6b65 2074 6861 740a 6120 636f 6d70  like that.a comp
+000005e0: 616e 7920 6c69 6b65 204d 6963 726f 736f  any like Microso
+000005f0: 6674 206d 6179 2070 726f 6669 7420 6672  ft may profit fr
+00000600: 6f6d 206f 7065 6e20 736f 7572 6365 2070  om open source p
+00000610: 726f 6a65 6374 732e 0a0a 4920 636f 6e74  rojects...I cont
+00000620: 696e 7565 2074 6f20 7573 6520 4769 7448  inue to use GitH
+00000630: 7562 2062 6563 6175 7365 2069 7420 6f66  ub because it of
+00000640: 6665 7273 2074 6865 2073 6572 7669 6365  fers the service
+00000650: 7320 4920 6e65 6564 2066 6f72 2066 7265  s I need for fre
+00000660: 652e 2020 4275 742c 2049 2063 6f6e 7469  e.  But, I conti
+00000670: 6e75 650a 746f 206d 6f6e 6974 6f72 2074  nue.to monitor t
+00000680: 6865 6972 2074 6572 6d73 206f 6620 7365  heir terms of se
+00000690: 7276 6963 652e 0a0a 416e 7920 7573 6520  rvice...Any use 
+000006a0: 6f66 2074 6869 7320 7072 6f6a 6563 7427  of this project'
+000006b0: 7320 636f 6465 2062 7920 4769 7448 7562  s code by GitHub
+000006c0: 2043 6f70 696c 6f74 2c20 7061 7374 206f   Copilot, past o
+000006d0: 7220 7072 6573 656e 742c 2069 7320 646f  r present, is do
+000006e0: 6e65 0a77 6974 686f 7574 206d 7920 7065  ne.without my pe
+000006f0: 726d 6973 7369 6f6e 2e20 2049 2064 6f20  rmission.  I do 
+00000700: 6e6f 7420 636f 6e73 656e 7420 746f 2047  not consent to G
+00000710: 6974 4875 6227 7320 7573 6520 6f66 2074  itHub's use of t
+00000720: 6869 7320 7072 6f6a 6563 7427 730a 636f  his project's.co
+00000730: 6465 2069 6e20 436f 7069 6c6f 742e 0a0a  de in Copilot...
+00000740: 4120 7265 706f 7369 746f 7279 206f 776e  A repository own
+00000750: 6572 206d 6179 206f 7074 206f 7574 206f  er may opt out o
+00000760: 6620 436f 7069 6c6f 7420 6279 2063 6861  f Copilot by cha
+00000770: 6e67 696e 6720 5365 7474 696e 6773 202d  nging Settings -
+00000780: 2d3e 2047 6974 4875 6220 436f 7069 6c6f  -> GitHub Copilo
+00000790: 742e 0a0a 4920 6861 7665 2064 6f6e 6520  t...I have done 
+000007a0: 736f 2e0a                                so..
```

### Comparing `pyutplugins-0.8.42/pyutplugins/ExternalTypes.py` & `pyutplugins-0.8.50/pyutplugins/ExternalTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/IPluginAdapter.py` & `pyutplugins-0.8.50/pyutplugins/IPluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/PluginManager.py` & `pyutplugins-0.8.50/pyutplugins/PluginManager.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ElementTreeData.py` & `pyutplugins-0.8.50/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-0.8.50/pyutplugins/common/LinkMakerMixin.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-0.8.50/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ui/Dimensions.py` & `pyutplugins-0.8.50/pyutplugins/common/ui/Dimensions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ui/DimensionsControl.py` & `pyutplugins-0.8.50/pyutplugins/common/ui/DimensionsControl.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ui/DualSpinnerControl.py` & `pyutplugins-0.8.50/pyutplugins/common/ui/DualSpinnerControl.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-0.8.50/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOMermaid.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/IOXml.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,28 @@
 from datetime import datetime
 
 from pathlib import Path
 
 from pyutmodel.PyutField import PyutField
 from pyutmodel.PyutField import PyutFields
 from pyutmodel.PyutLink import PyutLink
+from pyutmodel.PyutLinkedObject import PyutLinkedObject
+from pyutmodel.PyutNote import PyutNote
+from pyutmodel.PyutText import PyutText
 from pyutmodel.PyutType import PyutType
 from pyutmodel.PyutClass import PyutClass
 from pyutmodel.PyutMethod import PyutMethod
 from pyutmodel.PyutParameter import PyutParameter
 from pyutmodel.PyutStereotype import PyutStereotype
 from pyutmodel.PyutVisibilityEnum import PyutVisibilityEnum
 
+from ogl.OglNote import OglNote
+from ogl.OglText import OglText
 from ogl.OglLink import OglLink
+from ogl.OglNoteLink import OglNoteLink
 from ogl.OglClass import OglClass
 from ogl.OglInterface2 import OglInterface2
 from ogl.OglAggregation import OglAggregation
 from ogl.OglInheritance import OglInheritance
 from ogl.OglComposition import OglComposition
 from ogl.OglAssociation import OglAssociation
 from ogl.OglInterface import OglInterface
@@ -84,23 +90,38 @@
 
         for oglObject in oglObjects:
             match oglObject:
                 case OglClass():
                     oglClass:  OglClass  = cast(OglClass, oglObject)
                     generatedString: str = self._generateClassStanza(oglClass)
                     mermaidString += f'{generatedString}'
+                case OglNote():
+                    pass
+                case OglText():
+                    oglText: OglText = cast(OglText, oglObject)
+                    generatedString = self._mermaidStandaloneNoteStanza(oglText)
+                    mermaidString += f'{generatedString}'
                 case OglLink():
                     pass
                 case _:
                     self.logger.warning(f'Unsupported Ogl element: {oglObject}')
 
         mermaidString += f'```{eol}'
         with self._fqFileName.open(mode='a') as fd:
             fd.write(f'{mermaidString}')
 
+    def _mermaidStandaloneNoteStanza(self, oglText: OglText) -> str:
+
+        pyutText: PyutText = oglText.pyutObject
+        generatedString: str = (
+            f'{indent1}note "{pyutText.content}"{eol}'
+        )
+
+        return generatedString
+
     def _generateClassStanza(self, oglObject: OglClass) -> str:
         """
 
         Args:
             oglObject:  A Pyut Class Definition
 
         Returns:  A Mermaid class definition
@@ -148,25 +169,63 @@
                     linkRefrain = self._getAssociationLinkRefrain(oglAssociation=oglAggregation, arrowType=MermaidArrow.AGGREGATION_LINK)
                 case OglComposition():
                     oglComposition: OglComposition = cast(OglComposition, oglObject)
                     linkRefrain = self._getAssociationLinkRefrain(oglAssociation=oglComposition, arrowType=MermaidArrow.COMPOSITION_LINK)
                 case OglInterface():
                     oglInterface: OglInterface = cast(OglInterface, oglObject)
                     linkRefrain = self._getRealizationLinkRefrain(oglInterface)
+                case OglNoteLink():
+                    oglNoteLink: OglNoteLink = cast(OglNoteLink, oglObject)
+                    linkRefrain = self._getNoteLinkRefrain(oglNoteLink)
                 case OglAssociation():      # Most general needs to be last
                     oglAssociation: OglAssociation = cast(OglAssociation, oglObject)
                     linkRefrain = self._getAssociationLinkRefrain(oglAssociation=oglAssociation, arrowType=MermaidArrow.ASSOCIATION_LINK)
                 case OglInterface2():
-                    pass
+                    self.logger.warning(f'OglInterface2 (lollipops) not supported in Mermaid')
                 case _:
                     pass        # Ignore non links
             linksStanza += linkRefrain
 
         return linksStanza
 
+    def _getInheritanceLinkRefrain(self, oglLink: OglLink) -> str:
+        """
+        Produces strings of the form:
+
+        Animal<|--Duck
+
+        Where Animal is the parent class and Duck is the subclass
+
+        Args:
+            oglLink:  The inheritance link
+
+        Returns:  Mermaid string for inheritance
+        """
+        pyutLink: PyutLink = oglLink.pyutObject
+
+        subClassName:  str = pyutLink.getSource().name
+        baseClassName: str = pyutLink.getDestination().name
+        self.logger.info(f'{subClassName=} {pyutLink.linkType=} {baseClassName=}')
+
+        linkRefrain: str  = (
+            f'{indent1}{baseClassName}{MermaidArrow.INHERITANCE_ARROW.value}{subClassName}{eol}'
+        )
+
+        return linkRefrain
+
+    def _getRealizationLinkRefrain(self, oglInterface: OglInterface) -> str:
+        pyutLink: PyutLink = oglInterface.pyutObject
+        interfaceName:   str = pyutLink.getSource().name
+        implementorName: str = pyutLink.getDestination().name
+        linkRefrain: str = (
+            f'{indent1}{interfaceName} {MermaidArrow.INTERFACE_LINK.value} {implementorName}{eol}'
+        )
+
+        return linkRefrain
+
     def _getAssociationLinkRefrain(self, oglAssociation: OglAssociation, arrowType: MermaidArrow) -> str:
         """
         For Composition and Aggregation the diamond is on the source side
         Produces refrains of the form:
 
         For composition:
         Person "1" *-- "1" Heart
@@ -187,52 +246,33 @@
         """
         pyutLink: PyutLink = oglAssociation.pyutObject
         sourceName:      str = pyutLink.getSource().name
         destinationName: str = pyutLink.getDestination().name
         self.logger.info(f'{oglAssociation} {sourceName=} {destinationName=}')
 
         sourceCardinality, destinationCardinality = self._getCardinalityStrings(pyutLink)
-        linkRefrain = (
+        linkRefrain: str = (
             f'{indent1}{sourceName} {sourceCardinality} {arrowType.value} {destinationCardinality} {destinationName} : {pyutLink.name}{eol}'
         )
         return linkRefrain
 
-    def _getInheritanceLinkRefrain(self, oglLink: OglLink) -> str:
+    def _getNoteLinkRefrain(self, oglNoteLink: OglNoteLink) -> str:
         """
-        Produces strings of the form:
-
-        Animal<|--Duck
-
-        Where Animal is the parent class and Duck is the subclass
 
         Args:
-            oglLink:  The inheritance link
+            oglNoteLink: The note link
 
-        Returns:  Mermaid string for inheritance
+        Returns:  Mermaid string for a note link
         """
-        pyutLink: PyutLink = oglLink.pyutObject
-
-        subClassName:  str = pyutLink.getSource().name
-        baseClassName: str = pyutLink.getDestination().name
-        self.logger.info(f'{subClassName=} {pyutLink.linkType=} {baseClassName=}')
-
-        linkRefrain: str  = (
-            f'{indent1}{baseClassName}{MermaidArrow.INHERITANCE_ARROW.value}{subClassName}{eol}'
-        )
-
-        return linkRefrain
-
-    def _getRealizationLinkRefrain(self, oglInterface: OglInterface) -> str:
-        pyutLink: PyutLink = oglInterface.pyutObject
-        interfaceName:   str = pyutLink.getSource().name
-        implementorName: str = pyutLink.getDestination().name
+        pyutLink:  PyutLink          = oglNoteLink.pyutObject
+        destObject: PyutLinkedObject = pyutLink.getDestination()
+        pyutNote:   PyutNote         = pyutLink.getSource()
         linkRefrain: str = (
-            f'{indent1}{interfaceName} {MermaidArrow.INTERFACE_LINK.value} {implementorName}{eol}'
+            f'{indent1}note for {destObject.name} "{pyutNote.content}"{eol}'
         )
-
         return linkRefrain
 
     def _getCardinalityStrings(self, pyutLink) -> Tuple[str, str]:
         """
 
         Args:
             pyutLink:
```

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/pdf/OglToPyUmlDefinition.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/Python3LexerBase.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/Python3LexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/PyutPythonVisitor.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/PyutPythonVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/ReverseEngineerPython2.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/ReverseEngineerPython2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserListener.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/pyantlrparser/Python3ParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/python/transformGrammar.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/python/transformGrammar.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-0.8.50/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-0.8.50/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-0.8.50/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-0.8.50/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-0.8.50/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-0.8.50/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-0.8.50/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-0.8.50/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-0.8.50/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/ToolAscii.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/ToolAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-0.8.50/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-0.8.50/pyutplugins.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7574  : 2.1.Name: pyut
 00000020: 706c 7567 696e 730a 5665 7273 696f 6e3a  plugins.Version:
-00000030: 2030 2e38 2e34 320a 5375 6d6d 6172 793a   0.8.42.Summary:
+00000030: 2030 2e38 2e35 300a 5375 6d6d 6172 793a   0.8.50.Summary:
 00000040: 2050 7975 7420 506c 7567 696e 730a 486f   Pyut Plugins.Ho
 00000050: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000060: 2f67 6974 6875 622e 636f 6d2f 6861 7369  /github.com/hasi
 00000070: 6932 3031 312f 7079 7574 706c 7567 696e  i2011/pyutplugin
 00000080: 730a 4175 7468 6f72 3a20 4875 6d62 6572  s.Author: Humber
 00000090: 746f 2041 2e20 5361 6e63 6865 7a20 4949  to A. Sanchez II
 000000a0: 0a41 7574 686f 722d 656d 6169 6c3a 2068  .Author-email: h
@@ -68,64 +68,78 @@
 00000430: 7254 6865 4261 6467 652e 636f 6d2f 696d  rTheBadge.com/im
 00000440: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
 00000450: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
 00000460: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
 00000470: 7974 686f 6e2e 6f72 672f 290a 0a0a 2320  ython.org/)...# 
 00000480: 496e 7472 6f64 7563 7469 6f6e 0a2a 2a54  Introduction.**T
 00000490: 4244 2a2a 0a0a 2320 4f76 6572 7669 6577  BD**..# Overview
-000004a0: 0a0a 2a2a 5442 442a 2a0a 0a2d 2d2d 2d2d  ..**TBD**..-----
-000004b0: 2d0a 0a55 7365 6420 746f 2062 6520 6361  -..Used to be ca
-000004c0: 6c6c 6564 2070 7975 7470 6c75 6769 6e63  lled pyutpluginc
-000004d0: 6f72 650a 0a21 5b48 756d 6265 7274 6f27  ore..![Humberto'
-000004e0: 7320 4d6f 6469 6669 6564 204c 6f67 6f5d  s Modified Logo]
-000004f0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000500: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000510: 6f6d 2f77 696b 692f 6861 7369 6932 3031  om/wiki/hasii201
-00000520: 312f 6769 7474 6f64 6f69 7374 636c 6f6e  1/gittodoistclon
-00000530: 652f 696d 6167 6573 2f53 696c 6c79 4769  e/images/SillyGi
-00000540: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
-00000550: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
-00000560: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
-00000570: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
-00000580: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
-00000590: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
-000005a0: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
-000005b0: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
-000005c0: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
-000005d0: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
-000005e0: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
-000005f0: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
-00000600: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
-00000610: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
-00000620: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
-00000630: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
-00000640: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
-00000650: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
-00000660: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
-00000670: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
-00000680: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
-00000690: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
-000006a0: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
-000006b0: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
-000006c0: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
-000006d0: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
-000006e0: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
-000006f0: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
-00000700: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
-00000710: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
-00000720: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
-00000730: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
-00000740: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
-00000750: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
-00000760: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
-00000770: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
-00000780: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
-00000790: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
-000007a0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-000007b0: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
-000007c0: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
-000007d0: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
-000007e0: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
-000007f0: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
-00000800: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
-00000810: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
-00000820: 6e65 2073 6f2e 0a                        ne so..
+000004a0: 0a0a 2a2a 5442 442a 2a0a 0a23 2320 4465  ..**TBD**..## De
+000004b0: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+000004c0: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+000004d0: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+000004e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004f0: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+00000500: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+00000510: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+00000520: 6e74 2062 7569 6c64 730a 0a5f 5f5f 0a0a  nt builds..___..
+00000530: 5772 6974 7465 6e20 6279 203c 6120 6872  Written by <a hr
+00000540: 6566 3d22 6d61 696c 746f 3a65 6d61 696c  ef="mailto:email
+00000550: 4068 756d 6265 7274 6f2e 612e 7361 6e63  @humberto.a.sanc
+00000560: 6865 7a2e 6969 4067 6d61 696c 2e63 6f6d  hez.ii@gmail.com
+00000570: 3f73 7562 6a65 6374 3d48 656c 6c6f 2048  ?subject=Hello H
+00000580: 756d 6265 7274 6f22 3e48 756d 6265 7274  umberto">Humbert
+00000590: 6f20 412e 2053 616e 6368 657a 2049 493c  o A. Sanchez II<
+000005a0: 2f61 3e20 2028 4329 2032 3032 330a 0a5f  /a>  (C) 2023.._
+000005b0: 5f5f 0a0a 0a21 5b48 756d 6265 7274 6f27  __...![Humberto'
+000005c0: 7320 4d6f 6469 6669 6564 204c 6f67 6f5d  s Modified Logo]
+000005d0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+000005e0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000005f0: 6f6d 2f77 696b 692f 6861 7369 6932 3031  om/wiki/hasii201
+00000600: 312f 6769 7474 6f64 6f69 7374 636c 6f6e  1/gittodoistclon
+00000610: 652f 696d 6167 6573 2f53 696c 6c79 4769  e/images/SillyGi
+00000620: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
+00000630: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
+00000640: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
+00000650: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
+00000660: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
+00000670: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
+00000680: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
+00000690: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
+000006a0: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
+000006b0: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
+000006c0: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
+000006d0: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
+000006e0: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
+000006f0: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
+00000700: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
+00000710: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
+00000720: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
+00000730: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
+00000740: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
+00000750: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
+00000760: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
+00000770: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
+00000780: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
+00000790: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
+000007a0: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
+000007b0: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
+000007c0: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
+000007d0: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
+000007e0: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
+000007f0: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
+00000800: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
+00000810: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
+00000820: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
+00000830: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
+00000840: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
+00000850: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
+00000860: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
+00000870: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
+00000880: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
+00000890: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
+000008a0: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
+000008b0: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
+000008c0: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
+000008d0: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
+000008e0: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
+000008f0: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
+00000900: 6e65 2073 6f2e 0a                        ne so..
```

### Comparing `pyutplugins-0.8.42/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-0.8.50/pyutplugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutplugins-0.8.42/setup.py` & `pyutplugins-0.8.50/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="pyutplugins",
-    version="0.8.42",
+    version="0.8.50",
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Pyut Plugins',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -55,15 +55,15 @@
     ],
     install_requires=[
                       'antlr4-python3-runtime==4.11.1',
                       'pyumldiagrams==2.30.8',
                       'networkx==3.0',
                       'orthogonal==1.1.8',
                       'wxPython~=4.2.0',
-                      'hasiihelper~=0.1.0',
-                      'hasiicommon~=0.2.1',
-                      'pyutmodel==1.4.2',
-                      'ogl==0.70.22',
-                      'untanglepyut==0.6.41',
-                      'oglio==0.6.0',
+                      'hasiihelper~=0.2.0',
+                      'hasiicommon~=0.2.2',
+                      'pyutmodel==1.4.3',
+                      'ogl==0.70.26',
+                      'untanglepyut==0.6.50',
+                      'oglio==0.7.1',
                       ]
 )
```

