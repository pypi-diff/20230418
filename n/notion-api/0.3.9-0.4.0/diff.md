# Comparing `tmp/notion_api-0.3.9.tar.gz` & `tmp/notion_api-0.4.0.tar.gz`

## Comparing `notion_api-0.3.9.tar` & `notion_api-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 notion_api-0.3.9/README.md
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/py.typed
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/_about.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/_pkgv.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/blockmixin.py
--rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/blocktypefactory.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/client.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/notionblock.py
--rw-r--r--   0        0        0    19574 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    17575 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/notionpage.py
--rw-r--r--   0        0        0    18078 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/api/notionworkspace.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/__init__.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/build.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/common.py
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/files.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/options.py
--rw-r--r--   0        0        0    14887 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/properties/richtext.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/conditions.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.3.9/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.3.9/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.3.9/LICENSE
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 notion_api-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 notion_api-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 notion_api-0.4.0/README.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/py.typed
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/_about.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/blockmixin.py
+-rw-r--r--   0        0        0    20946 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/blocktypefactory.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/client.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionblock.py
+-rw-r--r--   0        0        0    25778 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20082 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionpage.py
+-rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/__init__.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/build.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/common.py
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/options.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/compound.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/conditions.py
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/sort.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.4.0/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 notion_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 notion_api-0.4.0/PKG-INFO
```

### Comparing `notion_api-0.3.9/README.md` & `notion_api-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,169 +9,194 @@
     &nbsp;
     <img alt="last commit" src="https://img.shields.io/github/last-commit/ayvi-0001/notion-api?color=%239146ff"></a>
     &nbsp;
     <a href="https://developers.notion.com/reference/versioning"><img alt="notion versioning" src="https://img.shields.io/static/v1?label=notion-API-version&message=2022-06-28&color=%232e1a00"></a>
     &nbsp;
 </p>
 <p align="center">
-    <a href="https://github.com/ayvi-0001/notion-api/blob/main/LICENSE"><img alt="license: MIT" src="https://img.shields.io/static/v1?label=license&message=MIT&color=informational"></a>
+    <a href="https://github.com/ayvi-0001/notion-api/blob/main/LICENSE"><img alt="license: MIT" src="https://img.shields.io/github/license/ayvi-0001/notion-api?color=informational"></a>
     &nbsp;
     <a href="https://github.com/psf/black"><img alt="code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     &nbsp;
     <a href="https://pycqa.github.io/isort/"><img alt="code style: black" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
+A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion. This project is still a work in progress, and features will continue to change. Below are a few examples of the current functionality. 
+
+<br>
+
 <div border="0" align="center">
     <table>
         <tr>
-            <td align="center"><b>A few useful links:</b></td>
+            <td align="center"><b>Links: Notion API Updates</b></td>
         </tr>
             <td> <a href="https://developers.notion.com/reference/intro">API Reference</a></td><tr>
         </td>
-            <td><a href="https://developers.notion.com/page/changelog">Notion API Changlog </img></a></tr>
+            <td><a href="https://developers.notion.com/page/changelog">Notion API Changelog </img></a></tr>
             <td> <a href="https://www.notion.so/releases">Notion.so Releases</a></td></tr>
             <td> <a href="https://developers.notion.com/page/notion-platform-roadmap">Notion Platform Roadmap</a></td>
         </tr>
     </table>
 </div>
 
-<br>
-
-
-A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
-
-This project is still a work in progress, and features will continue to change. Below are a few examples of the current functionality. 
+---
 
-# Install
+## Install
 ```
 pip install -U notion-api
 ```
 
-# Usage
+## Usage
 ```py
 import dotenv
 
 import notion
 
-dotenv.load_dotenv()  # client will check for env variable 'NOTION_TOKEN'.
+# client will check env variables for 'NOTION_TOKEN'
+dotenv.load_dotenv()  
 
 homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
 parent_db = notion.Database(homepage.parent_id)
 
-# or assign through `token` parameter.
-homepage = notion.Page('773b08ff38b44521b44b115827e850f2', token="secret_n2m52d1***")
+# will also look for env var `TZ` to set the timezone for all notion objects. If not found, will default to local timezone.
+```
 
+`__getitem__` searchs for page property values when indexing a Page, and for property objects when indexing a Database.
 
-# __get_item__ searchs for page property values if indexing a Page..
+```py
 homepage['dependencies']
 # {
 #     "id": "WYYq",
 #     "type": "relation",
 #     "relation": [
 #         {
 #             "id": "7bcbc8e6-e237-434b-bd0d-6b56e044200b"
 #         }
 #     ],
 #     "has_more": false
 # }
 
-# ..and searchs for property objects if indexing a Database.
 parent_db['dependencies']
 # {
 #     "id": "WYYq",
 #     "name": "dependencies",
 #     "type": "relation",
 #     "relation": {
 #         "database_id": "f5984a7e-2257-4ab0-9d0a-23ea12324031",
 #         "type": "dual_property",
 #         "dual_property": {
 #             "synced_property_name": "blocked",
 #             "synced_property_id": "wx%7DQ"
 #         }
 #     }
 # }
+```
+
+**_See usage of retrieving values from a page in examples/retrieving-property-items.md_**  
+
+Below is a brief example if we were wanting to get the page id from the above property `dependencies` in `homepage`.
+
+```py
+from notion import propertyitems
 
-homepage.last_edited.date() # out: 01/15/2023
-homepage.title = "New Page Title"
+related_id: list[str] = propertyitems.relation(homepage.dependencies)
+```
+```py
+>>> ["7bcbc8e6-e237-434b-bd0d-6b56e044200b"]
 ```
 
----
+Both Page's and Database's have setters for title/icon/cover.
+
+```py
+homepage.title = "new page"
+homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg"
+```
+
+<p align="center"> <img src="examples/images/new_page.png"> </p>
+
 <br>
 
 ## Creating Pages/Databases/Blocks
 
-The current version of the Notion api does not allow pages to be created to the parent `workspace`.
+The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
 Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
 
 ```py
 new_database = notion.Database.create(
-    homepage, database_title="A new database", name_column="name"
-) 
-# name column refers to the column containing pages/page titles. 
-# Defaults to "Name" if None (all strings in Notion API are case-sensitive).
+    parent_instance=testpage,
+    database_title="Title",
+    name_column="page", # This is the column containing page names. Defaults to "Name".
+    is_inline=True,
+    description="Example Database.",
+)
 
 new_page = notion.Page.create(new_database, page_title="A new database row")
 ```
 
-Blocks can be created with `notion.api.blocktypefactory.BlockFactory` by appending to an exisiting Block or Page. The new block is always returned as a `notion.api.notionblock.Block` instance.
+Blocks can be created with `notion.api.blocktypefactory.BlockFactory` by appending to an exisiting Block or Page.  
+The new block is always returned as an instance of `notion.api.notionblock.Block`.
 ```py
 from notion import properties as prop
 
 # `new_synced_block` refers to the original synced block in the Notion UI.
 original_synced_block = notion.BlockFactory.new_synced_block(homepage)
 
 # Adding content to the synced block
-notion.BlockFactory.paragraph(original_synced_block, [prop.RichText('This is a synced block.')])
-
+notion.BlockFactory.paragraph(
+    original_synced_block, [prop.RichText("This is a synced block.")]
+)
 # Referencing the synced block in a new page.
 notion.BlockFactory.reference_synced_block(new_page, original_synced_block.id)
 ```
 
-**_Example function: Appending blocks to a page as a reminder._**
+<br>
+
+### Example Workflow: **_Appending blocks to a page as a reminder._**
 
 ```py
-def in_block_reminder(page_id: str, message: str, user_name: str) -> None:
-    target_page = notion.Page(page_id)
+def in_block_reminder(page: notion.Page, message: str, user_name: str) -> None:
     mentionblock = notion.BlockFactory.paragraph(
-        target_page,
+        page,
         [
             prop.Mention.user(
-                notion.Workspace.retrieve_user(user_name=user_name),
+                notion.Workspace().retrieve_user(user_name=user_name),
                 annotations=prop.Annotations(
                     code=True, bold=True, color=prop.BlockColor.purple
                 ),
             ),
             prop.RichText(" - "),
             prop.Mention.date(
                 datetime.now().astimezone(target_page.tz).isoformat(),
                 annotations=prop.Annotations(
                     code=True, bold=True, color=prop.BlockColor.purple_background
                 ),
             ),
             prop.RichText(":"),
         ],
     )
+    # First method returned the newly created block that we append to here:
     notion.BlockFactory.paragraph(mentionblock, [prop.RichText(message)])
-    notion.BlockFactory.divider(target_page)
+    notion.BlockFactory.divider(page)
 ```
 
 ```py
->>> in_block_reminder(page_id="0b9eccfa890e4c3390175ee10c664a35", message="message here", user_name="Your Name")
+>>> my_page = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
+>>> in_block_reminder(page=my_page, message="message here", user_name="Your Name")
 ```
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/example_function_reminder.png">
+    <img src="examples/images/example_function_reminder.png">
 </p>
 
----
 <br>
 
-## Add, Set, & Delete - Page property values / Database property objects
+## Add, Set, & Delete: Page property values | Database property objects
 
 The first argument for all database column methods is the name of the property,  
 If it does not exist, then a new property object is created.  
 If it already exists, then the method will overwrite it.
 
 If the name passed already exists, but it's a different column type than the method used - then the API will overwrite this and change the property object to the new column type.  
 The original parameters will be saved if you decide to switch back (i.e. if you change a formula column to a select column, upon changing it back to a formula column, the original formula expression will still be there).   
@@ -192,15 +217,14 @@
 
 # if an option does not already exist, a new one will be created with a random color.
 # this is not true for `status` column types, which can only be edited via UI.
 
 new_page.set_multiselect("options", ["option-a", "option-b"])
 ```
 
----
 <br>
 
 ## Database Queries
 
 A single `notion.query.propfilter.PropertyFilter` is equivalent to filtering one property type in Notion.
 To build filters equivalent to Notion's 'advanced filters', use `notion.query.compound.CompoundFilter`.
 
@@ -232,22 +256,25 @@
 query_result = new_database.query(
     filter=query_filter,
     sort=query_sort,
     page_size=5,
     filter_property_values=["name", "options"],
 )
 ```
----
+
+A database also has the `query_pages()` method. It takes the same parameters, but for each page object in the `results` array, it retrieves the id(s), and instead returns a list of `notion.Page`.
+
 <br>
 
 ## Exceptions & Validating Responses
 
-```py
-# Errors in Notion requests return an object with the keys: 'object', 'status', 'code', and 'message'
+Errors in Notion requests return an object with the keys: 'object', 'status', 'code', and 'message'.
+Exceptions are raised by matching the error code and returning the message. For example:
 
+```py
 homepage._patch_properties(payload={'an_incorrect_key':'value'})
 # Example error object for line above..
 # {
 #   'object': 'error', 
 #   'status': 400, 
 #   'code': 'validation_error', 
 #   'message': 'body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.'
@@ -260,25 +287,32 @@
     homepage._patch_properties(payload={'an_incorrect_key':'value'})
 File "c:\...\notion\exceptions\validate.py", line 48, in validate_response
     raise NotionValidationError(message)
 notion.exceptions.errors.NotionValidationError: body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.
 Error 400: The request body does not match the schema for the expected parameters.
 ```
 
-A common error to look out for is `notion.exceptions.errors.NotionObjectNotFound`  
+Possible errors are:
+ - `NotionInvalidJson`
+ - `NotionInvalidRequestUrl`
+ - `NotionInvalidRequest`
+ - `NotionValidationError`
+ - `NotionMissingVersion`
+ - `NotionUnauthorized`
+ - `NotionRestrictedResource`
+ - `NotionObjectNotFound`
+ - `NotionConflictError`
+ - `NotionRateLimited`
+ - `NotionInternalServerError`
+ - `NotionServiceUnavailable`
+ - `NotionDatabaseConnectionUnavailable`
 
-This error is often raised because your bot has not been added as a connection to the page.  
+A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/directory_add_connections.png">  
+    <img src="examples/images/directory_add_connections.png">  
 </p>
 
-By default, a bot will have access to the children of any Parent object it has access too.
-
-Certain errors are returned with a long list of possible causes for failing validation,
-In these cases, the error is often the outlier in the list - for example:
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/append_child_block_error.png"> 
-</p>
+By default, a bot will have access to the children of any Parent object it has access too. Be sure to double check this connection when moving pages.  
+If you're working on a page that your token has access to via its parent page/database, but you never explicitly granted access to the child page -  and you later move that child page out, then it will lose access.
 
 ---
```

### Comparing `notion_api-0.3.9/notion/__init__.py` & `notion_api-0.4.0/notion/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,34 +19,26 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """ 
 ### Properties:
 >>> from notion import properties as prop
 
+### PropertyItems:
+>>> from notion import propertyitems
+
 ### Queries:
 >>> from notion import query
-query objects:
- - SortFilter[PropertyValueSort | EntryTimestampSort]
- - CompoundFilter[CompoundFilter | PropertyFilter | TimestampFilter]
- - PropertyFilter
- - TimestampFilter
 """
 from typing import Sequence
 
-import notion.properties as properties
-import notion.query as query
 from notion.api import Block, BlockFactory, Database, Page, Workspace
 from notion.api._pkgv import inspect_pkg_version
-from notion.properties.build import build_payload
 
 __all__: Sequence[str] = (
     "Page",
     "Database",
     "Block",
     "Workspace",
     "BlockFactory",
-    "build_payload",
-    "properties",
-    "query",
     "inspect_pkg_version",
 )
```

### Comparing `notion_api-0.3.9/notion/api/__init__.py` & `notion_api-0.4.0/notion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/api/_about.py` & `notion_api-0.4.0/notion/api/_about.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.3.9"
+__version__: Final[str] = "0.4.0"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
```

### Comparing `notion_api-0.3.9/notion/api/_pkgv.py` & `notion_api-0.4.0/notion/api/_pkgv.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/api/blockmixin.py` & `notion_api-0.4.0/notion/api/blockmixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,24 +18,28 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
+import os
 from datetime import datetime, tzinfo
 from functools import cached_property
 from typing import Any, MutableMapping, Optional, Sequence, Union, cast
 
-from pytz import BaseTzInfo, timezone
-from tzlocal import get_localzone
+from pytz import timezone
+from tzlocal import get_localzone_name
 
 from notion.api._about import *
 from notion.api.client import _NotionClient
 
+LOCAL_TIMEZONE = get_localzone_name()
+
+
 __all__: Sequence[str] = ["_TokenBlockMixin"]
 
 
 class _TokenBlockMixin(_NotionClient):
     """
     Any object you interact with in Notion;
     Databases/Pages/individual child blocks, are all considered 'Blocks'
@@ -44,90 +48,112 @@
 
     def __init__(
         self,
         id: str,
         /,
         *,
         token: Optional[str] = None,
-        notion_version: Optional[str] = None,
     ) -> None:
-        super().__init__(token=token, notion_version=notion_version)
+        super().__init__(token=token)
 
-        self.tz: BaseTzInfo = get_localzone()
         self.id: str = id.replace("-", "")
 
+        try:
+            self.tz = timezone(os.environ["TZ"])
+        except KeyError:
+            self.tz = timezone(LOCAL_TIMEZONE)
+
+    def __repr__(self) -> str:
+        id = getattr(self, "id", "")
+        # This is to avoid certain errors occuring
+        # before the object is fully initialized
+        return f"notion.{self.__class__.__name__}('{id}')"
+
+    def set_tz(self, tz: Union[tzinfo, str]) -> None:
+        """
+        :param tz: (required) Set the instance timezone. Takes either str or pytz.timezone\
+                    Use `pytz.all_timezones()` to retrieve list of tz options.\
+                    Class will first check for environment variable `TZ`.\
+                    If not found, class default checks the system-configured timezone.
+        """
+        if isinstance(tz, tzinfo):
+            self.__setattr__("tz", tz)
+        elif isinstance(tz, str):
+            self.__setattr__("tz", timezone(tz))
+
     @cached_property
     def _block(self) -> MutableMapping[str, Any]:
         """
-        Same result as retrieve() for `notion.api.notionblock.Block`.
-        If used with `notion.api.notionpage.Page` or `notion.api.notiondatabase.Database`,
+        Same result as retrieve() for notion.api.notionblock.Block.
+        If used with notion.api.notionpage.Page or notion.api.notiondatabase.Database,
         retrieves the page or database object from the blocks endpoint.
         """
         return self._get(self._block_endpoint(self.id))
 
     @property
     def type(self) -> str:
-        return str(self._block["type"])
+        return cast(str, self._block["type"])
 
     @property
     def object(self) -> str:
-        return str(self._block["object"])
+        return cast(str, (self._block["object"]))
 
     @property
     def has_children(self) -> bool:
-        return bool(self._block["has_children"])
+        return cast(bool, self._block["has_children"])
 
     @property
     def is_archived(self) -> bool:
-        return bool(self._block["archived"])
+        return cast(bool, self._block["archived"])
 
     @property
     def parent_type(self) -> str:
         ptype = cast(str, self._block["parent"]["type"])
         if "workspace" in ptype:
             return "workspace"
         return ptype
 
     @property
     def parent_id(self) -> str:
         _parent_id = self._block["parent"][self.parent_type]
         if _parent_id is True:  # parent is workspace
             workspace = self._get("%s%s" % (__base_url__, "users/me"))
             # return workspace name
-            return "workspace: %s" % workspace["bot"]["workspace_name"]
+            return "workspace-%s" % workspace["bot"]["workspace_name"]
         else:
             return cast(str, _parent_id.replace("-", ""))
 
-    def set_tz(self, tz: Union[tzinfo, str]) -> None:
-        """
-        :param timezone: (required) set default timezone.
-            class default matches the Windows-configured timezone
-            Use `pytz.all_timezones` to retrieve list of tz options.
-            Pass either str or `pytz.timezone(...)`
-        """
-        if isinstance(tz, tzinfo):
-            self.__setattr__("tz", tz)
-        elif isinstance(tz, str):
-            self.__setattr__("tz", timezone(tz))
-
     @property
-    def last_edited(self) -> datetime:
+    def last_edited_time(self) -> datetime:
         """
-        Notion returns datetime ISO 8601, UTC.
-        Class default matches the Windows-configured timezone.
+        Returns date and time when this page/block/database was created.
+        Converted from ISO 8601, UTC to instance timezone.
+        Class will first check for environment variable `TZ`.
+        If not found, class default checks the system-configured timezone.
         Change default timezone with method `set_tz(...)`
         """
         dt = datetime.fromisoformat(self._block["last_edited_time"])
         return dt.astimezone(tz=self.tz)
 
     @property
     def created_time(self) -> datetime:
         """
-        Notion returns datetime ISO 8601, UTC.
-        Class default matches the Windows-configured timezone.
+        Returns date and time when this page/block/database was created.
+        Converted from ISO 8601, UTC to instance timezone.
+        Class will first check for environment variable `TZ`.
+        If not found, class default checks the system-configured timezone.
         Change default timezone with method `set_tz(...)`
         """
         dt = datetime.fromisoformat(self._block["created_time"])
         return dt.astimezone(tz=self.tz)
 
-    def __repr__(self) -> str:
-        return f"notion.{self.__class__.__name__}('{getattr(self, 'id', '')}')"
+    @property
+    def last_edited_by(self) -> str:
+        user_id = self._block["last_edited_by"]["id"]
+        user = self._get("%s%s" % (__base_url__, "users/%s" % user_id))
+        return cast(str, user)
+
+    @property
+    def created_by(self) -> str:
+        user_id = self._block["created_by"]["id"]
+        user = self._get("%s%s" % (__base_url__, "users/%s" % user_id))
+        return cast(str, user)
```

### Comparing `notion_api-0.3.9/notion/api/blocktypefactory.py` & `notion_api-0.4.0/notion/api/blocktypefactory.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/api/client.py` & `notion_api-0.4.0/notion/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,31 @@
 except ModuleNotFoundError:
     import json
 
     default_json: ModuleType = json
 
 import requests
 
-from notion.api._about import *
+from notion.api._about import __base_url__, __content_type__
 from notion.exceptions import NotionUnauthorized, validate_response
 
 __all__: Sequence[str] = ["_NotionClient"]
 
 logging.basicConfig(level=logging.INFO)
 
 _NLOG = logging.getLogger("notion-api")
 
 
 class _NotionClient:
     """Base Class to inherit: token, headers, requests, and endpoints."""
 
     def __init__(
-        self, *, token: Optional[str] = None, notion_version: Optional[str] = None
+        self,
+        *,
+        token: Optional[str] = None,
     ) -> None:
         if token:
             self.token = token
         else:
             try:
                 self.token = os.environ["NOTION_TOKEN"]
             except KeyError:
@@ -64,26 +66,30 @@
                     "%s. %s."
                     % (
                         f"notion.{self.__class__.__name__}: Missing Token",
                         "Check if `NOTION_TOKEN` is set in environment variables",
                     )
                 )
 
+        try:
+            __notion_version__ = os.environ["NOTION_VERSION"]
+        except KeyError:
+            from notion.api._about import __notion_version__
+
+        self.notion_version = __notion_version__
+
         __auth__ = f"Bearer {self.token}"
 
         self.headers: dict[str, str] = {
             "Authorization": __auth__,
             "Accept": __content_type__,
             "Content-type": __content_type__,
             "Notion-Version": __notion_version__,
         }
 
-        if notion_version:
-            self.headers["Notion-Version"] = notion_version
-
     @staticmethod
     def _block_endpoint(
         object_id: Optional[str] = None,
         /,
         *,
         children: Optional[bool] = None,
         page_size: Optional[int] = None,
```

### Comparing `notion_api-0.3.9/notion/api/notionblock.py` & `notion_api-0.4.0/notion/api/notionblock.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,36 +37,35 @@
 
     These are the individual 'nodes' in a page that you typically interact with in Notion.
     Some blocks have more content nested inside them.
     Some examples are indented paragraphs, lists, and toggles.
     The nested content is called children, and children are blocks, too.
 
     ---
+    ### Versioning:
+    To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
+    For more info see: https://developers.notion.com/reference/versioning
+
+    ---
     :param id: (required) `block_id` of object in Notion.
-    :param token: (required) Bearer token provided when you create an integration.\
-                   set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
-                   see https://developers.notion.com/reference/authentication.
-    :param notion_version: (optional) API version. see https://developers.notion.com/reference/versioning
+    :param token: Bearer token provided when you create an integration.\
+                  Set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
+                  See https://developers.notion.com/reference/authentication.
 
     https://developers.notion.com/reference/block
     """
 
     def __init__(
         self,
         id: str,
         /,
         *,
         token: Optional[str] = None,
-        notion_version: Optional[str] = None,
     ) -> None:
-        super().__init__(id, token=token, notion_version=notion_version)
-        if token:
-            self.token = token
-
-        self.notion_version: Optional[str] = notion_version
+        super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
     @cached_property
     def retrieve(self) -> MutableMapping[str, Any]:
         """
         Retrieves a Block object using the ID specified.
 
@@ -106,72 +105,59 @@
         Used internally by notion.api.blocktypefactory.BlockFactory.
 
         https://developers.notion.com/reference/patch-block-children
         """
         return self._patch(self._block_endpoint(self.id, children=True), payload=payload)
 
     @property
-    def delete_self(self) -> Union[MutableMapping[str, Any], None]:
+    def delete_self(self) -> None:
         """
         Sets a Block object, including page blocks, to archived: true
         using the ID specified. Note: in the Notion UI application,
         this moves the block to the "Trash" where it can still be
         accessed and restored. To restore the block with the API,
         use the Update a block or Update page respectively.
 
-        :returns: Mapping of the deleted block object.
-
         https://developers.notion.com/reference/delete-a-block
         """
         if self.is_archived:
-            self.logger.info("delete_self did nothing. Block is already archived.")
             return None
 
-        block = self._delete(self._block_endpoint(self.id))
-        self.logger.info("Deleted Self.")
-        return block
+        self._delete(self._block_endpoint(self.id))
 
     @property
-    def restore_self(self) -> Union[MutableMapping[str, Any], None]:
+    def restore_self(self) -> None:
         """
         Sets "archived" key to false. Parent page must still exist in Notion's trash.
         :returns: If block is archived, a Mapping of the restored block object, else None.
 
         https://developers.notion.com/reference/update-a-block
         """
         if not self.is_archived:
-            self.logger.info("restore_self did nothing. Block is not archived.")
             return None
 
-        block = self._patch(
-            self._block_endpoint(self.id), payload=(b'{"archived": false}')
-        )
-        self.logger.info("Restored Self.")
-        return block
+        self._patch(self._block_endpoint(self.id), payload=(b'{"archived": false}'))
 
     def delete_child(
         self, children_id: Optional[list[str]] = None, *, all: Optional[bool] = False
     ) -> None:
         if not self.has_children:
-            self.logger.info("delete_child did nothing. Block has no children.")
             return
 
         if all:
             children = [
                 block["id"] for block in self.retrieve_children().get("results", [])
             ]
             for id in children:
                 self._delete(self._block_endpoint(id))
-            self.logger.info(f"Deleted all child blocks.")
             return
 
         if children_id:
             for id in children_id:
                 self._delete(self._block_endpoint(id))
-                self.logger.info(f"Deleted child block `{id}`.")
 
     def update(
         self,
         payload: Union[MutableMapping[str, Any], Union[bytearray, bytes, bytearray]],
     ) -> MutableMapping[str, Any]:
         """
         Updates content for the specified block_id based on the block
```

### Comparing `notion_api-0.3.9/notion/api/notionpage.py` & `notion_api-0.4.0/notion/api/notionpage.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,24 +20,38 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 from datetime import datetime
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterator,
+    MutableMapping,
+    Optional,
+    Sequence,
+    Union,
+    cast,
+)
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.api.client import _NLOG
 from notion.api.notionblock import Block
 from notion.api.notiondatabase import Database
-from notion.exceptions.errors import NotionInvalidJson
 from notion.properties.build import build_payload
 from notion.properties.common import Parent, UserObject, _NotionUUID
-from notion.properties.files import ExternalFile, FilesPropertyValue, InternalFile
+from notion.properties.files import (
+    Cover,
+    ExternalFile,
+    FilesPropertyValue,
+    Icon,
+    InternalFile,
+)
 from notion.properties.propertyobjects import Option
 from notion.properties.propertyvalues import (
     CheckboxPropertyValue,
     DatePropertyValue,
     EmailPropertyValue,
     MultiSelectPropertyValue,
     NumberPropertyValue,
@@ -48,14 +62,15 @@
     RichTextPropertyValue,
     SelectPropertyValue,
     StatusPropertyValue,
     TitlePropertyValue,
     URLPropertyValue,
 )
 from notion.properties.richtext import RichText
+from notion.propertyitems.base import PropertyItem
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
 __all__: Sequence[str] = ["Page"]
 
 
@@ -70,52 +85,56 @@
         - Read using retrieve block children.
         - Appended using append block children.
 
     NOTE: The current version of the Notion api does not allow pages to be created to the parent `workspace`. 
     Objects created through the API must be created with a parent of an existing Page/Database/Block.
 
     ---
+    ### Versioning:
+    To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
+    For more info see: https://developers.notion.com/reference/versioning
+
+    ---
     :param id: (required) `page_id` of object in Notion.
-    :param token: (required) Bearer token provided when you create an integration.\
-                   set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
-                   see https://developers.notion.com/reference/authentication.
-    :param notion_version: (optional) API version. see https://developers.notion.com/reference/versioning
+    :param token: Bearer token provided when you create an integration.\
+                  Set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
+                  See https://developers.notion.com/reference/authentication.
 
     https://developers.notion.com/reference/page
     """
 
     def __init__(
         self,
         id: str,
         /,
         *,
         token: Optional[str] = None,
-        notion_version: Optional[str] = None,
     ) -> None:
-        super().__init__(id, token=token, notion_version=notion_version)
-        if token:
-            self.token = token
-
-        self.notion_version: Optional[str] = notion_version
+        super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
     @classmethod
     def create(
-        cls, parent_instance: Union[Page, Database, Block], page_title: str
+        cls,
+        parent_instance: Union[Page, Database, Block],
+        page_title: str,
+        *,
+        cover_url: Optional[str] = None,
+        icon_url: Optional[str] = None,
     ) -> Page:
         """
         Creates a blank page.
         Use Page methods to add values to properties described in parent database schema.
         Add content to page by appending block children with notion.api.blocktypefactory.BlockFactory.
 
         ---
-        :param parent_instance: (required) eithr a Page or Database instance.
-        :param page_title: (required)
-        :param icon_url: (optional) #not yet implemented
-        :param cover: (optional) #not yet implemented
+        :param parent_instance: (required) Either a Page or Database instance.
+        :param page_title: (required) Title of page.
+        :param cover_url: (optional) Url of image to use as cover.
+        :param icon_url: (optional) Url of image to use as icon.
 
         https://developers.notion.com/reference/post-page
         """
         if "child_database" in parent_instance.type:
             payload = build_payload(
                 Parent.database(parent_instance.id),
                 Properties(TitlePropertyValue([RichText(page_title)])),
@@ -125,133 +144,154 @@
                 Parent.page(parent_instance.id),
                 Properties(TitlePropertyValue([RichText(page_title)])),
             )
 
         new_page = cls._post(parent_instance, cls._pages_endpoint(), payload=payload)
 
         cls_ = cls(new_page["id"])
-        cls_.logger.info(
+        cls_.logger.debug(
             f"Page created in {parent_instance.__repr__()}. Url: {new_page['url']}"
         )
+
+        if icon_url:
+            cls_.icon = icon_url
+        if cover_url:
+            cls_.cover = cover_url
+
         return cls_
 
+    def __getattr__(self, attr: str) -> PropertyItem:
+        def lower_alnum(s: str) -> str:
+            return "".join([c if c.isalnum() else "_" for c in s]).lower()
+
+        for property in self:
+            if lower_alnum(attr) == lower_alnum(property):
+                return PropertyItem(
+                    map=self.retrieve_property_item(property), source_page=self.id
+                )
+
+        raise AttributeError(f"{attr} not found in page property values.")
+
+    def __contains__(self, property_name: str) -> bool:
+        return property_name in self.properties
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self.properties)
+
     def __getitem__(self, property_name: str) -> MutableMapping[str, Any]:
         if property_name in self.properties:
             return cast(MutableMapping[str, Any], self.properties[property_name])
-        raise NotionInvalidJson(f"{property_name} not found in page property values.")
-
-    @cached_property
-    def _retrieve(self) -> MutableMapping[str, Any]:
-        return self.retrieve(filter_properties=None)
+        raise KeyError(f"{property_name} not found in page property values.")
 
     @cached_property
     def properties(self) -> MutableMapping[str, Any]:
-        return cast(MutableMapping[str, Any], self._retrieve["properties"])
+        return cast(MutableMapping[str, Any], self.retrieve()["properties"])
 
     @property
     def title(self) -> str:
+        """:return: (str) title of page"""
         try:
             if ("workspace" or "page_id") in self.parent_type:
                 return cast(str, self.properties["title"]["title"][0]["plain_text"])
 
             database_title_property = self.properties[
                 [k for k, v in self.properties.items() if "title" in v][0]
             ]
             return cast(str, database_title_property["title"][0]["plain_text"])
         except IndexError:
             return ""  # title is empty
 
     @title.setter
     def title(self, __new_title: str) -> None:
-        self._patch_properties(
-            payload=Properties(TitlePropertyValue([RichText(__new_title)]))
-        )
+        self._patch_properties(Properties(TitlePropertyValue([RichText(__new_title)])))
 
     @property
-    def url(self) -> MutableMapping[str, Any]:
-        return cast(MutableMapping[str, Any], self._retrieve["url"])
+    def icon(self) -> str:
+        """:return: (str) url of icon"""
+        icon = self.properties["icon"]["external"]["url"]
+        return cast(str, icon)
+
+    @icon.setter
+    def icon(self, icon_url: str) -> None:
+        """>>> page.icon = "https://www.notion.so/icons/code_gray.svg" """
+        self._patch_properties(Icon(icon_url))
 
     @property
-    def icon(self) -> MutableMapping[str, Any]:
-        return cast(MutableMapping[str, Any], self._retrieve["icon"])
+    def cover(self) -> str:
+        """:return: (str) url of cover"""
+        cover = self.properties["cover"]["external"]["url"]
+        return cast(str, cover)
+
+    @cover.setter
+    def cover(self, cover_url: str) -> None:
+        """>>> page.cover = "https://www.notion.so/images/page-cover/webb1.jpg" """
+        self._patch_properties(Cover(cover_url))
 
     @property
-    def cover(self) -> MutableMapping[str, Any]:
-        return cast(MutableMapping[str, Any], self._retrieve["cover"])
+    def url(self) -> str:
+        """:return: (str) url of page"""
+        return cast(str, self.properties["url"])
 
     @property
     def delete_self(self) -> None:
         if self.is_archived:
-            self.logger.info("delete_self did nothing. Page is already archived.")
             return
 
         self._delete(self._block_endpoint(self.id))
-        self.logger.info("Deleted self.")
 
     @property
     def restore_self(self) -> None:
         if not self.is_archived:
-            self.logger.info("restore_self did nothing. Page is not archived.")
             return
 
         self._patch(self._pages_endpoint(self.id), payload=(b'{"archived": false}'))
-        self.logger.info("Restored self.")
 
     def retrieve(
         self, *, filter_properties: Optional[list[str]] = None
     ) -> MutableMapping[str, Any]:
         """ 
         Retrieves a Page object using the ID specified.
 
-        :param filter_properties: (optional) A list of page property value IDs associated with the page.\
-                                   Use this param to limit the response to a specific page property value or values.\
-                                   To retrieve multiple properties, specify each page property ID.\
-                                   E.g. ?filter_properties=iAk8&filter_properties=b7dh.
+        :param filter_properties: (optional) A list of page property value names associated with the page.\
+                                   Use this param to limit the response to a specific page property value(s).\
 
         https://developers.notion.com/reference/retrieve-a-page
         """
         if filter_properties:
             _pages_endpoint_filtered_prop = f"{self._pages_endpoint(self.id)}?"
             for name in filter_properties:
-                name_id = self.properties[name]["id"]
+                name_id = self[name]["id"]
                 _pages_endpoint_filtered_prop += f"filter_properties={name_id}&"
             return self._get(_pages_endpoint_filtered_prop)
+
         return self._get(self._pages_endpoint(self.id))
 
     def _retrieve_property_id(self, property_name: str) -> str:
         """Internal function to retrieve the id of a property."""
-        if property_name in self.properties:
-            return str(self.properties[property_name]["id"])
-        raise NotionInvalidJson("Property name not found in parent schema.")
+        return cast(str, self[property_name]["id"])
 
     def retrieve_property_item(
         self,
         property_name: str,
     ) -> MutableMapping[str, Any]:
         """
         Retrieves a property_item object for a given page_id and property_id.
         The object returned will either be:
             - a value.
             - a paginated list of property item values.
 
-        ---
-        :param property_name: (required) property name in Notion *case-sensitive\
-                               this endpoint only works with property_id's, internal function will retrieve this.
-        :param results_only: if true, returns the `results` key index[0] for paginated responses.\
-                             will be either a single dictionary or a list of dictionaries.
-        :param property_item_only: if true, returns the `property_item` key.
+        :param property_name: (required) property name in Notion *case-sensitive.
+
+        https://developers.notion.com/reference/property-item-object
 
         https://developers.notion.com/reference/retrieve-a-page-property
         """
+        property_id = self._retrieve_property_id(property_name)
         return self._get(
-            self._pages_endpoint(
-                self.id,
-                properties=True,
-                property_id=self._retrieve_property_id(property_name),
-            )
+            self._pages_endpoint(self.id, properties=True, property_id=property_id)
         )
 
     def _patch_properties(
         self, payload: MutableMapping[str, Any]
     ) -> MutableMapping[str, Any]:
         """
         Updates page property values for the specified page.
@@ -285,143 +325,171 @@
         """
         Used internally by notion.api.blocktypefactory.BlockFactory.
 
         https://developers.notion.com/reference/patch-block-children
         """
         return self._patch(self._block_endpoint(self.id, children=True), payload=payload)
 
-    def set_select(self, column_name: str, select_option: str) -> None:
+    def set_select(self, property_name: str, /, select_option: str) -> None:
         """
-        :param select_option: (required) if the option already exists, then it is\
-                               case sensitive. if the option does not exist, it will be created.
+        :param select_option: (required) If the option already exists, then it is case sensitive.\
+                               If the option does not exist, it will be created.
+        
+        https://developers.notion.com/reference/page-property-values#select
         """
-        parent_db = Database(
-            self.parent_id,
-            token=self.token,
-            notion_version=self.notion_version,
-        )
+        parent_db = Database(self.parent_id, token=self.token)
 
-        current_options = parent_db[column_name]["select"]["options"]
+        current_options = parent_db[property_name]["select"]["options"]
         names = {o.get("name"): o.get("color") for o in current_options}
 
         if set([select_option]).issubset(names):
             option = Option(select_option, names.get(select_option))
         else:
             option = Option(select_option)
 
-        self._patch_properties(Properties(SelectPropertyValue(column_name, option)))
+        self._patch_properties(Properties(SelectPropertyValue(property_name, option)))
 
-    def set_multiselect(self, column_name: str, multi_select_options: list[str]) -> None:
+    def set_multiselect(
+        self, property_name: str, /, multi_select_options: list[str]
+    ) -> None:
         """
-        :param multi_select_options: (required) list of strings for each select option.\
-                                      if the option already exists, then it is case sensitive.\
-                                      if the option does not exist, it will be created.
+        :param multi_select_options: (required) List of strings for each select option.\
+                                      If the option already exists, then it is case sensitive.\
+                                      If the option does not exist, it will be created.
+
+        https://developers.notion.com/reference/page-property-values#multi-select
         """
         selected_options: list[Option] = []
+        parent_db = Database(self.parent_id, token=self.token)
 
-        parent_db = Database(
-            self.parent_id,
-            token=self.token,
-            notion_version=self.notion_version,
-        )
-
-        current_options = parent_db[column_name]["multi_select"]["options"]
+        current_options = parent_db[property_name]["multi_select"]["options"]
         names = {o.get("name"): o.get("color") for o in current_options}
 
         for option in multi_select_options:
             if set([option]).issubset(names):
                 selected_options.append(Option(option, names.get(option)))
             else:
                 selected_options.append(Option(option))
 
         self._patch_properties(
-            Properties(MultiSelectPropertyValue(column_name, selected_options))
+            Properties(MultiSelectPropertyValue(property_name, selected_options))
         )
 
-    def set_status(self, column_name: str, status_option: str) -> None:
+    def set_status(self, property_name: str, /, status_option: str) -> None:
         """
         :param status_option: (required) unlike select/multi-select,\
                                status option must already exist when using this endpoint.\
                                to create a new status option, use the database endpoints.\
                                option is case-sensitive.
+
+        https://developers.notion.com/reference/page-property-values#status
         """
-        parent_db = Database(
-            self.parent_id,
-            token=self.token,
-            notion_version=self.notion_version,
-        )
+        parent_db = Database(self.parent_id, token=self.token)
 
-        current_options = parent_db[column_name]["status"]["options"]
+        current_options = parent_db[property_name]["status"]["options"]
         names = {o.get("name"): o.get("color") for o in current_options}
 
         if set([status_option]).issubset(names):
             option = Option(status_option, names.get(status_option))
         else:
             option = Option(status_option)
 
-        self._patch_properties(Properties(StatusPropertyValue(column_name, option)))
+        self._patch_properties(Properties(StatusPropertyValue(property_name, option)))
 
     def set_date(
         self,
-        column_name: str,
+        property_name: str,
+        /,
         start: Union[str, datetime],
         end: Optional[Union[str, datetime]] = None,
     ) -> None:
         """
         :param start: (required) A date, with an optional time.\
-                       If the "date" value is a range, then start represents the start of the range.
-        :param end: (optional) A string representing the end of a date range.\
-                     If the value is null, then the date value is not a range.
+                       If value is a string, it must be ISO 8601 format.\
+                       If value is datetime.datetime, it will be converted to self.tz, in isoformat.
+        :param end: (optional) A date, with an optional time.\
+                     If value is provided, then date property becomes a range, with start and end values.\
+                     If value is not provided, then the date value is not a range.
+                     If value is a string, it must be ISO 8601 format.\
+                     If value is datetime.datetime, it will be converted to self.tz, in isoformat.
+
+        https://developers.notion.com/reference/page-property-values#date
         """
         if isinstance(start, datetime):
-            start = start.astimezone(self.tz)
+            start = start.astimezone(self.tz).isoformat()
         if end and isinstance(end, datetime):
-            end = end.astimezone(self.tz)
+            end = end.astimezone(self.tz).isoformat()
 
         self._patch_properties(
-            Properties(DatePropertyValue(column_name, start=start, end=end))
+            Properties(DatePropertyValue(property_name, start=start, end=end))
         )
 
-    def set_text(self, column_name: str, new_text: Union[str, Any]) -> None:
+    def set_text(self, property_name: str, /, text: str) -> None:
+        """https://developers.notion.com/reference/page-property-values#rich-text"""
         self._patch_properties(
-            Properties(RichTextPropertyValue(column_name, [RichText(new_text)]))
+            Properties(RichTextPropertyValue(property_name, [RichText(text)]))
         )
 
     def set_files(
-        self, column_name: str, array_of_files: list[Union[InternalFile, ExternalFile]]
+        self,
+        property_name: str,
+        /,
+        array_of_files: Sequence[Union[InternalFile, ExternalFile]],
     ) -> None:
+        """
+        When updating a file property, the value is overwritten by the array of files passed.
+        Although Notion doesn't support uploading files, if you pass a file object containing a file hosted by Notion,
+        it remains one of the files. To remove any file, just don't pass it in the update response.
+
+        InternalFiles are a file object corresponding to a file that has been uploaded to Notion.
+        ExternalFiles are a file object corresponding to an external file that has been linked to in Notion.
+
+        ---
+        :param array_of_files: (required) An array of objects containing information about the files.\
+                                Either InternalFile(), ExternalFile() or a combination of both.
+
+        https://developers.notion.com/reference/page-property-values#files
+        """
         self._patch_properties(
-            Properties(FilesPropertyValue(column_name, array_of_files))
+            Properties(FilesPropertyValue(property_name, array_of_files))
         )
 
-    def set_phonenumber(self, column_name: str, phone_number: str) -> None:
+    def set_phone_number(self, property_name: str, /, phone_number: str) -> None:
+        """https://developers.notion.com/reference/page-property-values#phone-number"""
         self._patch_properties(
-            Properties(PhoneNumberPropertyValue(column_name, phone_number))
+            Properties(PhoneNumberPropertyValue(property_name, phone_number))
         )
 
-    def set_related(self, column_name: str, related_ids: list[str]) -> None:
-        """
-        :param related_ids: (required) list of notion page ids to reference
-        """
-        list_ids: list[_NotionUUID] = []
-        for id in related_ids:
-            list_ids.append(_NotionUUID(id))
-
-        self._patch_properties(Properties(RelationPropertyValue(column_name, list_ids)))
-
-    def set_checkbox(self, column_name: str, value: bool) -> None:
-        self._patch_properties(Properties(CheckboxPropertyValue(column_name, value)))
-
-    def set_number(self, column_name: str, new_number: Union[float, timedelta]) -> None:
+    def set_related(self, property_name: str, /, related_ids: Sequence[str]) -> None:
         """
-        :param new_number: (required) to replace the current number
+        :param related_ids: (required) An array of related page references.\
+                             A page reference is an object with an id key and a string value (UUIDv4)\
+                             corresponding to a page ID in another database.
+        
+        https://developers.notion.com/reference/page-property-values#relation
         """
-        self._patch_properties(Properties(NumberPropertyValue(column_name, new_number)))
+        list_related_ids = [_NotionUUID(id) for id in related_ids]
+        self._patch_properties(
+            Properties(RelationPropertyValue(property_name, list_related_ids))
+        )
 
-    def set_people(self, column_name: str, user_array: Sequence[UserObject]) -> None:
-        self._patch_properties(Properties(PeoplePropertyValue(column_name, user_array)))
+    def set_checkbox(self, property_name: str, /, value: bool) -> None:
+        """https://developers.notion.com/reference/page-property-values#checkbox"""
+        self._patch_properties(Properties(CheckboxPropertyValue(property_name, value)))
 
-    def set_email(self, column_name: str, email: str) -> None:
-        self._patch_properties(Properties(EmailPropertyValue(column_name, email)))
+    def set_number(
+        self, property_name: str, /, new_number: Union[float, timedelta]
+    ) -> None:
+        """https://developers.notion.com/reference/page-property-values#number"""
+        self._patch_properties(Properties(NumberPropertyValue(property_name, new_number)))
 
-    def set_url(self, column_name: str, url: str) -> None:
-        self._patch_properties(Properties(URLPropertyValue(column_name, url)))
+    def set_people(self, property_name: str, /, user_array: Sequence[UserObject]) -> None:
+        """https://developers.notion.com/reference/page-property-values#people"""
+        self._patch_properties(Properties(PeoplePropertyValue(property_name, user_array)))
+
+    def set_email(self, property_name: str, /, email: str) -> None:
+        """https://developers.notion.com/reference/page-property-values#email"""
+        self._patch_properties(Properties(EmailPropertyValue(property_name, email)))
+
+    def set_url(self, property_name: str, /, url: str) -> None:
+        """https://developers.notion.com/reference/page-property-values#url"""
+        self._patch_properties(Properties(URLPropertyValue(property_name, url)))
```

### Comparing `notion_api-0.3.9/notion/api/notionworkspace.py` & `notion_api-0.4.0/notion/api/notionworkspace.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,47 +16,42 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from operator import methodcaller
 from typing import Any, MutableMapping, Optional, Sequence, Union, cast
 
-from notion.api._about import __base_url__, __notion_version__
+from notion.api._about import __base_url__
 from notion.api.client import _NotionClient
 from notion.api.notionblock import Block
 from notion.api.notionpage import Page
-from notion.exceptions.errors import (
-    NotionInvalidRequest,
-    NotionInvalidRequestUrl,
-    NotionObjectNotFound,
-    NotionValidationError,
-)
 from notion.properties.build import NotionObject, build_payload
-from notion.properties.common import BotObject, Parent, UserObject
+from notion.properties.common import Parent, UserObject
 from notion.properties.richtext import Mention, RichText
 from notion.query.sort import EntryTimestampSort, SortFilter
 
 __all__: Sequence[str] = ["Workspace"]
 
 
 class Workspace(_NotionClient):
     """
-    notion.api.notionworkspace.Workspace uses static methods and doesn't require an instance,
-    but currently requires the token be set as an environment variable.
+    Workspace class is to provide general methods that are not specific to a single object.
+    Post/retrieve comments, retrieve users/bots, and search for pages/databases.
     """
 
-    def __init__(self) -> None:
-        super().__init__(token=None, notion_version=None)
+    def __init__(
+        self,
+        token: Optional[str] = None,
+    ) -> None:
+        super().__init__(token=token)
 
-    @staticmethod
-    def __repr__() -> str:
-        return f"notion.{Workspace().__class__.__name__}()"
+    def __repr__(self) -> str:
+        return f"notion.{self.__class__.__name__}()"
 
     @staticmethod
     def _workspace_endpoint(
         *,
         users: Optional[bool] = False,
         search: Optional[bool] = None,
         user_id: Optional[str] = None,
@@ -80,150 +75,112 @@
         return "%scomments%s%s%s" % (
             __base_url__,
             f"?block_id={block_id}" if block_id else "",
             f"&page_size={page_size}" if page_size else "",
             f"&start_cursor={start_cursor}" if start_cursor else "",
         )
 
-    @staticmethod
-    def retrieve_token_bot() -> MutableMapping[str, Any]:
+    def retrieve_token_bot(self) -> MutableMapping[str, Any]:
         """
         Retrieves the bot User associated with the API token provided in the authorization header.
         The bot will have an owner field with information about the person who authorized the integration.
 
         https://developers.notion.com/reference/get-self
         """
-        retrieve_token_bot_endpoint = methodcaller(
-            "_workspace_endpoint", users=True, me=True
-        )(Workspace())
-        retrieve_bot_token_method = methodcaller("_get", retrieve_token_bot_endpoint)
-
-        return cast(
-            MutableMapping[str, Any],
-            retrieve_bot_token_method(Workspace()),
-        )
+        return self._get(self._workspace_endpoint(users=True, me=True))
 
-    @staticmethod
     def list_all_users(
-        *, page_size: Optional[int] = None, cursor: Optional[str] = None
+        self, *, page_size: Optional[int] = None, next_cursor: Optional[str] = None
     ) -> MutableMapping[str, Any]:
         """
         Returns a paginated list of Users for the workspace.
         https://developers.notion.com/reference/get-users
         """
-        all_users_endpoint = methodcaller("_workspace_endpoint", users=True)(Workspace())
-
-        if any([page_size, cursor]):
-            payload: dict[str, Any] = {}
+        if any([page_size, next_cursor]):
+            payload: NotionObject = NotionObject()
             if page_size:
-                payload |= {"page_size": page_size}
-            if cursor:
-                payload |= {"next_cursor": cursor}
+                payload.set("page_size", page_size)
+            if next_cursor:
+                payload.set("next_cursor", next_cursor)
 
-            all_users_method = methodcaller("_get", all_users_endpoint, payload=payload)
-        else:
-            all_users_method = methodcaller("_get", all_users_endpoint)
+            return self._get(self._workspace_endpoint(users=True), payload=payload)
 
-        return cast(
-            MutableMapping[str, Any],
-            all_users_method(Workspace()),
-        )
+        return self._get(self._workspace_endpoint(users=True))
 
-    @staticmethod
     def retrieve_user(
-        *, user_name: Optional[str] = None, user_id: Optional[str] = None
-    ) -> Union[UserObject, BotObject]:
+        self, *, user_name: Optional[str] = None, user_id: Optional[str] = None
+    ) -> UserObject:
         """
         Retrieves a User using either the user name or ID specified.
 
         :param user_name: (1 of user_name or user_id required) User name in Notion.
         :param user_id: (1 of user_name or user_id required) Identifier for a Notion user
 
         https://developers.notion.com/reference/get-users
         """
-        try:
-            if not any([user_name, user_id]):
-                raise ValueError("Must input either user_name or user_id.")
+        if not any([user_name, user_id]):
+            raise ValueError("Must input either user_name or user_id.")
 
+        if user_name:
             all_users = {
                 n.get("name"): n.get("id")
-                for n in Workspace.list_all_users().get("results", [])
+                for n in self.list_all_users().get("results", [])
             }
-
             if set([user_name]).issubset(all_users):
                 user_id = cast(str, all_users.get(user_name))
 
-            retrieve_user_endpoint = methodcaller(
-                "_workspace_endpoint",
-                users=True,
-                user_id=user_id,
-            )(Workspace())
-
-            user = methodcaller("_get", retrieve_user_endpoint)(Workspace())
-
-            if user["type"] == "bot":
-                return BotObject(
-                    id=user["id"],
-                    name=user["name"],
-                    avatar_url=user["avatar_url"] if user["avatar_url"] else None,
-                    bot=user["bot"],
-                    workspace_name=user["bot"]["workspace_name"],
-                )
+        user = self._get(self._workspace_endpoint(users=True, user_id=user_id))
+
+        if user["type"] == "bot":
+            raise TypeError("User is a bot. Use retrieve_token_bot() instead.")
 
+        try:
             return UserObject(
                 id=user["id"],
                 name=user["name"],
                 avatar_url=user["avatar_url"] if user["avatar_url"] else None,
                 email=user["person"]["email"] if user["person"]["email"] else None,
             )
-
-        except TypeError:
-            raise NotionInvalidRequest(
-                f"{Workspace.__repr__()}: Cannot use positional arguments for this method.",
-            )
-        except (KeyError, NotionValidationError):
-            method = "user_name" if user_name else "user_id"
-            raise NotionInvalidRequest(
-                f"{Workspace.__repr__()}: Could not find {method}: {user_name if user_name else user_id} ",
+        except KeyError:
+            raise ValueError(
+                "%s. %s"
+                % (
+                    f"{self.__repr__()}: Could not find user with name: {user_name}",
+                    f"Only members and guests in the integration's workspace are visible.",
+                )
             )
 
-    @staticmethod
     def retrieve_comments(
+        self,
         *,
         thread: Union[Page, Block, str],
         page_size: Optional[int] = None,
         start_cursor: Optional[str] = None,
     ) -> MutableMapping[str, Any]:
-        """When retrieving comments, one or more Comment objects will be returned in the form of an array,
+        """
+        When retrieving comments, one or more Comment objects will be returned in the form of an array,
         sorted in ascending chronological order.
 
-        retrieving comments from a page parent will return all comments on the page, but not
-        comments from any blocks inside the page
+        Retrieving comments from a page parent will return all comments on the page, but not
+        comments from any blocks inside the page.
 
         https://developers.notion.com/reference/retrieve-a-comment
         """
         if isinstance(thread, Page) or isinstance(thread, Block):
-            block = thread.id
+            block_id = thread.id
         else:
-            block = thread
+            block_id = thread
 
-        retrieve_comments_endpoint = methodcaller(
-            "_comments_endpoint",
-            block_id=block,
-            page_size=page_size,
-            start_cursor=start_cursor,
-        )(Workspace())
-
-        return cast(
-            MutableMapping[str, Any],
-            methodcaller("_get", retrieve_comments_endpoint)(Workspace()),
+        comments_endpoint = self._comments_endpoint(
+            block_id=block_id, page_size=page_size, start_cursor=start_cursor
         )
+        return self._get(comments_endpoint)
 
-    @staticmethod
     def comment(
+        self,
         *,
         page: Optional[Union[Page, Block, str]] = None,
         block: Optional[Union[Block, str]] = None,
         discussion_id: Optional[str] = None,
         comment: Sequence[Union[RichText, Mention]],
     ) -> Union[MutableMapping[str, Any], None]:
         """
@@ -244,94 +201,60 @@
                         and comment in that thread if found.
         :param discussion_id: (1 of page/block/discussion_id required)\
                                a string representing the discussion_id of a comment object.
         :param comment: (required) either a Richtext/Mention object.
 
         https://developers.notion.com/reference/create-a-comment
         """
-        retrieve_comments_endpoint = methodcaller(
-            "_comments_endpoint",
-        )(Workspace())
+        if len([k for k, v in locals().items() if v is not None]) > 3:
+            raise ValueError("Only one of page/block/discussion_id can be provided.")
 
         comment_object: NotionObject = NotionObject()
         comment_object.set("rich_text", comment)
 
         if page:
             if isinstance(page, Page):
                 payload = build_payload(Parent.page(page.id), comment_object)
             elif isinstance(page, Block):
                 payload = build_payload(Parent.page(page.parent_id), comment_object)
             elif isinstance(page, str):
                 payload = build_payload(Parent.page(page), comment_object)
 
-            comment_method = methodcaller(
-                "_post",
-                retrieve_comments_endpoint,
-                payload=payload,
-            )
-            return cast(
-                MutableMapping[str, Any],
-                comment_method(Workspace()),
-            )
+            return self._post(self._comments_endpoint(), payload=payload)
 
         if block:
             if isinstance(block, Block):
-                comment_thread = Workspace.retrieve_comments(thread=block.id)
-            else:
-                comment_thread = Workspace.retrieve_comments(thread=block)
-
-            if not comment_thread.get("results", []):
-                raise NotionObjectNotFound(
-                    "%s %s %s"
+                comment_thread = self.retrieve_comments(thread=block.id).get("results")
+            else:  # if str of block.id
+                comment_thread = self.retrieve_comments(thread=block).get("results")
+
+            if not comment_thread:
+                raise ValueError(
+                    "%s %s"
                     % (
                         "Did not find a comment thread in this block.",
-                        f"Notion API version {__notion_version__} currently does not",
-                        "Support creating new comment threads on a block.",
+                        f"Starting new comment threads on a block not supported.",
                     )
                 )
-            # regardless of the discussion_id used in a comment thread on a block,
-            # the next comment will always appear last, so we only get the first discussion_id.
-            payload = build_payload(
-                {
-                    "discussion_id": comment_thread.get("results", [])[0].get(
-                        "discussion_id"
-                    )
-                },
-                comment_object,
-            )
-            comment_method = methodcaller(
-                "_post",
-                retrieve_comments_endpoint,
-                payload=payload,
-            )
-            return cast(
-                MutableMapping[str, Any],
-                comment_method(Workspace()),
-            )
+            # Regardless of which discussion_id in a comment thread is used,
+            # The next comment will always appear last, so we only get the first discussion_id.
+            thread_id = comment_thread[0]["discussion_id"]
+            payload = build_payload({"discussion_id": thread_id}, comment_object)
+            return self._post(self._comments_endpoint(), payload=payload)
 
         if discussion_id:
             payload = build_payload({"discussion_id": discussion_id}, comment_object)
-            comment_method = methodcaller(
-                "_post",
-                retrieve_comments_endpoint,
-                payload=payload,
-            )
-            return cast(
-                MutableMapping[str, Any],
-                comment_method(Workspace()),
-            )
+            return self._post(self._comments_endpoint(), payload=payload)
 
-        elif not any([page, block, discussion_id]):
-            raise NotionInvalidRequestUrl(
-                "Either a parent page/block, or a discussion_id is required (not both)"
-            )
-        return None
+        raise ValueError(
+            "Either a parent page/block, or a discussion_id is required (not both)"
+        )
 
-    @staticmethod
     def search(
+        self,
         *,
         page_size: Optional[int] = 100,
         query: Optional[str] = None,
         filter_pages: Optional[bool] = False,
         filter_databases: Optional[bool] = False,
         start_cursor: Optional[str] = None,
         sort_ascending: Optional[bool] = None,
@@ -383,32 +306,23 @@
         :param sort_ascending: (optional) Limitation: Currently only a single sort is allowed and\
                                 is limited to last_edited_time. The default sort is by last_edited_time descending.\
                                 If sort_ascending is set to `True`, the default sort will be overridden.
         :param start_cursor: (optional) If supplied, will return a page of results starting after provided cursor.
 
         https://developers.notion.com/reference/post-search
         """
-        payload = NotionObject()
+        payload: NotionObject = NotionObject()
         payload.set("page_size", page_size)
         if query:
             payload.set("query", query)
         if filter_pages:
             payload.nest("filter", "property", "object")
             payload.nest("filter", "value", "page")
         if filter_databases:
             payload.nest("filter", "property", "object")
             payload.nest("filter", "value", "database")
         if start_cursor:
             payload.set("start_cursor", start_cursor)
         if sort_ascending:
             payload |= SortFilter([EntryTimestampSort.last_edited_time_ascending()])
 
-        workspace_endpoint = methodcaller("_workspace_endpoint", search=True)
-        search_method = methodcaller(
-            "_post",
-            workspace_endpoint(Workspace()),
-            payload=payload,
-        )
-        return cast(
-            MutableMapping[str, Any],
-            search_method(Workspace()),
-        )
+        return self._post(self._workspace_endpoint(search=True), payload=payload)
```

### Comparing `notion_api-0.3.9/notion/exceptions/__init__.py` & `notion_api-0.4.0/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/exceptions/errors.py` & `notion_api-0.4.0/notion/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/exceptions/validate.py` & `notion_api-0.4.0/notion/exceptions/validate.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/properties/__init__.py` & `notion_api-0.4.0/notion/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/properties/blocktypes.py` & `notion_api-0.4.0/notion/properties/blocktypes.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/properties/build.py` & `notion_api-0.4.0/notion/properties/build.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/properties/common.py` & `notion_api-0.4.0/notion/properties/common.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/properties/files.py` & `notion_api-0.4.0/notion/properties/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,28 @@
 from notion.properties.build import NotionObject
 from notion.properties.common import _NotionURL
 from notion.properties.propertyvalues import PagePropertyValue
 from notion.properties.richtext import Equation, Mention, RichText
 
 __all__: Sequence[str] = (
     "Icon",
+    "Cover",
     "ExternalFile",
     "InternalFile",
     "FilesPropertyValue",
 )
 
 
 class FilesPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        array_of_files: list[Union[InternalFile, ExternalFile]],
+        array_of_files: Sequence[Union[InternalFile, ExternalFile]],
     ) -> None:
         """
         When updating a file property, the value is overwritten by the array of files passed.
         Although Notion doesn't support uploading files, if you pass a file object containing a file hosted by Notion,
         it remains one of the files. To remove any file, just don't pass it in the update response.
 
         InternalFiles are a file object corresponding to a file that has been uploaded to Notion.
@@ -72,32 +73,46 @@
 
 
 class Icon(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(self, file_url: str, /) -> None:
         """
-        Internal object for setting the icon of a page. Internal file type Icons currently not supported.
+        Internal object for setting the icon of a page.
+        Internal file type Icons currently not supported.
         """
         super().__init__()
         self.set("icon", ExternalFile(file_url))
 
 
+class Cover(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(self, file_url: str, /) -> None:
+        """
+        Internal object for setting the cover of a page.
+        Internal file type covers currently not supported.
+        """
+        super().__init__()
+        self.set("cover", ExternalFile(file_url))
+
+
 class ExternalFile(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         url: str,
         /,
         *,
         caption: Optional[Sequence[Union[RichText, Mention, Equation]]] = None,
     ) -> None:
-        """The Notion API supports adding, retrieving, and updating links to external files.
-        The name of the file. For "external" file objects, the name is the same as the file's host URL.
+        """
+        The Notion API supports adding, retrieving, and updating links to external files.
+        For "external" file objects, the name is the same as the file's host URL.
 
         https://developers.notion.com/reference/file-object#external-files
         """
         super().__init__()
         self.set("type", "external")
         self.set("external", _NotionURL(url))
         self.set("caption", caption) if caption else None
```

### Comparing `notion_api-0.3.9/notion/properties/options.py` & `notion_api-0.4.0/notion/properties/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from enum import Enum
 from typing import Sequence
 
 __all__: Sequence[str] = (
     "CodeBlockLang",
     "BlockColor",
     "FunctionFormat",
-    "NumberFormats",
+    "NumberFormat",
     "PropertyColor",
 )
 
 
 class CodeBlockLang(str, Enum):
     abap = "abap"
     arduino = "arduino"
@@ -130,15 +130,15 @@
     show_original = "show_original"
     show_unique = "show_unique"
     sum = "sum"
     unchecked = "unchecked"
     unique = "unique"
 
 
-class NumberFormats(str, Enum):
+class NumberFormat(str, Enum):
     number = "number"
     number_with_commas = "number_with_commas"
     percent = "percent"
     dollar = "dollar"
     canadian_dollar = "canadian_dollar"
     euro = "euro"
     pound = "pound"
```

### Comparing `notion_api-0.3.9/notion/properties/propertyobjects.py` & `notion_api-0.4.0/notion/properties/propertyobjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,26 @@
 NOTE: It is not possible to update a status database property in the current version of the Notion API. 
       Update these values from the Notion UI, instead.
 
 https://developers.notion.com/reference/property-object
 """
 from __future__ import annotations
 
-import abc
+from abc import ABCMeta
 from typing import Optional, Sequence, Union
 
-from notion.exceptions.errors import NotionInvalidJson
 from notion.properties.build import NotionObject
-from notion.properties.options import FunctionFormat, NumberFormats, PropertyColor
+from notion.properties.options import FunctionFormat, NumberFormat, PropertyColor
+from notion.properties.richtext import RichText
 
 __all__: Sequence[str] = (
+    "DatabaseDescription",
+    "TitlePropertyObject",
     "RelationPropertyObject",
+    "Option",
     "MultiSelectPropertyObject",
     "SelectPropertyObject",
     "NumberPropertyObject",
     "FormulaPropertyObject",
     "CheckboxPropertyObject",
     "PeoplePropertyObject",
     "PhoneNumberPropertyObject",
@@ -57,26 +60,32 @@
     "CreatedTimePropertyObject",
     "CreatedByPropertyObject",
     "LastEditedTimePropertyObject",
     "LastEditedByPropertyObject",
     "DatePropertyObject",
     "EmailPropertyObject",
     "FilesPropertyObject",
-    "TitlePropertyObject",
     "URLPropertyObject",
     "RollupPropertyObject",
-    "Option",
 )
 
 
-class PropertyObject(metaclass=abc.ABCMeta):
+class PropertyObject(metaclass=ABCMeta):
     def __init__(self, property_name: str) -> None:
         self.name = property_name
 
 
+class DatabaseDescription(NotionObject):
+    __slots__: Sequence[str] = ()
+
+    def __init__(self, description: Sequence[RichText]) -> None:
+        super().__init__()
+        self.set("description", description)
+
+
 class TitlePropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(self, property_name: str, /) -> None:
         """
         A title database property controls the title that appears at the top of a page when a
         database row is opened. The title type object itself is empty; there is no additional configuration.
@@ -117,65 +126,51 @@
         super().__init__()
         self.set("database_id", database_id)
         self.set("type", "single_property")
         self.set("single_property", {})
 
 
 class RelationPropertyObject(PropertyObject, NotionObject):
-    __slots__: Sequence[str] = ("name", "_related_to")
+    __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        /,
-        *,
-        database_id: str,
-        synced_property_name: Optional[str] = None,
+        relation_type: Optional[Union[_DualProperty, _SingleProperty]] = None,
     ) -> None:
         """
         Use classmethods:
          - `dual`
          - `single`
 
         https://developers.notion.com/reference/property-object#relation
         """
         super().__init__(property_name=property_name)
-        self.relation_type: Union[_DualProperty, _SingleProperty]
-
-        try:
-            self.set("type", "relation")
-            self.set("relation", self.relation_type)
-        except AttributeError:
-            raise NotionInvalidJson("Use classmethods.")
+        self.set("type", "relation")
+        self.set("relation", relation_type)
 
     @classmethod
     def dual(
-        cls, property_name: str, database_id: str, synced_property_name: str, /
+        cls, property_name: str, database_id: str, synced_property_name: str
     ) -> RelationPropertyObject:
         """
         :param database_id: (required) The database that the relation property refers to.\
                              The corresponding linked page values must belong to the database in order to be valid.
         :param synced_property_name: (required) The name of the corresponding property that is\
                                       updated in the related database when this property is changed.
         """
-        cls.relation_type = _DualProperty(database_id, synced_property_name)
-        return cls(
-            property_name,
-            database_id=database_id,
-            synced_property_name=synced_property_name,
-        )
+        return cls(property_name, _DualProperty(database_id, synced_property_name))
 
     @classmethod
-    def single(cls, property_name: str, database_id: str, /) -> RelationPropertyObject:
+    def single(cls, property_name: str, database_id: str) -> RelationPropertyObject:
         """
         :param database_id: (required) The database that the relation property refers to.\
                              The corresponding linked page values must belong to the database in order to be valid.
         """
-        cls.relation_type = _SingleProperty(database_id)
-        return cls(property_name, database_id=database_id)
+        return cls(property_name, _SingleProperty(database_id))
 
 
 class Option(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self, option_name: str, color: Optional[Union[PropertyColor, str]] = None, /
@@ -190,57 +185,53 @@
         self.set("name", option_name)
         self.set("color", color) if color else None
 
 
 class MultiSelectPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, *, options: list[Option]) -> None:
+    def __init__(self, property_name: str, /, options: list[Option]) -> None:
         """https://developers.notion.com/reference/property-object#multi-select"""
         super().__init__(property_name=property_name)
         self.set("type", "multi_select")
         self.nest("multi_select", "options", options)
 
 
 class SelectPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, *, options: list[Option]) -> None:
+    def __init__(self, property_name: str, /, options: list[Option]) -> None:
         """https://developers.notion.com/reference/property-object#select"""
         super().__init__(property_name=property_name)
         self.set("type", "select")
         self.nest("select", "options", options)
 
 
 class NumberPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        format: Optional[Union[NumberFormats, str]] = None,
         /,
+        format: Optional[Union[NumberFormat, str]] = NumberFormat.number.value,
     ) -> None:
         """https://developers.notion.com/reference/property-object#number"""
-
         super().__init__(property_name=property_name)
         self.set("type", "number")
-        if not format:
-            self.nest("number", "format", NumberFormats.number)
-        else:
-            self.nest("number", "format", format)
+        self.nest("number", "format", format)
 
 
 class FormulaPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, expression: str, /) -> None:
+    def __init__(self, property_name: str, /, expression: str) -> None:
         """
         :param expression: (required) The formula that is used to compute the values for this property.\
-            Refer to the Notion help center for information about formula syntax.
+                            Refer to the Notion help center for information about formula syntax.
             
         https://developers.notion.com/reference/property-object#formula
         """
         super().__init__(property_name=property_name)
         self.set("type", "formula")
         self.nest("formula", "expression", expression)
 
@@ -369,15 +360,17 @@
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
         relation_property_name: str,
         rollup_property_name: str,
-        function: Union[FunctionFormat, str],
+        function: Optional[
+            Union[FunctionFormat, str]
+        ] = FunctionFormat.show_original.value,
         /,
     ) -> None:
         """https://developers.notion.com/reference/property-object#rollup"""
         super().__init__(property_name=property_name)
         self.set("type", "rollup")
         self.nest("rollup", "relation_property_name", relation_property_name)
         self.nest("rollup", "rollup_property_name", rollup_property_name)
```

### Comparing `notion_api-0.3.9/notion/properties/propertyvalues.py` & `notion_api-0.4.0/notion/properties/propertyvalues.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 
 FilesPropertyValue can be found in `notion.properties.files`.
 
 https://developers.notion.com/reference/page-property-values
 """
 from __future__ import annotations
 
-import abc
+from abc import ABCMeta
 from datetime import datetime
 from typing import TYPE_CHECKING, Optional, Sequence, Union
 
 from notion.properties.build import NotionObject
-from notion.properties.common import BotObject, UserObject, _NotionUUID
+from notion.properties.common import UserObject, _NotionUUID
 from notion.properties.options import FunctionFormat
 from notion.properties.propertyobjects import Option, PropertyObject
 from notion.properties.richtext import Equation, Mention, RichText
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
@@ -77,15 +77,15 @@
     "EmailPropertyValue",
     "NumberPropertyValue",
     "PhoneNumberPropertyValue",
     "URLPropertyValue",
 )
 
 
-class PagePropertyValue(metaclass=abc.ABCMeta):
+class PagePropertyValue(metaclass=ABCMeta):
     def __init__(self, property_name: str) -> None:
         self.name = property_name
 
 
 class Properties(NotionObject):
     __slots__: Sequence[str] = ()
 
@@ -94,15 +94,14 @@
         A page object is made up of page properties that contain data about the page.
         When you send a request to Create a page, you set the page properties in the properties object body param.
         Retrieve a page gets the identifier, type, and value of a page's properties.
         Retrieve a page property item returns information about a single property ID.
 
         https://developers.notion.com/reference/page-property-values"""
         super().__init__()
-
         for prop in properties:
             if not hasattr(prop, "name"):
                 raise AttributeError("Missing attribute `property_name`")
 
             if isinstance(prop, TitlePropertyValue):
                 self.nest("properties", prop.name, prop.get("title"))
             else:
@@ -111,23 +110,23 @@
 
 class RichTextPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        rich_text_array: Sequence[Union[RichText, Mention, Equation]],
         /,
+        rich_text: Sequence[Union[RichText, Mention, Equation]],
     ) -> None:
         r"""
         The purpose of the rich text property value is to provide the key `rich_text`,
         whereas the object `notion.properties.RichText` has the key `text`.
 
         ---
-        :param rich_text_array: (required) An array of rich text objects.
+        :param rich_text: (required) An array of rich text objects.
         Using `shift+enter` for multi-line text blocks results in a separate `text` key with a newline escape.
         ```json
         },  // ... first text line above
         {
             "type": "text",
             "text": {
                 "content": "\nthis is the second line of a block"
@@ -152,23 +151,23 @@
 
         The RichText Object: https://developers.notion.com/reference/rich-text
 
         The RichText Property Value: https://developers.notion.com/reference/page-property-values#rich-text
         """
         super().__init__(property_name=property_name)
         self.set("type", "rich_text")
-        self.set("rich_text", rich_text_array)
+        self.set("rich_text", rich_text)
 
 
 class TitlePropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, title_: Sequence[Union[RichText, Mention, Equation]], /) -> None:
+    def __init__(self, title_: Sequence[Union[RichText, Mention]]) -> None:
         """
-        :param title: (required) An array of rich text objects: `notion.properties.propertyvalues.RichText`
+        :param title: (required) An array of rich text objects
 
         https://developers.notion.com/reference/page-property-values#title
         """
         super().__init__(property_name="title")
         self.set_array(self.name, title_)
 
 
@@ -192,68 +191,61 @@
                        If the "date" value is a range, then start represents the start of the range.
         :param end: (optional) A string representing the end of a date range.\
                      If the value is null, then the date value is not a range.
 
         https://developers.notion.com/reference/page-property-values#date
         """
         super().__init__(property_name=property_name)
-
         self.nest("date", "start", start)
         self.nest("date", "end", end) if end else None
 
 
 class RelationPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        *related_ids: list[_NotionUUID],
-        has_more: Optional[bool] = None,
+        /,
+        related_ids: Sequence[_NotionUUID],
     ) -> None:
         """
         NOTE: updating a relation property value with an empty array will clear the list.
 
         ---
         :param related_ids: (required) An array of related page references.\
                              A page reference is an object with an id key and a string value (UUIDv4)\
                              corresponding to a page ID in another database.
 
-        :param has_more: (optional) If a relation has more than 25 references, then the has_more value for\
-                          the relation in the response object is true. If a relation doesn't\
-                          exceed the limit, then has_more is false.
-
         https://developers.notion.com/reference/page-property-values#relation
         """
         super().__init__(property_name=property_name)
         self.set("type", "relation")
-        self.set("relation", [id for id in related_ids][0])
-        if has_more:
-            self.set("has_more", True)
+        self.set("relation", [id for id in related_ids])
 
 
 class StatusPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, status_option: Option, /) -> None:
+    def __init__(self, property_name: str, /, status_option: Option) -> None:
         """
         :param status_option: (required) a single status option: `notion.properties.Option`\
                                containing `name` and `notion.properties.PropertyColor`
 
         https://developers.notion.com/reference/page-property-values#status
         """
         super().__init__(property_name=property_name)
         self.set("type", "status")
         self.set("status", status_option)
 
 
 class SelectPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, select_option: Option, /) -> None:
+    def __init__(self, property_name: str, /, select_option: Option) -> None:
         """
         When selecting options, If the select database property does not yet have an option by the input name,
         then the name will be added to the database schema if the integration also has write access to the parent database.
         
         ---
         :param select_option: (required) a single select option: `notion.properties.Option`\
                                containing `name` and `notion.properties.PropertyColor`\
@@ -265,15 +257,15 @@
         self.set("type", "select")
         self.set("select", select_option)
 
 
 class MultiSelectPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, options_array: list[Option], /) -> None:
+    def __init__(self, property_name: str, /, options_array: list[Option]) -> None:
         """
         The MultiSelectPropertyValue contains an array of `notion.properties.Option` objects.
         When selecting options, If the multi-select database property does not yet have an option by the input name,
         then the name will be added to the database schema if the integration also has write access to the parent database.
 
         ---
         :param options_array: (required) array of `notion.properties.Option`\
@@ -286,29 +278,25 @@
         self.set("type", "multi_select")
         self.set("multi_select", options_array)
 
 
 class CheckboxPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, checkbox_value: bool, /) -> None:
-        """
-        :param checkbox_value: (required) Whether the checkbox is checked (true) or unchecked (false).
-
-        https://developers.notion.com/reference/page-property-values#checkbox
-        """
+    def __init__(self, property_name: str, /, checkbox_value: bool) -> None:
+        """https://developers.notion.com/reference/page-property-values#checkbox"""
         super().__init__(property_name=property_name)
         self.set("type", "checkbox")
         self.set("checkbox", checkbox_value)
 
 
 class PeoplePropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, user_array: Sequence[UserObject], /) -> None:
+    def __init__(self, property_name: str, /, user_array: Sequence[UserObject]) -> None:
         """
         :param user_array: (required) An array of user objects.\
                             The Retrieve a page endpoint can't be guaranteed to return more than 25 people\
                             per people page property. If a people page property includes more than 25 people,\
                             then you can use the Retrieve a page property item endpoint for the specific
                             people property to get a complete list of people.
 
@@ -318,19 +306,18 @@
         self.set("type", "people")
         self.set("people", user_array)
 
 
 class RollupPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, function: FunctionFormat, /) -> None:
+    def __init__(
+        self, property_name: str, /, function: Union[FunctionFormat, str]
+    ) -> None:
         """
-        :param function: (required) `notion.properties.FunctionFormat`, function to update property to.
-
-        ---
         If the results of the rollup is a date (e.g. function = latest date),
         the results will be a DatePropertyValue.
 
         If the results of the rollup is a number (e.g. function = sum),
         the results will be a NumberPropertyValue.
 
         If the results of the rollup is anything requireing multiple values (e.g. function = show original),
@@ -344,47 +331,42 @@
         self.set("type", "rollup")
         self.nest("rollup", "function", function)
 
 
 class EmailPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, email: str, /) -> None:
+    def __init__(self, property_name: str, /, email: str) -> None:
         """https://developers.notion.com/reference/page-property-values#email"""
         super().__init__(property_name=property_name)
         self.set("type", "email")
         self.set("email", email)
 
 
 class NumberPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, number: Union[float, timedelta], /) -> None:
+    def __init__(self, property_name: str, /, number: Union[float, timedelta]) -> None:
         """https://developers.notion.com/reference/page-property-values#number"""
         super().__init__(property_name=property_name)
         self.set("type", "number")
         self.set("number", number)
 
 
 class PhoneNumberPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, phone_number: str, /) -> None:
-        """
-        :param phone_number: (required) A string representing a phone number.
-            No phone number format is enforced.
-
-        https://developers.notion.com/reference/page-property-values#phone-number
-        """
+    def __init__(self, property_name: str, /, phone_number: str) -> None:
+        """https://developers.notion.com/reference/page-property-values#phone-number"""
         super().__init__(property_name=property_name)
         self.set("type", "phone_number")
         self.set("phone_number", phone_number)
 
 
 class URLPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, url: str, /) -> None:
+    def __init__(self, property_name: str, /, url: str) -> None:
         """https://developers.notion.com/reference/page-property-values#url"""
         super().__init__(property_name=property_name)
         self.set("type", "url")
         self.set("url", url)
```

### Comparing `notion_api-0.3.9/notion/properties/richtext.py` & `notion_api-0.4.0/notion/properties/richtext.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/query/__init__.py` & `notion_api-0.4.0/notion/query/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/query/compound.py` & `notion_api-0.4.0/notion/query/compound.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/query/conditions.py` & `notion_api-0.4.0/notion/query/conditions.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/query/propfilter.py` & `notion_api-0.4.0/notion/query/propfilter.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,31 +17,32 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
 
+from datetime import datetime
 from typing import Any, Sequence, Union
 
 from notion.properties.build import NotionObject
 from notion.query.conditions import *
 
 __all__: Sequence[str] = ["PropertyFilter"]
 
 
 class PropertyFilter(NotionObject):
-    __slots__: Sequence[str] = ("_property_type",)
+    __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         property_name: str,
         filter_condition: FilterConditions,
         filter_value: Any,
-        _property_type: str,
+        property_type: str,
     ) -> None:
         """
         A filter is a single condition used to specify and limit the entries returned from a database query.
         Database queries can be filtered by page property values.
 
         Use classmethods:
             - text
@@ -64,152 +65,152 @@
         and a key corresponding with the type of the database property identified by property.
         The value is an object containing a type-specific filter condition
 
         https://developers.notion.com/reference/post-database-query-filter#type-specific-filter-conditions
         """
         super().__init__()
         self.nest("filter", "property", property_name)
-        self.nest("filter", _property_type, {filter_condition: filter_value})
+        self.nest("filter", property_type, {filter_condition: filter_value})
 
     @classmethod
     def text(
         cls,
         property_name: str,
         property_type: TextTypes,
         filter_condition: TextConditions,
         filter_value: Union[str, bool],
         /,
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#rich-text"""
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type=property_type
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def checkbox(
         cls,
         property_name: str,
         filter_condition: CheckboxConditions,
         filter_value: bool,
         /,
+        *,
+        property_type: str = "checkbox",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#checkbox"""
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type="checkbox"
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def number(
         cls,
         property_name: str,
         filter_condition: NumberConditions,
         filter_value: Union[str, float, bool],
         /,
+        property_type: str = "number",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#number"""
 
-        return cls(property_name, filter_condition, filter_value, _property_type="number")
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def select(
         cls,
         property_name: str,
         filter_condition: SelectConditions,
         filter_value: Union[str, bool],
         /,
+        property_type: str = "select",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#select"""
 
-        return cls(property_name, filter_condition, filter_value, _property_type="select")
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def multi_select(
         cls,
         property_name: str,
         filter_condition: MultiSelectConditions,
         filter_value: Union[str, bool],
         /,
+        property_type: str = "multi_select",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#multi-select"""
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type="multi_select"
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def status(
         cls,
         property_name: str,
         filter_condition: StatusConditions,
         filter_value: Union[str, bool],
         /,
+        property_type: str = "status",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#status"""
 
-        return cls(property_name, filter_condition, filter_value, _property_type="status")
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def date(
         cls,
         property_name: str,
         property_type: DateTypes,
         filter_condition: DateConditions,
-        filter_value: Union[str, bool, dict[str, Any]],
+        filter_value: Union[str, bool, dict[str, Any], datetime],
         /,
     ) -> PropertyFilter:
         """
         When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`
 
+        :param filter_value: - When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`\
+                             - If value is datetime, it will be converted to ISO 8601 format.
+
         https://developers.notion.com/reference/post-database-query-filter#date
         """
+        if isinstance(filter_value, datetime):
+            filter_value = filter_value.isoformat()
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type=property_type
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def people(
         cls,
         property_name: str,
         property_type: PeopleTypes,
         filter_condition: PeopleConditions,
         filter_value: Union[str, bool],
         /,
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#people"""
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type=property_type
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def files(
         cls,
         property_name: str,
         filter_condition: FilesConditions,
         /,
+        filter_value: bool = True,
+        property_type: str = "files",
     ) -> PropertyFilter:
         """
         Only available `filter_value` is `true`.
 
         https://developers.notion.com/reference/post-database-query-filter#files-filter-condition
         """
 
-        return cls(
-            property_name, filter_condition, filter_value=True, _property_type="files"
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def relation(
         cls,
         property_name: str,
         filter_condition: RelationConditions,
         filter_value: Union[str, bool],
         /,
+        property_type: str = "relation",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#relation"""
 
-        return cls(
-            property_name, filter_condition, filter_value, _property_type="relation"
-        )
+        return cls(property_name, filter_condition, filter_value, property_type)
```

### Comparing `notion_api-0.3.9/notion/query/sort.py` & `notion_api-0.4.0/notion/query/sort.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/notion/query/timestamp.py` & `notion_api-0.4.0/notion/query/timestamp.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/.gitignore` & `notion_api-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/LICENSE` & `notion_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.3.9/pyproject.toml` & `notion_api-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "notion-api", 
     "wrapper", 
     "notion-version-2022-06-28"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
 dependencies = [
     "python-dotenv==1.0.0",
     "requests==2.28.2",
```

### Comparing `notion_api-0.3.9/PKG-INFO` & `notion_api-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: notion-api
-Version: 0.3.9
+Version: 0.4.0
 Summary: An unofficial wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.
 Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api
 Author-email: Alan Vickers <alan.k.vickers@gmail.com>
 License-File: LICENSE
 Keywords: notion-api,notion-version-2022-06-28,wrapper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: pytz==2022.7.1
 Requires-Dist: requests==2.28.2
 Requires-Dist: tzlocal==4.2
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
@@ -42,169 +43,194 @@
     &nbsp;
     <img alt="last commit" src="https://img.shields.io/github/last-commit/ayvi-0001/notion-api?color=%239146ff"></a>
     &nbsp;
     <a href="https://developers.notion.com/reference/versioning"><img alt="notion versioning" src="https://img.shields.io/static/v1?label=notion-API-version&message=2022-06-28&color=%232e1a00"></a>
     &nbsp;
 </p>
 <p align="center">
-    <a href="https://github.com/ayvi-0001/notion-api/blob/main/LICENSE"><img alt="license: MIT" src="https://img.shields.io/static/v1?label=license&message=MIT&color=informational"></a>
+    <a href="https://github.com/ayvi-0001/notion-api/blob/main/LICENSE"><img alt="license: MIT" src="https://img.shields.io/github/license/ayvi-0001/notion-api?color=informational"></a>
     &nbsp;
     <a href="https://github.com/psf/black"><img alt="code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
     &nbsp;
     <a href="https://pycqa.github.io/isort/"><img alt="code style: black" src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336"></a>
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
+A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion. This project is still a work in progress, and features will continue to change. Below are a few examples of the current functionality. 
+
+<br>
+
 <div border="0" align="center">
     <table>
         <tr>
-            <td align="center"><b>A few useful links:</b></td>
+            <td align="center"><b>Links: Notion API Updates</b></td>
         </tr>
             <td> <a href="https://developers.notion.com/reference/intro">API Reference</a></td><tr>
         </td>
-            <td><a href="https://developers.notion.com/page/changelog">Notion API Changlog </img></a></tr>
+            <td><a href="https://developers.notion.com/page/changelog">Notion API Changelog </img></a></tr>
             <td> <a href="https://www.notion.so/releases">Notion.so Releases</a></td></tr>
             <td> <a href="https://developers.notion.com/page/notion-platform-roadmap">Notion Platform Roadmap</a></td>
         </tr>
     </table>
 </div>
 
-<br>
-
-
-A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
-
-This project is still a work in progress, and features will continue to change. Below are a few examples of the current functionality. 
+---
 
-# Install
+## Install
 ```
 pip install -U notion-api
 ```
 
-# Usage
+## Usage
 ```py
 import dotenv
 
 import notion
 
-dotenv.load_dotenv()  # client will check for env variable 'NOTION_TOKEN'.
+# client will check env variables for 'NOTION_TOKEN'
+dotenv.load_dotenv()  
 
 homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
 parent_db = notion.Database(homepage.parent_id)
 
-# or assign through `token` parameter.
-homepage = notion.Page('773b08ff38b44521b44b115827e850f2', token="secret_n2m52d1***")
+# will also look for env var `TZ` to set the timezone for all notion objects. If not found, will default to local timezone.
+```
 
+`__getitem__` searchs for page property values when indexing a Page, and for property objects when indexing a Database.
 
-# __get_item__ searchs for page property values if indexing a Page..
+```py
 homepage['dependencies']
 # {
 #     "id": "WYYq",
 #     "type": "relation",
 #     "relation": [
 #         {
 #             "id": "7bcbc8e6-e237-434b-bd0d-6b56e044200b"
 #         }
 #     ],
 #     "has_more": false
 # }
 
-# ..and searchs for property objects if indexing a Database.
 parent_db['dependencies']
 # {
 #     "id": "WYYq",
 #     "name": "dependencies",
 #     "type": "relation",
 #     "relation": {
 #         "database_id": "f5984a7e-2257-4ab0-9d0a-23ea12324031",
 #         "type": "dual_property",
 #         "dual_property": {
 #             "synced_property_name": "blocked",
 #             "synced_property_id": "wx%7DQ"
 #         }
 #     }
 # }
+```
+
+**_See usage of retrieving values from a page in examples/retrieving-property-items.md_**  
+
+Below is a brief example if we were wanting to get the page id from the above property `dependencies` in `homepage`.
+
+```py
+from notion import propertyitems
 
-homepage.last_edited.date() # out: 01/15/2023
-homepage.title = "New Page Title"
+related_id: list[str] = propertyitems.relation(homepage.dependencies)
+```
+```py
+>>> ["7bcbc8e6-e237-434b-bd0d-6b56e044200b"]
 ```
 
----
+Both Page's and Database's have setters for title/icon/cover.
+
+```py
+homepage.title = "new page"
+homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg"
+```
+
+<p align="center"> <img src="examples/images/new_page.png"> </p>
+
 <br>
 
 ## Creating Pages/Databases/Blocks
 
-The current version of the Notion api does not allow pages to be created to the parent `workspace`.
+The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
 Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
 
 ```py
 new_database = notion.Database.create(
-    homepage, database_title="A new database", name_column="name"
-) 
-# name column refers to the column containing pages/page titles. 
-# Defaults to "Name" if None (all strings in Notion API are case-sensitive).
+    parent_instance=testpage,
+    database_title="Title",
+    name_column="page", # This is the column containing page names. Defaults to "Name".
+    is_inline=True,
+    description="Example Database.",
+)
 
 new_page = notion.Page.create(new_database, page_title="A new database row")
 ```
 
-Blocks can be created with `notion.api.blocktypefactory.BlockFactory` by appending to an exisiting Block or Page. The new block is always returned as a `notion.api.notionblock.Block` instance.
+Blocks can be created with `notion.api.blocktypefactory.BlockFactory` by appending to an exisiting Block or Page.  
+The new block is always returned as an instance of `notion.api.notionblock.Block`.
 ```py
 from notion import properties as prop
 
 # `new_synced_block` refers to the original synced block in the Notion UI.
 original_synced_block = notion.BlockFactory.new_synced_block(homepage)
 
 # Adding content to the synced block
-notion.BlockFactory.paragraph(original_synced_block, [prop.RichText('This is a synced block.')])
-
+notion.BlockFactory.paragraph(
+    original_synced_block, [prop.RichText("This is a synced block.")]
+)
 # Referencing the synced block in a new page.
 notion.BlockFactory.reference_synced_block(new_page, original_synced_block.id)
 ```
 
-**_Example function: Appending blocks to a page as a reminder._**
+<br>
+
+### Example Workflow: **_Appending blocks to a page as a reminder._**
 
 ```py
-def in_block_reminder(page_id: str, message: str, user_name: str) -> None:
-    target_page = notion.Page(page_id)
+def in_block_reminder(page: notion.Page, message: str, user_name: str) -> None:
     mentionblock = notion.BlockFactory.paragraph(
-        target_page,
+        page,
         [
             prop.Mention.user(
-                notion.Workspace.retrieve_user(user_name=user_name),
+                notion.Workspace().retrieve_user(user_name=user_name),
                 annotations=prop.Annotations(
                     code=True, bold=True, color=prop.BlockColor.purple
                 ),
             ),
             prop.RichText(" - "),
             prop.Mention.date(
                 datetime.now().astimezone(target_page.tz).isoformat(),
                 annotations=prop.Annotations(
                     code=True, bold=True, color=prop.BlockColor.purple_background
                 ),
             ),
             prop.RichText(":"),
         ],
     )
+    # First method returned the newly created block that we append to here:
     notion.BlockFactory.paragraph(mentionblock, [prop.RichText(message)])
-    notion.BlockFactory.divider(target_page)
+    notion.BlockFactory.divider(page)
 ```
 
 ```py
->>> in_block_reminder(page_id="0b9eccfa890e4c3390175ee10c664a35", message="message here", user_name="Your Name")
+>>> my_page = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
+>>> in_block_reminder(page=my_page, message="message here", user_name="Your Name")
 ```
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/example_function_reminder.png">
+    <img src="examples/images/example_function_reminder.png">
 </p>
 
----
 <br>
 
-## Add, Set, & Delete - Page property values / Database property objects
+## Add, Set, & Delete: Page property values | Database property objects
 
 The first argument for all database column methods is the name of the property,  
 If it does not exist, then a new property object is created.  
 If it already exists, then the method will overwrite it.
 
 If the name passed already exists, but it's a different column type than the method used - then the API will overwrite this and change the property object to the new column type.  
 The original parameters will be saved if you decide to switch back (i.e. if you change a formula column to a select column, upon changing it back to a formula column, the original formula expression will still be there).   
@@ -225,15 +251,14 @@
 
 # if an option does not already exist, a new one will be created with a random color.
 # this is not true for `status` column types, which can only be edited via UI.
 
 new_page.set_multiselect("options", ["option-a", "option-b"])
 ```
 
----
 <br>
 
 ## Database Queries
 
 A single `notion.query.propfilter.PropertyFilter` is equivalent to filtering one property type in Notion.
 To build filters equivalent to Notion's 'advanced filters', use `notion.query.compound.CompoundFilter`.
 
@@ -265,22 +290,25 @@
 query_result = new_database.query(
     filter=query_filter,
     sort=query_sort,
     page_size=5,
     filter_property_values=["name", "options"],
 )
 ```
----
+
+A database also has the `query_pages()` method. It takes the same parameters, but for each page object in the `results` array, it retrieves the id(s), and instead returns a list of `notion.Page`.
+
 <br>
 
 ## Exceptions & Validating Responses
 
-```py
-# Errors in Notion requests return an object with the keys: 'object', 'status', 'code', and 'message'
+Errors in Notion requests return an object with the keys: 'object', 'status', 'code', and 'message'.
+Exceptions are raised by matching the error code and returning the message. For example:
 
+```py
 homepage._patch_properties(payload={'an_incorrect_key':'value'})
 # Example error object for line above..
 # {
 #   'object': 'error', 
 #   'status': 400, 
 #   'code': 'validation_error', 
 #   'message': 'body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.'
@@ -293,25 +321,32 @@
     homepage._patch_properties(payload={'an_incorrect_key':'value'})
 File "c:\...\notion\exceptions\validate.py", line 48, in validate_response
     raise NotionValidationError(message)
 notion.exceptions.errors.NotionValidationError: body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.
 Error 400: The request body does not match the schema for the expected parameters.
 ```
 
-A common error to look out for is `notion.exceptions.errors.NotionObjectNotFound`  
+Possible errors are:
+ - `NotionInvalidJson`
+ - `NotionInvalidRequestUrl`
+ - `NotionInvalidRequest`
+ - `NotionValidationError`
+ - `NotionMissingVersion`
+ - `NotionUnauthorized`
+ - `NotionRestrictedResource`
+ - `NotionObjectNotFound`
+ - `NotionConflictError`
+ - `NotionRateLimited`
+ - `NotionInternalServerError`
+ - `NotionServiceUnavailable`
+ - `NotionDatabaseConnectionUnavailable`
 
-This error is often raised because your bot has not been added as a connection to the page.  
+A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/directory_add_connections.png">  
+    <img src="examples/images/directory_add_connections.png">  
 </p>
 
-By default, a bot will have access to the children of any Parent object it has access too.
-
-Certain errors are returned with a long list of possible causes for failing validation,
-In these cases, the error is often the outlier in the list - for example:
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/ayvi-0001/notion-api/main/images/append_child_block_error.png"> 
-</p>
+By default, a bot will have access to the children of any Parent object it has access too. Be sure to double check this connection when moving pages.  
+If you're working on a page that your token has access to via its parent page/database, but you never explicitly granted access to the child page -  and you later move that child page out, then it will lose access.
 
 ---
```

