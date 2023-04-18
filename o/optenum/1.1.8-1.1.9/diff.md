# Comparing `tmp/optenum-1.1.8.tar.gz` & `tmp/optenum-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optenum-1.1.8.tar", last modified: Tue Nov  8 17:11:36 2022, max compression
+gzip compressed data, was "optenum-1.1.9.tar", last modified: Tue Apr 18 02:40:38 2023, max compression
```

## Comparing `optenum-1.1.8.tar` & `optenum-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2022-11-08 17:11:36.000000 optenum-1.1.8/
--rw-r--r--   0 samuel     (501) staff       (20)     1091 2019-04-03 09:42:21.000000 optenum-1.1.8/LICENSE
--rw-r--r--   0 samuel     (501) staff       (20)      130 2019-04-03 09:29:59.000000 optenum-1.1.8/MANIFEST.in
--rw-r--r--   0 samuel     (501) staff       (20)    12084 2022-11-08 17:11:36.000000 optenum-1.1.8/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)    10940 2019-06-03 15:07:26.000000 optenum-1.1.8/README.md
--rw-r--r--   0 samuel     (501) staff       (20)      928 2022-11-08 17:10:30.000000 optenum-1.1.8/RELEASENOTE.md
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum/
--rw-r--r--   0 samuel     (501) staff       (20)     1450 2019-06-03 15:07:26.000000 optenum-1.1.8/optenum/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)      442 2019-06-03 15:07:26.000000 optenum-1.1.8/optenum/mysix.py
--rw-r--r--   0 samuel     (501) staff       (20)     3960 2022-11-08 16:54:09.000000 optenum-1.1.8/optenum/option.py
--rw-r--r--   0 samuel     (501) staff       (20)    11641 2019-05-29 08:08:04.000000 optenum-1.1.8/optenum/option.v1.py
--rw-r--r--   0 samuel     (501) staff       (20)    12624 2022-11-08 16:55:45.000000 optenum-1.1.8/optenum/options.py
--rw-r--r--   0 samuel     (501) staff       (20)       44 2022-11-08 17:08:26.000000 optenum-1.1.8/optenum/version.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/
--rw-r--r--   0 samuel     (501) staff       (20)    12084 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)      355 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/SOURCES.txt
--rw-r--r--   0 samuel     (501) staff       (20)        1 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/dependency_links.txt
--rw-r--r--   0 samuel     (501) staff       (20)       20 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/entry_points.txt
--rw-r--r--   0 samuel     (501) staff       (20)       43 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/requires.txt
--rw-r--r--   0 samuel     (501) staff       (20)        8 2022-11-08 17:11:36.000000 optenum-1.1.8/optenum.egg-info/top_level.txt
--rw-r--r--   0 samuel     (501) staff       (20)       38 2022-11-08 17:11:36.000000 optenum-1.1.8/setup.cfg
--rw-r--r--   0 samuel     (501) staff       (20)     9313 2019-05-29 08:08:04.000000 optenum-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:40:38.667024 optenum-1.1.9/
+-rw-rw-rw-   0        0        0     1112 2023-04-18 02:35:06.000000 optenum-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-04-18 02:35:06.000000 optenum-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12399 2023-04-18 02:40:38.666023 optenum-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11263 2023-04-18 02:35:06.000000 optenum-1.1.9/README.md
+-rw-rw-rw-   0        0        0      972 2023-04-18 02:35:06.000000 optenum-1.1.9/RELEASENOTE.md
+drwxrwxrwx   0        0        0        0 2023-04-18 02:40:38.657027 optenum-1.1.9/optenum/
+-rw-rw-rw-   0        0        0     1483 2023-04-18 02:35:06.000000 optenum-1.1.9/optenum/__init__.py
+-rw-rw-rw-   0        0        0      462 2023-04-18 02:35:06.000000 optenum-1.1.9/optenum/mysix.py
+-rw-rw-rw-   0        0        0     4076 2023-04-18 02:35:06.000000 optenum-1.1.9/optenum/option.py
+-rw-rw-rw-   0        0        0    11984 2023-04-18 02:35:06.000000 optenum-1.1.9/optenum/option.v1.py
+-rw-rw-rw-   0        0        0    13064 2023-04-18 02:37:15.000000 optenum-1.1.9/optenum/options.py
+-rw-rw-rw-   0        0        0       47 2023-04-18 02:38:59.000000 optenum-1.1.9/optenum/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:40:38.661023 optenum-1.1.9/optenum.egg-info/
+-rw-rw-rw-   0        0        0    12399 2023-04-18 02:40:38.000000 optenum-1.1.9/optenum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-04-18 02:40:38.000000 optenum-1.1.9/optenum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:40:38.000000 optenum-1.1.9/optenum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-18 02:40:38.000000 optenum-1.1.9/optenum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 02:40:38.000000 optenum-1.1.9/optenum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:40:38.667024 optenum-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     9534 2023-04-18 02:35:06.000000 optenum-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:40:38.664027 optenum-1.1.9/tests/
+-rw-rw-rw-   0        0        0    15903 2023-04-18 02:35:06.000000 optenum-1.1.9/tests/test_option.py
+-rw-rw-rw-   0        0        0    10731 2023-04-18 02:35:06.000000 optenum-1.1.9/tests/test_options_customized.py
+-rw-rw-rw-   0        0        0      959 2023-04-18 02:35:06.000000 optenum-1.1.9/tests/test_others.py
```

### Comparing `optenum-1.1.8/LICENSE` & `optenum-1.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Samuel Chen <me(at)samuelchen.net>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Samuel Chen <me(at)samuelchen.net>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `optenum-1.1.8/PKG-INFO` & `optenum-1.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,354 +1,351 @@
-Metadata-Version: 2.1
-Name: optenum
-Version: 1.1.8
-Summary: A missing Python Option/Enum library
-Home-page: http://en.samuelchen.net/project/optenum/
-Author: Samuel Chen
-Author-email: samuel.net@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/samuelchen/optenum/issues
-Project-URL: Source, https://github.com/samuelchen/optenum
-Keywords: enum library development
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
-# Optenum
-
-[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
-[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-
-
-	
-A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
-
-Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
-
-Compatible with `Python 2.7+` and `Python 3.0+`.
-
-# Install
-
-Python 3.x, 2.7
-
-```bash
-pip install optenum
-```
-
-For those probably missing `six` module:
-
-```bash
-pip install six optenum
-```
-
-# Quick start
-
-1. Simple as Enum type
-
-    Says we define a simple enum:
-    
-    ```python
-    from optenum import Options
- 
-    class Fruit(Options):
-        APPLE = 1
-        ORANGE = 2
-        BANANA = 3 
-    ```
-    
-    Try the following in Python command line:
-    
-    ```
-    >>> from optenum import Option, Options
-    >>> class Fruit(Options):
-    ...     APPLE = 1
-    ...     ORANGE = 2
-    ...     BANANA = 3
-    >>> 
-    >>> Fruit.APPLE
-    <Option code=1 name=APPLE text=None>
-    >>> print(Fruit.APPLE)
-    1
-    >>> Fruit.APPLE.code
-    1
-    >>> Fruit.APPLE.name
-    'APPLE'
-    >>> Fruit.APPLE.text
-    >>> print(Fruit.APPLE.text)
-    None
-    >>> Fruit.APPLE.get_text()
-    'apple'
-    
-    ```
-
-2. Complex declaration
-
-    You may declare your Options (Enums) in many annotations.
-
-    ```python
-    from optenum import Option, Options
- 
-    class EnumCellPhone(Options):
-        APPLE = 1
-        SAMSUNG = Option(2, name='SAMSUNG')
-        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
-    
-    
-    class DoorState(Options):
-        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
-        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
-        IN_OPENING = 'IO'
-        IN_CLOSING = 'IC'
-    
-        _FLAG = False           # underscore leading name is not an option
-        x = lambda y: y         # function/callable is not an option
-    ```
-
-3. Operators
-
-    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
-    
-    ```
-    >>> class Favorite(Options):
-    ...     APPLE = 1
-    ...     BANANA = 3, 'Banana hot'
-    ... 
-    >>> 
-    >>> Fruit.APPLE == Favorite.APPLE
-    True
-    >>> Fruit.BANANA == Favorite.BANANA
-    False
-    >>> Fruit.APPLE + 1 == Fruit.ORANGE
-    True>>> Fruit.BANANA >> 2
-    0
-    >>> Fruit.BANANA << 2
-    12>>> Fruit.BANANA > Favorite.APPLE
-    True
-    ```
-
-4. Collections
-
-    `Options` provides some collections for accessing option and it's fields.
-    See section "Collections for Options" below for more information.
-    
-    ```
-    >>> Fruit.codes
-    [1, 2, 3]
-    >>> Fruit.names
-    ['ORANGE', 'APPLE', 'BANANA']
-    >>> Fruit.all
-    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
-    >>> Fruit.tuples
-    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
-    >>> Favorite.items
-    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
-    >>> Favorite.get_list('code','text')
-    [(1, None), (3, 'Banana hot')]
-    >>> Favorite.get_dict('name','text')
-    {'APPLE': None, 'BANANA': 'Banana hot'}
-    
-    ```
-
-5. Django model choices
-
-        To be written
-
-# Background
-
-Often we need to define some enums or options. But looks python missing this class.
-Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
-
-For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
-
-```python
-class MyOption(object):
-    foo = 1
-    bar = 2
-```
-But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
-
-Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
-
-# Features
-
-  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
-  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
-  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
-  * List - Retrieve list of code, name or text `[0, 1, -1]`
-  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
-  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
-  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
-  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
-  * Access **name**, **text** by **code**
-  * Lookup enum/option by **name**, **code**
-  
-# Guide / Tutor
-
-# Type converting for `Option`
-
-    since v1.1.1
-
-An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
-`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
-
-For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
-The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
-an `Option(str)` class will be constructed internally.
-
-The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
-`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
- `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
- your option as its value(`code`) is such in `dict` as key and so on.
- 
-
-    Deprecated since v1.1.0
-    
-    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
-    
-    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
-    
-    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
-
-# Boolean for `Option`
-
-    Deprecated since v1.1.0
-    No special implementation. It behaves as `object` is.
-
-# Group and tags 
-
-See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
-
-# Operators for `Option`
-
-Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
-
-    Deprecated since v1.1.0
-    
-    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
-    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
-    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
-    directly reference to its real value.
-    
-    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
-
-# Collections for `Options`
-
-Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
-equals to `Option.FOO`.
-
-We could also access the following collections from within an Options class. 
-
-  * `Options.codes` - list of codes
-    
-  * `Options.names` - list of names
-  
-  * `Options.all` - list of options
-
-  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
-
-  * `Options.items` - dict of {`name`: `Option`} mapping
-
-  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
-  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
-  
-  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
-  `key_field` specify which Option field is key such as `name`, `code`. 
-  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
-  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
-
-    Deprecated since v1.1.0
-    
-    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
-    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
-    If you want to check if name in `Options`), use collection instead. 
-    e.g. `if 'APPLE' in Fruit.names`.
-
-
-# Configuration
-
-Some flags can be used to make some simple configuration to your Options.
-
-  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
-  
-    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
-    functions. The following example is valid definition.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        _flag = False
-        
-        def switch(self):
-            pass
-    ```
-    
-    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Invalid Option name. Exception raised.
-    ```
-    
-    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
-    But to be noticed, it still not an `Option`.
-  
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        __IGNORE_INVALID_NAME__ = True
-        
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Exception ignored. But still not an Option.
-    ```
-  
-  * `__ORDER_BY__`
-  
-        Not supported yet
-
-# FAQ
-
-* Why not use *namedtuple* ?
-
-*namedtuple* is also a good way to define enum/options. But it has not enough features
-you may required such as *collection*, *operator*, *compare*, *text* and so on.
-
-* Why only uppercase allowed for Option name ?
-
-Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
-And enumerations commonly are defined with uppercase identifier.
-
-# Contributors
-
-List of contributors:
-
-* Samuel Chen - The project owner and maintainer.
-
+Metadata-Version: 2.1
+Name: optenum
+Version: 1.1.9
+Summary: A missing Python Option/Enum library
+Home-page: http://en.samuelchen.net/project/optenum/
+Author: Samuel Chen
+Author-email: samuel.net@gmail.com
+Project-URL: Bug Reports, https://github.com/samuelchen/optenum/issues
+Project-URL: Source, https://github.com/samuelchen/optenum
+Keywords: enum library development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+# Optenum
+
+[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
+[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+
+
+	
+A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
+
+Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
+
+Compatible with `Python 2.7+` and `Python 3.0+`.
+
+# Install
+
+Python 3.x, 2.7
+
+```bash
+pip install optenum
+```
+
+For those probably missing `six` module:
+
+```bash
+pip install six optenum
+```
+
+# Quick start
+
+1. Simple as Enum type
+
+    Says we define a simple enum:
+    
+    ```python
+    from optenum import Options
+ 
+    class Fruit(Options):
+        APPLE = 1
+        ORANGE = 2
+        BANANA = 3 
+    ```
+    
+    Try the following in Python command line:
+    
+    ```
+    >>> from optenum import Option, Options
+    >>> class Fruit(Options):
+    ...     APPLE = 1
+    ...     ORANGE = 2
+    ...     BANANA = 3
+    >>> 
+    >>> Fruit.APPLE
+    <Option code=1 name=APPLE text=None>
+    >>> print(Fruit.APPLE)
+    1
+    >>> Fruit.APPLE.code
+    1
+    >>> Fruit.APPLE.name
+    'APPLE'
+    >>> Fruit.APPLE.text
+    >>> print(Fruit.APPLE.text)
+    None
+    >>> Fruit.APPLE.get_text()
+    'apple'
+    
+    ```
+
+2. Complex declaration
+
+    You may declare your Options (Enums) in many annotations.
+
+    ```python
+    from optenum import Option, Options
+ 
+    class EnumCellPhone(Options):
+        APPLE = 1
+        SAMSUNG = Option(2, name='SAMSUNG')
+        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
+    
+    
+    class DoorState(Options):
+        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
+        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
+        IN_OPENING = 'IO'
+        IN_CLOSING = 'IC'
+    
+        _FLAG = False           # underscore leading name is not an option
+        x = lambda y: y         # function/callable is not an option
+    ```
+
+3. Operators
+
+    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
+    
+    ```
+    >>> class Favorite(Options):
+    ...     APPLE = 1
+    ...     BANANA = 3, 'Banana hot'
+    ... 
+    >>> 
+    >>> Fruit.APPLE == Favorite.APPLE
+    True
+    >>> Fruit.BANANA == Favorite.BANANA
+    False
+    >>> Fruit.APPLE + 1 == Fruit.ORANGE
+    True>>> Fruit.BANANA >> 2
+    0
+    >>> Fruit.BANANA << 2
+    12>>> Fruit.BANANA > Favorite.APPLE
+    True
+    ```
+
+4. Collections
+
+    `Options` provides some collections for accessing option and it's fields.
+    See section "Collections for Options" below for more information.
+    
+    ```
+    >>> Fruit.codes
+    [1, 2, 3]
+    >>> Fruit.names
+    ['ORANGE', 'APPLE', 'BANANA']
+    >>> Fruit.all
+    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
+    >>> Fruit.tuples
+    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
+    >>> Favorite.items
+    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
+    >>> Favorite.get_list('code','text')
+    [(1, None), (3, 'Banana hot')]
+    >>> Favorite.get_dict('name','text')
+    {'APPLE': None, 'BANANA': 'Banana hot'}
+    
+    ```
+
+5. Django model choices
+
+        To be written
+
+# Background
+
+Often we need to define some enums or options. But looks python missing this class.
+Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
+
+For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
+
+```python
+class MyOption(object):
+    foo = 1
+    bar = 2
+```
+But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
+
+Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
+
+# Features
+
+  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
+  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
+  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
+  * List - Retrieve list of code, name or text `[0, 1, -1]`
+  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
+  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
+  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
+  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
+  * Access **name**, **text** by **code**
+  * Lookup enum/option by **name**, **code**
+  
+# Guide / Tutor
+
+# Type converting for `Option`
+
+    since v1.1.1
+
+An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
+`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
+
+For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
+The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
+an `Option(str)` class will be constructed internally.
+
+The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
+`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
+ `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
+ your option as its value(`code`) is such in `dict` as key and so on.
+ 
+
+    Deprecated since v1.1.0
+    
+    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
+    
+    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
+    
+    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
+
+# Boolean for `Option`
+
+    Deprecated since v1.1.0
+    No special implementation. It behaves as `object` is.
+
+# Group and tags 
+
+See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
+
+# Operators for `Option`
+
+Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
+
+    Deprecated since v1.1.0
+    
+    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
+    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
+    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
+    directly reference to its real value.
+    
+    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
+
+# Collections for `Options`
+
+Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
+equals to `Option.FOO`.
+
+We could also access the following collections from within an Options class. 
+
+  * `Options.codes` - list of codes
+    
+  * `Options.names` - list of names
+  
+  * `Options.all` - list of options
+
+  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
+
+  * `Options.items` - dict of {`name`: `Option`} mapping
+
+  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
+  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
+  
+  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
+  `key_field` specify which Option field is key such as `name`, `code`. 
+  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
+  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
+
+    Deprecated since v1.1.0
+    
+    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
+    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
+    If you want to check if name in `Options`), use collection instead. 
+    e.g. `if 'APPLE' in Fruit.names`.
+
+
+# Configuration
+
+Some flags can be used to make some simple configuration to your Options.
+
+  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
+  
+    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
+    functions. The following example is valid definition.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        _flag = False
+        
+        def switch(self):
+            pass
+    ```
+    
+    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Invalid Option name. Exception raised.
+    ```
+    
+    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
+    But to be noticed, it still not an `Option`.
+  
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        __IGNORE_INVALID_NAME__ = True
+        
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Exception ignored. But still not an Option.
+    ```
+  
+  * `__ORDER_BY__`
+  
+        Not supported yet
+
+# FAQ
+
+* Why not use *namedtuple* ?
+
+*namedtuple* is also a good way to define enum/options. But it has not enough features
+you may required such as *collection*, *operator*, *compare*, *text* and so on.
+
+* Why only uppercase allowed for Option name ?
+
+Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
+And enumerations commonly are defined with uppercase identifier.
+
+# Contributors
+
+List of contributors:
+
+* Samuel Chen - The project owner and maintainer.
```

### Comparing `optenum-1.1.8/README.md` & `optenum-1.1.9/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-# Optenum
-
-[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
-[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-
-
-	
-A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
-
-Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
-
-Compatible with `Python 2.7+` and `Python 3.0+`.
-
-# Install
-
-Python 3.x, 2.7
-
-```bash
-pip install optenum
-```
-
-For those probably missing `six` module:
-
-```bash
-pip install six optenum
-```
-
-# Quick start
-
-1. Simple as Enum type
-
-    Says we define a simple enum:
-    
-    ```python
-    from optenum import Options
- 
-    class Fruit(Options):
-        APPLE = 1
-        ORANGE = 2
-        BANANA = 3 
-    ```
-    
-    Try the following in Python command line:
-    
-    ```
-    >>> from optenum import Option, Options
-    >>> class Fruit(Options):
-    ...     APPLE = 1
-    ...     ORANGE = 2
-    ...     BANANA = 3
-    >>> 
-    >>> Fruit.APPLE
-    <Option code=1 name=APPLE text=None>
-    >>> print(Fruit.APPLE)
-    1
-    >>> Fruit.APPLE.code
-    1
-    >>> Fruit.APPLE.name
-    'APPLE'
-    >>> Fruit.APPLE.text
-    >>> print(Fruit.APPLE.text)
-    None
-    >>> Fruit.APPLE.get_text()
-    'apple'
-    
-    ```
-
-2. Complex declaration
-
-    You may declare your Options (Enums) in many annotations.
-
-    ```python
-    from optenum import Option, Options
- 
-    class EnumCellPhone(Options):
-        APPLE = 1
-        SAMSUNG = Option(2, name='SAMSUNG')
-        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
-    
-    
-    class DoorState(Options):
-        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
-        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
-        IN_OPENING = 'IO'
-        IN_CLOSING = 'IC'
-    
-        _FLAG = False           # underscore leading name is not an option
-        x = lambda y: y         # function/callable is not an option
-    ```
-
-3. Operators
-
-    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
-    
-    ```
-    >>> class Favorite(Options):
-    ...     APPLE = 1
-    ...     BANANA = 3, 'Banana hot'
-    ... 
-    >>> 
-    >>> Fruit.APPLE == Favorite.APPLE
-    True
-    >>> Fruit.BANANA == Favorite.BANANA
-    False
-    >>> Fruit.APPLE + 1 == Fruit.ORANGE
-    True>>> Fruit.BANANA >> 2
-    0
-    >>> Fruit.BANANA << 2
-    12>>> Fruit.BANANA > Favorite.APPLE
-    True
-    ```
-
-4. Collections
-
-    `Options` provides some collections for accessing option and it's fields.
-    See section "Collections for Options" below for more information.
-    
-    ```
-    >>> Fruit.codes
-    [1, 2, 3]
-    >>> Fruit.names
-    ['ORANGE', 'APPLE', 'BANANA']
-    >>> Fruit.all
-    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
-    >>> Fruit.tuples
-    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
-    >>> Favorite.items
-    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
-    >>> Favorite.get_list('code','text')
-    [(1, None), (3, 'Banana hot')]
-    >>> Favorite.get_dict('name','text')
-    {'APPLE': None, 'BANANA': 'Banana hot'}
-    
-    ```
-
-5. Django model choices
-
-        To be written
-
-# Background
-
-Often we need to define some enums or options. But looks python missing this class.
-Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
-
-For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
-
-```python
-class MyOption(object):
-    foo = 1
-    bar = 2
-```
-But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
-
-Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
-
-# Features
-
-  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
-  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
-  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
-  * List - Retrieve list of code, name or text `[0, 1, -1]`
-  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
-  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
-  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
-  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
-  * Access **name**, **text** by **code**
-  * Lookup enum/option by **name**, **code**
-  
-# Guide / Tutor
-
-# Type converting for `Option`
-
-    since v1.1.1
-
-An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
-`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
-
-For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
-The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
-an `Option(str)` class will be constructed internally.
-
-The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
-`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
- `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
- your option as its value(`code`) is such in `dict` as key and so on.
- 
-
-    Deprecated since v1.1.0
-    
-    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
-    
-    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
-    
-    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
-
-# Boolean for `Option`
-
-    Deprecated since v1.1.0
-    No special implementation. It behaves as `object` is.
-
-# Group and tags 
-
-See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
-
-# Operators for `Option`
-
-Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
-
-    Deprecated since v1.1.0
-    
-    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
-    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
-    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
-    directly reference to its real value.
-    
-    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
-
-# Collections for `Options`
-
-Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
-equals to `Option.FOO`.
-
-We could also access the following collections from within an Options class. 
-
-  * `Options.codes` - list of codes
-    
-  * `Options.names` - list of names
-  
-  * `Options.all` - list of options
-
-  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
-
-  * `Options.items` - dict of {`name`: `Option`} mapping
-
-  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
-  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
-  
-  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
-  `key_field` specify which Option field is key such as `name`, `code`. 
-  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
-  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
-
-    Deprecated since v1.1.0
-    
-    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
-    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
-    If you want to check if name in `Options`), use collection instead. 
-    e.g. `if 'APPLE' in Fruit.names`.
-
-
-# Configuration
-
-Some flags can be used to make some simple configuration to your Options.
-
-  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
-  
-    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
-    functions. The following example is valid definition.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        _flag = False
-        
-        def switch(self):
-            pass
-    ```
-    
-    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Invalid Option name. Exception raised.
-    ```
-    
-    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
-    But to be noticed, it still not an `Option`.
-  
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        __IGNORE_INVALID_NAME__ = True
-        
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Exception ignored. But still not an Option.
-    ```
-  
-  * `__ORDER_BY__`
-  
-        Not supported yet
-
-# FAQ
-
-* Why not use *namedtuple* ?
-
-*namedtuple* is also a good way to define enum/options. But it has not enough features
-you may required such as *collection*, *operator*, *compare*, *text* and so on.
-
-* Why only uppercase allowed for Option name ?
-
-Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
-And enumerations commonly are defined with uppercase identifier.
-
-# Contributors
-
-List of contributors:
-
+# Optenum
+
+[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
+[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+
+
+	
+A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
+
+Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
+
+Compatible with `Python 2.7+` and `Python 3.0+`.
+
+# Install
+
+Python 3.x, 2.7
+
+```bash
+pip install optenum
+```
+
+For those probably missing `six` module:
+
+```bash
+pip install six optenum
+```
+
+# Quick start
+
+1. Simple as Enum type
+
+    Says we define a simple enum:
+    
+    ```python
+    from optenum import Options
+ 
+    class Fruit(Options):
+        APPLE = 1
+        ORANGE = 2
+        BANANA = 3 
+    ```
+    
+    Try the following in Python command line:
+    
+    ```
+    >>> from optenum import Option, Options
+    >>> class Fruit(Options):
+    ...     APPLE = 1
+    ...     ORANGE = 2
+    ...     BANANA = 3
+    >>> 
+    >>> Fruit.APPLE
+    <Option code=1 name=APPLE text=None>
+    >>> print(Fruit.APPLE)
+    1
+    >>> Fruit.APPLE.code
+    1
+    >>> Fruit.APPLE.name
+    'APPLE'
+    >>> Fruit.APPLE.text
+    >>> print(Fruit.APPLE.text)
+    None
+    >>> Fruit.APPLE.get_text()
+    'apple'
+    
+    ```
+
+2. Complex declaration
+
+    You may declare your Options (Enums) in many annotations.
+
+    ```python
+    from optenum import Option, Options
+ 
+    class EnumCellPhone(Options):
+        APPLE = 1
+        SAMSUNG = Option(2, name='SAMSUNG')
+        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
+    
+    
+    class DoorState(Options):
+        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
+        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
+        IN_OPENING = 'IO'
+        IN_CLOSING = 'IC'
+    
+        _FLAG = False           # underscore leading name is not an option
+        x = lambda y: y         # function/callable is not an option
+    ```
+
+3. Operators
+
+    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
+    
+    ```
+    >>> class Favorite(Options):
+    ...     APPLE = 1
+    ...     BANANA = 3, 'Banana hot'
+    ... 
+    >>> 
+    >>> Fruit.APPLE == Favorite.APPLE
+    True
+    >>> Fruit.BANANA == Favorite.BANANA
+    False
+    >>> Fruit.APPLE + 1 == Fruit.ORANGE
+    True>>> Fruit.BANANA >> 2
+    0
+    >>> Fruit.BANANA << 2
+    12>>> Fruit.BANANA > Favorite.APPLE
+    True
+    ```
+
+4. Collections
+
+    `Options` provides some collections for accessing option and it's fields.
+    See section "Collections for Options" below for more information.
+    
+    ```
+    >>> Fruit.codes
+    [1, 2, 3]
+    >>> Fruit.names
+    ['ORANGE', 'APPLE', 'BANANA']
+    >>> Fruit.all
+    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
+    >>> Fruit.tuples
+    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
+    >>> Favorite.items
+    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
+    >>> Favorite.get_list('code','text')
+    [(1, None), (3, 'Banana hot')]
+    >>> Favorite.get_dict('name','text')
+    {'APPLE': None, 'BANANA': 'Banana hot'}
+    
+    ```
+
+5. Django model choices
+
+        To be written
+
+# Background
+
+Often we need to define some enums or options. But looks python missing this class.
+Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
+
+For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
+
+```python
+class MyOption(object):
+    foo = 1
+    bar = 2
+```
+But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
+
+Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
+
+# Features
+
+  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
+  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
+  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
+  * List - Retrieve list of code, name or text `[0, 1, -1]`
+  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
+  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
+  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
+  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
+  * Access **name**, **text** by **code**
+  * Lookup enum/option by **name**, **code**
+  
+# Guide / Tutor
+
+# Type converting for `Option`
+
+    since v1.1.1
+
+An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
+`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
+
+For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
+The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
+an `Option(str)` class will be constructed internally.
+
+The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
+`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
+ `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
+ your option as its value(`code`) is such in `dict` as key and so on.
+ 
+
+    Deprecated since v1.1.0
+    
+    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
+    
+    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
+    
+    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
+
+# Boolean for `Option`
+
+    Deprecated since v1.1.0
+    No special implementation. It behaves as `object` is.
+
+# Group and tags 
+
+See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
+
+# Operators for `Option`
+
+Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
+
+    Deprecated since v1.1.0
+    
+    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
+    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
+    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
+    directly reference to its real value.
+    
+    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
+
+# Collections for `Options`
+
+Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
+equals to `Option.FOO`.
+
+We could also access the following collections from within an Options class. 
+
+  * `Options.codes` - list of codes
+    
+  * `Options.names` - list of names
+  
+  * `Options.all` - list of options
+
+  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
+
+  * `Options.items` - dict of {`name`: `Option`} mapping
+
+  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
+  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
+  
+  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
+  `key_field` specify which Option field is key such as `name`, `code`. 
+  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
+  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
+
+    Deprecated since v1.1.0
+    
+    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
+    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
+    If you want to check if name in `Options`), use collection instead. 
+    e.g. `if 'APPLE' in Fruit.names`.
+
+
+# Configuration
+
+Some flags can be used to make some simple configuration to your Options.
+
+  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
+  
+    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
+    functions. The following example is valid definition.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        _flag = False
+        
+        def switch(self):
+            pass
+    ```
+    
+    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Invalid Option name. Exception raised.
+    ```
+    
+    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
+    But to be noticed, it still not an `Option`.
+  
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        __IGNORE_INVALID_NAME__ = True
+        
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Exception ignored. But still not an Option.
+    ```
+  
+  * `__ORDER_BY__`
+  
+        Not supported yet
+
+# FAQ
+
+* Why not use *namedtuple* ?
+
+*namedtuple* is also a good way to define enum/options. But it has not enough features
+you may required such as *collection*, *operator*, *compare*, *text* and so on.
+
+* Why only uppercase allowed for Option name ?
+
+Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
+And enumerations commonly are defined with uppercase identifier.
+
+# Contributors
+
+List of contributors:
+
 * Samuel Chen - The project owner and maintainer.
```

### Comparing `optenum-1.1.8/RELEASENOTE.md` & `optenum-1.1.9/RELEASENOTE.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-
-# v1.1.8
-
-* Do not convert Option.text to string. It may cause `gettext_lazy` executed so that some times error occurs in Django.
-
-# v1.1.7
-
-* (lost information)
-
-# v1.1.6
-
-* Group supports +(plus) operator
-
-# v1.1.5
-
-* Fix issue of creating single option group as class attribute
-
-# v1.1.4
-
-* Fix option not found issue when creating option group as class attribute (class attributes creation is not in order)
-* Fix option attributes order in python 3.4 & 3.5
-
-# v1.1.3
-
-* Tagged option group support construct as class attribute and support +, -
-* fix "random ordered options in group" issue
-* fix "tag name checking" issue
-
-# v1.1.2
-
-* Support Option tags 
-* Support access tagged options as group (tuple)
-* fix "Option.get_text is missed" issue.
-
-# v1.1.1
-
-* Fix issue that `__IGNORE_INVALID_NAME__` does not work.
-
-# v1.1.0
-
-* Change `Option` to make its instance object same as its `code`. 
-
-# v1.0.0
-
+
+# v1.1.8
+
+* Do not convert Option.text to string. It may cause `gettext_lazy` executed so that some times error occurs in Django.
+
+# v1.1.7
+
+* (lost information)
+
+# v1.1.6
+
+* Group supports +(plus) operator
+
+# v1.1.5
+
+* Fix issue of creating single option group as class attribute
+
+# v1.1.4
+
+* Fix option not found issue when creating option group as class attribute (class attributes creation is not in order)
+* Fix option attributes order in python 3.4 & 3.5
+
+# v1.1.3
+
+* Tagged option group support construct as class attribute and support +, -
+* fix "random ordered options in group" issue
+* fix "tag name checking" issue
+
+# v1.1.2
+
+* Support Option tags 
+* Support access tagged options as group (tuple)
+* fix "Option.get_text is missed" issue.
+
+# v1.1.1
+
+* Fix issue that `__IGNORE_INVALID_NAME__` does not work.
+
+# v1.1.0
+
+* Change `Option` to make its instance object same as its `code`. 
+
+# v1.0.0
+
 * General Available
```

### Comparing `optenum-1.1.8/optenum/__init__.py` & `optenum-1.1.9/optenum/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-optenum
-==========
-
-A missing python Enum/option lib supports enum code, name, text, even (code, name) tuple list and so on.
-
-Compatible with Python 2.7+ and Python 3.0+.
-
-Features:
-
-  * Code - Enumration/option by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
-  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access.
-  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped')
-  * List - Retrieve list of code, name or text `[0, 1, -1]`
-  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
-  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
-  * Grouping - Group a set of enums/options. e.g. IN_PROGERSS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
-  * Access **name**, **text** by **code**
-  * Lookup enum/option by **name**, **code**
-
-"""
-
-from __future__ import absolute_import
-from .version import __version__
-from .option import Option
-from .options import Options, OptionGroup
-
-__all__ = ('Option', 'Options', 'OptionGroup' '__version__')
-
-__copyright__ = "Copyright (c) 2019 Samuel Chen (Chen Wei)"
-__license__ = "MIT"
-__summary__ = "A missing python Enum/option lib supports enum code, name, text, even (code, name) tuple list and so on."
-__uri__ = "https://github.com/samuelchen/optenum.git"
+"""
+optenum
+==========
+
+A missing python Enum/option lib supports enum code, name, text, even (code, name) tuple list and so on.
+
+Compatible with Python 2.7+ and Python 3.0+.
+
+Features:
+
+  * Code - Enumration/option by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
+  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access.
+  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped')
+  * List - Retrieve list of code, name or text `[0, 1, -1]`
+  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
+  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
+  * Grouping - Group a set of enums/options. e.g. IN_PROGERSS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
+  * Access **name**, **text** by **code**
+  * Lookup enum/option by **name**, **code**
+
+"""
+
+from __future__ import absolute_import
+from .version import __version__
+from .option import Option
+from .options import Options, OptionGroup
+
+__all__ = ('Option', 'Options', 'OptionGroup' '__version__')
+
+__copyright__ = "Copyright (c) 2019 Samuel Chen (Chen Wei)"
+__license__ = "MIT"
+__summary__ = "A missing python Enum/option lib supports enum code, name, text, even (code, name) tuple list and so on."
+__uri__ = "https://github.com/samuelchen/optenum.git"
```

### Comparing `optenum-1.1.8/optenum/option.py` & `optenum-1.1.9/optenum/option.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""
-Option class represents a single option in a list of options/enum
-"""
-import six
-from .mysix import is_identifier
-
-NUMBER_TYPES = six.integer_types + (float,)
-DATE_TYPES = ()  # (datetime, date, time)
-
-AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
-AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
-
-
-class OptionPseudo(object):
-
-    def __init__(self, o):
-        self.__tags = set()
-        self.tag_added = None
-        self.tag_removed = None
-
-    @property
-    def tags(self):
-        """Generator of tags"""
-        return (tag for tag in self.__tags)
-
-    def add_tag(self, tag):
-        self.__tags.add(tag)
-        if callable(self.tag_added):
-            self.tag_added(tag)
-
-    def remove_tag(self, tag):
-        self.__tags.remove(tag)
-        if callable(self.tag_removed):
-            self.tag_removed(tag)
-
-    def get_text(self):
-        return self.text if self.text is not None else self.name
-
-
-class OptionMeta(type):
-
-    def __new__(mcs, name, bases, namespace):
-        cls_instance = super(OptionMeta, mcs).__new__(mcs, name, bases, namespace)
-
-        cls_instance.NOT_DEFINED = None
-        """Not defined option."""
-
-        cls_instance.NUMBER_TYPES = six.integer_types + (float,)
-        cls_instance.DATE_TYPES = ()  # (datetime, date, time)
-
-        cls_instance.AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
-        cls_instance.AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
-
-        return cls_instance
-
-    def __call__(cls, code, name, text=None, tags=None):
-
-        if code is None or name is None:
-            raise ValueError('code or name can not be None')
-
-        if not (code is None or isinstance(code, Option.AVAILABLE_CODE_TYPES)):
-            raise TypeError('Option code must be one of %s' % AVAILABLE_CODE_TYPES_STR)
-
-        if name is not None:
-            if not isinstance(name, six.string_types):
-                raise ValueError('Option name must be string type.')
-
-            if not (name[0].isalpha() and is_identifier(name) and name.isupper()):
-                raise ValueError('Option name must be alphanumeric or "_"  in uppercase and start with alphabet.')
-
-        if not ((code is None and name is None and text is None) or (code is not None and name is not None)):
-            raise ValueError('Option code and name must be not None unless code, name and text are all None.')
-
-        if tags is not None and not isinstance(tags, (tuple, list)):
-            raise ValueError('"tags" must be a tuple or list of strings.')
-
-        cls_code = type(code)
-        cls_option = type('Option(%s)' % cls_code.__name__, (cls_code, OptionPseudo), {})
-        obj_option = cls_option(code)
-        obj_option.code = code
-        obj_option.name = name
-        obj_option.text = text
-
-        if tags is not None:
-            for tag in tags:
-                if not isinstance(tag, six.string_types):
-                    raise ValueError('"tags" must be a tuple or list of strings. "%s" is not a string object.' % tag)
-                if len(tag) == 0:
-                    raise ValueError('A tag can not be empty')
-                if not is_identifier(tag) or tag.startswith('_') or not tag.isupper():
-                    raise ValueError('Tags must be uppercase alphanumeric or "_" and must starts with alphabet.')
-                obj_option.add_tag(tag)
-
-        return obj_option
-
-    def __subclasscheck__(cls, subclass):
-        if issubclass(subclass, OptionPseudo):
-            return True
-        else:
-            return super(OptionMeta, cls).__subclasscheck__(subclass)
-
-    def __instancecheck__(cls, instance):
-        if isinstance(instance, OptionPseudo):
-            return True
-        else:
-            return super(OptionMeta, cls).__instancecheck__(instance)
-
-
-@six.add_metaclass(OptionMeta)     # py2,3 compatibility
-class Option(object):
-    pass
-
-
-__all__ = ('Option', )
-
-
+"""
+Option class represents a single option in a list of options/enum
+"""
+import six
+from .mysix import is_identifier
+
+NUMBER_TYPES = six.integer_types + (float,)
+DATE_TYPES = ()  # (datetime, date, time)
+
+AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
+AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
+
+
+class OptionPseudo(object):
+
+    def __init__(self, o):
+        self.__tags = set()
+        self.tag_added = None
+        self.tag_removed = None
+
+    @property
+    def tags(self):
+        """Generator of tags"""
+        return (tag for tag in self.__tags)
+
+    def add_tag(self, tag):
+        self.__tags.add(tag)
+        if callable(self.tag_added):
+            self.tag_added(tag)
+
+    def remove_tag(self, tag):
+        self.__tags.remove(tag)
+        if callable(self.tag_removed):
+            self.tag_removed(tag)
+
+    def get_text(self):
+        return self.text if self.text is not None else self.name
+
+
+class OptionMeta(type):
+
+    def __new__(mcs, name, bases, namespace):
+        cls_instance = super(OptionMeta, mcs).__new__(mcs, name, bases, namespace)
+
+        cls_instance.NOT_DEFINED = None
+        """Not defined option."""
+
+        cls_instance.NUMBER_TYPES = six.integer_types + (float,)
+        cls_instance.DATE_TYPES = ()  # (datetime, date, time)
+
+        cls_instance.AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
+        cls_instance.AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
+
+        return cls_instance
+
+    def __call__(cls, code, name, text=None, tags=None):
+
+        if code is None or name is None:
+            raise ValueError('code or name can not be None')
+
+        if not (code is None or isinstance(code, Option.AVAILABLE_CODE_TYPES)):
+            raise TypeError('Option code must be one of %s' % AVAILABLE_CODE_TYPES_STR)
+
+        if name is not None:
+            if not isinstance(name, six.string_types):
+                raise ValueError('Option name must be string type.')
+
+            if not (name[0].isalpha() and is_identifier(name) and name.isupper()):
+                raise ValueError('Option name must be alphanumeric or "_"  in uppercase and start with alphabet.')
+
+        if not ((code is None and name is None and text is None) or (code is not None and name is not None)):
+            raise ValueError('Option code and name must be not None unless code, name and text are all None.')
+
+        if tags is not None and not isinstance(tags, (tuple, list)):
+            raise ValueError('"tags" must be a tuple or list of strings.')
+
+        cls_code = type(code)
+        cls_option = type('Option(%s)' % cls_code.__name__, (cls_code, OptionPseudo), {})
+        obj_option = cls_option(code)
+        obj_option.code = code
+        obj_option.name = name
+        obj_option.text = text
+
+        if tags is not None:
+            for tag in tags:
+                if not isinstance(tag, six.string_types):
+                    raise ValueError('"tags" must be a tuple or list of strings. "%s" is not a string object.' % tag)
+                if len(tag) == 0:
+                    raise ValueError('A tag can not be empty')
+                if not is_identifier(tag) or tag.startswith('_') or not tag.isupper():
+                    raise ValueError('Tags must be uppercase alphanumeric or "_" and must starts with alphabet.')
+                obj_option.add_tag(tag)
+
+        return obj_option
+
+    def __subclasscheck__(cls, subclass):
+        if issubclass(subclass, OptionPseudo):
+            return True
+        else:
+            return super(OptionMeta, cls).__subclasscheck__(subclass)
+
+    def __instancecheck__(cls, instance):
+        if isinstance(instance, OptionPseudo):
+            return True
+        else:
+            return super(OptionMeta, cls).__instancecheck__(instance)
+
+
+@six.add_metaclass(OptionMeta)     # py2,3 compatibility
+class Option(object):
+    pass
+
+
+__all__ = ('Option', )
+
+
```

### Comparing `optenum-1.1.8/optenum/option.v1.py` & `optenum-1.1.9/optenum/option.v1.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-"""
-Option class represents a single option in a list of options/enum
-
-DEPRECATED from v1.1.0 version.
-"""
-import six
-from datetime import datetime, date, time
-from .mysix import is_identifier
-
-
-class Option(object):
-    """ A single option with code, name and text"""
-
-    NOT_DEFINED = None
-    """Not defined option."""
-
-    NUMBER_TYPES = six.integer_types + (float, )
-    DATE_TYPES = ()    # (datetime, date, time)
-
-    AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
-    AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
-
-    def __init__(self, code, name, text=None):
-        """
-        Initialize an option
-        :param code: The real value of an option or enum entry.
-        :param name: The readable name of an option or enum entry. It can also be used as dot annotation.
-                        It is alphanumeric or "_"  in uppercase and start with alphabet.
-        :param text: The description of the option/enum entry. It's used to display. Can be i18n.
-        """
-
-        if not (code is None or isinstance(code, self.AVAILABLE_CODE_TYPES)):
-            raise TypeError('Option code must be one of %s' % self.AVAILABLE_CODE_TYPES_STR)
-
-        if name is not None:
-            if not isinstance(name, six.string_types):
-                raise ValueError('Option name must be string type.')
-
-            if not (name[0].isalpha() and is_identifier(name) and name.isupper()):
-                raise ValueError('Option name must be alphanumeric or "_"  in uppercase and start with alphabet.')
-
-        if not ((code is None and name is None and text is None) or (code is not None and name is not None)):
-            raise ValueError('Option code and name must be not None unless code, name and text are all None.')
-
-        self.__code = code
-        self.__name = name
-        self.__text = text
-
-        self.__code_type = type(code)
-
-    @property
-    def code(self):
-        """The real value of an option or enum entry."""
-        return self.__code
-
-    @property
-    def name(self):
-        """
-        The readable string of an option or enum entry. It's commonly uppercase.
-        It can also be used as dot annotation.
-        """
-        return self.__name
-
-    @property
-    def text(self):
-        """The description of the option/enum entry. It's used to display. Can be i18n."""
-        return self.__text
-
-    def get_text(self):
-        """
-        Returns `text` of the option. If `text` is None, returns `name` in lower case as text.
-        If name is also None, return `None` object converted string.
-        """
-        return str(None) if self.name is None else self.name.lower() if self.text is None else self.text
-
-    def __repr__(self):
-        return "<%s code=%s name=%s text=%s>" % (self.__class__.__name__, self.code, self.name, self.text)
-
-    def __str__(self):
-        return str(self.code)
-
-    # Compare Operators
-
-    def __op_cmp_check__(self, op, other):
-        """
-        Check if self is compatible with `other` on operation `op`
-        :param op: operation such as "+", "-" and so on
-        :param other: The other value of the operation to be compared with self.
-        :return: void.  (raise error directly if not compatible)
-        """
-        other_is_option = False
-        if isinstance(other, Option):
-            other = other.code
-            other_is_option = True
-        type_other = type(other)
-
-        if isinstance(other, self.NUMBER_TYPES + self.DATE_TYPES) and isinstance(self.code, self.NUMBER_TYPES + self.DATE_TYPES):
-            pass
-        elif isinstance(other, six.string_types) and isinstance(self.code, six.string_types):
-            pass
-        elif other is None or self.code is None or self == Option.NOT_DEFINED:
-            pass
-        else:
-            raise TypeError("'%s' not supported between instances of 'Option(%s)' and '%s'" % (
-                op, self.__code_type.__name__,
-                'Option(%s)' % type_other.__name__ if other_is_option else type_other.__name__
-            ))
-
-    # if six.PY2:
-    #     def __cmp__(self, other):
-    #         self.__op_cmp_check__('==', other)
-    #
-    #         if isinstance(other, Option):
-    #             if self.code == other.code and self.name == other.name and self.text == other.text:
-    #                 return 0
-    #             elif self.code < other.code:
-    #                 return -1
-    #             else:
-    #                 return 1
-    #         else:
-    #             return self.code.__cmp__(other)
-
-    def __eq__(self, other):
-        self.__op_cmp_check__('==', other)
-
-        if isinstance(other, Option):
-            return self.code == other.code and self.name == other.name and self.text == other.text
-        else:
-            return self.code == other
-
-    def __hash__(self):
-        """return hash of `code` to ensure key access to `set`, `dict` or other hash based collection"""
-        # return super(Option, self).__hash__()
-        return self.code.__hash__()
-
-    def __lt__(self, other):
-        self.__op_cmp_check__('<', other)
-
-        return self.code < (other.code if isinstance(other, Option) else other)
-
-    def __le__(self, other):
-        self.__op_cmp_check__('<=', other)
-
-        return self.code <= (other.code if isinstance(other, Option) else other)
-
-    def __gt__(self, other):
-        self.__op_cmp_check__('>', other)
-
-        return self.code > (other.code if isinstance(other, Option) else other)
-
-    def __ge__(self, other):
-        self.__op_cmp_check__('>=', other)
-
-        return self.code >= (other.code if isinstance(other, Option) else other)
-
-    # Math Operators
-
-    def __op_math_check__(self, op, other):
-        """
-        Check if self is compatible with `other` on math operation `op`
-        :param op: operation such as "+", "-" and so on
-        :param other: The other value of the operation to be compared with self.
-        :return: void.  (raise error directly if not compatible)
-        """
-        other_is_option = False
-        if isinstance(other, Option):
-            other = other.code
-            other_is_option = True
-        type_other = type(other)
-
-        if isinstance(other, self.NUMBER_TYPES) and isinstance(self.code, self.NUMBER_TYPES):
-            pass
-        elif isinstance(other, six.string_types) and isinstance(self.code, six.string_types):
-            pass
-        elif isinstance(other, self.DATE_TYPES) and isinstance(self.code, self.DATE_TYPES):
-            pass
-        else:
-            raise TypeError("'%s' not supported between instances of 'Option(%s)' and '%s'" % (
-                op, self.__code_type.__name__,
-                'Option(%s)' % type_other.__name__ if other_is_option else type_other.__name__
-            ))
-
-    def __op_num_check__(self, op, val):
-
-        val, val_is_option = (val.code, True) if isinstance(val, Option) else (val, False)
-        type_val = type(val)
-        type_str = 'Option(%s)' % type_val.__name__ if val_is_option else type_val.__name__
-
-        if not isinstance(val, self.NUMBER_TYPES):
-            raise TypeError("'%s' not supported on instances of '%s'" % (op, type_str))
-
-    def __op_int_check__(self, op, val):
-
-        val, val_is_option = (val.code, True) if isinstance(val, Option) else (val, False)
-        type_val = type(val)
-        type_str = 'Option(%s)' % type_val.__name__ if val_is_option else type_val.__name__
-
-        if not isinstance(val, six.integer_types):
-            raise TypeError("'%s' not supported on instances of '%s'" % (op, type_str))
-
-    def __neg__(self):
-        self.__op_num_check__('-(negative)', self)
-
-        return - self.code
-
-    def __pos__(self):
-        self.__op_num_check__('+(positive)', self)
-
-        return + self.code
-
-    def __abs__(self):
-        self.__op_num_check__('abs', self)
-
-        return abs(self.code)
-
-    def __int__(self):
-        return int(self.code)
-
-    def __float__(self):
-        return float(self.code)
-
-    def __invert__(self):
-        self.__op_int_check__('~', self)
-
-        return ~ self.code
-
-    def __lshift__(self, other):
-        self.__op_int_check__('<<', self)
-        self.__op_int_check__('<<', other)
-
-        return self.code << other
-
-    def __rlshift__(self, other):
-        self.__op_int_check__('<<', self)
-        self.__op_int_check__('<<', other)
-
-        return other << self.code
-
-    def __rshift__(self, other):
-        self.__op_int_check__('>>', self)
-        self.__op_int_check__('>>', other)
-
-        return self.code >> other
-
-    def __rrshift__(self, other):
-        self.__op_int_check__('>>', self)
-        self.__op_int_check__('>>', other)
-
-        return other >> self.code
-
-    def __add__(self, other):
-        self.__op_math_check__('+', other)
-
-        return self.code + (other.code if isinstance(other, Option) else other)
-
-    def __radd__(self, other):
-        return self.__add__(other)
-
-    def __sub__(self, other):
-        self.__op_math_check__('-', other)
-
-        return self.code - (other.code if isinstance(other, Option) else other)
-
-    def __rsub__(self, other):
-        self.__op_math_check__('-', other)
-
-        return (other.code if isinstance(other, Option) else other) - self.code
-
-    def __mul__(self, other):
-        self.__op_num_check__('*', other)
-
-        return self.code * (other.code if isinstance(other, Option) else other)
-
-    def __rmul__(self, other):
-        return self.__mul__(other)
-
-    def __truediv__(self, other):
-        self.__op_num_check__('/', self)
-        self.__op_num_check__('/', other)
-
-        return self.code.__truediv__(other.code if isinstance(other, Option) else other)
-
-    def __rtruediv__(self, other):
-        self.__op_num_check__('/', self)
-        self.__op_num_check__('/', other)
-
-        return self.code.__rtruediv__(other.code if isinstance(other, Option) else other)
-
-    def __floordiv__(self, other):
-        self.__op_num_check__('//', self)
-        self.__op_num_check__('//', other)
-
-        return self.code.__floordiv__(other.code if isinstance(other, Option) else other)
-
-    def __rfloordiv__(self, other):
-        self.__op_num_check__('//', self)
-        self.__op_num_check__('//', other)
-
-        return self.code.__rfloordiv__(other.code if isinstance(other, Option) else other)
-
-    # compatible with PY2 without "from __future__ import division"
-    def __div__(self, other):
-        self.__op_num_check__('/', self)
-        self.__op_num_check__('/', other)
-
-        return self.code.__div__(other.code if isinstance(other, Option) else other)
-
-    def __rdiv__(self, other):
-        self.__op_num_check__('/', self)
-        self.__op_num_check__('/', other)
-
-        return self.code.__rdiv__(other.code if isinstance(other, Option) else other)
-
-    def __divmod__(self, other):
-        self.__op_num_check__('%', self)
-        self.__op_num_check__('%', other)
-
-        return self.code.__divmod__(other.code if isinstance(other, Option) else other)
-
-    def __rdivmod__(self, other):
-        self.__op_num_check__('%', self)
-        self.__op_num_check__('%', other)
-
-        return self.code.__rdivmod__(other.code if isinstance(other, Option) else other)
-
-    def __mod__(self, other):
-
-        self.__op_num_check__('%', self)
-        self.__op_num_check__('%', other)
-
-        return self.code.__mod__(other.code if isinstance(other, Option) else other)
-
-    def __rmod__(self, other):
-        self.__op_num_check__('%', self)
-        self.__op_num_check__('%', other)
-
-        return self.code.__rmod__(other.code if isinstance(other, Option) else other)
-
-
-Option.NOT_DEFINED = Option(None, None, None)
-
-
-__all__ = ('Option', )
+"""
+Option class represents a single option in a list of options/enum
+
+DEPRECATED from v1.1.0 version.
+"""
+import six
+from datetime import datetime, date, time
+from .mysix import is_identifier
+
+
+class Option(object):
+    """ A single option with code, name and text"""
+
+    NOT_DEFINED = None
+    """Not defined option."""
+
+    NUMBER_TYPES = six.integer_types + (float, )
+    DATE_TYPES = ()    # (datetime, date, time)
+
+    AVAILABLE_CODE_TYPES = six.string_types + NUMBER_TYPES + DATE_TYPES
+    AVAILABLE_CODE_TYPES_STR = ', '.join(t.__name__ for t in AVAILABLE_CODE_TYPES)
+
+    def __init__(self, code, name, text=None):
+        """
+        Initialize an option
+        :param code: The real value of an option or enum entry.
+        :param name: The readable name of an option or enum entry. It can also be used as dot annotation.
+                        It is alphanumeric or "_"  in uppercase and start with alphabet.
+        :param text: The description of the option/enum entry. It's used to display. Can be i18n.
+        """
+
+        if not (code is None or isinstance(code, self.AVAILABLE_CODE_TYPES)):
+            raise TypeError('Option code must be one of %s' % self.AVAILABLE_CODE_TYPES_STR)
+
+        if name is not None:
+            if not isinstance(name, six.string_types):
+                raise ValueError('Option name must be string type.')
+
+            if not (name[0].isalpha() and is_identifier(name) and name.isupper()):
+                raise ValueError('Option name must be alphanumeric or "_"  in uppercase and start with alphabet.')
+
+        if not ((code is None and name is None and text is None) or (code is not None and name is not None)):
+            raise ValueError('Option code and name must be not None unless code, name and text are all None.')
+
+        self.__code = code
+        self.__name = name
+        self.__text = text
+
+        self.__code_type = type(code)
+
+    @property
+    def code(self):
+        """The real value of an option or enum entry."""
+        return self.__code
+
+    @property
+    def name(self):
+        """
+        The readable string of an option or enum entry. It's commonly uppercase.
+        It can also be used as dot annotation.
+        """
+        return self.__name
+
+    @property
+    def text(self):
+        """The description of the option/enum entry. It's used to display. Can be i18n."""
+        return self.__text
+
+    def get_text(self):
+        """
+        Returns `text` of the option. If `text` is None, returns `name` in lower case as text.
+        If name is also None, return `None` object converted string.
+        """
+        return str(None) if self.name is None else self.name.lower() if self.text is None else self.text
+
+    def __repr__(self):
+        return "<%s code=%s name=%s text=%s>" % (self.__class__.__name__, self.code, self.name, self.text)
+
+    def __str__(self):
+        return str(self.code)
+
+    # Compare Operators
+
+    def __op_cmp_check__(self, op, other):
+        """
+        Check if self is compatible with `other` on operation `op`
+        :param op: operation such as "+", "-" and so on
+        :param other: The other value of the operation to be compared with self.
+        :return: void.  (raise error directly if not compatible)
+        """
+        other_is_option = False
+        if isinstance(other, Option):
+            other = other.code
+            other_is_option = True
+        type_other = type(other)
+
+        if isinstance(other, self.NUMBER_TYPES + self.DATE_TYPES) and isinstance(self.code, self.NUMBER_TYPES + self.DATE_TYPES):
+            pass
+        elif isinstance(other, six.string_types) and isinstance(self.code, six.string_types):
+            pass
+        elif other is None or self.code is None or self == Option.NOT_DEFINED:
+            pass
+        else:
+            raise TypeError("'%s' not supported between instances of 'Option(%s)' and '%s'" % (
+                op, self.__code_type.__name__,
+                'Option(%s)' % type_other.__name__ if other_is_option else type_other.__name__
+            ))
+
+    # if six.PY2:
+    #     def __cmp__(self, other):
+    #         self.__op_cmp_check__('==', other)
+    #
+    #         if isinstance(other, Option):
+    #             if self.code == other.code and self.name == other.name and self.text == other.text:
+    #                 return 0
+    #             elif self.code < other.code:
+    #                 return -1
+    #             else:
+    #                 return 1
+    #         else:
+    #             return self.code.__cmp__(other)
+
+    def __eq__(self, other):
+        self.__op_cmp_check__('==', other)
+
+        if isinstance(other, Option):
+            return self.code == other.code and self.name == other.name and self.text == other.text
+        else:
+            return self.code == other
+
+    def __hash__(self):
+        """return hash of `code` to ensure key access to `set`, `dict` or other hash based collection"""
+        # return super(Option, self).__hash__()
+        return self.code.__hash__()
+
+    def __lt__(self, other):
+        self.__op_cmp_check__('<', other)
+
+        return self.code < (other.code if isinstance(other, Option) else other)
+
+    def __le__(self, other):
+        self.__op_cmp_check__('<=', other)
+
+        return self.code <= (other.code if isinstance(other, Option) else other)
+
+    def __gt__(self, other):
+        self.__op_cmp_check__('>', other)
+
+        return self.code > (other.code if isinstance(other, Option) else other)
+
+    def __ge__(self, other):
+        self.__op_cmp_check__('>=', other)
+
+        return self.code >= (other.code if isinstance(other, Option) else other)
+
+    # Math Operators
+
+    def __op_math_check__(self, op, other):
+        """
+        Check if self is compatible with `other` on math operation `op`
+        :param op: operation such as "+", "-" and so on
+        :param other: The other value of the operation to be compared with self.
+        :return: void.  (raise error directly if not compatible)
+        """
+        other_is_option = False
+        if isinstance(other, Option):
+            other = other.code
+            other_is_option = True
+        type_other = type(other)
+
+        if isinstance(other, self.NUMBER_TYPES) and isinstance(self.code, self.NUMBER_TYPES):
+            pass
+        elif isinstance(other, six.string_types) and isinstance(self.code, six.string_types):
+            pass
+        elif isinstance(other, self.DATE_TYPES) and isinstance(self.code, self.DATE_TYPES):
+            pass
+        else:
+            raise TypeError("'%s' not supported between instances of 'Option(%s)' and '%s'" % (
+                op, self.__code_type.__name__,
+                'Option(%s)' % type_other.__name__ if other_is_option else type_other.__name__
+            ))
+
+    def __op_num_check__(self, op, val):
+
+        val, val_is_option = (val.code, True) if isinstance(val, Option) else (val, False)
+        type_val = type(val)
+        type_str = 'Option(%s)' % type_val.__name__ if val_is_option else type_val.__name__
+
+        if not isinstance(val, self.NUMBER_TYPES):
+            raise TypeError("'%s' not supported on instances of '%s'" % (op, type_str))
+
+    def __op_int_check__(self, op, val):
+
+        val, val_is_option = (val.code, True) if isinstance(val, Option) else (val, False)
+        type_val = type(val)
+        type_str = 'Option(%s)' % type_val.__name__ if val_is_option else type_val.__name__
+
+        if not isinstance(val, six.integer_types):
+            raise TypeError("'%s' not supported on instances of '%s'" % (op, type_str))
+
+    def __neg__(self):
+        self.__op_num_check__('-(negative)', self)
+
+        return - self.code
+
+    def __pos__(self):
+        self.__op_num_check__('+(positive)', self)
+
+        return + self.code
+
+    def __abs__(self):
+        self.__op_num_check__('abs', self)
+
+        return abs(self.code)
+
+    def __int__(self):
+        return int(self.code)
+
+    def __float__(self):
+        return float(self.code)
+
+    def __invert__(self):
+        self.__op_int_check__('~', self)
+
+        return ~ self.code
+
+    def __lshift__(self, other):
+        self.__op_int_check__('<<', self)
+        self.__op_int_check__('<<', other)
+
+        return self.code << other
+
+    def __rlshift__(self, other):
+        self.__op_int_check__('<<', self)
+        self.__op_int_check__('<<', other)
+
+        return other << self.code
+
+    def __rshift__(self, other):
+        self.__op_int_check__('>>', self)
+        self.__op_int_check__('>>', other)
+
+        return self.code >> other
+
+    def __rrshift__(self, other):
+        self.__op_int_check__('>>', self)
+        self.__op_int_check__('>>', other)
+
+        return other >> self.code
+
+    def __add__(self, other):
+        self.__op_math_check__('+', other)
+
+        return self.code + (other.code if isinstance(other, Option) else other)
+
+    def __radd__(self, other):
+        return self.__add__(other)
+
+    def __sub__(self, other):
+        self.__op_math_check__('-', other)
+
+        return self.code - (other.code if isinstance(other, Option) else other)
+
+    def __rsub__(self, other):
+        self.__op_math_check__('-', other)
+
+        return (other.code if isinstance(other, Option) else other) - self.code
+
+    def __mul__(self, other):
+        self.__op_num_check__('*', other)
+
+        return self.code * (other.code if isinstance(other, Option) else other)
+
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
+    def __truediv__(self, other):
+        self.__op_num_check__('/', self)
+        self.__op_num_check__('/', other)
+
+        return self.code.__truediv__(other.code if isinstance(other, Option) else other)
+
+    def __rtruediv__(self, other):
+        self.__op_num_check__('/', self)
+        self.__op_num_check__('/', other)
+
+        return self.code.__rtruediv__(other.code if isinstance(other, Option) else other)
+
+    def __floordiv__(self, other):
+        self.__op_num_check__('//', self)
+        self.__op_num_check__('//', other)
+
+        return self.code.__floordiv__(other.code if isinstance(other, Option) else other)
+
+    def __rfloordiv__(self, other):
+        self.__op_num_check__('//', self)
+        self.__op_num_check__('//', other)
+
+        return self.code.__rfloordiv__(other.code if isinstance(other, Option) else other)
+
+    # compatible with PY2 without "from __future__ import division"
+    def __div__(self, other):
+        self.__op_num_check__('/', self)
+        self.__op_num_check__('/', other)
+
+        return self.code.__div__(other.code if isinstance(other, Option) else other)
+
+    def __rdiv__(self, other):
+        self.__op_num_check__('/', self)
+        self.__op_num_check__('/', other)
+
+        return self.code.__rdiv__(other.code if isinstance(other, Option) else other)
+
+    def __divmod__(self, other):
+        self.__op_num_check__('%', self)
+        self.__op_num_check__('%', other)
+
+        return self.code.__divmod__(other.code if isinstance(other, Option) else other)
+
+    def __rdivmod__(self, other):
+        self.__op_num_check__('%', self)
+        self.__op_num_check__('%', other)
+
+        return self.code.__rdivmod__(other.code if isinstance(other, Option) else other)
+
+    def __mod__(self, other):
+
+        self.__op_num_check__('%', self)
+        self.__op_num_check__('%', other)
+
+        return self.code.__mod__(other.code if isinstance(other, Option) else other)
+
+    def __rmod__(self, other):
+        self.__op_num_check__('%', self)
+        self.__op_num_check__('%', other)
+
+        return self.code.__rmod__(other.code if isinstance(other, Option) else other)
+
+
+Option.NOT_DEFINED = Option(None, None, None)
+
+
+__all__ = ('Option', )
```

### Comparing `optenum-1.1.8/optenum/options.py` & `optenum-1.1.9/optenum/options.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,334 +1,337 @@
-"""
-Options represents an set of option items (enumerations). It can also represent as a collection of options/enum entries.
-"""
-
-import six
-from collections import OrderedDict
-from .option import Option
-import logging
-
-log = logging.getLogger(__name__)
-
-
-class OptionGroup(list):
-
-    def __init__(self, *args):
-
-        # to ensure args are in list, consider the following
-        #
-        # class Foo(Options):
-        #     A = 1
-        #     B = 2, 'B is 2'
-        #
-        #     G1 = OptionGroup(A)       # should get args [ 1 ]
-        #     G2 = OptionGroup(B)       # should get args [ (2, 'B is 2') ]
-        #
-
-        super(OptionGroup, self).__init__()
-        for arg in args:
-            if isinstance(arg, OptionGroup):
-                for a in arg:
-                    if a not in self:
-                        self.append(a)
-            else:
-                if arg not in self:
-                    self.append(arg)
-
-    def add(self, opt):
-        if isinstance(opt, Option):
-            super(OptionGroup, self).append(opt)
-        else:
-            raise TypeError('Only "%s" can be added into "%s". "%s" is "%s".'
-                            % (Option.__name__, OptionGroup.__name__, opt, type(opt)))
-
-    def remove(self, opt):
-        super(OptionGroup, self).remove(opt)
-
-    def __add__(self, other):
-        if isinstance(other, OptionGroup):
-            r = OptionGroup(*super(OptionGroup, self).__add__(other))
-            return r
-        elif isinstance(other, Option):
-            r = OptionGroup(*super(OptionGroup, self).__add__([other]))
-            return r
-        else:
-            raise TypeError('Can not add "%s"<%s> to %s. Please explicitly convert it to "%s" or "%s"'
-                            % (other, type(other).__name__, OptionGroup.__name__, Option.__name__, OptionGroup.__name__))
-
-
-class OptionsMeta(type):
-
-    @classmethod
-    def __prepare__(mcs, name, bases, **kwargs):
-
-        # hack for python 3.4 and 3.5. It returns OrderedDict by default after 3.6.
-        return OrderedDict()
-
-    def __new__(mcs, name, bases, namespace):
-        instance = super(OptionsMeta, mcs).__new__(mcs, name, bases, namespace)
-        name_options_mapping = {}
-        code_options_mapping = {}
-        groups = {}
-
-        ignore_invalid_name = namespace.get('__IGNORE_INVALID_NAME__', False)
-        order_by = namespace.get('__ORDER_BY__', None)
-
-        if not isinstance(ignore_invalid_name, bool):
-            raise ValueError("'__IGNORE_INVALID_NAME__' must be bool type True or False.")
-
-        if order_by not in ['code', 'name', None]:
-            raise ValueError("'__ORDER_BY__' only supported on `code` and `name` field")
-
-        if name != 'Options':
-            for attr, val in namespace.items():
-                if attr.startswith('_'):
-                    continue
-                elif not attr.isupper():
-                    if callable(val) or isinstance(val, (staticmethod, classmethod, property)):
-                        pass    # function
-                    else:
-                        if not ignore_invalid_name:
-                            raise AttributeError('Option name must be uppercase. Attribute "%s" is not.' % attr)
-                else:
-                    if attr in name_options_mapping.keys() or hasattr(mcs, attr):
-                        raise AttributeError('Duplicated attribute "%s" found' % attr)
-
-                    if isinstance(val, OptionGroup):
-                        groups[attr] = val
-                        continue
-                    else:
-                        if isinstance(val, Option):
-                            if val.name != attr:
-                                raise ValueError('Option name of option %s must be same as attribute "%s"' % (val, attr))
-                            else:
-                                opt = val
-                        elif isinstance(val, (list, tuple)):
-                            if len(val) == 0:
-                                raise ValueError('Option code can not be empty list or tuple')
-                            elif len(val) == 1:
-                                opt = Option(code=val[0], name=attr)
-                            elif len(val) == 2:
-                                opt = Option(code=val[0], name=attr, text=val[1])
-                            elif len(val) == 3:
-                                opt = Option(code=val[0], name=attr, text=val[1], tags=val[2])
-                            else:
-                                raise ValueError('Tuple/list style Option accept only 3 arguments (code, text, tags).' 
-                                                 '"name" is same as attribute an not required.')
-                        elif isinstance(val, Option.AVAILABLE_CODE_TYPES):
-                            opt = Option(code=val, name=attr)
-                        else:
-                            raise TypeError('"%s" can not be converted to Option.' % attr)
-
-                        if opt.code in code_options_mapping.keys():
-                            raise ValueError('Duplicated code "%s" found' % opt.code)
-
-                        setattr(instance, attr, opt)
-                        name_options_mapping[attr] = opt
-                        code_options_mapping[opt.code] = opt
-                        mcs.__scan_option_tags_for_group(instance, opt)
-
-            for attr, val in groups.items():
-                # grouping options
-                for code in val:
-                    if isinstance(code, (tuple, list)):
-                        code = code[0]
-                    opt = code_options_mapping.get(code, None)
-                    if opt is None or not isinstance(opt, Option):
-                        raise SyntaxError('"%s" is not available Option of %s' % (code, instance.__name__))
-                    assert callable(opt.tag_added)
-                    assert callable(opt.tag_removed)
-                    opt.add_tag(attr)
-
-        instance.__name_options_mapping__ = name_options_mapping
-        instance.__code_options_mapping__ = code_options_mapping
-
-        return instance
-
-    def __scan_option_tags_for_group(cls, opt):
-        """
-        Scan all tags in a given Option object and add the object to appropriate group of the tag.
-        :param opt: Option object
-        :return:
-        """
-
-        def add_option_to_group(atag):
-            __group = '__%s' % atag
-            group = getattr(cls, __group, None)
-            if group is not None:
-                if isinstance(group, OptionGroup):
-                    group.add(opt)
-                else:
-                    raise ValueError('Tag "%s" is duplicated as attribute of "%s"'
-                                     % (atag, cls.__name__))
-            else:
-                group = OptionGroup()
-                group.add(opt)
-                setattr(cls, __group, group)
-            setattr(cls, atag, tuple(group))
-
-        def remove_option_from_group(atag):
-            __group = '__%s' % atag
-            group = getattr(cls, __group, None)
-            if group is not None:
-                if isinstance(group, OptionGroup):
-                    group.remove(opt)
-                else:
-                    raise ValueError('No options are grouped in with "%s" in "%s"' % (atag, cls.__name__))
-            else:
-                raise ValueError('Option group for tag "%s" is not existing in "%s"' % (atag, cls.__name__))
-            setattr(cls, atag, tuple(group))
-
-        for tag in opt.tags:
-            add_option_to_group(tag)
-
-        opt.tag_added = add_option_to_group
-        opt.tag_removed = remove_option_from_group
-
-    # Options class methods or properties
-    def __get_name_options_mapping(cls):
-        """
-        Dict of {'name': option} mapping.
-        DO NOT change this dict. TODO: make it immutable.
-
-        :return: dict {"name": option}
-        """
-        return cls.__name_options_mapping__
-
-    def __get_code_options_mapping(cls):
-        """
-        Dict of {'code': option} mapping
-        DO NOT change this dict. TODO: make it immutable.
-        :return: dict {"name": option}
-        """
-        return cls.__code_options_mapping__
-
-    def __getitem__(cls, item):
-        return cls.__get_name_options_mapping()[item]
-
-    def __setitem__(cls, key, value):
-        raise TypeError("'%s' class does not support item assignment" % cls.__name__)
-
-    def __delitem__(cls, key):
-        raise TypeError("'%s' class does not support item deletion" % cls.__name__)
-
-    def __contains__(cls, item):
-        if isinstance(item, Option):
-            return item in cls.__get_name_options_mapping().values()
-        else:
-            return item in cls.__get_code_options_mapping().keys()
-
-    def get(cls, key, default=None):
-        return cls.__get_name_options_mapping().get(key, default)
-
-    @property
-    def codes(cls):
-        """List of `code`s"""
-        return list(cls.__get_code_options_mapping().keys())
-
-    @property
-    def names(cls):
-        """List of `name`s"""
-        return list(cls.__get_name_options_mapping().keys())
-
-    @property
-    def all(cls):
-        """List of `Option` objects"""
-        return list(cls.__get_name_options_mapping().values())
-
-    @property
-    def tuples(cls):
-        """List of (`name`, `code`, `text`) tuples"""
-        return [(o.name, o.code, o.text) for o in cls.__get_name_options_mapping().values()]
-
-    @property
-    def items(cls):
-        """Dict of {`name`: Option} mapping"""
-        return {o.name: o for o in cls.__get_name_options_mapping().values()}
-
-    def get_list(cls, *fields):
-        """
-        List of *fields.
-        :param fields: Field name of `Option`. Such as `code`, (`name`, `code`), [`code`, `name`, `text`] or etc.
-        :return: List of *fields tuple or single value.
-        """
-
-        if len(fields) == 0:
-            raise ValueError("No fields argument found.")
-
-        found_fields = set()
-        for f in fields:
-            if f not in ['code', 'name', 'text']:
-                raise NameError(
-                    "'%s' is incorrect Option field. Only 'code', 'name' and 'text' are available." % str(f))
-            if f in found_fields:
-                raise ValueError("Duplicated fields '%s' found." % str(f))
-            found_fields.add(f)
-
-        lst = []
-        for o in cls.__get_name_options_mapping().values():
-            value = []
-            for f in fields:
-                value.append(getattr(o, f))
-            lst.append(value[0] if len(value) == 1 else tuple(value))
-        return lst
-
-    def get_dict(cls, key_field, *fields):
-        """
-        Retrieve as dict of {key_field: *fields} mapping. If `fields` is single value, returns `{key:value}` mapping.
-                If `fields` is **tuple**, returns `{key: (tuple of fields value)}` mapping.
-        :param key_field: name of Option field for dict key. Only `code` and `name` are available.
-        :param fields: Names of Option field for values. Can be tuple or single value. Impact value part of return dict.
-        :return: dict of {key_field: *fields} mapping.
-        """
-        if key_field not in ['code', 'name']:
-            raise NameError("'%s' is not correct key field. Only 'code' and 'name' can be key field." % str(key_field))
-
-        if len(fields) == 0:
-            raise ValueError("No fields argument found.")
-
-        found_fields = set()
-        for f in fields:
-            if f not in ['code', 'name', 'text']:
-                raise NameError(
-                    "'%s' is incorrect Option field. Only 'code', 'name' and 'text' are available." % str(f))
-            if f in found_fields:
-                raise ValueError("Duplicated fields '%s' found." % str(f))
-            found_fields.add(f)
-
-        items = {}
-        for o in cls.__get_name_options_mapping().values():
-            key = getattr(o, key_field)
-            value = []
-            for f in fields:
-                value.append(getattr(o, f))
-            items[key] = value[0] if len(value) == 1 else tuple(value)
-
-        return items
-
-
-@six.add_metaclass(OptionsMeta)     # py2,3 compatibility
-class Options(object):
-    """
-    Derive class `Options` to implement your enum/options.
-    e.g
-    ```
-        # simple way
-        class Fruit(Options):
-            APPLE = 1
-            ORANGE = 2
-            BANANA = 3
-
-        # option `code` + `text` description in tuple
-        class DoorState(Options):
-            OPEN = 'O', 'Door is opened'
-            CLOSED = ('C', 'Door is closed')
-            IN_OPENING = 'IO'
-            IN_CLOSING = 'IC'
-    ```
-    """
-
-    pass
-
-
-__all__ = ('Options', 'OptionGroup')
-
+"""
+Options represents an set of option items (enumerations). It can also represent as a collection of options/enum entries.
+"""
+
+import six
+from collections import OrderedDict
+from .option import Option
+import logging
+
+log = logging.getLogger(__name__)
+
+
+class OptionGroup(list):
+
+    def __init__(self, *args):
+
+        # to ensure args are in list, consider the following
+        #
+        # class Foo(Options):
+        #     A = 1
+        #     B = 2, 'B is 2'
+        #
+        #     G1 = OptionGroup(A)       # should get args [ 1 ]
+        #     G2 = OptionGroup(B)       # should get args [ (2, 'B is 2') ]
+        #
+
+        super(OptionGroup, self).__init__()
+        for arg in args:
+            if isinstance(arg, OptionGroup):
+                for a in arg:
+                    if a not in self:
+                        self.append(a)
+            else:
+                if arg not in self:
+                    self.append(arg)
+
+    def add(self, opt):
+        if isinstance(opt, Option):
+            super(OptionGroup, self).append(opt)
+        else:
+            raise TypeError('Only "%s" can be added into "%s". "%s" is "%s".'
+                            % (Option.__name__, OptionGroup.__name__, opt, type(opt)))
+
+    def remove(self, opt):
+        super(OptionGroup, self).remove(opt)
+
+    def __add__(self, other):
+        if isinstance(other, OptionGroup):
+            r = OptionGroup(*super(OptionGroup, self).__add__(other))
+            return r
+        elif isinstance(other, Option):
+            r = OptionGroup(*super(OptionGroup, self).__add__([other]))
+            return r
+        else:
+            raise TypeError('Can not add "%s"<%s> to %s. Please explicitly convert it to "%s" or "%s"'
+                            % (other, type(other).__name__, OptionGroup.__name__, Option.__name__, OptionGroup.__name__))
+
+
+class OptionsMeta(type):
+
+    @classmethod
+    def __prepare__(mcs, name, bases, **kwargs):
+
+        # hack for python 3.4 and 3.5. It returns OrderedDict by default after 3.6.
+        return OrderedDict()
+
+    def __new__(mcs, name, bases, namespace):
+        instance = super(OptionsMeta, mcs).__new__(mcs, name, bases, namespace)
+        name_options_mapping = {}
+        code_options_mapping = {}
+        groups = {}
+
+        ignore_invalid_name = namespace.get('__IGNORE_INVALID_NAME__', False)
+        order_by = namespace.get('__ORDER_BY__', None)
+
+        if not isinstance(ignore_invalid_name, bool):
+            raise ValueError("'__IGNORE_INVALID_NAME__' must be bool type True or False.")
+
+        if order_by not in ['code', 'name', None]:
+            raise ValueError("'__ORDER_BY__' only supported on `code` and `name` field")
+
+        if name != 'Options':
+            for attr, val in namespace.items():
+                if attr.startswith('_'):
+                    continue
+                elif not attr.isupper():
+                    if callable(val) or isinstance(val, (staticmethod, classmethod, property)):
+                        pass    # function
+                    else:
+                        if not ignore_invalid_name:
+                            raise AttributeError('Option name must be uppercase. Attribute "%s" is not.' % attr)
+                else:
+                    if attr in name_options_mapping.keys() or hasattr(mcs, attr):
+                        raise AttributeError('Duplicated attribute "%s" found' % attr)
+
+                    if isinstance(val, OptionGroup):
+                        groups[attr] = val
+                        continue
+                    else:
+                        if isinstance(val, Option):
+                            if val.name != attr:
+                                raise ValueError('Option name of option %s must be same as attribute "%s"' % (val, attr))
+                            else:
+                                opt = val
+                        elif isinstance(val, (list, tuple)):
+                            if len(val) == 0:
+                                raise ValueError('Option code can not be empty list or tuple')
+                            elif len(val) == 1:
+                                opt = Option(code=val[0], name=attr)
+                            elif len(val) == 2:
+                                opt = Option(code=val[0], name=attr, text=val[1])
+                            elif len(val) == 3:
+                                opt = Option(code=val[0], name=attr, text=val[1], tags=val[2])
+                            else:
+                                raise ValueError('Tuple/list style Option accept only 3 arguments (code, text, tags).' 
+                                                 '"name" is same as attribute an not required.')
+                        elif isinstance(val, Option.AVAILABLE_CODE_TYPES):
+                            opt = Option(code=val, name=attr)
+                        else:
+                            raise TypeError('"%s" can not be converted to Option.' % attr)
+
+                        if opt.code in code_options_mapping.keys():
+                            raise ValueError('Duplicated code "%s" found' % opt.code)
+
+                        setattr(instance, attr, opt)
+                        name_options_mapping[attr] = opt
+                        code_options_mapping[opt.code] = opt
+                        mcs.__scan_option_tags_for_group(instance, opt)
+
+            for attr, val in groups.items():
+                # grouping options
+                for code in val:
+                    if isinstance(code, (tuple, list)):
+                        code = code[0]
+                    opt = code_options_mapping.get(code, None)
+                    if opt is None or not isinstance(opt, Option):
+                        raise SyntaxError('"%s" is not available Option of %s' % (code, instance.__name__))
+                    assert callable(opt.tag_added)
+                    assert callable(opt.tag_removed)
+                    opt.add_tag(attr)
+
+        instance.__name_options_mapping__ = name_options_mapping
+        instance.__code_options_mapping__ = code_options_mapping
+
+        return instance
+
+    def __scan_option_tags_for_group(cls, opt):
+        """
+        Scan all tags in a given Option object and add the object to appropriate group of the tag.
+        :param opt: Option object
+        :return:
+        """
+
+        def add_option_to_group(atag):
+            __group = '__%s' % atag
+            group = getattr(cls, __group, None)
+            if group is not None:
+                if isinstance(group, OptionGroup):
+                    group.add(opt)
+                else:
+                    raise ValueError('Tag "%s" is duplicated as attribute of "%s"'
+                                     % (atag, cls.__name__))
+            else:
+                group = OptionGroup()
+                group.add(opt)
+                setattr(cls, __group, group)
+            setattr(cls, atag, tuple(group))
+
+        def remove_option_from_group(atag):
+            __group = '__%s' % atag
+            group = getattr(cls, __group, None)
+            if group is not None:
+                if isinstance(group, OptionGroup):
+                    group.remove(opt)
+                else:
+                    raise ValueError('No options are grouped in with "%s" in "%s"' % (atag, cls.__name__))
+            else:
+                raise ValueError('Option group for tag "%s" is not existing in "%s"' % (atag, cls.__name__))
+            setattr(cls, atag, tuple(group))
+
+        for tag in opt.tags:
+            add_option_to_group(tag)
+
+        opt.tag_added = add_option_to_group
+        opt.tag_removed = remove_option_from_group
+
+    # Options class methods or properties
+    def __get_name_options_mapping(cls):
+        """
+        Dict of {'name': option} mapping.
+        DO NOT change this dict. TODO: make it immutable.
+
+        :return: dict {"name": option}
+        """
+        return cls.__name_options_mapping__
+
+    def __get_code_options_mapping(cls):
+        """
+        Dict of {'code': option} mapping
+        DO NOT change this dict. TODO: make it immutable.
+        :return: dict {"name": option}
+        """
+        return cls.__code_options_mapping__
+
+    def __getitem__(cls, item):
+        return cls.__get_name_options_mapping()[item]
+
+    def __setitem__(cls, key, value):
+        raise TypeError("'%s' class does not support item assignment" % cls.__name__)
+
+    def __delitem__(cls, key):
+        raise TypeError("'%s' class does not support item deletion" % cls.__name__)
+
+    def __contains__(cls, item):
+        if isinstance(item, Option):
+            return item in cls.__get_name_options_mapping().values()
+        else:
+            return item in cls.__get_code_options_mapping().keys()
+
+    def get(cls, key, default=None):
+        return cls.__get_name_options_mapping().get(key, default)
+
+    @property
+    def codes(cls):
+        """List of `code`s"""
+        return list(cls.__get_code_options_mapping().keys())
+
+    @property
+    def names(cls):
+        """List of `name`s"""
+        return list(cls.__get_name_options_mapping().keys())
+
+    @property
+    def all(cls):
+        """List of `Option` objects"""
+        return list(cls.__get_name_options_mapping().values())
+
+    @property
+    def tuples(cls):
+        """List of (`name`, `code`, `text`) tuples"""
+        return [(o.name, o.code, o.text) for o in cls.__get_name_options_mapping().values()]
+
+    @property
+    def items(cls):
+        """Dict of {`name`: Option} mapping"""
+        return {o.name: o for o in cls.__get_name_options_mapping().values()}
+
+    def get_list(cls, *fields):
+        """
+        List of *fields.
+        :param fields: Field name of `Option`. Such as `code`, (`name`, `code`), [`code`, `name`, `text`] or etc.
+        :return: List of *fields tuple or single value.
+        """
+
+        if len(fields) == 0:
+            raise ValueError("No fields argument found.")
+
+        found_fields = set()
+        for f in fields:
+            if f not in ['code', 'name', 'text']:
+                raise NameError(
+                    "'%s' is incorrect Option field. Only 'code', 'name' and 'text' are available." % str(f))
+            if f in found_fields:
+                raise ValueError("Duplicated fields '%s' found." % str(f))
+            found_fields.add(f)
+
+        lst = []
+        for o in cls.__get_name_options_mapping().values():
+            value = []
+            for f in fields:
+                value.append(getattr(o, f))
+            lst.append(value[0] if len(value) == 1 else tuple(value))
+        return lst
+
+    def get_dict(cls, key_field, *fields):
+        """
+        Retrieve as dict of {key_field: *fields} mapping. If `fields` is single value, returns `{key:value}` mapping.
+                If `fields` is **tuple**, returns `{key: (tuple of fields value)}` mapping.
+        :param key_field: name of Option field for dict key. Only `code` and `name` are available.
+        :param fields: Names of Option field for values. Can be tuple or single value. Impact value part of return dict.
+        :return: dict of {key_field: *fields} mapping.
+        """
+        if key_field not in ['code', 'name']:
+            raise NameError("'%s' is not correct key field. Only 'code' and 'name' can be key field." % str(key_field))
+
+        if len(fields) == 0:
+            raise ValueError("No fields argument found.")
+
+        found_fields = set()
+        for f in fields:
+            if f not in ['code', 'name', 'text']:
+                raise NameError(
+                    "'%s' is incorrect Option field. Only 'code', 'name' and 'text' are available." % str(f))
+            if f in found_fields:
+                raise ValueError("Duplicated fields '%s' found." % str(f))
+            found_fields.add(f)
+
+        items = {}
+        for o in cls.__get_name_options_mapping().values():
+            key = getattr(o, key_field)
+            value = []
+            for f in fields:
+                value.append(getattr(o, f))
+            items[key] = value[0] if len(value) == 1 else tuple(value)
+
+        return items
+
+
+@six.add_metaclass(OptionsMeta)     # py2,3 compatibility
+class Options(object):
+    """
+    Derive class `Options` to implement your enum/options.
+    e.g
+    ```
+        # simple way
+        class Fruit(Options):
+            APPLE = 1
+            ORANGE = 2
+            BANANA = 3
+
+        # option `code` + `text` description in tuple
+        class DoorState(Options):
+            OPEN = 'O', 'Door is opened'
+            CLOSED = ('C', 'Door is closed')
+            IN_OPENING = 'IO'
+            IN_CLOSING = 'IC'
+    ```
+    """
+
+    @classmethod
+    def choices(cls):
+        # for django choices
+        return cls.get_list('code', 'text')
+
+
+__all__ = ('Options', 'OptionGroup')
+
```

### Comparing `optenum-1.1.8/optenum.egg-info/PKG-INFO` & `optenum-1.1.9/optenum.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,354 +1,351 @@
-Metadata-Version: 2.1
-Name: optenum
-Version: 1.1.8
-Summary: A missing Python Option/Enum library
-Home-page: http://en.samuelchen.net/project/optenum/
-Author: Samuel Chen
-Author-email: samuel.net@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/samuelchen/optenum/issues
-Project-URL: Source, https://github.com/samuelchen/optenum
-Keywords: enum library development
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
-# Optenum
-
-[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
-[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
-
-
-	
-A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
-
-Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
-
-Compatible with `Python 2.7+` and `Python 3.0+`.
-
-# Install
-
-Python 3.x, 2.7
-
-```bash
-pip install optenum
-```
-
-For those probably missing `six` module:
-
-```bash
-pip install six optenum
-```
-
-# Quick start
-
-1. Simple as Enum type
-
-    Says we define a simple enum:
-    
-    ```python
-    from optenum import Options
- 
-    class Fruit(Options):
-        APPLE = 1
-        ORANGE = 2
-        BANANA = 3 
-    ```
-    
-    Try the following in Python command line:
-    
-    ```
-    >>> from optenum import Option, Options
-    >>> class Fruit(Options):
-    ...     APPLE = 1
-    ...     ORANGE = 2
-    ...     BANANA = 3
-    >>> 
-    >>> Fruit.APPLE
-    <Option code=1 name=APPLE text=None>
-    >>> print(Fruit.APPLE)
-    1
-    >>> Fruit.APPLE.code
-    1
-    >>> Fruit.APPLE.name
-    'APPLE'
-    >>> Fruit.APPLE.text
-    >>> print(Fruit.APPLE.text)
-    None
-    >>> Fruit.APPLE.get_text()
-    'apple'
-    
-    ```
-
-2. Complex declaration
-
-    You may declare your Options (Enums) in many annotations.
-
-    ```python
-    from optenum import Option, Options
- 
-    class EnumCellPhone(Options):
-        APPLE = 1
-        SAMSUNG = Option(2, name='SAMSUNG')
-        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
-    
-    
-    class DoorState(Options):
-        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
-        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
-        IN_OPENING = 'IO'
-        IN_CLOSING = 'IC'
-    
-        _FLAG = False           # underscore leading name is not an option
-        x = lambda y: y         # function/callable is not an option
-    ```
-
-3. Operators
-
-    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
-    
-    ```
-    >>> class Favorite(Options):
-    ...     APPLE = 1
-    ...     BANANA = 3, 'Banana hot'
-    ... 
-    >>> 
-    >>> Fruit.APPLE == Favorite.APPLE
-    True
-    >>> Fruit.BANANA == Favorite.BANANA
-    False
-    >>> Fruit.APPLE + 1 == Fruit.ORANGE
-    True>>> Fruit.BANANA >> 2
-    0
-    >>> Fruit.BANANA << 2
-    12>>> Fruit.BANANA > Favorite.APPLE
-    True
-    ```
-
-4. Collections
-
-    `Options` provides some collections for accessing option and it's fields.
-    See section "Collections for Options" below for more information.
-    
-    ```
-    >>> Fruit.codes
-    [1, 2, 3]
-    >>> Fruit.names
-    ['ORANGE', 'APPLE', 'BANANA']
-    >>> Fruit.all
-    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
-    >>> Fruit.tuples
-    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
-    >>> Favorite.items
-    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
-    >>> Favorite.get_list('code','text')
-    [(1, None), (3, 'Banana hot')]
-    >>> Favorite.get_dict('name','text')
-    {'APPLE': None, 'BANANA': 'Banana hot'}
-    
-    ```
-
-5. Django model choices
-
-        To be written
-
-# Background
-
-Often we need to define some enums or options. But looks python missing this class.
-Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
-
-For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
-
-```python
-class MyOption(object):
-    foo = 1
-    bar = 2
-```
-But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
-
-Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
-
-# Features
-
-  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
-  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
-  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
-  * List - Retrieve list of code, name or text `[0, 1, -1]`
-  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
-  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
-  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
-  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
-  * Access **name**, **text** by **code**
-  * Lookup enum/option by **name**, **code**
-  
-# Guide / Tutor
-
-# Type converting for `Option`
-
-    since v1.1.1
-
-An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
-`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
-
-For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
-The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
-an `Option(str)` class will be constructed internally.
-
-The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
-`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
- `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
- your option as its value(`code`) is such in `dict` as key and so on.
- 
-
-    Deprecated since v1.1.0
-    
-    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
-    
-    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
-    
-    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
-
-# Boolean for `Option`
-
-    Deprecated since v1.1.0
-    No special implementation. It behaves as `object` is.
-
-# Group and tags 
-
-See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
-
-# Operators for `Option`
-
-Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
-
-    Deprecated since v1.1.0
-    
-    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
-    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
-    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
-    directly reference to its real value.
-    
-    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
-
-# Collections for `Options`
-
-Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
-equals to `Option.FOO`.
-
-We could also access the following collections from within an Options class. 
-
-  * `Options.codes` - list of codes
-    
-  * `Options.names` - list of names
-  
-  * `Options.all` - list of options
-
-  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
-
-  * `Options.items` - dict of {`name`: `Option`} mapping
-
-  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
-  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
-  
-  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
-  `key_field` specify which Option field is key such as `name`, `code`. 
-  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
-  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
-
-    Deprecated since v1.1.0
-    
-    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
-    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
-    If you want to check if name in `Options`), use collection instead. 
-    e.g. `if 'APPLE' in Fruit.names`.
-
-
-# Configuration
-
-Some flags can be used to make some simple configuration to your Options.
-
-  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
-  
-    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
-    functions. The following example is valid definition.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        _flag = False
-        
-        def switch(self):
-            pass
-    ```
-    
-    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
-    
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Invalid Option name. Exception raised.
-    ```
-    
-    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
-    But to be noticed, it still not an `Option`.
-  
-    ```python
-    from optenum import Options
-
-    class MyEnum(Options):
-        __IGNORE_INVALID_NAME__ = True
-        
-        FOO = 1
-        BAR = 2
-        
-        Baz = 3     # <- Exception ignored. But still not an Option.
-    ```
-  
-  * `__ORDER_BY__`
-  
-        Not supported yet
-
-# FAQ
-
-* Why not use *namedtuple* ?
-
-*namedtuple* is also a good way to define enum/options. But it has not enough features
-you may required such as *collection*, *operator*, *compare*, *text* and so on.
-
-* Why only uppercase allowed for Option name ?
-
-Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
-And enumerations commonly are defined with uppercase identifier.
-
-# Contributors
-
-List of contributors:
-
-* Samuel Chen - The project owner and maintainer.
-
+Metadata-Version: 2.1
+Name: optenum
+Version: 1.1.9
+Summary: A missing Python Option/Enum library
+Home-page: http://en.samuelchen.net/project/optenum/
+Author: Samuel Chen
+Author-email: samuel.net@gmail.com
+Project-URL: Bug Reports, https://github.com/samuelchen/optenum/issues
+Project-URL: Source, https://github.com/samuelchen/optenum
+Keywords: enum library development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+# Optenum
+
+[![Travis](https://img.shields.io/github/languages/top/samuelchen/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/travis/samuelchen/optenum.svg?branch=master?style=flat-square)](https://travis-ci.org/samuelchen/optenum)
+[![Travis](https://img.shields.io/pypi/pyversions/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/v/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/status/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+[![Travis](https://img.shields.io/pypi/format/optenum.svg?style=flat-square)](https://pypi.org/project/optenum/)
+
+
+	
+A missing Python Option/Enum library which supports enum code, name, text, even (code, name) tuple list and so on.
+
+Name "**optenum**" comes from '**opt**ion' + '**enum**eration'.
+
+Compatible with `Python 2.7+` and `Python 3.0+`.
+
+# Install
+
+Python 3.x, 2.7
+
+```bash
+pip install optenum
+```
+
+For those probably missing `six` module:
+
+```bash
+pip install six optenum
+```
+
+# Quick start
+
+1. Simple as Enum type
+
+    Says we define a simple enum:
+    
+    ```python
+    from optenum import Options
+ 
+    class Fruit(Options):
+        APPLE = 1
+        ORANGE = 2
+        BANANA = 3 
+    ```
+    
+    Try the following in Python command line:
+    
+    ```
+    >>> from optenum import Option, Options
+    >>> class Fruit(Options):
+    ...     APPLE = 1
+    ...     ORANGE = 2
+    ...     BANANA = 3
+    >>> 
+    >>> Fruit.APPLE
+    <Option code=1 name=APPLE text=None>
+    >>> print(Fruit.APPLE)
+    1
+    >>> Fruit.APPLE.code
+    1
+    >>> Fruit.APPLE.name
+    'APPLE'
+    >>> Fruit.APPLE.text
+    >>> print(Fruit.APPLE.text)
+    None
+    >>> Fruit.APPLE.get_text()
+    'apple'
+    
+    ```
+
+2. Complex declaration
+
+    You may declare your Options (Enums) in many annotations.
+
+    ```python
+    from optenum import Option, Options
+ 
+    class EnumCellPhone(Options):
+        APPLE = 1
+        SAMSUNG = Option(2, name='SAMSUNG')
+        HUAWEI = 3, 'Huawei cellphone'     # tuple annotation. name = code, text
+    
+    
+    class DoorState(Options):
+        OPEN = 'O', 'Door is opened'       # tuple annotation. name = code, text
+        CLOSED = ('C', 'Door is closed')   # tuple annotation, too.
+        IN_OPENING = 'IO'
+        IN_CLOSING = 'IC'
+    
+        _FLAG = False           # underscore leading name is not an option
+        x = lambda y: y         # function/callable is not an option
+    ```
+
+3. Operators
+
+    `Option` support some operators. See more in [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md).
+    
+    ```
+    >>> class Favorite(Options):
+    ...     APPLE = 1
+    ...     BANANA = 3, 'Banana hot'
+    ... 
+    >>> 
+    >>> Fruit.APPLE == Favorite.APPLE
+    True
+    >>> Fruit.BANANA == Favorite.BANANA
+    False
+    >>> Fruit.APPLE + 1 == Fruit.ORANGE
+    True>>> Fruit.BANANA >> 2
+    0
+    >>> Fruit.BANANA << 2
+    12>>> Fruit.BANANA > Favorite.APPLE
+    True
+    ```
+
+4. Collections
+
+    `Options` provides some collections for accessing option and it's fields.
+    See section "Collections for Options" below for more information.
+    
+    ```
+    >>> Fruit.codes
+    [1, 2, 3]
+    >>> Fruit.names
+    ['ORANGE', 'APPLE', 'BANANA']
+    >>> Fruit.all
+    [<Option code=2 name=ORANGE text=None>, <Option code=1 name=APPLE text=None>, <Option code=3 name=BANANA text=None>]
+    >>> Fruit.tuples
+    [('ORANGE', 2, None), ('APPLE', 1, None), ('BANANA', 3, None)]
+    >>> Favorite.items
+    {'APPLE': <Option code=1 name=APPLE text=None>, 'BANANA': <Option code=3 name=BANANA text=Banana hot>}
+    >>> Favorite.get_list('code','text')
+    [(1, None), (3, 'Banana hot')]
+    >>> Favorite.get_dict('name','text')
+    {'APPLE': None, 'BANANA': 'Banana hot'}
+    
+    ```
+
+5. Django model choices
+
+        To be written
+
+# Background
+
+Often we need to define some enums or options. But looks python missing this class.
+Sometimes we uses class, tuples or dict as the replacement. But they are not convenience.
+
+For example, we could define a class as enumeration. We can use `MyOption.foo` to get the enum value `1`.
+
+```python
+class MyOption(object):
+    foo = 1
+    bar = 2
+```
+But how can we get the enum name foo ? How can we get the list of all enums ? Even list of tuples `[ (1, 'foo'), (2, 'bar')]` (useful in Django model)
+
+Although Python 3.7 comes with [data classes](https://docs.python.org/3/whatsnew/3.7.html#whatsnew37-pep557). So far it looks like a piece of syntax sugar for me and it can not solve these problems.
+
+# Features
+
+  * Code - Enumeration/options by different types - e.g. 0, 1, -1 (or 'new', 'running', 'stopped')
+  * Name - Name of an enum/option - e.g.  'NEW', 'RUNNING', 'STOPPED'. Support dot access. 
+  * Text - Meaning or description of the enum/option. support i18n - e.g. _('new'), _('running'), _('stopped') (translated to '新建', '运行中', ‘停止中’)
+  * List - Retrieve list of code, name or text `[0, 1, -1]`
+  * Dict - Retrieve dict of `{code: name}` mapping. even `{code: text}`, `{name: text}` mapping if required.
+  * List of tuples - Retrieve list of `[(code, name), ...]` tuples. Useful in **Django** model.
+  * Operators support - e.g. `Fruit.APPLE == 1`, `Fruit.BANANA > Fruit.APPLE`
+  * Grouping - Group a set of enums/options. e.g. IN_PROGRESS_STATE = ['STARTING', 'STOPPING'], but 'STARTED' and 'STOPPED' are not belongs to it.
+  * Access **name**, **text** by **code**
+  * Lookup enum/option by **name**, **code**
+  
+# Guide / Tutor
+
+# Type converting for `Option`
+
+    since v1.1.1
+
+An `Option` instance will be constructed dynamically. Optenum will construct a new sub type 
+`Option(?)` class based on your option value(`code`) to initialize the new instance object.  
+
+For example, `Option(code=1, name='APPLE', text='an apple')` will construct a class `Option(int)`.
+The `int` is your `code`'s type. If your option is for a string, e.g. `Option('A', 'ADMIN', 'Administration user')`,
+an `Option(str)` class will be constructed internally.
+
+The internal `Option(?)` class is derived from either `Option` and `?` (e.g. `int`). That means you can use 
+`isinstance` to check your object. For example, says we have `apple = Option(1, 'APPLE', 'an apple')`. Then
+ `isinstance(apple, int)` is `True`. And `isinstance(apple, Option)` is `True`, too. So that you can use
+ your option as its value(`code`) is such in `dict` as key and so on.
+ 
+
+    Deprecated since v1.1.0
+    
+    `str()` or implicit string converting will convert `Option.code` to string type and returns. ~
+    
+    `repr()` will returns the object as string format of `<Option code=??? name=??? text=???>`.
+    
+    `int`, `float` will be performed on `Option.code` and returns the value or raises corresponding exception.
+
+# Boolean for `Option`
+
+    Deprecated since v1.1.0
+    No special implementation. It behaves as `object` is.
+
+# Group and tags 
+
+See [this doc](https://github.com/samuelchen/optenum/blob/master/docs/tag-and-group.md).
+
+# Operators for `Option`
+
+Since v1.1.1, an `Option` behaves as its value(`code`) is. So it will support all operators its `code` supports.
+
+    Deprecated since v1.1.0
+    
+    `Option.code` is the real value of the enum/option item. Somehow we need to use codes 
+    like `if active_state == MyOption.RUNNING.code:  # Do something ...` to check the status. For convenience using it, some of the operators
+    are override. Then we could use `if active_state == MyOption.RUNNING:`, `x = MyOption.RUNNING + 1` and so on to
+    directly reference to its real value.
+    
+    See doc [operators.md](https://github.com/samuelchen/optenum/blob/master/docs/operators.md) for override operators.
+
+# Collections for `Options`
+
+Option can be accessed directly as subscribe annotation. For example `Option['FOO']`
+equals to `Option.FOO`.
+
+We could also access the following collections from within an Options class. 
+
+  * `Options.codes` - list of codes
+    
+  * `Options.names` - list of names
+  
+  * `Options.all` - list of options
+
+  * `Options.tuples` - list of (`name`, `code`, `text`) tuple
+
+  * `Options.items` - dict of {`name`: `Option`} mapping
+
+  * `Options.get_list(*fields)` - list of *files tuple. *fields are names of Option filed 
+  such as `code`, *(`name`, `code`) or *(`code`, `name`, `text`)
+  
+  * `Options.get_dict(key_field, *fields)` - dict of `{key_filed: (*fields)}` (`{str: tuple}`) mapping.
+  `key_field` specify which Option field is key such as `name`, `code`. 
+  `fields` specify the value tuple combined of which Option fields such as (`name`, `text`) or `name`.
+  if fields is tuple, the value is tuple. if fields is single filed, value is single field.
+
+    Deprecated since v1.1.0
+    
+    `in` operator could check if a `code` in `Options`. e.g. `if Fruit.APPLE in Fruit`.
+    The `Option.name` will not work. e.g. `if 'APPLE' in Fruit` will got `False`. 
+    If you want to check if name in `Options`), use collection instead. 
+    e.g. `if 'APPLE' in Fruit.names`.
+
+
+# Configuration
+
+Some flags can be used to make some simple configuration to your Options.
+
+  * `__IGNORE_INVALID_NAME__` - Ignore invalid `Option` name so that you may add your own attribute/function to class.
+  
+    Underscore `_` leading attributes and any functions will be ignored so that you can add your own attributes and 
+    functions. The following example is valid definition.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        _flag = False
+        
+        def switch(self):
+            pass
+    ```
+    
+    But if an attributes is not uppercase (all characters), it will be treat as invalid `Option` and cause exception.
+    
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Invalid Option name. Exception raised.
+    ```
+    
+    If you want this available, add `__IGNORE_INVALID_NAME__` to your class like below. The exception will ignored.
+    But to be noticed, it still not an `Option`.
+  
+    ```python
+    from optenum import Options
+
+    class MyEnum(Options):
+        __IGNORE_INVALID_NAME__ = True
+        
+        FOO = 1
+        BAR = 2
+        
+        Baz = 3     # <- Exception ignored. But still not an Option.
+    ```
+  
+  * `__ORDER_BY__`
+  
+        Not supported yet
+
+# FAQ
+
+* Why not use *namedtuple* ?
+
+*namedtuple* is also a good way to define enum/options. But it has not enough features
+you may required such as *collection*, *operator*, *compare*, *text* and so on.
+
+* Why only uppercase allowed for Option name ?
+
+Because you can define other none-option attributes if sets `__IGNORE_INVALID_NAME__` to `True`.
+And enumerations commonly are defined with uppercase identifier.
+
+# Contributors
+
+List of contributors:
+
+* Samuel Chen - The project owner and maintainer.
```

### Comparing `optenum-1.1.8/setup.py` & `optenum-1.1.9/setup.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-"""A setuptools based setup module.
-From:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-
-common:
-  - clean: rm ./dist/*; rm -rf ./build/*
-  - build: python3 setup.py sdist bdist_wheel
-  - twine: python3 -m pip install --user --upgrade twine
-
-Test PyPi:
-  - upload: python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-  - install: pip install --index-url https://test.pypi.org/simple/ optenum
-
-
-PyPi Release:
-  - upload: python3 -m twine upload dist/*
-  - install: pip install optenum
-"""
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-from os import path
-# io.open is needed for projects that support Python 2.7
-# It ensures open() defaults to text mode with universal newlines,
-# and accepts an argument to specify the text encoding
-# Python 3 only projects can skip this import
-from io import open
-from optenum import __version__
-
-here = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-# Arguments marked as "Required" below must be included for upload to PyPI.
-# Fields marked as "Optional" may be commented out.
-
-setup(
-    # This is the name of your project. The first time you publish this
-    # package, this name will be registered for you. It will determine how
-    # users can install this project, e.g.:
-    #
-    # $ pip install optenum
-    #
-    # And where it will live on PyPI: https://pypi.org/project/optenum/
-    #
-    # There are some restrictions on what makes a valid project name
-    # specification here:
-    # https://packaging.python.org/specifications/core-metadata/#name
-    name='optenum',  # Required
-
-    # Versions should comply with PEP 440:
-    # https://www.python.org/dev/peps/pep-0440/
-    #
-    # For a discussion on single-sourcing the version across setup.py and the
-    # project code, see
-    # https://packaging.python.org/en/latest/single_source_version.html
-    version=__version__,  # Required
-
-    # This is a one-line description or tagline of what your project does. This
-    # corresponds to the "Summary" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#summary
-    description='A missing Python Option/Enum library',  # Optional
-
-    # This is an optional longer description of your project that represents
-    # the body of text which users will see when they visit PyPI.
-    #
-    # Often, this is the same as your README, so you can just read it in from
-    # that file directly (as we have already done above)
-    #
-    # This field corresponds to the "Description" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-optional
-    long_description=long_description,  # Optional
-
-    # Denotes that our long_description is in Markdown; valid values are
-    # text/plain, text/x-rst, and text/markdown
-    #
-    # Optional if long_description is written in reStructuredText (rst) but
-    # required for plain-text or Markdown; if unspecified, "applications should
-    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
-    # fall back to text/plain if it is not valid rst" (see link below)
-    #
-    # This field corresponds to the "Description-Content-Type" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
-    long_description_content_type='text/markdown',  # Optional (see note above)
-
-    # This should be a valid link to your project's main homepage.
-    #
-    # This field corresponds to the "Home-Page" metadata field:
-    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url='http://en.samuelchen.net/project/optenum/',  # Optional
-
-    # This should be your name or the name of the organization which owns the
-    # project.
-    author='Samuel Chen',  # Optional
-
-    # This should be a valid email address corresponding to the author listed
-    # above.
-    author_email='samuel.net@gmail.com',  # Optional
-
-    # Classifiers help users find your project by categorizing it.
-    #
-    # For a list of valid classifiers, see https://pypi.org/classifiers/
-    classifiers=[  # Optional
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        'Development Status :: 5 - Production/Stable',
-
-        # Indicate who your project is intended for
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-
-        # Pick your license as you wish
-        'License :: OSI Approved :: MIT License',
-
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        # These classifiers are *not* checked by 'pip install'. See instead
-        # 'python_requires' below.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-    ],
-
-    # This field adds keywords for your project which will appear on the
-    # project page. What does your project relate to?
-    #
-    # Note that this is a string of words separated by whitespace, not a list.
-    keywords='enum library development',  # Optional
-
-    # You can just specify package directories manually here if your project is
-    # simple. Or you can use find_packages().
-    #
-    # Alternatively, if you just want to distribute a single Python file, use
-    # the `py_modules` argument instead as follows, which will expect a file
-    # called `my_module.py` to exist:
-    #
-    #   py_modules=["my_module"],
-    #
-    packages=find_packages(exclude=['contrib', 'docs', 'tests', 'samples']),  # Required
-
-    # Specify which Python versions you support. In contrast to the
-    # 'Programming Language' classifiers above, 'pip install' will check this
-    # and refuse to install the project if the version does not match. If you
-    # do not support Python 2, you can simplify this to '>=3.5' or similar, see
-    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
-
-    # This field lists other packages that your project depends on to run.
-    # Any package you put here will be installed by pip when your project is
-    # installed, so they must be valid existing projects.
-    #
-    # For an analysis of "install_requires" vs pip's requirements files see:
-    # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['six'],  # Optional
-
-    # List additional groups of dependencies here (e.g. development
-    # dependencies). Users will be able to install these using the "extras"
-    # syntax, for example:
-    #
-    #   $ pip install optenum[dev]
-    #
-    # Similar to `install_requires` above, these must be valid existing
-    # projects.
-    extras_require={  # Optional
-        'dev': ['check-manifest'],
-        'test': ['coverage'],
-    },
-
-    # If there are data files included in your packages that need to be
-    # installed, specify them here.
-    #
-    # If using Python 2.6 or earlier, then these have to be included in
-    # MANIFEST.in as well.
-    package_data={  # Optional
-        # 'sample': ['package_data.dat'],
-    },
-
-    # Although 'package_data' is the preferred approach, in some case you may
-    # need to place data files outside of your packages. See:
-    # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
-    #
-    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    # data_files=[('my_data', ['data/data_file'])],  # Optional
-
-    # To provide executable scripts, use entry points in preference to the
-    # "scripts" keyword. Entry points provide cross-platform support and allow
-    # `pip` to create the appropriate form of executable for the target
-    # platform.
-    #
-    # For example, the following would provide a command called `sample` which
-    # executes the function `main` from this package when invoked:
-    entry_points={  # Optional
-        'console_scripts': [
-            # 'sample=sample:main',
-        ],
-    },
-
-    # List additional URLs that are relevant to your project as a dict.
-    #
-    # This field corresponds to the "Project-URL" metadata fields:
-    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-    #
-    # Examples listed include a pattern for specifying where the package tracks
-    # issues, where the source is hosted, where to say thanks to the package
-    # maintainers, and where to support the project financially. The key is
-    # what's used to render the link text on PyPI.
-    project_urls={  # Optional
-        'Bug Reports': 'https://github.com/samuelchen/optenum/issues',
-        # 'Funding': '',
-        # 'Say Thanks!': '',
-        'Source': 'https://github.com/samuelchen/optenum',
-    },
+"""A setuptools based setup module.
+From:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+
+common:
+  - clean: rm ./dist/*; rm -rf ./build/*
+  - build: python3 setup.py sdist bdist_wheel
+  - twine: python3 -m pip install --user --upgrade twine
+
+Test PyPi:
+  - upload: python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+  - install: pip install --index-url https://test.pypi.org/simple/ optenum
+
+
+PyPi Release:
+  - upload: python3 -m twine upload dist/*
+  - install: pip install optenum
+"""
+
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+from os import path
+# io.open is needed for projects that support Python 2.7
+# It ensures open() defaults to text mode with universal newlines,
+# and accepts an argument to specify the text encoding
+# Python 3 only projects can skip this import
+from io import open
+from optenum import __version__
+
+here = path.abspath(path.dirname(__file__))
+
+# Get the long description from the README file
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+# Arguments marked as "Required" below must be included for upload to PyPI.
+# Fields marked as "Optional" may be commented out.
+
+setup(
+    # This is the name of your project. The first time you publish this
+    # package, this name will be registered for you. It will determine how
+    # users can install this project, e.g.:
+    #
+    # $ pip install optenum
+    #
+    # And where it will live on PyPI: https://pypi.org/project/optenum/
+    #
+    # There are some restrictions on what makes a valid project name
+    # specification here:
+    # https://packaging.python.org/specifications/core-metadata/#name
+    name='optenum',  # Required
+
+    # Versions should comply with PEP 440:
+    # https://www.python.org/dev/peps/pep-0440/
+    #
+    # For a discussion on single-sourcing the version across setup.py and the
+    # project code, see
+    # https://packaging.python.org/en/latest/single_source_version.html
+    version=__version__,  # Required
+
+    # This is a one-line description or tagline of what your project does. This
+    # corresponds to the "Summary" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#summary
+    description='A missing Python Option/Enum library',  # Optional
+
+    # This is an optional longer description of your project that represents
+    # the body of text which users will see when they visit PyPI.
+    #
+    # Often, this is the same as your README, so you can just read it in from
+    # that file directly (as we have already done above)
+    #
+    # This field corresponds to the "Description" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-optional
+    long_description=long_description,  # Optional
+
+    # Denotes that our long_description is in Markdown; valid values are
+    # text/plain, text/x-rst, and text/markdown
+    #
+    # Optional if long_description is written in reStructuredText (rst) but
+    # required for plain-text or Markdown; if unspecified, "applications should
+    # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
+    # fall back to text/plain if it is not valid rst" (see link below)
+    #
+    # This field corresponds to the "Description-Content-Type" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
+    long_description_content_type='text/markdown',  # Optional (see note above)
+
+    # This should be a valid link to your project's main homepage.
+    #
+    # This field corresponds to the "Home-Page" metadata field:
+    # https://packaging.python.org/specifications/core-metadata/#home-page-optional
+    url='http://en.samuelchen.net/project/optenum/',  # Optional
+
+    # This should be your name or the name of the organization which owns the
+    # project.
+    author='Samuel Chen',  # Optional
+
+    # This should be a valid email address corresponding to the author listed
+    # above.
+    author_email='samuel.net@gmail.com',  # Optional
+
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see https://pypi.org/classifiers/
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 5 - Production/Stable',
+
+        # Indicate who your project is intended for
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+
+        # Pick your license as you wish
+        'License :: OSI Approved :: MIT License',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        # These classifiers are *not* checked by 'pip install'. See instead
+        # 'python_requires' below.
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+    ],
+
+    # This field adds keywords for your project which will appear on the
+    # project page. What does your project relate to?
+    #
+    # Note that this is a string of words separated by whitespace, not a list.
+    keywords='enum library development',  # Optional
+
+    # You can just specify package directories manually here if your project is
+    # simple. Or you can use find_packages().
+    #
+    # Alternatively, if you just want to distribute a single Python file, use
+    # the `py_modules` argument instead as follows, which will expect a file
+    # called `my_module.py` to exist:
+    #
+    #   py_modules=["my_module"],
+    #
+    packages=find_packages(exclude=['contrib', 'docs', 'tests', 'samples']),  # Required
+
+    # Specify which Python versions you support. In contrast to the
+    # 'Programming Language' classifiers above, 'pip install' will check this
+    # and refuse to install the project if the version does not match. If you
+    # do not support Python 2, you can simplify this to '>=3.5' or similar, see
+    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
+
+    # This field lists other packages that your project depends on to run.
+    # Any package you put here will be installed by pip when your project is
+    # installed, so they must be valid existing projects.
+    #
+    # For an analysis of "install_requires" vs pip's requirements files see:
+    # https://packaging.python.org/en/latest/requirements.html
+    install_requires=['six'],  # Optional
+
+    # List additional groups of dependencies here (e.g. development
+    # dependencies). Users will be able to install these using the "extras"
+    # syntax, for example:
+    #
+    #   $ pip install optenum[dev]
+    #
+    # Similar to `install_requires` above, these must be valid existing
+    # projects.
+    extras_require={  # Optional
+        'dev': ['check-manifest'],
+        'test': ['coverage'],
+    },
+
+    # If there are data files included in your packages that need to be
+    # installed, specify them here.
+    #
+    # If using Python 2.6 or earlier, then these have to be included in
+    # MANIFEST.in as well.
+    package_data={  # Optional
+        # 'sample': ['package_data.dat'],
+    },
+
+    # Although 'package_data' is the preferred approach, in some case you may
+    # need to place data files outside of your packages. See:
+    # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
+    #
+    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
+    # data_files=[('my_data', ['data/data_file'])],  # Optional
+
+    # To provide executable scripts, use entry points in preference to the
+    # "scripts" keyword. Entry points provide cross-platform support and allow
+    # `pip` to create the appropriate form of executable for the target
+    # platform.
+    #
+    # For example, the following would provide a command called `sample` which
+    # executes the function `main` from this package when invoked:
+    entry_points={  # Optional
+        'console_scripts': [
+            # 'sample=sample:main',
+        ],
+    },
+
+    # List additional URLs that are relevant to your project as a dict.
+    #
+    # This field corresponds to the "Project-URL" metadata fields:
+    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+    #
+    # Examples listed include a pattern for specifying where the package tracks
+    # issues, where the source is hosted, where to say thanks to the package
+    # maintainers, and where to support the project financially. The key is
+    # what's used to render the link text on PyPI.
+    project_urls={  # Optional
+        'Bug Reports': 'https://github.com/samuelchen/optenum/issues',
+        # 'Funding': '',
+        # 'Say Thanks!': '',
+        'Source': 'https://github.com/samuelchen/optenum',
+    },
 )
```

