# Comparing `tmp/pyobjconfig-0.1.2.tar.gz` & `tmp/pyobjconfig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyobjconfig-0.1.2.tar", last modified: Thu Jan 14 22:46:03 2021, max compression
+gzip compressed data, was "pyobjconfig-0.1.3.tar", last modified: Tue Apr 18 21:10:20 2023, max compression
```

## Comparing `pyobjconfig-0.1.2.tar` & `pyobjconfig-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 wwoods    (1000) wwoods    (1000)        0 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)     3676 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/PKG-INFO
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)     2719 2021-01-14 22:42:39.000000 pyobjconfig-0.1.2/README.md
-drwxrwxr-x   0 wwoods    (1000) wwoods    (1000)        0 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig/
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)      113 2020-10-14 17:47:34.000000 pyobjconfig-0.1.2/pyobjconfig/__init__.py
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)    12036 2021-01-14 22:41:25.000000 pyobjconfig-0.1.2/pyobjconfig/common.py
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)      844 2020-10-14 17:47:34.000000 pyobjconfig-0.1.2/pyobjconfig/torch.py
-drwxrwxr-x   0 wwoods    (1000) wwoods    (1000)        0 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)     3676 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/PKG-INFO
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)      284 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)        1 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)        9 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/requires.txt
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)       12 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/pyobjconfig.egg-info/top_level.txt
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)       38 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/setup.cfg
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)      544 2021-01-14 22:42:46.000000 pyobjconfig-0.1.2/setup.py
-drwxrwxr-x   0 wwoods    (1000) wwoods    (1000)        0 2021-01-14 22:46:03.000000 pyobjconfig-0.1.2/test/
--rw-rw-r--   0 wwoods    (1000) wwoods    (1000)     2668 2021-01-14 22:45:35.000000 pyobjconfig-0.1.2/test/test_pyobjconfig.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     1067 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/LICENSE
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3162 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/PKG-INFO
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     2871 2023-04-18 21:03:52.000000 pyobjconfig-0.1.3/README.md
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.251229 pyobjconfig-0.1.3/pyobjconfig/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      113 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/pyobjconfig/__init__.py
+-rw-r--r--   0 waltw     (1000) waltw     (1000)    12438 2023-04-18 21:01:54.000000 pyobjconfig-0.1.3/pyobjconfig/common.py
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      844 2023-04-18 20:42:16.000000 pyobjconfig-0.1.3/pyobjconfig/torch.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/pyobjconfig.egg-info/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3162 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/PKG-INFO
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      292 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)        1 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)        9 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/requires.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)       12 2023-04-18 21:10:20.000000 pyobjconfig-0.1.3/pyobjconfig.egg-info/top_level.txt
+-rw-r--r--   0 waltw     (1000) waltw     (1000)       38 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/setup.cfg
+-rw-r--r--   0 waltw     (1000) waltw     (1000)      544 2023-04-18 21:03:57.000000 pyobjconfig-0.1.3/setup.py
+drwxr-xr-x   0 waltw     (1000) waltw     (1000)        0 2023-04-18 21:10:20.254562 pyobjconfig-0.1.3/test/
+-rw-r--r--   0 waltw     (1000) waltw     (1000)     3418 2023-04-18 21:02:48.000000 pyobjconfig-0.1.3/test/test_pyobjconfig.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyobjconfig-0.1.2/PKG-INFO` & `pyobjconfig-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: pyobjconfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: An argparse+pydantic-based configuration system for Python.
 Home-page: https://github.com/wwoods/pyobjconfig
 Author: Walt Woods
 Author-email: woodswalben@gmail.com
-License: UNKNOWN
-Description: # pyobjconfig
-        
-        `pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
-        
-        ## Example usage
-        
-        Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
-        
-        ```python
-        
-        import argparse
-        import pyobjconfig as poc
-        
-        # Any class which plugs into pyobjconfig should derive from `ConfigurableObject`
-        class Child(poc.ConfigurableObject):
-            # To register configuration options for this class, add a `config` member
-            # which derives from a pydantic model.
-            class config(poc.PydanticBaseModel):
-                # Pydantic handles basic type validation and allows default values to be
-                # set
-                inner: str = 'hello'
-        
-        class Base(poc.ConfigurableObject):
-            class config(poc.PydanticBaseModel):
-                hello: str = 'hi'
-        
-            # Assigning a class deriving from `ConfigurableObject` as a member of a
-            # class definition results in a nested object, which will be instantiated
-            # using parameters from the command line.
-            child = Child
-        
-        ap = argparse.ArgumentParser()
-        Base.argparse_setup(ap)
-        
-        args = ap.parse_args(['--child-inner', 'beep']).__dict__
-        obj = Base.argparse_create(args)
-        print(obj.config.hello)  # Prints 'hi'
-        print(obj.child.config.inner)  # Prints 'beep'
-        
-        ap.print_help()
-        # usage: ipython [-h] [--hello HELLO] [--child-inner CHILD-INNER]
-        #
-        # optional arguments:
-        #   -h, --help            show this help message and exit
-        #   --hello HELLO         Default: hi
-        #   --child-inner CHILD-INNER
-        #                         Default: hello
-        
-        ```
-        
-        Switches are also supported, such that the class (or value) of a child member may be changed at initialization time. Additionally, the `--help` for the `argparse` parser will change to reflect the choice of child:
-        
-        ```python
-        import pyobjconfig as poc
-        class A(poc.ConfigurableObject):
-            pass
-        class B(poc.ConfigurableObject):
-            pass
-        class Base(poc.ConfigurableObject):
-            child = poc.ConfigurableSwitch({
-                'a': A,
-                'b': B,
-                'none': None,
-            }, default='none')
-        ```
-        
-        Experimentally, environment variables are supported. Not yet well tested, but calling `argparse_create(args, env='PREFIX')` will allow e.g. `PREFIX_CHILD=a` to be specified in the environment. Arguments on the command line take precedence.
-        
-        ```python
-        import argparse
-        import pyobjconfig as poc
-        ```
-        
-        ## Usage with pytorch
-        
-        Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
-        
-        
-        # Changelog
-        * 2021-01-14 - v0.1.2. Support lists on the command line.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyobjconfig
+
+`pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
+
+## Example usage
+
+Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
+
+```python
+
+import argparse
+import pyobjconfig as poc
+
+# Any class which plugs into pyobjconfig should derive from `ConfigurableObject`
+class Child(poc.ConfigurableObject):
+    # To register configuration options for this class, add a `config` member
+    # which derives from a pydantic model.
+    class config(poc.PydanticBaseModel):
+        # Pydantic handles basic type validation and allows default values to be
+        # set
+        inner: str = 'hello'
+
+class Base(poc.ConfigurableObject):
+    class config(poc.PydanticBaseModel):
+        hello: str = 'hi'
+
+    # Assigning a class deriving from `ConfigurableObject` as a member of a
+    # class definition results in a nested object, which will be instantiated
+    # using parameters from the command line.
+    child = Child
+
+ap = argparse.ArgumentParser()
+Base.argparse_setup(ap)
+
+args = ap.parse_args(['--child-inner', 'beep']).__dict__
+obj = Base.argparse_create(args)
+print(obj.config.hello)  # Prints 'hi'
+print(obj.child.config.inner)  # Prints 'beep'
+
+ap.print_help()
+# usage: ipython [-h] [--hello HELLO] [--child-inner CHILD-INNER]
+#
+# optional arguments:
+#   -h, --help            show this help message and exit
+#   --hello HELLO         Default: hi
+#   --child-inner CHILD-INNER
+#                         Default: hello
+
+```
+
+Switches are also supported, such that the class (or value) of a child member may be changed at initialization time. Additionally, the `--help` for the `argparse` parser will change to reflect the choice of child:
+
+```python
+import pyobjconfig as poc
+class A(poc.ConfigurableObject):
+    pass
+class B(poc.ConfigurableObject):
+    pass
+class Base(poc.ConfigurableObject):
+    child = poc.ConfigurableSwitch({
+        'a': A,
+        'b': B,
+        'none': None,
+    }, default='none')
+```
+
+Experimentally, environment variables are supported. Not yet well tested, but calling `argparse_create(args, env='PREFIX')` will allow e.g. `PREFIX_CHILD=a` to be specified in the environment. Arguments on the command line take precedence.
+
+```python
+import argparse
+import pyobjconfig as poc
+```
+
+## Usage with pytorch
+
+Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
+
+
+# Changelog
+* 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
+* 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.2/README.md` & `pyobjconfig-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,8 +73,9 @@
 
 ## Usage with pytorch
 
 Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
 
 
 # Changelog
+* 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
 * 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.2/pyobjconfig/common.py` & `pyobjconfig-0.1.3/pyobjconfig/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         r = cls._argparse_create(env, '', args)
         assert not args, args
         return r
 
 
     @classmethod
     def argparse_setup(cls, parser):
+        # Force exact matches only when specifying arguments
+        parser.allow_abbrev = False
         cls._argparse_setup('', parser)
 
 
     def argparse_hparams(self):
         settings = {}
         self._argparse_hparams(self, '', settings)
         def m(v):
@@ -219,14 +221,20 @@
             if type(v) is type and issubclass(v, ConfigurableObject):
                 post_init[k] = v._argparse_create(env_prefix, prefix + k + '-',
                         args)
         try:
             r = cls(config=config, child_configurables=post_init)
         except:
             raise TypeError(cls)
+        if r.config is not None:
+            for k, v in r.config.dict().items():
+                if v is None:
+                    raise ValueError(f'Cannot leave parameters as `None`, as '
+                            f' that would break json serialization: '
+                            f'{prefix}{k}')
         return r
 
 
 class _ConfigurableChildWithExtraHparams:
     def __init__(self, value, hparams):
         self.value = value
         self.hparams = hparams
```

### Comparing `pyobjconfig-0.1.2/pyobjconfig/torch.py` & `pyobjconfig-0.1.3/pyobjconfig/torch.py`

 * *Files identical despite different names*

### Comparing `pyobjconfig-0.1.2/pyobjconfig.egg-info/PKG-INFO` & `pyobjconfig-0.1.3/pyobjconfig.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: pyobjconfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: An argparse+pydantic-based configuration system for Python.
 Home-page: https://github.com/wwoods/pyobjconfig
 Author: Walt Woods
 Author-email: woodswalben@gmail.com
-License: UNKNOWN
-Description: # pyobjconfig
-        
-        `pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
-        
-        ## Example usage
-        
-        Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
-        
-        ```python
-        
-        import argparse
-        import pyobjconfig as poc
-        
-        # Any class which plugs into pyobjconfig should derive from `ConfigurableObject`
-        class Child(poc.ConfigurableObject):
-            # To register configuration options for this class, add a `config` member
-            # which derives from a pydantic model.
-            class config(poc.PydanticBaseModel):
-                # Pydantic handles basic type validation and allows default values to be
-                # set
-                inner: str = 'hello'
-        
-        class Base(poc.ConfigurableObject):
-            class config(poc.PydanticBaseModel):
-                hello: str = 'hi'
-        
-            # Assigning a class deriving from `ConfigurableObject` as a member of a
-            # class definition results in a nested object, which will be instantiated
-            # using parameters from the command line.
-            child = Child
-        
-        ap = argparse.ArgumentParser()
-        Base.argparse_setup(ap)
-        
-        args = ap.parse_args(['--child-inner', 'beep']).__dict__
-        obj = Base.argparse_create(args)
-        print(obj.config.hello)  # Prints 'hi'
-        print(obj.child.config.inner)  # Prints 'beep'
-        
-        ap.print_help()
-        # usage: ipython [-h] [--hello HELLO] [--child-inner CHILD-INNER]
-        #
-        # optional arguments:
-        #   -h, --help            show this help message and exit
-        #   --hello HELLO         Default: hi
-        #   --child-inner CHILD-INNER
-        #                         Default: hello
-        
-        ```
-        
-        Switches are also supported, such that the class (or value) of a child member may be changed at initialization time. Additionally, the `--help` for the `argparse` parser will change to reflect the choice of child:
-        
-        ```python
-        import pyobjconfig as poc
-        class A(poc.ConfigurableObject):
-            pass
-        class B(poc.ConfigurableObject):
-            pass
-        class Base(poc.ConfigurableObject):
-            child = poc.ConfigurableSwitch({
-                'a': A,
-                'b': B,
-                'none': None,
-            }, default='none')
-        ```
-        
-        Experimentally, environment variables are supported. Not yet well tested, but calling `argparse_create(args, env='PREFIX')` will allow e.g. `PREFIX_CHILD=a` to be specified in the environment. Arguments on the command line take precedence.
-        
-        ```python
-        import argparse
-        import pyobjconfig as poc
-        ```
-        
-        ## Usage with pytorch
-        
-        Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
-        
-        
-        # Changelog
-        * 2021-01-14 - v0.1.2. Support lists on the command line.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyobjconfig
+
+`pyobjconfig` is a module suite designed with Machine Learning (ML) experiments in mind, but should work for a broad range of hierarchical configurations.
+
+## Example usage
+
+Pyobjconfig supports configuring nested objects, such that each object has control over its own configuration:
+
+```python
+
+import argparse
+import pyobjconfig as poc
+
+# Any class which plugs into pyobjconfig should derive from `ConfigurableObject`
+class Child(poc.ConfigurableObject):
+    # To register configuration options for this class, add a `config` member
+    # which derives from a pydantic model.
+    class config(poc.PydanticBaseModel):
+        # Pydantic handles basic type validation and allows default values to be
+        # set
+        inner: str = 'hello'
+
+class Base(poc.ConfigurableObject):
+    class config(poc.PydanticBaseModel):
+        hello: str = 'hi'
+
+    # Assigning a class deriving from `ConfigurableObject` as a member of a
+    # class definition results in a nested object, which will be instantiated
+    # using parameters from the command line.
+    child = Child
+
+ap = argparse.ArgumentParser()
+Base.argparse_setup(ap)
+
+args = ap.parse_args(['--child-inner', 'beep']).__dict__
+obj = Base.argparse_create(args)
+print(obj.config.hello)  # Prints 'hi'
+print(obj.child.config.inner)  # Prints 'beep'
+
+ap.print_help()
+# usage: ipython [-h] [--hello HELLO] [--child-inner CHILD-INNER]
+#
+# optional arguments:
+#   -h, --help            show this help message and exit
+#   --hello HELLO         Default: hi
+#   --child-inner CHILD-INNER
+#                         Default: hello
+
+```
+
+Switches are also supported, such that the class (or value) of a child member may be changed at initialization time. Additionally, the `--help` for the `argparse` parser will change to reflect the choice of child:
+
+```python
+import pyobjconfig as poc
+class A(poc.ConfigurableObject):
+    pass
+class B(poc.ConfigurableObject):
+    pass
+class Base(poc.ConfigurableObject):
+    child = poc.ConfigurableSwitch({
+        'a': A,
+        'b': B,
+        'none': None,
+    }, default='none')
+```
+
+Experimentally, environment variables are supported. Not yet well tested, but calling `argparse_create(args, env='PREFIX')` will allow e.g. `PREFIX_CHILD=a` to be specified in the environment. Arguments on the command line take precedence.
+
+```python
+import argparse
+import pyobjconfig as poc
+```
+
+## Usage with pytorch
+
+Pytorch overrides `__setattr__` in a way that is incompatible with the `ConfigurableObject` class provided by `pyobjconfig`. To work around this, use the `pyobjconfig.torch.ConfigurableModule` as a drop-in replacement for `torch.nn.Module`.
+
+
+# Changelog
+* 2023-04-18 - v0.1.3. Disallow `None` as parameter values because it serializes poorly, and disallow abbreviated parameter matches to avoid confusion.
+* 2021-01-14 - v0.1.2. Support lists on the command line.
```

### Comparing `pyobjconfig-0.1.2/setup.py` & `pyobjconfig-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as f:
     long_desc = f.read()
 
 setuptools.setup(
         name='pyobjconfig',
-        version='0.1.2',
+        version='0.1.3',
         author='Walt Woods',
         author_email='woodswalben@gmail.com',
         description="An argparse+pydantic-based configuration system for Python.",
         long_description=long_desc,
         long_description_content_type='text/markdown',
         url='https://github.com/wwoods/pyobjconfig',
         packages=setuptools.find_packages(),
```

### Comparing `pyobjconfig-0.1.2/test/test_pyobjconfig.py` & `pyobjconfig-0.1.3/test/test_pyobjconfig.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,14 +38,28 @@
 
     with pytest.raises(TypeError) as exc:
         args = ap.parse_args(['--a', 'yodel']).__dict__
         print(args)
         obj = BaseObject.argparse_create(args)
 
 
+def test_default_none():
+    """Ensure that an object with a default value of None MUST be overridden.
+    """
+    class A1(ConfigurableObject):
+        class config(PydanticBaseModel):
+            setting: int = None
+
+    with pytest.raises(ValueError) as exc:
+        A1.argparse_create({})
+    assert 'Cannot leave parameters as `None`' in str(exc)
+
+    A1.argparse_create({'setting': 8})
+
+
 def test_enum():
     class A(ConfigurableObject):
         def get(self):
             return 'A'
     class B(ConfigurableObject):
         def get(self):
             return 'B'
@@ -91,7 +105,20 @@
     A.argparse_setup(ap)
 
     args = A.argparse_create(ap.parse_args([]).__dict__)
     assert args.config.thing == [1]
     args = A.argparse_create(ap.parse_args(['--thing', '2', '--thing', '3']).__dict__)
     assert args.config.thing == [2, 3]
 
+
+def test_prefix():
+    class A(ConfigurableObject):
+        class B(ConfigurableObject):
+            class config(PydanticBaseModel):
+                lr_value: float = 1
+
+    ap = argparse.ArgumentParser(description=__doc__)
+    A.argparse_setup(ap)
+
+    with pytest.raises(SystemExit):
+        A.argparse_create(ap.parse_args(['--B-lr', '8']).__dict__)
+
```

