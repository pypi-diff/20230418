# Comparing `tmp/n0struct-0.2.91.tar.gz` & `tmp/n0struct-0.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.91.tar", last modified: Tue Apr 18 04:25:19 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.92.tar", last modified: Tue Apr 18 04:33:57 2023, max compression
```

## Comparing `n0struct-0.2.91.tar` & `n0struct-0.2.92.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.087728 n0struct-0.2.91/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.91/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-04-18 04:25:19.087728 n0struct-0.2.91/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.91/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 04:25:18.978374 n0struct-0.2.91/n0struct/
--rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.91/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.91/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.91/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.91/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.91/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.91/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.91/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    16003 2023-04-17 11:25:17.000000 n0struct-0.2.91/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4027 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20923 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.91/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    11638 2023-04-18 04:13:47.000000 n0struct-0.2.91/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17432 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7507 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    77681 2023-04-18 04:23:46.000000 n0struct-0.2.91/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.91/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3863 2023-02-26 20:17:13.000000 n0struct-0.2.91/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.91/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.91/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6670 2023-02-26 19:26:05.000000 n0struct-0.2.91/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4123 2023-03-28 07:56:46.000000 n0struct-0.2.91/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.087728 n0struct-0.2.91/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.91/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.91/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.91/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.91/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.91/n0struct/test/test_n0struct3.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:25:19.072142 n0struct-0.2.91/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2023-04-18 04:25:18.000000 n0struct-0.2.91/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 04:25:17.000000 n0struct-0.2.91/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 04:25:19.103386 n0struct-0.2.91/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.884253 n0struct-0.2.92/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.92/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-04-18 04:33:57.885253 n0struct-0.2.92/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.92/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.808189 n0struct-0.2.92/n0struct/
+-rw-rw-rw-   0        0        0    13230 2023-04-02 07:25:19.000000 n0struct-0.2.92/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3665 2023-04-02 13:22:27.000000 n0struct-0.2.92/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2646 2023-04-02 07:35:55.000000 n0struct-0.2.92/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13040 2023-04-02 06:07:40.000000 n0struct-0.2.92/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     2847 2023-04-17 17:27:53.000000 n0struct-0.2.92/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    22639 2023-04-02 12:49:20.000000 n0struct-0.2.92/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7171 2023-04-02 12:54:45.000000 n0struct-0.2.92/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15645 2023-04-18 03:40:30.000000 n0struct-0.2.92/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-18 03:45:21.000000 n0struct-0.2.92/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20911 2023-04-18 03:47:04.000000 n0struct-0.2.92/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-03-10 04:00:32.000000 n0struct-0.2.92/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    11636 2023-04-18 04:27:09.000000 n0struct-0.2.92/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17317 2023-04-18 04:08:26.000000 n0struct-0.2.92/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     7527 2023-04-18 04:15:40.000000 n0struct-0.2.92/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    77456 2023-04-18 04:22:33.000000 n0struct-0.2.92/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-02-26 06:04:26.000000 n0struct-0.2.92/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-18 04:31:43.000000 n0struct-0.2.92/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3233 2023-04-02 06:21:50.000000 n0struct-0.2.92/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    17303 2023-04-02 06:34:23.000000 n0struct-0.2.92/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6658 2023-04-18 04:28:52.000000 n0struct-0.2.92/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4117 2023-04-18 04:29:28.000000 n0struct-0.2.92/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.880258 n0struct-0.2.92/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.92/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.92/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    29786 2023-02-26 19:17:57.000000 n0struct-0.2.92/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.92/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0     1177 2023-03-23 03:01:29.000000 n0struct-0.2.92/n0struct/test/test_n0struct3.py
+drwxrwxrwx   0        0        0        0 2023-04-18 04:33:57.857859 n0struct-0.2.92/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2023-04-18 04:33:57.000000 n0struct-0.2.92/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 04:33:56.000000 n0struct-0.2.92/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 04:33:57.891284 n0struct-0.2.92/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.92/setup.py
```

### Comparing `n0struct-0.2.91/LICENSE` & `n0struct-0.2.92/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/PKG-INFO` & `n0struct-0.2.92/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.91
+Version: 0.2.92
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.91/README.md` & `n0struct-0.2.92/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/__init__.py` & `n0struct-0.2.92/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_arrays.py` & `n0struct-0.2.92/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.92/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_date.py` & `n0struct-0.2.92/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_files.py` & `n0struct-0.2.92/n0struct/n0struct_files.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_files_csv.py` & `n0struct-0.2.92/n0struct/n0struct_files_csv.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.92/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_findall.py` & `n0struct-0.2.92/n0struct/n0struct_findall.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,17 +253,14 @@
             if found:
                 multi_found.update(found)
             # ******************************************************************
             # and just after check recursively all branches below
             for child_name in parent_node: # checking * sub-nodes
                 child_node = parent_node[child_name]
                 if isinstance(child_node, (dict, list)):
-                    # n0debug("seeked_xpath_list")
-                    # n0debug_calc(found_xpath_list + [child_name], "found_xpath_list + [child_name]") ## n0debug_calc(found_xpath_list + seeked_xpath_list[0:1], "found_xpath_list + seeked_xpath_list[0:1]")
-                    # n0debug_calc("/".join(found_xpath_list).replace('/[', '['), "parent_node")
                     found = _findall(
                                     child_node,
                                     seeked_xpath_list,
                                     found_xpath_list + [child_name], ##found_xpath_list + seeked_xpath_list[0:1],
                                     {**parent_nodes_stack, **{"//" + "/".join(found_xpath_list).replace('/[', '['): parent_node}},
                                     raise_exception,
                                     level + 1,
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_git.py` & `n0struct-0.2.92/n0struct/n0struct_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,39 +26,42 @@
                                 ["clone", repository_url] +
                                 ["--config", "core.sshCommand=ssh -i " + rsa_key_path + " -F /dev/null"] if rsa_key_path else []
             )
             self._repository_name = repository_url.split("/")[-1].split(".git")[0]
             self._repository_path = os.path.join(self._repository_path, self._repository_name)
         else:
             self._repository_name = os.path.split(self._repository_path)[1]
-            n0print("Other repository '%s' is already existed" % self._repository_name)
+            n0print(f"Other repository '{self._repository_name}' is already existed")
 
         if errs and "already exists and is not an empty directory." in errs:
             outs, errs = self.run("pull")
             if outs != "Already up to date.\n":
                 n0debug_calc(outs.strip(), "outs")
                 n0debug_calc(errs.strip(), "errs")
     # ##############################################################################################
     def run(self, git_arguments: typing.Union[str, list], show_result = True) -> tuple:
         if isinstance(git_arguments, str):
             git_arguments = git_arguments.split(" ")
-        n0print("*** git %s" % " ".join(git_arguments))
+        n0print(f"*** git {' '.join(git_arguments)}")
         command_line = ["git",] + git_arguments  # removed walrus operator for compatibility with 3.7
         p = subprocess.Popen(   command_line,
                                 cwd = self._repository_path,
                                 stdout = subprocess.PIPE,
                                 stderr = subprocess.PIPE,
                                 shell = True,
                                 encoding = "utf-8",
         )
         try:
             timeout_sec = 600  # removed walrus operator for compatibility with 3.7
             outs, errs = p.communicate(timeout = timeout_sec)
         except subprocess.TimeoutExpired:
-            raise TimeoutError("Timeout %d seconds were happened during execution:\n%s>%s" % (timeout_sec, self._repository_path, " ".join(command_line)))
+            raise TimeoutError(
+                f"Timeout {timeout_sec} seconds were happened during execution:\n" +
+                f"{self._repository_path}>{' '.join(command_line)}"
+            )
 
         if show_result:
             n0debug_calc(outs.strip(), "outs")
             n0debug_calc(errs.strip(), "errs")
         return outs, errs
     # ##############################################################################################
     def checkout(self, branch_name: str):
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_logging.py` & `n0struct-0.2.92/n0struct/n0struct_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,20 +446,20 @@
         attrib = getattr(class_object, attrib_name)
         if callable(attrib):
             class_methods.add(attrib_name)
         else:
             class_attribs.add(attrib_name)
 
     for attrib_name in class_methods:
-        to_print += "=*= function %s()\n" % attrib_name
+        to_print += f"=*= function {attrib_name}()\n"
 
     for attrib_name in class_attribs:
         attrib = getattr(class_object, attrib_name)
         prefix = str(type(attrib)) if __debug_show_object_type else "" + \
-                 " id=%s" % id(attrib) if __debug_show_object_id else ""
+                 f" id={id(attrib)}" if __debug_show_object_id else ""
         if prefix:
             prefix = "(" + prefix + ")"
-        to_print += "=== %s%s = %s\n" % (prefix, attrib_name, n0pretty(attrib))
+        to_print += f"=== {prefix}{attrib_name} = {n0pretty(attrib)}\n"
 
     n0print(to_print, level = level, internal_call = True)
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_mask.py` & `n0struct-0.2.92/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.92/n0struct/n0struct_n0dict_.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             elif isinstance(value, dict):
                 sub_result = self.__json(value, indent+inc_indent, inc_indent)
                 if sub_result:
                     result += " "*indent + f'"{key}": ' + "{" + f"\n{sub_result}\n" + " "*indent + "}"
                 else:
                     result += " "*indent + f'"{key}": null'
             elif value is None:
-                result += " "*indent + '"%s": null' % key
+                result += " "*indent + f'"{key}": null'
             else:
                 raise TypeError(f"Unknown type ({type(value)}) {key} == {value}")
         return result
     # **************************************************************************
     def to_json(self,
                 indent: int = 4,
                 pairs_in_one_line = True,
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.92/n0struct/n0struct_n0dict__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
         return self[where1/where2/.../whereN]
             AKA
         return self[where1][where2]...[whereN]
 
         If any of [where1][where2]...[whereN] are not found, exception IndexError will be raised
         """
         if not xpath:
-            raise IndexError("xpath '%s' is not valid" % str(xpath))
+            raise IndexError(f"xpath '{xpath}' is not valid")
         if xpath.startswith('?'):
             xpath = xpath[1:]
             raise_exception = False
             if_not_found = ''
         if any(char in xpath for char in "/["):
             parent_node, node_name_index, cur_value, xpath_found_str, not_found_xpath_list = self._find(xpath, self, return_lists)
             if not not_found_xpath_list:
                 return cur_value
             else:
                 if raise_exception:
-                    raise IndexError("not found '%s' in '%s'" % ('/'.join(not_found_xpath_list), xpath_found_str))
+                    raise IndexError(f"not found '{'/'.join(not_found_xpath_list)}' in '{xpath_found_str}'")
                 else:
                     return if_not_found
         else:
             try:
                 return super(n0dict__, self).__getitem__(xpath)
             except KeyError as ex:
                 if raise_exception:
@@ -124,23 +124,23 @@
             parent_node, node_name_index, cur_value, xpath_found_str, not_found_xpath_list = self._find(xpath, self, return_lists = True)
             if not_found_xpath_list:
                 parent_node, node_name_index = self._add(parent_node, node_name_index, not_found_xpath_list)
 
             node_name, node_index = split_name_index(node_name_index)
             if isinstance(parent_node, dict):
                 if node_index:
-                    raise IndexError("How is it possible: index '%s' for dictionary (%s)'%s'?"% (node_index, type(parent_node), parent_node))
+                    raise IndexError(f"How is it possible: index '{node_index}' for dictionary ({type(parent_node)})'{parent_node}'?")
                 parent_node.update({node_name_index: new_value})
             elif isinstance(parent_node, (list, tuple)):
                 if node_name:
-                    raise IndexError("How is it possible: key '%s' for list (%s)'%s'?" % (node_name, type(parent_node), parent_node))
+                    raise IndexError(f"How is it possible: key '{node_name}' for list ({type(parent_node)})'{parent_node}'?")
                 eval_node_index = n0eval(node_index)
                 parent_node[n0eval(node_index)] = new_value
             else:
-                raise TypeError("How is it possible: unknown type of parent node (%s) of '%s'" % (type(parent_node), parent_node))
+                raise TypeError(f"How is it possible: unknown type of parent node ({type(parent_node)}) of '{parent_node}'")
         else:
             super(n0dict__, self).__setitem__(xpath, new_value)
 
         return new_value  # For speed
     # **************************************************************************
     def delete(self, xpath: str, recursively: bool = False) -> n0dict__:
         xpath_list = xpath.split('/')
@@ -275,15 +275,15 @@
 
         # TO DO: redo with 'in'
         try:
             if self[xpath]:
                 return validation_results
         except:
             pass
-        validation_results["differences"].append("[%s] doesn't exist" % xpath)
+        validation_results["differences"].append(f"[{xpath}] doesn't exist")
         validation_results["other_unique"].append((xpath, None))
         return validation_results
     # **************************************************************************
     # **************************************************************************
     def is_exist(self, xpath: str) -> bool:
         """
         Public function: return True, if self[xpath] exists
@@ -325,15 +325,15 @@
         if notemptyitems(validation_results):
             return validation_results
         try:
             if self[xpath] == value:
                 return []
         except:
             pass
-        validation_results["differences"].append("[%s]=='%s' != '%s'" % (xpath, self[xpath], value))
+        validation_results["differences"].append(f"[{xpath}]=='{self[xpath]}' != '{value}'")
         validation_results["not_equal"].append((xpath, (self[xpath], value)))
         return validation_results
     # **************************************************************************
     # **************************************************************************
     def isTheSame(self, xpath, other_n0dict, other_xpath=None, transformation=lambda x: x):
         """
         Public function: return empty lists in dict, if transformation(self[xpath]) == transformation(other_n0dict[other_xpath])
@@ -345,16 +345,14 @@
             return validation_results
         try:
             if transformation(self[xpath]) == transformation(other_n0dict[other_xpath]):
                 return validation_results
         except:
             # n0print("EXCEPTION in 'if transformation(self[xpath]) == transformation(other_n0dict[other_xpath]):'")
             pass
-        validation_results["differences"].append("[%s]=='%s' != [%s]=='%s'" % (
-            xpath, transformation(self[xpath]),
-            other_xpath, transformation(other_n0dict[other_xpath])
+        validation_results["differences"].append(
+            f"[{xpath}]=='{transformation(self[xpath])}' != [{other_xpath}]=='{transformation(other_n0dict[other_xpath])}'"
         )
-                                              )
         validation_results["not_equal"].append((xpath, (self[xpath], other_n0dict[other_xpath])))
         return validation_results
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_n0list_.py` & `n0struct-0.2.92/n0struct/n0struct_n0list_.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             if_not_found = ''
         if any(char in xpath for char in "/["):
             parent_node, node_name_index, cur_value, xpath_found_str, not_found_xpath_list = self._find(xpath, self, return_lists)
             if not not_found_xpath_list:
                 return cur_value
             else:
                 if raise_exception:
-                    raise IndexError("not found '%s' in '%s'" % ('/'.join(not_found_xpath_list), xpath_found_str))
+                    raise IndexError(f"not found '{'/'.join(not_found_xpath_list)}' in '{xpath_found_str}'")
                 else:
                     return if_not_found
         else:
             try:
                 return super(n0list_, self).__getitem__(n0eval(xpath))
             except IndexError as ex:
                 if raise_exception:
@@ -91,27 +91,27 @@
 
         If any of [where1][where2]...[whereN] are not found, exception IndexError will be raised
         """
         if isinstance(xpath, str):
             return self._get(xpath, raise_exception = True)
         else:
             return super(n0list_, self).__getitem__(xpath)
-    # **************************************************************************
-    # def append(self, sigle_item):
-    # if isinstance(sigle_item, (list,n0list_)):
-    # raise (TypeError, '(%s)%s must be scalar' % (type(sigle_item), sigle_item))
-    # super(n0list_, self).append(sigle_item)  #append the item to itself (the list)
-    # return self
-    # **************************************************************************
-    # def extend(self, other_list):
-    # if not isinstance(other_list, (list,n0list_)):
-    # raise (TypeError, '(%s)%s must be list' % (type(sigle_item), sigle_item))
-    # super(n0list_, self).extend(other_list)
-    # return self
-    # **************************************************************************
+    # # **************************************************************************
+    # # def append(self, sigle_item):
+    # # if isinstance(sigle_item, (list,n0list_)):
+    # # raise (TypeError, '(%s)%s must be scalar' % (type(sigle_item), sigle_item))
+    # # super(n0list_, self).append(sigle_item)  #append the item to itself (the list)
+    # # return self
+    # # **************************************************************************
+    # # def extend(self, other_list):
+    # # if not isinstance(other_list, (list,n0list_)):
+    # # raise (TypeError, '(%s)%s must be list' % (type(sigle_item), sigle_item))
+    # # super(n0list_, self).extend(other_list)
+    # # return self
+    # # **************************************************************************
     def _in(self, other_list, in_is_expected: bool):
         if not isinstance(other_list, (list, tuple)):
             other_list = [other_list]
         for itm in self:
             if (itm in other_list) == in_is_expected:
                 return True
         return False
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.92/n0struct/n0struct_n0list_n0dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,29 +155,29 @@
                     len__parent_node = 1
                     parent_node = [parent_node]
 
                 if node_index_int >= len__parent_node or node_index_int < -len__parent_node:
                     #--------------------------------
                     # NOT FOUND: Element in n0list
                     #--------------------------------
-                    return parent_node, "[%s]" % str(node_index_int), None, xpath_found_str, xpath_list
+                    return parent_node, f"[{node_index_int}]", None, xpath_found_str, xpath_list
                 if len(xpath_list) == 1:
                     #================================
                     # FOUND: the last is n0list
                     #================================
-                    return parent_node, "[%s]" % str(node_index_int), parent_node[node_index_int], xpath_found_str, None
+                    return parent_node, f"[{node_index_int}]", parent_node[node_index_int], xpath_found_str, None
                 else:
                     #*******************************
                     # Deeper: any type under n0dict
                     #*******************************
                     next_parent_node =  parent_node[node_index_int]
                     if isinstance(next_parent_node, dict):
-                        return n0dict._find(next_parent_node, xpath_list[1:], next_parent_node, return_lists, "%s[%d]" % (xpath_found_str, node_index_int))
+                        return n0dict._find(next_parent_node, xpath_list[1:], next_parent_node, return_lists, f"{xpath_found_str}[{node_index_int}]")
                     if isinstance(next_parent_node, (list, tuple)):
-                        return self._find(xpath_list[1:], next_parent_node, return_lists, "%s[%d]" % (xpath_found_str, node_index_int))
+                        return self._find(xpath_list[1:], next_parent_node, return_lists, f"{xpath_found_str}[{node_index_int}]")
                     else:
                         raise TypeError(f"Unexpected type ({type(next_parent_node)}) of {str(next_parent_node)}")
     # **************************************************************************
     # * n0list. direct_compare(..): only n0dict. direct_compare/compare have one_of_list_compare
     # **************************************************************************
     def direct_compare(
             self,
@@ -249,15 +249,15 @@
                     (
                         self_name, other_name,
                         self_name, i, str(self[i]),
                         other_name
                     )
                 )
                 if get__flag_compare_return_place():
-                    result["self_unique"].append(("%s[%i]" % (prefix, i), self[i]))
+                    result["self_unique"].append((f"{prefix}[{i}]", self[i]))
                 else:
                     result["self_unique"].append(self[i])
                 continue
             # ######### if i >= len(other):
             # --- TRANSFORM: START -------------------------------------
             # Transform self and other linked values with function transform[]()
             self_value = self[i]
@@ -275,15 +275,15 @@
             # --- TRANSFORM: END ---------------------------------------
             if type(self_value) == type(other_value):
                 if isinstance(self_value, (str, int, float)):
                     if self_value != other_value:
                         # VERY IMPORTANT TO SHOW ORIGINAL VALUES, NOT TRANSFORMED
                         result["not_equal"].append(
                             (
-                                "%s[%i]" % (prefix, i),
+                                f"{prefix}[{i}]",
                                 [
                                     self[i],
                                     other[i]
                                 ]
                             )
                         )
                         if get__flag_compare_return_difference_of_values():
@@ -305,29 +305,29 @@
                         if get__flag_compare_return_equal():
                             result["self_equal"].append(self)
                             result["other_equal"].append(other)
                 elif isinstance(self[i], (list, tuple)):
                     result.update_extend(
                         self[i].direct_compare(
                             other[i],
-                            "%s[%i]" % (self_name, i),
-                            "%s[%i]" % (other_name, i),
-                            "%s[%i]" % (prefix, i),
+                            f"{self_name}[{i}]",
+                            f"{other_name}[{i}]",
+                            f"{prefix}[{i}]",
                             # Not used in real, just for compatibility with compare(..)
                             composite_key=composite_key, compare_only=compare_only,
                             exclude_xpaths=exclude_xpaths, transform=transform,
                         )
                     )
                 elif isinstance(self[i], dict):
                     result.update_extend(
                         n0dict(self[i]).direct_compare(
                             n0dict(other[i]),
-                            "%s[%i]" % (self_name, i),
-                            "%s[%i]" % (other_name, i),
-                            "%s[%i]" % (prefix, i),
+                            f"{self_name}[{i}]",
+                            f"{other_name}[{i}]",
+                            f"{prefix}[{i}]",
                             one_of_list_compare=self.direct_compare,
                             composite_key=composite_key, compare_only=compare_only,
                             # Not used in real, just for compatibility
                             exclude_xpaths=exclude_xpaths, transform=transform,
                         )
                     )
                 elif self[i] is None:
@@ -337,34 +337,30 @@
                 else:
                     raise TypeError(f"Not expected type {type(self[i])} in {self_name}[{i}]/{other_name}[{i}]")
             # ######### if type(self[i]) == type(other[i]):
             else:
                 if get__flag_compare_check_different_types():
                     result["difftypes"].append(
                         (
-                            "%s[%i]" % (prefix, i),
+                            f"{prefix}[{i}]",
                             (
                                 type(self[i]),
                                 self[i],
                                 type(other[i]),
                                 other[i]
                             )
                         )
                     )
                     result["differences"].append(
-                        "!!Types are different: %s[%d]=(%s)%s != %s[%d]=(%s)%s" %
-                        (
-                            self_name, i, type(self[i]), str(self[i]),
-                            other_name, i, type(other[i]), str(other[i]),
-                        )
+                        f"!!Types are different: {self_name}[{i}]=({type(self[i])}){self[i]} != {other_name}[{i}]=({type(other[i])}){other[i]}"
                     )
                 else:
                     result["not_equal"].append(
                         (
-                            "%s[%i]" % (prefix, i),
+                            f"{prefix}[{i}]",
                             (
                                 self[i],
                                 other[i]
                             )
                         )
                     )
                     result["differences"].append(
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_random.py` & `n0struct-0.2.92/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_references.py` & `n0struct-0.2.92/n0struct/n0struct_references.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,16 @@
             raise KeyError('set is empty')
         key = self.end[1][0] if last else self.end[2][0]
         self.discard(key)
         return key
 
     def __repr__(self) -> str:
         if not self:
-            return '%s()' % (self.__class__.__name__,)
-        return '%s(%r)' % (self.__class__.__name__, list(self))
+            return f"{self.__class__.__name__}()"
+        return f"{self.__class__.__name__}({list(self)})"
 
     def __eq__(self, other) -> bool:
         if isinstance(other, OrderedSet):
             return len(self) == len(other) and list(self) == list(other)
         return set(self) == set(other)
 # ******************************************************************************
 # 2 levels dict:
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.92/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_utils.py` & `n0struct-0.2.92/n0struct/n0struct_utils.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.92/n0struct/n0struct_utils_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,21 @@
         if isinstance(line, dict):
             created_composite_key = ""
             if elements_for_composite_key:
                 for key in elements_for_composite_key:
                     if key in line:
                         if created_composite_key:
                             created_composite_key += ";"
-                        fullxpath = "%s/%s" % (prefix, key)
+                        fullxpath = f"{prefix}/{key}"
                         transform_i = xpath_match(fullxpath, attributes_to_transform)
                         if transform_i:
                             transform_i -= 1
                             tranformed = transform[transform_i][1](line[key])
                         else:
                             tranformed = str(line[key])
                         created_composite_key += key + "=" + tranformed
         else:
-            raise TypeError("generate_composite_keys(..): expected element dict inside list, but got (%s)%s" % (type(line), line))
+            raise TypeError(f"generate_composite_keys(..): expected element dict inside list, but got ({type(line)}){line}")
         composite_keys_for_all_lines.append((created_composite_key, line_i))
     return composite_keys_for_all_lines
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.91/n0struct/n0struct_utils_find.py` & `n0struct-0.2.92/n0struct/n0struct_utils_find.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                                                         str,
                                                         typing.Union[
                                                             str,
                                                             typing.Tuple[str, str, typing.Union[str, bool]]
                                                         ]
                                                     ]:
     if not isinstance(node_name, str):
-        raise TypeError("node_name (%s)%s must be string" % (type(node_name), node_name))
+        raise TypeError(f"node_name ({type(node_name)}){node_name} must be string")
 
     node_index_tuple = None
     if '[' in node_name and node_name.endswith(']'):
         node_name, node_index_str = node_name[:-1].split('[', 1)
         node_name = node_name.strip()
         node_index_str = node_index_str.strip()
         if node_index_str:
```

### Comparing `n0struct-0.2.91/n0struct/test/test_n0struct.py` & `n0struct-0.2.92/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/test/test_n0struct2.py` & `n0struct-0.2.92/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct/test/test_n0struct3.py` & `n0struct-0.2.92/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.92/n0struct.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.91
+Version: 0.2.92
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.91/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.92/n0struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.91/setup.py` & `n0struct-0.2.92/setup.py`

 * *Files identical despite different names*

