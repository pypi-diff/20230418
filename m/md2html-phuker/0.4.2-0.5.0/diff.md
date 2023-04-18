# Comparing `tmp/md2html-phuker-0.4.2.tar.gz` & `tmp/md2html-phuker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2html-phuker-0.4.2.tar", last modified: Wed Aug 25 15:17:16 2021, max compression
+gzip compressed data, was "md2html-phuker-0.5.0.tar", last modified: Tue Apr 18 15:56:00 2023, max compression
```

## Comparing `md2html-phuker-0.4.2.tar` & `md2html-phuker-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2021-08-25 15:17:16.257601 md2html-phuker-0.4.2/
--rw-r--r--   0 shen       (501) staff       (20)    35149 2020-10-21 12:33:14.000000 md2html-phuker-0.4.2/LICENSE
--rw-r--r--   0 shen       (501) staff       (20)       29 2020-10-20 20:11:23.000000 md2html-phuker-0.4.2/MANIFEST.in
--rw-r--r--   0 shen       (501) staff       (20)      779 2021-08-25 15:17:16.257757 md2html-phuker-0.4.2/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      119 2020-10-21 12:08:29.000000 md2html-phuker-0.4.2/Readme.PyPI.md
--rw-r--r--   0 shen       (501) staff       (20)     6092 2020-11-22 20:58:48.000000 md2html-phuker-0.4.2/Readme.md
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2021-08-25 15:17:16.255511 md2html-phuker-0.4.2/md2html/
--rwxr-xr-x   0 shen       (501) staff       (20)    10651 2021-08-25 15:15:45.000000 md2html-phuker-0.4.2/md2html/__init__.py
--rw-r--r--   0 shen       (501) staff       (20)    16608 2020-10-06 00:08:37.000000 md2html-phuker-0.4.2/md2html/github-markdown.css
--rw-r--r--   0 shen       (501) staff       (20)     3038 2020-11-21 17:27:31.000000 md2html-phuker-0.4.2/md2html/main.css
--rw-r--r--   0 shen       (501) staff       (20)     4394 2020-11-21 13:27:24.000000 md2html-phuker-0.4.2/md2html/pygments.css
--rw-r--r--   0 shen       (501) staff       (20)     1063 2020-11-22 20:47:48.000000 md2html-phuker-0.4.2/md2html/style-dark.css
--rw-r--r--   0 shen       (501) staff       (20)      419 2020-11-17 11:35:10.000000 md2html-phuker-0.4.2/md2html/style-sidebar-toc.css
-drwxr-xr-x   0 shen       (501) staff       (20)        0 2021-08-25 15:17:16.257285 md2html-phuker-0.4.2/md2html_phuker.egg-info/
--rw-r--r--   0 shen       (501) staff       (20)      779 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/PKG-INFO
--rw-r--r--   0 shen       (501) staff       (20)      432 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/SOURCES.txt
--rw-r--r--   0 shen       (501) staff       (20)        1 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/dependency_links.txt
--rw-r--r--   0 shen       (501) staff       (20)       42 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/entry_points.txt
--rw-r--r--   0 shen       (501) staff       (20)       82 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/requires.txt
--rw-r--r--   0 shen       (501) staff       (20)        8 2021-08-25 15:17:16.000000 md2html-phuker-0.4.2/md2html_phuker.egg-info/top_level.txt
--rw-r--r--   0 shen       (501) staff       (20)      101 2021-08-25 15:17:16.258234 md2html-phuker-0.4.2/setup.cfg
--rwxr-xr-x   0 shen       (501) staff       (20)     1223 2021-02-15 17:26:40.000000 md2html-phuker-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     5799 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.856723 md2html-phuker-0.5.0/md2html/
+-rwxr-xr-x   0 root         (0) root         (0)     9671 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16608 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/github-markdown.css
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/main.css
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/pygments.css
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/style-dark.css
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/style-sidebar-toc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.856723 md2html-phuker-0.5.0/md2html_phuker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1193 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/setup.py
```

### Comparing `md2html-phuker-0.4.2/LICENSE` & `md2html-phuker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.4.2/PKG-INFO` & `md2html-phuker-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.4.2
+Version: 0.5.0
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [Project homepage](https://github.com/Phuker/md2html)
 
 [Readme](https://github.com/Phuker/md2html/blob/main/Readme.md)
-
-
```

### Comparing `md2html-phuker-0.4.2/Readme.md` & `md2html-phuker-0.5.0/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 
 This is a *feng-he-guai* program. Python code based on:
 
 - [Python-Markdown](https://python-markdown.github.io/) and its officially supported extensions
 - [Phuker/markdown_link_attr_modifier](https://github.com/Phuker/markdown_link_attr_modifier), my `Python-Markdown` extension to add attributes like `target="_blank"` to `<a>` tags
 - [Zopieux/py-gfm](https://github.com/Zopieux/py-gfm), a `Python-Markdown` extension to support some [GFM](https://github.github.com/gfm/) features
-- [juancarlospaco/css-html-js-minify](https://github.com/juancarlospaco/css-html-js-minify), a library to minify CSS and HTML code
 
 CSS based on:
 
 - [sindresorhus/github-markdown-css](https://github.com/sindresorhus/github-markdown-css), the GitHub Markdown style, main theme
 - [Pygments](https://pygments.org/), style for Code highlight code blocks
 - Others copy & modify from [my blog](https://phuker.github.io/). The fonts are optimized for contents in Simplified Chinese.
 
@@ -64,34 +63,32 @@
 
 ## Usage
 
 ### Show help
 
 ```console
 $ md2html --help
-usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--style PRESET] [--append-css FILE] [--no-min-css] [--min-html] [--head-insert HTML] [--head-append HTML] [--body-insert HTML] [--body-append HTML] [input_file]
+usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert HTML] [--body-append HTML] [input_file]
 
 Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 
 positional arguments:
   input_file            If omitted or "-", use stdin.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --verbose         Verbose output
   -V, --version         Output version info and exit
   -t TITLE, --title TITLE
                         If omitted, generate from input filename
   -f, --force           Force overwrite if output file exists
   -o FILE, --output-file FILE
                         If omitted, auto decide. If "-", stdout.
   --style PRESET        Preset style addons, choices: sidebar-toc, dark
   --append-css FILE     Append embedded CSS files, may specify multiple times.
-  --no-min-css          Disable minify CSS, default enabled.
-  --min-html            Enable minify HTML, default disabled.
   --head-insert HTML    HTML to insert to the start of <head>, may specify multiple times.
   --head-append HTML    HTML to append to the end of <head>, may specify multiple times.
   --body-insert HTML    HTML to insert to the start of <body>, may specify multiple times.
   --body-append HTML    HTML to append to the end of <body>, may specify multiple times.
 ```
 
 If you are not sure about what will happen if you combine `[-o FILE]`, `[input_file]` and `[-t TITLE]`, see `test.py`, which contains tens of input cases and their intended behaviors.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_k5stb_am_/tmp9uftfogr_TarContainer/0/5.md", line 178, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_k5stb_am_/tmp9uftfogr_TarContainer/0/5.md", line 178, column 0: CDATA terminal not found*

```diff
@@ -1,57 +1,53 @@
 # md2html Yet another markdown to html converter, generate an offline all-in-
 one single HTML file. This is a *feng-he-guai* program. Python code based on: -
 [Python-Markdown](https://python-markdown.github.io/) and its officially
 supported extensions - [Phuker/markdown_link_attr_modifier](https://github.com/
 Phuker/markdown_link_attr_modifier), my `Python-Markdown` extension to add
 attributes like `target="_blank"` to `` tags - [Zopieux/py-gfm](https://
 github.com/Zopieux/py-gfm), a `Python-Markdown` extension to support some [GFM]
-(https://github.github.com/gfm/) features - [juancarlospaco/css-html-js-minify]
-(https://github.com/juancarlospaco/css-html-js-minify), a library to minify CSS
-and HTML code CSS based on: - [sindresorhus/github-markdown-css](https://
-github.com/sindresorhus/github-markdown-css), the GitHub Markdown style, main
-theme - [Pygments](https://pygments.org/), style for Code highlight code blocks
-- Others copy & modify from [my blog](https://phuker.github.io/). The fonts are
-optimized for contents in Simplified Chinese. ## Features ### Generated HTML
-The principle is: keep it simple. - All-in-one single HTML file - Completely
-offline, no CDN, no web fonts - No JavaScript ### Markdown syntax This is a
-Markdown dialect, similar but different from [GitHub Flavored Markdown (GFM)]
-(https://github.github.com/gfm/). Default enabled Markdown features: - [Extra]
-(https://python-markdown.github.io/extensions/extra/) extensions - [CodeHilite]
-(https://python-markdown.github.io/extensions/code_hilite/) - [Table of
-Contents](https://python-markdown.github.io/extensions/toc/) - [New Line to
-Break](https://python-markdown.github.io/extensions/nl2br/) - [Admonition]
-(https://python-markdown.github.io/extensions/admonition/) - ` - Part of GitHub
-Flavored Markdown For details, see `convert()` function of `md2html/
-__init__.py`, and the demo below. ## Demo - Default style: [docs/demo-
-default.html](https://phuker.github.io/md2html/demo-default.html) - With addon
-`--style sidebar-toc`: [docs/demo-sidebar-toc.html](https://phuker.github.io/
-md2html/demo-sidebar-toc.html) - With addon `--style dark`: [docs/demo-
-dark.html](https://phuker.github.io/md2html/demo-dark.html) - With addon `--
-style sidebar-toc --style dark`: [docs/demo-sidebar-toc-dark.html](https://
-phuker.github.io/md2html/demo-sidebar-toc-dark.html) All above files are
-generated from [docs/demo.md](./docs/demo.md). You can view its content to see
-supported syntax. ## Requirements - Python >= `3.6`, with `pip` installed ##
-Install ```bash python3 -m pip install -U md2html-phuker ``` There are too many
-similar projects with similar names in PyPI, `md2html`, `md-to-html`,
-`markdown2html`, `markdown-to-html`, `mrkdwn2html` ... I have to add a suffix
-to keep away from this war of naming. ## Usage ### Show help ```console $
-md2html --help usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--style
-PRESET] [--append-css FILE] [--no-min-css] [--min-html] [--head-insert HTML] [-
--head-append HTML] [--body-insert HTML] [--body-append HTML] [input_file] Yet
-another markdown to html converter, generate an offline all-in-one single HTML
-file. positional arguments: input_file If omitted or "-", use stdin. optional
-arguments: -h, --help show this help message and exit -v, --verbose Verbose
-output -V, --version Output version info and exit -t TITLE, --title TITLE If
-omitted, generate from input filename -f, --force Force overwrite if output
-file exists -o FILE, --output-file FILE If omitted, auto decide. If "-",
-stdout. --style PRESET Preset style addons, choices: sidebar-toc, dark --
-append-css FILE Append embedded CSS files, may specify multiple times. --no-
-min-css Disable minify CSS, default enabled. --min-html Enable minify HTML,
-default disabled. --head-insert HTML HTML to insert to the start of
+(https://github.github.com/gfm/) features CSS based on: - [sindresorhus/github-
+markdown-css](https://github.com/sindresorhus/github-markdown-css), the GitHub
+Markdown style, main theme - [Pygments](https://pygments.org/), style for Code
+highlight code blocks - Others copy & modify from [my blog](https://
+phuker.github.io/). The fonts are optimized for contents in Simplified Chinese.
+## Features ### Generated HTML The principle is: keep it simple. - All-in-one
+single HTML file - Completely offline, no CDN, no web fonts - No JavaScript ###
+Markdown syntax This is a Markdown dialect, similar but different from [GitHub
+Flavored Markdown (GFM)](https://github.github.com/gfm/). Default enabled
+Markdown features: - [Extra](https://python-markdown.github.io/extensions/
+extra/) extensions - [CodeHilite](https://python-markdown.github.io/extensions/
+code_hilite/) - [Table of Contents](https://python-markdown.github.io/
+extensions/toc/) - [New Line to Break](https://python-markdown.github.io/
+extensions/nl2br/) - [Admonition](https://python-markdown.github.io/extensions/
+admonition/) - ` - Part of GitHub Flavored Markdown For details, see `convert
+()` function of `md2html/__init__.py`, and the demo below. ## Demo - Default
+style: [docs/demo-default.html](https://phuker.github.io/md2html/demo-
+default.html) - With addon `--style sidebar-toc`: [docs/demo-sidebar-toc.html]
+(https://phuker.github.io/md2html/demo-sidebar-toc.html) - With addon `--style
+dark`: [docs/demo-dark.html](https://phuker.github.io/md2html/demo-dark.html) -
+With addon `--style sidebar-toc --style dark`: [docs/demo-sidebar-toc-
+dark.html](https://phuker.github.io/md2html/demo-sidebar-toc-dark.html) All
+above files are generated from [docs/demo.md](./docs/demo.md). You can view its
+content to see supported syntax. ## Requirements - Python >= `3.6`, with `pip`
+installed ## Install ```bash python3 -m pip install -U md2html-phuker ``` There
+are too many similar projects with similar names in PyPI, `md2html`, `md-to-
+html`, `markdown2html`, `markdown-to-html`, `mrkdwn2html` ... I have to add a
+suffix to keep away from this war of naming. ## Usage ### Show help ```console
+$ md2html --help usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--
+style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--
+body-insert HTML] [--body-append HTML] [input_file] Yet another markdown to
+html converter, generate an offline all-in-one single HTML file. positional
+arguments: input_file If omitted or "-", use stdin. options: -h, --help show
+this help message and exit -v, --verbose Verbose output -V, --version Output
+version info and exit -t TITLE, --title TITLE If omitted, generate from input
+filename -f, --force Force overwrite if output file exists -o FILE, --output-
+file FILE If omitted, auto decide. If "-", stdout. --style PRESET Preset style
+addons, choices: sidebar-toc, dark --append-css FILE Append embedded CSS files,
+may specify multiple times. --head-insert HTML HTML to insert to the start of
 , may specify multiple times. --head-append HTML HTML to append to the end of
 , may specify multiple times. --body-insert HTML HTML to insert to the start of
 , may specify multiple times. --body-append HTML HTML to append to the end of
 , may specify multiple times. ``` If you are not sure about what will happen if
 you combine `[-o FILE]`, `[input_file]` and `[-t TITLE]`, see `test.py`, which
 contains tens of input cases and their intended behaviors. ### Convert a file
 Generate `foo.html` in the same dir, with HTML title `foo`: ```bash md2html
```

### Comparing `md2html-phuker-0.4.2/md2html/github-markdown.css` & `md2html-phuker-0.5.0/md2html/github-markdown.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.4.2/md2html/main.css` & `md2html-phuker-0.5.0/md2html/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 .markdown-body h3:hover a.headerlink,
 .markdown-body h4:hover a.headerlink,
 .markdown-body h5:hover a.headerlink,
 .markdown-body h6:hover a.headerlink {
     visibility: visible;
 }
 
+.markdown-body img.inline {
+    display: inline;
+    vertical-align: text-bottom;
+    max-height: 2em;
+}
+
 /* 
 Admonition alerts
 Modified from Bootstrap v4.5.2 CSS .alert
 */
 .admonition {
     position: relative;
     padding: 0.5em 1.5em;
```

### Comparing `md2html-phuker-0.4.2/md2html/pygments.css` & `md2html-phuker-0.5.0/md2html/pygments.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.4.2/md2html/style-dark.css` & `md2html-phuker-0.5.0/md2html/style-dark.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.4.2/md2html_phuker.egg-info/PKG-INFO` & `md2html-phuker-0.5.0/md2html_phuker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.4.2
+Version: 0.5.0
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [Project homepage](https://github.com/Phuker/md2html)
 
 [Readme](https://github.com/Phuker/md2html/blob/main/Readme.md)
-
-
```

### Comparing `md2html-phuker-0.4.2/setup.py` & `md2html-phuker-0.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 with open('Readme.PyPI.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='md2html-phuker',
     description='Yet another markdown to html converter, generate an offline all-in-one single HTML file.',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     author='Phuker',
     author_email='Phuker@users.noreply.github.com',
     url='https://github.com/Phuker/md2html',
     license='GNU General Public License v3.0',
     keywords='markdown html convert',
     packages=['md2html'],
     py_modules = [],
     package_data={
-        "md2html": ["*.css"],
+        'md2html': ['*.css'],
     },
     entry_points={
         'console_scripts': [
             'md2html=md2html:main'
         ]
     },
     install_requires=[
         'markdown>=3',
         'pygments',
-        'css-html-js-minify',
         'markdown-link-attr-modifier >= 0.2.0',
         'py-gfm',
     ],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Environment :: Console',
         'Programming Language :: Python :: 3',
```

