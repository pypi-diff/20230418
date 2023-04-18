# Comparing `tmp/pollev-history-compiler-1.0.1.tar.gz` & `tmp/pollev-history-compiler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollev-history-compiler-1.0.1.tar", last modified: Mon Apr 17 23:39:09 2023, max compression
+gzip compressed data, was "pollev-history-compiler-1.0.2.tar", last modified: Tue Apr 18 17:18:49 2023, max compression
```

## Comparing `pollev-history-compiler-1.0.1.tar` & `pollev-history-compiler-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.756001 pollev-history-compiler-1.0.1/
--rw-rw-rw-   0        0        0     1898 2023-04-17 23:39:09.755000 pollev-history-compiler-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1244 2023-04-17 23:35:47.000000 pollev-history-compiler-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.751003 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/
--rw-rw-rw-   0        0        0     1898 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 23:39:09.000000 pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.753003 pollev-history-compiler-1.0.1/pollev_tools/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:46:25.000000 pollev-history-compiler-1.0.1/pollev_tools/__init__.py
--rw-rw-rw-   0        0        0    26266 2023-04-17 23:22:21.000000 pollev-history-compiler-1.0.1/pollev_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-04-17 23:39:09.754001 pollev-history-compiler-1.0.1/resources/
--rw-rw-rw-   0        0        0      567 2023-04-16 17:02:01.000000 pollev-history-compiler-1.0.1/resources/config.ini
--rw-rw-rw-   0        0        0      424 2023-04-17 23:31:29.000000 pollev-history-compiler-1.0.1/resources/html-styles.css
--rw-rw-rw-   0        0        0       42 2023-04-17 23:39:09.756001 pollev-history-compiler-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1251 2023-04-17 23:37:10.000000 pollev-history-compiler-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/
+-rw-rw-rw-   0        0        0     1898 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.923589 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/
+-rw-rw-rw-   0        0        0     1898 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 17:18:49.000000 pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.929186 pollev-history-compiler-1.0.2/pollev_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/pollev_tools/__init__.py
+-rw-rw-rw-   0        0        0    27958 2023-04-18 17:14:01.000000 pollev-history-compiler-1.0.2/pollev_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/resources/
+-rw-rw-rw-   0        0        0      567 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/resources/config.ini
+-rw-rw-rw-   0        0        0      424 2023-04-18 17:02:41.000000 pollev-history-compiler-1.0.2/resources/html-styles.css
+-rw-rw-rw-   0        0        0       42 2023-04-18 17:18:49.933287 pollev-history-compiler-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-04-18 17:14:40.000000 pollev-history-compiler-1.0.2/setup.py
```

### Comparing `pollev-history-compiler-1.0.1/PKG-INFO` & `pollev-history-compiler-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pollev-history-compiler-1.0.1/README.md` & `pollev-history-compiler-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pollev-history-compiler-1.0.1/pollev_history_compiler.egg-info/PKG-INFO` & `pollev-history-compiler-1.0.2/pollev_history_compiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollev-history-compiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: A script for the compilation of PollEverywhere history CSV files into more usable forms.
 Home-page: https://github.com/tony-zeidan/PollEvHistoryCompiler
 Author: Tony Abou Zeidan
 Author-email: tony.azp25@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pollev-history-compiler-1.0.1/pollev_tools/reader.py` & `pollev-history-compiler-1.0.2/pollev_tools/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,14 +343,52 @@
         
 
         with open(output_file, 'w', encoding=encoding) as out_file:
             out_file.write(html_gen)
 
     except KeyError:
         raise ValueError("Column couldn't be found, can't continue.")
+    
+def to_markdown_report(data_df: pd.DataFrame, output_file: str, show_correct: bool = True, encoding: str = None):
+    """
+    Converts the CSV dataframe into a LaTeX exam report.
+
+    :param data_df: The dataframe
+    :param output_file: The file to output to (.TeX)
+    :param encoding: The encoding to use when outputting
+    """
+    import markdownify
+
+    name, _ = os.path.splitext(output_file)
+
+    html_lst =  '\n'.join(data_df.apply(lambda x: html_helper(x, show_correct=show_correct), axis=1))
+
+    html_gen = f'''
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha384-KyZXEAg3QhqLMpG8r+Knujsl5/1zwaQ7wxt2NN9138DhxUeK5l/5Vp1+XWlFm_tv" crossorigin="anonymous"></script>
+    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway&display=swap" />
+    <link rel="stylesheet" href="html-styles.css">
+    <title>{name}</title>
+</head> 
+<body>
+    <div class='center-container'>
+        <div class='center-div'>
+            <h1>PollEverywhere Report</h1>
+        </div>          
+        {html_lst}
+    </div>
+</body>
+</html>
+        '''
+
+    md_str = markdownify.markdownify(html_gen)
+    with open(output_file, 'w', encoding=encoding) as out_file:
+        out_file.write(md_str)
 
 
 def dict_helper(row, show_correct: bool = True, question_col: str = 'Activity title'):
     """
     To Dict helper.
 
     """
@@ -610,14 +648,17 @@
     parser_tex.add_argument('--resp_opt_correct_block_type', type=str, help='LaTeX block used for a single response (if correct)', default=default_tex_opts['resp_opt_correct_block_type'])
     parser_tex.add_argument('--end_spacing', type=int, help='The amount of space to add after each response option', default=default_tex_opts['end_spacing'])
     parser_tex.add_argument('--end_spacing_metric', type=str, help='The metric for end_spacing', default=default_tex_opts['end_spacing_metric'])
     
     # HTML transform
     parser_html = transform_parser.add_parser('html', help='Convert to HTML', parents=[global_parser], add_help=True)
 
+    # Markdown transform
+    parser_markdown = transform_parser.add_parser('markdown', help='Convert to MARKDOWN', parents=[global_parser], add_help=True)
+
     # YAML transform
     parser_yaml = transform_parser.add_parser('yaml', help='Convert to YAML', parents=[global_parser], add_help=True)
     parser_yaml.add_argument('--root_name', type=str, help='Root name of YAML', default=default_yaml_opts['root_name'])
 
     # JSON transform
     parser_json = transform_parser.add_parser('json', help='Convert to JSON', parents=[global_parser], add_help=True)
     parser_json.add_argument('--root_name', type=str, help='Root name of JSON', default=default_json_opts['root_name'])
@@ -665,14 +706,16 @@
         # copy over the CSS file
         try:
             shutil.copyfile(styles_path, os.path.join(html_path, f'html-styles.css'))
         except Exception:
             pass
     elif args.transform == 'toml':
         to_toml_report(data_df, os.path.join(args.output_path, f'{name}.toml'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_toml_opts))
+    elif args.transform == 'markdown':
+        to_markdown_report(data_df, os.path.join(args.output_path, f'{name}.md'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_toml_opts))
     elif args.transform == 'txt':
         to_txt_exam(data_df, os.path.join(args.output_path, f'{name}.txt'), encoding=args.encoding, show_correct=show_correct, **update_defaults(args, default_text_opts))
     
     else:
         raise ValueError("You can't use that type of output transform, look at the docs for help.")
 
 if __name__ == '__main__':
```

### Comparing `pollev-history-compiler-1.0.1/resources/config.ini` & `pollev-history-compiler-1.0.2/resources/config.ini`

 * *Files identical despite different names*

### Comparing `pollev-history-compiler-1.0.1/setup.py` & `pollev-history-compiler-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pollev-history-compiler",
-    version="1.0.1",
+    version="1.0.2",
     author="Tony Abou Zeidan",
     author_email="tony.azp25@gmail.com",
     description="A script for the compilation of PollEverywhere history CSV files into more usable forms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tony-zeidan/PollEvHistoryCompiler",
     packages=find_packages(),
@@ -19,15 +19,16 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pandas'
+        'pandas',
+        'markdownify'
     ],
     package_data={
         "pollev_tools": [
             "../resources/html-styles.css",
             "../resources/config.ini",
 
         ],
```

