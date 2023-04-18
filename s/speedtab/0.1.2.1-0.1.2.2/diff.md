# Comparing `tmp/speedtab-0.1.2.1.tar.gz` & `tmp/speedtab-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.2.1.tar", max compression
+gzip compressed data, was "speedtab-0.1.2.2.tar", max compression
```

## Comparing `speedtab-0.1.2.1.tar` & `speedtab-0.1.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      586 2022-09-07 08:00:21.277651 speedtab-0.1.2.1/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.2.1/speedtab/__init__.py
--rw-r--r--   0        0        0    31204 2022-08-23 18:18:55.168517 speedtab-0.1.2.1/speedtab/client.py
--rw-r--r--   0        0        0     4686 2022-08-23 18:18:55.159509 speedtab-0.1.2.1/speedtab/enums.py
--rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.2.1/speedtab/formats.py
--rw-r--r--   0        0        0      808 2022-09-07 08:00:24.334832 speedtab-0.1.2.1/setup.py
--rw-r--r--   0        0        0      797 2022-09-07 08:00:24.334832 speedtab-0.1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-04-18 15:36:53.978276 speedtab-0.1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.2.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    36004 2023-04-18 15:30:15.913324 speedtab-0.1.2.2/speedtab/client.py
+-rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.2.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.2.2/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-04-18 15:38:21.542499 speedtab-0.1.2.2/setup.py
+-rw-r--r--   0        0        0      808 2023-04-18 15:38:21.542499 speedtab-0.1.2.2/PKG-INFO
```

### Comparing `speedtab-0.1.2.1/pyproject.toml` & `speedtab-0.1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.2.1"
+version = "0.1.2.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 google-api-python-client = "^2.58.0"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.5.2"
-pandas = "^1.4.3"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `speedtab-0.1.2.1/speedtab/client.py` & `speedtab-0.1.2.2/speedtab/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from collections.abc import Iterable
 from datetime import datetime, date
 from enum import Enum
 from itertools import zip_longest
 from typing import Union
 
 import pandas as pd
+import numpy as np
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from speedtab.enums import MergeType, BorderStyle, HorizontalAlignment, VerticalAlignment, WrapStrategy, ShareRole, \
-    ChartType, StackedType, LegendPosition, AxisPosition
+    ChartType, StackedType, LegendPosition, AxisPosition, BooleanConditionTypes
 from speedtab.formats import Color, Border, Number, BaseNumberFormat
 
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/drive', 'https://www.googleapis.com/auth/drive.file']
 BORDER_SIDES = ('top', 'bottom', 'left', 'right', 'innerHorizontal', 'innerVertical')
 SHIFT_DIM = {
     'startRowIndex': 0,
     'startColumnIndex': 0,
@@ -29,15 +30,15 @@
     'ROWS': 'ROWS',
     'COLUMNS': 'COLUMNS',
     0: 'ROWS',
     1: 'COLUMNS'
 }
 
 
-def create_token(input_cred: str = 'creds.json', output_token: str = 'token.json'):
+def create_token(input_cred, output_token: str = 'token.json'):
     flow = InstalledAppFlow.from_client_secrets_file(input_cred, SCOPES)
     creds = flow.run_local_server(port=0)
     with open(output_token, 'w') as token:
         token.write(creds.to_json())
 
 
 def col_num_to_string(n, start_from_0=True):
@@ -94,39 +95,54 @@
     else:
         cells = input_range + (None,)*4
     return cells
 
 depth = lambda l: isinstance(l, list) and max(map(depth, l)) + 1
 
 
+class BooleanCondition:
+    def __init__(self, type: BooleanConditionTypes, value):
+        self.type = type.value
+        self.value = value
+
+    def boolean_condition(self):
+        return {
+            'booleanRule': {
+                'condition': {
+                    'type': self.type,
+                    'values': [
+                        {'userEnteredValue': self.value}
+                    ]}}}
+
+
 class Task:
     def __init__(self, task_type, position, sheetId, task, data_cell=None):
         self.task_type = task_type
         self.position = position
         self.sheetId = sheetId
         self.task = task
         self.data_cell = data_cell
 
 
 class SpreedSheet:
     def __init__(self, spreadsheet_id, token_path, credentials, connect):
         self.spreadsheet_id = spreadsheet_id
         self.token_path = token_path
         self.credentials = credentials
-        self.connect = connect
+        self.connect_v4 = connect
         self._get_metadata()
         self._task_queue = []
 
     def _regroup_tasks(self):
         groups = []
         for id in [x.get('sheetId') for x in self.sheets.values()]:
             current_id_tasks = [x for x in self._task_queue if x.sheetId == id]
             clear_ids = [0] + [i for i, x in enumerate(current_id_tasks) if x.task_type == 'clear']
             groups_ids = clear_ids[:1] + [clear_ids[i] for i in range(1, len(clear_ids))
-                              if clear_ids[i] - clear_ids[i - 1] > 1] + [len(current_id_tasks)]
+                                          if clear_ids[i] - clear_ids[i - 1] > 1] + [len(current_id_tasks)]
 
             merged_group = []
             shift = []
             for elem in [current_id_tasks[i:j] for i, j in [groups_ids[i:i + 2] for i in range(0, len(groups_ids) - 1, 1)]]:
                 if not any(d.task_type == 'data' for d in elem):
                     shift += elem
                 else:
@@ -150,16 +166,16 @@
                 elif task.task_type == 'clear' and 'appendDimension' in task.task.keys():
                     vals = task.task.get('appendDimension')
                     if vals.get('dimension') == 'ROWS':
                         curr_size[task.sheetId][0] += vals.get('length')
                     if vals.get('dimension') == 'COLUMNS':
                         curr_size[task.sheetId][1] += vals.get('length')
                 elif task.task_type == 'data':
-                    curr_size[task.sheetId] = [max(curr_size[task.sheetId][0], task.data_cell[0]),
-                                               max(curr_size[task.sheetId][1], task.data_cell[1])]
+                    curr_size[task.sheetId] = [max(curr_size[task.sheetId][0], task.data_cell[0] + 1),
+                                               max(curr_size[task.sheetId][1], task.data_cell[1] + 1)]
             for key, (rows, columns) in curr_size.items():
                 self._set_sheet_size(rows, columns, key, group)
 
         return [sorted(group, key=lambda x: (TYPE_ORDER[x.task_type], x.position)) for group in full_groups]
 
     def _set_sheet_size(self, rows: int, columns: int, sheet_id, group):
         group.append(Task('format', len(self._task_queue), sheet_id, {
@@ -167,19 +183,19 @@
                 'properties': {
                     'gridProperties': {
                         'rowCount': rows,
                         'columnCount': columns,
                     },
                     'sheetId': sheet_id,
                 },
-                'fields': 'gridProperties',
+                'fields': 'gridProperties.rowCount, gridProperties.columnCount',
             }}))
 
     def _get_metadata(self):
-        metadata = self.connect.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
+        metadata = self.connect_v4.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
         self.sheets = dict(
             [(prop.get('title'), {
                 'max_column': prop.get('gridProperties').get('columnCount'),
                 'max_row': prop.get('gridProperties').get('rowCount'),
                 'sheetId': prop.get('sheetId'),
                 'position': prop.get('index'),
             }) for prop in [sheet.get('properties') for sheet in metadata.get('sheets')]]
@@ -197,36 +213,38 @@
                 if task.task_type == 'data':
                     batch_update_data_list.append(task.task)
                 elif task.task_type == 'chart':
                     batch_update_chart_list.append(task.task)
                 else:
                     batch_update_list.append(task.task)
             if batch_update_list:
-                self.connect.spreadsheets().batchUpdate(**{
+                print('Update tasks:', batch_update_list)
+                self.connect_v4.spreadsheets().batchUpdate(**{
                     'spreadsheetId': self.spreadsheet_id,
                     'body': {
                         'requests': batch_update_list
                     }}).execute()
 
             if batch_update_data_list:
-                self.connect.spreadsheets().values().batchUpdate(**{
+                print('Update tasks:', batch_update_data_list)
+                self.connect_v4.spreadsheets().values().batchUpdate(**{
                     'spreadsheetId': self.spreadsheet_id,
                     'body': {
                         'valueInputOption': 'RAW',
                         'data': batch_update_data_list,
                     }}).execute()
         if batch_update_chart_list:
-            self.connect.spreadsheets().batchUpdate(**{
+            self.connect_v4.spreadsheets().batchUpdate(**{
                 'spreadsheetId': self.spreadsheet_id,
                 'body': {
                     'requests': batch_update_chart_list
                 }}).execute()
 
     def add_sheets(self, sheets):
-        self.connect.spreadsheets().batchUpdate(**{
+        self.connect_v4.spreadsheets().batchUpdate(**{
             'spreadsheetId': self.spreadsheet_id,
             'body': {
                 'requests': [{
                     'addSheet': {
                         'properties': {
                             'title': title,
                             'gridProperties': {
@@ -245,159 +263,25 @@
         return self
 
     def sheet(self, sheet_name):
         return Sheet(sheet_name, self.sheets.get(sheet_name).get('sheetId'), self._task_queue, self.sheets, self)
 
 
 class Range:
-    def __init__(self, sheet_id, _task_queue, work_zone, start_data_index, start_data_cell, base, data_cell):
+    def __init__(self, sheet_id, _task_queue, work_zone, start_data_cell, base, data_cell):
         self.sheet_id = sheet_id
         self._task_queue = _task_queue
         self.work_zone = work_zone
-        self.start_data_index = start_data_index
         self.start_data_cell = start_data_cell
         self.base = base
         self.data_cell = data_cell
 
     def _increment_task(self):
         return len(self._task_queue)
 
-    def merge_cells(self, merge_type: MergeType = MergeType.MERGE_ALL):
-        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'mergeCells': {
-                    'mergeType': merge_type.value,
-                    'range': self.work_zone
-                }}))
-        return self
-
-    def delete_axis(self, axis: Union[str, int] = 1):
-        axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
-        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
-                'deleteDimension': {
-                    'range': {
-                        'sheetId': self.sheet_id,
-                        'dimension': axis,
-                        'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
-                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
-                    }}}))
-
-        return self
-
-    def write_range(self, values, axis: Union[str, int] = 0):
-        values = list(values) if not isinstance(values, list) else values
-        while depth(values) < 2:
-            values = [values]
-        values = apply(values, datetime_to_xls)
-        self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
-                'range': self.start_data_cell,
-                'values': values,
-                'majorDimension': DIMENSION.get(axis.upper() if isinstance(axis, str) else axis),
-              }, self.start_data_index))
-
-        return self
-
-    def write_dataframe(self, df: pd.DataFrame, header=True, index=True):
-        df = df.applymap(datetime_to_xls).where(pd.notnull(df), None)
-        df = df.reset_index() if index else df
-
-        if header:
-            if isinstance(df.columns, pd.MultiIndex):
-                values = [[str(elem) for elem in level] for level in list(zip(*df.columns.to_list()))] + df.values.tolist()
-            else:
-                values = [[str(elem) for elem in df.columns.to_list()]] + df.values.tolist()
-        else:
-            values = df.values.tolist()
-
-        self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
-                'range': self.start_data_cell,
-                'values': values,
-                'majorDimension': 'ROWS',
-        }, self.start_data_index))
-        return self
-
-    def read_range(self):
-        return (self.base._connect().spreadsheets().values()
-                .get(spreadsheetId=self.sheet_id,
-                     range=self.data_cell,
-                     valueRenderOption='UNFORMATTED_VALUE').execute()
-                .get('values', []))
-
-    def read_dataframe(self):
-        rows = self.read_range()
-        return pd.DataFrame(data=rows[1:], columns=rows[0])
-
-    def clear(self, values=True, formats=True):
-        field = None
-        if values and formats:
-            field = '*'
-        elif formats:
-            field = 'userEnteredFormat'
-        elif values:
-            field = 'userEnteredValue'
-
-        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
-                'updateCells': {
-                    'range': self.work_zone,
-                    'fields': field,
-                }}))
-
-        return self
-
-    def set_sheet_size(self, rows: int, columns: int):
-        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
-                'updateSheetProperties': {
-                    'properties': {
-                        'gridProperties': {
-                            'rowCount': rows,
-                            'columnCount': columns,
-                        },
-                        'sheetId': self.sheet_id,
-                    },
-                    'fields': 'gridProperties',
-                }}))
-
-        return self
-
-    def extend_sheet(self, rows: int = None, cols: int = None):
-        if cols:
-            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
-                'appendDimension': {
-                    'sheetId': self.sheet_id,
-                    'dimension': 'COLUMNS',
-                    'length': cols,
-                }}))
-        if rows:
-            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
-                'appendDimension': {
-                    'sheetId': self.sheet_id,
-                    'dimension': 'ROWS',
-                    'length': rows,
-                }}))
-
-        return self
-
-    def unmerge_cells(self):
-        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'unmergeCells': {
-                    'range': self.work_zone,
-                }}))
-        return self
-
-    def auto_size(self, axis: Union[str, int] = 1):
-        axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
-        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'autoResizeDimensions': {
-                    'dimensions': {
-                        'sheetId': self.sheet_id,
-                        'dimension': axis,
-                        'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
-                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
-                    }}}))
-        return self
-
     def add_chart(self, columns,
                   target_axis: AxisPosition = AxisPosition.LEFT_AXIS,
                   index_column: int = 0,
                   chart_type: ChartType = ChartType.LINE,
                   stacked_type: StackedType = StackedType.NONE,
                   title: str = None,
                   legend_position: LegendPosition = LegendPosition.BOTTOM_LEGEND,
@@ -501,170 +385,391 @@
                             'widthPixels': 800 * x_scale,
                             'heightPixels': 400 * y_scale,
                         }
                     }}}}))
 
         return self
 
-    def set_size(self, size: int = None, axis: Union[str, int] = 1):
+    def auto_size(self, axis: Union[str, int] = 1):
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'updateDimensionProperties': {
+                'autoResizeDimensions': {
+                    'dimensions': {
+                        'sheetId': self.sheet_id,
+                        'dimension': axis,
+                        'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
+                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
+                    }}}))
+        return self
+
+    def clear(self, values=True, formats=True):
+        field = None
+        if values and formats:
+            field = '*'
+        elif formats:
+            field = 'userEnteredFormat'
+        elif values:
+            field = 'userEnteredValue'
+
+        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+                'updateCells': {
+                    'range': self.work_zone,
+                    'fields': field,
+                }}))
+
+        return self
+
+    def delete_axis(self, axis: Union[str, int] = 1):
+        axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
+        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+                'deleteDimension': {
                     'range': {
                         'sheetId': self.sheet_id,
                         'dimension': axis,
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
-                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex'),
-                    },
-                    'properties': {
-                        'pixelSize': size,
+                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
+                    }}}))
+
+        return self
+
+    def extend_sheet(self, rows: int = None, cols: int = None):
+        if cols:
+            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+                'appendDimension': {
+                    'sheetId': self.sheet_id,
+                    'dimension': 'COLUMNS',
+                    'length': cols,
+                }}))
+        if rows:
+            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+                'appendDimension': {
+                    'sheetId': self.sheet_id,
+                    'dimension': 'ROWS',
+                    'length': rows,
+                }}))
+
+        return self
+
+    def hide_grid_lines(self, hide_grid=True):
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+            'updateSheetProperties': {
+                'properties': {
+                    'sheetId': self.sheet_id,
+                    'gridProperties': {
+                        'hideGridlines': hide_grid,
                     },
-                    'fields': 'pixelSize',
+                },
+                'fields': 'gridProperties.hideGridlines',
+            }
+        }))
+        return self
+
+    def merge_cells(self, merge_type: MergeType = MergeType.MERGE_ALL):
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'mergeCells': {
+                    'mergeType': merge_type.value,
+                    'range': self.work_zone
+                }}))
+        return self
+
+    def read_dataframe(self):
+        rows = self.read_range()
+        return pd.DataFrame(data=rows[1:], columns=rows[0])
+
+    def read_range(self):
+        return (self.base._connect().spreadsheets().values()
+                .get(spreadsheetId=self.sheet_id,
+                     range=self.data_cell,
+                     valueRenderOption='UNFORMATTED_VALUE').execute()
+                .get('values', []))
+
+    def set_background_color(self, color: Color = Color((255, 255, 255))):
+        color = color.value if isinstance(color, Enum) else color
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'repeatCell': {
+                    'range': self.work_zone,
+                    'cell': {
+                        'userEnteredFormat': {
+                            'backgroundColor': color.color
+                        }},
+                    'fields': 'userEnteredFormat(backgroundColor)',
+                }}))
+        return self
+
+    def set_borders(self, border_style: BorderStyle = BorderStyle.SOLID,
+                    border_width: int = 1,
+                    color: Color = Color((0, 0, 0)),
+                    border_sides: list = BORDER_SIDES,
+                    ):
+        color = color.value if isinstance(color, Enum) else color
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'updateBorders': {
+                    'range': self.work_zone,
+                    **dict((x, Border(border_style, border_width, color).__dict__) for x in border_sides),
                 }}))
         return self
 
+    def set_freeze_cell(self):
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+            'updateSheetProperties': {
+                'properties': {
+                    'gridProperties': {
+                        'frozenRowCount': self.work_zone.get('startRowIndex'),
+                        'frozenColumnCount': self.work_zone.get('startColumnIndex')},
+                    'sheetId': self.sheet_id
+                },
+                'fields': 'gridProperties.frozenRowCount, gridProperties.frozenColumnCount'
+            }
+        }))
+        return self
+
     def set_num_format(self, default_format: BaseNumberFormat = Number):
         default_format = default_format.value if isinstance(default_format, Enum) else default_format
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     **default_format.__dict__,
                 }}))
         return self
 
+    def set_sheet_size(self, rows: int, columns: int):
+        self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+                'updateSheetProperties': {
+                    'properties': {
+                        'gridProperties': {
+                            'rowCount': rows,
+                            'columnCount': columns,
+                        },
+                        'sheetId': self.sheet_id,
+                    },
+                    'fields': 'gridProperties.rowCount, gridProperties.columnCount',
+                }}))
+
+        return self
+
+    def set_size(self, size: int = None, axis: Union[str, int] = 1):
+        axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'updateDimensionProperties': {
+                    'range': {
+                        'sheetId': self.sheet_id,
+                        'dimension': axis,
+                        'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
+                        'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex'),
+                    },
+                    'properties': {
+                        'pixelSize': size,
+                    },
+                    'fields': 'pixelSize',
+                }}))
+        return self
+
     def set_text_format(self, horizontal_alignment: HorizontalAlignment = None,
                         vertical_alignment: VerticalAlignment = None,
                         wrap_strategy: WrapStrategy = None,
                         font_size: int = None,
                         bold: bool = None,
                         italic: bool = None,
                         strikethrough: bool = None,
                         underline: bool = None,
                         font_family: str = None,
                         text_color: Color = None):
-        """
-        Function to set cell text format for Google Sheet
-        :param horizontal_alignment: 'LEFT', 'CENTER', 'RIGHT'
-        :param vertical_alignment: 'TOP', 'MIDDLE', 'BOTTOM'
-        :param wrap_strategy: 'OVERFLOW_CELL', 'LEGACY_WRAP', 'CLIP', 'WRAP'
-        :param font_size: font size
-        :param bold: True or False
-        :param italic: True or False
-        :param strikethrough: True or False
-        :param underline: True or False
-        :param font_family: font family
-        :param text_color: foreground color of the text in rgb format
-        """
+
         text_color = text_color.value if isinstance(text_color, Enum) else text_color
         list_of_inputs = ', '.join(
             [f'textFormat.{s}' for s, x in
              zip(('fontFamily', 'fontSize', 'bold', 'italic', 'strikethrough', 'underline', 'foregroundColor'),
                  (font_family, font_size, bold, italic, strikethrough, underline, text_color)) if x is not None]
             + [s for s, x in zip(('horizontalAlignment', 'verticalAlignment', 'wrapStrategy'),
                                  (horizontal_alignment, vertical_alignment, wrap_strategy)) if x is not None])
 
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     'cell': {
                         'userEnteredFormat': {
-                            'horizontalAlignment': horizontal_alignment.value if horizontal_alignment is not None else None,
-                            'verticalAlignment': vertical_alignment.value if vertical_alignment is not None else None,
-                            'wrapStrategy': wrap_strategy.value if wrap_strategy is not None else None,
+                            'horizontalAlignment': horizontal_alignment.value if horizontal_alignment is not None or False else None,
+                            'verticalAlignment': vertical_alignment.value if vertical_alignment is not None or False else None,
+                            'wrapStrategy': wrap_strategy.value if wrap_strategy is not None or False else None,
                             'textFormat': {
-                                'foregroundColor': text_color.color if text_color is not None else None,
-                                'fontFamily': font_family,
-                                'fontSize': font_size,
-                                'bold': bold,
-                                'italic': italic,
-                                'strikethrough': strikethrough,
-                                'underline': underline,
+                                'foregroundColor': text_color.color if text_color is not None or False else None,
+                                'fontFamily': font_family if font_family is not None or False else None,
+                                'fontSize': font_size if font_size is not None or False else None,
+                                'bold': bold if bold is not None or False else None,
+                                'italic': italic if italic is not None or False else None,
+                                'strikethrough': strikethrough if strikethrough is not None or False else None,
+                                'underline': underline if underline is not None or False else None,
                             }}},
                     'fields': f'userEnteredFormat({list_of_inputs})',
                 }}))
         return self
 
-    def set_borders(self, border_style: BorderStyle = BorderStyle.SOLID,
-                    border_width: int = 1,
-                    color: Color = Color((0, 0, 0)),
-                    border_sides: list = BORDER_SIDES,
-                    ):
-        color = color.value if isinstance(color, Enum) else color
+    def unmerge_cells(self):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'updateBorders': {
+                'unmergeCells': {
                     'range': self.work_zone,
-                    **dict((x, Border(border_style, border_width, color).__dict__) for x in border_sides),
                 }}))
         return self
 
-    def set_background_color(self, color: Color = Color((255, 255, 255))):
-        color = color.value if isinstance(color, Enum) else color
+    def write_dataframe(self, df: pd.DataFrame, header=True, index=True):
+        df = df.copy()
+
+        for column, column_type in zip(df.dtypes.index, df.dtypes.values):
+            if isinstance(column_type, pd.CategoricalDtype):
+                df[column] = df[column].cat.add_categories('').fillna('').astype(str)
+            elif np.dtype('timedelta64[ns]') == column_type:
+                df[column] = df[column].astype(str)
+
+        if index:
+            if isinstance(df.index, pd.CategoricalIndex) or any(isinstance(x, pd.Interval) for x in df.index.values):
+                df.index = df.index.astype(str)
+            try:
+                df = df.reset_index(col_level=-1)
+            except:
+                df = pd.merge(df.index.to_frame(index=False), df.reset_index(drop=True), left_index=True, right_index=True)
+
+        df = df.applymap(datetime_to_xls).replace([np.inf, -np.inf], None).where(pd.notnull(df), None)
+
+        if header:
+            if isinstance(df.columns, pd.MultiIndex):
+                values = [[str(elem) for elem in level] for level in list(zip(*df.columns.to_list()))] + df.values.tolist()
+            else:
+                values = [[str(elem) for elem in df.columns.to_list()]] + df.values.tolist()
+        else:
+            values = df.values.tolist()
+
+        self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
+                'range': self.start_data_cell,
+                'values': values,
+                'majorDimension': 'ROWS',
+        }, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+        return self
+
+    def write_formula(self, value):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
-                'repeatCell': {
-                    'range': self.work_zone,
-                    'cell': {
-                        'userEnteredFormat': {
-                            'backgroundColor': color.color
-                        }},
-                    'fields': 'userEnteredFormat(backgroundColor)',
-                }}))
+            'repeatCell': {
+                'range': self.work_zone,
+                'cell': {
+                    'userEnteredValue': {
+                        'formulaValue': value
+                    }
+                },
+                'fields': 'userEnteredValue'
+            }}, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+
+        return self
+
+    def write_range(self, values, axis: Union[str, int] = 0):
+        values = list(values) if not isinstance(values, list) else values
+        while depth(values) < 2:
+            values = [values]
+        values = apply(values, datetime_to_xls)
+        self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
+                'range': self.start_data_cell,
+                'values': values,
+                'majorDimension': DIMENSION.get(axis.upper() if isinstance(axis, str) else axis),
+              }, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+
         return self
 
 
 class Sheet(Range):
     def __init__(self, sheet_name, sheet_id, task_query, sheets, base, cells=(0, 0, None, None)):
         self.base = base
         self.sheet_name = sheet_name
         self.sheet_id = sheet_id
         self._task_queue = task_query
         self.sheets = sheets
         cells = parse_range(cells)
 
         self.start_data_cell = f'{sheet_name}!{col_num_to_string(cells[1])}{num_to_string(cells[0])}'
         self.data_cell = self.start_data_cell + f':{col_num_to_string(cells[3])}{num_to_string(cells[2])}'
-        self.start_data_index = cells[:2]
         self.work_zone = dict([(key, val + SHIFT_DIM.get(key) if val is not None else val)
                                for key, val in zip(SHIFT_DIM.keys(), cells)]
                               + [('sheetId', self.sheet_id)])
 
-        super().__init__(self.sheet_id, self._task_queue, self.work_zone, self.start_data_index,
-                         self.start_data_cell, self.base, self.data_cell)
+        super().__init__(self.sheet_id, self._task_queue, self.work_zone, self.start_data_cell, self.base,
+                         self.data_cell)
 
     def sheet(self, sheet_name):
         return Sheet(sheet_name, self.sheet_id, self._task_queue, self.sheets, self.base)
 
     def cell_range(self, input_range):
         return Sheet(self.sheet_name, self.sheet_id, self._task_queue, self.sheets, self.base, input_range)
 
 
 class Client:
     def __init__(self, token_path='token.json'):
         self.token_path = token_path
         self.credentials = Credentials.from_authorized_user_file(self.token_path, SCOPES)
         self.list_of_spreadsheets = []
-        self.connect = self._connect()
+        self.connect_v4 = self._connect_v4()
         self.connect_v3 = self._connect_v3()
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.exec()
 
     def create_spreadsheet(self, title, sheets: list = ['Sheet1']):
-        ss = SpreedSheet(build('sheets', 'v4', credentials=self.credentials).spreadsheets()
+        ss = SpreedSheet(self._connect_v4().spreadsheets()
                          .create(fields='spreadsheetId',
                                  body={
                                      'properties': {'title': title},
                                      'sheets': [{'properties': {'title': sheet_name}} for sheet_name in sheets]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
                          credentials=self.credentials, connect=self.connect)
         self.list_of_spreadsheets.append(ss)
         return ss
 
+    def create_folder(self, folderName, parentID=None):
+        return self._connect_v3().files().create(body={
+            'name': folderName,
+            'mimeType': "application/vnd.google-apps.folder",
+            'parents': [parentID] if parentID else None,
+        }, supportsAllDrives=True).execute()['id']
+
+    def rename_folder(self, fileId, name):
+        self._connect_v3().files().update(body={
+            'name': name,
+        }, fileId=fileId, supportsAllDrives=True).execute()
+
+    def search_files(self, folder_id=None, trashed=False):
+        files = []
+        page_token = None
+        while True:
+            response = self._connect_v3().files().list(q=('trashed = true' if trashed else 'trashed = false') + (
+                f' and "{folder_id}" in parents' if folder_id else ''),
+                                                       spaces='drive',
+                                                       fields='nextPageToken, files(id, name, mimeType)',
+                                                       includeItemsFromAllDrives=True,
+                                                       supportsAllDrives=True,
+                                                       pageToken=page_token,
+                                                       ).execute()
+
+            files.extend([{'id': file.get('id'), 'name': file.get('name'), 'file_type': file.get('mimeType').split('.')[-1]} for file in response.get('files', [])])
+            page_token = response.get('nextPageToken', None)
+
+            if page_token is None:
+                break
+
+        return files
+
+    def search_folder(self, folder_name, current_folder, mkdir=False):
+        folders = [file for file in self.search_files(current_folder) if
+                   file.get('file_type') == 'folder' and file.get('name') == folder_name]
+
+        if folders:
+            return folders[0].get('id')
+        elif mkdir:
+            return self.create_folder(folder_name, current_folder)
+        else:
+            return None
+
     def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id):
         previous_parents = ','.join(self.connect_v3.files().get(fileId=ss.spreadsheet_id, fields='parents').execute().get('parents'))
         self.connect_v3.files().update(fileId=ss.spreadsheet_id, addParents=real_folder_id,
                                        removeParents=previous_parents, fields='id, parents').execute()
 
     def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain, role: ShareRole):
         self.connect_v3.permissions().create(**{
@@ -691,15 +796,15 @@
 
     def get_spreadsheet(self, spreadsheet_id):
         ss = SpreedSheet(spreadsheet_id=spreadsheet_id, token_path=self.token_path,
                          credentials=self.credentials, connect=self.connect)
         self.list_of_spreadsheets.append(ss)
         return ss
 
-    def _connect(self):
+    def _connect_v4(self):
         return build('sheets', 'v4', credentials=self.credentials)
 
     def _connect_v3(self):
         return build('drive', 'v3', credentials=self.credentials)
 
     def exec(self):
         for st in self.list_of_spreadsheets:
```

### Comparing `speedtab-0.1.2.1/speedtab/formats.py` & `speedtab-0.1.2.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.1/setup.py` & `speedtab-0.1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
- 'google-auth-oauthlib>=0.5.2,<0.6.0',
- 'pandas>=1.4.3,<2.0.0']
+ 'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.2.1',
+    'version': '0.1.2.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

