# Comparing `tmp/via-hub-logistc-1.0.0.tar.gz` & `tmp/via-hub-logistc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-hub-logistc-1.0.0.tar", max compression
+gzip compressed data, was "via-hub-logistc-1.0.1.tar", max compression
```

## Comparing `via-hub-logistc-1.0.0.tar` & `via-hub-logistc-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      434 2023-04-14 13:29:22.164363 via-hub-logistc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7347 2023-04-12 22:34:20.470829 via-hub-logistc-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-1.0.0/via_hub_logistc/__init__.py
--rw-r--r--   0        0        0      396 2023-04-12 22:34:20.479827 via-hub-logistc-1.0.0/via_hub_logistc/core/via_file.py
--rw-r--r--   0        0        0      276 2023-04-12 22:34:20.482829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_number.py
--rw-r--r--   0        0        0     9591 2023-04-04 16:49:43.006120 via-hub-logistc-1.0.0/via_hub_logistc/core/via_report.py
--rw-r--r--   0        0        0      418 2023-04-12 22:34:20.485828 via-hub-logistc-1.0.0/via_hub_logistc/core/via_scenario.py
--rw-r--r--   0        0        0      549 2023-04-12 22:34:20.487829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_text.py
--rw-r--r--   0        0        0      599 2023-04-12 22:34:20.490829 via-hub-logistc-1.0.0/via_hub_logistc/core/via_timer.py
--rw-r--r--   0        0        0     1097 2023-04-12 17:18:04.992073 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_db2.py
--rw-r--r--   0        0        0     1888 2023-04-12 17:18:43.091789 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_microsoft.py
--rw-r--r--   0        0        0     1664 2023-04-12 17:19:00.638957 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_mongodb.py
--rw-r--r--   0        0        0      307 2023-04-04 15:39:11.800307 via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_text.py
--rw-r--r--   0        0        0     1143 2023-03-06 17:06:38.522855 via-hub-logistc-1.0.0/via_hub_logistc/model/zephry.py
--rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.0/setup.py
--rw-r--r--   0        0        0     7514 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-04-18 20:56:57.516414 via-hub-logistc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7703 2023-04-18 20:56:48.040816 via-hub-logistc-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-1.0.1/via_hub_logistc/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-12 22:34:20.479827 via-hub-logistc-1.0.1/via_hub_logistc/core/via_file.py
+-rw-r--r--   0        0        0      276 2023-04-12 22:34:20.482829 via-hub-logistc-1.0.1/via_hub_logistc/core/via_number.py
+-rw-r--r--   0        0        0     9591 2023-04-04 16:49:43.006120 via-hub-logistc-1.0.1/via_hub_logistc/core/via_report.py
+-rw-r--r--   0        0        0      418 2023-04-12 22:34:20.485828 via-hub-logistc-1.0.1/via_hub_logistc/core/via_scenario.py
+-rw-r--r--   0        0        0      549 2023-04-12 22:34:20.487829 via-hub-logistc-1.0.1/via_hub_logistc/core/via_text.py
+-rw-r--r--   0        0        0      599 2023-04-12 22:34:20.490829 via-hub-logistc-1.0.1/via_hub_logistc/core/via_timer.py
+-rw-r--r--   0        0        0     1097 2023-04-12 17:18:04.992073 via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_db2.py
+-rw-r--r--   0        0        0     1888 2023-04-12 17:18:43.091789 via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_microsoft.py
+-rw-r--r--   0        0        0     2103 2023-04-18 20:55:26.838948 via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_mongodb.py
+-rw-r--r--   0        0        0      307 2023-04-04 15:39:11.800307 via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_text.py
+-rw-r--r--   0        0        0     1143 2023-03-06 17:06:38.522855 via-hub-logistc-1.0.1/via_hub_logistc/model/zephry.py
+-rw-r--r--   0        0        0     8424 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.1/setup.py
+-rw-r--r--   0        0        0     7863 1970-01-01 00:00:00.000000 via-hub-logistc-1.0.1/PKG-INFO
```

### Comparing `via-hub-logistc-1.0.0/README.md` & `via-hub-logistc-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,21 @@
 	  > Returns one json or list the json result by parameter <br>
     > Params:<br>
     > - **client**: connection :: *Connection*<br>
     > - **baseName**: name the database :: *str*<br>
     > - **collectionName**: name the collection:: *str*<br>
     > - **query**: Query which will be used in the search:: *dict*<br>
 
+  - Mongo Find One By Parameter
+	  > Returns one json or list the json result by parameter <br>
+    > Params:<br>
+    > - **client**: connection :: *Connection*<br>
+    > - **baseName**: name the database :: *str*<br>
+    > - **collectionName**: name the collection:: *str*<br>
+    > - **query**: Query which will be used in the search:: *dict*<br>
 
 **Mongodb**
 
   ```robotframework
     *** Settings***
     $  Library    via_hub_logistc.keywords.kws_text.ViaText
   ```
```

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/core/via_report.py` & `via-hub-logistc-1.0.1/via_hub_logistc/core/via_report.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/core/via_text.py` & `via-hub-logistc-1.0.1/via_hub_logistc/core/via_text.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/core/via_timer.py` & `via-hub-logistc-1.0.1/via_hub_logistc/core/via_timer.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_db2.py` & `via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_db2.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_microsoft.py` & `via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_microsoft.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/keyword/kws_mongodb.py` & `via-hub-logistc-1.0.1/via_hub_logistc/keyword/kws_mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,7 +49,20 @@
             dataBase = client[baseName]
 
             collection = dataBase[collectionName]
 
             return collection.find(query)
         except Exception as e:
             raise Error(e)
+
+### Returns one json or list the json result by parameter ###
+    @keyword(name="Mongo Find One By Parameter")
+    def mongo_find_one_by_parameter(self, client, baseName:str, collectionName:str, query:str):
+        try:
+            dataBase = client[baseName]
+
+            collection = dataBase[collectionName]
+
+            return collection.find_one(query)
+        
+        except Exception as e:
+            raise Error(e)
```

### Comparing `via-hub-logistc-1.0.0/via_hub_logistc/model/zephry.py` & `via-hub-logistc-1.0.1/via_hub_logistc/model/zephry.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-1.0.0/setup.py` & `via-hub-logistc-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
  'via_hub_logistc.model']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'via-hub-logistc',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'This project is intended to be a facilitator for new developments for test automation',
-    'long_description': '# Biblioteca customizada para testes automatizados com robotframework\n\nA finalidade deste documento é a de passar informações das funções e keywords que estão sendo entregues.\n\n## 🔧 Instalação\n\t$ pip install via-hub-logistic\n\n## 🚀 Keywords:\n**Microsoft Azure**\n\n  ```robotframework\n    *** Settings ***\n    $  Library    via_hub_logistc.keywords.kws_microsoft.ViaAzure\n  ```\n  - Azure Connect Blob Server\n\t  > Return the one object connction with azure blob server<br>\n    > Params:<br>\n    > - **host**: Url blob server :: *str*<br> \n    > - **account_name**: name user the account :: *str*<br>\n    > -  **account_key**: access token the account :: *str*\n\n  - Azure List All Directories In Container\n\t  > Return the json with all directories in a container<br>\n    > Params:<br>\n    > - **connection**: Object with connection :: *Connection*<br> \n    > - **container_name**: name container :: *str*<br>\n    > - **folder**: name the folder :: *str*<br>\n    > - **format**: Default false for return o path name the folder, true for return o full path name with folder :: *boolean*\n\n  - Azure Is Exist Directory In Container\n\t  > Return  True if the folder exists in the container or False if the folder not exist in container<br>\n    > Params:<br>\n    > - **connection**: Object with connection :: *Connection*<br>\n    > - **container_name**:  name container :: *str*<br>\n    > - **folder**:  name the folder :: *str*<br>\n    > - **directory**:  diectory search :: *srt*\n\n\n**Ibm Db2**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_db2.ViaDb2\n  ```\n  - Db2 Connect To Dataase\n\t  > Return the one object connction with database bd2 server<br>\n    > Params:<br>\n    > - **host**:  server name :: *str*<br>\n    > - **db_name**:  database name :: *str*<br>\n    > - **user_id**:  user name :: *str*<br>\n    > - **password**:  password id :: *str*\n\n  - Db2 Execute Qury\n\t  > Return json with result the of query <br>\n    > Params:<br>\n    > - **connection**: Object with connection the of database :: *Connection*<br>\n    > - **query**:  Query which will be used in the search :: *str*\n\n\n**Mongodb**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_mongodb.ViaMongo\n  ```\n  - Mongo Connect To Database\n\t  > Return conncection with mongoDB<br>\n    > Params:<br>\n    > - **strConnction**:  string connection :: *str*<br>\n\n  - Mongo Disconnect To Database\n\t  > Execute a disconnection with the server <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n\n  - Mongo Find All\n\t  > Returns one json or list the json result <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n    > - **baseName**: name the database :: *str*<br>\n    > - **collectionName**: name the collection:: *str*<br>\n\n  - Mongo Find By Parameter\n\t  > Returns one json or list the json result by parameter <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n    > - **baseName**: name the database :: *str*<br>\n    > - **collectionName**: name the collection:: *str*<br>\n    > - **query**: Query which will be used in the search:: *dict*<br>\n\n\n**Mongodb**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_text.ViaText\n  ```\n  - Split Text\n\t  > Return text divide<br>\n    > Params:<br>\n    > - **text**:  text :: *str*<br>\n    > - **lengh**:  size limit caracteres :: *int*<br>\n\n## 🚀 Funcoes:\n**Arquivos**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_file.FileYaml\n  ```\n  - read_yaml_file\n\t  > Return json with data file yaml<br>\n    > Params:<br>\n    > - **filename**:  path the file :: *str*<br>\n\n**Number**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_number.ViaNumber\n  ```\n  - choose_number\n\t  > Return Choose number in range<br>\n    > Params:<br>\n    > - **stopNumber**:  number final the range :: *int*<br>\n  \n**Text**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_text.ViaNumber\n  ```\n  - split_text\n\t  > Return split text informations $text and $length cut<br>\n    > Params:<br>\n    > - **text**:  text :: *int*<br>\n    > - **length**:  size the cut the text :: *int*<br>\n\n  - cut_text\n\t  > Return cut text informations $separator and $length cut<br>\n    > Params:<br>\n    > - **text**:  text :: *int*<br>\n    > - **separator**:  caracterer separator :: *int*<br>\n    > - **maxsplit**:  size the cut the text :: *int*<br>\n\n**Timer**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_timer.ViaTimer\n  ```\n  - interval\n\t  > Return calculate date in two date<br>\n    > Params:<br>\n    > - **start**:  date start :: *int*<br>\n    > - **end**:  date end :: *int*<br>\n\n  - str_to_date\n\t  > Return on a date in format string<br>\n    > Params:<br>\n    > - **value**:  date  :: *int*<br>\n    > - **format**:  date format :: *int*<br>\n\n**Scenarios**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_scenarios.ViaTimer\n  ```\n  - get_id_scenario\n\t  > Return id the scenarios<br>\n    > Params:<br>\n    > - **lst_tags**:  date start :: *list*<br>\n    > - **tag_id**: tag id for load in list :: *int*<br>\n\n\n**Conector Zephry**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_report.ReportManager\n  ```\n  - get_cycle_id\n\t  > Return id the of cycle in jira<br>\n    > Params:<br>\n    > - **cycle**: cycle name :: *list*<br>\n\n  - create_cycle_name\n\t  > Return name the of cycle test in jira<br>\n    > Params:<br>\n    > - **project_id**: id project jira :: *list*<br>\n    > - **release**: name the branch the regression :: *list*<br>\n\n  - create_folder\n\t  > Return name new folder for test regression<br>\n    > Params:<br>\n    > - **projectKey**: key project jira :: *list*<br>\n    > - **folder_name**: name the folder the regression :: *list*<br>\n\n  - create_cycle_test\n\t  > Return new cycle for test regression<br>\n    > Params:<br>\n    > - **folder_name**: name the folder the regression :: *str*<br>\n    > - **test_plan**: id test plan:: *str*<br>\n    > - **key**: key the project :: *str*<br>\n    > - **name_cycle**: name the cycle the regression :: *str*<br>\n    > - **descripption**: description the cycle the regression :: *str*<br>\n    > - **iteration**: iteration the cycle the regression :: *str*<br>\n    > - **owner**: name the of runner the regression :: *str*<br>\n    > - **cycle_date**: date the cycle the regression :: *str*<br>\n    > - **status**: status the cycle the regression :: *str*<br>\n\n  - save_result_runner_tests\n\t  > Add scenarios to an existing cycle <br>\n    > Params:<br>\n    > - **cycle**: cycle the runner regression :: *str*<br>\n    > - **list_scenarios**: list with scenarios :: *list*<br>\n\n  - get_owner_test_case\n\t  > Return Get info the of created test case<br>\n    > Params:<br>\n    > - **test_key**: name teste case :: *str*<br>\n\n  - update_cycle_execution\n\t  > Change status upadate cycle test br>\n    > Params:<br>\n    > - **project_id**: id project the jira :: *str*<br>\n    > - **cycle_id**: id cycle :: *str*<br>\n    > - **status**: status the execution :: *str*<br>',
+    'long_description': '# Biblioteca customizada para testes automatizados com robotframework\n\nA finalidade deste documento é a de passar informações das funções e keywords que estão sendo entregues.\n\n## 🔧 Instalação\n\t$ pip install via-hub-logistic\n\n## 🚀 Keywords:\n**Microsoft Azure**\n\n  ```robotframework\n    *** Settings ***\n    $  Library    via_hub_logistc.keywords.kws_microsoft.ViaAzure\n  ```\n  - Azure Connect Blob Server\n\t  > Return the one object connction with azure blob server<br>\n    > Params:<br>\n    > - **host**: Url blob server :: *str*<br> \n    > - **account_name**: name user the account :: *str*<br>\n    > -  **account_key**: access token the account :: *str*\n\n  - Azure List All Directories In Container\n\t  > Return the json with all directories in a container<br>\n    > Params:<br>\n    > - **connection**: Object with connection :: *Connection*<br> \n    > - **container_name**: name container :: *str*<br>\n    > - **folder**: name the folder :: *str*<br>\n    > - **format**: Default false for return o path name the folder, true for return o full path name with folder :: *boolean*\n\n  - Azure Is Exist Directory In Container\n\t  > Return  True if the folder exists in the container or False if the folder not exist in container<br>\n    > Params:<br>\n    > - **connection**: Object with connection :: *Connection*<br>\n    > - **container_name**:  name container :: *str*<br>\n    > - **folder**:  name the folder :: *str*<br>\n    > - **directory**:  diectory search :: *srt*\n\n\n**Ibm Db2**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_db2.ViaDb2\n  ```\n  - Db2 Connect To Dataase\n\t  > Return the one object connction with database bd2 server<br>\n    > Params:<br>\n    > - **host**:  server name :: *str*<br>\n    > - **db_name**:  database name :: *str*<br>\n    > - **user_id**:  user name :: *str*<br>\n    > - **password**:  password id :: *str*\n\n  - Db2 Execute Qury\n\t  > Return json with result the of query <br>\n    > Params:<br>\n    > - **connection**: Object with connection the of database :: *Connection*<br>\n    > - **query**:  Query which will be used in the search :: *str*\n\n\n**Mongodb**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_mongodb.ViaMongo\n  ```\n  - Mongo Connect To Database\n\t  > Return conncection with mongoDB<br>\n    > Params:<br>\n    > - **strConnction**:  string connection :: *str*<br>\n\n  - Mongo Disconnect To Database\n\t  > Execute a disconnection with the server <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n\n  - Mongo Find All\n\t  > Returns one json or list the json result <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n    > - **baseName**: name the database :: *str*<br>\n    > - **collectionName**: name the collection:: *str*<br>\n\n  - Mongo Find By Parameter\n\t  > Returns one json or list the json result by parameter <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n    > - **baseName**: name the database :: *str*<br>\n    > - **collectionName**: name the collection:: *str*<br>\n    > - **query**: Query which will be used in the search:: *dict*<br>\n\n  - Mongo Find One By Parameter\n\t  > Returns one json or list the json result by parameter <br>\n    > Params:<br>\n    > - **client**: connection :: *Connection*<br>\n    > - **baseName**: name the database :: *str*<br>\n    > - **collectionName**: name the collection:: *str*<br>\n    > - **query**: Query which will be used in the search:: *dict*<br>\n\n**Mongodb**\n\n  ```robotframework\n    *** Settings***\n    $  Library    via_hub_logistc.keywords.kws_text.ViaText\n  ```\n  - Split Text\n\t  > Return text divide<br>\n    > Params:<br>\n    > - **text**:  text :: *str*<br>\n    > - **lengh**:  size limit caracteres :: *int*<br>\n\n## 🚀 Funcoes:\n**Arquivos**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_file.FileYaml\n  ```\n  - read_yaml_file\n\t  > Return json with data file yaml<br>\n    > Params:<br>\n    > - **filename**:  path the file :: *str*<br>\n\n**Number**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_number.ViaNumber\n  ```\n  - choose_number\n\t  > Return Choose number in range<br>\n    > Params:<br>\n    > - **stopNumber**:  number final the range :: *int*<br>\n  \n**Text**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_text.ViaNumber\n  ```\n  - split_text\n\t  > Return split text informations $text and $length cut<br>\n    > Params:<br>\n    > - **text**:  text :: *int*<br>\n    > - **length**:  size the cut the text :: *int*<br>\n\n  - cut_text\n\t  > Return cut text informations $separator and $length cut<br>\n    > Params:<br>\n    > - **text**:  text :: *int*<br>\n    > - **separator**:  caracterer separator :: *int*<br>\n    > - **maxsplit**:  size the cut the text :: *int*<br>\n\n**Timer**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_timer.ViaTimer\n  ```\n  - interval\n\t  > Return calculate date in two date<br>\n    > Params:<br>\n    > - **start**:  date start :: *int*<br>\n    > - **end**:  date end :: *int*<br>\n\n  - str_to_date\n\t  > Return on a date in format string<br>\n    > Params:<br>\n    > - **value**:  date  :: *int*<br>\n    > - **format**:  date format :: *int*<br>\n\n**Scenarios**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_scenarios.ViaTimer\n  ```\n  - get_id_scenario\n\t  > Return id the scenarios<br>\n    > Params:<br>\n    > - **lst_tags**:  date start :: *list*<br>\n    > - **tag_id**: tag id for load in list :: *int*<br>\n\n\n**Conector Zephry**\n\n  ```Pytho\n    *** Settings***\n    $ Library    via_hub_logistc.core.via_report.ReportManager\n  ```\n  - get_cycle_id\n\t  > Return id the of cycle in jira<br>\n    > Params:<br>\n    > - **cycle**: cycle name :: *list*<br>\n\n  - create_cycle_name\n\t  > Return name the of cycle test in jira<br>\n    > Params:<br>\n    > - **project_id**: id project jira :: *list*<br>\n    > - **release**: name the branch the regression :: *list*<br>\n\n  - create_folder\n\t  > Return name new folder for test regression<br>\n    > Params:<br>\n    > - **projectKey**: key project jira :: *list*<br>\n    > - **folder_name**: name the folder the regression :: *list*<br>\n\n  - create_cycle_test\n\t  > Return new cycle for test regression<br>\n    > Params:<br>\n    > - **folder_name**: name the folder the regression :: *str*<br>\n    > - **test_plan**: id test plan:: *str*<br>\n    > - **key**: key the project :: *str*<br>\n    > - **name_cycle**: name the cycle the regression :: *str*<br>\n    > - **descripption**: description the cycle the regression :: *str*<br>\n    > - **iteration**: iteration the cycle the regression :: *str*<br>\n    > - **owner**: name the of runner the regression :: *str*<br>\n    > - **cycle_date**: date the cycle the regression :: *str*<br>\n    > - **status**: status the cycle the regression :: *str*<br>\n\n  - save_result_runner_tests\n\t  > Add scenarios to an existing cycle <br>\n    > Params:<br>\n    > - **cycle**: cycle the runner regression :: *str*<br>\n    > - **list_scenarios**: list with scenarios :: *list*<br>\n\n  - get_owner_test_case\n\t  > Return Get info the of created test case<br>\n    > Params:<br>\n    > - **test_key**: name teste case :: *str*<br>\n\n  - update_cycle_execution\n\t  > Change status upadate cycle test br>\n    > Params:<br>\n    > - **project_id**: id project the jira :: *str*<br>\n    > - **cycle_id**: id cycle :: *str*<br>\n    > - **status**: status the execution :: *str*<br>',
     'author': 'Jaderson Macedo',
     'author_email': 'jaderson.macedo@viavarejo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `via-hub-logistc-1.0.0/PKG-INFO` & `via-hub-logistc-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: via-hub-logistc
-Version: 1.0.0
+Version: 1.0.1
 Summary: This project is intended to be a facilitator for new developments for test automation
 Author: Jaderson Macedo
 Author-email: jaderson.macedo@viavarejo.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -95,14 +95,21 @@
 	  > Returns one json or list the json result by parameter <br>
     > Params:<br>
     > - **client**: connection :: *Connection*<br>
     > - **baseName**: name the database :: *str*<br>
     > - **collectionName**: name the collection:: *str*<br>
     > - **query**: Query which will be used in the search:: *dict*<br>
 
+  - Mongo Find One By Parameter
+	  > Returns one json or list the json result by parameter <br>
+    > Params:<br>
+    > - **client**: connection :: *Connection*<br>
+    > - **baseName**: name the database :: *str*<br>
+    > - **collectionName**: name the collection:: *str*<br>
+    > - **query**: Query which will be used in the search:: *dict*<br>
 
 **Mongodb**
 
   ```robotframework
     *** Settings***
     $  Library    via_hub_logistc.keywords.kws_text.ViaText
   ```
```

