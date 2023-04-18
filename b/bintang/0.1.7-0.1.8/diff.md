# Comparing `tmp/bintang-0.1.7-py3-none-any.whl.zip` & `tmp/bintang-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22856 bytes, number of entries: 14
+Zip file size: 23071 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       25 b- defN 22-Sep-15 02:00 bintang/__init__.py
 -rw-rw-rw-  2.0 fat     6439 b- defN 22-Jul-05 11:25 bintang/besqlite.py
 -rw-rw-rw-  2.0 fat     1526 b- defN 23-Apr-14 06:25 bintang/cell.py
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Mar-29 02:17 bintang/column.py
 -rw-rw-rw-  2.0 fat    24155 b- defN 23-Apr-17 08:28 bintang/core.py
 -rw-rw-rw-  2.0 fat     5027 b- defN 23-Apr-14 06:27 bintang/iterdict.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-Apr-17 08:59 bintang/log.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 23-Apr-12 12:29 bintang/row.py
--rw-rw-rw-  2.0 fat    53510 b- defN 23-Apr-17 09:08 bintang/table.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-17 09:20 bintang-0.1.7.dist-info/RECORD
-14 files, 95303 bytes uncompressed, 21156 bytes compressed:  77.8%
+-rw-rw-rw-  2.0 fat    54492 b- defN 23-Apr-18 13:55 bintang/table.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/RECORD
+14 files, 96285 bytes uncompressed, 21371 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: bintang/row.py
 Comment: 
 
 Filename: bintang/table.py
 Comment: 
 
-Filename: bintang-0.1.7.dist-info/LICENSE
+Filename: bintang-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: bintang-0.1.7.dist-info/METADATA
+Filename: bintang-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: bintang-0.1.7.dist-info/WHEEL
+Filename: bintang-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: bintang-0.1.7.dist-info/top_level.txt
+Filename: bintang-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: bintang-0.1.7.dist-info/RECORD
+Filename: bintang-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bintang/table.py

```diff
@@ -3,15 +3,17 @@
 from bintang.cell import Cell
 from bintang.row import Row
 import json
 import sqlite3
 import uuid
 import re
 import types
+import sys
 import unicodedata
+from thefuzz import process as thefuzzprocess
 from bintang.log import log
 # import logging
 
 # log = logging.getLogger(__name__)
 # FORMAT = "[%(filename)s:%(lineno)s - %(funcName)10s() ] %(message)s"
 # logging.basicConfig(format=FORMAT)
 # log.setLevel(logging.DEBUG)
@@ -305,14 +307,15 @@
 
     def get_columnid(self,column):
         for id, cobj in self.__columns.items():
             # match the column case insensitive
             if cobj.get_name_uppercased() == column.upper():
                 return id
         return None
+        
 
     
     def get_columnids(self,columns=None):
         columnids = []
         if columns is None: # assume user want all available column ids
             return [id for id in self.__columns.keys()]
         for column in columns:
@@ -380,15 +383,24 @@
         """return columns from those stored in table.columns"""
         res = []
         for column in columns:
             if column.lower() in self._get_columnnames_lced().keys():
                 res.append(self._get_columnnames_lced().get(column.lower()))
             else:
                 raise ColumnNotFoundError(self.name, column)
-        return res                
+        return res
+
+
+    def check_column(self, column):
+        """check if column exits in table.columns"""
+        if column.lower() not in self._get_columnnames_lced().keys():
+            extracted = thefuzzprocess.extract(column, self.get_columns(), limit=2)
+            fuzzies = [x[0] for x in extracted if x[1]>85]
+            raise ValueError ('could not find column {}. Did you mean {}?'.format(column,' or '.join(fuzzies)))
+            
 
 
     def VOID_validate_columns(self,columns):
         res = []
         for column in columns:
             columnid = self.get_columnid(column)
             if columnid is not None:
@@ -718,15 +730,23 @@
         return self._gen_row_aslist(self.__rows[idx],columnids)
 
 
     def _gen_row_aslist(self, row, columnids):
         return row.get_values(columnids)
 
        
-    def iterrows(self, columns=None, row_type='dict', where=None, rowid=False):
+    def iterrows(self, 
+                 columns: list=None, 
+                 row_type: str='dict', 
+                 where=None, 
+                 rowid: bool=False):
+        # validate user's args
+        if columns is not None:
+            for column in columns:
+                self.check_column(column)
         if columns is None:
                 columns = self.get_columns() # assign all available column names
         if row_type == 'dict': 
             if self.__be is None:
                 if where is not None:
                     for idx, row in self.__rows.items():
                         if where(self._gen_row_asdict(row, columns, rowid)):
@@ -996,16 +1016,15 @@
                         tobj.insert(columns_,values)
                 except:
                     pass        
         return tobj
 
 
     def innerjoin(self
-                #,ltable: str #, lkeys
-                ,rtable: str #, rkeys
+                ,rtable # either string or Table object
                 ,on: list[tuple] # list of lkey & r key tuple
                 ,into: str
                 ,out_lcolumns: list=None
                 ,out_rcolumns: list=None
                 ,rowid=False):
         
         rtable_obj = None
@@ -1124,56 +1143,66 @@
     #         used_type = type(row[column]).__name__
     #         if used_type not in used_types:
     #             used_types.append(used_type)
     #     return used_types    
 
 
     #def blookup(self, rtable, keys, lkkeys, out_rcolumns, ret_ascolumns = None):
-    def blookup(self, rtable, on, out_rcolumns):
+    def blookup(self, 
+                rtable, 
+                on: str, 
+                out_rcolumns: list[str] | list[tuple]):
         #rtable = self.bing[rtable] 
+        rtable_obj = None
+        if isinstance(rtable,Table):
+            rtable_obj = rtable
+            rtable = rtable.name
+        else:
+            rtable_obj = self.bing[rtable]
         
         # validate input eg. column etc
         lkeys = [x[0] for x in on] # generate lkeys from on (1st sequence)
         rkeys = [x[1] for x in on] # generate rkeys from on (2nd sequence)
         lkeys = self.validate_columns(lkeys)
-        rkeys = self.bing[rtable].validate_columns(rkeys)
+        rkeys = rtable_obj.validate_columns(rkeys)
         lcolumn_prematch = self.get_columns() # will use this list when matching occurs below
         # validate out_rcolumns once:
         # otherwise will make lots of call later
         valid_out_rcolumns = []
         for item in out_rcolumns:
             if isinstance(item,str):
-                item = self.bing[rtable].validate_column(item)
+                item = rtable_obj.validate_column(item)
                 valid_out_rcolumns.append(item)
             if isinstance(item, tuple):
-                valid_column  = self.bing[rtable].validate_column(item[0])
+                valid_column  = rtable_obj.validate_column(item[0])
                 item_ = tuple([valid_column,item[1]])
                 valid_out_rcolumns.append(item_)
         numof_keys = len(on)
         for lidx, lrow in self.iterrows(lkeys, rowid=True):
-            for ridx, rrow in self.bing[rtable].iterrows():
+            for ridx, rrow in rtable_obj.iterrows():
                 matches = 0
                 for i in range(numof_keys):
                     # if lrow[lkeys[i]] == rrow[rkeys[i]]:
                     if _match_caseless_unicode(lrow[lkeys[i]], rrow[rkeys[i]]):
                         matches += 1 # increment
                 if matches == numof_keys:
                     # update this table lrow for each out_rcolumns
                     for item in valid_out_rcolumns:
                         if isinstance(item, str): # if item is a column
-                            value = self.bing[rtable][ridx][item]
+                            value = rtable_obj[ridx][item]
                             if item in lcolumn_prematch:
                                 print('item',item,'in',self.name)
-                                self.update_row(lidx, self.bing[rtable].name + '_' + item, value)
+                                self.update_row(lidx, rtable_obj.name + '_' + item, value)
                             else:
                                 self.update_row(lidx, item, value)
-                        if isinstance(item, tuple): # if a tuple
-                            value = self.bing[rtable][ridx][item[0]]
+                        if isinstance(item, tuple): # if a tuple (0=column to return from rtable, 1=as_column)
+                            value = rtable_obj[ridx][item[0]]
                             self.update_row(lidx, item[1], value)                   
 
+
     def groupbycount(self, column):
         res_dict = {}
         for idx, row in self.iterrows(column):
             value = next(iter(row.values()))
             if value not in res_dict:
                 res_dict[value] = 1
             else:
@@ -1258,14 +1287,15 @@
             res_list = []
             for idx, row in self.iterrows([column]):
                 res_list.append(next(iter(row.values())))
             return res_list    
         else:
             raise ValueError('column must be a single column string!')
 
+
 class Table_Path(Table):
     def __init__(self, name):
         super().__init__(name)
         self.path = name
         self.children = []
```

## Comparing `bintang-0.1.7.dist-info/LICENSE` & `bintang-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bintang-0.1.7.dist-info/RECORD` & `bintang-0.1.8.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 bintang/besqlite.py,sha256=4vfwMAheTgqudMuCH3wlwwWyGJY5aVDd_tmTCiStcJg,6439
 bintang/cell.py,sha256=JW-k_CgYu4nHX3Qk1nTcBP6fkjlsSXMgOuGRz5Dwcs4,1526
 bintang/column.py,sha256=zTMxofr4FXGR95Zcru9G2DlR35e8I3IVifEzOissONM,566
 bintang/core.py,sha256=6rupSkjfpEGcJny5SvdFPg-R5JRgF4L7FxnoKp49FU4,24155
 bintang/iterdict.py,sha256=lTxhrivwbCWhSQNN_TrPWaCg2QyeKa9vqf0X5j3vv2M,5027
 bintang/log.py,sha256=N6LImpolwYOJn4zW-nEpX6o63gInJKSzsw2NKM9V1sE,186
 bintang/row.py,sha256=I63-FY9p-lxmaeOOutKQbF9-jOPC3fTW-6frTqmzBOc,1385
-bintang/table.py,sha256=ijaGmD1S7JOisq_Rqg-NNG_0dDcBJYuXHG7ITenF9gs,53510
-bintang-0.1.7.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
-bintang-0.1.7.dist-info/METADATA,sha256=g4GFwu1N-2AJh_6eTCCOSfEeKwLGZvPHs7Rn7niXP5M,249
-bintang-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bintang-0.1.7.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
-bintang-0.1.7.dist-info/RECORD,,
+bintang/table.py,sha256=LEw0csB_23VOa7CPuWDlINwC7FiASF3W2cJZtDQSC1k,54492
+bintang-0.1.8.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
+bintang-0.1.8.dist-info/METADATA,sha256=PMIaoNjASUMd3I1-YoQ5eLO2De0G5fs3IfWALLXXLNo,249
+bintang-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bintang-0.1.8.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
+bintang-0.1.8.dist-info/RECORD,,
```

