# Comparing `tmp/yao-0.0.1.tar.gz` & `tmp/yao-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.1.tar", last modified: Wed Apr  5 07:23:57 2023, max compression
+gzip compressed data, was "yao-0.0.2.tar", last modified: Tue Apr 18 07:27:56 2023, max compression
```

## Comparing `yao-0.0.1.tar` & `yao-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.064075 yao-0.0.1/
--rw-r--r--   0 ke         (501) wheel        (0)      429 2023-04-05 07:23:57.063666 yao-0.0.1/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-04-05 07:23:57.064144 yao-0.0.1/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      967 2023-04-05 07:18:58.000000 yao-0.0.1/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.058381 yao-0.0.1/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-17 09:50:59.000000 yao-0.0.1/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-02 06:21:11.000000 yao-0.0.1/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-02 04:59:57.000000 yao-0.0.1/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     7904 2023-04-02 03:13:11.000000 yao-0.0.1/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.059485 yao-0.0.1/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:08:06.000000 yao-0.0.1/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.060035 yao-0.0.1/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.1/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-03-13 11:43:18.000000 yao-0.0.1/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-02 03:15:28.000000 yao-0.0.1/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-03-29 09:20:32.000000 yao-0.0.1/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.060600 yao-0.0.1/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.1/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-03-11 07:41:38.000000 yao-0.0.1/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4414 2023-04-02 03:15:28.000000 yao-0.0.1/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-03-11 08:51:27.000000 yao-0.0.1/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.061165 yao-0.0.1/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.1/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-02-27 07:13:36.000000 yao-0.0.1/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4066 2023-03-25 02:33:40.000000 yao-0.0.1/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-03-11 07:41:38.000000 yao-0.0.1/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.061686 yao-0.0.1/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:01.000000 yao-0.0.1/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-03-11 05:26:27.000000 yao-0.0.1/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4446 2023-04-02 03:15:28.000000 yao-0.0.1/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-03-11 07:41:38.000000 yao-0.0.1/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.062200 yao-0.0.1/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.1/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-03-10 11:36:17.000000 yao-0.0.1/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3307 2023-03-25 05:43:46.000000 yao-0.0.1/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-03-11 07:41:38.000000 yao-0.0.1/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-03-13 11:51:16.000000 yao-0.0.1/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7969 2023-03-25 05:51:56.000000 yao-0.0.1/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.062708 yao-0.0.1/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:19.000000 yao-0.0.1/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-03-11 05:25:41.000000 yao-0.0.1/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8252 2023-03-25 04:02:20.000000 yao-0.0.1/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-03-11 08:51:04.000000 yao-0.0.1/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.063342 yao-0.0.1/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:21:23.000000 yao-0.0.1/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-03-11 05:25:26.000000 yao-0.0.1/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11169 2023-04-02 03:15:28.000000 yao-0.0.1/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-03-25 03:02:47.000000 yao-0.0.1/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6841 2023-04-02 03:15:28.000000 yao-0.0.1/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    11439 2023-03-24 03:00:55.000000 yao-0.0.1/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     1803 2023-03-30 03:35:08.000000 yao-0.0.1/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-05 07:23:57.059088 yao-0.0.1/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      429 2023-04-05 07:23:57.000000 yao-0.0.1/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-04-05 07:23:57.000000 yao-0.0.1/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-04-05 07:23:57.000000 yao-0.0.1/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-04-05 07:23:57.000000 yao-0.0.1/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-04-05 07:23:57.000000 yao-0.0.1/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.426909 yao-0.0.2/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-18 07:27:56.426647 yao-0.0.2/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-04-18 07:27:56.426957 yao-0.0.2/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-04-18 07:22:00.000000 yao-0.0.2/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.421226 yao-0.0.2/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-17 09:50:59.000000 yao-0.0.2/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-02 06:21:11.000000 yao-0.0.2/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-02 04:59:57.000000 yao-0.0.2/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7904 2023-04-02 03:13:11.000000 yao-0.0.2/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.422379 yao-0.0.2/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:08:06.000000 yao-0.0.2/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.423055 yao-0.0.2/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.2/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-03-13 11:43:18.000000 yao-0.0.2/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-02 03:15:28.000000 yao-0.0.2/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-03-29 09:20:32.000000 yao-0.0.2/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.423608 yao-0.0.2/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:09.000000 yao-0.0.2/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-03-11 08:51:27.000000 yao-0.0.2/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.424213 yao-0.0.2/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.2/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-02-27 07:13:36.000000 yao-0.0.2/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.424782 yao-0.0.2/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:01.000000 yao-0.0.2/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-03-11 05:26:27.000000 yao-0.0.2/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.425329 yao-0.0.2/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.2/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-03-10 11:36:17.000000 yao-0.0.2/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-03-11 07:41:38.000000 yao-0.0.2/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-03-13 11:51:16.000000 yao-0.0.2/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-07 10:50:08.000000 yao-0.0.2/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.425885 yao-0.0.2/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 06:17:19.000000 yao-0.0.2/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-03-11 05:25:41.000000 yao-0.0.2/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:24:25.000000 yao-0.0.2/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-03-11 08:51:04.000000 yao-0.0.2/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.426441 yao-0.0.2/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:21:23.000000 yao-0.0.2/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-03-11 05:25:26.000000 yao-0.0.2/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:25:25.000000 yao-0.0.2/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-03-25 03:02:47.000000 yao-0.0.2/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-08 07:18:19.000000 yao-0.0.2/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-12 11:57:41.000000 yao-0.0.2/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1803 2023-03-30 03:35:08.000000 yao-0.0.2/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-18 07:27:56.421937 yao-0.0.2/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-04-18 07:27:56.000000 yao-0.0.2/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.1/setup.py` & `yao-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.1",
+    version="0.0.2",
     description="Dev",
     python_requires=">=3.9",
     author="Lsshu",
     author_email="admin@lsshu.cn",
-    url="https://github.com/lsshu",
+    url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3",
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
```

### Comparing `yao-0.0.1/yao/crud.py` & `yao-0.0.2/yao/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/db.py` & `yao-0.0.2/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/depends.py` & `yao-0.0.2/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/annex/main.py` & `yao-0.0.2/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/annex/schema.py` & `yao-0.0.2/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/appointment/crud.py` & `yao-0.0.2/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/appointment/main.py` & `yao-0.0.2/yao/function/appointment/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionAppointment.init().first(session=session, where=("name", item.name))
     if db_model is not None:
-        return SchemasError(message="Data Already Registered")
+        return SchemasError(message="数据已经存在！")
     bool_model = CrudFunctionAppointment.init().store(session=session, item=item)
     return Schemas(data=SchemasFunctionAppointmentResponse(**bool_model.to_dict()))
 
 
 @route("/_M_/{uuid}", module=name, router=router, methods=['patch'])
 @item_name_prefix
 async def update_patch_model(uuid: str, item: SchemasFunctionAppointmentStoreUpdate, session: Session = Depends(_session),
@@ -85,15 +85,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionAppointment.init().first(session=session, uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     CrudFunctionAppointment.init().update(session=session, uuid=uuid, item=item, exclude_unset=True)
     return Schemas()
 
 
 @route("/_M_", module=name, router=router, methods=['delete'])
 async def delete_models(uuids: List[str], session: Session = Depends(_session), auth: SchemasFunctionScopes = Security(auth_user, scopes=role_scopes + ["%s.delete" % name])):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yao-0.0.1/yao/function/appointment/schema.py` & `yao-0.0.2/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/company/main.py` & `yao-0.0.2/yao/function/company/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionCompany.init().first(session=session, where=("name", item.name))
     if db_model is not None:
-        return SchemasError(message="Data Already Registered")
+        return SchemasError(message="数据已经存在！")
     bool_model = CrudFunctionCompany.init().store(session=session, item=item)
     return Schemas(data=SchemasFunctionResponse(**bool_model.to_dict()))
 
 
 @route("/_M_/{uuid}", module=name, router=router, methods=['patch'])
 @item_name_prefix
 async def update_patch_model(uuid: str, item: SchemasFunctionStoreUpdate, session: Session = Depends(_session),
@@ -81,15 +81,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionCompany.init().first(session=session, uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     CrudFunctionCompany.init().update(session=session, uuid=uuid, item=item, exclude_unset=True)
     return Schemas()
 
 
 @route("/_M_", module=name, router=router, methods=['delete'])
 async def delete_models(uuids: List[str], session: Session = Depends(_session), auth: SchemasFunctionScopes = Security(auth_user, scopes=role_scopes + ["%s.delete" % name])):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yao-0.0.1/yao/function/company/schema.py` & `yao-0.0.2/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/department/main.py` & `yao-0.0.2/yao/function/department/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionDepartment.init().first(session=session, where=("name", item.name))
     if db_model is not None:
-        return SchemasError(message="Data Already Registered")
+        return SchemasError(message="数据已经存在！")
     if item.parent_id:
         parent_model = CrudFunctionDepartment.init().first(session=session, uuid=item.parent_id)
         if parent_model:
             item.parent_id = parent_model.id
     bool_model = CrudFunctionDepartment.init().store(session=session, item=item)
     return Schemas(data=SchemasFunctionResponse(**bool_model.to_dict()))
 
@@ -87,15 +87,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionDepartment.init().first(session=session, uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     CrudFunctionDepartment.init().update(session=session, uuid=uuid, item=item, exclude_unset=True)
     return Schemas()
 
 
 @route("/_M_", module=name, router=router, methods=['delete'])
 async def delete_models(uuids: List[str], session: Session = Depends(_session), auth: SchemasFunctionScopes = Security(auth_user, scopes=role_scopes + ["%s.delete" % name])):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yao-0.0.1/yao/function/department/schema.py` & `yao-0.0.2/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/log/main.py` & `yao-0.0.2/yao/function/log/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionLog.init().first(session=session, uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     CrudFunctionLog.init().update(session=session, uuid=uuid, item=item, exclude_unset=True)
     return Schemas()
 
 
 @route("/_M_", module=name, router=router, methods=['delete'])
 async def delete_models(uuids: List[str], session: Session = Depends(_session), auth: SchemasFunctionScopes = Security(auth_user, scopes=role_scopes + ["%s.delete" % name])):
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yao-0.0.1/yao/function/log/schema.py` & `yao-0.0.2/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/main.py` & `yao-0.0.2/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/model.py` & `yao-0.0.2/yao/function/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
     size = Column(Integer, nullable=False, comment="SIZE")
     width = Column(String(100), nullable=True, comment="宽")
     height = Column(String(190), nullable=True, comment="高")
 
     @property
     def preview_path(self):
         import os
-        from config import HOST_URL
-        return os.path.join(HOST_URL, self.path)
+        from config import STATIC_URL
+        return os.path.join(STATIC_URL, self.path)
 
 
 class ModelFunctionLogs(BaseCompanyModel):
     """ 日志 """
     __tablename__ = function_log_table_name
     scope = Column(String(100), nullable=True, comment="scope")
     methods = Column(String(32), nullable=True, comment="methods", index=True)
```

### Comparing `yao-0.0.1/yao/function/permission/main.py` & `yao-0.0.2/yao/function/permission/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,30 +91,30 @@
     :param pk:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionPermission.init(session=session).first(pk=pk)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     return Schemas(data=SchemasFunctionResponse(**db_model.to_dict()))
 
 
 @router.post('/{}'.format(name), name="get {}".format(name))
 async def store_model(item: SchemasFunctionStoreUpdate, session: Session = Depends(_session),
                       auth: SchemasFunctionScopes = Security(auth_user, scopes=permission_scopes + ["%s.store" % name])):
     """
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionPermission.init(session=session).first(where=("name", item.name))
     if db_model is not None:
-        return SchemasError(message="Data Already Registered")
+        return SchemasError(message="数据已经存在！")
     bool_model = CrudFunctionPermission.init(session=session).store(item=item)
     return Schemas(data=SchemasFunctionResponse(**bool_model.to_dict()))
 
 
 @router.put("/{}/{{pk}}".format(name), name="update {}".format(name))
 async def update_put_model(pk: int, item: SchemasFunctionStoreUpdate, session: Session = Depends(_session),
                            auth: SchemasFunctionScopes = Security(auth_user, scopes=permission_scopes + ["%s.update" % name])):
@@ -123,15 +123,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionPermission.init(session=session).first(pk=pk)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     bool_model = CrudFunctionPermission.init(session=session).update(pk=pk, item=item)
     return Schemas(data=SchemasFunctionResponse(**bool_model.to_dict()))
 
 
 @router.patch("/{}/{{pk}}".format(name), name="update {}".format(name))
 async def update_patch_model(pk: int, item: SchemasFunctionStoreUpdate, session: Session = Depends(_session),
                              auth: SchemasFunctionScopes = Security(auth_user, scopes=permission_scopes + ["%s.update" % name])):
@@ -140,15 +140,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionPermission.init(session=session).first(pk=pk)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     bool_model = CrudFunctionPermission.init(session=session).update(pk=pk, item=item, exclude_unset=True)
     return Schemas(data=SchemasFunctionResponse(**bool_model.to_dict()))
 
 
 @router.patch("/{}/{{pk}}/move_inside".format(name), name="update {}".format(name))
 async def move_inside_permission_model(pk: int, inside_id: int, session: Session = Depends(_session),
                                        auth: SchemasFunctionScopes = Security(auth_user, scopes=permission_scopes + ["%s.update" % name])):
```

### Comparing `yao-0.0.1/yao/function/permission/schema.py` & `yao-0.0.2/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/user/crud.py` & `yao-0.0.2/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/function/user/main.py` & `yao-0.0.2/yao/function/user/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     :param session:
     :param username:
     :param password:
     :return:
     """
     user = CrudFunctionUser.init().first(session=session, where=("username", username))
     if not user or not token_verify_password(plain_password=password, hashed_password=user.password):
-        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Incorrect username or password")
+        raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="账号或者密码不正确！")
     return user
 
 
 def token_authenticate_access_token(session, username: str, password: str, scopes: list) -> str:
     """
     认证用户且生成用户token
     :param session:
@@ -169,15 +169,15 @@
     :param uuid:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionUser.init(session=session).first(uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     return Schemas(data=SchemasFunctionUserResponse(**db_model.to_dict()))
 
 
 @router.post('/{}'.format(name), name="get {}".format(name))
 async def store_model(item: SchemasFunctionUserStoreUpdate, session: Session = Depends(_session),
                       auth: SchemasFunctionScopes = Security(auth_user, scopes=user_scopes + ["%s.store" % name])):
     """
@@ -186,15 +186,15 @@
     :param auth:
     :return:
     """
     item.prefix = item.prefix or auth.prefix
     item.username = "%s@%s" % (item.prefix, item.username.replace("%s@" % item.prefix, ""))
     db_model = CrudFunctionUser.init().first(session=session, where=("username", item.username))
     if db_model is not None:
-        return SchemasError(message="Data Already Registered")
+        return SchemasError(message="数据已经存在！")
     bool_model = CrudFunctionUser.init().store(session=session, item=item)
     return Schemas(data=SchemasFunctionUserResponse(**bool_model.to_dict()))
 
 
 @router.put("/{}/{{uuid}}".format(name), name="update {}".format(name))
 async def update_put_model(uuid: str, item: SchemasFunctionUserStoreUpdate, session: Session = Depends(_session),
                            auth: SchemasFunctionScopes = Security(auth_user, scopes=user_scopes + ["%s.update" % name])):
@@ -203,15 +203,15 @@
     :param item:
     :param session:
     :param auth:
     :return:
     """
     db_model = CrudFunctionUser.init(session=session).first(uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     item.prefix = item.prefix or auth.prefix
     item.username = "%s@%s" % (auth.prefix, item.username)
     CrudFunctionUser.init(session=session).update(uuid=uuid, item=item, exclude_unset=False)
     return Schemas()
 
 
 @router.patch("/{}/{{uuid}}".format(name), name="update {}".format(name))
@@ -224,15 +224,15 @@
     :param auth:
     :return:
     """
     item.prefix = item.prefix or auth.prefix
     item.username = "%s@%s" % (item.prefix, item.username.replace("%s@" % item.prefix, ""))
     db_model = CrudFunctionUser.init().first(session=session, uuid=uuid)
     if db_model is None:
-        return SchemasError(message="Data Not Found")
+        return SchemasError(message="数据没有找到！")
     CrudFunctionUser.init().update(session=session, uuid=uuid, item=item, exclude_unset=True, event=True, close=True)
     return Schemas()
 
 
 @router.delete("/{}/{{uuid}}".format(name), name="delete {}".format(name))
 async def delete_model(uuid: str, session: Session = Depends(_session),
                        auth: SchemasFunctionScopes = Security(auth_user, scopes=user_scopes + ["%s.delete" % name])):
```

### Comparing `yao-0.0.1/yao/function/user/schema.py` & `yao-0.0.2/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao/helpers.py` & `yao-0.0.2/yao/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     permissionObj = CrudFunctionPermission.init()
     for permission in permissions:
         _scope = permission.get('scope')
         _name = permission.get('name')
         _action = permission.get('action', [])
         _children = permission.get('children', None)
         _is_menu = permission.get('is_menu', True)
-        _is_action = permission.get('is_action', True)
+        _is_action = permission.get('is_action', False)
         icon = permission.get('icon', None)
         parent = permissionObj.find_or_store_model(
             session=session,
             where=('scope', _scope), item=SchemasFunctionPermissionStoreUpdate(
                 name=_name, scope=_scope, parent_id=parent_pk, is_menu=_is_menu, is_action=_is_action, icon=icon
             ), commit=True, refresh=False
         )
```

### Comparing `yao-0.0.1/yao/method.py` & `yao-0.0.2/yao/method.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,18 +226,18 @@
             else:
                 res = ob
                 break
         return res
     return None
 
 
-def get_file_content(path: str, mode="rb"):
+def get_file_content(path: str, mode="rb", **kwargs):
     """获取文件内容"""
     if os.path.isfile(path):
-        with open(path, mode) as f:
+        with open(path, mode, **kwargs) as f:
             return f.read()
     return bytes()
 
 
 def file_to_base64(path: str):
     """文件转base64"""
     import filetype
```

### Comparing `yao-0.0.1/yao/schema.py` & `yao-0.0.2/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.1/yao.egg-info/SOURCES.txt` & `yao-0.0.2/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

