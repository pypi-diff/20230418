# Comparing `tmp/n0struct-0.2.90.tar.gz` & `tmp/n0struct-0.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.90.tar", last modified: Sun Apr  2 13:23:08 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.91.tar", last modified: Tue Apr 18 04:25:19 2023, max compression
```

## Comparing `n0struct-0.2.90.tar` & `n0struct-0.2.91.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 13:23:08.778880 n0struct-0.2.90/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.90/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-04-02 13:23:08.779853 n0struct-0.2.90/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.90/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 13:23:08.753917 n0struct-0.2.90/n0struct/
--rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.90/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.90/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.90/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.90/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     2606 2023-04-02 07:38:19.000000 n0struct-0.2.90/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.90/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.90/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15997 2023-04-02 07:33:41.000000 n0struct-0.2.90/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4027 2023-04-02 07:07:41.000000 n0struct-0.2.90/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20923 2023-04-02 13:07:43.000000 n0struct-0.2.90/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.90/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    11962 2023-04-02 12:56:29.000000 n0struct-0.2.90/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17432 2023-04-02 07:23:42.000000 n0struct-0.2.90/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7507 2023-02-26 18:25:37.000000 n0struct-0.2.90/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    77681 2023-03-28 07:39:22.000000 n0struct-0.2.90/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.90/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3863 2023-02-26 20:17:13.000000 n0struct-0.2.90/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.90/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.90/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6670 2023-02-26 19:26:05.000000 n0struct-0.2.90/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4123 2023-03-28 07:56:46.000000 n0struct-0.2.90/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:23:08.778880 n0struct-0.2.90/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.90/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.90/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.90/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.90/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.90/n0struct/test/test_n0struct3.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:23:08.772867 n0struct-0.2.90/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-02 13:23:08.000000 n0struct-0.2.90/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 13:23:08.780856 n0struct-0.2.90/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.90/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.087728 n0struct-0.2.91/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.91/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-04-18 04:25:19.087728 n0struct-0.2.91/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.91/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 04:25:18.978374 n0struct-0.2.91/n0struct/
+-rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.91/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.91/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.91/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.91/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.91/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.91/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.91/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    16003 2023-04-17 11:25:17.000000 n0struct-0.2.91/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4027 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20923 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.91/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    11638 2023-04-18 04:13:47.000000 n0struct-0.2.91/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17432 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    77681 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.91/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3863 2023-02-26 20:17:13.000000 n0struct-0.2.91/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.91/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.91/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6670 2023-02-26 19:26:05.000000 n0struct-0.2.91/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4123 2023-03-28 07:56:46.000000 n0struct-0.2.91/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.087728 n0struct-0.2.91/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.91/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.91/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.91/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.91/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.91/n0struct/test/test_n0struct3.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.072142 n0struct-0.2.91/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-04-18 04:25:18.000000 n0struct-0.2.91/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 04:25:19.103386 n0struct-0.2.91/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.91/setup.py
```

### Comparing `n0struct-0.2.90/LICENSE` & `n0struct-0.2.91/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/PKG-INFO` & `n0struct-0.2.91/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.90
+Version: 0.2.91
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.90/README.md` & `n0struct-0.2.91/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/__init__.py` & `n0struct-0.2.91/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_arrays.py` & `n0struct-0.2.91/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.91/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_date.py` & `n0struct-0.2.91/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_files.py` & `n0struct-0.2.91/n0struct/n0struct_files.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,31 +32,36 @@
                 line = in_filehandler.readline()
                 if not line:
                     break
                 yield line.rstrip(EOL)
 # ******************************************************************************
 def save_file(
                 file_path: str,
-                lines: typing.Union[tuple, list, dict, str],
+                lines: typing.Union[tuple, list, dict, str, bytes, bytearray],
                 mode: str = 't',
-                encoding: str = 'utf-8',
+                encoding: str = "utf-8",
                 EOL: str = '\n',
                 equal_tag: str = "=",
 ):
     Path(file_path).parent.mkdir(parents=True, exist_ok=True)
 
     if isinstance(lines, (list, tuple)):
         output_buffer = EOL.join(lines)
     if isinstance(lines, dict):
         output_buffer = EOL.join([key+equal_tag+lines[key] for key in lines])
     elif isinstance(lines, str):
         output_buffer = lines
+    elif isinstance(lines, (bytes, bytearray)):
+        output_buffer = lines
+        mode = 'b' + ('+' if '+' in mode else '')
     else:
         output_buffer = str(lines)
 
     if 'b' in mode:
-        output_buffer = output_buffer.encode(encoding)
+        if isinstance(output_buffer, str):
+            output_buffer = output_buffer.encode(encoding)
+        encoding = None
 
-    with open(file_path, 'w'+mode) as out_filehandler:
+    with open(file_path, 'w'+mode, encoding=encoding) as out_filehandler:
         out_filehandler.write(output_buffer)
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.90/n0struct/n0struct_files_csv.py` & `n0struct-0.2.91/n0struct/n0struct_files_csv.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.91/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_findall.py` & `n0struct-0.2.91/n0struct/n0struct_findall.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,17 +253,17 @@
             if found:
                 multi_found.update(found)
             # ******************************************************************
             # and just after check recursively all branches below
             for child_name in parent_node: # checking * sub-nodes
                 child_node = parent_node[child_name]
                 if isinstance(child_node, (dict, list)):
-                    n0debug("seeked_xpath_list")
-                    n0debug_calc(found_xpath_list + [child_name], "found_xpath_list + [child_name]") ## n0debug_calc(found_xpath_list + seeked_xpath_list[0:1], "found_xpath_list + seeked_xpath_list[0:1]")
-                    n0debug_calc("/".join(found_xpath_list).replace('/[', '['), "parent_node")
+                    # n0debug("seeked_xpath_list")
+                    # n0debug_calc(found_xpath_list + [child_name], "found_xpath_list + [child_name]") ## n0debug_calc(found_xpath_list + seeked_xpath_list[0:1], "found_xpath_list + seeked_xpath_list[0:1]")
+                    # n0debug_calc("/".join(found_xpath_list).replace('/[', '['), "parent_node")
                     found = _findall(
                                     child_node,
                                     seeked_xpath_list,
                                     found_xpath_list + [child_name], ##found_xpath_list + seeked_xpath_list[0:1],
                                     {**parent_nodes_stack, **{"//" + "/".join(found_xpath_list).replace('/[', '['): parent_node}},
                                     raise_exception,
                                     level + 1,
```

### Comparing `n0struct-0.2.90/n0struct/n0struct_git.py` & `n0struct-0.2.91/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_logging.py` & `n0struct-0.2.91/n0struct/n0struct_logging.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_mask.py` & `n0struct-0.2.91/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.91/n0struct/n0struct_n0dict_.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     def __xpath(self, value, path: str = None, mode: int = None) -> list:
         """
         Private function: recursively collect elements xpath starts from parent
         """
         result = []
         if isinstance(value, (list, tuple)):
             for i, subitm in enumerate(value):
-                result += self.__xpath(subitm, "%s[%d]" % (path, i), mode)
+                result += self.__xpath(subitm, f"{path}[{i}]", mode)
         elif isinstance(value, dict):
             for key, value in value.items():
-                result += self.__xpath(value, "%s/%s" % (path, key), mode)
+                result += self.__xpath(value, f"{path}/{key}", mode)
         elif isinstance(value, (str, int, float)) or value is None:
             result.append((path, value))
         else:
             raise TypeError(f"Not expected type ({type(value)}) in {path} == {value}")
         return result
     # **************************************************************************
     def xpath(self, mode: int = None) -> list:  # list[(xpath, value)]
@@ -103,68 +103,66 @@
                 for key, value in parent.items():
                     if result:
                         result += "\n"
                     if isinstance(value, (list, tuple)):
                         for i, subitm in enumerate(value):
                             if i:
                                 result += "\n"
-                            sub_result = self.__xml(subitm, indent + inc_indent, inc_indent)
+                            sub_result = self.__xml(subitm, indent+inc_indent, inc_indent)
                             if not sub_result:
                                 if isinstance(sub_result, str):
-                                    result += " " * indent + "<%s></%s>" % (key,key)
+                                    result += " "*indent + f"<{key}></{key}>"
                                 else:
-                                    result += " " * indent + "<%s/>" % key
+                                    result += " "*indent + f"<{key}/>"
                             else:
                                 if '>' in sub_result:
-                                    result += (" " * indent + "<%s>\n%s\n" + " " * indent + "</%s>") % (key, sub_result, key)
+                                    result += " "*indent + f"<{key}>\n{sub_result}\n" + " "*indent + f"</{key}>"
                                 else:
-                                    result += (" " * indent + "<%s>%s</%s>") % (key, sub_result, key)
+                                    result += " "*indent + f"<{key}>{sub_result}</{key}>"
                     elif isinstance(value, (str, int, float)):
                         if not key.startswith("@"):
-                            result += " " * indent + ("<%s>%s</%s>" % (key, str(value).translate(html_entities), key))
+                            result += " "*indent + f"<{key}>{str(value).translate(html_entities)}</{key}>"
                     elif isinstance(value, dict):
-                        sub_result = self.__xml(value, indent + inc_indent, inc_indent)
+                        sub_result = self.__xml(value, indent+inc_indent, inc_indent)
 
                         attribs = ""
                         attribs_of_current_key = [(__key[1:], __value) for __key,__value in value.items() if __key.startswith("@")]
                         if len(attribs_of_current_key):
                             for __key, __value in attribs_of_current_key:
-                                attribs += " %s=\"%s\"" % (__key, __value)
+                                attribs += f' {__key}="{__value}"'
                         if sub_result:
-                            result += (" " * indent + "<%s%s>\n%s\n" + " " * indent + "</%s>") % (key, attribs, sub_result, key)
+                            result += " "*indent + f"<{key}{attribs}>\n{sub_result}\n" + " "*indent + f"</{key}>"
                         else:
-                            result += " " * indent + "<%s%s/>" % (key, attribs)
+                            result += " "*indent + f"<{key}{attribs}/>"
                     elif value is None:
-                        result += " " * indent + "<%s/>" % key
+                        result += " "*indent + f"<{key}/>"
                     else:
-                        raise TypeError("__xml(..): Unknown type (%s) %s ==  %s" % (type(value), key, str(value)))
+                        raise TypeError(f"__xml(..): Unknown type ({type(value)}) {key} == {value}")
             elif isinstance(parent, (list, tuple)):
                 if not len(parent):
                     return None
                 for i, itm in enumerate(parent):
                     if i:
                         result += "\n"
-                    result += self.__xml(itm, indent + inc_indent, inc_indent)
+                    result += self.__xml(itm, indent+inc_indent, inc_indent)
             elif isinstance(parent, (str, int, float)):
                 result += str(parent)
             else:
-                raise TypeError("__xml(..): Unknown type (%s) ==  %s" % (type(parent), str(parent)))
+                raise TypeError(f"__xml(..): Unknown type ({type(parent)}) == {parent}")
 
             return result
         else:
             return ""
     # **************************************************************************
     def to_xml(self, indent: int = 4, encoding: str = "utf-8") -> str:
         """
         Public function: export self into xml result string
         """
-        result = ""
-        if encoding:
-            result = "<?xml version=\"1.0\" encoding=\"%s\"?>\n" % encoding
-        return result + self.__xml(self, 0, indent)
+        return (f'<?xml version="1.0" encoding="{encoding}"?>\n' if encoding else '') + \
+            self.__xml(self, 0, indent)
     # **************************************************************************
     # JSON
     # **************************************************************************
     def __json(self, parent: dict, indent: int, inc_indent: int) -> str:
         """
         Private function: recursively export n0dict into json result string
         """
@@ -173,53 +171,51 @@
             if result:
                 result += ",\n"
             if isinstance(value, list):
                 sub_result = ""
                 for i, subitm in enumerate(value):
                     if sub_result:
                         sub_result += ",\n"
-                    sub_sub_result = self.__json(subitm, indent + inc_indent * 2, inc_indent)
+                    sub_sub_result = self.__json(subitm, (indent+inc_indent)*2, inc_indent)
                     if sub_sub_result:
                         if isinstance(subitm, dict):
-                            sub_result += (" " * (indent + inc_indent) + "{\n%s\n" + " " * (
-                                    indent + inc_indent) + "}") % sub_sub_result
+                            sub_result += " "*(indent+inc_indent) + "{" + f"\n{sub_sub_result}\n" + " "*(indent+inc_indent) + "}"
                         elif isinstance(subitm, (list, tuple)):
-                            sub_result += (" " * (indent + inc_indent) + "[\n%s\n" + " " * (
-                                    indent + inc_indent) + "]") % sub_sub_result
+                            sub_result += " "*(indent+inc_indent) + f"[\n{sub_sub_result}\n" + " "*(indent+inc_indent) + "]"
                 if sub_result:
-                    result += (" " * indent + '"%s": [\n%s\n' + " " * indent + "]") % (key, sub_result)
+                    result += " "*indent + f'"{key}": [\n{sub_result}\n' + " "*indent + "]"
                 else:
-                    result += " " * indent + '"%s": null' % key
+                    result += " "*indent + f'"{key}": null'
             elif isinstance(value, str):
-                result += " " * indent + ('"%s": "%s"' % (key, value))
+                result += " "*indent + f'"{key}": "{value}"'
             elif isinstance(value, dict):
-                sub_result = self.__json(value, indent + inc_indent, inc_indent)
+                sub_result = self.__json(value, indent+inc_indent, inc_indent)
                 if sub_result:
-                    result += (" " * indent + '"%s": {\n%s\n' + " " * indent + "}") % (key, sub_result)
+                    result += " "*indent + f'"{key}": ' + "{" + f"\n{sub_result}\n" + " "*indent + "}"
                 else:
-                    result +=  " " * indent + '"%s": null' % key
+                    result += " "*indent + f'"{key}": null'
             elif value is None:
-                result += " " * indent + '"%s": null' % key
+                result += " "*indent + '"%s": null' % key
             else:
-                raise TypeError("Unknown type (%s) %s ==  %s" % (type(value), key, str(value)))
+                raise TypeError(f"Unknown type ({type(value)}) {key} == {value}")
         return result
     # **************************************************************************
-    def to_json(self, 
+    def to_json(self,
                 indent: int = 4,
                 pairs_in_one_line = True,
                 json_convention: bool = True,
                 skip_empty_arrays: bool = False,
                 compress: bool = False,
     ) -> str:
         """
         Public function: export self into json result string
         """
         if compress:
             indent = 0
-        
+
         return n0pretty(self,
                         show_type=False,
                         auto_quotes=False,
                         __quotes='"',
                         __indent_size=indent,
                         pairs_in_one_line=pairs_in_one_line,
                         json_convention=json_convention,
```

### Comparing `n0struct-0.2.90/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.91/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_n0list_.py` & `n0struct-0.2.91/n0struct/n0struct_n0list_.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.91/n0struct/n0struct_n0list_n0dict.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_random.py` & `n0struct-0.2.91/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_references.py` & `n0struct-0.2.91/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.91/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_utils.py` & `n0struct-0.2.91/n0struct/n0struct_utils.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.91/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/n0struct_utils_find.py` & `n0struct-0.2.91/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/test/test_n0struct.py` & `n0struct-0.2.91/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/test/test_n0struct2.py` & `n0struct-0.2.91/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct/test/test_n0struct3.py` & `n0struct-0.2.91/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.91/n0struct.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.90
+Version: 0.2.91
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.90/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.91/n0struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.90/setup.py` & `n0struct-0.2.91/setup.py`

 * *Files identical despite different names*

